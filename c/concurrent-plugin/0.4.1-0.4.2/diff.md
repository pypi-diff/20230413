# Comparing `tmp/concurrent_plugin-0.4.1-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 30645 bytes, number of entries: 18
+Zip file size: 30813 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        2 b- defN 22-Nov-27 22:37 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    31511 b- defN 23-Mar-03 20:08 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    31658 b- defN 23-Apr-13 18:25 concurrent_plugin/concurrent_backend.py
 -rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-17 04:51 concurrent_plugin/concurrent_core.py
 -rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 23:54 concurrent_plugin/login.py
 -rw-rw-r--  2.0 unx     3994 b- defN 22-Dec-20 19:35 concurrent_plugin/periodic_run.py
 -rw-rw-r--  2.0 unx     1298 b- defN 23-Jan-19 23:36 concurrent_plugin/periodic_run_utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/__init__.py
 -rw-rw-r--  2.0 unx      990 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     5326 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinmount.py
 -rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    14896 b- defN 23-Mar-05 00:13 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      249 b- defN 23-Mar-05 00:15 concurrent_plugin-0.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-05 00:15 concurrent_plugin-0.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      182 b- defN 23-Mar-05 00:15 concurrent_plugin-0.4.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Mar-05 00:15 concurrent_plugin-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1663 b- defN 23-Mar-05 00:15 concurrent_plugin-0.4.1.dist-info/RECORD
-18 files, 106062 bytes uncompressed, 27857 bytes compressed:  73.7%
+-rw-rw-r--  2.0 unx    15276 b- defN 23-Apr-09 17:20 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      205 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      182 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/RECORD
+18 files, 106545 bytes uncompressed, 28025 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.4.1.dist-info/METADATA
+Filename: concurrent_plugin-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.4.1.dist-info/WHEEL
+Filename: concurrent_plugin-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.4.1.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.1.dist-info/top_level.txt
+Filename: concurrent_plugin-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.1.dist-info/RECORD
+Filename: concurrent_plugin-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_backend.py

```diff
@@ -550,14 +550,16 @@
         env_vars['DAGID'] = os.getenv('DAGID')
         job_template = mlflow.projects.kubernetes._get_kubernetes_job_definition(
             project_name, image_tag, image_digest, _get_run_command(command), env_vars, job_template
         )
         job_name = job_template["metadata"]["name"]
         job_namespace = job_template["metadata"]["namespace"]
         _load_kube_context(context=kube_context)
+        kubernetes.client.configuration.retries = 10
+        print(f'run_eks_job: Overrode default kubernetes.client.configuration.retries to 10')
 
         core_api_instance = kubernetes.client.CoreV1Api()
         tok = base64.b64encode(get_token_file_obj('r').read().encode('utf-8')).decode('utf-8')
         token_secret_name = 'parallelstokenfile-' + str(uuid.uuid4())
         try:
             core_api_instance.delete_namespaced_secret(namespace=job_namespace, name=token_secret_name)
         except Exception:
```

## concurrent_plugin/infinfs/mount_service.py

```diff
@@ -111,36 +111,42 @@
 
 
 def update_mlflow_run(run_id, status):
     client = MlflowClient()
     client.set_terminated(run_id, status)
 
 def _filter_empty_in_dict_list_scalar(dict_list_scalar:Union[list, dict, Any]):
+    """
+    given a 'dict' or 'list' as input, removes all elements in these containers that are empty: scalars with None, strings that are '', lists and dicts that are empty.  Note that the filtering is in-place: modifies the passed list or dict
+
+    Args:
+        dict_list_scalar (Union[list, dict, Any]): see above
+    """
     try:
         # depth first traveral
         if isinstance(dict_list_scalar, dict):
             keys_to_del:list = []
             for k in dict_list_scalar.keys():  
                 _filter_empty_in_dict_list_scalar(dict_list_scalar[k])
                 
                 # check if the 'key' is now None or empty.  If so, remove the 'key'
                 if not dict_list_scalar[k]: 
-                    # RuntimeError: dictionary changed size during iteration
+                    # cannont do dict.pop(): RuntimeError: dictionary changed size during iteration
                     # dict_list_scalar.pop(k)
                     keys_to_del.append(k)
             
             # now delete the keys from the map
             for k in keys_to_del:
                 dict_list_scalar.pop(k)
         elif isinstance(dict_list_scalar, list):
             i = 0; length = len(dict_list_scalar)
             while i < length: 
                 _filter_empty_in_dict_list_scalar(dict_list_scalar[i])
             
-                # check if element is now None or empty.  If so, remove the element from the list
+                # check if element is now None (if scalar) or empty (if list or dict).  If so, remove the element from the list
                 if not dict_list_scalar[i]:
                     dict_list_scalar.remove(dict_list_scalar[i])
                     i -= 1; length -= 1
                 
                 i += 1
         else: # this must be a non container, like int, str, datatime.datetime
             pass
```

## Comparing `concurrent_plugin-0.4.1.dist-info/RECORD` & `concurrent_plugin-0.4.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-concurrent_plugin/concurrent_backend.py,sha256=b_hwtFCsE19JokIn9Uc3L-hKF9lNsYcWtqSo4i7TeLQ,31511
+concurrent_plugin/concurrent_backend.py,sha256=u8iTg8RKtpvkoZPPXtvFyQRST4PzetQsfMJjT1CrI6M,31658
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
 concurrent_plugin/periodic_run_utils.py,sha256=MZuX9uSFEuA7B8UFDAchsrWhidXT5QyuOA-GDtzIPOo,1298
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
-concurrent_plugin/infinfs/mount_service.py,sha256=wnPr5Py9Wi36fQKTOSfoRs2zwWbARqqC7tYbRirTLIM,14896
-concurrent_plugin-0.4.1.dist-info/METADATA,sha256=h36Qg8nqKy77yy_pP-Bd8Y7dGrShBG3-xCf-BJyiVWc,249
-concurrent_plugin-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.4.1.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
-concurrent_plugin-0.4.1.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.4.1.dist-info/RECORD,,
+concurrent_plugin/infinfs/mount_service.py,sha256=y2vNoDpEXLm95ch_GDhnVNF7oXf8I9fvQZhjc_JNcX4,15276
+concurrent_plugin-0.4.2.dist-info/METADATA,sha256=bwxXwlbkanwtMdpB9j0ofqdOwYaFiwTw1JO0_ArJ1jc,205
+concurrent_plugin-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.4.2.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
+concurrent_plugin-0.4.2.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.4.2.dist-info/RECORD,,
```

