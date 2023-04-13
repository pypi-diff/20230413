# Comparing `tmp/env_color_logger-0.0.1.tar.gz` & `tmp/env_color_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_color_logger-0.0.1.tar", last modified: Thu Apr 13 17:47:32 2023, max compression
+gzip compressed data, was "env_color_logger-0.0.3.tar", last modified: Thu Apr 13 18:31:00 2023, max compression
```

## Comparing `env_color_logger-0.0.1.tar` & `env_color_logger-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:47:32.221103 env_color_logger-0.0.1/
--rw-rw-rw-   0        0        0      456 2023-04-13 17:47:32.219624 env_color_logger-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-04-13 12:30:30.000000 env_color_logger-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:47:32.203113 env_color_logger-0.0.1/env_color_logger/
--rw-rw-rw-   0        0        0     1911 2023-04-13 12:09:11.000000 env_color_logger-0.0.1/env_color_logger/__init__.py
--rw-rw-rw-   0        0        0     1095 2023-04-13 12:00:43.000000 env_color_logger-0.0.1/env_color_logger/color.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:47:32.217584 env_color_logger-0.0.1/env_color_logger.egg-info/
--rw-rw-rw-   0        0        0      456 2023-04-13 17:47:32.000000 env_color_logger-0.0.1/env_color_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-13 17:47:32.000000 env_color_logger-0.0.1/env_color_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:47:32.000000 env_color_logger-0.0.1/env_color_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 17:47:32.000000 env_color_logger-0.0.1/env_color_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 17:47:32.221103 env_color_logger-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-04-13 17:44:22.000000 env_color_logger-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:31:00.561982 env_color_logger-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 18:30:51.000000 env_color_logger-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-13 18:31:00.561982 env_color_logger-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-13 18:30:51.000000 env_color_logger-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:31:00.561982 env_color_logger-0.0.3/env_color_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-13 18:30:51.000000 env_color_logger-0.0.3/env_color_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 18:30:51.000000 env_color_logger-0.0.3/env_color_logger/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:31:00.561982 env_color_logger-0.0.3/env_color_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-13 18:31:00.000000 env_color_logger-0.0.3/env_color_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 18:31:00.000000 env_color_logger-0.0.3/env_color_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:31:00.000000 env_color_logger-0.0.3/env_color_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 18:31:00.000000 env_color_logger-0.0.3/env_color_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:31:00.561982 env_color_logger-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 18:30:51.000000 env_color_logger-0.0.3/setup.py
```

### Comparing `env_color_logger-0.0.1/env_color_logger/__init__.py` & `env_color_logger-0.0.3/env_color_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `env_color_logger-0.0.1/env_color_logger/color.py` & `env_color_logger-0.0.3/env_color_logger/color.py`

 * *Files identical despite different names*

### Comparing `env_color_logger-0.0.1/setup.py` & `env_color_logger-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from pathlib import Path
-
-from setuptools import setup
-
-long_description = Path(__file__).with_name("README.md").read_text(encoding="utf-8")
-
-requirements = Path(__file__).with_name("requirements.txt").read_text().split()
-
-setup(
-    name="env_color_logger",
-    version="0.0.1",
-    packages=["env_color_logger"],
-    url="https://github.com/ofersadan85/env_color_logger",
-    license="MIT License",
-    author="Ofer Sadan",
-    author_email="ofersadan85@gmail.com",
-    description="Simple logging using env variables",
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.11",
-    ],
-    include_package_data=True,
-)
+from pathlib import Path
+
+from setuptools import setup
+
+long_description = Path(__file__).with_name("README.md").read_text(encoding="utf-8")
+requirements = Path(__file__).with_name("requirements.txt").read_text().split()
+
+setup(
+    name="env_color_logger",
+    version="0.0.3",
+    packages=["env_color_logger"],
+    url="https://github.com/ofersadan85/env_color_logger",
+    license="MIT License",
+    author="Ofer Sadan",
+    author_email="ofersadan85@gmail.com",
+    description="Simple logging using env variables",
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.11",
+    ],
+    include_package_data=True,
+)
```

