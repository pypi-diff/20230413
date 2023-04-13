# Comparing `tmp/tcw-0.0.9.tar.gz` & `tmp/tcw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcw-0.0.9.tar", last modified: Wed Dec 21 05:52:16 2022, max compression
+gzip compressed data, was "tcw-0.1.0.tar", last modified: Thu Apr 13 11:26:27 2023, max compression
```

## Comparing `tcw-0.0.9.tar` & `tcw-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.0.9/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2022-12-21 05:52:16.911610 tcw-0.0.9/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.0.9/README.md
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2022-12-21 05:52:16.911610 tcw-0.0.9/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      564 2022-12-20 22:01:31.000000 tcw-0.0.9/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1615 2022-12-21 05:31:36.000000 tcw-0.0.9/tcw/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/apps/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/apps/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/apps/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/apps/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.0.9/tcw/apps/contest/forms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3475 2022-12-21 05:16:49.000000 tcw-0.0.9/tcw/apps/contest/models.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/apps/contest/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/apps/contest/templates/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/apps/contest/templates/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/apps/contest/templates/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3166 2022-12-21 05:48:23.000000 tcw-0.0.9/tcw/apps/contest/views.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.0.9/tcw/config.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      166 2022-12-19 06:59:06.000000 tcw-0.0.9/tcw/run.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/srv.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/static/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/static/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/static/images/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/static/images/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.0.9/tcw/templates/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.0.9/tcw/utils.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2022-12-21 05:52:16.911610 tcw-0.0.9/tcw.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2022-12-21 05:52:16.000000 tcw-0.0.9/tcw.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      535 2022-12-21 05:52:16.000000 tcw-0.0.9/tcw.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2022-12-21 05:52:16.000000 tcw-0.0.9/tcw.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       45 2022-12-21 05:52:16.000000 tcw-0.0.9/tcw.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2022-12-21 05:52:16.000000 tcw-0.0.9/tcw.egg-info/top_level.txt
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.0/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-04-13 11:26:27.403007 tcw-0.1.0/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.0/README.md
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-04-13 11:26:27.403007 tcw-0.1.0/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-04-13 11:12:51.000000 tcw-0.1.0/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1615 2022-12-21 05:31:36.000000 tcw-0.1.0/tcw/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.1.0/tcw/apps/contest/forms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3534 2023-01-01 20:54:30.000000 tcw-0.1.0/tcw/apps/contest/models.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/contest/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/contest/templates/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/contest/templates/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/contest/templates/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3313 2023-01-21 12:31:08.000000 tcw-0.1.0/tcw/apps/contest/views.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.1.0/tcw/config.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      166 2023-04-13 11:23:23.000000 tcw-0.1.0/tcw/run.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/srv.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/static/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/static/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/static/images/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/static/images/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/templates/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.1.0/tcw/utils.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      535 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/top_level.txt
```

### Comparing `tcw-0.0.9/LICENSE` & `tcw-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/PKG-INFO` & `tcw-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.0.9
+Version: 0.1.0
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.0.9/README.md` & `tcw-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/setup.py` & `tcw-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tcw',
-    version='0.0.9',
+    version='0.1.0',
     author='J Leary',
     author_email='tinycontestwinners@gmail.com',
     description='tiny contest winners application',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
         'flask',
         'flask-wtf',
         'sqlalchemy',
         'markdown',
-        'gunicorn',
     ],
 )
```

### Comparing `tcw-0.0.9/tcw/__init__.py` & `tcw-0.1.0/tcw/__init__.py`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/tcw/apps/contest/forms.py` & `tcw-0.1.0/tcw/apps/contest/forms.py`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/tcw/apps/contest/models.py` & `tcw-0.1.0/tcw/apps/contest/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,17 @@
             None
         returns:
             list - a list of winning names
         """
 
         results = []
         nwinners = self.winners
+        if len(self.entrants) == 0:
+            return []
+
         if len(self.entrants) < self.winners:
             nwinners = len(self.entrants)
 
         choices = [e.name for e in self.entrants]
         while len(results) < self.winners:
             name = secrets.choice(choices)
             if name not in results:
```

### Comparing `tcw-0.0.9/tcw/apps/contest/views.py` & `tcw-0.1.0/tcw/apps/contest/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import datetime
+import logging
 from flask import (Blueprint, render_template, redirect, request, abort,
     url_for, Response)
 from sqlalchemy.exc import IntegrityError
 from tcw.database import session
 from tcw.utils import (contest_by_name, fossil_by_name, random_name,
     expires_time)
 from .forms import ContestForm, SignupForm
 from .models import Contest, Entrant
 
 
+logger = logging.getLogger(__name__)
 bp = Blueprint('contest', __name__, template_folder='templates')
 
 
 @bp.route('/', methods=['GET'])
 def index():
     return render_template('contest/index.html')
 
@@ -44,28 +46,30 @@
 
         try:
             obj = Contest(**options)
             session.add(obj)
             session.commit()
             options['expires'] = options['expires'].isoformat() + "Z"
         except Exception as x:
-            abort(404, str(x))
+            logger.warning(x)
+            abort(404)
 
         return redirect(url_for('contest.success', **options))
 
     return render_template('contest/form.html', form=form)
 
 
 @bp.route('/signup', methods=['GET', 'POST'])
 def signup():
     form = SignupForm()
 
     try:
         name = request.args.get('name')
-    except:
+    except Exception as x:
+        logger.warning(x)
         abort(404)
 
     try:
         contest = contest_by_name(name)
     except:
         try:
             fossil = fossil_by_name(name)
@@ -89,15 +93,16 @@
                 url_for('contest.thanks',
                     contest=contest.title,
                     entrant=form.name.data), code=303)
         except IntegrityError:
             session.rollback()
             return render_template('contest/sorry.html',
                 contest=contest, form=form)
-        except:
+        except Exception as x:
+            logg
             abort(404)
     else:
         return render_template('contest/signup.html',
             contest=contest, form=form)
 
 
 @bp.route('/success', methods=['GET'])
```

### Comparing `tcw-0.0.9/tcw/config.py` & `tcw-0.1.0/tcw/config.py`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/tcw/database.py` & `tcw-0.1.0/tcw/database.py`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/tcw/utils.py` & `tcw-0.1.0/tcw/utils.py`

 * *Files identical despite different names*

### Comparing `tcw-0.0.9/tcw.egg-info/PKG-INFO` & `tcw-0.1.0/tcw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.0.9
+Version: 0.1.0
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.0.9/tcw.egg-info/SOURCES.txt` & `tcw-0.1.0/tcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

