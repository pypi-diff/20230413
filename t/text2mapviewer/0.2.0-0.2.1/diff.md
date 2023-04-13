# Comparing `tmp/text2mapviewer-0.2.0.tar.gz` & `tmp/text2mapviewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2mapviewer-0.2.0.tar", last modified: Thu Apr 13 12:38:26 2023, max compression
+gzip compressed data, was "text2mapviewer-0.2.1.tar", last modified: Thu Apr 13 13:09:34 2023, max compression
```

## Comparing `text2mapviewer-0.2.0.tar` & `text2mapviewer-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/LICENSE
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       40 2023-04-13 11:39:22.000000 text2mapviewer-0.2.0/MANIFEST.in
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1889 2023-04-13 12:35:34.000000 text2mapviewer-0.2.0/README.md
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      801 2023-04-13 12:35:47.000000 text2mapviewer-0.2.0/pyproject.toml
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     4130 2023-04-13 11:33:40.000000 text2mapviewer-0.2.0/requirements.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/setup.cfg
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.370601 text2mapviewer-0.2.0/text2mapviewer/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapviewer-0.2.0/text2mapviewer/__init__.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/text2mapviewer/examples/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/text2mapviewer/examples/map_embedding.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/text2mapviewer/fondamental/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/text2mapviewer/fondamental/bases.py
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/text2mapviewer/main.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/text2mapviewer.egg-info/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      377 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/SOURCES.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/dependency_links.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1300 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/requires.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       15 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/top_level.txt
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/LICENSE
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       40 2023-04-13 11:39:22.000000 text2mapviewer-0.2.1/MANIFEST.in
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1889 2023-04-13 12:35:34.000000 text2mapviewer-0.2.1/README.md
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      801 2023-04-13 13:09:22.000000 text2mapviewer-0.2.1/pyproject.toml
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     4626 2023-04-13 13:08:51.000000 text2mapviewer-0.2.1/requirements.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/setup.cfg
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapviewer-0.2.1/text2mapviewer/__init__.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer/examples/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/text2mapviewer/examples/map_embedding.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer/fondamental/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/text2mapviewer/fondamental/bases.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/text2mapviewer/main.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer.egg-info/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      377 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       66 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/requires.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       15 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/top_level.txt
```

### Comparing `text2mapviewer-0.2.0/LICENSE` & `text2mapviewer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.2.0/PKG-INFO` & `text2mapviewer-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2mapviewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapviewer
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `text2mapviewer-0.2.0/README.md` & `text2mapviewer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.2.0/pyproject.toml` & `text2mapviewer-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2mapviewer"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name= "Papa Séga WADE", email= "pasega.wade@gmail.com"}
 ]
 
 description = "A python package to map your own csv files data using Atlas from NOMIC"
 readme={file = "README.md", content-type = "text/markdown"} 
 keywords=[
```

### Comparing `text2mapviewer-0.2.0/requirements.txt` & `text2mapviewer-0.2.1/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,215 +1,223 @@
-#
-# This file is autogenerated by pip-compile with Python 3.10
-# by the following command:
-#
-#    pip-compile pyproject.toml
-#
-aiohttp==3.8.4
-    # via cohere
-aiosignal==1.3.1
-    # via aiohttp
-async-timeout==4.0.2
-    # via aiohttp
-attrs==22.2.0
-    # via
-    #   aiohttp
-    #   jsonlines
-backoff==2.2.1
-    # via cohere
-certifi==2022.12.7
-    # via requests
-charset-normalizer==3.1.0
-    # via
-    #   aiohttp
-    #   requests
-click==8.1.3
-    # via
-    #   nltk
-    #   nomic
-    #   text2mapviewer (pyproject.toml)
-cmake==3.26.3
-    # via triton
-cohere==4.1.4
-    # via nomic
-filelock==3.11.0
-    # via
-    #   huggingface-hub
-    #   torch
-    #   transformers
-    #   triton
-frozenlist==1.3.3
-    # via
-    #   aiohttp
-    #   aiosignal
-huggingface-hub==0.13.4
-    # via
-    #   sentence-transformers
-    #   transformers
-idna==3.4
-    # via
-    #   requests
-    #   yarl
-jinja2==3.1.2
-    # via torch
-joblib==1.2.0
-    # via
-    #   nltk
-    #   scikit-learn
-jsonlines==3.1.0
-    # via nomic
-lit==16.0.1
-    # via triton
-loguru==0.7.0
-    # via nomic
-markdown-it-py==2.2.0
-    # via rich
-markupsafe==2.1.2
-    # via jinja2
-mdurl==0.1.2
-    # via markdown-it-py
-mpmath==1.3.0
-    # via sympy
-multidict==6.0.4
-    # via
-    #   aiohttp
-    #   yarl
-networkx==3.1
-    # via torch
-nltk==3.8.1
-    # via sentence-transformers
-nomic==1.1.6
-    # via text2mapviewer (pyproject.toml)
-numpy==1.24.2
-    # via
-    #   nomic
-    #   pandas
-    #   pyarrow
-    #   scikit-learn
-    #   scipy
-    #   sentence-transformers
-    #   text2mapviewer (pyproject.toml)
-    #   torchvision
-    #   transformers
-nvidia-cublas-cu11==11.10.3.66
-    # via
-    #   nvidia-cudnn-cu11
-    #   nvidia-cusolver-cu11
-    #   torch
-nvidia-cuda-cupti-cu11==11.7.101
-    # via torch
-nvidia-cuda-nvrtc-cu11==11.7.99
-    # via torch
-nvidia-cuda-runtime-cu11==11.7.99
-    # via torch
-nvidia-cudnn-cu11==8.5.0.96
-    # via torch
-nvidia-cufft-cu11==10.9.0.58
-    # via torch
-nvidia-curand-cu11==10.2.10.91
-    # via torch
-nvidia-cusolver-cu11==11.4.0.1
-    # via torch
-nvidia-cusparse-cu11==11.7.4.91
-    # via torch
-nvidia-nccl-cu11==2.14.3
-    # via torch
-nvidia-nvtx-cu11==11.7.91
-    # via torch
-packaging==23.1
-    # via
-    #   huggingface-hub
-    #   transformers
-pandas==2.0.0
-    # via text2mapviewer (pyproject.toml)
-pillow==9.5.0
-    # via torchvision
-pyarrow==11.0.0
-    # via nomic
-pydantic==1.10.7
-    # via nomic
-pygments==2.15.0
-    # via rich
-python-dateutil==2.8.2
-    # via pandas
-pytz==2023.3
-    # via pandas
-pyyaml==6.0
-    # via
-    #   huggingface-hub
-    #   transformers
-regex==2023.3.23
-    # via
-    #   nltk
-    #   transformers
-requests==2.28.2
-    # via
-    #   cohere
-    #   huggingface-hub
-    #   nomic
-    #   torchvision
-    #   transformers
-rich==13.3.4
-    # via nomic
-scikit-learn==1.2.2
-    # via sentence-transformers
-scipy==1.10.1
-    # via
-    #   scikit-learn
-    #   sentence-transformers
-sentence-transformers==2.2.2
-    # via text2mapviewer (pyproject.toml)
-sentencepiece==0.1.98
-    # via sentence-transformers
-six==1.16.0
-    # via python-dateutil
-sympy==1.11.1
-    # via torch
-threadpoolctl==3.1.0
-    # via scikit-learn
-tokenizers==0.13.3
-    # via transformers
-torch==2.0.0
-    # via
-    #   sentence-transformers
-    #   text2mapviewer (pyproject.toml)
-    #   torchvision
-    #   triton
-torchvision==0.15.1
-    # via sentence-transformers
-tqdm==4.65.0
-    # via
-    #   huggingface-hub
-    #   nltk
-    #   nomic
-    #   sentence-transformers
-    #   transformers
-transformers==4.27.4
-    # via
-    #   sentence-transformers
-    #   text2mapviewer (pyproject.toml)
-triton==2.0.0
-    # via torch
-typing-extensions==4.5.0
-    # via
-    #   huggingface-hub
-    #   pydantic
-    #   torch
-tzdata==2023.3
-    # via pandas
-urllib3==1.26.15
-    # via requests
-wheel==0.40.0
-    # via
-    #   nvidia-cublas-cu11
-    #   nvidia-cuda-cupti-cu11
-    #   nvidia-cuda-runtime-cu11
-    #   nvidia-curand-cu11
-    #   nvidia-cusparse-cu11
-    #   nvidia-nvtx-cu11
-wonderwords==2.2.0
-    # via nomic
-yarl==1.8.2
-    # via aiohttp
+click
+torch 
+transformers
+sentence-transformers
+nomic
+numpy
+pandas
 
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+# #
+# # This file is autogenerated by pip-compile with Python 3.10
+# # by the following command:
+# #
+# #    pip-compile pyproject.toml
+# #
+# aiohttp==3.8.4
+#     # via cohere
+# aiosignal==1.3.1
+#     # via aiohttp
+# async-timeout==4.0.2
+#     # via aiohttp
+# attrs==22.2.0
+#     # via
+#     #   aiohttp
+#     #   jsonlines
+# backoff==2.2.1
+#     # via cohere
+# certifi==2022.12.7
+#     # via requests
+# charset-normalizer==3.1.0
+#     # via
+#     #   aiohttp
+#     #   requests
+# click==8.1.3
+#     # via
+#     #   nltk
+#     #   nomic
+#     #   text2mapviewer (pyproject.toml)
+# cmake==3.26.3
+#     # via triton
+# cohere==4.1.4
+#     # via nomic
+# filelock==3.11.0
+#     # via
+#     #   huggingface-hub
+#     #   torch
+#     #   transformers
+#     #   triton
+# frozenlist==1.3.3
+#     # via
+#     #   aiohttp
+#     #   aiosignal
+# huggingface-hub==0.13.4
+#     # via
+#     #   sentence-transformers
+#     #   transformers
+# idna==3.4
+#     # via
+#     #   requests
+#     #   yarl
+# jinja2==3.1.2
+#     # via torch
+# joblib==1.2.0
+#     # via
+#     #   nltk
+#     #   scikit-learn
+# jsonlines==3.1.0
+#     # via nomic
+# lit==16.0.1
+#     # via triton
+# loguru==0.7.0
+#     # via nomic
+# markdown-it-py==2.2.0
+#     # via rich
+# markupsafe==2.1.2
+#     # via jinja2
+# mdurl==0.1.2
+#     # via markdown-it-py
+# mpmath==1.3.0
+#     # via sympy
+# multidict==6.0.4
+#     # via
+#     #   aiohttp
+#     #   yarl
+# networkx==3.1
+#     # via torch
+# nltk==3.8.1
+#     # via sentence-transformers
+# nomic==1.1.6
+#     # via text2mapviewer (pyproject.toml)
+# numpy==1.24.2
+#     # via
+#     #   nomic
+#     #   pandas
+#     #   pyarrow
+#     #   scikit-learn
+#     #   scipy
+#     #   sentence-transformers
+#     #   text2mapviewer (pyproject.toml)
+#     #   torchvision
+#     #   transformers
+# nvidia-cublas-cu11==11.10.3.66
+#     # via
+#     #   nvidia-cudnn-cu11
+#     #   nvidia-cusolver-cu11
+#     #   torch
+# nvidia-cuda-cupti-cu11==11.7.101
+#     # via torch
+# nvidia-cuda-nvrtc-cu11==11.7.99
+#     # via torch
+# nvidia-cuda-runtime-cu11==11.7.99
+#     # via torch
+# nvidia-cudnn-cu11==8.5.0.96
+#     # via torch
+# nvidia-cufft-cu11==10.9.0.58
+#     # via torch
+# nvidia-curand-cu11==10.2.10.91
+#     # via torch
+# nvidia-cusolver-cu11==11.4.0.1
+#     # via torch
+# nvidia-cusparse-cu11==11.7.4.91
+#     # via torch
+# nvidia-nccl-cu11==2.14.3
+#     # via torch
+# nvidia-nvtx-cu11==11.7.91
+#     # via torch
+# packaging==23.1
+#     # via
+#     #   huggingface-hub
+#     #   transformers
+# pandas==2.0.0
+#     # via text2mapviewer (pyproject.toml)
+# pillow==9.5.0
+#     # via torchvision
+# pyarrow==11.0.0
+#     # via nomic
+# pydantic==1.10.7
+#     # via nomic
+# pygments==2.15.0
+#     # via rich
+# python-dateutil==2.8.2
+#     # via pandas
+# pytz==2023.3
+#     # via pandas
+# pyyaml==6.0
+#     # via
+#     #   huggingface-hub
+#     #   transformers
+# regex==2023.3.23
+#     # via
+#     #   nltk
+#     #   transformers
+# requests==2.28.2
+#     # via
+#     #   cohere
+#     #   huggingface-hub
+#     #   nomic
+#     #   torchvision
+#     #   transformers
+# rich==13.3.4
+#     # via nomic
+# scikit-learn==1.2.2
+#     # via sentence-transformers
+# scipy==1.10.1
+#     # via
+#     #   scikit-learn
+#     #   sentence-transformers
+# sentence-transformers==2.2.2
+#     # via text2mapviewer (pyproject.toml)
+# sentencepiece==0.1.98
+#     # via sentence-transformers
+# six==1.16.0
+#     # via python-dateutil
+# sympy==1.11.1
+#     # via torch
+# threadpoolctl==3.1.0
+#     # via scikit-learn
+# tokenizers==0.13.3
+#     # via transformers
+# torch==2.0.0
+#     # via
+#     #   sentence-transformers
+#     #   text2mapviewer (pyproject.toml)
+#     #   torchvision
+#     #   triton
+# torchvision==0.15.1
+#     # via sentence-transformers
+# tqdm==4.65.0
+#     # via
+#     #   huggingface-hub
+#     #   nltk
+#     #   nomic
+#     #   sentence-transformers
+#     #   transformers
+# transformers==4.27.4
+#     # via
+#     #   sentence-transformers
+#     #   text2mapviewer (pyproject.toml)
+# triton==2.0.0
+#     # via torch
+# typing-extensions==4.5.0
+#     # via
+#     #   huggingface-hub
+#     #   pydantic
+#     #   torch
+# tzdata==2023.3
+#     # via pandas
+# urllib3==1.26.15
+#     # via requests
+# wheel==0.40.0
+#     # via
+#     #   nvidia-cublas-cu11
+#     #   nvidia-cuda-cupti-cu11
+#     #   nvidia-cuda-runtime-cu11
+#     #   nvidia-curand-cu11
+#     #   nvidia-cusparse-cu11
+#     #   nvidia-nvtx-cu11
+# wonderwords==2.2.0
+#     # via nomic
+# yarl==1.8.2
+#     # via aiohttp
+
+# # The following packages are considered to be unsafe in a requirements file:
+# # setuptools
```

### Comparing `text2mapviewer-0.2.0/text2mapviewer/fondamental/bases.py` & `text2mapviewer-0.2.1/text2mapviewer/fondamental/bases.py`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.2.0/text2mapviewer/main.py` & `text2mapviewer-0.2.1/text2mapviewer/main.py`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.2.0/text2mapviewer.egg-info/PKG-INFO` & `text2mapviewer-0.2.1/text2mapviewer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2mapviewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapviewer
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

