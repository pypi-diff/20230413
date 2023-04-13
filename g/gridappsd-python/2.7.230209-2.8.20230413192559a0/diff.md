# Comparing `tmp/gridappsd_python-2.7.230209.tar.gz` & `tmp/gridappsd_python-2.8.20230413192559a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_python-2.7.230209.tar", max compression
+gzip compressed data, was "gridappsd_python-2.8.20230413192559a0.tar", max compression
```

## Comparing `gridappsd_python-2.7.230209.tar` & `gridappsd_python-2.8.20230413192559a0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    10501 2023-02-09 21:09:17.000100 gridappsd_python-2.7.230209/README.md
--rw-r--r--   0        0        0     3756 2023-02-09 21:09:17.000100 gridappsd_python-2.7.230209/gridappsd/__init__.py
--rw-r--r--   0        0        0     4620 2023-02-09 21:09:17.000100 gridappsd_python-2.7.230209/gridappsd/__main__.py
--rw-r--r--   0        0        0     7189 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/app_registration.py
--rwxr-xr-x   0        0        0      555 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/conf/entrypoint.sh
--rwxr-xr-x   0        0        0      434 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/conf/run-gridappsd.sh
--rw-r--r--   0        0        0     4689 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/difference_builder.py
--rw-r--r--   0        0        0    27595 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/docker_handler.py
--rw-r--r--   0        0        0      231 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      280 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0     9731 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     1180 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0     1435 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0    10996 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0    17129 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/goss.py
--rw-r--r--   0        0        0    12684 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/gridappsd.py
--rw-r--r--   0        0        0     3318 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/houses.py
--rw-r--r--   0        0        0     2723 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/loghandler.py
--rw-r--r--   0        0        0     2449 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/register_app.py
--rw-r--r--   0        0        0    12220 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/simulation.py
--rw-r--r--   0        0        0     3234 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/timeseries.py
--rw-r--r--   0        0        0     8662 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/topics.py
--rw-r--r--   0        0        0     3177 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/gridappsd/utils.py
--rw-r--r--   0        0        0     1354 2023-02-09 21:09:17.004100 gridappsd_python-2.7.230209/pyproject.toml
--rw-r--r--   0        0        0    11913 1970-01-01 00:00:00.000000 gridappsd_python-2.7.230209/setup.py
--rw-r--r--   0        0        0    11456 1970-01-01 00:00:00.000000 gridappsd_python-2.7.230209/PKG-INFO
+-rw-r--r--   0        0        0    10501 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/README.md
+-rw-r--r--   0        0        0     3756 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4620 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/__main__.py
+-rw-r--r--   0        0        0     7189 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/app_registration.py
+-rwxr-xr-x   0        0        0      555 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/conf/entrypoint.sh
+-rwxr-xr-x   0        0        0      434 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/conf/run-gridappsd.sh
+-rw-r--r--   0        0        0     4689 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/difference_builder.py
+-rw-r--r--   0        0        0    27595 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/docker_handler.py
+-rw-r--r--   0        0        0      227 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/field_interface/__init__.py
+-rw-r--r--   0        0        0      280 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/field_interface/agents/__init__.py
+-rw-r--r--   0        0        0    13584 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/field_interface/agents/agents.py
+-rw-r--r--   0        0        0     2038 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/field_interface/context.py
+-rw-r--r--   0        0        0     1840 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/field_interface/gridappsd_field_bus.py
+-rw-r--r--   0        0        0     7538 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/field_interface/interfaces.py
+-rw-r--r--   0        0        0    17130 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/goss.py
+-rw-r--r--   0        0        0    12684 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/gridappsd.py
+-rw-r--r--   0        0        0     3318 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/houses.py
+-rw-r--r--   0        0        0     2723 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/loghandler.py
+-rw-r--r--   0        0        0     2449 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/register_app.py
+-rw-r--r--   0        0        0    12220 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/simulation.py
+-rw-r--r--   0        0        0     3234 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/timeseries.py
+-rw-r--r--   0        0        0    12052 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/topics.py
+-rw-r--r--   0        0        0     3177 2023-04-13 19:25:12.013235 gridappsd_python-2.8.20230413192559a0/gridappsd/utils.py
+-rw-r--r--   0        0        0     1132 2023-04-13 19:25:59.709993 gridappsd_python-2.8.20230413192559a0/pyproject.toml
+-rw-r--r--   0        0        0    11466 1970-01-01 00:00:00.000000 gridappsd_python-2.8.20230413192559a0/PKG-INFO
```

### Comparing `gridappsd_python-2.7.230209/README.md` & `gridappsd_python-2.8.20230413192559a0/README.md`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/__init__.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/__main__.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/app_registration.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/app_registration.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/conf/entrypoint.sh` & `gridappsd_python-2.8.20230413192559a0/gridappsd/conf/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/difference_builder.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/difference_builder.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/docker_handler.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/docker_handler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/goss.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/goss.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         self._topics_callback_map = defaultdict(list)
         self._queue_callerback = Queue()
         self._thread = threading.Thread(target=self.run_callbacks)
         self._thread.daemon = True
         self._thread.start()
 
     def run_callbacks(self):
-        _log.info("Starting thread queue")
+        _log.debug("Starting thread queue")
         while True:
             cb, hdrs, msg = self._queue_callerback.get()
             try:
                 msg = json.loads(msg)
             except:
                 pass
                 # msg = message
```

### Comparing `gridappsd_python-2.7.230209/gridappsd/gridappsd.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/gridappsd.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/houses.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/houses.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/loghandler.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/loghandler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/register_app.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/register_app.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/simulation.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/simulation.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/timeseries.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/timeseries.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/gridappsd/utils.py` & `gridappsd_python-2.8.20230413192559a0/gridappsd/utils.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2.7.230209/pyproject.toml` & `gridappsd_python-2.8.20230413192559a0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-python"
-version = "v2.7.230209"
+version = "2.8.20230413192559a0"
 description = "A GridAPPS-D Python Adapter"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -29,18 +29,16 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.7.9,<4.0"
 PyYAML = "^6.0"
 pytz = "^2022.7"
 dateutils = "^0.6.7"
-#gridappsd-cim-profile={url="https://github.com/GRIDAPPSD/gridappsd-cim-profile/releases/download/v0.7.20230120180831a0/gridappsd_cim_profile-0.7.20230120180831a0-py3-none-any.whl"}
-#gridappsd-cim-profile = "^0.10.20230208223046a0"
 stomp-py = "6.0.0"
-gridappsd-cim-lab = "^0.11.230209"
+cim-graph = "^0.1.20230413185916a0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
 docker = "^4.4.4"
 yapf = "^0.32.0"
```

### Comparing `gridappsd_python-2.7.230209/setup.py` & `gridappsd_python-2.8.20230413192559a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,354 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gridappsd-python
+Version: 2.8.20230413192559a0
+Summary: A GridAPPS-D Python Adapter
+Home-page: https://gridappsd.readthedocs.io
+License: BSD-3-Clause
+Keywords: gridappsd,grid,activmq,powergrid,simulation,library
+Author: C. Allwardt
+Author-email: 3979063+craig8@users.noreply.github.com
+Requires-Python: >=3.7.9,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: cim-graph (>=0.1.20230413185916a0,<0.2.0)
+Requires-Dist: dateutils (>=0.6.7,<0.7.0)
+Requires-Dist: pytz (>=2022.7,<2023.0)
+Requires-Dist: stomp-py (==6.0.0)
+Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
+Description-Content-Type: text/markdown
 
-packages = \
-['gridappsd', 'gridappsd.field_interface', 'gridappsd.field_interface.agents']
+[![Run All Pytests](https://github.com/GRIDAPPSD/gridappsd-python/actions/workflows/run-pytest.yml/badge.svg)](https://github.com/GRIDAPPSD/gridappsd-python/actions/workflows/run-pytest.yml)
 
-package_data = \
-{'': ['*'], 'gridappsd': ['conf/*']}
+# gridappsd-python
+Python library for developing applications and services against the gridappsd api
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'dateutils>=0.6.7,<0.7.0',
- 'gridappsd-cim-lab>=0.11.230209,<0.12.0',
- 'pytz>=2022.7,<2023.0',
- 'stomp-py==6.0.0']
-
-entry_points = \
-{'console_scripts': ['gridappsd-cli = gridappsd.cli:_main',
-                     'register_app = gridappsd.register_app:main']}
-
-setup_kwargs = {
-    'name': 'gridappsd-python',
-    'version': '2.7.230209',
-    'description': 'A GridAPPS-D Python Adapter',
-    'long_description': '[![Run All Pytests](https://github.com/GRIDAPPSD/gridappsd-python/actions/workflows/run-pytest.yml/badge.svg)](https://github.com/GRIDAPPSD/gridappsd-python/actions/workflows/run-pytest.yml)\n\n# gridappsd-python\nPython library for developing applications and services against the gridappsd api\n\n## Requirements\n\nThe gridappsd-python library requires a  python version >= 3.6 and < 4 in order to work properly (Note no testing\nhas been done with python 4 to date).\n\n## Installation\n\nThe recommended installation of `gridappsd-python` is in a separate virtual environment.  Executing the following\nwill create an environment called `griddapps-env`.\n\n```shell\npython3 -m venv gridappsd-env\n```\n\nSourcing the gridappsd-env activates the newly created python environment.\n\n```shell\nsource gridappsd-env/bin/activate\n```\n\nUpgrade pip to the latest (some packages require 19.0+ version of pip).\n\n```shell\npython -m pip install pip --upgrade\n```\n\nInstall the latest `gridappsd-python` and its dependencies in the virtual environment.\n\n```shell\npip install gridappsd-python\n```\n\n### Verifying things are working properly\n\nThe following code snippet assumes you have created a gridappsd instance using the steps in\nhttps://github.com/GRIDAPPSD/gridappsd-docker.\n\nCreate a test script (tester.py) with the following content.\n\n```python\n\nfrom gridappsd import GridAPPSD\n\ndef on_message_callback(header, message):\n    print(f"header: {header} message: {message}")\n\n# Note these should be changed on the server in a cyber secure environment!\nusername = "app_user"\npassword = "1234App"\n\n# Note: there are other parameters for connecting to\n# systems other than localhost\ngapps = GridAPPSD(username=username, password=password)\n\nassert gapps.connected\n\ngapps.send(\'send.topic\', {"foo": "bar"})\n\n# Note we are sending the function not executing the function in the second parameter\ngapps.subscribe(\'subscribe.topic\', on_message_callback)\n\ngapps.send(\'subcribe.topic\', \'A message about subscription\')\n\ntime.sleep(5)\n\ngapps.close()\n\n```\n\nStart up the gridappsd-docker enabled platform.  Then run the following to execute the tester.py script\n\n```shell\npython tester.py\n```\n\n## Application Developers\n\n### Deployment\n\nPlease see [DOCKER_CONTAINER.md](DOCKER_CONTAINER.md) for working within the docker application base container.\n\n### Local Development\n\nDeveloping applications against gridappsd using the `gridappsd-python` library should follow the same steps\nas above, however with a couple of environmental variables specified.  The following environmental variables are\navailable to provide the same context that would be available from inside the application docker container.  These\nare useful to know for developing your application outside of the docker context (e.g. in a python notebook).\n\n***NOTE: you can also define these your ~./bashrc file so you don\'t have to specify them all the time***\n\n```shell\n# export allows all processes started by this shell to have access to the global variable\n\n# address where the gridappsd server is running - default localhost\nexport GRIDAPPSD_ADDRESS=localhost\n\n# port to connect to on the gridappsd server (the stomp client port)\nexport GRIDAPPSD_PORT=61613\n\n# username to connect to the gridappsd server\nexport GRIDAPPSD_USER=app_user\n\n# password to connect to the gridappsd server\nexport GRIDAPPSD_PASSWORD=1234App\n\n# Note these should be changed on the server in a cyber secure environment!\n```\n\nThe following is the same tester code as above, but with the environment variables set.  The environment variables\nshould be set in your environment when running the application inside our docker container.\n\n```python\n\nfrom gridappsd import GridAPPSD\n\ndef on_message_callback(header, message):\n    print(f"header: {header} message: {message}")\n\n# Create GridAPPSD object and connect to the gridappsd server.\ngapps = GridAPPSD()\n\nassert gapps.connected\n\ngapps.send(\'send.topic\', {"foo": "bar"})\n\n# Note we are sending the function not executing the function in the second parameter\ngapps.subscribe(\'subscribe.topic\', on_message_callback)\n\ngapps.send(\'subcribe.topic\', \'A message about subscription\')\n\ntime.sleep(5)\n\ngapps.close()\n\n```\n\n## Developers\n\nThis project uses poetry to build the environment for execution.  Follow the instructions\nhttps://python-poetry.org/docs/#installation to install poetry.  As a developer I prefer not to have poetry installed\nin the same virtual environment that my projects are in.\n\nClone the github repository:\n\n```shell\ngit clone https://github.com/GRIDAPPSD/gridappsd-python -b develop\ncd gridappsd-python\n```\n\nThe following commands build and install a local wheel into an environment created just for this package.\n\n```shell\n# Build the project (stores in dist directory both .tar.gz and .whl file)\npoetry build\n\n# Install the wheel into the environment and the dev dependencies\npoetry install\n\n# Install only the library dependencies\npoetry install --no-dev\n```\n\n***Note:*** Poetry does not have a setup.py that you can install in editable mode like with pip install -e ., however\nyou can extract the generated setup.py file from the built tar.gz file in the dist directory.  Just extract the\n.tar.gz file and copy the setup.py file from the extracted directory to the root of gridappsd-python.  Then you can\nenable editing through pip install -e. as normal.\n\n\n## Testing\n\nTesting has become an integral part of the software lifecycle.  The `gridappsd-python` library has both unit and\nintegration tests available to be run.  In order to execute these, you must have installed the gridappsd-python library\nas above with dev-dependencies.\n\nDuring the testing phase the docker containers required for the tests are downloaded from\ndockerhub and started.  By default the `develop` tag is used to test the library using pytest.  \nOne can customize the docker image tag by setting the environmental\nvariable `GRIDAPPSD_TAG_ENV` either by `export GRIDAPPSD_TAG_ENV=other_tag` or by executing \npytest with the following:\n\n```shell script\n\n# Export environmental variables and all tests will use the same tag (other_tag) to pull from docker hub.\n# Default tag is develop\nexport GRIDAPPSD_TAG_ENV=other_tag\npytest\n\n# Tests also require the username and password to be avaialable as environmental variables \n# in order for them to properly run these tests\nexport GRIDAPPSD_USER=user\nexport GRIDAPPSD_PASSWORD=pass\n\npytest\n```\n\n ***NOTE: the first running the tests will download all of the docker images associated with the\n [GOSS-GridAPPS-D](http://github.com/GRIDAPPSD/GOSS-GridAPPS-D) repository.  This process may take some time.***\n \n### Running tests created in a new project\n\nThe `gridappsd-python` library exposes a testing environment through the `gridappsd.docker_handler` module.  Including the following\n`conftest.py` in the root of your base test directory allows tests to reference these.  Using these fixtures will start all of the\nbase containers required for `gridappsd` to run.  \n\n```python\n\n# conftest.py\n# Create a conftest.py file in the root of the tests directory to enable usage throughout the tests directory and below. \n# \n# Tested project structure an layout\n#\n# project-folder\\\n#   mainmodule\\\n#     __init__.py\n#     myapplication.py\n#   tests\\\n#     conftest.py\n#     test_myapplication.py\n#   README.md\n\nimport logging\nimport os\nimport sys\n\nimport pytest\n\nfrom gridappsd import GridAPPSD, GOSS\nfrom gridappsd.docker_handler import run_dependency_containers, run_gridappsd_container, Containers\n\nlevels = dict(\n    CRITICAL=50,\n    FATAL=50,\n    ERROR=40,\n    WARNING=30,\n    WARN=30,\n    INFO=20,\n    DEBUG=10,\n    NOTSET=0\n)\n\n# Get string representation of the log level passed\nLOG_LEVEL = os.environ.get("LOG_LEVEL", "INFO")\n\n# Make sure the level passed is one of the valid levels.\nif LOG_LEVEL not in levels.keys():\n    raise AttributeError("Invalid LOG_LEVEL environmental variable set.")\n\n# Set the numeric version of log level to pass to the basicConfig function\nLOG_LEVEL = levels[LOG_LEVEL]\n\nlogging.basicConfig(stream=sys.stdout, level=LOG_LEVEL,\n                    format="%(asctime)s|%(levelname)s|%(name)s|%(message)s")\nlogging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)\nlogging.getLogger("docker.utils.config").setLevel(logging.INFO)\nlogging.getLogger("docker.auth").setLevel(logging.INFO)\n\n\nSTOP_CONTAINER_AFTER_TEST = os.environ.get(\'GRIDAPPSD_STOP_CONTAINERS_AFTER_TESTS\', True)\n\n\n@pytest.fixture(scope="module")\ndef docker_dependencies():\n    print("Docker dependencies")\n    # Containers.reset_all_containers()\n\n    with run_dependency_containers(stop_after=STOP_CONTAINER_AFTER_TEST) as dep:\n        yield dep\n    print("Cleanup docker dependencies")\n\n\n@pytest.fixture\ndef gridappsd_client(request, docker_dependencies):\n    with run_gridappsd_container(stop_after=STOP_CONTAINER_AFTER_TEST):\n        gappsd = GridAPPSD()\n        gappsd.connect()\n        assert gappsd.connected\n        models = gappsd.query_model_names()\n        assert models is not None\n        if request.cls is not None:\n            request.cls.gridappsd_client = gappsd\n        yield gappsd\n\n        gappsd.disconnect()\n\n\n@pytest.fixture\ndef goss_client(docker_dependencies):\n    with run_gridappsd_container(stop_after=STOP_CONTAINER_AFTER_TEST):\n        goss = GOSS()\n        goss.connect()\n        assert goss.connected\n\n        yield goss\n\n```\n\nUsing the above fixtures from inside a test module and test function looks like the following:\n\n```python\n\n# Example test function using the gridappsd_client fixture \n\n@mock.patch.dict(os.environ, {"GRIDAPPSD_APPLICATION_ID": "helics_goss_bridge.py"})\ndef test_gridappsd_status(gridappsd_client):\n    gappsd = gridappsd_client\n    assert "helics_goss_bridge.py" == gappsd.get_application_id()\n    assert gappsd.get_application_status() == ProcessStatusEnum.STARTING.value\n    assert gappsd.get_service_status() == ProcessStatusEnum.STARTING.value\n    gappsd.set_application_status("RUNNING")\n\n    assert gappsd.get_service_status() == ProcessStatusEnum.RUNNING.value\n    assert gappsd.get_application_status() == ProcessStatusEnum.RUNNING.value\n\n    gappsd.set_service_status("COMPLETE")\n    assert gappsd.get_service_status() == ProcessStatusEnum.COMPLETE.value\n    assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value\n\n    # Invalid\n    gappsd.set_service_status("Foo")\n    assert gappsd.get_service_status() == ProcessStatusEnum.COMPLETE.value\n    assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value\n\n```\n\n',
-    'author': 'C. Allwardt',
-    'author_email': '3979063+craig8@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gridappsd.readthedocs.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.9,<4.0',
-}
+## Requirements
+
+The gridappsd-python library requires a  python version >= 3.6 and < 4 in order to work properly (Note no testing
+has been done with python 4 to date).
+
+## Installation
+
+The recommended installation of `gridappsd-python` is in a separate virtual environment.  Executing the following
+will create an environment called `griddapps-env`.
+
+```shell
+python3 -m venv gridappsd-env
+```
+
+Sourcing the gridappsd-env activates the newly created python environment.
+
+```shell
+source gridappsd-env/bin/activate
+```
+
+Upgrade pip to the latest (some packages require 19.0+ version of pip).
+
+```shell
+python -m pip install pip --upgrade
+```
+
+Install the latest `gridappsd-python` and its dependencies in the virtual environment.
+
+```shell
+pip install gridappsd-python
+```
+
+### Verifying things are working properly
+
+The following code snippet assumes you have created a gridappsd instance using the steps in
+https://github.com/GRIDAPPSD/gridappsd-docker.
+
+Create a test script (tester.py) with the following content.
+
+```python
+
+from gridappsd import GridAPPSD
+
+def on_message_callback(header, message):
+    print(f"header: {header} message: {message}")
+
+# Note these should be changed on the server in a cyber secure environment!
+username = "app_user"
+password = "1234App"
+
+# Note: there are other parameters for connecting to
+# systems other than localhost
+gapps = GridAPPSD(username=username, password=password)
+
+assert gapps.connected
+
+gapps.send('send.topic', {"foo": "bar"})
+
+# Note we are sending the function not executing the function in the second parameter
+gapps.subscribe('subscribe.topic', on_message_callback)
+
+gapps.send('subcribe.topic', 'A message about subscription')
+
+time.sleep(5)
+
+gapps.close()
+
+```
+
+Start up the gridappsd-docker enabled platform.  Then run the following to execute the tester.py script
+
+```shell
+python tester.py
+```
+
+## Application Developers
+
+### Deployment
+
+Please see [DOCKER_CONTAINER.md](DOCKER_CONTAINER.md) for working within the docker application base container.
+
+### Local Development
+
+Developing applications against gridappsd using the `gridappsd-python` library should follow the same steps
+as above, however with a couple of environmental variables specified.  The following environmental variables are
+available to provide the same context that would be available from inside the application docker container.  These
+are useful to know for developing your application outside of the docker context (e.g. in a python notebook).
+
+***NOTE: you can also define these your ~./bashrc file so you don't have to specify them all the time***
+
+```shell
+# export allows all processes started by this shell to have access to the global variable
+
+# address where the gridappsd server is running - default localhost
+export GRIDAPPSD_ADDRESS=localhost
+
+# port to connect to on the gridappsd server (the stomp client port)
+export GRIDAPPSD_PORT=61613
+
+# username to connect to the gridappsd server
+export GRIDAPPSD_USER=app_user
+
+# password to connect to the gridappsd server
+export GRIDAPPSD_PASSWORD=1234App
+
+# Note these should be changed on the server in a cyber secure environment!
+```
+
+The following is the same tester code as above, but with the environment variables set.  The environment variables
+should be set in your environment when running the application inside our docker container.
+
+```python
+
+from gridappsd import GridAPPSD
+
+def on_message_callback(header, message):
+    print(f"header: {header} message: {message}")
+
+# Create GridAPPSD object and connect to the gridappsd server.
+gapps = GridAPPSD()
+
+assert gapps.connected
+
+gapps.send('send.topic', {"foo": "bar"})
+
+# Note we are sending the function not executing the function in the second parameter
+gapps.subscribe('subscribe.topic', on_message_callback)
+
+gapps.send('subcribe.topic', 'A message about subscription')
+
+time.sleep(5)
+
+gapps.close()
+
+```
+
+## Developers
+
+This project uses poetry to build the environment for execution.  Follow the instructions
+https://python-poetry.org/docs/#installation to install poetry.  As a developer I prefer not to have poetry installed
+in the same virtual environment that my projects are in.
+
+Clone the github repository:
+
+```shell
+git clone https://github.com/GRIDAPPSD/gridappsd-python -b develop
+cd gridappsd-python
+```
+
+The following commands build and install a local wheel into an environment created just for this package.
+
+```shell
+# Build the project (stores in dist directory both .tar.gz and .whl file)
+poetry build
+
+# Install the wheel into the environment and the dev dependencies
+poetry install
+
+# Install only the library dependencies
+poetry install --no-dev
+```
+
+***Note:*** Poetry does not have a setup.py that you can install in editable mode like with pip install -e ., however
+you can extract the generated setup.py file from the built tar.gz file in the dist directory.  Just extract the
+.tar.gz file and copy the setup.py file from the extracted directory to the root of gridappsd-python.  Then you can
+enable editing through pip install -e. as normal.
+
+
+## Testing
+
+Testing has become an integral part of the software lifecycle.  The `gridappsd-python` library has both unit and
+integration tests available to be run.  In order to execute these, you must have installed the gridappsd-python library
+as above with dev-dependencies.
+
+During the testing phase the docker containers required for the tests are downloaded from
+dockerhub and started.  By default the `develop` tag is used to test the library using pytest.  
+One can customize the docker image tag by setting the environmental
+variable `GRIDAPPSD_TAG_ENV` either by `export GRIDAPPSD_TAG_ENV=other_tag` or by executing 
+pytest with the following:
+
+```shell script
+
+# Export environmental variables and all tests will use the same tag (other_tag) to pull from docker hub.
+# Default tag is develop
+export GRIDAPPSD_TAG_ENV=other_tag
+pytest
+
+# Tests also require the username and password to be avaialable as environmental variables 
+# in order for them to properly run these tests
+export GRIDAPPSD_USER=user
+export GRIDAPPSD_PASSWORD=pass
+
+pytest
+```
+
+ ***NOTE: the first running the tests will download all of the docker images associated with the
+ [GOSS-GridAPPS-D](http://github.com/GRIDAPPSD/GOSS-GridAPPS-D) repository.  This process may take some time.***
+ 
+### Running tests created in a new project
+
+The `gridappsd-python` library exposes a testing environment through the `gridappsd.docker_handler` module.  Including the following
+`conftest.py` in the root of your base test directory allows tests to reference these.  Using these fixtures will start all of the
+base containers required for `gridappsd` to run.  
+
+```python
+
+# conftest.py
+# Create a conftest.py file in the root of the tests directory to enable usage throughout the tests directory and below. 
+# 
+# Tested project structure an layout
+#
+# project-folder\
+#   mainmodule\
+#     __init__.py
+#     myapplication.py
+#   tests\
+#     conftest.py
+#     test_myapplication.py
+#   README.md
+
+import logging
+import os
+import sys
+
+import pytest
+
+from gridappsd import GridAPPSD, GOSS
+from gridappsd.docker_handler import run_dependency_containers, run_gridappsd_container, Containers
+
+levels = dict(
+    CRITICAL=50,
+    FATAL=50,
+    ERROR=40,
+    WARNING=30,
+    WARN=30,
+    INFO=20,
+    DEBUG=10,
+    NOTSET=0
+)
+
+# Get string representation of the log level passed
+LOG_LEVEL = os.environ.get("LOG_LEVEL", "INFO")
+
+# Make sure the level passed is one of the valid levels.
+if LOG_LEVEL not in levels.keys():
+    raise AttributeError("Invalid LOG_LEVEL environmental variable set.")
+
+# Set the numeric version of log level to pass to the basicConfig function
+LOG_LEVEL = levels[LOG_LEVEL]
+
+logging.basicConfig(stream=sys.stdout, level=LOG_LEVEL,
+                    format="%(asctime)s|%(levelname)s|%(name)s|%(message)s")
+logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
+logging.getLogger("docker.utils.config").setLevel(logging.INFO)
+logging.getLogger("docker.auth").setLevel(logging.INFO)
+
+
+STOP_CONTAINER_AFTER_TEST = os.environ.get('GRIDAPPSD_STOP_CONTAINERS_AFTER_TESTS', True)
+
+
+@pytest.fixture(scope="module")
+def docker_dependencies():
+    print("Docker dependencies")
+    # Containers.reset_all_containers()
+
+    with run_dependency_containers(stop_after=STOP_CONTAINER_AFTER_TEST) as dep:
+        yield dep
+    print("Cleanup docker dependencies")
+
+
+@pytest.fixture
+def gridappsd_client(request, docker_dependencies):
+    with run_gridappsd_container(stop_after=STOP_CONTAINER_AFTER_TEST):
+        gappsd = GridAPPSD()
+        gappsd.connect()
+        assert gappsd.connected
+        models = gappsd.query_model_names()
+        assert models is not None
+        if request.cls is not None:
+            request.cls.gridappsd_client = gappsd
+        yield gappsd
+
+        gappsd.disconnect()
+
+
+@pytest.fixture
+def goss_client(docker_dependencies):
+    with run_gridappsd_container(stop_after=STOP_CONTAINER_AFTER_TEST):
+        goss = GOSS()
+        goss.connect()
+        assert goss.connected
+
+        yield goss
+
+```
+
+Using the above fixtures from inside a test module and test function looks like the following:
+
+```python
+
+# Example test function using the gridappsd_client fixture 
+
+@mock.patch.dict(os.environ, {"GRIDAPPSD_APPLICATION_ID": "helics_goss_bridge.py"})
+def test_gridappsd_status(gridappsd_client):
+    gappsd = gridappsd_client
+    assert "helics_goss_bridge.py" == gappsd.get_application_id()
+    assert gappsd.get_application_status() == ProcessStatusEnum.STARTING.value
+    assert gappsd.get_service_status() == ProcessStatusEnum.STARTING.value
+    gappsd.set_application_status("RUNNING")
+
+    assert gappsd.get_service_status() == ProcessStatusEnum.RUNNING.value
+    assert gappsd.get_application_status() == ProcessStatusEnum.RUNNING.value
+
+    gappsd.set_service_status("COMPLETE")
+    assert gappsd.get_service_status() == ProcessStatusEnum.COMPLETE.value
+    assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value
+
+    # Invalid
+    gappsd.set_service_status("Foo")
+    assert gappsd.get_service_status() == ProcessStatusEnum.COMPLETE.value
+    assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value
+
+```
 
 
-setup(**setup_kwargs)
```

