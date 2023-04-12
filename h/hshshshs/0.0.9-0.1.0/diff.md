# Comparing `tmp/hshshshs-0.0.9.tar.gz` & `tmp/hshshshs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hshshshs-0.0.9.tar", last modified: Wed Apr 12 07:24:05 2023, max compression
+gzip compressed data, was "hshshshs-0.1.0.tar", last modified: Wed Apr 12 23:49:41 2023, max compression
```

## Comparing `hshshshs-0.0.9.tar` & `hshshshs-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:05.171918 hshshshs-0.0.9/
--rw-rw-rw-   0        0        0      261 2023-04-12 07:24:05.170919 hshshshs-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:05.160925 hshshshs-0.0.9/hshshshs/
--rw-rw-rw-   0        0        0        0 2023-03-17 08:41:46.000000 hshshshs-0.0.9/hshshshs/__init__.py
--rw-rw-rw-   0        0        0     5714 2023-04-12 07:22:47.000000 hshshshs-0.0.9/hshshshs/cFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:24:05.168920 hshshshs-0.0.9/hshshshs.egg-info/
--rw-rw-rw-   0        0        0      261 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 07:24:05.171918 hshshshs-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-12 07:22:54.000000 hshshshs-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 23:49:41.274477 hshshshs-0.1.0/
+-rw-rw-rw-   0        0        0      261 2023-04-12 23:49:41.274477 hshshshs-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 23:49:41.274477 hshshshs-0.1.0/hshshshs/
+-rw-rw-rw-   0        0        0        0 2023-03-17 08:41:46.000000 hshshshs-0.1.0/hshshshs/__init__.py
+-rw-rw-rw-   0        0        0     5721 2023-04-12 23:47:56.000000 hshshshs-0.1.0/hshshshs/cFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-12 23:49:41.274477 hshshshs-0.1.0/hshshshs.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-04-12 23:49:41.000000 hshshshs-0.1.0/hshshshs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-12 23:49:41.000000 hshshshs-0.1.0/hshshshs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 23:49:41.000000 hshshshs-0.1.0/hshshshs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-12 23:49:41.000000 hshshshs-0.1.0/hshshshs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 23:49:41.000000 hshshshs-0.1.0/hshshshs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 23:49:41.274477 hshshshs-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-12 23:49:16.000000 hshshshs-0.1.0/setup.py
```

### Comparing `hshshshs-0.0.9/hshshshs/cFunction.py` & `hshshshs-0.1.0/hshshshs/cFunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     parameter(입력값) x: 기준 년도와 주차 y : 빼고싶은 주차
     return : 기준 년도에서 빼고싶은 주차를 뺀 값 : x와 형식 동일
     """
 
        
 
     # 년도와 주차를 인덱스로 나누기 위해 String으로
-    inputdata = str(x)
+    inputdata = str(yearWeek)
 
     inputyear = inputdata[:4]
 
     inputweek = inputdata[4:]
 
     # 계산하기 위해 다시 숫자로
     proceccedYear = int(inputyear)
```

### Comparing `hshshshs-0.0.9/setup.py` & `hshshshs-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 module_name = "%(base)s.%(item)s" % vars()
             else:
                 module_name = item
             packages[module_name] = dir
             packages.update(find_packages(dir, module_name))
     return packages
 setup(  name="hshshshs",
-        version="0.0.9",
+        version="0.1.0",
         url="http://github.com/kimhansu/hshshshs",
         license="MIT",
         author="kimhansu",
         author_email="gimhansu@naver.com",
         keywords=["calendar","isoweek","listsum"],
         description="math function",
         packages=find_packages("."),
```

