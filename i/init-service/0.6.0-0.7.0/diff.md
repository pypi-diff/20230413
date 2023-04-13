# Comparing `tmp/init_service-0.6.0.tar.gz` & `tmp/init_service-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_service-0.6.0.tar", max compression
+gzip compressed data, was "init_service-0.7.0.tar", max compression
```

## Comparing `init_service-0.6.0.tar` & `init_service-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-03-24 15:57:40.744794 init_service-0.6.0/LICENSE
--rw-r--r--   0        0        0      683 2023-03-24 15:57:40.744794 init_service-0.6.0/init_service/__init__.py
--rw-r--r--   0        0        0    10586 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/init_service.py
--rw-r--r--   0        0        0    50425 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/pyratemp.py
--rw-r--r--   0        0        0      353 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/.gitignore
--rw-r--r--   0        0        0      299 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/build.sbt
--rw-r--r--   0        0        0      308 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/project/LibDependencies.scala
--rw-r--r--   0        0        0       28 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/project/build.properties
--rw-r--r--   0        0        0      369 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/project/plugins.sbt
--rw-r--r--   0        0        0       82 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/src/main/scala/uk/gov/hmrc/hello/HelloWorld.scala
--rw-r--r--   0        0        0      275 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/library/src/test/scala/uk/gov/hmrc/hello/HelloWorldSpec.scala
--rw-r--r--   0        0        0      353 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/.gitignore
--rw-r--r--   0        0        0       41 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/assets/stylesheets/application.scss
--rw-r--r--   0        0        0      447 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/config/AppConfig.scala
--rw-r--r--   0        0        0      626 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/config/ErrorHandler.scala
--rw-r--r--   0        0        0      221 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/config/Module.scala
--rw-r--r--   0        0        0      620 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/controllers/HelloWorldController.scala
--rw-r--r--   0        0        0      503 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/controllers/MicroserviceHelloWorldController.scala
--rw-r--r--   0        0        0      374 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/views/ErrorTemplate.scala.html
--rw-r--r--   0        0        0      260 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/views/HelloWorldPage.scala.html
--rw-r--r--   0        0        0      454 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/app/views/Layout.scala.html
--rw-r--r--   0        0        0      855 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/build.sbt
--rw-r--r--   0        0        0      472 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/app.routes
--rw-r--r--   0        0        0      300 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/application-json-logger.xml
--rw-r--r--   0        0        0     3359 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/application.conf
--rw-r--r--   0        0        0     2337 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/logback.xml
--rw-r--r--   0        0        0       68 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/messages
--rw-r--r--   0        0        0       69 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/messages.cy
--rw-r--r--   0        0        0      247 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/prod.routes
--rw-r--r--   0        0        0     1098 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes
--rw-r--r--   0        0        0     1024 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala
--rw-r--r--   0        0        0     1239 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/project/AppDependencies.scala
--rw-r--r--   0        0        0      566 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/project/CodeCoverageSettings.scala
--rw-r--r--   0        0        0       28 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/project/build.properties
--rw-r--r--   0        0        0      770 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/project/plugins.sbt
--rw-r--r--   0        0        0      232 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/template/BACKEND.delete
--rw-r--r--   0        0        0      115 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/template/FRONTEND.delete
--rw-r--r--   0        0        0      914 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala
--rw-r--r--   0        0        0     1119 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala
--rw-r--r--   0        0        0      623 2023-03-24 15:57:40.748794 init_service-0.6.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala
--rw-r--r--   0        0        0      902 2023-03-24 15:57:40.748794 init_service-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 init_service-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 16:06:56.962055 init_service-0.7.0/LICENSE
+-rw-r--r--   0        0        0      683 2023-04-13 16:06:56.962055 init_service-0.7.0/init_service/__init__.py
+-rw-r--r--   0        0        0    10586 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/init_service.py
+-rw-r--r--   0        0        0    50425 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/pyratemp.py
+-rw-r--r--   0        0        0      353 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/.gitignore
+-rw-r--r--   0        0        0      299 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/build.sbt
+-rw-r--r--   0        0        0      308 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/project/LibDependencies.scala
+-rw-r--r--   0        0        0       28 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/project/build.properties
+-rw-r--r--   0        0        0      369 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/project/plugins.sbt
+-rw-r--r--   0        0        0       82 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/src/main/scala/uk/gov/hmrc/hello/HelloWorld.scala
+-rw-r--r--   0        0        0      275 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/src/test/scala/uk/gov/hmrc/hello/HelloWorldSpec.scala
+-rw-r--r--   0        0        0      353 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/.gitignore
+-rw-r--r--   0        0        0       41 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/assets/stylesheets/application.scss
+-rw-r--r--   0        0        0      447 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/config/AppConfig.scala
+-rw-r--r--   0        0        0      626 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/config/ErrorHandler.scala
+-rw-r--r--   0        0        0      221 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/config/Module.scala
+-rw-r--r--   0        0        0      620 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/controllers/HelloWorldController.scala
+-rw-r--r--   0        0        0      503 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/controllers/MicroserviceHelloWorldController.scala
+-rw-r--r--   0        0        0      374 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/views/ErrorTemplate.scala.html
+-rw-r--r--   0        0        0      260 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/views/HelloWorldPage.scala.html
+-rw-r--r--   0        0        0      454 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/views/Layout.scala.html
+-rw-r--r--   0        0        0      855 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/build.sbt
+-rw-r--r--   0        0        0      472 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/app.routes
+-rw-r--r--   0        0        0      300 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/application-json-logger.xml
+-rw-r--r--   0        0        0     3070 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/application.conf
+-rw-r--r--   0        0        0     2337 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/logback.xml
+-rw-r--r--   0        0        0       68 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/messages
+-rw-r--r--   0        0        0       69 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/messages.cy
+-rw-r--r--   0        0        0      247 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/prod.routes
+-rw-r--r--   0        0        0     1098 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes
+-rw-r--r--   0        0        0     1024 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala
+-rw-r--r--   0        0        0     1239 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/AppDependencies.scala
+-rw-r--r--   0        0        0      566 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/CodeCoverageSettings.scala
+-rw-r--r--   0        0        0       28 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/build.properties
+-rw-r--r--   0        0        0      770 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/plugins.sbt
+-rw-r--r--   0        0        0      232 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/template/BACKEND.delete
+-rw-r--r--   0        0        0      115 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/template/FRONTEND.delete
+-rw-r--r--   0        0        0      914 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala
+-rw-r--r--   0        0        0     1119 2023-04-13 16:06:56.970055 init_service-0.7.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala
+-rw-r--r--   0        0        0      623 2023-04-13 16:06:56.970055 init_service-0.7.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala
+-rw-r--r--   0        0        0      902 2023-04-13 16:06:56.970055 init_service-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 init_service-0.7.0/PKG-INFO
```

### Comparing `init_service-0.6.0/LICENSE` & `init_service-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/__init__.py` & `init_service-0.7.0/init_service/__init__.py`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/init_service.py` & `init_service-0.7.0/init_service/init_service.py`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/pyratemp.py` & `init_service-0.7.0/init_service/pyratemp.py`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/app/config/ErrorHandler.scala` & `init_service-0.7.0/init_service/templates/service/app/config/ErrorHandler.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/app/controllers/HelloWorldController.scala` & `init_service-0.7.0/init_service/templates/service/app/controllers/HelloWorldController.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/build.sbt` & `init_service-0.7.0/init_service/templates/service/build.sbt`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/conf/application.conf` & `init_service-0.7.0/init_service/templates/service/conf/application.conf`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,14 @@
       protocol = http
       host = localhost
       port = 9250
     }
   }
 }
 
-metrics.enabled = true
-
 play.i18n.langCookieHttpOnly: "true"
 
 # Change this value to true to enable Welsh translations to be loaded from messages.cy, and to display the language toggle
 features.welsh-language-support = false
 
 # Replace play.i18n.langs with the commented out line below when your service has been fully translated into Welsh
 # to enable Welsh translations for all content, including the standard headers and footers.
@@ -85,42 +83,30 @@
 # Controller
 # ~~~~~
 # By default all controllers will have authorisation, logging and
 # auditing (transaction monitoring) enabled.
 # The below controllers are the default exceptions to this rule.
 
 controllers {
-  # 300 is the default, you may need to change this according to your needs
-  confidenceLevel = 300
-
   uk.gov.hmrc.$!APP_PACKAGE_NAME!$.controllers.MicroserviceHelloWorldController = {
     needsAuth = false
     needsLogging = false
     needsAuditing = false
   }
 }
 
-# Metrics plugin settings - graphite reporting is configured on a per env basis
-metrics.enabled = true
-
 # Microservice specific config
 
     <!--(if MONGO)-->
 mongodb {
   uri = "mongodb://localhost:27017/$!APP_NAME!$"
 }
     <!--(end)-->
 
 microservice {
-  metrics {
-    graphite {
-      host = graphite
-    }
-  }
-
   services {
     <!--(if type =="BACKEND")-->
     auth {
       host = localhost
       port = 8500
     }
     <!--(end)-->
```

### Comparing `init_service-0.6.0/init_service/templates/service/conf/logback.xml` & `init_service-0.7.0/init_service/templates/service/conf/logback.xml`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes` & `init_service-0.7.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala` & `init_service-0.7.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/project/AppDependencies.scala` & `init_service-0.7.0/init_service/templates/service/project/AppDependencies.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/project/CodeCoverageSettings.scala` & `init_service-0.7.0/init_service/templates/service/project/CodeCoverageSettings.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/project/plugins.sbt` & `init_service-0.7.0/init_service/templates/service/project/plugins.sbt`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala` & `init_service-0.7.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala` & `init_service-0.7.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala` & `init_service-0.7.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.6.0/pyproject.toml` & `init_service-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "init-service"
-version = "0.6.0"
+version = "0.7.0"
 description = "A templating tool for HMRC MDTP repositories"
 authors = ["Your Name <you@example.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
```

