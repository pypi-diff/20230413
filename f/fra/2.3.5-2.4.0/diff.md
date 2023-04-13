# Comparing `tmp/fra-2.3.5.tar.gz` & `tmp/fra-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fra-2.3.5.tar", max compression
+gzip compressed data, was "fra-2.4.0.tar", max compression
```

## Comparing `fra-2.3.5.tar` & `fra-2.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2023-03-15 23:08:27.832029 fra-2.3.5/LICENSE
--rw-r--r--   0        0        0     1446 2023-04-12 00:25:23.546185 fra-2.3.5/README.md
--rw-r--r--   0        0        0    85510 2023-03-15 23:08:27.836029 fra-2.3.5/docs/architecture_1.png
--rw-r--r--   0        0        0       41 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/README
--rw-r--r--   0        0        0      857 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/alembic.ini
--rw-r--r--   0        0        0     2745 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/env.py
--rw-r--r--   0        0        0      494 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/script.py.mako
--rw-r--r--   0        0        0     1056 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/222c027bbdec_file_type.py
--rw-r--r--   0        0        0     1239 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/55161145af8f_add_user_recommendations_model.py
--rw-r--r--   0        0        0      937 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/5c34861d9ef9_add_file_to_organization.py
--rw-r--r--   0        0        0     2337 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/78c25d669d9c_first_models.py
--rw-r--r--   0        0        0      956 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py
--rw-r--r--   0        0        0      757 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py
--rw-r--r--   0        0        0     1463 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/ff9e18b937bd_.py
--rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/motor/__init__.py
--rw-r--r--   0        0        0      237 2023-03-15 23:08:30.335994 fra-2.3.5/motor/adaptors.py
--rw-r--r--   0        0        0     2963 2023-03-15 23:08:30.335994 fra-2.3.5/motor/models.py
--rw-r--r--   0        0        0     5842 2023-03-15 23:08:30.335994 fra-2.3.5/motor/processor.py
--rw-r--r--   0        0        0      376 2023-03-15 23:08:30.335994 fra-2.3.5/motor/tasks.py
--rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/organizations/__init__.py
--rw-r--r--   0        0        0      447 2023-03-15 23:08:30.335994 fra-2.3.5/organizations/models.py
--rw-r--r--   0        0        0      804 2023-04-12 00:22:24.590617 fra-2.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/__init__.py
--rw-r--r--   0        0        0     2207 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/file_loader.py
--rw-r--r--   0        0        0     1919 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/organizations.py
--rw-r--r--   0        0        0      813 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/recommendations.py
--rw-r--r--   0        0        0      632 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/register_all_handlers.py
--rw-r--r--   0        0        0     2404 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/user_ratings.py
--rw-r--r--   0        0        0     1237 2023-03-15 23:08:30.335994 fra-2.3.5/server/app.py
--rw-r--r--   0        0        0     1226 2023-03-15 23:08:30.335994 fra-2.3.5/server/config.py
--rw-r--r--   0        0        0      118 2023-03-15 23:08:30.335994 fra-2.3.5/server/database.py
--rw-r--r--   0        0        0      464 2023-04-12 00:22:34.571618 fra-2.3.5/server/rebar.py
--rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/__init__.py
--rw-r--r--   0        0        0      445 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/file_data.py
--rw-r--r--   0        0        0      276 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/general.py
--rw-r--r--   0        0        0      731 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/organization.py
--rw-r--r--   0        0        0      950 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/user_ratings.py
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 fra-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-15 23:08:27.832029 fra-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1446 2023-04-12 00:25:23.546185 fra-2.4.0/README.md
+-rw-r--r--   0        0        0    85510 2023-03-15 23:08:27.836029 fra-2.4.0/docs/architecture_1.png
+-rw-r--r--   0        0        0       41 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/README
+-rw-r--r--   0        0        0      857 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/alembic.ini
+-rw-r--r--   0        0        0     2745 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/script.py.mako
+-rw-r--r--   0        0        0     1056 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/222c027bbdec_file_type.py
+-rw-r--r--   0        0        0     1239 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/55161145af8f_add_user_recommendations_model.py
+-rw-r--r--   0        0        0      937 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/5c34861d9ef9_add_file_to_organization.py
+-rw-r--r--   0        0        0     2337 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/78c25d669d9c_first_models.py
+-rw-r--r--   0        0        0      956 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py
+-rw-r--r--   0        0        0      757 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py
+-rw-r--r--   0        0        0     1463 2023-03-15 23:08:30.335994 fra-2.4.0/migrations/versions/ff9e18b937bd_.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.4.0/motor/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-13 02:05:16.398257 fra-2.4.0/motor/adaptors.py
+-rw-r--r--   0        0        0     2963 2023-03-15 23:08:30.335994 fra-2.4.0/motor/models.py
+-rw-r--r--   0        0        0     5843 2023-04-13 02:20:52.612003 fra-2.4.0/motor/processor.py
+-rw-r--r--   0        0        0      376 2023-03-15 23:08:30.335994 fra-2.4.0/motor/tasks.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.4.0/organizations/__init__.py
+-rw-r--r--   0        0        0      447 2023-03-15 23:08:30.335994 fra-2.4.0/organizations/models.py
+-rw-r--r--   0        0        0      804 2023-04-13 15:58:01.124609 fra-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.4.0/server/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.4.0/server/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.4.0/server/api/handlers/__init__.py
+-rw-r--r--   0        0        0     2319 2023-04-13 02:29:17.250074 fra-2.4.0/server/api/handlers/file_loader.py
+-rw-r--r--   0        0        0     1916 2023-04-13 01:51:17.561440 fra-2.4.0/server/api/handlers/organizations.py
+-rw-r--r--   0        0        0      813 2023-03-15 23:08:30.335994 fra-2.4.0/server/api/handlers/recommendations.py
+-rw-r--r--   0        0        0      632 2023-03-15 23:08:30.335994 fra-2.4.0/server/api/handlers/register_all_handlers.py
+-rw-r--r--   0        0        0     2404 2023-03-15 23:08:30.335994 fra-2.4.0/server/api/handlers/user_ratings.py
+-rw-r--r--   0        0        0     1237 2023-03-15 23:08:30.335994 fra-2.4.0/server/app.py
+-rw-r--r--   0        0        0     1229 2023-04-13 15:57:44.508572 fra-2.4.0/server/config.py
+-rw-r--r--   0        0        0      118 2023-03-15 23:08:30.335994 fra-2.4.0/server/database.py
+-rw-r--r--   0        0        0      464 2023-04-12 00:22:34.571618 fra-2.4.0/server/rebar.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.4.0/server/schemas/__init__.py
+-rw-r--r--   0        0        0      445 2023-03-15 23:08:30.335994 fra-2.4.0/server/schemas/file_data.py
+-rw-r--r--   0        0        0      276 2023-03-15 23:08:30.335994 fra-2.4.0/server/schemas/general.py
+-rw-r--r--   0        0        0      731 2023-03-15 23:08:30.335994 fra-2.4.0/server/schemas/organization.py
+-rw-r--r--   0        0        0      950 2023-03-15 23:08:30.335994 fra-2.4.0/server/schemas/user_ratings.py
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 fra-2.4.0/PKG-INFO
```

### Comparing `fra-2.3.5/LICENSE` & `fra-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/README.md` & `fra-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/docs/architecture_1.png` & `fra-2.4.0/docs/architecture_1.png`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/alembic.ini` & `fra-2.4.0/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/env.py` & `fra-2.4.0/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/222c027bbdec_file_type.py` & `fra-2.4.0/migrations/versions/222c027bbdec_file_type.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/55161145af8f_add_user_recommendations_model.py` & `fra-2.4.0/migrations/versions/55161145af8f_add_user_recommendations_model.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/5c34861d9ef9_add_file_to_organization.py` & `fra-2.4.0/migrations/versions/5c34861d9ef9_add_file_to_organization.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/78c25d669d9c_first_models.py` & `fra-2.4.0/migrations/versions/78c25d669d9c_first_models.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py` & `fra-2.4.0/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py` & `fra-2.4.0/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/migrations/versions/ff9e18b937bd_.py` & `fra-2.4.0/migrations/versions/ff9e18b937bd_.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/motor/models.py` & `fra-2.4.0/motor/models.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/motor/processor.py` & `fra-2.4.0/motor/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def load_file(organization_id: UUID, file_type: str):
     raw_file = RawFileModel.query.filter_by(
         organization_id=organization_id, file_type=file_type
     ).first()
     with open(
-        os.path.join(basedir + f"uploads/{organization_id}", raw_file.filename), "r"
+        os.path.join(basedir + f"/uploads/{organization_id}", raw_file.filename), "r"
     ) as file:
         return (
             pd.read_csv(file),
             FileMapModel.query.filter_by(file_id=raw_file.id).first(),
         )
```

### Comparing `fra-2.3.5/pyproject.toml` & `fra-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fra"
-version = "2.3.5"
+version = "2.4.0"
 description = "Simple Recommendation System, content based."
 authors = ["Eliecer Daza"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/elin3t/fra"
 packages = [
     { include = "server"},
```

### Comparing `fra-2.3.5/server/api/handlers/file_loader.py` & `fra-2.4.0/server/api/handlers/file_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     rule="/organization/<uuid:organization_id>/dataset/add",
     method="POST",
     mimetype="multipart/form-data",
 )
 def file_upload(organization_id: UUID):
     """
     Upload files for train the model.
+    ::params:: file: binary file
+    ::params:: file_type: optional, "data", "ratings", "other", default "data"
     """
     file = request.files["file"]
     file_name = file.filename
     if file_name == "":
         return {"msg": "empty filename"}, 400
 
     file_type = request.form.get("file_type")
```

### Comparing `fra-2.3.5/server/api/handlers/organizations.py` & `fra-2.4.0/server/api/handlers/organizations.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,9 +55,9 @@
     """
     Return all the users in the organization
     """
     organization_users = UserOrganization.query.filter_by(
         organization_id=organization_id
     ).all()
     users_ids = [user.user_id for user in organization_users]
-    users = UserModel.query.filter_by(UserModel.id.in_(users_ids)).all()
+    users = UserModel.query.filter(UserModel.id.in_(users_ids)).all()
     return users, 200
```

### Comparing `fra-2.3.5/server/api/handlers/recommendations.py` & `fra-2.4.0/server/api/handlers/recommendations.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/server/api/handlers/register_all_handlers.py` & `fra-2.4.0/server/api/handlers/register_all_handlers.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/server/api/handlers/user_ratings.py` & `fra-2.4.0/server/api/handlers/user_ratings.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/server/app.py` & `fra-2.4.0/server/app.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/server/config.py` & `fra-2.4.0/server/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 basedir = os.path.abspath(os.path.dirname(__file__))
-postgres_local_base = os.getenv("FRA_DB_URL","postgresql://postgres:@localhost/")
-database_name = os.getenv("FRA_DB_NAME","content_based_data")
+postgres_local_base = os.getenv("FRA_DB_URL", "postgresql://postgres:postgres@db/")
+database_name = os.getenv("FRA_DB_NAME", "content_based_data")
 
 
 class BaseConfig:
     """Base configuration."""
 
     SECRET_KEY = os.getenv("FRA_SECRET_KEY", "my_precious")
     DEBUG = False
```

### Comparing `fra-2.3.5/server/schemas/organization.py` & `fra-2.4.0/server/schemas/organization.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/server/schemas/user_ratings.py` & `fra-2.4.0/server/schemas/user_ratings.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.5/PKG-INFO` & `fra-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fra
-Version: 2.3.5
+Version: 2.4.0
 Summary: Simple Recommendation System, content based.
 Home-page: https://gitlab.com/elin3t/fra
 License: MIT
 Author: Eliecer Daza
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

