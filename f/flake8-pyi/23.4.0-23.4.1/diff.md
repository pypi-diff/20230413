# Comparing `tmp/flake8_pyi-23.4.0.tar.gz` & `tmp/flake8_pyi-23.4.1.tar.gz`

## Comparing `flake8_pyi-23.4.0.tar` & `flake8_pyi-23.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.editorconfig
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.flake8
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    79960 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/pyi.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/scripts/typeshed_primer_download_errors.js
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/scripts/typeshed_primer_post_comment.js
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/check.yml
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/typeshed_primer.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/typeshed_primer_comment.yml
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/aliases.pyi
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/attribute_annotations.pyi
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/calls.pyi
--rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/classdefs.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/comparisons.pyi
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/defaults.pyi
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/defaults_py38.pyi
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/del.pyi
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/emptyclasses.pyi
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/emptyfunctions.pyi
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/exit_methods.pyi
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/forward_refs.pyi
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/forward_refs_annassign.pyi
--rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/imports.pyi
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/names_requiring_values.pyi
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/never_vs_noreturn.pyi
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/pep604_union_types.pyi
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/quotes.pyi
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/sysplatform.pyi
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/sysversioninfo.pyi
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/test_pyi_files.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/type_comments.pyi
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/typevar.pyi
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/union_duplicates.pyi
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/unused_things.pyi
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/vanilla_flake8_not_clean_forward_refs.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/LICENSE
--rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/README.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/pyproject.toml
--rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.editorconfig
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.flake8
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    81855 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/pyi.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/scripts/typeshed_primer_download_errors.js
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/scripts/typeshed_primer_post_comment.js
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/typeshed_primer.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/typeshed_primer_comment.yml
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/aliases.pyi
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/attribute_annotations.pyi
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/calls.pyi
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/classdefs.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/comparisons.pyi
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/defaults.pyi
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/defaults_py38.pyi
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/del.pyi
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/emptyclasses.pyi
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/emptyfunctions.pyi
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/exit_methods.pyi
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/forward_refs.pyi
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/forward_refs_annassign.pyi
+-rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/imports.pyi
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/names_requiring_values.pyi
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/never_vs_noreturn.pyi
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/pep604_union_types.pyi
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/quotes.pyi
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/sysplatform.pyi
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/sysversioninfo.pyi
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/test_pyi_files.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/type_comments.pyi
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/typevar.pyi
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/union_duplicates.pyi
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/unused_things.pyi
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/vanilla_flake8_not_clean_forward_refs.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/LICENSE
+-rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/README.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/pyproject.toml
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/PKG-INFO
```

### Comparing `flake8_pyi-23.4.0/.flake8` & `flake8_pyi-23.4.1/.flake8`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.pre-commit-config.yaml` & `flake8_pyi-23.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/CHANGELOG.md` & `flake8_pyi-23.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change Log
 
+## 23.4.1
+
+New error codes:
+* Y055: Unions of the form `type[X] | type[Y]` can be simplified to `type[X | Y]`.
+  Similarly, `Union[type[X], type[Y]]` can be simplified to `type[Union[X, Y]]`.
+  Contributed by [tomasr8](https://github.com/tomasr8).
+
 ## 23.4.0
 
 * Update error messages for Y019 and Y034 to recommend using
   `typing_extensions.Self` rather than `_typeshed.Self`.
 
 ## 23.3.1
```

### Comparing `flake8_pyi-23.4.0/CONTRIBUTING.md` & `flake8_pyi-23.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/pyi.py` & `flake8_pyi-23.4.1/pyi.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 
 if TYPE_CHECKING:
     # We don't have typing_extensions as a runtime dependency,
     # but all our annotations are stringized due to __future__ annotations,
     # and mypy thinks typing_extensions is part of the stdlib.
     from typing_extensions import Literal, TypeAlias, TypeGuard
 
-__version__ = "23.4.0"
+__version__ = "23.4.1"
 
 LOG = logging.getLogger("flake8.pyi")
 FLAKE8_MAJOR_VERSION = flake8.__version_info__[0]
 
 if sys.version_info >= (3, 9):
-    _LiteralMember: TypeAlias = ast.expr
+    _SliceContents: TypeAlias = ast.expr
 else:
-    _LiteralMember: TypeAlias = Union[ast.expr, ast.slice]
+    _SliceContents: TypeAlias = Union[ast.expr, ast.slice]
 
 
 class Error(NamedTuple):
     lineno: int
     col: int
     message: str
     type: type
@@ -360,14 +360,15 @@
 _is_abstractmethod = partial(_is_object, name="abstractmethod", from_={"abc"})
 _is_Any = partial(_is_object, name="Any", from_={"typing"})
 _is_overload = partial(_is_object, name="overload", from_=_TYPING_MODULES)
 _is_final = partial(_is_object, name="final", from_=_TYPING_MODULES)
 _is_Self = partial(_is_object, name="Self", from_=({"_typeshed"} | _TYPING_MODULES))
 _is_TracebackType = partial(_is_object, name="TracebackType", from_={"types"})
 _is_builtins_object = partial(_is_object, name="object", from_={"builtins"})
+_is_builtins_type = partial(_is_object, name="type", from_={"builtins"})
 _is_Unused = partial(_is_object, name="Unused", from_={"_typeshed"})
 _is_Iterable = partial(_is_object, name="Iterable", from_={"typing", "collections.abc"})
 _is_AsyncIterable = partial(
     _is_object, name="AsyncIterable", from_={"collections.abc"} | _TYPING_MODULES
 )
 _is_Protocol = partial(_is_object, name="Protocol", from_=_TYPING_MODULES)
 _is_NoReturn = partial(_is_object, name="NoReturn", from_=_TYPING_MODULES)
@@ -632,21 +633,26 @@
 
 class UnionAnalysis(NamedTuple):
     members_by_dump: defaultdict[str, list[ast.expr]]
     dupes_in_union: bool
     builtins_classes_in_union: set[str]
     multiple_literals_in_union: bool
     non_literals_in_union: bool
-    combined_literal_members: list[_LiteralMember]
+    combined_literal_members: list[_SliceContents]
+    # type subscript == type[Foo]
+    multiple_type_subscripts_in_union: bool
+    combined_type_subscripts: list[_SliceContents]
 
 
 def _analyse_union(members: Sequence[ast.expr]) -> UnionAnalysis:
     """Return a tuple providing analysis of a given sequence of union members.
 
-    >>> union = _ast_node_for('Union[int, memoryview, memoryview, Literal["foo"], Literal[1]]')
+    >>> union = _ast_node_for(
+    ...     'Union[int, memoryview, memoryview, Literal["foo"], Literal[1], type[float], type[str]]'
+    ... )
     >>> members = union.slice.elts if sys.version_info >= (3, 9) else union.slice.value.elts
     >>> analysis = _analyse_union(members)
     >>> len(analysis.members_by_dump["Name(id='memoryview', ctx=Load())"])
     2
     >>> analysis.dupes_in_union
     True
     >>> "int" in analysis.builtins_classes_in_union
@@ -655,47 +661,56 @@
     False
     >>> analysis.multiple_literals_in_union
     True
     >>> analysis.non_literals_in_union
     True
     >>> unparse(ast.Tuple(analysis.combined_literal_members))
     "('foo', 1)"
+    >>> analysis.multiple_type_subscripts_in_union
+    True
+    >>> unparse(ast.Tuple(analysis.combined_type_subscripts))
+    '(float, str)'
     """
 
     non_literals_in_union = False
     members_by_dump: defaultdict[str, list[ast.expr]] = defaultdict(list)
     builtins_classes_in_union: set[str] = set()
     literals_in_union = []
-    combined_literal_members: list[_LiteralMember] = []
+    combined_literal_members: list[_SliceContents] = []
+    type_subscripts_in_union: list[_SliceContents] = []
 
     for member in members:
         members_by_dump[ast.dump(member)].append(member)
         name_if_builtins_cls = _get_name_of_class_if_from_modules(
             member, modules={"builtins"}
         )
         if name_if_builtins_cls is not None:
             builtins_classes_in_union.add(name_if_builtins_cls)
         if isinstance(member, ast.Subscript) and _is_Literal(member.value):
             literals_in_union.append(member.slice)
         else:
             non_literals_in_union = True
+        if isinstance(member, ast.Subscript) and _is_builtins_type(member.value):
+            type_subscripts_in_union.append(member.slice)
 
     for literal in literals_in_union:
         if isinstance(literal, ast.Tuple):
             combined_literal_members.extend(literal.elts)
         else:
             combined_literal_members.append(literal)
 
     return UnionAnalysis(
         members_by_dump=members_by_dump,
         dupes_in_union=any(len(lst) > 1 for lst in members_by_dump.values()),
         builtins_classes_in_union=builtins_classes_in_union,
         multiple_literals_in_union=len(literals_in_union) >= 2,
         non_literals_in_union=non_literals_in_union,
         combined_literal_members=combined_literal_members,
+        multiple_type_subscripts_in_union=len(type_subscripts_in_union) >= 2,
+        combined_type_subscripts=type_subscripts_in_union,
     )
 
 
 _ALLOWED_MATH_ATTRIBUTES_IN_DEFAULTS = frozenset(
     {"math.inf", "math.nan", "math.e", "math.pi", "math.tau"}
 )
 
@@ -1242,32 +1257,38 @@
             node_value, (ast.Attribute, ast.Name)
         ):
             return
 
         if node_value and not _is_valid_default_value_with_annotation(node_value):
             self.error(node, Y015)
 
-    def _check_union_members(self, members: Sequence[ast.expr]) -> None:
+    def _check_union_members(
+        self, members: Sequence[ast.expr], is_pep_604_union: bool
+    ) -> None:
         first_union_member = members[0]
         analysis = _analyse_union(members)
 
         for member_list in analysis.members_by_dump.values():
             if len(member_list) >= 2:
                 self.error(member_list[1], Y016.format(unparse(member_list[1])))
 
         if not analysis.dupes_in_union:
             self._check_for_Y051_violations(analysis)
             if analysis.multiple_literals_in_union:
                 self._error_for_multiple_literals_in_union(first_union_member, analysis)
+            elif analysis.multiple_type_subscripts_in_union:
+                self._error_for_multiple_type_subscripts_in_union(
+                    first_union_member, analysis, is_pep_604_union
+                )
             if self.visiting_arg.active:
                 self._check_for_redundant_numeric_unions(first_union_member, analysis)
 
     def _check_for_Y051_violations(self, analysis: UnionAnalysis) -> None:
         """Search for redundant unions fitting the pattern `str | Literal["foo"]`, etc."""
-        literal_classes_present: defaultdict[str, list[_LiteralMember]]
+        literal_classes_present: defaultdict[str, list[_SliceContents]]
         literal_classes_present = defaultdict(list)
         for literal in analysis.combined_literal_members:
             if isinstance(literal, ast.Str):
                 literal_classes_present["str"].append(literal)
             elif isinstance(literal, ast.Bytes):
                 literal_classes_present["bytes"].append(literal)
             elif isinstance(literal, ast.Num):
@@ -1315,14 +1336,35 @@
         if analysis.non_literals_in_union:
             suggestion = f'Combine them into one, e.g. "Literal[{new_literal_slice}]".'
         else:
             suggestion = f'Use a single Literal, e.g. "Literal[{new_literal_slice}]".'
 
         self.error(first_union_member, Y030.format(suggestion=suggestion))
 
+    def _error_for_multiple_type_subscripts_in_union(
+        self,
+        first_union_member: ast.expr,
+        analysis: UnionAnalysis,
+        is_pep_604_union: bool,
+    ) -> None:
+        # Union using bit or, e.g. type[str] | type[int]
+        if is_pep_604_union:
+            new_union = " | ".join(
+                unparse(expr) for expr in analysis.combined_type_subscripts
+            )
+        # Union is the explicit Union type, e.g. Union[type[str], type[int]]
+        else:
+            type_slice = unparse(ast.Tuple(analysis.combined_type_subscripts)).strip(
+                "()"
+            )
+            new_union = f"Union[{type_slice}]"
+
+        suggestion = f'Combine them into one, e.g. "type[{new_union}]".'
+        self.error(first_union_member, Y055.format(suggestion=suggestion))
+
     def visit_BinOp(self, node: ast.BinOp) -> None:
         if not isinstance(node.op, ast.BitOr):
             self.generic_visit(node)
             return
 
         # str|int|None parses as BinOp(BinOp(str, |, int), |, None)
         current: ast.expr = node
@@ -1335,15 +1377,15 @@
         members.reverse()
 
         # Do not call generic_visit(node),
         # that would call this method again unnecessarily
         for member in members:
             self.visit(member)
 
-        self._check_union_members(members)
+        self._check_union_members(members, is_pep_604_union=True)
 
     def visit_Subscript(self, node: ast.Subscript) -> None:
         subscripted_object = node.value
         subscripted_object_name = _get_name_of_class_if_from_modules(
             subscripted_object, modules=_TYPING_MODULES
         )
         self.visit(subscripted_object)
@@ -1355,15 +1397,15 @@
         if isinstance(node.slice, ast.Tuple):
             self._visit_slice_tuple(node.slice, subscripted_object_name)
         else:
             self.visit(node.slice)
 
     def _visit_slice_tuple(self, node: ast.Tuple, parent: str | None) -> None:
         if parent == "Union":
-            self._check_union_members(node.elts)
+            self._check_union_members(node.elts, is_pep_604_union=False)
             self.visit(node)
         elif parent == "Annotated":
             # Allow literals, except in the first argument
             if len(node.elts) > 1:
                 self.visit(node.elts[0])
                 with self.string_literals_allowed.enabled():
                     for elt in node.elts[1:]:
@@ -2080,7 +2122,8 @@
 Y051 = 'Y051 "{literal_subtype}" is redundant in a union with "{builtin_supertype}"'
 Y052 = 'Y052 Need type annotation for "{variable}"'
 Y053 = "Y053 String and bytes literals >50 characters long are not permitted"
 Y054 = (
     "Y054 Numeric literals with a string representation "
     ">10 characters long are not permitted"
 )
+Y055 = 'Y055 Multiple "type[Foo]" members in a union. {suggestion}'
```

### Comparing `flake8_pyi-23.4.0/.github/scripts/typeshed_primer_download_errors.js` & `flake8_pyi-23.4.1/.github/scripts/typeshed_primer_download_errors.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.github/scripts/typeshed_primer_post_comment.js` & `flake8_pyi-23.4.1/.github/scripts/typeshed_primer_post_comment.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.github/workflows/check.yml` & `flake8_pyi-23.4.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.github/workflows/publish.yml` & `flake8_pyi-23.4.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.github/workflows/typeshed_primer.yml` & `flake8_pyi-23.4.1/.github/workflows/typeshed_primer.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.github/workflows/typeshed_primer_comment.yml` & `flake8_pyi-23.4.1/.github/workflows/typeshed_primer_comment.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/aliases.pyi` & `flake8_pyi-23.4.1/tests/aliases.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/attribute_annotations.pyi` & `flake8_pyi-23.4.1/tests/attribute_annotations.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/calls.pyi` & `flake8_pyi-23.4.1/tests/calls.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/classdefs.pyi` & `flake8_pyi-23.4.1/tests/classdefs.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/defaults.pyi` & `flake8_pyi-23.4.1/tests/defaults.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/emptyfunctions.pyi` & `flake8_pyi-23.4.1/tests/emptyfunctions.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/exit_methods.pyi` & `flake8_pyi-23.4.1/tests/exit_methods.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/imports.pyi` & `flake8_pyi-23.4.1/tests/imports.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/names_requiring_values.pyi` & `flake8_pyi-23.4.1/tests/names_requiring_values.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/never_vs_noreturn.pyi` & `flake8_pyi-23.4.1/tests/never_vs_noreturn.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/pep604_union_types.pyi` & `flake8_pyi-23.4.1/tests/pep604_union_types.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/quotes.pyi` & `flake8_pyi-23.4.1/tests/quotes.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/sysversioninfo.pyi` & `flake8_pyi-23.4.1/tests/sysversioninfo.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/test_pyi_files.py` & `flake8_pyi-23.4.1/tests/test_pyi_files.py`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/type_comments.pyi` & `flake8_pyi-23.4.1/tests/type_comments.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/typevar.pyi` & `flake8_pyi-23.4.1/tests/typevar.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/tests/unused_things.pyi` & `flake8_pyi-23.4.1/tests/unused_things.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/.gitignore` & `flake8_pyi-23.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/LICENSE` & `flake8_pyi-23.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/README.md` & `flake8_pyi-23.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 | Y048 | Function bodies should contain exactly one statement. (Note that if a function body includes a docstring, the docstring counts as a "statement".)
 | Y049 | A private `TypedDict` should be used at least once in the file in which it is defined.
 | Y050 | Prefer `typing_extensions.Never` over `typing.NoReturn` for argument annotations. This is a purely stylistic choice in the name of readability.
 | Y051 | Y051 detects redundant unions between `Literal` types and builtin supertypes. For example, `Literal[5]` is redundant in the union `int \| Literal[5]`, and `Literal[True]` is redundant in the union `Literal[True] \| bool`.
 | Y052 | Y052 disallows assignments to constant values where the assignment does not have a type annotation. For example, `x = 0` in the global namespace is ambiguous in a stub, as there are four different types that could be inferred for the variable `x`: `int`, `Final[int]`, `Literal[0]`, or `Final[Literal[0]]`. Enum members are excluded from this check, as are various special assignments such as `__all__` and `__match_args__`.
 | Y053 | Only string and bytes literals <=50 characters long are permitted.
 | Y054 | Only numeric literals with a string representation <=10 characters long are permitted.
+| Y055 | Unions of the form `type[X] \| type[Y]` can be simplified to `type[X \| Y]`. Similarly, `Union[type[X], type[Y]]` can be simplified to `type[Union[X, Y]]`.
 
 Note that several error codes recommend using types from `typing_extensions` or
 `_typeshed`. Strictly speaking, these packages are not part of the standard
 library. However, these packages are included in typeshed's `stdlib/`
 directory, meaning that type checkers believe them to be part of the standard
 library even if this does not reflect the reality at runtime. As such, since
 stubs are never executed at runtime, types from `typing_extensions` and
```

### Comparing `flake8_pyi-23.4.0/pyproject.toml` & `flake8_pyi-23.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.0/PKG-INFO` & `flake8_pyi-23.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pyi
-Version: 23.4.0
+Version: 23.4.1
 Summary: A plugin for flake8 to enable linting .pyi stub files.
 Project-URL: Homepage, https://github.com/PyCQA/flake8-pyi
 Project-URL: Source, https://github.com/PyCQA/flake8-pyi
 Project-URL: Bug Tracker, https://github.com/PyCQA/flake8-pyi/issues
 Project-URL: Changelog, https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md
 Author-email: Łukasz Langa <=lukasz@langa.pl>
 Maintainer: Sebastian Rittau, Akuli, Shantanu
@@ -127,14 +127,15 @@
 | Y048 | Function bodies should contain exactly one statement. (Note that if a function body includes a docstring, the docstring counts as a "statement".)
 | Y049 | A private `TypedDict` should be used at least once in the file in which it is defined.
 | Y050 | Prefer `typing_extensions.Never` over `typing.NoReturn` for argument annotations. This is a purely stylistic choice in the name of readability.
 | Y051 | Y051 detects redundant unions between `Literal` types and builtin supertypes. For example, `Literal[5]` is redundant in the union `int \| Literal[5]`, and `Literal[True]` is redundant in the union `Literal[True] \| bool`.
 | Y052 | Y052 disallows assignments to constant values where the assignment does not have a type annotation. For example, `x = 0` in the global namespace is ambiguous in a stub, as there are four different types that could be inferred for the variable `x`: `int`, `Final[int]`, `Literal[0]`, or `Final[Literal[0]]`. Enum members are excluded from this check, as are various special assignments such as `__all__` and `__match_args__`.
 | Y053 | Only string and bytes literals <=50 characters long are permitted.
 | Y054 | Only numeric literals with a string representation <=10 characters long are permitted.
+| Y055 | Unions of the form `type[X] \| type[Y]` can be simplified to `type[X \| Y]`. Similarly, `Union[type[X], type[Y]]` can be simplified to `type[Union[X, Y]]`.
 
 Note that several error codes recommend using types from `typing_extensions` or
 `_typeshed`. Strictly speaking, these packages are not part of the standard
 library. However, these packages are included in typeshed's `stdlib/`
 directory, meaning that type checkers believe them to be part of the standard
 library even if this does not reflect the reality at runtime. As such, since
 stubs are never executed at runtime, types from `typing_extensions` and
```

