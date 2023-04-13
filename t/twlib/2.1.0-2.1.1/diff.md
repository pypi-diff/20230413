# Comparing `tmp/twlib-2.1.0.tar.gz` & `tmp/twlib-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twlib-2.1.0.tar", last modified: Thu Dec 22 14:15:01 2022, max compression
+gzip compressed data, was "twlib-2.1.1.tar", last modified: Thu Apr 13 15:07:54 2023, max compression
```

## Comparing `twlib-2.1.0.tar` & `twlib-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-22 14:15:01.052420 twlib-2.1.0/
--rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-16 17:27:49.000000 twlib-2.1.0/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)     3356 2022-12-22 14:15:01.052530 twlib-2.1.0/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     1323 2022-12-22 11:29:47.000000 twlib-2.1.0/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      100 2022-12-16 17:27:49.000000 twlib-2.1.0/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1959 2022-12-22 14:15:01.053200 twlib-2.1.0/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:27:49.000000 twlib-2.1.0/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-22 14:15:01.028729 twlib-2.1.0/src/
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-22 14:15:01.047412 twlib-2.1.0/src/twlib/
--rw-r--r--   0 Q187392    (501) staff       (20)       89 2022-12-16 17:27:49.000000 twlib-2.1.0/src/twlib/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)       46 2022-12-16 17:27:49.000000 twlib-2.1.0/src/twlib/__main__.py
--rw-r--r--   0 Q187392    (501) staff       (20)      856 2022-12-22 06:58:30.000000 twlib-2.1.0/src/twlib/environment.py
--rw-r--r--   0 Q187392    (501) staff       (20)     1401 2022-12-22 11:24:08.000000 twlib-2.1.0/src/twlib/git_open.py
--rw-r--r--   0 Q187392    (501) staff       (20)     1226 2022-12-22 13:28:35.000000 twlib-2.1.0/src/twlib/lib.py
--rw-r--r--   0 Q187392    (501) staff       (20)     6190 2022-12-22 14:13:18.000000 twlib-2.1.0/src/twlib/main.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-22 14:15:01.051983 twlib-2.1.0/src/twlib.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     3356 2022-12-22 14:15:01.000000 twlib-2.1.0/src/twlib.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      377 2022-12-22 14:15:01.000000 twlib-2.1.0/src/twlib.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2022-12-22 14:15:01.000000 twlib-2.1.0/src/twlib.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       71 2022-12-22 14:15:01.000000 twlib-2.1.0/src/twlib.egg-info/entry_points.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       55 2022-12-22 14:15:01.000000 twlib-2.1.0/src/twlib.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        6 2022-12-22 14:15:01.000000 twlib-2.1.0/src/twlib.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 15:07:54.329824 twlib-2.1.1/
+-rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-16 17:27:49.000000 twlib-2.1.1/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)     3356 2023-04-13 15:07:54.329932 twlib-2.1.1/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     1323 2022-12-22 11:29:47.000000 twlib-2.1.1/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      100 2022-12-16 17:27:49.000000 twlib-2.1.1/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1966 2023-04-13 15:07:54.330537 twlib-2.1.1/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:27:49.000000 twlib-2.1.1/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 15:07:54.310974 twlib-2.1.1/src/
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 15:07:54.317615 twlib-2.1.1/src/twlib/
+-rw-r--r--   0 Q187392    (501) staff       (20)       89 2022-12-16 17:27:49.000000 twlib-2.1.1/src/twlib/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)       46 2022-12-16 17:27:49.000000 twlib-2.1.1/src/twlib/__main__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)      856 2022-12-22 06:58:30.000000 twlib-2.1.1/src/twlib/environment.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1401 2022-12-22 11:24:08.000000 twlib-2.1.1/src/twlib/git_open.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1226 2022-12-22 13:28:35.000000 twlib-2.1.1/src/twlib/lib.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     9472 2023-04-13 15:07:47.000000 twlib-2.1.1/src/twlib/main.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 15:07:54.321380 twlib-2.1.1/src/twlib.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3356 2023-04-13 15:07:54.000000 twlib-2.1.1/src/twlib.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      485 2023-04-13 15:07:54.000000 twlib-2.1.1/src/twlib.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 15:07:54.000000 twlib-2.1.1/src/twlib.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-04-13 15:07:54.000000 twlib-2.1.1/src/twlib.egg-info/entry_points.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       61 2023-04-13 15:07:54.000000 twlib-2.1.1/src/twlib.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        6 2023-04-13 15:07:54.000000 twlib-2.1.1/src/twlib.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 15:07:54.329375 twlib-2.1.1/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)      115 2022-12-16 17:27:49.000000 twlib-2.1.1/tests/test_environment.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1233 2022-12-16 17:27:49.000000 twlib-2.1.1/tests/test_git_open.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     2314 2022-12-22 14:13:18.000000 twlib-2.1.1/tests/test_lib.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     5999 2023-04-13 15:07:47.000000 twlib-2.1.1/tests/test_main.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1721 2022-12-16 17:27:49.000000 twlib-2.1.1/tests/test_pattern.py
```

### Comparing `twlib-2.1.0/LICENSE` & `twlib-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twlib-2.1.0/PKG-INFO` & `twlib-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twlib
-Version: 2.1.0
+Version: 2.1.1
 Summary: "twlib"
 Home-page: https://github.com/sysid/twlib
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `twlib-2.1.0/README.md` & `twlib-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `twlib-2.1.0/setup.cfg` & `twlib-2.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twlib
-version = 2.1.0
+version = 2.1.1
 description = "twlib"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/twlib
 classifiers = 
@@ -22,14 +22,15 @@
 install_requires = 
 	typer
 	pydantic
 	python-dateutil
 	pytz
 	pillow
 	pillow-heif
+	boto3
 include_package_data = True
 python_requires = >=3.11
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `twlib-2.1.0/src/twlib/environment.py` & `twlib-2.1.1/src/twlib/environment.py`

 * *Files identical despite different names*

### Comparing `twlib-2.1.0/src/twlib/git_open.py` & `twlib-2.1.1/src/twlib/git_open.py`

 * *Files identical despite different names*

### Comparing `twlib-2.1.0/src/twlib/lib.py` & `twlib-2.1.1/src/twlib/lib.py`

 * *Files identical despite different names*

### Comparing `twlib-2.1.0/src/twlib/main.py` & `twlib-2.1.1/src/twlib/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import datetime
 import logging
 import os
 import shutil
 from pathlib import Path
-from typing import Iterable
 
+import boto3
 import typer
 from dateutil.parser import parse
 from PIL import Image
 from pillow_heif import register_heif_opener
 
 from twlib.lib import filter_path
 
 _log = logging.getLogger(__name__)
 
+__version__ = "2.1.1"
+
 register_heif_opener()  # register PILLOW plugin
 
 app = typer.Typer(name="twlib")
 
 
 @app.command()
 def snake_say(
@@ -127,14 +129,95 @@
     ).name  # Gotcha: source_path.name is not the same as target_path.name
     rel_path = os.path.relpath(target_path, source_path)
     typer.echo(Path(rel_path) / name)
     return Path(rel_path) / name
 
 
 @app.command()
+def sqs_purge(
+    queue_url: str = typer.Option(None, "-q", "--queue-url", help="Queue URL"),
+) -> None:
+    session = boto3.Session()
+    sqs = session.client("sqs")
+
+    if queue_url is None:
+        queue_url = sqs_choice(sqs)
+    if not queue_url.startswith("https://"):
+        typer.secho(f"Invalid queue URL: {queue_url}", fg=typer.colors.RED, bold=True)
+        raise typer.Exit(1)
+
+    # Purge the SQS queue
+    response = sqs.purge_queue(QueueUrl=queue_url)
+
+    if response["ResponseMetadata"]["HTTPStatusCode"] == 200:
+        typer.echo(f"The queue {queue_url} has been purged.")
+    else:
+        typer.echo("Failed to purge the queue.")
+
+
+@app.command()
+def sqs(
+    n_messages: int = typer.Option(3, "-n", "--n-messages", help="Number of messages"),
+    visibility_timeout: int = typer.Option(
+        0, "-t", "--visibility-timeout", help="Visibility timeout"
+    ),
+) -> None:
+    session = boto3.Session()
+    sqs = session.client("sqs")
+    queue_url = sqs_choice(sqs)
+
+    # Get the approximate number of messages in the selected queue
+    response = sqs.get_queue_attributes(
+        QueueUrl=queue_url, AttributeNames=["ApproximateNumberOfMessages"]
+    )
+    message_count = response["Attributes"]["ApproximateNumberOfMessages"]
+
+    typer.echo(f"Approximate number of messages in the selected queue: {message_count}")
+
+    if int(message_count) == 0:
+        raise typer.Exit()
+
+    response = sqs.receive_message(
+        QueueUrl=queue_url,
+        AttributeNames=["All"],
+        MaxNumberOfMessages=n_messages,
+        VisibilityTimeout=visibility_timeout,
+    )
+
+    messages = response.get("Messages", [])
+
+    if messages:
+        typer.echo(f"Last {len(messages)} messages in the queue:")
+        for i, message in enumerate(messages, 1):
+            typer.echo(f"Message {i}:")
+            typer.echo(f"Message ID: {message['MessageId']}")
+            typer.echo(f"Message Body: {message['Body']}")
+            typer.echo(f"Receipt Handle: {message['ReceiptHandle']}")
+            typer.echo()
+    else:
+        typer.echo("No messages found in the queue.")
+
+
+def sqs_choice(sqs):
+    typer.echo("Select a queue:")
+    response = sqs.list_queues()
+    queues = response.get("QueueUrls", [])
+    for i, queue_url in enumerate(queues):
+        typer.echo(f"{i + 1}: {queue_url}")
+    queue_index = typer.prompt("Queue index", type=int)
+    if 0 < queue_index <= len(queues):
+        queue_url = queues[queue_index - 1]
+        typer.echo(f"Selected queue: {queue_url}")
+    else:
+        typer.secho(f"Invalid queue index: {queue_index}", fg=typer.colors.RED)
+        raise typer.Exit()
+    return queue_url
+
+
+@app.command()
 def revert_lks(
     dir_: Path = typer.Argument(
         ..., help="Directory containing the lks files", exists=True
     ),
     excludes: list[str] = typer.Option(
         [".venv", ".git"], "-e", "--exclude", help="Exclude dirs/files"
     ),
@@ -180,24 +263,39 @@
             else:
                 shutil.copytree(target, f, symlinks=True)
                 _log.debug(f"Copied {target} to {f}")
 
     typer.secho(f"Reverted {len(symlks)} symlinks", fg=typer.colors.GREEN, bold=False)
 
 
-@app.callback()
+@app.callback(invoke_without_command=True)
 def main(
+    ctx: typer.Context,
     verbose: bool = typer.Option(False, "-v", "--verbose", help="verbosity"),
+    version: bool = typer.Option(False, "-V", "--version", help="show version"),
 ):
     log_fmt = r"%(asctime)-15s %(levelname)-7s %(message)s"
     if verbose:
         logging.basicConfig(
             format=log_fmt, level=logging.DEBUG, datefmt="%m-%d %H:%M:%S"
         )
     else:
         logging.basicConfig(
             format=log_fmt, level=logging.INFO, datefmt="%m-%d %H:%M:%S"
         )
+    logging.getLogger("botocore").setLevel(logging.INFO)
+    logging.getLogger("boto3").setLevel(logging.INFO)
+    logging.getLogger("urllib3").setLevel(logging.INFO)
+
+    if ctx.invoked_subcommand is None and version:
+        ctx.invoke(print_version)
+    if ctx.invoked_subcommand is None and not version:
+        typer.echo(ctx.get_help())
+
+
+@app.command("version", help="Show version", hidden=True)
+def print_version() -> None:
+    typer.echo(f"Confguard version: {__version__}")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `twlib-2.1.0/src/twlib.egg-info/PKG-INFO` & `twlib-2.1.1/src/twlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twlib
-Version: 2.1.0
+Version: 2.1.1
 Summary: "twlib"
 Home-page: https://github.com/sysid/twlib
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

