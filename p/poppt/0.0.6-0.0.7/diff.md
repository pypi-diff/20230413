# Comparing `tmp/poppt-0.0.6.tar.gz` & `tmp/poppt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppt-0.0.6.tar", last modified: Wed Apr 12 13:11:10 2023, max compression
+gzip compressed data, was "poppt-0.0.7.tar", last modified: Thu Apr 13 14:32:36 2023, max compression
```

## Comparing `poppt-0.0.6.tar` & `poppt-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.277933 poppt-0.0.6/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5248 2023-04-12 13:11:10.278931 poppt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.230660 poppt-0.0.6/poppt/
--rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.6/poppt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.260656 poppt-0.0.6/poppt/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.6/poppt/api/__init__.py
--rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.6/poppt/api/ppt.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.266666 poppt-0.0.6/poppt/core/
--rw-rw-rw-   0        0        0     2120 2023-04-12 13:10:10.000000 poppt-0.0.6/poppt/core/PPTType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.6/poppt/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.268663 poppt-0.0.6/poppt/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.6/poppt/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.271658 poppt-0.0.6/poppt/lib/ppt/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.6/poppt/lib/ppt/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.6/poppt/lib/ppt/ppt2pdf_service.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.257657 poppt-0.0.6/poppt.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.6/poppt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2023-04-12 13:11:10.280943 poppt-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.275929 poppt-0.0.6/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      530 2023-04-12 13:02:45.000000 poppt-0.0.6/tests/test_ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.963542 poppt-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5248 2023-04-13 14:32:36.964543 poppt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.925535 poppt-0.0.7/poppt/
+-rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.7/poppt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.948541 poppt-0.0.7/poppt/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.7/poppt/api/__init__.py
+-rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.7/poppt/api/ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.952536 poppt-0.0.7/poppt/core/
+-rw-rw-rw-   0        0        0     2240 2023-04-13 14:29:56.000000 poppt-0.0.7/poppt/core/PPTType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.7/poppt/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.954535 poppt-0.0.7/poppt/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.7/poppt/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.957532 poppt-0.0.7/poppt/lib/ppt/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.7/poppt/lib/ppt/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.7/poppt/lib/ppt/ppt2pdf_service.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.940539 poppt-0.0.7/poppt.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-04-13 14:32:36.000000 poppt-0.0.7/poppt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-13 14:32:36.000000 poppt-0.0.7/poppt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:32:36.000000 poppt-0.0.7/poppt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.7/poppt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-04-13 14:32:36.000000 poppt-0.0.7/poppt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 14:32:36.000000 poppt-0.0.7/poppt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      722 2023-04-13 14:32:36.966542 poppt-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:32:36.961544 poppt-0.0.7/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      475 2023-04-13 14:29:24.000000 poppt-0.0.7/tests/test_ppt.py
```

### Comparing `poppt-0.0.6/LICENSE` & `poppt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poppt-0.0.6/PKG-INFO` & `poppt-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.6
+Version: 0.0.7
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.0.6/README.md` & `poppt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `poppt-0.0.6/poppt/api/ppt.py` & `poppt-0.0.7/poppt/api/ppt.py`

 * *Files identical despite different names*

### Comparing `poppt-0.0.6/poppt/core/PPTType.py` & `poppt-0.0.7/poppt/core/PPTType.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-import time
 from pathlib import *
 
 import win32com.client
 from pofile import get_files, mkdir
 from poprogress import simple_progress
 
 from poppt.lib.ppt.ppt2pdf_service import ppt2pdf_single
@@ -29,29 +27,30 @@
     def ppt2img(self, input_path, output_path, img_type):
         '''将PPT另存为图片格式
           arguments:
               pptFullName: 要转换的ppt文件，
               pptName：转换后的存放JPG文件的目录
               imgType: 图片类型
         '''
+        filenames = get_files(input_path)
         # 启动PPT
         pptClient = win32com.client.Dispatch('PowerPoint.Application')
         # 设置为0表示后台运行，不显示，1则显示
-        pptClient.Visible = False
-        # 打开PPT文件
-        ppt = pptClient.Presentations.Open(input_path)
-
-        # 另存为图片
-        # Python路径操作模块pathlib，看这篇就够了！ https://zhuanlan.zhihu.com/p/475661402
-        output_dir = Path(output_path) / str(Path(input_path).stem)
-        if not os.path.exists(output_dir):
-            os.mkdir(output_dir)
-        # JPG是17
-        img_type_jpg = 17
-        # PNG是18
-        img_type_png = 18
-        if img_type == 'jpg':
-            ppt.SaveAs(output_dir, img_type_jpg)
-        else:
-            ppt.SaveAs(output_dir, img_type_png)
-        # 退出
+        pptClient.Visible = True
+        for ppt_file in filenames:
+            # Python路径操作模块pathlib，看这篇就够了！ https://zhuanlan.zhihu.com/p/475661402
+            output_dir = Path(output_path).absolute() / str(Path(ppt_file).stem)
+            exsit, output_dir = mkdir(output_dir)
+            # JPG是17
+            img_type_jpg = 17
+            # PNG是18
+            img_type_png = 18
+
+            # 打开PPT文件
+            ppt = pptClient.Presentations.Open(ppt_file, WithWindow=False, ReadOnly=1)
+            # 另存为图片
+            if img_type == 'jpg':
+                ppt.SaveAs(output_dir, img_type_jpg)
+            else:
+                ppt.SaveAs(output_dir, img_type_png)
+            # 退出
         pptClient.Quit()
```

### Comparing `poppt-0.0.6/poppt/lib/ppt/ppt2pdf_service.py` & `poppt-0.0.7/poppt/lib/ppt/ppt2pdf_service.py`

 * *Files identical despite different names*

### Comparing `poppt-0.0.6/poppt.egg-info/PKG-INFO` & `poppt-0.0.7/poppt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.6
+Version: 0.0.7
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.0.6/setup.cfg` & `poppt-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 7074 0d0a 7665 7273 696f   = poppt..versio
-00000020: 6e20 3d20 302e 302e 360d 0a64 6573 6372  n = 0.0.6..descr
+00000020: 6e20 3d20 302e 302e 370d 0a64 6573 6372  n = 0.0.7..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 7074 0d0a 6c6f 6e67  tall poppt..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -31,15 +31,16 @@
 000001e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000001f0: 636f 6d2f 436f 6465 7257 616e 4665 6e67  com/CoderWanFeng
 00000200: 2f70 6f70 7074 0d0a 0d0a 5b6f 7074 696f  /poppt....[optio
 00000210: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
 00000220: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
 00000230: 6571 7569 7265 7320 3d20 0d0a 0970 7970  equires = ...pyp
 00000240: 6977 696e 3332 0d0a 0970 6f70 726f 6772  iwin32...poprogr
-00000250: 6573 730d 0a70 7974 686f 6e5f 7265 7175  ess..python_requ
-00000260: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
-00000270: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000280: 7461 203d 2054 7275 650d 0a7a 6970 5f73  ta = True..zip_s
-00000290: 6166 6520 3d20 4661 6c73 650d 0a0d 0a5b  afe = False....[
-000002a0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000002b0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000002c0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000250: 6573 730d 0a09 706f 6669 6c65 0d0a 7079  ess...pofile..py
+00000260: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000270: 3e3d 332e 370d 0a69 6e63 6c75 6465 5f70  >=3.7..include_p
+00000280: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000290: 7565 0d0a 7a69 705f 7361 6665 203d 2046  ue..zip_safe = F
+000002a0: 616c 7365 0d0a 0d0a 5b65 6767 5f69 6e66  alse....[egg_inf
+000002b0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+000002c0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000002d0: 0d0a                                     ..
```

