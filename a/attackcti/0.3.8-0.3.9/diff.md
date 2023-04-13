# Comparing `tmp/attackcti-0.3.8.tar.gz` & `tmp/attackcti-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attackcti-0.3.8.tar", last modified: Sat Nov 19 05:20:17 2022, max compression
+gzip compressed data, was "attackcti-0.3.9.tar", last modified: Thu Apr 13 01:25:20 2023, max compression
```

## Comparing `attackcti-0.3.8.tar` & `attackcti-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-11-19 05:20:16.989775 attackcti-0.3.8/
--rw-rw-rw-   0        0        0     1546 2021-05-14 02:44:16.000000 attackcti-0.3.8/LICENSE
--rw-rw-rw-   0        0        0     5265 2022-11-19 05:20:16.989775 attackcti-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3522 2022-01-19 04:33:51.000000 attackcti-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-19 05:20:16.900859 attackcti-0.3.8/attackcti/
--rw-rw-rw-   0        0        0       62 2021-05-14 02:44:16.000000 attackcti-0.3.8/attackcti/__init__.py
--rw-rw-rw-   0        0        0    90958 2022-11-19 05:06:44.000000 attackcti-0.3.8/attackcti/attack_api.py
-drwxrwxrwx   0        0        0        0 2022-11-19 05:20:16.981778 attackcti-0.3.8/attackcti.egg-info/
--rw-rw-rw-   0        0        0     5265 2022-11-19 05:20:16.000000 attackcti-0.3.8/attackcti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2022-11-19 05:20:16.000000 attackcti-0.3.8/attackcti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-19 05:20:16.000000 attackcti-0.3.8/attackcti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-11-19 05:20:16.000000 attackcti-0.3.8/attackcti.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-19 05:20:16.000000 attackcti-0.3.8/attackcti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-11-19 05:20:16.989775 attackcti-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1677 2022-11-19 05:16:48.000000 attackcti-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:25:20.887669 attackcti-0.3.9/
+-rw-rw-rw-   0        0        0     1546 2021-05-14 02:44:16.000000 attackcti-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0     5265 2023-04-13 01:25:20.887669 attackcti-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3522 2022-01-19 04:33:51.000000 attackcti-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 01:25:20.858364 attackcti-0.3.9/attackcti/
+-rw-rw-rw-   0        0        0       62 2021-05-14 02:44:16.000000 attackcti-0.3.9/attackcti/__init__.py
+-rw-rw-rw-   0        0        0    92732 2023-04-13 01:23:17.000000 attackcti-0.3.9/attackcti/attack_api.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:25:20.886669 attackcti-0.3.9/attackcti.egg-info/
+-rw-rw-rw-   0        0        0     5265 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-13 01:25:20.889672 attackcti-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-04-13 01:24:52.000000 attackcti-0.3.9/setup.py
```

### Comparing `attackcti-0.3.8/LICENSE` & `attackcti-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `attackcti-0.3.8/PKG-INFO` & `attackcti-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.3.8
+Version: 0.3.9
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
```

### Comparing `attackcti-0.3.8/README.md` & `attackcti-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `attackcti-0.3.8/attackcti/attack_api.py` & `attackcti-0.3.9/attackcti/attack_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
             "tools": self.get_enterprise_tools,
             "data-source": self.get_enterprise_data_sources,
             "relationships": self.get_enterprise_relationships,
             "tactics": self.get_enterprise_tactics,
             "matrix": Filter("type", "=", "x-mitre-matrix"),
             "identity": Filter("type", "=", "identity"),
             "marking-definition": Filter("type", "=", "marking-definition"),
-            "campaign": self.get_enterprise_campaigns
+            "campaigns": self.get_enterprise_campaigns
         }
         enterprise_stix_objects = dict()
         for key in enterprise_filter_objects:
             enterprise_stix_objects[key] = self.TC_ENTERPRISE_SOURCE.query(enterprise_filter_objects[key]) if isinstance(enterprise_filter_objects[key], Filter) else enterprise_filter_objects[key]()
             if not stix_format:
                 enterprise_stix_objects[key] = self.translate_stix_objects(enterprise_stix_objects[key])
         return enterprise_stix_objects
@@ -684,15 +684,15 @@
         for key in mobile_filter_objects:
             mobile_stix_objects[key] = self.TC_MOBILE_SOURCE.query(mobile_filter_objects[key]) if isinstance(mobile_filter_objects[key], Filter) else mobile_filter_objects[key]()
             if not stix_format:
                 mobile_stix_objects[key] = self.translate_stix_objects(mobile_stix_objects[key])           
         return mobile_stix_objects
 
     def get_mobile_campaigns(self, skip_revoked_deprecated=True, stix_format=True):
-        """  Extracts all the available techniques STIX objects in the Mobile ATT&CK matrix
+        """  Extracts all the available campaign STIX objects in the Mobile ATT&CK matrix
 
         Args:
             skip_revoked_deprecated (bool): default True. Skip revoked and deprecated STIX objects. 
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
         
         Returns:
             List of STIX objects
@@ -838,28 +838,54 @@
         
         Returns:
             List of STIX objects
         
         """
         ics_filter_objects = {
             "techniques": self.get_ics_techniques,
+            "data-component": self.get_ics_data_components,
             "mitigations": self.get_ics_mitigations,
             "groups": self.get_ics_groups,
             "malware": self.get_ics_malware,
+            "tools": self.get_ics_tools,
+            "data-source": self.get_ics_data_sources,
             "relationships": self.get_ics_relationships,
             "tactics": self.get_ics_tactics,
-            "matrix": Filter("type", "=", "x-mitre-matrix")
+            "matrix": Filter("type", "=", "x-mitre-matrix"),
+            "identity": Filter("type", "=", "identity"),
+            "marking-definition": Filter("type", "=", "marking-definition"),
+            "campaigns": self.get_ics_campaigns
         }
         ics_stix_objects = {}
         for key in ics_filter_objects:
             ics_stix_objects[key] = self.TC_ICS_SOURCE.query(ics_filter_objects[key]) if isinstance(ics_filter_objects[key], Filter) else ics_filter_objects[key]()
             if not stix_format:
                 ics_stix_objects[key] = self.translate_stix_objects(ics_stix_objects[key])           
         return ics_stix_objects
 
+    def get_ics_campaigns(self, skip_revoked_deprecated=True, stix_format=True):
+        """  Extracts all the available techniques STIX objects in the ICS ATT&CK matrix
+
+        Args:
+            skip_revoked_deprecated (bool): default True. Skip revoked and deprecated STIX objects.
+            stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
+
+        Returns:
+            List of STIX objects
+        """
+
+        ics_campaigns = self.TC_ICS_SOURCE.query(Filter("type", "=", "campaign"))
+
+        if skip_revoked_deprecated:
+            ics_campaigns = self.remove_revoked_deprecated(ics_campaigns)
+
+        if not stix_format:
+            ics_campaigns = self.translate_stix_objects(ics_campaigns)
+        return ics_campaigns
+
     def get_ics_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, stix_format=True):
         """ Extracts all the available techniques STIX objects in the ICS ATT&CK matrix
 
         Args:
             skip_revoked_deprecated (bool): default True. Skip revoked and deprecated STIX objects. 
             include_subtechniques (bool): default True. Include techniques and sub-techniques STIX objects.
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
@@ -944,14 +970,29 @@
         
         """
         ics_malware = self.TC_ICS_SOURCE.query(Filter("type", "=", "malware"))
         if not stix_format:
             ics_malware = self.translate_stix_objects(ics_malware)
         return ics_malware
 
+    def get_ics_tools(self, stix_format=True):
+        """Extracts all the available tools STIX objects in the ICS ATT&CK matrix
+
+        Args:
+            stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
+
+        Returns:
+            List of STIX objects
+
+        """
+        ics_tools = self.TC_ICS_SOURCE.query(Filter("type", "=", "tool"))
+        if not stix_format:
+            ics_tools = self.translate_stix_objects(ics_tools)
+        return ics_tools
+
     def get_ics_relationships(self, stix_format=True):
         """ Extracts all the available relationships STIX objects in the ICS ATT&CK matrix
 
         Args:
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
         
         Returns:
@@ -1017,17 +1058,18 @@
         
         Returns:
             List of STIX objects
         """
         
         enterprise_campaigns = self.get_enterprise_campaigns()
         mobile_campaigns = self.get_mobile_campaigns()
-        for mc in mobile_campaigns:
-            if mc not in enterprise_campaigns:
-                enterprise_campaigns.append(mc)
+        ics_campaigns = self.get_ics_campaigns()
+        for c in mobile_campaigns + ics_campaigns:
+            if c not in enterprise_campaigns:
+                enterprise_campaigns.append(c)
 
         if skip_revoked_deprecated:
             enterprise_campaigns = self.remove_revoked_deprecated(enterprise_campaigns)
 
         if not stix_format:
             enterprise_campaigns = self.translate_stix_objects(enterprise_campaigns)
```

### Comparing `attackcti-0.3.8/attackcti.egg-info/PKG-INFO` & `attackcti-0.3.9/attackcti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.3.8
+Version: 0.3.9
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
```

### Comparing `attackcti-0.3.8/setup.py` & `attackcti-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md')as f:
     long_description = f.read()
 
 setup(
     name="attackcti",
-    version="0.3.8",
+    version="0.3.9",
     author="Roberto Rodriguez",
     description="MITRE ATTACK CTI Python Libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OTRF/ATTACK-Python-Client",
     project_urls={
         "Documentation": "https://attackcti.com",
```

