# Comparing `tmp/py_assimilator-1.2.2.tar.gz` & `tmp/py_assimilator-1.2.3.tar.gz`

## Comparing `py_assimilator-1.2.2.tar` & `py_assimilator-1.2.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/__init__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/error_wrapper.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/model_utils.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/repository.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/specifications/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/database/specifications/specifications.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/events/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/events/outbox_relay.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/events/database/__init__.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/alchemy/events/database/repository.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/exceptions.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/exceptions.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/models.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/repository.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/specifications/__init__.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/specifications/adaptive.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/specifications/specifications.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/database/specifications/types.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/events/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/events/events.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/events/events_bus.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/events/exceptions.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/events/outbox_relay.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/patterns/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/patterns/context_managers.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/patterns/error_wrapper.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/patterns/lazy_command.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/services/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/services/base.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/core/services/crud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/error_wrapper.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/models_utils.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/repository.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/specifications/__init__.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/specifications/filter_specifications.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/specifications/internal_operator.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/specifications/specifications.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/database/specifications/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/events/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/internal/events/events_bus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/kafka_/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/kafka_/events/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/kafka_/events/events_bus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/__init__.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/error_wrapper.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/models.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/repository.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/specifications/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/mongo/database/specifications/specifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/database/__init__.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/database/models.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/database/repository.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/database/unit_of_work.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/events/__init__.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/assimilator/redis_/events/events_bus.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/LICENSE.md
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/README.md
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 py_assimilator-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/__init__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/error_wrapper.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/model_utils.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/repository.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/specifications/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/specifications/specifications.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/outbox_relay.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/database/__init__.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/database/repository.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/exceptions.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/exceptions.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/models.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/repository.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/__init__.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/adaptive.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/specifications.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/types.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/events.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/events_bus.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/exceptions.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/outbox_relay.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/context_managers.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/error_wrapper.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/lazy_command.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/services/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/services/base.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/services/crud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/error_wrapper.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/models_utils.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/repository.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/__init__.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/filter_specifications.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/internal_operator.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/specifications.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/utils.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/events/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/events/events_bus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/kafka_/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/kafka_/events/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/kafka_/events/events_bus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/__init__.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/error_wrapper.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/models.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/repository.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/specifications/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/specifications/specifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/__init__.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/models.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/repository.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/unit_of_work.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/events/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/events/events_bus.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/LICENSE.md
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/README.md
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/PKG-INFO
```

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/database/error_wrapper.py` & `py_assimilator-1.2.3/assimilator/alchemy/database/error_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/database/model_utils.py` & `py_assimilator-1.2.3/assimilator/alchemy/database/model_utils.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/database/repository.py` & `py_assimilator-1.2.3/assimilator/alchemy/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/database/unit_of_work.py` & `py_assimilator-1.2.3/assimilator/alchemy/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/database/specifications/filtering_options.py` & `py_assimilator-1.2.3/assimilator/alchemy/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/database/specifications/specifications.py` & `py_assimilator-1.2.3/assimilator/alchemy/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/events/outbox_relay.py` & `py_assimilator-1.2.3/assimilator/alchemy/events/outbox_relay.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/alchemy/events/database/repository.py` & `py_assimilator-1.2.3/assimilator/alchemy/events/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/models.py` & `py_assimilator-1.2.3/assimilator/core/database/models.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/repository.py` & `py_assimilator-1.2.3/assimilator/core/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/unit_of_work.py` & `py_assimilator-1.2.3/assimilator/core/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/specifications/adaptive.py` & `py_assimilator-1.2.3/assimilator/core/database/specifications/adaptive.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/specifications/filtering_options.py` & `py_assimilator-1.2.3/assimilator/core/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/specifications/specifications.py` & `py_assimilator-1.2.3/assimilator/core/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/database/specifications/types.py` & `py_assimilator-1.2.3/assimilator/core/database/specifications/types.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/events/events.py` & `py_assimilator-1.2.3/assimilator/core/events/events.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/events/events_bus.py` & `py_assimilator-1.2.3/assimilator/core/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/events/outbox_relay.py` & `py_assimilator-1.2.3/assimilator/core/events/outbox_relay.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/patterns/context_managers.py` & `py_assimilator-1.2.3/assimilator/core/patterns/context_managers.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/patterns/error_wrapper.py` & `py_assimilator-1.2.3/assimilator/core/patterns/error_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/patterns/lazy_command.py` & `py_assimilator-1.2.3/assimilator/core/patterns/lazy_command.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/core/services/crud.py` & `py_assimilator-1.2.3/assimilator/core/services/crud.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/models_utils.py` & `py_assimilator-1.2.3/assimilator/internal/database/models_utils.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/repository.py` & `py_assimilator-1.2.3/assimilator/internal/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/unit_of_work.py` & `py_assimilator-1.2.3/assimilator/internal/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/specifications/filter_specifications.py` & `py_assimilator-1.2.3/assimilator/internal/database/specifications/filter_specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/specifications/filtering_options.py` & `py_assimilator-1.2.3/assimilator/internal/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/specifications/internal_operator.py` & `py_assimilator-1.2.3/assimilator/internal/database/specifications/internal_operator.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/specifications/specifications.py` & `py_assimilator-1.2.3/assimilator/internal/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/database/specifications/utils.py` & `py_assimilator-1.2.3/assimilator/internal/database/specifications/utils.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/internal/events/events_bus.py` & `py_assimilator-1.2.3/assimilator/internal/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/kafka_/events/events_bus.py` & `py_assimilator-1.2.3/assimilator/kafka_/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/mongo/database/error_wrapper.py` & `py_assimilator-1.2.3/assimilator/mongo/database/error_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/mongo/database/models.py` & `py_assimilator-1.2.3/assimilator/mongo/database/models.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/mongo/database/repository.py` & `py_assimilator-1.2.3/assimilator/mongo/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/mongo/database/unit_of_work.py` & `py_assimilator-1.2.3/assimilator/mongo/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/mongo/database/specifications/filtering_options.py` & `py_assimilator-1.2.3/assimilator/mongo/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/mongo/database/specifications/specifications.py` & `py_assimilator-1.2.3/assimilator/mongo/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/redis_/database/models.py` & `py_assimilator-1.2.3/assimilator/redis_/database/models.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/redis_/database/repository.py` & `py_assimilator-1.2.3/assimilator/redis_/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/redis_/database/unit_of_work.py` & `py_assimilator-1.2.3/assimilator/redis_/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/assimilator/redis_/events/events_bus.py` & `py_assimilator-1.2.3/assimilator/redis_/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/.gitignore` & `py_assimilator-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/LICENSE.md` & `py_assimilator-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.2/README.md` & `py_assimilator-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,14 @@
     <img src="https://img.shields.io/github/last-commit/knucklesuganda/py_assimilator?color=%237e56c2&style=for-the-badge" alt="Last commit">
 </a>
 </p>
 
 
 ## Install now
 * `pip install py-assimilator`
-* `pip install py-assimilator[alchemy]` - Optional SQLAlchemy support 
-* `pip install py-assimilator[kafka]` - Optional Kafka support 
-* `pip install py-assimilator[redis]` - Optional Redis support 
-* `pip install py-assimilator[mongo]` - Optional MongoDB support 
-
 
 ## What is that all about?
 
 1. We want to write the best code.
 2. We need the best patterns and techniques for this.
 3. We use PyAssimilator and save lots of time.
 4. We use PyAssimilator and write the best code.
@@ -100,21 +95,36 @@
 ## Sources
 * [Github](https://github.com/knucklesuganda/py_assimilator)
 * [PyPI](https://pypi.org/project/py-assimilator/)
 * [Documentation](https://knucklesuganda.github.io/py_assimilator/)
 * [Github](https://github.com/knucklesuganda/py_assimilator)
 * [Author's YouTube RU](https://www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw)
 * [Author's YouTube ENG](https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA)
+* [Discord channel](https://discord.gg/gTVaGu7DHN)
+
+ ## Contributors
 
+<a href="https://github.com/knucklesuganda/py_assimilator/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=knucklesuganda/py_assimilator" />
+</a>
 
 ## Stars history
 
 [![Star History Chart](https://api.star-history.com/svg?repos=knucklesuganda/py_assimilator&type=Date)](https://star-history.com/#knucklesuganda/py_assimilator&Date)
 
 
+## ⭐Stargazers⭐
+
+We love all people who star our library. You can look at all stargazers in the documentation:
+
+https://knucklesuganda.github.io/py_assimilator/#stars-history
+
+> If you star the library you will appear there as well!
+
+
 ## Types of patterns
 These are different use cases for the patterns implemented:
 
 - Database - patterns for database/data layer interactions.
 - Events(in development) - projects with events or event-driven architecture.
 - Unidentified - patterns that are useful for different purposes.
```

#### html2text {}

```diff
@@ -1,57 +1,59 @@
 # Assimilator - the best Python patterns for the best projects
                                 [PyAssimilator]
                         [License] [Stars] [Last_commit]
-## Install now * `pip install py-assimilator` * `pip install py-assimilator
-[alchemy]` - Optional SQLAlchemy support * `pip install py-assimilator[kafka]`
-- Optional Kafka support * `pip install py-assimilator[redis]` - Optional Redis
-support * `pip install py-assimilator[mongo]` - Optional MongoDB support ##
-What is that all about? 1. We want to write the best code. 2. We need the best
-patterns and techniques for this. 3. We use PyAssimilator and save lots of
-time. 4. We use PyAssimilator and write the best code. 4. We use PyAssimilator
-and use the best patterns. 6. We use PyAssimilator and have no dependencies in
-our code. 7. We use PyAssimilator and can switch one database to another in a
-matter of seconds. 7. We learn PyAssimilator once and use it forever! 7. **And
-most importantly, we make Python projects better!** ## Code comparison Before
-PyAssimilator: ```Python # BAD CODE :( def create_user(username: str, email:
-str): # NO PATTERNS! # ONLY ONE DATABASE CHOICE! new_user = User
-(username=username, email=email, balance=0) # DEPENDENCY! session = db_session
-() # DEPENDENCY! session.add(new_user) session.commit() # NO ACID TRANSACTIONS!
-return new_user ``` After: ```Python # GOOD CODE :) def create_user(username:
-str, email: str, uow: UnitOfWork): # BEST DDD PATTERNS # PATTERN SUBSTITUTION/
-MULTIPLE DATABASES AT ONCE with uow: # ACID TRANSACTIONS IN ANY DATABASE
-new_user = uow.repository.save( username=username, # NO MODEL DEPENDENCIES
-email=email, balance=0, ) uow.commit() # AUTO ROLLBACK return new_user ``` ##
-So, do I really need it? If you want to spend less time writing your code, but
-write better code - then you must use PyAssimilator. It can be hard to start if
-you have no experience with good code, so you can watch creator's [video
-tutorials](https://knucklesuganda.github.io/py_assimilator/video_tutorials/).
-## Our vision Make Python the best programming language for enterprise
-development and use all of its dynamic capabilities to write things that other
-languages can't even comprehend! - Pattern substitution(switch databases
-easily) âï¸ - Event-based apps(in development) ð ï¸ - 45% of all Python
-projects use PyAssimilator ð ï¸ - Independent code(in development) ð ï¸ -
-Adaptive patterns(in development) ð ï¸ - Automatic code improvements(in
-development) ð ï¸ - Decentralized code management(in development) ð ï¸ If
-you want to help with any of those things - be free to contribute to the
-project. Remember, you never do anything for free - and that will not be the
-case either. ## Sources * [Github](https://github.com/knucklesuganda/
-py_assimilator) * [PyPI](https://pypi.org/project/py-assimilator/) *
-[Documentation](https://knucklesuganda.github.io/py_assimilator/) * [Github]
-(https://github.com/knucklesuganda/py_assimilator) * [Author's YouTube RU]
-(https://www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw) * [Author's YouTube
-ENG](https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA) ## Stars history
-[![Star History Chart](https://api.star-history.com/svg?repos=knucklesuganda/
+## Install now * `pip install py-assimilator` ## What is that all about? 1. We
+want to write the best code. 2. We need the best patterns and techniques for
+this. 3. We use PyAssimilator and save lots of time. 4. We use PyAssimilator
+and write the best code. 4. We use PyAssimilator and use the best patterns. 6.
+We use PyAssimilator and have no dependencies in our code. 7. We use
+PyAssimilator and can switch one database to another in a matter of seconds. 7.
+We learn PyAssimilator once and use it forever! 7. **And most importantly, we
+make Python projects better!** ## Code comparison Before PyAssimilator:
+```Python # BAD CODE :( def create_user(username: str, email: str): # NO
+PATTERNS! # ONLY ONE DATABASE CHOICE! new_user = User(username=username,
+email=email, balance=0) # DEPENDENCY! session = db_session() # DEPENDENCY!
+session.add(new_user) session.commit() # NO ACID TRANSACTIONS! return new_user
+``` After: ```Python # GOOD CODE :) def create_user(username: str, email: str,
+uow: UnitOfWork): # BEST DDD PATTERNS # PATTERN SUBSTITUTION/MULTIPLE DATABASES
+AT ONCE with uow: # ACID TRANSACTIONS IN ANY DATABASE new_user =
+uow.repository.save( username=username, # NO MODEL DEPENDENCIES email=email,
+balance=0, ) uow.commit() # AUTO ROLLBACK return new_user ``` ## So, do I
+really need it? If you want to spend less time writing your code, but write
+better code - then you must use PyAssimilator. It can be hard to start if you
+have no experience with good code, so you can watch creator's [video tutorials]
+(https://knucklesuganda.github.io/py_assimilator/video_tutorials/). ## Our
+vision Make Python the best programming language for enterprise development and
+use all of its dynamic capabilities to write things that other languages can't
+even comprehend! - Pattern substitution(switch databases easily) âï¸ -
+Event-based apps(in development) ð ï¸ - 45% of all Python projects use
+PyAssimilator ð ï¸ - Independent code(in development) ð ï¸ - Adaptive
+patterns(in development) ð ï¸ - Automatic code improvements(in development)
+ð ï¸ - Decentralized code management(in development) ð ï¸ If you want to
+help with any of those things - be free to contribute to the project. Remember,
+you never do anything for free - and that will not be the case either. ##
+Sources * [Github](https://github.com/knucklesuganda/py_assimilator) * [PyPI]
+(https://pypi.org/project/py-assimilator/) * [Documentation](https://
+knucklesuganda.github.io/py_assimilator/) * [Github](https://github.com/
+knucklesuganda/py_assimilator) * [Author's YouTube RU](https://www.youtube.com/
+channel/UCSNpJHMOU7FqjD4Ttux0uuw) * [Author's YouTube ENG](https://
+www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA) * [Discord channel](https://
+discord.gg/gTVaGu7DHN) ## Contributors [https://contrib.rocks/
+image?repo=knucklesuganda/py_assimilator] ## Stars history [![Star History
+Chart](https://api.star-history.com/svg?repos=knucklesuganda/
 py_assimilator&type=Date)](https://star-history.com/#knucklesuganda/
-py_assimilator&Date) ## Types of patterns These are different use cases for the
-patterns implemented: - Database - patterns for database/data layer
-interactions. - Events(in development) - projects with events or event-driven
-architecture. - Unidentified - patterns that are useful for different purposes.
-## Available providers Providers are different patterns for external modules
-like SQLAlchemy or FastAPI. - Alchemy(Database, Events) - patterns for
+py_assimilator&Date) ## â­Stargazersâ­ We love all people who star our
+library. You can look at all stargazers in the documentation: https://
+knucklesuganda.github.io/py_assimilator/#stars-history > If you star the
+library you will appear there as well! ## Types of patterns These are different
+use cases for the patterns implemented: - Database - patterns for database/data
+layer interactions. - Events(in development) - projects with events or event-
+driven architecture. - Unidentified - patterns that are useful for different
+purposes. ## Available providers Providers are different patterns for external
+modules like SQLAlchemy or FastAPI. - Alchemy(Database, Events) - patterns for
 [SQLAlchemy](https://docs.sqlalchemy.org/en/20/) for both database and events.
 - Kafka(Events) - patterns in [Kafka](https://kafka.apache.org/) related to
 events. - Internal(Database, Events) - internal is the type of provider that
 saves everything in memory(dict, list and all the tools within your app). -
 Redis(Database, Events) - redis_ allows us to work with [Redis](https://
 redis.io/) memory database. - MongoDB(Database) - mongo allows us to work with
 [MongoDB](https://www.mongodb.com/) database.
```

### Comparing `py_assimilator-1.2.2/pyproject.toml` & `py_assimilator-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ignore-vcs = true
 include = [
     "assimilator"
 ]
 
 [project]
 name = "py_assimilator"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Andrey Ivanov", email="python.on.papyrus@gmail.com" },
 ]
 maintainers = [
   { name="Andrey Ivanov", email="python.on.papyrus@gmail.com" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "Events", "Architecture", "Patterns", "Backend"]
```

### Comparing `py_assimilator-1.2.2/PKG-INFO` & `py_assimilator-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_assimilator
-Version: 1.2.2
+Version: 1.2.3
 Summary: The best Domain-driven design patterns for your projects
 Project-URL: Documentation, https://knucklesuganda.github.io/py_assimilator/
 Project-URL: Github, https://github.com/knucklesuganda/py_assimilator/
 Project-URL: Youtube RU, https://www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw
 Project-URL: Youtube ENG, https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA
 Author-email: Andrey Ivanov <python.on.papyrus@gmail.com>
 Maintainer-email: Andrey Ivanov <python.on.papyrus@gmail.com>
@@ -65,19 +65,14 @@
     <img src="https://img.shields.io/github/last-commit/knucklesuganda/py_assimilator?color=%237e56c2&style=for-the-badge" alt="Last commit">
 </a>
 </p>
 
 
 ## Install now
 * `pip install py-assimilator`
-* `pip install py-assimilator[alchemy]` - Optional SQLAlchemy support 
-* `pip install py-assimilator[kafka]` - Optional Kafka support 
-* `pip install py-assimilator[redis]` - Optional Redis support 
-* `pip install py-assimilator[mongo]` - Optional MongoDB support 
-
 
 ## What is that all about?
 
 1. We want to write the best code.
 2. We need the best patterns and techniques for this.
 3. We use PyAssimilator and save lots of time.
 4. We use PyAssimilator and write the best code.
@@ -150,21 +145,36 @@
 ## Sources
 * [Github](https://github.com/knucklesuganda/py_assimilator)
 * [PyPI](https://pypi.org/project/py-assimilator/)
 * [Documentation](https://knucklesuganda.github.io/py_assimilator/)
 * [Github](https://github.com/knucklesuganda/py_assimilator)
 * [Author's YouTube RU](https://www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw)
 * [Author's YouTube ENG](https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA)
+* [Discord channel](https://discord.gg/gTVaGu7DHN)
+
+ ## Contributors
 
+<a href="https://github.com/knucklesuganda/py_assimilator/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=knucklesuganda/py_assimilator" />
+</a>
 
 ## Stars history
 
 [![Star History Chart](https://api.star-history.com/svg?repos=knucklesuganda/py_assimilator&type=Date)](https://star-history.com/#knucklesuganda/py_assimilator&Date)
 
 
+## ⭐Stargazers⭐
+
+We love all people who star our library. You can look at all stargazers in the documentation:
+
+https://knucklesuganda.github.io/py_assimilator/#stars-history
+
+> If you star the library you will appear there as well!
+
+
 ## Types of patterns
 These are different use cases for the patterns implemented:
 
 - Database - patterns for database/data layer interactions.
 - Events(in development) - projects with events or event-driven architecture.
 - Unidentified - patterns that are useful for different purposes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py_assimilator Version: 1.2.2 Summary: The best
+Metadata-Version: 2.1 Name: py_assimilator Version: 1.2.3 Summary: The best
 Domain-driven design patterns for your projects Project-URL: Documentation,
 https://knucklesuganda.github.io/py_assimilator/ Project-URL: Github, https://
 github.com/knucklesuganda/py_assimilator/ Project-URL: Youtube RU, https://
 www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw Project-URL: Youtube ENG,
 https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA Author-email: Andrey
 Ivanov
 on.papyrus@gmail.com> Maintainer-email: Andrey Ivanov
@@ -29,61 +29,63 @@
 alchemy Requires-Dist: sqlalchemy>=2.0.0; extra == 'alchemy' Provides-Extra:
 kafka Requires-Dist: kafka-python>=2.0.2; extra == 'kafka' Provides-Extra:
 mongo Requires-Dist: pymongo>=4.3.3; extra == 'mongo' Provides-Extra: redis
 Requires-Dist: redis>=4.4.0; extra == 'redis' Description-Content-Type: text/
 markdown # Assimilator - the best Python patterns for the best projects
                                 [PyAssimilator]
                         [License] [Stars] [Last_commit]
-## Install now * `pip install py-assimilator` * `pip install py-assimilator
-[alchemy]` - Optional SQLAlchemy support * `pip install py-assimilator[kafka]`
-- Optional Kafka support * `pip install py-assimilator[redis]` - Optional Redis
-support * `pip install py-assimilator[mongo]` - Optional MongoDB support ##
-What is that all about? 1. We want to write the best code. 2. We need the best
-patterns and techniques for this. 3. We use PyAssimilator and save lots of
-time. 4. We use PyAssimilator and write the best code. 4. We use PyAssimilator
-and use the best patterns. 6. We use PyAssimilator and have no dependencies in
-our code. 7. We use PyAssimilator and can switch one database to another in a
-matter of seconds. 7. We learn PyAssimilator once and use it forever! 7. **And
-most importantly, we make Python projects better!** ## Code comparison Before
-PyAssimilator: ```Python # BAD CODE :( def create_user(username: str, email:
-str): # NO PATTERNS! # ONLY ONE DATABASE CHOICE! new_user = User
-(username=username, email=email, balance=0) # DEPENDENCY! session = db_session
-() # DEPENDENCY! session.add(new_user) session.commit() # NO ACID TRANSACTIONS!
-return new_user ``` After: ```Python # GOOD CODE :) def create_user(username:
-str, email: str, uow: UnitOfWork): # BEST DDD PATTERNS # PATTERN SUBSTITUTION/
-MULTIPLE DATABASES AT ONCE with uow: # ACID TRANSACTIONS IN ANY DATABASE
-new_user = uow.repository.save( username=username, # NO MODEL DEPENDENCIES
-email=email, balance=0, ) uow.commit() # AUTO ROLLBACK return new_user ``` ##
-So, do I really need it? If you want to spend less time writing your code, but
-write better code - then you must use PyAssimilator. It can be hard to start if
-you have no experience with good code, so you can watch creator's [video
-tutorials](https://knucklesuganda.github.io/py_assimilator/video_tutorials/).
-## Our vision Make Python the best programming language for enterprise
-development and use all of its dynamic capabilities to write things that other
-languages can't even comprehend! - Pattern substitution(switch databases
-easily) âï¸ - Event-based apps(in development) ð ï¸ - 45% of all Python
-projects use PyAssimilator ð ï¸ - Independent code(in development) ð ï¸ -
-Adaptive patterns(in development) ð ï¸ - Automatic code improvements(in
-development) ð ï¸ - Decentralized code management(in development) ð ï¸ If
-you want to help with any of those things - be free to contribute to the
-project. Remember, you never do anything for free - and that will not be the
-case either. ## Sources * [Github](https://github.com/knucklesuganda/
-py_assimilator) * [PyPI](https://pypi.org/project/py-assimilator/) *
-[Documentation](https://knucklesuganda.github.io/py_assimilator/) * [Github]
-(https://github.com/knucklesuganda/py_assimilator) * [Author's YouTube RU]
-(https://www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw) * [Author's YouTube
-ENG](https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA) ## Stars history
-[![Star History Chart](https://api.star-history.com/svg?repos=knucklesuganda/
+## Install now * `pip install py-assimilator` ## What is that all about? 1. We
+want to write the best code. 2. We need the best patterns and techniques for
+this. 3. We use PyAssimilator and save lots of time. 4. We use PyAssimilator
+and write the best code. 4. We use PyAssimilator and use the best patterns. 6.
+We use PyAssimilator and have no dependencies in our code. 7. We use
+PyAssimilator and can switch one database to another in a matter of seconds. 7.
+We learn PyAssimilator once and use it forever! 7. **And most importantly, we
+make Python projects better!** ## Code comparison Before PyAssimilator:
+```Python # BAD CODE :( def create_user(username: str, email: str): # NO
+PATTERNS! # ONLY ONE DATABASE CHOICE! new_user = User(username=username,
+email=email, balance=0) # DEPENDENCY! session = db_session() # DEPENDENCY!
+session.add(new_user) session.commit() # NO ACID TRANSACTIONS! return new_user
+``` After: ```Python # GOOD CODE :) def create_user(username: str, email: str,
+uow: UnitOfWork): # BEST DDD PATTERNS # PATTERN SUBSTITUTION/MULTIPLE DATABASES
+AT ONCE with uow: # ACID TRANSACTIONS IN ANY DATABASE new_user =
+uow.repository.save( username=username, # NO MODEL DEPENDENCIES email=email,
+balance=0, ) uow.commit() # AUTO ROLLBACK return new_user ``` ## So, do I
+really need it? If you want to spend less time writing your code, but write
+better code - then you must use PyAssimilator. It can be hard to start if you
+have no experience with good code, so you can watch creator's [video tutorials]
+(https://knucklesuganda.github.io/py_assimilator/video_tutorials/). ## Our
+vision Make Python the best programming language for enterprise development and
+use all of its dynamic capabilities to write things that other languages can't
+even comprehend! - Pattern substitution(switch databases easily) âï¸ -
+Event-based apps(in development) ð ï¸ - 45% of all Python projects use
+PyAssimilator ð ï¸ - Independent code(in development) ð ï¸ - Adaptive
+patterns(in development) ð ï¸ - Automatic code improvements(in development)
+ð ï¸ - Decentralized code management(in development) ð ï¸ If you want to
+help with any of those things - be free to contribute to the project. Remember,
+you never do anything for free - and that will not be the case either. ##
+Sources * [Github](https://github.com/knucklesuganda/py_assimilator) * [PyPI]
+(https://pypi.org/project/py-assimilator/) * [Documentation](https://
+knucklesuganda.github.io/py_assimilator/) * [Github](https://github.com/
+knucklesuganda/py_assimilator) * [Author's YouTube RU](https://www.youtube.com/
+channel/UCSNpJHMOU7FqjD4Ttux0uuw) * [Author's YouTube ENG](https://
+www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA) * [Discord channel](https://
+discord.gg/gTVaGu7DHN) ## Contributors [https://contrib.rocks/
+image?repo=knucklesuganda/py_assimilator] ## Stars history [![Star History
+Chart](https://api.star-history.com/svg?repos=knucklesuganda/
 py_assimilator&type=Date)](https://star-history.com/#knucklesuganda/
-py_assimilator&Date) ## Types of patterns These are different use cases for the
-patterns implemented: - Database - patterns for database/data layer
-interactions. - Events(in development) - projects with events or event-driven
-architecture. - Unidentified - patterns that are useful for different purposes.
-## Available providers Providers are different patterns for external modules
-like SQLAlchemy or FastAPI. - Alchemy(Database, Events) - patterns for
+py_assimilator&Date) ## â­Stargazersâ­ We love all people who star our
+library. You can look at all stargazers in the documentation: https://
+knucklesuganda.github.io/py_assimilator/#stars-history > If you star the
+library you will appear there as well! ## Types of patterns These are different
+use cases for the patterns implemented: - Database - patterns for database/data
+layer interactions. - Events(in development) - projects with events or event-
+driven architecture. - Unidentified - patterns that are useful for different
+purposes. ## Available providers Providers are different patterns for external
+modules like SQLAlchemy or FastAPI. - Alchemy(Database, Events) - patterns for
 [SQLAlchemy](https://docs.sqlalchemy.org/en/20/) for both database and events.
 - Kafka(Events) - patterns in [Kafka](https://kafka.apache.org/) related to
 events. - Internal(Database, Events) - internal is the type of provider that
 saves everything in memory(dict, list and all the tools within your app). -
 Redis(Database, Events) - redis_ allows us to work with [Redis](https://
 redis.io/) memory database. - MongoDB(Database) - mongo allows us to work with
 [MongoDB](https://www.mongodb.com/) database.
```

