# Comparing `tmp/pyvosklivesubtitle-0.1.2.tar.gz` & `tmp/pyvosklivesubtitle-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvosklivesubtitle-0.1.2.tar", last modified: Mon Apr 10 02:10:48 2023, max compression
+gzip compressed data, was "pyvosklivesubtitle-0.1.3.tar", last modified: Thu Apr 13 16:51:10 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.2.tar` & `pyvosklivesubtitle-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:10:48.889864 pyvosklivesubtitle-0.1.2/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1617 2023-04-10 02:10:48.890610 pyvosklivesubtitle-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 02:10:48.849403 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0    90112 2023-04-10 02:09:51.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:10:48.888363 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1617 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-10 02:10:48.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-10 02:10:47.000000 pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-10 02:10:48.893607 pyvosklivesubtitle-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-04-10 02:10:11.000000 pyvosklivesubtitle-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:51:10.030189 pyvosklivesubtitle-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1617 2023-04-13 16:51:10.030783 pyvosklivesubtitle-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:51:10.010554 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0   101666 2023-04-13 16:16:39.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:51:10.028535 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1617 2023-04-13 16:51:09.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-13 16:51:09.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:51:09.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-13 16:51:09.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-04-13 16:51:09.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-13 16:51:09.000000 pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-13 16:51:10.033031 pyvosklivesubtitle-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-04-12 10:56:50.000000 pyvosklivesubtitle-0.1.3/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.2/LICENSE` & `pyvosklivesubtitle-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.2/PKG-INFO` & `pyvosklivesubtitle-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.2/README.md` & `pyvosklivesubtitle-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.2/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.3/pyvosklivesubtitle/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 except ImportError:
     import Queue  # Python 2 import
 
 import tempfile
 from datetime import datetime, timedelta
 import subprocess
 import ctypes
-import platform
+import ctypes.wintypes
 from streamlink import Streamlink
 from streamlink.exceptions import NoPluginError
 import six
 import pysrt
 import shutil
 import re
 import select
 
 
 #---------------------------------------------------------VOSK PART---------------------------------------------------------------------#
 
+
 import requests
 from zipfile import ZipFile
 from re import match
 from pathlib import Path
 from tqdm import tqdm
 import _cffi_backend
 
@@ -644,16 +645,16 @@
 
 map_dst_of_language = dict(zip(arraylist_dst_languages, arraylist_dst))
 map_language_of_dst = dict(zip(arraylist_dst, arraylist_dst_languages))
 
 thread_record_streaming = None
 thread_recognize = None
 thread_timed_translate = None
-text=''
-
+text = ""
+translated_text = ""
 
 #-------------------------------------------------------------MISC FUNCTIONS-------------------------------------------------------------#
 
 
 def srt_formatter(subtitles, padding_before=0, padding_after=0):
     """
     Serialize a list of subtitles according to the SRT format, with optional time padding.
@@ -706,18 +707,21 @@
     'vtt': vtt_formatter,
     'json': json_formatter,
     'raw': raw_formatter,
 }
 
 
 def check_thread_status():
-    global thread_recognize
+    global thread_recognize, thread_timed_translate
     if thread_recognize != None:
         if thread_recognize.is_alive():
             main_window.TKroot.after(100, check_thread_status) # check again in 100 milliseconds
+    elif thread_timed_translate != None:
+        if thread_timed_translate.is_alive():
+            main_window.TKroot.after(100, check_thread_status) # check again in 100 milliseconds
     else:
         pass
 
 
 def int_or_str(text):
     """Helper function for argument parsing."""
     try:
@@ -729,32 +733,39 @@
 def callback(indata, frames, time, status):
     """This is called (from a separate thread) for each audio block."""
     if status:
         print(status, file=sys.stderr)
     q.put(bytes(indata))
 
 
-def worker_recognize(src):
-    global main_window, recognizing, text, Device, SampleRate, wav_file_name, regions, transcripts, start_button_click_time, ffmpeg_start_run_time, get_tmp_recorded_streaming_filepath_time, loading_time, first_streaming_duration_recorded
+def worker_recognize(src, dst):
+    global main_window, recognizing, text, Device, SampleRate, wav_file_name, regions, transcripts, \
+        start_button_click_time, ffmpeg_start_run_time, get_tmp_recorded_streaming_filepath_time, \
+        loading_time, first_streaming_duration_recorded
 
     p = 0
     f = 0
     l = 0
 
     start_time = None
     end_time = None
     first_streaming_duration_recorded = None
     absolute_start_time = None
 
     time_value_filename = "time_value"
     time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
+    #print("time_value_filepath = {}".format(time_value_filepath))
+    #print("os.path.isfile(time_value_filepath) = {}".format(os.path.isfile(time_value_filepath)))
     if os.path.isfile(time_value_filepath):
         time_value_file = open(time_value_filepath, "r")
         time_value_string = time_value_file.read()
-        first_streaming_duration_recorded = datetime.strptime(time_value_string, "%H:%M:%S.%f") - datetime(1900, 1, 1)
+        if time_value_string:
+            first_streaming_duration_recorded = datetime.strptime(time_value_string, "%H:%M:%S.%f") - datetime(1900, 1, 1)
+        else:
+            first_streaming_duration_recorded = None
         time_value_file.close()
 
     try:
         if SampleRate is None:
             #soundfile expects an int, sounddevice provides a float:
             device_info = sd.query_devices(Device, "input")
             SampleRate = int(device_info["default_samplerate"])
@@ -763,36 +774,42 @@
             dump_fn = open(wav_file_name, "wb")
         else:
             dump_fn = None
 
         model = Model(lang = src)
 
         with sd.RawInputStream(samplerate=SampleRate, blocksize=8000, device=Device, dtype="int16", channels=1, callback=callback):
+
             rec = KaldiRecognizer(model, SampleRate)
 
             while recognizing:
                 if not recognizing:
                     rec = None
                     data = None
                     result = None
                     results_text = None
                     partial_results_text = None
-                    print("BREAK")
+                    #print("BREAK")
                     break
 
                 data = q.get()
+
                 results_text = ''
                 partial_results_text = ''
 
                 if rec.AcceptWaveform(data):
+
                     result = json.loads(rec.Result())
+
                     if result["text"] and absolute_start_time:
+
                         text = result["text"]
+
                         if len(text) > 0:
-                            main_window.write_event_value('-EVENT-VOICE-RECOGNIZED-', text)
+                            main_window.write_event_value('-EVENT-RESULTS-', text)
                             transcripts.append(text)
 
                             f += 1
                             p = 0
 
                             absolute_end_time = datetime.now()
                             end_time = start_time + (absolute_end_time - absolute_start_time)
@@ -812,40 +829,66 @@
                                 (end_time.seconds // 60) % 60,  # minutes
                                 end_time.seconds % 60, # seconds
                                 end_time.microseconds / 1000000  # microseconds
                             )
 
                             time_stamp_string = start_time_str + "-" + end_time_str
 
-                            src_tmp_txt_transcription_filename = "record.txt"
-                            src_tmp_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), src_tmp_txt_transcription_filename)
-                            src_tmp_txt_transcription_file = open(src_tmp_txt_transcription_filepath, "a")
-                            src_tmp_txt_transcription_file.write(time_stamp_string + " " + text + "\n")
-                            src_tmp_txt_transcription_file.close()
+                            tmp_src_txt_transcription_filename = "record.txt"
+                            tmp_src_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), tmp_src_txt_transcription_filename)
+                            tmp_src_txt_transcription_file = open(tmp_src_txt_transcription_filepath, "a")
+                            tmp_src_txt_transcription_file.write(time_stamp_string + " " + text + "\n")
+                            tmp_src_txt_transcription_file.close()
 
                 else:
+
                     result = json.loads(rec.PartialResult())
+
                     if result["partial"]:
+
                         text = result["partial"]
+
+                        if len(text) == 0:
+                            print("len(text) == 0")
+                            main_window.write_event_value('-EVENT-NULL-RESULTS-', text)
+
                         if len(text)>0:
-                            main_window.write_event_value('-EVENT-VOICE-RECOGNIZED-', text)
+                            main_window.write_event_value('-EVENT-PARTIAL-RESULTS-', text)
 
                             if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
+
                                 if ffmpeg_start_run_time and l == 0:
 
                                     loading_time = datetime.now() - ffmpeg_start_run_time - (ffmpeg_start_run_time - get_tmp_recorded_streaming_filepath_time)
                                     if first_streaming_duration_recorded:
 
-                                        # A ROUGH GUESS OF THE FIRST PARTIAL RESULT START TIME :)
-                                        start_time = first_streaming_duration_recorded + loading_time
-                                        #start_time = first_streaming_duration_recorded + timedelta(seconds=1)
+                                        # A ROUGH GUESS OF THE FIRST PARTIAL RESULT START TIME
+                                        # USING PyAutoSRT IS THE ONLY OPTION TO GET ACCURATE SUBTITLE SYNC
+
+                                        #start_time = first_streaming_duration_recorded + loading_time
+                                        #start_time = first_streaming_duration_recorded
+                                        start_time = first_streaming_duration_recorded + timedelta(seconds=0.7)
 
                                         # MAKE SURE THAT IT'S EXECUTED ONLY ONCE
                                         l += 1
 
+                                    else:
+                                        time_value_filename = "time_value"
+                                        time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
+                                        #print("time_value_filepath = {}".format(time_value_filepath))
+                                        #print("os.path.isfile(time_value_filepath) = {}".format(os.path.isfile(time_value_filepath)))
+                                        if os.path.isfile(time_value_filepath):
+                                            time_value_file = open(time_value_filepath, "r")
+                                            time_value_string = time_value_file.read()
+                                            if time_value_string:
+                                                first_streaming_duration_recorded = datetime.strptime(time_value_string, "%H:%M:%S.%f") - datetime(1900, 1, 1)
+                                            else:
+                                                first_streaming_duration_recorded = None
+                                            time_value_file.close()
+
                                 else:
                                     if p == 0:
                                         absolute_start_time = datetime.now()
 
                                         if end_time:
                                             start_time = end_time
                                         p += 1
@@ -864,24 +907,27 @@
                                         if end_time:
                                             start_time = end_time
                                         p += 1
 
                 if dump_fn is not None:
                     dump_fn.write(data)
 
+
+
     except KeyboardInterrupt:
         recognizing==False
         rec = None
         data = None
         parser.exit(0)
 
     except Exception as e:
         parser.exit(type(e).__name__ + ": " + str(e))
 
 
+'''
 class TranscriptionTranslator(object):
     def __init__(self, src, dst, patience=-1):
         self.src = src
         self.dst = dst
         self.patience = patience
 
     def __call__(self, sentence):
@@ -898,48 +944,97 @@
             if translated_sentence[-1] == '\n':
                 if patience == -1:
                     continue
                 patience -= 1
             else:
                 fail_to_translate = False
         return translated_sentence
+'''
 
 
 def GoogleTranslate(text, src, dst):
     url = 'https://translate.googleapis.com/translate_a/'
     params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
     with httpx.Client(http2=True) as client:
         client.headers.update({'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',})
         response = client.get(url+params)
-        #print('response.status_code = {}'.format(response.status_code))
+        #print("response.status_code = {}".format(response.status_code))
         if response.status_code == 200:
             response_json = response.json()[0]
-            #print('response_json = {}'.format(response_json))
+            #print("response_json = {}".format(response_json))
             if response_json!= None:
                 length = len(response_json)
-                #print('length = {}'.format(length))
+                #print("length = {}".format(length))
                 translation = ""
                 for i in range(length):
                     #print("{} {}".format(i, response_json[i][0]))
                     translation = translation + response_json[i][0]
                 return translation
         return
 
 
 def worker_timed_translate(src, dst):
     global main_window, recognizing
 
     while (recognizing==True):
-        phrase = str(main_window['-ML1-'].get())
-        if len(phrase)>0:
-            translated_text = GoogleTranslate(phrase, src, dst)
-            main_window.write_event_value('-EVENT-VOICE-TRANSLATED-', translated_text)
-
         if not recognizing:
             break
+        #phrase = str(main_window['-ML-SRC-PARTIAL-RESULTS-'].get())
+        partial_result_filename = "partial_result"
+        partial_result_filepath = os.path.join(tempfile.gettempdir(), partial_result_filename)
+        if os.path.isfile(partial_result_filepath):
+            partial_result_file = open(partial_result_filepath, "r")
+            partial_result = partial_result_file.read()
+
+            n_words = len(partial_result.split())
+            if partial_result and n_words % 3 == 0:
+                translated_text = GoogleTranslate(partial_result, src, dst)
+                main_window.write_event_value('-EVENT-VOICE-TRANSLATED-', translated_text)
+
+
+def stop_thread2(thread):
+    exc = ctypes.py_object(SystemExit)
+    res = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(thread.ident), exc)
+    if res == 0:
+        raise ValueError("nonexistent thread id")
+    elif res > 1:
+        # """if it returns a number greater than one, you're in trouble,
+        # and you should call it again with exc=NULL to revert the effect"""
+        ctypes.pythonapi.PyThreadState_SetAsyncExc(thread.ident, None)
+        raise SystemError("PyThreadState_SetAsyncExc failed")
+
+
+def stop_thread(thread):
+    if thread and thread.is_alive():
+        if sys.platform == "win32":
+            # Use ctypes to call the TerminateThread() function from the Windows API
+            # This forcibly terminates the thread, which can be unsafe in some cases
+            kernel32 = ctypes.windll.kernel32
+            thread_handle = kernel32.OpenThread(1, False, thread.ident)
+            if thread_handle:
+                ret = kernel32.TerminateThread(thread_handle, 0)
+                if ret == 0:
+                    msg = thread.name + "TERMINATION ERROR!"
+                else:
+                    msg = thread.name + "TERMINATED"
+                    thread = None
+                #print(msg)
+        elif sys.platform == "linux":
+            exc = ctypes.py_object(SystemExit)
+            res = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(thread.ident), exc)
+            if res == 0:
+                raise ValueError("nonexistent thread id")
+            elif res > 1:
+                # """if it returns a number greater than one, you're in trouble,
+                # and you should call it again with exc=NULL to revert the effect"""
+                ctypes.pythonapi.PyThreadState_SetAsyncExc(thread.ident, None)
+                raise SystemError("PyThreadState_SetAsyncExc failed")
+
+    else:
+        return
 
 
 def is_streaming_url(url):
 
     streamlink = Streamlink()
 
     if is_valid_url(url):
@@ -1045,15 +1140,15 @@
                 main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
 
     process.wait()
 
 
 # subprocess.Popen(ffmpeg_cmd) THREAD BEHAVIOR IS DIFFERENT IN LINUX
 def record_streaming_linux(url, output_file):
-    global ffmpeg_start_run_time, first_streaming_duration_recorded
+    global recognizing, ffmpeg_start_run_time, first_streaming_duration_recorded
 
     #ffmpeg_cmd = ['ffmpeg', '-y', '-i', url, '-c', 'copy', '-bsf:a', 'aac_adtstoasc', '-f', 'mp4', output_file]
     ffmpeg_cmd = ['ffmpeg', '-y', '-i', f'{url}',  '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov', '-fflags', 'nobuffer', f'{output_file}']
 
     ffmpeg_start_run_time = datetime.now()
     #first_streaming_duration_recorded = None
 
@@ -1069,15 +1164,15 @@
 
         # Set up a timer to periodically check for new output
         timeout = 1.0
         timer = threading.Timer(timeout, lambda: None)
         timer.start()
 
         # Read output from ffmpeg process
-        while True:
+        while recognizing:
             # Check if the process has finished
             if process.poll() is not None:
                 break
 
             # Check if there is new output to read, special for linux
             rlist, _, _ = select.select([process.stderr], [], [], timeout)
             if not rlist:
@@ -1100,85 +1195,43 @@
 
                     first_streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
                     #print("first_streaming_duration_recorded = {}".format(first_streaming_duration_recorded))
 
                     # MAKE SURE THAT first_streaming_duration_recorded EXECUTED ONLY ONCE
                     i += 1
 
+                    #print("writing time_value")
                     time_value_filename = "time_value"
                     time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
                     time_value_file = open(time_value_filepath, "w")
                     time_value_file.write(str(time_value))
                     time_value_file.close()
+                    #print("time_value = {}".format(time_value))
 
                 streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
                 #print("streaming_duration_recorded = {}".format(streaming_duration_recorded))
                 main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
 
             # Restart the timer to check for new output
             timer.cancel()
             timer = threading.Timer(timeout, lambda: None)
-            timer.start()
+            if recognizing: timer.start()
 
         # Close the ffmpeg process and print the return code
         process.stdout.close()
         process.stderr.close()
-        #print(f"FFmpeg exited with return code {process.returncode}")
 
     # Start the thread to run ffmpeg
     thread = threading.Thread(target=run_ffmpeg)
-    thread.start()
+    if recognizing: thread.start()
 
     # Return the thread object so that the caller can join it if needed
     return thread
 
 
-def stop_thread(thread):
-    if thread and thread.is_alive():
-        if platform.system() == 'Windows':
-            # Use ctypes to call the TerminateThread() function from the Windows API
-            # This forcibly terminates the thread, which can be unsafe in some cases
-            kernel32 = ctypes.windll.kernel32
-            thread_handle = kernel32.OpenThread(1, False, thread.ident)
-            if thread_handle:
-                ret = kernel32.TerminateThread(thread_handle, 0)
-                if ret == 0:
-                    msg = thread.name + "TERMINATION ERROR!"
-                else:
-                    msg = thread.name + "TERMINATED"
-                    thread = None
-                #print(msg)
-        elif platform.system() == 'Linux':
-            libpthread = ctypes.CDLL('libpthread.so.0')
-            thread_id = thread.ident
-            if thread_id:
-                print('thread_id = {}'.format(thread_id))
-                ret = libpthread.pthread_cancel(thread_id)
-                if ret == 0:
-                    msg = thread.name + "TERMINATION ERROR!"
-                else:
-                    msg = thread.name + "TERMINATED"
-                    thread = None
-                #print(msg)
-
-
-def stop_record_streaming_linux():
-    global main_window
-
-    msg = "TERMINATED"
-    main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
-
-    ffmpeg_pid = subprocess.check_output(['pgrep', '-f', 'ffmpeg']).strip()
-    if ffmpeg_pid:
-        subprocess.Popen(['kill', ffmpeg_pid])
-    else:
-        msg = 'FFMPEG HAS TERMINATED'
-        main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
-
-
 def stop_record_streaming_windows():
     global main_window, thread_record_streaming
 
     if thread_record_streaming and thread_record_streaming.is_alive():
         # Use ctypes to call the TerminateThread() function from the Windows API
         # This forcibly terminates the thread, which can be unsafe in some cases
         kernel32 = ctypes.windll.kernel32
@@ -1188,48 +1241,73 @@
             msg = "TERMINATION ERROR!"
         else:
             msg = "TERMINATED"
             thread_record_streaming = None
         main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
 
         tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
-
         ffmpeg_pid = None
         for line in tasklist_output.split('\n'):
-            if 'ffmpeg' in line:
+            if "ffmpeg" in line:
                 ffmpeg_pid = line.split()[1]
                 break
         if ffmpeg_pid:
             devnull = open(os.devnull, 'w')
             subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=devnull, stderr=devnull, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
             msg = 'FFMPEG HAS TERMINATED'
             main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
 
     else:
         msg = "NOT RUNNING"
         main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
 
 
+def stop_record_streaming_linux():
+    global main_window, thread_record_streaming
+
+    if thread_record_streaming and thread_record_streaming.is_alive():
+        print("thread_record_streaming.is_alive()")
+        exc = ctypes.py_object(SystemExit)
+        res = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(thread_record_streaming.ident), exc)
+        if res == 0:
+            raise ValueError("nonexistent thread id")
+        elif res > 1:
+            # """if it returns a number greater than one, you're in trouble,
+            # and you should call it again with exc=NULL to revert the effect"""
+            ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_record_streaming.ident, None)
+            raise SystemError("PyThreadState_SetAsyncExc failed")
+
+    msg = "TERMINATED"
+    if main_window: main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
+
+    ffmpeg_pid = subprocess.check_output(['pgrep', '-f', 'ffmpeg']).strip()
+    if ffmpeg_pid:
+        subprocess.Popen(['kill', ffmpeg_pid])
+    else:
+        msg = 'FFMPEG HAS TERMINATED'
+        if main_window: main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
+
+
 #-------------------------------------------------------------GUI FUNCTIONS-------------------------------------------------------------#
 
 
 def handle_focus(event):
     if event.widget == window:
         window.focus_set()
 
 
 def steal_focus():
     global main_window, overlay_translation_window
 
-    #print('debug')
+    #print("debug")
     if overlay_translation_window:
         overlay_translation_window.close()
         overlay_translation_window=None
-    if(platform.system() == "Windows"):
+    if(sys.platform == "win32"):
         main_window.TKroot.attributes('-topmost', True)
         main_window.TKroot.attributes('-topmost', False)
         main_window.TKroot.deiconify()
     if(sys.platform == "linux"):
         #main_window.TKroot.attributes('-topmost', 1)
         #main_window.TKroot.attributes('-topmost', 0)
         #main_window.TKroot.deiconify()
@@ -1258,34 +1336,34 @@
 
 
 def make_overlay_translation_window(translated_text):
     xmax, ymax = sg.Window.get_screen_size()
     max_columns = None
     max_lines = None
 
-    if platform.system() == 'Windows':
+    if sys.platform == "win32":
         SM_CXSCREEN = 0
         SM_CYSCREEN = 1
         width = ctypes.windll.user32.GetSystemMetrics(SM_CXSCREEN)
         height = ctypes.windll.user32.GetSystemMetrics(SM_CYSCREEN)
 
         max_columns = int(width/8.5)
         max_lines = int(height/18)
 
-    elif platform.system() == 'Linux':
+    elif sys.platform == "linux":
         output = subprocess.check_output(['xrandr'])
         primary_line = [line for line in output.decode().splitlines() if ' connected primary' in line][0]
         primary_size = primary_line.split()[3].replace("+"," ").split()[0]
 
         max_columns, max_lines = int(primary_size.split('x')[0]) // 8, int(primary_size.split('x')[1]) // 18
 
     columns = max_columns
     rows = max_lines
 
-    FONT_TYPE = 'Arial'
+    FONT_TYPE = 'Helvetica'
     FONT_SIZE = 16
 
     if len(translated_text)<=96:
         window_width = int(9.9*(xmax/1280)*len(translated_text) + 60)
         #window_width = font_length(translated_text, FONT_TYPE, FONT_SIZE)
     else:
         window_width=int(960*xmax/1280)
@@ -1312,55 +1390,80 @@
     sg.set_options(font=("Arial", FONT_SIZE))
 
     multiline_width = len(translated_text)
     multiline_height = nl
 
     TRANSPARENT_BLACK='#add123'
 
-    if not (platform.system() == "Windows"):
-        layout = [[sg.Multiline(default_text=translated_text, size=(multiline_width, multiline_height), text_color='yellow1', border_width=0,
-            background_color='black', no_scrollbar=True,
-            justification='l', expand_x=True, expand_y=True,  key='-ML-LS2-')]]
-
-        overlay_translation_window = sg.Window('text', layout, no_titlebar=True, keep_on_top=True, size=(window_width,window_height), location=(window_x,window_y), 
-            margins=(0, 0), background_color='black', alpha_channel=0.7, return_keyboard_events=True, finalize=True)
+    if not (sys.platform == "win32"):
+        layout = [[sg.Multiline(default_text=translated_text, size=(multiline_width, multiline_height), text_color='yellow1',
+            border_width=0, background_color='black', no_scrollbar=True, justification='l', expand_x=True, expand_y=True,
+            key='-ML-OVERLAY-DST-PARTIAL-RESULTS-')]]
+
+        overlay_translation_window = sg.Window('text', layout, no_titlebar=True, keep_on_top=True,
+            size=(window_width,window_height), location=(window_x,window_y), margins=(0, 0), background_color='black',
+            alpha_channel=0.7, return_keyboard_events=True, finalize=True)
 
         overlay_translation_window.TKroot.attributes('-type', 'splash')
         overlay_translation_window.TKroot.attributes('-topmost', 1)
         #overlay_translation_window.TKroot.attributes('-topmost', 0)
     else:
-        layout = [[sg.Multiline(default_text=translated_text, size=(multiline_width, multiline_height), text_color='yellow1', border_width=0,
-            background_color='white', no_scrollbar=True,
-            justification='l', expand_x=True, expand_y=True,  key='-ML-LS2-')]]
-
-        overlay_translation_window = sg.Window('Translation', layout, no_titlebar=True, keep_on_top=True, size=(window_width,window_height), location=(window_x,window_y), 
-            margins=(0, 0), background_color='white', transparent_color='white', grab_anywhere=True, return_keyboard_events=True, 
-            finalize=True)
+        layout = [[sg.Multiline(default_text=translated_text, size=(multiline_width, multiline_height), text_color='yellow1',
+            border_width=0, background_color='white', no_scrollbar=True, justification='l', expand_x=True, expand_y=True,
+            key='-ML-OVERLAY-DST-PARTIAL-RESULTS-')]]
+
+        overlay_translation_window = sg.Window('Translation', layout, no_titlebar=True, keep_on_top=True,
+            size=(window_width,window_height), location=(window_x,window_y), margins=(0, 0), background_color='white',
+            transparent_color='white', grab_anywhere=True, return_keyboard_events=True, finalize=True)
 
     #event, values = overlay_translation_window.read(timeout=TIMEOUT, close=True)
     event, values = overlay_translation_window.read(500)
 
     return overlay_translation_window
 
 
 def move_center(window):
     screen_width, screen_height = window.get_screen_dimensions()
     win_width, win_height = window.size
     x, y = (screen_width - win_width)//2, (screen_height - win_height)//2-30
     window.move(x, y)
 
 
+def get_clipboard_text():
+    return subprocess.check_output(['xclip', '-selection', 'clipboard', '-out']).decode()
+
+
+def set_clipboard_text(text):
+    subprocess.run(['xclip', '-selection', 'clipboard'], input=text.encode())
+
+
+
 #=============================================================MAIN PROGRAM=============================================================#
 
 def main():
     global main_window, thread_recognize, thread_timed_translate, thread_record_streaming, text, recognizing, \
         Device, SampleRate, wav_file_name, tmp_recorded_streaming_filepath, regions, transcripts, \
         start_button_click_time, ffmpeg_start_run_time, get_tmp_recorded_streaming_filepath_time, \
         first_streaming_duration_recorded, is_valid_url_streaming, stop_event
 
+    if sys.platform == "win32":
+        user32 = ctypes.windll.user32
+        kernel32 = ctypes.windll.kernel32
+        kernel32.GlobalLock.argtypes = [ctypes.wintypes.HGLOBAL]
+        kernel32.GlobalLock.restype = ctypes.wintypes.LPVOID
+        kernel32.GlobalSize.argtypes = [ctypes.wintypes.HGLOBAL]
+        kernel32.GlobalSize.restype = ctypes.c_size_t
+        user32.OpenClipboard.argtypes = [ctypes.wintypes.HWND]
+        user32.OpenClipboard.restype = ctypes.wintypes.BOOL
+        user32.CloseClipboard.argtypes = []
+        user32.CloseClipboard.restype = ctypes.wintypes.BOOL
+        user32.GetClipboardData.argtypes = [ctypes.wintypes.UINT]
+        user32.GetClipboardData.restype = ctypes.wintypes.HANDLE
+
+
 #--------------------------------------------------------------GUI PARTS--------------------------------------------------------------#
 
     xmax, ymax = sg.Window.get_screen_size()
     main_window_width = int(0.5*xmax)
     main_window_height = int(0.5*ymax)
     multiline_width = int(0.15*main_window_width)
     multiline_height = int(0.0125*main_window_height)
@@ -1371,34 +1474,36 @@
     layout = [[sg.Frame('Hints',[
                                 [sg.Text('Click \"Start\" button to start listening and printing subtitles on screen.', expand_x=True, expand_y=True)],
                                 [sg.Text('Paste the streaming URL into URL inputbox then check the \"Record Streaming\" checkbox to record the streaming.', expand_x=True, expand_y=True)],
                                 [sg.Text('If you record the streaming, when you save transcriptions, all timestamps will be relative to the \"Start\" button clicked time.', expand_x=True, expand_y=True)],
                                 [sg.Text('If you don\'t record the streaming, all timestamps will be based on your system clock.', expand_x=True, expand_y=True)],
                                 [sg.Text('If you need accurate subtitles sync for the video, please use PyAutoSRT (https://github.com/botbahlul/PyAutoSRT) ', expand_x=True, expand_y=True, enable_events=True)],
                                 ], border_width=2, expand_x=True, expand_y=True)],
-              [sg.Text('URL'), sg.Input(size=(12, 1), expand_x=True, expand_y=True, key='-URL-'),
+              [sg.Text('URL'), sg.Input(size=(12, 1), expand_x=True, expand_y=True, key='-URL-', enable_events=True, right_click_menu=['&Edit', ['&Paste',]]),
                sg.Checkbox("Record Streaming", key='-RECORD-STREAMING-', enable_events=True)],
               [sg.Text('', size=(3, 1)),
                sg.Text('Thread status'),
                sg.Text('NOT RUNNING', size=(24, 1), background_color='green1', text_color='black', expand_x=True, expand_y=True, key='-RECORD-STREAMING-STATUS-'),
                sg.Text('Duration recorded', size=(16, 1)),
                sg.Text('0:00:00.000000', size=(9, 1), background_color='green1', text_color='black', expand_x=True, expand_y=True, key='-STREAMING-DURATION-RECORDED-'),
                sg.Text('', size=(14, 1), expand_x=True, expand_y=True)],
               [sg.Text('', expand_x=True, expand_y=True),
                sg.Button('SAVE RECORDED STREAMING', size=(31,1), expand_x=True, expand_y=True, key='-EVENT-SAVE-RECORDED-STREAMING-'),
                sg.Text('', expand_x=True, expand_y=True)],
               [sg.Text('Audio language', size=(12, 1), expand_x=True, expand_y=True),
                sg.Combo(list(map_src_of_language), size=(int(0.2*multiline_width), 1), default_value="English", expand_x=True, expand_y=True, key='-SRC-')],
-              [sg.Multiline(size=(multiline_width, multiline_height), expand_x=True, expand_y=True, key='-ML1-')],
+              [sg.Multiline(size=(multiline_width, multiline_height), expand_x=True, expand_y=True, key='-ML-SRC-RESULTS-')],
+              [sg.Multiline(size=(multiline_width, 0.5*multiline_height), expand_x=True, expand_y=True, key='-ML-SRC-PARTIAL-RESULTS-')],
               [sg.Text('', expand_x=True, expand_y=True),
                sg.Button('SAVE TRANSCRIPTION', size=(31,1), expand_x=True, expand_y=True, key='-EVENT-SAVE-SRC-TRANSCRIPTION-'),
                sg.Text('', expand_x=True, expand_y=True)],
               [sg.Text('Translation language', size=(12, 1),expand_x=True, expand_y=True),
                sg.Combo(list(map_dst_of_language), size=(int(0.2*multiline_width), 1), default_value="Indonesian", expand_x=True, expand_y=True, key='-DST-')],
-              [sg.Multiline(size=(multiline_width, multiline_height), expand_x=True, expand_y=True, key='-ML2-')],
+              [sg.Multiline(size=(multiline_width, multiline_height), expand_x=True, expand_y=True, key='-ML-DST-RESULTS-')],
+              [sg.Multiline(size=(multiline_width, 0.5*multiline_height), expand_x=True, expand_y=True, key='-ML-DST-PARTIAL-RESULTS-')],
               [sg.Text('', expand_x=True, expand_y=True, key='-SPACES3-'),
                sg.Button('SAVE TRANSLATED TRANSCRIPTION', size=(31,1), expand_x=True, expand_y=True, key='-EVENT-SAVE-DST-TRANSCRIPTION-'),
                sg.Text('', expand_x=True, expand_y=True, key='-SPACES4-')],
               [sg.Button('Start', expand_x=True, expand_y=True, button_color=('white', '#283b5b'), key='-START-BUTTON-'),
                sg.Button('Exit', expand_x=True, expand_y=True)]]
 
 
@@ -1427,14 +1532,22 @@
     tmp_recorded_streaming_filename = "record.mp4"
     tmp_recorded_streaming_filepath = os.path.join(tempfile.gettempdir(), tmp_recorded_streaming_filename)
     if os.path.isfile(tmp_recorded_streaming_filepath):
         os.remove(tmp_recorded_streaming_filepath)
 
     saved_recorded_streaming_filename = None
 
+    partial_result_filename = "partial_result"
+    partial_result_filepath = os.path.join(tempfile.gettempdir(), partial_result_filename)
+    if os.path.isfile(partial_result_filepath): os.remove(partial_result_filepath)
+
+    time_value_filename = "time_value"
+    time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
+    if os.path.isfile(time_value_filepath): os.remove(time_value_filepath)
+
     subtitle_file_types = [
         ('SRT Files', '*.srt'),
         ('VTT Files', '*.vtt'),
         ('JSON Files', '*.json'),
         ('RAW Files', '*.raw'),
         ('Text Files', '*.txt'),
         ('All Files', '*.*'),
@@ -1447,26 +1560,29 @@
         'raw': raw_formatter,
     }
 
     video_file_types = [
         ('MP4 Files', '*.mp4'),
     ]
 
-    src_tmp_txt_transcription_filename = "record.txt"
-    src_tmp_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), src_tmp_txt_transcription_filename)
-    if os.path.isfile(src_tmp_txt_transcription_filepath):
-        os.remove(src_tmp_txt_transcription_filepath)
-
-    dst_tmp_txt_transcription_filename = "record.translated.txt"
-    dst_tmp_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), dst_tmp_txt_transcription_filename)
-    if os.path.isfile(dst_tmp_txt_transcription_filepath):
-        os.remove(dst_tmp_txt_transcription_filepath)
-
-    tmp_src_subtitle_filepath = None
-    tmp_dst_subtitle_filepath = None
+    tmp_src_txt_transcription_filename = "record.txt"
+    tmp_src_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), tmp_src_txt_transcription_filename)
+    if os.path.isfile(tmp_src_txt_transcription_filepath): os.remove(tmp_src_txt_transcription_filepath)
+
+    tmp_dst_txt_transcription_filename = "record.translated.txt"
+    tmp_dst_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), tmp_dst_txt_transcription_filename)
+    if os.path.isfile(tmp_dst_txt_transcription_filepath): os.remove(tmp_dst_txt_transcription_filepath)
+
+    tmp_src_subtitle_filename = "record.srt"
+    tmp_src_subtitle_filepath = os.path.join(tempfile.gettempdir(), tmp_src_subtitle_filename)
+    if os.path.isfile(tmp_src_subtitle_filepath): os.remove(tmp_src_subtitle_filepath)
+
+    tmp_dst_subtitle_filename = "record.translated.srt"
+    tmp_dst_subtitle_filepath = os.path.join(tempfile.gettempdir(), tmp_dst_subtitle_filename)
+    if os.path.isfile(tmp_dst_subtitle_filepath): os.remove(tmp_dst_subtitle_filepath)
 
     saved_src_subtitle_filename = None
     saved_dst_subtitle_filename = None
 
     ffmpeg_start_run_time = None
 
     parser = argparse.ArgumentParser(add_help=False)
@@ -1497,15 +1613,15 @@
         parser.exit(0)
 
     parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter, parents=[parser])
 
     parser.add_argument("-af", "--audio-filename", type=str, metavar="AUDIO_FILENAME", help="audio file to store recording to")
     parser.add_argument("-d", "--device", type=int_or_str, help="input device (numeric ID or substring)")
     parser.add_argument("-r", "--samplerate", type=int, help="sampling rate in Hertz for example 8000, 16000, 44100, or 48000")
-    parser.add_argument('-v', '--version', action='version', version='0.1.2')
+    parser.add_argument('-v', '--version', action='version', version='0.1.3')
 
     parser.add_argument("-u", "--url", type=str, metavar="URL", help="URL of live streaming if you want to record the streaming")
     parser.add_argument("-vf", "--video-filename", type=str, metavar="VIDEO_FILENAME", help="video file to store recording to", default=None)
 
     args = parser.parse_args(remaining)
     args = parser.parse_args()
 
@@ -1572,20 +1688,20 @@
 
 #-------------------------------------REMAINING GUI PARTS NEEDED TO LOAD AT LAST BEFORE MAIN LOOP-------------------------------------#
 
 
     main_window = sg.Window('VOSK Live Subtitles', layout, resizable=True, keep_on_top=True, finalize=True)
     main_window['-SRC-'].block_focus()
 
-    if (platform.system() == "Windows"):
+    if (sys.platform == "win32"):
         if main_window.TKroot is not None:
             main_window.TKroot.attributes('-topmost', True)
             main_window.TKroot.attributes('-topmost', False)
 
-    if not (platform.system() == "Windows"):
+    if not (sys.platform == "win32"):
         if main_window.TKroot is not None:
             main_window.TKroot.attributes('-topmost', 1)
             main_window.TKroot.attributes('-topmost', 0)
 
     main_window.finalize()
     overlay_translation_window = None
     move_center(main_window)
@@ -1602,65 +1718,127 @@
         is_valid_url_streaming = is_streaming_url(args.url)
         #print("is_valid_url_streaming = {}".format(is_valid_url_streaming))
         if is_valid_url_streaming:
             url = args.url
             main_window['-URL-'].update(url)
             main_window['-RECORD-STREAMING-'].update(True)
 
+    main_window['-ML-SRC-PARTIAL-RESULTS-'].update("")
+    main_window['-ML-SRC-RESULTS-'].update("")
+    main_window['-ML-DST-PARTIAL-RESULTS-'].update("")
+    main_window['-ML-DST-RESULTS-'].update("")
+
 
 #---------------------------------------------------------------MAIN LOOP--------------------------------------------------------------#
 
 
     while True:
         window, event, values = sg.read_all_windows(500)
 
-        #print('event =', event)
-        #print('recognizing =', recognizing)
+        #print("event = {}".format(event))
+        #print("recognizing = {}".format(recognizing))
 
         src = map_src_of_language[str(main_window['-SRC-'].get())]
         last_selected_src = src
         src_file = open(src_filepath, "w")
         src_file.write(src)
         src_file.close()
 
         dst = map_dst_of_language[str(main_window['-DST-'].get())]
         last_selected_dst = dst
         dst_file = open(dst_filepath, "w")
         dst_file.write(dst)
         dst_file.close()
 
+
         if event == 'Exit' or event == sg.WIN_CLOSED:
+
+            if recognizing:
+                recognizing = False
+
+                if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
+                    if sys.platform == "win32":
+                        stop_record_streaming_windows()
+                    elif sys.platform == "linux":
+                        stop_record_streaming_linux()
+
+                text = ""
+                translated_text = ""
+
+                if overlay_translation_window:
+                    overlay_translation_window.close()
+                    overlay_translation_window = None
+
             break
 
 
+        elif event.endswith('+R') and values['-URL-']:
+
+            if sys.platform == "win32":
+                user32.OpenClipboard(None)
+                clipboard_data = user32.GetClipboardData(1)  # 1 is CF_TEXT
+                if clipboard_data:
+                    data = ctypes.c_char_p(clipboard_data)
+                    main_window['-URL-'].update(data.value.decode('utf-8'))
+                user32.CloseClipboard()
+            elif sys.platform == "linux":
+                text = get_clipboard_text()
+                if text:
+                    main_window['-URL-'].update(text.strip())
+
+
+        elif event == 'Paste':
+
+            if sys.platform == "win32":
+                user32.OpenClipboard(None)
+                clipboard_data = user32.GetClipboardData(1)  # 1 is CF_TEXT
+                if clipboard_data:
+                    data = ctypes.c_char_p(clipboard_data)
+                    main_window['-URL-'].update(data.value.decode('utf-8'))
+                user32.CloseClipboard()
+            elif sys.platform == "linux":
+                text = get_clipboard_text()
+                if text:
+                    main_window['-URL-'].update(text.strip())
+
+
         elif event == '-RECORD-STREAMING-':
+
             if values['-RECORD-STREAMING-']:
                 is_valid_url_streaming = is_streaming_url(str(values['-URL-']).strip())
                 if not is_valid_url_streaming:
                     FONT_TYPE = "Helvetica"
                     FONT_SIZE = 9
                     sg.set_options(font=(FONT_TYPE, FONT_SIZE))
                     sg.Popup('Invalid URL, please enter a valid URL.                   ', title="Info")
                     main_window['-RECORD-STREAMING-'].update(False)
 
 
         elif event == '-START-BUTTON-':
             recognizing = not recognizing
-            #print('Start button clicked, changing recognizing status')
-            #print('recognizing =', recognizing)
+            #print("Start button clicked, changing recognizing status")
+            #print("recognizing = {}".format(recognizing))
 
             main_window['-START-BUTTON-'].update(('Stop','Start')[not recognizing], button_color=(('white', ('red', '#283b5b')[not recognizing])))
 
             if recognizing:
-                #print('VOSK Live Subtitle is START LISTENING now')
-                #print('recognizing =', recognizing)
+                #print("VOSK Live Subtitle is START LISTENING now")
+                #print("recognizing = {}".format(recognizing))
 
                 start_button_click_time = datetime.now()
                 #print("start_button_click_time = {}".format(start_button_click_time))
 
+                if tmp_recorded_streaming_filepath and os.path.isfile(tmp_recorded_streaming_filepath): os.remove(tmp_recorded_streaming_filepath)
+                if partial_result_filepath and os.path.isfile(partial_result_filepath): os.remove(partial_result_filepath)
+                if time_value_filepath and os.path.isfile(time_value_filepath): os.remove(time_value_filepath)
+                if tmp_src_subtitle_filepath and os.path.isfile(tmp_src_subtitle_filepath): os.remove(tmp_src_subtitle_filepath)
+                if tmp_dst_subtitle_filepath and os.path.isfile(tmp_dst_subtitle_filepath): os.remove(tmp_dst_subtitle_filepath)
+                if tmp_src_txt_transcription_filepath and os.path.isfile(tmp_src_txt_transcription_filepath): os.remove(tmp_src_txt_transcription_filepath)
+                if tmp_dst_txt_transcription_filepath and os.path.isfile(tmp_dst_txt_transcription_filepath): os.remove(tmp_dst_txt_transcription_filepath)
+
                 if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
 
                     if is_valid_url_streaming:
 
                         url = values['-URL-']
 
                         tmp_recorded_streaming_filename = "record.mp4"
@@ -1675,88 +1853,87 @@
                         os.environ['STREAMLINK_PLUGIN_DIR'] = './streamlink/plugins/'
 
                         streamlink = Streamlink()
                         streams = streamlink.streams(url)
                         stream_url = streams['360p']
 
                         # WINDOWS AND LINUX HAS DIFFERENT BEHAVIOR WHEN RUNNING FFMPEG AS THREAD
-                        if platform.system() == "Windows":
+                        # EVEN thread_record_streaming WS DECLARED FIRST, IT ALWAYS GET LOADED AT LAST
+                        if sys.platform == "win32":
                             thread_record_streaming = threading.Thread(target=record_streaming_windows, args=(stream_url.url, tmp_recorded_streaming_filepath), daemon=True)
                             thread_record_streaming.start()
 
-                        elif platform.system() == "Linux":
+                        elif sys.platform == "linux":
                             thread_record_streaming = threading.Thread(target=record_streaming_linux, args=(stream_url.url, tmp_recorded_streaming_filepath))
                             thread_record_streaming.start()
 
                     else:
                         FONT_TYPE = "Helvetica"
                         FONT_SIZE = 9
                         sg.set_options(font=(FONT_TYPE, FONT_SIZE))
                         sg.Popup('Invalid URL, please enter a valid URL.                   ', title="Info")
                         recognizing = False
                         main_window['-START-BUTTON-'].update(('Stop','Start')[not recognizing], button_color=(('white', ('red', '#283b5b')[not recognizing])))
                         main_window['-RECORD-STREAMING-'].update(False)
 
-                # SHOWING OVERLAY TRANSLATION WINDOW
-                if not overlay_translation_window:
-                    overlay_translation_window = make_overlay_translation_window(100*' ')
-                    overlay_translation_window.Hide()
-
                 regions = []
                 transcripts = []
 
                 if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
                     time.sleep(1)
 
-                src_tmp_txt_transcription_filename = "record.txt"
-                src_tmp_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), src_tmp_txt_transcription_filename)
-                src_tmp_txt_transcription_file = open(src_tmp_txt_transcription_filepath, "w")
-                src_tmp_txt_transcription_file.write("")
-                src_tmp_txt_transcription_file.close()
-
-                src_tmp_txt_transcription_filename = "record.translated.txt"
-                src_tmp_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), src_tmp_txt_transcription_filename)
-                src_tmp_txt_transcription_file = open(src_tmp_txt_transcription_filepath, "w")
-                src_tmp_txt_transcription_file.write("")
-                src_tmp_txt_transcription_file.close()
+                tmp_src_txt_transcription_filename = "record.txt"
+                tmp_src_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), tmp_src_txt_transcription_filename)
+                tmp_src_txt_transcription_file = open(tmp_src_txt_transcription_filepath, "w")
+                tmp_src_txt_transcription_file.write("")
+                tmp_src_txt_transcription_file.close()
+
+                tmp_dst_txt_transcription_filename = "record.translated.txt"
+                tmp_dst_txt_transcription_filepath = os.path.join(tempfile.gettempdir(), tmp_dst_txt_transcription_filename)
+                tmp_dst_txt_transcription_file = open(tmp_src_txt_transcription_filepath, "w")
+                tmp_dst_txt_transcription_file.write("")
+                tmp_dst_txt_transcription_file.close()
+
+                main_window['-ML-SRC-PARTIAL-RESULTS-'].update("")
+                main_window['-ML-SRC-RESULTS-'].update("")
+                main_window['-ML-DST-PARTIAL-RESULTS-'].update("")
+                main_window['-ML-DST-RESULTS-'].update("")
 
-                thread_recognize = threading.Thread(target=worker_recognize, args=(src,), daemon=True)
+                thread_recognize = threading.Thread(target=worker_recognize, args=(src, dst), daemon=True)
                 thread_recognize.start()
 
-                thread_timed_translate = threading.Timer(0.2, worker_timed_translate, args=(src, dst))
-                thread_timed_translate.daemon = True
+                thread_timed_translate = threading.Thread(target=worker_timed_translate, args=(src, dst), daemon=True)
                 thread_timed_translate.start()
 
                 main_window.TKroot.after(100, check_thread_status)
 
             else:
-                #print('VOSK Live Subtitle is STOP LISTENING now')
-                #print('recognizing =', recognizing)
+                #print("VOSK Live Subtitle is STOP LISTENING now")
+                #print("recognizing = {}".format(recognizing))
 
                 if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
 
-                    if platform.system() == "Windows":
+                    if sys.platform == "win32":
                         #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
                         stop_record_streaming_windows()
 
-                    elif platform.system() == "Linux":
+                    elif sys.platform == "linux":
                         #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
                         stop_record_streaming_linux()
 
-                text=''
-                main_window['-ML1-'].update(text, background_color_for_value='yellow1', autoscroll=True)
-                translated_text=''
-                main_window['-ML2-'].update(translated_text, background_color_for_value='yellow1', autoscroll=True)
+                text = ""
+                main_window['-ML-SRC-PARTIAL-RESULTS-'].update(text, background_color_for_value='yellow1', autoscroll=True)
+                translated_text = ""
+                main_window['-ML-DST-PARTIAL-RESULTS-'].update(translated_text, background_color_for_value='yellow1', autoscroll=True)
 
                 if overlay_translation_window:
                     overlay_translation_window.close()
                     overlay_translation_window=None
 
                 # SAVING TRANSCRIPTIONS IN A TEMPORARY SUBTITLE FILE
-                #print("Saving transcriptions")
                 timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
                 subtitle_format = "srt"
                 formatter = FORMATTERS.get(subtitle_format)
                 formatted_subtitles = formatter(timed_subtitles)
 
                 if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
                     tmp_src_subtitle_basename, extension = os.path.splitext(os.path.basename(tmp_recorded_streaming_filepath))
@@ -1770,155 +1947,177 @@
                 tmp_src_subtitle_file.write(formatted_subtitles.encode("utf-8"))
                 tmp_src_subtitle_file.close()
 
                 # SAVING TRANSCRIPTIONS AS FORMATTED SUBTITLE FILE WITH FILENAME DECLARED IN COMMAND LINE ARGUMENTS
                 if args.subtitle_filename:
                     subtitle_file_base, subtitle_file_extension = os.path.splitext(args.subtitle_filename)
                     subtitle_file_extension = subtitle_file_extension[1:]
-                    #print("subtitle_file_base = {}".format(subtitle_file_base))
-                    #print("subtitle_file_extension = {}".format(subtitle_file_extension))
 
                     if subtitle_file_extension and subtitle_file_extension in FORMATTERS.keys():
-                        #print("subtitle_file_extension in FORMATTERS.keys()")
                         subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=subtitle_file_extension)
                         timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
                         subtitle_format = subtitle_file_extension
                         formatter = FORMATTERS.get(subtitle_format)
                         formatted_subtitles = formatter(timed_subtitles)
                         subtitle_file = open(subtitle_filepath, 'wb')
                         subtitle_file.write(formatted_subtitles.encode("utf-8"))
                         subtitle_file.close()
                     else:
-                        #print("subtitle_file_extension not in FORMATTERS.keys()")
                         FONT_TYPE = "Helvetica"
                         FONT_SIZE = 9
                         sg.set_options(font=(FONT_TYPE, FONT_SIZE))
                         sg.Popup("Subtitle format you typed is not supported, subtitle file will be saved in TXT format.", title="Info")
                         subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format="txt")
-                        shutil.copy(src_tmp_txt_transcription_filepath, subtitle_filepath)
+                        shutil.copy(tmp_src_txt_transcription_filepath, subtitle_filepath)
 
                 if thread_record_streaming and thread_record_streaming.is_alive():
-                    if platform.system() == "Windows":
+                    if sys.platform == "win32":
                         stop_record_streaming_windows()
 
-                    elif platform.system() == "Linux":
+                    elif sys.platform == "linux":
                         stop_record_streaming_linux()
 
                 # SAVING TEMPORARY TRANSLATED TRANSCRIPTIONS AS FORMATTED SUBTITLE FILE
-                #print("Saving translated transcriptions")
                 created_regions = []
                 created_subtitles = []
                 for entry in timed_subtitles:
                     created_regions.append(entry[0])
                     created_subtitles.append(entry[1])
 
                 translated_transcriptions = []
                 i = 0
-                progressbar = make_progress_bar_window(len(created_subtitles), "Saving translated transcriptions...")
-                for created_subtitle in created_subtitles:
-                    translated_transcription = GoogleTranslate(created_subtitle, src, dst)
-                    translated_transcriptions.append(translated_transcription)
-                    i += 1
-                    progressbar['-INFO-'].update('Saving translated transcriptions...')
-                    progressbar['-PERCENTAGE-'].update(f'{int(i*100/len(created_subtitles))}%')
-                    progressbar['-PROGRESS-'].update(i)
-                progressbar['-INFO-'].update('Saving translated transcriptions...')
-                progressbar['-PERCENTAGE-'].update(f'{int(len(created_subtitles)*100/len(created_subtitles))}%')
-                progressbar['-PROGRESS-'].update(len(created_subtitles))
-                time.sleep(1)
-                progressbar.close()
 
-                timed_translated_subtitles = [(r, t) for r, t in zip(created_regions, translated_transcriptions) if t]
-                formatter = FORMATTERS.get(subtitle_format)
-                formatted_translated_subtitles = formatter(timed_translated_subtitles)
+                if len(created_subtitles)>0:
+                    progressbar = make_progress_bar_window(len(created_subtitles), "Saving temporary translated transcriptions...")
+                    for created_subtitle in created_subtitles:
+                        translated_transcription = GoogleTranslate(created_subtitle, src, dst)
+                        translated_transcriptions.append(translated_transcription)
+                        i += 1
+                        progressbar['-INFO-'].update("Saving temporary translated transcriptions...")
+                        progressbar['-PERCENTAGE-'].update(f'{int(i*100/len(created_subtitles))}%')
+                        progressbar['-PROGRESS-'].update(i)
+                    progressbar['-INFO-'].update("Saving temporary translated transcriptions...")
+                    progressbar['-PERCENTAGE-'].update(f'{int(len(created_subtitles)*100/len(created_subtitles))}%')
+                    progressbar['-PROGRESS-'].update(len(created_subtitles))
+                    time.sleep(1)
+                    progressbar.close()
 
-                tmp_dst_subtitle_filepath = tmp_src_subtitle_filepath[ :-4] + ".translated." + subtitle_format
+                    timed_translated_subtitles = [(r, t) for r, t in zip(created_regions, translated_transcriptions) if t]
+                    formatter = FORMATTERS.get(subtitle_format)
+                    formatted_translated_subtitles = formatter(timed_translated_subtitles)
 
-                with open(tmp_dst_subtitle_filepath, 'wb') as f:
-                    f.write(formatted_translated_subtitles.encode("utf-8"))
-                f.close()
+                    tmp_dst_subtitle_filepath = tmp_src_subtitle_filepath[ :-4] + ".translated." + subtitle_format
 
-                with open(tmp_dst_subtitle_filepath, 'a') as f:
-                    f.write("\n")
-                f.close()
+                    with open(tmp_dst_subtitle_filepath, 'wb') as f:
+                        f.write(formatted_translated_subtitles.encode("utf-8"))
+                    f.close()
 
-                # SAVING TEMPORARY TRANSLATED TRANSCRIPTION AS TEXT FILE
-                with open(dst_tmp_txt_transcription_filepath, 'w') as f:
-                    for i in range(len(translated_transcriptions)):
+                    with open(tmp_dst_subtitle_filepath, 'a') as f:
+                        f.write("\n")
+                    f.close()
 
-                        start_time_delta = timedelta(seconds=created_regions[i][0])
-                        start_time_str = "{:02d}:{:02d}:{:02.0f}.{:03.0f}".format(
-                            start_time_delta.seconds // 3600,  # hours
-                            (start_time_delta.seconds // 60) % 60,  # minutes
-                            start_time_delta.seconds % 60, # seconds
-                            start_time_delta.microseconds / 1000000  # microseconds
-                        )
+                    # SAVING TEMPORARY TRANSLATED TRANSCRIPTION AS TEXT FILE
+                    with open(tmp_dst_txt_transcription_filepath, 'w') as f:
+                        for i in range(len(translated_transcriptions)):
 
-                        end_time_delta = timedelta(seconds=created_regions[i][1])
-                        end_time_str = "{:02d}:{:02d}:{:02.0f}.{:03.0f}".format(
-                            end_time_delta.seconds // 3600,  # hours
-                            (end_time_delta.seconds // 60) % 60,  # minutes
-                            end_time_delta.seconds % 60, # seconds
-                            end_time_delta.microseconds / 1000000  # microseconds
-                        )
+                            start_time_delta = timedelta(seconds=created_regions[i][0])
+                            start_time_str = "{:02d}:{:02d}:{:02.0f}.{:03.0f}".format(
+                                start_time_delta.seconds // 3600,  # hours
+                                (start_time_delta.seconds // 60) % 60,  # minutes
+                                start_time_delta.seconds % 60, # seconds
+                                start_time_delta.microseconds / 1000000  # microseconds
+                            )
 
-                        time_stamp_string = start_time_str + "-" + end_time_str
-                        f.write(time_stamp_string + " " + translated_transcriptions[i] + "\n")
+                            end_time_delta = timedelta(seconds=created_regions[i][1])
+                            end_time_str = "{:02d}:{:02d}:{:02.0f}.{:03.0f}".format(
+                                end_time_delta.seconds // 3600,  # hours
+                                (end_time_delta.seconds // 60) % 60,  # minutes
+                                end_time_delta.seconds % 60, # seconds
+                                end_time_delta.microseconds / 1000000  # microseconds
+                            )
 
-                f.close()
+                            time_stamp_string = start_time_str + "-" + end_time_str
+                            f.write(time_stamp_string + " " + translated_transcriptions[i] + "\n")
 
+                    f.close()
 
-                # SAVING TRANSLATED SUBTITLE FILE WITH FILENAME BASED ON SUBTITLE FILENAME DECLARED IN COMMAND LINE ARGUMENTS
-                if args.subtitle_filename:
+                    # SAVING TRANSLATED SUBTITLE FILE WITH FILENAME BASED ON SUBTITLE FILENAME DECLARED IN COMMAND LINE ARGUMENTS
+                    if args.subtitle_filename:
 
-                    saved_dst_subtitle_filepath = subtitle_filepath[ :-4] + ".translated." + subtitle_format
+                        saved_dst_subtitle_filepath = subtitle_filepath[ :-4] + ".translated." + subtitle_format
 
-                    if subtitle_file_extension and subtitle_file_extension in FORMATTERS.keys():
-                        timed_translated_subtitles = [(r, t) for r, t in zip(created_regions, translated_transcriptions) if t]
-                        subtitle_format = subtitle_file_extension
-                        formatter = FORMATTERS.get(subtitle_format)
-                        formatted_translated_subtitles = formatter(timed_translated_subtitles)
-                        saved_dst_subtitle_file = open(saved_dst_subtitle_filepath, 'wb')
-                        saved_dst_subtitle_file.write(formatted_translated_subtitles.encode("utf-8"))
-                        saved_dst_subtitle_file.close()
-                    else:
-                        shutil.copy(dst_tmp_txt_transcription_filepath, saved_dst_subtitle_filepath)
+                        if subtitle_file_extension and subtitle_file_extension in FORMATTERS.keys():
+                            timed_translated_subtitles = [(r, t) for r, t in zip(created_regions, translated_transcriptions) if t]
+                            subtitle_format = subtitle_file_extension
+                            formatter = FORMATTERS.get(subtitle_format)
+                            formatted_translated_subtitles = formatter(timed_translated_subtitles)
+                            saved_dst_subtitle_file = open(saved_dst_subtitle_filepath, 'wb')
+                            saved_dst_subtitle_file.write(formatted_translated_subtitles.encode("utf-8"))
+                            saved_dst_subtitle_file.close()
+                        else:
+                            shutil.copy(tmp_dst_txt_transcription_filepath, saved_dst_subtitle_filepath)
 
-                if args.video_filename:
-                    shutil.copy(tmp_recorded_streaming_filepath, saved_recorded_streaming_filename)
+                    if args.video_filename:
+                        shutil.copy(tmp_recorded_streaming_filepath, saved_recorded_streaming_filename)
 
-            if not (platform.system() == "Windows"):
+            if not (sys.platform == "win32"):
                 main_window.TKroot.attributes('-topmost', 1)
                 main_window.TKroot.attributes('-topmost', 0)
 
 
-        elif event == '-EVENT-VOICE-RECOGNIZED-' and recognizing==True:
+        elif event == '-EVENT-NULL-RESULTS-' and recognizing==True:
+            overlay_translation_window.Hide()
 
-            text=str(values[event]).strip().lower()
-            main_window['-ML1-'].update(text,background_color_for_value='yellow1',autoscroll=True)
-            
-            if not (platform.system() == "Windows"):
+
+        elif event == '-EVENT-PARTIAL-RESULTS-' and recognizing==True:
+
+            text = str(values[event]).strip().lower()
+            main_window['-ML-SRC-PARTIAL-RESULTS-'].update(text,background_color_for_value='yellow1',autoscroll=True)
+
+            partial_result_filename = "partial_result"
+            partial_result_filepath = os.path.join(tempfile.gettempdir(), partial_result_filename)
+            partial_result_file = open(partial_result_filepath, "w")
+            partial_result_file.write(text)
+            partial_result_file.close()
+
+            if not (sys.platform == "win32"):
                 main_window.TKroot.attributes('-topmost', 1)
                 main_window.TKroot.attributes('-topmost', 0)
 
 
         elif event == '-EVENT-VOICE-TRANSLATED-' and recognizing==True:
 
-            overlay_translation_window.UnHide()
-            translated_text=str(values[event]).strip().lower()
-            main_window['-ML2-'].update(translated_text,background_color_for_value='yellow1',autoscroll=True)
+            translated_text = str(values[event]).strip().lower()
+            if translated_text:
+                main_window['-ML-DST-PARTIAL-RESULTS-'].update(translated_text,background_color_for_value='yellow1',autoscroll=True)
 
-            if (overlay_translation_window):
-                overlay_translation_window['-ML-LS2-'].update(translated_text,background_color_for_value='black', autoscroll=True)
+                # SHOWING OVERLAY TRANSLATION WINDOW
+                if not overlay_translation_window:
+                    overlay_translation_window = make_overlay_translation_window(100*' ')
 
-            if not (platform.system() == "Windows"):
+                overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_text,background_color_for_value='black', visible=True, autoscroll=True)
+            else:
+                overlay_translation_window.Hide()
+
+            if not (sys.platform == "win32"):
                 main_window.TKroot.attributes('-topmost', 1)
                 main_window.TKroot.attributes('-topmost', 0)
 
 
+        elif event == '-EVENT-RESULTS-' and recognizing==True:
+
+            line = str(values[event]).strip().lower()
+            main_window['-ML-SRC-RESULTS-'].update(line + "\n", background_color_for_value='yellow1', append=True, autoscroll=True)
+            translated_line = GoogleTranslate(line, src, dst)
+            main_window['-ML-DST-RESULTS-'].update(translated_line + "\n", background_color_for_value='yellow1', append=True, autoscroll=True)
+            if overlay_translation_window:
+                overlay_translation_window.UnHide
+                overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_line, background_color_for_value='black', visible=True, autoscroll=True)
+
+
         elif event == '-EVENT-STREAMING-DURATION-RECORDED-':
 
             record_duration = str(values[event]).strip()
             main_window['-STREAMING-DURATION-RECORDED-'].update(record_duration)
 
 
         elif event == '-EVENT-THREAD-RECORD-STREAMING-STATUS-':
@@ -1950,15 +2149,15 @@
                 FONT_TYPE = "Helvetica"
                 FONT_SIZE = 9
                 sg.set_options(font=(FONT_TYPE, FONT_SIZE))
                 sg.Popup("No streaming was recorded.                             ", title="Info")
 
 
         elif event == '-EVENT-SAVE-SRC-TRANSCRIPTION-':
-            if os.path.isfile(src_tmp_txt_transcription_filepath):
+            if os.path.isfile(tmp_src_txt_transcription_filepath):
 
                 saved_src_subtitle_filename = sg.popup_get_file('', no_window=True, save_as=True, font=(FONT_TYPE, FONT_SIZE), file_types=subtitle_file_types)
 
                 if saved_src_subtitle_filename:
 
                     selected_subtitle_format = saved_src_subtitle_filename.split('.')[-1]
 
@@ -1969,31 +2168,31 @@
                         formatted_subtitles = formatter(timed_subtitles)
                         tmp_src_subtitle_filename = saved_src_subtitle_filename
                         subtitle_file = open(tmp_src_subtitle_filename, 'wb')
                         subtitle_file.write(formatted_subtitles.encode("utf-8"))
                         subtitle_file.close()
                     else:
                         saved_src_subtitle_file = open(saved_src_subtitle_filename, "w")
-                        src_tmp_txt_transcription_file = open(src_tmp_txt_transcription_filepath, "r")
-                        for line in src_tmp_txt_transcription_file:
+                        tmp_src_txt_transcription_file = open(tmp_src_txt_transcription_filepath, "r")
+                        for line in tmp_src_txt_transcription_file:
                             if line:
                                 saved_src_subtitle_file.write(line)
                         saved_src_subtitle_file.close()
-                        src_tmp_txt_transcription_file.close()
+                        tmp_src_txt_transcription_file.close()
 
             else:
                 FONT_TYPE = "Helvetica"
                 FONT_SIZE = 9
                 sg.set_options(font=(FONT_TYPE, FONT_SIZE))
                 sg.Popup("No transcriptions was recorded.                             ", title="Info")
 
 
         elif event == '-EVENT-SAVE-DST-TRANSCRIPTION-':
 
-            if os.path.isfile(dst_tmp_txt_transcription_filepath):
+            if os.path.isfile(tmp_dst_txt_transcription_filepath):
 
                 saved_dst_subtitle_filename = sg.popup_get_file('', no_window=True, save_as=True, font=(FONT_TYPE, FONT_SIZE), file_types=subtitle_file_types)
 
                 if saved_dst_subtitle_filename:
 
                     selected_subtitle_format = saved_dst_subtitle_filename.split('.')[-1]
 
@@ -2003,32 +2202,40 @@
                         formatter = FORMATTERS.get(subtitle_format)
                         formatted_translated_subtitles = formatter(timed_translated_subtitles)
                         saved_dst_subtitle_file = open(saved_dst_subtitle_filename, 'wb')
                         saved_dst_subtitle_file.write(formatted_translated_subtitles.encode("utf-8"))
                         saved_dst_subtitle_file.close()
                     else:
                         saved_dst_subtitle_file = open(saved_dst_subtitle_filename, "w")
-                        dst_tmp_txt_transcription_file = open(dst_tmp_txt_transcription_filepath, "r")
-                        for line in dst_tmp_txt_transcription_file:
+                        tmp_dst_txt_transcription_file = open(tmp_dst_txt_transcription_filepath, "r")
+                        for line in tmp_dst_txt_transcription_file:
                             if line:
                                 saved_dst_subtitle_file.write(line)
                         saved_dst_subtitle_file.close()
-                        dst_tmp_txt_transcription_file.close()
+                        tmp_dst_txt_transcription_file.close()
             else:
                 FONT_TYPE = "Helvetica"
                 FONT_SIZE = 9
                 sg.set_options(font=(FONT_TYPE, FONT_SIZE))
                 sg.Popup("No translated transcriptions was recorded.                 ", title="Info")
 
-
     if thread_recognize and thread_recognize.is_alive():
-        stop_thread(thread_recognize)
+        stop_thread2(thread_recognize)
 
     if thread_timed_translate and thread_timed_translate.is_alive():
-        stop_thread(thread_timed_translate)
+        stop_thread2(thread_timed_translate)
+
+    time.sleep(1)
+    if tmp_recorded_streaming_filepath and os.path.isfile(tmp_recorded_streaming_filepath): os.remove(tmp_recorded_streaming_filepath)
+    if partial_result_filepath and os.path.isfile(partial_result_filepath): os.remove(partial_result_filepath)
+    if time_value_filepath and os.path.isfile(time_value_filepath): os.remove(time_value_filepath)
+    if tmp_src_subtitle_filepath and os.path.isfile(tmp_src_subtitle_filepath): os.remove(tmp_src_subtitle_filepath)
+    if tmp_dst_subtitle_filepath and os.path.isfile(tmp_dst_subtitle_filepath): os.remove(tmp_dst_subtitle_filepath)
+    if tmp_src_txt_transcription_filepath and os.path.isfile(tmp_src_txt_transcription_filepath): os.remove(tmp_src_txt_transcription_filepath)
+    if tmp_dst_txt_transcription_filepath and os.path.isfile(tmp_dst_txt_transcription_filepath): os.remove(tmp_dst_txt_transcription_filepath)
 
     main_window.close()
     sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyvosklivesubtitle-0.1.2/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.3/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.2/setup.py` & `pyvosklivesubtitle-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'pyvosklivesubtitle is a python based desktop aplication which can recognize any live streaming'
     'in 21 languages that supported by VOSK then translate and display it as LIVE SUBTITLES'
     )
 
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
-    version="0.1.2",
+    version="0.1.3",
     include_package_data=True,
     author='Bot Bahlul',
     author_email='bot.bahlul@gmail.com',
     url='https://github.com/botbahlul/pyvosklivesubtitle',
     packages=[str('pyvosklivesubtitle')],
     entry_points={
         'console_scripts': [
```

