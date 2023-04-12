# Comparing `tmp/mypy-boto3-managedblockchain-1.26.81.tar.gz` & `tmp/mypy-boto3-managedblockchain-1.26.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-1.26.81.tar", last modified: Tue Feb 28 20:28:07 2023, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-1.26.9.tar", last modified: Mon Nov 14 20:49:29 2022, max compression
```

## Comparing `mypy-boto3-managedblockchain-1.26.81.tar` & `mypy-boto3-managedblockchain-1.26.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.518319 mypy-boto3-managedblockchain-1.26.81/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16168 2023-02-28 20:28:07.518319 mypy-boto3-managedblockchain-1.26.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.506319 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-02-28 20:27:54.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26424 2023-02-28 20:27:54.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-02-28 20:27:54.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 20:27:53.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.518319 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16168 2023-02-28 20:28:07.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-28 20:28:07.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 20:28:07.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-28 20:28:07.000000 mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 20:28:07.518319 mypy-boto3-managedblockchain-1.26.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-28 20:27:52.000000 mypy-boto3-managedblockchain-1.26.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.644561 mypy-boto3-managedblockchain-1.26.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    16116 2022-11-14 20:49:29.640561 mypy-boto3-managedblockchain-1.26.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14641 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.636561 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20302 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20267 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-11-14 20:48:57.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8517 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1928 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    26054 2022-11-14 20:48:57.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26027 2022-11-14 20:48:57.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.640561 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    16116 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 20:49:29.644561 mypy-boto3-managedblockchain-1.26.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/setup.py
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/LICENSE` & `mypy-boto3-managedblockchain-1.26.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.81/PKG-INFO` & `mypy-boto3-managedblockchain-1.26.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.26.81
-Summary: Type annotations for boto3.ManagedBlockchain 1.26.81 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.9
+Summary: Type annotations for boto3.ManagedBlockchain 1.26.9 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/README.md` & `mypy-boto3-managedblockchain-1.26.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/__init__.py` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/__init__.pyi` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/__main__.py` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchain 1.26.81\nVersion:         1.26.81\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchain 1.26.9\nVersion:         1.26.9\nBuilder"
+        " version: 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.81")
+    print("1.26.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/client.py` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,22 +115,18 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#close)
         """
 
     def create_accessor(
-        self,
-        *,
-        ClientRequestToken: str,
-        AccessorType: Literal["BILLING_TOKEN"],
-        Tags: Mapping[str, str] = ...
+        self, *, ClientRequestToken: str, AccessorType: Literal["BILLING_TOKEN"]
     ) -> CreateAccessorOutputTypeDef:
         """
-        Creates a new accessor for use with Managed Blockchain Ethereum nodes.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_accessor)
         """
 
     def create_member(
         self,
@@ -199,15 +195,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_proposal)
         """
 
     def delete_accessor(self, *, AccessorId: str) -> Dict[str, Any]:
         """
-        Deletes an accessor that your Amazon Web Services account owns.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_accessor)
         """
 
     def delete_member(self, *, NetworkId: str, MemberId: str) -> Dict[str, Any]:
         """
@@ -237,15 +233,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#generate_presigned_url)
         """
 
     def get_accessor(self, *, AccessorId: str) -> GetAccessorOutputTypeDef:
         """
-        Returns detailed information about an accessor.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_accessor)
         """
 
     def get_member(self, *, NetworkId: str, MemberId: str) -> GetMemberOutputTypeDef:
         """
@@ -279,15 +275,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_proposal)
         """
 
     def list_accessors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAccessorsOutputTypeDef:
         """
-        Returns a list of the accessors and their properties.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_accessors)
         """
 
     def list_invitations(
         self, *, MaxResults: int = ..., NextToken: str = ...
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/client.pyi` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -108,22 +108,18 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#close)
         """
     def create_accessor(
-        self,
-        *,
-        ClientRequestToken: str,
-        AccessorType: Literal["BILLING_TOKEN"],
-        Tags: Mapping[str, str] = ...
+        self, *, ClientRequestToken: str, AccessorType: Literal["BILLING_TOKEN"]
     ) -> CreateAccessorOutputTypeDef:
         """
-        Creates a new accessor for use with Managed Blockchain Ethereum nodes.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_accessor)
         """
     def create_member(
         self,
         *,
@@ -187,15 +183,15 @@
         can vote on, for example, a proposal to add a new member to the network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_proposal)
         """
     def delete_accessor(self, *, AccessorId: str) -> Dict[str, Any]:
         """
-        Deletes an accessor that your Amazon Web Services account owns.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_accessor)
         """
     def delete_member(self, *, NetworkId: str, MemberId: str) -> Dict[str, Any]:
         """
         Deletes a member.
@@ -221,15 +217,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#generate_presigned_url)
         """
     def get_accessor(self, *, AccessorId: str) -> GetAccessorOutputTypeDef:
         """
-        Returns detailed information about an accessor.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_accessor)
         """
     def get_member(self, *, NetworkId: str, MemberId: str) -> GetMemberOutputTypeDef:
         """
         Returns detailed information about a member.
@@ -258,15 +254,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_proposal)
         """
     def list_accessors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAccessorsOutputTypeDef:
         """
-        Returns a list of the accessors and their properties.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_accessors)
         """
     def list_invitations(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInvitationsOutputTypeDef:
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/literals.py` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -111,31 +110,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -164,15 +159,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -217,19 +211,17 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -240,33 +232,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -298,32 +287,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -351,58 +336,52 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/literals.pyi` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -109,31 +108,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -162,15 +157,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -215,19 +209,17 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -238,33 +230,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -296,32 +285,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -349,58 +334,52 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/paginator.py` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/paginator.pyi` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/type_defs.py` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,50 +144,35 @@
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
         "BillingToken": str,
         "Status": AccessorStatusType,
         "CreationDate": datetime,
         "Arn": str,
-        "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
     total=False,
 )
 
-_RequiredCreateAccessorInputRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessorInputRequestTypeDef",
+CreateAccessorInputRequestTypeDef = TypedDict(
+    "CreateAccessorInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "AccessorType": Literal["BILLING_TOKEN"],
     },
 )
-_OptionalCreateAccessorInputRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessorInputRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateAccessorInputRequestTypeDef(
-    _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
-):
-    pass
-
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain/type_defs.pyi` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,48 +143,35 @@
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
         "BillingToken": str,
         "Status": AccessorStatusType,
         "CreationDate": datetime,
         "Arn": str,
-        "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
     total=False,
 )
 
-_RequiredCreateAccessorInputRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessorInputRequestTypeDef",
+CreateAccessorInputRequestTypeDef = TypedDict(
+    "CreateAccessorInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "AccessorType": Literal["BILLING_TOKEN"],
     },
 )
-_OptionalCreateAccessorInputRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessorInputRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateAccessorInputRequestTypeDef(
-    _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
-):
-    pass
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.26.81
-Summary: Type annotations for boto3.ManagedBlockchain 1.26.81 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.9
+Summary: Type annotations for boto3.ManagedBlockchain 1.26.9 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-managedblockchain-1.26.81/mypy_boto3_managedblockchain.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.81/setup.py` & `mypy-boto3-managedblockchain-1.26.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-managedblockchain",
-    version="1.26.81",
+    version="1.26.9",
     packages=["mypy_boto3_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchain 1.26.81 service generated with"
-        " mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.ManagedBlockchain 1.26.9 service generated with"
+        " mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_managedblockchain": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_managedblockchain": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

