# Comparing `tmp/tts_arranger-0.1.0.tar.gz` & `tmp/tts_arranger-0.1.1.tar.gz`

## Comparing `tts_arranger-0.1.0.tar` & `tts_arranger-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    26358 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    14625 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/LICENSE
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    26358 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/PKG-INFO
```

### Comparing `tts_arranger-0.1.0/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.1/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.1/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.1/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.1/src/tts_arranger/tts_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,36 +328,44 @@
                 else:
                     # Don’t concatenate, convert the chapter temp files to the target format
                     os.makedirs(output_filename, exist_ok=True)
 
                     for name, file in self.temp_files:
                         output_chapter_filename = os.path.join(output_filename, name + output_extension)
 
+                        output_args = {'metadata': f'title={self.project.title} - {name}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}
+
+                        if self.output_format is 'mp3':
+                            output_args['audio_bitrate'] = '320k'
+
                         # Convert to target format, adding metadata
                         (
                             ffmpeg
                             .input(file)
-                            .output(output_chapter_filename, **{'metadata': f'title={self.project.title} - {name}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}, loglevel='error')
+                            .output(output_chapter_filename, **output_args, loglevel='error')
                             .run(overwrite_output=True)
                         )
 
                         output_files.append(output_chapter_filename)
                     log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under {output_filename}.')
 
-                image_added = False
-                for output_file in output_files:
-                    # Add image
-                    output_path_with_image = output_file + '_tmp' + output_extension
-
-                    if self.project.image_bytes:
+                if self.project.image_bytes:
+                    if self.output_format in ['m4b', 'm4a', 'mp3']:
                         image_bytes = base64.b64decode(self.project.image_bytes)
                         image_file = io.BytesIO(image_bytes)
                         image = Image.open(image_file)
 
                         if image.format:
-                            self._add_image(image, output_file, output_path_with_image)
-                            os.remove(output_file)
-                            os.rename(output_path_with_image, output_file)
-                            image_added = True
-
-                if image_added:
-                    log(LOG_TYPE.SUCCESS, 'Project image added to final output for all files.')
+                            image_added = False
+                            for output_file in output_files:
+                                # Add image
+                                output_path_with_image = output_file + '_tmp' + output_extension
+
+                                self._add_image(image, output_file, output_path_with_image)
+                                os.remove(output_file)
+                                os.rename(output_path_with_image, output_file)
+                                image_added = True
+
+                            if image_added:
+                                log(LOG_TYPE.SUCCESS, 'Project image added to final output for all files.')
+                    else:
+                        log(LOG_TYPE.WARNING, f'Images are only possible for m4b/m4a and mp3 at the moment.')
```

### Comparing `tts_arranger-0.1.0/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.1.1/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.1/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.1/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.1/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.1/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/tests/tts_arranger_test.py` & `tts_arranger-0.1.1/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/LICENSE` & `tts_arranger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/README.md` & `tts_arranger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.0/pyproject.toml` & `tts_arranger-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.1.0"
+version = "0.1.1"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.1.0/PKG-INFO` & `tts_arranger-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

