# Comparing `tmp/deepprofile-0.0.7.tar.gz` & `tmp/deepprofile-0.0.8.tar.gz`

## Comparing `deepprofile-0.0.7.tar` & `deepprofile-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 deepprofile-0.0.7/deepprofile/__about__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deepprofile-0.0.7/deepprofile/__init__.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 deepprofile-0.0.7/deepprofile/ncu.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 deepprofile-0.0.7/deepprofile/nsight.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 deepprofile-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepprofile-0.0.7/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 deepprofile-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 deepprofile-0.0.7/README.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deepprofile-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 deepprofile-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepprofile-0.0.8/tmp.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/__about__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/__init__.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/dcgm.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/nsight.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 deepprofile-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepprofile-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 deepprofile-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 deepprofile-0.0.8/README.md
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deepprofile-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 deepprofile-0.0.8/PKG-INFO
```

### Comparing `deepprofile-0.0.7/deepprofile/nsight.py` & `deepprofile-0.0.8/deepprofile/nsight.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,20 @@
         for result in results:
             c.execute(
                 f"SELECT value FROM StringIds WHERE id = {result['shortName']}",
             )
             result["name"] = c.fetchone()[0]
         return results
 
+    def get_generic_events(self):
+        c = self._conn.cursor()
+        c.execute("SELECT data FROM GENERIC_EVENTS")
+        results = query_results_to_json(c)
+        return results
+
     def compute_occupancy(self, device_id, blocks, grids):
         gpu_info = [x for x in self.get_gpu_info() if x["id"] == device_id][0]
         gpu_max_blocks = (
             gpu_info["maxBlockDimX"]
             * gpu_info["maxBlockDimY"]
             * gpu_info["maxBlockDimZ"]
         )
@@ -138,14 +144,18 @@
         return {
             "block_occupancy": blocks / gpu_max_blocks,
             "grid_occupancy": grids / gpu_max_grids,
         }
 
 
 if __name__ == "__main__":
+    import torch
 
     def foo(a, b):
         return a + b
 
+    (arg1, arg2) = (torch.randn(10, 10), torch.randn(10, 10))
+    # (arg1, arg2) = (arg1.to("cuda"), arg2.to("cuda"))
     with run(foo, 1, 2) as s:
         analyzer = NsightAnalyzer(s)
         print(analyzer.get_nvtx_events())
+        print(analyzer.get_generic_events())
```

### Comparing `deepprofile-0.0.7/LICENSE.txt` & `deepprofile-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.7/README.md` & `deepprofile-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.7/pyproject.toml` & `deepprofile-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.7/PKG-INFO` & `deepprofile-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepprofile
-Version: 0.0.7
+Version: 0.0.8
 Project-URL: Documentation, https://github.com/unknown/deepprofile#readme
 Project-URL: Issues, https://github.com/unknown/deepprofile/issues
 Project-URL: Source, https://github.com/unknown/deepprofile
 Author-email: SamKG <samyak.k.gupta@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

