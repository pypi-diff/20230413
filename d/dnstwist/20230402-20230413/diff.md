# Comparing `tmp/dnstwist-20230402.tar.gz` & `tmp/dnstwist-20230413.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnstwist-20230402.tar", last modified: Sun Apr  2 12:42:42 2023, max compression
+gzip compressed data, was "dnstwist-20230413.tar", last modified: Thu Apr 13 07:31:33 2023, max compression
```

## Comparing `dnstwist-20230402.tar` & `dnstwist-20230413.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-04-02 12:42:42.612799 dnstwist-20230402/
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-04-02 12:42:42.612799 dnstwist-20230402/PKG-INFO
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     9422 2023-04-02 12:37:37.000000 dnstwist-20230402/README.md
-drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-04-02 12:42:42.612799 dnstwist-20230402/dnstwist.egg-info/
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-04-02 12:42:42.000000 dnstwist-20230402/dnstwist.egg-info/PKG-INFO
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      224 2023-04-02 12:42:42.000000 dnstwist-20230402/dnstwist.egg-info/SOURCES.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        1 2023-04-02 12:42:42.000000 dnstwist-20230402/dnstwist.egg-info/dependency_links.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       43 2023-04-02 12:42:42.000000 dnstwist-20230402/dnstwist.egg-info/entry_points.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       89 2023-04-02 12:42:42.000000 dnstwist-20230402/dnstwist.egg-info/requires.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        9 2023-04-02 12:42:42.000000 dnstwist-20230402/dnstwist.egg-info/top_level.txt
--rwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)    43397 2023-04-02 12:42:09.000000 dnstwist-20230402/dnstwist.py
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       38 2023-04-02 12:42:42.612799 dnstwist-20230402/setup.cfg
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     1163 2023-03-02 11:24:31.000000 dnstwist-20230402/setup.py
+drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-04-13 07:31:33.392742 dnstwist-20230413/
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-04-13 07:31:33.392742 dnstwist-20230413/PKG-INFO
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     9422 2023-04-02 12:37:37.000000 dnstwist-20230413/README.md
+drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-04-13 07:31:33.392742 dnstwist-20230413/dnstwist.egg-info/
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/PKG-INFO
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      224 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        1 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       43 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/entry_points.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      104 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/requires.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        9 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/top_level.txt
+-rwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)    43475 2023-04-13 07:31:22.000000 dnstwist-20230413/dnstwist.py
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       38 2023-04-13 07:31:33.392742 dnstwist-20230413/setup.cfg
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     1163 2023-03-02 11:24:31.000000 dnstwist-20230413/setup.py
```

### Comparing `dnstwist-20230402/PKG-INFO` & `dnstwist-20230413/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnstwist
-Version: 20230402
+Version: 20230413
 Summary: Domain name permutation engine for detecting homograph phishing attacks, typo squatting, and brand impersonation
 Home-page: https://github.com/elceef/dnstwist
 Author: Marcin Ulikowski
 Author-email: marcin@ulikowski.pl
 License: ASL 2.0
 Description: Project website: https://github.com/elceef/dnstwist
 Platform: UNKNOWN
```

### Comparing `dnstwist-20230402/README.md` & `dnstwist-20230413/README.md`

 * *Files identical despite different names*

### Comparing `dnstwist-20230402/dnstwist.egg-info/PKG-INFO` & `dnstwist-20230413/dnstwist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnstwist
-Version: 20230402
+Version: 20230413
 Summary: Domain name permutation engine for detecting homograph phishing attacks, typo squatting, and brand impersonation
 Home-page: https://github.com/elceef/dnstwist
 Author: Marcin Ulikowski
 Author-email: marcin@ulikowski.pl
 License: ASL 2.0
 Description: Project website: https://github.com/elceef/dnstwist
 Platform: UNKNOWN
```

### Comparing `dnstwist-20230402/dnstwist.py` & `dnstwist-20230413/dnstwist.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 '''
 
 __author__ = 'Marcin Ulikowski'
-__version__ = '20230402'
+__version__ = '20230413'
 __email__ = 'marcin@ulikowski.pl'
 
 import re
 import sys
 import socket
 socket.setdefaulttimeout(10.0)
 import signal
@@ -40,14 +40,15 @@
 import smtplib
 import json
 import queue
 import urllib.request
 import urllib.parse
 import gzip
 from io import BytesIO
+import contextlib
 
 def _debug(msg):
 	if 'DEBUG' in os.environ:
 		if isinstance(msg, Exception):
 			print('{}:{} {}'.format(__file__, msg.__traceback__.tb_lineno, str(msg)), file=sys.stderr, flush=True)
 		else:
 			print(str(msg), file=sys.stderr, flush=True)
@@ -626,14 +627,15 @@
 		return sorted(domains)
 
 
 class Scanner(threading.Thread):
 	def __init__(self, queue):
 		threading.Thread.__init__(self)
 		self._stop_event = threading.Event()
+		self.daemon = True
 		self.id = 0
 		self.jobs = queue
 		self.lsh_init = ''
 		self.lsh_effective_url = ''
 		self.phash_init = None
 		self.screenshot_dir = None
 		self.url = None
@@ -1233,15 +1235,14 @@
 
 	for task in domains:
 		jobs.put(task)
 
 	sid = int.from_bytes(os.urandom(4), sys.byteorder)
 	for _ in range(args.threads):
 		worker = Scanner(jobs)
-		worker.daemon = True
 		worker.id = sid
 		worker.url = url
 		worker.option_extdns = MODULE_DNSPYTHON
 		if args.geoip:
 			worker.option_geoip = True
 		if args.banners:
 			worker.option_banners = True
@@ -1288,18 +1289,18 @@
 
 	if args.whois:
 		total = sum([1 for x in domains if x.is_registered()])
 		for i, domain in enumerate([x for x in domains if x.is_registered()]):
 			p_cli(ST_CLR + '\rWHOIS: {} ({:.2%})'.format(domain['domain'], (i+1)/total))
 			try:
 				_, dom, tld = domain_tld(domain['domain'])
-				whoisq = whois.query('.'.join([dom, tld]))
+				with open(os.devnull, 'w') as devnull, contextlib.redirect_stderr(devnull):
+					whoisq = whois.query('.'.join([dom, tld]))
 			except Exception as e:
-				if args.debug:
-					p_err(e)
+				_debug(e)
 			else:
 				if whoisq is None:
 					continue
 				if whoisq.creation_date:
 					domain['whois_created'] = str(whoisq.creation_date).split(' ')[0]
 				if whoisq.registrar:
 					domain['whois_registrar'] = str(whoisq.registrar)
```

### Comparing `dnstwist-20230402/setup.py` & `dnstwist-20230413/setup.py`

 * *Files identical despite different names*

