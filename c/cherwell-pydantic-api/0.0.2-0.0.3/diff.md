# Comparing `tmp/cherwell_pydantic_api-0.0.2.tar.gz` & `tmp/cherwell_pydantic_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherwell_pydantic_api-0.0.2.tar", max compression
+gzip compressed data, was "cherwell_pydantic_api-0.0.3.tar", max compression
```

## Comparing `cherwell_pydantic_api-0.0.2.tar` & `cherwell_pydantic_api-0.0.3.tar`

### file list

```diff
@@ -1,67 +1,66 @@
--rw-r--r--   0        0        0     1116 2023-03-22 07:46:47.868533 cherwell_pydantic_api-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     1319 2023-03-24 16:48:45.840721 cherwell_pydantic_api-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-03-24 10:49:18.447842 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/__init__.py
--rw-r--r--   0        0        0       61 2023-03-21 17:35:37.123101 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/__main__.py
--rw-r--r--   0        0        0        0 2023-03-19 11:38:25.782849 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/__init__.py
--rw-r--r--   0        0        0     3729 2023-03-22 21:12:46.838028 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Approval.py
--rw-r--r--   0        0        0    69093 2023-03-22 21:12:47.276035 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py
--rw-r--r--   0        0        0    17154 2023-03-22 21:12:47.394037 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Core.py
--rw-r--r--   0        0        0     6515 2023-03-22 21:12:47.439037 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Forms.py
--rw-r--r--   0        0        0     7155 2023-03-22 21:12:47.484038 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py
--rw-r--r--   0        0        0     9966 2023-03-22 21:12:47.549039 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py
--rw-r--r--   0        0        0     8838 2023-03-22 21:12:47.608040 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Queues.py
--rw-r--r--   0        0        0    42096 2023-03-22 21:12:47.954046 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Searches.py
--rw-r--r--   0        0        0    25601 2023-03-22 21:12:48.114049 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Security.py
--rw-r--r--   0        0        0     4662 2023-03-22 21:12:48.142049 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Service.py
--rw-r--r--   0        0        0    15417 2023-03-22 21:12:48.314052 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Teams.py
--rw-r--r--   0        0        0    15747 2023-03-22 21:12:48.410054 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Users.py
--rw-r--r--   0        0        0      788 2023-03-22 21:12:48.417054 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/__init__.py
--rw-r--r--   0        0        0     1016 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py
--rw-r--r--   0        0        0    14554 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py
--rw-r--r--   0        0        0     8790 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py
--rw-r--r--   0        0        0     1517 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py
--rw-r--r--   0        0        0     2865 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py
--rw-r--r--   0        0        0     1086 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py
--rw-r--r--   0        0        0     2777 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py
--rw-r--r--   0        0        0    15593 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Searches.py
--rw-r--r--   0        0        0     8542 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Security.py
--rw-r--r--   0        0        0     4787 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py
--rw-r--r--   0        0        0     7824 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py
--rw-r--r--   0        0        0      481 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/__init__.py
--rw-r--r--   0        0        0      106 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/__init__.py
--rw-r--r--   0        0        0      642 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py
--rw-r--r--   0        0        0   774308 2023-03-22 20:34:06.754499 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/__init__.py
--rw-r--r--   0        0        0     8096 2023-03-26 11:47:33.549850 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/api.py
--rw-r--r--   0        0        0        0 2023-03-22 21:08:27.552764 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/__init__.py
--rw-r--r--   0        0        0     2433 2023-03-23 18:10:18.008072 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/model_base.py
--rw-r--r--   0        0        0        0 2023-03-21 10:59:09.605023 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/__init__.py
--rw-r--r--   0        0        0     7707 2023-03-28 10:35:51.744045 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/collector.py
--rw-r--r--   0        0        0     4370 2023-03-23 17:20:21.655392 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/model_generator.py
--rw-r--r--   0        0        0     4824 2023-03-23 10:25:43.144095 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/repo.py
--rw-r--r--   0        0        0     9015 2023-03-28 09:22:12.005006 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/registry.py
--rw-r--r--   0        0        0      501 2023-03-23 13:27:49.336587 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/templates/base.py.j2
--rw-r--r--   0        0        0      949 2023-03-21 16:09:57.127883 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/templates/dot_gitignore
--rw-r--r--   0        0        0     1589 2023-03-23 17:01:30.651109 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/templates/model.py.j2
--rw-r--r--   0        0        0     2816 2023-03-27 15:51:43.057608 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/valid_schema.py
--rw-r--r--   0        0        0     1859 2023-03-22 18:17:35.702277 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/wrapper.py
--rw-r--r--   0        0        0     2759 2023-03-24 17:25:31.371877 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/__init__.py
--rw-r--r--   0        0        0      720 2023-03-24 17:04:55.919724 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/check.py
--rwxr-xr-x   0        0        0     3700 2023-03-24 19:02:21.683110 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/ipython.py
--rw-r--r--   0        0        0      208 2023-03-24 15:05:53.471857 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/utils.py
--rw-r--r--   0        0        0     3775 2023-03-24 15:11:48.600681 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/welcome.py
--rw-r--r--   0        0        0     4839 2023-03-22 16:07:26.244266 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/generated_api_utils.py
--rw-r--r--   0        0        0     4504 2023-03-26 11:50:21.378612 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/instance.py
--rw-r--r--   0        0        0     5392 2023-03-27 13:23:32.152829 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/interactive.py
--rw-r--r--   0        0        0     1013 2023-03-21 13:34:01.763557 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/interfaces.py
--rw-r--r--   0        0        0        0 2023-03-15 17:53:17.042051 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/py.typed
--rw-r--r--   0        0        0     9774 2023-03-15 16:15:32.830474 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/schema/__init__.py
--rw-r--r--   0        0        0     2253 2023-03-15 16:15:32.831474 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/schema/fields.py
--rw-r--r--   0        0        0     3557 2023-03-24 14:12:48.922113 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/settings.py
--rw-r--r--   0        0        0     3916 2023-03-23 18:05:54.954794 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/types.py
--rw-r--r--   0        0        0     1149 2023-03-26 12:00:50.198963 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/utils.py
--rw-r--r--   0        0        0     1348 2023-03-24 12:08:49.757333 cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/validators.py
--rw-r--r--   0        0        0     2132 2023-04-02 07:17:05.215932 cherwell_pydantic_api-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0    14496 2023-03-22 20:34:26.591817 cherwell_pydantic_api-0.0.2/scripts/codegen.py
--rw-r--r--   0        0        0      513 2023-03-19 11:38:54.064313 cherwell_pydantic_api-0.0.2/scripts/codegen_templates/Enum.jinja2
--rw-r--r--   0        0        0     1789 2023-03-22 20:33:52.685272 cherwell_pydantic_api-0.0.2/scripts/codegen_templates/pydantic/BaseModel.jinja2
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 cherwell_pydantic_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-03-22 07:46:47.868533 cherwell_pydantic_api-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1319 2023-03-24 16:48:45.840721 cherwell_pydantic_api-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-24 10:49:18.447842 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-21 17:35:37.123101 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-19 11:38:25.782849 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/__init__.py
+-rw-r--r--   0        0        0     3729 2023-03-22 21:12:46.838028 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Approval.py
+-rw-r--r--   0        0        0    69093 2023-03-22 21:12:47.276035 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py
+-rw-r--r--   0        0        0    17154 2023-03-22 21:12:47.394037 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Core.py
+-rw-r--r--   0        0        0     6515 2023-03-22 21:12:47.439037 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Forms.py
+-rw-r--r--   0        0        0     7155 2023-03-22 21:12:47.484038 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py
+-rw-r--r--   0        0        0     9966 2023-03-22 21:12:47.549039 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py
+-rw-r--r--   0        0        0     8838 2023-03-22 21:12:47.608040 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Queues.py
+-rw-r--r--   0        0        0    42096 2023-03-22 21:12:47.954046 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Searches.py
+-rw-r--r--   0        0        0    25601 2023-03-22 21:12:48.114049 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Security.py
+-rw-r--r--   0        0        0     4662 2023-03-22 21:12:48.142049 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Service.py
+-rw-r--r--   0        0        0    15417 2023-03-22 21:12:48.314052 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Teams.py
+-rw-r--r--   0        0        0    15747 2023-03-22 21:12:48.410054 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Users.py
+-rw-r--r--   0        0        0      788 2023-03-22 21:12:48.417054 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     1016 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py
+-rw-r--r--   0        0        0    14554 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py
+-rw-r--r--   0        0        0     8790 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py
+-rw-r--r--   0        0        0     1517 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py
+-rw-r--r--   0        0        0     2865 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py
+-rw-r--r--   0        0        0     1086 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py
+-rw-r--r--   0        0        0     2777 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py
+-rw-r--r--   0        0        0    15593 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Searches.py
+-rw-r--r--   0        0        0     8542 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Security.py
+-rw-r--r--   0        0        0     4787 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py
+-rw-r--r--   0        0        0     7824 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py
+-rw-r--r--   0        0        0      481 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/__init__.py
+-rw-r--r--   0        0        0      106 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/__init__.py
+-rw-r--r--   0        0        0      642 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py
+-rw-r--r--   0        0        0   774308 2023-03-22 20:34:06.754499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/__init__.py
+-rw-r--r--   0        0        0     8096 2023-03-26 11:47:33.549850 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/api.py
+-rw-r--r--   0        0        0        0 2023-03-22 21:08:27.552764 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/__init__.py
+-rw-r--r--   0        0        0     2433 2023-03-23 18:10:18.008072 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/model_base.py
+-rw-r--r--   0        0        0        0 2023-03-21 10:59:09.605023 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/__init__.py
+-rw-r--r--   0        0        0     8693 2023-04-13 18:11:05.072587 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/collector.py
+-rw-r--r--   0        0        0     4504 2023-04-13 18:11:19.745824 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/model_generator.py
+-rw-r--r--   0        0        0     7132 2023-04-13 18:11:31.563014 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/repo.py
+-rw-r--r--   0        0        0     9015 2023-03-28 09:22:12.005006 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/registry.py
+-rw-r--r--   0        0        0      504 2023-04-13 17:50:00.815498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/base.py.j2
+-rw-r--r--   0        0        0      949 2023-03-21 16:09:57.127883 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/dot_gitignore
+-rw-r--r--   0        0        0     1618 2023-04-13 15:40:06.593367 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/model.py.j2
+-rw-r--r--   0        0        0     2507 2023-04-13 17:21:15.916322 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/valid_schema.py
+-rw-r--r--   0        0        0     1859 2023-03-22 18:17:35.702277 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/wrapper.py
+-rw-r--r--   0        0        0     3514 2023-04-13 20:28:04.639752 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/__init__.py
+-rw-r--r--   0        0        0      720 2023-03-24 17:04:55.919724 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/check.py
+-rwxr-xr-x   0        0        0     3700 2023-03-24 19:02:21.683110 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/ipython.py
+-rw-r--r--   0        0        0     2262 2023-04-13 18:10:09.585693 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/repo.py
+-rw-r--r--   0        0        0      530 2023-04-13 17:00:06.941981 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/utils.py
+-rw-r--r--   0        0        0     3775 2023-04-13 17:10:51.016290 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/welcome.py
+-rw-r--r--   0        0        0    15776 2023-04-13 20:36:03.816552 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/examples/GettingStarted.ipynb
+-rw-r--r--   0        0        0     4839 2023-04-11 17:44:23.221370 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/generated_api_utils.py
+-rw-r--r--   0        0        0     4504 2023-03-26 11:50:21.378612 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/instance.py
+-rw-r--r--   0        0        0     5392 2023-03-27 13:23:32.152829 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interactive.py
+-rw-r--r--   0        0        0     1013 2023-03-21 13:34:01.763557 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interfaces.py
+-rw-r--r--   0        0        0        0 2023-03-15 17:53:17.042051 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/py.typed
+-rw-r--r--   0        0        0     9766 2023-04-11 17:44:47.629821 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/__init__.py
+-rw-r--r--   0        0        0     2253 2023-03-15 16:15:32.831474 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/fields.py
+-rw-r--r--   0        0        0     3557 2023-03-24 14:12:48.922113 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/settings.py
+-rw-r--r--   0        0        0     3916 2023-03-23 18:05:54.954794 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/types.py
+-rw-r--r--   0        0        0     1149 2023-03-26 12:00:50.198963 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/utils.py
+-rw-r--r--   0        0        0     1348 2023-03-24 12:08:49.757333 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/validators.py
+-rw-r--r--   0        0        0     2356 2023-04-13 18:42:00.570801 cherwell_pydantic_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 cherwell_pydantic_api-0.0.3/PKG-INFO
```

### Comparing `cherwell_pydantic_api-0.0.2/LICENSE.md` & `cherwell_pydantic_api-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/README.md` & `cherwell_pydantic_api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Approval.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Approval.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Core.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Core.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Forms.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Forms.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Queues.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Queues.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Searches.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Searches.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Security.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Security.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Service.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Service.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Teams.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Teams.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/Users.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Users.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/endpoints/__init__.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Searches.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Searches.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Security.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Security.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/_generated/api/models/__init__.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/api.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/api.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/model_base.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/model_base.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/collector.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/collector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from functools import cached_property
 from typing import Optional, Pattern, Union, cast
 
 from async_lru import alru_cache
+from pydantic import BaseModel
 
 from cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject import (
     SchemaResponse,
     Summary,
 )
 from cherwell_pydantic_api.bo.modelgen.model_generator import PydanticModelGenerator
 from cherwell_pydantic_api.bo.modelgen.repo import FileGenerator, ModelRepo
@@ -78,18 +79,22 @@
                 'bo_type': self.bo_type,
                 'num_fields': len(self.schema.fieldDefinitions) if (self.schema and self.schema.fieldDefinitions) else None,
                 'displayName': self.summary.displayName,
                 'lookup': self.summary.lookup,
                 'major': self.summary.major,
                 'supporting': self.summary.supporting,
                 'parent_name': self.parent_item.name if self.parent_item else None,
-                '__self': self,
                 }
 
 
+class CollectorSettings(BaseModel):
+    bo_include_filter: Optional[Pattern]
+    bo_exclude_filter: Optional[Pattern]
+
+
 class Collector:
     "Collects Business Object summaries and schemas from a Cherwell instance, in order to filter them and generate models."
 
     def __init__(self, instance: Instance, *, bo_include_filter: FilterType = None, bo_exclude_filter: FilterType = None, verbose: bool = False):
         self._instance = instance
         self._bo_include_filter = compile_filter(bo_include_filter)
         self._bo_exclude_filter = compile_filter(bo_exclude_filter)
@@ -188,23 +193,41 @@
 
 
     def generate_models(self) -> FileGenerator:
         yield ('__init__.py', '### autogenerated by cherwell_pydantic_api ###\n')
         model_generator = PydanticModelGenerator(self._instance.settings)
         yield ('__base.py', model_generator.generate_base())
         for item in self.items:
+            if not item.verdict:
+                continue
             schema = self._instance.bo.get_schema(item.busobid)
             yield (f"{schema.identifier}.py", model_generator.generate_model(schema))
 
 
     def save_models(self, repo: ModelRepo):
         return repo.save(instance=self._instance, file_type='model', file_generator=self.generate_models())
 
 
+    def generate_settings(self) -> FileGenerator:
+        collector_settings = CollectorSettings(
+            bo_include_filter=self.bo_include_filter, bo_exclude_filter=self.bo_exclude_filter)
+        yield ('collector_settings.json', collector_settings.json(indent=2, sort_keys=True))
+
+
+    def save_settings(self, repo: ModelRepo):
+        return repo.save(instance=self._instance, file_type='registry', file_generator=self.generate_settings())
+
+
+    def load_settings(self, repo: ModelRepo):
+        collector_settings = CollectorSettings.parse_file(
+            repo._repo_dir / self._instance.settings.get_repo_subpackage() / 'registry/collector_settings.json')
+        self.bo_include_filter = collector_settings.bo_include_filter
+        self.bo_exclude_filter = collector_settings.bo_exclude_filter
+
+
     def clear_caches(self):
         self.get_bo_summaries.cache_clear()
         self.get_bo_schema.cache_clear()
 
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._instance}, bo_include_filter={self._bo_include_filter}, bo_exclude_filter={self._bo_exclude_filter})"
-
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/model_generator.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/model_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from collections import defaultdict
 from typing import Any, Optional, cast
 
 import black
 from jinja2 import Environment, PackageLoader, select_autoescape
 
 from cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject import FieldDefinition
@@ -56,15 +55,16 @@
                 self.python_type_validator = 'validator_int'
             else:
                 self.python_type = 'decimal.Decimal'
                 self.python_type_validator = 'validator_decimal'
                 self.python_type_modules.add('decimal')
                 self.pydantic_field_args['decimal_places'] = self.decimalDigits
                 if self.wholeDigits:
-                    self.pydantic_field_args['max_digits'] = self.wholeDigits + cast(int, self.decimalDigits)
+                    self.pydantic_field_args['max_digits'] = self.wholeDigits + \
+                        cast(int, self.decimalDigits)
         elif self.type == 'Logical':
             self.python_type = 'bool'
         else:
             raise ValueError(
                 f"Unknown type: {self.type} for field {self.name}")
         if not self.required:
             self.python_type = f"Optional[{self.python_type}]"
@@ -72,19 +72,21 @@
 
 
 class PydanticModelGenerator:
     def __init__(self, instance_settings: InstanceSettingsBase):
         self._instance_settings = instance_settings
         self._jinja_env = Environment(loader=PackageLoader('cherwell_pydantic_api.bo', 'templates'),
                                       autoescape=select_autoescape(['py']), trim_blocks=True, lstrip_blocks=True)
+        self._jinja_env.filters['repr'] = repr
 
     def generate_base(self) -> str:
         template = self._jinja_env.get_template('base.py.j2')
         base_str = template.render(settings=self._instance_settings)
-        base_str = black.format_str(base_str, mode=black.FileMode(preview=True))
+        base_str = black.format_str(
+            base_str, mode=black.FileMode(preview=True))
         return base_str
 
     def generate_model(self, schema: ValidSchema) -> str:
         template = self._jinja_env.get_template('model.py.j2')
         fields = [ParsedFieldDefinition(**field.dict())
                   for field in schema.fieldDefinitions]
         modules = set()
@@ -92,10 +94,12 @@
         for field in fields:
             field.resolve_type()
             if field.python_type_modules:
                 modules.update(field.python_type_modules)
             if field.python_type_validator:
                 validators[field.python_type_validator].append(field)
             assert field.fieldid_parts['BO'] == schema.busObId
-        model_str = template.render(schema=schema, fields=fields, modules=modules, validators=validators, settings=self._instance_settings)
-        model_str = black.format_str(model_str, mode=black.FileMode(preview=True))
+        model_str = template.render(schema=schema, fields=fields, modules=modules,
+                                    validators=validators, settings=self._instance_settings)
+        model_str = black.format_str(
+            model_str, mode=black.FileMode(preview=True))
         return model_str
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/modelgen/repo.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/repo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Iterable, Literal, Optional
+from typing import Any, Iterable, Literal, Optional, Union
 
 from dulwich import porcelain
 from dulwich.errors import NotGitRepository
 from dulwich.repo import Repo
 
 from cherwell_pydantic_api.instance import Instance
 from cherwell_pydantic_api.settings import Settings
@@ -15,22 +15,27 @@
 
 
 FileTypeLiteral = Literal['registry', 'model']
 FileGenerator = Iterable[tuple[str, str]]
 
 
 class ModelRepo:
-    def __init__(self, create: bool = False):
+    _repo: Repo
+
+    def __init__(self, *, create: bool = False, permit_missing: bool = False):
         is_new = False
         self._repo_dir = Settings().repo_dir.absolute()
         if not self._repo_dir.exists():
             if create:
                 self._repo_dir.mkdir(parents=True)
+            elif permit_missing:
+                self._repo = None  # type: ignore
+                return
             else:
-                raise ValueError(
+                raise FileNotFoundError(
                     f'Repo directory {self._repo_dir} does not exist')
         try:
             self._repo = Repo(root=str(self._repo_dir))
         except NotGitRepository:
             if create:
                 self._repo = Repo.init(path=str(self._repo_dir))
                 is_new = True
@@ -71,45 +76,97 @@
 
 
     def save(self, *,
              instance_name: Optional[str] = None,
              instance: Optional[Instance] = None,
              file_type: FileTypeLiteral = 'registry',
              file_generator: FileGenerator,
-             commit: bool = True):
+             commit: bool = True) -> Optional[bytes]:
         instance, instance_dir = self.prepare_save(
             instance_name=instance_name, instance=instance)
         file_type_dir = instance_dir / file_type
         if not file_type_dir.exists():
             logging.info(
                 f'Creating {file_type} directory {file_type_dir} for instance {instance_name}')
             file_type_dir.mkdir()
         for filename, content in file_generator:
             filepath = file_type_dir / filename
             logging.info(f'Writing file {filepath}')
             filepath.write_text(content)
             self._repo.stage(str(filepath.relative_to(self._repo_dir)))
         if commit:
-            self.commit(instance=instance, file_type=file_type)
+            return self.commit(instance=instance, file_type=file_type)
+        return None
 
 
     def commit(self, *, instance: Instance, file_type: FileTypeLiteral) -> Optional[bytes]:
         # Check if there are any changes to commit (because dulwich allows empty commits)
+        encoding = self._repo.get_config().encoding
         repo_status = porcelain.status(self._repo)  # type: ignore
         if not repo_status.staged['add'] and not repo_status.staged['delete'] and not repo_status.staged['modify']:
             logging.info(
                 f'No {file_type} changes to commit for instance {instance.settings.name}')
             return None
         commit = f'cherwell_pydantic_api: update {file_type} for instance {instance.settings.name}'
         author = Settings().repo_author
         branch = instance.settings.get_repo_branch()
+        if branch.encode(encoding) not in porcelain.branch_list(self._repo):
+            porcelain.branch_create(self._repo, branch.encode(encoding))
         ref = f'refs/heads/{branch}'
         porcelain.update_head(self._repo, ref)  # this is like git checkout
         logging.info(
             f'Committing {file_type} to {branch} for instance {instance.settings.name}')
         return self._repo.do_commit(message=commit.encode(),
                                     author=author.encode(), ref=ref.encode())
 
 
-    def save_all(self):
+    def save_instance(self, instance: Instance) -> Optional[bytes]:
+        return self.save(instance=instance, file_generator=instance.bo.marshal())
+
+
+    def save_all(self) -> dict[str, Optional[bytes]]:
+        r = {}
         for instance in Instance._instances.values():
-            self.save(instance=instance, file_generator=instance.bo.marshal())
+            r[instance.settings.name] = self.save_instance(instance)
+        return r
+
+
+    def get_info(self, *,
+                 instance_name: Optional[str] = None,
+                 instance: Optional[Instance] = None) -> dict[str, Union[str, bool, dict[str, Union[str, bool]]]]:
+        # resolve arguments
+        if instance is None:
+            if instance_name is None:
+                raise ValueError(
+                    'Either instance_name or instance must be given')
+            instance = Instance._instances[instance_name]
+        else:
+            instance_name = instance.settings.name
+        instance_dir = self._repo_dir / instance.settings.get_repo_subpackage()
+        r = {'instance': {
+            'name': instance.settings.name,
+            'repo_subpackage': str(instance.settings.get_repo_subpackage()),
+            'repo_branch': instance.settings.get_repo_branch()
+        },
+            'repo': {
+                'path': self._repo.path if self._repo else None,
+                'settings_path': str(self._repo_dir),
+                'instance_path': str(instance_dir),
+                'instance_path_exists': instance_dir.exists(),
+                'author': Settings().repo_author,
+        },
+        }
+        if self._repo is not None:
+            repo_status = porcelain.status(self._repo)  # type: ignore
+            r['status'] = {
+                'dirty': repo_status.unstaged or repo_status.untracked or repo_status.staged['add'] or repo_status.staged['delete'] or repo_status.staged['modify']
+            }
+            r['ready'] = True
+        else:
+            r['ready'] = False
+        return r
+
+
+    @property
+    def directory(self) -> str:
+        "The absolute path to the repo directory"
+        return self._repo.path
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/registry.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/registry.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/templates/dot_gitignore` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/dot_gitignore`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/templates/model.py.j2` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/model.py.j2`

 * *Files 16% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 {% for module in modules|sort %}
 import {{ module }}
 {% endfor %}
 
 
 class {{ schema.name }}(BusinessObjectModelInstanceBase):
     class _ModelData:
-        busobid = "{{ schema.busObId }}"
-        statefieldid = "{{ schema.stateFieldId }}"
-        firstrecidfield = "{{ schema.firstRecIdField }}"
-        recidfields = "{{ schema.recIdFields }}"
+        busobid = {{ schema.busObId|repr }}
+        statefieldid = {{ schema.stateFieldId|repr }}
+        firstrecidfield = {{ schema.firstRecIdField|repr }}
+        recidfields = {{ schema.recIdFields|repr }}
         {% if schema.states %}
         states = {{ schema.states.split(',') }}
         {% endif %}
 
     class Config:
-        title = "{{ schema.name }}"
+        title = {{ schema.name|repr }}
         orm_mode = True
 
     {% for field in fields %}
     {{ field.name }}: {{ field.python_type }} = Field(None,
-        {% if field.displayName %}title="{{ field.displayName }}",{% endif %}
-        {% if field.description %}description="""{{ field.description }}""",{% endif %}
-        cw_fi="{{ field.fieldid_parts['FI'] }}",
-        {% if field.category %}cw_category="{{ field.category }}",{% endif %}
-        {% if field.details %}cw_details="{{ field.details }}",{% endif %}
+        {% if field.displayName %}title={{ field.displayName|repr }},{% endif %}
+        {% if field.description %}description={{ field.description|repr }},{% endif %}
+        cw_fi={{ field.fieldid_parts['FI']|repr }},
+        {% if field.category %}cw_category={{ field.category|repr }},{% endif %}
+        {% if field.details %}cw_details={{ field.details|repr }},{% endif %}
         {{ field.pydantic_field_params }})
     {% endfor %}
 
     {% for validator, v_fields in validators.items() %}
     _{{ validator }} = validator(
         {% for field in v_fields %}
-        "{{ field.name }}",
+        {{ field.name|repr }},
         {% endfor %}
         pre=True, allow_reuse=True)(validators.{{ validator }})
     {% endfor %}
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/valid_schema.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/valid_schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,23 +22,14 @@
     identifier: FieldIdentifier
 
     def __init__(self, **data):
         data['short_field_id'] = fieldid_parts(data['fieldId'])['FI']
         data['identifier'] = FieldIdentifier(data['name'])
         super().__init__(**data)
 
-    def to_dict(self) -> dict:
-        "Convert to dictionary e.g. for DataFrame use"
-        return {'name': self.name,
-                'type': self.type,
-                'short_field_id': self.short_field_id,
-                'identifier': self.identifier,
-                '__self': self,
-                }
-
 
 
 class ValidSchema(ApiBaseModel):
     "Corresponds to the type SchemaResponse, but with stricter types and omitting relationship details"
     busObId: BusObID
     fieldDefinitions: list[ValidFieldDefinition]
     firstRecIdField: Optional[str] = None
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/bo/wrapper.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/wrapper.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/__init__.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,21 +16,25 @@
         "cherwell_pydantic_api is not installed properly as a package. Please check the documentation.")
     sys.stderr.write(f"Error: {e}")
     sys.exit(1)
 try:
     import click
 except ImportError:
     sys.stderr.write("""To use the CLI, click must be installed.
-One way of achieving this is to install cherwell_pydantic_api with the modelgen option.
+One way of achieving this is to install cherwell_pydantic_api with the modelgen or all extra.
 But you can also install click separately.
 
 To fix this, run pip or poetry as follows:
     pip install cherwell_pydantic_api[modelgen]
 or
+    pip install cherwell_pydantic_api[all]
+or
     poetry add -E modelgen cherwell_pydantic_api
+or
+    poetry add -E all cherwell_pydantic_api
 
 """)
     sys.exit(1)
 
 
 def check_envpath(offer_setup=True):
     envpath = Path.cwd().joinpath('cherwell.env')
@@ -40,21 +44,23 @@
         from .welcome import initial_setup
         initial_setup(envpath)
     return envpath
 
 
 def welcome_banner():
     click.echo()
-    lines = ['Welcome to cherwell_pydantic_api!', '', 'For more information, please visit:', '', 'https://github.com/dataway/cherwell_pydantic_api']
+    lines = ['Welcome to cherwell_pydantic_api!', '', 'For more information, please visit:',
+             '', 'https://github.com/dataway/cherwell_pydantic_api']
     width = max([len(line) for line in lines])
     hash = '\u2592'
     style = {'fg': 'white', 'bg': 'blue'}
     click.secho(hash * (width + 6), **style)
     for line in lines:
-        click.secho(f"{hash}  {line}{' ' * (width - len(line))}  {hash}", **style)
+        click.secho(
+            f"{hash}  {line}{' ' * (width - len(line))}  {hash}", **style)
     click.secho(hash * (width + 6), **style)
     click.echo()
 
 
 
 def cli_welcome():
     "Check for existing env file and offer to create one if not found. Return 0 if successful, 1 if aborted."
@@ -67,36 +73,54 @@
 
     try:
         envpath = check_envpath()
     except click.exceptions.Abort:
         click.secho("\nAborted.\n", fg='red')
         return 1
     if settings is None or not settings.suppress_banner:
-        click.secho(f"\nFound existing cherwell.env file at {envpath}\n", fg='green')
+        click.secho(
+            f"\nFound existing cherwell.env file at {envpath}\n", fg='green')
     return 0
 
 
 @click.group()
 def root():
+    "cherwell_pydantic_api CLI"
     pass
 
 
+@root.command(context_settings=dict(ignore_unknown_options=True, allow_extra_args=True))
+@click.pass_context
+def getting_started(ctx):
+    "Launch the Getting Started notebook in JupyterLab"
+    try:
+        import jupyterlab.labapp
+    except:
+        click.secho(
+            "To use the JupyterLab interface, you must install cherwell_pydantic_api[all].\n", fg='red')
+        return
+    import os.path
+    nb = os.path.dirname(__file__) + '/../examples/GettingStarted.ipynb'
+    jupyterlab.labapp.main(ctx.args + [nb])
+
+
 def cli_normal():
     from . import check
     root.add_command(check.check)
     from . import ipython
     root.add_command(ipython.ipython_shell)
+    from . import repo
+    root.add_command(repo.repo_group)
     root()
 
 
 def cli():
     "Main CLI entry point."
-    if len(sys.argv) == 1: # No CLI arguments
+    if len(sys.argv) == 1:  # No CLI arguments
         r = cli_welcome()
         if r != 0:
             return r
     return cli_normal()
 
 
 if __name__ == '__main__':
     cli()
-
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/check.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/check.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/ipython.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/ipython.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/cli/welcome.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/welcome.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/generated_api_utils.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/generated_api_utils.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/instance.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/instance.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/interactive.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interactive.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/interfaces.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interfaces.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/schema/__init__.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
 
 class CherwellSchemaMetaPathFinder(importlib.abc.MetaPathFinder):
     """docstring for CherwellSchemaMetaPathFinder"""
     def __init__(self):
         super(CherwellSchemaMetaPathFinder, self).__init__()
         self.schemas = dict()
-        
+
     @classmethod
     def find_spec(cls, fullname: str, path: Optional[Sequence[str]], target: Optional[types.ModuleType] = ...) -> Optional[object]:
         if fullname.startswith(cls.__module__ + '.'):
             print("fullname: {0}".format(fullname))
             schema = fullname[len(cls.__module__) + 1:]
             if '.' in schema:
                 schema, ob = schema.split('.')
```

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/schema/fields.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/fields.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/settings.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/settings.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/types.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/types.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/utils.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/utils.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/cherwell_pydantic_api/validators.py` & `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/validators.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.2/pyproject.toml` & `cherwell_pydantic_api-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 [tool.poetry]
 name = "cherwell_pydantic_api"
-version = "0.0.2"
+version = "0.0.3"
 description = "A pythonic, asyncio connector for the Cherwell CSM API with full usage of Pydantic types"
 authors = ["Anthony Uk <uk@anthonyuk.dev>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/dataway/cherwell_pydantic_api"
 homepage = "https://github.com/dataway/cherwell_pydantic_api"
-packages = [
-    { include = "cherwell_pydantic_api" },
-    { include = "scripts", format="sdist" }
-]
 
 classifiers = [
     'Development Status :: 1 - Planning',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3 :: Only',
@@ -28,40 +24,41 @@
 ]
 keywords = ["cherwell", "pydantic"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pydantic = {extras = ["dotenv"], version = "^1.10.6"}
-httpx = "^0.23.3"
+httpx = "^0.24.0"
 async-lru = "^2.0.2"
 click = "^8.1.3"
 black = { version = "^23.1.0", optional = true }
 dulwich = { version = "^0.21.3", optional = true }
+jupyter = { version = "^1.0.0", optional = true }
+nest-asyncio = { version = "^1.5.6", optional = true }
+ipywidgets = { version = "^8.0.5", optional = true }
+jupyterlab = { version = "^3.6.2", optional = true }
+ipyaggrid = { version = "^0.4.0", optional = true }
+jinja2 = { version = "^3.1.2", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.11.0"
 dulwich = "^0.21.3"
-
-# Link to my patch until it's merged upstream
 datamodel-code-generator = "^0.17.2"
 black = "^23.1.0"
 pdoc = "^13.0.0"
 rich = "^13.3.2"
-
-[tool.poetry.group.jupyter.dependencies]
-jupyter = "^1.0.0"
-nest-asyncio = "^1.5.6"
-pandas = "^1.5.3"
-ipywidgets = "^8.0.5"
-ipydatagrid = "^1.1.15"
-jupyterlab = "^3.6.2"
+pre-commit = "^3.2.2"
+cherwell_pydantic_api = {path = ".", extras = ["modelgen", "jupyter"]}
+autopep8 = "^2.0.2"
 
 [tool.poetry.extras]
-modelgen = ["black", "dulwich", "click"]
+modelgen = ["black", "dulwich", "click", "jinja2"]
+jupyter = ["jupyter", "ipywidgets", "jupyterlab", "ipyaggrid", "nest-asyncio"]
+all = ["modelgen", "jupyter"]
 
 [tool.poetry.scripts]
 cherwell-pydantic-api-cli = "cherwell_pydantic_api.cli:cli"
 cwcli = "cherwell_pydantic_api.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `cherwell_pydantic_api-0.0.2/PKG-INFO` & `cherwell_pydantic_api-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cherwell-pydantic-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pythonic, asyncio connector for the Cherwell CSM API with full usage of Pydantic types
 Home-page: https://github.com/dataway/cherwell_pydantic_api
 License: MIT
 Keywords: cherwell,pydantic
 Author: Anthony Uk
 Author-email: uk@anthonyuk.dev
 Requires-Python: >=3.9,<4.0
@@ -20,20 +20,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Provides-Extra: all
+Provides-Extra: jupyter
 Provides-Extra: modelgen
 Requires-Dist: async-lru (>=2.0.2,<3.0.0)
 Requires-Dist: black (>=23.1.0,<24.0.0) ; extra == "modelgen"
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "modelgen"
 Requires-Dist: dulwich (>=0.21.3,<0.22.0) ; extra == "modelgen"
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: ipyaggrid (>=0.4.0,<0.5.0) ; extra == "jupyter"
+Requires-Dist: ipywidgets (>=8.0.5,<9.0.0) ; extra == "jupyter"
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "modelgen"
+Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: jupyterlab (>=3.6.2,<4.0.0) ; extra == "jupyter"
+Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0) ; extra == "jupyter"
 Requires-Dist: pydantic[dotenv] (>=1.10.6,<2.0.0)
 Project-URL: Repository, https://github.com/dataway/cherwell_pydantic_api
 Description-Content-Type: text/markdown
 
 # cherwell_pydantic_api
 ## a pythonic, asyncio connector for the Cherwell CSM API with full usage of Pydantic types
```

