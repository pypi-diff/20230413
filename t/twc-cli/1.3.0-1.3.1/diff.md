# Comparing `tmp/twc_cli-1.3.0.tar.gz` & `tmp/twc_cli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twc_cli-1.3.0.tar", max compression
+gzip compressed data, was "twc_cli-1.3.1.tar", max compression
```

## Comparing `twc_cli-1.3.0.tar` & `twc_cli-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7000 2023-04-13 11:28:03.272172 twc_cli-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-1.3.0/COPYING
--rw-r--r--   0        0        0      847 2023-02-27 17:17:26.000000 twc_cli-1.3.0/README.md
--rw-r--r--   0        0        0     1078 2023-04-13 11:28:39.190610 twc_cli-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-02-27 15:10:37.000000 twc_cli-1.3.0/twc/__init__.py
--rw-r--r--   0        0        0     2620 2023-04-11 18:52:08.673104 twc_cli-1.3.0/twc/__main__.py
--rw-r--r--   0        0        0      420 2023-04-13 11:28:47.584499 twc_cli-1.3.0/twc/__version__.py
--rw-r--r--   0        0        0       59 2023-02-02 19:40:27.000000 twc_cli-1.3.0/twc/api/__init__.py
--rw-r--r--   0        0        0    40159 2023-04-12 18:59:45.905765 twc_cli-1.3.0/twc/api/client.py
--rw-r--r--   0        0        0      851 2023-03-15 17:12:36.000000 twc_cli-1.3.0/twc/api/exceptions.py
--rw-r--r--   0        0        0     1185 2023-03-31 23:29:24.000000 twc_cli-1.3.0/twc/click_ext.py
--rw-r--r--   0        0        0     7517 2023-04-12 23:56:34.801064 twc_cli-1.3.0/twc/commands/__init__.py
--rw-r--r--   0        0        0     5368 2023-02-20 20:02:22.000000 twc_cli-1.3.0/twc/commands/account.py
--rw-r--r--   0        0        0     5108 2023-04-12 23:56:55.730939 twc_cli-1.3.0/twc/commands/config.py
--rw-r--r--   0        0        0    17457 2023-03-31 22:55:25.000000 twc_cli-1.3.0/twc/commands/database.py
--rw-r--r--   0        0        0     9510 2023-03-27 17:32:43.000000 twc_cli-1.3.0/twc/commands/image.py
--rw-r--r--   0        0        0    11669 2023-03-31 19:42:48.000000 twc_cli-1.3.0/twc/commands/project.py
--rw-r--r--   0        0        0    71079 2023-04-03 11:55:13.000000 twc_cli-1.3.0/twc/commands/server.py
--rw-r--r--   0        0        0     8218 2023-02-20 16:39:53.000000 twc_cli-1.3.0/twc/commands/ssh_key.py
--rw-r--r--   0        0        0    23777 2023-04-12 23:44:59.955500 twc_cli-1.3.0/twc/commands/storage.py
--rw-r--r--   0        0        0     6283 2023-04-12 23:58:02.933876 twc_cli-1.3.0/twc/fmt.py
--rw-r--r--   0        0        0      616 2023-03-31 16:59:37.000000 twc_cli-1.3.0/twc/utils.py
--rw-r--r--   0        0        0      634 2023-04-12 20:15:47.148238 twc_cli-1.3.0/twc/vars.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 twc_cli-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7474 2023-04-13 18:24:27.742949 twc_cli-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-1.3.1/COPYING
+-rw-r--r--   0        0        0      847 2023-02-27 17:17:26.000000 twc_cli-1.3.1/README.md
+-rw-r--r--   0        0        0     1078 2023-04-13 18:09:55.234206 twc_cli-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-02-27 15:10:37.000000 twc_cli-1.3.1/twc/__init__.py
+-rw-r--r--   0        0        0     2620 2023-04-11 18:52:08.673104 twc_cli-1.3.1/twc/__main__.py
+-rw-r--r--   0        0        0      420 2023-04-13 18:10:03.704217 twc_cli-1.3.1/twc/__version__.py
+-rw-r--r--   0        0        0       59 2023-02-02 19:40:27.000000 twc_cli-1.3.1/twc/api/__init__.py
+-rw-r--r--   0        0        0    40159 2023-04-12 18:59:45.905765 twc_cli-1.3.1/twc/api/client.py
+-rw-r--r--   0        0        0      851 2023-03-15 17:12:36.000000 twc_cli-1.3.1/twc/api/exceptions.py
+-rw-r--r--   0        0        0     1185 2023-03-31 23:29:24.000000 twc_cli-1.3.1/twc/click_ext.py
+-rw-r--r--   0        0        0     7517 2023-04-12 23:56:34.801064 twc_cli-1.3.1/twc/commands/__init__.py
+-rw-r--r--   0        0        0     5368 2023-02-20 20:02:22.000000 twc_cli-1.3.1/twc/commands/account.py
+-rw-r--r--   0        0        0     5478 2023-04-13 16:44:35.143437 twc_cli-1.3.1/twc/commands/config.py
+-rw-r--r--   0        0        0    17457 2023-03-31 22:55:25.000000 twc_cli-1.3.1/twc/commands/database.py
+-rw-r--r--   0        0        0     9510 2023-03-27 17:32:43.000000 twc_cli-1.3.1/twc/commands/image.py
+-rw-r--r--   0        0        0    11669 2023-03-31 19:42:48.000000 twc_cli-1.3.1/twc/commands/project.py
+-rw-r--r--   0        0        0    71079 2023-04-03 11:55:13.000000 twc_cli-1.3.1/twc/commands/server.py
+-rw-r--r--   0        0        0     8218 2023-02-20 16:39:53.000000 twc_cli-1.3.1/twc/commands/ssh_key.py
+-rw-r--r--   0        0        0    23854 2023-04-13 18:20:28.396938 twc_cli-1.3.1/twc/commands/storage.py
+-rw-r--r--   0        0        0     6283 2023-04-12 23:58:02.933876 twc_cli-1.3.1/twc/fmt.py
+-rw-r--r--   0        0        0      616 2023-03-31 16:59:37.000000 twc_cli-1.3.1/twc/utils.py
+-rw-r--r--   0        0        0      634 2023-04-12 20:15:47.148238 twc_cli-1.3.1/twc/vars.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 twc_cli-1.3.1/PKG-INFO
```

### Comparing `twc_cli-1.3.0/CHANGELOG.md` & `twc_cli-1.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # Релизы Timeweb Cloud CLI
 
 В этом файле описаны все значимые изменения в Timeweb Cloud CLI. В выпусках мы придерживается правил [семантического версионирования](https://semver.org/lang/ru/).
 
+# Версия 1.3.1 (2023.04.13)
+
+Изменено:
+
+- В команде `twc s3 mb` опция `--preset-id` теперь необязательная. Будет выбран минимальный пресет.
+
+Исправлено:
+
+- Исправлена ошибка при попытке создать дополнительный профиль через `twc config`.
+
 # Версия 1.3.0 (2023.04.13)
 
 Добавлено:
 
-- Добавлена команда `twc storage` (алиас `twc s3`) для управления бакетами в объектном хранилище Timeweb Cloud. Доступны базовые операции с бакетами. Также реализованы субкоманды для работы с доменами и пользователями хранилища. Обратите внимание, что в twc не планируется добавлять реализацию S3-клиента, пользуйтесь любым совместимым клиентом, например, [s3cmd](https://s3tools.org/s3cmd) или [rclone](https://rclone.org/), команда `twc s3 genconfig` позволит сгенерировать конфигурационный файл для этих утилит (см. документацию).
+- Добавлена команда `twc storage` (алиас `twc s3`) для управления бакетами в объектном хранилище Timeweb Cloud. Доступны базовые операции с бакетами. Также реализованы субкоманды для работы с доменами и пользователями хранилища. Обратите внимание, что в twc не планируется добавлять реализацию S3-клиента, пользуйтесь любым совместимым клиентом, например, [s3cmd](https://s3tools.org/s3cmd) или [rclone](https://rclone.org/), команда `twc s3 genconfig` позволит сгенерировать конфигурационный файл для этих утилит (см. [документацию](docs/ru/README.md#получение-конфигурации-для-s3-клиентов)).
 - Добавлены субкоманды для `twc config`. Теперь можно: сделать дамп настроек CLI (`twc config dump`), изменять настройки без ручного редактирования файла (`twc config set`), получить путь до файла (`twc config file`), открыть файл в редакторе по умолчанию (`twc config edit`).
 
 Изменено:
 
 - Изменены тексты ошибок при работе с конфигурационным файлом, теперь они более наглядные и явно указывают на проблему.
 - Изменено поведение команды `twc config`. Теперь если уже иммется конфигурационный файл команда предложит добавить новый профиль или отредактировать существующий.
```

### Comparing `twc_cli-1.3.0/COPYING` & `twc_cli-1.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/README.md` & `twc_cli-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/pyproject.toml` & `twc_cli-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twc-cli"
-version = "1.3.0"
+version = "1.3.1"
 description = "Timeweb Cloud Command Line Interface."
 authors = ["ge <dev@timeweb.cloud>"]
 homepage = "https://github.com/timeweb-cloud/twc"
 repository = "https://github.com/timeweb-cloud/twc"
 license="MIT"
 readme = "README.md"
 include = ["CHANGELOG.md", "COPYING"]
```

### Comparing `twc_cli-1.3.0/twc/__main__.py` & `twc_cli-1.3.1/twc/__main__.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/api/client.py` & `twc_cli-1.3.1/twc/api/client.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/api/exceptions.py` & `twc_cli-1.3.1/twc/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/click_ext.py` & `twc_cli-1.3.1/twc/click_ext.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/__init__.py` & `twc_cli-1.3.1/twc/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/account.py` & `twc_cli-1.3.1/twc/commands/account.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/config.py` & `twc_cli-1.3.1/twc/commands/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,27 @@
         if click.confirm(
             "You already have TWC CLI configured, continue?",
             default=False,
         ):
             current_config = load_config()
             profile = click.prompt("Enter profile name", default="default")
             token = click.prompt(f"Enter API token for '{profile}'")
-            current_config[profile] = utils.merge_dicts(
-                current_config[profile],
-                {"token": token},
-            )
+            try:
+                # Edit existing profile
+                current_config[profile] = utils.merge_dicts(
+                    current_config[profile],
+                    {"token": token},
+                )
+            except KeyError:
+                # Add new profile
+                current_config[profile] = {}  # init new config section
+                current_config[profile] = utils.merge_dicts(
+                    current_config[profile],
+                    {"token": token},
+                )
             write_to_file(current_config, filepath)
         else:
             sys.exit("Aborted!")
 
     click.echo("Create new configuration file. Enter your API token.")
     while True:
         token = input("Token: ")
```

### Comparing `twc_cli-1.3.0/twc/commands/database.py` & `twc_cli-1.3.1/twc/commands/database.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/image.py` & `twc_cli-1.3.1/twc/commands/image.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/project.py` & `twc_cli-1.3.1/twc/commands/project.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/server.py` & `twc_cli-1.3.1/twc/commands/server.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/ssh_key.py` & `twc_cli-1.3.1/twc/commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/commands/storage.py` & `twc_cli-1.3.1/twc/commands/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 # $ twc storage mb                                              #
 # ------------------------------------------------------------- #
 
 
 @storage.command("mb", help="Make bucket.")
 @options(GLOBAL_OPTIONS)
 @options(OUTPUT_FORMAT_OPTION)
-@click.option("--preset-id", type=int, required=True, help="Bucket preset ID.")
+@click.option("--preset-id", type=int, help="Bucket preset ID.")
 @click.option(
     "--project-id",
     type=int,
     default=None,
     envvar="TWC_PROJECT",
     callback=set_value_from_config,
     help="Add bucket to specific project.",
@@ -253,14 +253,19 @@
     project_id,
     bucket_type,
     bucket_name,
 ):
     # pylint: disable=too-many-locals
 
     client = create_client(config, profile)
+
+    if not preset_id:
+        # Select minimal preset
+        preset_id = 389  # 10G disk
+
     is_public = False
     if bucket_type == "public":
         is_public = True
 
     if project_id:
         debug("Check project_id")
         projects = _project_list(client).json()["projects"]
```

### Comparing `twc_cli-1.3.0/twc/fmt.py` & `twc_cli-1.3.1/twc/fmt.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/utils.py` & `twc_cli-1.3.1/twc/utils.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/twc/vars.py` & `twc_cli-1.3.1/twc/vars.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.0/PKG-INFO` & `twc_cli-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twc-cli
-Version: 1.3.0
+Version: 1.3.1
 Summary: Timeweb Cloud Command Line Interface.
 Home-page: https://github.com/timeweb-cloud/twc
 License: MIT
 Author: ge
 Author-email: dev@timeweb.cloud
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

