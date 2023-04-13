# Comparing `tmp/ncompress-1.0.0.tar.gz` & `tmp/ncompress-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncompress-1.0.0.tar", last modified: Sat Dec 18 20:36:56 2021, max compression
+gzip compressed data, was "ncompress-1.0.1.tar", last modified: Thu Apr 13 11:05:08 2023, max compression
```

## Comparing `ncompress-1.0.0.tar` & `ncompress-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 20:36:56.847711 ncompress-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-18 20:36:42.000000 ncompress-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-12-18 20:36:42.000000 ncompress-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-12-18 20:36:56.847711 ncompress-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-12-18 20:36:42.000000 ncompress-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 20:36:56.847711 ncompress-1.0.0/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-12-18 20:36:42.000000 ncompress-1.0.0/include/ncompress.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 20:36:56.847711 ncompress-1.0.0/ncompress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-12-18 20:36:56.000000 ncompress-1.0.0/ncompress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-18 20:36:56.000000 ncompress-1.0.0/ncompress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-18 20:36:56.000000 ncompress-1.0.0/ncompress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-18 20:36:56.000000 ncompress-1.0.0/ncompress.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-18 20:36:56.000000 ncompress-1.0.0/ncompress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-18 20:36:56.000000 ncompress-1.0.0/ncompress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-12-18 20:36:42.000000 ncompress-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-12-18 20:36:56.847711 ncompress-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-12-18 20:36:42.000000 ncompress-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 20:36:56.847711 ncompress-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)    18389 2021-12-18 20:36:42.000000 ncompress-1.0.0/src/ncompress.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    18633 2021-12-18 20:36:42.000000 ncompress-1.0.0/src/pystreambuf.h
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-12-18 20:36:42.000000 ncompress-1.0.0/src/python.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 20:36:56.847711 ncompress-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2961 2021-12-18 20:36:42.000000 ncompress-1.0.0/test/test_ncompress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:05:08.578453 ncompress-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 11:04:53.000000 ncompress-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 11:04:53.000000 ncompress-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-13 11:05:08.578453 ncompress-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-13 11:04:53.000000 ncompress-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:05:08.574453 ncompress-1.0.1/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-13 11:04:53.000000 ncompress-1.0.1/include/ncompress.h
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-13 11:04:53.000000 ncompress-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-13 11:05:08.578453 ncompress-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-13 11:04:53.000000 ncompress-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:05:08.574453 ncompress-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:05:08.578453 ncompress-1.0.1/src/ncompress/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 11:04:53.000000 ncompress-1.0.1/src/ncompress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-04-13 11:04:53.000000 ncompress-1.0.1/src/ncompress.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:05:08.578453 ncompress-1.0.1/src/ncompress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-13 11:05:08.000000 ncompress-1.0.1/src/ncompress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 11:05:08.000000 ncompress-1.0.1/src/ncompress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:05:08.000000 ncompress-1.0.1/src/ncompress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:05:08.000000 ncompress-1.0.1/src/ncompress.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 11:05:08.000000 ncompress-1.0.1/src/ncompress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 11:05:08.000000 ncompress-1.0.1/src/ncompress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-04-13 11:04:53.000000 ncompress-1.0.1/src/pystreambuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-13 11:04:53.000000 ncompress-1.0.1/src/python.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:05:08.578453 ncompress-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-13 11:04:53.000000 ncompress-1.0.1/test/test_ncompress.py
```

### Comparing `ncompress-1.0.0/LICENSE` & `ncompress-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncompress-1.0.0/PKG-INFO` & `ncompress-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: ncompress
-Version: 1.0.0
+Version: 1.0.1
 Summary: LZW compression and decompression
 Home-page: https://github.com/valgur/ncompress
 Author: Martin Valgur
 Author-email: martin.valgur@gmail.com
 License: Unlicense
 Keywords: LZW,compression
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
-# ncompress [![PyPI](https://img.shields.io/pypi/v/ncompress)](https://pypi.org/project/ncompress/) [![Build](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml/badge.svg?event=push)](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml)
+# ncompress [![PyPI](https://img.shields.io/pypi/v/ncompress)](https://pypi.org/project/ncompress/) [![Build](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml/badge.svg?event=push)](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/ncompress)](https://pypistats.org/packages/ncompress)
 
 LZW compression and decompression in Python and C++.
 
 Ported with minimal changes from the [(N)compress](https://github.com/vapier/ncompress) CLI tool.
 
 ## Installation
 
-Wheels are available for Python 3.6+ and all operating systems on PyPI.
+Wheels are available for Python 3.8+ and all operating systems on PyPI.
 
 ```bash
 pip install ncompress
 ```
 
 ## Usage
 
 Functions `compress()` and `decompress()` are available with the following inputs/outputs:
 
 * `bytes` → `bytes`
 * `BytesIO` → `bytes`
 * `BytesIO`, `BytesIO` → `None`
 * `bytes`, `BytesIO` → `None`
 
-The `BytesIO`-based functions are slightly (about 15%) faster.
+The `BytesIO`-based functions are slightly (about 15%) faster due to avoiding a copy of the contents on `bytes`⇄`std::string` conversion.
 
 ## Authors
 
 * Martin Valgur ([@valgur](https://github.com/valgur))
 
 The core functionality has been adapted from [vapier/ncompress](https://github.com/vapier/ncompress).
 
@@ -50,9 +50,7 @@
 
 All modifications and additions are released under the [Unlicense](LICENSE).
 
 The base (N)compress code has been released into the public domain.
 
 The `BytesIO` wrapper in [pystreambuf.h](src/pystreambuf.h) has been adapted from the [cctbx](https://github.com/cctbx/cctbx_project) project.
 See the license in the linked file for details.
-
-
```

### Comparing `ncompress-1.0.0/README.md` & `ncompress-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# ncompress [![PyPI](https://img.shields.io/pypi/v/ncompress)](https://pypi.org/project/ncompress/) [![Build](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml/badge.svg?event=push)](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml)
+# ncompress [![PyPI](https://img.shields.io/pypi/v/ncompress)](https://pypi.org/project/ncompress/) [![Build](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml/badge.svg?event=push)](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/ncompress)](https://pypistats.org/packages/ncompress)
 
 LZW compression and decompression in Python and C++.
 
 Ported with minimal changes from the [(N)compress](https://github.com/vapier/ncompress) CLI tool.
 
 ## Installation
 
-Wheels are available for Python 3.6+ and all operating systems on PyPI.
+Wheels are available for Python 3.8+ and all operating systems on PyPI.
 
 ```bash
 pip install ncompress
 ```
 
 ## Usage
 
 Functions `compress()` and `decompress()` are available with the following inputs/outputs:
 
 * `bytes` → `bytes`
 * `BytesIO` → `bytes`
 * `BytesIO`, `BytesIO` → `None`
 * `bytes`, `BytesIO` → `None`
 
-The `BytesIO`-based functions are slightly (about 15%) faster.
+The `BytesIO`-based functions are slightly (about 15%) faster due to avoiding a copy of the contents on `bytes`⇄`std::string` conversion.
 
 ## Authors
 
 * Martin Valgur ([@valgur](https://github.com/valgur))
 
 The core functionality has been adapted from [vapier/ncompress](https://github.com/vapier/ncompress).
```

### Comparing `ncompress-1.0.0/include/ncompress.h` & `ncompress-1.0.1/include/ncompress.h`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,11 @@
  * Decompresses the LZW-compressed input.
  *
  * @throws std::ios_base::failure on stream errors
  * @throws std::invalid_argument on invalid or corrupted input data
  */
 void decompress(std::istream &in, std::ostream &out);
 
+static const unsigned char MAGIC_1 = 0x1fU; /* First byte of compressed file */
+static const unsigned char MAGIC_2 = 0x9dU; /* Second byte of compressed file */
+
 } // namespace ncompress
```

### Comparing `ncompress-1.0.0/ncompress.egg-info/PKG-INFO` & `ncompress-1.0.1/src/ncompress.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: ncompress
-Version: 1.0.0
+Version: 1.0.1
 Summary: LZW compression and decompression
 Home-page: https://github.com/valgur/ncompress
 Author: Martin Valgur
 Author-email: martin.valgur@gmail.com
 License: Unlicense
 Keywords: LZW,compression
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
-# ncompress [![PyPI](https://img.shields.io/pypi/v/ncompress)](https://pypi.org/project/ncompress/) [![Build](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml/badge.svg?event=push)](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml)
+# ncompress [![PyPI](https://img.shields.io/pypi/v/ncompress)](https://pypi.org/project/ncompress/) [![Build](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml/badge.svg?event=push)](https://github.com/valgur/velodyne_decoder/actions/workflows/build.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/ncompress)](https://pypistats.org/packages/ncompress)
 
 LZW compression and decompression in Python and C++.
 
 Ported with minimal changes from the [(N)compress](https://github.com/vapier/ncompress) CLI tool.
 
 ## Installation
 
-Wheels are available for Python 3.6+ and all operating systems on PyPI.
+Wheels are available for Python 3.8+ and all operating systems on PyPI.
 
 ```bash
 pip install ncompress
 ```
 
 ## Usage
 
 Functions `compress()` and `decompress()` are available with the following inputs/outputs:
 
 * `bytes` → `bytes`
 * `BytesIO` → `bytes`
 * `BytesIO`, `BytesIO` → `None`
 * `bytes`, `BytesIO` → `None`
 
-The `BytesIO`-based functions are slightly (about 15%) faster.
+The `BytesIO`-based functions are slightly (about 15%) faster due to avoiding a copy of the contents on `bytes`⇄`std::string` conversion.
 
 ## Authors
 
 * Martin Valgur ([@valgur](https://github.com/valgur))
 
 The core functionality has been adapted from [vapier/ncompress](https://github.com/vapier/ncompress).
 
@@ -50,9 +50,7 @@
 
 All modifications and additions are released under the [Unlicense](LICENSE).
 
 The base (N)compress code has been released into the public domain.
 
 The `BytesIO` wrapper in [pystreambuf.h](src/pystreambuf.h) has been adapted from the [cctbx](https://github.com/cctbx/cctbx_project) project.
 See the license in the linked file for details.
-
-
```

### Comparing `ncompress-1.0.0/setup.cfg` & `ncompress-1.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ncompress
-version = 1.0.0
+version = 1.0.1
 author = Martin Valgur
 author_email = martin.valgur@gmail.com
 url = https://github.com/valgur/ncompress
 description = LZW compression and decompression
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Unlicense
@@ -14,18 +14,18 @@
 	compression
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	License :: OSI Approved :: The Unlicense (Unlicense)
 
 [options]
-packages = find:
+include_package_data = True
 zip_safe = False
+python_requires = >= 3.8
 
 [options.extras_require]
-tests = 
-	pytest
+tests = pytest
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ncompress-1.0.0/src/ncompress.cpp` & `ncompress-1.0.1/src/ncompress.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -7,112 +7,111 @@
  *   Ken Turkowski       (decvax!decwrl!turtlevax!ken)
  *   James A. Woods      (decvax!ihnp4!ames!jaw)
  *   Joe Orost           (decvax!vax135!petsd!joe)
  *   Dave Mack           (csu@alembic.acs.com)
  *   Peter Jannesen, Network Communication Systems
  *                       (peter@ncs.nl)
  *   Mike Frysinger      (vapier@gmail.com)
- *   Martin Valgur       (martin.valgur@gmail.com)
- */
+ *   Martin Valgur       (martin.valgur@gmail.com) */
 
 #include "ncompress.h"
 
 #include <cstdio>
 #include <cstring>
 #include <istream>
 #include <ostream>
 #include <string>
 
+namespace ncompress
+{
+
 #ifndef IBUFSIZ
-#  define IBUFSIZ BUFSIZ /* Default input buffer size							*/
+#  define IBUFSIZ BUFSIZ /* Default input buffer size */
 #endif
 #ifndef OBUFSIZ
-#  define OBUFSIZ BUFSIZ /* Default output buffer size							*/
+#  define OBUFSIZ BUFSIZ /* Default output buffer size */
 #endif
 
-/* Defines for third byte of header 					*/
-#define MAGIC_1  (char_type)'\037' /* First byte of compressed file				*/
-#define MAGIC_2  (char_type)'\235' /* Second byte of compressed file				*/
-#define BIT_MASK 0x1f /* Mask for 'number of compression bits'		*/
-/* Masks 0x20 and 0x40 are free.  				*/
-/* I think 0x20 should mean that there is		*/
-/* a fourth header byte (for expansion).    	*/
-#define BLOCK_MODE 0x80 /* Block compression if table is full and		*/
-/* compression rate is dropping flush tables	*/
-
-/* the next two codes should not be changed lightly, as they must not	*/
-/* lie within the contiguous general code space.						*/
-#define FIRST 257 /* first free entry 							*/
-#define CLEAR 256 /* table clear output code 						*/
-
-#define INIT_BITS 9 /* initial number of bits/code */
-
-#define HBITS  17 /* 50% occupancy */
-#define HSIZE  (1 << HBITS)
-#define HMASK  (HSIZE - 1)
-#define HPRIME 9941
-#define BITS   16
-
-#define CHECK_GAP 10000
-
-typedef long int code_int;
-typedef long int count_int;
-typedef long int cmp_code_int;
-typedef unsigned char char_type;
-
-#define MAXCODE(n) (1L << (n))
-
-#define output(b, o, c, n)             \
-  {                                    \
-    char_type *p = &(b)[(o) >> 3];     \
-    long i = ((long)(c)) << ((o)&0x7); \
-    p[0] |= (char_type)(i);            \
-    p[1] |= (char_type)(i >> 8);       \
-    p[2] |= (char_type)(i >> 16);      \
-    (o) += (n);                        \
-  }
-#define input(b, o, c, n, m)                       \
-  {                                                \
-    char_type *p = &(b)[(o) >> 3];                 \
-    (c) = ((((long)(p[0])) | ((long)(p[1]) << 8) | \
-               ((long)(p[2]) << 16)) >>            \
-              ((o)&0x7)) &                         \
-        (m);                                       \
-    (o) += (n);                                    \
-  }
+using code_int = long;
+using count_int = long;
+using cmp_code_int = long;
+using char_type = unsigned char;
+using codetab_type = unsigned short;
+
+/* Defines for third byte of header */
+const char_type BIT_MASK = 0x1fU; /* Mask for 'number of compression bits' */
+/* Masks 0x20 and 0x40 are free. */
+/* I think 0x20 should mean that there is */
+/* a fourth header byte (for expansion). */
+const char_type BLOCK_MODE = 0x80U; /* Block compression if table is full and
+                                           compression rate is dropping flush tables */
+
+/* the next two codes should not be changed lightly, as they must not */
+/* lie within the contiguous general code space. */
+const code_int FIRST = 257; /* first free entry */
+const code_int CLEAR = 256; /* table clear output code */
+
+const int INIT_BITS = 9; /* initial number of bits/code */
+
+const int HBITS = 17; /* 50% occupancy */
+const int HSIZE = 1 << HBITS;
+const int HMASK = HSIZE - 1;
+const int BITS = 16;
 
-#define reset_n_bits_for_compressor(n_bits, stcode, free_ent, extcode, maxbits) \
-  {                                                                             \
-    n_bits = INIT_BITS;                                                         \
-    stcode = 1;                                                                 \
-    free_ent = FIRST;                                                           \
-    extcode = MAXCODE(n_bits);                                                  \
-    if (n_bits < maxbits)                                                       \
-      extcode++;                                                                \
-  }
+const long CHECK_GAP = 10000;
 
-#define reset_n_bits_for_decompressor(n_bits, bitmask, maxbits, maxcode, maxmaxcode) \
-  {                                                                                  \
-    n_bits = INIT_BITS;                                                              \
-    bitmask = (1 << n_bits) - 1;                                                     \
-    if (n_bits == maxbits)                                                           \
-      maxcode = maxmaxcode;                                                          \
-    else                                                                             \
-      maxcode = MAXCODE(n_bits) - 1;                                                 \
-  }
+constexpr code_int
+MAXCODE(int n)
+{
+  return 1L << n;
+}
+
+void
+output(char_type *buf, int &bits, code_int code, int n_bits)
+{
+  char_type *p = &buf[bits >> 3];
+  long i = static_cast<long>(code) << (bits & 0x7);
+  p[0] |= static_cast<char_type>(i);
+  p[1] |= static_cast<char_type>(i >> 8);
+  p[2] |= static_cast<char_type>(i >> 16);
+  bits += n_bits;
+}
+
+code_int
+input(char_type *buf, int &bits, int n_bits, int bitmask)
+{
+  char_type *p = &buf[bits >> 3];
+  long i = ((long)(p[0])) | ((long)(p[1]) << 8) | ((long)(p[2]) << 16);
+  code_int code = (i >> (bits & 0x7)) & bitmask;
+  bits += n_bits;
+  return code;
+}
 
-#define tab_prefixof(i)      codetab[i]
-#define tab_suffixof(i)      ((char_type *)(htab))[i]
-#define de_stack             ((char_type *)&(htab[HSIZE - 1]))
-#define clear_htab()         memset(htab, -1, sizeof(htab))
-#define clear_tab_prefixof() memset(codetab, 0, 256);
+void
+reset_n_bits_for_compressor(
+    int &n_bits, int &stcode, code_int &free_ent, code_int &extcode, int maxbits)
+{
+  n_bits = INIT_BITS;
+  stcode = 1;
+  free_ent = FIRST;
+  extcode = MAXCODE(n_bits);
+  if (n_bits < maxbits)
+    extcode++;
+}
 
-namespace ncompress
+void
+reset_n_bits_for_decompressor(
+    int &n_bits, int &bitmask, int maxbits, code_int &maxcode, code_int maxmaxcode)
 {
+  n_bits = INIT_BITS;
+  bitmask = (1 << n_bits) - 1;
+  maxcode = (n_bits == maxbits) ? maxmaxcode : MAXCODE(n_bits) - 1;
+}
 
+/* clang-format off */
 static const int primetab[256] = /* Special secudary hash table.		*/
     {
       1013, -1061, 1109, -1181, 1231, -1291, 1361, -1429,
       1481, -1531, 1583, -1627, 1699, -1759, 1831, -1889,
       1973, -2017, 2083, -2137, 2213, -2273, 2339, -2383,
       2441, -2531, 2593, -2663, 2707, -2753, 2819, -2887,
       2957, -3023, 3089, -3181, 3251, -3313, 3361, -3449,
@@ -140,14 +139,15 @@
       15733, -15791, 15881, -15937, 16057, -16097, 16189, -16267,
       16363, -16447, 16529, -16619, 16691, -16763, 16879, -16937,
       17021, -17093, 17183, -17257, 17341, -17401, 17477, -17551,
       17623, -17713, 17791, -17891, 17957, -18041, 18097, -18169,
       18233, -18307, 18379, -18451, 18523, -18637, 18731, -18803,
       18919, -19031, 19121, -19211, 19273, -19381, 19429, -19477
     };
+/* clang-format on */
 
 void read_error();
 void write_error();
 
 /*
  * Compress in stream to out stream.
  *
@@ -157,91 +157,83 @@
  * secondary probe.  Here, the modular division first probe is gives way
  * to a faster exclusive-or manipulation.  Also do block compression with
  * an adaptive reset, whereby the code table is cleared when the compression
  * ratio decreases, but after the table fills.  The variable-length output
  * codes are re-sized at this point, and a special CLEAR code is generated
  * for the decompressor.  Late addition:  construct the table according to
  * file size for noticeable speed improvement on small files.  Please direct
- * questions about this implementation to ames!jaw.
- */
+ * questions about this implementation to ames!jaw. */
 void
 compress(std::istream &in, std::ostream &out)
 {
-  long hp;
-  int rpos;
-  long fc;
-  int outbits;
-  int rlop;
-  int rsize;
+  char_type inbuf[IBUFSIZ + 64]; /* Input buffer */
+  char_type outbuf[OBUFSIZ + 2048]; /* Output buffer */
+
+  long bytes_in = 0; /* Total number of bytes from input */
+  long bytes_out = 0; /* Total number of bytes to output */
+
+  count_int htab[HSIZE];
+  unsigned short codetab[HSIZE];
+
+  auto clear_htab = [&]() { memset(htab, -1, sizeof(htab)); };
+
+  int n_bits;
   int stcode;
   code_int free_ent;
-  int boff;
-  int n_bits;
+  code_int extcode;
+  int maxbits = BITS; /* user settable max # bits/code */
+  reset_n_bits_for_compressor(n_bits, stcode, free_ent, extcode, maxbits);
   int ratio = 0;
   long checkpoint = CHECK_GAP;
-  code_int extcode;
   union
   {
     long code = 0;
     struct
     {
       char_type c;
       unsigned short ent;
     } e;
   } fcode;
 
-  int maxbits = BITS; /* user settable max # bits/code 				*/
-
-  char_type inbuf[IBUFSIZ + 64]; /* Input buffer									*/
-  char_type outbuf[OBUFSIZ + 2048]; /* Output buffer								*/
-
-  long bytes_in = 0; /* Total number of bytes from input				*/
-  long bytes_out = 0; /* Total number of bytes to output				*/
-
-  count_int htab[HSIZE];
-  unsigned short codetab[HSIZE];
-
-  reset_n_bits_for_compressor(n_bits, stcode, free_ent, extcode, maxbits);
-
   memset(outbuf, 0, sizeof(outbuf));
   outbuf[0] = MAGIC_1;
   outbuf[1] = MAGIC_2;
-  outbuf[2] = (char)(maxbits | BLOCK_MODE);
-  boff = outbits = (3 << 3);
+  outbuf[2] = (char_type)(maxbits | BLOCK_MODE);
+  int outbits = 3 << 3;
+  int boff = outbits;
 
   clear_htab();
 
   while (in.good())
   {
     in.read((char *)inbuf, IBUFSIZ);
-    rsize = (int)in.gcount();
+    int rsize = (int)in.gcount();
     if (rsize <= 0)
       break;
 
+    int rpos = 0;
     if (bytes_in == 0)
     {
       fcode.e.ent = inbuf[0];
       rpos = 1;
     }
-    else
-      rpos = 0;
 
-    rlop = 0;
+    int rlop = 0;
 
     do
     {
       if (free_ent >= extcode && fcode.e.ent < FIRST)
       {
         if (n_bits < maxbits)
         {
-          boff = outbits = (outbits - 1) + ((n_bits << 3) - ((outbits - boff - 1 + (n_bits << 3)) % (n_bits << 3)));
-          if (++n_bits < maxbits)
-            extcode = MAXCODE(n_bits) + 1;
-          else
-            extcode = MAXCODE(n_bits);
+          outbits = (outbits - 1) +
+              ((n_bits << 3) - ((outbits - boff - 1 + (n_bits << 3)) % (n_bits << 3)));
+          boff = outbits;
+          ++n_bits;
+          extcode = (n_bits < maxbits) ? MAXCODE(n_bits) + 1 : MAXCODE(n_bits);
         }
         else
         {
           extcode = MAXCODE(16) + OBUFSIZ;
           stcode = 0;
         }
       }
@@ -266,15 +258,17 @@
         if (rat >= ratio)
           ratio = (int)rat;
         else
         {
           ratio = 0;
           clear_htab();
           output(outbuf, outbits, CLEAR, n_bits);
-          boff = outbits = (outbits - 1) + ((n_bits << 3) - ((outbits - boff - 1 + (n_bits << 3)) % (n_bits << 3)));
+          outbits = (outbits - 1) +
+              ((n_bits << 3) - ((outbits - boff - 1 + (n_bits << 3)) % (n_bits << 3)));
+          boff = outbits;
           reset_n_bits_for_compressor(n_bits, stcode, free_ent, extcode, maxbits);
         }
       }
 
       if (outbits >= (OBUFSIZ << 3))
       {
         out.write((char *)outbuf, OBUFSIZ);
@@ -286,91 +280,95 @@
         bytes_out += OBUFSIZ;
 
         memcpy(outbuf, outbuf + OBUFSIZ, (outbits >> 3) + 1);
         memset(outbuf + (outbits >> 3) + 1, '\0', OBUFSIZ);
       }
 
       {
-        int i;
-
-        i = rsize - rlop;
+        int i = rsize - rlop;
 
         if ((code_int)i > extcode - free_ent)
           i = (int)(extcode - free_ent);
         if (i > (((int)sizeof(outbuf) - 32) * 8 - outbits) / n_bits)
           i = (((int)sizeof(outbuf) - 32) * 8 - outbits) / n_bits;
 
         if (!stcode && (long)i > checkpoint - bytes_in)
           i = (int)(checkpoint - bytes_in);
 
         rlop += i;
         bytes_in += i;
       }
 
-      goto next;
-    hfound:
-      fcode.e.ent = codetab[hp];
-    next:
-      if (rpos >= rlop)
-        goto endlop;
-    next2:
-      fcode.e.c = inbuf[rpos++];
-      {
-        long i;
-        long p;
-        fc = fcode.code;
-        hp = ((((long)(fcode.e.c)) << (HBITS - 8)) ^ (long)(fcode.e.ent));
-
-        if ((i = htab[hp]) == fc)
-          goto hfound;
-        if (i == -1)
-          goto out;
-
-        p = primetab[fcode.e.c];
-      lookup:
-        hp = (hp + p) & HMASK;
-        if ((i = htab[hp]) == fc)
-          goto hfound;
-        if (i == -1)
-          goto out;
-        hp = (hp + p) & HMASK;
-        if ((i = htab[hp]) == fc)
-          goto hfound;
-        if (i == -1)
-          goto out;
-        hp = (hp + p) & HMASK;
-        if ((i = htab[hp]) == fc)
-          goto hfound;
-        if (i == -1)
-          goto out;
-        goto lookup;
-      }
-    out:;
-      output(outbuf, outbits, fcode.e.ent, n_bits);
-
-      {
-        long fc_tmp = fcode.code;
-        fcode.e.ent = fcode.e.c;
-        if (stcode)
+      {
+        long hp;
+
+        goto next;
+      hfound:
+        fcode.e.ent = codetab[hp];
+      next:
+        if (rpos >= rlop)
+          goto endlop;
+      next2:
+        fcode.e.c = inbuf[rpos++];
         {
-          codetab[hp] = (unsigned short)free_ent++;
-          htab[hp] = fc_tmp;
+          long fc = fcode.code;
+          hp = (((long)(fcode.e.c)) << (HBITS - 8)) ^ (long)(fcode.e.ent);
+
+          long i = htab[hp];
+          if (i == fc)
+            goto hfound;
+          if (i == -1)
+            goto out;
+
+          long p = primetab[fcode.e.c];
+        lookup:
+          hp = (hp + p) & HMASK;
+          i = htab[hp];
+          if (i == fc)
+            goto hfound;
+          if (i == -1)
+            goto out;
+          hp = (hp + p) & HMASK;
+          i = htab[hp];
+          if (i == fc)
+            goto hfound;
+          if (i == -1)
+            goto out;
+          hp = (hp + p) & HMASK;
+          i = htab[hp];
+          if (i == fc)
+            goto hfound;
+          if (i == -1)
+            goto out;
+          goto lookup;
+        }
+      out:;
+        output(outbuf, outbits, fcode.e.ent, n_bits);
+
+        {
+          long fc = fcode.code;
+          fcode.e.ent = fcode.e.c;
+          if (stcode)
+          {
+            codetab[hp] = (unsigned short)free_ent++;
+            htab[hp] = fc;
+          }
         }
-      }
 
-      goto next;
+        goto next;
 
-    endlop:
-      if (fcode.e.ent >= FIRST && rpos < rsize)
-        goto next2;
+      endlop:
+        if (fcode.e.ent >= FIRST && rpos < rsize)
+          goto next2;
 
-      if (rpos > rlop)
-      {
-        bytes_in += rpos - rlop;
-        rlop = rpos;
+        if (rpos > rlop)
+        {
+          bytes_in += rpos - rlop;
+          rlop = rpos;
+        }
       }
     }
     while (rlop < rsize);
   }
 
   if (in.bad())
     read_error();
@@ -385,100 +383,84 @@
   bytes_out += (outbits + 7) >> 3;
 }
 
 /*
  * Decompress input stream to output stream. This routine adapts to the codes in the
  * file building the "string" table on-the-fly; requiring no table to
  * be stored in the compressed file.  The tables used herein are shared
- * with those of the compress() routine.  See the definitions above.
- */
+ * with those of the compress() routine.  See the definitions above. */
 void
 decompress(std::istream &in, std::ostream &out)
 {
-  char_type *stackp;
-  code_int code;
-  int finchar;
-  code_int oldcode;
-  code_int incode;
-  int inbits;
-  int posbits;
-  int outpos;
-  int insize = 0;
-  int bitmask;
-  code_int free_ent;
-  code_int maxcode;
-  code_int maxmaxcode;
-  int n_bits;
-  int rsize;
-  int block_mode;
-
-  int maxbits = BITS; /* user settable max # bits/code 				*/
-
-  char_type inbuf[IBUFSIZ + 64]; /* Input buffer									*/
-  char_type outbuf[OBUFSIZ + 2048]; /* Output buffer								*/
+  char_type inbuf[IBUFSIZ + 64]; /* Input buffer */
+  char_type outbuf[OBUFSIZ + 2048]; /* Output buffer */
 
-  long bytes_in = 0; /* Total number of bytes from input				*/
+  long bytes_in = 0; /* Total number of bytes from input */
 
   count_int htab[HSIZE];
   unsigned short codetab[HSIZE];
 
+  auto tab_prefixof = [&codetab](code_int i) -> codetab_type & { return codetab[i]; };
+  auto tab_suffixof = [&htab](
+                          code_int i) -> char_type & { return ((char_type *)htab)[i]; };
+  auto de_stack = [&htab]() { return (char_type *)&(htab[HSIZE - 1]); };
+  auto clear_tab_prefixof = [&]() { memset(codetab, 0, 256); };
+
+  int insize = 0;
+  int rsize;
   while (insize < 3 && in.good())
   {
     in.read((char *)(inbuf + insize), IBUFSIZ);
     rsize = (int)in.gcount();
     insize += rsize;
   }
-
   if (insize < 3 || inbuf[0] != MAGIC_1 || inbuf[1] != MAGIC_2)
   {
     if (in.bad())
       read_error();
     if (insize == 0)
       throw std::invalid_argument("input stream is empty");
     throw std::invalid_argument("not in LZW-compressed format");
   }
+  bytes_in = insize;
 
-  maxbits = inbuf[2] & BIT_MASK;
-  block_mode = inbuf[2] & BLOCK_MODE;
-
+  const int maxbits = inbuf[2] & BIT_MASK;
+  const int block_mode = inbuf[2] & BLOCK_MODE;
   if (maxbits > BITS)
   {
     throw std::invalid_argument("compressed with " + std::to_string(maxbits) +
         " bits, can only handle " + std::to_string(BITS) + " bits");
   }
 
-  maxmaxcode = MAXCODE(maxbits);
-
-  bytes_in = insize;
+  int n_bits;
+  int bitmask;
+  code_int maxcode;
+  const code_int maxmaxcode = MAXCODE(maxbits);
   reset_n_bits_for_decompressor(n_bits, bitmask, maxbits, maxcode, maxmaxcode);
-  oldcode = -1;
-  finchar = 0;
-  outpos = 0;
-  posbits = 3 << 3;
 
-  free_ent = ((block_mode) ? FIRST : 256);
+  code_int oldcode = -1;
+  int finchar = 0;
+  int outpos = 0;
+  int posbits = 3 << 3;
+  code_int free_ent = block_mode ? FIRST : 256;
 
   clear_tab_prefixof(); /* As above, initialize the first
-                   256 entries in the table. */
+                           256 entries in the table. */
 
-  for (code = 255; code >= 0; --code)
+  for (code_int code = 255; code >= 0; --code)
     tab_suffixof(code) = (char_type)code;
 
   do
   {
   resetbuf:;
     {
-      int i;
-      int e;
-      int o;
-
-      o = posbits >> 3;
-      e = o <= insize ? insize - o : 0;
+      int o = posbits >> 3;
+      int e = (o <= insize) ? insize - o : 0;
 
-      for (i = 0; i < e; ++i)
+      for (int i = 0; i < e; ++i)
         inbuf[i] = inbuf[i + o];
 
       insize = e;
       posbits = 0;
     }
 
     if (insize < (int)sizeof(inbuf) - IBUFSIZ)
@@ -486,92 +468,95 @@
       in.read((char *)(inbuf + insize), IBUFSIZ);
       if (in.bad())
         read_error();
       rsize = (int)in.gcount();
       insize += rsize;
     }
 
-    inbits = ((rsize > 0) ? (insize - insize % n_bits) << 3 : (insize << 3) - (n_bits - 1));
+    int inbits =
+        (rsize > 0) ? (insize - insize % n_bits) << 3 : (insize << 3) - (n_bits - 1);
 
     while (inbits > posbits)
     {
       if (free_ent > maxcode)
       {
-        posbits = ((posbits - 1) + ((n_bits << 3) - (posbits - 1 + (n_bits << 3)) % (n_bits << 3)));
+        posbits = (posbits - 1) +
+            ((n_bits << 3) - (posbits - 1 + (n_bits << 3)) % (n_bits << 3));
 
         ++n_bits;
-        if (n_bits == maxbits)
-          maxcode = maxmaxcode;
-        else
-          maxcode = MAXCODE(n_bits) - 1;
-
+        maxcode = (n_bits == maxbits) ? maxmaxcode : MAXCODE(n_bits) - 1;
         bitmask = (1 << n_bits) - 1;
         goto resetbuf;
       }
 
-      input(inbuf, posbits, code, n_bits, bitmask);
+      code_int code = input(inbuf, posbits, n_bits, bitmask);
 
       if (oldcode == -1)
       {
         if (code >= 256)
         {
-          throw std::invalid_argument("corrupt input - oldcode: -1, code: " + std::to_string((int)(code)));
+          throw std::invalid_argument(
+              "corrupt input - oldcode: -1, code: " + std::to_string((int)(code)));
         }
-        outbuf[outpos++] = (char_type)(finchar = (int)(oldcode = code));
+        oldcode = code;
+        finchar = (int)(code);
+        outbuf[outpos++] = (char_type)(code);
         continue;
       }
 
       if (code == CLEAR && block_mode)
       {
         clear_tab_prefixof();
         free_ent = FIRST - 1;
-        posbits = ((posbits - 1) + ((n_bits << 3) - (posbits - 1 + (n_bits << 3)) % (n_bits << 3)));
+        posbits = (posbits - 1) +
+            ((n_bits << 3) - (posbits - 1 + (n_bits << 3)) % (n_bits << 3));
         reset_n_bits_for_decompressor(n_bits, bitmask, maxbits, maxcode, maxmaxcode);
         goto resetbuf;
       }
 
-      incode = code;
-      stackp = de_stack;
+      code_int incode = code;
+      char_type *stackp = de_stack();
 
-      if (code >= free_ent) /* Special case for KwKwK string.	*/
+      if (code >= free_ent) /* Special case for KwKwK string. */
       {
         if (code > free_ent)
         {
           char_type *p;
 
           posbits -= n_bits;
           p = &inbuf[posbits >> 3];
           if (p == inbuf)
             p++;
 
           char err[200];
           snprintf(err, 200,
-              "corrupt input - insize: %d, posbits: %d, inbuf: %02X %02X %02X %02X %02X (%d)",
+              "corrupt input - insize: %d, posbits: %d, "
+              "inbuf: %02X %02X %02X %02X %02X (%d)",
               insize, posbits, p[-1], p[0], p[1], p[2], p[3], (posbits & 07));
           throw std::invalid_argument(err);
         }
 
         *--stackp = (char_type)finchar;
         code = oldcode;
       }
 
       while ((cmp_code_int)code >= (cmp_code_int)256)
       { /* Generate output characters in reverse order */
         *--stackp = tab_suffixof(code);
         code = tab_prefixof(code);
       }
 
-      *--stackp = (char_type)(finchar = tab_suffixof(code));
+      finchar = tab_suffixof(code);
+      *--stackp = (char_type)(finchar);
 
       /* And put them out in forward order */
 
       {
-        int i;
-
-        if (outpos + (i = (int)(de_stack - stackp)) >= OBUFSIZ)
+        int i = (int)(de_stack() - stackp);
+        if (outpos + i >= OBUFSIZ)
         {
           do
           {
             if (i > OBUFSIZ - outpos)
               i = OBUFSIZ - outpos;
 
             if (i > 0)
@@ -585,32 +570,34 @@
               out.write((char *)outbuf, outpos);
               if (out.fail())
                 write_error();
 
               outpos = 0;
             }
             stackp += i;
+            i = (int)(de_stack() - stackp);
           }
-          while ((i = (int)(de_stack - stackp)) > 0);
+          while (i > 0);
         }
         else
         {
           memcpy(outbuf + outpos, stackp, i);
           outpos += i;
         }
       }
 
-      if ((code = free_ent) < maxmaxcode) /* Generate the new entry. */
+      code = free_ent;
+      if (code < maxmaxcode) /* Generate the new entry. */
       {
         tab_prefixof(code) = (unsigned short)oldcode;
         tab_suffixof(code) = (char_type)finchar;
         free_ent = code + 1;
       }
 
-      oldcode = incode; /* Remember previous code.	*/
+      oldcode = incode; /* Remember previous code. */
     }
 
     bytes_in += rsize;
   }
   while (rsize > 0);
 
   if (outpos > 0)
```

### Comparing `ncompress-1.0.0/src/pystreambuf.h` & `ncompress-1.0.1/src/pystreambuf.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 // Based on https://gist.github.com/asford/544323a5da7dddad2c9174490eb5ed06
 // and https://github.com/CadQuery/OCP/blob/master/pystreambuf.h
 // which derive from
 // https://github.com/cctbx/cctbx_project/blob/master/boost_adaptbx/python_streambuf.h
+// and adapted to nanobind.
 //
 // *** License agreement ***
 //
 // cctbx Copyright (c) 2006, The Regents of the University of
 // California, through Lawrence Berkeley National Laboratory (subject to
 // receipt of any required approvals from the U.S. Dept. of Energy).  All
 // rights reserved.
@@ -46,26 +47,29 @@
 // the following license: a  non-exclusive, royalty-free perpetual license
 // to install, use, modify, prepare derivative works, incorporate into
 // other computer software, distribute, and sublicense such enhancements or
 // derivative works thereof, in binary and source code form.
 
 #pragma once
 
-#include <pybind11/pybind11.h>
+#include <nanobind/nanobind.h>
+
+#include <bytesobject.h>
+#include <pyerrors.h>
 
-#include <iostream>
 #include <istream>
+#include <memory>
 #include <ostream>
 #include <streambuf>
 #include <vector>
 
 namespace pystream
 {
 
-namespace py = pybind11;
+namespace nb = nanobind;
 
 /// A stream buffer getting data from and putting data into a Python file object
 /** The aims are as follow:
 
     - Given a C++ function acting on a standard stream, e.g.
 
       \code
@@ -153,41 +157,39 @@
       the Python file object. It can be modified from Python.
   */
   static const size_t default_buffer_size = 1024;
 
   /// Construct from a Python file object
   /** if buffer_size is 0 the current default_buffer_size is used.
    */
-  streambuf(
-      py::object &python_file_obj,
-      size_t buffer_size_ = 0)
-      : py_read(getattr(python_file_obj, "read", py::none()))
-      , py_write(getattr(python_file_obj, "write", py::none()))
-      , py_seek(getattr(python_file_obj, "seek", py::none()))
-      , py_tell(getattr(python_file_obj, "tell", py::none()))
+  explicit streambuf(nb::object &python_file_obj, size_t buffer_size_ = 0)
+      : py_read(getattr(python_file_obj, "read", nb::none()))
+      , py_write(getattr(python_file_obj, "write", nb::none()))
+      , py_seek(getattr(python_file_obj, "seek", nb::none()))
+      , py_tell(getattr(python_file_obj, "tell", nb::none()))
       , buffer_size(buffer_size_ != 0 ? buffer_size_ : default_buffer_size)
       , pos_of_read_buffer_end_in_py_file(0)
-      , pos_of_write_buffer_end_in_py_file(buffer_size)
+      , pos_of_write_buffer_end_in_py_file((off_type)buffer_size)
       , farthest_pptr(nullptr)
   {
     assert(buffer_size != 0);
     /* Some Python file objects (e.g. sys.stdout and sys.stdin)
        have non-functional seek and tell. If so, assign None to
        py_tell and py_seek.
      */
     if (!py_tell.is_none())
     {
       try
       {
         py_tell();
       }
-      catch (py::error_already_set &err)
+      catch (nb::python_error &err)
       {
-        py_tell = py::none();
-        py_seek = py::none();
+        py_tell = nb::none();
+        py_seek = nb::none();
         err.restore();
         PyErr_Clear();
       }
     }
 
     if (!py_write.is_none())
     {
@@ -199,100 +201,94 @@
     {
       // The first attempt at output will result in a call to overflow
       setp(nullptr, nullptr);
     }
 
     if (!py_tell.is_none())
     {
-      off_type py_pos = py_tell().cast<off_type>();
+      auto py_pos = nb::cast<off_type>(py_tell());
       pos_of_read_buffer_end_in_py_file = py_pos;
       pos_of_write_buffer_end_in_py_file = py_pos;
     }
   }
 
   /// C.f. C++ standard section 27.5.2.4.3
   /** It is essential to override this virtual function for the stream
       member function readsome to work correctly (c.f. 27.6.1.3, alinea 30)
    */
-  virtual std::streamsize showmanyc()
+  std::streamsize showmanyc() override
   {
     int_type const failure = traits_type::eof();
     int_type status = underflow();
     if (status == failure)
       return -1;
     return egptr() - gptr();
   }
 
   /// C.f. C++ standard section 27.5.2.4.3
-  virtual int_type underflow()
+  int_type underflow() override
   {
     int_type const failure = traits_type::eof();
     if (py_read.is_none())
     {
-      throw std::invalid_argument(
-          "That Python file object has no 'read' attribute");
+      throw std::invalid_argument("That Python file object has no 'read' attribute");
     }
-    read_buffer = py_read(buffer_size);
+    read_buffer = nb::cast<nb::bytes>(py_read(buffer_size));
     char *read_buffer_data;
-    py::ssize_t py_n_read;
-    if (PYBIND11_BYTES_AS_STRING_AND_SIZE(read_buffer.ptr(),
-            &read_buffer_data, &py_n_read) == -1)
+    Py_ssize_t py_n_read;
+    if (PyBytes_AsStringAndSize(read_buffer.ptr(), &read_buffer_data, &py_n_read) == -1)
     {
       setg(nullptr, nullptr, nullptr);
-      throw std::invalid_argument(
-          "The method 'read' of the Python file object "
-          "did not return a string.");
+      throw std::invalid_argument("The method 'read' of the Python file object "
+                                  "did not return a string.");
     }
     off_type n_read = py_n_read;
     pos_of_read_buffer_end_in_py_file += n_read;
     setg(read_buffer_data, read_buffer_data, read_buffer_data + n_read);
     // ^^^27.5.2.3.1 (4)
     if (n_read == 0)
       return failure;
     return traits_type::to_int_type(read_buffer_data[0]);
   }
 
   /// C.f. C++ standard section 27.5.2.4.5
-  virtual int_type overflow(int_type c = traits_type::eof())
+  int_type overflow(int_type c = traits_type::eof()) override
   {
     if (py_write.is_none())
     {
-      throw std::invalid_argument(
-          "That Python file object has no 'write' attribute");
+      throw std::invalid_argument("That Python file object has no 'write' attribute");
     }
     farthest_pptr = std::max(farthest_pptr, pptr());
     off_type n_written = farthest_pptr - pbase();
-    py::bytes chunk(pbase(), (py::ssize_t)n_written);
+    nb::bytes chunk(pbase(), (size_t)n_written);
     py_write(chunk);
     if (!traits_type::eq_int_type(c, traits_type::eof()))
     {
       char cs = traits_type::to_char_type(c);
-      py_write(py::bytes(&cs, 1));
+      py_write(nb::bytes(&cs, 1));
       n_written++;
     }
     if (n_written)
     {
       pos_of_write_buffer_end_in_py_file += n_written;
       setp(pbase(), epptr());
       // ^^^ 27.5.2.4.5 (5)
       farthest_pptr = pptr();
     }
-    return traits_type::eq_int_type(c, traits_type::eof())
-        ? traits_type::not_eof(c)
-        : c;
+    return traits_type::eq_int_type(c, traits_type::eof()) ? traits_type::not_eof(c) : c;
   }
 
   /// Update the python file to reflect the state of this stream buffer
   /** Empty the write buffer into the Python file object and set the seek
       position of the latter accordingly (C++ standard section 27.5.2.4.2).
       If there is no write buffer or it is empty, but there is a non-empty
       read buffer, set the Python file object seek position to the
       seek position in that read buffer.
   */
-  virtual int sync()
+  int sync() override
   {
     int result = 0;
     farthest_pptr = std::max(farthest_pptr, pptr());
     if (farthest_pptr && farthest_pptr > pbase())
     {
       off_type delta = pptr() - farthest_pptr;
       int_type status = overflow();
@@ -312,28 +308,27 @@
   /// C.f. C++ standard section 27.5.2.4.2
   /** This implementation is optimised to look whether the position is within
       the buffers, so as to avoid calling Python seek or tell. It is
       important for many applications that the overhead of calling into Python
       is avoided as much as possible (e.g. parsers which may do a lot of
       backtracking)
   */
-  virtual pos_type seekoff(off_type off, std::ios_base::seekdir way,
-      std::ios_base::openmode which = std::ios_base::in | std::ios_base::out)
+  pos_type seekoff(off_type off, std::ios_base::seekdir way,
+      std::ios_base::openmode which = std::ios_base::in | std::ios_base::out) override
   {
     /* In practice, "which" is either std::ios_base::in or out
        since we end up here because either seekp or seekg was called
        on the stream using this buffer. That simplifies the code
        in a few places.
     */
     int const failure = off_type(-1);
 
     if (py_seek.is_none())
     {
-      throw std::invalid_argument(
-          "That Python file object has no 'seek' attribute");
+      throw std::invalid_argument("That Python file object has no 'seek' attribute");
     }
 
     // we need the read buffer to contain something!
     if (which == std::ios_base::in && !gptr())
     {
       if (traits_type::eq_int_type(underflow(), traits_type::eof()))
       {
@@ -369,54 +364,50 @@
       {
         if (which == std::ios_base::in)
           off -= egptr() - gptr();
         else if (which == std::ios_base::out)
           off += pptr() - pbase();
       }
       py_seek(off, whence);
-      result = off_type(py_tell().cast<off_type>());
+      result = nb::cast<off_type>(py_tell());
       if (which == std::ios_base::in)
         underflow();
     }
     return result;
   }
 
   /// C.f. C++ standard section 27.5.2.4.2
-  virtual pos_type seekpos(pos_type sp,
-      std::ios_base::openmode which = std::ios_base::in | std::ios_base::out)
+  pos_type seekpos(pos_type sp,
+      std::ios_base::openmode which = std::ios_base::in | std::ios_base::out) override
   {
     return streambuf::seekoff(sp, std::ios_base::beg, which);
   }
 
   private:
-  py::object py_read, py_write, py_seek, py_tell;
+  nb::object py_read, py_write, py_seek, py_tell;
 
   size_t buffer_size;
 
   /* This is actually a Python bytes object and the actual read buffer is
      its internal data, i.e. an array of characters.
    */
-  py::bytes read_buffer;
+  nb::bytes read_buffer;
 
   /* A mere array of char's allocated on the heap at construction time and
      de-allocated only at destruction time.
   */
   std::vector<char> write_buffer;
 
-  off_type pos_of_read_buffer_end_in_py_file,
-      pos_of_write_buffer_end_in_py_file;
+  off_type pos_of_read_buffer_end_in_py_file, pos_of_write_buffer_end_in_py_file;
 
   // the farthest place the buffer has been written into
   char *farthest_pptr;
 
-  bool seekoff_without_calling_python(
-      off_type off,
-      std::ios_base::seekdir way,
-      std::ios_base::openmode which,
-      off_type &result)
+  bool seekoff_without_calling_python(off_type off, std::ios_base::seekdir way,
+      std::ios_base::openmode which, off_type &result)
   {
     // Buffer range and current position
     off_type buf_begin, buf_end, buf_cur, upper_bound;
     off_type pos_of_buffer_end_in_py_file;
     if (which == std::ios_base::in)
     {
       pos_of_buffer_end_in_py_file = pos_of_read_buffer_end_in_py_file;
@@ -474,162 +465,148 @@
     return true;
   }
 
   public:
   class istream : public std::istream
   {
 public:
-    istream(streambuf &buf)
+    explicit istream(streambuf &buf)
         : std::istream(&buf)
     {
       exceptions(std::ios_base::badbit);
     }
 
-    ~istream()
+    ~istream() override
     {
       if (this->good())
         this->sync();
     }
   };
 
   class ostream : public std::ostream
   {
 public:
-    ostream(streambuf &buf)
+    explicit ostream(streambuf &buf)
         : std::ostream(&buf)
     {
       exceptions(std::ios_base::badbit);
     }
 
-    ~ostream()
+    ~ostream() override
     {
       if (this->good())
         this->flush();
     }
   };
 };
 
 struct streambuf_capsule
 {
   streambuf python_streambuf;
 
-  streambuf_capsule(
-      py::object &python_file_obj,
-      size_t buffer_size = 0)
+  explicit streambuf_capsule(nb::object &python_file_obj, size_t buffer_size = 0)
       : python_streambuf(python_file_obj, buffer_size)
   {
   }
 };
 
 struct ostream : private streambuf_capsule, streambuf::ostream
 {
-  ostream(
-      py::object &python_file_obj,
-      size_t buffer_size = 0)
+  explicit ostream(nb::object &python_file_obj, size_t buffer_size = 0)
       : streambuf_capsule(python_file_obj, buffer_size)
       , streambuf::ostream(python_streambuf)
   {
   }
 
-  ~ostream()
+  ~ostream() override
   {
     if (this->good())
     {
       this->flush();
     }
   }
 };
 
 struct istream : private streambuf_capsule, streambuf::istream
 {
-  istream(
-      py::object &python_file_obj,
-      size_t buffer_size = 0)
+  explicit istream(nb::object &python_file_obj, size_t buffer_size = 0)
       : streambuf_capsule(python_file_obj, buffer_size)
       , streambuf::istream(python_streambuf)
   {
   }
 
-  ~istream()
+  ~istream() override
   {
     if (this->good())
     {
       this->sync();
     }
   }
 };
 
 } // namespace pystream
 
-namespace pybind11
+namespace nanobind::detail
 {
-namespace detail
+namespace nb = nanobind;
+
+template <> struct type_caster<std::istream>
 {
-  namespace py = pybind11;
+  using Value = std::istream;
+  template <typename T_> using Cast = movable_cast_t<T_>;
+  static constexpr auto Name = const_name("BinaryIO");
+  static constexpr bool IsClass = false;
 
-  template <>
-  struct type_caster<std::istream>
+  bool from_python(handle src, [[maybe_unused]] uint8_t flags, cleanup_list *) noexcept
   {
-public:
-    bool load(handle src, bool)
-    {
-      if (getattr(src, "read", py::none()).is_none())
-      {
-        return false;
-      }
+    if (!hasattr(src, "read"))
+      return false;
+    obj = nb::borrow(src);
+    value = std::make_unique<pystream::istream>(obj, 0);
+    return true;
+  }
 
-      obj = py::reinterpret_borrow<object>(src);
-      value = std::unique_ptr<pystream::istream>(new pystream::istream(obj, 0));
+  static handle from_cpp([[maybe_unused]] Value &value, rv_policy, cleanup_list *)
+  {
+    return none().release();
+  }
 
-      return true;
-    }
+  operator Value *() { return value.get(); }
+  operator Value &() { return *value; }
+  operator Value &&() && { return (Value &&)*value; }
 
-protected:
-    py::object obj;
-    std::unique_ptr<pystream::istream> value;
+  protected:
+  nb::object obj;
+  std::unique_ptr<pystream::istream> value;
+};
 
-public:
-    static constexpr auto name = _("io.BytesIO");
-    static handle cast(std::istream & /*src*/, return_value_policy /*policy*/, handle /*parent*/)
-    {
-      return none().release();
-    }
-    operator std::istream *() { return value.get(); }
-    operator std::istream &() { return *value; }
-    template <typename _T>
-    using cast_op_type = pybind11::detail::cast_op_type<_T>;
-  };
+template <> struct type_caster<std::ostream>
+{
+  using Value = std::ostream;
+  template <typename T_> using Cast = movable_cast_t<T_>;
+  static constexpr auto Name = const_name("BinaryIO");
+  static constexpr bool IsClass = false;
 
-  template <>
-  struct type_caster<std::ostream>
+  public:
+  bool from_python(handle src, [[maybe_unused]] uint8_t flags, cleanup_list *) noexcept
   {
-public:
-    bool load(handle src, bool)
-    {
-      if (getattr(src, "write", py::none()).is_none())
-      {
-        return false;
-      }
-
-      obj = py::reinterpret_borrow<object>(src);
-      value = std::unique_ptr<pystream::ostream>(new pystream::ostream(obj, 0));
+    if (!hasattr(src, "write"))
+      return false;
+    obj = nb::borrow(src);
+    value = std::make_unique<pystream::ostream>(obj, 0);
+    return true;
+  }
 
-      return true;
-    }
+  static handle from_cpp([[maybe_unused]] Value &value, rv_policy, cleanup_list *)
+  {
+    return none().release();
+  }
 
-protected:
-    py::object obj;
-    std::unique_ptr<pystream::ostream> value;
+  operator Value *() { return value.get(); }
+  operator Value &() { return *value; }
+  operator Value &&() && { return (Value &&)*value; }
 
-public:
-    static constexpr auto name = _("io.BytesIO");
-    static handle cast(std::ostream & /*src*/, return_value_policy /*policy*/, handle /*parent*/)
-    {
-      return none().release();
-    }
-    operator std::ostream *() { return value.get(); }
-    operator std::ostream &() { return *value; }
-    template <typename _T>
-    using cast_op_type = pybind11::detail::cast_op_type<_T>;
-  };
-} // namespace detail
-} // namespace pybind11
+  protected:
+  nb::object obj;
+  std::unique_ptr<pystream::ostream> value;
+};
+} // namespace nanobind::detail
```

### Comparing `ncompress-1.0.0/test/test_ncompress.py` & `ncompress-1.0.1/test/test_ncompress.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     assert decompress(BytesIO(sample_compressed)) == sample_data
 
 
 def test_empty_input(sample_data):
     assert decompress(compress(b"")) == b""
     with pytest.raises(ValueError):
         decompress(b"")
-    with pytest.raises(TypeError):
-        compress()
-    with pytest.raises(TypeError):
-        decompress()
+
+    assert decompress(BytesIO(compress(b""))) == b""
+    with pytest.raises(ValueError):
+        decompress(BytesIO(b""))
 
 
 def test_corrupted_input(sample_compressed):
     sample = sample_compressed
     for x in [
         b"123",
         sample[1:],
@@ -79,19 +79,22 @@
     ]:
         with pytest.raises(ValueError) as ex:
             decompress(x)
         assert ("not in LZW-compressed format" in str(ex.value) or
                 "corrupt input - " in str(ex.value))
 
 
-def test_str(sample_data, sample_compressed):
+@pytest.mark.parametrize("args",
+                         [["abc"], [0], [None], []],
+                         ids=["str", "int", "None", "empty"])
+def test_invalid_input(args):
     with pytest.raises(TypeError):
-        compress(sample_data.decode("latin1", errors="replace"))
+        compress(*args)
     with pytest.raises(TypeError):
-        decompress(sample_compressed.decode("latin1", errors="replace"))
+        decompress(*args)
 
 
 def test_closed_input(sample_data, sample_compressed):
     expected = "I/O operation on closed file."
     with pytest.raises(ValueError) as ex:
         stream = BytesIO(sample_data)
         stream.close()
```

