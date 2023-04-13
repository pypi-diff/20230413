# Comparing `tmp/dokuwikidumper-0.1.7.tar.gz` & `tmp/dokuwikidumper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dokuwikidumper-0.1.7.tar", max compression
+gzip compressed data, was "dokuwikidumper-0.1.8.tar", max compression
```

## Comparing `dokuwikidumper-0.1.7.tar` & `dokuwikidumper-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-02-14 14:44:04.142863 dokuwikidumper-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     6888 2023-03-26 15:28:34.017152 dokuwikidumper-0.1.7/README.md
--rw-r--r--   0        0        0       57 2023-02-16 17:41:45.629101 dokuwikidumper-0.1.7/dokuWikiDumper/__init__.py
--rw-r--r--   0        0        0       73 2023-03-13 09:45:13.311407 dokuwikidumper-0.1.7/dokuWikiDumper/__main__.py
--rw-r--r--   0        0        0       24 2023-03-30 16:06:11.456914 dokuwikidumper-0.1.7/dokuWikiDumper/__version__.py
--rw-r--r--   0        0        0     7965 2023-03-26 15:05:48.062602 dokuwikidumper-0.1.7/dokuWikiDumper/dump/content/__init__.py
--rw-r--r--   0        0        0     7672 2023-03-30 16:00:51.487847 dokuwikidumper-0.1.7/dokuWikiDumper/dump/content/revisions.py
--rw-r--r--   0        0        0     2863 2023-03-18 10:37:28.215096 dokuwikidumper-0.1.7/dokuWikiDumper/dump/content/titles.py
--rw-r--r--   0        0        0     8223 2023-03-26 15:28:09.556722 dokuwikidumper-0.1.7/dokuWikiDumper/dump/dokuDumper.py
--rw-r--r--   0        0        0       27 2023-03-21 03:34:03.164081 dokuwikidumper-0.1.7/dokuWikiDumper/dump/html/__init__.py
--rw-r--r--   0        0        0     4067 2023-03-26 15:11:17.495346 dokuwikidumper-0.1.7/dokuWikiDumper/dump/html/html.py
--rw-r--r--   0        0        0      216 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.7/dokuWikiDumper/dump/info/__init__.py
--rw-r--r--   0        0        0     3239 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.7/dokuWikiDumper/dump/info/info.py
--rw-r--r--   0        0        0       38 2023-02-18 16:00:58.611751 dokuwikidumper-0.1.7/dokuWikiDumper/dump/media/__init__.py
--rw-r--r--   0        0        0     5741 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.7/dokuWikiDumper/dump/media/media.py
--rw-r--r--   0        0        0       82 2023-03-26 14:53:46.352338 dokuwikidumper-0.1.7/dokuWikiDumper/dump/pdf/__init__.py
--rw-r--r--   0        0        0     4404 2023-03-26 17:20:10.040898 dokuwikidumper-0.1.7/dokuWikiDumper/dump/pdf/pdf.py
--rw-r--r--   0        0        0     1208 2023-03-26 09:59:17.227185 dokuwikidumper-0.1.7/dokuWikiDumper/exceptions.py
--rw-r--r--   0        0        0      694 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.7/dokuWikiDumper/utils/config.py
--rw-r--r--   0        0        0     4259 2023-03-26 09:18:58.054344 dokuwikidumper-0.1.7/dokuWikiDumper/utils/session.py
--rw-r--r--   0        0        0     3971 2023-03-30 15:59:35.730647 dokuwikidumper-0.1.7/dokuWikiDumper/utils/util.py
--rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.7/dokuWikiUploader/__init__.py
--rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.7/dokuWikiUploader/__main__.py
--rw-r--r--   0        0        0       26 2023-03-30 16:06:17.061003 dokuwikidumper-0.1.7/dokuWikiUploader/__version__.py
--rw-r--r--   0        0        0     7365 2023-03-26 15:22:57.215211 dokuwikidumper-0.1.7/dokuWikiUploader/uploader.py
--rw-r--r--   0        0        0      828 2023-03-30 16:05:58.060702 dokuwikidumper-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     8176 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.7/setup.py
--rw-r--r--   0        0        0     7766 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-14 14:44:04.142863 dokuwikidumper-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     7029 2023-04-13 08:43:03.808779 dokuwikidumper-0.1.8/README.md
+-rw-r--r--   0        0        0       57 2023-02-16 17:41:45.629101 dokuwikidumper-0.1.8/dokuWikiDumper/__init__.py
+-rw-r--r--   0        0        0       73 2023-03-13 09:45:13.311407 dokuwikidumper-0.1.8/dokuWikiDumper/__main__.py
+-rw-r--r--   0        0        0       24 2023-04-13 08:15:56.104911 dokuwikidumper-0.1.8/dokuWikiDumper/__version__.py
+-rw-r--r--   0        0        0     8138 2023-04-02 14:44:11.506070 dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/__init__.py
+-rw-r--r--   0        0        0     7672 2023-03-30 16:00:51.487847 dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/revisions.py
+-rw-r--r--   0        0        0     2863 2023-03-18 10:37:28.215096 dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/titles.py
+-rw-r--r--   0        0        0     9267 2023-04-13 08:40:42.244757 dokuwikidumper-0.1.8/dokuWikiDumper/dump/dokuDumper.py
+-rw-r--r--   0        0        0       27 2023-03-21 03:34:03.164081 dokuwikidumper-0.1.8/dokuWikiDumper/dump/html/__init__.py
+-rw-r--r--   0        0        0     4067 2023-03-26 15:11:17.495346 dokuwikidumper-0.1.8/dokuWikiDumper/dump/html/html.py
+-rw-r--r--   0        0        0      216 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiDumper/dump/info/__init__.py
+-rw-r--r--   0        0        0     3325 2023-04-13 06:47:42.540273 dokuwikidumper-0.1.8/dokuWikiDumper/dump/info/info.py
+-rw-r--r--   0        0        0       38 2023-02-18 16:00:58.611751 dokuwikidumper-0.1.8/dokuWikiDumper/dump/media/__init__.py
+-rw-r--r--   0        0        0     5741 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiDumper/dump/media/media.py
+-rw-r--r--   0        0        0       82 2023-03-26 14:53:46.352338 dokuwikidumper-0.1.8/dokuWikiDumper/dump/pdf/__init__.py
+-rw-r--r--   0        0        0     4404 2023-03-26 17:20:10.040898 dokuwikidumper-0.1.8/dokuWikiDumper/dump/pdf/pdf.py
+-rw-r--r--   0        0        0     1208 2023-03-26 09:59:17.227185 dokuwikidumper-0.1.8/dokuWikiDumper/exceptions.py
+-rw-r--r--   0        0        0      756 2023-04-13 06:46:25.970991 dokuwikidumper-0.1.8/dokuWikiDumper/utils/config.py
+-rw-r--r--   0        0        0     4259 2023-04-13 08:08:16.985223 dokuwikidumper-0.1.8/dokuWikiDumper/utils/session.py
+-rw-r--r--   0        0        0     4248 2023-04-13 07:21:43.558449 dokuwikidumper-0.1.8/dokuWikiDumper/utils/util.py
+-rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiUploader/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiUploader/__main__.py
+-rw-r--r--   0        0        0       26 2023-04-13 08:16:05.381066 dokuwikidumper-0.1.8/dokuWikiUploader/__version__.py
+-rw-r--r--   0        0        0     7264 2023-04-13 07:00:32.369164 dokuwikidumper-0.1.8/dokuWikiUploader/uploader.py
+-rw-r--r--   0        0        0      845 2023-04-13 08:16:17.337266 dokuwikidumper-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     8368 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.8/setup.py
+-rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.8/PKG-INFO
```

### Comparing `dokuwikidumper-0.1.7/LICENSE.md` & `dokuwikidumper-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/README.md` & `dokuwikidumper-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ### dokuWikiDumper
 
 - Python 3.8+ (developed on py3.10)
 - beautifulsoup4
 - requests
 - lxml
+- rich
 
 ### dokuWikiUploader
 
 > Upload wiki dump to [Internet Archive](https://archive.org/).
 > `dokuWikiUploader -h` for help.
 
 - internetarchive
@@ -123,14 +124,16 @@
 | `pages/`                | latest page content. (wikitext)             |
 <!-- /Dump structure -->
 
 ## Available Backups/Dumps
 
 I made some backups for testing, you can check out the list: <https://github.com/orgs/saveweb/projects/4>.
 
+> Some wikidump has been uploaded to IA, you can check out the list: <https://archive.org/search?query=subject%3A"dokuWikiDumper">
+> 
 > If you dumped a DokuWiki and want to share it, please feel free to open an issue, I will add it to the list.
 
 ## How to import dump to DokuWiki
 
 If you need to import Dokuwiki, please add the following configuration to `local.php`
 
 ```php
```

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/content/__init__.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,19 +155,21 @@
             else:
                 # Different date formats in different versions of DokuWiki.
                 # If no ID was found, make one up based on the date (since rev IDs are Unix times)
                 # Maybe this is evil. Not sure.
 
                 print(
                     msg_header, '    One revision of [[%s]] missing rev_id. Using date to rebuild...' % title, end=' ')
-                date_formats = ["%Y-%m-%d %H:%M", "%Y/%m/%d %H:%M", "%d.%m.%Y %H:%M"]
+                date_formats = ["%Y-%m-%d %H:%M", "%Y/%m/%d %H:%M", "%d.%m.%Y %H:%M", "%d/%m/%Y %H:%M"]
                 # Try each date format until one works.
                 # Example below:
                 # %Y-%m-%d %H:%M | <https://www.dokuwiki.org/dokuwiki?do=revisions> # 2019/01/01 00:00
-                #  
+                # TODO: %Y-%m-%d %H:%M
+                # TODO: %Y/%m/%d %H:%M
+                # %d/%m/%Y %H:%M | <https://eolienne.f4jr.org/?do=revisions> #  28/02/2013 12:12
                 for date_format in date_formats:
                     try:
                         date = datetime.strptime(rev['date'], date_format)
                         id = str(int(time.mktime(date.utctimetuple())))
                         break
                     except:
                         id = None
```

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/content/revisions.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/revisions.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/content/titles.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/titles.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/dokuDumper.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/dokuDumper.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import os
 import time
 
 import requests
 # import gzip, 7z
+from rich import print
 
 from dokuWikiDumper.__version__ import DUMPER_VERSION
 from dokuWikiDumper.dump.content import dumpContent
 from dokuWikiDumper.dump.html import dump_HTML
 from dokuWikiDumper.dump.info import update_info
 from dokuWikiDumper.dump.media import dumpMedia
 from dokuWikiDumper.dump.pdf import dump_PDF
@@ -137,15 +138,15 @@
                        username=args.username, password=args.password)
     if args.cookies:
         load_cookies(session, args.cookies)
 
 
     base_url = buildBaseUrl(doku_url)
     dumpDir = url2prefix(doku_url) + '-' + \
-        time.strftime("%Y%m%d") if not args.path else args.path
+        time.strftime("%Y%m%d") if not args.path else args.path.rstrip('/')
     if args.no_resume:
         if os.path.exists(dumpDir):
             print(
                 'Dump directory already exists. (You can use --path to specify a different directory.)')
             return 1
 
     smkdirs(dumpDir, '/dumpMeta')
@@ -158,31 +159,51 @@
                'doku_url': doku_url,  # type: str
                'base_url': base_url,  # type: str
                'dokuWikiDumper_version': DUMPER_VERSION,
                }
     update_config(dumpDir=dumpDir, config=_config)
     update_info(dumpDir, doku_url=doku_url, session=session)
     if args.content:
-        print('\nDumping content...\n')
-        dumpContent(doku_url=doku_url, dumpDir=dumpDir,
-                    session=session, skipTo=skip_to, threads=args.threads,
-                    ignore_errors=args.ignore_errors,
-                    ignore_action_disabled_edit=args.ignore_action_disabled_edit)
+        if os.path.exists(os.path.join(dumpDir, 'content_dumped.mark')):
+            print('Content already dumped.')
+        else:
+            print('\nDumping content...\n')
+            dumpContent(doku_url=doku_url, dumpDir=dumpDir,
+                        session=session, skipTo=skip_to, threads=args.threads,
+                        ignore_errors=args.ignore_errors,
+                        ignore_action_disabled_edit=args.ignore_action_disabled_edit)
+            with open(os.path.join(dumpDir, 'content_dumped.mark'), 'w') as f:
+                f.write('done')
     if args.html:
-        print('\nDumping HTML...\n')
-        dump_HTML(doku_url=doku_url, dumpDir=dumpDir,
-                  session=session, skipTo=skip_to, threads=args.threads,
-                  ignore_errors=args.ignore_errors, current_only=args.current_only)
+        if os.path.exists(os.path.join(dumpDir, 'html_dumped.mark')):
+            print('HTML already dumped.')
+        else:
+            print('\nDumping HTML...\n')
+            dump_HTML(doku_url=doku_url, dumpDir=dumpDir,
+                    session=session, skipTo=skip_to, threads=args.threads,
+                    ignore_errors=args.ignore_errors, current_only=args.current_only)
+            with open(os.path.join(dumpDir, 'html_dumped.mark'), 'w') as f:
+                f.write('done')
     if args.media: # last, so that we can know the dump is complete.
-        print('\nDumping media...\n')
-        dumpMedia(url=base_url, dumpDir=dumpDir,
-                  session=session, threads=args.threads,
-                  ignore_errors=args.ignore_errors)
+        if os.path.exists(os.path.join(dumpDir, 'media_dumped.mark')):
+            print('Media already dumped.')
+        else:
+            print('\nDumping media...\n')
+            dumpMedia(url=base_url, dumpDir=dumpDir,
+                    session=session, threads=args.threads,
+                    ignore_errors=args.ignore_errors)
+            with open(os.path.join(dumpDir, 'media_dumped.mark'), 'w') as f:
+                f.write('done')
     if args.pdf:
-        print('\nDumping PDF...\n')
-        dump_PDF(doku_url=base_url, dumpDir=dumpDir,
-                session=session, threads=args.threads,
-                ignore_errors=args.ignore_errors, current_only=True)
-                # to avoid overload the server, we only dump the current revision of the PDF.
+        if os.path.exists(os.path.join(dumpDir, 'pdf_dumped.mark')):
+            print('PDF already dumped.')
+        else:
+            print('\nDumping PDF...\n')
+            dump_PDF(doku_url=base_url, dumpDir=dumpDir,
+                    session=session, threads=args.threads,
+                    ignore_errors=args.ignore_errors, current_only=True)
+                    # to avoid overload the server, we only dump the current revision of the PDF.
+            with open(os.path.join(dumpDir, 'pdf_dumped.mark'), 'w') as f:
+                f.write('done')
 
 
     print('\n\n--Done--')
```

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/html/html.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/html/html.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/info/info.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/info/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import os
 import re
 from typing import Optional
 from urllib.parse import urljoin
 
 from bs4 import BeautifulSoup
 import requests
+from rich import print
 
+from dokuWikiDumper.utils.util import print_with_lock as print
 from dokuWikiDumper.utils.util import uopen
 
 INFO_FILEPATH = 'dumpMeta/info.json'
 HOMEPAGE_FILEPATH = 'dumpMeta/index.html'
 CHECKPAGE_FILEPATH = 'dumpMeta/check.html'
 ICON_FILEPATH = 'dumpMeta/favicon.ico'
```

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/media/media.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/media/media.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/dump/pdf/pdf.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/dump/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/exceptions.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/exceptions.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/utils/config.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/utils/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import json
 import os
-
+from dokuWikiDumper.utils.util import print_with_lock as print
 from dokuWikiDumper.utils.util import uopen
 
 CONFIG_FILEPATH = 'dumpMeta/config.json'
 
 
 def update_config(dumpDir: str, config: dict):
     '''Only updates given keys in config.'''
```

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/utils/session.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/utils/session.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.7/dokuWikiDumper/utils/util.py` & `dokuwikidumper-0.1.8/dokuWikiDumper/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 import re
 import sys
 import threading
 import time
 from typing import *
 from urllib.parse import urlparse
-
+from rich import print as rprint
 import requests
 
+USE_RICH = True
+
 fileLock = threading.Lock()
 printLock = threading.Lock()
 
 
 def check_int(s: str = ''):
     """ Check if a string is an integer
     :return: None if not an integer, otherwise the raw string
@@ -21,15 +23,21 @@
         int(s)
         return s
     except:
         return None
 
 def print_with_lock(*args, **kwargs):
     printLock.acquire()
-    builtins.print(*args, **kwargs)
+    if USE_RICH:
+        # replace [[ and ]] with "
+        args = [re.sub(r'\[\[', '\"', str(arg)) for arg in args]
+        args = [re.sub(r'\]\]', '\"', str(arg)) for arg in args]
+        rprint(*args, **kwargs)
+    else:
+        builtins.print(*args, **kwargs)
     printLock.release()
 
 
 def avoidSites(url: str = ''):
     #check robots.txt
     r = requests.get(urlparse(url).scheme + '://' + urlparse(url).netloc + '/robots.txt')
     if r.status_code == 200:
```

### Comparing `dokuwikidumper-0.1.7/dokuWikiUploader/uploader.py` & `dokuwikidumper-0.1.8/dokuWikiUploader/uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,16 +73,15 @@
         identifier_local = _dump_dir_basename
     except Exception as e:
         print(e)
         print("\nSomething went wrong during generating the identifier. \n")
         raise e
     
     identifier_remote = 'wiki-' + identifier_local # 'wiki-' is the prefix of all wikis in archive.org
-    # currently(>=0.0.4), just add 'wiki-' as the prefix of the remote identifier
-    # but still use the local identifier as the filename prefix of the remote files
+    # with the prefix, wikidump can go into wikiteam collection.
 
     # identifier_remote = 'test-wiki-' + identifier_local # 
 
     description = \
 f'''DokuWiki: [{title}].
 
 Dumped with <a href="https://github.com/saveweb/dokuwiki-dumper" rel="nofollow">DokuWiki-Dumper</a> v{config.get('dokuWikiDumper_version')}, and uploaded with dokuWikiUploader v{UPLOADER_VERSION}.
```

### Comparing `dokuwikidumper-0.1.7/pyproject.toml` & `dokuwikidumper-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dokuWikiDumper"
-version = "0.1.7"
+version = "0.1.8"
 description = "A tool for archiving DokuWiki"
 authors = ["yzqzss <yzqzss@yandex.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 packages = [
     { include = "dokuWikiDumper/**/*" },
@@ -17,14 +17,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 beautifulsoup4 = "^4.11.2"
 lxml = "^4.9.2"
 internetarchive = "^3.3.0"
+rich = "^13.3.4"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 flake8 = "^4.0.1"
 
 [tool.poetry.scripts]
```

### Comparing `dokuwikidumper-0.1.7/setup.py` & `dokuwikidumper-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.11.2,<5.0.0',
  'internetarchive>=3.3.0,<4.0.0',
  'lxml>=4.9.2,<5.0.0',
- 'requests>=2.28.2,<3.0.0']
+ 'requests>=2.28.2,<3.0.0',
+ 'rich>=13.3.4,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['dokuWikiDumper = dokuWikiDumper:main',
                      'dokuWikiUploader = dokuWikiUploader:main']}
 
 setup_kwargs = {
     'name': 'dokuwikidumper',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'A tool for archiving DokuWiki',
-    'long_description': "# DokuWiki Dumper\n\n> A tool for archiving DokuWiki.\n\nRecommend using `dokuWikiDumper` on _modern_ filesystems, such as `ext4` or `btrfs`. `NTFS` is not recommended because of it denys many special characters in filename.\n\n## Requirements\n\n### dokuWikiDumper\n\n- Python 3.8+ (developed on py3.10)\n- beautifulsoup4\n- requests\n- lxml\n\n### dokuWikiUploader\n\n> Upload wiki dump to [Internet Archive](https://archive.org/).\n> `dokuWikiUploader -h` for help.\n\n- internetarchive\n- 7z (`7z` command)\n\n## Install `dokuWikiDumper`\n\n> `dokuWikiUploader` is included in `dokuWikiDumper`.\n\n### Install `dokuWikiDumper` with `pip` (recommended)\n\n> <https://pypi.org/project/dokuwikidumper/>\n\n```bash\npip3 install dokuWikiDumper\n```\n\n### Install `dokuWikiDumper` with `Poetry` (for developers)\n\n- Install `Poetry`\n\n    ```bash\n    pip3 install poetry\n    ```\n\n- Install `dokuWikiDumper`\n\n    ```bash\n    git clone https://github.com/saveweb/dokuwiki-dumper\n    cd dokuwiki-dumper\n    poetry install\n    rm dist/ -rf\n    poetry build\n    pip install --force-reinstall dist/dokuWikiDumper*.whl\n    ```\n\n## Usage\n\n```bash\nusage: dokuWikiDumper [-h] [--content] [--media] [--html] [--skip-to SKIP_TO] [--path PATH] [--no-resume] [--threads THREADS]\n                      [--insecure] [--ignore-errors] [--ignore-action-disabled-edit] [--username USERNAME] [--password PASSWORD]\n                      [--cookies COOKIES] [--auto]\n                      url\n\ndokuWikiDumper\n\npositional arguments:\n  url                   URL of the dokuWiki\n\noptions:\n  -h, --help            show this help message and exit\n  --content             Dump content\n  --media               Dump media\n  --html                Dump HTML\n  --pdf                 Dump PDF [default: false] (Only available on some wikis with the PDF export plugin) (Only dumps the latest PDF revision)\n  --current-only        Dump latest revision, no history [default: false] (only for HTML at the moment)\n  --skip-to SKIP_TO     !DEV! Skip to title number [default: 0]\n  --path PATH           Specify dump directory [default: <site>-<date>]\n  --no-resume           Do not resume a previous dump [default: resume]\n  --threads THREADS     Number of sub threads to use [default: 1], not recommended to set > 5\n  --insecure            Disable SSL certificate verification\n  --ignore-errors       !DANGEROUS! ignore errors in the sub threads. This may cause incomplete dumps.\n  --ignore-action-disabled-edit\n                        Some sites disable edit action for anonymous users and some core pages. This option will ignore this error and textarea not found error.But\n                        you may only get a partial dump. (only works with --content)\n  --username USERNAME   login: username\n  --password PASSWORD   login: password\n  --cookies COOKIES     cookies file\n  --auto                dump: content+media+html, threads=5, ignore-action-disable-edit\n```\n\nFor most cases, you can use `--auto` to dump the site.\n\n```bash\ndokuWikiDumper https://example.com/wiki/ --auto\n```\n\nwhich is equivalent to\n\n```bash\ndokuWikiDumper https://example.com/wiki/ --content --media --html --threads 5 --ignore-action-disabled-edit\n```\n\n> Highly recommend using `--username` and `--password` to login (or using `--cookies`), because some sites may disable anonymous users to access some pages or check the raw wikitext.\n\n`--cookies` accepts a Netscape cookies file, you can use [cookies.txt Extension](https://addons.mozilla.org/en-US/firefox/addon/cookies-txt/) to export cookies from Firefox. It also accepts a json cookies file created by [Cookie Quick Manager](https://addons.mozilla.org/en-US/firefox/addon/cookie-quick-manager/).\n\n## Dump structure\n\n<!-- Dump structure -->\n| Directory or File       | Description                                 |\n|-----------              |-------------                                |\n| `attic/`                | old revisions of page. (wikitext)           |\n| `dumpMeta/`             | (dokuWikiDumper only) metadata of the dump. |\n| `dumpMeta/check.html`   | ?do=check page of the wiki.                 |\n| `dumpMeta/config.json`  | dump's configuration.                       |\n| `dumpMeta/favicon.ico`  | favicon of the site.                        |\n| `dumpMeta/files.txt`    | list of filename.                           |\n| `dumpMeta/index.html`   | homepage of the wiki.                       |\n| `dumpMeta/info.json`    | infomations of the wiki.                    |\n| `dumpMeta/titles.txt`   | list of page title.                         |\n| `html/`                 | (dokuWikiDumper only) HTML of the pages.    |\n| `media/`                | media files.                                |\n| `meta/`                 | metadata of the pages.                      |\n| `pages/`                | latest page content. (wikitext)             |\n<!-- /Dump structure -->\n\n## Available Backups/Dumps\n\nI made some backups for testing, you can check out the list: <https://github.com/orgs/saveweb/projects/4>.\n\n> If you dumped a DokuWiki and want to share it, please feel free to open an issue, I will add it to the list.\n\n## How to import dump to DokuWiki\n\nIf you need to import Dokuwiki, please add the following configuration to `local.php`\n\n```php\n$conf['fnencode'] = 'utf-8'; // Dokuwiki default: 'safe' (url encode)\n# 'safe' => Non-ASCII characters will be escaped as %xx form.\n# 'utf-8' => Non-ASCII characters will be preserved as UTF-8 characters.\n\n$conf['compression'] = '0'; // Dokuwiki default: 'gz'.\n# 'gz' => attic/<id>.<rev_id>.txt.gz\n# 'bz2' => attic/<id>.<rev_id>.txt.bz2\n# '0' => attic/<id>.<rev_id>.txt\n```\n\nImport `pages` dir if you only need the latest version of the page.  \nImport `meta` dir if you need the **changelog** of the page.  \nImport `attic` and `meta` dirs if you need the old revisions **content** of the page.  \nImport `media` dir if you need the media files.\n\n`dumpMeta` and `html` dirs are only used by `dokuWikiDumper`, you can ignore it.\n\n## Information\n\n### DokuWiki links\n\n- [DokuWiki](https://www.dokuwiki.org/)\n- [DokuWiki changelog](https://www.dokuwiki.org/changelog)\n- [DokuWiki source code](https://github.com/splitbrain/dokuwiki)\n\n### Other tools\n\n- [MediaWiki Scraper](https://github.com/mediawiki-client-tools/mediawiki-scraper) (aka `wikiteam3`), a tool for archiving MediaWiki, forked from [WikiTeam](https://github.com/wikiteam/wikiteam/) and has been rewritten in Python 3.\n- [WikiTeam](https://github.com/wikiteam/wikiteam/), a tool for archiving MediaWiki, written in Python 2.\n\n## License\n\nGPLv3\n\n## Contributors\n\nThis tool is based on an unmerged PR (_8 years ago!_) of [WikiTeam](https://github.com/WikiTeam/wikiteam/): [DokuWiki dump alpha](https://github.com/WikiTeam/wikiteam/pull/243) by [@PiRSquared17](https://github.com/PiRSquared17).\n\nI ([@yzqzss](https://github.com/yzqzss)) have rewritten the code in Python 3 and added some features, also fixed some bugs.\n",
+    'long_description': '# DokuWiki Dumper\n\n> A tool for archiving DokuWiki.\n\nRecommend using `dokuWikiDumper` on _modern_ filesystems, such as `ext4` or `btrfs`. `NTFS` is not recommended because of it denys many special characters in filename.\n\n## Requirements\n\n### dokuWikiDumper\n\n- Python 3.8+ (developed on py3.10)\n- beautifulsoup4\n- requests\n- lxml\n- rich\n\n### dokuWikiUploader\n\n> Upload wiki dump to [Internet Archive](https://archive.org/).\n> `dokuWikiUploader -h` for help.\n\n- internetarchive\n- 7z (`7z` command)\n\n## Install `dokuWikiDumper`\n\n> `dokuWikiUploader` is included in `dokuWikiDumper`.\n\n### Install `dokuWikiDumper` with `pip` (recommended)\n\n> <https://pypi.org/project/dokuwikidumper/>\n\n```bash\npip3 install dokuWikiDumper\n```\n\n### Install `dokuWikiDumper` with `Poetry` (for developers)\n\n- Install `Poetry`\n\n    ```bash\n    pip3 install poetry\n    ```\n\n- Install `dokuWikiDumper`\n\n    ```bash\n    git clone https://github.com/saveweb/dokuwiki-dumper\n    cd dokuwiki-dumper\n    poetry install\n    rm dist/ -rf\n    poetry build\n    pip install --force-reinstall dist/dokuWikiDumper*.whl\n    ```\n\n## Usage\n\n```bash\nusage: dokuWikiDumper [-h] [--content] [--media] [--html] [--skip-to SKIP_TO] [--path PATH] [--no-resume] [--threads THREADS]\n                      [--insecure] [--ignore-errors] [--ignore-action-disabled-edit] [--username USERNAME] [--password PASSWORD]\n                      [--cookies COOKIES] [--auto]\n                      url\n\ndokuWikiDumper\n\npositional arguments:\n  url                   URL of the dokuWiki\n\noptions:\n  -h, --help            show this help message and exit\n  --content             Dump content\n  --media               Dump media\n  --html                Dump HTML\n  --pdf                 Dump PDF [default: false] (Only available on some wikis with the PDF export plugin) (Only dumps the latest PDF revision)\n  --current-only        Dump latest revision, no history [default: false] (only for HTML at the moment)\n  --skip-to SKIP_TO     !DEV! Skip to title number [default: 0]\n  --path PATH           Specify dump directory [default: <site>-<date>]\n  --no-resume           Do not resume a previous dump [default: resume]\n  --threads THREADS     Number of sub threads to use [default: 1], not recommended to set > 5\n  --insecure            Disable SSL certificate verification\n  --ignore-errors       !DANGEROUS! ignore errors in the sub threads. This may cause incomplete dumps.\n  --ignore-action-disabled-edit\n                        Some sites disable edit action for anonymous users and some core pages. This option will ignore this error and textarea not found error.But\n                        you may only get a partial dump. (only works with --content)\n  --username USERNAME   login: username\n  --password PASSWORD   login: password\n  --cookies COOKIES     cookies file\n  --auto                dump: content+media+html, threads=5, ignore-action-disable-edit\n```\n\nFor most cases, you can use `--auto` to dump the site.\n\n```bash\ndokuWikiDumper https://example.com/wiki/ --auto\n```\n\nwhich is equivalent to\n\n```bash\ndokuWikiDumper https://example.com/wiki/ --content --media --html --threads 5 --ignore-action-disabled-edit\n```\n\n> Highly recommend using `--username` and `--password` to login (or using `--cookies`), because some sites may disable anonymous users to access some pages or check the raw wikitext.\n\n`--cookies` accepts a Netscape cookies file, you can use [cookies.txt Extension](https://addons.mozilla.org/en-US/firefox/addon/cookies-txt/) to export cookies from Firefox. It also accepts a json cookies file created by [Cookie Quick Manager](https://addons.mozilla.org/en-US/firefox/addon/cookie-quick-manager/).\n\n## Dump structure\n\n<!-- Dump structure -->\n| Directory or File       | Description                                 |\n|-----------              |-------------                                |\n| `attic/`                | old revisions of page. (wikitext)           |\n| `dumpMeta/`             | (dokuWikiDumper only) metadata of the dump. |\n| `dumpMeta/check.html`   | ?do=check page of the wiki.                 |\n| `dumpMeta/config.json`  | dump\'s configuration.                       |\n| `dumpMeta/favicon.ico`  | favicon of the site.                        |\n| `dumpMeta/files.txt`    | list of filename.                           |\n| `dumpMeta/index.html`   | homepage of the wiki.                       |\n| `dumpMeta/info.json`    | infomations of the wiki.                    |\n| `dumpMeta/titles.txt`   | list of page title.                         |\n| `html/`                 | (dokuWikiDumper only) HTML of the pages.    |\n| `media/`                | media files.                                |\n| `meta/`                 | metadata of the pages.                      |\n| `pages/`                | latest page content. (wikitext)             |\n<!-- /Dump structure -->\n\n## Available Backups/Dumps\n\nI made some backups for testing, you can check out the list: <https://github.com/orgs/saveweb/projects/4>.\n\n> Some wikidump has been uploaded to IA, you can check out the list: <https://archive.org/search?query=subject%3A"dokuWikiDumper">\n> \n> If you dumped a DokuWiki and want to share it, please feel free to open an issue, I will add it to the list.\n\n## How to import dump to DokuWiki\n\nIf you need to import Dokuwiki, please add the following configuration to `local.php`\n\n```php\n$conf[\'fnencode\'] = \'utf-8\'; // Dokuwiki default: \'safe\' (url encode)\n# \'safe\' => Non-ASCII characters will be escaped as %xx form.\n# \'utf-8\' => Non-ASCII characters will be preserved as UTF-8 characters.\n\n$conf[\'compression\'] = \'0\'; // Dokuwiki default: \'gz\'.\n# \'gz\' => attic/<id>.<rev_id>.txt.gz\n# \'bz2\' => attic/<id>.<rev_id>.txt.bz2\n# \'0\' => attic/<id>.<rev_id>.txt\n```\n\nImport `pages` dir if you only need the latest version of the page.  \nImport `meta` dir if you need the **changelog** of the page.  \nImport `attic` and `meta` dirs if you need the old revisions **content** of the page.  \nImport `media` dir if you need the media files.\n\n`dumpMeta` and `html` dirs are only used by `dokuWikiDumper`, you can ignore it.\n\n## Information\n\n### DokuWiki links\n\n- [DokuWiki](https://www.dokuwiki.org/)\n- [DokuWiki changelog](https://www.dokuwiki.org/changelog)\n- [DokuWiki source code](https://github.com/splitbrain/dokuwiki)\n\n### Other tools\n\n- [MediaWiki Scraper](https://github.com/mediawiki-client-tools/mediawiki-scraper) (aka `wikiteam3`), a tool for archiving MediaWiki, forked from [WikiTeam](https://github.com/wikiteam/wikiteam/) and has been rewritten in Python 3.\n- [WikiTeam](https://github.com/wikiteam/wikiteam/), a tool for archiving MediaWiki, written in Python 2.\n\n## License\n\nGPLv3\n\n## Contributors\n\nThis tool is based on an unmerged PR (_8 years ago!_) of [WikiTeam](https://github.com/WikiTeam/wikiteam/): [DokuWiki dump alpha](https://github.com/WikiTeam/wikiteam/pull/243) by [@PiRSquared17](https://github.com/PiRSquared17).\n\nI ([@yzqzss](https://github.com/yzqzss)) have rewritten the code in Python 3 and added some features, also fixed some bugs.\n',
     'author': 'yzqzss',
     'author_email': 'yzqzss@yandex.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dokuwikidumper-0.1.7/PKG-INFO` & `dokuwikidumper-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dokuwikidumper
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for archiving DokuWiki
 License: GPL-3.0
 Author: yzqzss
 Author-email: yzqzss@yandex.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: internetarchive (>=3.3.0,<4.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Project-URL: Bug Tracker, https://github.com/saveweb/dokuwiki-dumper/issues
 Project-URL: repository, https://github.com/saveweb/dokuwiki-dumper/
 Description-Content-Type: text/markdown
 
 # DokuWiki Dumper
 
 > A tool for archiving DokuWiki.
@@ -30,14 +31,15 @@
 
 ### dokuWikiDumper
 
 - Python 3.8+ (developed on py3.10)
 - beautifulsoup4
 - requests
 - lxml
+- rich
 
 ### dokuWikiUploader
 
 > Upload wiki dump to [Internet Archive](https://archive.org/).
 > `dokuWikiUploader -h` for help.
 
 - internetarchive
@@ -145,14 +147,16 @@
 | `pages/`                | latest page content. (wikitext)             |
 <!-- /Dump structure -->
 
 ## Available Backups/Dumps
 
 I made some backups for testing, you can check out the list: <https://github.com/orgs/saveweb/projects/4>.
 
+> Some wikidump has been uploaded to IA, you can check out the list: <https://archive.org/search?query=subject%3A"dokuWikiDumper">
+> 
 > If you dumped a DokuWiki and want to share it, please feel free to open an issue, I will add it to the list.
 
 ## How to import dump to DokuWiki
 
 If you need to import Dokuwiki, please add the following configuration to `local.php`
 
 ```php
```

