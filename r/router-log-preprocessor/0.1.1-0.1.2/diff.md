# Comparing `tmp/router_log_preprocessor-0.1.1.tar.gz` & `tmp/router_log_preprocessor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "router_log_preprocessor-0.1.1.tar", max compression
+gzip compressed data, was "router_log_preprocessor-0.1.2.tar", max compression
```

## Comparing `router_log_preprocessor-0.1.1.tar` & `router_log_preprocessor-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.1/LICENSE
--rw-r--r--   0        0        0     1384 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.1/README.md
--rw-r--r--   0        0        0      794 2023-04-04 19:54:56.399186 router_log_preprocessor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.1/router_log_preprocessor/__init__.py
--rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.1/router_log_preprocessor/__main__.py
--rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__init__.py
--rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
--rw-r--r--   0        0        0     1317 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
--rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/_dnsmasq_dhcp.py
--rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/_message.py
--rw-r--r--   0        0        0     1536 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/domain/_wlc.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/__init__.py
--rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/abc.py
--rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__init__.py
--rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
--rw-r--r--   0        0        0     1839 2023-04-04 19:37:27.472797 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     3872 2023-04-04 19:07:48.135263 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
--rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/_known_clients.py
--rw-r--r--   0        0        0     2646 2023-04-04 19:37:25.988779 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/_mapper.py
--rw-r--r--   0        0        0     4747 2023-04-04 19:07:45.231229 router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/_trapper.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__init__.py
--rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
--rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
--rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/handler.py
--rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/server.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__init__.py
--rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
--rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
--rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
--rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/typing.py
--rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/wlc.py
--rw-r--r--   0        0        0     2192 2023-04-04 19:21:22.415159 router_log_preprocessor-0.1.1/router_log_preprocessor/settings.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/util/__init__.py
--rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.1/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.1/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
--rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.1/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
--rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/util/logging.py
--rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.1/router_log_preprocessor/util/rfc3164_parser.py
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.1/setup.py
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.2/README.md
+-rw-r--r--   0        0        0      794 2023-04-13 13:07:15.158555 router_log_preprocessor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/router_log_preprocessor/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/router_log_preprocessor/__main__.py
+-rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
+-rw-r--r--   0        0        0     1317 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
+-rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_dnsmasq_dhcp.py
+-rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_message.py
+-rw-r--r--   0        0        0     1536 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_wlc.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/abc.py
+-rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
+-rw-r--r--   0        0        0     1907 2023-04-13 12:48:57.905739 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
+-rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_known_clients.py
+-rw-r--r--   0        0        0     2654 2023-04-13 12:48:56.785731 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_mapper.py
+-rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_trapper.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
+-rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
+-rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/handler.py
+-rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/server.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
+-rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
+-rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/typing.py
+-rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/wlc.py
+-rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.2/router_log_preprocessor/settings.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
+-rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/util/logging.py
+-rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/util/rfc3164_parser.py
+-rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.2/setup.py
+-rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.2/PKG-INFO
```

### Comparing `router_log_preprocessor-0.1.1/LICENSE` & `router_log_preprocessor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/pyproject.toml` & `router_log_preprocessor-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "router-log-preprocessor"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 repository = "https://github.com/mastdi/router-log-preprocessor"
 authors = ["Martin Storgaard Dieu <martin@storgaarddieu.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "router_log_preprocessor"}]
```

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/__main__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/_dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/_message.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_message.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/domain/_wlc.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/abc.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/abc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  4 19:37:25 2023 UTC, .py size: 2646 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,120 @@
-00000000: 550d 0d0a 0000 0000 757c 2c64 560a 0000  U.......u|,dV...
+00000000: 550d 0d0a 0000 0000 38fa 3764 5e0a 0000  U.......8.7d^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 6d07 5a07 0100 6400 6401 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 0200 0100 6d0a 0200 0100 6d0b 5a0b  m.....m.....m.Z.
-00000080: 0100 6507 6a0c 6507 6a0d 6505 6a0e 6402  ..e.j.e.j.e.j.d.
-00000090: 9c03 6403 6404 8404 5a0f 6507 6a0c 650b  ..d.d...Z.e.j.e.
-000000a0: 6a10 6505 6a0e 6405 9c03 6406 6407 8404  j.e.j.d...d.d...
-000000b0: 5a11 6401 5300 2908 e900 0000 004e 2903  Z.d.S.)......N).
-000000c0: da06 7265 636f 7264 da07 6d65 7373 6167  ..record..messag
-000000d0: 65da 0672 6574 7572 6e63 0200 0000 0000  e..returnc......
-000000e0: 0000 0000 0000 0800 0000 0c00 0000 4300  ..............C.
-000000f0: 0000 73c6 0000 007c 006a 0064 006b 0973  ..s....|.j.d.k.s
-00000100: 0e74 0182 017c 006a 00a0 02a1 00a0 0364  .t...|.j.......d
-00000110: 0164 02a1 027d 0274 047c 006a 05a0 05a1  .d...}.t.|.j....
-00000120: 0083 017d 0374 06a0 07a1 007d 0474 08a0  ...}.t.....}.t..
-00000130: 097c 01a1 017d 057c 0544 005d 7c7d 067c  .|...}.|.D.]|}.|
-00000140: 066a 0a64 036b 0272 5471 4474 0b7c 017c  .j.d.k.rTqDt.|.|
-00000150: 066a 0a83 027d 0774 0c7c 0774 0d6a 0e83  .j...}.t.|.t.j..
-00000160: 0272 747c 076a 0f7d 076e 1a74 0c7c 0774  .rt|.j.}.n.t.|.t
-00000170: 106a 1174 106a 1266 0283 0272 8e74 137c  .j.t.j.f...r.t.|
-00000180: 0783 017d 077c 04a0 1474 066a 157c 006a  ...}.|...t.j.|.j
-00000190: 1664 047c 029b 0064 057c 066a 0a9b 0064  .d.|...d.|.j...d
-000001a0: 067c 016a 179b 0064 079d 077c 077c 0364  .|.j...d...|.|.d
-000001b0: 088d 04a1 0101 0071 447c 0453 0029 094e  .......qD|.S.).N
-000001c0: fa01 2dda 015f da0b 6d61 635f 6164 6472  ..-.._..mac_addr
-000001d0: 6573 737a 0472 6c70 2efa 015b fa01 2cfa  essz.rlp...[..,.
-000001e0: 015d a904 da04 686f 7374 da03 6b65 79da  .]....host..key.
-000001f0: 0576 616c 7565 da05 636c 6f63 6b29 18da  .value..clock)..
-00000200: 0770 726f 6365 7373 da0e 4173 7365 7274  .process..Assert
-00000210: 696f 6e45 7272 6f72 da05 6c6f 7765 72da  ionError..lower.
-00000220: 0772 6570 6c61 6365 da03 696e 74da 0974  .replace..int..t
-00000230: 696d 6573 7461 6d70 da15 6173 796e 6369  imestamp..asynci
-00000240: 6f5f 7a61 6262 6978 5f73 656e 6465 72da  o_zabbix_sender.
-00000250: 0c4d 6561 7375 7265 6d65 6e74 73da 0b64  .Measurements..d
-00000260: 6174 6163 6c61 7373 6573 da06 6669 656c  ataclasses..fiel
-00000270: 6473 da04 6e61 6d65 da07 6765 7461 7474  ds..name..getatt
-00000280: 72da 0a69 7369 6e73 7461 6e63 65da 0465  r..isinstance..e
-00000290: 6e75 6dda 0445 6e75 6d72 0e00 0000 da09  num..Enumr......
-000002a0: 6970 6164 6472 6573 73da 0b49 5076 3441  ipaddress..IPv4A
-000002b0: 6464 7265 7373 da0b 4950 7636 4164 6472  ddress..IPv6Addr
-000002c0: 6573 73da 0373 7472 da0f 6164 645f 6d65  ess..str..add_me
-000002d0: 6173 7572 656d 656e 74da 0b4d 6561 7375  asurement..Measu
-000002e0: 7265 6d65 6e74 da08 686f 7374 6e61 6d65  rement..hostname
-000002f0: 7207 0000 0029 0872 0200 0000 7203 0000  r....).r....r...
-00000300: 0072 1000 0000 720f 0000 00da 0c6d 6561  .r....r......mea
-00000310: 7375 7265 6d65 6e74 735a 0c6d 6f64 656c  surementsZ.model
-00000320: 5f66 6965 6c64 73da 0566 6965 6c64 720e  _fields..fieldr.
-00000330: 0000 00a9 0072 2800 0000 fa69 2f68 6f6d  .....r(....i/hom
-00000340: 652f 6d79 732f 446f 6375 6d65 6e74 732f  e/mys/Documents/
-00000350: 4769 7448 7562 2f6d 6173 7464 692f 726f  GitHub/mastdi/ro
-00000360: 7574 6572 2d6c 6f67 2d70 7265 7072 6f63  uter-log-preproc
-00000370: 6573 736f 722f 726f 7574 6572 5f6c 6f67  essor/router_log
-00000380: 5f70 7265 7072 6f63 6573 736f 722f 686f  _preprocessor/ho
-00000390: 6f6b 732f 7a61 6262 6978 2f5f 6d61 7070  oks/zabbix/_mapp
-000003a0: 6572 2e70 79da 126d 6170 5f63 6c69 656e  er.py..map_clien
-000003b0: 745f 6d65 7373 6167 651a 0000 0073 2c00  t_message....s,.
-000003c0: 0000 0003 0e03 1202 0e03 0801 0a01 0801  ................
-000003d0: 0a01 0201 0c01 0c01 0801 1201 0801 0401  ................
-000003e0: 0401 0401 1a01 0201 02fc 04ff 0608 722a  ..............r*
-000003f0: 0000 0029 0372 0200 0000 da0d 6b6e 6f77  ...).r......know
-00000400: 6e5f 636c 6965 6e74 7372 0400 0000 6302  n_clientsr....c.
-00000410: 0000 0000 0000 0000 0000 0003 0000 0009  ................
-00000420: 0000 0043 0000 0073 6400 0000 7c00 6a00  ...C...sd...|.j.
-00000430: 6400 6b09 730e 7401 8201 7402 6a03 6401  d.k.s.t...t.j.d.
-00000440: 6402 8400 7c01 a004 7c00 6a00 a101 4400  d...|...|.j...D.
-00000450: 8301 6400 6403 6404 8d03 7d02 7405 a006  ..d.d.d...}.t...
-00000460: 7405 6a07 7c00 6a08 6405 7c00 6a00 a009  t.j.|.j.d.|.j...
-00000470: a100 9b00 6406 9d03 7c02 740a 7c00 6a0b  ....d...|.t.|.j.
-00000480: a00b a100 8301 6407 8d04 6701 a101 5300  ......d...g...S.
-00000490: 2908 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-000004a0: 0200 0000 0500 0000 5300 0000 7318 0000  ........S...s...
-000004b0: 0067 007c 005d 107d 0164 0074 007c 0183  .g.|.].}.d.t.|..
-000004c0: 0169 0191 0271 0453 0029 01da 036d 6163  .i...q.S.)...mac
-000004d0: 2901 7222 0000 0029 02da 022e 3072 2c00  ).r"...)....0r,.
-000004e0: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
-000004f0: 00da 0a3c 6c69 7374 636f 6d70 3e3f 0000  ...<listcomp>?..
-00000500: 0073 0400 0000 0600 0200 7a28 6d61 705f  .s........z(map_
-00000510: 636c 6965 6e74 5f64 6973 636f 7665 7279  client_discovery
-00000520: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000530: 6f6d 703e 2902 7209 0000 00fa 013a 2902  omp>).r......:).
-00000540: da06 696e 6465 6e74 da0a 7365 7061 7261  ..indent..separa
-00000550: 746f 7273 7a15 726c 702e 636c 6965 6e74  torsz.rlp.client
-00000560: 5f64 6973 636f 7665 7279 5b72 0a00 0000  _discovery[r....
-00000570: 720b 0000 0029 0c72 1000 0000 7211 0000  r....).r....r...
-00000580: 00da 046a 736f 6eda 0564 756d 7073 da07  ...json..dumps..
-00000590: 636c 6965 6e74 7372 1600 0000 7217 0000  clientsr....r...
-000005a0: 0072 2400 0000 7225 0000 0072 1200 0000  .r$...r%...r....
-000005b0: 7214 0000 0072 1500 0000 2903 7202 0000  r....r....).r...
-000005c0: 0072 2b00 0000 720e 0000 0072 2800 0000  .r+...r....r(...
-000005d0: 7228 0000 0072 2900 0000 da14 6d61 705f  r(...r).....map_
-000005e0: 636c 6965 6e74 5f64 6973 636f 7665 7279  client_discovery
-000005f0: 3a00 0000 731c 0000 0000 030e 0104 0114  :...s...........
-00000600: 0102 0102 fd06 0504 0104 0104 0110 0102  ................
-00000610: 010c fc04 ff72 3500 0000 2912 7218 0000  .....r5...).r...
-00000620: 0072 1d00 0000 721f 0000 0072 3200 0000  .r....r....r2...
-00000630: da06 7479 7069 6e67 7216 0000 00da 1e72  ..typingr......r
-00000640: 6f75 7465 725f 6c6f 675f 7072 6570 726f  outer_log_prepro
-00000650: 6365 7373 6f72 2e64 6f6d 6169 6eda 0664  cessor.domain..d
-00000660: 6f6d 6169 6eda 3372 6f75 7465 725f 6c6f  omain.3router_lo
-00000670: 675f 7072 6570 726f 6365 7373 6f72 2e68  g_preprocessor.h
-00000680: 6f6f 6b73 2e7a 6162 6269 782e 5f6b 6e6f  ooks.zabbix._kno
-00000690: 776e 5f63 6c69 656e 7473 da05 686f 6f6b  wn_clients..hook
-000006a0: 73da 067a 6162 6269 78da 0e5f 6b6e 6f77  s..zabbix.._know
-000006b0: 6e5f 636c 6965 6e74 73da 094c 6f67 5265  n_clients..LogRe
-000006c0: 636f 7264 da07 4d65 7373 6167 6572 1700  cord..Messager..
-000006d0: 0000 722a 0000 00da 0c4b 6e6f 776e 436c  ..r*.....KnownCl
-000006e0: 6965 6e74 7372 3500 0000 7228 0000 0072  ientsr5...r(...r
-000006f0: 2800 0000 7228 0000 0072 2900 0000 da08  (...r(...r).....
-00000700: 3c6d 6f64 756c 653e 0e00 0000 731e 0000  <module>....s...
-00000710: 0008 0108 0108 0108 0108 0208 020c 0118  ................
-00000720: 0404 0004 0104 fe0c 2104 0004 0104 fe    ........!......
+00000080: 0100 6507 6a0c 6507 6a0d 6504 6a0e 6505  ..e.j.e.j.e.j.e.
+00000090: 6a0f 6401 6401 6603 1900 6402 9c03 6403  j.d.d.f...d...d.
+000000a0: 6404 8404 5a10 6507 6a0c 650b 6a11 6505  d...Z.e.j.e.j.e.
+000000b0: 6a12 6405 9c03 6406 6407 8404 5a13 6401  j.d...d.d...Z.d.
+000000c0: 5300 2908 e900 0000 004e 2903 da06 7265  S.)......N)...re
+000000d0: 636f 7264 da07 6d65 7373 6167 65da 0672  cord..message..r
+000000e0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
+000000f0: 0000 0800 0000 0a00 0000 6300 0000 73d8  ..........c...s.
+00000100: 0000 007c 006a 0064 006b 0973 0e74 0182  ...|.j.d.k.s.t..
+00000110: 017c 006a 00a0 02a1 00a0 0364 0164 02a1  .|.j.......d.d..
+00000120: 027d 0274 047c 006a 05a0 05a1 0083 017d  .}.t.|.j.......}
+00000130: 0364 007d 0474 067c 0174 076a 0883 0272  .d.}.t.|.t.j...r
+00000140: 4a7c 016a 096a 0a64 0314 007d 0474 0ba0  J|.j.j.d...}.t..
+00000150: 0c7c 01a1 017d 057c 0544 005d 7a7d 067c  .|...}.|.D.]z}.|
+00000160: 066a 0d64 046b 0272 6871 5874 0e7c 017c  .j.d.k.rhqXt.|.|
+00000170: 066a 0d83 027d 0774 067c 0774 0f6a 1083  .j...}.t.|.t.j..
+00000180: 0272 887c 076a 0a7d 076e 1a74 067c 0774  .r.|.j.}.n.t.|.t
+00000190: 116a 1274 116a 1366 0283 0272 a274 147c  .j.t.j.f...r.t.|
+000001a0: 0783 017d 0774 156a 167c 006a 1764 057c  ...}.t.j.|.j.d.|
+000001b0: 029b 0064 067c 066a 0d9b 0064 077c 016a  ...d.|.j...d.|.j
+000001c0: 189b 0064 089d 077c 077c 037c 0464 098d  ...d...|.|.|.d..
+000001d0: 0556 0001 0071 5864 0053 0029 0a4e fa01  .V...qXd.S.).N..
+000001e0: 2dda 015f 6940 420f 00da 0b6d 6163 5f61  -.._i@B....mac_a
+000001f0: 6464 7265 7373 7a04 726c 702e fa01 5bfa  ddressz.rlp...[.
+00000200: 012c fa01 5d29 05da 0468 6f73 74da 036b  .,..])...host..k
+00000210: 6579 da05 7661 6c75 65da 0563 6c6f 636b  ey..value..clock
+00000220: da02 6e73 2919 da07 7072 6f63 6573 73da  ..ns)...process.
+00000230: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
+00000240: 056c 6f77 6572 da07 7265 706c 6163 65da  .lower..replace.
+00000250: 0369 6e74 da09 7469 6d65 7374 616d 70da  .int..timestamp.
+00000260: 0a69 7369 6e73 7461 6e63 65da 0664 6f6d  .isinstance..dom
+00000270: 6169 6eda 0d57 6c63 4576 656e 744d 6f64  ain..WlcEventMod
+00000280: 656c da05 6576 656e 7472 0d00 0000 da0b  el..eventr......
+00000290: 6461 7461 636c 6173 7365 73da 0666 6965  dataclasses..fie
+000002a0: 6c64 73da 046e 616d 65da 0767 6574 6174  lds..name..getat
+000002b0: 7472 da04 656e 756d da04 456e 756d da09  tr..enum..Enum..
+000002c0: 6970 6164 6472 6573 73da 0b49 5076 3441  ipaddress..IPv4A
+000002d0: 6464 7265 7373 da0b 4950 7636 4164 6472  ddress..IPv6Addr
+000002e0: 6573 73da 0373 7472 da15 6173 796e 6369  ess..str..asynci
+000002f0: 6f5f 7a61 6262 6978 5f73 656e 6465 72da  o_zabbix_sender.
+00000300: 0b4d 6561 7375 7265 6d65 6e74 da08 686f  .Measurement..ho
+00000310: 7374 6e61 6d65 7207 0000 0029 0872 0200  stnamer....).r..
+00000320: 0000 7203 0000 0072 1000 0000 720e 0000  ..r....r....r...
+00000330: 0072 0f00 0000 5a0c 6d6f 6465 6c5f 6669  .r....Z.model_fi
+00000340: 656c 6473 da05 6669 656c 6472 0d00 0000  elds..fieldr....
+00000350: a900 7228 0000 00fa 692f 686f 6d65 2f6d  ..r(....i/home/m
+00000360: 7973 2f44 6f63 756d 656e 7473 2f47 6974  ys/Documents/Git
+00000370: 4875 622f 6d61 7374 6469 2f72 6f75 7465  Hub/mastdi/route
+00000380: 722d 6c6f 672d 7072 6570 726f 6365 7373  r-log-preprocess
+00000390: 6f72 2f72 6f75 7465 725f 6c6f 675f 7072  or/router_log_pr
+000003a0: 6570 726f 6365 7373 6f72 2f68 6f6f 6b73  eprocessor/hooks
+000003b0: 2f7a 6162 6269 782f 5f6d 6170 7065 722e  /zabbix/_mapper.
+000003c0: 7079 da12 6d61 705f 636c 6965 6e74 5f6d  py..map_client_m
+000003d0: 6573 7361 6765 1a00 0000 732c 0000 0000  essage....s,....
+000003e0: 030e 0312 020e 0104 010c 010c 030a 0108  ................
+000003f0: 010a 0102 010c 010c 0108 0112 0108 0104  ................
+00000400: 0104 011a 0102 0102 0102 fb72 2a00 0000  ...........r*...
+00000410: 2903 7202 0000 00da 0d6b 6e6f 776e 5f63  ).r......known_c
+00000420: 6c69 656e 7473 7204 0000 0063 0200 0000  lientsr....c....
+00000430: 0000 0000 0000 0000 0300 0000 0900 0000  ................
+00000440: 4300 0000 7364 0000 007c 006a 0064 006b  C...sd...|.j.d.k
+00000450: 0973 0e74 0182 0174 026a 0364 0164 0284  .s.t...t.j.d.d..
+00000460: 007c 01a0 047c 006a 00a1 0144 0083 0164  .|...|.j...D...d
+00000470: 0064 0364 048d 037d 0274 05a0 0674 056a  .d.d...}.t...t.j
+00000480: 077c 006a 0864 057c 006a 00a0 09a1 009b  .|.j.d.|.j......
+00000490: 0064 069d 037c 0274 0a7c 006a 0ba0 0ba1  .d...|.t.|.j....
+000004a0: 0083 0164 078d 0467 01a1 0153 0029 084e  ...d...g...S.).N
+000004b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000004c0: 0005 0000 0053 0000 0073 1800 0000 6700  .....S...s....g.
+000004d0: 7c00 5d10 7d01 6400 7400 7c01 8301 6901  |.].}.d.t.|...i.
+000004e0: 9102 7104 5300 2901 da03 6d61 6329 0172  ..q.S.)...mac).r
+000004f0: 2300 0000 2902 da02 2e30 722c 0000 0072  #...)....0r,...r
+00000500: 2800 0000 7228 0000 0072 2900 0000 da0a  (...r(...r).....
+00000510: 3c6c 6973 7463 6f6d 703e 3f00 0000 7304  <listcomp>?...s.
+00000520: 0000 0006 0002 007a 286d 6170 5f63 6c69  .......z(map_cli
+00000530: 656e 745f 6469 7363 6f76 6572 792e 3c6c  ent_discovery.<l
+00000540: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000550: 3e29 0272 0900 0000 fa01 3a29 02da 0669  >).r......:)...i
+00000560: 6e64 656e 74da 0a73 6570 6172 6174 6f72  ndent..separator
+00000570: 737a 1572 6c70 2e63 6c69 656e 745f 6469  sz.rlp.client_di
+00000580: 7363 6f76 6572 795b 720a 0000 0029 0472  scovery[r....).r
+00000590: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+000005a0: 0000 0029 0c72 1000 0000 7211 0000 00da  ...).r....r.....
+000005b0: 046a 736f 6eda 0564 756d 7073 da07 636c  .json..dumps..cl
+000005c0: 6965 6e74 7372 2400 0000 da0c 4d65 6173  ientsr$.....Meas
+000005d0: 7572 656d 656e 7473 7225 0000 0072 2600  urementsr%...r&.
+000005e0: 0000 7212 0000 0072 1400 0000 7215 0000  ..r....r....r...
+000005f0: 0029 0372 0200 0000 722b 0000 0072 0d00  .).r....r+...r..
+00000600: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
+00000610: 00da 146d 6170 5f63 6c69 656e 745f 6469  ...map_client_di
+00000620: 7363 6f76 6572 793a 0000 0073 1c00 0000  scovery:...s....
+00000630: 0003 0e01 0401 1401 0201 02fd 0605 0401  ................
+00000640: 0401 0401 1001 0201 0cfc 04ff 7236 0000  ............r6..
+00000650: 0029 1472 1a00 0000 721e 0000 0072 2000  .).r....r....r .
+00000660: 0000 7232 0000 00da 0674 7970 696e 6772  ..r2.....typingr
+00000670: 2400 0000 da1e 726f 7574 6572 5f6c 6f67  $.....router_log
+00000680: 5f70 7265 7072 6f63 6573 736f 722e 646f  _preprocessor.do
+00000690: 6d61 696e 7217 0000 00da 3372 6f75 7465  mainr.....3route
+000006a0: 725f 6c6f 675f 7072 6570 726f 6365 7373  r_log_preprocess
+000006b0: 6f72 2e68 6f6f 6b73 2e7a 6162 6269 782e  or.hooks.zabbix.
+000006c0: 5f6b 6e6f 776e 5f63 6c69 656e 7473 da05  _known_clients..
+000006d0: 686f 6f6b 73da 067a 6162 6269 78da 0e5f  hooks..zabbix.._
+000006e0: 6b6e 6f77 6e5f 636c 6965 6e74 73da 094c  known_clients..L
+000006f0: 6f67 5265 636f 7264 da07 4d65 7373 6167  ogRecord..Messag
+00000700: 65da 0947 656e 6572 6174 6f72 7225 0000  e..Generatorr%..
+00000710: 0072 2a00 0000 da0c 4b6e 6f77 6e43 6c69  .r*.....KnownCli
+00000720: 656e 7473 7235 0000 0072 3600 0000 7228  entsr5...r6...r(
+00000730: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
+00000740: 0000 da08 3c6d 6f64 756c 653e 0e00 0000  ....<module>....
+00000750: 731e 0000 0008 0108 0108 0108 0108 0208  s...............
+00000760: 020c 0118 0404 0004 0110 fe0c 2104 0004  ............!...
+00000770: 0104 fe                                  ...
```

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  4 19:07:45 2023 UTC, .py size: 4747 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,242 +1,264 @@
-00000000: 550d 0d0a 0000 0000 8175 2c64 8b12 0000  U........u,d....
+00000000: 550d 0d0a 0000 0000 89fa 3764 bc16 0000  U.........7d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 0200 0100 6d06 5a06 0100 6400 6401  m.....m.Z...d.d.
-00000060: 6c07 6d05 0200 0100 6d08 0200 0100 6d09  l.m.....m.....m.
-00000070: 5a0a 0100 6400 6401 6c0b 6d05 0200 0100  Z...d.d.l.m.....
-00000080: 6d08 0200 0100 6d0c 5a0d 0100 6400 6401  m.....m.Z...d.d.
-00000090: 6c0e 6d0f 0200 0100 6d10 5a10 0100 4700  l.m.....m.Z...G.
-000000a0: 6402 6403 8400 6403 6506 6a11 8303 5a12  d.d...d.e.j...Z.
-000000b0: 6401 5300 2904 e900 0000 004e 6300 0000  d.S.)......Nc...
-000000c0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-000000d0: 0000 0000 0073 5000 0000 6500 5a01 6400  .....sP...e.Z.d.
-000000e0: 5a02 640a 8700 6601 6402 6403 8409 5a03  Z.d...f.d.d...Z.
-000000f0: 6504 6a05 6506 6a07 6504 6a08 1900 6404  e.j.e.j.e.j...d.
-00000100: 6405 9c03 6406 6407 8404 5a09 6504 6a05  d...d.d...Z.e.j.
-00000110: 6504 6a08 650a 6405 9c03 6408 6409 8404  e.j.e.d...d.d...
-00000120: 5a0b 8700 0400 5a0c 5300 290b da0d 5a61  Z.....Z.S.)...Za
-00000130: 6262 6978 5472 6170 7065 72e9 3c00 0000  bbixTrapper.<...
-00000140: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000150: 0003 0000 0003 0000 0073 2600 0000 7400  .........s&...t.
-00000160: 8300 a001 a100 0100 7c01 7c00 5f02 7c02  ........|.|._.|.
-00000170: 7c00 5f03 7404 a005 7c02 a101 7c00 5f06  |._.t...|...|._.
-00000180: 6400 5300 2901 4e29 07da 0573 7570 6572  d.S.).N)...super
-00000190: da08 5f5f 696e 6974 5f5f da07 5f73 656e  ..__init__.._sen
-000001a0: 6465 72da 1b5f 636c 6965 6e74 5f64 6973  der.._client_dis
-000001b0: 636f 7665 7279 5f77 6169 745f 7469 6d65  covery_wait_time
-000001c0: da0d 6b6e 6f77 6e5f 636c 6965 6e74 735a  ..known_clientsZ
-000001d0: 0c4b 6e6f 776e 436c 6965 6e74 73da 0e5f  .KnownClients.._
-000001e0: 6b6e 6f77 6e5f 636c 6965 6e74 7329 03da  known_clients)..
-000001f0: 0473 656c 66da 0673 656e 6465 725a 1a63  .self..senderZ.c
-00000200: 6c69 656e 745f 6469 7363 6f76 6572 795f  lient_discovery_
-00000210: 7761 6974 5f74 696d 65a9 01da 095f 5f63  wait_time....__c
-00000220: 6c61 7373 5f5f a900 fa6a 2f68 6f6d 652f  lass__...j/home/
-00000230: 6d79 732f 446f 6375 6d65 6e74 732f 4769  mys/Documents/Gi
-00000240: 7448 7562 2f6d 6173 7464 692f 726f 7574  tHub/mastdi/rout
-00000250: 6572 2d6c 6f67 2d70 7265 7072 6f63 6573  er-log-preproces
-00000260: 736f 722f 726f 7574 6572 5f6c 6f67 5f70  sor/router_log_p
-00000270: 7265 7072 6f63 6573 736f 722f 686f 6f6b  reprocessor/hook
-00000280: 732f 7a61 6262 6978 2f5f 7472 6170 7065  s/zabbix/_trappe
-00000290: 722e 7079 7205 0000 001a 0000 0073 0800  r.pyr........s..
-000002a0: 0000 0001 0a01 0601 0601 7a16 5a61 6262  ..........z.Zabb
-000002b0: 6978 5472 6170 7065 722e 5f5f 696e 6974  ixTrapper.__init
-000002c0: 5f5f 4e29 03da 0672 6563 6f72 64da 076d  __N)...record..m
-000002d0: 6573 7361 6765 da06 7265 7475 726e 6303  essage..returnc.
-000002e0: 0000 0000 0000 0000 0000 0006 0000 0006  ................
-000002f0: 0000 00c3 0000 0073 8a00 0000 7c02 6401  .......s....|.d.
-00000300: 6b08 720c 6401 5300 7c00 a000 7c01 7c02  k.r.d.S.|...|.|.
-00000310: a102 4900 6401 4800 7d03 7c03 6402 6b04  ..I.d.H.}.|.d.k.
-00000320: 724c 7401 6a02 a003 6403 7c02 6a04 7c01  rLt.j...d.|.j.|.
-00000330: 6a05 7c03 a104 0100 7406 a007 7c03 a101  j.|.....t...|...
-00000340: 4900 6401 4800 0100 7408 a009 7c01 7c02  I.d.H...t...|.|.
-00000350: a102 7d04 7401 6a02 a00a 6404 7c04 a102  ..}.t.j...d.|...
-00000360: 0100 7c00 6a0b a00c 7c04 a101 4900 6401  ..|.j...|...I.d.
-00000370: 4800 7d05 7401 6a02 a00a 6405 7c05 a102  H.}.t.j...d.|...
-00000380: 0100 6401 5300 2906 61fe 0100 0053 656e  ..d.S.).a....Sen
-00000390: 6420 7468 6520 7072 6570 726f 6365 7373  d the preprocess
-000003a0: 6564 206d 6573 7361 6765 2074 6f20 7468  ed message to th
-000003b0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-000003c0: 5a61 6262 6978 2054 7261 7070 6572 2069  Zabbix Trapper i
-000003d0: 7465 6d28 7329 2e0a 0a20 2020 2020 2020  tem(s)...       
-000003e0: 2046 6f72 2063 6c69 656e 7420 6d65 7373   For client mess
-000003f0: 6167 6573 2061 206c 6f77 2d6c 6576 656c  ages a low-level
-00000400: 2064 6973 636f 7665 7279 2077 696c 6c20   discovery will 
-00000410: 6265 2073 656e 7420 6669 7273 7420 616e  be sent first an
-00000420: 6420 7468 650a 2020 2020 2020 2020 636f  d the.        co
-00000430: 7272 6573 706f 6e64 696e 6720 5a61 6262  rresponding Zabb
-00000440: 6978 2054 7261 7070 6572 2069 7465 6d28  ix Trapper item(
-00000450: 7329 2077 696c 6c20 6265 2064 656c 6179  s) will be delay
-00000460: 6564 2075 6e74 696c 205a 6162 6269 7820  ed until Zabbix 
-00000470: 6861 7665 2062 6565 6e0a 2020 2020 2020  have been.      
-00000480: 2020 6769 7665 6e20 7469 6d65 2074 6f20    given time to 
-00000490: 7379 6e63 6872 6f6e 697a 6520 6361 6368  synchronize cach
-000004a0: 6573 2e0a 0a20 2020 2020 2020 2049 6620  es...        If 
-000004b0: 7468 6520 6d65 7373 6167 6520 6973 204e  the message is N
-000004c0: 6f6e 652c 2074 6865 6e20 7468 6973 206d  one, then this m
-000004d0: 6574 686f 6420 7265 7475 726e 7320 696d  ethod returns im
-000004e0: 6d65 6469 6174 656c 792e 0a0a 2020 2020  mediately...    
-000004f0: 2020 2020 3a70 6172 616d 2072 6563 6f72      :param recor
-00000500: 643a 2054 6865 206c 6f67 2072 6563 6f72  d: The log recor
-00000510: 6420 636f 6e74 6169 6e69 6e67 2068 6f73  d containing hos
-00000520: 746e 616d 652c 2070 726f 6365 7373 206e  tname, process n
-00000530: 616d 6520 616e 6420 7469 6d65 7374 616d  ame and timestam
-00000540: 702e 0a20 2020 2020 2020 203a 7061 7261  p..        :para
-00000550: 6d20 6d65 7373 6167 653a 2054 6865 206d  m message: The m
-00000560: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
-00000570: 6720 7468 6520 6d61 6320 6164 6472 6573  g the mac addres
-00000580: 732e 0a20 2020 2020 2020 204e 7201 0000  s..        Nr...
-00000590: 007a 3750 656e 6469 6e67 2064 6973 636f  .z7Pending disco
-000005a0: 7665 7279 2065 7665 6e74 206f 6620 2573  very event of %s
-000005b0: 206f 6e20 2573 2e20 5761 6974 696e 6720   on %s. Waiting 
-000005c0: 2566 2073 6563 6f6e 6473 7a10 5365 6e64  %f secondsz.Send
-000005d0: 696e 6720 6461 7461 3a20 2572 fa0c 5265  ing data: %r..Re
-000005e0: 7370 6f6e 7365 3a20 2572 290d da0f 6469  sponse: %r)...di
-000005f0: 7363 6f76 6572 5f63 6c69 656e 74da 076c  scover_client..l
-00000600: 6f67 6769 6e67 da06 6c6f 6767 6572 da05  ogging..logger..
-00000610: 6465 6275 67da 0b6d 6163 5f61 6464 7265  debug..mac_addre
-00000620: 7373 da07 7072 6f63 6573 73da 0561 6e79  ss..process..any
-00000630: 696f da05 736c 6565 70da 066d 6170 7065  io..sleep..mappe
-00000640: 725a 126d 6170 5f63 6c69 656e 745f 6d65  rZ.map_client_me
-00000650: 7373 6167 65da 0469 6e66 6f72 0600 0000  ssage..infor....
-00000660: da04 7365 6e64 2906 720a 0000 0072 1000  ..send).r....r..
-00000670: 0000 7211 0000 005a 1873 6563 6f6e 6473  ..r....Z.seconds
-00000680: 5f75 6e74 696c 5f64 6973 636f 7665 7265  _until_discovere
-00000690: 64da 0c6d 6561 7375 7265 6d65 6e74 73da  d..measurements.
-000006a0: 0872 6573 706f 6e73 6572 0e00 0000 720e  .responser....r.
-000006b0: 0000 0072 0f00 0000 721e 0000 0020 0000  ...r....r.... ..
-000006c0: 0073 1e00 0000 000e 0801 0401 1201 0802  .s..............
-000006d0: 0601 0201 0401 0401 02fc 0406 1001 0c02  ................
-000006e0: 0e01 1201 7a12 5a61 6262 6978 5472 6170  ....z.ZabbixTrap
-000006f0: 7065 722e 7365 6e64 6303 0000 0000 0000  per.sendc.......
-00000700: 0000 0000 0005 0000 0004 0000 00c3 0000  ................
-00000710: 0073 9800 0000 7c01 6a00 6401 6b09 730e  .s....|.j.d.k.s.
-00000720: 7401 8201 7c00 6a02 a003 7c01 6a00 7c02  t...|.j...|.j.|.
-00000730: 6a04 a102 7232 7c00 6a02 a005 7c01 6a00  j...r2|.j...|.j.
-00000740: 7c02 6a04 a102 5300 7c00 6a02 a006 7c01  |.j...S.|.j...|.
-00000750: 6a00 7c02 6a04 a102 0100 7407 a008 7c01  j.|.j.....t...|.
-00000760: 7c00 6a02 a102 7d03 7409 6a0a a00b 6402  |.j...}.t.j...d.
-00000770: 7c03 a102 0100 7c00 6a0c a00d 7c03 a101  |.....|.j...|...
-00000780: 4900 6401 4800 7d04 7409 6a0a a00b 6403  I.d.H.}.t.j...d.
-00000790: 7c04 a102 0100 7c04 6a0e 6404 6b02 7392  |.....|.j.d.k.s.
-000007a0: 7401 7c04 8301 8201 7c00 6a0f 5300 2905  t.|.....|.j.S.).
-000007b0: 613a 0400 0044 6973 636f 7665 7220 6120  a:...Discover a 
-000007c0: 6e65 7720 636c 6965 6e74 2062 6173 6564  new client based
-000007d0: 206f 6e20 7468 6520 6d61 6320 6164 6472   on the mac addr
-000007e0: 6573 7320 696e 2074 6865 206d 6573 7361  ess in the messa
-000007f0: 6765 2e0a 0a20 2020 2020 2020 2054 6865  ge...        The
-00000800: 7265 2061 7265 2074 6872 6565 2063 6173  re are three cas
-00000810: 6573 206f 6620 636c 6965 6e74 2064 6973  es of client dis
-00000820: 636f 7665 7279 3a0a 2020 2020 2020 2020  covery:.        
-00000830: 3129 2054 6865 2063 6c69 656e 7420 6861  1) The client ha
-00000840: 7665 206e 6f74 2062 6565 6e20 6469 7363  ve not been disc
-00000850: 6f76 6572 6564 2062 6566 6f72 650a 2020  overed before.  
-00000860: 2020 2020 2020 3229 2054 6865 2063 6c69        2) The cli
-00000870: 656e 7420 6861 7665 2072 6563 656e 746c  ent have recentl
-00000880: 7920 6265 656e 2064 6973 636f 7665 7265  y been discovere
-00000890: 640a 2020 2020 2020 2020 3329 2054 6865  d.        3) The
-000008a0: 2063 6c69 656e 7420 6861 7665 2062 6565   client have bee
-000008b0: 6e20 6469 7363 6f76 6572 6564 2066 6f72  n discovered for
-000008c0: 2061 206c 6f6e 6720 7469 6d65 0a0a 2020   a long time..  
-000008d0: 2020 2020 2020 4120 6469 7363 6f76 6572        A discover
-000008e0: 7920 7061 636b 6574 2077 696c 6c20 6f6e  y packet will on
-000008f0: 6c79 2062 6520 7365 6e74 2074 6f20 5a61  ly be sent to Za
-00000900: 6262 6978 2069 6e20 7468 6520 6669 7273  bbix in the firs
-00000910: 7420 6361 7365 2061 6e64 2074 6865 2063  t case and the c
-00000920: 616c 6c65 650a 2020 2020 2020 2020 7769  allee.        wi
-00000930: 6c6c 2062 6520 696e 7374 7275 6374 6564  ll be instructed
-00000940: 2074 6f20 7761 6974 2066 6f72 2074 6865   to wait for the
-00000950: 2066 756c 6c20 6465 6661 756c 745f 7761   full default_wa
-00000960: 6974 5f74 696d 6520 7065 7269 6f64 2062  it_time period b
-00000970: 6566 6f72 6520 7365 6e64 696e 670a 2020  efore sending.  
-00000980: 2020 2020 2020 7468 6520 6163 7475 616c        the actual
-00000990: 2064 6174 6120 746f 205a 6162 6269 782e   data to Zabbix.
-000009a0: 2054 6869 7320 656e 7375 7265 7320 7468   This ensures th
-000009b0: 6174 2074 6865 205a 6162 6269 7820 5472  at the Zabbix Tr
-000009c0: 6170 7065 7220 7072 6f63 6573 7320 6973  apper process is
-000009d0: 2061 7761 7265 0a20 2020 2020 2020 206f   aware.        o
-000009e0: 6620 7468 6520 286e 6577 6c79 2063 7265  f the (newly cre
-000009f0: 6174 6564 2920 6974 656d 2070 726f 746f  ated) item proto
-00000a00: 7479 7065 2873 292e 0a0a 2020 2020 2020  type(s)...      
-00000a10: 2020 4966 2061 2063 6c69 656e 7420 6861    If a client ha
-00000a20: 7665 2072 6563 656e 746c 7920 6265 656e  ve recently been
-00000a30: 2064 6973 636f 7665 7265 6420 7468 6520   discovered the 
-00000a40: 6361 6c6c 6565 2077 696c 6c20 6265 2069  callee will be i
-00000a50: 6e73 7472 7563 7465 6420 746f 2077 6169  nstructed to wai
-00000a60: 740a 2020 2020 2020 2020 7468 6520 7265  t.        the re
-00000a70: 6d61 696e 696e 6720 7469 6d65 206f 6620  maining time of 
-00000a80: 7468 6520 6465 6661 756c 745f 7761 6974  the default_wait
-00000a90: 5f74 696d 6520 6265 666f 7265 2073 656e  _time before sen
-00000aa0: 6469 6e67 2074 6865 2061 6374 7561 6c20  ding the actual 
-00000ab0: 6461 7461 2074 6f0a 2020 2020 2020 2020  data to.        
-00000ac0: 5a61 6262 6978 2e0a 0a20 2020 2020 2020  Zabbix...       
-00000ad0: 2046 6f72 2074 6865 206c 6173 7420 6361   For the last ca
-00000ae0: 7365 2074 6865 2063 616c 6c65 6520 7769  se the callee wi
-00000af0: 6c6c 2062 6520 696e 7374 7275 6374 6564  ll be instructed
-00000b00: 2074 6f20 7761 6974 2030 2073 6563 6f6e   to wait 0 secon
-00000b10: 6473 2c20 692e 652e 2074 6865 7920 6361  ds, i.e. they ca
-00000b20: 6e0a 2020 2020 2020 2020 7365 6e64 2074  n.        send t
-00000b30: 6865 2064 6174 6120 746f 205a 6162 6269  he data to Zabbi
-00000b40: 7820 696d 6d65 6469 6174 656c 792e 0a0a  x immediately...
-00000b50: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-00000b60: 6563 6f72 643a 2054 6865 206c 6f67 2072  ecord: The log r
-00000b70: 6563 6f72 6420 636f 6e74 6169 6e69 6e67  ecord containing
-00000b80: 2068 6f73 746e 616d 652c 2070 726f 6365   hostname, proce
-00000b90: 7373 206e 616d 6520 616e 6420 7469 6d65  ss name and time
-00000ba0: 7374 616d 702e 0a20 2020 2020 2020 203a  stamp..        :
-00000bb0: 7061 7261 6d20 6d65 7373 6167 653a 2054  param message: T
-00000bc0: 6865 206d 6573 7361 6765 2063 6f6e 7461  he message conta
-00000bd0: 696e 696e 6720 7468 6520 6d61 6320 6164  ining the mac ad
-00000be0: 6472 6573 732e 0a20 2020 2020 2020 204e  dress..        N
-00000bf0: 7a0f 4469 7363 6f76 6572 696e 673a 2025  z.Discovering: %
-00000c00: 7272 1300 0000 e901 0000 0029 1072 1900  rr.........).r..
-00000c10: 0000 da0e 4173 7365 7274 696f 6e45 7272  ....AssertionErr
-00000c20: 6f72 7209 0000 005a 0f69 735f 636c 6965  orr....Z.is_clie
-00000c30: 6e74 5f6b 6e6f 776e 7218 0000 005a 1372  nt_knownr....Z.r
-00000c40: 656d 6169 6e69 6e67 5f77 6169 745f 7469  emaining_wait_ti
-00000c50: 6d65 5a0a 6164 645f 636c 6965 6e74 721c  meZ.add_clientr.
-00000c60: 0000 005a 146d 6170 5f63 6c69 656e 745f  ...Z.map_client_
-00000c70: 6469 7363 6f76 6572 7972 1500 0000 7216  discoveryr....r.
-00000c80: 0000 0072 1d00 0000 7206 0000 0072 1e00  ...r....r....r..
-00000c90: 0000 da09 7072 6f63 6573 7365 6472 0700  ....processedr..
-00000ca0: 0000 2905 720a 0000 0072 1000 0000 7211  ..).r....r....r.
-00000cb0: 0000 0072 1f00 0000 7220 0000 0072 0e00  ...r....r ...r..
-00000cc0: 0000 720e 0000 0072 0f00 0000 7214 0000  ..r....r....r...
-00000cd0: 0040 0000 0073 1a00 0000 0019 0e01 1203  .@...s..........
-00000ce0: 0601 0400 04ff 0404 1202 0e02 0e01 1201  ................
-00000cf0: 0e01 1201 7a1d 5a61 6262 6978 5472 6170  ....z.ZabbixTrap
-00000d00: 7065 722e 6469 7363 6f76 6572 5f63 6c69  per.discover_cli
-00000d10: 656e 7429 0172 0300 0000 290d da08 5f5f  ent).r....)...__
-00000d20: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000d30: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000d40: 7205 0000 00da 0664 6f6d 6169 6eda 094c  r......domain..L
-00000d50: 6f67 5265 636f 7264 da06 7479 7069 6e67  ogRecord..typing
-00000d60: da08 4f70 7469 6f6e 616c da07 4d65 7373  ..Optional..Mess
-00000d70: 6167 6572 1e00 0000 da05 666c 6f61 7472  ager......floatr
-00000d80: 1400 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00000d90: 6c5f 5f72 0e00 0000 720e 0000 0072 0c00  l__r....r....r..
-00000da0: 0000 720f 0000 0072 0200 0000 1900 0000  ..r....r........
-00000db0: 7312 0000 0008 010e 0704 000a 0102 fe0c  s...............
-00000dc0: 2104 0004 0102 fe72 0200 0000 2913 7229  !......r....).r)
-00000dd0: 0000 0072 1a00 0000 5a1e 726f 7574 6572  ...r....Z.router
-00000de0: 5f6c 6f67 5f70 7265 7072 6f63 6573 736f  _log_preprocesso
-00000df0: 722e 646f 6d61 696e 7227 0000 005a 2172  r.domainr'...Z!r
-00000e00: 6f75 7465 725f 6c6f 675f 7072 6570 726f  outer_log_prepro
-00000e10: 6365 7373 6f72 2e68 6f6f 6b73 2e61 6263  cessor.hooks.abc
-00000e20: da05 686f 6f6b 73da 0361 6263 5a33 726f  ..hooks..abcZ3ro
-00000e30: 7574 6572 5f6c 6f67 5f70 7265 7072 6f63  uter_log_preproc
-00000e40: 6573 736f 722e 686f 6f6b 732e 7a61 6262  essor.hooks.zabb
-00000e50: 6978 2e5f 6b6e 6f77 6e5f 636c 6965 6e74  ix._known_client
-00000e60: 73da 067a 6162 6269 7872 0900 0000 7208  s..zabbixr....r.
-00000e70: 0000 005a 2c72 6f75 7465 725f 6c6f 675f  ...Z,router_log_
-00000e80: 7072 6570 726f 6365 7373 6f72 2e68 6f6f  preprocessor.hoo
-00000e90: 6b73 2e7a 6162 6269 782e 5f6d 6170 7065  ks.zabbix._mappe
-00000ea0: 725a 075f 6d61 7070 6572 721c 0000 00da  rZ._mapperr.....
-00000eb0: 2472 6f75 7465 725f 6c6f 675f 7072 6570  $router_log_prep
-00000ec0: 726f 6365 7373 6f72 2e75 7469 6c2e 6c6f  rocessor.util.lo
-00000ed0: 6767 696e 67da 0475 7469 6c72 1500 0000  gging..utilr....
-00000ee0: 5a04 486f 6f6b 7202 0000 0072 0e00 0000  Z.Hookr....r....
-00000ef0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000f00: 083c 6d6f 6475 6c65 3e0e 0000 0073 0e00  .<module>....s..
-00000f10: 0000 0802 0802 0c01 1201 1801 1801 1203  ................
+00000040: 6401 6c02 5a02 6400 6401 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6400 6401 6c05 6d06 0200 0100 6d07  ..d.d.l.m.....m.
+00000060: 5a07 0100 6400 6401 6c08 6d06 0200 0100  Z...d.d.l.m.....
+00000070: 6d09 0200 0100 6d0a 5a0b 0100 6400 6401  m.....m.Z...d.d.
+00000080: 6c0c 6d06 0200 0100 6d09 0200 0100 6d0d  l.m.....m.....m.
+00000090: 5a0e 0100 6400 6401 6c0f 6d10 0200 0100  Z...d.d.l.m.....
+000000a0: 6d11 5a11 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+000000b0: 6507 6a12 8303 5a13 6401 5300 2904 e900  e.j...Z.d.S.)...
+000000c0: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
+000000d0: 0000 0000 0004 0000 0000 0000 0073 5000  .............sP.
+000000e0: 0000 6500 5a01 6400 5a02 640b 8700 6601  ..e.Z.d.Z.d...f.
+000000f0: 6403 6404 8409 5a03 6504 6a05 6506 6a07  d.d...Z.e.j.e.j.
+00000100: 6504 6a08 1900 6405 6406 9c03 6407 6408  e.j...d.d...d.d.
+00000110: 8404 5a09 6504 6a05 6504 6a08 650a 6406  ..Z.e.j.e.j.e.d.
+00000120: 9c03 6409 640a 8404 5a0b 8700 0400 5a0c  ..d.d...Z.....Z.
+00000130: 5300 290c da0d 5a61 6262 6978 5472 6170  S.)...ZabbixTrap
+00000140: 7065 72e9 3200 0000 e90a 0000 0063 0400  per.2........c..
+00000150: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+00000160: 0000 0300 0000 733c 0000 0074 0083 00a0  ......s<...t....
+00000170: 01a1 0001 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
+00000180: 0374 04a0 057c 02a1 017c 005f 067c 037c  .t...|...|._.|.|
+00000190: 005f 0764 017c 005f 0874 09a0 0aa1 007c  ._.d.|._.t.....|
+000001a0: 005f 0b64 0053 0029 024e 4629 0cda 0573  ._.d.S.).NF)...s
+000001b0: 7570 6572 da08 5f5f 696e 6974 5f5f da07  uper..__init__..
+000001c0: 5f73 656e 6465 72da 1b5f 636c 6965 6e74  _sender.._client
+000001d0: 5f64 6973 636f 7665 7279 5f77 6169 745f  _discovery_wait_
+000001e0: 7469 6d65 da0d 6b6e 6f77 6e5f 636c 6965  time..known_clie
+000001f0: 6e74 735a 0c4b 6e6f 776e 436c 6965 6e74  ntsZ.KnownClient
+00000200: 73da 0e5f 6b6e 6f77 6e5f 636c 6965 6e74  s.._known_client
+00000210: 73da 1d5f 6d65 6173 7572 656d 656e 745f  s.._measurement_
+00000220: 6275 6e64 6c65 5f77 6169 745f 7469 6d65  bundle_wait_time
+00000230: da19 5f69 735f 6275 6e64 6c69 6e67 5f6d  .._is_bundling_m
+00000240: 6561 7375 7265 6d65 6e74 73da 1561 7379  easurements..asy
+00000250: 6e63 696f 5f7a 6162 6269 785f 7365 6e64  ncio_zabbix_send
+00000260: 6572 da0c 4d65 6173 7572 656d 656e 7473  er..Measurements
+00000270: da0d 5f6d 6561 7375 7265 6d65 6e74 7329  .._measurements)
+00000280: 04da 0473 656c 66da 0673 656e 6465 725a  ...self..senderZ
+00000290: 1a63 6c69 656e 745f 6469 7363 6f76 6572  .client_discover
+000002a0: 795f 7761 6974 5f74 696d 655a 1c6d 6561  y_wait_timeZ.mea
+000002b0: 7375 7265 6d65 6e74 5f62 756e 646c 655f  surement_bundle_
+000002c0: 7761 6974 5f74 696d 65a9 01da 095f 5f63  wait_time....__c
+000002d0: 6c61 7373 5f5f a900 fa6a 2f68 6f6d 652f  lass__...j/home/
+000002e0: 6d79 732f 446f 6375 6d65 6e74 732f 4769  mys/Documents/Gi
+000002f0: 7448 7562 2f6d 6173 7464 692f 726f 7574  tHub/mastdi/rout
+00000300: 6572 2d6c 6f67 2d70 7265 7072 6f63 6573  er-log-preproces
+00000310: 736f 722f 726f 7574 6572 5f6c 6f67 5f70  sor/router_log_p
+00000320: 7265 7072 6f63 6573 736f 722f 686f 6f6b  reprocessor/hook
+00000330: 732f 7a61 6262 6978 2f5f 7472 6170 7065  s/zabbix/_trappe
+00000340: 722e 7079 7206 0000 001b 0000 0073 0e00  r.pyr........s..
+00000350: 0000 0003 0a01 0601 0601 0c01 0601 0601  ................
+00000360: 7a16 5a61 6262 6978 5472 6170 7065 722e  z.ZabbixTrapper.
+00000370: 5f5f 696e 6974 5f5f 4e29 03da 0672 6563  __init__N)...rec
+00000380: 6f72 64da 076d 6573 7361 6765 da06 7265  ord..message..re
+00000390: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
+000003a0: 0007 0000 0006 0000 00c3 0000 0073 d400  .............s..
+000003b0: 0000 7c02 6401 6b08 720c 6401 5300 7c00  ..|.d.k.r.d.S.|.
+000003c0: a000 7c01 7c02 a102 4900 6401 4800 7d03  ..|.|...I.d.H.}.
+000003d0: 7c03 6402 6b04 724c 7401 6a02 a003 6403  |.d.k.rLt.j...d.
+000003e0: 7c02 6a04 7c01 6a05 7c03 a104 0100 7406  |.j.|.j.|.....t.
+000003f0: a007 7c03 a101 4900 6401 4800 0100 7408  ..|...I.d.H...t.
+00000400: a009 7c01 7c02 a102 4400 5d10 7d04 7c00  ..|.|...D.].}.|.
+00000410: 6a0a a00b 7c04 a101 0100 7158 7c00 6a0c  j...|.....qX|.j.
+00000420: 7274 6401 5300 6404 7c00 5f0c 7406 a007  rtd.S.d.|._.t...
+00000430: 7c00 6a0d a101 4900 6401 4800 0100 6405  |.j...I.d.H...d.
+00000440: 7c00 5f0c 7c00 6a0a 7d05 740e a00f a100  |._.|.j.}.t.....
+00000450: 7c00 5f0a 7401 6a02 a010 6406 7c05 a102  |._.t.j...d.|...
+00000460: 0100 7c00 6a11 a012 7c05 a101 4900 6401  ..|.j...|...I.d.
+00000470: 4800 7d06 7401 6a02 a010 6407 7c06 a102  H.}.t.j...d.|...
+00000480: 0100 6401 5300 2908 61fe 0100 0053 656e  ..d.S.).a....Sen
+00000490: 6420 7468 6520 7072 6570 726f 6365 7373  d the preprocess
+000004a0: 6564 206d 6573 7361 6765 2074 6f20 7468  ed message to th
+000004b0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+000004c0: 5a61 6262 6978 2054 7261 7070 6572 2069  Zabbix Trapper i
+000004d0: 7465 6d28 7329 2e0a 0a20 2020 2020 2020  tem(s)...       
+000004e0: 2046 6f72 2063 6c69 656e 7420 6d65 7373   For client mess
+000004f0: 6167 6573 2061 206c 6f77 2d6c 6576 656c  ages a low-level
+00000500: 2064 6973 636f 7665 7279 2077 696c 6c20   discovery will 
+00000510: 6265 2073 656e 7420 6669 7273 7420 616e  be sent first an
+00000520: 6420 7468 650a 2020 2020 2020 2020 636f  d the.        co
+00000530: 7272 6573 706f 6e64 696e 6720 5a61 6262  rresponding Zabb
+00000540: 6978 2054 7261 7070 6572 2069 7465 6d28  ix Trapper item(
+00000550: 7329 2077 696c 6c20 6265 2064 656c 6179  s) will be delay
+00000560: 6564 2075 6e74 696c 205a 6162 6269 7820  ed until Zabbix 
+00000570: 6861 7665 2062 6565 6e0a 2020 2020 2020  have been.      
+00000580: 2020 6769 7665 6e20 7469 6d65 2074 6f20    given time to 
+00000590: 7379 6e63 6872 6f6e 697a 6520 6361 6368  synchronize cach
+000005a0: 6573 2e0a 0a20 2020 2020 2020 2049 6620  es...        If 
+000005b0: 7468 6520 6d65 7373 6167 6520 6973 204e  the message is N
+000005c0: 6f6e 652c 2074 6865 6e20 7468 6973 206d  one, then this m
+000005d0: 6574 686f 6420 7265 7475 726e 7320 696d  ethod returns im
+000005e0: 6d65 6469 6174 656c 792e 0a0a 2020 2020  mediately...    
+000005f0: 2020 2020 3a70 6172 616d 2072 6563 6f72      :param recor
+00000600: 643a 2054 6865 206c 6f67 2072 6563 6f72  d: The log recor
+00000610: 6420 636f 6e74 6169 6e69 6e67 2068 6f73  d containing hos
+00000620: 746e 616d 652c 2070 726f 6365 7373 206e  tname, process n
+00000630: 616d 6520 616e 6420 7469 6d65 7374 616d  ame and timestam
+00000640: 702e 0a20 2020 2020 2020 203a 7061 7261  p..        :para
+00000650: 6d20 6d65 7373 6167 653a 2054 6865 206d  m message: The m
+00000660: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
+00000670: 6720 7468 6520 6d61 6320 6164 6472 6573  g the mac addres
+00000680: 732e 0a20 2020 2020 2020 204e 7201 0000  s..        Nr...
+00000690: 007a 3750 656e 6469 6e67 2064 6973 636f  .z7Pending disco
+000006a0: 7665 7279 2065 7665 6e74 206f 6620 2573  very event of %s
+000006b0: 206f 6e20 2573 2e20 5761 6974 696e 6720   on %s. Waiting 
+000006c0: 2566 2073 6563 6f6e 6473 5446 7a10 5365  %f secondsTFz.Se
+000006d0: 6e64 696e 6720 6461 7461 3a20 2572 fa0c  nding data: %r..
+000006e0: 5265 7370 6f6e 7365 3a20 2572 2913 da0f  Response: %r)...
+000006f0: 6469 7363 6f76 6572 5f63 6c69 656e 74da  discover_client.
+00000700: 076c 6f67 6769 6e67 da06 6c6f 6767 6572  .logging..logger
+00000710: da05 6465 6275 67da 0b6d 6163 5f61 6464  ..debug..mac_add
+00000720: 7265 7373 da07 7072 6f63 6573 73da 0561  ress..process..a
+00000730: 6e79 696f da05 736c 6565 70da 066d 6170  nyio..sleep..map
+00000740: 7065 725a 126d 6170 5f63 6c69 656e 745f  perZ.map_client_
+00000750: 6d65 7373 6167 6572 0f00 0000 da0f 6164  messager......ad
+00000760: 645f 6d65 6173 7572 656d 656e 7472 0c00  d_measurementr..
+00000770: 0000 720b 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000780: 00da 0469 6e66 6f72 0700 0000 da04 7365  ...infor......se
+00000790: 6e64 2907 7210 0000 0072 1600 0000 7217  nd).r....r....r.
+000007a0: 0000 005a 1873 6563 6f6e 6473 5f75 6e74  ...Z.seconds_unt
+000007b0: 696c 5f64 6973 636f 7665 7265 64da 0b6d  il_discovered..m
+000007c0: 6561 7375 7265 6d65 6e74 da0c 6d65 6173  easurement..meas
+000007d0: 7572 656d 656e 7473 da08 7265 7370 6f6e  urements..respon
+000007e0: 7365 7214 0000 0072 1400 0000 7215 0000  ser....r....r...
+000007f0: 0072 2500 0000 2600 0000 732e 0000 0000  .r%...&...s.....
+00000800: 0e08 0104 0112 0108 0206 0102 0104 0104  ................
+00000810: 0102 fc04 0610 0210 010e 0206 0304 0306  ................
+00000820: 0112 0506 0106 010a 020e 0112 017a 125a  .............z.Z
+00000830: 6162 6269 7854 7261 7070 6572 2e73 656e  abbixTrapper.sen
+00000840: 6463 0300 0000 0000 0000 0000 0000 0500  dc..............
+00000850: 0000 0400 0000 c300 0000 7398 0000 007c  ..........s....|
+00000860: 016a 0064 016b 0973 0e74 0182 017c 006a  .j.d.k.s.t...|.j
+00000870: 02a0 037c 016a 007c 026a 04a1 0272 327c  ...|.j.|.j...r2|
+00000880: 006a 02a0 057c 016a 007c 026a 04a1 0253  .j...|.j.|.j...S
+00000890: 007c 006a 02a0 067c 016a 007c 026a 04a1  .|.j...|.j.|.j..
+000008a0: 0201 0074 07a0 087c 017c 006a 02a1 027d  ...t...|.|.j...}
+000008b0: 0374 096a 0aa0 0b64 027c 03a1 0201 007c  .t.j...d.|.....|
+000008c0: 006a 0ca0 0d7c 03a1 0149 0064 0148 007d  .j...|...I.d.H.}
+000008d0: 0474 096a 0aa0 0b64 037c 04a1 0201 007c  .t.j...d.|.....|
+000008e0: 046a 0e64 046b 0273 9274 017c 0483 0182  .j.d.k.s.t.|....
+000008f0: 017c 006a 0f53 0029 0561 3a04 0000 4469  .|.j.S.).a:...Di
+00000900: 7363 6f76 6572 2061 206e 6577 2063 6c69  scover a new cli
+00000910: 656e 7420 6261 7365 6420 6f6e 2074 6865  ent based on the
+00000920: 206d 6163 2061 6464 7265 7373 2069 6e20   mac address in 
+00000930: 7468 6520 6d65 7373 6167 652e 0a0a 2020  the message...  
+00000940: 2020 2020 2020 5468 6572 6520 6172 6520        There are 
+00000950: 7468 7265 6520 6361 7365 7320 6f66 2063  three cases of c
+00000960: 6c69 656e 7420 6469 7363 6f76 6572 793a  lient discovery:
+00000970: 0a20 2020 2020 2020 2031 2920 5468 6520  .        1) The 
+00000980: 636c 6965 6e74 2068 6176 6520 6e6f 7420  client have not 
+00000990: 6265 656e 2064 6973 636f 7665 7265 6420  been discovered 
+000009a0: 6265 666f 7265 0a20 2020 2020 2020 2032  before.        2
+000009b0: 2920 5468 6520 636c 6965 6e74 2068 6176  ) The client hav
+000009c0: 6520 7265 6365 6e74 6c79 2062 6565 6e20  e recently been 
+000009d0: 6469 7363 6f76 6572 6564 0a20 2020 2020  discovered.     
+000009e0: 2020 2033 2920 5468 6520 636c 6965 6e74     3) The client
+000009f0: 2068 6176 6520 6265 656e 2064 6973 636f   have been disco
+00000a00: 7665 7265 6420 666f 7220 6120 6c6f 6e67  vered for a long
+00000a10: 2074 696d 650a 0a20 2020 2020 2020 2041   time..        A
+00000a20: 2064 6973 636f 7665 7279 2070 6163 6b65   discovery packe
+00000a30: 7420 7769 6c6c 206f 6e6c 7920 6265 2073  t will only be s
+00000a40: 656e 7420 746f 205a 6162 6269 7820 696e  ent to Zabbix in
+00000a50: 2074 6865 2066 6972 7374 2063 6173 6520   the first case 
+00000a60: 616e 6420 7468 6520 6361 6c6c 6565 0a20  and the callee. 
+00000a70: 2020 2020 2020 2077 696c 6c20 6265 2069         will be i
+00000a80: 6e73 7472 7563 7465 6420 746f 2077 6169  nstructed to wai
+00000a90: 7420 666f 7220 7468 6520 6675 6c6c 2064  t for the full d
+00000aa0: 6566 6175 6c74 5f77 6169 745f 7469 6d65  efault_wait_time
+00000ab0: 2070 6572 696f 6420 6265 666f 7265 2073   period before s
+00000ac0: 656e 6469 6e67 0a20 2020 2020 2020 2074  ending.        t
+00000ad0: 6865 2061 6374 7561 6c20 6461 7461 2074  he actual data t
+00000ae0: 6f20 5a61 6262 6978 2e20 5468 6973 2065  o Zabbix. This e
+00000af0: 6e73 7572 6573 2074 6861 7420 7468 6520  nsures that the 
+00000b00: 5a61 6262 6978 2054 7261 7070 6572 2070  Zabbix Trapper p
+00000b10: 726f 6365 7373 2069 7320 6177 6172 650a  rocess is aware.
+00000b20: 2020 2020 2020 2020 6f66 2074 6865 2028          of the (
+00000b30: 6e65 776c 7920 6372 6561 7465 6429 2069  newly created) i
+00000b40: 7465 6d20 7072 6f74 6f74 7970 6528 7329  tem prototype(s)
+00000b50: 2e0a 0a20 2020 2020 2020 2049 6620 6120  ...        If a 
+00000b60: 636c 6965 6e74 2068 6176 6520 7265 6365  client have rece
+00000b70: 6e74 6c79 2062 6565 6e20 6469 7363 6f76  ntly been discov
+00000b80: 6572 6564 2074 6865 2063 616c 6c65 6520  ered the callee 
+00000b90: 7769 6c6c 2062 6520 696e 7374 7275 6374  will be instruct
+00000ba0: 6564 2074 6f20 7761 6974 0a20 2020 2020  ed to wait.     
+00000bb0: 2020 2074 6865 2072 656d 6169 6e69 6e67     the remaining
+00000bc0: 2074 696d 6520 6f66 2074 6865 2064 6566   time of the def
+00000bd0: 6175 6c74 5f77 6169 745f 7469 6d65 2062  ault_wait_time b
+00000be0: 6566 6f72 6520 7365 6e64 696e 6720 7468  efore sending th
+00000bf0: 6520 6163 7475 616c 2064 6174 6120 746f  e actual data to
+00000c00: 0a20 2020 2020 2020 205a 6162 6269 782e  .        Zabbix.
+00000c10: 0a0a 2020 2020 2020 2020 466f 7220 7468  ..        For th
+00000c20: 6520 6c61 7374 2063 6173 6520 7468 6520  e last case the 
+00000c30: 6361 6c6c 6565 2077 696c 6c20 6265 2069  callee will be i
+00000c40: 6e73 7472 7563 7465 6420 746f 2077 6169  nstructed to wai
+00000c50: 7420 3020 7365 636f 6e64 732c 2069 2e65  t 0 seconds, i.e
+00000c60: 2e20 7468 6579 2063 616e 0a20 2020 2020  . they can.     
+00000c70: 2020 2073 656e 6420 7468 6520 6461 7461     send the data
+00000c80: 2074 6f20 5a61 6262 6978 2069 6d6d 6564   to Zabbix immed
+00000c90: 6961 7465 6c79 2e0a 0a20 2020 2020 2020  iately...       
+00000ca0: 203a 7061 7261 6d20 7265 636f 7264 3a20   :param record: 
+00000cb0: 5468 6520 6c6f 6720 7265 636f 7264 2063  The log record c
+00000cc0: 6f6e 7461 696e 696e 6720 686f 7374 6e61  ontaining hostna
+00000cd0: 6d65 2c20 7072 6f63 6573 7320 6e61 6d65  me, process name
+00000ce0: 2061 6e64 2074 696d 6573 7461 6d70 2e0a   and timestamp..
+00000cf0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
+00000d00: 6573 7361 6765 3a20 5468 6520 6d65 7373  essage: The mess
+00000d10: 6167 6520 636f 6e74 6169 6e69 6e67 2074  age containing t
+00000d20: 6865 206d 6163 2061 6464 7265 7373 2e0a  he mac address..
+00000d30: 2020 2020 2020 2020 4e7a 0f44 6973 636f          Nz.Disco
+00000d40: 7665 7269 6e67 3a20 2572 7219 0000 00e9  vering: %rr.....
+00000d50: 0100 0000 2910 721f 0000 00da 0e41 7373  ....).r......Ass
+00000d60: 6572 7469 6f6e 4572 726f 7272 0a00 0000  ertionErrorr....
+00000d70: 5a0f 6973 5f63 6c69 656e 745f 6b6e 6f77  Z.is_client_know
+00000d80: 6e72 1e00 0000 5a13 7265 6d61 696e 696e  nr....Z.remainin
+00000d90: 675f 7761 6974 5f74 696d 655a 0a61 6464  g_wait_timeZ.add
+00000da0: 5f63 6c69 656e 7472 2200 0000 5a14 6d61  _clientr"...Z.ma
+00000db0: 705f 636c 6965 6e74 5f64 6973 636f 7665  p_client_discove
+00000dc0: 7279 721b 0000 0072 1c00 0000 7224 0000  ryr....r....r$..
+00000dd0: 0072 0700 0000 7225 0000 00da 0970 726f  .r....r%.....pro
+00000de0: 6365 7373 6564 7208 0000 0029 0572 1000  cessedr....).r..
+00000df0: 0000 7216 0000 0072 1700 0000 7227 0000  ..r....r....r'..
+00000e00: 0072 2800 0000 7214 0000 0072 1400 0000  .r(...r....r....
+00000e10: 7215 0000 0072 1a00 0000 5800 0000 731a  r....r....X...s.
+00000e20: 0000 0000 190e 0112 0306 0104 0004 ff04  ................
+00000e30: 0412 020e 020e 0112 010e 0112 017a 1d5a  .............z.Z
+00000e40: 6162 6269 7854 7261 7070 6572 2e64 6973  abbixTrapper.dis
+00000e50: 636f 7665 725f 636c 6965 6e74 2902 7203  cover_client).r.
+00000e60: 0000 0072 0400 0000 290d da08 5f5f 6e61  ...r....)...__na
+00000e70: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000e80: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
+00000e90: 0000 00da 0664 6f6d 6169 6eda 094c 6f67  .....domain..Log
+00000ea0: 5265 636f 7264 da06 7479 7069 6e67 da08  Record..typing..
+00000eb0: 4f70 7469 6f6e 616c da07 4d65 7373 6167  Optional..Messag
+00000ec0: 6572 2500 0000 da05 666c 6f61 7472 1a00  er%.....floatr..
+00000ed0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+00000ee0: 5f72 1400 0000 7214 0000 0072 1200 0000  _r....r....r....
+00000ef0: 7215 0000 0072 0200 0000 1a00 0000 7316  r....r........s.
+00000f00: 0000 0008 0200 0000 ff0e 0c04 000a 0102  ................
+00000f10: fe0c 3304 0004 0102 fe72 0200 0000 2914  ..3......r....).
+00000f20: 7231 0000 0072 2000 0000 720d 0000 005a  r1...r ...r....Z
+00000f30: 1e72 6f75 7465 725f 6c6f 675f 7072 6570  .router_log_prep
+00000f40: 726f 6365 7373 6f72 2e64 6f6d 6169 6e72  rocessor.domainr
+00000f50: 2f00 0000 5a21 726f 7574 6572 5f6c 6f67  /...Z!router_log
+00000f60: 5f70 7265 7072 6f63 6573 736f 722e 686f  _preprocessor.ho
+00000f70: 6f6b 732e 6162 63da 0568 6f6f 6b73 da03  oks.abc..hooks..
+00000f80: 6162 635a 3372 6f75 7465 725f 6c6f 675f  abcZ3router_log_
+00000f90: 7072 6570 726f 6365 7373 6f72 2e68 6f6f  preprocessor.hoo
+00000fa0: 6b73 2e7a 6162 6269 782e 5f6b 6e6f 776e  ks.zabbix._known
+00000fb0: 5f63 6c69 656e 7473 da06 7a61 6262 6978  _clients..zabbix
+00000fc0: 720a 0000 0072 0900 0000 5a2c 726f 7574  r....r....Z,rout
+00000fd0: 6572 5f6c 6f67 5f70 7265 7072 6f63 6573  er_log_preproces
+00000fe0: 736f 722e 686f 6f6b 732e 7a61 6262 6978  sor.hooks.zabbix
+00000ff0: 2e5f 6d61 7070 6572 5a07 5f6d 6170 7065  ._mapperZ._mappe
+00001000: 7272 2200 0000 da24 726f 7574 6572 5f6c  rr"....$router_l
+00001010: 6f67 5f70 7265 7072 6f63 6573 736f 722e  og_preprocessor.
+00001020: 7574 696c 2e6c 6f67 6769 6e67 da04 7574  util.logging..ut
+00001030: 696c 721b 0000 005a 0448 6f6f 6b72 0200  ilr....Z.Hookr..
+00001040: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00001050: 0072 1500 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001060: 0e00 0000 7310 0000 0008 0208 0108 020c  ....s...........
+00001070: 0112 0118 0118 0112 03                   .........
```

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/_known_clients.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_known_clients.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/hooks/zabbix/_mapper.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_mapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,42 +21,42 @@
 
 import router_log_preprocessor.domain as domain
 import router_log_preprocessor.hooks.zabbix._known_clients as _known_clients
 
 
 def map_client_message(
     record: domain.LogRecord, message: domain.Message
-) -> asyncio_zabbix_sender.Measurements:
+) -> typing.Generator[asyncio_zabbix_sender.Measurement, None, None]:
     assert record.process is not None
 
     # Ensure process is formatted according to Zabbix recommendations
     process = record.process.lower().replace("-", "_")
     # Convert record datetime to timestamp in full seconds
     clock = int(record.timestamp.timestamp())
+    ns = None
+    if isinstance(message, domain.WlcEventModel):
+        ns = message.event.value * 1000000
 
-    # Construct the measurements from the model
-    measurements = asyncio_zabbix_sender.Measurements()
+    # Generate the measurements from the model
     model_fields = dataclasses.fields(message)
     for field in model_fields:
         if field.name == "mac_address":
             continue
         value = getattr(message, field.name)
         if isinstance(value, enum.Enum):
             value = value.value
         elif isinstance(value, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
             value = str(value)
-        measurements.add_measurement(
-            asyncio_zabbix_sender.Measurement(
-                host=record.hostname,
-                key=f"rlp.{process}[{field.name},{message.mac_address}]",
-                value=value,
-                clock=clock,
-            )
+        yield asyncio_zabbix_sender.Measurement(
+            host=record.hostname,
+            key=f"rlp.{process}[{field.name},{message.mac_address}]",
+            value=value,
+            clock=clock,
+            ns=ns,
         )
-    return measurements
 
 
 def map_client_discovery(
     record: domain.LogRecord, known_clients: _known_clients.KnownClients
 ) -> asyncio_zabbix_sender.Measurements:
     assert record.process is not None
     value = json.dumps(
```

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/handler.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/handler.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/log_server/server.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/server.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/typing.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/typing.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/preprocessors/wlc.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/settings.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         description="A IP address or DNS name of the Zabbix instance.",
     )
     zabbix_port: int = Field(
         default=10051,
         description="The port used in the Zabbix instance.",
     )
 
+    class Config:
+        env_file = '.env', '.env.dev', '.env.test', '.env.staging', '.env.prod'
+        env_file_encoding = 'utf-8'
+
 
 @lru_cache
 def settings() -> Settings:
     """Get the settings of the applications.
     :return:
     """
     return Settings()
```

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/util/__init__.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc` & `router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/util/logging.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/util/logging.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.1/router_log_preprocessor/util/rfc3164_parser.py` & `router_log_preprocessor-0.1.2/router_log_preprocessor/util/rfc3164_parser.py`

 * *Files identical despite different names*

