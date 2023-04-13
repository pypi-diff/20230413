# Comparing `tmp/selfie-0.2.0-py2.py3-none-any.whl.zip` & `tmp/selfie-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 3163 bytes, number of entries: 5
--rwxr-xr-x  2.0 unx     5329 b- defN 20-Dec-03 20:41 selfie-0.2.0.data/scripts/selfie
--rw-r--r--  2.0 unx      284 b- defN 20-Dec-03 20:41 selfie-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Dec-03 20:41 selfie-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 20-Dec-03 20:41 selfie-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      382 b- defN 20-Dec-03 20:41 selfie-0.2.0.dist-info/RECORD
-5 files, 6106 bytes uncompressed, 2449 bytes compressed:  59.9%
+Zip file size: 3874 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      624 b- defN 23-Apr-13 20:21 selfie/__init__.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Apr-13 20:16 selfie/__version__.py
+-rwxr-xr-x  2.0 unx     5085 b- defN 23-Apr-13 20:24 selfie-0.3.0.data/scripts/selfie
+-rw-r--r--  2.0 unx      239 b- defN 23-Apr-13 20:24 selfie-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-13 20:24 selfie-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-13 20:24 selfie-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      533 b- defN 23-Apr-13 20:24 selfie-0.3.0.dist-info/RECORD
+7 files, 6855 bytes uncompressed, 2930 bytes compressed:  57.3%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: selfie-0.2.0.data/scripts/selfie
+Filename: selfie/__init__.py
 Comment: 
 
-Filename: selfie-0.2.0.dist-info/METADATA
+Filename: selfie/__version__.py
 Comment: 
 
-Filename: selfie-0.2.0.dist-info/WHEEL
+Filename: selfie-0.3.0.data/scripts/selfie
 Comment: 
 
-Filename: selfie-0.2.0.dist-info/top_level.txt
+Filename: selfie-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: selfie-0.2.0.dist-info/RECORD
+Filename: selfie-0.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: selfie-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: selfie-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `selfie-0.2.0.data/scripts/selfie` & `selfie-0.3.0.data/scripts/selfie`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,30 @@
 import socket
 import hashlib
 import logging
 import getpass as gp
 import datetime as dt
 import argparse as ap
 import subprocess as sp
+from selfie import getenv
 
 logger = logging.getLogger(__name__)
 
 def main():
     parser = ap.ArgumentParser()
     parser.add_argument('-o', '--output-file', type=os.path.expanduser,
         help='Output provenance file')
     parser.add_argument('-l', '--lock', action='store_true',
         help='Lock the provenance file for duration of subprocess')
     parser.add_argument('-m', '--mask',
         help='Comma separated list of environment variables to mask out')
     parser.add_argument('-p', '--polling-interval', default=0.5,
         help='How frequently to check for process termination, in seconds')
+    parser.add_argument('-e', '--include-env', action='store_true',
+        help='Include environment variables in output file')
     parser.add_argument('command', nargs=ap.REMAINDER)
     parser.add_argument('-v', '--verbose', action='store_true',
         help='Increase verbosity')
     args = parser.parse_args()
 
     level = logging.INFO
     if args.verbose:
@@ -68,21 +71,23 @@
         'start_time': dt.datetime.fromtimestamp(start).strftime('%H:%M:%S'),
         'end': None,
         'end_date': None,
         'end_time': None,
         'username': gp.getuser(),
         'mtime': dt.datetime.fromtimestamp(os.path.getmtime(exe)).isoformat(),
         'cwd': cwd,
-        'os': getOS(),
+        'os': getos(),
         'cpu': getcpu(),
         'hostname': socket.gethostname(),
-        'dist': getDistro(),
-        'elapsed': None,
-        'env': getenv(mask=args.mask)
+        'dist': getdistro(),
+        'elapsed': None
     }
+    # add environment variables
+    if args.include_env:
+        P['env'] = getenv(mask=args.mask)
     # write the provenance file and lock it
     if args.output_file:
         fd = os.open(args.output_file, os.O_RDWR|os.O_CREAT)
         fo = os.fdopen(fd, 'w')
         if args.lock:
             try:
                 logger.debug('locking %s', args.output_file)
@@ -118,19 +123,19 @@
         fo.write(json.dumps(P, indent=2))
         fo.flush()
         os.fsync(fd)
         fo.close()
     # exit with returncode of subprocess
     sys.exit(int(proc.returncode))
 
-def getDistro():
+def getdistro():
     output = sp.check_output(['cat', '/etc/system-release']).strip()
     return output.decode()
 
-def getOS():
+def getos():
     output = sp.check_output(['uname', '-a']).strip()
     return output.decode()
 
 def which(x):
     for p in os.environ.get('PATH').split(os.pathsep):
         p = os.path.join(p, x)
         if os.path.exists(p):
@@ -152,24 +157,9 @@
     pass
 
 def sha512file(f):
     f = os.path.expanduser(f)
     with open(f, 'rb') as fo:
         return hashlib.sha512(fo.read()).hexdigest()
 
-def getenv(mask=None, mask_file='~/.config/selfie/ignore'):
-    if not mask:
-        mask = list()
-    mask_file = os.path.expanduser(mask_file)
-    if os.path.exists(mask_file):
-        with open(mask_file) as fo:
-            mask.extend(fo.read().splitlines())
-    environ = dict()
-    for k,v in os.environ.items():
-        for pattern in mask:
-            if re.match(pattern, k):
-                v = '********'
-        environ[k] = v
-    return environ
-
 if __name__ == '__main__':
     main()
```

