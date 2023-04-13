# Comparing `tmp/pyranker-0.1.2-py3-none-any.whl.zip` & `tmp/pyranker-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 5970 bytes, number of entries: 13
+Zip file size: 6138 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 10:50 pyranker/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 18:01 pyranker/preprocessing/__init__.py
 -rw-r--r--  2.0 unx      507 b- defN 23-Apr-12 11:00 pyranker/preprocessing/normalizer.py
 -rw-r--r--  2.0 unx      216 b- defN 23-Apr-12 11:00 pyranker/preprocessing/tokenizer.py
--rw-r--r--  2.0 unx     1274 b- defN 23-Apr-12 11:00 pyranker/rankers/__init__.py
--rw-r--r--  2.0 unx     1611 b- defN 23-Apr-12 11:52 pyranker/rankers/bm25.py
--rw-r--r--  2.0 unx      801 b- defN 23-Apr-12 11:00 pyranker/rankers/tf_idf.py
--rw-r--r--  2.0 unx     1172 b- defN 23-Apr-12 11:00 pyranker/rankers/vspace.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1139 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/RECORD
-13 files, 8959 bytes uncompressed, 4174 bytes compressed:  53.4%
+-rw-r--r--  2.0 unx     1226 b- defN 23-Apr-12 19:28 pyranker/rankers/__init__.py
+-rw-r--r--  2.0 unx     1720 b- defN 23-Apr-13 04:30 pyranker/rankers/bm25.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Apr-12 18:11 pyranker/rankers/tf_idf.py
+-rw-r--r--  2.0 unx     1576 b- defN 23-Apr-13 04:01 pyranker/rankers/vspace.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-13 05:56 pyranker-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1139 b- defN 23-Apr-13 05:56 pyranker-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 05:56 pyranker-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-13 05:56 pyranker-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-13 05:56 pyranker-0.1.3.dist-info/RECORD
+13 files, 9434 bytes uncompressed, 4342 bytes compressed:  54.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pyranker/rankers/tf_idf.py
 Comment: 
 
 Filename: pyranker/rankers/vspace.py
 Comment: 
 
-Filename: pyranker-0.1.2.dist-info/LICENSE
+Filename: pyranker-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyranker-0.1.2.dist-info/METADATA
+Filename: pyranker-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pyranker-0.1.2.dist-info/WHEEL
+Filename: pyranker-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyranker-0.1.2.dist-info/top_level.txt
+Filename: pyranker-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyranker-0.1.2.dist-info/RECORD
+Filename: pyranker-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyranker/rankers/__init__.py

```diff
@@ -33,16 +33,16 @@
         for word, f in freq.items():
             try:
                 self.word_freq[word] += 1
             except KeyError:
                 self.word_freq[word] = 1
 
     def _tokenize_corpus(self, corpus):
-        with Pool(cpu_count()) as pool:
-            yield from pool.imap(self.tokenizer, corpus, chunksize=1000)
+        for doc in corpus:
+            yield self.tokenizer(doc)
 
     def _calc_idf(self):
         """
         Gets the idf score of all terms
         """
         corpus_size = np.log2(self.corpus_size)
         for word, freq in self.word_freq.items():
```

## pyranker/rankers/bm25.py

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 from pyranker.preprocessing.tokenizer import tokenize
 
 from . import TfIdfWeighter
 
 
 class BM25Ranker(TfIdfWeighter):
     def __init__(self, corpus, k1=1.5, b=0.75):
@@ -37,15 +38,18 @@
                 continue
             q_freq = np.array([doc.get(word, 0) for doc in self.doc_freqs])
             score += self.idf.get(word, 0) * (
                 q_freq
                 * (self.k1 + 1)
                 / (q_freq + self.k1 * (1 - self.b + self.b * self.doc_len / avg_dl))
             )
+
+        if score.sum() == 0:
+            raise ValueError("Either query is empty or all words are pruned")
         return score
 
-    def get_top_n(self, query, prune=0, n=5):
+    def get_top_n(self, query, n=5, prune=0):
         """
         Get top n documents ranked by tf-idf
         """
         scores = self.get_scores(query, prune)
         return np.argsort(scores)[::-1][:n], scores
```

## pyranker/rankers/tf_idf.py

```diff
@@ -1,9 +1,10 @@
 import numpy as np
-from preprocessing.tokenizer import tokenize
+
+from pyranker.preprocessing.tokenizer import tokenize
 
 from . import TfIdfWeighter
 
 
 class TfIdfRanking(TfIdfWeighter):
     def __init__(self, corpus):
         super().__init__(corpus, tokenize)
```

## pyranker/rankers/vspace.py

```diff
@@ -1,35 +1,47 @@
 import numpy as np
-from preprocessing.tokenizer import tokenize
+
+from pyranker.preprocessing.tokenizer import tokenize
 
 from . import TfIdfWeighter
 
 
 class VSpaceRanker(TfIdfWeighter):
     def __init__(self, corpus):
         super().__init__(corpus, tokenize)
 
-    def get_scores(self, query):
+    def get_vector_dim(self, prune=0):
+        """
+        Gets the dimension of the vector space
+        """
+        return sum(1 for v in self.idf.values() if v >= prune)
+
+    def get_scores(self, query, prune=0):
         """
         Gets the cosine scores of all documents w.r.t. query
-        Default configuration is lnc.ltc
+        Configuration is lnc.lnc
         """
         score = np.empty(shape=(0, self.corpus_size))
         q_score = []
         query = self._calc_freq(self.tokenizer(query))
         for word in self.word_freq.keys():
+            if self.idf.get(word, 0) < prune:
+                continue
             q_score.append(self.idf.get(word, 0) * query.get(word, 0))
             d_freq = np.array([doc.get(word, 0) for doc in self.doc_freqs])
             score = np.vstack((score, self.idf.get(word, 0) * d_freq))
 
         # Normalize scores
-        q_score = q_score / np.linalg.norm(q_score)
+        norm_val = np.linalg.norm(q_score)
+        if norm_val == 0:
+            raise ValueError("Either query is empty or all words are pruned")
+        q_score = q_score / norm_val
         score = score / np.linalg.norm(score, axis=0)
         # Calculate cosine score
         return np.dot(q_score.T, score).flatten()
 
-    def get_top_n(self, query, n=5):
+    def get_top_n(self, query, n=5, prune=0):
         """
         Get top n documents ranked by tf-idf
         """
-        scores = self.get_scores(query)
+        scores = self.get_scores(query, prune)
         return np.argsort(scores)[::-1][:n], scores
```

## Comparing `pyranker-0.1.2.dist-info/LICENSE` & `pyranker-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyranker-0.1.2.dist-info/METADATA` & `pyranker-0.1.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranker
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python based package consisiting of BM25 and         Vector Space Rankers for Information Retrieval
 Home-page: https://github.com/AvishrantsSh/PyRanker
 Author: AvishrantSh (Avishrant Sharma)
 Author-email: <avishrants@gmail.com>
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AvishrantsSh/PyRanker/issues
 Platform: UNKNOWN
```

## Comparing `pyranker-0.1.2.dist-info/RECORD` & `pyranker-0.1.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pyranker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyranker/preprocessing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyranker/preprocessing/normalizer.py,sha256=9VMOgBU0k4fo-06GMWHCLZHWOwN1a9LdBtO6tUDzwcw,507
 pyranker/preprocessing/tokenizer.py,sha256=GeS6SjmgIxXOnjATMkQSU1rFgFZfnPZABo4eJDwMfbg,216
-pyranker/rankers/__init__.py,sha256=HpfP50YusSq4fohtLLwSXGl0XDd5kWVHgdBMkaQKajk,1274
-pyranker/rankers/bm25.py,sha256=koZmYYe_R89UoY1KExyWyCbn9upKApbVQWmPCVcCMUk,1611
-pyranker/rankers/tf_idf.py,sha256=N8Z8SaX32Rmn-JPSXUJZakr44KmzuWClJmTjzXX7lgU,801
-pyranker/rankers/vspace.py,sha256=XXn0lqSwteU7-eKQ-Mw0ndOVnd408_9Sv82D8KHeYIE,1172
-pyranker-0.1.2.dist-info/LICENSE,sha256=5-dETpK1DgmAC-cXgfwkldJnpVpdt_U0f32yQ3lRBCQ,1072
-pyranker-0.1.2.dist-info/METADATA,sha256=OPx9y500j74-Y3SY83dDrNWPNzI0lqkEDdpCpqY1z1g,1139
-pyranker-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyranker-0.1.2.dist-info/top_level.txt,sha256=oJAiLyQwtBSkOcLtjGX9bR5qQwmCiSk2DxIXyxzvr6w,9
-pyranker-0.1.2.dist-info/RECORD,,
+pyranker/rankers/__init__.py,sha256=ax0TyULrFthiJH1t-FhGUlDN6T-XC-QtQe2wIy98HwY,1226
+pyranker/rankers/bm25.py,sha256=o5tKDc-CuCSeJwZVlomh2ZlfWqNqctU22CB2cpP0hhc,1720
+pyranker/rankers/tf_idf.py,sha256=OxF_ed8rOWz62xmr5pbhkYTz9nU1WoGJat0cO2VmPyo,811
+pyranker/rankers/vspace.py,sha256=nNQ-NTsU4mbhoijvXAkhf2iKihhZCvlDNtGKDo9gFpI,1576
+pyranker-0.1.3.dist-info/LICENSE,sha256=5-dETpK1DgmAC-cXgfwkldJnpVpdt_U0f32yQ3lRBCQ,1072
+pyranker-0.1.3.dist-info/METADATA,sha256=WUi3vB2yH8ApUdrHJDlcrOdTflQklAdC7qVGnnX5SEU,1139
+pyranker-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyranker-0.1.3.dist-info/top_level.txt,sha256=oJAiLyQwtBSkOcLtjGX9bR5qQwmCiSk2DxIXyxzvr6w,9
+pyranker-0.1.3.dist-info/RECORD,,
```

