# Comparing `tmp/extr-0.0.3.tar.gz` & `tmp/extr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.3.tar", last modified: Wed Apr 12 10:53:28 2023, max compression
+gzip compressed data, was "extr-0.0.4.tar", last modified: Thu Apr 13 10:25:53 2023, max compression
```

## Comparing `extr-0.0.3.tar` & `extr-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.633602 extr-0.0.3/
--rw-rw-rw-   0        0        0     2422 2023-04-12 10:53:28.633602 extr-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1586 2023-04-11 09:38:34.000000 extr-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 10:53:28.654589 extr-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-04-12 10:52:32.000000 extr-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.460178 extr-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.549514 extr-0.0.3/src/extr/
--rw-rw-rw-   0        0        0      236 2023-04-12 10:21:01.000000 extr-0.0.3/src/extr/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-04-12 10:52:20.000000 extr-0.0.3/src/extr/entities.py
--rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.3/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     1780 2023-04-12 10:52:00.000000 extr-0.0.3/src/extr/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.3/src/extr/regex.py
--rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.3/src/extr/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.625555 extr-0.0.3/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2422 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 10:25:53.212402 extr-0.0.4/
+-rw-rw-rw-   0        0        0     2422 2023-04-13 10:25:53.207452 extr-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1586 2023-04-11 09:38:34.000000 extr-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 10:25:53.217674 extr-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-04-13 10:25:49.000000 extr-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:25:53.027955 extr-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 10:25:53.110778 extr-0.0.4/src/extr/
+-rw-rw-rw-   0        0        0      236 2023-04-12 10:21:01.000000 extr-0.0.4/src/extr/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-04-13 10:18:22.000000 extr-0.0.4/src/extr/entities.py
+-rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.4/src/extr/iterutils.py
+-rw-rw-rw-   0        0        0     2189 2023-04-13 10:16:15.000000 extr-0.0.4/src/extr/models.py
+-rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.4/src/extr/regex.py
+-rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.4/src/extr/relations.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:25:53.203766 extr-0.0.4/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2422 2023-04-13 10:25:52.000000 extr-0.0.4/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-13 10:25:52.000000 extr-0.0.4/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 10:25:52.000000 extr-0.0.4/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-13 10:25:52.000000 extr-0.0.4/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.3/PKG-INFO` & `extr-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
```

### Comparing `extr-0.0.3/README.md` & `extr-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `extr-0.0.3/src/extr/models.py` & `extr-0.0.4/src/extr/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,54 @@
 # pylint: enable=C0103
 
 @dataclass(frozen=True)
 class Location:
     start: int
     end: int
 
+    @property
+    def actual_end(self) -> int:
+        return self.end - 1
+
     def is_in(self: TLocation, other: TLocation) -> bool:
-        return self.start >= other.start and self.start <= other.end \
-            or self.end >= other.start and self.end <= other.end
+        return self.start >= other.start and self.start <= other.actual_end \
+            or self.actual_end >= other.start and self.actual_end <= other.actual_end
 
     def contains(self: TLocation, other: TLocation) -> bool:
-        return other.start >= self.start and other.end <= self.end
+        return other.start >= self.start and other.actual_end <= self.actual_end
 
     def __repr__(self) -> str:
         return f'({self.start}, {self.end})'
 
+# pylint: disable=C0103
+TEntity = TypeVar('TEntity', bound='Entity')
+# pylint: enable=C0103
+
 @dataclass()
 class Entity:
     label: str
     text: str
     location: Location
     identifer: int = NOT_DEFINED_FLAG
-    token_id: int = NOT_DEFINED_FLAG
     attributes: Dict[str, Any] = field(default_factory=dict)
 
     @property
     def start(self) -> int:
         return self.location.start
 
     @property
     def end(self) -> int:
         return self.location.end
 
+    def is_in(self: TEntity, other: TEntity) -> bool:
+            return self.location.is_in(other.location)
+
+    def contains(self: TEntity, other: TEntity) -> bool:
+        return self.location.contains(other.location)
+
     def __repr__(self) -> str:
         return f'<Entity label="{self.label}" text="{self.text}" span={repr(self.location)}>'
 
     def __str__(self) -> str:
         return f'##ENTITY_{self.label}_{self.identifer}##'
 
 @dataclass(frozen=True)
```

### Comparing `extr-0.0.3/src/extr/regex.py` & `extr-0.0.4/src/extr/regex.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.3/src/extr/relations.py` & `extr-0.0.4/src/extr/relations.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.3/src/extr.egg-info/PKG-INFO` & `extr-0.0.4/src/extr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
```

