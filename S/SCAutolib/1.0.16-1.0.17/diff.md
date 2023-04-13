# Comparing `tmp/SCAutolib-1.0.16.tar.gz` & `tmp/SCAutolib-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SCAutolib-1.0.16.tar", last modified: Wed Nov 30 13:27:24 2022, max compression
+gzip compressed data, was "SCAutolib-1.0.17.tar", last modified: Thu Apr 13 08:04:40 2023, max compression
```

## Comparing `SCAutolib-1.0.16.tar` & `SCAutolib-1.0.17.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:27:24.764065 SCAutolib-1.0.16/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2022-11-30 13:27:24.764065 SCAutolib-1.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:27:24.756065 SCAutolib-1.0.16/SCAutolib/
--rw-r--r--   0 runner    (1001) docker     (122)     5036 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5363 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    17793 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/controller.py
--rw-r--r--   0 runner    (1001) docker     (122)      857 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:27:24.760065 SCAutolib-1.0.16/SCAutolib/models/
--rw-r--r--   0 runner    (1001) docker     (122)    25480 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/models/CA.py
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3443 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/models/authselect.py
--rw-r--r--   0 runner    (1001) docker     (122)     9885 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/models/card.py
--rw-r--r--   0 runner    (1001) docker     (122)    20818 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (122)    12112 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:27:24.760065 SCAutolib-1.0.16/SCAutolib/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/templates/ca.cnf
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/templates/softhsm2.conf
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/templates/sssd.conf
--rw-r--r--   0 runner    (1001) docker     (122)      454 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/templates/user.cnf
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/templates/virt_cacard.service
--rw-r--r--   0 runner    (1001) docker     (122)      167 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/templates/virtcacard.cil
--rw-r--r--   0 runner    (1001) docker     (122)     6738 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/SCAutolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:27:24.760065 SCAutolib-1.0.16/SCAutolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2022-11-30 13:27:24.000000 SCAutolib-1.0.16/SCAutolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      910 2022-11-30 13:27:24.000000 SCAutolib-1.0.16/SCAutolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 13:27:24.000000 SCAutolib-1.0.16/SCAutolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2022-11-30 13:27:24.000000 SCAutolib-1.0.16/SCAutolib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-30 13:27:24.000000 SCAutolib-1.0.16/SCAutolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-30 13:27:24.000000 SCAutolib-1.0.16/SCAutolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 13:27:24.764065 SCAutolib-1.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:27:24.764065 SCAutolib-1.0.16/test/
--rw-r--r--   0 runner    (1001) docker     (122)     6859 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (122)     3549 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_card.py
--rw-r--r--   0 runner    (1001) docker     (122)     2523 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2708 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      523 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_openssl_conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_sssd_conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (122)      355 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      966 2022-11-30 13:27:12.000000 SCAutolib-1.0.16/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.852830 SCAutolib-1.0.17/SCAutolib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/SCAutolib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/authselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/SCAutolib/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/ca.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/softhsm2.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/sssd.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/user.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/virt_cacard.service
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/virtcacard.cil
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/SCAutolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_openssl_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_sssd_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/tox.ini
```

### Comparing `SCAutolib-1.0.16/LICENSE` & `SCAutolib-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/PKG-INFO` & `SCAutolib-1.0.17/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SCAutolib
-Version: 1.0.16
+Version: 1.0.17
 Summary: Python library for automation tests of smart cards using virtualization.
-Home-page: https://github.com/x00Pavel/SCAutolib
+Home-page: https://github.com/redhat-qe-security/SCAutolib
 Author: Pavel Yadlouski
 Author-email: pyadlous@redhat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
```

### Comparing `SCAutolib-1.0.16/README.md` & `SCAutolib-1.0.17/README.md`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/__init__.py` & `SCAutolib-1.0.17/SCAutolib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 LIB_DUMP_CARDS = LIB_DUMP.joinpath("cards")
 
 
 schema_cas = Schema(And(
     Use(dict),
     # Check that CA section contains at least one and maximum
     # two entries
-    lambda l: 1 <= len(l.keys()) <= 2,
+    lambda l: 1 <= len(l.keys()) <= 2,  # noqa: E741
     {Optional("local_ca"): {
         Optional("dir", default=Path("/etc/SCAutolib/ca")): Use(Path)},
         Optional("ipa"): {
             'admin_passwd': Use(str),
             'root_passwd': Use(str),
             Optional('ip_addr', default=None): Use(str),
             'server_hostname': Use(str),
```

### Comparing `SCAutolib-1.0.16/SCAutolib/cli_commands.py` & `SCAutolib-1.0.17/SCAutolib/cli_commands.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/controller.py` & `SCAutolib-1.0.17/SCAutolib/controller.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/exceptions.py` & `SCAutolib-1.0.17/SCAutolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/models/CA.py` & `SCAutolib-1.0.17/SCAutolib/models/CA.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 """
 import shutil
 
 import re
 
 import json
 import os
-import paramiko
 import python_freeipa
 from cryptography import x509
-from fabric.connection import Connection
 from hashlib import md5
-from invoke import Responder
 from pathlib import Path, PosixPath
 from python_freeipa import exceptions
 from python_freeipa.client_meta import ClientMeta
-from shutil import rmtree
+from shutil import rmtree, copy2
 from socket import gethostname
 
 from SCAutolib import TEMPLATES_DIR, logger, run, LIB_DIR, LIB_DUMP_CAS
 from SCAutolib.exceptions import SCAutolibException
 from SCAutolib.models.file import OpensslCnf
 
 
@@ -312,14 +309,15 @@
     _ipa_server_ip: str = None
     _ipa_server_hostname: str = None
     _ipa_server_domain: str = None
     _ipa_server_admin_passwd: str = None
     _ipa_server_realm: str = None
     _ipa_client_hostname: str = None
     _ipa_server_root_passwd: str = None
+    _ipa_client_script = Path(LIB_DIR, "ipa-client-sc.sh")
     meta_client: ClientMeta = None
     dump_file = LIB_DUMP_CAS.joinpath("ipa-server.json")
 
     def __init__(self, ip_addr: str, server_hostname: str, domain: str,
                  admin_passwd: str, root_passwd: str, client_hostname: str,
                  realm: str = None):
         """
@@ -412,17 +410,26 @@
         except:
             logger.critical("Installation of IPA client is failed")
             rmtree("/etc/ipa/*")
             logger.debug("Directory /etc/ipa is removed")
             raise
         logger.debug("IPA client is installed")
 
-        ipa_client_script = self._get_sc_setup_script()
+        try:
+            copy2("/tmp/cont-data/config-client-for-smart-card-auth.sh",
+                  self._ipa_client_script)
+            logger.info("Script for setting up IPA client for smart cards was "
+                        f"found and copied to {self._ipa_client_script}")
+        except FileNotFoundError:
+            logger.info("Script for setting up IPA client for smart cards was "
+                        "not found. It will be generated on IPA server and "
+                        "fetched")
+            self._get_sc_setup_script()
         run("kinit admin", input=self._ipa_server_admin_passwd)
-        run(f'bash {ipa_client_script} /etc/ipa/ca.crt', check=True)
+        run(f'bash {self._ipa_client_script} /etc/ipa/ca.crt', check=True)
         logger.debug("Setup of IPA client for smart card is finished")
 
         self._meta_client_login()
 
         policy = self.meta_client.pwpolicy_show(a_cn="global_policy")["result"]
         if ["0"] != policy["krbminpwdlife"]:
             self.meta_client.pwpolicy_mod(a_cn="global_policy",
@@ -490,23 +497,36 @@
             if entry not in cnt:
                 f.write(f"\n{entry}\n")
                 logger.warning(
                     f"New entry {entry} for IPA server is added to /etc/hosts")
             logger.info(
                 f"Entry for IPA server {entry} presents in the /etc/hosts")
 
-    def _get_sc_setup_script(self) -> Path:
+    def _get_sc_setup_script(self):
         """
-        Fetch script for smart card setup of IPA client. Script is generated
-        only on IPA server. Fetching is made by connecting to the host via SSH.
+        Fetch script for smart card setup of IPA client and place it to
+        predefined location. Script is generated only on IPA server.
+        Fetching is done by connecting to the host via SSH.
+        """
+        import paramiko
+        from invoke import Responder
+        from fabric.connection import Connection
+
+        class __PKeyChild(paramiko.PKey):
+            """This child class is need to fix SSH connection with MD5 algorithm
+            in FIPS mode
+
+            This is just workaround until PR in paramiko would be accepted
+            https://github.com/paramiko/paramiko/issues/396. After this PR is
+            merged, delete this class
+            """
+
+            def get_fingerprint_improved(self):
+                return md5(self.asbytes(), usedforsecurity=False).digest()
 
-        :return: Path to script
-        :rtype: patlib.Path
-        """
-        ipa_client_script = Path(LIB_DIR, "ipa-client-sc.sh")
         kinitpass = Responder(
             pattern=f"Password for admin@{self._ipa_server_realm}: ",
             response=f"{self._ipa_server_admin_passwd}\n")
         logger.debug("Start receiving client script for setting up smart card "
                      "on IPA client")
         with Connection(self._ipa_server_ip, user="root",
                         connect_kwargs={
@@ -523,25 +543,26 @@
             # in_stream = False is required because while testing with pytest
             # it collision appears with capturing of the output.
             logger.debug("Running kinit on the IPA server")
             c.run("kinit admin", pty=True, watchers=[kinitpass], in_stream=False)
             result = c.run("ipa-advise config-client-for-smart-card-auth",
                            hide=True, in_stream=False)
             logger.debug("Script is generated on server side")
-            with open(ipa_client_script, "w") as f:
+            with open(self._ipa_client_script, "w") as f:
                 f.write(result.stdout)
-        if os.stat(ipa_client_script).st_size == 0:
+
+        if os.stat(self._ipa_client_script).st_size == 0:
             msg = "Script for IPA client smart card setup is not correctly " \
                   "copied to the host"
             logger.error(result.stdout)
             logger.error(result.stderr)
             raise SCAutolibException(msg)
+
         logger.debug("File for setting up IPA client for smart cards is "
-                     f"copied to {ipa_client_script}")
-        return ipa_client_script
+                     f"copied to {self._ipa_client_script}")
 
     def request_cert(self, csr: Path, username: str, cert_out: Path):
         """
         Request certificate using CSR from IPA CA for given username. It is
         a wrapper around the python_freeipa.client_meta.ClientMeta.cert_request
         method. It works with a file, extracts CSR data from it and then
         stores in PEM format adding required prefix and suffix as in normal
@@ -639,22 +660,10 @@
         except exceptions.NotFound:
             logger.error(f"Current hostname ({gethostname()}) is not found "
                          f"on the IPA server")
         # Return code 2 means that the IPA client is not configured
         run(["ipa-client-install", "--uninstall", "-U"], return_code=[0, 2])
         logger.info("IPA client is removed.")
 
-    class __PKeyChild(paramiko.PKey):
-        """This child class is need to fix SSH connection with MD5 algorithm
-        in FIPS mode
-
-        This is just workaround until PR in paramiko would be accepted
-        https://github.com/paramiko/paramiko/issues/396. After this PR is merged,
-        delete this class
-        """
-
-        def get_fingerprint_improved(self):
-            return md5(self.asbytes(), usedforsecurity=False).digest()
-
     @property
     def ipa_server_hostname(self):
         return self._ipa_server_hostname
```

### Comparing `SCAutolib-1.0.16/SCAutolib/models/authselect.py` & `SCAutolib-1.0.17/SCAutolib/models/authselect.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/models/card.py` & `SCAutolib-1.0.17/SCAutolib/models/card.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/models/file.py` & `SCAutolib-1.0.17/SCAutolib/models/file.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/models/user.py` & `SCAutolib-1.0.17/SCAutolib/models/user.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/templates/ca.cnf` & `SCAutolib-1.0.17/SCAutolib/templates/ca.cnf`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib/utils.py` & `SCAutolib-1.0.17/SCAutolib/utils.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/SCAutolib.egg-info/PKG-INFO` & `SCAutolib-1.0.17/SCAutolib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SCAutolib
-Version: 1.0.16
+Version: 1.0.17
 Summary: Python library for automation tests of smart cards using virtualization.
-Home-page: https://github.com/x00Pavel/SCAutolib
+Home-page: https://github.com/redhat-qe-security/SCAutolib
 Author: Pavel Yadlouski
 Author-email: pyadlous@redhat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
```

### Comparing `SCAutolib-1.0.16/SCAutolib.egg-info/SOURCES.txt` & `SCAutolib-1.0.17/SCAutolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/setup.py` & `SCAutolib-1.0.17/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     reqs = f.readlines()
 
 with readme.open() as f:
     long_description = f.read()
 
 setup(
     name="SCAutolib",
-    version="1.0.16",
+    version="1.0.17",
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/x00Pavel/SCAutolib",
+    url="https://github.com/redhat-qe-security/SCAutolib",
     author="Pavel Yadlouski",
     author_email="pyadlous@redhat.com",
     classifiers=[
         'Programming Language :: Python :: 3',
         'Environment :: Console',
         'Framework :: Pytest',
         'Framework :: tox',
```

### Comparing `SCAutolib-1.0.16/test/test_ca.py` & `SCAutolib-1.0.17/test/test_ca.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_card.py` & `SCAutolib-1.0.17/test/test_card.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_cli.py` & `SCAutolib-1.0.17/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_controller.py` & `SCAutolib-1.0.17/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_file.py` & `SCAutolib-1.0.17/test/test_file.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_openssl_conf.py` & `SCAutolib-1.0.17/test/test_openssl_conf.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_sssd_conf.py` & `SCAutolib-1.0.17/test/test_sssd_conf.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/test/test_user.py` & `SCAutolib-1.0.17/test/test_user.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.16/tox.ini` & `SCAutolib-1.0.17/tox.ini`

 * *Files identical despite different names*

