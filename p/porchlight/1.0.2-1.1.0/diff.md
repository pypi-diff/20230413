# Comparing `tmp/porchlight-1.0.2.tar.gz` & `tmp/porchlight-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porchlight-1.0.2.tar", max compression
+gzip compressed data, was "porchlight-1.1.0.tar", max compression
```

## Comparing `porchlight-1.0.2.tar` & `porchlight-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-03-10 00:08:43.891543 porchlight-1.0.2/LICENSE
--rw-r--r--   0        0        0     2668 2023-03-10 00:08:43.891543 porchlight-1.0.2/README.md
--rw-r--r--   0        0        0      199 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/__init__.py
--rw-r--r--   0        0        0    33565 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/door.py
--rw-r--r--   0        0        0    29265 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/neighborhood.py
--rw-r--r--   0        0        0     4628 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/param.py
--rw-r--r--   0        0        0      221 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/README.md
--rw-r--r--   0        0        0        0 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/__init__.py
--rw-r--r--   0        0        0    11767 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_basedoor.py
--rw-r--r--   0        0        0    11812 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_door.py
--rw-r--r--   0        0        0     4605 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_dynamicdoor.py
--rw-r--r--   0        0        0    26662 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_neighborhood.py
--rw-r--r--   0        0        0     2948 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_param.py
--rw-r--r--   0        0        0     4842 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_utils_inspect_functions.py
--rw-r--r--   0        0        0     2124 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/tests/test_utils_typing_functions.py
--rw-r--r--   0        0        0        0 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/utils/__init__.py
--rw-r--r--   0        0        0     2113 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/utils/inspect_functions.py
--rw-r--r--   0        0        0     2532 2023-03-10 00:08:43.927543 porchlight-1.0.2/porchlight/utils/typing_functions.py
--rw-r--r--   0        0        0      392 2023-03-10 00:08:43.927543 porchlight-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 porchlight-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 08:32:20.484620 porchlight-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2594 2023-04-13 08:32:20.484620 porchlight-1.1.0/README.md
+-rw-r--r--   0        0        0      835 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/__init__.py
+-rw-r--r--   0        0        0    35222 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/door.py
+-rw-r--r--   0        0        0    28904 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/neighborhood.py
+-rw-r--r--   0        0        0     5841 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/param.py
+-rw-r--r--   0        0        0      167 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/tests/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/tests/__init__.py
+-rw-r--r--   0        0        0    11767 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/tests/test_basedoor.py
+-rw-r--r--   0        0        0    11812 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/tests/test_door.py
+-rw-r--r--   0        0        0     4605 2023-04-13 08:32:20.516620 porchlight-1.1.0/porchlight/tests/test_dynamicdoor.py
+-rw-r--r--   0        0        0    26847 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/tests/test_neighborhood.py
+-rw-r--r--   0        0        0     2948 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/tests/test_param.py
+-rw-r--r--   0        0        0     4842 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/tests/test_utils_inspect_functions.py
+-rw-r--r--   0        0        0     2124 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/tests/test_utils_typing_functions.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/utils/__init__.py
+-rw-r--r--   0        0        0     2113 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/utils/inspect_functions.py
+-rw-r--r--   0        0        0     2532 2023-04-13 08:32:20.520620 porchlight-1.1.0/porchlight/utils/typing_functions.py
+-rw-r--r--   0        0        0      392 2023-04-13 08:32:20.520620 porchlight-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3166 1970-01-01 00:00:00.000000 porchlight-1.1.0/PKG-INFO
```

### Comparing `porchlight-1.0.2/LICENSE` & `porchlight-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/README.md` & `porchlight-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="docs/source/porchlight_logo.gif" width="200" height="200" alt="porchlight logo. A snake's head erupts from the bottom of a porchlight casing, reaching towards a spinning triangular pyramid. The pyramid radiates bright, saturated, multicolored light." style="float:left" />
+<img src="docs/source/porchlight_logo.gif" width="200" height="200" alt="porchlight logo. A snake's head erupts from the bottom of a Victorian-style porchlight casing, reaching towards a spinning triangular pyramid. The pyramid radiates bright, saturated, multicolored light." style="float:left" />
 
 [porchlight](https://porchlight.readthedocs.io/en/latest/)
 ==========
 
 `porchlight` is a function management suite that handles shared inputs and
 outputs of methods and/or functions which evolve over the lifetime of a program.
 
@@ -13,16 +13,15 @@
 `porchlight` does not have any dependencies outside of the standard CPython
 library. Please note that `porchlight` requires Python 3.9\+, and that examples
 may require external libraries such as `numpy` and `matplotlib`.
 
 Installation
 ------------
 
-You can install `porchlight` by cloning this repository to a local directory.
-Alternatively, you may use `pip` in the command line:
+You can install `porchlight` using `pip`:
 ```console
 pip install porchlight
 ```
 
 Usage
 -----
```

### Comparing `porchlight-1.0.2/porchlight/door.py` & `porchlight-1.1.0/porchlight/door.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-"""
-.. |Basedoor| replace:: :py:class:`~porchlight.door.BaseDoor`
+"""Function adapter classes for callable Python objects.
+
+This module contains definitions for BaseDoor, Door, and DynamicDoor. It also
+defines the DoorError exception and DoorWarning warning.
+
+These objects all take a python callable object in some form, extract metadata
+from the object (if possible), and provide a calling interface with optional
+checks and actions (see individual descriptions).
+
 """
 import inspect
 import re
 import types
 
 from .param import Empty, ParameterError, Param
 from .utils.typing_functions import decompose_type
@@ -24,63 +31,71 @@
 
 
 class DoorWarning(Warning):
     pass
 
 
 class BaseDoor:
-    """Contains the basic information about a function such as expected
+    """Contains basic information about a function such as expected
     arguments, type annotations, and named return values.
 
     Attributes
     ----------
-    arguments : :py:obj:`dict`, :py:obj:`str`: :class:`~typing.Type`
-        Dictionary of all arguments taken as input when the `BaseDoor` object
+    arguments : :`dict`, `str`: :class:`~typing.Type`
+        Dictionary of all arguments taken as input when the |BaseDoor| object
         is called.
 
-    positional_only : :py:obj:`list` of :py:obj:`str`
+    positional_only : `list` of `str`
         List of positional-only arguments accepted by the function.
 
-    keyword_args : :py:obj:`dict`, :py:obj:`str`: :class:`~typing.Any`
-        Keyword arguments accepted by the `BaseDoor` as input when called. This
+    keyword_args : `dict`, `str`: :class:`~typing.Any`
+        Keyword arguments accepted by the |BaseDoor| as input when called. This
         includes all arguments that are not positional-only. Positional
         arguments without a default value are assigned a
         :class:~porchlight.param.Empty` value instead of their default value.
 
-    n_args : :py:obj:`int`
-        Number of arguments accepted by this `BaseDoor`
+    n_args : `int`
+        Number of arguments accepted by this |BaseDoor|
 
-    name : :py:obj:`str`
+    name : `str`
         The name of the function as visible from the base function's __name__.
 
-    return_types : :py:obj:`dict` of :py:obj:`str`, :py:obj:`Type` pairs.
+    return_types : `dict` of `str`, `Type` pairs.
         Values returned by any return statements in the base function.
 
-    return_vals : :py:obj:`list` of :py:obj:`str`
+    return_vals : `list` of `str`
         Names of parameters returned by the base function. Any return
         statements in a Door much haveidentical return parameters. I.e., the
-        following would fail if imported as a Door.
+        following would fail if used to initialize a Door.
 
         .. code-block:: python
 
            def fxn(x):
                if x < 1:
                    y = x + 1
                    return x, y
 
                return x
 
-    typecheck : :py:obj:`bool`
-        If True, when arguments are passed to the `BaseDoor`'s base function
-        the input types are checked against the types in `BaseDoor.arguments`.
-        If there is a mismatch, a `TypeError` will be thrown.
+    typecheck : `bool`
+        If True, when arguments are passed to the |BaseDoor|'s base function
+        the input types are checked against the types in
+        :py:attr:`BaseDoor.arguments`.  If there is a mismatch, a `TypeError`
+        will be thrown.
 
-    _base_function : :py:obj:`~typing.Callable`
-        This holds a reference to the function being managed by the `BaseDoor`
+    _base_function : `~typing.Callable`
+        This holds a reference to the function being managed by the |BaseDoor|
         instance.
+
+    Notes
+    -----
+    +   In version 2.0, this class will be permanently renamed or refactored. It
+        is strongly suggested you use |Door| or |PorchlightAdapter| unless
+        absolutely necessary, as those will remain forward and backward
+        compatible across the 2.0 update.
     """
 
     _base_function: Callable
     arguments: Dict[str, Type]
     keyword_args: Dict[str, Any]
     n_args: int
     name: str
@@ -90,47 +105,51 @@
 
     def __init__(
         self,
         function: Callable,
         typecheck: bool = True,
         returned_def_to_door: bool = False,
     ):
-        """Initializes the BaseDoor class. It takes any callable (function,
+        """Initializes the |BaseDoor| class. It takes any callable (function,
         lambda, method...) and inspects it to get at its arguments and
         structure.
 
         if typecheck is True (default True), the type of inputs passed to
-        BaseDoor.__call__ will be checked for matches to known input Types.
+        :py:class:`BaseDoor.__call__` will be checked for matches to known
+        input Types.
 
         Parameters
         ----------
         function : :py:class:`typing.Callable`
             The callable/function to be managed by the BaseDoor class.
 
-        typecheck : :py:obj:`bool`, optional
-            If `True`, the `BaseDoor` object will assert that arguments passed
-            to `__call__` (when the `BaseDoor` itself is called like a
-            function) have the type expected by type annotations and any user
-            specifications. By default, this is `True`.
+        typecheck : `bool`, optional
+            If `True`, the |BaseDoor| object will assert that arguments passed
+            to :py:class:`BaseDoor.__call__` (when the |BaseDoor| itself is
+            called like a function) have the type expected by type annotations
+            and any user specifications. By default, this is `True`.
 
-        returned_def_to_door : :py:obj:`bool`, optional
+        returned_def_to_door : `bool`, optional
             Returns a Door generated from the output of the base function.
-            Note, this is not the same as a DynamicDoor, and internal
-            variables/updating is not handled as with a DynamicDoor. This just
-            calls Door's initializer on the output of the base function.
+            Note, this is not the same as a |DynamicDoor|, and internal
+            variables/updating is not handled as with a |DynamicDoor|. This
+            just creates a new |Door| instance using the output of the base
+            function.
         """
         self._returned_def_to_door = returned_def_to_door
         self._base_function = function
         self.typecheck = typecheck
         self._inspect_base_callable()
 
         logging.debug(f"Door {self.name} initialized.")
 
     def __eq__(self, other) -> bool:
-        """Equality is defined as referencing the same base function."""
+        """|BaseDoor| equality is defined as referencing the same base
+        function.
+        """
         if isinstance(other, BaseDoor) and self.name is other.name:
             return True
 
         return False
 
     def __repr__(self):
         info = {
@@ -146,15 +165,15 @@
 
         return outstr
 
     def _inspect_base_callable(self):
         """Inspect the BaseDoor's baseline callable for primary attributes.
 
         This checks for type annotations, return statements, and all
-        information accessible to :py:obj:`inspect.Signature` relevant to
+        information accessible to `inspect.Signature` relevant to
         |BaseDoor|.
         """
         # Need to find the un-wrapped function that actually takes the
         # arguments in the end.
         function = get_wrapped_function(self._base_function)
 
         # Name may be otherwise assigned, this is a safe way to ensure that
@@ -192,18 +211,14 @@
             # This may be a real function that just doesn't have return types.
             logger.info(
                 f"Function proceeding without return types due to "
                 f"a TypeError raised while attempting to inspect the "
                 f"source: {e}"
             )
 
-            if isinstance(function, Callable):
-                # This is still a function, and has otherwise worked.
-                pass
-
         # Ensure the function can be inspected. If not, raise
         # NotImplementedError
         if not self._can_inspect(function):
             msg = (
                 f"Function {self.name} could not be inspected and is not "
                 f"yet supported. You should wrap the function within a "
                 f"user-defined function, something like:\n\n"
@@ -277,15 +292,15 @@
         else:
             self.return_vals = return_vals
 
         logger.debug(f"Found {self.n_args} arguments in {self.name}.")
 
     @property
     def __closure__(self):
-        """Since BaseDoor is a wrapper, and we use utils.get_all_source to
+        """Since |BaseDoor| is a wrapper, and we use utils.get_all_source to
         retrieve source, this mimicks the type a function wrapper would have
         here.
         """
         return (types.CellType(self._base_function),)
 
     def __call__(self, *args, **kwargs):
         """Calls the BaseDoor's function as normal.
@@ -363,41 +378,40 @@
         checking_for_returns = True
         main_def_found = False
 
         # These include mandatory space at the beginning since syntactically
         # there must exist non-\n whitespace for all lines after a funciton
         # definition.
         defmatch_str = r"^(\ )+def\s+"
-        retmatch_str = r".*\s+return\s(.*)"
         retmatch_str = r"^\s+(?:return|yield)\s(.*)"
         indentmatch_str = r"^(\s)*"
 
         for i, line in enumerate(lines):
             orig_line = line.strip()
 
-            # Remove comments
+            # Remove comments.
             if "#" in line:
                 line = line[: line.index("#")]
 
-            # Ignore empty lines
+            # Ignore empty lines.
             if not line.strip():
                 continue
 
             # Get the current indent level.
             indentmatch = re.match(indentmatch_str, line)
             cur_indent = len(indentmatch.group())
 
             # Ignore empty lines
             # Check for matches for both, in case there's something like
-            #   def wtf(): return 5
-            # Which is atrocious but possible.
+            #   def example(): return 5
+            # Which is atrocious but a valid definition.
             defmatch = re.match(defmatch_str, line)
             retmatch = re.match(retmatch_str, line)
 
-            # Ignore decorators
+            # Ignore decorators.
             if re.match(r"^\s*@\w+.*", line):
                 continue
 
             # Catch in-function definitions and ignore them.
             if defmatch and i > 0 and main_def_found:
                 checking_for_returns = False
                 last_check_indent = cur_indent
@@ -434,27 +448,26 @@
                 # SyntaxError. Trusting the parser here.
                 if not [v for v in vals if v != ""]:
                     # This is empty.
                     vals = []
 
                 for val in vals:
                     if not re.match(r"\w+$", val):
-                        # This is undefined, not an error. So assign return
-                        # value 'undefined' for this return statement and issue
-                        # a warning.
+                        # This is undefined, not an error. Issue a warning
+                        # since this may be unexpected behavior.
                         source_file = inspect.getfile(function)
 
                         msg = (
                             f"Could not define any set of return variable "
                             f"names for the following return line: \n"
                             f"{source_file}: {start_line+i}) "
                             f"{orig_line.strip()}\n While not crucial to "
                             f"this function, be aware that this means no "
-                            f"return value will be modified by this "
-                            f"callable."
+                            f"return parameter will be modified by this "
+                            f"callable in a Neighborhood."
                         )
 
                         logger.warning(msg)
 
                         warnings.warn(msg, DoorWarning)
 
                         vals = []
@@ -471,79 +484,77 @@
 
     @property
     def kwargs(self):
         return self.keyword_args
 
 
 class Door(BaseDoor):
-    """Inherits from and extends :class:`~porchlight.door.BaseDoor`"""
+    """Extends |BaseDoor| with Neighborhood-specific methods and handling."""
 
     def __init__(
         self,
         function: Callable = None,
         *,
         argument_mapping: dict = {},
         wrapped: bool = False,
         arguments: dict = {},
         keyword_args: dict = {},
         return_vals: List = [],
         name: str = "",
         typecheck: bool = False,
     ):
-        """Initializes the :py:class:`~porchlight.door.Door` object using a
-        callable.
+        """Initializes the |Door| object.
 
         Arguments
         ---------
 
         function : Callable
-            A callable object to be parsed by :py:class:`~BaseDoor`.
+            A callable object to be parsed by |BaseDoor|.
 
         argument_mapping : dict, keyword-only, optional
             Maps parameters automatically by name. For example, to have a Door
-            accept "a" and "b" ans arguments instead of "x" and "y", one could
+            accept "a" and "b" and arguments instead of "x" and "y", one could
             use
 
             .. code-block:: python
 
                 def fxn(x):
                     y = 2 * x
                     return y
 
                 my_door = Door(fxn, argument_mapping={'x': 'a', 'y': 'b'})
 
             to accomplish what would otherwise require wrapping the function
             yourself.
 
         wrapped : bool, keyword-only, optional
-            If `True`, will not parse the function using
-            :py:class:`~porchlight.door.BaseDoor`. Instead, it will take user
-            arguments and generate a function wrapper using the following
-            keyword-only arguments:
+            If `True`, will not parse the function using |BaseDoor|. Instead,
+            it will take user arguments and generate a function wrapper using
+            the following keyword-only arguments:
 
                 - arguments
                 - keyword_args
                 - return_vals
 
             And this wrapper will be used to initialize the
-            :py:class:`~porchlight.door.BaseDoor` properties.
+            |BaseDoor| properties.
 
         arguments : dict, keyword-only, optional
             Arguments to be passed to the function if it is wrapped. Does not
-            override :py:class:`~porchlight.door.BaseDoor` if ``wrapped`` is
+            override |BaseDoor| if ``wrapped`` is
             ``False``.
 
         keyword_args : dict, keyword-only, optional
             Corresponds to keyword arguments that may be passed positionally.
             Only used when ``wrapped`` is ``True``.
 
         name : str, keyword-only, optional
             Overrides the default name for the Door if provided.
 
-        typecheck : :py:obj:`bool`, optional
+        typecheck : `bool`, optional
             If `True`, the `Door` object will assert that arguments passed
             to `__call__` (when the `Door` itself is called like a
             function) have the type expected by type annotations and any user
             specifications. By default, this is `True`.
         """
         self.argmap = argument_mapping
         self.name = name
@@ -575,29 +586,29 @@
             return
 
         self.__call__(function)
 
     def _initialize_wrapped_function(
         self, arguments, keyword_args, return_vals
     ):
-        """Initializes a function that is auto-wrapped by
-        :py:class:`~porchlight.door.Door` instead of being passed to
-        :py:class:`~porchlight.door.BaseDoor`
+        """Initializes a function that is auto-wrapped by |Door| instead of
+        being passed to |BaseDoor|.
         """
         if not self.name:
             self.name = "AutoWrappedFunctionDoor"
             self.__name__ = self.name
 
         self.arguments = arguments
         self.keyword_args = keyword_args
         self.return_vals = return_vals
 
         self.function_initialized = True
 
     def __call__(self, *args, **kwargs):
+        # To account for @Door behavior in one call stack,
         if not self.function_initialized:
             # Need to recieve the function.
             if len(args) != 1:
                 msg = f"Expected a function, but recieved {args}"
 
                 if kwargs:
                     msg += f" and kwargs {kwargs}. Has Door been initialized?"
@@ -618,20 +629,17 @@
 
             # Perform any necessary argument mapping.
             self.map_arguments()
 
             return self
 
         if self.wrapped:
-            result = self._base_function(*args, **kwargs)
-            return result
+            return self._base_function(*args, **kwargs)
 
-        # Check argument mappings.
         if not self.argmap:
-            # Just pass arguments normally
             return super().__call__(*args, **kwargs)
 
         input_kwargs = {}
         for key, value in kwargs.items():
             if key in self.argmap:
                 input_kwargs[self.argmap[key]] = value
 
@@ -649,76 +657,99 @@
 
         self.arguments = _temp_arguments
         self.keyword_args = _temp_keyword_arguments
 
         return result
 
     def map_arguments(self):
-        """Maps arguments if self.argmap is not {}."""
+        """Maps arguments if self.argmap is not empty and the function has been
+        initialized.
+
+        This is done by modifying the door arguments directly, and using the
+        argument mapping as a converter between the two systems if the original
+        arguments are needed. This makes the |Door| mimic the same arguments
+        when accessed by a |Neighborhood| or when arguments are given to it.
+
+        Mapped arguments are *overridden*, meaning they will no longer be
+        recognized by the Door as appropriate arguments passed through
+        :py:meth:`Door.__call__`.
+        """
+        # Function metadata is required for argument mapping. Check this before
+        # checking argument mapping, since this should always be the case for
+        # Doors accepting a new argument map.
         if not self.function_initialized:
             msg = "Door has not yet been initialized with a function."
             logging.error(msg)
             raise DoorError(msg)
 
-        if self.argmap:
-            Door._check_argmap(self.argmap)
-
-            arg_order = tuple(self.arguments.keys())
-            kwarg_order = tuple(self.kwargs.keys())
-
-            for mapped_name, old_name in self.argmap.items():
-                # Catch mappings that would conflict with an existing key.
-                if mapped_name in self.arguments:
-                    msg = (
-                        f"Conflicting map key: {mapped_name} is in arguments "
-                        f"list."
-                    )
-
-                    logger.error(msg)
-                    raise DoorError(msg)
-
-                if old_name not in self.arguments and not any(
-                    old_name in retvals for retvals in self.return_vals
-                ):
-                    msg = f"{old_name} is not a valid argument for {self.name}"
-                    logger.error(msg)
-                    raise DoorError(msg)
-
-                if old_name in self.arguments:
-                    self.arguments[mapped_name] = self.arguments[old_name]
-                    del self.arguments[old_name]
+        if not self.argmap:
+            return
 
-                # Change keyword arguments as well.
-                if old_name in self.keyword_args:
-                    self.keyword_args[mapped_name] = self.keyword_args[old_name]
+        # After catching any yet-forseen inconsistencies that might arise in
+        # argument mapping, preserve the structure of the original arguments
+        # (especially order) and generate a new set of argument and return
+        # values using the mapped arguments.
+        Door._check_argmap(self.argmap)
+
+        arg_order = tuple(self.arguments.keys())
+        kwarg_order = tuple(self.kwargs.keys())
+
+        for mapped_name, old_name in self.argmap.items():
+            # Catch conflicts with existing keys.
+            if mapped_name in self.arguments:
+                msg = (
+                    f"Conflicting map key: {mapped_name} is in arguments "
+                    f"list."
+                )
 
-                    # Need to change the parameter name to reflect the mapping.
-                    self.keyword_args[mapped_name]._name = mapped_name
+                logger.error(msg)
+                raise DoorError(msg)
 
-                    del self.keyword_args[old_name]
+            # Check that the name exists in the Door's known arguments and
+            # return values, raise an error if not.
+            if old_name not in self.arguments and not any(
+                old_name in retvals for retvals in self.return_vals
+            ):
+                msg = f"{old_name} is not a valid argument for {self.name}"
+                logger.error(msg)
+                raise DoorError(msg)
 
-                # Also change outputs that contain the same name.
-                ret_tuple = self.return_vals
-                for i, ret_val in enumerate(ret_tuple):
-                    if old_name == ret_val:
-                        self.return_vals[i] = mapped_name
+            # Replace arguments with their mapped versions in the arguments
+            # dictionaries.
+            if old_name in self.arguments:
+                self.arguments[mapped_name] = self.arguments[old_name]
+                del self.arguments[old_name]
+
+            if old_name in self.keyword_args:
+                self.keyword_args[mapped_name] = self.keyword_args[old_name]
+
+                # Need to change the Param name to reflect the mapping.
+                self.keyword_args[mapped_name]._name = mapped_name
+
+                del self.keyword_args[old_name]
+
+            # Also change outputs that contain the same name.
+            ret_tuple = self.return_vals
+            for i, ret_val in enumerate(ret_tuple):
+                if old_name == ret_val:
+                    self.return_vals[i] = mapped_name
 
-            # Place back in the original order.
-            rev_argmap = {v: k for k, v in self.argmap.items()}
+        # Re-construct the newly mapped dictionaries, with all values in order.
+        rev_argmap = {v: k for k, v in self.argmap.items()}
 
-            arg_order = (
-                k if k not in rev_argmap else rev_argmap[k] for k in arg_order
-            )
+        arg_order = (
+            k if k not in rev_argmap else rev_argmap[k] for k in arg_order
+        )
 
-            kwarg_order = (
-                k if k not in rev_argmap else rev_argmap[k] for k in kwarg_order
-            )
+        kwarg_order = (
+            k if k not in rev_argmap else rev_argmap[k] for k in kwarg_order
+        )
 
-            self.arguments = {a: self.arguments[a] for a in arg_order}
-            self.keyword_args = {a: self.keyword_args[a] for a in kwarg_order}
+        self.arguments = {a: self.arguments[a] for a in arg_order}
+        self.keyword_args = {a: self.keyword_args[a] for a in kwarg_order}
 
     def _check_argmap(argmap):
         """Assesses if an argument mapping is valid, raises an appropriate
         exception if it is invalid. Will also raise warnings for certain
         non-fatal actions.
         """
         builtin_set = set(bi for bi in __builtins__.keys())
@@ -740,122 +771,135 @@
                 logger.warning(msg)
                 warnings.warn(msg, DoorWarning)
 
     def __repr__(self):
         return super().__repr__().replace("BaseDoor", "Door")
 
     @property
-    def original_arguments(self):
+    def original_arguments(self) -> dict[str, Type]:
+        """Returns a dict with original positional arguments required by the
+        base function.
+        """
         arguments = copy.copy(self.arguments)
 
         for i, arg in enumerate(self.arguments):
             if arg in self.argmap:
                 orig_arg = self.argmap[arg]
                 _type = arguments[arg]
 
                 arguments[orig_arg] = _type
                 del arguments[arg]
 
         return arguments
 
     @property
-    def original_kw_arguments(self):
+    def original_kw_arguments(self) -> dict[str, Type]:
+        """Returns a dict with original keyword arguments required by the base
+        function.
+        """
         arguments = copy.copy(self.keyword_args)
 
         for i, arg in enumerate(self.keyword_args):
             if arg in self.argmap:
                 orig_arg = self.argmap[arg]
                 _type = arguments[arg]
 
                 arguments[orig_arg] = _type
                 del arguments[arg]
 
         return arguments
 
     @property
-    def original_return_vals(self):
+    def original_return_vals(self) -> list[str]:
+        """Returns a list with original return values of the base function."""
         return_vals = copy.copy(self.return_vals)
 
         # Also change outputs that contain the same name.
         for i, ret_val in enumerate(return_vals):
             if ret_val in self.argmap:
                 return_vals[i] = self.argmap[ret_val]
 
         return return_vals
 
     @property
-    def argument_mapping(self):
+    def argument_mapping(self) -> dict[str, str]:
         return self.argmap
 
     @argument_mapping.setter
     def argument_mapping(self, value):
         self.arguments = self.original_arguments
         self.keyword_args = self.original_kw_arguments
         self.argmap = value
+
+        # Need to re-execute the argument mapper. By this time, the function
+        # must be initialized.
         self.map_arguments()
 
     @property
     def variables(self) -> List[str]:
-        """Returns a list of all known return values and input arguments."""
+        """Returns a list of all known return values and input arguments as
+        strs.
+        """
         all_vars = []
 
         for arg in self.arguments:
             if arg not in all_vars:
                 all_vars.append(arg)
 
         for ret in self.return_vals:
             if ret not in all_vars:
                 all_vars.append(ret)
 
         return all_vars
 
     @property
     def required_arguments(self) -> List[str]:
-        """Returns a list of arguments with no default values."""
+        """Returns a list of arguments with no default value."""
         required = []
 
         for x in self.arguments:
             if self.keyword_args[x].value == Empty():
                 required.append(x)
 
         return required
 
 
 class DynamicDoor(Door):
     """A dynamic door takes a door-generating function as its initializer.
 
-    Unlike :py:class:`~porchlight.door.BaseDoor` and
-    :py:class:`~porchlight.door.Door`, dynamic doors will only parse the
+    Unlike |BaseDoor| and |Door|, |DynamicDoor| will only parse the
     definition's source once it is generated.
 
-    These objects a function that returns a :py:class:`~porchlight.door.Door`.
-    The `DynamicDoor` then contains identical attributes to the generated door.
+    These objects a function that returns a |Door|.
+    The |DynamicDoor| then contains identical attributes to the generated door.
     Once called again, all attributes update to match the most recent call.
 
     Attributes
     ----------
     _door_generator : `Callable`
-        A function returning a `~porchlight.door.Door` as its output.
+        A function returning a |Door| as its output.
 
     generator_args : `List`
         List of arguments to be passed as positional arguments to the
-        `_door_generator` function.
+        :py:attr:`DynamicDoor._door_generator` function.
 
     generator_kwards : `Dict`
         Dict of key: value pairs representing keyword arguments to be passed as
-        positional arguments to the `_door_generator` function.
+        positional arguments to the :py:attr:`DynamicDoor._door_generator`
+        function.
     """
 
     def __init__(
         self,
         door_generator: Callable[Any, Door],
         generator_args: List = [],
         generator_kwargs: Dict = {},
     ):
-        """Initializes the Dynamic Door. When __call__ is invoked, the door
+        """Initializes the |DynamicDoor|. When
+        :py:meth:`DynamicDoor.__call__` is invoked, the door
         generator is called.
 
         Arguments
         ---------
         _door_generator : `~typing.Callable[Any, Door]`
             A callable function that returns an initialized Door object.
 
@@ -880,46 +924,45 @@
         self.keyword_only_args = {}
         self.return_vals = []
         self._cur_door = None
         self._last_door = None
 
     def __call__(self, *args, **kwargs) -> Any:
         """Executes the function stored in
-        `~porchlight.door.DynamicDoorc._base_function` once
-        `~porchlight.door.DynamicDoor.update` has executed.
+        :py:attr:`DynamicDoor._base_function` once
+        :py:meth:`DynamicDoor.update` has executed.
 
         Arguments
         ---------
         *args : positional arguments
-            Arguments directly passed to
-            `~porchlight.door.DynamicDoor._base_function`.
+            Arguments directly passed to :py:attr:`DynamicDoor._base_function`.
 
         **kwargs : keyword arguments
             Keyword arguments directly passed to
-            `~porchlight.door.DynamicDoor._base_function`.
+            :py:attr:`DynamicDoor._base_function`.
         """
         self.update()
         result = super().__call__(*args, **kwargs)
 
         return result
 
     def call_without_update(self, *args, **kwargs) -> Any:
         """Executes the function stored in
-        `~porchlight.door.DynamicDoor._base_function` *WITHOUT* executing
-        `~porchlight.door.DynamicDoor.update()`
+        :py:attr:`DynamicDoor._base_function` *WITHOUT* executing
+        :py:meth:`~porchlight.door.DynamicDoor.update()`
 
         Arguments
         ---------
         *args : positional arguments
             Arguments directly passed to
-            `~porchlight.door.DynamicDoor._base_function`.
+            :py:attr:`DynamicDoor._base_function`.
 
         **kwargs : keyword arguments
             Keyword arguments directly passed to
-            `~porchlight.door.DynamicDoor._base_function`.
+            :py:attr:`DynamicDoor._base_function`.
         """
         # Give a specific, useful message if self._base_function is not
         # initialized.
         if "_base_function" not in self.__dict__:
             msg = (
                 "DynamicDoor does not contain _base_function attribute. "
                 "Did you means to call DynamicDoor directly or with "
@@ -942,17 +985,17 @@
 
         except AttributeError:
             outstr = "DynamicDoor(uninitialized)"
 
         return outstr
 
     def update(self):
-        """Updates the DynamicDoor using `DynamicDoor._door_generator`
+        """Updates the DynamicDoor using :py:attr:`DynamicDoor._door_generator`
 
-        This method is called when DynamicDoor.__call__ is invoked.
+        This method is called when :py:meth:`DynamicDoor.__call__` is invoked.
         """
         self._last_door = self._cur_door
 
         updated_door = self._door_generator(
             *self.generator_args, **self.generator_kwargs
         )
```

### Comparing `porchlight-1.0.2/porchlight/neighborhood.py` & `porchlight-1.1.0/porchlight/neighborhood.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-"""Defines the `Neighborhood` class."""
+"""A mediator object for sequentially executing callables with a variable set
+of data values.
+
+The primary mediator object is the |Neighborhood| class. It acts as an
+interface for other parts of the |porchlight| library, meaning it will manage
+|Door| creation, |Param| assignment, and other checks. It can be further
+extended using user-defined |Door|.
+
+Also contains the definition for
+:py:class:`~porchlight.neighborhood.NeighborhoodError`.
+"""
 from . import door
 from . import param
 from .utils.typing_functions import decompose_type
 from typing import Any, Callable, Dict, List, Tuple, Union
 
 import logging
 
@@ -11,39 +21,37 @@
 
 class NeighborhoodError(Exception):
     pass
 
 
 class Neighborhood:
     """A neighborhood manages the interactions between Doors. It consists of a
-    modifiable collection of :class:`~porchlight.door.Door` (or
-    :class:`~porchlight.door.BaseDoor`) objects.
+    modifiable collection of |Door| (or |BaseDoor|) objects.
 
     Attributes
     ----------
-    _doors : :py:obj:`dict`, :py:obj:`str`: :class:`~porchlight.door.Door`
-        Contains all data for :class:`~porchlight.door.Door` objects. The keys
-        are, by default, the :meth:`~porchlight.door.Door.name`
-        property for the corresponding :class:`~porchlight.door.Door` values.
+    _doors : ``dict``, ``str``: |Door|
+        Contains all data for |Door| objects. The keys are, by default, the
+        :meth:`~porchlight.door.Door.name` property for the corresponding
+        |Door| values.
 
-    _params : :py:obj:`dict`, :py:obj:`str`: :class:`~porchlight.param.Param`
+    _params : ``dict``, ``str``: |Param|
         Contains all the parameters currently known to and managed by the
-        :class:`~porchlight.neighborhood.Neighborhood` object.
+        |Neighborhood| object.
+
+    _call_order : ``list``, ``str``
+        The order in which the |Door| objects in `_doors` are called. By
+        default, this is the order in which |Door| are added to the
+        |Neighborhood|.
 
-    _call_order : :py:obj:`list`, :py:obj:`str`
-        The order in which the :class:`~porchlight.door.Door` objects in
-        `_doors` are called. By default, this is the order in which
-        :class:`~porchlight.door.Door`s are added to the `Neighborhood`.
-
-    initialization : :py:obj:`list` of ``Callable``, `keyword-only`
-        These will be called once the
-        :class:`~porchlight.neighborhood.Neighborhood` object begins any
+    initialization : ``list`` of ``Callable``, `keyword-only`
+        These will be called once the |Neighborhood| object begins any
         execution (e.g., via
-        :py:meth:`~porchlight.neighborhood.Neighborhood.run_step`) will
-        run these callables. This will only execute again if
+        :py:meth:`~porchlight.neighborhood.Neighborhood.run_step`) will run
+        these callables. This will only execute again if
         ``Neighborhood.has_initialized`` is set to ``False``.
     """
 
     _doors: Dict[str, door.Door]
     _params: Dict[str, param.Param]
     _call_order: List[str]
 
@@ -116,26 +124,26 @@
         dynamic_door: bool = False,
     ):
         """Adds a new function to the Neighborhood object.
 
         Parameters
         ----------
         function : Callable
-            The function to be added. This is converted to a
-            :class:`~porchlight.door.Door` object by this method.
+            The function to be added. This is converted to a |Door| object by
+            this method.
 
         overwrite_defaults : bool, optional
             If `True`, will overwrite any parameters shared between the
             `function` and `Neighborhood._params` to be equal to the defaults
             set by `function`. If `False` (default), no parameters that exist
-            in the `Neighborhood` object already will be changed.
+            in the |Neighborhood| object already will be changed.
 
         dynamic_door : bool, optional
-            If `True` (default `False`), then the output(s) of this `Door` will
-            be converted into a `Door` or set of `Door`s in the `Neighborhood`
+            If `True` (default `False`), then the output(s) of this |Door| will
+            be converted into a |Door| or set of |Door| in the |Neighborhood|
             object.
         """
         new_door = door.Door(function)
         logging.debug(f"Adding new function to neighborhood: {new_door.name}")
 
         self.add_door(new_door, overwrite_defaults, dynamic_door)
 
@@ -145,31 +153,30 @@
         overwrite_defaults: bool = False,
         dynamic_door: bool = False,
     ):
         """Adds an already-initialized Door to the neighborhood.
 
         Parameters
         ----------
-        new_door : :class:`~porchlight.door.Door`,
-            :class:`~porchlight.door.DynamicDoor`, or :py:obj:`list` of
-            :class:`~porchlight.door.Door` objects.
+        new_door : |Door|,
+            |DynamicDoor|, or ``list`` of |Door| objects.
 
-            Either a single initialized `door.Door` object or a list of them.
+            Either a single initialized |Door| object or a list of them.
             If a list is provided, this function is called for each item in the
             list.
 
         overwrite_defaults : bool, optional
             If `True`, will overwrite any parameters shared between the
             `new_door` and `Neighborhood._params` to be equal to the defaults
             set by `new_door`. If `False` (default), no parameters that exist
-            in the `Neighborhood` object already will be changed.
+            in the |Neighborhood| object already will be changed.
 
         dynamic_door : bool, optional
-            If `True` (default `False`), then the output(s) of this `Door` will
-            be converted into a `Door` or set of `Door`s in the `Neighborhood`
+            If `True` (default `False`), then the output(s) of this |Door| will
+            be converted into a |Door| or set of |Door| in the |Neighborhood|
             object.
         """
         if isinstance(new_door, List):
             for nd in new_door:
                 self.add_door(
                     nd,
                     overwrite_defaults=overwrite_defaults,
@@ -239,20 +246,20 @@
                     template_ddoor.name = ret_val
                     template_ddoor.generator_kwargs = {"param_name": ret_val}
 
                     self.add_door(template_ddoor)
                     self.add_param(ret_val, param.Empty())
 
     def remove_door(self, name: str):
-        """Removes a :class:`~porchlight.door.Door` from :attr:`_doors`.
+        """Removes a |Door| from :attr:`_doors`.
 
         Parameters
         ----------
-        name : :py:obj:`str`
-            The name of the :class:`~porchlight.door.Door` to be removed. It
+        name : ``str``
+            The name of the |Door| to be removed. It
             must correspond to a key in `Neighborhood._doors` attribute.
 
         Raises
         ------
         KeyError
             If `name` is not present in `_doors` attribute.
         """
@@ -281,31 +288,31 @@
         ignore_constant: bool = False,
     ) -> param.Param:
         """Set the value of a parameter to a new value. Since parameters are
         not meant to be modified like this right now, generate a new parameter.
 
         Parameters
         ----------
-        parameter_name : :py:obj:`str`
+        parameter_name : ``str``
             The name of the parameter to modify.
 
         new_value : `Any`
             The value to be assigned to this parameter.
 
-        constant : :py:obj:`bool`
-            Will be passed to :class:`~porchlight.param.Param` as the
+        constant : ``bool``
+            Will be passed to |Param| as the
             `constant` keyword argument.
 
-        ignore_constant : :py:obj:`bool`, optional, keyword-only
+        ignore_constant : ``bool``, optional, keyword-only
             When assigning this parameter, it will ignore the `constant`
             attribute of the current parameter.
 
         Raises
         ------
-        :class:`~porchlight.param.ParameterError`
+        |ParameterError|
             Is raised if the parameter attempting to be changed has `True` for
             its `constant` attribute. Will not be raised by this method if
             `ignore_constant` is `True`.
         """
         _old_param = self._params[parameter_name]
 
         if not ignore_constant and _old_param.constant:
@@ -322,28 +329,28 @@
     def add_param(
         self,
         parameter_name: str,
         value: Any,
         constant: bool = False,
         restrict: Union[Callable, None] = None,
     ):
-        """Adds a new parameter to the `Neighborhood` object.
+        """Adds a new parameter to the |Neighborhood| object.
 
         The parameters all correspond to arguments passed directly to the
-        :class:`~porchlight.param.Param` initializer.
+        |Param| initializer.
 
         Parameters
         ----------
-        parameter_name : :py:obj:`str`
+        parameter_name : ``str``
             Name of the parameter being created.
 
         value : `Any`
             Parameter value
 
-        constant : :py:obj:`bool`, optional
+        constant : ``bool``, optional
             If `True`, the parameter is set to constant.
 
         restrict : :py:class:`~typing.Callable` or None, optional
             Either a callable that returns something that can be evaluated to
             True or False, or None. Raises an error if the parameter is set to
             a value that fails the restriction check.
 
@@ -383,15 +390,15 @@
 
         return True
 
     def call_all_doors(self):
         """Calls every door currently present in the neighborhood object.
 
         This order is currently dictated by the order in which
-        :class:`~porchlight.door.Door`s are added to the `Neighborhood`.
+        |Door| are added to the |Neighborhood|.
 
         The way this is currently set up, it will not handle positional
         arguments. That is, if an input cannot be passed using its variable
         name, this will break.
         """
         # Need to call the doors directly.
         for doorname in self._call_order:
@@ -527,22 +534,22 @@
         # call.
         return output
 
     def gather_door_arguments(
         self, input_door: door.Door, defaults: Dict[str, Any] = {}
     ) -> Tuple[List, Dict]:
         """This retrieves all parameters required by a
-        :py:class:`~porchlight.door.Door`, returning them as a list (positional
+        |Door|, returning them as a list (positional
         arguments) and a dictionary (keyword arguments). If there are no
         positional-only arguments and/or no no keyword arguments, then empty
         objects are returned.
 
         Arguments
         ---------
-        input_door : :py:class:`~porchlight.door.Door`
+        input_door : |Door|
             The door to gather necessary parameters for.
 
         defaults : dict[str, Any]
             Default values for any arguments that may be missing from the
             Neighborhood. Keys must correspond to an arg or kwarg present in
             the input_door.
 
@@ -553,15 +560,15 @@
 
         kwargs : dict[str, Any]
             Keyword arguments for the door.
 
         Notes
         -----
         The return values must be unpacked before being used to call the
-        :py:class:`~porchlight.door.Door`.
+        |Door|.
         """
         # Gather the arguments needed by the door. Defaults are folded into a
         # new dictionary to keep them temporary.
         req_params = input_door.arguments
         known_params = defaults | self._params
 
         input_params = {p: known_params[p].value for p in req_params}
@@ -578,15 +585,15 @@
 
         return args, kwargs
 
     def initialize(self):
         """Runs initialization functions present in
         :py:attr:`~porchlight.neighborhood.Neighborhood.initialization` if
         ``has_initialized`` is ``False`` for this
-        :py:class:`~porchlight.neighborhood.Neighborhood`.
+        |Neighborhood|.
         """
         # Do nothing if initialization has already happened.
         if self.has_initialized or not self.initialization:
             return
 
         # Ensure initialization is iterable, if not
         if not hasattr(self.initialization, "__iter__"):
@@ -643,15 +650,15 @@
                     self.add_param(retval, value)
 
     def finalize(self):
         """Finalization executes doors/callables found in
         ``Neighborhood.finalization``. It must be invoked directly by the user.
 
         Unlike initialization, finalization will add new constant
-        :py:class:`~porchlight.param.Param`s to the ``Neighborhood`` object.
+        |Param| to the `|Neighborhood|` object.
         """
         # Ensure finalization is iterable, if not raise either a ValueError
         # (because it is not a valid object) or TypeError (because it is not a
         # list nor a door.Door).
         if not hasattr(self.finalization, "__iter__"):
             self.finalization = [self.finalization]
 
@@ -722,21 +729,21 @@
 
         self.call_all_doors()
 
     def order_doors(self, order: List[str]):
         """Allows the doors to be ordered when called.
 
         If this is never called, the call order will be equivalent to the order
-        in which the doors are added to the `Neighborhood`. As of right now,
+        in which the doors are added to the |Neighborhood|. As of right now,
         all doors present must be included in the `order` argument or a
         `KeyError` will be thrown.
 
         Arguments
         ---------
-        order : :py:obj:`list`, str
+        order : ``list``, str
             The order for doors to be called in. Each `str` must correspond to
             a key in `Neighborhood._doors`.
         """
         # The order list must:
         #  + Contain all doors once.
         #  + All doors must already exist and be known.
         if not order:
```

### Comparing `porchlight-1.0.2/porchlight/param.py` & `porchlight-1.1.0/porchlight/param.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,35 @@
+"""A constainer class for arbitrary data, with type and state checking.
+
+|Param| is the primary class introduces in this file. |Empty| is a singleton
+class denoting an "empty" parameter. The :py:class:`ParameterError` class is
+also defined here.
+"""
 from typing import Any, Callable, Type, Union
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class ParameterError(Exception):
-    """Error for Param-specific issues."""
+    """Error for Param-specific exceptions."""
 
     pass
 
 
 class Empty:
     """An empty class representing missing parameters values.
 
-    At initializtion, if an instance does not already exist it is created.
+    At initialization, if an instance does not already exist it is created. No
+    instance of Empty exists until it has been instantiated once.
+
+    It is recommended that |Empty| be used over :py:obj:`None` to denote
+    parameters that have not been initialized with any value, so that
+    :py:obj:`None` can be treated unambiguously when using |porchlight|.
     """
 
     def __new__(cls):
         # Return the singleton instance if it exists already, otherwise become
         # the singleton instance.
         if not hasattr(cls, "_singleton_instance"):
             cls._singleton_instance = super(Empty, cls).__new__(cls)
@@ -33,36 +44,60 @@
             return False
 
     def __neq__(self, other):
         return not (self == other)
 
 
 class Param:
-    """Parameter class. while not frozen, for most purposes it should not be
-    modified outside of a porchlight object.
+    """Container class for arbitrary Python data.
 
-    `Param` uses `__slots__`, and no attributes other than those listed below
-    may be assigned to `Param` objects.
+    Although mutable, editing |Param| objects directly is strongly discouraged
+    unless absolutely necessary.
+
+    |Param| uses `__slots__`, and no attributes other than those listed below
+    may be assigned to |Param| objects.
 
     Attributes
     ----------
     _name : :py:obj:`str`
         Parameter name.
 
     _value : :py:class:`~typing.Any`
         Value of the parameter. If the parameter does not contain an assigned
-        value, this should be :class:`~porchlight.param.Empty`
+        value, this should be |Empty|.
 
     _type : :py:class:`~typing.type`
-        The type corresponding to the type of `Param._value`
+        The type corresponding to the type of :py:attr:`Param._value`.
 
     constants : :py:obj:`bool`
-        True if this object should be considered a constant. If the `Param`
-        value is modified by :class:`Param.value`'s `setter`, but `constant` is
-        True, a :class:`~porchlight.param.ParameterError` will be raised.
+        True if this object should be considered a constant. If the |Param|
+        value is modified by :py:attr:`Param.value`'s `setter`, but
+        `constant` is True, a :py:class:`~porchlight.param.ParameterError` will
+        be raised.
+
+    restrict : `Callable` or `None`
+        If a callable, it will be invoked on the parameter whenever the
+        parameter is changed. If it evaluates to False, a |ParameterError| is
+        raised.
+
+        Example: "temperature" parameter should not be negative or zero in our
+        model:
+
+        .. code-block::python
+
+            temp = Param(
+                "temperature",
+                restrict=lambda x: x > 0
+            )
+
+            # The below would raise a ParameterError, the check occuring
+            # automatically.
+            temp.value = -500
+
+        See :py:attr:`Param.value` for further details.
     """
 
     # A parameter, to be updated from the API, needs to be replaced rather than
     # reassigned. That said there are a few use cases where it may be useful to
     # have easy access, so just hiding these behind properties.
     __slots__ = ["_name", "_value", "constant", "_type", "restrict"]
 
@@ -81,15 +116,15 @@
             Parameter name.
 
         value : :py:class:`~typing.Any`
             Value of the parameter. If the parameter does not contain an
             assigned value, this should be `~porchlight.param.Empty`
 
         constant : :py:obj:`bool`
-            True if this object should be considered a constant. If the `Param`
+            True if this object should be considered a constant. If the |Param|
             value is modified by `Param.value`'s `setter`, but `constant` is
             True, a :class:`~porchlight.param.ParameterError` will be raised.
 
         restrict : :py:class:`~typing.Callable` or `None`
             If a callable is passed, whenever the value property of the
             parameter is set, restrict will be called on the candidate value.
             If the result evaluates to False, a ParameterError will be raised.
```

### Comparing `porchlight-1.0.2/porchlight/tests/test_basedoor.py` & `porchlight-1.1.0/porchlight/tests/test_basedoor.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/tests/test_door.py` & `porchlight-1.1.0/porchlight/tests/test_door.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/tests/test_dynamicdoor.py` & `porchlight-1.1.0/porchlight/tests/test_dynamicdoor.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/tests/test_neighborhood.py` & `porchlight-1.1.0/porchlight/tests/test_neighborhood.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,26 +752,29 @@
             return f"{arg}: {kwarg}"
 
         def inittest4(arg, kwarg=12):
             # Note: using a different kwarg default value here.
             retval_needed = f"{kwarg}: {arg}"
             return retval_needed
 
+        # This warns the user about the invalid return argument that will be
+        # ignored.
         neighborhood_4 = Neighborhood(
             initialization=[inittest1, inittest2, inittest3, inittest4]
         )
 
         neighborhood_4.add_param("retval_needed", None)
 
-        with self.assertRaises(KeyError):
+        with self.assertWarns(door.DoorWarning), self.assertRaises(KeyError):
             neighborhood_4.run_step()
 
         neighborhood_4.add_param("arg", "Hello world")
 
-        neighborhood_4.run_step()
+        with self.assertWarns(door.DoorWarning):
+            neighborhood_4.run_step()
 
     def test_plain_finalization(self):
         # Testing specifically a None-returning function.
         def inittest1():
             pass
 
         neighborhood = Neighborhood([], finalization=inittest1)
```

### Comparing `porchlight-1.0.2/porchlight/tests/test_param.py` & `porchlight-1.1.0/porchlight/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/tests/test_utils_inspect_functions.py` & `porchlight-1.1.0/porchlight/tests/test_utils_inspect_functions.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/tests/test_utils_typing_functions.py` & `porchlight-1.1.0/porchlight/tests/test_utils_typing_functions.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/utils/inspect_functions.py` & `porchlight-1.1.0/porchlight/utils/inspect_functions.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/porchlight/utils/typing_functions.py` & `porchlight-1.1.0/porchlight/utils/typing_functions.py`

 * *Files identical despite different names*

### Comparing `porchlight-1.0.2/PKG-INFO` & `porchlight-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: porchlight
-Version: 1.0.2
+Version: 1.1.0
 Summary: A function-managing package for models and systems with shared variables.
 License: GPL-3.0-or-later
 Author: Teal, D
 Author-email: teal.dillon@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-<img src="docs/source/porchlight_logo.gif" width="200" height="200" alt="porchlight logo. A snake's head erupts from the bottom of a porchlight casing, reaching towards a spinning triangular pyramid. The pyramid radiates bright, saturated, multicolored light." style="float:left" />
+<img src="docs/source/porchlight_logo.gif" width="200" height="200" alt="porchlight logo. A snake's head erupts from the bottom of a Victorian-style porchlight casing, reaching towards a spinning triangular pyramid. The pyramid radiates bright, saturated, multicolored light." style="float:left" />
 
 [porchlight](https://porchlight.readthedocs.io/en/latest/)
 ==========
 
 `porchlight` is a function management suite that handles shared inputs and
 outputs of methods and/or functions which evolve over the lifetime of a program.
 
@@ -28,16 +28,15 @@
 `porchlight` does not have any dependencies outside of the standard CPython
 library. Please note that `porchlight` requires Python 3.9\+, and that examples
 may require external libraries such as `numpy` and `matplotlib`.
 
 Installation
 ------------
 
-You can install `porchlight` by cloning this repository to a local directory.
-Alternatively, you may use `pip` in the command line:
+You can install `porchlight` using `pip`:
 ```console
 pip install porchlight
 ```
 
 Usage
 -----
```

