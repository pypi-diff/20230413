# Comparing `tmp/purgelogs-0.2.0.tar.gz` & `tmp/purgelogs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purgelogs-0.2.0.tar", last modified: Mon Aug 29 18:19:27 2022, max compression
+gzip compressed data, was "purgelogs-0.2.1.tar", last modified: Thu Apr 13 07:29:48 2023, max compression
```

## Comparing `purgelogs-0.2.0.tar` & `purgelogs-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 18:19:27.694030 purgelogs-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      183 2022-08-29 18:19:27.694030 purgelogs-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       37 2022-08-29 18:19:00.000000 purgelogs-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 18:19:27.693029 purgelogs-0.2.0/purgelogs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      183 2022-08-29 18:19:27.000000 purgelogs-0.2.0/purgelogs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      199 2022-08-29 18:19:27.000000 purgelogs-0.2.0/purgelogs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-29 18:19:27.000000 purgelogs-0.2.0/purgelogs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-08-29 18:19:27.000000 purgelogs-0.2.0/purgelogs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-08-29 18:19:27.000000 purgelogs-0.2.0/purgelogs.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)     4523 2022-08-29 18:19:00.000000 purgelogs-0.2.0/purgelogs.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-29 18:19:27.694030 purgelogs-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      772 2022-08-29 18:19:00.000000 purgelogs-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:29:48.113049 purgelogs-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-13 07:28:31.000000 purgelogs-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-13 07:29:48.112049 purgelogs-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-13 07:28:31.000000 purgelogs-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:29:48.112049 purgelogs-0.2.1/purgelogs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-13 07:29:48.000000 purgelogs-0.2.1/purgelogs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)     4644 2023-04-13 07:28:32.000000 purgelogs-0.2.1/purgelogs.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 07:29:48.113049 purgelogs-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-13 07:28:32.000000 purgelogs-0.2.1/setup.py
```

### Comparing `purgelogs-0.2.0/purgelogs.py` & `purgelogs-0.2.1/purgelogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,19 @@
 def usage(argv: List[str]) -> argparse.Namespace:
     """The script usage
 
     >>> usage([])
     Namespace(debug=False, dry_run=False, log_path_dir='/var/www/logs', loop=None, retention_days=31)
     """
     parser = argparse.ArgumentParser(description="Purge old logs")
+    parser.add_argument('--debug', action='store_true')
     parser.add_argument('--dry-run', action='store_true')
-    parser.add_argument('--retention-days', type=int, default=31)
     parser.add_argument('--log-path-dir', default='/var/www/logs')
-    parser.add_argument('--debug', action='store_true')
     parser.add_argument('--loop', type=int, metavar="SECONDS", help="Continuously run every SECONDS")
+    parser.add_argument('--retention-days', type=int, default=31)
     return parser.parse_args(argv)
 
 def setup_logging(debug: bool) -> Logger:
     """Create the logger with a nice format string"""
     logging.basicConfig(
         format='%(asctime)s %(levelname)-5.5s %(message)s',
         level=logging.DEBUG if debug else logging.INFO)
@@ -112,14 +112,16 @@
     root = check_dir_path(args.log_path_dir)
     calculated_time = datetime.now() - timedelta(days=args.retention_days)
     log = setup_logging(args.debug)
     if not root:
         log.error("The provided log path dir does not exists")
         exit(1)
     while True:
+        logging.info("Starting cleaning-up log dir...")
         search_and_destroy(log, calculated_time, args.dry_run, root)
         if not args.loop:
             break
+        logging.info("Cleanup done! Sleeping %s..." % args.loop)
         time.sleep(args.loop)
 
 if __name__ == "__main__":
     main()
```

### Comparing `purgelogs-0.2.0/setup.py` & `purgelogs-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from setuptools import setup
 
 setup(
     name='purgelogs',
-    version='0.2.0',
+    version='0.2.1',
     py_modules=['purgelogs'],
     entry_points = {
         'console_scripts': ['purgelogs=purgelogs:main']
     }
 )
```

