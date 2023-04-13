# Comparing `tmp/twc_cli-1.2.0.tar.gz` & `tmp/twc_cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twc_cli-1.2.0.tar", max compression
+gzip compressed data, was "twc_cli-1.3.0.tar", max compression
```

## Comparing `twc_cli-1.2.0.tar` & `twc_cli-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     5109 2023-04-03 11:51:47.632398 twc_cli-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.968435 twc_cli-1.2.0/COPYING
--rw-r--r--   0        0        0      847 2023-02-27 17:17:26.238623 twc_cli-1.2.0/README.md
--rw-r--r--   0        0        0     1047 2023-04-03 11:52:13.159177 twc_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-02-27 15:10:37.741551 twc_cli-1.2.0/twc/__init__.py
--rw-r--r--   0        0        0     2508 2023-03-31 23:29:33.360857 twc_cli-1.2.0/twc/__main__.py
--rw-r--r--   0        0        0      420 2023-04-03 11:52:22.222550 twc_cli-1.2.0/twc/__version__.py
--rw-r--r--   0        0        0       59 2023-02-02 19:40:27.815419 twc_cli-1.2.0/twc/api/__init__.py
--rw-r--r--   0        0        0    34039 2023-03-31 16:59:38.168750 twc_cli-1.2.0/twc/api/client.py
--rw-r--r--   0        0        0      851 2023-03-15 17:12:36.163338 twc_cli-1.2.0/twc/api/exceptions.py
--rw-r--r--   0        0        0     1185 2023-03-31 23:29:24.914163 twc_cli-1.2.0/twc/click_ext.py
--rw-r--r--   0        0        0     7363 2023-03-31 23:34:25.871810 twc_cli-1.2.0/twc/commands/__init__.py
--rw-r--r--   0        0        0     5368 2023-02-20 20:02:22.604110 twc_cli-1.2.0/twc/commands/account.py
--rw-r--r--   0        0        0     1491 2023-03-31 23:35:59.085447 twc_cli-1.2.0/twc/commands/config.py
--rw-r--r--   0        0        0    17457 2023-03-31 22:55:25.407517 twc_cli-1.2.0/twc/commands/database.py
--rw-r--r--   0        0        0     9510 2023-03-27 17:32:43.874755 twc_cli-1.2.0/twc/commands/image.py
--rw-r--r--   0        0        0    11669 2023-03-31 19:42:48.822800 twc_cli-1.2.0/twc/commands/project.py
--rw-r--r--   0        0        0    71079 2023-04-03 11:55:13.059962 twc_cli-1.2.0/twc/commands/server.py
--rw-r--r--   0        0        0     8218 2023-02-20 16:39:53.540123 twc_cli-1.2.0/twc/commands/ssh_key.py
--rw-r--r--   0        0        0     5874 2023-03-13 22:59:16.243616 twc_cli-1.2.0/twc/fmt.py
--rw-r--r--   0        0        0      616 2023-03-31 16:59:37.665415 twc_cli-1.2.0/twc/utils.py
--rw-r--r--   0        0        0      637 2023-04-01 00:37:28.507268 twc_cli-1.2.0/twc/vars.py
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 twc_cli-1.2.0/setup.py
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 twc_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7000 2023-04-13 11:28:03.272172 twc_cli-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-1.3.0/COPYING
+-rw-r--r--   0        0        0      847 2023-02-27 17:17:26.000000 twc_cli-1.3.0/README.md
+-rw-r--r--   0        0        0     1078 2023-04-13 11:28:39.190610 twc_cli-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-02-27 15:10:37.000000 twc_cli-1.3.0/twc/__init__.py
+-rw-r--r--   0        0        0     2620 2023-04-11 18:52:08.673104 twc_cli-1.3.0/twc/__main__.py
+-rw-r--r--   0        0        0      420 2023-04-13 11:28:47.584499 twc_cli-1.3.0/twc/__version__.py
+-rw-r--r--   0        0        0       59 2023-02-02 19:40:27.000000 twc_cli-1.3.0/twc/api/__init__.py
+-rw-r--r--   0        0        0    40159 2023-04-12 18:59:45.905765 twc_cli-1.3.0/twc/api/client.py
+-rw-r--r--   0        0        0      851 2023-03-15 17:12:36.000000 twc_cli-1.3.0/twc/api/exceptions.py
+-rw-r--r--   0        0        0     1185 2023-03-31 23:29:24.000000 twc_cli-1.3.0/twc/click_ext.py
+-rw-r--r--   0        0        0     7517 2023-04-12 23:56:34.801064 twc_cli-1.3.0/twc/commands/__init__.py
+-rw-r--r--   0        0        0     5368 2023-02-20 20:02:22.000000 twc_cli-1.3.0/twc/commands/account.py
+-rw-r--r--   0        0        0     5108 2023-04-12 23:56:55.730939 twc_cli-1.3.0/twc/commands/config.py
+-rw-r--r--   0        0        0    17457 2023-03-31 22:55:25.000000 twc_cli-1.3.0/twc/commands/database.py
+-rw-r--r--   0        0        0     9510 2023-03-27 17:32:43.000000 twc_cli-1.3.0/twc/commands/image.py
+-rw-r--r--   0        0        0    11669 2023-03-31 19:42:48.000000 twc_cli-1.3.0/twc/commands/project.py
+-rw-r--r--   0        0        0    71079 2023-04-03 11:55:13.000000 twc_cli-1.3.0/twc/commands/server.py
+-rw-r--r--   0        0        0     8218 2023-02-20 16:39:53.000000 twc_cli-1.3.0/twc/commands/ssh_key.py
+-rw-r--r--   0        0        0    23777 2023-04-12 23:44:59.955500 twc_cli-1.3.0/twc/commands/storage.py
+-rw-r--r--   0        0        0     6283 2023-04-12 23:58:02.933876 twc_cli-1.3.0/twc/fmt.py
+-rw-r--r--   0        0        0      616 2023-03-31 16:59:37.000000 twc_cli-1.3.0/twc/utils.py
+-rw-r--r--   0        0        0      634 2023-04-12 20:15:47.148238 twc_cli-1.3.0/twc/vars.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 twc_cli-1.3.0/PKG-INFO
```

### Comparing `twc_cli-1.2.0/CHANGELOG.md` & `twc_cli-1.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Релизы Timeweb Cloud CLI
 
 В этом файле описаны все значимые изменения в Timeweb Cloud CLI. В выпусках мы придерживается правил [семантического версионирования](https://semver.org/lang/ru/).
 
+# Версия 1.3.0 (2023.04.13)
+
+Добавлено:
+
+- Добавлена команда `twc storage` (алиас `twc s3`) для управления бакетами в объектном хранилище Timeweb Cloud. Доступны базовые операции с бакетами. Также реализованы субкоманды для работы с доменами и пользователями хранилища. Обратите внимание, что в twc не планируется добавлять реализацию S3-клиента, пользуйтесь любым совместимым клиентом, например, [s3cmd](https://s3tools.org/s3cmd) или [rclone](https://rclone.org/), команда `twc s3 genconfig` позволит сгенерировать конфигурационный файл для этих утилит (см. документацию).
+- Добавлены субкоманды для `twc config`. Теперь можно: сделать дамп настроек CLI (`twc config dump`), изменять настройки без ручного редактирования файла (`twc config set`), получить путь до файла (`twc config file`), открыть файл в редакторе по умолчанию (`twc config edit`).
+
+Изменено:
+
+- Изменены тексты ошибок при работе с конфигурационным файлом, теперь они более наглядные и явно указывают на проблему.
+- Изменено поведение команды `twc config`. Теперь если уже иммется конфигурационный файл команда предложит добавить новый профиль или отредактировать существующий.
+
 # Версия 1.2.0 (2023.04.03)
 
 Добавлено:
 
 - Добавлена команда `twc database` (алиас `twc db`). Теперь можно:
     - создавать и удалять управляемые базы данных;
     - изменять параметры базы данных;
```

### Comparing `twc_cli-1.2.0/COPYING` & `twc_cli-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/README.md` & `twc_cli-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/pyproject.toml` & `twc_cli-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twc-cli"
-version = "1.2.0"
+version = "1.3.0"
 description = "Timeweb Cloud Command Line Interface."
 authors = ["ge <dev@timeweb.cloud>"]
 homepage = "https://github.com/timeweb-cloud/twc"
 repository = "https://github.com/timeweb-cloud/twc"
 license="MIT"
 readme = "README.md"
 include = ["CHANGELOG.md", "COPYING"]
@@ -16,14 +16,15 @@
 python = "^3.7.9"
 requests = "^2.28.1"
 pygments = "^2.14.0"
 click = "^8.1.3"
 click-aliases = "^1.0.1"
 toml = "^0.10.2"
 pyyaml = "^6.0"
+click-default-group = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pylint = "^2.17.0"
 
 [tool.poetry.scripts]
 twc = 'twc.__main__:cli'
```

### Comparing `twc_cli-1.2.0/twc/__main__.py` & `twc_cli-1.3.0/twc/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .commands.account import account
 from .commands.config import config
 from .commands.server import server
 from .commands.ssh_key import ssh_key
 from .commands.image import image
 from .commands.project import project
 from .commands.database import database
+from .commands.storage import storage
 
 
 class AliasedCmdGroup(click.Group):
     """Add aliases for Click commands. Needs a global variable
     ALIASES with dict. Exmaple:
 
     @click.group(cls=AliasedCmdGroup)
@@ -40,25 +41,25 @@
             cmd = self.get_command(ctx, subcommand)
             if cmd is None:
                 continue
             if cmd.hidden:
                 continue
             commands.append((subcommand, cmd))
 
-        if len(commands):
+        if commands:
             limit = formatter.width - 6 - max(len(cmd[0]) for cmd in commands)
             rows = []
             for subcommand, cmd in commands:
                 # Get command alias
                 alias = ""
                 for a in list(ALIASES.keys()):
                     if ALIASES[a].name == cmd.name:
                         alias = f" ({a})"
-                help = cmd.get_short_help_str(limit)
-                rows.append((subcommand + alias, help))
+                help_text = cmd.get_short_help_str(limit)
+                rows.append((subcommand + alias, help_text))
             if rows:
                 with formatter.section(_("Commands")):
                     formatter.write_dl(rows)
 
 
 @click.group(cls=AliasedCmdGroup)
 @options(GLOBAL_OPTIONS[:2])
@@ -69,14 +70,15 @@
 cli.add_command(account)
 cli.add_command(config)
 cli.add_command(server)
 cli.add_command(ssh_key)
 cli.add_command(image)
 cli.add_command(project)
 cli.add_command(database)
+cli.add_command(storage)
 
 
 # -- Aliases list for root level commands. --
 # If there are several aliases, only the last one will
 # be printed in the help text.
 ALIASES = {
     "servers": server,
@@ -85,8 +87,10 @@
     "k": ssh_key,
     "images": image,
     "i": image,
     "projects": project,
     "p": project,
     "dbs": database,
     "db": database,
+    "storages": storage,
+    "s3": storage,
 }
```

### Comparing `twc_cli-1.2.0/twc/api/client.py` & `twc_cli-1.3.0/twc/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,22 +28,23 @@
         try:
             is_json = response.headers.get("content-type").startswith(
                 "application/json"
             )
         except AttributeError:
             is_json = False
 
-        if status_code in [200, 201, 400, 403, 404, 409, 429, 500]:
+        # Remove 201 to avoid API bug (201 with no body)
+        if status_code in [200, 400, 403, 404, 409, 429, 500]:
             if is_json:
                 return response  # Success
             raise NonJSONResponseError(
                 f"Code: {status_code}, Response body: {response.text}"
             )
 
-        if status_code == 204:
+        if status_code in [201, 204]:
             return response  # Success
 
         if status_code == 401:
             raise UnauthorizedError
 
         raise UnexpectedResponseError(status_code)
 
@@ -981,7 +982,188 @@
         url = f"{self.api_url}/dbs/{db_id}/backups/{backup_id}"
         return requests.delete(url, headers=self.headers, timeout=self.timeout)
 
     def restore_database_backup(self, db_id: int, backup_id: int):
         """Restore database backup."""
         url = f"{self.api_url}/dbs/{db_id}/backups/{backup_id}"
         return requests.put(url, headers=self.headers, timeout=self.timeout)
+
+    # -----------------------------------------------------------------------
+    # Object Storage
+
+    def get_storage_presets(self):
+        """Get storage presets list."""
+        url = f"{self.api_url}/presets/storages"
+        return requests.get(url, headers=self.headers, timeout=self.timeout)
+
+    def get_buckets(self):
+        """Get buckets list."""
+        url = f"{self.api_url}/storages/buckets"
+        return requests.get(url, headers=self.headers, timeout=self.timeout)
+
+    def create_bucket(
+        self, name: str = None, preset_id: int = None, is_public: bool = False
+    ):
+        """Create storage bucket."""
+        url = f"{self.api_url}/storages/buckets"
+        self.headers.update({"Content-Type": "application/json"})
+        if is_public:
+            bucket_type = "public"
+        else:
+            bucket_type = "private"
+        payload = {
+            "name": name,
+            "type": bucket_type,
+            "preset_id": preset_id,
+        }
+        return requests.post(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
+
+    def delete_bucket(
+        self, bucket_id: int, delete_hash: str = None, code: int = None
+    ):
+        """Delete storage bucket."""
+        url = f"{self.api_url}/storages/buckets/{bucket_id}"
+        params = {}
+        if delete_hash:
+            params["hash"] = delete_hash
+        if code:
+            params["code"] = code
+        return requests.delete(
+            url, headers=self.headers, timeout=self.timeout, params=params
+        )
+
+    def update_bucket(
+        self, bucket_id: int, preset_id: int = None, is_public: bool = None
+    ):
+        """Update storage bucket."""
+        url = f"{self.api_url}/storages/buckets/{bucket_id}"
+        self.headers.update({"Content-Type": "application/json"})
+        payload = {}
+        if is_public is None:
+            pass
+        elif is_public is False:
+            payload["bucket_type"] = "private"
+        elif is_public is True:
+            payload["bucket_type"] = "public"
+        if preset_id:
+            payload["preset_id"] = preset_id
+        return requests.patch(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
+
+    def get_storage_users(self):
+        """Get storage users list."""
+        url = f"{self.api_url}/storages/users"
+        return requests.get(url, headers=self.headers, timeout=self.timeout)
+
+    def update_storage_user_secret(
+        self, user_id: int = None, secret_key: str = None
+    ):
+        """Update storage user secret key."""
+        url = f"{self.api_url}/storages/users/{user_id}"
+        self.headers.update({"Content-Type": "application/json"})
+        payload = {"secret_key": secret_key}
+        return requests.patch(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
+
+    def get_storage_transfer_status(self, bucket_id: int = None):
+        """Get storage transfer status."""
+        url = f"{self.api_url}/storages/buckets/{bucket_id}/transfer-status"
+        return requests.get(url, headers=self.headers, timeout=self.timeout)
+
+    def start_storage_transfer(
+        self,
+        src_bucket: str = None,
+        dst_bucket: str = None,
+        access_key: str = None,
+        secret_key: str = None,
+        location: str = None,
+        endpoint: str = None,
+        force_path_style: bool = False,
+    ):
+        """Start file transfer from any S3-compatible storage to Timeweb Cloud
+        Object Storage.
+        """
+        url = f"{self.api_url}/storages/transfer"
+        self.headers.update({"Content-Type": "application/json"})
+        payload = {
+            "access_key": access_key,
+            "secret_key": secret_key,
+            "location": location,
+            "is_force_path_style": force_path_style,
+            "endpoint": endpoint,
+            "bucket_name": src_bucket,
+            "new_bucket_name": dst_bucket,
+        }
+        return requests.post(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
+
+    def get_bucket_subdomains(self, bucket_id: int = None):
+        """Get bucket subdomains list."""
+        url = f"{self.api_url}/storages/buckets/{bucket_id}/subdomains"
+        return requests.get(url, headers=self.headers, timeout=self.timeout)
+
+    def add_bucket_subdomains(
+        self,
+        bucket_id: int = None,
+        subdomains: list = None,
+    ):
+        """Add subdomains to bucket."""
+        url = f"{self.api_url}/storages/buckets/{bucket_id}/subdomains"
+        self.headers.update({"Content-Type": "application/json"})
+        payload = {
+            "subdomains": subdomains,
+        }
+        return requests.post(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
+
+    def delete_bucket_subdomains(
+        self,
+        bucket_id: int = None,
+        subdomains: list = None,
+    ):
+        """Delete bucket subdomains."""
+        url = f"{self.api_url}/storages/buckets/{bucket_id}/subdomains"
+        self.headers.update({"Content-Type": "application/json"})
+        payload = {
+            "subdomains": subdomains,
+        }
+        return requests.delete(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
+
+    def gen_cert_for_bucket_subdomain(self, subdomain: str = None):
+        """Generate TLS certificate for subdomain attached to bucket."""
+        url = f"{self.api_url}/storages/certificates/generate"
+        self.headers.update({"Content-Type": "application/json"})
+        payload = {
+            "subdomain": subdomain,
+        }
+        return requests.post(
+            url,
+            headers=self.headers,
+            timeout=self.timeout,
+            data=json.dumps(payload),
+        )
```

### Comparing `twc_cli-1.2.0/twc/api/exceptions.py` & `twc_cli-1.3.0/twc/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/click_ext.py` & `twc_cli-1.3.0/twc/click_ext.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/commands/__init__.py` & `twc_cli-1.3.0/twc/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,22 @@
 
 
 def load_config(filepath: str = get_default_config_file()):
     """Load configuration from TOML config file."""
     try:
         with open(filepath, "r", encoding="utf-8") as file:
             return toml.load(file)
-    except (OSError, FileNotFoundError) as error:
-        sys.exit(f"Error: {filepath}: {error}: Try run 'twc config'")
+    except FileNotFoundError:
+        sys.exit(
+            f"Configuration file {filepath} not found. Try run 'twc config'"
+        )
+    except OSError as error:
+        sys.exit(f"Error: Cannot read configuration file {filepath}: {error}")
     except toml.TomlDecodeError as error:
-        sys.exit(f"Error: {filepath}: {error}")
+        sys.exit(f"Error: Check your TOML syntax in file {filepath}: {error}")
 
 
 def set_value_from_config(ctx, param, value):
     """Callback for Click to load option values from configuration file."""
     if value is None:
         if not os.path.exists(ctx.params["config"]):
             return None
```

### Comparing `twc_cli-1.2.0/twc/commands/account.py` & `twc_cli-1.3.0/twc/commands/account.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/commands/database.py` & `twc_cli-1.3.0/twc/commands/database.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/commands/image.py` & `twc_cli-1.3.0/twc/commands/image.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/commands/project.py` & `twc_cli-1.3.0/twc/commands/project.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/commands/server.py` & `twc_cli-1.3.0/twc/commands/server.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/commands/ssh_key.py` & `twc_cli-1.3.0/twc/commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/fmt.py` & `twc_cli-1.3.0/twc/fmt.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import json
 
 import click
 import yaml
 
 from pygments import highlight
-from pygments.lexers import JsonLexer, YamlLexer
+from pygments.lexers import JsonLexer, YamlLexer, IniLexer, TOMLLexer
 from pygments.formatters import TerminalFormatter
 
 
 class Table:
     """Print table. Example::
 
     >>> t = Table()
@@ -184,7 +184,20 @@
                     lambda x: str(query_dict(x, key.split("."))) == val,
                     objects,
                 )
             )
         except (KeyError, ValueError):
             return []
     return objects
+
+
+def print_colored(data: str, lang: str = None):
+    """Print colorized text to terminal."""
+    lexers = {
+        "json": JsonLexer(),
+        "yaml": YamlLexer(),
+        "toml": TOMLLexer(),
+        "ini": IniLexer(),
+    }
+    if lang not in lexers:
+        raise ValueError(f"Unsupported lexer: '{lang}'")
+    click.echo(highlight(data, lexers[lang], TerminalFormatter()).strip())
```

### Comparing `twc_cli-1.2.0/twc/utils.py` & `twc_cli-1.3.0/twc/utils.py`

 * *Files identical despite different names*

### Comparing `twc_cli-1.2.0/twc/vars.py` & `twc_cli-1.3.0/twc/vars.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module defines variables that depend on Timeweb Cloud products.
 They are subject to change at any time as cloud computing capabilities
 expand or other infrastructure or product changes occur.
 """
 
 # Service URLs
 TWC_CP_URL = "https://timeweb.cloud/my"
-TWC_S3_URL = "https://s3.timeweb.com"
+TWC_S3_ENDPOINT = "s3.timeweb.com"
 
 # CLI configuration file sceleton.
 DEFAULT_CONFIG = {"default": {"token": ""}}
 
 # Default Configurator ID for Cloud Servers.
 DEFAULT_CONFIGURATOR_ID = 11
```

### Comparing `twc_cli-1.2.0/PKG-INFO` & `twc_cli-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: twc-cli
-Version: 1.2.0
+Version: 1.3.0
 Summary: Timeweb Cloud Command Line Interface.
 Home-page: https://github.com/timeweb-cloud/twc
 License: MIT
 Author: ge
 Author-email: dev@timeweb.cloud
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
+Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/timeweb-cloud/twc
 Description-Content-Type: text/markdown
```

