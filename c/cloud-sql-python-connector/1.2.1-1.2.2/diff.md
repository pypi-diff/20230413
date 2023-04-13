# Comparing `tmp/cloud-sql-python-connector-1.2.1.tar.gz` & `tmp/cloud-sql-python-connector-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-sql-python-connector-1.2.1.tar", last modified: Tue Mar 14 19:09:58 2023, max compression
+gzip compressed data, was "cloud-sql-python-connector-1.2.2.tar", last modified: Thu Apr 13 19:16:41 2023, max compression
```

## Comparing `cloud-sql-python-connector-1.2.1.tar` & `cloud-sql-python-connector-1.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-14 19:09:58.689749 cloud-sql-python-connector-1.2.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/LICENSE
--rw-r--r--   0 root         (0)     1003    21638 2023-03-14 19:09:58.689749 cloud-sql-python-connector-1.2.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    20491 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-14 19:09:58.685747 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    21638 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      935 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      156 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-14 19:09:58.000000 cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-14 19:09:58.685747 cloud-sql-python-connector-1.2.1/google/
--rw-rw-r--   0 root         (0)     1003      746 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-14 19:09:58.685747 cloud-sql-python-connector-1.2.1/google/cloud/
--rw-rw-r--   0 root         (0)     1003      746 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-14 19:09:58.685747 cloud-sql-python-connector-1.2.1/google/cloud/sql/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-14 19:09:58.689749 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/
--rw-rw-r--   0 root         (0)     1003      876 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     1838 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/asyncpg.py
--rwxrwxr-x   0 root         (0)     1003    13625 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/connector.py
--rw-rw-r--   0 root         (0)     1003     1454 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003    17656 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     2031 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003     1926 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/pymysql.py
--rw-rw-r--   0 root         (0)     1003     2451 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/pytds.py
--rw-rw-r--   0 root         (0)     1003     2954 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     9329 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/refresh_utils.py
--rwxrwxr-x   0 root         (0)     1003     4371 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/version.py
--rw-rw-r--   0 root         (0)     1003       67 2023-03-14 19:09:58.689749 cloud-sql-python-connector-1.2.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2871 2023-03-14 19:08:58.000000 cloud-sql-python-connector-1.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/LICENSE
+-rw-r--r--   0 root         (0)     1003    21826 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    20679 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    21826 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      935 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      156 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/
+-rw-rw-r--   0 root         (0)     1003      746 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      746 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/cloud/sql/
+-rw-rw-r--   0 root         (0)     1003        0 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/
+-rw-rw-r--   0 root         (0)     1003      876 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1838 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/asyncpg.py
+-rwxrwxr-x   0 root         (0)     1003    13625 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003     1454 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    17656 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     2031 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003     1926 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pymysql.py
+-rw-rw-r--   0 root         (0)     1003     2451 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pytds.py
+-rw-rw-r--   0 root         (0)     1003     2954 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     9329 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/refresh_utils.py
+-rwxrwxr-x   0 root         (0)     1003     4371 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/version.py
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-13 19:16:41.734187 cloud-sql-python-connector-1.2.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2871 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/setup.py
```

### Comparing `cloud-sql-python-connector-1.2.1/LICENSE` & `cloud-sql-python-connector-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/PKG-INFO` & `cloud-sql-python-connector-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -136,14 +136,15 @@
 object and call it's `connect` method with the proper input parameters.
 
 The `Connector` itself creates connection objects by calling its `connect` method but does not manage database connection pooling. For this reason, it is recommended to use the connector alongside a library that can create connection pools, such as [SQLAlchemy](https://www.sqlalchemy.org/). This will allow for connections to remain open and be reused, reducing connection overhead and the number of connections needed.
 
 In the Connector's `connect` method below, input your connection string as the first positional argument and the name of the database driver for the second positional argument. Insert the rest of your connection keyword arguments like user, password and database. You can also set the optional `timeout` or `ip_type` keyword arguments.
 
 To use this connector with SQLAlchemy, use the `creator` argument for `sqlalchemy.create_engine`:
+
 ```python
 from google.cloud.sql.connector import Connector
 import sqlalchemy
 
 # initialize Connector object
 connector = Connector()
 
@@ -162,27 +163,31 @@
 pool = sqlalchemy.create_engine(
     "mysql+pymysql://",
     creator=getconn,
 )
 ```
 
 The returned connection pool engine can then be used to query and modify the database.
+
 ```python
 # insert statement
 insert_stmt = sqlalchemy.text(
     "INSERT INTO my_table (id, title) VALUES (:id, :title)",
 )
 
 with pool.connect() as db_conn:
     # insert into database
     db_conn.execute(insert_stmt, parameters={"id": "book1", "title": "Book One"})
 
     # query database
     result = db_conn.execute(sqlalchemy.text("SELECT * from my_table")).fetchall()
 
+    # commit transaction (SQLAlchemy v2.X.X is commit as you go)
+    db_conn.commit()
+
     # Do something with the results
     for row in result:
         print(row)
 ```
 
 To close the `Connector` object's background resources, call it's `close()` method as follows:
 
@@ -248,91 +253,104 @@
 )
 
 # interact with Cloud SQL database using connection pool
 with pool.connect() as db_conn:
     # insert into database
     db_conn.execute(insert_stmt, parameters={"id": "book1", "title": "Book One"})
 
+    # commit transaction (SQLAlchemy v2.X.X is commit as you go)
+    db_conn.commit()
+
     # query database
     result = db_conn.execute(sqlalchemy.text("SELECT * from my_table")).fetchall()
 
     # Do something with the results
     for row in result:
         print(row)
 ```
 
 ### Specifying Public or Private IP
+
 The Cloud SQL Connector for Python can be used to connect to Cloud SQL instances using both public and private IP addresses. To specify which IP address to use to connect, set the `ip_type` keyword argument Possible values are `IPTypes.PUBLIC` and `IPTypes.PRIVATE`.
 Example:
+
 ```python
 from google.cloud.sql.connector import IPTypes
 
 connector.connect(
     "project:region:instance",
     "pymysql",
     ip_type=IPTypes.PRIVATE # use private IP
 ... insert other kwargs ...
 )
 ```
 
 Note: If specifying Private IP, your application must already be in the same VPC network as your Cloud SQL Instance.
 
 ### IAM Authentication
+
 Connections using [Automatic IAM database authentication](https://cloud.google.com/sql/docs/postgres/authentication#automatic) are supported when using Postgres or MySQL drivers.
 First, make sure to [configure your Cloud SQL Instance to allow IAM authentication](https://cloud.google.com/sql/docs/postgres/create-edit-iam-instances#configure-iam-db-instance)
 and [add an IAM database user](https://cloud.google.com/sql/docs/postgres/create-manage-iam-users#creating-a-database-user).
 
 Now, you can connect using user or service account credentials instead of a password.
 In the call to connect, set the `enable_iam_auth` keyword argument to true and the `user` argument to the appropriately formatted IAM principal.
 > Postgres: For an IAM user account, this is the user's email address. For a service account, it is the service account's email without the `.gserviceaccount.com` domain suffix.
 
 > MySQL: For an IAM user account, this is the user's email address, without the @ or domain name. For example, for `test-user@gmail.com`, set the `user` argument to `test-user`. For a service account, this is the service account's email address without the `@project-id.iam.gserviceaccount.com` suffix.
 
 Example:
+
 ```python
 connector.connect(
      "project:region:instance",
      "pg8000",
      user="postgres-iam-user@gmail.com",
      db="my-db-name",
      enable_iam_auth=True,
  )
 ```
 
 ### SQL Server Active Directory Authentication
+
 Active Directory authentication for SQL Server instances is currently only supported on Windows. First, make sure to follow [these steps](https://cloud.google.com/blog/topics/developers-practitioners/creating-sql-server-instance-integrated-active-directory-using-google-cloud-sql) to set up a Managed AD domain and join your Cloud SQL instance to the domain. [See here for more info on Cloud SQL Active Directory integration](https://cloud.google.com/sql/docs/sqlserver/ad).
 
 Once you have followed the steps linked above, you can run the following code to return a connection object:
+
 ```python
 connector.connect(
     "project:region:instance",
     "pytds",
     db="my-db-name",
     active_directory_auth=True,
     server_name="public.[instance].[location].[project].cloudsql.[domain]",
 )
 ```
+
 Or, if using Private IP:
+
 ```python
 connector.connect(
     "project:region:instance",
     "pytds",
     db="my-db-name",
     active_directory_auth=True,
     server_name="private.[instance].[location].[project].cloudsql.[domain]",
     ip_type=IPTypes.PRIVATE
 )
 ```
 
 ### Using the Python Connector with Python Web Frameworks
+
 The Python Connector can be used alongside popular Python web frameworks such
 as Flask, FastAPI, etc, to integrate Cloud SQL databases within your
 web applications.
 
 #### Flask-SQLAlchemy
+
 [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
 is an extension for [Flask](https://flask.palletsprojects.com/en/2.2.x/)
 that adds support for [SQLAlchemy](https://www.sqlalchemy.org/) to your
 application. It aims to simplify using SQLAlchemy with Flask by providing
 useful defaults and extra helpers that make it easier to accomplish
 common tasks.
 
@@ -370,14 +388,15 @@
 db = SQLAlchemy(app)
 ```
 
 For more details on how to use Flask-SQLAlchemy, check out the
 [Flask-SQLAlchemy Quickstarts](https://flask-sqlalchemy.palletsprojects.com/en/2.x/quickstart/#)
 
 #### FastAPI
+
 [FastAPI](https://fastapi.tiangolo.com/) is a modern, fast (high-performance),
 web framework for building APIs with Python based on standard Python type hints.
 
 You can configure FastAPI to connect to a Cloud SQL database from
 your web application using [SQLAlchemy ORM](https://docs.sqlalchemy.org/en/14/orm/)
 through the following:
 
@@ -412,14 +431,15 @@
 Base = declarative_base()
 ```
 
 To learn more about integrating a database into your FastAPI application,
 follow along the [FastAPI SQL Database guide](https://fastapi.tiangolo.com/tutorial/sql-databases/#create-the-database-models).
 
 ### Async Driver Usage
+
 The Cloud SQL Connector is compatible with
 [asyncio](https://docs.python.org/3/library/asyncio.html) to improve the speed
 and efficiency of database connections through concurrency. You can use all
 non-asyncio drivers through the `Connector.connect_async` function, in addition
 to the following asyncio database drivers:
 - [asyncpg](https://magicstack.github.io/asyncpg) (Postgres)
```

### Comparing `cloud-sql-python-connector-1.2.1/README.md` & `cloud-sql-python-connector-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 object and call it's `connect` method with the proper input parameters.
 
 The `Connector` itself creates connection objects by calling its `connect` method but does not manage database connection pooling. For this reason, it is recommended to use the connector alongside a library that can create connection pools, such as [SQLAlchemy](https://www.sqlalchemy.org/). This will allow for connections to remain open and be reused, reducing connection overhead and the number of connections needed.
 
 In the Connector's `connect` method below, input your connection string as the first positional argument and the name of the database driver for the second positional argument. Insert the rest of your connection keyword arguments like user, password and database. You can also set the optional `timeout` or `ip_type` keyword arguments.
 
 To use this connector with SQLAlchemy, use the `creator` argument for `sqlalchemy.create_engine`:
+
 ```python
 from google.cloud.sql.connector import Connector
 import sqlalchemy
 
 # initialize Connector object
 connector = Connector()
 
@@ -136,27 +137,31 @@
 pool = sqlalchemy.create_engine(
     "mysql+pymysql://",
     creator=getconn,
 )
 ```
 
 The returned connection pool engine can then be used to query and modify the database.
+
 ```python
 # insert statement
 insert_stmt = sqlalchemy.text(
     "INSERT INTO my_table (id, title) VALUES (:id, :title)",
 )
 
 with pool.connect() as db_conn:
     # insert into database
     db_conn.execute(insert_stmt, parameters={"id": "book1", "title": "Book One"})
 
     # query database
     result = db_conn.execute(sqlalchemy.text("SELECT * from my_table")).fetchall()
 
+    # commit transaction (SQLAlchemy v2.X.X is commit as you go)
+    db_conn.commit()
+
     # Do something with the results
     for row in result:
         print(row)
 ```
 
 To close the `Connector` object's background resources, call it's `close()` method as follows:
 
@@ -222,91 +227,104 @@
 )
 
 # interact with Cloud SQL database using connection pool
 with pool.connect() as db_conn:
     # insert into database
     db_conn.execute(insert_stmt, parameters={"id": "book1", "title": "Book One"})
 
+    # commit transaction (SQLAlchemy v2.X.X is commit as you go)
+    db_conn.commit()
+
     # query database
     result = db_conn.execute(sqlalchemy.text("SELECT * from my_table")).fetchall()
 
     # Do something with the results
     for row in result:
         print(row)
 ```
 
 ### Specifying Public or Private IP
+
 The Cloud SQL Connector for Python can be used to connect to Cloud SQL instances using both public and private IP addresses. To specify which IP address to use to connect, set the `ip_type` keyword argument Possible values are `IPTypes.PUBLIC` and `IPTypes.PRIVATE`.
 Example:
+
 ```python
 from google.cloud.sql.connector import IPTypes
 
 connector.connect(
     "project:region:instance",
     "pymysql",
     ip_type=IPTypes.PRIVATE # use private IP
 ... insert other kwargs ...
 )
 ```
 
 Note: If specifying Private IP, your application must already be in the same VPC network as your Cloud SQL Instance.
 
 ### IAM Authentication
+
 Connections using [Automatic IAM database authentication](https://cloud.google.com/sql/docs/postgres/authentication#automatic) are supported when using Postgres or MySQL drivers.
 First, make sure to [configure your Cloud SQL Instance to allow IAM authentication](https://cloud.google.com/sql/docs/postgres/create-edit-iam-instances#configure-iam-db-instance)
 and [add an IAM database user](https://cloud.google.com/sql/docs/postgres/create-manage-iam-users#creating-a-database-user).
 
 Now, you can connect using user or service account credentials instead of a password.
 In the call to connect, set the `enable_iam_auth` keyword argument to true and the `user` argument to the appropriately formatted IAM principal.
 > Postgres: For an IAM user account, this is the user's email address. For a service account, it is the service account's email without the `.gserviceaccount.com` domain suffix.
 
 > MySQL: For an IAM user account, this is the user's email address, without the @ or domain name. For example, for `test-user@gmail.com`, set the `user` argument to `test-user`. For a service account, this is the service account's email address without the `@project-id.iam.gserviceaccount.com` suffix.
 
 Example:
+
 ```python
 connector.connect(
      "project:region:instance",
      "pg8000",
      user="postgres-iam-user@gmail.com",
      db="my-db-name",
      enable_iam_auth=True,
  )
 ```
 
 ### SQL Server Active Directory Authentication
+
 Active Directory authentication for SQL Server instances is currently only supported on Windows. First, make sure to follow [these steps](https://cloud.google.com/blog/topics/developers-practitioners/creating-sql-server-instance-integrated-active-directory-using-google-cloud-sql) to set up a Managed AD domain and join your Cloud SQL instance to the domain. [See here for more info on Cloud SQL Active Directory integration](https://cloud.google.com/sql/docs/sqlserver/ad).
 
 Once you have followed the steps linked above, you can run the following code to return a connection object:
+
 ```python
 connector.connect(
     "project:region:instance",
     "pytds",
     db="my-db-name",
     active_directory_auth=True,
     server_name="public.[instance].[location].[project].cloudsql.[domain]",
 )
 ```
+
 Or, if using Private IP:
+
 ```python
 connector.connect(
     "project:region:instance",
     "pytds",
     db="my-db-name",
     active_directory_auth=True,
     server_name="private.[instance].[location].[project].cloudsql.[domain]",
     ip_type=IPTypes.PRIVATE
 )
 ```
 
 ### Using the Python Connector with Python Web Frameworks
+
 The Python Connector can be used alongside popular Python web frameworks such
 as Flask, FastAPI, etc, to integrate Cloud SQL databases within your
 web applications.
 
 #### Flask-SQLAlchemy
+
 [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
 is an extension for [Flask](https://flask.palletsprojects.com/en/2.2.x/)
 that adds support for [SQLAlchemy](https://www.sqlalchemy.org/) to your
 application. It aims to simplify using SQLAlchemy with Flask by providing
 useful defaults and extra helpers that make it easier to accomplish
 common tasks.
 
@@ -344,14 +362,15 @@
 db = SQLAlchemy(app)
 ```
 
 For more details on how to use Flask-SQLAlchemy, check out the
 [Flask-SQLAlchemy Quickstarts](https://flask-sqlalchemy.palletsprojects.com/en/2.x/quickstart/#)
 
 #### FastAPI
+
 [FastAPI](https://fastapi.tiangolo.com/) is a modern, fast (high-performance),
 web framework for building APIs with Python based on standard Python type hints.
 
 You can configure FastAPI to connect to a Cloud SQL database from
 your web application using [SQLAlchemy ORM](https://docs.sqlalchemy.org/en/14/orm/)
 through the following:
 
@@ -386,14 +405,15 @@
 Base = declarative_base()
 ```
 
 To learn more about integrating a database into your FastAPI application,
 follow along the [FastAPI SQL Database guide](https://fastapi.tiangolo.com/tutorial/sql-databases/#create-the-database-models).
 
 ### Async Driver Usage
+
 The Cloud SQL Connector is compatible with
 [asyncio](https://docs.python.org/3/library/asyncio.html) to improve the speed
 and efficiency of database connections through concurrency. You can use all
 non-asyncio drivers through the `Connector.connect_async` function, in addition
 to the following asyncio database drivers:
 - [asyncpg](https://magicstack.github.io/asyncpg) (Postgres)
```

### Comparing `cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/PKG-INFO` & `cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -136,14 +136,15 @@
 object and call it's `connect` method with the proper input parameters.
 
 The `Connector` itself creates connection objects by calling its `connect` method but does not manage database connection pooling. For this reason, it is recommended to use the connector alongside a library that can create connection pools, such as [SQLAlchemy](https://www.sqlalchemy.org/). This will allow for connections to remain open and be reused, reducing connection overhead and the number of connections needed.
 
 In the Connector's `connect` method below, input your connection string as the first positional argument and the name of the database driver for the second positional argument. Insert the rest of your connection keyword arguments like user, password and database. You can also set the optional `timeout` or `ip_type` keyword arguments.
 
 To use this connector with SQLAlchemy, use the `creator` argument for `sqlalchemy.create_engine`:
+
 ```python
 from google.cloud.sql.connector import Connector
 import sqlalchemy
 
 # initialize Connector object
 connector = Connector()
 
@@ -162,27 +163,31 @@
 pool = sqlalchemy.create_engine(
     "mysql+pymysql://",
     creator=getconn,
 )
 ```
 
 The returned connection pool engine can then be used to query and modify the database.
+
 ```python
 # insert statement
 insert_stmt = sqlalchemy.text(
     "INSERT INTO my_table (id, title) VALUES (:id, :title)",
 )
 
 with pool.connect() as db_conn:
     # insert into database
     db_conn.execute(insert_stmt, parameters={"id": "book1", "title": "Book One"})
 
     # query database
     result = db_conn.execute(sqlalchemy.text("SELECT * from my_table")).fetchall()
 
+    # commit transaction (SQLAlchemy v2.X.X is commit as you go)
+    db_conn.commit()
+
     # Do something with the results
     for row in result:
         print(row)
 ```
 
 To close the `Connector` object's background resources, call it's `close()` method as follows:
 
@@ -248,91 +253,104 @@
 )
 
 # interact with Cloud SQL database using connection pool
 with pool.connect() as db_conn:
     # insert into database
     db_conn.execute(insert_stmt, parameters={"id": "book1", "title": "Book One"})
 
+    # commit transaction (SQLAlchemy v2.X.X is commit as you go)
+    db_conn.commit()
+
     # query database
     result = db_conn.execute(sqlalchemy.text("SELECT * from my_table")).fetchall()
 
     # Do something with the results
     for row in result:
         print(row)
 ```
 
 ### Specifying Public or Private IP
+
 The Cloud SQL Connector for Python can be used to connect to Cloud SQL instances using both public and private IP addresses. To specify which IP address to use to connect, set the `ip_type` keyword argument Possible values are `IPTypes.PUBLIC` and `IPTypes.PRIVATE`.
 Example:
+
 ```python
 from google.cloud.sql.connector import IPTypes
 
 connector.connect(
     "project:region:instance",
     "pymysql",
     ip_type=IPTypes.PRIVATE # use private IP
 ... insert other kwargs ...
 )
 ```
 
 Note: If specifying Private IP, your application must already be in the same VPC network as your Cloud SQL Instance.
 
 ### IAM Authentication
+
 Connections using [Automatic IAM database authentication](https://cloud.google.com/sql/docs/postgres/authentication#automatic) are supported when using Postgres or MySQL drivers.
 First, make sure to [configure your Cloud SQL Instance to allow IAM authentication](https://cloud.google.com/sql/docs/postgres/create-edit-iam-instances#configure-iam-db-instance)
 and [add an IAM database user](https://cloud.google.com/sql/docs/postgres/create-manage-iam-users#creating-a-database-user).
 
 Now, you can connect using user or service account credentials instead of a password.
 In the call to connect, set the `enable_iam_auth` keyword argument to true and the `user` argument to the appropriately formatted IAM principal.
 > Postgres: For an IAM user account, this is the user's email address. For a service account, it is the service account's email without the `.gserviceaccount.com` domain suffix.
 
 > MySQL: For an IAM user account, this is the user's email address, without the @ or domain name. For example, for `test-user@gmail.com`, set the `user` argument to `test-user`. For a service account, this is the service account's email address without the `@project-id.iam.gserviceaccount.com` suffix.
 
 Example:
+
 ```python
 connector.connect(
      "project:region:instance",
      "pg8000",
      user="postgres-iam-user@gmail.com",
      db="my-db-name",
      enable_iam_auth=True,
  )
 ```
 
 ### SQL Server Active Directory Authentication
+
 Active Directory authentication for SQL Server instances is currently only supported on Windows. First, make sure to follow [these steps](https://cloud.google.com/blog/topics/developers-practitioners/creating-sql-server-instance-integrated-active-directory-using-google-cloud-sql) to set up a Managed AD domain and join your Cloud SQL instance to the domain. [See here for more info on Cloud SQL Active Directory integration](https://cloud.google.com/sql/docs/sqlserver/ad).
 
 Once you have followed the steps linked above, you can run the following code to return a connection object:
+
 ```python
 connector.connect(
     "project:region:instance",
     "pytds",
     db="my-db-name",
     active_directory_auth=True,
     server_name="public.[instance].[location].[project].cloudsql.[domain]",
 )
 ```
+
 Or, if using Private IP:
+
 ```python
 connector.connect(
     "project:region:instance",
     "pytds",
     db="my-db-name",
     active_directory_auth=True,
     server_name="private.[instance].[location].[project].cloudsql.[domain]",
     ip_type=IPTypes.PRIVATE
 )
 ```
 
 ### Using the Python Connector with Python Web Frameworks
+
 The Python Connector can be used alongside popular Python web frameworks such
 as Flask, FastAPI, etc, to integrate Cloud SQL databases within your
 web applications.
 
 #### Flask-SQLAlchemy
+
 [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
 is an extension for [Flask](https://flask.palletsprojects.com/en/2.2.x/)
 that adds support for [SQLAlchemy](https://www.sqlalchemy.org/) to your
 application. It aims to simplify using SQLAlchemy with Flask by providing
 useful defaults and extra helpers that make it easier to accomplish
 common tasks.
 
@@ -370,14 +388,15 @@
 db = SQLAlchemy(app)
 ```
 
 For more details on how to use Flask-SQLAlchemy, check out the
 [Flask-SQLAlchemy Quickstarts](https://flask-sqlalchemy.palletsprojects.com/en/2.x/quickstart/#)
 
 #### FastAPI
+
 [FastAPI](https://fastapi.tiangolo.com/) is a modern, fast (high-performance),
 web framework for building APIs with Python based on standard Python type hints.
 
 You can configure FastAPI to connect to a Cloud SQL database from
 your web application using [SQLAlchemy ORM](https://docs.sqlalchemy.org/en/14/orm/)
 through the following:
 
@@ -412,14 +431,15 @@
 Base = declarative_base()
 ```
 
 To learn more about integrating a database into your FastAPI application,
 follow along the [FastAPI SQL Database guide](https://fastapi.tiangolo.com/tutorial/sql-databases/#create-the-database-models).
 
 ### Async Driver Usage
+
 The Cloud SQL Connector is compatible with
 [asyncio](https://docs.python.org/3/library/asyncio.html) to improve the speed
 and efficiency of database connections through concurrency. You can use all
 non-asyncio drivers through the `Connector.connect_async` function, in addition
 to the following asyncio database drivers:
 - [asyncpg](https://magicstack.github.io/asyncpg) (Postgres)
```

### Comparing `cloud-sql-python-connector-1.2.1/cloud_sql_python_connector.egg-info/SOURCES.txt` & `cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/__init__.py` & `cloud-sql-python-connector-1.2.2/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/__init__.py` & `cloud-sql-python-connector-1.2.2/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/__init__.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/asyncpg.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/connector.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/connector.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/exceptions.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/instance.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/instance.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/pg8000.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/pymysql.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pymysql.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/pytds.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pytds.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/rate_limiter.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/refresh_utils.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/refresh_utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/utils.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.1/google/cloud/sql/connector/version.py` & `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
```

### Comparing `cloud-sql-python-connector-1.2.1/setup.py` & `cloud-sql-python-connector-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         "Programming Language :: Python :: 3.11",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     namespace_packages=namespaces,
     install_requires=core_dependencies,
     extras_require={
-        "pymysql": ["PyMySQL==1.0.2"],
+        "pymysql": ["PyMySQL==1.0.3"],
         "pg8000": ["pg8000==1.29.4"],
         "pytds": ["python-tds==1.12.0"],
         "asyncpg": ["asyncpg==0.27.0"]
     },
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
```

