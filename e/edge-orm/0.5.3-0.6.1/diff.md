# Comparing `tmp/edge_orm-0.5.3.tar.gz` & `tmp/edge_orm-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.5.3.tar", max compression
+gzip compressed data, was "edge_orm-0.6.1.tar", max compression
```

## Comparing `edge_orm-0.5.3.tar` & `edge_orm-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.5.3/README.md
--rw-r--r--   0        0        0      774 2023-02-27 21:50:15.475075 edge_orm-0.5.3/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.5.3/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.5.3/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.5.3/edge_orm/execute.py
--rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.5.3/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.5.3/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.5.3/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.5.3/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.5.3/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.5.3/edge_orm/node/models.py
--rw-r--r--   0        0        0      259 2023-02-27 21:41:14.553137 edge_orm-0.5.3/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.5.3/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.5.3/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.5.3/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    40592 2023-04-11 22:22:13.354696 edge_orm-0.5.3/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.5.3/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3706 2023-02-08 20:21:01.356510 edge_orm-0.5.3/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.5.3/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.5.3/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.5.3/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    39673 2023-03-28 16:19:37.524744 edge_orm-0.5.3/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.5.3/edge_orm/unset.py
--rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.5.3/edge_orm/validators.py
--rw-r--r--   0        0        0      785 2023-04-11 22:19:36.080338 edge_orm-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.5.3/setup.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.6.1/README.md
+-rw-r--r--   0        0        0      774 2023-02-27 21:50:15.475075 edge_orm-0.6.1/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.6.1/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.6.1/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.6.1/edge_orm/execute.py
+-rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.6.1/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.6.1/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.6.1/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.6.1/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.6.1/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.6.1/edge_orm/node/models.py
+-rw-r--r--   0        0        0      259 2023-02-27 21:41:14.553137 edge_orm-0.6.1/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.6.1/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.6.1/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.6.1/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    40202 2023-04-13 18:54:49.007376 edge_orm-0.6.1/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.6.1/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.6.1/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.6.1/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.6.1/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.6.1/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.6.1/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.6.1/edge_orm/unset.py
+-rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.6.1/edge_orm/validators.py
+-rw-r--r--   0        0        0      785 2023-04-13 18:57:33.160171 edge_orm-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.6.1/setup.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.6.1/PKG-INFO
```

### Comparing `edge_orm-0.5.3/edge_orm/__init__.py` & `edge_orm-0.6.1/edge_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/cache.py` & `edge_orm-0.6.1/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/execute.py` & `edge_orm-0.6.1/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/external/encoders.py` & `edge_orm-0.6.1/edge_orm/external/encoders.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/helpers.py` & `edge_orm-0.6.1/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/logs.py` & `edge_orm-0.6.1/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/node/models.py` & `edge_orm-0.6.1/edge_orm/node/models.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/resolver/merging.py` & `edge_orm-0.6.1/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/resolver/model.py` & `edge_orm-0.6.1/edge_orm/resolver/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 
         return True
 
     """QUERY METHODS"""
 
     async def query(
         self,
-        client: edgedb.AsyncIOClient | None = None,
+        client: edgedb.AsyncIOClient,
         has_permission_str: str | None = None,
     ) -> T.List[NodeType]:
         has_permission_str = has_permission_str or self.has_permission_str_
         query_str, variables = self.full_query_str_and_vars(
             include_select=True, prefix=""
         )
         if has_permission_str:
@@ -452,15 +452,15 @@
                     models := __models {{ {second_part} }},
                 }}
             """
         with span.span(
             op=f"edgedb.query.{self.model_name}", description=query_str[:200]
         ):
             raw_response = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=query_str,
                 variables=variables,
                 only_one=False if not has_permission_str else True,
             )
 
         if has_permission_str:
             if raw_response["__has_permission"] is False:
@@ -469,79 +469,73 @@
 
         if not isinstance(raw_response, list):
             raise errors.ResolverException(
                 f"Expected a list from query, got {raw_response}."
             )
         return self.parse_obj_with_cache_list(raw_response)
 
-    async def query_first(
-        self, client: edgedb.AsyncIOClient | None = None
-    ) -> NodeType | None:
+    async def query_first(self, client: edgedb.AsyncIOClient) -> NodeType | None:
         if self._limit is not None and self._limit > 1:
             raise errors.ResolverException(
                 f"Limit is set to {self._limit} so you cannot query_first."
             )
         self._limit = 1
         model_lst = await self.query(client=client)
         if not model_lst:
             return None
         return model_lst[0]
 
-    async def count(self, client: edgedb.AsyncIOClient | None = None) -> int:
+    async def count(self, client: edgedb.AsyncIOClient) -> int:
         query_str, variables = self.full_query_str_and_vars(
             include_select=False, prefix=""
         )
 
         query_str = f"SELECT count({self.model_name} {query_str})"
         with span.span(
             op=f"edgedb.query.{self.model_name}", description=query_str[:200]
         ):
             c = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=query_str,
                 variables=variables,
                 only_one=True,
             )
             if not isinstance(c, int):
                 raise errors.ResolverException(f"Count must be an int {c=}.")
             return c
 
     async def _get(
         self,
         field_name: str,
         value: T.Any,
         *,
-        client: edgedb.AsyncIOClient | None = None,
+        client: edgedb.AsyncIOClient,
     ) -> NodeType | None:
         self.validate_field_name_value_filters(
             operation_name="get", field_name=field_name, value=value
         )
         query_str, variables = self.full_query_str_and_vars(
             include_select=True, prefix=""
         )
         custom_filter_str = f"FILTER {self.filter_str_from_field_name(field_name)}"
         query_str += f" {custom_filter_str}"
         with span.span(op=f"edgedb.get.{self.model_name}", description=query_str[:200]):
             raw_response = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=query_str,
                 variables={**variables, field_name: value},
                 only_one=True,
             )
 
         if not raw_response:
             return None
         return self.parse_obj_with_cache(raw_response)
 
     async def _gerror(
-        self,
-        field_name: str,
-        value: T.Any,
-        *,
-        client: edgedb.AsyncIOClient | None = None,
+        self, field_name: str, value: T.Any, *, client: edgedb.AsyncIOClient
     ) -> NodeType:
         model = await self._get(field_name=field_name, value=value, client=client)
         if not model:
             raise errors.ResolverException(
                 f"No {self.model_name} in db with fields {field_name} = {value}."
             )
         return model
@@ -599,15 +593,15 @@
 
         return conflict_str, conflict_variables
 
     async def insert_one(
         self,
         insert: InsertType,
         *,
-        client: edgedb.AsyncIOClient | None = None,
+        client: edgedb.AsyncIOClient,
         upsert_given_conflict_on: str = None,
         custom_conflict_on_str: str = None,
         return_model_for_conflict_on: str = None,
         mutate_on_update: bool = True,
     ) -> NodeType:
         if existing_filter_str := self.has_filters():
             raise errors.ResolverException(
@@ -632,28 +626,28 @@
         insert_s = f"INSERT {self.model_name} {insert_s}"
         if conflict_str:
             insert_s += f" {conflict_str}"
         final_insert_s = f"WITH model := ({insert_s}) {select_s}"
 
         with span.span(op=f"edgedb.add.{self.model_name}"):
             raw_response = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=final_insert_s,
                 variables={
                     **select_variables,
                     **insert_variables,
                     **conflict_variables,
                 },
                 only_one=True,
             )
         raw_response = T.cast(RAW_RESP_ONE, raw_response)
         return self.parse_obj_with_cache(raw_response)
 
     async def insert_many(
-        self, inserts: list[InsertType], *, client: edgedb.AsyncIOClient | None = None
+        self, inserts: list[InsertType], *, client: edgedb.AsyncIOClient
     ) -> list[NodeType]:
         if not inserts:
             return []
         conversion_map = self._node_config.insert_edgedb_conversion_map
         first_insert_s, _ = utils.model_to_set_str_vars(
             model=inserts[0], conversion_map=conversion_map, json_get_item="item"
         )
@@ -687,15 +681,15 @@
         variables = {
             **select_variables,
             "__data": json.dumps(encoders.jsonable_encoder(insert_vars_list)),
         }
         # debug(variables)
         with span.span(op=f"edgedb.add_many.{self.model_name}"):
             raw_response = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=final_insert_str,
                 variables=variables,
                 only_one=False,
             )
         raw_response = T.cast(RAW_RESP_MANY, raw_response)
         return self.parse_obj_with_cache_list(raw_response)
 
@@ -718,15 +712,15 @@
         self,
         patch: PatchType,
         *,
         field_name: str = None,
         value: T.Any = None,
         only_one: bool,
         mutate_on_update: bool,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
         include_changes: bool,
         include_permissions: bool,
     ) -> RAW_RESPONSE:
         update_s, update_variables = utils.model_to_set_str_vars(
             model=patch,
             conversion_map=self._node_config.patch_edgedb_conversion_map,
             additional_link_str=self.build_mutate_on_update_str(
@@ -770,15 +764,15 @@
             }}
             """
         else:
             update_s = f"UPDATE {self.model_name} {filters_s} SET {update_s}"
             final_update_s = f"WITH model := ({update_s}) {select_s}"
         with span.span(op=f"edgedb.update.{self.model_name}"):
             raw_response = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=final_update_s,
                 variables={**select_variables, **filters_vars, **update_variables},
                 only_one=only_one,
             )
         raw_response = T.cast(RAW_RESPONSE, raw_response)
         return raw_response
 
@@ -798,15 +792,15 @@
 
     async def _update_one(
         self,
         patch: PatchType,
         *,
         field_name: str,
         value: T.Any,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
         mutate_on_update: bool = True,
     ) -> NodeType:
         if not patch.set_fields_:
             raise errors.ResolverException("Patch is empty.")
         self.validate_field_name_value_filters(
             operation_name="update_one", field_name=field_name, value=value
         )
@@ -829,15 +823,15 @@
 
     async def _update_one_with_changes(
         self,
         patch: PatchType,
         *,
         field_name: str,
         value: T.Any,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
         mutate_on_update: bool = True,
     ) -> tuple[NodeType, CHANGES]:
         if not patch.set_fields_:
             raise errors.ResolverException("Patch is empty.")
         self.validate_field_name_value_filters(
             operation_name="update_one", field_name=field_name, value=value
         )
@@ -864,15 +858,15 @@
         return n, changes
 
     async def update_many(
         self,
         patch: PatchType,
         *,
         update_all: bool = False,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
         mutate_on_update: bool = True,
     ) -> list[NodeType]:
         # TODO make update_many_with_changes at some point, would not be hard
         if not patch.set_fields_:
             raise errors.ResolverException("Patch is empty.")
         if not update_all:
             if not self.has_filters():
@@ -893,15 +887,15 @@
 
     async def _delete(
         self,
         *,
         field_name: str = None,
         value: T.Any = None,
         only_one: bool,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
         include_permissions: bool,
     ) -> RAW_RESPONSE:
         filters_s, filters_vars = self.build_filters_str_and_vars(prefix="")
 
         if only_one:
             if field_name is None:
                 raise errors.ResolverException(
@@ -930,28 +924,28 @@
             }}
             """
         else:
             delete_s = f"DELETE {self.model_name} {filters_s}"
             final_delete_s = f"WITH model := ({delete_s}) {select_s}"
         with span.span(op=f"edgedb.delete.{self.model_name}"):
             raw_response = await execute.query(
-                client=client or self._node_config.client,
+                client=client,
                 query_str=final_delete_s,
                 variables={**select_variables, **filters_vars},
                 only_one=only_one,
             )
         raw_response = T.cast(RAW_RESPONSE, raw_response)
         return raw_response
 
     async def _delete_one(
         self,
         *,
         field_name: str,
         value: T.Any,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
     ) -> NodeType:
         self.validate_field_name_value_filters(
             operation_name="delete one", field_name=field_name, value=value
         )
         raw_response = await self._delete(
             field_name=field_name,
             value=value,
@@ -966,15 +960,15 @@
             raise errors.ObjectNotFound("Object not found.")
         return self.parse_obj_with_cache(raw_response["after"])
 
     async def delete_many(
         self,
         *,
         delete_all: bool = False,
-        client: edgedb.AsyncIOClient | None,
+        client: edgedb.AsyncIOClient,
     ) -> list[NodeType]:
         if not delete_all:
             if not self.has_filters():
                 raise errors.ResolverException(
                     "You did not give filters which means this will delete *all* models. "
                     "If this is your intention, pass delete_all=True."
                 )
```

### Comparing `edge_orm-0.5.3/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.6.1/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/resolver/utils.py` & `edge_orm-0.6.1/edge_orm/resolver/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     *,
     model: Insert | Patch,
     conversion_map: CONVERSION_MAP,
     json_get_item: str = None,
     additional_link_str: str | None = None,
 ) -> tuple[str, "VARS"]:
     """takes in a model dictionary and returns a string that represents a mutation with this dictionary
-    eg: {"name": "Jeremy Berman", "age": UNSET, "last_updated": 2022...} -> { name := <str>$name, age := <int>{}, ...}"""
+    eg: {"name": "Jeremy Berman", "age": UNSET, "last_updated": 2022...} -> { name := <str>$name, age := <int>{}, ...}
+    """
     str_lst: list[str] = []
     variables: VARS = {}
     for field_name in model.set_fields_:
         original_val = getattr(model, field_name)
         if field_name not in conversion_map:
             # this is a resolver
             rez_s, rez_vars = line_var_from_resolver(
```

### Comparing `edge_orm-0.5.3/edge_orm/span.py` & `edge_orm-0.6.1/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/types_generator/introspection.py` & `edge_orm-0.6.1/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/types_generator/main.py` & `edge_orm-0.6.1/edge_orm/types_generator/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,35 +223,35 @@
     raise ResolverException(
         f"Must only give one argument, received {{kwargs}}."
     )
 field_name, value = list(kwargs.items())[0]
 """.strip()
 
     get_str = f"""
-async def get(self, *, client: AsyncIOClient | None, {params_fields_str}) -> {node_name} | None:
+async def get(self, *, client: AsyncIOClient, {params_fields_str}) -> {node_name} | None:
 {indent_lines(validation_str)}
     return await self._get(field_name=field_name, value=value, client=client)
     """
     gerror_str = f"""
-async def gerror(self, *, client: AsyncIOClient | None, {params_fields_str}) -> {node_name}:
+async def gerror(self, *, client: AsyncIOClient, {params_fields_str}) -> {node_name}:
 {indent_lines(validation_str)}
     return await self._gerror(field_name=field_name, value=value, client=client)
     """
     update_one_str = f"""
-async def update_one(self, patch: {node_name}Patch, *, client: AsyncIOClient | None, {params_fields_str}) -> {node_name}:
+async def update_one(self, patch: {node_name}Patch, *, client: AsyncIOClient, {params_fields_str}) -> {node_name}:
 {indent_lines(validation_str)}
     return await self._update_one(patch=patch, field_name=field_name, value=value, client=client)
     """
     update_one_with_changes_str = f"""
-async def update_one_with_changes(self, patch: {node_name}Patch, *, client: AsyncIOClient | None, {params_fields_str}) -> tuple[{node_name}, CHANGES]:
+async def update_one_with_changes(self, patch: {node_name}Patch, *, client: AsyncIOClient, {params_fields_str}) -> tuple[{node_name}, CHANGES]:
 {indent_lines(validation_str)}
     return await self._update_one_with_changes(patch=patch, field_name=field_name, value=value, client=client)
     """
     delete_one_str = f"""
-async def delete_one(self, *, client: AsyncIOClient | None, {params_fields_str}) -> {node_name}:
+async def delete_one(self, *, client: AsyncIOClient, {params_fields_str}) -> {node_name}:
 {indent_lines(validation_str)}
     return await self._delete_one(field_name=field_name, value=value, client=client)
     """
     return f"{get_str}\n{gerror_str}\n{update_one_str}\n{update_one_with_changes_str}\n{delete_one_str}\n"
 
 
 def build_include_fields_function(
@@ -691,19 +691,21 @@
             build_resolver_link_function_str(
                 node_resolver_name=node_resolver_name, link=link
             )
         )
         # for insert
         if not link.is_computed and not link.not_insertable:
             insert_resolver_str = f"{link.target.model_name}Resolver"
+            default_value_str = ""
             if (not link.required) or (link.required and link.default):
-                insert_resolver_str = f"T.Optional[{insert_resolver_str}]"
-            default_value_str = (
-                " = None" if insert_resolver_str.startswith("T.Optional[") else ""
-            )
+                insert_resolver_str = (
+                    f"T.Union[T.Optional[{insert_resolver_str}], None, UnsetType]"
+                )
+                default_value_str = " = Field(UNSET)"
+
             insert_property_strs.append(
                 f"{link.name}: {insert_resolver_str}{default_value_str}"
             )
         # for update
         if not link.is_computed and not link.readonly:
             patch_resolver_str = f"{link.target.model_name}Resolver"
             if (not link.required) or (link.required and link.default):
```

### Comparing `edge_orm-0.5.3/edge_orm/unset.py` & `edge_orm-0.6.1/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/edge_orm/validators.py` & `edge_orm-0.6.1/edge_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.3/pyproject.toml` & `edge_orm-0.6.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.5.3"
+version = "0.6.1"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `edge_orm-0.5.3/setup.py` & `edge_orm-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'pydantic[email]>=1.10,<2.0']
 
 extras_require = \
 {'docs': ['mkdocs-material>=8.5.7,<9.0.0']}
 
 setup_kwargs = {
     'name': 'edge-orm',
-    'version': '0.5.3',
+    'version': '0.6.1',
     'description': '',
     'long_description': '# edge orm',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `edge_orm-0.5.3/PKG-INFO` & `edge_orm-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.5.3
+Version: 0.6.1
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
```

