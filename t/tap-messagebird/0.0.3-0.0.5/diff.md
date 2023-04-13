# Comparing `tmp/tap_messagebird-0.0.3.tar.gz` & `tmp/tap_messagebird-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_messagebird-0.0.3.tar", max compression
+gzip compressed data, was "tap_messagebird-0.0.5.tar", max compression
```

## Comparing `tap_messagebird-0.0.3.tar` & `tap_messagebird-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/LICENSE
--rw-r--r--   0        0        0     3370 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/README.md
--rw-r--r--   0        0        0      983 2023-02-17 15:25:46.886788 tap_messagebird-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      115 2023-02-17 15:25:24.986792 tap_messagebird-0.0.3/tap_messagebird/__init__.py
--rw-r--r--   0        0        0     3247 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/client.py
--rw-r--r--   0        0        0     3044 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/schemas/conversation.json
--rw-r--r--   0        0        0      993 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/schemas/conversation_message.json
--rw-r--r--   0        0        0     4240 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/schemas/message.json
--rw-r--r--   0        0        0     3210 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/streams.py
--rw-r--r--   0        0        0     1579 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/tap.py
--rw-r--r--   0        0        0       38 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/tests/__init__.py
--rw-r--r--   0        0        0      499 2023-02-17 15:14:21.736942 tap_messagebird-0.0.3/tap_messagebird/tests/test_core.py
--rw-r--r--   0        0        0     4496 1970-01-01 00:00:00.000000 tap_messagebird-0.0.3/setup.py
--rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 tap_messagebird-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3370 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/README.md
+-rw-r--r--   0        0        0     1163 2023-04-13 13:13:33.065255 tap_messagebird-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-04-13 13:13:33.069254 tap_messagebird-0.0.5/tap_messagebird/__init__.py
+-rw-r--r--   0        0        0     3857 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/client.py
+-rw-r--r--   0        0        0     3044 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/schemas/conversation.json
+-rw-r--r--   0        0        0      993 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/schemas/conversation_message.json
+-rw-r--r--   0        0        0     4240 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/schemas/message.json
+-rw-r--r--   0        0        0     3621 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/streams.py
+-rw-r--r--   0        0        0     1590 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/tap.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 tap_messagebird-0.0.5/PKG-INFO
```

### Comparing `tap_messagebird-0.0.3/LICENSE` & `tap_messagebird-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.3/README.md` & `tap_messagebird-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.3/tap_messagebird/client.py` & `tap_messagebird-0.0.5/tap_messagebird/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,78 @@
 """REST client handling, including MessagebirdStream base class."""
 
 from __future__ import annotations
 
+from http import HTTPStatus
 from pathlib import Path
-from typing import Any, Dict, Iterable, Optional
+from typing import TYPE_CHECKING, Any, Iterable
 from urllib.parse import parse_qsl, urlparse
 
-import requests
 from singer_sdk.helpers.jsonpath import extract_jsonpath
 from singer_sdk.pagination import BaseHATEOASPaginator, BaseOffsetPaginator
 from singer_sdk.streams import RESTStream
 
+if TYPE_CHECKING:
+    import requests
+
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class MessagebirdHATEOASPaginator(BaseHATEOASPaginator):
-    def get_next_url(self, response):
+    """Messagebird HATEOAS paginator class."""
+
+    def get_next_url(self, response: requests.Response) -> str:
+        """Return the next URL to use for pagination."""
         return response.json()["links"]["next"]
 
 
 class MessagebirdOffsetPaginator(BaseOffsetPaginator):
-    def get_next(self, response) -> int | None:
+    """Messagebird offset-based paginator class."""
+
+    def get_next(self, response: requests.Response) -> int | None:
+        """Return the next offset to use for pagination."""
         response_json = response.json()
         return response_json["offset"] + response_json["limit"]
 
-    def has_more(self, response) -> bool:
+    def has_more(self, response: requests.Response) -> bool:
+        """Return True if there are more pages to paginate, False otherwise."""
         response_json = response.json()
         offset = response_json["offset"]
         count = response_json["count"]
         total_count = response_json["totalCount"]
         return count + offset <= total_count
 
 
 class MessagebirdStream(RESTStream):
     """Messagebird stream class."""
 
     url_base = "https://rest.messagebird.com"
 
     records_jsonpath = "$.items[*]"
-    next_page_token_jsonpath = "$.next_page"  # Or override `get_next_page_token`.
+    next_page_token_jsonpath = "$.next_page"  # noqa: S105
     _LOG_REQUEST_METRIC_URLS: bool = True
 
-    def get_new_paginator(self):
+    def get_new_paginator(self) -> MessagebirdHATEOASPaginator:
+        """Return a new instance of a paginator for this stream."""
         return MessagebirdHATEOASPaginator()
 
     @property
     def http_headers(self) -> dict:
         """Return the http headers needed."""
         headers = {}
         if "user_agent" in self.config:
             headers["User-Agent"] = self.config.get("user_agent")
         headers["Authorization"] = f"AccessKey {self.config['api_key']}"
         return headers
 
     def get_url_params(
-        self, context: Optional[dict], next_page_token: Optional[Any]
-    ) -> Dict[str, Any]:
+        self,
+        context: dict | None,  # noqa: ARG002
+        next_page_token: Any | None,
+    ) -> dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization."""
         params: dict = {}
         if next_page_token:
             return dict(parse_qsl(next_page_token.query))
         if self.replication_key:
             params["sort"] = "asc"
             params["order_by"] = self.replication_key
@@ -78,15 +91,19 @@
             response: A `requests.Response`_ object.
 
         Returns:
             str: The error message
         """
         full_path = urlparse(response.url).path or self.path
         error_content = ""
-        if 400 <= response.status_code < 500:
+        if (
+            HTTPStatus.BAD_REQUEST
+            <= response.status_code
+            < HTTPStatus.INTERNAL_SERVER_ERROR
+        ):
             error_type = "Client"
             error_content = response.json()
         else:
             error_type = "Server"
 
         return (
             f"{response.status_code} {error_type} Error: "
```

### Comparing `tap_messagebird-0.0.3/tap_messagebird/schemas/conversation.json` & `tap_messagebird-0.0.5/tap_messagebird/schemas/conversation.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.3/tap_messagebird/schemas/conversation_message.json` & `tap_messagebird-0.0.5/tap_messagebird/schemas/conversation_message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.3/tap_messagebird/schemas/message.json` & `tap_messagebird-0.0.5/tap_messagebird/schemas/message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.3/tap_messagebird/streams.py` & `tap_messagebird-0.0.5/tap_messagebird/streams.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """Stream type classes for tap-messagebird."""
 
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Any
 
 from tap_messagebird.client import MessagebirdOffsetPaginator, MessagebirdStream
 
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class MessagebirdConversations(MessagebirdStream):
+    """Messagebird Conversations stream class."""
+
     url_base = "https://conversations.messagebird.com/v1"
 
-    def limit(self):
+    def limit(self) -> int:
+        """Return the page size for this stream."""
         return 20
 
-    def get_new_paginator(self):
+    def get_new_paginator(self) -> MessagebirdOffsetPaginator:
+        """Return a new instance of a paginator for this stream."""
         return MessagebirdOffsetPaginator(
-            start_value=0, page_size=self.limit()
-        )  # type: ignore
+            start_value=0,
+            page_size=self.limit(),
+        )
 
     def get_url_params(
-        self, context: Optional[dict], next_page_token: Optional[Any]
-    ) -> Dict[str, Any]:
+        self,
+        context: dict | None,  # noqa: ARG002
+        next_page_token: Any | None,
+    ) -> dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization.
-        Overrode as we have a different paginator for this api
+
+        Overrode as we have a different paginator for this api.
         """
         params = {}
         if next_page_token:
             params["offset"] = next_page_token
         params["status"] = "all"
         params["limit"] = self.limit()
         return params
@@ -39,38 +49,51 @@
     name = "conversation"
     path = "/conversations"
     primary_keys = ["id"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     schema_filepath = SCHEMAS_DIR / "conversation.json"
 
-    def get_child_context(self, record: dict, context: Optional[dict]) -> dict:
+    def get_child_context(
+        self,
+        record: dict,
+        context: dict | None,  # noqa: ARG002
+    ) -> dict | None:
         """Return a context dictionary for child streams."""
+        if record["status"] == "archived":
+            return None
+
         return {
             "_sdc_conversations_id": record["id"],
         }
 
 
 class ConversationMessagesStream(MessagebirdConversations):
-    """Conversation Messages stream. Messages stream doesn't pull all messages as we were expecting"""
+    """Conversation Messages stream.
+
+    Messages stream doesn't pull all messages.
+    """
 
     name = "conversation_message"
     path = "/conversations/{_sdc_conversations_id}/messages"
     primary_keys = ["id"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     schema_filepath = SCHEMAS_DIR / "conversation_message.json"
     parent_stream_type = ConversationsStream
 
     def get_url_params(
-        self, context: Optional[dict], next_page_token: Optional[Any]
-    ) -> Dict[str, Any]:
+        self,
+        context: dict | None,
+        next_page_token: Any | None,
+    ) -> dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization."""
         params = super().get_url_params(
-            context=context, next_page_token=next_page_token
+            context=context,
+            next_page_token=next_page_token,
         )
         if params.get("from") is None:
             params["from"] = self.config["start_date"]
         return params
 
 
 class MessagesStream(MessagebirdStream):
@@ -80,16 +103,19 @@
     path = "/messages"
     primary_keys = ["id"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     schema_filepath = SCHEMAS_DIR / "message.json"
 
     def get_url_params(
-        self, context: Optional[dict], next_page_token: Optional[Any]
-    ) -> Dict[str, Any]:
+        self,
+        context: dict | None,
+        next_page_token: Any | None,
+    ) -> dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization."""
         params = super().get_url_params(
-            context=context, next_page_token=next_page_token
+            context=context,
+            next_page_token=next_page_token,
         )
         if params.get("from") is None:
             params["from"] = self.config["start_date"]
         return params
```

### Comparing `tap_messagebird-0.0.3/tap_messagebird/tap.py` & `tap_messagebird-0.0.5/tap_messagebird/tap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Messagebird tap class."""
 
-from typing import List
+from __future__ import annotations
 
 import pendulum
 from singer_sdk import Stream, Tap
 from singer_sdk import typing as th  # JSON schema typing helpers
 
 from tap_messagebird.streams import (
     ConversationMessagesStream,
@@ -43,14 +43,14 @@
             description=(
                 "When to pull records starting at what date. "
                 "ISO8601 format of date, defaults to 3 years ago."
             ),
         ),
     ).to_dict()
 
-    def discover_streams(self) -> List[Stream]:
+    def discover_streams(self) -> list[Stream]:
         """Return a list of discovered streams."""
         return [stream_class(tap=self) for stream_class in STREAM_TYPES]
 
 
 if __name__ == "__main__":
     TapMessagebird.cli()
```

### Comparing `tap_messagebird-0.0.3/setup.py` & `tap_messagebird-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,134 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tap-messagebird
+Version: 0.0.5
+Summary: `tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK.
+License: Apache 2.0
+Keywords: ELT,Messagebird
+Author: Meltano Team
+Author-email: hello@meltano.com
+Requires-Python: >=3.7.1,<3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: s3
+Requires-Dist: fs-s3fs (>=1.1.1,<2.0.0) ; extra == "s3"
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: singer-sdk (>=0.24.0,<0.25.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['tap_messagebird', 'tap_messagebird.tests']
+# `tap-messagebird`
 
-package_data = \
-{'': ['*'], 'tap_messagebird': ['schemas/*']}
+Messagebird tap class.
 
-install_requires = \
-['requests>=2.25.1,<3.0.0', 'singer-sdk>=0.17.0,<0.18.0']
-
-extras_require = \
-{'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
-
-entry_points = \
-{'console_scripts': ['tap-messagebird = '
-                     'tap_messagebird.tap:TapMessagebird.cli']}
-
-setup_kwargs = {
-    'name': 'tap-messagebird',
-    'version': '0.0.3',
-    'description': '`tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK.',
-    'long_description': "# `tap-messagebird`\n\nMessagebird tap class.\n\nBuilt with the [Meltano Singer SDK](https://sdk.meltano.com).\n\n## Capabilities\n\n* `catalog`\n* `discover`\n* `about`\n* `stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting             | Required | Default | Description |\n|:--------------------|:--------:|:-------:|:------------|\n| api_key             | True     | None    | The token to authenticate against the API service. Test keys are not supported for Conversations see https://support.messagebird.com/hc/en-us/articles/360000670709-What-is-the-difference-between-a-live-key-and-a-test-key- |\n| start_date          | False    | now -3 years | When to pull records starting at what date. ISO8601 format of date, defaults to 3 years ago. |\n| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |\n| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth| False    | None    | The max depth to flatten schemas. |\n\nA full list of supported settings and capabilities is available by running: `tap-messagebird --about`\n\n\n## Installation\n\nInstall from PyPi:\n\n```bash\npipx install tap-messagebird\n```\n\n\n### Configure using environment variables\n\nThis Singer tap will automatically import any environment variables within the working directory's\n`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching\nenvironment variable is set either in the terminal context or in the `.env` file.\n\n### Source Authentication and Authorization\n\nNote that Conversations do not work without a Production API key\n\n## Usage\n\nYou can easily run `tap-messagebird` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-messagebird --version\ntap-messagebird --help\ntap-messagebird --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\nFollow these instructions to contribute to this project.\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tap_messagebird/tests` subfolder and\n  then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-messagebird` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-messagebird --help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nNext, install Meltano (if you haven't already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-messagebird\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-messagebird --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-messagebird target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n",
-    'author': 'Meltano',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
-}
+Built with the [Meltano Singer SDK](https://sdk.meltano.com).
 
+## Capabilities
+
+* `catalog`
+* `discover`
+* `about`
+* `stream-maps`
+* `schema-flattening`
+
+## Settings
+
+| Setting             | Required | Default | Description |
+|:--------------------|:--------:|:-------:|:------------|
+| api_key             | True     | None    | The token to authenticate against the API service. Test keys are not supported for Conversations see https://support.messagebird.com/hc/en-us/articles/360000670709-What-is-the-difference-between-a-live-key-and-a-test-key- |
+| start_date          | False    | now -3 years | When to pull records starting at what date. ISO8601 format of date, defaults to 3 years ago. |
+| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
+| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
+| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth| False    | None    | The max depth to flatten schemas. |
+
+A full list of supported settings and capabilities is available by running: `tap-messagebird --about`
+
+
+## Installation
+
+Install from PyPi:
+
+```bash
+pipx install tap-messagebird
+```
+
+
+### Configure using environment variables
+
+This Singer tap will automatically import any environment variables within the working directory's
+`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
+environment variable is set either in the terminal context or in the `.env` file.
+
+### Source Authentication and Authorization
+
+Note that Conversations do not work without a Production API key
+
+## Usage
+
+You can easily run `tap-messagebird` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Tap Directly
+
+```bash
+tap-messagebird --version
+tap-messagebird --help
+tap-messagebird --config CONFIG --discover > ./catalog.json
+```
+
+## Developer Resources
+
+Follow these instructions to contribute to this project.
+
+### Initialize your Development Environment
+
+```bash
+pipx install poetry
+poetry install
+```
+
+### Create and Run Tests
+
+Create tests within the `tap_messagebird/tests` subfolder and
+  then run:
+
+```bash
+poetry run pytest
+```
+
+You can also test the `tap-messagebird` CLI interface directly using `poetry run`:
+
+```bash
+poetry run tap-messagebird --help
+```
+
+### Testing with [Meltano](https://www.meltano.com)
+
+_**Note:** This tap will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Next, install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+cd tap-messagebird
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke tap-messagebird --version
+# OR run a test `elt` pipeline:
+meltano elt tap-messagebird target-jsonl
+```
+
+### SDK Dev Guide
+
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
+develop your own taps and targets.
 
-setup(**setup_kwargs)
```

