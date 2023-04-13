# Comparing `tmp/tcw-tasks-0.3.0.tar.gz` & `tmp/tcw-tasks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcw-tasks-0.3.0.tar", last modified: Sun Feb  5 05:45:00 2023, max compression
+gzip compressed data, was "tcw-tasks-0.4.0.tar", last modified: Thu Apr 13 11:30:27 2023, max compression
```

## Comparing `tcw-tasks-0.3.0.tar` & `tcw-tasks-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-05 05:45:00.268934 tcw-tasks-0.3.0/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-01 04:24:20.000000 tcw-tasks-0.3.0/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      293 2023-02-05 05:45:00.268934 tcw-tasks-0.3.0/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       74 2022-12-01 04:28:02.000000 tcw-tasks-0.3.0/README.md
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-02-05 05:45:00.268934 tcw-tasks-0.3.0/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      646 2023-02-05 05:40:39.000000 tcw-tasks-0.3.0/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-05 05:45:00.264934 tcw-tasks-0.3.0/tcw_tasks/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-11-20 20:32:55.000000 tcw-tasks-0.3.0/tcw_tasks/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1995 2022-12-20 21:56:03.000000 tcw-tasks-0.3.0/tcw_tasks/models.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2501 2022-12-21 05:17:24.000000 tcw-tasks-0.3.0/tcw_tasks/notify.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2561 2022-12-20 21:51:36.000000 tcw-tasks-0.3.0/tcw_tasks/templates.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      767 2023-02-05 05:36:51.000000 tcw-tasks-0.3.0/tcw_tasks/utils.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-05 05:45:00.268934 tcw-tasks-0.3.0/tcw_tasks.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      293 2023-02-05 05:45:00.000000 tcw-tasks-0.3.0/tcw_tasks.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      330 2023-02-05 05:45:00.000000 tcw-tasks-0.3.0/tcw_tasks.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-02-05 05:45:00.000000 tcw-tasks-0.3.0/tcw_tasks.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       52 2023-02-05 05:45:00.000000 tcw-tasks-0.3.0/tcw_tasks.egg-info/entry_points.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       28 2023-02-05 05:45:00.000000 tcw-tasks-0.3.0/tcw_tasks.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       10 2023-02-05 05:45:00.000000 tcw-tasks-0.3.0/tcw_tasks.egg-info/top_level.txt
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:30:27.272335 tcw-tasks-0.4.0/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-01 04:24:20.000000 tcw-tasks-0.4.0/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      293 2023-04-13 11:30:27.272335 tcw-tasks-0.4.0/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       74 2022-12-01 04:28:02.000000 tcw-tasks-0.4.0/README.md
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-04-13 11:30:27.272335 tcw-tasks-0.4.0/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      645 2023-04-13 11:13:18.000000 tcw-tasks-0.4.0/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:30:27.268335 tcw-tasks-0.4.0/tcw_tasks/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-11-20 20:32:55.000000 tcw-tasks-0.4.0/tcw_tasks/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2002 2023-04-13 11:18:04.000000 tcw-tasks-0.4.0/tcw_tasks/models.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2539 2023-04-13 11:20:18.000000 tcw-tasks-0.4.0/tcw_tasks/notify.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2570 2023-04-13 11:15:20.000000 tcw-tasks-0.4.0/tcw_tasks/templates.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      767 2023-02-05 05:36:51.000000 tcw-tasks-0.4.0/tcw_tasks/utils.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:30:27.272335 tcw-tasks-0.4.0/tcw_tasks.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      293 2023-04-13 11:30:27.000000 tcw-tasks-0.4.0/tcw_tasks.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      330 2023-04-13 11:30:27.000000 tcw-tasks-0.4.0/tcw_tasks.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-04-13 11:30:27.000000 tcw-tasks-0.4.0/tcw_tasks.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       52 2023-04-13 11:30:27.000000 tcw-tasks-0.4.0/tcw_tasks.egg-info/entry_points.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       27 2023-04-13 11:30:27.000000 tcw-tasks-0.4.0/tcw_tasks.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       10 2023-04-13 11:30:27.000000 tcw-tasks-0.4.0/tcw_tasks.egg-info/top_level.txt
```

### Comparing `tcw-tasks-0.3.0/LICENSE` & `tcw-tasks-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcw-tasks-0.3.0/setup.py` & `tcw-tasks-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tcw-tasks',
-    version='0.3.0',
+    version='0.4.0',
     author='J Leary',
     author_email='tinycontestwinners@gmail.com',
     description='contest cleanup script for tcw app',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
-        'tcw>=0.0.11',
+        'tcw>=0.1.0',
         'jinja2',
         'sendgrid',
     ],
     entry_points={
         'console_scripts': [
             'tcwinners = tcw_tasks.notify:main',
         ]
```

### Comparing `tcw-tasks-0.3.0/tcw_tasks/models.py` & `tcw-tasks-0.4.0/tcw_tasks/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Create email message for a finished contest
     """
 
     def __init__(self, *args, **kwargs):
         self.contest = None
         self.winners = []
         self.mail_from = os.getenv('TCW_MAIL_FROM', 'user@localhost')
-        self.subject = 'Your Contest Kitty contest results'
+        self.subject = 'Your Tiny Contest Winners contest results'
         for k, v in kwargs.items():
             if hasattr(self, k):
                 setattr(self, k, v)
 
         if self.contest is None:
             raise Exception('Contest object required')
```

### Comparing `tcw-tasks-0.3.0/tcw_tasks/notify.py` & `tcw-tasks-0.4.0/tcw_tasks/notify.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,21 @@
     if not uri:
         logger.error('Must have SQLALCHEMY_DATABASE_URI environment var')
         sys.exit(1)
 
     init_engine(uri)
     logger.info("STARTING. Debug=%s" % args.debug)
 
+    '''
     while True:
         finish_contests()
         logger.debug("Sleeping...")
         time.sleep(60)
+    '''
+    finish_contests()
 
 
 def finish_contests():
     contests = []
     now = datetime.datetime.utcnow()
 
     try:
```

### Comparing `tcw-tasks-0.3.0/tcw_tasks/templates.py` & `tcw-tasks-0.4.0/tcw_tasks/templates.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 Thank You!
 {%- else %}
 Sorry. There were no winners selected, because no one signed up.
 {% endif %}
 
 Please do not respond directly to this e-mail. The originating e-mail account is not monitored.
 
-thecontestkitty.com
+tinycontestwinners.com
 """
 
 HTML_TEMPLATE = """
 <html>
   <head>
     <style>
       .container {
@@ -80,15 +80,15 @@
         </div>
         <footer>
             <p>
             It is your responsibilty to contact the winners.
             Please do not respond directly to this e-mail. The originating e-mail account is not monitored.
             </p>
             <p>
-            <a href="https://thecontestkitty.com">thecontestkitty.com</a>
+            <a href="https://tinycontestwinners.com">tinycontestwinners.com</a>
             </p>
         </footer>
         {%- else %}
         <p>Sorry. There were no winners selected, because no one signed up.</p>
         {% endif %}
       </div>
     </div>
```

#### html2text {}

```diff
@@ -2,27 +2,27 @@
 STATISTICS: - max_entrants: {{ contest.max_entrants }} - number of winners: {
 { winners | length }} - sign ups: {{ contest.entrants | length }} - expired: {
 { contest.expires.strftime('%Y-%m-%d %H:%M:%S') }} UTC {% if winners | length -
 %} THE WINNERS: {% for winner in winners -%} {{ loop.index }}. {{ winner }} {%
 endfor %} It is your responsibilty to contact the winners. Thank You! {%- else
 %} Sorry. There were no winners selected, because no one signed up. {% endif %}
 Please do not respond directly to this e-mail. The originating e-mail account
-is not monitored. thecontestkitty.com """ HTML_TEMPLATE = """
+is not monitored. tinycontestwinners.com """ HTML_TEMPLATE = """
 **** Contest Expired ****
 {{ contest.title }}
 **** Statistics ****
 max entrants = {{ contest.max_entrants }}
 number of winners = {{ winners | length }}
 sign-ups = {{ contest.entrants | length }}
 expired = {{ contest.expires.strftime('%Y-%m-%d %H:%M:%S') }} UTC
 {% if winners | length %}
 **** The Winners ****
    1. {% for winner in winners -%}
    2. {{ winner }}
    3. {% endfor %}
 It is your responsibilty to contact the winners. Please do not respond directly
 to this e-mail. The originating e-mail account is not monitored.
-thecontestkitty.com
+tinycontestwinners.com
  {%- else %}
 Sorry. There were no winners selected, because no one signed up.
 {% endif %}
 """
```

### Comparing `tcw-tasks-0.3.0/tcw_tasks/utils.py` & `tcw-tasks-0.4.0/tcw_tasks/utils.py`

 * *Files identical despite different names*

