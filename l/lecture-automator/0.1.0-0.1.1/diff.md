# Comparing `tmp/lecture-automator-0.1.0.tar.gz` & `tmp/lecture-automator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecture-automator-0.1.0.tar", max compression
+gzip compressed data, was "lecture-automator-0.1.1.tar", max compression
```

## Comparing `lecture-automator-0.1.0.tar` & `lecture-automator-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1140 2023-04-11 18:25:06.815497 lecture-automator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.1.0/src/lecture_automator/__init__.py
--rw-r--r--   0        0        0      831 2023-04-11 18:02:48.539135 lecture-automator-0.1.0/src/lecture_automator/cli.py
--rw-r--r--   0        0        0     1934 2023-04-11 16:44:42.058381 lecture-automator-0.1.0/src/lecture_automator/gen_speech.py
--rw-r--r--   0        0        0     1919 2023-04-11 17:50:28.846174 lecture-automator-0.1.0/src/lecture_automator/gen_video.py
--rw-r--r--   0        0        0     1031 2023-04-11 19:05:03.976910 lecture-automator-0.1.0/src/lecture_automator/marp_api.py
--rw-r--r--   0        0        0     2430 2023-04-11 18:00:24.487850 lecture-automator-0.1.0/src/lecture_automator/parser.py
--rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.1.0/src/lecture_automator/settings.py
--rw-r--r--   0        0        0      904 2023-04-11 19:18:00.330171 lecture-automator-0.1.0/setup.py
--rw-r--r--   0        0        0      534 2023-04-11 19:18:00.330323 lecture-automator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1140 2023-04-13 20:31:53.497325 lecture-automator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.1.1/src/lecture_automator/__init__.py
+-rw-r--r--   0        0        0      831 2023-04-11 18:02:48.539135 lecture-automator-0.1.1/src/lecture_automator/cli.py
+-rw-r--r--   0        0        0     1934 2023-04-11 16:44:42.058381 lecture-automator-0.1.1/src/lecture_automator/gen_speech.py
+-rw-r--r--   0        0        0     1995 2023-04-13 20:31:53.497461 lecture-automator-0.1.1/src/lecture_automator/gen_video.py
+-rw-r--r--   0        0        0     1051 2023-04-13 20:31:53.497573 lecture-automator-0.1.1/src/lecture_automator/marp_api.py
+-rw-r--r--   0        0        0     2430 2023-04-11 18:00:24.487850 lecture-automator-0.1.1/src/lecture_automator/parser.py
+-rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.1.1/src/lecture_automator/settings.py
+-rw-r--r--   0        0        0      904 2023-04-13 20:36:27.090350 lecture-automator-0.1.1/setup.py
+-rw-r--r--   0        0        0      534 2023-04-13 20:36:27.090498 lecture-automator-0.1.1/PKG-INFO
```

### Comparing `lecture-automator-0.1.0/pyproject.toml` & `lecture-automator-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lecture-automator"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["CapBlood <stalker.anonim@mail.ru>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ffmpeg-python = "^0.2.0"
 torch = "^2.0.0"
```

### Comparing `lecture-automator-0.1.0/src/lecture_automator/cli.py` & `lecture-automator-0.1.1/src/lecture_automator/cli.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.1.0/src/lecture_automator/gen_speech.py` & `lecture-automator-0.1.1/src/lecture_automator/gen_speech.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.1.0/src/lecture_automator/gen_video.py` & `lecture-automator-0.1.1/src/lecture_automator/gen_video.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,26 +17,29 @@
     """
 
     files = []
     for path_image, path_wav in zip(path_images, path_wavs):
         files.extend([ffmpeg.input(path_image), ffmpeg.input(path_wav)])
 
     joined = ffmpeg.concat(*files, v=1, a=1).node
-    ffmpeg.output(joined[0], joined[1], output_name).run(overwrite_output=True)
+    ffmpeg.output(
+        joined[0], joined[1], output_name, 
+        f='mp4', vcodec='libx264', acodec='aac'
+    ).run(overwrite_output=True)
 
 
 if __name__ == '__main__':
     # with open('examples/Example_2.md') as file:
     #     md_text = file.read()
     # generate_marp_slides("examples", md_text)
-    path_to_image = "/Users/donsangre/PycharmProjects/lecture-automator/examples/Slide.001.png"
-    path_to_image_2 = "/Users/donsangre/PycharmProjects/lecture-automator/examples/Slide.002.png"
+    path_to_image = "/Users/donsangre/PycharmProjects/lecture-automator/examples/Example.001.png"
+    path_to_image_2 = "/Users/donsangre/PycharmProjects/lecture-automator/examples/Example.002.png"
     path_to_audio = "/Users/donsangre/PycharmProjects/lecture-automator/examples/Example.wav"
 
-    generate_video([path_to_image, path_to_image_2], [path_to_audio, path_to_audio], 'output2.mp4')
+    generate_video([path_to_image, path_to_image_2], [path_to_audio, path_to_audio], 'examples/output.mp4')
 
     # input_still = ffmpeg.input(path_to_image)
     # input_audio = ffmpeg.input("/Users/donsangre/PycharmProjects/lecture-automator/examples/Example.wav")
 
     # (
     #     ffmpeg
     #     .concat(input_still, input_audio, v=1, a=1)
```

### Comparing `lecture-automator-0.1.0/src/lecture_automator/marp_api.py` & `lecture-automator-0.1.1/src/lecture_automator/marp_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     with tempfile.TemporaryDirectory() as tmpdirname:
         path_to_md = os.path.join(tmpdirname, "input.md")
         with open(path_to_md, "w") as file:
             file.write(md_text)
 
         subprocess.run(
-            ['marp', '--images', type_images, '-o', 'Slide.png', path_to_md],
+            ['marp', '--images', type_images, '--image-scale', '2', '-o', 'Slide.png', path_to_md],
             cwd=outdir
         )
 
 
 if __name__ == '__main__':
-    with open('examples/Example_2.md') as file:
+    with open('examples/Example.md') as file:
         text = file.read()
 
     generate_marp_slides('examples', text)
```

### Comparing `lecture-automator-0.1.0/src/lecture_automator/parser.py` & `lecture-automator-0.1.1/src/lecture_automator/parser.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.1.0/setup.py` & `lecture-automator-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 entry_points = \
 {'console_scripts': ['lecture-automator = '
                      'lecture_automator.cli:convert_md_to_mp4']}
 
 setup_kwargs = {
     'name': 'lecture-automator',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': None,
     'author': 'CapBlood',
     'author_email': 'stalker.anonim@mail.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `lecture-automator-0.1.0/PKG-INFO` & `lecture-automator-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecture-automator
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: CapBlood
 Author-email: stalker.anonim@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

