# Comparing `tmp/awscli_mate-0.3.1.tar.gz` & `tmp/awscli_mate-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awscli_mate-0.3.1.tar", last modified: Fri Apr  7 03:48:53 2023, max compression
+gzip compressed data, was "awscli_mate-0.3.2.tar", last modified: Wed Apr 12 22:17:16 2023, max compression
```

## Comparing `awscli_mate-0.3.1.tar` & `awscli_mate-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-07 03:48:53.928111 awscli_mate-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-04-04 15:13:55.000000 awscli_mate-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1121 2023-04-04 15:13:55.000000 awscli_mate-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      319 2023-04-04 15:13:55.000000 awscli_mate-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5374 2023-04-07 03:48:53.927967 awscli_mate-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4274 2023-04-07 03:18:16.000000 awscli_mate-0.3.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-07 03:48:53.925868 awscli_mate-0.3.1/awscli_mate/
--rw-r--r--   0 sanhehu    (501) staff       (20)      630 2023-04-07 02:45:19.000000 awscli_mate-0.3.1/awscli_mate/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-04-07 02:46:19.000000 awscli_mate-0.3.1/awscli_mate/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-04-07 02:48:38.000000 awscli_mate-0.3.1/awscli_mate/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8578 2023-04-07 03:35:48.000000 awscli_mate-0.3.1/awscli_mate/awscli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      707 2023-04-06 01:57:32.000000 awscli_mate-0.3.1/awscli_mate/cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      636 2023-04-04 17:52:15.000000 awscli_mate-0.3.1/awscli_mate/constants.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-07 03:48:53.926874 awscli_mate-0.3.1/awscli_mate/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-04-04 15:13:55.000000 awscli_mate-0.3.1/awscli_mate/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      245 2023-04-07 02:32:41.000000 awscli_mate-0.3.1/awscli_mate/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      307 2023-04-04 18:03:25.000000 awscli_mate-0.3.1/awscli_mate/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-07 03:48:53.927639 awscli_mate-0.3.1/awscli_mate/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-04-04 15:56:46.000000 awscli_mate-0.3.1/awscli_mate/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-04-02 05:07:43.000000 awscli_mate-0.3.1/awscli_mate/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-04-02 05:07:43.000000 awscli_mate-0.3.1/awscli_mate/tests/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-07 03:48:53.926718 awscli_mate-0.3.1/awscli_mate.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5374 2023-04-07 03:48:53.000000 awscli_mate-0.3.1/awscli_mate.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      655 2023-04-07 03:48:53.000000 awscli_mate-0.3.1/awscli_mate.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-04-07 03:48:53.000000 awscli_mate-0.3.1/awscli_mate.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-04-07 03:48:53.000000 awscli_mate-0.3.1/awscli_mate.egg-info/entry_points.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      248 2023-04-07 03:48:53.000000 awscli_mate-0.3.1/awscli_mate.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       12 2023-04-07 03:48:53.000000 awscli_mate-0.3.1/awscli_mate.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1276 2023-04-07 03:39:55.000000 awscli_mate-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-04-07 03:08:21.000000 awscli_mate-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-04-04 15:13:55.000000 awscli_mate-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      196 2023-04-07 03:08:26.000000 awscli_mate-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       64 2023-04-07 03:15:36.000000 awscli_mate-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-04-07 03:48:53.928273 awscli_mate-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7837 2023-04-07 03:48:12.000000 awscli_mate-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-12 22:17:16.411817 awscli_mate-0.3.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-04-04 15:13:55.000000 awscli_mate-0.3.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1121 2023-04-04 15:13:55.000000 awscli_mate-0.3.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      319 2023-04-04 15:13:55.000000 awscli_mate-0.3.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5529 2023-04-12 22:17:16.411659 awscli_mate-0.3.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4429 2023-04-12 22:11:04.000000 awscli_mate-0.3.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-12 22:17:16.409698 awscli_mate-0.3.2/awscli_mate/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      653 2023-04-12 21:58:55.000000 awscli_mate-0.3.2/awscli_mate/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-04-12 22:09:19.000000 awscli_mate-0.3.2/awscli_mate/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      211 2023-04-12 21:58:40.000000 awscli_mate-0.3.2/awscli_mate/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8886 2023-04-12 21:58:32.000000 awscli_mate-0.3.2/awscli_mate/awscli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      707 2023-04-06 01:57:32.000000 awscli_mate-0.3.2/awscli_mate/cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      636 2023-04-04 17:52:15.000000 awscli_mate-0.3.2/awscli_mate/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-12 22:17:16.410509 awscli_mate-0.3.2/awscli_mate/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-04-04 15:13:55.000000 awscli_mate-0.3.2/awscli_mate/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      245 2023-04-07 02:32:41.000000 awscli_mate-0.3.2/awscli_mate/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      307 2023-04-04 18:03:25.000000 awscli_mate-0.3.2/awscli_mate/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-12 22:17:16.411251 awscli_mate-0.3.2/awscli_mate/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-04-04 15:56:46.000000 awscli_mate-0.3.2/awscli_mate/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-04-02 05:07:43.000000 awscli_mate-0.3.2/awscli_mate/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-04-02 05:07:43.000000 awscli_mate-0.3.2/awscli_mate/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-12 22:17:16.410401 awscli_mate-0.3.2/awscli_mate.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5529 2023-04-12 22:17:16.000000 awscli_mate-0.3.2/awscli_mate.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      655 2023-04-12 22:17:16.000000 awscli_mate-0.3.2/awscli_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-04-12 22:17:16.000000 awscli_mate-0.3.2/awscli_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-04-12 22:17:16.000000 awscli_mate-0.3.2/awscli_mate.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      248 2023-04-12 22:17:16.000000 awscli_mate-0.3.2/awscli_mate.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       12 2023-04-12 22:17:16.000000 awscli_mate-0.3.2/awscli_mate.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1612 2023-04-12 22:10:07.000000 awscli_mate-0.3.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-04-07 03:08:21.000000 awscli_mate-0.3.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-04-04 15:13:55.000000 awscli_mate-0.3.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      196 2023-04-07 03:08:26.000000 awscli_mate-0.3.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       64 2023-04-07 03:15:36.000000 awscli_mate-0.3.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-04-12 22:17:16.411877 awscli_mate-0.3.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7837 2023-04-07 03:48:12.000000 awscli_mate-0.3.2/setup.py
```

### Comparing `awscli_mate-0.3.1/LICENSE.txt` & `awscli_mate-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awscli_mate-0.3.1/PKG-INFO` & `awscli_mate-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: awscli_mate
-Version: 0.3.1
+Version: 0.3.2
 Summary: AWS CLI improvement.
 Home-page: https://github.com/MacHu-GWU/awscli_mate-project
-Download-URL: https://pypi.python.org/pypi/awscli_mate/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/awscli_mate/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -112,14 +112,19 @@
 .. code-block:: python
 
     awscli_mate mfa_auth --profile=your_profile --mfa_code=123456 --hours=12 --overwrite_default=True
 
 Note that this command also automatically set the MFA profile as default profile. If you don't want to set the ``your_profile_mfa`` as default profile automatically, you can just remove the ``--overwrite_default`` part.
 
 
+Use ``awscli_mate`` as a Python Library
+------------------------------------------------------------------------------
+See `example <./example.ipynb>`_.
+
+
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``awscli_mate`` is released on PyPI, so all you need is:
```

### Comparing `awscli_mate-0.3.1/README.rst` & `awscli_mate-0.3.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 .. code-block:: python
 
     awscli_mate mfa_auth --profile=your_profile --mfa_code=123456 --hours=12 --overwrite_default=True
 
 Note that this command also automatically set the MFA profile as default profile. If you don't want to set the ``your_profile_mfa`` as default profile automatically, you can just remove the ``--overwrite_default`` part.
 
 
+Use ``awscli_mate`` as a Python Library
+------------------------------------------------------------------------------
+See `example <./example.ipynb>`_.
+
+
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``awscli_mate`` is released on PyPI, so all you need is:
```

### Comparing `awscli_mate-0.3.1/awscli_mate/__init__.py` & `awscli_mate-0.3.2/awscli_mate/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 __license__ = "MIT"
 __author__ = "Sanhe Hu"
 __author_email__ = "husanhe@gmail.com"
 __github_username__ = "MacHu-GWU"
 
 try:
     from .api import (
+        strip_comment,
         AWSCliConfig,
         SectionTypeEnum,
         ConfigKeyEnum,
         CredentialKeyEnum,
     )
 except ImportError as e:  # pragma: no cover
     print(e)
```

### Comparing `awscli_mate-0.3.1/awscli_mate/awscli.py` & `awscli_mate-0.3.2/awscli_mate/awscli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 from atomicwrites import atomic_write
 from commentedconfigparser import CommentedConfigParser
 
 from .paths import path_config, path_credentials
 from . import exc
 
 
+def strip_comment(s: str) -> str:
+    return s.split("#")[0]
+
+
 @dataclasses.dataclass
 class AWSCliConfig:
     """
     Abstraction of the AWS CLI config files.
     """
 
     path_config: Path = dataclasses.field(default=path_config)
@@ -126,22 +130,26 @@
         if dict(config[from_section_name]) == dict(config[to_section_name]):
             return False
 
         self.clear_section_data(config, to_section_name)
         self.copy_section_data(config, from_section_name, to_section_name)
         return True
 
-    def set_profile_as_default(self, profile: str):
+    def set_profile_as_default(
+        self,
+        profile: str,
+    ) -> T.Tuple[T.Optional[CommentedConfigParser], T.Optional[CommentedConfigParser]]:
         """
         Set the given profile as the default profile by replacing the section data.
         """
         if profile == "default":
-            return
+            return None, None
 
         config, credentials = self.read_config()
+
         self.ensure_profile_exists("default", config, credentials)
         self.ensure_profile_exists(profile, config, credentials)
 
         flag_is_config_changed = self.replace_section_data(
             config,
             from_section_name=f"profile {profile}",
             to_section_name="default",
@@ -156,21 +164,23 @@
             with self.path_config.open("w") as f:
                 config.write(f)
 
         if flag_is_credentials_changed:
             with self.path_credentials.open("w") as f:
                 credentials.write(f)
 
+        return config, credentials
+
     def mfa_auth(
         self,
         profile: str,
         mfa_code: str,
         hours: int = 12,
         overwrite_default: bool = False,
-    ):  # pragma: no cover
+    ) -> T.Tuple[CommentedConfigParser, CommentedConfigParser]:  # pragma: no cover
         """
         Given a base ``${profile}``, do MFA authentication with ``mfa_code``,
         create / update the new aws profile ``${profile}_mfa`` using the returned
         temp token. This function will update the ``~/.aws/credential`` and
         ``~/.aws/config`` file inplace.
 
         :param aws_profile: The source AWS profile which has MFA enabled
@@ -246,7 +256,9 @@
         # update ~/.aws/config and ~/.aws/credentials file
         if flag_is_config_changed:
             with atomic_write(f"{self.path_config}", overwrite=True) as f:
                 config.write(f)
 
         with atomic_write(f"{self.path_credentials}", overwrite=True) as f:
             credentials.write(f)
+
+        return config, credentials
```

### Comparing `awscli_mate-0.3.1/awscli_mate/cli.py` & `awscli_mate-0.3.2/awscli_mate/cli.py`

 * *Files identical despite different names*

### Comparing `awscli_mate-0.3.1/awscli_mate/constants.py` & `awscli_mate-0.3.2/awscli_mate/constants.py`

 * *Files identical despite different names*

### Comparing `awscli_mate-0.3.1/awscli_mate/tests/helper.py` & `awscli_mate-0.3.2/awscli_mate/tests/helper.py`

 * *Files identical despite different names*

### Comparing `awscli_mate-0.3.1/awscli_mate.egg-info/PKG-INFO` & `awscli_mate-0.3.2/awscli_mate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: awscli-mate
-Version: 0.3.1
+Version: 0.3.2
 Summary: AWS CLI improvement.
 Home-page: https://github.com/MacHu-GWU/awscli_mate-project
-Download-URL: https://pypi.python.org/pypi/awscli_mate/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/awscli_mate/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -112,14 +112,19 @@
 .. code-block:: python
 
     awscli_mate mfa_auth --profile=your_profile --mfa_code=123456 --hours=12 --overwrite_default=True
 
 Note that this command also automatically set the MFA profile as default profile. If you don't want to set the ``your_profile_mfa`` as default profile automatically, you can just remove the ``--overwrite_default`` part.
 
 
+Use ``awscli_mate`` as a Python Library
+------------------------------------------------------------------------------
+See `example <./example.ipynb>`_.
+
+
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``awscli_mate`` is released on PyPI, so all you need is:
```

### Comparing `awscli_mate-0.3.1/awscli_mate.egg-info/SOURCES.txt` & `awscli_mate-0.3.2/awscli_mate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awscli_mate-0.3.1/release-history.rst` & `awscli_mate-0.3.2/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.2 (2023-04-12)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- add return value to :meth:`awscli_mate.awscli.AWSCliConfig.set_profile_as_default`.
+- add return value to :meth:`awscli_mate.awscli.AWSCliConfig.mfa_auth`.
+
+**Miscellaneous**
+
+- add an example jupyter notebook
+
+
 0.3.1 (2023-04-06)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``SectionTypeEnum``, ``ConfigKeyEnum``, ``CredentialKeyEnum`` to public API.
 
 **Minor Improvements**
```

### Comparing `awscli_mate-0.3.1/requirements-doc.txt` & `awscli_mate-0.3.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `awscli_mate-0.3.1/setup.py` & `awscli_mate-0.3.2/setup.py`

 * *Files identical despite different names*

