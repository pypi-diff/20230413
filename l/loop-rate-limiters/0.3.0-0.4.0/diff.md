# Comparing `tmp/loop-rate-limiters-0.3.0.tar.gz` & `tmp/loop-rate-limiters-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loop-rate-limiters-0.3.0.tar", last modified: Fri Jan 20 14:31:25 2023, max compression
+gzip compressed data, was "loop-rate-limiters-0.4.0.tar", last modified: Thu Apr 13 18:18:58 2023, max compression
```

## Comparing `loop-rate-limiters-0.3.0.tar` & `loop-rate-limiters-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2662 2023-01-20 14:30:45.658299 loop-rate-limiters-0.3.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       39 2023-01-17 15:33:40.872366 loop-rate-limiters-0.3.0/.gitignore
--rw-r--r--   0        0        0      496 2023-01-20 14:31:02.456536 loop-rate-limiters-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-01-17 15:33:40.872366 loop-rate-limiters-0.3.0/LICENSE
--rw-r--r--   0        0        0     1702 2023-01-20 14:30:45.658299 loop-rate-limiters-0.3.0/README.md
--rw-r--r--   0        0        0      824 2023-01-20 14:31:13.689153 loop-rate-limiters-0.3.0/loop_rate_limiters/__init__.py
--rw-r--r--   0        0        0     4732 2023-01-20 14:30:45.658299 loop-rate-limiters-0.3.0/loop_rate_limiters/async_rate_limiter.py
--rw-r--r--   0        0        0     2688 2023-01-20 14:30:45.658299 loop-rate-limiters-0.3.0/loop_rate_limiters/rate_limiter.py
--rw-r--r--   0        0        0     1491 2023-01-20 14:30:45.658299 loop-rate-limiters-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      699 2023-01-17 15:33:40.876365 loop-rate-limiters-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2096 2023-01-17 15:33:40.876365 loop-rate-limiters-0.3.0/tests/test_async_rate.py
--rw-r--r--   0        0        0     1902 2023-01-20 14:30:45.658299 loop-rate-limiters-0.3.0/tests/test_rate_limiter.py
--rw-r--r--   0        0        0      632 2023-01-20 14:30:45.662299 loop-rate-limiters-0.3.0/tox.ini
--rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 loop-rate-limiters-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2662 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       39 2023-01-17 15:33:40.872366 loop-rate-limiters-0.4.0/.gitignore
+-rw-r--r--   0        0        0      586 2023-04-13 18:18:15.934034 loop-rate-limiters-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-01-17 15:33:40.872366 loop-rate-limiters-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1702 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/README.md
+-rw-r--r--   0        0        0      824 2023-04-13 18:14:28.520187 loop-rate-limiters-0.4.0/loop_rate_limiters/__init__.py
+-rw-r--r--   0        0        0     4732 2023-04-13 18:13:51.023598 loop-rate-limiters-0.4.0/loop_rate_limiters/async_rate_limiter.py
+-rw-r--r--   0        0        0     3017 2023-04-13 18:14:19.952092 loop-rate-limiters-0.4.0/loop_rate_limiters/rate_limiter.py
+-rw-r--r--   0        0        0     1491 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      699 2023-01-17 15:33:40.876365 loop-rate-limiters-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2096 2023-01-17 15:33:40.876365 loop-rate-limiters-0.4.0/tests/test_async_rate.py
+-rw-r--r--   0        0        0     1902 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/tests/test_rate_limiter.py
+-rw-r--r--   0        0        0      632 2023-01-20 14:30:45.662299 loop-rate-limiters-0.4.0/tox.ini
+-rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 loop-rate-limiters-0.4.0/PKG-INFO
```

### Comparing `loop-rate-limiters-0.3.0/.github/workflows/main.yml` & `loop-rate-limiters-0.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/LICENSE` & `loop-rate-limiters-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/README.md` & `loop-rate-limiters-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/loop_rate_limiters/__init__.py` & `loop-rate-limiters-0.4.0/loop_rate_limiters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Loop rate limiters."""
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 from .async_rate_limiter import AsyncRateLimiter
 from .rate_limiter import RateLimiter
 
 __all__ = [
     "AsyncRateLimiter",
     "RateLimiter",
```

### Comparing `loop-rate-limiters-0.3.0/loop_rate_limiters/async_rate_limiter.py` & `loop-rate-limiters-0.4.0/loop_rate_limiters/async_rate_limiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     _loop: asyncio.AbstractEventLoop
     _next_tick: float
     measured_period: float
     name: str
     period: float
     slack: float
 
-    def __init__(self, frequency: float, name: str = "rate_limiter"):
+    def __init__(self, frequency: float, name: str = "rate limiter"):
         """Initialize rate limiter.
 
         Args:
             frequency: Desired loop frequency in hertz.
             name: Human-readable name used for logging.
         """
         loop = asyncio.get_event_loop()
```

### Comparing `loop-rate-limiters-0.3.0/loop_rate_limiters/rate_limiter.py` & `loop-rate-limiters-0.4.0/loop_rate_limiters/rate_limiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Basic rate limiter."""
 
+import logging
 from time import perf_counter, sleep
 
 
 class RateLimiter:
     """Regulate the frequency between calls to the same instruction.
 
     This rate limniter is meant to be used in e.g. a loop or callback function.
@@ -33,23 +34,25 @@
         https://github.com/ros/ros_comm/blob/noetic-devel/clients/rospy/src/rospy/timer.py
     """
 
     __period: float
     __slack: float
     __next_tick: float
 
-    def __init__(self, frequency: float):
+    def __init__(self, frequency: float, name: str = "rate limiter"):
         """Initialize rate limiter.
 
         Args:
             frequency: Desired frequency in hertz.
+            name: Human-readable name used for logging.
         """
         period = 1.0 / frequency
         self.__next_tick = perf_counter() + period
         self.__period = period
+        self.name = name
 
     @property
     def dt(self) -> float:
         """Desired period between two calls to :func:`sleep`, in seconds."""
         return self.__period
 
     @property
@@ -79,8 +82,14 @@
         return self.__next_tick - perf_counter()
 
     def sleep(self):
         """Sleep for the duration required to regulate inter-call frequency."""
         self.__slack = self.__next_tick - perf_counter()
         if self.__slack > 0.0:
             sleep(self.__slack)
+        elif self.__slack < -0.1 * self.period:
+            logging.warning(
+                "%s is late by %f [ms]",
+                self.name,
+                round(1e3 * self.__slack, 1),
+            )
         self.__next_tick = perf_counter() + self.__period
```

### Comparing `loop-rate-limiters-0.3.0/pyproject.toml` & `loop-rate-limiters-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/tests/__init__.py` & `loop-rate-limiters-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/tests/test_async_rate.py` & `loop-rate-limiters-0.4.0/tests/test_async_rate.py`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/tests/test_rate_limiter.py` & `loop-rate-limiters-0.4.0/tests/test_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/tox.ini` & `loop-rate-limiters-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.3.0/PKG-INFO` & `loop-rate-limiters-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loop-rate-limiters
-Version: 0.3.0
+Version: 0.4.0
 Summary: Loop rate limiters.
 Keywords: rate,loop,frequency,regulator,limiter
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

