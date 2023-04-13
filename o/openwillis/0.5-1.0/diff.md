# Comparing `tmp/openwillis-0.5.tar.gz` & `tmp/openwillis-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-0.5.tar", last modified: Wed Apr 12 18:35:38 2023, max compression
+gzip compressed data, was "openwillis-1.0.tar", last modified: Thu Apr 13 19:13:56 2023, max compression
```

## Comparing `openwillis-0.5.tar` & `openwillis-1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-12 18:35:17.000000 openwillis-0.5/LICENSE.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-12 18:35:17.000000 openwillis-0.5/MANIFEST.in
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-12 18:35:38.447394 openwillis-0.5/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-12 18:35:17.000000 openwillis-0.5/README.md
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-12 18:35:17.000000 openwillis-0.5/RELEASE.md
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/api.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/audio/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/audio/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    15855 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/audio/acoustic.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/audio/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/audio/config/acoustic.json
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/speech/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     2388 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/aws_transcribe.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/speech/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/config/speech.json
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     6061 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/speech_attribute.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     7234 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/speech_separation.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     9148 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/speech_transcribe.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    30695 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/util.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/video/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/video/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/config/facial.json
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    16067 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/face_landmark.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    10471 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/facial_emotion.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/usability.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis.egg-info/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/SOURCES.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/dependency_links.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/not-zip-safe
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/requires.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/top_level.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-12 18:35:17.000000 openwillis-0.5/requirements.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-12 18:35:38.447394 openwillis-0.5/setup.cfg
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      934 2023-04-12 18:35:17.000000 openwillis-0.5/setup.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-13 19:13:26.000000 openwillis-1.0/LICENSE.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-13 19:13:26.000000 openwillis-1.0/MANIFEST.in
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-13 19:13:56.121919 openwillis-1.0/PKG-INFO
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-13 19:13:26.000000 openwillis-1.0/README.md
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-13 19:13:26.000000 openwillis-1.0/RELEASE.md
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.111919 openwillis-1.0/openwillis/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/__init__.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/api.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/audio/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/audio/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    15855 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/audio/acoustic.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/audio/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/audio/config/acoustic.json
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/speech/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     2388 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/aws_transcribe.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/speech/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/config/speech.json
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     6061 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/speech_attribute.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     7234 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/speech_separation.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     9092 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/speech_transcribe.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    30695 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/util.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/video/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/__init__.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/video/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/config/facial.json
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    16067 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/face_landmark.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    10471 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/facial_emotion.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/usability.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis.egg-info/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/PKG-INFO
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/not-zip-safe
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/requires.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/top_level.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-13 19:13:26.000000 openwillis-1.0/requirements.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-13 19:13:56.131919 openwillis-1.0/setup.cfg
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      934 2023-04-13 19:13:26.000000 openwillis-1.0/setup.py
```

### Comparing `openwillis-0.5/LICENSE.txt` & `openwillis-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/PKG-INFO` & `openwillis-1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 0.5
+Version: 1.0
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6.*
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-0.5/README.md` & `openwillis-1.0/README.md`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/audio/acoustic.py` & `openwillis-1.0/openwillis/features/audio/acoustic.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/audio/config/acoustic.json` & `openwillis-1.0/openwillis/features/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/speech/aws_transcribe.py` & `openwillis-1.0/openwillis/features/speech/aws_transcribe.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/speech/config/speech.json` & `openwillis-1.0/openwillis/features/speech/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/speech/speech_attribute.py` & `openwillis-1.0/openwillis/features/speech/speech_attribute.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/speech/speech_separation.py` & `openwillis-1.0/openwillis/features/speech/speech_separation.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/speech/speech_transcribe.py` & `openwillis-1.0/openwillis/features/speech/speech_transcribe.py`

 * *Files 4% similar despite different names*

```diff
@@ -252,28 +252,28 @@
         The name of the transcription job. Only applicable if model is 'aws'. Default is 'transcribe_job_01'.
     transcribe_interval : list, optional
         A list of tuples representing the start and end times (in seconds) of segments of the audio file to be transcribed.
         Only applicable if model is 'vosk'. Default is an empty list.
 
     Returns:
     ...........
-    framewise : pandas.DataFrame
-        A DataFrame containing the framewise transcription of the audio file.
-    summary : pandas.DataFrame
-        A DataFrame containing the summary of the transcription results.
+    json_response : JSON Object
+        A transcription response object in JSON format
+    transcript : str
+        The transcript of the recording.
 
     ------------------------------------------------------------------------------------------------------
     """
     model = kwargs.get('model', 'vosk')
     language = kwargs.get('language', 'en-us')
 
     region = kwargs.get('region', 'us-east-1')
     job_name = kwargs.get('job_name', 'transcribe_job_01')
     transcribe_interval = kwargs.get('transcribe_interval', [])
 
     if model.lower() == 'aws':
-        json_response, transcript = aws.transcribe_audio(filepath, region, job_name)
+        json_response, transcript = aws.transcribe_audio(filepath, region, job_name, language)
 
     else:
         json_response, transcript = run_vosk(filepath, language, transcribe_interval)
 
     return json_response, transcript
```

### Comparing `openwillis-0.5/openwillis/features/speech/util.py` & `openwillis-1.0/openwillis/features/speech/util.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/video/face_landmark.py` & `openwillis-1.0/openwillis/features/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis/features/video/facial_emotion.py` & `openwillis-1.0/openwillis/features/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/openwillis.egg-info/PKG-INFO` & `openwillis-1.0/openwillis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 0.5
+Version: 1.0
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6.*
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-0.5/openwillis.egg-info/SOURCES.txt` & `openwillis-1.0/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-0.5/setup.py` & `openwillis-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='0.5',
+                 version='1.0',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6.*',
                  install_requires=install_requires,
```

