# Comparing `tmp/clibrary-1.5.0.tar.gz` & `tmp/clibrary-1.6.1.tar.gz`

## Comparing `clibrary-1.5.0.tar` & `clibrary-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.5.0/Makefile
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 clibrary-1.5.0/docs.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.5.0/src/CLIbrary/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.5.0/src/CLIbrary/files.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 clibrary-1.5.0/src/CLIbrary/inputs.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 clibrary-1.5.0/src/CLIbrary/interface.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 clibrary-1.5.0/src/CLIbrary/outputs.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.5.0/src/CLIbrary/settings.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.5.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.5.0/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 clibrary-1.5.0/README.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 clibrary-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 clibrary-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.6.1/Makefile
+-rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 clibrary-1.6.1/docs.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.6.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.6.1/src/CLIbrary/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.6.1/src/CLIbrary/files.py
+-rw-r--r--   0        0        0    10422 2020-02-02 00:00:00.000000 clibrary-1.6.1/src/CLIbrary/inputs.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 clibrary-1.6.1/src/CLIbrary/interface.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 clibrary-1.6.1/src/CLIbrary/outputs.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.6.1/src/CLIbrary/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.6.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.6.1/LICENSE
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 clibrary-1.6.1/README.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 clibrary-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 clibrary-1.6.1/PKG-INFO
```

### Comparing `clibrary-1.5.0/docs.md` & `clibrary-1.6.1/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,19 @@
 
 1. `CLIbrary.style.setting_darkMode`, bool: Enables global dark mode.
 2. `CLIbrary.style.setting_plainMode`, bool: Disables styling.
 3. `CLIbrary.data.setting_fileExtension`, str: Defines a file extension for *CLIbrary.aDump* and *CLIbrary.aLoad*. Default value based on Python's module *pickle*.
 
 ### Import CLIbrary
 
-**CLIbrary** can be imported by:
+**CLIbrary** can be installed by:
+
+	python3 -m pip install --upgrade CLIbrary
+	
+imported by:
 
 	import CLIbrary
 
 and all the functions can be accessed by:
 
 	CLIbrary.FUNCTION_NAME()
 
@@ -239,23 +243,26 @@
 * Bools.
 	* verbose.
 
 ### Dates
 
 	CLIbrary.dateIn(dateHandler={}) -> str
 
-*dateIn* stands for *Date Input* as this function's purpose is receiving date inputs.
+*dateIn* stands for *Date Input* as this function's purpose is receiving date[^4] inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
 * Bools.
+	* placeholders: Enables the use of "x"s as placeholders for not fully known dates.
 	* verbose.
 
+[^4]: Dates have to be passed in respect to the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) standard. 
+
 ### List handling
 
 	CLIbrary.listCh(listHandler={})
 
 *listCh* stands for *List Choice* as this function returns the choosen element from a list.
 
 The handler for this function makes use of the following parameters:
@@ -278,8 +285,8 @@
 	* string: The output string.
 	* type: The output type, to be choosen from:
 		* `"error"`,
 		* `"warning"`,
 		* `"verbose"`,
 		* `""`: A plain style, similar to that of `CLIbrary.style.setting_plainMode`.
 	* before: A string that gets printed before the output and is unaffected by the output styling.
-	* after: A string that gets printed after the output and is unaffected by the output styling.
+	* after: A string that gets printed after the output and is unaffected by the output styling.
```

### Comparing `clibrary-1.5.0/.github/workflows/python-publish.yml` & `clibrary-1.6.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `clibrary-1.5.0/src/CLIbrary/files.py` & `clibrary-1.6.1/src/CLIbrary/files.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.5.0/src/CLIbrary/inputs.py` & `clibrary-1.6.1/src/CLIbrary/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,25 +141,28 @@
 	handler = {}
 
 	# Strings.
 	handler["request"] = "Date"
 	handler["added"] = " [YYYY-MM-DD]: "
 
 	# Bools.
+	handler["placeholders"] = False
 	handler["verbose"] = False
 
 	# Updates the handler.
 	handler.update(dateHandler)
 
 	# Checks types and values.
 	if not type(handler["request"]) == str:
 		handler["request"] = "Date"
 	if not type(handler["added"]) == str:
 		handler["added"] = " [YYYY-MM-DD]: "
 
+	if not type(handler["placeholders"]) == bool:
+		handler["placeholders"] = False
 	if not type(handler["verbose"]) == bool:
 		handler["verbose"] = False
 
 	# String handler.
 	strHandler = {}
 	strHandler["request"] = handler["request"]
 	strHandler["added"] = handler["added"]
@@ -170,15 +173,15 @@
 	while True:
 		answer = strIn(strHandler)
 
 		if handler["verbose"]:
 			output({"type": "verbose", "string": "VERBOSE, INPUT: " + answer})
 
 		try: # From an answer of Eduard Stepanov on https://stackoverflow.com/questions/16870663/how-do-i-validate-a-date-string-format-in-python
-			if answer != datetime.strptime(answer, "%Y-%m-%d").strftime('%Y-%m-%d'):
+			if answer != datetime.strptime(answer.replace("xxxx", "0001").replace("xxx", "001").replace("xx", "01").replace("x", "1") if handler["placeholders"] else answer, "%Y-%m-%d").strftime('%Y-%m-%d'):
 				raise(ValueError)
 
 			return answer
 		
 		except(ValueError):
 			pass
```

### Comparing `clibrary-1.5.0/src/CLIbrary/interface.py` & `clibrary-1.6.1/src/CLIbrary/interface.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.5.0/src/CLIbrary/outputs.py` & `clibrary-1.6.1/src/CLIbrary/outputs.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.5.0/LICENSE` & `clibrary-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clibrary-1.5.0/pyproject.toml` & `clibrary-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "colorama", "datetime"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CLIbrary"
-version = "1.5.0"
+version = "1.6.1"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "A standardized collection of CLI utilities written in Python to handle commands, I/O and files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `clibrary-1.5.0/PKG-INFO` & `clibrary-1.6.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLIbrary
-Version: 1.5.0
+Version: 1.6.1
 Summary: A standardized collection of CLI utilities written in Python to handle commands, I/O and files.
 Project-URL: Homepage, https://github.com/diantonioandrea/CLIbrary
 Project-URL: Documentation, https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/CLIbrary/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,7 +27,24 @@
 	python3 -m pip install --upgrade CLIbrary
 
 ### Importing CLIbrary
 
 **CLIbrary** can be imported by:
 
 	import CLIbrary
+
+## Examples
+
+### Entering commands with options
+
+Code:
+
+	import CLIbrary
+
+	commandHandler = {"request": "Command", "allowedCommands": ["sample"]}
+	command = CLIbrary.cmdIn(commandHandler)
+	print(command)
+
+Output:
+
+	Command: sample -option1 value --option2
+	{'command': 'sample', 'sdOpts': {'option1': 'value'}, 'ddOpts': ['option2']}
```

