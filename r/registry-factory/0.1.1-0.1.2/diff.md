# Comparing `tmp/registry_factory-0.1.1.tar.gz` & `tmp/registry_factory-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "registry_factory-0.1.1.tar", max compression
+gzip compressed data, was "registry_factory-0.1.2.tar", max compression
```

## Comparing `registry_factory-0.1.1.tar` & `registry_factory-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1119 2023-01-17 11:25:36.888129 registry_factory-0.1.1/LICENSE
--rw-r--r--   0        0        0     8923 2023-02-01 09:53:39.402902 registry_factory-0.1.1/README.md
--rw-r--r--   0        0        0     1130 2023-02-01 10:19:35.180404 registry_factory-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-27 14:34:50.205276 registry_factory-0.1.1/registry_factory/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 14:34:50.205276 registry_factory-0.1.1/registry_factory/checks/__init__.py
--rw-r--r--   0        0        0     1147 2023-01-31 16:02:59.724654 registry_factory-0.1.1/registry_factory/checks/accreditation.py
--rw-r--r--   0        0        0     1975 2023-01-31 16:09:26.327900 registry_factory-0.1.1/registry_factory/checks/factory_pattern.py
--rw-r--r--   0        0        0     1004 2023-01-31 15:46:51.558479 registry_factory-0.1.1/registry_factory/checks/testing.py
--rw-r--r--   0        0        0      456 2023-01-31 14:54:48.888673 registry_factory-0.1.1/registry_factory/checks/versioning.py
--rw-r--r--   0        0        0     3445 2023-01-31 14:32:23.787603 registry_factory-0.1.1/registry_factory/factory.py
--rw-r--r--   0        0        0     5168 2023-01-31 14:09:15.982395 registry_factory-0.1.1/registry_factory/index.py
--rw-r--r--   0        0        0        0 2023-01-27 14:34:50.209276 registry_factory-0.1.1/registry_factory/patterns/__init__.py
--rw-r--r--   0        0        0     2500 2023-01-31 13:56:15.495765 registry_factory-0.1.1/registry_factory/patterns/facade.py
--rw-r--r--   0        0        0     1900 2023-01-31 15:01:07.175882 registry_factory-0.1.1/registry_factory/patterns/mediator.py
--rw-r--r--   0        0        0     2811 2023-01-30 14:19:16.766350 registry_factory-0.1.1/registry_factory/patterns/metacoding.py
--rw-r--r--   0        0        0     2765 2023-01-31 11:18:37.562584 registry_factory-0.1.1/registry_factory/patterns/observer.py
--rw-r--r--   0        0        0     5198 2023-01-31 14:30:29.055865 registry_factory-0.1.1/registry_factory/registry.py
--rw-r--r--   0        0        0      763 2023-01-27 14:34:50.209276 registry_factory-0.1.1/registry_factory/tools.py
--rw-r--r--   0        0        0      507 2023-01-31 13:42:57.681472 registry_factory-0.1.1/registry_factory/tracker.py
--rw-r--r--   0        0        0      170 2023-01-27 14:34:50.209276 registry_factory-0.1.1/registry_factory/typescripts.py
--rw-r--r--   0        0        0      796 2023-01-27 16:47:09.992975 registry_factory-0.1.1/registry_factory/utils.py
--rw-r--r--   0        0        0     9872 1970-01-01 00:00:00.000000 registry_factory-0.1.1/setup.py
--rw-r--r--   0        0        0     9871 1970-01-01 00:00:00.000000 registry_factory-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1120 2023-02-01 13:31:18.135422 registry_factory-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1130 2023-04-13 10:40:26.721368 registry_factory-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8873 2023-02-01 13:31:18.139422 registry_factory-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-01-27 14:34:50.205276 registry_factory-0.1.2/registry_factory/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-27 14:34:50.205276 registry_factory-0.1.2/registry_factory/checks/__init__.py
+-rw-r--r--   0        0        0     1148 2023-04-13 10:29:41.465149 registry_factory-0.1.2/registry_factory/checks/accreditation.py
+-rw-r--r--   0        0        0     1974 2023-04-13 10:29:45.424636 registry_factory-0.1.2/registry_factory/checks/factory_pattern.py
+-rw-r--r--   0        0        0     1005 2023-04-13 10:30:07.808508 registry_factory-0.1.2/registry_factory/checks/testing.py
+-rw-r--r--   0        0        0      457 2023-04-13 10:30:10.130839 registry_factory-0.1.2/registry_factory/checks/versioning.py
+-rw-r--r--   0        0        0     5323 2023-04-13 10:26:58.123305 registry_factory-0.1.2/registry_factory/factory.py
+-rw-r--r--   0        0        0     5165 2023-04-13 10:27:18.575627 registry_factory-0.1.2/registry_factory/index.py
+-rw-r--r--   0        0        0        0 2023-01-27 14:34:50.209276 registry_factory-0.1.2/registry_factory/patterns/__init__.py
+-rw-r--r--   0        0        0     2500 2023-01-31 13:56:15.495765 registry_factory-0.1.2/registry_factory/patterns/facade.py
+-rw-r--r--   0        0        0     1855 2023-04-13 10:24:33.999597 registry_factory-0.1.2/registry_factory/patterns/mediator.py
+-rw-r--r--   0        0        0     2811 2023-01-30 14:19:16.766350 registry_factory-0.1.2/registry_factory/patterns/metacoding.py
+-rw-r--r--   0        0        0     2765 2023-01-31 11:18:37.562584 registry_factory-0.1.2/registry_factory/patterns/observer.py
+-rw-r--r--   0        0        0     6350 2023-04-13 10:27:25.548502 registry_factory-0.1.2/registry_factory/registry.py
+-rw-r--r--   0        0        0      763 2023-04-13 10:30:03.547762 registry_factory-0.1.2/registry_factory/tools.py
+-rw-r--r--   0        0        0      508 2023-04-13 10:28:09.425955 registry_factory-0.1.2/registry_factory/tracker.py
+-rw-r--r--   0        0        0      170 2023-04-13 10:28:13.666937 registry_factory-0.1.2/registry_factory/typescripts.py
+-rw-r--r--   0        0        0      796 2023-04-13 10:28:18.383764 registry_factory-0.1.2/registry_factory/utils.py
+-rw-r--r--   0        0        0     9821 1970-01-01 00:00:00.000000 registry_factory-0.1.2/PKG-INFO
```

### Comparing `registry_factory-0.1.1/LICENSE` & `registry_factory-0.1.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Advanced machine learning for Innovative Drug Discovery (AIDD)
+Copyright (c) 2022 Advanced machine learning for Innovative Drug Discovery (AIDD) 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `registry_factory-0.1.1/README.md` & `registry_factory-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # RegistryFactory
 
-![PyPI](https://img.shields.io/pypi/v/registry-factory)
+[![PyPI version](https://badge.fury.io/py/registry-factory.svg)](https://badge.fury.io/py/registry-factory)
+[![PyPI](https://img.shields.io/github/license/aidd-msca/registry-factory)](LICENSE)
 ![PyPI](https://img.shields.io/pypi/pyversions/registry-factory)
-![PyPI](https://img.shields.io/github/license/aidd-msca/registry-factory)
+[![GitHub Repo stars](https://img.shields.io/github/stars/aidd-msca/registry-factory)](https://github.com/aidd-msca/registry-factory/stargazers)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jlyEd1yxhvFCN82YqEFI82q2n0k_y06F?usp=sharing)
 
 An abstract implementation of the software design pattern called registry proposed in (Hartog et. al., 2023),
 providing a factory for creating registries to which categorically similar modules can be organized.
 
-**Content:**
 **[Installation](#installation)**
 | **[Dependencies](#dependencies)**
 | **[Usage](#usage)**
 | **[Citation](#citation)**
-| **[Code of Conduct](#code-of-conduct)**
 
 ### Overview
 
 The registry design patterns provides a way to organize modular
 functionalities dynamically and achieve a unified, reusable, and interchangeable interface.
 It extends the Factory design pattern without the explicit class dependency.
 Additionally, the registry supports optional meta information such as versioning, accreditation,
@@ -260,12 +259,7 @@
 
 The work behind this package has received funding from the European Union’s Horizon 2020
 research and innovation programme under the Marie Skłodowska-Curie
 Actions, grant agreement “Advanced machine learning for Innovative Drug
 Discovery (AIDD)” No 956832”. [Homepage](https://ai-dd.eu/).
 
 ![plot](figures/aidd.png)
-
-## Code of Conduct
-
-Everyone interacting in the codebase, issue trackers, chat rooms, and mailing lists is expected to follow the
-[PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).
```

### Comparing `registry_factory-0.1.1/pyproject.toml` & `registry_factory-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "registry-factory"
-version = "0.1.1"
+version = "0.1.2"
 description = "Abstract codebase with utilities to register generic modules."
 authors = ["Peter Hartog <peter.hartog@hotmail.nl>", "Emma Svensson <svensson@ml.jku.at>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidd-msca/registry-factory"
 repository = "https://github.com/aidd-msca/registry-factory"
 keywords = ["registry", "factory", "codebase", "module registry", "accreditation system"]
```

### Comparing `registry_factory-0.1.1/registry_factory/checks/accreditation.py` & `registry_factory-0.1.2/registry_factory/checks/accreditation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Accreditation postchecks for a codebase."""
 
+from dataclasses import dataclass
 from typing import Any, List, Optional
+
 from registry_factory.patterns.observer import MetaInformationObserver
-from dataclasses import dataclass
 
 __all__ = ["Accreditation", "CreditFields"]
 
 
 @dataclass
 class CreditFields:
     """Credit information."""
```

### Comparing `registry_factory-0.1.1/registry_factory/checks/factory_pattern.py` & `registry_factory-0.1.2/registry_factory/checks/factory_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Any, Dict, Optional, Tuple
-from types import FunctionType
-
 import warnings
+from types import FunctionType
+from typing import Any, Dict, Optional, Tuple
 
 from registry_factory.patterns.observer import RegistryObserver
 
 
 class FactoryPattern(RegistryObserver):
     """An instance factory pattern observer."""
```

### Comparing `registry_factory-0.1.1/registry_factory/checks/testing.py` & `registry_factory-0.1.2/registry_factory/checks/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Any, Callable, Dict, Optional, Tuple
 import warnings
+from typing import Any, Callable, Dict, Optional, Tuple
+
 from registry_factory.patterns.observer import RegistryObserver
 
 
 class Testing(RegistryObserver):
     """A testing observer."""
 
     def __init__(self, test_module: Callable, forced: bool = False):
```

### Comparing `registry_factory-0.1.1/registry_factory/index.py` & `registry_factory-0.1.2/registry_factory/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Any, Dict, Optional, Tuple
-import warnings
-from registry_factory.patterns.metacoding import UniqueDict
 import random
+import warnings
+from typing import Any, Dict, Optional, Tuple
 
+from registry_factory.patterns.metacoding import UniqueDict
 from registry_factory.typescripts import Dataclass
 
 
 class IndexDict(UniqueDict):
     """Dict that raises when reassigning an existing key."""
 
     _instance = None
@@ -62,14 +62,15 @@
     slots: Dict[int, Tuple[str, Dict]]
     data: Dict[int, Any]
     arg_dict: Dict[int, Dataclass]
     meta_dict: Dict[int, Dict]
 
     def __init__(self, bitsize: int = 256, max_generation: int = 1000):
         super().__init__(bitsize, max_generation)
+        self.arg_dict = {}
         self.meta_dict = {}
 
     def set(self, key: str, key_dict: Dict, obj: Any, meta: Optional[Dict] = None) -> None:
         full_key: Tuple[str, Dict] = (key, key_dict)
         if full_key in self.slots.values():
             hash_value = self.get_hash(key, key_dict)
             if hash_value in self.data.keys():
@@ -79,18 +80,18 @@
             self.slots[hash_value] = full_key
         self.data[hash_value] = obj
         if meta is not None:
             self.meta_dict[hash_value] = meta
 
     def set_arguments(self, key: str, key_dict: Dict, arguments: Dataclass) -> None:
         full_key: Tuple[str, Dict] = (key, key_dict)
-        if full_key in self.slots.values() and full_key in self.arg_dict.values():
-            raise KeyError(f"{key}, {key_dict} arguments already exist in the registry.")
-        elif full_key in self.slots.values():
+        if full_key in self.slots.values():
             hash_value = self.get_hash(key, key_dict)
+            if hash_value in self.arg_dict.keys():
+                raise KeyError(f"{key}, {key_dict} arguments already exist in the registry.")
         else:
             hash_value = self.generate_hash()
             self.slots[hash_value] = full_key
         self.arg_dict[hash_value] = arguments
 
     def get_hash(self, key: str, key_dict: Dict) -> int:
         for k, v in self.slots.items():
```

### Comparing `registry_factory-0.1.1/registry_factory/patterns/facade.py` & `registry_factory-0.1.2/registry_factory/patterns/facade.py`

 * *Files identical despite different names*

### Comparing `registry_factory-0.1.1/registry_factory/patterns/mediator.py` & `registry_factory-0.1.2/registry_factory/patterns/mediator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Mediator pattern implementation."""
 from typing import Any, Dict, Optional, Tuple
+
 from registry_factory.index import HashTable
 from registry_factory.patterns.facade import ObserverFacade
 
 
 class HashMediator:
     connection_hash: int
     hash_table: HashTable
@@ -28,16 +29,14 @@
         key_dict = self.generate_key_dict(key=key, **kwargs)
         obj = self.hash_table.get(key, key_dict)
         (key, key_dict, obj, meta_dict) = self.observer_facade.call_event(key=key, obj=obj, **kwargs)
         return (key, key_dict, obj, meta_dict)
 
     def get_meta(self, key: str, **kwargs) -> Dict:
         key_dict = self.generate_key_dict(key=key, **kwargs)
-        print("heya")
-        print(key_dict)
         return self.hash_table.get_meta(key, key_dict)
 
 
 class HashConnection:
     connection: Dict[int, HashMediator]
 
     def add_connection(self, connection_hash: int, mediator: HashMediator) -> None:
```

### Comparing `registry_factory-0.1.1/registry_factory/patterns/metacoding.py` & `registry_factory-0.1.2/registry_factory/patterns/metacoding.py`

 * *Files identical despite different names*

### Comparing `registry_factory-0.1.1/registry_factory/patterns/observer.py` & `registry_factory-0.1.2/registry_factory/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `registry_factory-0.1.1/registry_factory/registry.py` & `registry_factory-0.1.2/registry_factory/registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Registry module for a codebase."""
-from abc import ABC
 import warnings
-from typing import Any, Callable, List, Optional, Dict, Tuple
+from abc import ABC
+from dataclasses import dataclass, is_dataclass
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 # from registry_factory.tracker import Tracker
 from registry_factory.patterns.mediator import HashMediator
 from registry_factory.typescripts import Dataclass
 from registry_factory.utils import RegistrationError, RegistrationWarning
 
 __all__ = ["AbstractRegistry"]
@@ -54,14 +55,30 @@
 
     @classmethod
     def __repr__(cls) -> str:
         """Return a string representation of the registry."""
         return f"{cls.__name__}({cls.mediator.hash_table.slots})"
 
     @classmethod
+    def items(cls) -> List[Tuple[Tuple[str, Dict], Any]]:
+        """Return a list of registered keys."""
+        hashes = [key for key in cls.mediator.hash_table.slots.keys()]
+        return [(cls.mediator.hash_table.slots[_hash], cls.mediator.hash_table.data[_hash]) for _hash in hashes]
+
+    @classmethod
+    def keys(cls) -> List[Tuple[str, Dict]]:
+        """Return a list of registered keys."""
+        return [(key, key_dict) for key, key_dict in cls.mediator.hash_table.slots.values()]
+
+    @classmethod
+    def values(cls) -> List[Any]:
+        """Return a list of registered keys."""
+        return [cls.mediator.hash_table.data.values()]
+
+    @classmethod
     def register(cls, key: str, **kwargs) -> Callable:
         """Register the object to the key with the option to use as a decorator."""
 
         def wrapper(obj: Callable) -> Callable:
             """Register the object to the key."""
             cls.mediator.register_event(key=key, obj=obj, **kwargs)
             return obj
@@ -91,15 +108,15 @@
     def get_info(cls, key: str, **kwargs) -> Dict:
         """Return the meta information for the key."""
         return cls.mediator.get_meta(key, **kwargs)
 
     @classmethod
     def show_choices(cls) -> List[Tuple[str, Dict]]:
         """Returns the indexes of all registered objects."""
-        return list(cls.mediator.hash_table.slots.values())
+        return cls.keys()
 
     @classmethod
     def check_choice(cls, key: str, **kwargs) -> bool:
         """Checks if a choice is valid and returns a bool."""
         key_dict = cls.mediator.generate_key_dict(key=key, **kwargs)
         if (key, key_dict) not in cls.mediator.hash_table.slots.values():
             warnings.warn(RegistrationWarning(f"{key} is not a valid choice."))
@@ -119,24 +136,31 @@
         cls.mediator.hash_table.clear()
 
     @classmethod
     def register_arguments(cls, key: str, **kwargs) -> Callable:
         """Register the arguments to the key."""
 
         def wrapper(argument_class: Dataclass) -> Any:
+            if not is_dataclass(argument_class):
+                try:
+                    argument_class = dataclass(argument_class)  # type: ignore
+                except Exception:
+                    raise RegistrationError("The argument class must be a dataclass.")
+                else:
+                    warnings.warn(RegistrationWarning("The argument class has been converted to a dataclass."))
             key_dict = cls.mediator.generate_key_dict(key=key, **kwargs)
             cls.mediator.hash_table.set_arguments(key, key_dict, argument_class)
             return argument_class
 
         return wrapper
 
     @classmethod
-    def get_arguments(cls, key: str, **kwargs) -> Dataclass:
+    def get_arguments(cls, key: str, key_dict: Optional[Dict] = None, **kwargs) -> Dataclass:
         """Return the arguments registered to the key."""
-        key_dict = cls.mediator.generate_key_dict(key=key, **kwargs)
+        key_dict = cls.mediator.generate_key_dict(key=key, **kwargs) if key_dict is None else key_dict
         return cls.mediator.hash_table.get_arguments(key, key_dict)
 
     # Legacy methods
     @classmethod
     def get_choice(cls, key: str, **kwargs) -> Any:  # Legacy
         """Legacy: Returns an object from the index."""
         return cls.get(key, **kwargs)
```

### Comparing `registry_factory-0.1.1/registry_factory/tools.py` & `registry_factory-0.1.2/registry_factory/tools.py`

 * *Files identical despite different names*

### Comparing `registry_factory-0.1.1/registry_factory/utils.py` & `registry_factory-0.1.2/registry_factory/utils.py`

 * *Files identical despite different names*

### Comparing `registry_factory-0.1.1/setup.py` & `registry_factory-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,288 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: registry-factory
+Version: 0.1.2
+Summary: Abstract codebase with utilities to register generic modules.
+Home-page: https://github.com/aidd-msca/registry-factory
+License: MIT
+Keywords: registry,factory,codebase,module registry,accreditation system
+Author: Peter Hartog
+Author-email: peter.hartog@hotmail.nl
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Project-URL: Repository, https://github.com/aidd-msca/registry-factory
+Description-Content-Type: text/markdown
 
-packages = \
-['registry_factory', 'registry_factory.checks', 'registry_factory.patterns']
+# RegistryFactory
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/registry-factory.svg)](https://badge.fury.io/py/registry-factory)
+[![PyPI](https://img.shields.io/github/license/aidd-msca/registry-factory)](LICENSE)
+![PyPI](https://img.shields.io/pypi/pyversions/registry-factory)
+[![GitHub Repo stars](https://img.shields.io/github/stars/aidd-msca/registry-factory)](https://github.com/aidd-msca/registry-factory/stargazers)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jlyEd1yxhvFCN82YqEFI82q2n0k_y06F?usp=sharing)
 
-setup_kwargs = {
-    'name': 'registry-factory',
-    'version': '0.1.1',
-    'description': 'Abstract codebase with utilities to register generic modules.',
-    'long_description': '# RegistryFactory\n\n![PyPI](https://img.shields.io/pypi/v/registry-factory)\n![PyPI](https://img.shields.io/pypi/pyversions/registry-factory)\n![PyPI](https://img.shields.io/github/license/aidd-msca/registry-factory)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jlyEd1yxhvFCN82YqEFI82q2n0k_y06F?usp=sharing)\n\nAn abstract implementation of the software design pattern called registry proposed in (Hartog et. al., 2023),\nproviding a factory for creating registries to which categorically similar modules can be organized.\n\n**Content:**\n**[Installation](#installation)**\n| **[Dependencies](#dependencies)**\n| **[Usage](#usage)**\n| **[Citation](#citation)**\n| **[Code of Conduct](#code-of-conduct)**\n\n### Overview\n\nThe registry design patterns provides a way to organize modular\nfunctionalities dynamically and achieve a unified, reusable, and interchangeable interface.\nIt extends the Factory design pattern without the explicit class dependency.\nAdditionally, the registry supports optional meta information such as versioning, accreditation,\ntesting, etc.\nThe UML diagrams show the differences between the factory and registry patterns.\n\n<p align="center">\n  <br>\n  <img alt="UML diagram of the pattern" src="figures/registry_uml.png">\n  <br>\n<i>Created with BioRender.com</i>\n </p>\n\n## Installation\n\nThe codebase can be installed from PyPI using `pip`, or your package manager of choice, with\n\n```bash\n$ pip install registry-factory\n```\n\n## Dependencies\n\nNo third-party dependencies are required to use the minimal functionality of the RegistryFactory.\n\n## Usage\n\nThe workflow of creating a registry is the following. 1) Identify a part of the code that can be\nseparated from the rest. 2) Modularize the section to be independent of the rest of the code. 3)\nCreate a registry from the RegistryFactory. 4) Register any modules that provide similar\nfunctionalities. 5) Call the optional module from the registry from the main workflow. See below.\n\n<p align="center">\n  <br>\n  <img alt="Workflow" src="figures/registry_creation.png" width="750">\n  <br>\n<i>Created with BioRender.com</i>\n </p>\n\nFurther available options and use-cases are described in the following sections.\n\n### A basic registry\n\nA simple registry is created as such.\n\n```Python\nfrom registry_factory.factory import Factory\n\nclass Registries(Factory):\n    TestRegistry = Factory.create_registry(shared=False)\n```\n\nNext, any models can be added to the ModelRegistry as such.\n\n```Python\nimport torch.nn as nn\n\n@Registries.ModelRegistry.register(call_name="simple_model")\nclass SimpleModel(nn.Module):\n    ...\n```\n\n### Shared modules\n\nA registry can be created to store shared modules. Shared modules are modules that are used in multiple registries (e.g. a model and a module).\n\n```Python\nfrom registry_factory.factory import Factory\n\nclass Registries(Factory):\n    ModelRegistry = Factory.create_registry(shared=True)\n    ModuleRegistry = Factory.create_registry(shared=True)\n\n@Registries.ModelRegistry.register(call_name="encoder")\nclass Encoder(nn.Module):\n    ...\n\nRegistries.ModuleRegistry.get("encoder")\n```\n\n### Arguments\n\nA registry can be created to store modules with arguments. The arguments can be set when registering a module.\n\n```Python\nfrom registry_factory.factory import Factory\n\nclass Registries(Factory):\n    ModelRegistry = Factory.create_registry(shared=True)\n\n@Registries.ModelRegistry.register_arguments(key="simple_model")\n@dataclass\nclass SimpleModelArguments:\n    input_size: int\n    output_size: int\n```\n\nOnly dataclasses can be used as arguments.\n\n### Versioning and accreditation\n\nTwo examples of additional meta information that can be stored in a registry is module versioning\nand accreditation regarding how and to who credit should be attributed the module.\n\nVersioning can be used to keep track of changes in a module. The version can be set when registering a module.\n\n```Python\nfrom registry_factory.factory import Factory\nfrom registry_factory.checks.versioning import Versioning\n\nclass Registries(Factory):\n    ModelRegistry = Factory.create_registry(checks=[Versioning(forced=False)])\n\n@Registries.ModelRegistry.register(call_name="simple_model", version="1.0.0")\nclass SimpleModel(nn.Module):\n    ...\n\nRegistries.ModelRegistry.get("simple_model") # Error, version not specified.\nRegistries.ModelRegistry.get("simple_model", version="1.0.0") # Returns the module.\n```\n\nAccreditation can be used to keep track of how and to who credit should be attributed the module.\nThe accreditation can be set when registering a module.\n\n```Python\nfrom registry_factory.factory import Factory\nfrom registry_factory.checks.accreditation import Accreditation\n\nclass Registries(Factory):\n    ModelRegistry = Factory.create_registry(checks=[Accreditation(forced=False)])\n\n@Registries.ModelRegistry.register(\n    call_name="simple_model",\n    author="Author name",\n    credit_type="reference",\n    additional_information="Reference published work in (link)."\n)\nclass SimpleModel(nn.Module):\n    ...\n\nRegistries.ModelRegistry.get("simple_model")  # Returns the module.\nRegistries.ModelRegistry.get_info("simple_model")  # Returns all meta information including the accreditation information.\n```\n\nThe reason why accreditation can return an object without specification is because the accreditation does not have "key" information. In the versioning module, the version is the key information which is used to grab the module from the registry. Without specifying the version, the registry will not know which module to return. In the accreditation module, the author, credit type, and additional information are not key information. Without specifying the author, credit type, and additional information, the registry will still know which module to return.\n\n### Testing and Factory Patterns\n\nWe also provide defining tests and post checks applied to all modules in a registry. Define test\nor post checks as follows when creating the registry.\n\n```Python\nclass Pattern:\n    """Test pattern."""\n\n    def __init__(self):\n        pass\n\n    def hello_world(self):\n        """Hello world."""\n        print("Hello world")\n\nclass Registries(Factory):\n    ModelRegistry = Factory.create_registry(\n        shared=False, checks=[FactoryPattern(factory_pattern=Pattern, forced=False)]\n    )\n\n# No error, the module passes the test.\n@ModelRegistry.register(\n    call_name="hello_world"\n)\nclass HelloWorld(Pattern):\n    pass\n\n# No error, the module passes the test.\n@ModelRegistry.register(\n    call_name="hello_world2"\n)\nclass HelloWorld:\n    def __init__(self):\n        pass\n\n    def hello_world(self):\n        """Hello world."""\n        print("Hello world")\n\n# Error, the module does not pass the test.\n@ModelRegistry.register(\n    call_name="hello_world2"\n)\nclass HelloWorld:\n    def __init__(self):\n        pass\n\n    def goodday_world(self):\n        """Good day world."""\n        print("Good day world")\n```\n\nThe factory also supports adding a callable test module to the registry. The callable test module can be specified to be called when a module is registered. The callable test module can be used to test the module when it is registered. The callable test module can be specified as follows when creating the registry.\n\n```Python\nclass CallableTestModule:\n    """Module to test."""\n\n    def __init__(self, key: str, obj: Any, **kwargs):\n        self.name = obj\n        self.assert_name()\n\n    def assert_name(self):\n        assert self.name == "test", "Name is not test"\n\n\n\nclass Registries(Factory):\n    ModelRegistry = Factory.create_registry(\n        shared=False, checks=[Testing(test_module=CallableTestModule, forced=True)]\n    )\n\nRegistries.ModelRegistry.register_prebuilt(key="name_test", obj="test") # No error, the module passes the test.\n```\n\n## Citation\n\nOur paper in which we propose the registry design pattern, on which this package is built, is currently\navailable as a preprint. If you make use of the design pattern or this package please cite our work accordingly.\n\n!!!!!! ADD PAPER LINK !!!!!!\n\n<!-- ```\n@inproceedings{hartog2023registry,\n    title={Registry: a design pattern to promote code reuse in machine learning-based drug discovery},\n    author={Hartog, Peter and Svensson, Emma and Mervin, Lewis and Genheden, Samuel and Engkvist, Ola and Tetko, Igor},\n    year={2023},\n    note={Preprint}\n}\n``` -->\n\n### Funding\n\nThe work behind this package has received funding from the European Union’s Horizon 2020\nresearch and innovation programme under the Marie Skłodowska-Curie\nActions, grant agreement “Advanced machine learning for Innovative Drug\nDiscovery (AIDD)” No 956832”. [Homepage](https://ai-dd.eu/).\n\n![plot](figures/aidd.png)\n\n## Code of Conduct\n\nEveryone interacting in the codebase, issue trackers, chat rooms, and mailing lists is expected to follow the\n[PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).\n',
-    'author': 'Peter Hartog',
-    'author_email': 'peter.hartog@hotmail.nl',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/aidd-msca/registry-factory',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+An abstract implementation of the software design pattern called registry proposed in (Hartog et. al., 2023),
+providing a factory for creating registries to which categorically similar modules can be organized.
+
+**[Installation](#installation)**
+| **[Dependencies](#dependencies)**
+| **[Usage](#usage)**
+| **[Citation](#citation)**
+
+### Overview
+
+The registry design patterns provides a way to organize modular
+functionalities dynamically and achieve a unified, reusable, and interchangeable interface.
+It extends the Factory design pattern without the explicit class dependency.
+Additionally, the registry supports optional meta information such as versioning, accreditation,
+testing, etc.
+The UML diagrams show the differences between the factory and registry patterns.
+
+<p align="center">
+  <br>
+  <img alt="UML diagram of the pattern" src="figures/registry_uml.png">
+  <br>
+<i>Created with BioRender.com</i>
+ </p>
+
+## Installation
+
+The codebase can be installed from PyPI using `pip`, or your package manager of choice, with
+
+```bash
+$ pip install registry-factory
+```
+
+## Dependencies
+
+No third-party dependencies are required to use the minimal functionality of the RegistryFactory.
+
+## Usage
+
+The workflow of creating a registry is the following. 1) Identify a part of the code that can be
+separated from the rest. 2) Modularize the section to be independent of the rest of the code. 3)
+Create a registry from the RegistryFactory. 4) Register any modules that provide similar
+functionalities. 5) Call the optional module from the registry from the main workflow. See below.
+
+<p align="center">
+  <br>
+  <img alt="Workflow" src="figures/registry_creation.png" width="750">
+  <br>
+<i>Created with BioRender.com</i>
+ </p>
+
+Further available options and use-cases are described in the following sections.
+
+### A basic registry
+
+A simple registry is created as such.
+
+```Python
+from registry_factory.factory import Factory
+
+class Registries(Factory):
+    TestRegistry = Factory.create_registry(shared=False)
+```
+
+Next, any models can be added to the ModelRegistry as such.
+
+```Python
+import torch.nn as nn
+
+@Registries.ModelRegistry.register(call_name="simple_model")
+class SimpleModel(nn.Module):
+    ...
+```
+
+### Shared modules
+
+A registry can be created to store shared modules. Shared modules are modules that are used in multiple registries (e.g. a model and a module).
+
+```Python
+from registry_factory.factory import Factory
+
+class Registries(Factory):
+    ModelRegistry = Factory.create_registry(shared=True)
+    ModuleRegistry = Factory.create_registry(shared=True)
+
+@Registries.ModelRegistry.register(call_name="encoder")
+class Encoder(nn.Module):
+    ...
+
+Registries.ModuleRegistry.get("encoder")
+```
+
+### Arguments
+
+A registry can be created to store modules with arguments. The arguments can be set when registering a module.
+
+```Python
+from registry_factory.factory import Factory
+
+class Registries(Factory):
+    ModelRegistry = Factory.create_registry(shared=True)
+
+@Registries.ModelRegistry.register_arguments(key="simple_model")
+@dataclass
+class SimpleModelArguments:
+    input_size: int
+    output_size: int
+```
+
+Only dataclasses can be used as arguments.
+
+### Versioning and accreditation
+
+Two examples of additional meta information that can be stored in a registry is module versioning
+and accreditation regarding how and to who credit should be attributed the module.
+
+Versioning can be used to keep track of changes in a module. The version can be set when registering a module.
+
+```Python
+from registry_factory.factory import Factory
+from registry_factory.checks.versioning import Versioning
+
+class Registries(Factory):
+    ModelRegistry = Factory.create_registry(checks=[Versioning(forced=False)])
+
+@Registries.ModelRegistry.register(call_name="simple_model", version="1.0.0")
+class SimpleModel(nn.Module):
+    ...
+
+Registries.ModelRegistry.get("simple_model") # Error, version not specified.
+Registries.ModelRegistry.get("simple_model", version="1.0.0") # Returns the module.
+```
+
+Accreditation can be used to keep track of how and to who credit should be attributed the module.
+The accreditation can be set when registering a module.
+
+```Python
+from registry_factory.factory import Factory
+from registry_factory.checks.accreditation import Accreditation
+
+class Registries(Factory):
+    ModelRegistry = Factory.create_registry(checks=[Accreditation(forced=False)])
+
+@Registries.ModelRegistry.register(
+    call_name="simple_model",
+    author="Author name",
+    credit_type="reference",
+    additional_information="Reference published work in (link)."
+)
+class SimpleModel(nn.Module):
+    ...
+
+Registries.ModelRegistry.get("simple_model")  # Returns the module.
+Registries.ModelRegistry.get_info("simple_model")  # Returns all meta information including the accreditation information.
+```
+
+The reason why accreditation can return an object without specification is because the accreditation does not have "key" information. In the versioning module, the version is the key information which is used to grab the module from the registry. Without specifying the version, the registry will not know which module to return. In the accreditation module, the author, credit type, and additional information are not key information. Without specifying the author, credit type, and additional information, the registry will still know which module to return.
+
+### Testing and Factory Patterns
+
+We also provide defining tests and post checks applied to all modules in a registry. Define test
+or post checks as follows when creating the registry.
+
+```Python
+class Pattern:
+    """Test pattern."""
+
+    def __init__(self):
+        pass
+
+    def hello_world(self):
+        """Hello world."""
+        print("Hello world")
+
+class Registries(Factory):
+    ModelRegistry = Factory.create_registry(
+        shared=False, checks=[FactoryPattern(factory_pattern=Pattern, forced=False)]
+    )
+
+# No error, the module passes the test.
+@ModelRegistry.register(
+    call_name="hello_world"
+)
+class HelloWorld(Pattern):
+    pass
+
+# No error, the module passes the test.
+@ModelRegistry.register(
+    call_name="hello_world2"
+)
+class HelloWorld:
+    def __init__(self):
+        pass
+
+    def hello_world(self):
+        """Hello world."""
+        print("Hello world")
+
+# Error, the module does not pass the test.
+@ModelRegistry.register(
+    call_name="hello_world2"
+)
+class HelloWorld:
+    def __init__(self):
+        pass
+
+    def goodday_world(self):
+        """Good day world."""
+        print("Good day world")
+```
+
+The factory also supports adding a callable test module to the registry. The callable test module can be specified to be called when a module is registered. The callable test module can be used to test the module when it is registered. The callable test module can be specified as follows when creating the registry.
+
+```Python
+class CallableTestModule:
+    """Module to test."""
+
+    def __init__(self, key: str, obj: Any, **kwargs):
+        self.name = obj
+        self.assert_name()
+
+    def assert_name(self):
+        assert self.name == "test", "Name is not test"
+
+
+
+class Registries(Factory):
+    ModelRegistry = Factory.create_registry(
+        shared=False, checks=[Testing(test_module=CallableTestModule, forced=True)]
+    )
+
+Registries.ModelRegistry.register_prebuilt(key="name_test", obj="test") # No error, the module passes the test.
+```
+
+## Citation
+
+Our paper in which we propose the registry design pattern, on which this package is built, is currently
+available as a preprint. If you make use of the design pattern or this package please cite our work accordingly.
+
+!!!!!! ADD PAPER LINK !!!!!!
+
+<!-- ```
+@inproceedings{hartog2023registry,
+    title={Registry: a design pattern to promote code reuse in machine learning-based drug discovery},
+    author={Hartog, Peter and Svensson, Emma and Mervin, Lewis and Genheden, Samuel and Engkvist, Ola and Tetko, Igor},
+    year={2023},
+    note={Preprint}
 }
+``` -->
+
+### Funding
+
+The work behind this package has received funding from the European Union’s Horizon 2020
+research and innovation programme under the Marie Skłodowska-Curie
+Actions, grant agreement “Advanced machine learning for Innovative Drug
+Discovery (AIDD)” No 956832”. [Homepage](https://ai-dd.eu/).
 
+![plot](figures/aidd.png)
 
-setup(**setup_kwargs)
```

