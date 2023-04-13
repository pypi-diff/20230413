# Comparing `tmp/pysros-22.7.2.tar.gz` & `tmp/pysros-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysros-22.7.2.tar", last modified: Fri Sep 16 22:46:22 2022, max compression
+gzip compressed data, was "pysros-23.3.1.tar", last modified: Fri Mar 17 22:30:59 2023, max compression
```

## Comparing `pysros-22.7.2.tar` & `pysros-23.3.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 22:46:22.354499 pysros-22.7.2/
--rw-r--r--   0 runner    (1001) docker     (121)    17026 2022-09-16 22:46:13.000000 pysros-22.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-09-16 22:46:22.354499 pysros-22.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-09-16 22:46:13.000000 pysros-22.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 22:46:22.354499 pysros-22.7.2/pysros/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7404 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/identifier.py
--rw-r--r--   0 runner    (1001) docker     (121)    41692 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/management.py
--rw-r--r--   0 runner    (1001) docker     (121)    18309 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    22497 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/model_path.py
--rw-r--r--   0 runner    (1001) docker     (121)    19504 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/model_walker.py
--rw-r--r--   0 runner    (1001) docker     (121)    26080 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/pprint.py
--rw-r--r--   0 runner    (1001) docker     (121)    29523 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/request_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11951 2022-09-16 22:46:13.000000 pysros-22.7.2/pysros/yang_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 22:46:22.354499 pysros-22.7.2/pysros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-09-16 22:46:22.000000 pysros-22.7.2/pysros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-16 22:46:22.000000 pysros-22.7.2/pysros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 22:46:22.000000 pysros-22.7.2/pysros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-16 22:46:22.000000 pysros-22.7.2/pysros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-16 22:46:22.000000 pysros-22.7.2/pysros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 22:46:22.354499 pysros-22.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-16 22:46:13.000000 pysros-22.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:30:59.166184 pysros-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-03-17 22:30:50.000000 pysros-23.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-17 22:30:59.166184 pysros-23.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-17 22:30:50.000000 pysros-23.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:30:59.166184 pysros-23.3.1/pysros/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58667 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26080 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46775 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/request_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/yang_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:30:59.166184 pysros-23.3.1/pysros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 22:30:59.166184 pysros-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-17 22:30:50.000000 pysros-23.3.1/setup.py
```

### Comparing `pysros-22.7.2/LICENSE.md` & `pysros-23.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysros-22.7.2/PKG-INFO` & `pysros-23.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 22.7.2
+Version: 23.3.1
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
```

### Comparing `pysros-22.7.2/README.md` & `pysros-23.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pysros-22.7.2/pysros/errors.py` & `pysros-23.3.1/pysros/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from .exceptions import *
 from .exceptions import make_exception
 
 __doc__ = """This module contains error definitions for pySROS.
 
 .. reviewed by PLM 20211201
-.. reviewed by TechComms 21211202
+.. reviewed by TechComms 20211202
 """
 
+pysros_err_action_subtree_not_supported = (SrosMgmtError, """Md-compare subtree-path is not supported in action method, use compare method instead""")
 pysros_err_arg_must_be_string = (TypeError, """Argument "module" must be a string""")
 pysros_err_attr_cannot_be_deleted = (AttributeError, "'{obj}' object attribute '{attribute}' cannot be deleted")
 pysros_err_attr_is_read_only = (AttributeError, "'{obj:.50}' object attribute '{attribute:.100}' is read-only")
 pysros_err_can_check_state_from_running_only = (SrosMgmtError, "State can be checked from running datastore only")
 pysros_err_can_get_state_from_running_only = (LookupError, "State can be retrieved from running datastore only")
 pysros_err_can_have_one_semicolon = (InvalidPathError, "Identifier can contain only one ':'")
 pysros_err_can_not_find_yang = (ModelProcessingError, "Cannot find yang '{yang_name}'")
 pysros_err_cannot_call_go_to_parent = (InvalidPathError, "Cannot call go_to_parent on root")
 pysros_err_cannot_delete_from_state = (SrosMgmtError, "Cannot delete from state tree")
-pysros_err_cannot_find_module_set_id_or_content_id = (RuntimeError, "Cannot find module-set-id or content-id")
 pysros_err_cannot_lock_and_unlock_running = (SrosMgmtError, "Cannot lock and unlock running config")
 pysros_err_cannot_modify_config = (SrosMgmtError, "Cannot modify running config")
 pysros_err_cannot_modify_state = (SrosMgmtError, "Cannot modify state tree")
 pysros_err_cannot_pars_path = (ModelProcessingError, "Cannot parse path {path!r}")
 pysros_err_cannot_remove_node = (ModelProcessingError, "Cannot remove {node}")
 pysros_err_cannot_specify_non_key_leaf = (InvalidPathError, "Cannot specify non-key leaf as path attribute")
 pysros_err_commit_conflicts_detected = (SrosConfigConflictError, "Commit failed - conflict detected, configuration changes cleared")
@@ -35,23 +35,24 @@
 pysros_err_even_num_of_columns_required = (ValueError, "Even number of data columns required")
 pysros_err_expected_end_bracket = (InvalidPathError, "Expected ']'")
 pysros_err_expected_equal_operator = (InvalidPathError, "Expected '='")
 pysros_err_filter_empty_string = (SrosMgmtError, "Cannot filter by an empty string")
 pysros_err_filter_not_supported_on_leaves = (InvalidPathError, "Filter is not supported for leaves")
 pysros_err_filter_should_be_dict = (TypeError, "Filter argument should be a dict")
 pysros_err_filter_wrong_leaf_value = (TypeError, "Unsupported leaf filter for '{leaf_name}'")
-pysros_err_incorrect_leaf_value = (TypeError, "Value {value!r} is not correct for leaf {leaf_name}")
+pysros_err_incorrect_leaf_value = (SrosMgmtError, "Invalid value for leaf {leaf_name}")
 pysros_err_invalid_align = (ValueError, "Invalid align: '{align}'")
 pysros_err_invalid_col_description = (TypeError, "Invalid column description")
 pysros_err_invalid_config = (ModelProcessingError, "Invalid config statement")
 pysros_err_invalid_identifier = (InvalidPathError, "Invalid identifier")
+pysros_err_invalid_json_structure = (ValueError, "Invalid JSON structure")
 pysros_err_invalid_key_in_path = (SrosMgmtError, "Invalid key value in path")
 pysros_err_invalid_module_set_id_or_content_id = (RuntimeError, "Invalid module-set-id")
-pysros_err_invalid_operation_on_key = (InvalidPathError, "Operation can not be performed on key")
-pysros_err_invalid_operation_on_leaflist = (InvalidPathError, "Operation can not be performed on leaflist")
+pysros_err_invalid_operation_on_key = (InvalidPathError, "Operation cannot be performed on key")
+pysros_err_invalid_operation_on_leaflist = (InvalidPathError, "Operation cannot be performed on leaflist")
 pysros_err_invalid_path_operation_missing_keys = (InvalidPathError, "Cannot perform operation on list without specifying keys")
 pysros_err_invalid_target = (ValueError, "Invalid target")
 pysros_err_invalid_transport = (TypeError, "Currently only NETCONF transport is supported")
 pysros_err_invalid_value = (TypeError, "MO contents not a dict '{data}'")
 pysros_err_invalid_value_for_type = (TypeError, "Invalid value for {type}: {value}")
 pysros_err_invalid_yang_path = (ModelProcessingError, "Invalid path {path!r}")
 pysros_err_key_val_mismatch = (SrosMgmtError, "Cannot change value of key-leaf '{key_name}'")
@@ -60,17 +61,14 @@
 pysros_err_missing_keys = (InvalidPathError, "Missing keys on element '{element}'")
 pysros_err_no_data_found = (LookupError, "No data found")
 pysros_err_not_connected = (RuntimeError, "Not connected")
 pysros_err_not_found_slash_before_name = (InvalidPathError, "'/' not found before element name")
 pysros_err_path_should_be_string = (TypeError, "path argument should be a string")
 pysros_err_prefix_does_not_have_ns = (LookupError, "prefix '{prefix}' of '{name}' does not have corresponding namespace")
 pysros_err_root_path = (InvalidPathError, "Operation cannot be performed on root")
-pysros_err_schema_box_keys_mismatch = (ModelProcessingError, "Keys in schema do not correspond to keys returned by box, '{schema_keys}' - '{box_keys}'")
-pysros_err_server_dos_not_have_required_yang_lib = (RuntimeError, "NETCONF server does not have required yang-library")
-pysros_err_server_dos_not_have_yang_lib = (RuntimeError, "NETCONF server does not have yang-library capability")
 pysros_err_target_should_be_list = (InvalidPathError, "Target should be a list")
 pysros_err_type_must_be = (TypeError, "must be {expected:.50s}, not {actual:.50s}")
 pysros_err_unended_quoted_string = (InvalidPathError, "Unended quoted string")
 pysros_err_unexpected_change_of_path_ctx = (ModelProcessingError, "Unexpected change of path ctx")
 pysros_err_unexpected_end_of_yang = (ModelProcessingError, "Unexpected end of YANG")
 pysros_err_unexpected_token = (ModelProcessingError, "Unexpected token {token}")
 pysros_err_unexpected_value_of_type = (TypeError, "Unexpected value of type '{val_type}' in '{type}'")
@@ -85,7 +83,23 @@
 pysros_err_unresolved_leafref = (InternalError, "Unresolved leafref {type}")
 pysros_err_unresolved_type = (InternalError, "Unresolved type in schema: {type}")
 pysros_err_unsupported_set_method = (SrosMgmtError, "Unsupported set method")
 pysros_err_unsupported_type_for_wrapper = (TypeError, "Unsupported type for {wrapper_name} data")
 pysros_err_use_deepcopy = (NotImplementedError, "Use '.deepcopy' instead")
 pysros_err_wrong_netconf_response = (SrosMgmtError, "Wrong NETCONF response")
 pysros_err_wrong_rhs = (ModelProcessingError, "Invalid argument to the right of the plus symbol")
+pysros_err_unsupported_compare_method = (SrosMgmtError, "Unsupported compare method")
+pysros_err_unsupported_compare_datastore = (SrosMgmtError, "Compare is only supported against the candidate datastore")
+pysros_err_unsupported_compare_endpoint = (InvalidPathError, "Unsupported compare path endpoint")
+pysros_err_unsupported_action_path = (InvalidPathError, "Path does not point to an action")
+pysros_err_unsupported_convert_method = (SrosMgmtError, "Unsupported convert method")
+pysros_err_unsupported_action_io = (SrosMgmtError, "Unsupported value of argument action_io")
+pysros_err_invalid_rd_state = (InternalError, "Invalid database state")
+pysros_err_convert_root_not_support_pysros = (SrosMgmtError, "'pysros' format is not supported for root")
+pysros_err_convert_wrong_payload_type = (TypeError, "Invalid payload type for convert")
+pysros_err_wrong_json_root = (JsonDecodeError, "JSON root must be object")
+pysros_err_malformed_xml = (ValueError, "Malformed XML")
+pysros_err_multiple_occurences_of_node = (SrosMgmtError, "Multiple occurrences of node")
+pysros_err_multiple_occurences_of_entry = (SrosMgmtError, "Multiple occurrences of list entry")
+pysros_err_convert_invalid_value_for_type = (SrosMgmtError, "Invalid value for {name}")
+pysros_err_invalid_xml_element = (ValueError, 'XML element {element} can be empty or contain another XML element')
+pysros_err_invalid_xml_root = (ValueError, 'XML root element can be empty or contain another XML element')
```

### Comparing `pysros-22.7.2/pysros/exceptions.py` & `pysros-23.3.1/pysros/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2021 Nokia
 
-__all__ = ("SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError", )
+__all__ = ("SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError", )
 
 __doc__ = """This module contains exceptions for error handling within pySROS.
 
 .. reviewed by PLM 20211201
 .. reviewed by TechComms 20211202
 """
 
@@ -74,14 +74,22 @@
     completes with a ``terminated-incomplete`` status.
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     pass
 
+class JsonDecodeError(Exception):
+    """Exception raised when parsing json input fail."""
+    pass
+
+class XmlDecodeError(Exception):
+    """Exception raised when parsing xml input fail."""
+    pass
+
 def make_exception(arg, **kwarg):
     """Create an exception.
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     return arg[0](arg[1].format(**kwarg))
```

### Comparing `pysros-22.7.2/pysros/identifier.py` & `pysros-23.3.1/pysros/identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2021 Nokia
 
 import re
 
 from .errors import *
-from .wrappers import _Singleton
+from .singleton import _Singleton
 
 class LazyBindModule(metaclass=_Singleton):
     def __str__(self):
         return f"{self.__class__.__name__}()"
 
     def __hash__(self):
         return id(self)
```

### Comparing `pysros-22.7.2/pysros/management.py` & `pysros-23.3.1/pysros/management.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 from enum import Enum, auto
 from typing import NamedTuple, Tuple
 
 from lxml import etree
 from ncclient import manager
 from ncclient.operations.rpc import RPCError as nc_RPCError
 from ncclient.transport.errors import TransportError as nc_TransportError
-from ncclient.xml_ import new_ele, to_ele
+from ncclient.xml_ import new_ele, new_ele_nsmap, to_ele
 
 from .errors import *
 from .model import Model
 from .model_builder import ModelBuilder
-from .model_walker import FilteredDataModelWalker
-from .request_data import RequestData
-from .wrappers import Empty, Container, Leaf, LeafList
+from .model_walker import FilteredDataModelWalker, ActionInputFilteredDataModelWalker, ActionOutputFilteredDataModelWalker
+from .request_data import RequestData, COMMON_NAMESPACES
+from .singleton import Empty
+from .wrappers import Container, Leaf, LeafList
 
-__all__ = ("connect", "sros", "Connection", "Datastore", "Empty", "SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError",)
+__all__ = ("connect", "sros", "Connection", "Datastore", "Empty", "SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError", )
 __doc__ = """This module contains basic primitives for managing an SR OS node.
 It contains functions to obtain and manipulate configuration and state data.
 
 .. reviewed by PLM 20210624
 .. reviewed by TechComms 20210713
 """
 
@@ -62,15 +63,15 @@
     :param rebuild: Trigger the rebuild of an already cached YANG schema.
     :type rebuild: bool, optional
     :param timeout: Timeout of the transport protocol, in seconds. Default 300.
     :type timeout: int, optional
     :param hostkey_verify: Enables hostkey verification using the SSH known_hosts file. Default True.
     :type hostkey_verify: bool, optional
     :return: Connection object for specific SR OS node.
-    :rtype: .Connection
+    :rtype: :py:class:`Connection`
     :raises RuntimeError: Error occurred during creation of connection
     :raises ModelProcessingError: Error occurred during compilation of the YANG modules
 
 
     .. note ::
 
        When executing a Python application using the pySROS libraries on a remote workstation,
@@ -87,17 +88,17 @@
 
        from pysros.management import connect
        from pysros.exceptions import ModelProcessingError
        import sys
 
        def get_connection():
            try:
-               connection_object = connect(host="192.168.74.51",
-                                           username="admin",
-                                           password="admin")
+               connection_object = connect(host="192.168.1.1",
+                                           username="myusername",
+                                           password="mypassword")
            except RuntimeError as runtime_error:
                print("Failed to connect.  Error:", runtime_error)
                sys.exit(-1)
            except ModelProcessingError as model_proc_error:
                print("Failed to create model-driven schema.  Error:", model_proc_error)
                sys.exit(-2)
            return connection_object
@@ -112,17 +113,17 @@
 
        from pysros.management import connect
        from pysros.exceptions import ModelProcessingError
        import sys
 
        def get_connection():
            try:
-               connection_object = connect(host="192.168.74.51",
-                                           username="admin",
-                                           password="admin",
+               connection_object = connect(host="192.168.1.1",
+                                           username="myusername",
+                                           password="mypassword",
                                            yang_directory="./YANG")
            except RuntimeError as runtime_error:
                print("Failed to connect.  Error:", runtime_error)
                sys.exit(-1)
            except ModelProcessingError as model_proc_error:
                print("Failed to create model-driven schema.  Error:", model_proc_error)
                sys.exit(-2)
@@ -184,55 +185,51 @@
     :vartype running: .Datastore
     :ivar candidate: candidate datastore
     :vartype candidate: .Datastore
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
-    _common_namespaces = {
-        "ncbase": "urn:ietf:params:xml:ns:netconf:base:1.0",
-        "monitoring": "urn:ietf:params:xml:ns:yang:ietf-netconf-monitoring",
-        "library": "urn:ietf:params:xml:ns:yang:ietf-yang-library",
-        "nokiaoper": "urn:nokia.com:sros:ns:yang:sr:oper-global",
-    }
 
     def __init__(self, *args, yang_directory, rebuild, **kwargs):
         try:
             self._nc        = manager.connect_ssh(*args, **kwargs)
         except Exception as e:
             raise make_exception(pysros_err_could_not_create_conn, reason=e) from None
 
         self.running    = Datastore(self, 'running')
         self.candidate  = Datastore(self, 'candidate')
 
         self.yang_directory = yang_directory
         self.rebuild = rebuild
         self._models    = self._get_yang_models()
         self._ns_map    = types.MappingProxyType({model.name: model.namespace for model in self._models})
+        self._mod_revs  = {model.name: model.revision for model in self._models}
         self.root = self._get_root(self._models)
+        self.debug      = False
 
     def _get_root(self, modules):
         hasher = hashlib.sha256()
         yangs = sorted(modules, key = lambda m: m.name)
-        hasher.update(b"Schema ver 2\n")
+        hasher.update(b"Schema ver 5\n")
         for m in yangs:
             hasher.update(f"mod:{m.name};rev:{m.revision};".encode())
             for sm in sorted(m.submodules, key = lambda sm: sm.name):
                 hasher.update(f" smod:{sm.name};srev:{sm.revision};".encode())
         cache_dir = pathlib.Path.home() / '.pysros' / 'cache'
         cache_name_txt = f"model_{base64.b32encode(hasher.digest()).decode('utf-8')}.ver"
         cache_name = cache_dir / cache_name_txt
 
         if not self.rebuild:
             with contextlib.suppress(FileNotFoundError):
                 with cache_name.open("rb") as f:
                     return Model(pickle.load(f), 0, None)
 
         # attempt to pickle. If load fails, we need to create a new tree
-        model_builder = ModelBuilder(self._yang_getter)
+        model_builder = ModelBuilder(self._yang_getter, self._ns_map)
         for mod in yangs:
             model_builder.register_yang(mod.name)
         model_builder.process_all_yangs()
 
         cache_dir.mkdir(mode=0o755, exist_ok=True, parents = True)
         # write to temp file instead of locking file
         # make hard link to correct name before close + unlink
@@ -256,82 +253,138 @@
 
         # download using netconf protocol
         if debug:
             start = datetime.datetime.now()
             print(f"GET SCHEMA {yang_name}")
 
         response = self._nc.get_schema(yang_name)
-        data = response.xpath("/ncbase:rpc-reply/monitoring:data", self._common_namespaces)[0].text
+        data = response.xpath("/ncbase:rpc-reply/monitoring:data", COMMON_NAMESPACES)[0].text
         if debug:
             print(f" * {len(data)/1024:.1f} kB downloaded in {(datetime.datetime.now()-start).total_seconds():.3f} sec")
 
         return data
 
     def _find_module(self, yang_name):
         if os.path.isfile(f"""{self.yang_directory}/nokia-combined/{yang_name}.yang"""):
             return f"""{self.yang_directory}/nokia-combined/{yang_name}.yang"""
+        if yang_name in self._ns_map: #module
+            for candidate in pathlib.Path(self.yang_directory).rglob(f"{yang_name}*.yang"):
+                if candidate.parts and re.fullmatch(f"{yang_name}[@]{self._mod_revs[yang_name]}.yang", str(candidate.parts[-1])):
+                    return candidate
         for candidate in pathlib.Path(self.yang_directory).rglob(f"{yang_name}*.yang"):
-            if candidate.parts and re.fullmatch(f"{yang_name}(?:[@]\\d{{4}}[-]\\d{{2}}[-]\\d{{2}})?.yang", str(candidate.parts[-1])):
+            if candidate.parts and re.fullmatch(f"{yang_name}.yang", str(candidate.parts[-1])):
                 return candidate
         raise make_exception(pysros_err_can_not_find_yang, yang_name=yang_name)
 
-    def _get_module_set_id(self):
-        caps = list(self._nc.server_capabilities)
-        yang_cap = list(filter(lambda x: x.startswith("urn:ietf:params:netconf:capability:yang-library:"), self._nc.server_capabilities))
-        if len(yang_cap) == 0:
-            raise make_exception(pysros_err_server_dos_not_have_yang_lib)
-        if yang_cap[0].find("yang-library:1.0") != -1:
-            match = re.search("module-set-id=([^&]*)", yang_cap[0])
-        elif yang_cap[0].find("yang-library:1.1") != -1:
-            match = re.search("content-id=([^&]*)", yang_cap[0])
-        else:
-            raise make_exception(pysros_err_server_dos_not_have_required_yang_lib)
-        if match is None:
-            raise make_exception(pysros_err_cannot_find_module_set_id_or_content_id)
-        return match.group(1)
-
     def _get_yang_models(self):
         subtree = to_ele("""
             <modules-state xmlns="urn:ietf:params:xml:ns:yang:ietf-yang-library">
                 <module-set-id/>
                 <module/>
             </modules-state>""")
         with self._process_connected():
             yangs_resp = self._nc.get(filter=("subtree", subtree))
-        module_set_id = yangs_resp.xpath(
-            "/ncbase:rpc-reply/ncbase:data/library:modules-state/library:module-set-id",
-            self._common_namespaces
-        )[0].text
-
-        if module_set_id != self._get_module_set_id():
-            raise make_exception(pysros_err_invalid_module_set_id_or_content_id)
 
         result = []
         modules = yangs_resp.xpath(
             "/ncbase:rpc-reply/ncbase:data/library:modules-state/library:module",
-            self._common_namespaces
+            COMMON_NAMESPACES
         )
 
-        get_text = lambda e, path: e.findtext(path, namespaces=self._common_namespaces)
+        get_text = lambda e, path: e.findtext(path, namespaces=COMMON_NAMESPACES)
         for m in modules:
             submodules = []
-            for sm in m.xpath("./library:submodule", namespaces=self._common_namespaces):
+            for sm in m.xpath("./library:submodule", namespaces=COMMON_NAMESPACES):
                 submodules.append(YangSubmodule(
                     name      = get_text(sm, "./library:name"),
                     revision  = get_text(sm, "./library:revision"),
                 ))
             submodules.sort(key = lambda sm: sm.name)
             result.append(YangModule(
                 name       = get_text(m, "./library:name"),
                 namespace  = get_text(m, "./library:namespace"),
                 revision   = get_text(m, "./library:revision"),
                 submodules = tuple(submodules)
             ))
         return tuple(result)
 
+    def _action(self, path, value):
+        rd = RequestData(self.root, self._ns_map, walker=ActionInputFilteredDataModelWalker)
+        current = rd.process_path(path)
+        if not current.is_action():
+            raise make_exception(pysros_err_unsupported_action_path)
+        if current._walker.current.name.name == "md-compare" and "path" in value and "subtree-path" in value["path"]:
+            raise make_exception(pysros_err_action_subtree_not_supported)
+        current.set(value)
+
+        xml_action = etree.Element(f"""{{{COMMON_NAMESPACES["yang_1_0"]}}}action""")
+        xml_action.extend(rd.to_xml())
+
+        if self.debug:
+            print("ACTION request")
+            print(etree.dump(xml_action))
+
+        response = self._nc.rpc(xml_action)
+
+        if self.debug:
+            print("ACTION response")
+            print(response)
+
+        del rd
+        rd = RequestData(self.root, self._ns_map, walker=ActionOutputFilteredDataModelWalker)
+        rd.set_action_as_xml(path, response)
+        current = rd.process_path(path, strict=True)
+        return current.to_model()
+
+    def _convert(self, path, payload, src_fmt, dst_fmt, pretty_print, action_io):
+        def convert_walker(action_io):
+            if action_io == "input":
+                return ActionInputFilteredDataModelWalker
+            elif action_io == "output":
+                return ActionOutputFilteredDataModelWalker
+            raise make_exception(pysros_err_unsupported_action_io)
+
+        if not all(fmt in ("xml", "json", "pysros") for fmt in (src_fmt, dst_fmt)):
+            raise make_exception(pysros_err_unsupported_convert_method)
+        rd = RequestData(self.root, self._ns_map, action=RequestData._Action.convert, walker=convert_walker(action_io))
+        current = rd.process_path(path)
+
+        if src_fmt == "pysros":
+            current.set(payload)
+        elif src_fmt == "xml":
+            if not isinstance(payload, str):
+                raise make_exception(pysros_err_convert_wrong_payload_type)
+            try:
+                data = to_ele(f"<dummy-root>{payload}</dummy-root>")
+            except Exception as e:
+                raise XmlDecodeError(*e.args)
+            current.set_as_xml(data)
+        elif src_fmt == "json":
+            if not isinstance(payload, str):
+                raise make_exception(pysros_err_convert_wrong_payload_type)
+            current.set_as_json(payload)
+        else:
+            raise NotImplementedError()
+
+        if dst_fmt == "pysros":
+            return current.to_model()
+        elif dst_fmt == "xml":
+            root = current.to_xml()
+            xml_output=""
+            for subtree in root:
+                if pretty_print:
+                    etree.indent(subtree, space="    ")
+                    if xml_output:  xml_output += "\n"
+                xml_output += etree.tostring(subtree).decode("utf-8")
+            return xml_output
+        elif dst_fmt == "json":
+            return current.to_json(pretty_print)
+        else:
+            raise NotImplementedError()
+
     @contextlib.contextmanager
     def _process_connected(self):
         try:
             if  not self._nc.connected:
                 # test wether connection is not disconected before start of the body
                 raise make_exception(pysros_err_not_connected)
             yield
@@ -375,31 +428,185 @@
                                                  with ``terminated-incomplete`` status.
 
         .. code-block:: python
            :caption: Example
            :name: pysros-cli
 
            from pysros.management import connect
-           connection_object = connect(host='192.168.1.1', username='admin', password='admin')
+           connection_object = connect(host='192.168.1.1', username='myusername', password='mypassword')
            print(connection_object.cli('show version'))
 
-        .. Reviewed by PLM 20211201
-        .. Reviewed by TechComms 20211202
+        .. Reviewed by PLM 20220901
         """
         with self._process_connected():
             output = self._nc.md_cli_raw_command(command)
-        status = output.xpath("/ncbase:rpc-reply/nokiaoper:status", self._common_namespaces)
+        status = output.xpath("/ncbase:rpc-reply/nokiaoper:status", COMMON_NAMESPACES)
         if status and status[0].text == "terminated-incomplete":
-            errors = output.xpath("/ncbase:rpc-reply/nokiaoper:error-message", self._common_namespaces)
+            errors = output.xpath("/ncbase:rpc-reply/nokiaoper:error-message", COMMON_NAMESPACES)
             errors = [e.text.strip() for e in errors]
             args = errors or ["MINOR: MGMT_AGENT #2007: Operation failed"]
             raise ActionTerminatedIncompleteError(*args)
-        output = output.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-cli-output-block", self._common_namespaces)
+        output = output.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-cli-output-block", COMMON_NAMESPACES)
         return output[0].text if output else ""
 
+    def action(self, path, value={}):
+        """Perform a YANG modeled action on SR OS by providing the *json-instance-path* to the
+        action statement in the chosen operations YANG model, and the pySROS data structure to
+        match the YANG modeled input for that action.
+        This method provides structured data input and output for available operations.
+
+        :param path: *json-instance-path* to the YANG action.
+        :type path: str
+        :param value: pySROS data structure providing the input data for the chosen action.
+        :type value: pySROS data structure
+        :returns: YANG modeled, structured data representing the output of the modeled action (operation)
+        :rtype: pySROS data structure
+
+        .. code-block:: python
+           :caption: Example calling the **ping** YANG modeled action (operation)
+           :name: pysros-action-example
+
+           >>> from pysros.management import connect
+           >>> from pysros.pprint import printTree
+           >>> connection_object = connect(host='192.168.1.1',
+           ... username='myusername', password='mypassword')
+           >>> path = '/nokia-oper-global:global-operations/ping'
+           >>> input_data = {'destination': '172.16.100.101'}
+           >>> output = connection_object.action(path, input_data)
+           >>> output
+           Container({'operation-id': Leaf(12), 'start-time': Leaf('2022-09-08T22:21:32.6Z'), 'results': Container({'test-parameters': Container({'destination': Leaf('172.16.100.101'), 'count': Leaf(5), 'output-format': Leaf('detail'), 'do-not-fragment': Leaf(False), 'fc': Leaf('nc'), 'interval': Leaf('1'), 'pattern': Leaf('sequential'), 'router-instance': Leaf('Base'), 'size': Leaf(56), 'timeout': Leaf(5), 'tos': Leaf(0), 'ttl': Leaf(64)}), 'probe': {1: Container({'probe-index': Leaf(1), 'status': Leaf('response-received'), 'round-trip-time': Leaf(2152), 'response-packet': Container({'size': Leaf(64), 'source-address': Leaf('172.16.100.101'), 'icmp-sequence-number': Leaf(1), 'ttl': Leaf(64)})}), 2: Container({'probe-index': Leaf(2), 'status': Leaf('response-received'), 'round-trip-time': Leaf(2097), 'response-packet': Container({'size': Leaf(64), 'source-address': Leaf('172.16.100.101'), 'icmp-sequence-number': Leaf(2), 'ttl': Leaf(64)})}), 3: Container({'probe-index': Leaf(3), 'status': Leaf('response-received'), 'round-trip-time': Leaf(2223), 'response-packet': Container({'size': Leaf(64), 'source-address': Leaf('172.16.100.101'), 'icmp-sequence-number': Leaf(3), 'ttl': Leaf(64)})}), 4: Container({'probe-index': Leaf(4), 'status': Leaf('response-received'), 'round-trip-time': Leaf(2164), 'response-packet': Container({'size': Leaf(64), 'source-address': Leaf('172.16.100.101'), 'icmp-sequence-number': Leaf(4), 'ttl': Leaf(64)})}), 5: Container({'probe-index': Leaf(5), 'status': Leaf('response-received'), 'round-trip-time': Leaf(1690), 'response-packet': Container({'size': Leaf(64), 'source-address': Leaf('172.16.100.101'), 'icmp-sequence-number': Leaf(5), 'ttl': Leaf(64)})})}, 'summary': Container({'statistics': Container({'packets': Container({'sent': Leaf(5), 'received': Leaf(5), 'loss': Leaf('0.0')}), 'round-trip-time': Container({'minimum': Leaf(1690), 'average': Leaf(2065), 'maximum': Leaf(2223), 'standard-deviation': Leaf(191)})})})}), 'status': Leaf('completed'), 'end-time': Leaf('2022-09-08T22:21:36.9Z')})
+           >>> printTree(output)
+           +-- operation-id: 13
+           +-- start-time: 2022-09-08T22:23:21.2Z
+           +-- results:
+           |   +-- test-parameters:
+           |   |   +-- destination: 172.16.100.101
+           |   |   +-- count: 5
+           |   |   +-- output-format: detail
+           |   |   +-- do-not-fragment: False
+           |   |   +-- fc: nc
+           |   |   +-- interval: 1
+           |   |   +-- pattern: sequential
+           |   |   +-- router-instance: Base
+           |   |   +-- size: 56
+           |   |   +-- timeout: 5
+           |   |   +-- tos: 0
+           |   |   `-- ttl: 64
+           |   +-- probe:
+           |   |   +-- 1:
+           |   |   |   +-- probe-index: 1
+           |   |   |   +-- status: response-received
+           |   |   |   +-- round-trip-time: 2159
+           |   |   |   `-- response-packet:
+           |   |   |       +-- size: 64
+           |   |   |       +-- source-address: 172.16.100.101
+           |   |   |       +-- icmp-sequence-number: 1
+           |   |   |       `-- ttl: 64
+           |   |   +-- 2:
+           |   |   |   +-- probe-index: 2
+           |   |   |   +-- status: response-received
+           |   |   |   +-- round-trip-time: 2118
+           |   |   |   `-- response-packet:
+           |   |   |       +-- size: 64
+           |   |   |       +-- source-address: 172.16.100.101
+           |   |   |       +-- icmp-sequence-number: 2
+           |   |   |       `-- ttl: 64
+           |   |   +-- 3:
+           |   |   |   +-- probe-index: 3
+           |   |   |   +-- status: response-received
+           |   |   |   +-- round-trip-time: 2098
+           |   |   |   `-- response-packet:
+           |   |   |       +-- size: 64
+           |   |   |       +-- source-address: 172.16.100.101
+           |   |   |       +-- icmp-sequence-number: 3
+           |   |   |       `-- ttl: 64
+           |   |   +-- 4:
+           |   |   |   +-- probe-index: 4
+           |   |   |   +-- status: response-received
+           |   |   |   +-- round-trip-time: 2084
+           |   |   |   `-- response-packet:
+           |   |   |       +-- size: 64
+           |   |   |       +-- source-address: 172.16.100.101
+           |   |   |       +-- icmp-sequence-number: 4
+           |   |   |       `-- ttl: 64
+           |   |   `-- 5:
+           |   |       +-- probe-index: 5
+           |   |       +-- status: response-received
+           |   |       +-- round-trip-time: 1735
+           |   |       `-- response-packet:
+           |   |           +-- size: 64
+           |   |           +-- source-address: 172.16.100.101
+           |   |           +-- icmp-sequence-number: 5
+           |   |           `-- ttl: 64
+           |   `-- summary:
+           |       `-- statistics:
+           |           +-- packets:
+           |           |   +-- sent: 5
+           |           |   +-- received: 5
+           |           |   `-- loss: 0.0
+           |           `-- round-trip-time:
+           |               +-- minimum: 1735
+           |               +-- average: 2038
+           |               +-- maximum: 2159
+           |               `-- standard-deviation: 153
+           +-- status: completed
+           `-- end-time: 2022-09-08T22:23:25.4Z
+
+        .. Reviewed by PLM 20220908
+
+        """
+        with self._process_connected():
+            return self._action(path, value)
+
+    def convert(self, path, payload, *, source_format, destination_format, pretty_print=False, action_io="output"):
+        """Returns converted version of the input data (payload) in the destination format.
+
+        The input data must be valid according to the YANG schema for the :py:class:`Connection`
+        object that :py:meth:`convert` is being called against.
+
+        :param path: *json-instance-path* to the location in the YANG schema that the
+                     payload uses as its YANG modeled root.
+        :type path: str
+        :param payload: Input data for conversion.  The payload must be valid data according
+                        to the YANG schema associated with the :py:class:`Connection` object and
+                        should be in the format as defined in the ``source_format`` argument.
+                        For ``pySROS``, the payload must be a pySROS data structure.  For
+                        ``xml`` or ``json``, the payload must be a *string* containing valid XML
+                        or JSON IETF data.
+        :type payload: pySROS data structure, str
+        :param source_format: Format of the input data.  Valid options are ``xml``, ``json``, or ``pysros``.
+        :type source_format: str
+        :param destination_format: Format of the output data. Valid options are ``xml``, ``json``, or ``pysros``.
+        :type destination_format: str
+        :param pretty_print: Format the output for human consumption.
+        :type pretty_print: bool, optional
+        :param action_io: When converting the input/output of a YANG modeled operation (action), it is possible
+                          for there to be conflicting fields in the input and output sections of the YANG.  This
+                          parameter selects whether to consider the payload against the ``input`` or ``output``
+                          section of the YANG. Default: ``output``.
+        :type action_io: str, optional
+        :returns: Data structure of the same format as ``destination_format``.
+        :rtype: pySROS data structure, str
+
+        An example of the :py:meth:`convert` function can be found in
+        the :ref:`Converting Data Formats` section.
+
+        .. note:: Any metadata associated with a YANG node is currently not converted.  Metadata
+                  includes SR OS configuration comments as well as more general metadata such as
+                  insert or delete operations defined in XML attributes.  If metadata is provided
+                  in the payload in XML or JSON format, it is stripped from the
+                  resulting output. Attention should be given to converting the output
+                  of the ``compare summary netconf-rpc`` MD-CLI command.
+
+        .. Reviewed by PLM 20221123
+        .. Reviewed by TechComms 20221124
+        """
+        return self._convert(path, payload, source_format, destination_format, pretty_print, action_io)
+
+
 class Datastore:
     """Datastore object that can be used to perform multiple operations on a specified datastore.
 
     .. Reviewed by PLM 20210614
     .. Reviewed by TechComms 20210705
     """
     class _SetAction(Enum):
@@ -490,15 +697,15 @@
             #two possible scenarions - entry does not exists or is empty
             #if has presence and LookupError is raised, it does not exists
             if model_walker.has_explicit_presence() and not filter:
                 raise e from None
             if model_walker.get_dds() == Model.StatementType.list_:
                 res = OrderedDict() if model_walker.current.user_ordered else {}
             else:
-                res = Container._with_module({}, model_walker.get_name().prefix)
+                res = Container._with_model({}, model_walker.current)
 
             model_walker_copy = model_walker.copy()
             #doing exists to check whether really exists or not
             model_walker_copy.go_to_last_with_presence()
             if model_walker_copy.is_root:
                 return res
             else:
@@ -513,26 +720,28 @@
         if self.target == 'running':
             raise make_exception(pysros_err_cannot_modify_config)
         if method != 'merge' and method != 'replace':
             raise make_exception(pysros_err_unsupported_set_method)
         model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
         if model_walker.current.config == False:
             raise make_exception(pysros_err_cannot_modify_state)
-        config = new_ele("config")
         rd = RequestData(self.connection.root, self.connection._ns_map)
         if action == Datastore._SetAction.delete:
             default_operation="none"
             rd.process_path(path).delete()
         else:
             default_operation="merge"
             current = rd.process_path(path)
             current.set(value)
             if method == "replace":
                 current.replace()
-        config.extend(rd.to_xml())
+        children = rd.to_xml()
+        config = new_ele_nsmap("config", rd._extra_namespaces)
+
+        config.extend(children)
         if self.debug:
             print("SET request")
             print(f"path: '{path}', value: '{value}'")
             print(etree.dump(config))
         self.nc.edit_config(target=self.target, default_operation=default_operation, config=config)
 
     def _delete(self, path):
@@ -606,14 +815,73 @@
                     self._get(path, custom_walker=model_walker_copy)
                 except LookupError:
                     raise e from None
                 return []
 
         return [*current.to_model()]
 
+    def _compare(self, output_format, user_path):
+        if self.target == 'running':
+            raise make_exception(pysros_err_unsupported_compare_datastore)
+        if output_format not in ("md-cli", "xml"):
+            raise make_exception(pysros_err_unsupported_compare_method)
+
+        path = user_path if user_path != "/" else ""
+
+        if path:
+            model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
+            if model_walker.current.config == False:
+                raise make_exception(pysros_err_unsupported_compare_endpoint)
+            rd = RequestData(self.connection.root, self.connection._ns_map)
+            current = rd.process_path(model_walker)
+            if not current.is_compare_supported_endpoint():
+                raise make_exception(pysros_err_unsupported_compare_endpoint)
+            path = rd.to_xml()
+
+        op_ns = COMMON_NAMESPACES["nokiaoper"]
+        xml_action = etree.Element(f"""{{{COMMON_NAMESPACES["yang_1_0"]}}}action""")
+        xml_gl_op = etree.SubElement(xml_action, f"{{{op_ns}}}global-operations")
+        xml_md_cmp = etree.SubElement(xml_gl_op, f"{{{op_ns}}}md-compare")
+        if path:
+            xml_path = etree.SubElement(xml_md_cmp, f"{{{op_ns}}}path")
+            xml_sbtr_path = etree.SubElement(xml_path, f"{{{op_ns}}}subtree-path")
+            xml_sbtr_path.extend(path)
+        xml_fmt = etree.Element(f"{{{op_ns}}}format")
+        xml_fmt.text=output_format if output_format == "xml" else "md-cli"
+        xml_md_cmp.append(xml_fmt)
+        xml_src = etree.SubElement(xml_md_cmp, f"{{{op_ns}}}source")
+        xml_src.append(etree.Element(f"{{{op_ns}}}{self.target}"))
+        xml_dst = etree.SubElement(xml_md_cmp, f"{{{op_ns}}}destination")
+        xml_dst.append(etree.Element(f"{{{op_ns}}}baseline"))
+
+        if self.debug:
+            print("COMPARE request")
+            print(etree.dump(xml_action))
+
+        reply = self.nc.rpc(xml_action)
+
+        if self.debug:
+            print("COMPARE reply")
+            print(reply)
+
+        if output_format == "md-cli":
+            return reply.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-compare-output/text()")[0].strip()
+
+        xml_output=""
+        for subtree in reply.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-compare-output/*"):
+            subtree.getparent().remove(subtree)
+            xml_output+=etree.tostring(subtree).decode("utf-8")
+
+        if xml_output:
+            xml_trees = etree.fromstring(f"<root>{xml_output}</root>", parser=etree.XMLParser(remove_blank_text=True))
+            for xml_tree in xml_trees:
+                etree.indent(xml_tree, space="    ")
+            return "\n".join(etree.tostring(xml_tree, pretty_print=True).decode("utf-8").strip() for xml_tree in xml_trees)
+        return ""
+
     def _commit(self):
         try:
             self.nc.commit()
         except nc_RPCError as e:
             if e.message and e.message.find("MGMT_CORE #2703:") > -1:
                 self.nc.discard_changes()
                 self.nc.commit()
@@ -665,31 +933,31 @@
            :caption: Example
            :name: pysros-management-datastore-get-example-usage
 
             from pysros.management import connect
             import sys
 
             connection_object = connect()
-           try:
-               oper_name = connection_object.running.get("/nokia-state:state/system/oper-name")
-           except RuntimeError as runtime_error:
-               print("Runtime Error:", runtime_error)
-               sys.exit(100)
-           except InvalidPathError as invalid_path_error:
-               print("Invalid Path Error:", invalid_path_error)
-               sys.exit(101)
-           except SrosMgmtError as sros_mgmt_error:
-               print("SR OS Management Error:", sros_mgmt_error)
-               sys.exit(102)
-           except TypeError as type_error:
-               print("Type Error:", type_error)
-               sys.exit(103)
-           except InternalError as internal_error:
-               print("Internal Error:", internal_error)
-               sys.exit(104)
+            try:
+                oper_name = connection_object.running.get("/nokia-state:state/system/oper-name")
+            except RuntimeError as runtime_error:
+                print("Runtime Error:", runtime_error)
+                sys.exit(100)
+            except InvalidPathError as invalid_path_error:
+                print("Invalid Path Error:", invalid_path_error)
+                sys.exit(101)
+            except SrosMgmtError as sros_mgmt_error:
+                print("SR OS Management Error:", sros_mgmt_error)
+                sys.exit(102)
+            except TypeError as type_error:
+                print("Type Error:", type_error)
+                sys.exit(103)
+            except InternalError as internal_error:
+                print("Internal Error:", internal_error)
+                sys.exit(104)
 
         .. code-block:: python
            :caption: Example using content node matching filters
            :name: pysros-management-datastore-get-example-content-node-filters
            :emphasize-lines: 5-7
 
            from pysros.management import connect
@@ -783,19 +1051,18 @@
            from pysros.management import connect
            from pysros.wrappers import *
 
            connection_object = connect()
            path = '/nokia-conf:configure/router[router-name="Base"]/interface[interface-name="demo1"]'
            data = Container({'interface-name': Leaf('demo1'), 'port': Leaf('1/1/c1/1:0'),
                   'ipv4': Container({'primary': Container({'prefix-length': Leaf(24),
-                  'address': Leaf('5.5.5.1')})}), 'admin-state': Leaf('enable')})
+                  'address': Leaf('192.168.100.1')})}), 'admin-state': Leaf('enable')})
            connection_object.candidate.set(path, data)
 
-        .. Reviewed by PLM 20211201
-        .. Reviewed by TechComms 20211202
+        .. Reviewed by PLM 20220901
         """
         with self.connection._process_connected():
             self._set(path, value, Datastore._SetAction.set, method)
             if commit:
                 self._commit()
 
     def delete(self, path, commit=True):
@@ -955,14 +1222,64 @@
         .. Reviewed by TechComms 20220624
         """
         with self.connection._process_connected():
             if self.target == 'running':
                 raise make_exception(pysros_err_cannot_modify_config)
             self.nc.discard_changes()
 
+
+    def compare(self, path="", *, output_format):
+        """Perform a comparison of the uncommitted candidate configuration with the baseline
+        configuration.
+        The output can be provided in XML or in MD-CLI format and provided in a format
+        where, if applied to the node, the resulting configuration would be the same as if the
+        candidate configuration is committed.
+
+        :param output_format: Specify output format of compare command. Supported formats are
+                              ``xml`` and ``md-cli``.  The ``md-cli`` output format displays similar output
+                              to that of the **compare summary** command on the MD-CLI.  The ``xml``
+                              output format displays similar output to that of the **compare summary netconf-rpc**
+                              MD-CLI command.
+        :type output_format: str
+        :param path: Specify json-instance-path to the location in the schema that the compare runs from.
+                     This is the root of the comparison.
+        :type path: str
+        :returns: The formatted differences between the configurations.
+        :rtype: str
+
+        .. note::
+           The :py:meth:`compare` method may only be called against the ``candidate`` configuration datastore.
+
+        .. code-block:: python
+           :caption: Example - Compare in XML format
+           :name: pysros-management-datastore-compare-example-usage-1
+           :emphasize-lines: 5,14
+
+           from pysros.management import connect
+
+           connection_object = connect()
+           path = '/nokia-conf:configure/policy-options/policy-statement[name="DEMO"]'
+           output_format = 'xml'
+
+           print("Current config in", path)
+           print(connection_object.candidate.get(path))
+
+           print("Deleting config in", path)
+           connection_object.candidate.delete(path, commit=False)
+
+           print("Comparing the candidate configuration to the baseline configuration in {} format".format(output_format))
+           print(connection_object.candidate.compare(output_format=output_format))
+
+        .. Reviewed by PLM 20220901
+        .. Reviewed by PLM 20221005
+
+        """
+        with self.connection._process_connected():
+            return self._compare(output_format, path)
+
     def __getitem__(self, path):
         return self.get(path)
 
     def __setitem__(self, path, value):
         self.set(path, value)
 
     def __delitem__(self, path):
```

### Comparing `pysros-22.7.2/pysros/model.py` & `pysros-23.3.1/pysros/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,14 +179,19 @@
         return res
 
 class BuildingModel(AModel):
     __slots__ = (
         "name",
         "children",
         "yang_type",
+        "units",
+        "namespace",
+        "default",
+        "mandatory",
+        "status",
         "presence_container",
         "user_ordered",
         "local_keys",
         "data_def_stm",
         "target_path",
         "identity_bases",
         "_parent",
@@ -194,14 +199,19 @@
         "blueprint",
     )
 
     def __init__(self, name: Identifier, data_def_stm: AModel.StatementType, parent):
         self.name = Identifier.builtin(name) if type(name) == str else name
         self.children: List[Model] = []
         self.yang_type: Optional[YangType] = None
+        self.units: Optional[str] = None
+        self.namespace: str = None
+        self.default: Optional[str] = None
+        self.mandatory: Optional[str] = None
+        self.status: Optional[str] = None
         self.presence_container = False
         self.user_ordered = False
         self.local_keys: List[str] = []
         self.data_def_stm = data_def_stm
         self.target_path = None
         self.parent = parent
         self.identity_bases = None if data_def_stm != AModel.StatementType.identity_ else []
@@ -269,24 +279,29 @@
     )
 
     class DataBitmask(IntFlag):
         data_def_stm        = 0xff
         presence_container  = 1 << 8
         user_ordered        = 1 << 9
         config              = 1 << 10
+        mandatory           = 1 << 11
+        status              = 1 << 12
 
     class DataMembers(IntEnum):
         name            = 0
         children        = 1
         yang_type       = 2
         local_keys      = 3
         target_path     = 4
         identity_bases  = 5
         parent          = 6
         bitmask         = 7
+        units           = 8
+        namespace       = 9
+        default         = 10
 
 class Model(StorageModel):
     """Class to represent a single YANG entry and hold additional information, such as type, configuration state, children, and data definition statement.
 
     .. Reviewed by TechComms 20210713
     """
     __slots__ = ("_data", "children", "parent", "name", "_bitmask", "data_def_stm",)
@@ -301,15 +316,15 @@
         self.parent = parent
 
     def __getattr__(self, name):
         getter = {
             "name": Model._name_getter,
             "children": Model._children_getter,
             "_bitmask": Model._bitmask_getter,
-            "data_def_stm": Model._data_def_stm_detter,
+            "data_def_stm": Model._data_def_stm_getter,
         }.get(name)
         if not getter:
             raise AttributeError(name)
         res = getter(self)
         setattr(self, name, res)
         return res
 
@@ -321,15 +336,15 @@
 
     def _children_getter(self):
         return [Model(self._storage, index, self) for index in self._data[Model.DataMembers.children]]
 
     def _bitmask_getter(self):
         return self._data[Model.DataMembers.bitmask]
 
-    def _data_def_stm_detter(self):
+    def _data_def_stm_getter(self):
         return Model.StatementType(int(self._bitmask & Model.DataBitmask.data_def_stm))
 
     @property
     def prefix(self):
         return self._data[Model.DataMembers.name][0]
 
     @property
@@ -345,14 +360,34 @@
         return self._data[Model.DataMembers.children]
 
     @property
     def yang_type(self):
         return self._data[Model.DataMembers.yang_type]
 
     @property
+    def units(self):
+        return self._data[Model.DataMembers.units]
+
+    @property
+    def namespace(self):
+        return self._data[Model.DataMembers.namespace]
+
+    @property
+    def default(self):
+        return self._data[Model.DataMembers.default]
+
+    @property
+    def mandatory(self):
+        return bool(self._bitmask & Model.DataBitmask.mandatory)
+
+    @property
+    def status(self):
+        return bool(self._bitmask & Model.DataBitmask.status)
+
+    @property
     def presence_container(self):
         return bool(self._bitmask & Model.DataBitmask.presence_container)
 
     @property
     def user_ordered(self):
         return bool(self._bitmask & Model.DataBitmask.user_ordered)
 
@@ -453,14 +488,60 @@
         return self._data[self.DataMembers.yang_type]
 
     @yang_type.setter
     def yang_type(self, value):
         self._data[self.DataMembers.yang_type] = value
 
     @property
+    def units(self):
+        return self._data[self.DataMembers.units]
+
+    @units.setter
+    def units(self, value):
+        self._data[self.DataMembers.units] = value
+
+    @property
+    def namespace(self):
+        return self._data[self.DataMembers.namespace]
+
+    @namespace.setter
+    def namespace(self, value):
+        self._data[self.DataMembers.namespace] = value
+
+    @property
+    def default(self):
+        return self._data[self.DataMembers.default]
+
+    @default.setter
+    def default(self, value):
+        self._data[self.DataMembers.default] = value
+
+    @property
+    def mandatory(self):
+        return bool(self._bitmask & self.DataBitmask.mandatory)
+
+    @mandatory.setter
+    def mandatory(self, value):
+        if value == "true":
+            self._bitmask |= int(self.DataBitmask.mandatory)
+        else:
+            self._bitmask &= int(~self.DataBitmask.mandatory)
+
+    @property
+    def status(self):
+        return bool(self._bitmask & self.DataBitmask.status)
+
+    @status.setter
+    def status(self, value):
+        if value in (None, "current", "deprecated"):
+            self._bitmask |= int(self.DataBitmask.status)
+        else:
+            self._bitmask &= int(~self.DataBitmask.status)
+
+    @property
     def presence_container(self):
         return bool(self._bitmask & self.DataBitmask.presence_container)
 
     @presence_container.setter
     def presence_container(self, value):
         if value:
             self._bitmask |= int(self.DataBitmask.presence_container)
@@ -578,8 +659,13 @@
         [],                                                                     # 1 = children
         None,                                                                   # 2 = yang_type
         [],                                                                     # 3 = local_keys
         None,                                                                   # 4 = target_path
         None if data_def_stm != Model.StatementType.identity_ else [],          # 5 = identity_bases
         parent if parent is None else parent._index,                            # 6 = parent
         data_def_stm.value | Model.DataBitmask.config,                          # 7 = bitmask
+        None,                                                                   # 8 = units
+        None,                                                                   # 9 = namespace
+        None,                                                                   # 10 = default
+        None,                                                                   # 11 = mandatory
+        None,                                                                   # 12 = status
     ]
```

### Comparing `pysros-22.7.2/pysros/model_builder.py` & `pysros-23.3.1/pysros/model_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Copyright 2021 Nokia
 
 import copy
 import xml.parsers.expat
 
 from collections import defaultdict
-from typing import Dict, DefaultDict, List, Set
+from typing import Dict, DefaultDict, List, Set, Union, Optional
 
 from .errors import *
 from .identifier import Identifier, NoModule, LazyBindModule
-from .model import Model, BuildingModel, StorageConstructionModel
+from .model import AModel, Model, BuildingModel, StorageConstructionModel
 from .model_path import ModelPath
 from .model_walker import ModelWalker, DataModelWalker
 from .tokenizer import yang_parser
-from .yang_type import IdentityRef, LeafRef, UnresolvedIdentifier, YangUnion, Enumeration, Bits, resolve_typedefs_deep, should_be_buildin, type_from_name
+from .yang_type import IdentityRef, LeafRef, PrimitiveType, UnresolvedIdentifier, YangType, YangTypeBase, YangUnion, Enumeration, Bits, should_be_buildin, type_from_name, DECIMAL_LEAF_TYPE, INTEGRAL_TYPES_MIN, INTEGRAL_TYPES_MAX, IP_TYPES
 
 class YangHandler:
     """Handler for yang processing."""
-    TAGS_WITH_MODEL = ("container", "list", "leaf", "typedef", "module", "submodule", "uses", "leaf-list", "import", "identity", "notification", "rpc", "input", "output", "choice", "case", "deviate")
+    TAGS_WITH_MODEL = ("container", "list", "leaf", "typedef", "module", "submodule", "uses", "leaf-list", "import", "identity", "notification", "rpc", "input", "output", "choice", "case", "deviate", "action")
     TAGS_FORCE_MODULE = ("grouping", "identity", "typedef", "uses", "augment", "deviation", "type", "base")
     TAGS_ARG_IS_IDENTIFIER = ("base", "type", )
     TAGS_ARG_IS_YANG_PATH_NOT_ABSOLUTE_SCHEMA_ID = ("path", )
-    assert not ({"config", "default", "mandatory", "max-elements", "min-elements", "must", "type", "unique", "units", } & set(TAGS_WITH_MODEL)), "Substmt of deviate can not have model"
+    assert not ({"config", "default", "fraction-digits", "length", "mandatory", "max-elements", "min-elements", "must", "range", "status", "type", "unique", "units", } & set(TAGS_WITH_MODEL)), "Substmt of deviate can not have model"
     TAGS_SHOULD_BE_PROCESSED = (
         "action",
         "anydata",
         "anyxml",
         "argument",
         "augment",
         "base",
@@ -155,15 +155,15 @@
         if self.ignore_depth:
             self.ignore_depth -= 1
             return
         if name == "grouping":
             self.grouping_depth -= 1
         elif name == "typedef":
             self.construct(self.model)
-            self.builder.types_to_resolve[self.model.name] = self.model.yang_type
+            self.builder.types_to_resolve[self.model.name] = TypeDefModel(self.model)
         elif name in ("action", "rpc"):
             for child in self.model.children:
                 if child.data_def_stm == BuildingModel.StatementType.input_:
                     break
             else:
                 self.enter("input", None)
                 self.leave("input")
@@ -257,19 +257,53 @@
 
     def handle_path(self, arg: str):
         if self.in_type:
             assert isinstance(self.last_yang_type, LeafRef)
             self.last_yang_type.set_path(arg)
 
     def handle_type(self, identifier: str):
-        if isinstance(self.model.yang_type, YangUnion):
-            self.model.yang_type.append(type_from_name(identifier))
-        else:
+        if not isinstance(self.model.yang_type, YangUnion):
             assert self.model.yang_type is None
             self.model.yang_type = type_from_name(identifier)
+        elif (identifier != Identifier.builtin('union')):
+            self.model.yang_type.append(type_from_name(identifier))
+
+    def handle_units(self, arg: str):
+        assert self.model.units is None
+        self.model.units = arg
+
+    def handle_namespace(self, arg: str):
+        assert self.model.namespace is None
+        self.model.namespace = arg
+
+    def handle_default(self, arg: str):
+        assert self.model.default is None
+        self.model.default = arg
+
+    def handle_mandatory(self, arg: str):
+        assert self.model.mandatory is None
+        self.model.mandatory = arg
+
+    def handle_range(self, arg: str):
+        assert isinstance(self.last_yang_type, (PrimitiveType, UnresolvedIdentifier))
+        assert self.last_yang_type.yang_range is None
+        self.last_yang_type.yang_range = arg
+
+    def handle_fraction_DASH_digits(self, arg: str):
+        assert isinstance(self.last_yang_type, (PrimitiveType, UnresolvedIdentifier))
+        assert self.last_yang_type.fraction_digits is None
+        self.last_yang_type.fraction_digits = int(arg)
+
+    def handle_length(self, arg: str):
+        assert isinstance(self.last_yang_type, (PrimitiveType, UnresolvedIdentifier))
+        assert self.last_yang_type.length is None
+        self.last_yang_type.length = arg
+
+    def handle_status(self, arg: str):
+        self.model.status = arg
 
     def handle_enum(self, value: str):
         if self.in_type:
             assert isinstance(self.last_yang_type, Enumeration), f"expected Enumeration, got {self.last_yang_type}"
             self.last_yang_type.add_enum(value)
 
     def handle_bit(self, value: str):
@@ -319,25 +353,26 @@
         self.model.config = (arg == 'true')
 
 def _dummy_getter(filename):
     assert False, "Missing getter"
 
 class ModelBuilder:
     """API for walking model tree."""
-    def __init__(self, yang_getter=_dummy_getter):
+    def __init__(self, yang_getter=_dummy_getter, ns_map={}):
         self.root = BuildingModel("root", BuildingModel.StatementType["container_"], None)
         self.types_to_resolve = dict()
         self.groupings = dict()
         self.resolved_types = dict()
         self.all_yangs = set()
         self.parsed_yangs = set()
         self.files_to_parse = []
         self.augments = []
         self.deviations = []
         self.registered_modules = {}
+        self._ns_map = ns_map
         self.yang_getter = yang_getter
 
     def get_module_content(self, yang_name):
         if yang_name in self.registered_modules:
             return self.registered_modules[yang_name]
         return self.yang_getter(yang_name)
 
@@ -368,17 +403,19 @@
 
     def resolve(self):
         self.resolve_groupings()
         self.resolve_augments()
         self.resolve_deviations()
         self.build_blueprints()
         self.resolve_typedefs()
+        self.resolve_type_ranges()
         self.resolve_identities()
         self.resolve_leafrefs()
         self.resolve_config()
+        self.resolve_namespaces()
         self.delete_blueprints()
         self.convert_model()
 
     def perform_parse(self, yang_name, yang_handler=None):
         if yang_name in self.parsed_yangs:
             return
         self.parsed_yangs.add(yang_name)
@@ -405,63 +442,128 @@
 
             for i in self.groupings[m.name].children:
                 i.deepcopy(m)
             m.recursive_walk(resolve_unresolved)
             return False
 
     def set_correct_types(self, m:BuildingModel):
-        if m.yang_type is None:
+        if isinstance(m.yang_type, (UnresolvedIdentifier, YangUnion)):
+            tdm = resolve_typedefs_deep(TypeDefModel(m), self.resolved_types)
+            m.yang_type         = tdm.yang_type
+            m.default           = tdm.default
+            m.units             = tdm.units
+
+    def resolve_typedefs(self):
+        for key, value in self.types_to_resolve.items():
+            assert not key in self.resolved_types
+            self.resolved_types[key] = resolve_typedefs_deep(value, self.types_to_resolve)
+            if key in IP_TYPES:
+                assert isinstance(self.resolved_types[key].yang_type, YangUnion)
+                self.resolved_types[key].yang_type.deduplicate()
+                assert len(self.resolved_types[key].yang_type) == 1 and self.resolved_types[key].yang_type._types[0].identifier.name == "string"
+                self.resolved_types[key].yang_type = self.resolved_types[key].yang_type._types[0]
+        self.root.recursive_walk(self.set_correct_types)
+
+    def set_correct_range(self, yt:YangTypeBase):
+        assert yt.json_name() != "decimal64" or yt.fraction_digits
+        if isinstance(yt, YangUnion):
+            for t in yt:
+                self.set_correct_range(t)
+
+        if not yt or not yt.json_name() in (*DECIMAL_LEAF_TYPE, "string", "binary"):    return
+        if yt.json_name() in ("string", "binary") and not yt.length:                    return
+
+        full_range = False if (yt.yang_range or yt.json_name() in ("string", "binary")) else True
+        work_range = yt.length if yt.json_name() in ("string", "binary") else yt.yang_range
+
+        if full_range: work_range = "min..max"
+        if yt.json_name() == "decimal64":
+            min_val = str(-2**63+1)
+            max_val = str(2**63-1)
+            min_val = min_val[:-yt.fraction_digits] + '.' + min_val[-yt.fraction_digits:]
+            max_val = max_val[:-yt.fraction_digits] + '.' + max_val[-yt.fraction_digits:]
+        elif yt.json_name() in ("string", "binary"):
+            min_val = str(0)
+            max_val = str(2**64-1)
+        else:
+            min_val = INTEGRAL_TYPES_MIN[yt.json_name()]
+            max_val = INTEGRAL_TYPES_MAX[yt.json_name()]
+
+        work_range = work_range.replace("min", min_val)
+        work_range = work_range.replace("max", max_val)
+
+        if full_range:
+            yt.yang_range = work_range
             return
 
-        if isinstance(m.yang_type, UnresolvedIdentifier):
-            m.yang_type = copy.deepcopy(resolve_typedefs_deep(m.yang_type, self.resolved_types))
+        # merge adjacent subranges, such as "0|1..100" to "0..100" or "0..10|11..20" to "0..20"
+        def process_subrange(subrange:str):
+            nonlocal yt
+            map_f       = float if yt.json_name() == "decimal64" else int
+            i_subrange  = list(map(map_f, subrange.split("..")))
+            assert len(i_subrange) in (1, 2)
+            return i_subrange if len(i_subrange) == 2 else 2 * i_subrange
+
+        subranges       = work_range.split("|")
+        res_subranges   = [process_subrange(subranges[0])]
+        for subrange in subranges[1:]:
+            i_subrange = process_subrange(subrange)
+            if res_subranges[-1][1] == i_subrange[0] - 1:
+                res_subranges[-1][1] = i_subrange[1]
+            else:
+                res_subranges.append(i_subrange)
 
-        if isinstance(m.yang_type, YangUnion):
-            m.yang_type = copy.deepcopy(resolve_typedefs_deep(m.yang_type, self.resolved_types))
+        res_subranges   = [subr if subr[0] != subr[1] else [subr[0]] for subr in res_subranges]
+        work_range      = "|".join(["..".join(map(str, subr)) for subr in res_subranges])
+        if yt.json_name() in ("string", "binary"):
+            yt.length       = work_range
+        else:
+            yt.yang_range   = work_range
 
-    def resolve_typedefs(self):
-        for name, value in self.types_to_resolve.items():
-            assert not name in self.resolved_types
-            self.resolved_types[name] = resolve_typedefs_deep(value, self.types_to_resolve)
-        self.root.recursive_walk(self.set_correct_types)
+    def resolve_type_ranges(self):
+        def setter(m:BuildingModel):
+            if isinstance(m.yang_type, YangTypeBase):
+                self.set_correct_range(m.yang_type)
+        self.root.recursive_walk(setter)
 
     def resolve_identities(self):
         # first step creates dict, where we find for each identity
         # its all identities, that are directly derived from it.
-        directly_derived: DefaultDict[Identifier, List[Identifier]] = defaultdict(list)
+        directly_derived: DefaultDict[Identifier, Set[Identifier]] = defaultdict(set)
         def find_derived(m:BuildingModel):
             if m.data_def_stm != BuildingModel.StatementType.identity_:
                 return
             for b in m.identity_bases:
-                directly_derived[b].append(m.name)
+                if m.status != 'obsolete':
+                    directly_derived[b].add(m.name)
 
         self.root.recursive_walk(find_derived)
         # second step adds all direct and indirect derived identities together
         def add_derived_recursive(result_set, id):
-            if id in result_set:
-                return
-            result_set.update(directly_derived.get(id, []))
-            for c in directly_derived.get(id, []):
+            got = directly_derived.get(id, set())
+            toUpdate = got - result_set
+            result_set.update(got)
+            for c in toUpdate:
                 add_derived_recursive(result_set, c)
 
         derived: Dict[Identifier, Set(Identifier)] = {}
         for id in directly_derived.keys():
             derived[id] = set()
             add_derived_recursive(derived[id], id)
 
         # last step iterates through all identityrefs and set possible values
         def identityref_set_value(m:BuildingModel):
             if m.yang_type is None:
                 return
             if type(m.yang_type) is IdentityRef:
-                m.yang_type.set_values(derived)
+                m.yang_type.set_values(derived, self._ns_map)
             elif type(m.yang_type) is YangUnion:
                 for st in m.yang_type:
                     if type(st) is IdentityRef:
-                        st.set_values(derived)
+                        st.set_values(derived, self._ns_map)
 
         self.root.recursive_walk(identityref_set_value)
 
     def resolve_leafrefs(self):
         def replace_leafrefs(m: BuildingModel):
             if not isinstance(m.yang_type, LeafRef):
                 return
@@ -548,14 +650,22 @@
                         if not depth:
                             w.current.blueprint = list(self.filter_blueprint(lambda b: b[0] != instruction[1][0], w.current.blueprint))
                         depth += 1 if instruction[0] else -1
                     w.current.blueprint = list(w.current.blueprint) + deviate.blueprint
                 if deviate.name.name == "not-supported":
                     w.current.delete_from_parent(quiet=False)
 
+    def resolve_namespaces(self):
+        def ns_set(m:BuildingModel):
+            if m.namespace or not m.name.prefix in self._ns_map.keys():
+                return
+            m.namespace = self._ns_map[m.name.prefix]
+        for root_child in self.root.children:
+            root_child.recursive_walk(ns_set)
+
     def build_blueprints(self):
         handler = YangHandler(self, self.root)
         handler.construct()
 
     def delete_blueprints(self):
         def deleter(m: BuildingModel):
             del m.blueprint
@@ -576,22 +686,119 @@
         w = DataModelWalker(self.root)
 
         stack = [new_root]
 
         def enter_fnc(w: DataModelWalker):
             nonlocal stack
             new = StorageConstructionModel(w.get_name(), w.get_dds(), stack[-1])
+            if isinstance(w.current.yang_type, YangUnion):
+                w.current.yang_type.deduplicate()
             new.yang_type = w.current.yang_type
+            new.units = w.current.units
+            new.namespace = w.current.namespace
+            new.default = w.current.default
+            new.mandatory = w.current.mandatory
+            new.status = w.current.status
             new.presence_container = w.current.presence_container
             new.user_ordered = w.current.user_ordered
             new.local_keys = w.current.local_keys
             new.target_path = w.current.target_path
             new.identity_bases = w.current.identity_bases
             new.config = w.current.config
             stack.append(new)
 
         def leave_fnc(w: DataModelWalker):
             nonlocal stack
             stack.pop()
 
         w.recursive_walk(enter_fnc=enter_fnc, leave_fnc=leave_fnc)
         self.root = Model(new_root._storage, new_root._index, None)
+
+class TypeDefModel:
+    __slots__ = ("yang_type", "default", "units")
+
+    def __init__(self, arg: Union[YangType, Model, BuildingModel], default: Optional[str] = None, units: Optional[str] = None) -> None:
+        assert isinstance(arg, (YangTypeBase, AModel))
+        if isinstance(arg, AModel):
+            self.yang_type          = arg.yang_type
+            self.default            = arg.default
+            self.units              = arg.units
+        else:
+            self.yang_type          = arg
+            self.default            = default
+            self.units              = units
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__) or self.__slots__ != other.__slots__:
+            return False
+        return all(getattr(self, name) == getattr(other, name) for name in self.__slots__)
+
+def merge_typedef_ranges(parent_range:str, child_range:str):
+    """
+    Vertically merge typedef integer ranges across typedef parent and child
+    - keep child's integer range values (non-'min' or 'max')
+    - replace child's 'min'/'max' strings with integer min or max values if present in parent
+    - return child's ranges as-is if parent has no range defined or child has no 'max' or 'min'
+    examples:
+        - parent typedef range "1..200", child type range "min..100", result "1..100"
+        - parent typedef range "1..200", child type range "100..max", result "100..200"
+        - parent typedef range is None, child type range "100..max", result "100..max"
+        - parent typedef range is '1..200', child type range "50..150", result "50..150"
+    """
+    if not parent_range:
+        return child_range
+
+    min_val     = parent_range.split("|")[0].split("..")[0]
+    child_range = child_range.replace("min", min_val)
+    max_val     = parent_range.split("|")[-1].split("..")[-1]
+    child_range = child_range.replace("max", max_val)
+
+    return child_range
+
+def resolve_typedefs_shallow(t: TypeDefModel, typedefs: Dict[Identifier, TypeDefModel]):
+    assert isinstance(t.yang_type, YangTypeBase)
+    yang_type, default, units = t.yang_type, t.default, t.units
+    while type(yang_type) is UnresolvedIdentifier and yang_type.identifier in typedefs:
+        r_model = typedefs[yang_type.identifier]
+        u_range = yang_type.yang_range
+        frac_d  = yang_type.fraction_digits
+        length  = yang_type.length
+        if any((u_range, frac_d, length)):
+            yang_type = copy.copy(r_model.yang_type)
+            if u_range:
+                yang_type.yang_range = merge_typedef_ranges(yang_type.yang_range, u_range)
+            if frac_d:
+                yang_type.fraction_digits = frac_d
+            if length:
+                yang_type.length = length
+        else:
+            yang_type = r_model.yang_type
+        default = default   or r_model.default
+        units   = units     or r_model.units
+
+    assert not isinstance(yang_type, UnresolvedIdentifier), f"Cannot resolve type {yang_type}"
+    assert isinstance(yang_type, YangTypeBase)
+    return TypeDefModel(
+        copy.copy(yang_type),
+        default,
+        units,
+    )
+
+def resolve_typedefs_deep(m: TypeDefModel, typedefs: Dict[Identifier, TypeDefModel]):
+    m = resolve_typedefs_shallow(m, typedefs)
+    if not isinstance(m.yang_type, YangUnion):
+        return m
+
+    u_yang_type, u_default, u_units = YangUnion(), None, None
+    for sub in m.yang_type:
+        tdm = resolve_typedefs_deep(TypeDefModel(sub), typedefs)
+        if type(tdm.yang_type) == YangUnion:
+            for t in tdm.yang_type:
+                u_yang_type.append(t)
+        else:
+            u_yang_type.append(tdm.yang_type)
+        u_default   = tdm.default
+        u_units     = tdm.units
+    m.yang_type         = u_yang_type
+    m.default           = m.default         or u_default
+    m.units             = m.units           or u_units
+    return m
```

### Comparing `pysros-22.7.2/pysros/model_path.py` & `pysros-23.3.1/pysros/model_path.py`

 * *Files identical despite different names*

### Comparing `pysros-22.7.2/pysros/model_walker.py` & `pysros-23.3.1/pysros/model_walker.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.value = ''
 
 class ModelWalker:
     """API representation for walking model tree.
 
     .. Reviewed by TechComms 20210712
     """
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.augment_, Model.StatementType.notification_, Model.StatementType.rpc_, Model.StatementType.input_, Model.StatementType.output_, Model.StatementType.choice_, Model.StatementType.case_)
+    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.augment_, Model.StatementType.notification_, Model.StatementType.rpc_, Model.StatementType.input_, Model.StatementType.output_, Model.StatementType.choice_, Model.StatementType.case_, Model.StatementType.action_)
     _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.grouping_, Model.StatementType.augment_)
 
     def __init__(self, model:Model):
         self.path = []
         self.keys = []
         while model.parent is not None:
             if model.data_def_stm in self._expected_dds:
@@ -75,34 +75,34 @@
                     raise InvalidPathError(*e.args) from None
                 continue
 
             if p.name == '..':
                 self.go_to_parent()
                 continue
 
-            namespace = self.path[-1].name.prefix if self.path else module
-            assert namespace
+            prefix = self.path[-1].name.prefix if self.path else module
+            assert prefix
 
             try:
                 self.go_to_child(
-                    Identifier(namespace, p.name))
+                    Identifier(prefix, p.name))
             except SrosMgmtError as e:
                 raise InvalidPathError(*e.args) from None
 
-    def check_child_field_value(self, name:Union[str, Identifier], value):
+    def check_child_field_value(self, name:Union[str, Identifier], value, *, json=False):
         with self.visit_child(name):
-            return self.check_field_value(value)
+            return self.check_field_value(value, json=json)
 
-    def check_field_value(self, value):
+    def check_field_value(self, value, *, json=False):
         if self.get_dds() == Model.StatementType.leaf_list_:
             if not isinstance(value, list):
                 raise make_exception(pysros_err_leaflist_should_be_list, type_name=value.__class__.__name__)
-            return all(self.get_type().check_field_value(i) for i in value)
+            return all(self.get_type().check_field_value(i, json) for i in value)
         elif self.get_dds() == Model.StatementType.leaf_:
-            return self.get_type().check_field_value(value)
+            return self.get_type().check_field_value(value, json)
         else:
             assert False, "Checking field value for non-field walker"
 
     def get_parent(self):
         res = self.__class__(self.model)
         if self.path:
             res.path = self.path[:-1]
@@ -140,16 +140,16 @@
                 i = (i,)
             if (len(self.get_local_key_names()) != len(i)):
                 return False
             if not all(self.check_child_field_value(key_name, key_val) for key_name, key_val in zip(self.get_local_key_names(), i)):
                 return False
         return all(isinstance(v, (dict, Container)) for v in value.values())
 
-    def entry_keys(self, value:"EntryKeysDictProxy"):
-        def correct_key(entry:"EntryKeysDictProxy", key):
+    def entry_keys(self, value:"DictionaryKeysProxy"):
+        def correct_key(entry:"DictionaryKeysProxy", key):
             if key in entry and self.check_child_field_value(key, entry[key]):
                 return True
             return False
 
         local_keys = [Identifier(self.get_name().prefix, k) for k in self.get_local_key_names()]
         return all(correct_key(value, k) for k in local_keys)
 
@@ -248,21 +248,24 @@
             except:
                 return False
             else:
                 return True
         else:
             return self.current.has_children
 
-    def validate_get_filter(self, filter: dict):
+    def validate_get_filter(self, filter: Union[dict, Container]):
+        if filter == Container({}):
+            filter = {}
         if self.get_dds() in (Model.StatementType.list_, Model.StatementType.container_):
             if isinstance(filter, Container):
                 filter = filter.data
             if not isinstance(filter, dict):
                 raise make_exception(pysros_err_filter_should_be_dict)
-            if "" in filter.values():
+            unwrap = lambda v: v.data if isinstance(v, Leaf) else v
+            if any(unwrap(v) == '' for v in filter.values()):
                 raise make_exception(pysros_err_filter_empty_string)
             for k, v in filter.items():
                 with self.visit_child(k):
                     self.validate_get_filter(v)
         elif self.get_dds() in (Model.StatementType.leaf_, Model.StatementType.leaf_list_):
             if isinstance(filter, Leaf) and self.get_dds() == Model.StatementType.leaf_:
                 filter = filter.data
@@ -270,15 +273,15 @@
                 filter = filter.data
             if isinstance(filter, dict):
                 if filter:
                     raise make_exception(pysros_err_filter_wrong_leaf_value, leaf_name=self.get_name().name)
             elif isinstance(filter, str):
                 pass
             elif not self.check_field_value(filter):
-                raise make_exception(pysros_err_incorrect_leaf_value, value=filter, leaf_name=self.get_name().name)
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self.get_name().name)
 
     class _TokenKind(Enum):
         string  = auto()
         symbol  = auto()
 
     @classmethod
     def _tokenize(cls, string):
@@ -329,18 +332,18 @@
                         raise make_exception(pysros_err_unended_quoted_string)
                 yield (cls._TokenKind.string, "".join(res))
                 res = []
                 continue
             res.append(i)
 
     @classmethod
-    def user_path_parse(cls, *args, **kwargs):
+    def user_path_parse(cls, *args, accept_root=False, **kwargs):
         res = cls.path_parse(*args, **kwargs)
         assert isinstance(res, ModelWalker)
-        if res.is_root:
+        if not accept_root and res.is_root:
             raise make_exception(pysros_err_root_path)
         for elem in res.path:
             if elem.is_region_blocked:
                 raise make_exception(pysros_err_unknown_element, element=elem.name.name)
         return res
 
     @classmethod
@@ -493,19 +496,31 @@
     def _is_allowed(self, model):
         return True
 
     def is_region_blocked_in_child(self, child_name:Union[str, Identifier]):
         return self._get_child(child_name).is_region_blocked
 
 class DataModelWalker(ModelWalker):
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_)
+    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.action_, Model.StatementType.input_, Model.StatementType.output_)
     _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.augment_, Model.StatementType.choice_, Model.StatementType.case_)
 
 class FilteredDataModelWalker(DataModelWalker):
+    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_)
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.config_only = False
+        self.return_blocked_regions = False
 
     def _is_allowed(self, model):
         if self.config_only and not model.config:
             return False
+        if not self.return_blocked_regions and model.is_region_blocked:
+            return False
         return any(i in model.name.prefix for i in ("nokia", "openconfig"))
+
+class ActionInputFilteredDataModelWalker(FilteredDataModelWalker):
+    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.action_)
+    _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.augment_, Model.StatementType.choice_, Model.StatementType.case_, Model.StatementType.input_)
+
+class ActionOutputFilteredDataModelWalker(FilteredDataModelWalker):
+    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.action_)
+    _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.augment_, Model.StatementType.choice_, Model.StatementType.case_, Model.StatementType.output_)
```

### Comparing `pysros-22.7.2/pysros/pprint.py` & `pysros-23.3.1/pysros/pprint.py`

 * *Files identical despite different names*

### Comparing `pysros-22.7.2/pysros/request_data.py` & `pysros-23.3.1/pysros/request_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,90 @@
 # Copyright 2021 Nokia
 
 import copy
 import pprint
+import json
 
 from abc import ABC, abstractmethod
 from collections import OrderedDict
-from typing import Union
 from contextlib import ExitStack
-
+from enum import Enum, auto
 from lxml import etree
+from ncclient.xml_ import to_ele
+from typing import Union
 
 from .errors import *
 from .identifier import NoModule, Identifier
 from .model import Model
 from .model_walker import FilteredDataModelWalker, ModelWalker
-from .wrappers import *
-from .wrappers import _Singleton, Wrapper
-
-_get_tag = lambda x: etree.QName(x).localname
+from .singleton import _Singleton, Empty
+from .wrappers import Wrapper, Action, Container, Leaf, LeafList
+from .yang_type import IdentityRef
+
+COMMON_NAMESPACES = {
+    "ncbase": "urn:ietf:params:xml:ns:netconf:base:1.0",
+    "monitoring": "urn:ietf:params:xml:ns:yang:ietf-netconf-monitoring",
+    "library": "urn:ietf:params:xml:ns:yang:ietf-yang-library",
+    "nokiaoper": "urn:nokia.com:sros:ns:yang:sr:oper-global",
+    "yang_1_0" : "urn:ietf:params:xml:ns:yang:1",
+    "attrs"    : "urn:nokia.com:sros:ns:yang:sr:attributes",
+}
+
+MO_STATEMENT_TYPES = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.action_)
+FIELD_STATEMENT_TYPES = (Model.StatementType.leaf_, Model.StatementType.leaf_list_)
+
+_get_tag_name = lambda x: etree.QName(x).localname
+_text_in_tag_tail = lambda x: x.tail and x.tail.strip()
+_text_in_tag_text = lambda x: x.text and x.text.strip()
+_create_root_ele = lambda : etree.Element("dummy-root", nsmap={"nokia-attr": COMMON_NAMESPACES["attrs"]})
+
+def _raise_invalid_text_exception(tag, check_parent_tag=True):
+    tag_to_check = tag.getparent() if check_parent_tag else tag
+    if tag_to_check.tag == "dummy-root":
+        raise make_exception(pysros_err_invalid_xml_root)
+    else:
+        raise make_exception(pysros_err_invalid_xml_element, element=_get_tag_name(tag_to_check))
+
+def _leaf_to_xml(value, root, walker, ns_map, replace_field=False):
+    if walker.get_dds() == Model.StatementType.leaf_:
+        value = (value, )
+    for i in value:
+        txt, add_ns = walker.get_type().to_string(i)
+        subelement(root, walker.current.name, ns_map, txt, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""":"replace"} if replace_field else {}, add_ns)
+        replace_field=False
 
 class RequestData:
     """Basic API for holding and handling data.
 
     .. Reviewed by TechComms 20210712
     """
-    def __init__(self, root:Model, ns_map:dict):
+
+    class _Action(Enum):
+        basic   = auto()
+        convert = auto()
+
+    def __init__(self, root:Model, ns_map:dict, action:_Action=_Action.basic, walker=FilteredDataModelWalker):
         self._root = root
-        self._data = _ListStorage(root)
+        self._data = _ListStorage(root, self)
         self._ns_map = ns_map
+        self._action = action
+        self._Walker = walker
+        self._extra_namespaces = {}
 
     def process_path(self, path:Union[str, FilteredDataModelWalker], *, strict=False):
         """Create all entries in given path and return setter for last section of the path.
 
         .. Reviewed by TechComms 20210712
         """
-        walker = path if isinstance(path, ModelWalker) else FilteredDataModelWalker.user_path_parse(self._root, path)
-        current = _ASetter.create_setter(self._data)
+        walker = path if isinstance(path, ModelWalker) else self._Walker.user_path_parse(self._root, path, accept_root=(self._action == self._Action.convert))
+        current = _ASetter.create_setter(self._data, self)
         for elem, keys in zip(walker.path, walker.keys):
             if not isinstance(current, _MoDataSetter):
                 raise make_exception(pysros_err_missing_keys, element=current._walker.get_name())
-            if elem.data_def_stm not in (Model.StatementType.leaf_, Model.StatementType.leaf_list_):
+            if elem.data_def_stm not in FIELD_STATEMENT_TYPES:
                 if strict and not current.child_mos.is_created(elem.name.name):
                     raise make_exception(pysros_err_no_data_found)
                 current = current.child_mos.get_or_create(elem.name.name)
                 if keys:
                     if strict and not current.entry_exists_nocheck(keys):
                         raise make_exception(pysros_err_no_data_found)
                     current = current.entry_nocheck(keys)
@@ -65,26 +106,43 @@
         .. Reviewed by TechComms 20210712
         """
         d = value.xpath("/ncbase:rpc-reply/ncbase:data", namespaces={"ncbase": "urn:ietf:params:xml:ns:netconf:base:1.0"})
         if len(d) != 1:
             raise make_exception(pysros_err_wrong_netconf_response)
         d = d[0]
 
-        root = _ASetter.create_setter(self._data)
+        root = _ASetter.create_setter(self._data, self)
         root.set_as_xml(d)
 
+    def set_action_as_xml(self, path, value):
+        data = value.xpath("/ncbase:rpc-reply", namespaces={"ncbase": "urn:ietf:params:xml:ns:netconf:base:1.0"})
+        if len(data) != 1:
+            raise make_exception(pysros_err_wrong_netconf_response)
+        data = data[0]
+
+        self.process_path(path).set_as_xml(data)
+
     def to_xml(self):
         """Return storage as xml.
 
         .. Reviewed by TechComms 20210712
         """
-        root = etree.Element("root")
-        self._data.to_xml(self._ns_map, root)
+        root = etree.Element(etree.QName('urn:ietf:params:xml:ns:netconf:base:1.0', 'root'))
+        self._data._to_xml(self._ns_map, root)
         return list(root[0])
 
+    def xml_tag_has_correct_ns(self, tag, walker):
+        """Check if xml namespace is correct.
+        """
+        if self._action == RequestData._Action.convert and etree.QName(tag).namespace:
+            prefix = walker.get_child(_get_tag_name(tag)).current.prefix
+            if prefix not in self._ns_map or self._ns_map[prefix] != etree.QName(tag).namespace:
+                return False
+        return True
+
     def debug_to_model(self):
         """Print storage as model.
 
         .. Reviewed by TechComms 20210712
         """
         model = self._data.to_model()
         pprint.pprint(model)
@@ -92,135 +150,181 @@
     def debug_dump(self):
         """Dump rquest data in raw form.
 
         .. Reviewed by TechComms 20210712
         """
         self._data.debug_dump()
 
+    def _unwrap(self, value):
+        return value.data if isinstance(value, Wrapper) else value
+
+    def _add_xml_namespace(self, identity):
+        assert self._ns_map[identity.module] == identity.namespace
+        self._extra_namespaces[identity.module] = identity.namespace
+
 
 class _AStorage(ABC):
     """Abstract representation of data storage.
 
     .. Reviewed by TechComms 20210712
     """
+    def __init__(self, rd:RequestData):
+        self.rd = rd
 
-    @abstractmethod
     def to_xml(self, ns_map, root):
         """Return data in xml format.
 
         .. Reviewed by TechComms 20210712
         """
+        return self._to_xml(ns_map, root)
+
+    @abstractmethod
+    def _to_xml(self, ns_map, root):
+        """Implementation of returning data in xml format.
+
+        """
         pass
 
     @abstractmethod
     def to_model(self, *, key_filter={}):
         """Return data as user model.
 
         .. Reviewed by TechComms 20210712
         """
         pass
 
     @property
     def _walker(self):
-        return FilteredDataModelWalker(self._model)
+        return self.rd._Walker(self._model)
 
     def _resolve_xml_name(self, model, ns_map):
         if model.name.prefix in ns_map:
             return etree.QName(ns_map[model.name.prefix], model.name.name)
         elif model.name.prefix is NoModule():
             return model.name.name
         else:
             raise make_exception(pysros_err_prefix_does_not_have_ns, prefix=model.name.prefix, name=model.name.name)
 
-def subelement(parent, tag, text=None, attrib=None):
+def subelement(parent, tag, nsmap, text=None, attrib=None, add_ns=None):
     """Wrapper around etree.Subelement, that raises SrosMgmtError instead of ValueError."""
+    local_nsmap = {}
+    if add_ns:
+        local_nsmap[add_ns] = nsmap[add_ns]
     try:
-        result = etree.SubElement(parent, tag, attrib)
-        if text:
+        if tag.is_builtin():
+            result = etree.SubElement(parent, tag.name, attrib, nsmap=local_nsmap)
+        else:
+            module = tag.prefix
+            uri = nsmap[module]
+            local_nsmap[module] = uri
+            result = etree.SubElement(
+                parent,
+                etree.QName(uri, tag.name),
+                attrib,
+                nsmap=local_nsmap
+            )
+
+        if text is not None:
             result.text = text
         return result
     except ValueError as err:
         raise SrosMgmtError(err.args) from None
 
 class _MoStorage(_AStorage):
-    """Data storage for containers and list entries(list+local keys).
+    """Data storage for containers and list entries (list+local keys).
 
     .. Reviewed by TechComms 20210712
     """
 
-    def __init__(self, model:Model, local_keys):
+    def __init__(self, model:Model, local_keys, rd:RequestData):
+        super().__init__(rd)
         self._model = model
         self._local_keys = copy.deepcopy(local_keys)
         self._child = {}
         self._operation = ""
-        self._replace_field = "" #TODO could be field storage
+        self._replace_field = "" # Could be field storage
 
-    def to_xml(self, ns_map, root):
-        root_attr = None if not self._operation else {"operation": self._operation}
-        root = subelement(root, self._resolve_xml_name(self._model, ns_map), None, root_attr)
+    def _to_xml(self, ns_map, root):
+        root_attr = None if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
+        root = subelement(root, self._model.name, ns_map, None, root_attr)
         for k, v in self._local_keys.items():
             if v is FieldValuePlaceholder():
                 pass
             elif v is GetValuePlaceholder():
                 self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
             else:
-               txt  = self._walker.get_child(k).get_type().to_string(v)
-               subelement(root, self._resolve_xml_name(self._walker.get_child(k).current, ns_map), txt)
+               txt, add_ns = self._walker.get_child(k).get_type().to_string(v)
+               subelement(root, self._walker.get_child(k).current.name, ns_map, txt, {}, add_ns)
 
         for k, v in self._child.items():
             if isinstance(v, (_MoStorage, _ListStorage)):
-                v.to_xml(ns_map, root)
+                v._to_xml(ns_map, root)
             else:
                 if v is Delete():
-                    subelement(root, self._resolve_xml_name(self._walker.get_child(k).current, ns_map), None, {"operation": "remove"})
+                    subelement(root, self._walker.get_child(k).current.name, ns_map, None, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": "remove"})
                 elif v is FieldValuePlaceholder():
                     pass
                 elif v is GetValuePlaceholder():
                     self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
                 elif self._replace_field and self._replace_field == k:
-                    self._leaf_to_xml(v, root, self._walker.get_child(k), ns_map, replace_field=True)
+                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map, replace_field=True)
                 else:
-                    self._leaf_to_xml(v, root, self._walker.get_child(k), ns_map)
+                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map)
 
-    def _leaf_to_xml(self, value, root, walker, ns_map, replace_field=False):
-        if walker.get_dds() == Model.StatementType.leaf_:
-            value = (value, )
-        for i in value:
-            txt = walker.get_type().to_string(i)
-            subelement(root, self._resolve_xml_name(walker.current, ns_map), txt, {"operation":"replace"} if replace_field else {})
-            replace_field=False
+    def to_xml(self, ns_map, root):
+        root_attr = None if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
+
+        for k, v in self._child.items():
+            if isinstance(v, (_MoStorage, _ListStorage)):
+                v._to_xml(ns_map, root)
+            else:
+                if v is Delete():
+                    subelement(root, self._walker.get_child(k).current.name, ns_map, None, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": "remove"})
+                elif v is FieldValuePlaceholder():
+                    pass
+                elif v is GetValuePlaceholder():
+                    self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
+                elif self._replace_field and self._replace_field == k:
+                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map, replace_field=True)
+                else:
+                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map)
 
     def _leaf_placeholder_to_xml(self, value, root, walker, ns_map):
-        subelement(root, self._resolve_xml_name(walker.current, ns_map))
+        subelement(root, walker.current.name, ns_map)
 
     def to_model(self, *, key_filter={}):
         data = {}
         is_selection_filter = {} in key_filter.values()
-        for k, v in self._child.items():
+        for k, v in self._local_keys.items():
             if is_selection_filter and k not in key_filter:
                 continue
+            data[k] = self._leaf_to_model(k, v)
+        for k, v in self._child.items():
+            key_proxy = DictionaryKeysProxy(self.rd._unwrap(key_filter))
+            if is_selection_filter and self._walker.get_child(k).current.name not in key_proxy:
+                continue
             if not isinstance(v, (_MoStorage, _ListStorage)):
                 data[k] = self._leaf_to_model(k, v)
             else:
                 data[k] = v.to_model(key_filter=(key_filter.get(k, {})))
                 if not data[k] and not self._walker.get_child(k).has_explicit_presence():
                     del data[k]
-        for k, v in self._local_keys.items():
-            if is_selection_filter and k not in key_filter:
-                continue
-            data[k] = self._leaf_to_model(k, v)
-        return Container._with_module(data, self._model.name.prefix)
+        if self._walker.is_root:
+            return data
+        if self._model.data_def_stm == Model.StatementType.action_:
+            return Action._with_model(data, self._model)
+        return Container._with_model(data, self._model)
 
     def _leaf_to_model(self, name, value):
-        assert value is not GetValuePlaceholder()
+        assert self.rd._action == RequestData._Action.convert or value is not GetValuePlaceholder()
         assert value is not FieldValuePlaceholder()
-        module = self._walker.get_child_name(name).prefix
+        model = self._walker.get_child(name).current
         if self._walker.get_child_dds(name) == Model.StatementType.leaf_:
-            return Leaf._with_module(value, module)
-        return LeafList._with_module(value, module)
+            return Leaf._with_model(value, model)
+        return LeafList._with_model(value, model)
 
     def keys_equal(self, keys):
         """Compare if keys are equal. Keys are expected as dict(name->value).
 
         .. Reviewed by TechComms 20210712
         """
         return self._local_keys == keys
@@ -250,29 +354,35 @@
 
 
 class _ListStorage(_AStorage):
     """Storage for all entries for a specific list.
 
     .. Reviewed by TechComms 20210712
     """
-    def __init__(self, model:Model):
-        if model.data_def_stm == Model.StatementType.container_:
+    def __init__(self, model:Model, rd:RequestData):
+        if model.data_def_stm in (Model.StatementType.container_, Model.StatementType.action_):
             self.__class__ = _MoStorage
-            self.__class__.__init__(self, model, {})
+            self.__class__.__init__(self, model, {}, rd)
         else:
+            super().__init__(rd)
             self._model = model
             self._entries = {}
             self._operation = ""
 
-    def to_xml(self, ns_map, root):
+    def _to_xml(self, ns_map, root):
         if self._entries:
             for entry in self._entries.values():
-                entry.to_xml(ns_map, root)
+                entry._to_xml(ns_map, root)
         else:
-            subelement(root, self._resolve_xml_name(self._model, ns_map))
+            subelement(root, self._model.name, ns_map)
+
+    def to_xml(self, ns_map, root):
+        if self._entries:
+            for entry in self._entries.values():
+                entry._to_xml(ns_map, root)
 
     def to_model(self, *, key_filter={}):
         d = OrderedDict() if self._model.user_ordered else {}
         for e in self._entries.values():
             d[e.get_keys_flat()] = e.to_model(key_filter=key_filter)
 
         return d
@@ -310,68 +420,97 @@
 
     def add_entry(self, keys):
         """Add new entry with specific keys. Entry cannot already exist. Keys are expected as dict(name->value).
 
         .. Reviewed by TechComms 20210712
         """
         assert not self.has_entry(keys)
-        res = _MoStorage(self._model, keys)
+        res = _MoStorage(self._model, keys, self.rd)
         self._entries[tuple(sorted(keys.items()))] = res
         return res
 
     def debug_dump(self, indent=0):
         for i in self._entries.values():
             i.debug_dump(indent+1)
 
-class EntryKeysDictProxy():
-    """Proxy for dict keys which unwraps keys and compares by performing Identifier.__eq__"""
+class DictionaryKeysProxy():
+    """Proxy for dictionary keys which unwraps keys and compares by performing Identifier.__eq__"""
     def __init__(self, data):
         if not isinstance(data, dict):
             raise make_exception(pysros_err_invalid_value, data=data)
         self.data = data
 
-    def __getitem__(self, key):
+    def __getitem__(self, key:Identifier):
         #need to call Identifier.__eq__
         for k in self.data.keys():
             if key == k:
                 return self._unwrap(self.data[k])
         raise KeyError(key)
 
-    def __contains__(self, val):
+    def __contains__(self, val:Identifier):
         #need to call Identifier.__eq__
         for ele in self.data:
             if val == ele:
                 return True
         return False
 
     def __str__(self):
         return str(self.data)
 
     def _unwrap(self, val):
         return val.data if isinstance(val, Wrapper) else val
 
+class RdJsonEncoder(json.JSONEncoder):
+    def add_ns(self, o, d, walker:ModelWalker):
+        if o is self.root:
+            return {walker.get_child(k).get_name().model_string: v for k, v in d.items()}
+        return {walker.get_child(k).get_name().model_string if walker.get_name().prefix != walker.get_child(k).get_name().prefix else k: v for k, v in d.items()}
+
+    def default(self, o):
+        is_root = o is self.root
+        if isinstance(o, _MoStorage):
+            res = {}
+            if not is_root:
+                res.update(self.add_ns(o, o._local_keys, o._walker))
+            elif is_root and self.force_key:
+                res[o._walker.get_child(self.force_key).get_name().model_string] = o._local_keys[self.force_key]
+            res.update(self.add_ns(o, o._child, o._walker))
+            stringify = lambda x, dds: [str(v) for v in x] if dds == Model.StatementType.leaf_list_ else str(x)
+            cvt = lambda k, v: stringify(v, o._walker.get_child_dds(k)) if o._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES and o._walker.get_child_type(k).json_name() in ("int64", "uint64") else v
+            res = {k: cvt(k, v) for k, v in res.items()}
+            return res
+        elif isinstance(o, _ListStorage):
+            res = list(o._entries.values())
+            return {o._walker.get_name().model_string: res} if is_root else res
+        elif isinstance(o, (str, list, dict, bool)):
+            return o
+        elif o is Empty:
+            return [None]
+        else:
+            return str(o)
 
 class _ASetter(ABC):
     """Data setter representation for storage classes.
 
     .. Reviewed by TechComms 20210712
     """
-    def __init__(self, storage:"_AStorage"):
+    def __init__(self, storage:"_AStorage", rd:RequestData):
         self._storage = storage
+        self.rd = rd
 
     @property
-    def _walker(self) -> FilteredDataModelWalker:
-        return FilteredDataModelWalker(self._storage._model)
+    def _walker(self):
+        return self.rd._Walker(self._storage._model)
 
     @staticmethod
-    def create_setter(storage:"_AStorage"):
+    def create_setter(storage:"_AStorage", rd:RequestData):
         if isinstance(storage, _MoStorage):
-            return _MoDataSetter(storage)
+            return _MoDataSetter(storage, rd)
         else:
-            return _ListSetter(storage)
+            return _ListSetter(storage, rd)
 
     @abstractmethod
     def set(self, value):
         """Set data in model format.
 
         .. Reviewed by TechComms 20210712
         """
@@ -381,14 +520,47 @@
     def set_as_xml(self, value):
         """Set data in xml format.
 
         .. Reviewed by TechComms 20210712
         """
         pass
 
+    def checkJsonDuplicates(x):
+        if len(x) != len({i[0] for i in x}):
+            raise make_exception(pysros_err_multiple_occurences_of_node)
+        return dict(x)
+
+    def set_as_json(self, value):
+        """Set data in json format."""
+        try:
+            val = json.loads(value, object_pairs_hook=_ASetter.checkJsonDuplicates)
+        except json.JSONDecodeError as e:
+            raise JsonDecodeError(*e.args) from None
+
+        if not isinstance(val, dict):
+            raise make_exception(pysros_err_wrong_json_root)
+
+        self._set_as_json(val, is_root = True)
+
+    @abstractmethod
+    def _set_as_json(self, value, is_root = False):
+        """Implementation of setter for JSON."""
+        pass
+
+    def to_json(self, pprint = True):
+        """Return data in json format."""
+        members = {
+            "root": self._storage,
+            "root_setter": self,
+            "force_key": getattr(self, "_key_name", None),
+        }
+        encoder = type("RdJsonEncoderSpecialization", (RdJsonEncoder, ), members)
+        indent = 4 if pprint else None
+        return json.dumps(self._storage, cls=encoder, indent=indent)
+
     @abstractmethod
     def delete(self):
         """Set data operation to delete"""
         pass
 
     @abstractmethod
     def replace(self):
@@ -403,65 +575,138 @@
     def to_model(self, *, key_filter={}):
         """Return data in model format.
 
         .. Reviewed by TechComms 20210712
         """
         return self._storage.to_model(key_filter=key_filter)
 
+    def to_xml(self):
+        """Return data in xml format."""
+        root = _create_root_ele()
+        self._storage.to_xml(self.rd._ns_map, root)
+        return root
+
+
     def set_filter(self, value):
         """Populate request data with filter syntax"""
         raise make_exception(pysros_err_filter_not_supported_on_leaves)
 
-    def _unwrap(self, value):
-        return value.data if isinstance(value, Wrapper) else value
+    def is_compare_supported_endpoint(self):
+        return False
 
+    def is_action(self):
+        return self._walker.get_dds() == Model.StatementType.action_
+
+    def entry_xml(self, value):
+        """For XML there is no tag for the list itself, only for entries.
+        Therefore, the list setter can be avoided, however, you must create
+        an entry setter and it simplifies the code if you always create
+        an entry regardless of the child type.  It is effective only for
+        the list setter."""
+        return self
 
     def _as_storage_type(self, val, *, child_name=None):
         walker = self._walker.get_child(child_name) if child_name else self._walker
         if walker.get_dds() == Model.StatementType.leaf_list_:
-            return [walker.get_type().as_storage_type(v) for v in val]
+            return [walker.get_type().as_storage_type(v, self.rd._action == RequestData._Action.convert, self.rd._add_xml_namespace) for v in val]
         else:
-            return walker.get_type().as_storage_type(val)
+            return walker.get_type().as_storage_type(val, self.rd._action == RequestData._Action.convert, self.rd._add_xml_namespace)
+
+    def _handle_entry_keys_namespaces(self, entry):
+        """Strip namespace prefixes from entry key names.
+        Also raise an error if there are two identical entry keys, one with the namespace prefix and other one without it.
+        """
+        local_keys = [Identifier(self._walker.get_name().prefix, k) for k in self._walker.get_local_key_names()]
+        for k in local_keys:
+            if k.model_string in entry:
+                if k.name in entry:
+                    raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=entry[k.model_string])
+                entry[k.name] = entry.pop(k.model_string)
 
 class _LeafSetter(_ASetter):
     """Interface for managing leafs. Because leafs do not have dedicated storage, the
        class has its own implementation of to_model method.
 
     .. Reviewed by TechComms 20210713
     """
-    def __init__(self, storage:"_ListStorage", leaf_name:str):
-        super().__init__(storage)
+    def __init__(self, storage:"_ListStorage", leaf_name:str, rd:RequestData):
+        super().__init__(storage, rd)
         self._leaf_name = leaf_name
 
     def set(self, value):
-        value = self._unwrap(value)
+        value = self.rd._unwrap(value)
         if not self._walker.check_field_value(value):
-            raise make_exception(pysros_err_incorrect_leaf_value, value=value, leaf_name=self._leaf_name)
+            raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._leaf_name)
         else:
-            self._set_nocheck(self._as_storage_type(value))
+            val = self._as_storage_type(value)
+            self._set_nocheck(val)
 
     def _set_nocheck(self, value):
         self._storage._child[self._leaf_name] = value
 
     def set_getValue(self):
         self._storage._child[self._leaf_name] = GetValuePlaceholder()
 
     def set_as_xml(self, value):
-        value = value.text or ""
-        self.set(self._walker.as_model_type(value))
+        if not len(value):
+            raise make_exception(pysros_err_malformed_xml)
+        for v in value:
+            self.set_or_append_as_xml(v)
+
+    def _set_as_json(self, value, is_root = False):
+        if not isinstance(value, dict):
+            raise make_exception(pysros_err_invalid_json_structure)
+        value = {k:v for k, v in value.items() if not k.startswith("@")}
+        if len(value) != 1:
+            raise make_exception(pysros_err_invalid_json_structure)
+
+        val = next(iter(value.items()))
+        if self._walker.get_name() != val[0]:
+            raise make_exception(pysros_err_invalid_json_structure)
+        val = val[1]
+        if self._walker.get_type().json_name() in ("int64", "uint64"):
+            if self._walker.get_dds() != Model.StatementType.leaf_list_:
+                val = [self.rd._unwrap(val)]
+            else:
+                val = self.rd._unwrap(val)
+            if not isinstance(val, list) or not all(isinstance(v, str) for v in val):
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name)
+            try:
+                value = [int(self.rd._unwrap(v)) for v in val]
+            except:
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name) from None
+        self.set(self._walker.as_model_type(val))
+
+    def set_or_append_as_xml(self, value_element):
+        if _text_in_tag_tail(value_element) or (self._walker.get_dds() == Model.StatementType.leaf_list_ and _text_in_tag_text(value_element.getparent())):
+            _raise_invalid_text_exception(value_element)
+        value = self._walker.as_model_type(value_element.text or "")
+
+        if isinstance(self._walker.get_type(), IdentityRef):
+            is_leaf_list = isinstance(value, list)
+            assert not is_leaf_list or len(value) == 1
+            identity = self._walker.get_type()._find_identity(value[0] if is_leaf_list else value)
+            if not identity:
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name = self._walker.current.name.name)
+            value_ns = value_element.nsmap.get(identity.module, None)
+            if value_ns is not None and value_ns!=identity.namespace:
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name = self._walker.current.name.name)
 
-    def set_or_append_as_xml(self, value):
-        value = self._walker.as_model_type(value.text or "")
-        if self._walker.get_dds() == Model.StatementType.leaf_list_ and self._leaf_name in self._storage._child:
+        if self._walker.get_dds() == Model.StatementType.leaf_list_ and isinstance(self._storage._child.get(self._leaf_name), list):
             value = self._storage._child[self._leaf_name] + value
         self.set(value)
 
     def to_model(self, *, key_filter={}):
         return self._storage._leaf_to_model(self._leaf_name, self._storage._child[self._leaf_name])
 
+    def to_xml(self):
+        root = _create_root_ele()
+        _leaf_to_xml(self._storage._child[self._leaf_name], root, self._walker, self.rd._ns_map)
+        return root
+
     def delete(self):
         if self._walker.get_dds() == Model.StatementType.leaf_list_:
             raise make_exception(pysros_err_invalid_operation_on_leaflist)
         self._storage._child[self._leaf_name] = Delete()
 
     def replace(self):
         self._storage._replace_field = self._leaf_name
@@ -469,43 +714,73 @@
     @property
     def _walker(self):
         return super()._walker.get_child(self._leaf_name)
 
 class _KeySetter(_ASetter):
     """Interface for keys. Most of this class are stub methods to provide
        setter interface to keys."""
-    def __init__(self, storage:"_ListStorage", key_name:str):
-        super().__init__(storage)
+    def __init__(self, storage:"_ListStorage", key_name:str, rd:RequestData):
+        super().__init__(storage, rd)
         self._key_name = key_name
 
     def set(self, value):
-        value = self._unwrap(value)
+        value = self.rd._unwrap(value)
         if not self._walker.check_field_value(value):
-            raise make_exception(pysros_err_incorrect_leaf_value, value=value, leaf_name=self._key_name)
+            raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._key_name)
         elif self._as_storage_type(value) != self._storage._local_keys[self._key_name]:
             raise make_exception(pysros_err_key_val_mismatch, key_name=self._key_name)
 
     def set_getValue(self):
         pass
 
     def set_placeholder(self):
         pass
 
     def to_model(self, *, key_filter={}):
         return self._storage._leaf_to_model(self._key_name, self._storage._local_keys[self._key_name])
 
+    def to_xml(self):
+        root = _create_root_ele()
+        _leaf_to_xml(self._storage._local_keys[self._key_name], root, self._walker, self.rd._ns_map)
+        return root
+
     def delete(self):
         raise make_exception(pysros_err_invalid_operation_on_key)
 
     def replace(self):
         raise make_exception(pysros_err_invalid_operation_on_key)
 
     def set_as_xml(self, value):
-        value = value.text or ""
-        self.set(self._walker.as_model_type(value))
+        if _text_in_tag_tail(value):
+            _raise_invalid_text_exception(value_element)
+        if not len(value):
+            raise make_exception(pysros_err_malformed_xml)
+        for v in value:
+            if _text_in_tag_tail(v):
+                _raise_invalid_text_exception(v)
+            self.set(self._walker.as_model_type(v.text or ""))
+
+    def _set_as_json(self, value, is_root = False):
+        if not isinstance(value, dict):
+            raise make_exception(pysros_err_invalid_json_structure)
+        value = {k:v for k, v in value.items() if not k.startswith("@")}
+        if  len(value) != 1:
+            raise make_exception(pysros_err_invalid_json_structure)
+
+        val = next(iter(value.items()))
+        if self._walker.get_name() != val[0]:
+            raise make_exception(pysros_err_invalid_json_structure)
+        if self._walker.get_type().json_name() in ("int64", "uint64"):
+            if not isinstance(val[1], str):
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name)
+            try:
+                value = int(val[1])
+            except:
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name) from None
+        self.set(self._walker.as_model_type(val[1]))
 
     @property
     def _walker(self):
         return super()._walker.get_child(self._key_name)
 
 class _ListSetter(_ASetter):
     """Interface for managing instances of specific list.
@@ -518,17 +793,17 @@
 
         Keys may be in format {(key1, key2) : Container({}), (key1, key2) : Container({})}
         or directly in entry {key1: value1, key2: value2, field1 : value}.
 
         .. Reviewed by PLM 20211018
         """
         is_wrapped = isinstance(value, Container)
-        value = self._unwrap(value)
+        value = self.rd._unwrap(value)
         value = copy.copy(value)
-        unwrapper = EntryKeysDictProxy(value)
+        unwrapper = DictionaryKeysProxy(value)
         if value and not is_wrapped and self._walker.dict_keys(value):
             for k, v in value.items():
                 self._handle_entry_keys_namespaces(v)
                 self.entry(self._tuple_to_dict(k)).set(v)
         elif self._walker.entry_keys(unwrapper):
             self._handle_entry_keys_namespaces(value)
             self.entry(value).set(value)
@@ -547,120 +822,150 @@
         return {k:v for k, v in zip(self._walker.get_local_key_names(), (t if isinstance(t, tuple) else (t, )))}
 
     def _extract_keys(self, entry):
         return {k:self._as_storage_type(v, child_name=k) for k, v in entry.items() if k in self._walker.get_local_key_names()}
 
     def _convert_keys_to_model(self, entry):
         try:
-            return {k: (GetValuePlaceholder() if v in (GetValuePlaceholder(), {}) else self._walker.as_child_model_type(k, v)) for k, v in entry.items() if v is not FieldValuePlaceholder()}
+            def unwrap(v):
+                return v.data if isinstance(v, Wrapper) else v
+            val =  {k: (GetValuePlaceholder() if unwrap(v) in (GetValuePlaceholder(), {}) else self._walker.as_child_model_type(k, unwrap(v))) for k, v in entry.items() if v is not FieldValuePlaceholder()}
+            return val
         except:
             raise make_exception(pysros_err_invalid_key_in_path) from None
 
-    def _handle_entry_keys_namespaces(self, entry):
-        """Strip namespace prefixes from entry key names.
-        Also raise an error if there are two identical entry keys, one with the namespace prefix and other one without it.
-        """
-        local_keys = [Identifier(self._walker.get_name().prefix, k) for k in self._walker.get_local_key_names()]
-        for k in local_keys:
-            if k.model_string in entry:
-                if k.name in entry:
-                    raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=entry[k.model_string])
-                entry[k.name] = entry.pop(k.model_string)
-
-    def _check_and_unwrap_keys(self, entry):
+    def _check_and_unwrap_keys(self, entry, *, json=False):
         for k in self._walker.get_local_key_names():
             if k not in entry:
-                raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=value)
-            entry[k] = self._unwrap(entry[k])
-            if not self._walker.check_child_field_value(k, entry[k]):
-                raise make_exception(pysros_err_incorrect_leaf_value, value=entry[k], leaf_name=k)
-            entry[k] = self._walker.get_child_type(k).as_storage_type(entry[k])
+                raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=k)
+            entry[k] = self.rd._unwrap(entry[k])
+            if not self._walker.check_child_field_value(k, entry[k], json=json):
+                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=k)
+            entry[k] = self._walker.get_child_type(k).as_storage_type(entry[k], self.rd._action == RequestData._Action.convert, self.rd._add_xml_namespace)
 
-    def entry(self, value):
+    def entry(self, value, *, json=False):
         """Receive entry with specified keys in value. Keys are expected as dict(name->value). Additional
         fields may be present (no verification for extra fields).
 
         .. Reviewed by TechComms 20210712
         """
+        if json:
+            value = copy.copy(value)
+        self._handle_entry_keys_namespaces(value)
+        self._check_and_unwrap_keys(value, json=json)
+        return _MoDataSetter(self._storage.get_or_create_entry(self._extract_keys(value)), self.rd)
+
+    def add_entry(self, value, *, json=False):
+        if json:
+            value = copy.copy(value)
         self._handle_entry_keys_namespaces(value)
-        self._check_and_unwrap_keys(value)
-        return _MoDataSetter(self._storage.get_or_create_entry(self._extract_keys(value)))
+        self._check_and_unwrap_keys(value, json=json)
+        keys = self._extract_keys(value)
+        if self._storage.has_entry(keys):
+            raise make_exception(pysros_err_multiple_occurences_of_entry)
+        return _MoDataSetter(self._storage.get_or_create_entry(keys), self.rd)
 
     def entry_nocheck(self, value):
         """Receive entry with specified keys in value without checking for the correct type. Keys are expected
         as dict(name->value). Additional fields may be present (no verification for extra fields).
 
         .. Reviewed by PLM 20211018
         """
-        return _MoDataSetter(self._storage.get_or_create_entry(self._convert_keys_to_model(self._extract_keys(value))))
+        return _MoDataSetter(self._storage.get_or_create_entry(self._convert_keys_to_model(self._extract_keys(value))), self.rd)
 
     def entry_exists_nocheck(self, value):
         """Receive entry with specified keys in value without checking for the correct type. Keys are expected
         as dict(name->value). Additional fields may be present (no verification for extra fields)
         Returns true if entry exists, otherwise false.
         """
         return self._storage.has_entry(self._convert_keys_to_model(self._extract_keys(value)))
 
     def entry_xml(self, value):
         keys = {}
         for e in value:
-            if _get_tag(e) in self._walker.get_local_key_names():
-                keys[_get_tag(e)] = e.text or ""
+            if _get_tag_name(e) in self._walker.get_local_key_names():
+                if _text_in_tag_tail(e):
+                    _raise_invalid_text_exception(e)
+                keys[_get_tag_name(e)] = e.text or ""
         if set(keys.keys()) != set(self._walker.get_local_key_names()):
-            raise make_exception(pysros_err_schema_box_keys_mismatch, schema_keys=self._walker.get_local_key_names(), box_keys=list(keys.keys()))
+            raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=keys)
+        if self.entry_exists_nocheck(keys):
+            raise make_exception(pysros_err_multiple_occurences_of_entry)
         return self.entry_nocheck(keys)
 
     def set_as_xml(self, value):
-        self.entry_xml(value).set_as_xml(value)
+        for v in value:
+            self.entry_xml(v).set_as_xml(v)
+
+    def _set_as_json(self, value, is_root = False):
+        if is_root:
+            if not isinstance(value, dict):
+                raise make_exception(pysros_err_invalid_json_structure)
+            value = {k:v for k, v in value.items() if not k.startswith("@")}
+            if len(value) != 1:
+                raise make_exception(pysros_err_invalid_json_structure)
+            value = next(iter(value.items()))
+            if self._walker.get_name() != value[0] or not isinstance(value[1], list):
+                raise make_exception(pysros_err_invalid_json_structure)
+            value = value[1]
+        else:
+            if not isinstance(value, list) or not all(isinstance(i, dict) for i in value):
+                raise make_exception(pysros_err_convert_invalid_value_for_type, name=self._walker.get_name().name)
+        for v in value:
+            self.add_entry(v, json=True)._set_as_json(v)
 
     def delete(self):
         raise make_exception(pysros_err_invalid_path_operation_missing_keys)
 
     def replace(self):
         for k, v in self._storage._entries.items():
             v._operation = "replace"
 
     def entry_get_keys(self):
         keys = {key:GetValuePlaceholder() for key in self._walker.get_local_key_names()}
-        setter = _MoDataSetter(self._storage.get_or_create_entry(keys))
+        setter = _MoDataSetter(self._storage.get_or_create_entry(keys), self.rd)
         setter.set({})
         return setter
 
 class _MoDataSetter(_ASetter):
     """Interface managing specific list entry or container.
 
     .. Reviewed by TechComms 20210712
     """
     class _AChild:
         def __init__(self, setter:"_MoDataSetter"):
             self._setter = setter
 
         @property
-        def _walker(self) -> FilteredDataModelWalker:
-            return FilteredDataModelWalker(self._setter._storage._model)
+        def _walker(self):
+            return self._setter.rd._Walker(self._setter._storage._model)
 
     class _Keys(_AChild):
         """Interface for retrieving and setting keys.
 
         .. Reviewed by TechComms 20210712
         """
         def set(self, name, value):
             name = Identifier.from_model_string(name).name
             self.get(name).set(value)
 
+        def set_as_json(self, name, value):
+            name = Identifier.from_model_string(name).name
+            self.get(name)._set_as_json({name: value})
+
         def set_getValue(self, name):
             self.get(name).set_getValue()
 
         def set_placeholder(self, name):
             self.get(name).set_placeholder()
 
         def get(self, name):
             if not self.can_contains(name):
                 raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
-            return _KeySetter(self._setter._storage, name)
+            return _KeySetter(self._setter._storage, name, self._setter.rd)
 
         def contains(self, name):
             return self.can_contains(name)
 
         def can_contains(self, name):
             return self._walker.has_local_key_named(name)
 
@@ -670,21 +975,32 @@
         .. Reviewed by TechComms 20210712
         """
 
         def set(self, name, value):
             name = Identifier.from_model_string(name).name
             self.get(name).set(value)
 
+        def set_as_json(self, name, value):
+            name = Identifier.from_model_string(name).name
+            self.get(name)._set_as_json({name: value})
+
         def set_getValue(self, name):
             self.get(name).set_getValue()
 
         def get(self, name):
             if not self.can_contains(name):
                 raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
-            return _LeafSetter(self._setter._storage, name)
+            return _LeafSetter(self._setter._storage, name, self._setter.rd)
+
+        def get_nonexisting(self, name):
+            if not self.can_contains(name):
+                raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
+            if self.contains(name) and self._walker.get_child_dds(name) != Model.StatementType.leaf_list_:
+                raise make_exception(pysros_err_multiple_occurences_of_node)
+            return _LeafSetter(self._setter._storage, name, self._setter.rd)
 
         def contains(self, name):
             return name in self._setter._storage._child
 
         def can_contains(self, name):
             return self._walker.has_field_named(name)
 
@@ -693,24 +1009,38 @@
         """Interface for retrieving and setting children.
 
         .. Reviewed by TechComms 20210712
         """
         def set(self, name, value):
             self.get_or_create(Identifier.from_model_string(name).name).set(value)
 
+        def set_as_json(self, name, value):
+            self.get_or_create(Identifier.from_model_string(name).name)._set_as_json(value)
+
         def get_or_create(self, name):
-            if self._walker.get_child_dds(name) in (Model.StatementType.container_, Model.StatementType.list_):
+            if self._walker.get_child_dds(name) in MO_STATEMENT_TYPES:
                 if not self.is_created(name):
-                    self._setter._storage._child[name] = _ListStorage(self._setter._walker.get_child(name).current)
-                return _ASetter.create_setter(self._setter._storage._child[name])
+                    self._setter._storage._child[name] = _ListStorage(self._setter._walker.get_child(name).current, self._setter.rd)
+                return _ASetter.create_setter(self._setter._storage._child[name], self._setter.rd)
+            else:
+                raise KeyError(name)
+
+        def get(self, name):
+            if self._walker.get_child_dds(name) in MO_STATEMENT_TYPES:
+                if self.is_created(name):
+                    if not self._walker.get_child_dds(name) == Model.StatementType.list_:
+                        raise make_exception(pysros_err_multiple_occurences_of_node)
+                else:
+                    self._setter._storage._child[name] = _ListStorage(self._setter._walker.get_child(name).current, self._setter.rd)
+                return _ASetter.create_setter(self._setter._storage._child[name], self._setter.rd)
             else:
                 raise KeyError(name)
 
         def is_created(self, name):
-            return self._walker.get_child_dds(name) in (Model.StatementType.container_, Model.StatementType.list_) and name in self._setter._storage._child
+            return self._walker.get_child_dds(name) in MO_STATEMENT_TYPES and name in self._setter._storage._child
 
 
     @property
     def keys(self):
         return self._Keys(self)
 
     @property
@@ -718,78 +1048,117 @@
         return self._Fields(self)
 
     @property
     def child_mos(self):
         return self._ChildMos(self)
 
     def set(self, value):
-        value = self._unwrap(value)
+        value = self.rd._unwrap(value)
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_value, data=value)
         children_to_set = set()
+        walker = self._walker
         for k, v in value.items():
-            if k in self._walker.get_local_key_names():
+            if k in walker.get_local_key_names():
                 self.keys.set(k, v)
-            elif self._walker.get_child_dds(k) in (Model.StatementType.leaf_, Model.StatementType.leaf_list_):
+            elif walker.get_child_dds(k) in FIELD_STATEMENT_TYPES:
                 self.fields.set(k, v)
-            elif self._walker.get_child_dds(k) in (Model.StatementType.container_, Model.StatementType.list_):
+            elif walker.get_child_dds(k) in MO_STATEMENT_TYPES:
                 self.child_mos.set(k, v)
             else:
-                raise make_exception(pysros_err_unknown_dds, dds=self._walker.get_child_dds(k))
+                raise make_exception(pysros_err_unknown_dds, dds=walker.get_child_dds(k))
             name = Identifier.from_model_string(k).name
             if name in children_to_set:
                 raise make_exception(pysros_err_duplicate_found, duplicate=name)
             children_to_set.add(name)
 
     def set_filter(self, value):
-        value = self._unwrap(value)
+        value = self.rd._unwrap(value)
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_value, data=value)
+        self._handle_entry_keys_namespaces(value)
         children_to_set = set()
         for k, v in value.items():
-            v = self._unwrap(v)
+            v = self.rd._unwrap(v)
             if k in self._walker.get_local_key_names():
                 if v == {} or v is GetValuePlaceholder():
                     self.keys.set_getValue(k)
                 elif v is FieldValuePlaceholder():
                     self.keys.set_placeholder(k)
                 else:
                     self.keys.set(k, v)
-            elif self._walker.get_child_dds(k) in (Model.StatementType.leaf_, Model.StatementType.leaf_list_):
+            elif self._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES:
                 if v == {}:
                     self.fields.set_getValue(k)
                 else:
                     self.fields.set(k, v)
-            elif self._walker.get_child_dds(k) in (Model.StatementType.container_, Model.StatementType.list_):
+            elif self._walker.get_child_dds(k) in MO_STATEMENT_TYPES:
                 self.child_mos.get_or_create(k).set_filter(v)
             else:
                 raise make_exception(pysros_err_unknown_dds, dds=self._walker.get_child_dds(k))
             name = Identifier.from_model_string(k).name
             if name in children_to_set:
                 raise make_exception(pysros_err_duplicate_found, duplicate=name)
             children_to_set.add(name)
 
     def set_as_xml(self, value):
+        walker = self._walker
+        if self.rd._action != RequestData._Action.convert:
+            walker.return_blocked_regions = True
+        if _text_in_tag_text(value):
+            _raise_invalid_text_exception(value, check_parent_tag=False)
+        if _text_in_tag_tail(value):
+            _raise_invalid_text_exception(value)
         for e in value:
-            if not self._walker.has_child(_get_tag(e)):
-                raise make_exception(pysros_err_unknown_child, child_name=_get_tag(e), path=self._walker._get_path())
-            if self._walker.is_region_blocked_in_child(_get_tag(e)):
+            if not walker.has_child(_get_tag_name(e)) or not self.rd.xml_tag_has_correct_ns(e, walker):
+                raise make_exception(pysros_err_unknown_child, child_name=_get_tag_name(e), path=walker._get_path())
+            if walker.is_region_blocked_in_child(_get_tag_name(e)):
+                continue
+            else:
+                if walker.get_child_dds(_get_tag_name(e)) in FIELD_STATEMENT_TYPES:
+                    if _get_tag_name(e) not in walker.get_local_key_names():
+                        self.fields.get_nonexisting(_get_tag_name(e)).set_or_append_as_xml(e)
+                    elif self.rd._action == RequestData._Action.convert:
+                        xml = to_ele(f"<{_get_tag_name(value)}>{etree.tostring(e, encoding='unicode')}</{_get_tag_name(value)}>")
+                        _KeySetter(self._storage, _get_tag_name(e), self.rd).set_as_xml(xml)
+                elif walker.get_child_dds(_get_tag_name(e)) in MO_STATEMENT_TYPES:
+                    self.child_mos.get(_get_tag_name(e)).entry_xml(e).set_as_xml(e)
+
+    def _set_as_json(self, value, is_root = False):
+        if not isinstance(value, dict):
+            raise make_exception(pysros_err_invalid_json_structure)
+
+        children_to_set = set()
+        for k, v in value.items():
+            if k.startswith("@"):
                 continue
+            self._walker.get_child(k) #module name check?
+            k = Identifier.from_model_string(k).name
+            if k in self._walker.get_local_key_names():
+                self.keys.set_as_json(k, v)
+            elif self._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES:
+                self.fields.set_as_json(k, v)
+            elif self._walker.get_child_dds(k) in MO_STATEMENT_TYPES:
+                self.child_mos.set_as_json(k, v)
             else:
-                if self._walker.get_child_dds(_get_tag(e)) in (Model.StatementType.leaf_, Model.StatementType.leaf_list_) and _get_tag(e) not in self._walker.get_local_key_names():
-                    self.fields.get(_get_tag(e)).set_or_append_as_xml(e)
-                elif self._walker.get_child_dds(_get_tag(e)) in (Model.StatementType.list_, Model.StatementType.container_):
-                    self.child_mos.get_or_create(_get_tag(e)).set_as_xml(e)
+                raise make_exception(pysros_err_unknown_dds, dds=self._walker.get_child_dds(k))
+            name = Identifier.from_model_string(k).name
+            if name in children_to_set:
+                raise make_exception(pysros_err_duplicate_found, duplicate=name)
+            children_to_set.add(name)
 
     def delete(self):
         self._storage._operation = "delete"
 
     def replace(self):
         self._storage._operation = "replace"
 
+    def is_compare_supported_endpoint(self):
+        return True
+
 class GetValuePlaceholder(metaclass=_Singleton):
     pass
 
 class FieldValuePlaceholder(metaclass=_Singleton):
     pass
 
 class Delete(metaclass=_Singleton):
```

### Comparing `pysros-22.7.2/pysros/tokenizer.py` & `pysros-23.3.1/pysros/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pysros-22.7.2/pysros.egg-info/PKG-INFO` & `pysros-23.3.1/pysros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 22.7.2
+Version: 23.3.1
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
```

### Comparing `pysros-22.7.2/setup.py` & `pysros-23.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pysros',
-    version='22.7.2',
+    version='23.3.1',
     packages=['pysros'],
     url='https://www.nokia.com',
     license='Copyright 2021 Nokia.  License available in the LICENSE.md file.',
     author='Nokia',
     author_email='',
     description='Python for the Nokia Service Router Operating Systems (pySROS)',
     project_urls={
@@ -23,14 +23,14 @@
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Topic :: Internet",
         "Development Status :: 5 - Production/Stable",
     ],
     install_requires=[
         "ncclient~=0.6.12",
-        "lxml~=4.6.3",
+        "lxml~=4.9.2",
     ],
     python_requires=">=3.6",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

