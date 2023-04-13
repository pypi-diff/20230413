# Comparing `tmp/momento-1.0.2.tar.gz` & `tmp/momento-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.0.2.tar", max compression
+gzip compressed data, was "momento-1.1.0.tar", max compression
```

## Comparing `momento-1.0.2.tar` & `momento-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    11357 2023-03-21 20:56:52.432873 momento-1.0.2/LICENSE
--rw-r--r--   0        0        0     5668 2023-03-21 20:56:52.432873 momento-1.0.2/README.md
--rw-r--r--   0        0        0     3692 2023-03-21 20:57:12.578108 momento-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      619 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2786 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     1264 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    30363 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/cache_client.py
--rw-r--r--   0        0        0    30860 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-03-21 20:56:52.432873 momento-1.0.2/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      360 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     3656 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1775 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5635 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    34156 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3163 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1748 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5553 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    33860 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2393 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/py.typed
--rw-r--r--   0        0        0      107 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0     5669 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0     2311 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1370 2023-03-21 20:56:52.436874 momento-1.0.2/src/momento/typing.py
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 momento-1.0.2/setup.py
--rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 momento-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 17:12:53.423168 momento-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5668 2023-04-13 17:12:53.423168 momento-1.1.0/README.md
+-rw-r--r--   0        0        0     3692 2023-04-13 17:13:12.383276 momento-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    30363 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/cache_client.py
+-rw-r--r--   0        0        0    30860 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      360 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     3656 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1775 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5635 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    34156 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3163 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1748 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5553 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    33860 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2393 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/py.typed
+-rw-r--r--   0        0        0      107 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0     5669 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0     2311 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-04-13 17:12:53.427168 momento-1.1.0/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-04-13 17:12:53.431168 momento-1.1.0/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-04-13 17:12:53.431168 momento-1.1.0/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-04-13 17:12:53.431168 momento-1.1.0/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-04-13 17:12:53.431168 momento-1.1.0/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-04-13 17:12:53.431168 momento-1.1.0/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1370 2023-04-13 17:12:53.431168 momento-1.1.0/src/momento/typing.py
+-rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 momento-1.1.0/setup.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 momento-1.1.0/PKG-INFO
```

### Comparing `momento-1.0.2/LICENSE` & `momento-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/README.md` & `momento-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/pyproject.toml` & `momento-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.0.2"
+version = "1.1.0"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
```

### Comparing `momento-1.0.2/src/momento/__init__.py` & `momento-1.1.0/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/auth/credential_provider.py` & `momento-1.1.0/src/momento/auth/credential_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,17 +56,18 @@
             Defaults to None.
             cache_endpoint (Optional[str], optional): Optionally overrides the default control endpoint.
             Defaults to None.
 
         Returns:
             CredentialProvider
         """
-        endpoints = momento_endpoint_resolver.resolve(auth_token)
-        control_endpoint = control_endpoint or endpoints.control_endpoint
-        cache_endpoint = cache_endpoint or endpoints.cache_endpoint
+        token_and_endpoints = momento_endpoint_resolver.resolve(auth_token)
+        control_endpoint = control_endpoint or token_and_endpoints.control_endpoint
+        cache_endpoint = cache_endpoint or token_and_endpoints.cache_endpoint
+        auth_token = token_and_endpoints.auth_token
         return CredentialProvider(auth_token, control_endpoint, cache_endpoint)
 
     def __repr__(self) -> str:
         attributes: Dict[str, str] = copy.copy(vars(self))  # type: ignore[misc]
         attributes["auth_token"] = self._obscure(attributes["auth_token"])
         message = ", ".join(f"{k}={v!r}" for k, v in attributes.items())
         return f"{self.__class__.__name__}({message})"
```

### Comparing `momento-1.0.2/src/momento/cache_client.py` & `momento-1.1.0/src/momento/cache_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/cache_client_async.py` & `momento-1.1.0/src/momento/cache_client_async.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/config/configuration.py` & `momento-1.1.0/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/config/configurations.py` & `momento-1.1.0/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/config/transport/transport_strategy.py` & `momento-1.1.0/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/errors/__init__.py` & `momento-1.1.0/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/errors/error_converter.py` & `momento-1.1.0/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/errors/error_details.py` & `momento-1.1.0/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/errors/exceptions.py` & `momento-1.1.0/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/_utilities/_data_validation.py` & `momento-1.1.0/src/momento/internal/_utilities/_data_validation.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.1.0/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.1.0/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/aio/_scs_control_client.py` & `momento-1.1.0/src/momento/internal/aio/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/aio/_scs_data_client.py` & `momento-1.1.0/src/momento/internal/aio/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.1.0/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.1.0/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.1.0/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.1.0/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.1.0/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.1.0/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/logs.py` & `momento-1.1.0/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/requests/collection_ttl.py` & `momento-1.1.0/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/__init__.py` & `momento-1.1.0/src/momento/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/control/cache/create.py` & `momento-1.1.0/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/control/cache/delete.py` & `momento-1.1.0/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/control/cache/list.py` & `momento-1.1.0/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/control/signing_key/create.py` & `momento-1.1.0/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/control/signing_key/list.py` & `momento-1.1.0/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/control/signing_key/revoke.py` & `momento-1.1.0/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/fetch.py` & `momento-1.1.0/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/get_field.py` & `momento-1.1.0/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.1.0/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/increment.py` & `momento-1.1.0/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.1.0/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.1.0/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/set_field.py` & `momento-1.1.0/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.1.0/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/concatenate_back.py` & `momento-1.1.0/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/concatenate_front.py` & `momento-1.1.0/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/fetch.py` & `momento-1.1.0/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/length.py` & `momento-1.1.0/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/pop_back.py` & `momento-1.1.0/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/pop_front.py` & `momento-1.1.0/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/push_back.py` & `momento-1.1.0/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/push_front.py` & `momento-1.1.0/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/list/remove_value.py` & `momento-1.1.0/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/scalar/delete.py` & `momento-1.1.0/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/scalar/get.py` & `momento-1.1.0/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/scalar/increment.py` & `momento-1.1.0/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/scalar/set.py` & `momento-1.1.0/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.1.0/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/set/add_element.py` & `momento-1.1.0/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/set/add_elements.py` & `momento-1.1.0/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/set/fetch.py` & `momento-1.1.0/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/set/remove_element.py` & `momento-1.1.0/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/data/set/remove_elements.py` & `momento-1.1.0/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/mixins.py` & `momento-1.1.0/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/responses/response.py` & `momento-1.1.0/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/retry/default_eligibility_strategy.py` & `momento-1.1.0/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.1.0/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/src/momento/typing.py` & `momento-1.1.0/src/momento/typing.py`

 * *Files identical despite different names*

### Comparing `momento-1.0.2/setup.py` & `momento-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 install_requires = \
 ['grpcio>=1.50.0,<2.0.0',
  'momento-wire-types>=0.39,<0.40',
  'pyjwt>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.0.2',
+    'version': '1.1.0',
     'description': 'SDK for Momento',
     'long_description': '<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md) \n\n# Momento Python Client Library\n\n\nPython client SDK for Momento Serverless Cache: a fast, simple, pay-as-you-go caching solution without\nany of the operational overhead required by traditional caching solutions!\n\n\n\n## Getting Started :running:\n\n### Requirements\n\n- [Python 3.7](https://www.python.org/downloads/) or above is required\n- A Momento Auth Token is required, you can generate one using the [Momento CLI](https://github.com/momentohq/momento-cli)\n\n### Examples\n\nReady to dive right in? Just check out the [examples](https://github.com/momentohq/client-sdk-python/tree/main/examples) directory for complete, working examples of\nhow to use the SDK.\n\n### Installation\n\nThe [Momento SDK is available on PyPi](https://pypi.org/project/momento/). To install via pip:\n\n```bash\npip install momento\n```\n\n### Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = "default-cache"\n    with CacheClient(\n        configuration=Configurations.Laptop.v1(),\n        credential_provider=CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n        default_ttl=timedelta(seconds=60),\n    ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        match create_cache_response:\n            case CreateCache.CacheAlreadyExists():\n                print(f"Cache with name: {cache_name} already exists.")\n            case CreateCache.Error() as error:\n                raise error.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, "foo", "FOO")\n        match set_response:\n            case CacheSet.Error() as error:\n                raise error.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, "foo")\n        match get_response:\n            case CacheGet.Hit() as hit:\n                print(f"Look up resulted in a hit: {hit}")\n                print(f"Looked up Value: {hit.value_string!r}")\n            case CacheGet.Miss():\n                print("Look up resulted in a: miss. This is unexpected.")\n            case CacheGet.Error() as error:\n                raise error.inner_exception\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = \'default-cache\'\n    with CacheClient(configuration=Configurations.Laptop.v1(),\n                     credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n                     default_ttl=timedelta(seconds=60)\n                     ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        if isinstance(create_cache_response, CreateCache.CacheAlreadyExists):\n            print(f"Cache with name: {cache_name} already exists.")\n        elif isinstance(create_cache_response, CreateCache.Error):\n            raise create_cache_response.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, \'foo\', \'FOO\')\n        if isinstance(set_response, CacheSet.Error):\n            raise set_response.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, \'foo\')\n        if isinstance(get_response, CacheGet.Hit):\n            print(f"Look up resulted in a hit: {get_response.value_string}")\n            print(f"Looked up Value: {get_response.value_string}")\n        elif isinstance(get_response, CacheGet.Miss):\n            print("Look up resulted in a: miss. This is unexpected.")\n        elif isinstance(get_response, CacheGet.Error):\n            raise get_response.inner_exception\n```\n\n### Logging\n\nTo avoid cluttering DEBUG logging with per-method logs the Momento SDK adds a TRACE logging level. This will only happen\nif the TRACE level does not already exist.\n\nTo enable TRACE level logging you can call logging.basicConfig() before making any log statements:\n\n```python\nimport logging\n\nlogging.basicConfig(level=\'TRACE\')\n```\n\n### Error Handling\n\nComing Soon!\n\n### Tuning\n\nComing Soon!\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
```

### Comparing `momento-1.0.2/PKG-INFO` & `momento-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.0.2
+Version: 1.1.0
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<3.12
```

