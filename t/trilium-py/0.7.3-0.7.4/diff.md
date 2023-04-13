# Comparing `tmp/trilium_py-0.7.3-py3-none-any.whl.zip` & `tmp/trilium_py-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27165 bytes, number of entries: 12
--rw-r--r--  2.0 unx      141 b- defN 22-Dec-13 06:44 trilium_py/__init__.py
--rw-r--r--  2.0 unx    27921 b- defN 23-Apr-04 07:03 trilium_py/client.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-13 06:44 trilium_py/utils/__init__.py
--rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:03 trilium_py/utils/markdown_math.py
--rw-r--r--  2.0 unx      675 b- defN 22-Dec-13 06:44 trilium_py/utils/param_util.py
--rw-r--r--  2.0 unx      208 b- defN 22-Dec-13 06:44 trilium_py/utils/time_util.py
--rw-r--r--  2.0 unx      470 b- defN 22-Dec-13 08:23 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 23-Apr-04 07:09 trilium_py-0.7.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    10195 b- defN 23-Apr-04 07:09 trilium_py-0.7.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 07:09 trilium_py-0.7.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-04 07:09 trilium_py-0.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-Apr-04 07:09 trilium_py-0.7.3.dist-info/RECORD
-12 files, 84543 bytes uncompressed, 25495 bytes compressed:  69.8%
+Zip file size: 27205 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      141 b- defN 23-Apr-04 07:07 trilium_py/__init__.py
+-rw-r--r--  2.0 unx    27921 b- defN 23-Apr-04 07:07 trilium_py/client.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 07:07 trilium_py/utils/__init__.py
+-rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:07 trilium_py/utils/markdown_math.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Apr-04 07:07 trilium_py/utils/param_util.py
+-rw-r--r--  2.0 unx      208 b- defN 23-Apr-04 07:07 trilium_py/utils/time_util.py
+-rw-r--r--  2.0 unx      470 b- defN 23-Apr-04 07:07 trilium_py/utils/url_util.py
+-rwxrwx---  2.0 unx    35184 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    10488 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/RECORD
+12 files, 84836 bytes uncompressed, 25535 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.7.3.dist-info/LICENSE.txt
+Filename: trilium_py-0.7.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.7.3.dist-info/METADATA
+Filename: trilium_py-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.7.3.dist-info/WHEEL
+Filename: trilium_py-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.7.3.dist-info/top_level.txt
+Filename: trilium_py-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.7.3.dist-info/RECORD
+Filename: trilium_py-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `trilium_py-0.7.3.dist-info/LICENSE.txt` & `trilium_py-0.7.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.7.3.dist-info/METADATA` & `trilium_py-0.7.4.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -23,18 +23,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: BeautifulSoup4
 Requires-Dist: requests
-Requires-Dist: python-magic
 Requires-Dist: markdown2[all]
 Requires-Dist: natsort
 Requires-Dist: python-magic-bin ; platform_system == "Windows"
+Requires-Dist: python-magic ; sys_platform == "darwin"
+Requires-Dist: python-magic ; sys_platform == "linux"
 
 # 🐍 trilium-py
 
 Python client for ETAPI of Trilium Note.
 
 [![Downloads](https://static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)](https://pypi.org/project/trilium-py)
@@ -44,73 +45,73 @@
 
 <a href="https://github.com/Nriver"><img align="center" src="https://moe-counter--nriver1.repl.co/get/@Nriver_trilium-py"></a><br>
 
 # 🦮 Table of Contents
 
 <!--ts-->
 
-* [trilium-py](#-trilium-py)
-* [Table of Contents](#-table-of-contents)
-* [Installation](#-installation)
-* [(Basic) Usage](#-basic-usage)
-    * [Initialization](#-initialization)
-    * [Application Information](#-application-information)
-    * [Search note](#-search-note)
-    * [Create Note](#-create-note)
-        * [Create Image note](#️-create-image-note)
-    * [Get note](#-get-note)
-    * [Update note](#-update-note)
-    * [Delete note](#️-delete-note)
-    * [Day note](#-day-note)
-    * [Export note](#-export-note)
-* [(Advanced Usage) TODO List](#advanced-usage--todo-list)
-    * [Add TODO item](#add-todo-item)
-    * [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
-    * [Update a TODO item](#update-a-todo-item)
-    * [Delete a TDOO item](#delete-a-tdoo-item)
-    * [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
-* [(Advanced Usage) Upload Markdown files](#advanced-usage--upload-markdown-files)
-    * [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
-    * [Bulk upload Markdown files in a folder!](#bulk-upload-markdown-files-in-a-folder)
-        * [Import from VNote](#import-from-vnote)
-        * [Import from Logseq](#import-from-logseq)
-        * [Import from Obsidian](#import-from-obsidian)
-        * [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
-        * [Import from other markdown software](#import-from-other-markdown-software)
-* [Develop](#️-develop)
-* [Original OpenAPI Documentation](#-original-openapi-documentation)
+- [🐍 trilium-py](#-trilium-py)
+- [🦮 Table of Contents](#-table-of-contents)
+- [🔧 Installation](#-installation)
+- [📖 (Basic) Usage](#-basic-usage)
+  - [🚀 Initialization](#-initialization)
+  - [📊 Application Information](#-application-information)
+  - [🔍 Search note](#-search-note)
+  - [🏭 Create Note](#-create-note)
+    - [🖼️ Create Image note](#️-create-image-note)
+  - [👀 Get note](#-get-note)
+  - [🔄 Update note](#-update-note)
+  - [🗑️ Delete note](#️-delete-note)
+  - [📅 Day note](#-day-note)
+  - [📤 Export note](#-export-note)
+- [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
+  - [Add TODO item](#add-todo-item)
+  - [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
+  - [Update a TODO item](#update-a-todo-item)
+  - [Delete a TDOO item](#delete-a-tdoo-item)
+  - [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
+- [(Advanced Usage) 🚚 Upload Markdown files](#advanced-usage--upload-markdown-files)
+  - [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
+  - [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
+    - [Import from VNote](#import-from-vnote)
+    - [Import from Logseq](#import-from-logseq)
+    - [Import from Obsidian](#import-from-obsidian)
+    - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
+    - [Import from other markdown software](#import-from-other-markdown-software)
+- [🛠️ Develop](#️-develop)
+- [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
 
 <!--te-->
 
 # 🔧 Installation
 
-```
+```bash
 python3 -m pip install trilium-py --user
 ```
 
 # 📖 (Basic) Usage
 
 These are basic function that Trilium's ETAPI provides. Down below are some simple example code to use this package.
 
 ## 🚀 Initialization
 
 If you have a ETAPI token, change the `server_url` and `token` to yours.
 
-```
+```python
 from trilium_py.client import ETAPI
 
 server_url = 'http://localhost:8080'
 token = 'YOUR_TOKEN'
 ea = ETAPI(server_url, token)
 ```
 
 If you haven't created ETAPI token, you can create one with your password. Please note, you can only see this token
 once, please save it if you want to reuse the token.
 
-```
+```python
 from trilium_py.client import ETAPI
 
 server_url = 'http://localhost:8080'
 password = '1234'
 ea = ETAPI(server_url)
 token = ea.login(password)
 print(token)
@@ -118,125 +119,125 @@
 
 After initialization, you can use Trilium ETAPI with python now. The following are some examples.
 
 ## 📊 Application Information
 
 To start with, you can get the application information like this.
 
-```
+```python
 print(ea.app_info())
 ```
 
 It should give you the version of your server application and some extra information.
 
 ## 🔍 Search note
 
 Search note with keyword.
 
-```
+```python
 res = ea.search_note(
     search="python",
 )
 
 for x in res['results']:
     print(x['noteId'], x['title'])
 ```
 
 ## 🏭 Create Note
 
 You can create a simple note like this.
 
-```
+```python
 res = ea.create_note(
     parentNoteId="root",
     title="Simple note 1",
     type="text",
     content="Simple note example",
     noteId="note1"
 )
 ```
 
 The `noteId` is not mandatory, if not provided, Trilium will generate a random one. You can retrieve it in the return.
 
-```
+```python
 noteId = res['note']['noteId']
 ```
 
 ### 🖼️ Create Image note
 
 Image note is a special kind of note. You can create an image note with minimal information like this. The `image_file`
 refers to the path of image.
 
-```
+```python
 res = ea.create_image_note(
     parentNoteId="root",
     title="Image note 1",
     image_file="shield.png",
 )
 ```
 
 ## 👀 Get note
 
 To retrieve the note's content.
 
-```
+```python
 ea.get_note_content("note1")
 ```
 
 You can get a note metadata by its id.
 
-```
+```python
 ea.get_note(note_id)
 ```
 
 ## 🔄 Update note
 
 Update note content
 
-```
+```python
 ea.update_note_content("note1", "updated by python")
 ```
 
 Modify note title
 
-```
+```python
 ea.patch_note(
     noteId="note1",
     title="Python client moded",
 )
 ```
 
 ## 🗑️ Delete note
 
 Simply delete a note by id.
 
-```
+```python
 ea.delete_note("note1")
 ```
 
 ## 📅 Day note
 
 You can get the content of a certain date with `get_day_note`. The date string should be in format of "%Y-%m-%d", e.g. "
 2022-02-25".
 
-```
+```python
 es.get_day_note("2022-02-25")
 ```
 
 Then set/update a day note with `set_day_note`. The content should be a (html) string.
 
-```
+```python
 self.set_day_note(date, new_content)
 ```
 
 ## 📤 Export note
 
 Export note comes in two formats `html` or `markdown`/`md`.
 
-```
+```python
 res = ea.export_note(
     noteId='sK5fn4T6yZRI',
     format='md',
     savePath='/home/nate/data/1/test.zip',
 )
 ```
 
@@ -244,85 +245,85 @@
 
 With the power of Python, I have expanded the basic usage of ETAPI. You can do something with todo list now.
 
 ## Add TODO item
 
 You can use `add_todo` to add a TODO item, param is the TODO description
 
-```
+```python
 ea.add_todo("买暖宝宝")
 ```
 
 ## Check/Uncheck a TODO item
 
 param is the index of the TODO item
 
-```
+```python
 ea.todo_check(0)
 ea.todo_uncheck(1)
 ```
 
 ## Update a TODO item
 
 Use `update_todo` to update a TODO item description at certain index.
 
-```
+```python
 ea.update_todo(0, "去码头整点薯条")
 ```
 
 ## Delete a TDOO item
 
 Remove a TODO item by its index.
 
-```
+```python
 ea.delete_todo(1)
 ```
 
 ## Move yesterday's unfinished todo to today
 
 As the title suggests, you can move yesterday's unfinished things to today. Unfinished todos will be deleted from
 yesterday's note.
 
-```
+```python
 ea.move_yesterday_unfinished_todo_to_today()
 ```
 
 # (Advanced Usage) 🚚 Upload Markdown files
 
 ## Upload single Markdown file with images
 
 You can import Markdown file with images into Trilium now! Trilium-py will help you to upload the images and fix the
 links for you!
 
-```
+```python
 res = ea.upload_md_file(
     parentNoteId="root",
     file="./md-demo/manjaro 修改caps lock.md",
 )
 ```
 
-## Bulk upload Markdown files in a folder!
+## Bulk upload Markdown files in a folder
 
 You can upload a folder with lots of Markdown files to Trilium and preserve the folder structure!
 
 ### Import from VNote
 
 Say, upload all the notes from [VNote](https://github.com/vnotex/vnote), simply do this:
 
-```
+```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="~/data/vnotebook/",
     ignoreFolder=['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'],
 )
 ```
 
 ### Import from Logseq
 
-```
+```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/logseq_data/",
     ignoreFolder=['assets', 'logseq'],
 )
 ```
 
@@ -330,57 +331,57 @@
 
 Obsidian has a very unique linking system for files. You should use [obsidian-export
 ](https://github.com/zoni/obsidian-export) to convert a Obsidian vault to regular Markdown files. Then you should be
 able to import the note into Trilium with trilium-py.
 
 Convert it first.
 
-```
+```bash
 obsidian-export /path/to/your/vault /out
 ```
 
 Then import just like a normal markdown, trilium-py will handle the images for you.
 
-```
+```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="E:/data/out",
 )
 ```
 
 ### Import from Youdao Note/有道云笔记
 
-Youdao does not provide an export feature anymore. Luckily, you can use https://github.com/DeppWang/youdaonote-pull to
+Youdao does not provide an export feature anymore. Luckily, you can use <https://github.com/DeppWang/youdaonote-pull> to
 download your notes and convert them into markdown files. After that, trilium-py should be able to help you import them.
 
-```
+```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/gitRepo/youdaonote-pull/out/",
 )
 ```
 
 ### Import from other markdown software
 
 In general, markdown files have variety of standards. You can always try import them with
 
-```
+```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/your_markdown_files/",
 )
 ```
 
 If there is any problem, please feel free to create an [issue](https://github.com/Nriver/trilium-py/issues/new).
 
 # 🛠️ Develop
 
 Install with pip egg link to make package change without reinstall.
 
-```
+```python
 python -m pip install --user -e .
 ```
 
 # 🔗 Original OpenAPI Documentation
 
 The original OpenAPI document is [here](https://github.com/zadam/trilium/blob/master/src/etapi/etapi.openapi.yaml). You
 can open it with [swagger editor](https://editor.swagger.io/).
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.7.3 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.7.4 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -11,119 +11,124 @@
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: BeautifulSoup4 Requires-Dist: requests
-Requires-Dist: python-magic Requires-Dist: markdown2[all] Requires-Dist:
-natsort Requires-Dist: python-magic-bin ; platform_system == "Windows" # ð
-trilium-py Python client for ETAPI of Trilium Note. [![Downloads](https://
-static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py) [!
+Requires-Dist: markdown2[all] Requires-Dist: natsort Requires-Dist: python-
+magic-bin ; platform_system == "Windows" Requires-Dist: python-magic ;
+sys_platform == "darwin" Requires-Dist: python-magic ; sys_platform == "linux"
+# ð trilium-py Python client for ETAPI of Trilium Note. [![Downloads](https:
+//static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py) [!
 [Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)]
 (https://pypi.org/project/trilium-py) [![Supported Versions](https://
 img.shields.io/pypi/v/trilium-py?color=%2334D058&label=pypi%20package)](https:/
 /pypi.org/project/trilium-py) [![PyPI license](https://img.shields.io/pypi/l/
 trilium-py.svg)](https://pypi.python.org/pypi/trilium-py/) [![Maintenance]
 (https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
 Naereen/StrapDown.js/graphs/commit-activity) [https://moe-counter--
 nriver1.repl.co/get/@Nriver_trilium-py]
-# ð¦® Table of Contents  * [trilium-py](#-trilium-py) * [Table of Contents](#-
-table-of-contents) * [Installation](#-installation) * [(Basic) Usage](#-basic-
-usage) * [Initialization](#-initialization) * [Application Information](#-
-application-information) * [Search note](#-search-note) * [Create Note](#-
-create-note) * [Create Image note](#ï¸-create-image-note) * [Get note](#-get-
-note) * [Update note](#-update-note) * [Delete note](#ï¸-delete-note) * [Day
-note](#-day-note) * [Export note](#-export-note) * [(Advanced Usage) TODO List]
-(#advanced-usage--todo-list) * [Add TODO item](#add-todo-item) * [Check/Uncheck
-a TODO item](#checkuncheck-a-todo-item) * [Update a TODO item](#update-a-todo-
-item) * [Delete a TDOO item](#delete-a-tdoo-item) * [Move yesterday's
-unfinished todo to today](#move-yesterdays-unfinished-todo-to-today) * [
-(Advanced Usage) Upload Markdown files](#advanced-usage--upload-markdown-files)
-* [Upload single Markdown file with images](#upload-single-markdown-file-with-
-images) * [Bulk upload Markdown files in a folder!](#bulk-upload-markdown-
-files-in-a-folder) * [Import from VNote](#import-from-vnote) * [Import from
-Logseq](#import-from-logseq) * [Import from Obsidian](#import-from-obsidian) *
-[Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
-noteæéäºç¬è®°) * [Import from other markdown software](#import-from-
-other-markdown-software) * [Develop](#ï¸-develop) * [Original OpenAPI
-Documentation](#-original-openapi-documentation)  # ð§ Installation ```
-python3 -m pip install trilium-py --user ``` # ð (Basic) Usage These are
-basic function that Trilium's ETAPI provides. Down below are some simple
+# ð¦® Table of Contents  - [ð trilium-py](#-trilium-py) - [ð¦® Table of
+Contents](#-table-of-contents) - [ð§ Installation](#-installation) - [ð
+(Basic) Usage](#-basic-usage) - [ð Initialization](#-initialization) - [ð
+Application Information](#-application-information) - [ð Search note](#-
+search-note) - [ð­ Create Note](#-create-note) - [ð¼ï¸ Create Image note]
+(#ï¸-create-image-note) - [ð Get note](#-get-note) - [ð Update note](#-
+update-note) - [ðï¸ Delete note](#ï¸-delete-note) - [ð Day note](#-day-
+note) - [ð¤ Export note](#-export-note) - [(Advanced Usage) â TODO List]
+(#advanced-usage--todo-list) - [Add TODO item](#add-todo-item) - [Check/Uncheck
+a TODO item](#checkuncheck-a-todo-item) - [Update a TODO item](#update-a-todo-
+item) - [Delete a TDOO item](#delete-a-tdoo-item) - [Move yesterday's
+unfinished todo to today](#move-yesterdays-unfinished-todo-to-today) - [
+(Advanced Usage) ð Upload Markdown files](#advanced-usage--upload-markdown-
+files) - [Upload single Markdown file with images](#upload-single-markdown-
+file-with-images) - [Bulk upload Markdown files in a folder](#bulk-upload-
+markdown-files-in-a-folder) - [Import from VNote](#import-from-vnote) - [Import
+from Logseq](#import-from-logseq) - [Import from Obsidian](#import-from-
+obsidian) - [Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
+noteæéäºç¬è®°) - [Import from other markdown software](#import-from-
+other-markdown-software) - [ð ï¸ Develop](#ï¸-develop) - [ð Original
+OpenAPI Documentation](#-original-openapi-documentation)  # ð§ Installation
+```bash python3 -m pip install trilium-py --user ``` # ð (Basic) Usage These
+are basic function that Trilium's ETAPI provides. Down below are some simple
 example code to use this package. ## ð Initialization If you have a ETAPI
-token, change the `server_url` and `token` to yours. ``` from trilium_py.client
-import ETAPI server_url = 'http://localhost:8080' token = 'YOUR_TOKEN' ea =
-ETAPI(server_url, token) ``` If you haven't created ETAPI token, you can create
-one with your password. Please note, you can only see this token once, please
-save it if you want to reuse the token. ``` from trilium_py.client import ETAPI
-server_url = 'http://localhost:8080' password = '1234' ea = ETAPI(server_url)
-token = ea.login(password) print(token) ``` After initialization, you can use
-Trilium ETAPI with python now. The following are some examples. ## ð
-Application Information To start with, you can get the application information
-like this. ``` print(ea.app_info()) ``` It should give you the version of your
-server application and some extra information. ## ð Search note Search note
-with keyword. ``` res = ea.search_note( search="python", ) for x in res
-['results']: print(x['noteId'], x['title']) ``` ## ð­ Create Note You can
-create a simple note like this. ``` res = ea.create_note( parentNoteId="root",
-title="Simple note 1", type="text", content="Simple note example",
-noteId="note1" ) ``` The `noteId` is not mandatory, if not provided, Trilium
-will generate a random one. You can retrieve it in the return. ``` noteId = res
-['note']['noteId'] ``` ### ð¼ï¸ Create Image note Image note is a special
-kind of note. You can create an image note with minimal information like this.
-The `image_file` refers to the path of image. ``` res = ea.create_image_note
-( parentNoteId="root", title="Image note 1", image_file="shield.png", ) ``` ##
-ð Get note To retrieve the note's content. ``` ea.get_note_content("note1")
-``` You can get a note metadata by its id. ``` ea.get_note(note_id) ``` ## ð
-Update note Update note content ``` ea.update_note_content("note1", "updated by
-python") ``` Modify note title ``` ea.patch_note( noteId="note1", title="Python
-client moded", ) ``` ## ðï¸ Delete note Simply delete a note by id. ```
-ea.delete_note("note1") ``` ## ð Day note You can get the content of a
-certain date with `get_day_note`. The date string should be in format of "%Y-
-%m-%d", e.g. " 2022-02-25". ``` es.get_day_note("2022-02-25") ``` Then set/
-update a day note with `set_day_note`. The content should be a (html) string.
-``` self.set_day_note(date, new_content) ``` ## ð¤ Export note Export note
-comes in two formats `html` or `markdown`/`md`. ``` res = ea.export_note
+token, change the `server_url` and `token` to yours. ```python from
+trilium_py.client import ETAPI server_url = 'http://localhost:8080' token =
+'YOUR_TOKEN' ea = ETAPI(server_url, token) ``` If you haven't created ETAPI
+token, you can create one with your password. Please note, you can only see
+this token once, please save it if you want to reuse the token. ```python from
+trilium_py.client import ETAPI server_url = 'http://localhost:8080' password =
+'1234' ea = ETAPI(server_url) token = ea.login(password) print(token) ``` After
+initialization, you can use Trilium ETAPI with python now. The following are
+some examples. ## ð Application Information To start with, you can get the
+application information like this. ```python print(ea.app_info()) ``` It should
+give you the version of your server application and some extra information. ##
+ð Search note Search note with keyword. ```python res = ea.search_note
+( search="python", ) for x in res['results']: print(x['noteId'], x['title'])
+``` ## ð­ Create Note You can create a simple note like this. ```python res =
+ea.create_note( parentNoteId="root", title="Simple note 1", type="text",
+content="Simple note example", noteId="note1" ) ``` The `noteId` is not
+mandatory, if not provided, Trilium will generate a random one. You can
+retrieve it in the return. ```python noteId = res['note']['noteId'] ``` ###
+ð¼ï¸ Create Image note Image note is a special kind of note. You can create
+an image note with minimal information like this. The `image_file` refers to
+the path of image. ```python res = ea.create_image_note( parentNoteId="root",
+title="Image note 1", image_file="shield.png", ) ``` ## ð Get note To
+retrieve the note's content. ```python ea.get_note_content("note1") ``` You can
+get a note metadata by its id. ```python ea.get_note(note_id) ``` ## ð
+Update note Update note content ```python ea.update_note_content("note1",
+"updated by python") ``` Modify note title ```python ea.patch_note
+( noteId="note1", title="Python client moded", ) ``` ## ðï¸ Delete note
+Simply delete a note by id. ```python ea.delete_note("note1") ``` ## ð Day
+note You can get the content of a certain date with `get_day_note`. The date
+string should be in format of "%Y-%m-%d", e.g. " 2022-02-25". ```python
+es.get_day_note("2022-02-25") ``` Then set/update a day note with
+`set_day_note`. The content should be a (html) string. ```python
+self.set_day_note(date, new_content) ``` ## ð¤ Export note Export note comes
+in two formats `html` or `markdown`/`md`. ```python res = ea.export_note
 ( noteId='sK5fn4T6yZRI', format='md', savePath='/home/nate/data/1/test.zip', )
 ``` # (Advanced Usage) â TODO List With the power of Python, I have expanded
 the basic usage of ETAPI. You can do something with todo list now. ## Add TODO
 item You can use `add_todo` to add a TODO item, param is the TODO description
-``` ea.add_todo("ä¹°æå®å®") ``` ## Check/Uncheck a TODO item param is the
-index of the TODO item ``` ea.todo_check(0) ea.todo_uncheck(1) ``` ## Update a
-TODO item Use `update_todo` to update a TODO item description at certain index.
-``` ea.update_todo(0, "å»ç å¤´æ´ç¹è¯æ¡") ``` ## Delete a TDOO item Remove
-a TODO item by its index. ``` ea.delete_todo(1) ``` ## Move yesterday's
-unfinished todo to today As the title suggests, you can move yesterday's
-unfinished things to today. Unfinished todos will be deleted from yesterday's
-note. ``` ea.move_yesterday_unfinished_todo_to_today() ``` # (Advanced Usage)
-ð Upload Markdown files ## Upload single Markdown file with images You can
-import Markdown file with images into Trilium now! Trilium-py will help you to
-upload the images and fix the links for you! ``` res = ea.upload_md_file
-( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps lock.md", ) ``` ##
-Bulk upload Markdown files in a folder! You can upload a folder with lots of
-Markdown files to Trilium and preserve the folder structure! ### Import from
-VNote Say, upload all the notes from [VNote](https://github.com/vnotex/vnote),
-simply do this: ``` res = ea.upload_md_folder( parentNoteId="root",
-mdFolder="~/data/vnotebook/", ignoreFolder=['vx_notebook', 'vx_recycle_bin',
-'vx_images', '_v_images'], ) ``` ### Import from Logseq ``` res =
-ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/data/
-logseq_data/", ignoreFolder=['assets', 'logseq'], ) ``` ### Import from
-Obsidian Obsidian has a very unique linking system for files. You should use
-[obsidian-export ](https://github.com/zoni/obsidian-export) to convert a
-Obsidian vault to regular Markdown files. Then you should be able to import the
-note into Trilium with trilium-py. Convert it first. ``` obsidian-export /path/
-to/your/vault /out ``` Then import just like a normal markdown, trilium-py will
-handle the images for you. ``` res = ea.upload_md_folder( parentNoteId="root",
-mdFolder="E:/data/out", ) ``` ### Import from Youdao Note/æéäºç¬è®°
-Youdao does not provide an export feature anymore. Luckily, you can use https:/
-/github.com/DeppWang/youdaonote-pull to download your notes and convert them
+```python ea.add_todo("ä¹°æå®å®") ``` ## Check/Uncheck a TODO item param is
+the index of the TODO item ```python ea.todo_check(0) ea.todo_uncheck(1) ``` ##
+Update a TODO item Use `update_todo` to update a TODO item description at
+certain index. ```python ea.update_todo(0, "å»ç å¤´æ´ç¹è¯æ¡") ``` ##
+Delete a TDOO item Remove a TODO item by its index. ```python ea.delete_todo(1)
+``` ## Move yesterday's unfinished todo to today As the title suggests, you can
+move yesterday's unfinished things to today. Unfinished todos will be deleted
+from yesterday's note. ```python ea.move_yesterday_unfinished_todo_to_today()
+``` # (Advanced Usage) ð Upload Markdown files ## Upload single Markdown
+file with images You can import Markdown file with images into Trilium now!
+Trilium-py will help you to upload the images and fix the links for you!
+```python res = ea.upload_md_file( parentNoteId="root", file="./md-demo/manjaro
+ä¿®æ¹caps lock.md", ) ``` ## Bulk upload Markdown files in a folder You can
+upload a folder with lots of Markdown files to Trilium and preserve the folder
+structure! ### Import from VNote Say, upload all the notes from [VNote](https:/
+/github.com/vnotex/vnote), simply do this: ```python res = ea.upload_md_folder
+( parentNoteId="root", mdFolder="~/data/vnotebook/", ignoreFolder=
+['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'], ) ``` ### Import
+from Logseq ```python res = ea.upload_md_folder( parentNoteId="root",
+mdFolder="/home/nate/data/logseq_data/", ignoreFolder=['assets', 'logseq'], )
+``` ### Import from Obsidian Obsidian has a very unique linking system for
+files. You should use [obsidian-export ](https://github.com/zoni/obsidian-
+export) to convert a Obsidian vault to regular Markdown files. Then you should
+be able to import the note into Trilium with trilium-py. Convert it first.
+```bash obsidian-export /path/to/your/vault /out ``` Then import just like a
+normal markdown, trilium-py will handle the images for you. ```python res =
+ea.upload_md_folder( parentNoteId="root", mdFolder="E:/data/out", ) ``` ###
+Import from Youdao Note/æéäºç¬è®° Youdao does not provide an export
+feature anymore. Luckily, you can use
+github.com/DeppWang/youdaonote-pull> to download your notes and convert them
 into markdown files. After that, trilium-py should be able to help you import
-them. ``` res = ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/
-gitRepo/youdaonote-pull/out/", ) ``` ### Import from other markdown software In
-general, markdown files have variety of standards. You can always try import
-them with ``` res = ea.upload_md_folder( parentNoteId="root", mdFolder="/home/
-nate/data/your_markdown_files/", ) ``` If there is any problem, please feel
-free to create an [issue](https://github.com/Nriver/trilium-py/issues/new). #
-ð ï¸ Develop Install with pip egg link to make package change without
-reinstall. ``` python -m pip install --user -e . ``` # ð Original OpenAPI
-Documentation The original OpenAPI document is [here](https://github.com/zadam/
-trilium/blob/master/src/etapi/etapi.openapi.yaml). You can open it with
-[swagger editor](https://editor.swagger.io/).
+them. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/
+home/nate/gitRepo/youdaonote-pull/out/", ) ``` ### Import from other markdown
+software In general, markdown files have variety of standards. You can always
+try import them with ```python res = ea.upload_md_folder( parentNoteId="root",
+mdFolder="/home/nate/data/your_markdown_files/", ) ``` If there is any problem,
+please feel free to create an [issue](https://github.com/Nriver/trilium-py/
+issues/new). # ð ï¸ Develop Install with pip egg link to make package change
+without reinstall. ```python python -m pip install --user -e . ``` # ð
+Original OpenAPI Documentation The original OpenAPI document is [here](https://
+github.com/zadam/trilium/blob/master/src/etapi/etapi.openapi.yaml). You can
+open it with [swagger editor](https://editor.swagger.io/).
```

## Comparing `trilium_py-0.7.3.dist-info/RECORD` & `trilium_py-0.7.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
 trilium_py/client.py,sha256=kpSEbnEiNgxLIs9KxUf8s-OXJmt-atzeNGLgW_oTiDE,27921
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/markdown_math.py,sha256=ORQwEXAPtcf2-NaYKx4Pr5q5B8CtupVRYt04JD-c3EY,8656
 trilium_py/utils/param_util.py,sha256=BOiblP1F-jMgggx8L_QxCH3s8-FIdG1kAM-4ykSbZ5E,675
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=U1Qn5UFzQO-Bi9DGjq2OEiVzCi6x5KXsyRKF-AOJV64,470
-trilium_py-0.7.3.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.7.3.dist-info/METADATA,sha256=irH-6onMNAD1MSQIn_YnJcm8PXqhx0Izdn5tZm2snU0,10195
-trilium_py-0.7.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-trilium_py-0.7.3.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.7.3.dist-info/RECORD,,
+trilium_py-0.7.4.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.7.4.dist-info/METADATA,sha256=6pQLG1NtC2G0YGl9wLDKhUGnP1jErTz8wi4adzXq6BE,10488
+trilium_py-0.7.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+trilium_py-0.7.4.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.7.4.dist-info/RECORD,,
```

