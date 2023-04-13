# Comparing `tmp/fabrictestbed-mflib-0.0.0b1.tar.gz` & `tmp/fabrictestbed-mflib-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-mflib-0.0.0b1.tar", last modified: Tue Jan 31 22:31:50 2023, max compression
+gzip compressed data, was "fabrictestbed-mflib-0.1.0b0.tar", last modified: Thu Apr 13 20:11:51 2023, max compression
```

## Comparing `fabrictestbed-mflib-0.0.0b1.tar` & `fabrictestbed-mflib-0.1.0b0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-01-31 22:31:50.677952 fabrictestbed-mflib-0.0.0b1/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1071 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/LICENSE
--rw-rw-r--   0 charles   (1000) charles   (1000)       24 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/MANIFEST.in
--rw-rw-r--   0 charles   (1000) charles   (1000)     3253 2023-01-31 22:31:50.677952 fabrictestbed-mflib-0.0.0b1/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     2791 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-01-31 22:31:50.677952 fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     3253 2023-01-31 22:31:50.000000 fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      354 2023-01-31 22:31:50.000000 fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-01-31 22:31:50.000000 fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       32 2023-01-31 22:31:50.000000 fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-01-31 22:31:50.000000 fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/top_level.txt
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-01-31 22:31:50.677952 fabrictestbed-mflib-0.0.0b1/mflib/
--rw-rw-r--   0 charles   (1000) charles   (1000)       45 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/mflib/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    38998 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/mflib/core.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    30674 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/mflib/mflib.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      345 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/mflib/mflib_version.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    27967 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/mflib/mfvis.py
--rw-rw-r--   0 charles   (1000) charles   (1000)       32 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/requirements.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-01-31 22:31:50.677952 fabrictestbed-mflib-0.0.0b1/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     2031 2023-01-31 22:30:52.000000 fabrictestbed-mflib-0.0.0b1/setup.py
+-rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b0/.gitignore
+-rw-r--r--   0        0        0      145 2023-04-13 19:31:49.113559 fabrictestbed-mflib-0.1.0b0/.pypirc
+-rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-0.1.0b0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b0/LICENSE
+-rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b0/MANIFEST.in
+-rw-r--r--   0        0        0   197138 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/MFLib.pdf
+-rw-r--r--   0        0        0     3730 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/README.md
+-rwxr-xr-x   0        0        0      817 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/create_html_doc.sh
+-rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/create_pdf_doc.sh
+-rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/create_release.sh
+-rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/make.bat
+-rw-r--r--   0        0        0       55 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/requirements.txt
+lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/_static/placeholder
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/_templates/placeholder
+-rw-r--r--   0        0        0     1297 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/source/conf.py
+-rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/core.rst
+-rw-r--r--   0        0        0      262 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/source/index.rst
+-rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/source/mflib.rst
+-rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/mflib/README.md
+-rw-r--r--   0        0        0      539 2023-04-13 19:31:49.113559 fabrictestbed-mflib-0.1.0b0/mflib/__init__.py
+-rw-r--r--   0        0        0    41613 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/mflib/core.py
+-rw-r--r--   0        0        0    11653 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/mflib/mf_timestamp.py
+-rw-r--r--   0        0        0    31859 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/mflib/mflib.py
+-rw-r--r--   0        0        0    27967 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b0/mflib/mfvis.py
+-rw-r--r--   0        0        0      735 2023-04-13 19:34:14.734792 fabrictestbed-mflib-0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b0/requirements.txt
+-rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 fabrictestbed-mflib-0.1.0b0/PKG-INFO
```

### Comparing `fabrictestbed-mflib-0.0.0b1/LICENSE` & `fabrictestbed-mflib-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.0.0b1/PKG-INFO` & `fabrictestbed-mflib-0.1.0b0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,92 @@
-Metadata-Version: 2.1
-Name: fabrictestbed-mflib
-Version: 0.0.0b1
-Summary: FABRIC Measurement Framework Python Client Library
-Home-page: https://github.com/fabric-testbed/mflib
-Author: Carpenter, Song, Pinyi, Hussam
-Author-email: 
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MFLIB Measurement Framework Library
+
+[![Documentation Status](https://readthedocs.org/projects/fabrictestbed-mflib/badge/?version=latest)](https://fabrictestbed-mflib.readthedocs.io/en/latest/?badge=latest)
+
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a FABRIC experimenter's slice. The monitoring system makes extensive use of industry standards such as Prometheus, Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and visualization.
 
 ## Documentation Resources
 For more information about FABRIC vist [fabric-testbed.net](https://fabric-testbed.net/)
 ### Example Jupyter Notebooks
 [FABRIC Jupyter Examples](https://github.com/fabric-testbed/jupyter-examples) GitHub repository contains many examples for using FABRIC from simple slice setup to advanced networking setups. Look for the MFLib section. These notebooks are designed to be easily used on the [FABRIC JupyterHub](https://jupyter.fabric-testbed.net/)
 
 ### FABRIC Learn Site
 [FABRIC Knowledge Base](https://learn.fabric-testbed.net/) 
 
 ### MFLib Python Package Documentation
-See [MFLib.pdf](https://github.com/fabric-testbed/mflib/blob/main/MFLib.pdf) for package documentation.
+Documentation for the package is presented in serveral different forms (and maybe include later in this document):
+* [ReadTheDocs](https://fabrictestbed-mflib.readthedocs.io/en/latest/)
+* [MFLib.pdf](https://github.com/fabric-testbed/mflib/blob/main/MFLib.pdf) in the source code/GitHub.
+* [MFLib HTML Index](https://github.com/fabric-testbed/mflib/blob/main/docs/html/index.html) in the source code/GitHub.
+* Or you may build the documentation from the source code. See Sphinx Documentation later in this document.
 
 ## MFLib Installation
 
-MFLib may be installed using PIP and PyPI [fabrictestbed-mflib](https://pypi.org/fabrictestbed-mflib)
-`pip install --user fabrictestbed-mflib`
+### Instaling via PIP
+MFLib may be installed using PIP and PyPI [fabrictestbed-mflib](https://pypi.org/project/fabrictestbed-mflib/)
+```
+pip install --user fabrictestbed-mflib
+```
 
 ### Installing via Source Code
 If you need a development version, clone the git repo, then use pip to install.
 ```
 git clone https://github.com/fabric-testbed/mflib.git
 cd mflib
 pip install --user .
 ```
 ## Building & Deploying
+
 ### Spinx Documentation
 This package is documented using sphinx. The `source` directories are already created and populated with reStructuredText ( .rst ) files. The `build` directories are deleted and/or are not included in the repository,
 
+API documentation can also be found at https://fabrictestbed-mflib.readthedocs.io/.
+
 #### Build HTML Documents
-The sphinx theme furo is used. This may need to be installed using  
-`pip install furo`   
-To parse the markdown files (README.md) sphinx needs myst-parser.   
-`pip install myst-parser`   
+
+Install the extra packages required to build API docs: (sphinx, furo theme, and myst-parser for parsing markdown files):
+
+```
+pip install -r docs/requirements.txt
+```
+
 Build the documentation by running the following command from the root directory of the repo.
-`sphinx-build -b html docs/source/ docs/build/html`  
+```
+sphinx-build -b html docs/source/ docs/build/html
+```  
 The completed documentation may be accessed by clicking on `/docs/build/html/index.html`
 
 #### Build PDF Document
 Latex must be installed. For Debian use: 
 ```
 sudo apt install texlive-latex-extra 
 sudo apt install latexmk
+
 ```
 Run the bash script to create the MFLIB.pdf documentation. MFLIB.pdf will be placed in the root directory of the repository.
-`./create_pdf_doc.sh`
-#### Building Distribution Package
+```
+./create_pdf_doc.sh
+```
 
+### Distribution Package
+
+MFLib package is created using [Flit](https://flit.pypa.io/en/stable/)
+Be sure to create and commit the PDF documentation to GitHub before building and publishing to PyPi. The MFLib.pdf is included in the distributition.
+```
+python3 -m pip install flit
+```
 To build python package for PyPi run  
-`python setup.py sdist`
+```
+flit build
+```
+
+
 #### Uploading to PyPI
+
 First test the package by uploading to test.pypi.org then test the install.
-`twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
+```
+flit publish --repository testpypi 
+```
 Once install is good, upload to PiPy  
-`twine upload dist/*`
+```
+flit publish --repository pypi 
+```
```

### Comparing `fabrictestbed-mflib-0.0.0b1/fabrictestbed_mflib.egg-info/PKG-INFO` & `fabrictestbed-mflib-0.1.0b0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,106 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-mflib
-Version: 0.0.0b1
-Summary: FABRIC Measurement Framework Python Client Library
-Home-page: https://github.com/fabric-testbed/mflib
-Author: Carpenter, Song, Pinyi, Hussam
-Author-email: 
+Version: 0.1.0b0
+Summary: FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
+Author: Song, Pinyi, Hussam
+Author-email: Carpenter <csacarp0@g.uky.edu>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Project-URL: Homepage, https://github.com/fabric-testbed/mflib
 
 # MFLIB Measurement Framework Library
+
+[![Documentation Status](https://readthedocs.org/projects/fabrictestbed-mflib/badge/?version=latest)](https://fabrictestbed-mflib.readthedocs.io/en/latest/?badge=latest)
+
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a FABRIC experimenter's slice. The monitoring system makes extensive use of industry standards such as Prometheus, Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and visualization.
 
 ## Documentation Resources
 For more information about FABRIC vist [fabric-testbed.net](https://fabric-testbed.net/)
 ### Example Jupyter Notebooks
 [FABRIC Jupyter Examples](https://github.com/fabric-testbed/jupyter-examples) GitHub repository contains many examples for using FABRIC from simple slice setup to advanced networking setups. Look for the MFLib section. These notebooks are designed to be easily used on the [FABRIC JupyterHub](https://jupyter.fabric-testbed.net/)
 
 ### FABRIC Learn Site
 [FABRIC Knowledge Base](https://learn.fabric-testbed.net/) 
 
 ### MFLib Python Package Documentation
-See [MFLib.pdf](https://github.com/fabric-testbed/mflib/blob/main/MFLib.pdf) for package documentation.
+Documentation for the package is presented in serveral different forms (and maybe include later in this document):
+* [ReadTheDocs](https://fabrictestbed-mflib.readthedocs.io/en/latest/)
+* [MFLib.pdf](https://github.com/fabric-testbed/mflib/blob/main/MFLib.pdf) in the source code/GitHub.
+* [MFLib HTML Index](https://github.com/fabric-testbed/mflib/blob/main/docs/html/index.html) in the source code/GitHub.
+* Or you may build the documentation from the source code. See Sphinx Documentation later in this document.
 
 ## MFLib Installation
 
-MFLib may be installed using PIP and PyPI [fabrictestbed-mflib](https://pypi.org/fabrictestbed-mflib)
-`pip install --user fabrictestbed-mflib`
+### Instaling via PIP
+MFLib may be installed using PIP and PyPI [fabrictestbed-mflib](https://pypi.org/project/fabrictestbed-mflib/)
+```
+pip install --user fabrictestbed-mflib
+```
 
 ### Installing via Source Code
 If you need a development version, clone the git repo, then use pip to install.
 ```
 git clone https://github.com/fabric-testbed/mflib.git
 cd mflib
 pip install --user .
 ```
 ## Building & Deploying
+
 ### Spinx Documentation
 This package is documented using sphinx. The `source` directories are already created and populated with reStructuredText ( .rst ) files. The `build` directories are deleted and/or are not included in the repository,
 
+API documentation can also be found at https://fabrictestbed-mflib.readthedocs.io/.
+
 #### Build HTML Documents
-The sphinx theme furo is used. This may need to be installed using  
-`pip install furo`   
-To parse the markdown files (README.md) sphinx needs myst-parser.   
-`pip install myst-parser`   
+
+Install the extra packages required to build API docs: (sphinx, furo theme, and myst-parser for parsing markdown files):
+
+```
+pip install -r docs/requirements.txt
+```
+
 Build the documentation by running the following command from the root directory of the repo.
-`sphinx-build -b html docs/source/ docs/build/html`  
+```
+sphinx-build -b html docs/source/ docs/build/html
+```  
 The completed documentation may be accessed by clicking on `/docs/build/html/index.html`
 
 #### Build PDF Document
 Latex must be installed. For Debian use: 
 ```
 sudo apt install texlive-latex-extra 
 sudo apt install latexmk
+
 ```
 Run the bash script to create the MFLIB.pdf documentation. MFLIB.pdf will be placed in the root directory of the repository.
-`./create_pdf_doc.sh`
-#### Building Distribution Package
+```
+./create_pdf_doc.sh
+```
+
+### Distribution Package
 
+MFLib package is created using [Flit](https://flit.pypa.io/en/stable/)
+Be sure to create and commit the PDF documentation to GitHub before building and publishing to PyPi. The MFLib.pdf is included in the distributition.
+```
+python3 -m pip install flit
+```
 To build python package for PyPi run  
-`python setup.py sdist`
+```
+flit build
+```
+
+
 #### Uploading to PyPI
+
 First test the package by uploading to test.pypi.org then test the install.
-`twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
+```
+flit publish --repository testpypi 
+```
 Once install is good, upload to PiPy  
-`twine upload dist/*`
+```
+flit publish --repository pypi 
+```
+
```

### Comparing `fabrictestbed-mflib-0.0.0b1/mflib/core.py` & `fabrictestbed-mflib-0.1.0b0/mflib/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,30 +23,32 @@
 
 
 import json
 import traceback
 import os
 
 from fabrictestbed_extensions.fablib.fablib import fablib
+
 # For getting vars to make tunnel
 from fabrictestbed_extensions.fablib.fablib import FablibManager
 
 
 import string
 import random
 
 import logging
 
-class Core():
+
+class Core:
     """
     MFLib core contains the core methods needed to create and interact with the Measurement Framework installed in a slice.
     It is not intended to be used by itself, but rather, it is the base object for creating Measurement Framework Library objects.
     """
 
-    core_class_version = "1.0.30"
+    core_class_version = "1.0.36"
 
     """
     An updatable version for debugging purposes to make sure the correct version of this file is being used. Anyone can update this value as they see fit.
     Should always be increasing.
 
     Returns:
         String: Version.sub-version.build
@@ -56,18 +58,21 @@
         """
         Sets up the core logging file.
         Note that the self.logging_filename will be set with the slice name when the slice is set.
         Args:
         filename (_type_, optional): _description_. Defaults to None.
         """
         self.core_logger = logging.getLogger(__name__)
-        self.core_logger.propagate = False # needed?
+        self.core_logger.propagate = False  # needed?
         self.core_logger.setLevel(self.log_level)
-        
-        formatter = logging.Formatter('%(asctime)s %(name)-8s %(levelname)-8s %(message)s', datefmt='%m/%d/%Y %H:%M:%S %p')
+
+        formatter = logging.Formatter(
+            "%(asctime)s %(name)-8s %(levelname)-8s %(message)s",
+            datefmt="%m/%d/%Y %H:%M:%S %p",
+        )
 
         # Make sure log directory exists
         if not os.path.exists(self.log_directory):
             os.makedirs(self.log_directory)
 
         file_handler = logging.FileHandler(self.log_filename)
         file_handler.setLevel(self.log_level)
@@ -79,46 +84,44 @@
     def slice_name(self):
         """
         Returns the name of the slice associated with this object.
 
         Returns:
             String: The name of the slice.
         """
-        return self._slice_name 
+        return self._slice_name
 
     @slice_name.setter
-    def slice_name( self, value ):
+    def slice_name(self, value):
         """
         Sets the name of the slice associated with this object. Also creates the directories used to store local informations for mflib about the slice.
         Generally should not be called directly. It is called when the slice is set.
         Args:
             value (str): Name of the slice
         """
         # Set the slice name
-        self._slice_name = value 
+        self._slice_name = value
 
         # Create the local slice directory
         try:
             os.makedirs(self.local_slice_directory)
             os.makedirs(self.log_directory)
-           
+
         except FileExistsError:
-            pass 
+            pass
             # Don't care if the file already exists.
 
-
         self.log_filename = os.path.join(self.log_directory, "mflib.log")
 
         self.set_core_logger()
 
         self.core_logger.info(f"Using core_class_version {self.core_class_version}")
-        #self.core_logger.basicConfig(filename=self.log_filename, format='%(asctime)s %(name)-8s %(levelname)-8s %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p', level="INFO", force=True)
+        # self.core_logger.basicConfig(filename=self.log_filename, format='%(asctime)s %(name)-8s %(levelname)-8s %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p', level="INFO", force=True)
         self.core_logger.info(f"-----Set slice name {value}.-----")
 
-
     @property
     def local_slice_directory(self):
         """
         The directory where local files associated with the slice are stored.
 
         Returns:
             str: The directory where local files associated files are stored.
@@ -130,528 +133,573 @@
         """
         The full path for the log directory.
 
         Returns:
             String: The full path to the log directory.
         """
         return os.path.join(self.local_slice_directory, "log")
-        
-    @property 
+
+    @property
     def bootstrap_status_file(self):
         """
         The full path to the local copy of the bootstrap status file.
 
         Returns:
             String: The full path tp the local copy of the bootsrap status file.
         """
         return os.path.join(self.local_slice_directory, "bootstrap_status.json")
 
-    @property 
+    @property
     def common_hosts_file(self):
         """
-        The full path to a local copy of the hosts.ini file. 
+        The full path to a local copy of the hosts.ini file.
 
         Returns:
             String: The full path to a local copy of the hosts.ini file.
         """
-        return os.path.join(self.local_slice_directory, "hosts.ini")    
+        return os.path.join(self.local_slice_directory, "hosts.ini")
 
-    @property 
+    @property
     def local_mfuser_private_key_filename(self):
         """
         The local copy of the private ssh key for the mfuser account.
 
         Returns:
             String: The local copy of the private ssh key for the mfuser account.
         """
-        return os.path.join(self.local_slice_directory, "mfuser_private_key")    
+        return os.path.join(self.local_slice_directory, "mfuser_private_key")
 
-    @property 
+    @property
     def local_mfuser_public_key_filename(self):
         """
         The local copy of the public ssh key for the mfuser account.
 
         Returns:
             String: The local copy of the public ssh key for the mfuser account.
         """
-        return os.path.join(self.local_slice_directory, "mfuser_pubic_key")    
+        return os.path.join(self.local_slice_directory, "mfuser_pubic_key")
 
     @property
     def meas_node(self):
         """
         The fablib node object for the Measurement Node in the slice.
 
         Returns:
             fablib.node: The fablib node object for the Measurement Node in the slice.
 
         """
         if self._meas_node:
-            return self._meas_node 
+            return self._meas_node
         else:
             self._find_meas_node()
-            return self._meas_node 
-            
+            return self._meas_node
+
     @property
     def meas_node_ip(self):
         """
         The management ip address for the Measurement Node
 
         Returns:
             String: ip address
         """
         if self.meas_node:
-            return self._meas_node.get_management_ip() 
+            return self._meas_node.get_management_ip()
         else:
             return ""
 
     @property
     def slice_username(self):
         """
         The default username for the Measurement Node for the slice.
 
         Returns:
             String: username
         """
         if self.meas_node:
-            return self._meas_node.get_username() 
+            return self._meas_node.get_username()
         else:
             return ""
 
-
     # Tunnels are needed to access the meas node via the bastion host
     # In the future these may be combinded into one port with diff nginx paths mappings.
-    # alt copy is a selection added to the fabric_rc file for setting a alertnate location for the files 
+    # alt copy is a selection added to the fabric_rc file for setting a alertnate location for the files
     #   such as on a laptop. This makes it easy to create a tunnel on a users laptop where they will need access
-    #   to the web uis. 
+    #   to the web uis.
 
     @property
     def tunnel_host(self):
         """
         If a tunnel is used, this value must be set for the localhost, Otherwise it is set to empty string.
 
         Returns:
             String: tunnel hostname
         """
         return self._tunnel_host
-        
+
     @tunnel_host.setter
     def tunnel_host(self, value):
-        """ 
+        """
         Set to "localhost" if using tunnnel.
         """
         self._tunnel_host = value
-        
 
     @property
     def grafana_tunnel_local_port(self):
         """
         If a tunnel is used for grafana, this value must be set for the port.
-          Returns: 
+          Returns:
             String: port number
         """
         return self._grafana_tunnel_local_port
-        
+
     @grafana_tunnel_local_port.setter
     def grafana_tunnel_local_port(self, value):
-        """ 
+        """
         Set to port_number if using tunnnel for grafana.
         """
         self._grafana_tunnel_local_port = value
 
-
     @property
     def kibana_tunnel_local_port(self):
         """
         If a tunnel is used for Kibana, this value must be set for the port"""
         return self._kibana_tunnel_local_port
-        
+
     @kibana_tunnel_local_port.setter
     def kibana_tunnel_local_port(self, value):
-        """ 
+        """
         Set to port_number if using tunnnel for Kibana.
         """
         self._kibana_tunnel_local_port = value
-                
+
     @property
     def grafana_tunnel(self):
         """
         Returns the command for createing an SSH tunnel for accesing Grafana.
 
         Returns:
             String: ssh command
         """
-        return self._meas_node_ssh_tunnel(local_port = self.grafana_tunnel_local_port, remote_port="443")
+        return self._meas_node_ssh_tunnel(
+            local_port=self.grafana_tunnel_local_port, remote_port="443"
+        )
 
     @property
     def kibana_tunnel(self):
         """
         Returns the command for createing an SSH tunnel for accesing Kibana.
 
         Returns:
             String: ssh command
         """
-        return self._meas_node_ssh_tunnel(local_port = self.kibana_tunnel_local_port, remote_port="80")
+        return self._meas_node_ssh_tunnel(
+            local_port=self.kibana_tunnel_local_port, remote_port="80"
+        )
 
     def _meas_node_ssh_tunnel(self, local_port, remote_port):
         """
         Creates the ssh tunnel command for accessing the Measurement Node using the given local and remote ports.
 
         Args:
             local_port (String): local port ie port on users machine
             remote_port (String): remote port ie port on Measurement Node
 
         Returns:
             String : SSH command string or error string.
         """
         slice_username = self.slice_username
         meas_node_ip = self.meas_node_ip
-        
+
         # User has setup an ssh config file
         extra_fm = FablibManager()
         errmsg = ""
         ssh_config = ""
         private_key_file = ""
-    
+
         extra_fm_vars = extra_fm.read_fabric_rc(extra_fm.default_fabric_rc)
         if extra_fm_vars:
             if "FABRIC_ALT_COPY_SSH_CONFIG" in extra_fm_vars:
                 ssh_config = extra_fm_vars["FABRIC_ALT_COPY_SSH_CONFIG"]
             else:
                 errmsg += "FABRIC_ALT_COPY_SSH_CONFIG not found in fabric_rc file. "
 
             if "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE" in extra_fm_vars:
-                private_key_file = extra_fm_vars["FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE"]
+                private_key_file = extra_fm_vars[
+                    "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE"
+                ]
             else:
                 errmsg += "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE not found in fabric_rc file. "
-            
+
         if errmsg:
-            self.core_logger.error(f"It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. {errmsg} ") 
-            return "It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. " + errmsg
+            self.core_logger.error(
+                f"It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. {errmsg} "
+            )
+            return (
+                "It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. "
+                + errmsg
+            )
         else:
-            #return f'ssh -L 10010:localhost:443 -F {extra_fm_vars["FABRIC_ALT_SSH_CONFIG"]} -i {extra_fm_vars["FABRIC_ALT_SLICE_PRIVATE_KEY_FILE"]} {self.slice_username}@{self.meas_node_ip}'
-            tunnel_cmd = f'ssh -L {local_port}:localhost:{remote_port} -F {ssh_config} -i {private_key_file} {slice_username}@{meas_node_ip}'
-            return tunnel_cmd 
-
+            # return f'ssh -L 10010:localhost:443 -F {extra_fm_vars["FABRIC_ALT_SSH_CONFIG"]} -i {extra_fm_vars["FABRIC_ALT_SLICE_PRIVATE_KEY_FILE"]} {self.slice_username}@{self.meas_node_ip}'
+            tunnel_cmd = f"ssh -L {local_port}:localhost:{remote_port} -F {ssh_config} -i {private_key_file} {slice_username}@{meas_node_ip}"
+            return tunnel_cmd
 
-
-
-
-    # Repo branch made class varible so it can be set before creating object
-    mf_repo_branch = "main"
     """
     The git branch to be used for cloning the MeasurementFramework branch to the Measusrement Node.
     """
 
-  
-    def __init__(self, local_storage_directory="/tmp/mflib"):
+    def __init__(
+        self,
+        local_storage_directory="/tmp/mflib",
+        mf_repo_branch="main",
+        logging_level=logging.DEBUG,
+    ):
         """
         Core constructor
 
         Args:
             local_storage_directory (str, optional): Directory where local data will be stored. Defaults to "/tmp/mflib".
+            mf_repo_branch (str, optional): git branch name to pull MeasurementFranework code from. Defaults to "main".
         """
-        #super().__init__()
+        # super().__init__()
 
         try:
             self.local_storage_directory = local_storage_directory
             os.makedirs(self.local_storage_directory)
         except FileExistsError:
             pass
 
         # The slice_name
         self._slice_name = ""
+        self.mf_repo_branch = mf_repo_branch
 
         self.core_logger = None
-        self.log_level = logging.INFO
+        self.log_level = logging_level
         self.log_filename = os.path.join(self.log_directory, "mflib_core.log")
         self.set_core_logger()
         self.core_logger.info("Creating mflib object.")
-        
+
         self.tunnel_host = "localhost"
         self.grafana_tunnel_local_port = "10010"
         self.kibana_tunnel_local_port = "10020"
 
-
         # The slice object
         self.slice = None
         # The meas_node object
-        self._meas_node = None 
+        self._meas_node = None
 
         # The following are normally constant values
         # Name given to the meas node
         self.measurement_node_name = "_meas_node"
         # Services directory on meas node
         self.services_directory = os.path.join("/", "home", "mfuser", "services")
         # Base names for keys
         self.mfuser_private_key_filename = "mfuser_private_key"
         self.mfuser_public_key_filename = "mfuser_public_key"
 
-          
-# User Methods 
+    # User Methods
     def create(self, service, data=None, files=[]):
         """
-        Creates a new service for the slice. 
-        :param service: The name of the service.
-        :type service: String
-        :param data: Data to be passed to a JSON file place in the service's meas node directory.
-        :type data: JSON serializable object.
-        :param files: List of filepaths to be uploaded.
-        :type files: List of Strings
+        Creates a new service for the slice.
+
+        Args:
+            service(String): The name of the service.
+            data (JSON serializable object) Data to be passed to a JSON file place in the service's meas node directory.
+            files (List of Strings): List of filepaths to be uploaded.
+        Returns:
+            dict: Dictionary of creation results.
         """
         self.core_logger.info(f"Run create for {service}")
         self.core_logger.debug(f"Data is {data}.")
         return self._run_on_meas_node(service, "create", data, files)
 
     def update(self, service, data=None, files=[]):
         """
         Updates an existing service for the slice.
-        :param service: The name of the service.
-        :type service: String
-        :param data: Data to be passed to a JSON file place in the service's meas node directory.
-        :type data: JSON serializable object.
-        :param files: List of filepaths to be uploaded.
-        :type files: List of Strings
+
+        Args:
+            service (String): The name of the service.
+            data (JSON Serializable Object): Data to be passed to a JSON file place in the service's meas node directory.
+            files (List of Strings): List of filepaths to be uploaded.
+
+        Returns:
+            dict: Dictionary of update results.
         """
+
         self.core_logger.info(f"Run update for {service}")
         self.core_logger.debug(f"Data is {data}.")
         return self._run_on_meas_node(service, "update", data, files)
 
     def info(self, service, data=None):
         """
         Gets inormation from an existing service. Strictly gets information, does not change how the service is running.
-        :param service: The name of the service.
-        :type service: String
-        :param data: Data to be passed to a JSON file place in the service's meas node directory.
-        :type data: JSON serializable object.
+
+        Args:
+            service (String): The name of the service.
+            data (JSON Serializable Object): Data to be passed to a JSON file place in the service's meas node directory.
+        Returns:
+            dict: Dictionary of info results.
         """
         self.core_logger.info(f"Run info for {service}")
         self.core_logger.debug(f"Data is {data}.")
         return self._run_on_meas_node(service, "info", data)
 
     def start(self, services=[]):
         """
         Restarts a stopped service using existing configs on meas node.
+
+        Args:
+            services (List of Strings): The name of the services to be restarted.
+        Returns:
+            List: List of start result dictionaries.
         """
+        ret_val = []
         for service in services:
             self.core_logger.info(f"Run start for {service}")
-            return self._run_on_meas_node(service, "start")
+            ret_val.append(
+                {
+                    "service": service,
+                    "results": self._run_on_meas_node(service, "start"),
+                }
+            )
+        return ret_val
 
     def stop(self, services=[]):
         """
         Stops a service, does not remove the service, just stops it from using resources.
+
+        Args:
+            services (List of Strings): The names of the services to be stopped.
+        Returns:
+            List: List of stop result dictionaries.
         """
+        ret_val = []
         for service in services:
             self.core_logger.info(f"Run stop for {service}")
-            return self._run_on_meas_node(service, "stop")
-
-    # def status(self, services=[]):
-    #     """
-    #     Deprecated?, use info instead?
-    #     Returns predefined status info. Does not change the running of the service.
-    #     """ 
-    #     for service in services:
-    #         return self._run_on_meas_node(service, "status")
+            ret_val.append(
+                {"service": service, "results": self._run_on_meas_node(service, "stop")}
+            )
+        return ret_val
 
     def remove(self, services=[]):
         """
         Stops a service running and removes anything setup on the experiment's nodes. Service will then need to be re-created using the create command before service can be started again.
+
+        Args:
+            services (List of Strings): The names of the services to be removed.
+        Returns:
+            List: List of remove result dictionaries.
         """
+
+        ret_val = []
         for service in services:
             self.core_logger.info(f"Run remove for {service}")
-            return self._run_on_meas_node(service, "remove")
-
+            ret_val.append(
+                {
+                    "service": service,
+                    "results": self._run_on_meas_node(service, "remove"),
+                }
+            )
 
-
-# Utility Methods
+    # Utility Methods
 
     def _upload_mfuser_keys(self, private_filename=None, public_filename=None):
         """
         Uploads the mfuser keys to the default user for easy access later.
+
         """
-        if  private_filename is None:
-            private_filename=self.local_mfuser_private_key_filename
-        if  public_filename is None:
-            public_filename=self.local_mfuser_public_key_filename
+        if private_filename is None:
+            private_filename = self.local_mfuser_private_key_filename
+        if public_filename is None:
+            public_filename = self.local_mfuser_public_key_filename
 
         try:
             local_file_path = private_filename
             remote_file_path = self.mfuser_private_key_filename
-            fa = self.meas_node.upload_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
+            fa = self.meas_node.upload_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
 
         except TypeError:
-            pass 
+            pass
             # TODO set file permissions on remote
             # This error is happening due to the file permmissions not being correctly set on the remote?
         except Exception as e:
             print(f"Failed Private Key Upload: {e}")
-            self.core_logger.exception("Failed to upload mfuser private key to default user.")
+            self.core_logger.exception(
+                "Failed to upload mfuser private key to default user."
+            )
 
         try:
             local_file_path = public_filename
             remote_file_path = self.mfuser_public_key_filename
-            fa = self.meas_node.upload_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
+            fa = self.meas_node.upload_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
         except TypeError:
-            pass 
-            self.core_logger.exception("Failed to upload mfuser public key to default user.")
+            pass
+            self.core_logger.exception(
+                "Failed to upload mfuser public key to default user."
+            )
             # TODO set file permissions on remote
-            # This error is happening due to the file permmissions not being correctly set on the remote?   
+            # This error is happening due to the file permmissions not being correctly set on the remote?
             # Errors are:
             # Failed Private Key Upload: cannot unpack non-iterable SFTPAttributes object
-            # Failed Public Key Upload: cannot unpack non-iterable SFTPAttributes object     
+            # Failed Public Key Upload: cannot unpack non-iterable SFTPAttributes object
         except Exception as e:
             print(f"Failed Public Key Upload: {e}")
             self.core_logger.exception("Failed to upload mfuser keys to default user.")
 
-
-        # Set the permissions correctly on the remote machine.
-        cmd = f"chmod 644 {self.mfuser_public_key_filename}"
-        self.meas_node.execute(cmd)
-        cmd = f"chmod 600 {self.mfuser_private_key_filename}"
-        self.meas_node.execute(cmd)
-        
     def _copy_mfuser_keys_to_mfuser_on_meas_node(self):
         """
         Copies mfuser keys from default location to mfuser .ssh folder and sets ownership & permissions.
         """
         try:
-            cmd = f"sudo cp {self.mfuser_public_key_filename} /home/mfuser/.ssh/{self.mfuser_public_key_filename}; sudo chown mfuser:mfuser /home/mfuser/.ssh/{self.mfuser_public_key_filename}; sudo chmod 644 /home/mfuser/.ssh/{self.mfuser_public_key_filename}"
-            stdout, stderr = self.meas_node.execute(cmd)
-        
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
-
-            cmd = f"sudo cp {self.mfuser_private_key_filename} /home/mfuser/.ssh/{self.mfuser_private_key_filename}; sudo chown mfuser:mfuser /home/mfuser/.ssh/{self.mfuser_private_key_filename}; sudo chmod 600 /home/mfuser/.ssh/{self.mfuser_private_key_filename}"
+            cmd = (
+                f"sudo cp {self.mfuser_public_key_filename} /home/mfuser/.ssh/{self.mfuser_public_key_filename};"
+                f"sudo cp {self.mfuser_private_key_filename} /home/mfuser/.ssh/{self.mfuser_private_key_filename};"
+                f"sudo chmod 644 /home/mfuser/.ssh/{self.mfuser_public_key_filename};"
+                f"sudo chmod 600 /home/mfuser/.ssh/{self.mfuser_private_key_filename};"
+                f"sudo chown -R mfuser:mfuser /home/mfuser/.ssh;"
+            )
             stdout, stderr = self.meas_node.execute(cmd)
-
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
+            if stdout:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr:
+                self.core_logger.debug(f"STDERR: {stderr}")
 
         except Exception as e:
             print(f"Failed mfuser key user key copy: {e}")
             self.core_logger.exception("Failed to copy mfuser keys to meas node.")
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
-            return False 
+            if stdout:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr:
+                self.core_logger.debug(f"STDERR: {stderr}")
+            return False
         return True
 
-
     def _download_mfuser_keys(self, private_filename=None, public_filename=None):
         """
         Downloads the mfuser keys.
         """
-        if  private_filename is None:
-            private_filename=self.local_mfuser_private_key_filename
-        if  public_filename is None:
-            public_filename=self.local_mfuser_public_key_filename
-        
+        if private_filename is None:
+            private_filename = self.local_mfuser_private_key_filename
+        if public_filename is None:
+            public_filename = self.local_mfuser_public_key_filename
 
         try:
             local_file_path = private_filename
             remote_file_path = self.mfuser_private_key_filename
-            stdout, stderr = self.meas_node.download_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
+            stdout, stderr = self.meas_node.download_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
 
             local_file_path = public_filename
             remote_file_path = self.mfuser_public_key_filename
-            stdout, stderr = self.meas_node.download_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
-            
+            stdout, stderr = self.meas_node.download_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
+
         except Exception as e:
             print(f"Download mfuser Keys Failed: {e}")
             self.core_logger.exception("Failed to download mfuser keys.")
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
-
+            if stdout:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr:
+                self.core_logger.debug(f"STDERR: {stderr}")
 
     def _find_meas_node(self):
         """
         Finds the node named "meas" in the slice and sets the value for class's meas_node
-        :return: If node found, sets self.meas_node and returns True. If node not found, clears self.meas_node and returns False.
-        :rtype: Boolean
+
+        Returns:
+        Boolean: If node found, sets self.meas_node and returns True. If node not found, clears self.meas_node and returns False.
         """
         try:
             for node in self.slice.get_nodes():
                 if node.get_name() == self.measurement_node_name:
-                    self._meas_node = node 
-                    return True 
+                    self._meas_node = node
+                    return True
         except Exception as e:
             print(f"Find Measure Node Failed: {e}")
             self.core_logger.exception("Failed to find Measure Node")
         self._meas_node = None
         return False
 
-        
     def _run_on_meas_node(self, service, command, data=None, files=[]):
         """
-        Runs a command on the meas node.
-        :param service: The name of the service.
-        :type service: String
-        :param command: The name of the command to run.
-        :type command: String
-        :param data: Data to be passed to a JSON file place in the service's meas node directory.
-        :type data: JSON serializable object.
-        :param files: List of filepaths to be uploaded.
-        :type files: List of Strings
-        :return: The stdout & stderr values from running the command ? Reformat to dict??
-        :rtype: String ? dict??
+        Runs one of the commands available for the service on the meas node. Commands are create, update, info, start, stop, remove
+
+        Args:
+            service(String): The name of the service.
+            command(String): The name of the command to run.
+            data(JSON Serializable Object): Data to be passed to a JSON file place in the service's meas node directory.
+            files(List of Strings): List of filepaths to be uploaded.
+
+        Returns:
+           Dictionary: The stdout & stderr values from running the command formated in dictionary.
         """
-        # upload resources 
+        # upload resources
         if data:
             self._upload_service_data(service, data)
         else:
             # Ensure old stale data is remove on meas node
             self._upload_service_data(service, {})
         if files:
             self._upload_service_files(service, files)
 
-        # run command 
-        return self._run_service_command(service, command )
+        # run command
+        return self._run_service_command(service, command)
 
-        
     def _upload_service_data(self, service, data):
         """
         Uploads the json serializable object data to a json file on the meas node.
-        :param service: The service to which the data belongs.
-        :type service: String
-        :param data: A JSON serializable dictionary 
-        :type data: dict
+
+        Args:
+            service(String): The service to which the data belongs.
+        :   data(Object): A JSON Serializable Object
         """
-        
-            
+
         letters = string.ascii_letters
         try:
             # Create temp file for serialized json data
-            randdataname = "mf_service_data_" + "".join(random.choice(letters) for i in range(10))
+            randdataname = "mf_service_data_" + "".join(
+                random.choice(letters) for i in range(10)
+            )
             local_file_path = os.path.join("/tmp", randdataname)
-            with open(local_file_path, 'w') as datafile:
-                #print("dumping data")
+            with open(local_file_path, "w") as datafile:
+                # print("dumping data")
                 json.dump(data, datafile)
-            
+
             # Create remote filenames
-            final_remote_file_path = os.path.join(self.services_directory, service, "data", "data.json")
+            final_remote_file_path = os.path.join(
+                self.services_directory, service, "data", "data.json"
+            )
             remote_tmp_file_path = os.path.join("/tmp", randdataname)
-    
+
             # upload file
             fa = self.meas_node.upload_file(local_file_path, remote_tmp_file_path)
-            
+
             # mv file to final location
             cmd = f"sudo mv {remote_tmp_file_path} {final_remote_file_path};  sudo chown mfuser:mfuser {final_remote_file_path}"
-            
+
             stdout, stderr = self.meas_node.execute(cmd)
-            
+
             # Remove local temp file.
             os.remove(local_file_path)
-            
+
         except Exception as e:
-            print(f"Service Data Upload Failed: {e}")  
+            print(f"Service Data Upload Failed: {e}")
             self.core_logger.exception("Upload service data failed")
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
+            if stdout:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr:
+                self.core_logger.debug(f"STDERR: {stderr}")
             return False
         return True
 
-
     def _upload_service_files(self, service, files):
         """
         Uploads the given local files to the given service's directory on the meas node.
         :param service: Service name for which the files are being upload to the meas node.
         :type service: String
         :param files: List of file paths on local machine.
         :type files: List
@@ -662,319 +710,384 @@
         letters = string.ascii_letters
 
         # TODO could add option to upload a directory of files using fablib.upload_directory
         try:
             for file in files:
                 # Set src/dst filenames
                 # file is local path
-                local_file_path = file 
+                local_file_path = file
                 filename = os.path.basename(file)
-                final_remote_file_path = os.path.join(self.services_directory, service, "files", filename)
-
-                randfilename = "mf_file_" + "".join(random.choice(letters) for i in range(10))
+                final_remote_file_path = os.path.join(
+                    self.services_directory, service, "files", filename
+                )
+
+                randfilename = "mf_file_" + "".join(
+                    random.choice(letters) for i in range(10)
+                )
                 remote_tmp_file_path = os.path.join("/tmp", randfilename)
-                
+
                 # upload file
-                fa = self.meas_node.upload_file(local_file_path, remote_tmp_file_path) # retry=3, retry_interval=10, username="mfuser", private_key="mfuser_private_key")
-                cmd = f"sudo mv {remote_tmp_file_path} {final_remote_file_path};  sudo chown mfuser:mfuser {final_remote_file_path}; sudo rm {remote_tmp_file_path}"
- 
+                fa = self.meas_node.upload_file(
+                    local_file_path, remote_tmp_file_path
+                )  # retry=3, retry_interval=10, username="mfuser", private_key="mfuser_private_key")
+                cmd = f"sudo mv {remote_tmp_file_path} {final_remote_file_path};  sudo chown mfuser:mfuser {final_remote_file_path};"
+
                 stdout, stderr = self.meas_node.execute(cmd)
 
         except Exception as e:
             print(f"Service File Upload Failed: {e}")
             self.core_logger.exception("Upload service files failed")
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
+            if stdout:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr:
+                self.core_logger.debug(f"STDERR: {stderr}")
             return False
         return True
 
-
-    def _run_service_command( self, service, command ):
+    def _run_service_command(self, service, command):
         """
-        Runs the given comand for the given service on the meas node. 
-        :param service: Service name for which the command is being run on the meas node.
-        :type service: String
-        :param files: Command name.
-        :type files: String
+        Runs the given comand for the given service on the meas node.
+
+        Args:
+            service(String): Service name for which the command is being run on the meas node.
+        :   files(List of ): Command name.
+
         :raises: Exception: for misc failures....
-        :return: Resulting output? JSON output or dictionary?
-        :rtype: ?
+        Returns:
+            Dictionary: Resulting output of comand JSON converted to dictionary.
+
         """
 
         try:
             full_command = f"sudo -u mfuser python3 {self.services_directory}/{service}/{command}.py"
-            stdout, stderr = self.meas_node.execute(full_command) #retry=3, retry_interval=10, username="mfuser", private_key="mfuser_private_key"
-            self.core_logger.info(f"STDOUT: {stdout}")
+            stdout, stderr = self.meas_node.execute(
+                full_command, quiet=True
+            )  # retry=3, retry_interval=10, username="mfuser", private_key="mfuser_private_key"
+            self.core_logger.debug(f"STDOUT: {json.dumps(stdout, indent=2)}")
+        except ValueError as e:
+            self.core_logger.debug(f"STDOUT: {stdout}")
         except Exception as e:
             print(f"Service Commnad Run Failed: {e}")
-#         print(type(stdout))
-#         print(stdout)
-#         print(stderr)
+        #         print(type(stdout))
+        #         print(stdout)
+        #         print(stderr)
         try:
             # Convert the json string to a dict
             jsonstr = stdout
             # remove non json string
-            jsonstr = jsonstr[ jsonstr.find('{'):jsonstr.rfind('}')+1]
+            jsonstr = jsonstr[jsonstr.find("{") : jsonstr.rfind("}") + 1]
             # Need to "undo" what the exceute command did
-            jsonstr = jsonstr.replace('\n','\\n')
-            #print(jsonstr)
+            jsonstr = jsonstr.replace("\n", "\\n")
+            # print(jsonstr)
             ret_data = json.loads(jsonstr)
             return ret_data
             # TODO add stderr to return value?
         except Exception as e:
             print("Unable to convert returned comand json.")
+            # TODO create dictionary with malformed data.
             print("STDOUT: ")
             print(stdout)
             print("STDERR: ")
             print(stderr)
             print(f"Fail: {e}")
 
             self.core_logger.exception("Unable to convert returned comand json.")
-            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
-
-        return {} #(stdout, stderr)
+            if stdout:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr:
+                self.core_logger.debug(f"STDERR: {stderr}")
 
+        return {}
 
     def _download_service_file(self, service, filename, local_file_path=""):
         """
         Downloads service files from the meas node and places them in the local storage directory.
         :param service: Service name
         :type service: String
         :param filename: The filename to download from the meas node.
         :param local_file_path: Optional filename for local saved file. If not given, file will be in default slice directory.# Fri Sep 09 2022 14:30
         :type local_file_path: String
         """
 
         if not local_file_path:
-            local_file_path = os.path.join(self.local_slice_directory, service, filename)
+            local_file_path = os.path.join(
+                self.local_slice_directory, service, filename
+            )
             # ensure local directory exists
-            local_dir_path = os.path.dirname(local_file_path) 
+            local_dir_path = os.path.dirname(local_file_path)
             if not os.path.exists(local_dir_path):
                 os.makedirs(local_dir_path)
 
-        # 
+        #
         #  Download a file from a service directory
         # Probably most useful for grabbing output from a command run.
         # TODO figure out how to name/where to put file locally
         try:
-            #local_file_path = os.path.join(self.local_slice_directory, service, filename)
+            # local_file_path = os.path.join(self.local_slice_directory, service, filename)
             remote_file_path = os.path.join(self.services_directory, service, filename)
-            file_attributes = self.meas_node.download_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
-            return {"success":True, "filename":local_file_path}
+            file_attributes = self.meas_node.download_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
+            return {"success": True, "filename": local_file_path}
         except Exception as e:
             print(f"Download service file Fail: {e}")
             self.core_logger.exception()
-            return {"success":False}
-        
-        
+            return {"success": False}
+
     def _clone_mf_repo(self):
         """
-        Clone the repo to the mfuser on the meas node.|
+        Clones the MeasurementFramework  git repository to /home/mfuser/mf_git on the meas node.
         """
-        cmd = f"sudo -u mfuser git clone -b {self.mf_repo_branch} https://github.com/fabric-testbed/MeasurementFramework.git /home/mfuser/mf_git"
-        stdout, stderr = self.meas_node.execute(cmd)
-        self.core_logger.info(f"Cloned MeasurementFramework branch '{self.mf_repo_branch}' to measure node.")
-        if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-        if stderr: self.core_logger.debug(f"STDERR: {stderr}")
-        
+        msg = f"Cloning Measurement Framework Repository from github.com..."
+        self.core_logger.debug(msg)
+        print(msg)
+
+        cmd = f"sudo -u mfuser git clone -q -b {self.mf_repo_branch} https://github.com/fabric-testbed/MeasurementFramework.git /home/mfuser/mf_git"
+        stdout, stderr = self.meas_node.execute(cmd, quiet=True)
+
+        msg = f"Cloning Measurement Framework Repository from github.com done."
+        self.core_logger.debug(msg)
+        print(msg)
+
+
+        if stdout:
+            self.core_logger.debug(f"STDOUT: {stdout}")
+        if stderr:
+            if "already exists and is not an empty directory" not in stderr:
+                msg = (
+                    f"Cloning Measurement Framework Repository from github.com Failed."
+                )
+                self.core_logger.error(msg)
+                self.core_logger.error(f"STDERR: {stderr}")
+                return False
+        return True
+
     def _run_bootstrap_script(self):
         """
         Run the initial bootstrap script in the meas node mf repo.
         """
-        cmd = f'sudo -u mfuser /home/mfuser/mf_git/instrumentize/experiment_bootstrap/bootstrap.sh'
-        stdout, stderr = self.meas_node.execute(cmd)
-        
-        self.core_logger.info(f"bootstrap bash script ran on measure node.")
-        self.core_logger.info(f"STDOUT: {stdout}")
-        if stderr: self.core_logger.info(f"STDERR: {stderr}")
-
-        print("Bootstrap script done")
+        msg = f"Starting Bootstrap Process on Measure Node (bash script)..."
+        self.core_logger.debug(msg)
+        print(msg)
+
+        cmd = f"sudo -u mfuser /home/mfuser/mf_git/instrumentize/experiment_bootstrap/bootstrap.sh"
+
+        stdout, stderr = self.meas_node.execute(cmd, quiet=True)
+
+        msg = f"Bootstrap Process on Measure Node (bash script) done."
+        self.core_logger.debug(msg)
+        print(msg)
+
+        if stdout:
+            self.core_logger.debug(f"STDOUT: {stdout}")
+        if stderr:
+            self.core_logger.info(f"STDERR: {stderr}")
 
     def _run_bootstrap_ansible(self):
         """
         Run the initial bootstrap ansible scripts in the meas node mf repo.
         """
-        cmd = f'sudo -u mfuser python3 /home/mfuser/mf_git/instrumentize/experiment_bootstrap/bootstrap_playbooks.py'
-        stdout, stderr = self.meas_node.execute(cmd)
-        
-        self.core_logger.info(f"bootstrap ansible script ran on measure node.")
-        self.core_logger.info(f"STDOUT: {stdout}")
-        if stderr: self.core_logger.info(f"STDERR: {stderr}")
-
+        msg = f"Starting Bootstrap Process on Measure Node (Ansible Playbook)..."
+        self.core_logger.debug(msg)
+        print(msg)
+
+        cmd = (
+            f"sudo cp /home/mfuser/mf_git/instrumentize/experiment_bootstrap/ansible.cfg /home/mfuser/services/common/ansible.cfg;"
+            f"sudo chown mfuser:mfuser /home/mfuser/services/common/ansible.cfg;"
+            f"sudo -u mfuser python3 /home/mfuser/mf_git/instrumentize/experiment_bootstrap/bootstrap_playbooks.py;"
+        )
+        stdout, stderr = self.meas_node.execute(cmd, quiet=True)
+
+        msg = f"Bootstrap Process on Measure Node (Ansible Playbook) done."
+        self.core_logger.debug(msg)
+        print(msg)
+
+        if stdout:
+            try:
+                self.core_logger.debug(f"STDOUT: {json.dumps(stdout, indent=2)}")
+            except ValueError as e:
+                self.core_logger.debug(f"STDOUT: {stdout}")
+        if stderr:
+            self.core_logger.info(f"STDERR: {stderr}")
 
         print("Bootstrap ansible scripts done")
-        
 
     ############################
     # Calls made as slice user
     ###########################
     def get_bootstrap_status(self, force=True):
         """
-        Returns the bootstrap status for the slice. Default setting of force will always download the most recent file from the meas node.
-        :param force: If downloaded file already exists locally, it will not be downloaded unless force is True. The downloaded file will be stored locally for future reference. 
-        :return: Bootstrap dict if any type of bootstraping has occured, None otherwise. 
-        :rtype: dict
+        Returns the bootstrap status for the slice. Default setting of force will always download the most recent file from the meas node. The downloaded file will be stored locally for future reference at self.bootstrap_status_file.
+
+        Args:
+            force(Boolean): If downloaded file already exists locally, it will not be downloaded unless force is True. .
+        Returns:
+            Dictionary: Bootstrap dict if any type of bootstraping has occured, Empty dict otherwise.
         """
         if force or not os.path.exists(self.bootstrap_status_file):
             if not self._download_bootstrap_status():
-                #print("Bootstrap file was not downloaded. Bootstrap most likely has not been done.")
+                # print("Bootstrap file was not downloaded. Bootstrap most likely has not been done.")
                 return {}
-        
-            
+
         if os.path.exists(self.bootstrap_status_file):
             with open(self.bootstrap_status_file) as bsf:
                 try:
                     bootstrap_dict = json.load(bsf)
-                    #print(bootstrap_dict)
+                    # print(bootstrap_dict)
                     if bootstrap_dict:
-                        return bootstrap_dict 
+                        return bootstrap_dict
                     else:
                         return {}
                 except Exception as e:
                     print(f"Bootstrap failed to decode")
                     print(f"Fail: {e}")
                     return {}
         else:
             return {}
 
-    # def clear_bootstrap_status(self):
-    #     """
-    #     Deletes the local and remote copy of the bootstrap_status files. This will then allow a rerunning of the init bootstrapping process.  
-    #     This is mainly intended for testing/debugging.
-    #     Note that nothing will be removed from the nodes.  
-    #     """
-            
-    #     # Delete local copy
-    #     if os.path.exists(self.bootstrap_status_file):
-    #         os.remove(self.bootstrap_status_file)
-
-    #     # Delete measurement node copy
-    #     try:
-    #         full_command = "rm bootstrap_status.json"
-    #         stdout, stderr = self.meas_node.execute(full_command)
-    #         self.core_logger.info("Removed remote bootstrap_status file.")
-    #     except Exception as e:
-    #         print(f"rm bootstrap_status.json Failed: {e}")
-    #         self.core_logger.exception(f"rm bootstrap_status.json Failed: {e}")
-    #         if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
-    #         if stderr: self.core_logger.debug(f"STDERR: {stderr}")
-    
+    def _clear_bootstrap_status(self):
+        """
+        Deletes the local and remote copy of the bootstrap_status files. This will then allow a rerunning of the init bootstrapping process.
+        This is mainly intended for testing/debugging.
+        Note that nothing will be removed from the nodes.
+        """
+
+        # Delete local copy
+        if os.path.exists(self.bootstrap_status_file):
+            os.remove(self.bootstrap_status_file)
 
+        # Delete measurement node copy
+        try:
+            full_command = "rm bootstrap_status.json"
+            stdout, stderr = self.meas_node.execute(full_command)
+            self.core_logger.info("Removed remote bootstrap_status file.")
+        except Exception as e:
+            print(f"rm bootstrap_status.json Failed: {e}")
+            self.core_logger.exception(f"rm bootstrap_status.json Failed: {e}")
+            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
 
     def _download_bootstrap_status(self):
         """
-        Downloaded file will be stored locally for future reference.  
-        :return: True if bootstrap file downloaded, False otherwise. 
-        :rtype: Boolean # or maybe just the entire json?
+        Downloads the bootstrap file from the meas_node. The downloaded file will be stored locally for future reference at self.bootstrap_status_file.
+
+        Returns:
+            Boolean: True if bootstrap file downloaded, False otherwise.
         """
         try:
             local_file_path = self.bootstrap_status_file
-            remote_file_path =  os.path.join("bootstrap_status.json")
-            #print(local_file_path)
-            #print(remote_file_path)
-            file_attributes = self.meas_node.download_file(local_file_path, remote_file_path, retry=1) #, retry=3, retry_interval=10): # note retry is really tries
-            #print(file_attributes)
-            
+            remote_file_path = os.path.join("bootstrap_status.json")
+            # print(local_file_path)
+            # print(remote_file_path)
+            file_attributes = self.meas_node.download_file(
+                local_file_path, remote_file_path, retry=1
+            )  # , retry=3, retry_interval=10): # note retry is really tries
+            # print(file_attributes)
+
             return True
         except FileNotFoundError:
-            pass 
+            pass
             # Most likely the file does not exist because it has not yet been created. So we will ignore this exception.
         except Exception as e:
             print("Bootstrap download has failed.")
             print(f"Fail: {e}")
             return False
-        return False  
-    
-    
-    
+        return False
+
     def get_mfuser_private_key(self, force=True):
         """
-        Returns the mfuser private key. Default setting of force will always download the most recent file from the meas node.
-        :param force: If downloaded file already exists locally, it will not be downloaded unless force is True. The downloaded file will be stored locally for future reference. 
-        :return: True if file is found, false otherwise. 
-        :rtype: Boolean
+        Downloads the mfuser private key. Default setting of force will always download the most recent file from the meas node. The downloaded file will be stored locally for future reference at self.local_mfuser_private_key_filename.
+
+
+        Args:
+            force(Boolean): If downloaded file already exists locally, it will not be downloaded unless force is True.
+        Returns:
+            Boolean: True if file is found, false otherwise.
         """
         if force or not os.path.exists(self.local_mfuser_private_key_filename):
             self._download_mfuser_private_key()
 
         if os.path.exists(self.local_mfuser_private_key_filename):
-                return True 
+            return True
         else:
-            return False 
-
+            return False
 
     def _download_mfuser_private_key(self):
         """
-        Downloaded file will be stored locally for future reference.  
-        :return: True if key file downloaded, False otherwise. 
-        :rtype: Boolean
+        Downloads the mfuser private key from the meas node. The downloaded file will be stored locally for future reference at self.local_mfuser_private_key_filename.
+
+        Returns:
+            Boolean: True if key file downloaded, False otherwise.
         """
         try:
             local_file_path = self.local_mfuser_private_key_filename
-            remote_file_path =  self.mfuser_private_key_filename
-            file_attributes = self.meas_node.download_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
-            #print(file_attributes)
+            remote_file_path = self.mfuser_private_key_filename
+            file_attributes = self.meas_node.download_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
+            # print(file_attributes)
             return True
         except Exception as e:
             print(f"Download mfuser private key Failed: {e}")
-        return False  
-    
-    
+            self.core_logger.error(f"Download mfuser private key Failed: {e}")
+        return False
+
     def _update_bootstrap(self, key, value):
         """
         Updates the given key to the given value in the bootstrap_status.json file on the meas node.
         """
         bsf_dict = self.get_bootstrap_status()
-        #self.download_bootstrap_status()
-        #bsf_dict = {}
+        # self.download_bootstrap_status()
+        # bsf_dict = {}
         bsf_dict[key] = value
-        
+
         with open(self.bootstrap_status_file, "w") as bsf:
             json.dump(bsf_dict, bsf)
-    
+
         try:
             local_file_path = self.bootstrap_status_file
-            remote_file_path =  os.path.join("bootstrap_status.json")
-            #print(local_file_path)
-            #print(remote_file_path)
-            file_attributes = self.meas_node.upload_file(local_file_path, remote_file_path) #, retry=3, retry_interval=10):
-            #print(file_attributes)
-            
+            remote_file_path = os.path.join("bootstrap_status.json")
+            # print(local_file_path)
+            # print(remote_file_path)
+            file_attributes = self.meas_node.upload_file(
+                local_file_path, remote_file_path
+            )  # , retry=3, retry_interval=10):
+            # print(file_attributes)
+
             return True
 
         except Exception as e:
             print("Bootstrap upload has failed.")
             print(f"Fail: {e}")
-        return False  
-    
-       
-    
+        return False
+
     def download_log_file(self, service, method):
         """
         Download the log file for the given service and method.
-        Downloaded file will be stored locally for future reference. 
+        Downloaded file will be stored locally for future reference.
         :param service: The name of the service.
-        :type service: String 
+        :type service: String
         :param method: The method name such as create, update, info, start, stop, remove.
         :type method: String
         :return: Writes file to local storage and returns text of the log file.
         :rtype: String
         """
         try:
-            local_file_path = os.path.join( self.local_slice_directory, f"{method}.log")
-            remote_file_path =  os.path.join("/","home","mfuser","services", service, "log", f"{method}.log")
-            #print(local_file_path)
-            #print(remote_file_path)
-            file_attributes = self.meas_node.download_file(local_file_path, remote_file_path, retry=1) #, retry=3, retry_interval=10): # note retry is really tries
-            #print(file_attributes)
-            
+            local_file_path = os.path.join(self.local_slice_directory, f"{method}.log")
+            remote_file_path = os.path.join(
+                "/", "home", "mfuser", "services", service, "log", f"{method}.log"
+            )
+            # print(local_file_path)
+            # print(remote_file_path)
+            file_attributes = self.meas_node.download_file(
+                local_file_path, remote_file_path, retry=1
+            )  # , retry=3, retry_interval=10): # note retry is really tries
+            # print(file_attributes)
+
             with open(local_file_path) as f:
                 log_text = f.read()
                 return local_file_path, log_text
 
         except Exception as e:
             print("Service log download has failed.")
             print(f"Downloading service log file has Failed. It may not exist: {e}")
-            return "",""
-
-    
+            return "", ""
```

### Comparing `fabrictestbed-mflib-0.0.0b1/mflib/mflib.py` & `fabrictestbed-mflib-0.1.0b0/mflib/mflib.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,66 +23,65 @@
 
 
 import json
 import traceback
 import os
 
 from fabrictestbed_extensions.fablib.fablib import fablib
+
 # For getting vars to make tunnel
 from fabrictestbed_extensions.fablib.fablib import FablibManager
 
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
 from os import chmod
 
-# import string
-# import random
-
-
 import logging
 
 from mflib.core import Core
 
 
 class MFLib(Core):
     """
     MFLib allows for adding and controlling the MeasurementFramework in a Fabric experiementers slice.
-
     """
 
-    mflib_class_version = "1.0.30"
+    mflib_class_version = "1.0.37"
 
     def set_mflib_logger(self):
         """
-        Sets up the mflib logging file. Filename is created from the self.logging_filename.
+        Sets up the mflib logging file. The filename is created from the self.logging_filename.
         Note that the self.logging_filename will be set with the slice when the slice name is set.
 
         This method uses the logging filename inherited from Core.
         """
 
         self.mflib_logger = logging.getLogger(__name__)
-        self.mflib_logger.propagate = False # needed?
+        self.mflib_logger.propagate = False  # needed?
         self.mflib_logger.setLevel(self.log_level)
-        
-        formatter = logging.Formatter('%(asctime)s %(name)-8s %(levelname)-8s %(message)s', datefmt='%m/%d/%Y H:%M:%S %p')
+
+        formatter = logging.Formatter(
+            "%(asctime)s %(name)-8s %(levelname)-8s %(message)s",
+            datefmt="%m/%d/%Y %H:%M:%S %p",
+        )
 
         # Make sure log directory exists
         if not os.path.exists(self.log_directory):
             os.makedirs(self.log_directory)
 
         # Remove existing log handler if present
         if self.mflib_log_handler:
             self.remove_mflib_log_handler(self.mflib_log_handler)
 
         file_handler = logging.FileHandler(self.log_filename)
         file_handler.setLevel(self.log_level)
         file_handler.setFormatter(formatter)
 
-        #self.mflib_logger.addHandler(file_handler)
+        # self.mflib_logger.addHandler(file_handler)
         self.add_mflib_log_handler(file_handler)
 
     def remove_mflib_log_handler(self, log_handler):
         """
         Removes the given log handler from the mflib_logger.
 
         Args:
@@ -97,629 +96,700 @@
 
         Args:
             log_handler (logging handler): Log handler to add to the mflib_logger.
         """
         if self.mflib_logger:
             self.mflib_logger.addHandler(log_handler)
 
-          
-    # This is a temporary method needed untill modify slice ability is avaialble. 
-    @staticmethod 
-    def addMeasNode(slice, cores=4, ram=16, disk=500):
+    # This is a temporary method needed untill modify slice ability is avaialble.
+    @staticmethod
+    def addMeasNode(
+        slice,
+        cores=4,
+        ram=16,
+        disk=500,
+        network_type="FABNetv4",
+        site="NCSA",
+        image="default_ubuntu_20",
+    ):
         """
-        Adds Measurement node and measurement network to unsubmitted slice object.
+        Adds Measurement node and measurement network to an unsubmitted slice object.
 
         Args:
             slice (fablib.slice): Slice object already set with experiment topology.
             cores (int, optional): Cores for measurement node. Defaults to 4 cores.
             ram (int, optional): _description_. Defaults to 16 GB ram.
             disk (int, optional): _description_. Defaults to 500 GB disk.
+            network_type (string, optional): _description_. Defaults to FABNetv4.
+            site (string, optional): _description_. Defaults to NCSA.
         """
-
-        interfaces = []
-        sites = []
-        num = 1
-        
+        interfaces = {}
         for node in slice.get_nodes():
-            interfaces.append(node.add_component(model='NIC_Basic', name=("Meas_Nic"+str(num))).get_interfaces()[0])
-            sites.append(node.get_site())
-            num += 1
-        site = max(set(sites), key = sites.count)
-        
-        meas = slice.add_node(name="_meas_node", site=site)
-
-        # if not cores: 
-        #     cores = meas.default_cores 
-
-        # if not ram: 
-        #     ram = meas.default_ram 
-
-        # if not disk: 
-        #     disk = 500
+            this_site = node.get_site()
+            if this_site not in interfaces.keys():
+                interfaces[this_site] = []
+            this_nodename = node.get_name()
+            this_interface = node.add_component(
+                model="NIC_Basic", name=(f"meas_nic_{this_nodename}_{this_site}")
+            ).get_interfaces()[0]
+            (interfaces[this_site]).append(this_interface)
+
+        meas_nodename = "_meas_node"
+        meas_image = image
+        meas = slice.add_node(name=meas_nodename, site=site)
 
         meas.set_capacities(cores=cores, ram=ram, disk=disk)
-        meas.set_image("default_ubuntu_20")
-        interfaces.append(meas.add_component(model='NIC_Basic', name="Meas_Nic").get_interfaces()[0])
-        meas_net = slice.add_l2network(name="_meas_net", interfaces=interfaces)
-    
+        meas.set_image(meas_image)
+        if site not in interfaces.keys():
+            interfaces[site] = []
+        if network_type == "FABNetv4":
+            meas_interface = meas.add_component(
+                model="NIC_Basic", name=(f"meas_nic_{meas_nodename}_{site}")
+            ).get_interfaces()[0]
+            (interfaces[site]).append(meas_interface)
+
+            for site in interfaces.keys():
+                slice.add_l3network(
+                    name=f"l3_meas_net_{site}", interfaces=interfaces[site]
+                )
+        else:
+            logging.info(f"Unknown {network_type} Network type")
+            return False
         # This logging will appear in the fablib log.
-        logging.info(f'Added Meas node & network to slice "{slice.get_name()}" topography. Cores: {cores}  RAM: {ram}GB Disk {disk}GB')
-
-    def __init__(self, slice_name="",local_storage_directory="/tmp/mflib"):
+        logging.info(
+            f'Added Meas node & network to slice "{slice.get_name()}" topology. Cores: {cores}  RAM: {ram}GB Disk {disk}GB'
+        )
+
+    def __init__(
+        self,
+        slice_name="",
+        local_storage_directory="/tmp/mflib",
+        mf_repo_branch="main",
+        optimize_repos=False,
+    ):
         """
-        Constructor.
+        Constructor
+        Args:
+            slice (fablib.slice): Slice object already set with experiment topology.
+            local_storage_directory (str, optional): Directory where local data will be stored. Defaults to "/tmp/mflib".
+            mf_repo_branch (str, optional): git branch name to pull MeasurementFranework code from. Defaults to "main".
         """
-        super().__init__(local_storage_directory=local_storage_directory)
+        super().__init__(
+            local_storage_directory=local_storage_directory,
+            mf_repo_branch=mf_repo_branch,
+        )
         self.mflib_log_handler = None
 
         if slice_name:
-            self.init(slice_name)
+            self.init(slice_name, optimize_repos)
 
-
-    def init(self,slice_name):
+    def init(self, slice_name, optimize_repos):
         """
         Sets up the slice to ensure it can be monitored. Sets up basic software on Measurement Node and experiment nodes.
-        Slice must already have a Measurement Node. 
+        Slice must already have a Measurement Node.
         See log file for details of init output.
 
         Args:
-            slice_name (str): The name of the slice to be monitored.    
+            slice_name (str): The name of the slice to be monitored.
         Returns:
             Bool: False if no Measure Node found or a init process fails. True otherwise.
 
         """
 
-        
         print(f'Inititializing slice "{slice_name}" for MeasurementFramework.')
-        
-        
-        
+
         ########################
-        # Get slice 
+        # Get slice
         ########################
         self.slice_name = slice_name
 
         self.slice = fablib.get_slice(name=slice_name)
 
         self.set_mflib_logger()
-        
-        self.mflib_logger.info(f'Inititializing slice "{slice_name}" for MeasurementFramework.')
+
+        if optimize_repos:
+            msg = f'Optimizing Software Repositories fetch strategies for "{slice_name}"...'
+            print(msg)
+            self.mflib_logger.info(msg)
+            self._optimize_repos()
+
+        self.mflib_logger.info(
+            f'Inititializing slice "{slice_name}" for MeasurementFramework.'
+        )
         ########################
         # Check for prequisites
         #######################
-        
+
         # Does Measurement Node exist in topology?
         if not self.meas_node:
             print("Failed to find meas node. Need to addMeasureNode first.")
-            self.mflib_logger.warning("Failed to find meas node. Need to addMeasureNode first.")
+            self.mflib_logger.warning(
+                "Failed to find meas node. Need to addMeasureNode first."
+            )
             return False
-        
-        print(f"Found meas node as {self.meas_node.get_name()} at {self.meas_node.get_management_ip()}")
-        self.mflib_logger.info(f"Found meas node as {self.meas_node.get_name()} at {self.meas_node.get_management_ip()}")
-        
+
+        print(
+            f"Found meas node as {self.meas_node.get_name()} at {self.meas_node.get_management_ip()}"
+        )
+        self.mflib_logger.info(
+            f"Found meas node as {self.meas_node.get_name()} at {self.meas_node.get_management_ip()}"
+        )
+
         bss = self.get_bootstrap_status()
         if bss:
-            #print("Bootstrap status is")
-            #print(bss)
+            # print("Bootstrap status is")
+            # print(bss)
             self.mflib_logger.info("Bootstrap status is")
             self.mflib_logger.info(bss)
         else:
             print("Bootstrap status not found. Will now start bootstrap process...")
-            self.mflib_logger.info("Bootstrap status not found. Will now start bootstrap process...")
-        
-        if ("status" in bss and bss["status"] == "ready"):
+            self.mflib_logger.info(
+                "Bootstrap status not found. Will now start bootstrap process..."
+            )
+
+        if "status" in bss and bss["status"] == "ready":
             # Slice already instrumentized and ready to go.
-            self.get_mfuser_private_key() 
+            self.get_mfuser_private_key()
             print("Bootstrap status indicates Slice Measurement Framework is ready.")
-            self.mflib_logger.info("Bootstrap status indicates Slice Measurement Framework is ready.")
+            self.mflib_logger.info(
+                "Bootstrap status indicates Slice Measurement Framework is ready."
+            )
             return
-        else: 
-            
+        else:
             ###############################
             # Need to do some bootstrapping
             ###############################
- 
 
-                
-            ######################   
+            ######################
             # Create MFUser keys
             #####################
-            if "mfuser_keys" in bss and bss["mfuser_keys"] =="ok":
-                print( "mfuser_keys already generated" )
-                self.mflib_logger.info( "mfuser_keys already generated" )
+            if "mfuser_keys" in bss and bss["mfuser_keys"] == "ok":
+                print("mfuser_keys already generated")
+                self.mflib_logger.info("mfuser_keys already generated")
             else:
-            #if True:
-                print ("Generating MFUser Keys...")
-                self.mflib_logger.info( "Generating MFUser Keys..." )
+                # if True:
+                print("Generating MFUser Keys...")
+                self.mflib_logger.info("Generating MFUser Keys...")
                 key = rsa.generate_private_key(
                     backend=crypto_default_backend(),
                     public_exponent=65537,
-                    key_size=2048
+                    key_size=2048,
                 )
 
                 private_key = key.private_bytes(
                     crypto_serialization.Encoding.PEM,
                     crypto_serialization.PrivateFormat.TraditionalOpenSSL,
-                    crypto_serialization.NoEncryption()
+                    crypto_serialization.NoEncryption(),
                 )
 
                 public_key = key.public_key().public_bytes(
                     crypto_serialization.Encoding.OpenSSH,
-                    crypto_serialization.PublicFormat.OpenSSH
+                    crypto_serialization.PublicFormat.OpenSSH,
                 )
 
                 # Decode to printable strings
-                private_key_str = private_key.decode('utf-8')
-                public_key_str = public_key.decode('utf-8')
+                private_key_str = private_key.decode("utf-8")
+                public_key_str = public_key.decode("utf-8")
 
                 # Save public key & change mode
-                public_key_file = open(self.local_mfuser_public_key_filename, 'w');
-                #public_key_file = open("/tmp/mflib/mfuser.pub", 'w');
-                public_key_file.write(public_key_str);
-                public_key_file.write('\n');
+                public_key_file = open(self.local_mfuser_public_key_filename, "w")
+                public_key_file.write(public_key_str)
+                public_key_file.write("\n")
                 public_key_file.close()
-                #chmod("/tmp/mflib/mfuser.pub", 0o644);
-                chmod(self.local_mfuser_public_key_filename, 0o644);
-
+                chmod(self.local_mfuser_public_key_filename, 0o644)
 
                 # Save private key & change mode
-                private_key_file = open(self.local_mfuser_private_key_filename, 'w');
-                #private_key_file = open("/tmp/mflib/mfuser", 'w');
-                private_key_file.write(private_key_str);
+                private_key_file = open(self.local_mfuser_private_key_filename, "w")
+                private_key_file.write(private_key_str)
                 private_key_file.close()
-                #chmod("/tmp/mflib/mfuser", 0o600);
-                chmod(self.local_mfuser_private_key_filename, 0o600);
+                chmod(self.local_mfuser_private_key_filename, 0o600)
 
                 # Upload mfuser keys to default user dir for future retrieval
                 self._upload_mfuser_keys()
 
                 self._update_bootstrap("mfuser_keys", "ok")
                 print("MFUser key generation Done.")
                 self.mflib_logger.info("MFUser key generation Done.")
-            
-            
-                
+
             ###############################
             # Add mfusers
             ##############################
-            if "mfuser_accounts" in bss and bss["mfuser_accounts"] =="ok":
+            if "mfuser_accounts" in bss and bss["mfuser_accounts"] == "ok":
                 print("mfuser accounts are already setup.")
                 self.mflib_logger.info("mfuser already setup.")
             else:
-            #if True:  
-                #Install mflib user/environment
-                self.mflib_logger.info("Installing mfuser accounts...")
-                print("Installing mfuser accounts...")
+                # if True:
+                # Install mflib user/environment
+                msg = f"Installing mfuser account..."
+                self.mflib_logger.info(msg)
+                print(msg)
                 mfusers_install_success = True
-   
-                #Add user
-                threads = []
-                for node in self.slice.get_nodes():
-                    try:
-                        threads.append( node.execute_thread("sudo useradd -G root -m mfuser") )
-                    
-                    except Exception as e:
-                        print(f"Failed to add user: {e}")
-                        self.mflib_logger.exception(f"Failed to add mfuser user.")
-                        mfusers_install_success = False
-
-                for thread in threads:
-                    stdout, stderr = thread.result()
-                    if stdout: self.core_logger.debug(f"STDOUT useradd mfuser: {stdout}")
-                    if stderr: self.core_logger.error(f"STDERR useradd mfuser: {stderr}")
 
-                #Setup ssh directory
+                # Upload keys
+                # Ansible.pub is nolonger a good name here
                 threads = []
                 for node in self.slice.get_nodes():
                     try:
-                        threads.append( node.execute_thread("sudo mkdir /home/mfuser/.ssh; sudo chmod 700 /home/mfuser/.ssh; sudo chown -R mfuser:mfuser /home/mfuser/.ssh"))
-                        
-                    except Exception as e:
-                        print(f"Fail to setup ssh directory: {e}")
-                        self.mflib_logger.error(f"Fail to setup ssh directory: {e}")
-                        mfusers_install_success = False
-           
-                for thread in threads:
-                    stdout, stderr = thread.result()
-                    if stdout: self.core_logger.debug(f"STDOUT mkdir ssh: {stdout}")
-                    if stderr: self.core_logger.error(f"STDERR mkdir ssh: {stderr}")
-
-
-                #Add mfuser to sudoers
-                threads=[]
-                for node in self.slice.get_nodes():
-                    try:
-                        threads.append( node.execute_thread("echo 'mfuser ALL=(ALL:ALL) NOPASSWD: ALL' | sudo tee -a /etc/sudoers.d/90-cloud-init-users"))
-                        
-                    except Exception as e:
-                        print(f"Fail to add to sudoers: {e}")
-                        self.mflib_logger.exception(f"Fail to add to sudoers:")
-                        mfusers_install_success = False
+                        threads.append(
+                            node.upload_file(
+                                self.local_mfuser_public_key_filename, "mfuser.pub"
+                            )
+                        )
 
-                for thread in threads:
-                    stdout, stderr = thread.result()
-                    if stdout: self.core_logger.debug(f"STDOUT sudoers: {stdout}")
-                    if stderr: self.core_logger.error(f"STDERR sudoers: {stderr}")
- 
-
-                #Upload keys
-                # Ansible.pub is nolonger a good name here
-                for node in self.slice.get_nodes():
-                    try:
-                        threads.append( node.upload_file(self.local_mfuser_public_key_filename ,"mfuser.pub"))
-                        
                     except Exception as e:
                         print(f"Failed to upload keys: {e}")
                         self.mflib_logger.exception("Failed to upload keys.")
 
                         mfusers_install_success = False
-                
-                #Edit commands
-                threads=[]
-                for node in self.slice.get_nodes():
-                    try:
-                        threads.append( node.execute_thread("sudo mv mfuser.pub /home/mfuser/.ssh/mfuser.pub; sudo chown mfuser:mfuser /home/mfuser/.ssh/mfuser.pub;"))
-                        
-                    except Exception as e:
-                        print(f"Fail to set key permissions: {e}")
-                        self.mflib_logger.exception("Fail to set key permissions.")
-                        mfusers_install_success = False
 
-                self.mflib_logger.info("Moved keys on node.")
-                for thread in threads:
-                    stdout, stderr = thread.result()
-                    if stdout: self.core_logger.debug(f"STDOUT keys moved: {stdout}")
-                    if stderr: self.core_logger.error(f"STDERR keys moved: {stderr}")
+                # Add user
+                threads = []
+                cmd = (
+                    f"sudo useradd -s /bin/bash -G root -m mfuser;"
+                    f"sudo mkdir /home/mfuser/.ssh;"
+                    f"sudo chmod 700 /home/mfuser/.ssh;"
+                    f"echo 'mfuser ALL=(ALL:ALL) NOPASSWD: ALL' | sudo tee -a /etc/sudoers.d/90-cloud-init-users;"
+                    f"sudo mv mfuser.pub /home/mfuser/.ssh/mfuser.pub;"
+                    f"sudo cat /home/mfuser/.ssh/mfuser.pub | sudo tee -a /home/mfuser/.ssh/authorized_keys;"
+                    f"sudo chmod 644 /home/mfuser/.ssh/authorized_keys;"
+                    f"sudo chown -R mfuser:mfuser /home/mfuser/.ssh;"
+                )
 
-                #Raise Key
-                threads=[]
                 for node in self.slice.get_nodes():
                     try:
-                        threads.append( node.execute_thread("sudo cat /home/mfuser/.ssh/mfuser.pub | sudo tee -a /home/mfuser/.ssh/authorized_keys;"))
-                        
-                    except Exception as e:
-                        print(f"Failed to create authorized_keys: {e}")
-                        self.mflib_logger.exception("Failed to create authorized_keys.")
-                        mfusers_install_success = False
-
-                for thread in threads:
-                    stdout, stderr = thread.result()
-                    if stdout: self.core_logger.debug(f"STDOUT set key permissions: {stdout}")
-                    if stderr: self.core_logger.error(f"STDERR set key permissions: {stderr}")
+                        threads.append(node.execute_thread(cmd))
 
-
-                #Authorize key
-                threads=[]
-                for node in self.slice.get_nodes():
-                    try:
-                        threads.append( node.execute_thread("sudo chmod 644 /home/mfuser/.ssh/authorized_keys; sudo chown mfuser:mfuser /home/mfuser/.ssh/authorized_keys"))
-                        
                     except Exception as e:
-                        print(f"Failed to set authorized_keys permissions: {e}")
-                        self.mflib_logger.exception("Failed to set authorized_keys permissions.")
+                        print(f"Failed to setup mfuser: {e}")
+                        self.mflib_logger.exception(f"Failed to setup mfuser user.")
                         mfusers_install_success = False
 
                 for thread in threads:
                     stdout, stderr = thread.result()
-                    if stdout: self.core_logger.debug(f"STDOUT authorized keys: {stdout}")
-                    if stderr: self.core_logger.error(f"STDERR authorized keys: {stderr}")
-
+                    if stdout:
+                        self.core_logger.debug(f"STDOUT useradd mfuser: {stdout}")
+                    if stderr:
+                        self.core_logger.error(f"STDERR useradd mfuser: {stderr}")
 
                 if not self._copy_mfuser_keys_to_mfuser_on_meas_node():
                     mfusers_install_success = False
 
-
                 if mfusers_install_success:
                     self._update_bootstrap("mfusers", "ok")
-                    print("mfuser installations Done.")
-                    self.mflib_logger.info("Mfuser installs done.")
+                    msg = f"Installing mfuser account done."
+                    print(msg)
+                    self.mflib_logger.info(msg)
                 else:
-                    print("mfuser installations Failed")
-                    self.mflib_logger.error("Mfuser installs Failed.")
+                    msg = f"Installing mfuser account failed."
+                    print(msg)
+                    self.mflib_logger.info(msg)
                     return False
-            
-
 
             #######################
-            # Set ipv6 to ipv4 DNS 
+            # Set ipv6 to ipv4 DNS
             #######################
-            if "ipv6_4_nat" in bss and (bss["ipv6_4_nat"] == "set" or bss["ipv6_4_nat"] == "not_needed"):
-                print("ipv6 to 4 DNS nat already set or is not needed.")
-                self.mflib_logger.info("ipv6 to 4 DNS nat already set or is not needed.")
+            if "ipv6_4_nat" in bss and (
+                bss["ipv6_4_nat"] == "set" or bss["ipv6_4_nat"] == "not_needed"
+            ):
+                msg = f"NAT64 Workaround not needed..."
+                print(msg)
+                self.mflib_logger.info(msg)
             else:
-            #if True:
+                # if True:
                 nat_set_results = self.set_DNS_all_nodes()
                 self.mflib_logger.info(f"ipv6_4_nat: {nat_set_results}")
                 self._update_bootstrap("ipv6_4_nat", nat_set_results)
 
             #######################
-            # Set the measurement node
-            # in the hosts files 
+            # Clone mf repo
             #######################
-            if "hosts_set" in bss and bss["hosts_set"] == "ok":
-                print("Hosts already set.")
-                self.mflib_logger.info("Hosts already set.")
+            if "repo_cloned" in bss and bss["repo_cloned"] == "ok":
+                msg = f"Measurement Framework github repository already cloned."
+                print(msg)
+                self.mflib_logger.info(msg)
             else:
-                self._set_all_hosts_file()
-                self._update_bootstrap("hosts_set","ok")
+                # if True:
+                if self._clone_mf_repo():
+                    self._update_bootstrap("repo_cloned", "ok")
+                else:
+                    msg = f"Measurement Framework github repository clone Failed."
+                    return False
 
-            #######################
-            # Clone mf repo 
-            #######################
-            if "repo_cloned" in bss and bss["repo_cloned"] =="ok":
-                print("repo already cloned.")
-                self.mflib_logger.info("MF repo already cloned")
-            else:
-            #if True:
-                self._clone_mf_repo()
-                self._update_bootstrap("repo_cloned", "ok")
-                
-                
-                
             #######################################
-            # Create measurement network interfaces  
+            # Create measurement network interfaces
             # & Get hosts info for hosts.ini
             ######################################
-            if "meas_network" in bss and bss["meas_network"] =="ok":
-                print("measurement network already setup.")
-                self.mflib_logger.info("measurement network already setup.")
+            if "meas_network" in bss and bss["meas_network"] == "ok":
+                msg = f"Measurement Network already setup."
+                print(msg)
+                self.mflib_logger.info(msg)
             else:
-            #if True:
+                # if True:
                 self._make_hosts_ini_file(set_ip=True)
                 self._update_bootstrap("meas_network", "ok")
-                
-                
-            
+
+            #######################
+            # Set the measurement node
+            # in the hosts files
+            #######################
+            if "hosts_set" in bss and bss["hosts_set"] == "ok":
+                msg = f"/etc/host entries already set."
+                print(msg)
+                self.mflib_logger.info(msg)
+            else:
+                self._set_all_hosts_file()
+                self._update_bootstrap("hosts_set", "ok")
+
             #######################
             # Run Bootstrap script
             ######################
-            if "bootstrap_script" in bss and bss["bootstrap_script"] =="ok":
-                print("Bootstrap script aleady run on measurment node.")
+            if "bootstrap_script" in bss and bss["bootstrap_script"] == "ok":
+                print("Bootstrap script already run on measurment node.")
             else:
-            #if True:
+                # if True:
                 print("Bootstrapping measurement node via bash...")
                 self.mflib_logger.info("Bootstrapping measurement node via bash...")
                 self._run_bootstrap_script()
                 self._update_bootstrap("bootstrap_script", "ok")
 
-
-            if "bootstrap_ansible" in bss and bss["bootstrap_ansible"] =="ok":
+            if "bootstrap_ansible" in bss and bss["bootstrap_ansible"] == "ok":
                 print("Bootstrap ansible script already run on measurement node.")
             else:
-            #if True:
+                # if True:
                 print("Bootstrapping measurement node via ansible...")
                 self.mflib_logger.info("Bootstrapping measurement node via ansible...")
                 self._run_bootstrap_ansible()
                 self._update_bootstrap("bootstrap_ansible", "ok")
-            
 
             self._update_bootstrap("status", "ready")
             print("Inititialization Done.")
             self.mflib_logger.info("Inititialization Done.")
             return True
 
-
-
-    def instrumentize(self):
+    def instrumentize(self, services=[ "prometheus", "elk"]):
         """
         Instrumentize the slice. This is a convenience method that sets up & starts the monitoring of the slice. Sets up Prometheus, ELK & Grafana.
 
+        Args:
+            services(List of Strings): Just add the listed components. Options are elk or prometheus.
+
         Returns:
             dict   : The output from each phase of instrumetizing.
         """
-        self.mflib_logger.info(f"Instrumentizing {self.slice_name}")
-        self.mflib_logger.info("Setting up Prometheus.")
-        print("Setting up Prometheus...")
-        prom_data = self.create("prometheus")
-        print(prom_data)
-        self.mflib_logger.info(prom_data)
-
-        self.mflib_logger.info("Setting up ELK.")
-        print("Setting up ELK...")
-        elk_data = self.create("elk")
-        print(elk_data)
-        self.mflib_logger.info(elk_data)
-
-        # Install the default grafana dashboards.
-        self.mflib_logger.info("Setting up grafana_manager & dashboards.")
-        grafana_manager_data = self.create("grafana_manager")
-        self.mflib_logger.info(grafana_manager_data)
-
-        print("Instrumentize Done.")
-        self.mflib_logger.info("Instrumetize Done")
-
         all_data = {}
-        all_data["elk"] = elk_data
-        all_data["prometheues"] = prom_data 
-        all_data["grafana_manager"] = grafana_manager_data
-        
-        return all_data
 
+        if not services:
+            msg = f"Nothing to Instrumentize on FABRIC Slice {self.slice_name}"
+            print(msg)
+            self.mflib_logger.debug(msg)
+            return all_data
+
+        msg = f'Instrumentizing slice "{self.slice_name}"'
+        print(msg)
+
+        self.mflib_logger.debug(msg)
+
+        for service in services:
+            service = service.strip()
+            if "prometheus" == service:
+                msg = f"   Setting up Prometheus..."
+                print(msg)
+                self.mflib_logger.debug(msg)
+
+                prom_data = self.create("prometheus")
+                if not prom_data["success"]:
+                    print(prom_data)
+                self.mflib_logger.debug(prom_data)
+
+                msg = f"   Setting up Prometheus done."
+                print(msg)
+                self.mflib_logger.debug(msg)
+
+                all_data["prometheues"] = prom_data
+
+                # Install the default grafana dashboards.
+                msg = f"   Setting up grafana_manager & dashboards..."
+                print(msg)
+                self.mflib_logger.info(msg)
+
+                grafana_manager_data = self.create("grafana_manager")
+                if not grafana_manager_data["success"]:
+                    print(grafana_manager_data)
+                self.mflib_logger.debug(grafana_manager_data)
+
+                msg = f"   Setting up grafana_manager & dashboards done."
+                print(msg)
+                self.mflib_logger.info(msg)
+                all_data["grafana_manager"] = grafana_manager_data
+
+            elif service:
+                msg = f"   Setting up {service}..."
+                print(msg)
+                self.mflib_logger.debug(msg)
+
+                service_data = self.create(service)
+                if not service_data["success"]:
+                    print(service_data)
+                self.mflib_logger.debug(service_data)
+
+                msg = f"   Setting up {service} done."
+                print(msg)
+                self.mflib_logger.debug(msg)
+                all_data[service] = service_data
+
+
+
+        msg = f"Instrumentize Process Complete."
+        print(msg)
+        self.mflib_logger.info(msg)
 
+        return all_data
 
     def _make_hosts_ini_file(self, set_ip=False):
-        """
-        Creates hosts.ini files needed by various services on the measurement node.
-        Optionally sets the ip interfaces for the measurement network
-        Args:
-            set_ip (bool, optional): Optionally sets the the measurement network interfaces. Defaults to False.
-        """
-        hosts = []                    
-        num=1
-        base = "10.0.0."
         hosts = []
+        mfuser = "mfuser"
         if set_ip:
-            print("Setting measurement nic IPs")
-            self.mflib_logger.info("Setting measurement nic IPs")
-        for node in self.slice.get_nodes():
-            for interface in node.get_interfaces():
-                if ("Meas_Nic" in interface.get_name()):
-                    ip = base + str(num)
-                   
-                    if set_ip:
-                        print(f"setting interface ip {ip}")
-                        self.mflib_logger.info(f"setting interface ip {ip}")
-                        interface.set_ip(ip = ip, cidr = "24")
-                    #hosts.append("{0} ansible_host={1} hostname={1} ansible_ssh_user={2} node_exporter_listen_ip={1} node_exporter_username={3} node_exporter_password={3} snmp_community_string={4} grafana_admin_password={3} fabric_prometheus_ht_user={3} fabric_prometheus_ht_password={3}".format(node.get_name(), ip ,"mfuser","fabric","not-in-use"))
-                    #hosts.append("{0} ansible_host={1} hostname={1} ansible_ssh_user={2} node_exporter_listen_ip={1}".format(node.get_name(), ip ,"mfuser"))
-                    hosts.append("{0} ansible_host={1} hostname={1} ansible_ssh_user={2} node_exporter_listen_ip={1} ansible_ssh_common_args='-o StrictHostKeyChecking=no'".format(node.get_name(), ip ,"mfuser"))
-                    num+=1
-
+            msg = f"Configuring Measurement Network..."
+            print(msg)
+            self.mflib_logger.info(msg)
+
+        meas_nodename = "_meas_node"
+        meas_node = self.slice.get_node(name=meas_nodename)
+        meas_site = meas_node.get_site()
+        meas_network = self.slice.get_network(name=f"l3_meas_net_{meas_site}")
+        meas_net_subnet = meas_network.get_subnet()
+        networks = self.slice.get_networks()
+
+        for network in networks:
+            network_name = network.get_name()
+            network_type = network.get_type()
+            if str(network_type) == "FABNetv4" and network_name.startswith(
+                "l3_meas_net_"
+            ):
+                network_site = network.get_site()
+                network_subnet = network.get_subnet()
+                interfaces = network.get_interfaces()
+                available_ips = network.get_available_ips()
+                for interface in interfaces:
+                    ip_addr = available_ips.pop(0)
+                    interface.ip_addr_add(addr=ip_addr, subnet=network_subnet)
+                    interface.ip_link_up()
+                    node = interface.get_node()
+                    if node.get_reservation_id() == meas_node.get_reservation_id():
+                        for other_network in networks:
+                            if other_network.get_name() == network_name:
+                                continue
+                            if str(
+                                other_network.get_type()
+                            ) == "FABNetv4" and other_network.get_name().startswith(
+                                "l3_meas_net_"
+                            ):
+                                node.ip_route_add(
+                                    subnet=other_network.get_subnet(),
+                                    gateway=network.get_gateway(),
+                                )
+                    else:
+                        node.ip_route_add(
+                            subnet=meas_net_subnet, gateway=network.get_gateway()
+                        )
+                    hosts.append(
+                        f"{node.get_name()} "
+                        f"ansible_host={ip_addr} "
+                        f"hostname={ip_addr} "
+                        f"ansible_ssh_user={mfuser} "
+                        f"node_exporter_listen_ip={ip_addr} "
+                        f"ansible_ssh_common_args='-o StrictHostKeyChecking=no' "
+                        f'management_ip_type="{node.validIPAddress(node.get_management_ip())}"'
+                    )
 
-        # print("Creating Ansible Hosts File\n")
         # Prometheus e_Elk
         hosts_txt = ""
-        e_hosts_txt = ""
+        # e_hosts_txt = ""
+        hosts_tail = f"""
+
+[elk:children]
+Meas_Node
+
+[workers:children]
+Experiment_Nodes
+"""
 
         experiment_nodes = "[Experiment_Nodes]\n"
         e_experiment_nodes = "[workers]\n"
         for host in hosts:
             if "_meas_node" in host:
-
                 hosts_txt += "[Meas_Node]\n"
-                hosts_txt += host + '\n\n'
-
-                e_hosts_txt += "[elk]\n"
-                e_hosts_txt += host + '\n\n'
-
-            else: # It is an experimenters node
-                experiment_nodes += host + '\n'
-                e_experiment_nodes += host + '\n'
+                hosts_txt += host + "\n\n"
+            else:  # It is an experimenters node
+                experiment_nodes += host + "\n"
 
         hosts_txt += experiment_nodes
-        e_hosts_txt += e_experiment_nodes
+        hosts_txt += hosts_tail
+        hosts_ini = "hosts.ini"
 
-        local_prom_hosts_filename = os.path.join(self.local_slice_directory, "promhosts.ini")
-        local_elk_hosts_filename = os.path.join(self.local_slice_directory, "elkhosts.ini")
+        local_prom_hosts_filename = os.path.join(self.local_slice_directory, hosts_ini)
 
-        with open(local_prom_hosts_filename, 'w') as f:
+        with open(local_prom_hosts_filename, "w") as f:
             f.write(hosts_txt)
-        with open(local_elk_hosts_filename, 'w') as f:
-            f.write(e_hosts_txt)
 
+        remote_dir = "/tmp"
         # Upload the files to the meas node and move to correct locations
-
-        # Upload Prom hosts
-        self.meas_node.upload_file(local_prom_hosts_filename,"promhosts.ini")
+        self.meas_node.upload_file(
+            local_prom_hosts_filename, f"{remote_dir}/{hosts_ini}"
+        )
+        msg = f"Measurement Network setup complete."
+        print(msg)
+        self.mflib_logger.info(msg)
 
         # create a common version of hosts.ini for all to access
-        self.mflib_logger.info("Setting up common hosts.ini file to measurement node.")
-        stdout, stderr = self.meas_node.execute("sudo mkdir -p /home/mfuser/services/common")
-        stdout, stderr = self.meas_node.execute("sudo chown mfuser:mfuser /home/mfuser/services")
-        stdout, stderr = self.meas_node.execute("sudo chown mfuser:mfuser /home/mfuser/services/common")
-        stdout, stderr = self.meas_node.execute("sudo cp promhosts.ini /home/mfuser/services/common/hosts.ini")
-        stdout, stderr = self.meas_node.execute("sudo chown mfuser:mfuser /home/mfuser/services/common/hosts.ini")
-        
-        # Upload the elkhosts.ini file.
-        self.meas_node.upload_file(local_elk_hosts_filename,"elkhosts.ini")
-
-        # create the elk.ini file
-        stdout, stderr = self.meas_node.execute("sudo mv elkhosts.ini /home/mfuser/mf_git/elkhosts.ini")
-        stdout, stderr = self.meas_node.execute("sudo chown mfuser:mfuser /home/mfuser/mf_git/elkhosts.ini")
-        
-               
- 
+        msg = f"Generating Ansible Inventory for Measurement Framework Deployment..."
+        print(msg)
+        self.mflib_logger.info(msg)
+
+        stdout, stderr = self.meas_node.execute(
+            f"sudo mkdir -p /home/mfuser/services/common;"
+            f"sudo mv {remote_dir}/{hosts_ini} /home/mfuser/services/common/hosts.ini;"
+            f"sudo chown -R mfuser:mfuser /home/mfuser/services /home/mfuser/mf_git;",
+            quiet=True,
+        )
+        if stderr:
+            print(f"STDERR: {stderr}")
+            self.mflib_logger.error(f"STDERR: {stderr}")
+        self.mflib_logger.debug(f"STDOUT: {stdout}")
+        msg = f"Ansible Inventory for Measurement Framework Deployment generated and saved."
+        print(msg)
+        self.mflib_logger.info(msg)
 
     def download_common_hosts(self):
         """
         Downloads hosts.ini file and returns file text.
-        Downloaded hosts.ini file will be stored locally for future reference.  
-        :param service: The name of the service.
-        :type service: String 
-        :param method: The method name such as create, update, info, start, stop, remove.
-        :type method: String
-        :return: Writes file to local storage and returns text of the log file.
-        :rtype: String
+        Downloaded hosts.ini file will be stored locally for future reference.
         """
         try:
             local_file_path = self.common_hosts_file
-            remote_file_path =  os.path.join("/home/mfuser/services/common/hosts.ini")
-            #print(local_file_path)
-            #print(remote_file_path)
-            file_attributes = self.meas_node.download_file(local_file_path, remote_file_path, retry=1) #, retry=3, retry_interval=10): # note retry is really tries
-            #print(file_attributes)
-            
+            remote_file_path = os.path.join("/home/mfuser/services/common/hosts.ini")
+            file_attributes = self.meas_node.download_file(
+                local_file_path, remote_file_path, retry=1
+            )  # , retry=3, retry_interval=10): # note retry is really tries
+
             with open(local_file_path) as f:
                 hosts_text = f.read()
                 return local_file_path, hosts_text
 
         except Exception as e:
-            print("Common hosts.ini download has failed.")
-            print(f"downloading common hosts file Failed: {e}")
-            self.mflib_logger.exception("Downloading common hosts.ini file has failed.")
-            return "",""
+            msg = f"downloading common hosts file Failed: {e}"
+            print(msg)
+            self.mflib_logger.error(msg)
+            return "", ""
 
-
-# IPV6 to IPV4 only sites fix
-# note: should set bootstrap status file when making these 2 calls, status should be set, restored, not needed.
+    # IPV6 to IPV4 only sites fix
+    # note: should set bootstrap status file when making these 2 calls, status should be set, restored, not needed.
     def set_DNS_all_nodes(self):
         """
         Sets DNS for nodes to allow them to access ipv4 networks.
 
         Returns:
             string: "set" if DNS set, "not needed" otherwise.
         """
         # Check if we need to
-        if(self.meas_node.validIPAddress(self.meas_node.get_management_ip())=="IPv6"):
-            for node in self.slice.get_nodes():
+        # if self.meas_node.validIPAddress(self.meas_node.get_management_ip()) == "IPv6":
+        nat64_set = False
+        for node in self.slice.get_nodes():
+            if node.validIPAddress(node.get_management_ip()) == "IPv6":
                 self.set_DNS(node)
+                nat64_set = True
+
+        if nat64_set:
             return "set"
         else:
             return "not needed"
 
     def restore_DNS_all_nodes(self):
         """
         Restores the DNS to default if previously set. See set_DNS_all_nodes.
 
         Returns:
             string: "restored" if restored, "not needed" if not needed
         """
         # Check if we need to
-        if(self.meas_node.validIPAddress(self.meas_node.get_management_ip())=="IPv6"):
-            for node in self.slice.get_nodes():
+        nat64_restored = False
+        for node in self.slice.get_nodes():
+            if node.validIPAddress(node.get_management_ip()) == "IPv6":
                 self.restore_DNS(node)
+                nat64_restored = True
+        if nat64_restored:
             return "restored"
         else:
             return "not needed"
 
-    def set_DNS(self,node):
+    def set_DNS(self, node):
         """
         Sets the DNS on IPv6 only nodes to enable access to IPv4 sites.
         """
-        if(node.validIPAddress(node.get_management_ip())=="IPv6"):
+        if node.validIPAddress(node.get_management_ip()) == "IPv6":
             # needed to fix sudo unable to resolve error
-            node.execute('sudo echo -n "127.0.0.1 " | sudo cat - /etc/hostname  | sudo tee -a /etc/hosts')
+            commands = """
+            sudo echo -n "127.0.0.1 " | sudo cat - /etc/hostname  | sudo tee -a /etc/hosts;
+            sudo echo -n "2a01:4f9:c010:3f02:64:0:8c52:7103       github.com\n"|sudo tee -a /etc/hosts;
+            sudo echo -n "2a01:4f9:c010:3f02:64:0:8c52:7009       codeload.github.com\n"|sudo tee -a /etc/hosts;
+            sudo echo -n "2a01:4f9:c010:3f02:64:0:b9c7:6e85       objects.githubusercontent.com\n"|sudo tee -a /etc/hosts;
+            sudo echo -n "2600:1fa0:80b4:db49:34d9:6d1e::         ansible-galaxy.s3.amazonaws.com\n"|sudo tee -a /etc/hosts;
+            sudo echo -n "2a01:4f9:c010:3f02:64:0:3455:9777       packages.confluent.io\n"|sudo tee -a /etc/hosts;
+            """
+            stdout, stderr = node.execute(commands, quiet=True)
+            self.mflib_logger.info(f"STDOUT: {stdout}")
+            if stderr:
+                self.mflib_logger.error(f"STDERR: {stderr}")
 
-            node.execute("""
-            printf 'nameserver 2a00:1098:2c::1\nnameserver 2a01:4f8:c2c:123f::1\nnameserver 2a01:4f9:c010:3f02::1' > resolv.new;
-            sudo mv /etc/resolv.conf /etc/resolv.old;
-            sudo mv resolv.new /etc/resolv.conf;
-            """)
-            #Needed for fedora
-            # Check if eth0 exists to prevent errors. TODO check if this is still needed or check if os is fedora instead.
-            if os.path.exists(os.path.join("sys", "class", "net", "eth0")):
-                node.execute("""
-                    sudo resolvectl dns eth0 2a00:1098:2c::1;
-                    sudo resolvectl dns eth0 2a01:4f8:c2c:123f::1;
-                    sudo resolvectl dns eth0 2a01:4f9:c010:3f02::1;
-                """)
-
-    def restore_DNS(self,node):
-        if(node.validIPAddress(node.get_management_ip())=="IPv6"):
-            node.execute("""
-                sudo mv /etc/resolv.old /etc/resolv.conf;
-            """)
-            #Needed for fedora
-            # Check if eth0 exists to prevent errors. TODO check if this is still needed or check if os is fedora instead.
-            if os.path.exists(os.path.join("sys", "class", "net", "eth0")):
-                node.execute("""
-                    resolvectl revert eth0;
-                """)
+    def restore_DNS(self, node):
+        return
 
     def _set_all_hosts_file(self):
-        for node in self.slice.get_nodes():
-            self._set_hosts_file(node)
-
-    def _set_hosts_file(self, node):
-        self.meas_node_ip
-        # Set the Measurement node ip
-        node.execute(f'sudo echo -n "{self.meas_node_ip} {self.measurement_node_name}" | sudo tee -a /etc/hosts')
+        meas_node_meas_net_ip = None
+        for interface in self.meas_node.get_interfaces():
+            if "_meas_node-meas_nic" in interface.get_name():
+                meas_node_meas_net_ip = interface.get_ip_addr()
+        if meas_node_meas_net_ip:
+            execute_threads = {}
+            cmd = f'sudo echo -n "{meas_node_meas_net_ip} {self.measurement_node_name}" | sudo tee -a /etc/hosts;'
+            for node in self.slice.get_nodes():
+                execute_threads[node] = node.execute_thread(cmd)
+            for node, thread in execute_threads.items():
+                self.mflib_logger.info(
+                    f"Waiting for result from node {node.get_name()}"
+                )
+                stdout, stderr = thread.result()
+                if stdout:
+                    self.mflib_logger.info(f"STDOUT: {stdout}")
+                if stderr:
+                    self.mflib_logger.error(f"STDERR: {stderr}")
+
+    def _optimize_repos(self):
+        nodes = self.slice.get_nodes()
+        for node in nodes:
+            IPv6Management = False
+            ip_proto_index = "4"
+            commands = "sudo ip -6 route del default via `ip -6 route show default|grep fe80|awk '{print $3}'` > /dev/null 2>&1"
+            if node.validIPAddress(node.get_management_ip()) == "IPv6":
+                IPv6Management = True
+                ip_proto_index = "6"
+            if [ele for ele in ["rocky", "centos"] if (ele in node.get_image())]:
+                commands = (
+                    f'sudo echo "max_parallel_downloads=10" |sudo tee -a /etc/dnf/dnf.conf;'
+                    f'sudo echo "fastestmirror=True" |sudo tee -a /etc/dnf/dnf.conf;'
+                    f'sudo echo "ip_resolve='
+                    + ip_proto_index
+                    + '" |sudo tee -a /etc/dnf/dnf.conf;'
+                )
+            elif [ele for ele in ["ubuntu", "debian"] if (ele in node.get_image())]:
+                commands = (
+                    'sudo echo "Acquire::ForceIPv'
+                    + ip_proto_index
+                    + ' "true";" | sudo tee -a /etc/apt/apt.conf.d/1000-force-ipv'
+                    + ip_proto_index
+                    + "-transport"
+                )
+            if commands:
+                stdout, stderr = node.execute(commands, quiet=True)
+                self.mflib_logger.info(f"STDOUT: {stdout}")
+                if stderr:
+                    self.mflib_logger.error(f"STDERR: {stderr}")
```

### Comparing `fabrictestbed-mflib-0.0.0b1/mflib/mfvis.py` & `fabrictestbed-mflib-0.1.0b0/mflib/mfvis.py`

 * *Files identical despite different names*

