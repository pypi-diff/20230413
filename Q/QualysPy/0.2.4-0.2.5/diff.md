# Comparing `tmp/qualyspy-0.2.4.tar.gz` & `tmp/qualyspy-0.2.5.tar.gz`

## Comparing `qualyspy-0.2.4.tar` & `qualyspy-0.2.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/remove_cookies.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/__init__.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/qutils.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/urls.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15254 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/certview/sql/certview_init.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.4/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.4/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.4/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.4/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/remove_cookies.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/__init__.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/urls.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/certview/sql/certview_init.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.5/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.5/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.5/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.5/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.5/PKG-INFO
```

### Comparing `qualyspy-0.2.4/.vscode/launch.json` & `qualyspy-0.2.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/debug/dtd.txt` & `qualyspy-0.2.5/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/debug/output.txt` & `qualyspy-0.2.5/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/debug/parse_dtd.py` & `qualyspy-0.2.5/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/debug/quickscan.py` & `qualyspy-0.2.5/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/debug/remove_cookies.py` & `qualyspy-0.2.5/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/docs/Makefile` & `qualyspy-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/docs/make.bat` & `qualyspy-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/docs/source/conf.py` & `qualyspy-0.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/qualysapi.py` & `qualyspy-0.2.5/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/qutils.py` & `qualyspy-0.2.5/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/urls.json` & `qualyspy-0.2.5/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/tags.py` & `qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/tags.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/assets/host_list.py` & `qualyspy-0.2.5/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/assets/host_list_detection.py` & `qualyspy-0.2.5/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/certview/certificate.py` & `qualyspy-0.2.5/qualyspy/certview/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,33 +37,34 @@
 
 ####################################################################################################
 # Subject_Alternative_Name
 
 
 class Subject_Alternative_Names(pd.BaseModel):
     dns_names = list[str]
-    ip_address = list[str]
+    ip_address = list[ipaddress.IPv4Address | ipaddress.IPv6Address]
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
 class Subject_Alternative_Names_ORM(Base):
     __tablename__ = "subject_alternative_name"
     pd_class = Subject_Alternative_Names
 
-    id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
     dns_names: orm.Mapped[list[str] | None] = orm.mapped_column(sa.ARRAY(sa.String))
     ips: orm.Mapped[
         list[ipaddress.IPv4Address | ipaddress.IPv6Address] | None
     ] = orm.mapped_column(sa.ARRAY(sa_pg.INET))
 
-    certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
+    certificate_id: orm.Mapped[int] = orm.mapped_column(
+        sa.ForeignKey("certificate.id"), primary_key=True
+    )
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="subject_alternative_names", uselist=False
     )
 
 
 ####################################################################################################
 
@@ -479,16 +480,18 @@
     def query(self, stmt: Any, *, echo: bool = False) -> list[_C]:
         engine = sa.create_engine(qutils.E_URL, echo=echo)
 
         output: list[_C] = []
         with orm.Session(engine) as session:
             results = session.execute(stmt)
             for result in results.all():
-                if issubclass(type(result), Base):
-                    i = type(result).pd_class.from_orm(result.scalars())  # type: ignore
+                r = result.tuple()[0]
+                r_type = type(r)
+                if issubclass(r_type, Base):
+                    i = r_type.pd_class.from_orm(r)  # type: ignore
                 else:
                     i = result
                 output.append(i)
 
         return output
 
     def reset(self, *, echo: bool = False) -> None:
```

### Comparing `qualyspy-0.2.4/qualyspy/certview/sql/certview_init.sql` & `qualyspy-0.2.5/qualyspy/certview/sql/certview_init.sql`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.2.5/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/.gitignore` & `qualyspy-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/LICENSE` & `qualyspy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.4/pyproject.toml` & `qualyspy-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.2.4/PKG-INFO` & `qualyspy-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

