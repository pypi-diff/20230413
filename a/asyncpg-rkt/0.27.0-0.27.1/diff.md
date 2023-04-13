# Comparing `tmp/asyncpg-rkt-0.27.0.tar.gz` & `tmp/asyncpg-rkt-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpg-rkt-0.27.0.tar", last modified: Wed Feb  8 20:20:09 2023, max compression
+gzip compressed data, was "asyncpg-rkt-0.27.1.tar", last modified: Thu Apr 13 17:40:02 2023, max compression
```

## Comparing `asyncpg-rkt-0.27.0.tar` & `asyncpg-rkt-0.27.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.562219 asyncpg-rkt-0.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-02-08 20:20:09.562219 asyncpg-rkt-0.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.542219 asyncpg-rkt-0.27.0/asyncpg/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.542219 asyncpg-rkt-0.27.0/asyncpg/_testbase/
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/_testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/_testbase/fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-08 20:20:09.562219 asyncpg-rkt-0.27.0/asyncpg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30096 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/connect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86027 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/connresource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.542219 asyncpg-rkt-0.27.0/asyncpg/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/exceptions/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/introspection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.546219 asyncpg-rkt-0.27.0/asyncpg/pgproto/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/array_writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/array_writer.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/buffer.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.546219 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/bits.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/bytea.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/context.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/datetime.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/float.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/geometry.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/hstore.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/int.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/json.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/jsonpath.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/misc.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/network.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/numeric.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/pg_snapshot.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/text.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/tid.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/uuid.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/consts.pxi
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/cpythonunsafe.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/cpythonx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/debug.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/frb.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/hton.h
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/hton.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/memalign.h
--rw-r--r--   0 runner    (1001) docker     (123)  2204445 2023-02-08 20:20:07.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/pgproto.c
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/pgproto.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/pgproto.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/tohex.h
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/tohex.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/utf8_to_ucs4.h
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pgproto/uuid.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    39219 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/prepared_stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.554220 asyncpg-rkt-0.27.0/asyncpg/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.554220 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/array.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/base.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    33079 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/base.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/pgproto.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/range.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/record.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/textutils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/consts.pxi
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/coreproto.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/coreproto.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/cpythonx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/encodings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/pgtypes.pxi
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/prepared_stmt.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/prepared_stmt.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  4531343 2023-02-08 20:20:09.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/protocol.c
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/protocol.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    34375 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/protocol.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.554220 asyncpg-rkt-0.27.0/asyncpg/protocol/record/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/record/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    27538 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/record/recordobj.c
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/record/recordobj.h
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/scram.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/scram.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/settings.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/protocol/settings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/rkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/serverversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/asyncpg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.554220 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-02-08 20:20:05.000000 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-02-08 20:20:09.000000 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:20:05.000000 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:20:05.000000 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-08 20:20:05.000000 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-08 20:20:05.000000 asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.558220 asyncpg-rkt-0.27.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.558220 asyncpg-rkt-0.27.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.558220 asyncpg-rkt-0.27.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23944 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/performance.png
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 20:20:09.562219 asyncpg-rkt-0.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.558220 asyncpg-rkt-0.27.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:20:09.562219 asyncpg-rkt-0.27.0/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/ca.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/ca.crl.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/ca.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/client.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/client.csr.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/client.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/client.key.protected.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/client_ca.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/client_ca.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/server.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/certs/server.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test__environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test__sourcecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_adversity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_cache_invalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    67068 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_numpy_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    36764 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_rkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-08 20:19:56.000000 asyncpg-rkt-0.27.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.172517 asyncpg-rkt-0.27.1/asyncpg/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.172517 asyncpg-rkt-0.27.1/asyncpg/_testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/_testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/_testbase/fuzzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/asyncpg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30096 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/connect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86027 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/connresource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.172517 asyncpg-rkt-0.27.1/asyncpg/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/exceptions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/introspection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.176518 asyncpg-rkt-0.27.1/asyncpg/pgproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.180518 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bits.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bytea.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/datetime.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/float.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/geometry.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/hstore.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/int.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/json.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/jsonpath.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/misc.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/network.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/numeric.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/pg_snapshot.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/text.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/tid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/uuid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/consts.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonunsafe.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/debug.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/frb.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/memalign.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2206477 2023-04-13 17:40:00.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.c
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/tohex.h
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/tohex.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/utf8_to_ucs4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/uuid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    39219 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/prepared_stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/array.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    33079 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/pgproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/range.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/record.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/textutils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/consts.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/cpythonx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/encodings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/pgtypes.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  4537051 2023-04-13 17:40:02.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    34375 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg/protocol/record/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/record/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    27538 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/rkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/serverversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-13 17:40:02.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23944 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/performance.png
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.192519 asyncpg-rkt-0.27.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/ca.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/ca.crl.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/ca.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.csr.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.key.protected.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client_ca.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client_ca.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/server.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/server.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test__environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test__sourcecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_adversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_cache_invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67068 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_numpy_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36764 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_rkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_utils.py
```

### Comparing `asyncpg-rkt-0.27.0/LICENSE` & `asyncpg-rkt-0.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/Makefile` & `asyncpg-rkt-0.27.1/Makefile`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/PKG-INFO` & `asyncpg-rkt-0.27.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-rkt
-Version: 0.27.0
+Version: 0.27.1
 Summary: An asyncio PostgreSQL driver that returns numpy arrays
 Home-page: https://github.com/MagicStack/asyncpg
 Author: MagicStack Inc
 Author-email: hello@magic.io
 License: Apache License, Version 2.0
 Platform: macOS
 Platform: POSIX
```

### Comparing `asyncpg-rkt-0.27.0/README.rst` & `asyncpg-rkt-0.27.1/README.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/__init__.py` & `asyncpg-rkt-0.27.1/asyncpg/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/_testbase/__init__.py` & `asyncpg-rkt-0.27.1/asyncpg/_testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/_testbase/fuzzer.py` & `asyncpg-rkt-0.27.1/asyncpg/_testbase/fuzzer.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/_version.py` & `asyncpg-rkt-0.27.1/asyncpg/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # The commit message MUST contain a properly formatted release
 # log, and the commit must be signed.
 #
 # The release automation will: build and test the packages for the
 # supported platforms, publish the packages on PyPI, merge the PR
 # to the target branch, create a Git tag pointing to the commit.
 
-__version__ = '0.27.0'
+__version__ = '0.27.1'
```

### Comparing `asyncpg-rkt-0.27.0/asyncpg/cluster.py` & `asyncpg-rkt-0.27.1/asyncpg/cluster.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/compat.py` & `asyncpg-rkt-0.27.1/asyncpg/compat.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/connect_utils.py` & `asyncpg-rkt-0.27.1/asyncpg/connect_utils.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/connection.py` & `asyncpg-rkt-0.27.1/asyncpg/connection.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/connresource.py` & `asyncpg-rkt-0.27.1/asyncpg/connresource.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/cursor.py` & `asyncpg-rkt-0.27.1/asyncpg/cursor.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/exceptions/__init__.py` & `asyncpg-rkt-0.27.1/asyncpg/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/exceptions/_base.py` & `asyncpg-rkt-0.27.1/asyncpg/exceptions/_base.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/introspection.py` & `asyncpg-rkt-0.27.1/asyncpg/introspection.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/array_writer.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/array_writer.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/buffer.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/buffer.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/__init__.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/__init__.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/bits.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bits.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/bytea.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bytea.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/datetime.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/datetime.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/float.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/float.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/geometry.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/geometry.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/hstore.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/hstore.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/int.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/int.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/json.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/json.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/jsonpath.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/jsonpath.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/misc.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/misc.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/network.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/network.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/numeric.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/numeric.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/pg_snapshot.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/pg_snapshot.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/text.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/text.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/tid.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/tid.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/codecs/uuid.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/uuid.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/cpythonunsafe.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonunsafe.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/cpythonx.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonx.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/frb.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/frb.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/hton.h` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/hton.pxd` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/pgproto.c` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "asyncpg/pgproto/debug.h",
             "asyncpg/pgproto/memalign.h",
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -228,15 +228,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -267,15 +267,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1042,20 +1042,20 @@
   "asyncpg/pgproto/./codecs/hstore.pyx",
   "asyncpg/pgproto/./codecs/misc.pyx",
   "asyncpg/pgproto/./codecs/network.pyx",
   "asyncpg/pgproto/./codecs/tid.pyx",
   "asyncpg/pgproto/./codecs/pg_snapshot.pyx",
   "asyncpg/pgproto/./buffer.pxd",
   ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/datetime.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/datetime.pxd",
   "asyncpg/pgproto/pgproto.pyx",
   "asyncpg/pgproto/././array_writer.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
 };
 
 /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
@@ -2431,20 +2431,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
@@ -46003,15 +46011,16 @@
   }
   if (__Pyx_SetVtable(__pyx_type_7asyncpg_7pgproto_7pgproto_ReadBuffer.tp_dict, __pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer) < 0) __PYX_ERR(1, 241, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ReadBuffer, (PyObject *)&__pyx_type_7asyncpg_7pgproto_7pgproto_ReadBuffer) < 0) __PYX_ERR(1, 241, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7asyncpg_7pgproto_7pgproto_ReadBuffer) < 0) __PYX_ERR(1, 241, __pyx_L1_error)
   __pyx_ptype_7asyncpg_7pgproto_7pgproto_ReadBuffer = &__pyx_type_7asyncpg_7pgproto_7pgproto_ReadBuffer;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(26, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_dtype) __PYX_ERR(26, 34, __pyx_L1_error)
   __pyx_type_7asyncpg_7pgproto_7pgproto_DTypeError.tp_base = (&((PyTypeObject*)PyExc_Exception)[0]);
   if (PyType_Ready(&__pyx_type_7asyncpg_7pgproto_7pgproto_DTypeError) < 0) __PYX_ERR(26, 59, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7asyncpg_7pgproto_7pgproto_DTypeError.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7asyncpg_7pgproto_7pgproto_DTypeError.tp_dictoffset && __pyx_type_7asyncpg_7pgproto_7pgproto_DTypeError.tp_getattro == PyObject_GenericGetAttr)) {
@@ -46107,75 +46116,97 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(27, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(27, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(28, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(28, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(29, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(29, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(24, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Date),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(24, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Time),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(24, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_DateTime),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(24, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Delta),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(24, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_TZInfo),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(24, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(23, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(23, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(23, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(23, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(23, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(23, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(23, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(23, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(23, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(23, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(23, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(23, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(23, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(23, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(23, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(23, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -48231,28 +48262,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -51086,44 +51117,62 @@
     return ret;
 }
 
 /* TypeImport */
     #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/pgproto.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/tohex.h` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/tohex.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/types.py` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/types.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/utf8_to_ucs4.h` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/utf8_to_ucs4.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pgproto/uuid.pyx` & `asyncpg-rkt-0.27.1/asyncpg/pgproto/uuid.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/pool.py` & `asyncpg-rkt-0.27.1/asyncpg/pool.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/prepared_stmt.py` & `asyncpg-rkt-0.27.1/asyncpg/prepared_stmt.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/array.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/array.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/base.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/base.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/pgproto.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/pgproto.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/range.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/range.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/record.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/record.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/codecs/textutils.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/textutils.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/coreproto.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/coreproto.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/cpythonx.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/cpythonx.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/encodings.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/encodings.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/pgtypes.pxi` & `asyncpg-rkt-0.27.1/asyncpg/protocol/pgtypes.pxi`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/prepared_stmt.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/prepared_stmt.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -386,22 +386,33 @@
                 frb_set_len(&rbuf, bl - flen)
 
         if frb_get_len(&rbuf) != 0:
             raise BufferError(f'unexpected trailing {frb_get_len(&rbuf)} bytes in buffer')
 
     cdef _parse_dtype(self):
         cdef str query = self.query
-        if not query.startswith("--🚀"):
+        pos = 0
+        while query.startswith("--", pos):
+            if query.startswith("🚀", pos + 2):
+                pos += 3
+                break
+            else:
+                pos = query.find("\n", pos + 2)
+                if pos >= 0:
+                    pos += 1
+                else:
+                    pos = len(query)
+        else:
             self.dtype = None
             return
-        end = query.find("🚀\n", 3)
-        if end == -1:
+        end = query.find("🚀\n", pos)
+        if end < 0:
             self.dtype = None
             return
-        self.dtype = pickle.loads(bytes.fromhex(query[3:end]))
+        self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
         assert isinstance(self.dtype, np_dtype)
         self.query = query[end + 2:]
 
 cdef _decode_parameters_desc(object desc):
     cdef:
         ReadBuffer reader
         int16_t nparams
```

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/protocol.c` & `asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "asyncpg/pgproto/debug.h"
         ],
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1031,17 +1031,17 @@
   "asyncpg/protocol/scram.pxd",
   "asyncpg/protocol/coreproto.pxd",
   "asyncpg/protocol/prepared_stmt.pxd",
   "asyncpg/protocol/protocol.pxd",
   "asyncpg/pgproto/./frb.pxd",
   "asyncpg/pgproto/./buffer.pxd",
   ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
-  ".eggs/Cython-0.29.33-py3.11-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
+  ".eggs/Cython-0.29.34-py3.11-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
   "asyncpg/pgproto/././array_writer.pxd",
   "asyncpg/protocol/pgtypes.pxi",
 };
 
 /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
@@ -3541,17 +3541,14 @@
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char);
 
 /* unicode_tailmatch.proto */
 static int __Pyx_PyUnicode_Tailmatch(
     PyObject* s, PyObject* substr, Py_ssize_t start, Py_ssize_t end, int direction);
 
-/* PyIntCompare.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
-
 /* PyUnicode_Substring.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Substring(
             PyObject* text, Py_ssize_t start, Py_ssize_t stop);
 
 /* RaiseKeywordRequired.proto */
 static void __Pyx_RaiseKeywordRequired(const char* func_name, PyObject* kw_name);
 
@@ -3793,20 +3790,28 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* PatchInspect.proto */
 static PyObject* __Pyx_patch_inspect(PyObject* module);
@@ -4643,16 +4648,18 @@
 static const char __pyx_k__41[] = ".";
 static const char __pyx_k__42[] = ", ";
 static const char __pyx_k__43[] = "'{}'";
 static const char __pyx_k__44[] = "$";
 static const char __pyx_k__45[] = ": ";
 static const char __pyx_k__47[] = "...";
 static const char __pyx_k__48[] = " (";
-static const char __pyx_k__49[] = "--\360\237\232\200";
-static const char __pyx_k__50[] = "\360\237\232\200\n";
+static const char __pyx_k__49[] = "--";
+static const char __pyx_k__50[] = "\360\237\232\200";
+static const char __pyx_k__51[] = "\n";
+static const char __pyx_k__52[] = "\360\237\232\200\n";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_alt[] = "alt";
 static const char __pyx_k_any[] = "any";
 static const char __pyx_k_big[] = "big";
 static const char __pyx_k_bit[] = "bit";
 static const char __pyx_k_box[] = "box";
 static const char __pyx_k_c_2[] = "c=";
@@ -5439,14 +5446,16 @@
 static PyObject *__pyx_kp_u__43;
 static PyObject *__pyx_kp_u__44;
 static PyObject *__pyx_kp_u__45;
 static PyObject *__pyx_kp_u__47;
 static PyObject *__pyx_kp_u__48;
 static PyObject *__pyx_kp_u__49;
 static PyObject *__pyx_kp_u__50;
+static PyObject *__pyx_kp_u__51;
+static PyObject *__pyx_kp_u__52;
 static PyObject *__pyx_kp_u__9;
 static PyObject *__pyx_kp_u_a_sized_iterable_container_expec;
 static PyObject *__pyx_n_s_abc;
 static PyObject *__pyx_n_u_abc;
 static PyObject *__pyx_n_s_abort;
 static PyObject *__pyx_n_u_abstime;
 static PyObject *__pyx_n_u_aclitem;
@@ -6186,14 +6195,15 @@
 static PyObject *__pyx_tp_new_7asyncpg_8protocol_8protocol___pyx_scope_struct_17_close(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_7asyncpg_8protocol_8protocol___pyx_scope_struct_18__wait_for_cancellation(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_pop = {0, &__pyx_n_s_pop, 0, 0, 0};
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
+static PyObject *__pyx_int_3;
 static PyObject *__pyx_int_4;
 static PyObject *__pyx_int_6;
 static PyObject *__pyx_int_16;
 static PyObject *__pyx_int_17;
 static PyObject *__pyx_int_18;
 static PyObject *__pyx_int_19;
 static PyObject *__pyx_int_20;
@@ -6300,15 +6310,14 @@
 static PyObject *__pyx_int_71763376;
 static PyObject *__pyx_int_120810133;
 static PyObject *__pyx_int_165592117;
 static PyObject *__pyx_int_172872881;
 static PyObject *__pyx_int_228230485;
 static PyObject *__pyx_int_245762207;
 static PyObject *__pyx_int_263996099;
-static PyObject *__pyx_int_neg_1;
 static enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat __pyx_k_;
 static PyObject *__pyx_k__10;
 static PyObject *__pyx_k__11;
 static enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat __pyx_k__13;
 static enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat __pyx_k__14;
 static enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat __pyx_k__15;
 static PyObject *__pyx_slice__8;
@@ -6333,42 +6342,42 @@
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__39;
 static PyObject *__pyx_tuple__40;
-static PyObject *__pyx_tuple__51;
-static PyObject *__pyx_tuple__52;
 static PyObject *__pyx_tuple__53;
 static PyObject *__pyx_tuple__54;
 static PyObject *__pyx_tuple__55;
 static PyObject *__pyx_tuple__56;
 static PyObject *__pyx_tuple__57;
 static PyObject *__pyx_tuple__58;
 static PyObject *__pyx_tuple__59;
 static PyObject *__pyx_tuple__60;
 static PyObject *__pyx_tuple__61;
+static PyObject *__pyx_tuple__62;
 static PyObject *__pyx_tuple__63;
 static PyObject *__pyx_tuple__65;
 static PyObject *__pyx_tuple__67;
 static PyObject *__pyx_tuple__69;
 static PyObject *__pyx_tuple__71;
 static PyObject *__pyx_tuple__73;
 static PyObject *__pyx_tuple__75;
 static PyObject *__pyx_tuple__77;
-static PyObject *__pyx_codeobj__62;
+static PyObject *__pyx_tuple__79;
 static PyObject *__pyx_codeobj__64;
 static PyObject *__pyx_codeobj__66;
 static PyObject *__pyx_codeobj__68;
 static PyObject *__pyx_codeobj__70;
 static PyObject *__pyx_codeobj__72;
 static PyObject *__pyx_codeobj__74;
 static PyObject *__pyx_codeobj__76;
 static PyObject *__pyx_codeobj__78;
+static PyObject *__pyx_codeobj__80;
 /* Late includes */
 
 /* "asyncpg/protocol/encodings.pyx":62
  * 
  * 
  * cdef get_python_encoding(pg_encoding):             # <<<<<<<<<<<<<<
  *     return ENCODINGS_MAP.get(pg_encoding.lower(), pg_encoding.lower())
@@ -56636,24 +56645,25 @@
 }
 
 /* "asyncpg/protocol/prepared_stmt.pyx":391
  *             raise BufferError(f'unexpected trailing {frb_get_len(&rbuf)} bytes in buffer')
  * 
  *     cdef _parse_dtype(self):             # <<<<<<<<<<<<<<
  *         cdef str query = self.query
- *         if not query.startswith("--"):
+ *         pos = 0
  */
 
 static PyObject *__pyx_f_7asyncpg_8protocol_8protocol_22PreparedStatementState__parse_dtype(struct __pyx_obj_7asyncpg_8protocol_8protocol_PreparedStatementState *__pyx_v_self) {
   PyObject *__pyx_v_query = 0;
+  PyObject *__pyx_v_pos = NULL;
   PyObject *__pyx_v_end = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
@@ -56663,177 +56673,318 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_dtype", 0);
 
   /* "asyncpg/protocol/prepared_stmt.pyx":392
  * 
  *     cdef _parse_dtype(self):
  *         cdef str query = self.query             # <<<<<<<<<<<<<<
- *         if not query.startswith("--"):
- *             self.dtype = None
+ *         pos = 0
+ *         while query.startswith("--", pos):
  */
   __pyx_t_1 = __pyx_v_self->query;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_query = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/prepared_stmt.pyx":393
  *     cdef _parse_dtype(self):
  *         cdef str query = self.query
- *         if not query.startswith("--"):             # <<<<<<<<<<<<<<
+ *         pos = 0             # <<<<<<<<<<<<<<
+ *         while query.startswith("--", pos):
+ *             if query.startswith("", pos + 2):
+ */
+  __Pyx_INCREF(__pyx_int_0);
+  __pyx_v_pos = __pyx_int_0;
+
+  /* "asyncpg/protocol/prepared_stmt.pyx":394
+ *         cdef str query = self.query
+ *         pos = 0
+ *         while query.startswith("--", pos):             # <<<<<<<<<<<<<<
+ *             if query.startswith("", pos + 2):
+ *                 pos += 3
+ */
+  while (1) {
+    if (unlikely(__pyx_v_query == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
+      __PYX_ERR(7, 394, __pyx_L1_error)
+    }
+    __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_v_pos); if (unlikely((__pyx_t_2 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 394, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Tailmatch(__pyx_v_query, __pyx_kp_u__49, __pyx_t_2, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(7, 394, __pyx_L1_error)
+    if (!(__pyx_t_3 != 0)) break;
+
+    /* "asyncpg/protocol/prepared_stmt.pyx":395
+ *         pos = 0
+ *         while query.startswith("--", pos):
+ *             if query.startswith("", pos + 2):             # <<<<<<<<<<<<<<
+ *                 pos += 3
+ *                 break
+ */
+    if (unlikely(__pyx_v_query == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
+      __PYX_ERR(7, 395, __pyx_L1_error)
+    }
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_pos, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 395, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 395, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_3 = __Pyx_PyUnicode_Tailmatch(__pyx_v_query, __pyx_kp_u__50, __pyx_t_2, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(7, 395, __pyx_L1_error)
+    if ((__pyx_t_3 != 0)) {
+
+      /* "asyncpg/protocol/prepared_stmt.pyx":396
+ *         while query.startswith("--", pos):
+ *             if query.startswith("", pos + 2):
+ *                 pos += 3             # <<<<<<<<<<<<<<
+ *                 break
+ *             else:
+ */
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_pos, __pyx_int_3, 3, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 396, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF_SET(__pyx_v_pos, __pyx_t_1);
+      __pyx_t_1 = 0;
+
+      /* "asyncpg/protocol/prepared_stmt.pyx":397
+ *             if query.startswith("", pos + 2):
+ *                 pos += 3
+ *                 break             # <<<<<<<<<<<<<<
+ *             else:
+ *                 pos = query.find("\n", pos + 2)
+ */
+      goto __pyx_L4_break;
+
+      /* "asyncpg/protocol/prepared_stmt.pyx":395
+ *         pos = 0
+ *         while query.startswith("--", pos):
+ *             if query.startswith("", pos + 2):             # <<<<<<<<<<<<<<
+ *                 pos += 3
+ *                 break
+ */
+    }
+
+    /* "asyncpg/protocol/prepared_stmt.pyx":399
+ *                 break
+ *             else:
+ *                 pos = query.find("\n", pos + 2)             # <<<<<<<<<<<<<<
+ *                 if pos >= 0:
+ *                     pos += 1
+ */
+    /*else*/ {
+      if (unlikely(__pyx_v_query == Py_None)) {
+        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "find");
+        __PYX_ERR(7, 399, __pyx_L1_error)
+      }
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_pos, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 399, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 399, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_4 = PyUnicode_Find(__pyx_v_query, __pyx_kp_u__51, __pyx_t_2, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-2))) __PYX_ERR(7, 399, __pyx_L1_error)
+      __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 399, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF_SET(__pyx_v_pos, __pyx_t_1);
+      __pyx_t_1 = 0;
+
+      /* "asyncpg/protocol/prepared_stmt.pyx":400
+ *             else:
+ *                 pos = query.find("\n", pos + 2)
+ *                 if pos >= 0:             # <<<<<<<<<<<<<<
+ *                     pos += 1
+ *                 else:
+ */
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_pos, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 400, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(7, 400, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (__pyx_t_3) {
+
+        /* "asyncpg/protocol/prepared_stmt.pyx":401
+ *                 pos = query.find("\n", pos + 2)
+ *                 if pos >= 0:
+ *                     pos += 1             # <<<<<<<<<<<<<<
+ *                 else:
+ *                     pos = len(query)
+ */
+        __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_pos, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 401, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF_SET(__pyx_v_pos, __pyx_t_1);
+        __pyx_t_1 = 0;
+
+        /* "asyncpg/protocol/prepared_stmt.pyx":400
+ *             else:
+ *                 pos = query.find("\n", pos + 2)
+ *                 if pos >= 0:             # <<<<<<<<<<<<<<
+ *                     pos += 1
+ *                 else:
+ */
+        goto __pyx_L6;
+      }
+
+      /* "asyncpg/protocol/prepared_stmt.pyx":403
+ *                     pos += 1
+ *                 else:
+ *                     pos = len(query)             # <<<<<<<<<<<<<<
+ *         else:
  *             self.dtype = None
- *             return
  */
-  if (unlikely(__pyx_v_query == Py_None)) {
-    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
-    __PYX_ERR(7, 393, __pyx_L1_error)
+      /*else*/ {
+        if (unlikely(__pyx_v_query == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+          __PYX_ERR(7, 403, __pyx_L1_error)
+        }
+        __pyx_t_4 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_query); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(7, 403, __pyx_L1_error)
+        __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 403, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF_SET(__pyx_v_pos, __pyx_t_1);
+        __pyx_t_1 = 0;
+      }
+      __pyx_L6:;
+    }
   }
-  __pyx_t_2 = __Pyx_PyUnicode_Tailmatch(__pyx_v_query, __pyx_kp_u__49, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(7, 393, __pyx_L1_error)
-  __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
-  if (__pyx_t_3) {
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":394
- *         cdef str query = self.query
- *         if not query.startswith("--"):
+  /* "asyncpg/protocol/prepared_stmt.pyx":405
+ *                     pos = len(query)
+ *         else:
  *             self.dtype = None             # <<<<<<<<<<<<<<
  *             return
- *         end = query.find("\n", 3)
+ *         end = query.find("\n", pos)
  */
+  /*else*/ {
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->dtype);
     __Pyx_DECREF(__pyx_v_self->dtype);
     __pyx_v_self->dtype = Py_None;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":395
- *         if not query.startswith("--"):
+    /* "asyncpg/protocol/prepared_stmt.pyx":406
+ *         else:
  *             self.dtype = None
  *             return             # <<<<<<<<<<<<<<
- *         end = query.find("\n", 3)
- *         if end == -1:
+ *         end = query.find("\n", pos)
+ *         if end < 0:
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
-
-    /* "asyncpg/protocol/prepared_stmt.pyx":393
- *     cdef _parse_dtype(self):
- *         cdef str query = self.query
- *         if not query.startswith("--"):             # <<<<<<<<<<<<<<
- *             self.dtype = None
- *             return
- */
   }
+  __pyx_L4_break:;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":396
+  /* "asyncpg/protocol/prepared_stmt.pyx":407
  *             self.dtype = None
  *             return
- *         end = query.find("\n", 3)             # <<<<<<<<<<<<<<
- *         if end == -1:
+ *         end = query.find("\n", pos)             # <<<<<<<<<<<<<<
+ *         if end < 0:
  *             self.dtype = None
  */
   if (unlikely(__pyx_v_query == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "find");
-    __PYX_ERR(7, 396, __pyx_L1_error)
+    __PYX_ERR(7, 407, __pyx_L1_error)
   }
-  __pyx_t_4 = PyUnicode_Find(__pyx_v_query, __pyx_kp_u__50, 3, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-2))) __PYX_ERR(7, 396, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 396, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_v_pos); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 407, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_Find(__pyx_v_query, __pyx_kp_u__52, __pyx_t_4, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-2))) __PYX_ERR(7, 407, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_end = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":397
+  /* "asyncpg/protocol/prepared_stmt.pyx":408
  *             return
- *         end = query.find("\n", 3)
- *         if end == -1:             # <<<<<<<<<<<<<<
+ *         end = query.find("\n", pos)
+ *         if end < 0:             # <<<<<<<<<<<<<<
  *             self.dtype = None
  *             return
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_end, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 397, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(7, 397, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_end, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 408, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(7, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_3) {
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":398
- *         end = query.find("\n", 3)
- *         if end == -1:
+    /* "asyncpg/protocol/prepared_stmt.pyx":409
+ *         end = query.find("\n", pos)
+ *         if end < 0:
  *             self.dtype = None             # <<<<<<<<<<<<<<
  *             return
- *         self.dtype = pickle.loads(bytes.fromhex(query[3:end]))
+ *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->dtype);
     __Pyx_DECREF(__pyx_v_self->dtype);
     __pyx_v_self->dtype = Py_None;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":399
- *         if end == -1:
+    /* "asyncpg/protocol/prepared_stmt.pyx":410
+ *         if end < 0:
  *             self.dtype = None
  *             return             # <<<<<<<<<<<<<<
- *         self.dtype = pickle.loads(bytes.fromhex(query[3:end]))
+ *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
  *         assert isinstance(self.dtype, np_dtype)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":397
+    /* "asyncpg/protocol/prepared_stmt.pyx":408
  *             return
- *         end = query.find("\n", 3)
- *         if end == -1:             # <<<<<<<<<<<<<<
+ *         end = query.find("\n", pos)
+ *         if end < 0:             # <<<<<<<<<<<<<<
  *             self.dtype = None
  *             return
  */
   }
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":400
+  /* "asyncpg/protocol/prepared_stmt.pyx":411
  *             self.dtype = None
  *             return
- *         self.dtype = pickle.loads(bytes.fromhex(query[3:end]))             # <<<<<<<<<<<<<<
+ *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))             # <<<<<<<<<<<<<<
  *         assert isinstance(self.dtype, np_dtype)
  *         self.query = query[end + 2:]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pickle); if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 400, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pickle); if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_loads); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 400, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_loads); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyBytes_Type)), __pyx_n_s_fromhex); if (unlikely(!__pyx_t_7)) __PYX_ERR(7, 400, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyBytes_Type)), __pyx_n_s_fromhex); if (unlikely(!__pyx_t_7)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (unlikely(__pyx_v_query == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(7, 400, __pyx_L1_error)
+    __PYX_ERR(7, 411, __pyx_L1_error)
   }
+  __Pyx_INCREF(__pyx_v_pos);
+  __pyx_t_8 = __pyx_v_pos;
+  __pyx_t_3 = (__pyx_t_8 == Py_None);
+  if (__pyx_t_3) {
+    __pyx_t_2 = 0;
+  } else {
+    __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_t_8); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 411, __pyx_L1_error)
+    __pyx_t_2 = __pyx_t_4;
+  }
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_INCREF(__pyx_v_end);
   __pyx_t_8 = __pyx_v_end;
   __pyx_t_3 = (__pyx_t_8 == Py_None);
   if (__pyx_t_3) {
     __pyx_t_4 = PY_SSIZE_T_MAX;
   } else {
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_8); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 400, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_8); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 411, __pyx_L1_error)
     __pyx_t_4 = __pyx_t_9;
   }
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyUnicode_Substring(__pyx_v_query, 3, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(7, 400, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_Substring(__pyx_v_query, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_5 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_10, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 400, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -56841,78 +56992,78 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 400, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->dtype);
   __Pyx_DECREF(__pyx_v_self->dtype);
   __pyx_v_self->dtype = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":401
+  /* "asyncpg/protocol/prepared_stmt.pyx":412
  *             return
- *         self.dtype = pickle.loads(bytes.fromhex(query[3:end]))
+ *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
  *         assert isinstance(self.dtype, np_dtype)             # <<<<<<<<<<<<<<
  *         self.query = query[end + 2:]
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     __pyx_t_1 = __pyx_v_self->dtype;
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_TypeCheck(__pyx_t_1, __pyx_ptype_5numpy_dtype); 
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!(__pyx_t_3 != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(7, 401, __pyx_L1_error)
+      __PYX_ERR(7, 412, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":402
- *         self.dtype = pickle.loads(bytes.fromhex(query[3:end]))
+  /* "asyncpg/protocol/prepared_stmt.pyx":413
+ *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
  *         assert isinstance(self.dtype, np_dtype)
  *         self.query = query[end + 2:]             # <<<<<<<<<<<<<<
  * 
  * cdef _decode_parameters_desc(object desc):
  */
   if (unlikely(__pyx_v_query == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(7, 402, __pyx_L1_error)
+    __PYX_ERR(7, 413, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_end, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 402, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_end, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_t_1 == Py_None);
   if (__pyx_t_3) {
     __pyx_t_4 = 0;
   } else {
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 402, __pyx_L1_error)
-    __pyx_t_4 = __pyx_t_9;
+    __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 413, __pyx_L1_error)
+    __pyx_t_4 = __pyx_t_2;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_query, __pyx_t_4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 402, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_query, __pyx_t_4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->query);
   __Pyx_DECREF(__pyx_v_self->query);
   __pyx_v_self->query = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/prepared_stmt.pyx":391
  *             raise BufferError(f'unexpected trailing {frb_get_len(&rbuf)} bytes in buffer')
  * 
  *     cdef _parse_dtype(self):             # <<<<<<<<<<<<<<
  *         cdef str query = self.query
- *         if not query.startswith("--"):
+ *         pos = 0
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -56921,14 +57072,15 @@
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("asyncpg.protocol.protocol.PreparedStatementState._parse_dtype", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_query);
+  __Pyx_XDECREF(__pyx_v_pos);
   __Pyx_XDECREF(__pyx_v_end);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "asyncpg/protocol/prepared_stmt.pxd":10
@@ -57250,15 +57402,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__51, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__53, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -57306,15 +57458,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__52, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__54, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -57329,15 +57481,15 @@
   __Pyx_AddTraceback("asyncpg.protocol.protocol.PreparedStatementState.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asyncpg/protocol/prepared_stmt.pyx":404
+/* "asyncpg/protocol/prepared_stmt.pyx":415
  *         self.query = query[end + 2:]
  * 
  * cdef _decode_parameters_desc(object desc):             # <<<<<<<<<<<<<<
  *     cdef:
  *         ReadBuffer reader
  */
 
@@ -57354,94 +57506,94 @@
   int32_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_parameters_desc", 0);
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":409
+  /* "asyncpg/protocol/prepared_stmt.pyx":420
  *         int16_t nparams
  *         uint32_t p_oid
  *         list result = []             # <<<<<<<<<<<<<<
  * 
  *     reader = ReadBuffer.new_message_parser(desc)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 409, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":411
+  /* "asyncpg/protocol/prepared_stmt.pyx":422
  *         list result = []
  * 
  *     reader = ReadBuffer.new_message_parser(desc)             # <<<<<<<<<<<<<<
  *     nparams = reader.read_int16()
  * 
  */
-  __pyx_t_1 = ((PyObject *)__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer->new_message_parser(__pyx_v_desc)); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 411, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer->new_message_parser(__pyx_v_desc)); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_reader = ((struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":412
+  /* "asyncpg/protocol/prepared_stmt.pyx":423
  * 
  *     reader = ReadBuffer.new_message_parser(desc)
  *     nparams = reader.read_int16()             # <<<<<<<<<<<<<<
  * 
  *     for i from 0 <= i < nparams:
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_2 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 412, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_2 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 423, __pyx_L1_error)
   __pyx_v_nparams = __pyx_t_2;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":414
+  /* "asyncpg/protocol/prepared_stmt.pyx":425
  *     nparams = reader.read_int16()
  * 
  *     for i from 0 <= i < nparams:             # <<<<<<<<<<<<<<
  *         p_oid = <uint32_t>reader.read_int32()
  *         result.append(p_oid)
  */
   __pyx_t_2 = __pyx_v_nparams;
   for (__pyx_v_i = 0; __pyx_v_i < __pyx_t_2; __pyx_v_i++) {
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":415
+    /* "asyncpg/protocol/prepared_stmt.pyx":426
  * 
  *     for i from 0 <= i < nparams:
  *         p_oid = <uint32_t>reader.read_int32()             # <<<<<<<<<<<<<<
  *         result.append(p_oid)
  * 
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 415, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 426, __pyx_L1_error)
     __pyx_v_p_oid = ((uint32_t)__pyx_t_3);
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":416
+    /* "asyncpg/protocol/prepared_stmt.pyx":427
  *     for i from 0 <= i < nparams:
  *         p_oid = <uint32_t>reader.read_int32()
  *         result.append(p_oid)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_p_oid); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 416, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_p_oid); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 427, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(7, 416, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(7, 427, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":418
+  /* "asyncpg/protocol/prepared_stmt.pyx":429
  *         result.append(p_oid)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":404
+  /* "asyncpg/protocol/prepared_stmt.pyx":415
  *         self.query = query[end + 2:]
  * 
  * cdef _decode_parameters_desc(object desc):             # <<<<<<<<<<<<<<
  *     cdef:
  *         ReadBuffer reader
  */
 
@@ -57454,15 +57606,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_reader);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asyncpg/protocol/prepared_stmt.pyx":421
+/* "asyncpg/protocol/prepared_stmt.pyx":432
  * 
  * 
  * cdef _decode_row_desc(object desc):             # <<<<<<<<<<<<<<
  *     cdef:
  *         ReadBuffer reader
  */
 
@@ -57492,167 +57644,167 @@
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_row_desc", 0);
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":437
+  /* "asyncpg/protocol/prepared_stmt.pyx":448
  *         list result
  * 
  *     reader = ReadBuffer.new_message_parser(desc)             # <<<<<<<<<<<<<<
  *     nfields = reader.read_int16()
  *     result = []
  */
-  __pyx_t_1 = ((PyObject *)__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer->new_message_parser(__pyx_v_desc)); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 437, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer->new_message_parser(__pyx_v_desc)); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_reader = ((struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":438
+  /* "asyncpg/protocol/prepared_stmt.pyx":449
  * 
  *     reader = ReadBuffer.new_message_parser(desc)
  *     nfields = reader.read_int16()             # <<<<<<<<<<<<<<
  *     result = []
  * 
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_2 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 438, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_2 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 449, __pyx_L1_error)
   __pyx_v_nfields = __pyx_t_2;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":439
+  /* "asyncpg/protocol/prepared_stmt.pyx":450
  *     reader = ReadBuffer.new_message_parser(desc)
  *     nfields = reader.read_int16()
  *     result = []             # <<<<<<<<<<<<<<
  * 
  *     for i from 0 <= i < nfields:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 439, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":441
+  /* "asyncpg/protocol/prepared_stmt.pyx":452
  *     result = []
  * 
  *     for i from 0 <= i < nfields:             # <<<<<<<<<<<<<<
  *         f_name = reader.read_null_str()
  *         f_table_oid = <uint32_t>reader.read_int32()
  */
   __pyx_t_2 = __pyx_v_nfields;
   for (__pyx_v_i = 0; __pyx_v_i < __pyx_t_2; __pyx_v_i++) {
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":442
+    /* "asyncpg/protocol/prepared_stmt.pyx":453
  * 
  *     for i from 0 <= i < nfields:
  *         f_name = reader.read_null_str()             # <<<<<<<<<<<<<<
  *         f_table_oid = <uint32_t>reader.read_int32()
  *         f_column_num = reader.read_int16()
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_null_str(__pyx_v_reader); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 442, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_null_str(__pyx_v_reader); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(7, 442, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(7, 453, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_f_name, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":443
+    /* "asyncpg/protocol/prepared_stmt.pyx":454
  *     for i from 0 <= i < nfields:
  *         f_name = reader.read_null_str()
  *         f_table_oid = <uint32_t>reader.read_int32()             # <<<<<<<<<<<<<<
  *         f_column_num = reader.read_int16()
  *         f_dt_oid = <uint32_t>reader.read_int32()
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 443, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 454, __pyx_L1_error)
     __pyx_v_f_table_oid = ((uint32_t)__pyx_t_3);
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":444
+    /* "asyncpg/protocol/prepared_stmt.pyx":455
  *         f_name = reader.read_null_str()
  *         f_table_oid = <uint32_t>reader.read_int32()
  *         f_column_num = reader.read_int16()             # <<<<<<<<<<<<<<
  *         f_dt_oid = <uint32_t>reader.read_int32()
  *         f_dt_size = reader.read_int16()
  */
-    __pyx_t_4 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_4 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 444, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_4 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 455, __pyx_L1_error)
     __pyx_v_f_column_num = __pyx_t_4;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":445
+    /* "asyncpg/protocol/prepared_stmt.pyx":456
  *         f_table_oid = <uint32_t>reader.read_int32()
  *         f_column_num = reader.read_int16()
  *         f_dt_oid = <uint32_t>reader.read_int32()             # <<<<<<<<<<<<<<
  *         f_dt_size = reader.read_int16()
  *         f_dt_mod = reader.read_int32()
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 445, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 456, __pyx_L1_error)
     __pyx_v_f_dt_oid = ((uint32_t)__pyx_t_3);
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":446
+    /* "asyncpg/protocol/prepared_stmt.pyx":457
  *         f_column_num = reader.read_int16()
  *         f_dt_oid = <uint32_t>reader.read_int32()
  *         f_dt_size = reader.read_int16()             # <<<<<<<<<<<<<<
  *         f_dt_mod = reader.read_int32()
  *         f_format = reader.read_int16()
  */
-    __pyx_t_4 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_4 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 446, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_4 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 457, __pyx_L1_error)
     __pyx_v_f_dt_size = __pyx_t_4;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":447
+    /* "asyncpg/protocol/prepared_stmt.pyx":458
  *         f_dt_oid = <uint32_t>reader.read_int32()
  *         f_dt_size = reader.read_int16()
  *         f_dt_mod = reader.read_int32()             # <<<<<<<<<<<<<<
  *         f_format = reader.read_int16()
  * 
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 447, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int32(__pyx_v_reader); if (unlikely(__pyx_t_3 == ((int32_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 458, __pyx_L1_error)
     __pyx_v_f_dt_mod = __pyx_t_3;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":448
+    /* "asyncpg/protocol/prepared_stmt.pyx":459
  *         f_dt_size = reader.read_int16()
  *         f_dt_mod = reader.read_int32()
  *         f_format = reader.read_int16()             # <<<<<<<<<<<<<<
  * 
  *         result.append(
  */
-    __pyx_t_4 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_4 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 448, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer *)__pyx_v_reader->__pyx_vtab)->read_int16(__pyx_v_reader); if (unlikely(__pyx_t_4 == ((int16_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 459, __pyx_L1_error)
     __pyx_v_f_format = __pyx_t_4;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":451
+    /* "asyncpg/protocol/prepared_stmt.pyx":462
  * 
  *         result.append(
  *             (f_name, f_table_oid, f_column_num, f_dt_oid,             # <<<<<<<<<<<<<<
  *              f_dt_size, f_dt_mod, f_format))
  * 
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_f_table_oid); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 451, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_f_table_oid); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyInt_From_int16_t(__pyx_v_f_column_num); if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 451, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int16_t(__pyx_v_f_column_num); if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_f_dt_oid); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 451, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_f_dt_oid); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":452
+    /* "asyncpg/protocol/prepared_stmt.pyx":463
  *         result.append(
  *             (f_name, f_table_oid, f_column_num, f_dt_oid,
  *              f_dt_size, f_dt_mod, f_format))             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __pyx_t_7 = __Pyx_PyInt_From_int16_t(__pyx_v_f_dt_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(7, 452, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_int16_t(__pyx_v_f_dt_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(7, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyInt_From_int32_t(__pyx_v_f_dt_mod); if (unlikely(!__pyx_t_8)) __PYX_ERR(7, 452, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_int32_t(__pyx_v_f_dt_mod); if (unlikely(!__pyx_t_8)) __PYX_ERR(7, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyInt_From_int16_t(__pyx_v_f_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(7, 452, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_From_int16_t(__pyx_v_f_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(7, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":451
+    /* "asyncpg/protocol/prepared_stmt.pyx":462
  * 
  *         result.append(
  *             (f_name, f_table_oid, f_column_num, f_dt_oid,             # <<<<<<<<<<<<<<
  *              f_dt_size, f_dt_mod, f_format))
  * 
  */
-    __pyx_t_10 = PyTuple_New(7); if (unlikely(!__pyx_t_10)) __PYX_ERR(7, 451, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(7); if (unlikely(!__pyx_t_10)) __PYX_ERR(7, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_INCREF(__pyx_v_f_name);
     __Pyx_GIVEREF(__pyx_v_f_name);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_v_f_name);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_5);
@@ -57668,36 +57820,36 @@
     __pyx_t_1 = 0;
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
     __pyx_t_8 = 0;
     __pyx_t_9 = 0;
 
-    /* "asyncpg/protocol/prepared_stmt.pyx":450
+    /* "asyncpg/protocol/prepared_stmt.pyx":461
  *         f_format = reader.read_int16()
  * 
  *         result.append(             # <<<<<<<<<<<<<<
  *             (f_name, f_table_oid, f_column_num, f_dt_oid,
  *              f_dt_size, f_dt_mod, f_format))
  */
-    __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_10); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(7, 450, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_10); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(7, 461, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":454
+  /* "asyncpg/protocol/prepared_stmt.pyx":465
  *              f_dt_size, f_dt_mod, f_format))
  * 
  *     return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "asyncpg/protocol/prepared_stmt.pyx":421
+  /* "asyncpg/protocol/prepared_stmt.pyx":432
  * 
  * 
  * cdef _decode_row_desc(object desc):             # <<<<<<<<<<<<<<
  *     cdef:
  *         ReadBuffer reader
  */
 
@@ -61472,15 +61624,15 @@
                 __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
                 __pyx_L32_try_end:;
               }
             }
             /*finally:*/ {
               /*normal exit:*/{
                 if (__pyx_t_9) {
-                  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple__53, NULL);
+                  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple__55, NULL);
                   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
                   if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 237, __pyx_L11_error)
                   __Pyx_GOTREF(__pyx_t_12);
                   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
                 }
                 goto __pyx_L24;
               }
@@ -64807,15 +64959,15 @@
             __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
             __pyx_L26_try_end:;
           }
         }
         /*finally:*/ {
           /*normal exit:*/{
             if (__pyx_t_6) {
-              __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__53, NULL);
+              __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__55, NULL);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
               if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 365, __pyx_L9_error)
               __Pyx_GOTREF(__pyx_t_9);
               __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
             }
             goto __pyx_L18;
           }
@@ -65098,15 +65250,15 @@
                   __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
                   __pyx_L56_try_end:;
                 }
               }
               /*finally:*/ {
                 /*normal exit:*/{
                   if (__pyx_t_7) {
-                    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_tuple__53, NULL);
+                    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_tuple__55, NULL);
                     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                     if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 372, __pyx_L35_error)
                     __Pyx_GOTREF(__pyx_t_15);
                     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
                   }
                   goto __pyx_L48;
                 }
@@ -66694,15 +66846,15 @@
                     __Pyx_ExceptionReset(__pyx_t_22, __pyx_t_23, __pyx_t_24);
                     __pyx_L41_try_end:;
                   }
                 }
                 /*finally:*/ {
                   /*normal exit:*/{
                     if (__pyx_t_21) {
-                      __pyx_t_24 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_tuple__53, NULL);
+                      __pyx_t_24 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_tuple__55, NULL);
                       __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
                       if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 458, __pyx_L8_error)
                       __Pyx_GOTREF(__pyx_t_24);
                       __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
                     }
                     goto __pyx_L33;
                   }
@@ -67141,15 +67293,15 @@
                     __Pyx_ExceptionReset(__pyx_t_24, __pyx_t_23, __pyx_t_22);
                     __pyx_L66_try_end:;
                   }
                 }
                 /*finally:*/ {
                   /*normal exit:*/{
                     if (__pyx_t_21) {
-                      __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_tuple__53, NULL);
+                      __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_tuple__55, NULL);
                       __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
                       if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 477, __pyx_L8_error)
                       __Pyx_GOTREF(__pyx_t_22);
                       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
                     }
                     goto __pyx_L58;
                   }
@@ -67347,15 +67499,15 @@
             /* "asyncpg/protocol/protocol.pyx":490
  *                     aiter = reader.__aiter__
  *                 except AttributeError:
  *                     raise TypeError('reader is not an asynchronous iterable')             # <<<<<<<<<<<<<<
  *                 else:
  *                     iterator = aiter()
  */
-            __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__54, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 490, __pyx_L74_except_error)
+            __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__56, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 490, __pyx_L74_except_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_Raise(__pyx_t_5, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             __PYX_ERR(0, 490, __pyx_L74_except_error)
           }
           goto __pyx_L74_except_error;
           __pyx_L74_except_error:;
@@ -67595,15 +67747,15 @@
                     __Pyx_ExceptionReset(__pyx_t_25, __pyx_t_27, __pyx_t_28);
                     __pyx_L101_try_end:;
                   }
                 }
                 /*finally:*/ {
                   /*normal exit:*/{
                     if (__pyx_t_24) {
-                      __pyx_t_28 = __Pyx_PyObject_Call(__pyx_t_24, __pyx_tuple__53, NULL);
+                      __pyx_t_28 = __Pyx_PyObject_Call(__pyx_t_24, __pyx_tuple__55, NULL);
                       __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
                       if (unlikely(!__pyx_t_28)) __PYX_ERR(0, 498, __pyx_L80_error)
                       __Pyx_GOTREF(__pyx_t_28);
                       __Pyx_DECREF(__pyx_t_28); __pyx_t_28 = 0;
                     }
                     goto __pyx_L93;
                   }
@@ -67881,15 +68033,15 @@
                     __Pyx_ExceptionReset(__pyx_t_28, __pyx_t_27, __pyx_t_25);
                     __pyx_L120_try_end:;
                   }
                 }
                 /*finally:*/ {
                   /*normal exit:*/{
                     if (__pyx_t_24) {
-                      __pyx_t_25 = __Pyx_PyObject_Call(__pyx_t_24, __pyx_tuple__53, NULL);
+                      __pyx_t_25 = __Pyx_PyObject_Call(__pyx_t_24, __pyx_tuple__55, NULL);
                       __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
                       if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 500, __pyx_L80_error)
                       __Pyx_GOTREF(__pyx_t_25);
                       __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
                     }
                     goto __pyx_L112;
                   }
@@ -78732,15 +78884,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x7336a95, 0xd9a8555, 0xea6089f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x7336a95, 0xd9a8555, 0xea6089f) = (_custom_type_codecs, _derived_type_codecs))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__55, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__57, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x7336a95, 0xd9a8555, 0xea6089f):
@@ -79146,15 +79298,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xfbc42c3, 0x2576f59, 0xa4dd4b1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xfbc42c3, 0x2576f59, 0xa4dd4b1) = (_discard_data, _execute_iter, _execute_portal_name, _execute_stmt_name, _skip_discard, backend_pid, backend_secret, buffer, con_params, con_status, encoding, result, result_execute_completed, result_param_desc, result_row_desc, result_status_msg, result_type, scram, state, transport, xact_status))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__56, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__58, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xfbc42c3, 0x2576f59, 0xa4dd4b1):
@@ -79762,15 +79914,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x3a81f09, 0x44705b0, 0x9debc35):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x3a81f09, 0x44705b0, 0x9debc35) = (_discard_data, _execute_iter, _execute_portal_name, _execute_stmt_name, _is_ssl, _skip_discard, address, backend_pid, backend_secret, buffer, cancel_sent_waiter, cancel_waiter, closing, completed_callback, con_params, con_status, conref, create_future, encoding, is_reading, last_query, loop, queries_count, record_class, result, result_execute_completed, result_param_desc, result_row_desc, result_status_msg, result_type, return_extra, scram, settings, state, statement, timeout_callback, timeout_handle, transport, waiter, writing_paused, xact_status))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__57, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__59, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x3a81f09, 0x44705b0, 0x9debc35):
@@ -81685,15 +81837,15 @@
       /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__58, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(18, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__60, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(18, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(18, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -81817,15 +81969,15 @@
       /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__59, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(18, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(18, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(18, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -81949,15 +82101,15 @@
       /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__59, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(18, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(18, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(18, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -86374,14 +86526,16 @@
   {&__pyx_kp_u__43, __pyx_k__43, sizeof(__pyx_k__43), 0, 1, 0, 0},
   {&__pyx_kp_u__44, __pyx_k__44, sizeof(__pyx_k__44), 0, 1, 0, 0},
   {&__pyx_kp_u__45, __pyx_k__45, sizeof(__pyx_k__45), 0, 1, 0, 0},
   {&__pyx_kp_u__47, __pyx_k__47, sizeof(__pyx_k__47), 0, 1, 0, 0},
   {&__pyx_kp_u__48, __pyx_k__48, sizeof(__pyx_k__48), 0, 1, 0, 0},
   {&__pyx_kp_u__49, __pyx_k__49, sizeof(__pyx_k__49), 0, 1, 0, 0},
   {&__pyx_kp_u__50, __pyx_k__50, sizeof(__pyx_k__50), 0, 1, 0, 0},
+  {&__pyx_kp_u__51, __pyx_k__51, sizeof(__pyx_k__51), 0, 1, 0, 0},
+  {&__pyx_kp_u__52, __pyx_k__52, sizeof(__pyx_k__52), 0, 1, 0, 0},
   {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
   {&__pyx_kp_u_a_sized_iterable_container_expec, __pyx_k_a_sized_iterable_container_expec, sizeof(__pyx_k_a_sized_iterable_container_expec), 0, 1, 0, 0},
   {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
   {&__pyx_n_u_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 1, 0, 1},
   {&__pyx_n_s_abort, __pyx_k_abort, sizeof(__pyx_k_abort), 0, 0, 1, 1},
   {&__pyx_n_u_abstime, __pyx_k_abstime, sizeof(__pyx_k_abstime), 0, 1, 0, 1},
   {&__pyx_n_u_aclitem, __pyx_k_aclitem, sizeof(__pyx_k_aclitem), 0, 1, 0, 1},
@@ -87289,202 +87443,203 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
+  __pyx_tuple__53 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__53);
+  __Pyx_GIVEREF(__pyx_tuple__53);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__52);
-  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_tuple__54 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
 
   /* "asyncpg/protocol/protocol.pyx":237
  * 
  *             while more:
  *                 with timer:             # <<<<<<<<<<<<<<
  *                     await asyncio.wait_for(
  *                         self.writing_allowed.wait(),
  */
-  __pyx_tuple__53 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 237, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
+  __pyx_tuple__55 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__55);
+  __Pyx_GIVEREF(__pyx_tuple__55);
 
   /* "asyncpg/protocol/protocol.pyx":490
  *                     aiter = reader.__aiter__
  *                 except AttributeError:
  *                     raise TypeError('reader is not an asynchronous iterable')             # <<<<<<<<<<<<<<
  *                 else:
  *                     iterator = aiter()
  */
-  __pyx_tuple__54 = PyTuple_Pack(1, __pyx_kp_u_reader_is_not_an_asynchronous_it); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 490, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__54);
-  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_tuple__56 = PyTuple_Pack(1, __pyx_kp_u_reader_is_not_an_asynchronous_it); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x7336a95, 0xd9a8555, 0xea6089f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x7336a95, 0xd9a8555, 0xea6089f) = (_custom_type_codecs, _derived_type_codecs))" % __pyx_checksum)
  */
-  __pyx_tuple__55 = PyTuple_Pack(3, __pyx_int_120810133, __pyx_int_228230485, __pyx_int_245762207); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__55);
-  __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_tuple__56 = PyTuple_Pack(3, __pyx_int_263996099, __pyx_int_39284569, __pyx_int_172872881); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__56);
-  __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_int_61349641, __pyx_int_71763376, __pyx_int_165592117); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_int_120810133, __pyx_int_228230485, __pyx_int_245762207); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
+  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_int_263996099, __pyx_int_39284569, __pyx_int_172872881); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_tuple__59 = PyTuple_Pack(3, __pyx_int_61349641, __pyx_int_71763376, __pyx_int_165592117); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__59);
+  __Pyx_GIVEREF(__pyx_tuple__59);
 
   /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__58 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(18, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__58);
-  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_tuple__60 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(18, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
 
   /* ".eggs/numpy-1.24.2-py3.11-linux-x86_64.egg/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__59 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(18, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__59);
-  __Pyx_GIVEREF(__pyx_tuple__59);
+  __pyx_tuple__61 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(18, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__61);
+  __Pyx_GIVEREF(__pyx_tuple__61);
 
   /* "asyncpg/protocol/pgtypes.pxi":116
  * DEF ANYCOMPATIBLERANGEOID = 5080
  * 
  * cdef ARRAY_TYPES = (_TEXTOID, _OIDOID,)             # <<<<<<<<<<<<<<
  * 
  * BUILTIN_TYPE_OID_MAP = {
  */
-  __pyx_tuple__60 = PyTuple_Pack(2, __pyx_int_1009, __pyx_int_1028); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(23, 116, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__60);
-  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_tuple__62 = PyTuple_Pack(2, __pyx_int_1009, __pyx_int_1028); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(23, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
 
   /* "asyncpg/protocol/protocol.pyx":989
  * 
  * class Timer:
  *     def __init__(self, budget):             # <<<<<<<<<<<<<<
  *         self._budget = budget
  *         self._started = 0
  */
-  __pyx_tuple__61 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_budget); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 989, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__61);
-  __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_init, 989, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 989, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_budget); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 989, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_init, 989, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 989, __pyx_L1_error)
 
   /* "asyncpg/protocol/protocol.pyx":993
  *         self._started = 0
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         if self._budget is not None:
  *             self._started = time.monotonic()
  */
-  __pyx_tuple__63 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 993, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__63);
-  __Pyx_GIVEREF(__pyx_tuple__63);
-  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_enter, 993, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_tuple__65 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__65);
+  __Pyx_GIVEREF(__pyx_tuple__65);
+  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_enter, 993, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 993, __pyx_L1_error)
 
   /* "asyncpg/protocol/protocol.pyx":997
  *             self._started = time.monotonic()
  * 
  *     def __exit__(self, et, e, tb):             # <<<<<<<<<<<<<<
  *         if self._budget is not None:
  *             self._budget -= time.monotonic() - self._started
  */
-  __pyx_tuple__65 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_et, __pyx_n_s_e, __pyx_n_s_tb); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 997, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__65);
-  __Pyx_GIVEREF(__pyx_tuple__65);
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_exit, 997, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 997, __pyx_L1_error)
+  __pyx_tuple__67 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_et, __pyx_n_s_e, __pyx_n_s_tb); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 997, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__67);
+  __Pyx_GIVEREF(__pyx_tuple__67);
+  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_exit, 997, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 997, __pyx_L1_error)
 
   /* "asyncpg/protocol/protocol.pyx":1001
  *             self._budget -= time.monotonic() - self._started
  * 
  *     def get_remaining_budget(self):             # <<<<<<<<<<<<<<
  *         return self._budget
  * 
  */
-  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 1001, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
-  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_get_remaining_budget, 1001, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __pyx_tuple__69 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__69);
+  __Pyx_GIVEREF(__pyx_tuple__69);
+  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_get_remaining_budget, 1001, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 1001, __pyx_L1_error)
 
   /* "asyncpg/protocol/protocol.pyx":1004
  *         return self._budget
  * 
  *     def has_budget_greater_than(self, amount):             # <<<<<<<<<<<<<<
  *         if self._budget is None:
  *             # Unlimited budget.
  */
-  __pyx_tuple__69 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_amount); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 1004, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__69);
-  __Pyx_GIVEREF(__pyx_tuple__69);
-  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_has_budget_greater_than, 1004, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __pyx_tuple__71 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_amount); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__71);
+  __Pyx_GIVEREF(__pyx_tuple__71);
+  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__71, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_has_budget_greater_than, 1004, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 1004, __pyx_L1_error)
 
   /* "asyncpg/protocol/protocol.pyx":1016
  * 
  * 
  * def _create_record(object mapping, tuple elems):             # <<<<<<<<<<<<<<
  *     # Exposed only for testing purposes.
  * 
  */
-  __pyx_tuple__71 = PyTuple_Pack(6, __pyx_n_s_mapping, __pyx_n_s_elems, __pyx_n_s_rec, __pyx_n_s_i, __pyx_n_s_desc, __pyx_n_s_elem); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(0, 1016, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__71);
-  __Pyx_GIVEREF(__pyx_tuple__71);
-  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__71, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_create_record, 1016, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 1016, __pyx_L1_error)
+  __pyx_tuple__73 = PyTuple_Pack(6, __pyx_n_s_mapping, __pyx_n_s_elems, __pyx_n_s_rec, __pyx_n_s_i, __pyx_n_s_desc, __pyx_n_s_elem); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(0, 1016, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__73);
+  __Pyx_GIVEREF(__pyx_tuple__73);
+  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asyncpg_protocol_protocol_pyx, __pyx_n_s_create_record, 1016, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 1016, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_DataCodecConfig(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__73 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__73);
-  __Pyx_GIVEREF(__pyx_tuple__73);
-  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DataCodecConfig, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_tuple__75 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__75);
   __Pyx_GIVEREF(__pyx_tuple__75);
-  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__75, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CoreProtocol, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__75, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DataCodecConfig, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_tuple__77 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__77)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__77);
   __Pyx_GIVEREF(__pyx_tuple__77);
-  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__77, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BaseProtocol, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__77, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CoreProtocol, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__79 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__79);
+  __Pyx_GIVEREF(__pyx_tuple__79);
+  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BaseProtocol, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
   __pyx_umethod_PyDict_Type_pop.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_6 = PyInt_FromLong(6); if (unlikely(!__pyx_int_6)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_17 = PyInt_FromLong(17); if (unlikely(!__pyx_int_17)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_18 = PyInt_FromLong(18); if (unlikely(!__pyx_int_18)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_19 = PyInt_FromLong(19); if (unlikely(!__pyx_int_19)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_20 = PyInt_FromLong(20); if (unlikely(!__pyx_int_20)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -87591,15 +87746,14 @@
   __pyx_int_71763376 = PyInt_FromLong(71763376L); if (unlikely(!__pyx_int_71763376)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_120810133 = PyInt_FromLong(120810133L); if (unlikely(!__pyx_int_120810133)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_165592117 = PyInt_FromLong(165592117L); if (unlikely(!__pyx_int_165592117)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_172872881 = PyInt_FromLong(172872881L); if (unlikely(!__pyx_int_172872881)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_228230485 = PyInt_FromLong(228230485L); if (unlikely(!__pyx_int_228230485)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_245762207 = PyInt_FromLong(245762207L); if (unlikely(!__pyx_int_245762207)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_263996099 = PyInt_FromLong(263996099L); if (unlikely(!__pyx_int_263996099)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -87708,15 +87862,16 @@
   }
   if (__Pyx_SetVtable(__pyx_type_7asyncpg_8protocol_8protocol_DataCodecConfig.tp_dict, __pyx_vtabptr_7asyncpg_8protocol_8protocol_DataCodecConfig) < 0) __PYX_ERR(3, 469, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DataCodecConfig, (PyObject *)&__pyx_type_7asyncpg_8protocol_8protocol_DataCodecConfig) < 0) __PYX_ERR(3, 469, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7asyncpg_8protocol_8protocol_DataCodecConfig) < 0) __PYX_ERR(3, 469, __pyx_L1_error)
   __pyx_ptype_7asyncpg_8protocol_8protocol_DataCodecConfig = &__pyx_type_7asyncpg_8protocol_8protocol_DataCodecConfig;
   __pyx_t_1 = PyImport_ImportModule("asyncpg.pgproto.pgproto"); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_CodecContext = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "CodecContext", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_CodecContext), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_CodecContext = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "CodecContext", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_CodecContext), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_CodecContext),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_CodecContext) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_7asyncpg_7pgproto_7pgproto_CodecContext = (struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_CodecContext*)__Pyx_GetVtable(__pyx_ptype_7asyncpg_7pgproto_7pgproto_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_CodecContext)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_7asyncpg_8protocol_8protocol_ConnectionSettings = &__pyx_vtable_7asyncpg_8protocol_8protocol_ConnectionSettings;
   __pyx_vtable_7asyncpg_8protocol_8protocol_ConnectionSettings.__pyx_base = *__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_CodecContext;
   __pyx_vtable_7asyncpg_8protocol_8protocol_ConnectionSettings.__pyx_base.get_text_codec = (PyObject *(*)(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_CodecContext *, int __pyx_skip_dispatch))__pyx_f_7asyncpg_8protocol_8protocol_18ConnectionSettings_get_text_codec;
   __pyx_vtable_7asyncpg_8protocol_8protocol_ConnectionSettings.__pyx_base.is_encoding_utf8 = (PyObject *(*)(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_CodecContext *))__pyx_f_7asyncpg_8protocol_8protocol_18ConnectionSettings_is_encoding_utf8;
   __pyx_vtable_7asyncpg_8protocol_8protocol_ConnectionSettings.add_setting = (PyObject *(*)(struct __pyx_obj_7asyncpg_8protocol_8protocol_ConnectionSettings *, PyObject *, PyObject *))__pyx_f_7asyncpg_8protocol_8protocol_18ConnectionSettings_add_setting;
@@ -88061,81 +88216,103 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(19, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(19, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(20, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(20, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(21, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(21, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("asyncpg.pgproto.pgproto"); if (unlikely(!__pyx_t_1)) __PYX_ERR(17, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_WriteBuffer = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "WriteBuffer", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_WriteBuffer), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_WriteBuffer = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "WriteBuffer", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_WriteBuffer), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_WriteBuffer),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_WriteBuffer) __PYX_ERR(17, 8, __pyx_L1_error)
   __pyx_vtabptr_7asyncpg_7pgproto_7pgproto_WriteBuffer = (struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_WriteBuffer*)__Pyx_GetVtable(__pyx_ptype_7asyncpg_7pgproto_7pgproto_WriteBuffer->tp_dict); if (unlikely(!__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_WriteBuffer)) __PYX_ERR(17, 8, __pyx_L1_error)
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_ReadBuffer = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "ReadBuffer", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ReadBuffer), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_ReadBuffer = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "ReadBuffer", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ReadBuffer), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ReadBuffer),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_ReadBuffer) __PYX_ERR(17, 68, __pyx_L1_error)
   __pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer = (struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ReadBuffer*)__Pyx_GetVtable(__pyx_ptype_7asyncpg_7pgproto_7pgproto_ReadBuffer->tp_dict); if (unlikely(!__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ReadBuffer)) __PYX_ERR(17, 68, __pyx_L1_error)
   __pyx_t_2 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_2)) __PYX_ERR(22, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_dtype = __Pyx_ImportType(__pyx_t_2, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_dtype = __Pyx_ImportType(__pyx_t_2, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_dtype) __PYX_ERR(22, 34, __pyx_L1_error)
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_DTypeError = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "DTypeError", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_DTypeError), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_DTypeError = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "DTypeError", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_DTypeError), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_DTypeError),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_DTypeError) __PYX_ERR(22, 59, __pyx_L1_error)
-  __pyx_ptype_7asyncpg_7pgproto_7pgproto_ArrayWriter = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "ArrayWriter", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ArrayWriter), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7asyncpg_7pgproto_7pgproto_ArrayWriter = __Pyx_ImportType(__pyx_t_1, "asyncpg.pgproto.pgproto", "ArrayWriter", sizeof(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ArrayWriter), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7asyncpg_7pgproto_7pgproto_ArrayWriter),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7asyncpg_7pgproto_7pgproto_ArrayWriter) __PYX_ERR(22, 68, __pyx_L1_error)
   __pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ArrayWriter = (struct __pyx_vtabstruct_7asyncpg_7pgproto_7pgproto_ArrayWriter*)__Pyx_GetVtable(__pyx_ptype_7asyncpg_7pgproto_7pgproto_ArrayWriter->tp_dict); if (unlikely(!__pyx_vtabptr_7asyncpg_7pgproto_7pgproto_ArrayWriter)) __PYX_ERR(22, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_2)) __PYX_ERR(18, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_2, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_2, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(18, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_2, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_2, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(18, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_2, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_2, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(18, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_2, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_2, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(18, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_2, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_2, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(18, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_2, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_2, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(18, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_2, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_2, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(18, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_2, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_2, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(18, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_2, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_2, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(18, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_2, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_2, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(18, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_2, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_2, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(18, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_2, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_2, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(18, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_2, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_2, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(18, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_2, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_2, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(18, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_2, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_2, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(18, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -88662,18 +88839,18 @@
   /* "asyncpg/protocol/pgtypes.pxi":116
  * DEF ANYCOMPATIBLERANGEOID = 5080
  * 
  * cdef ARRAY_TYPES = (_TEXTOID, _OIDOID,)             # <<<<<<<<<<<<<<
  * 
  * BUILTIN_TYPE_OID_MAP = {
  */
-  __Pyx_INCREF(__pyx_tuple__60);
+  __Pyx_INCREF(__pyx_tuple__62);
   __Pyx_XGOTREF(__pyx_v_7asyncpg_8protocol_8protocol_ARRAY_TYPES);
-  __Pyx_DECREF_SET(__pyx_v_7asyncpg_8protocol_8protocol_ARRAY_TYPES, __pyx_tuple__60);
-  __Pyx_GIVEREF(__pyx_tuple__60);
+  __Pyx_DECREF_SET(__pyx_v_7asyncpg_8protocol_8protocol_ARRAY_TYPES, __pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
 
   /* "asyncpg/protocol/pgtypes.pxi":119
  * 
  * BUILTIN_TYPE_OID_MAP = {
  *     ABSTIMEOID: 'abstime',             # <<<<<<<<<<<<<<
  *     ACLITEMOID: 'aclitem',
  *     ANYARRAYOID: 'anyarray',
@@ -90079,63 +90256,63 @@
   /* "asyncpg/protocol/protocol.pyx":989
  * 
  * class Timer:
  *     def __init__(self, budget):             # <<<<<<<<<<<<<<
  *         self._budget = budget
  *         self._started = 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_1__init__, 0, __pyx_n_s_Timer___init, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 989, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_1__init__, 0, __pyx_n_s_Timer___init, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_SetNameInClass(__pyx_t_16, __pyx_n_s_init, __pyx_t_1) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/protocol.pyx":993
  *         self._started = 0
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         if self._budget is not None:
  *             self._started = time.monotonic()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_3__enter__, 0, __pyx_n_s_Timer___enter, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_3__enter__, 0, __pyx_n_s_Timer___enter, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 993, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_SetNameInClass(__pyx_t_16, __pyx_n_s_enter, __pyx_t_1) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/protocol.pyx":997
  *             self._started = time.monotonic()
  * 
  *     def __exit__(self, et, e, tb):             # <<<<<<<<<<<<<<
  *         if self._budget is not None:
  *             self._budget -= time.monotonic() - self._started
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_5__exit__, 0, __pyx_n_s_Timer___exit, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 997, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_5__exit__, 0, __pyx_n_s_Timer___exit, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_SetNameInClass(__pyx_t_16, __pyx_n_s_exit, __pyx_t_1) < 0) __PYX_ERR(0, 997, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/protocol.pyx":1001
  *             self._budget -= time.monotonic() - self._started
  * 
  *     def get_remaining_budget(self):             # <<<<<<<<<<<<<<
  *         return self._budget
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_7get_remaining_budget, 0, __pyx_n_s_Timer_get_remaining_budget, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_7get_remaining_budget, 0, __pyx_n_s_Timer_get_remaining_budget, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1001, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_SetNameInClass(__pyx_t_16, __pyx_n_s_get_remaining_budget, __pyx_t_1) < 0) __PYX_ERR(0, 1001, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/protocol.pyx":1004
  *         return self._budget
  * 
  *     def has_budget_greater_than(self, amount):             # <<<<<<<<<<<<<<
  *         if self._budget is None:
  *             # Unlimited budget.
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_9has_budget_greater_than, 0, __pyx_n_s_Timer_has_budget_greater_than, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7asyncpg_8protocol_8protocol_5Timer_9has_budget_greater_than, 0, __pyx_n_s_Timer_has_budget_greater_than, NULL, __pyx_n_s_asyncpg_protocol_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1004, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_SetNameInClass(__pyx_t_16, __pyx_n_s_has_budget_greater_than, __pyx_t_1) < 0) __PYX_ERR(0, 1004, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/protocol.pyx":988
  * 
  * 
@@ -91298,28 +91475,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -93386,81 +93563,14 @@
                                      Py_ssize_t start, Py_ssize_t end, int direction) {
     if (unlikely(PyTuple_Check(substr))) {
         return __Pyx_PyUnicode_TailmatchTuple(s, substr, start, end, direction);
     }
     return (int) PyUnicode_Tailmatch(s, substr, start, end, direction);
 }
 
-/* PyIntCompare */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
-    if (op1 == op2) {
-        Py_RETURN_TRUE;
-    }
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long a = PyInt_AS_LONG(op1);
-        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        int unequal;
-        unsigned long uintval;
-        Py_ssize_t size = Py_SIZE(op1);
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        if (intval == 0) {
-            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-        } else if (intval < 0) {
-            if (size >= 0)
-                Py_RETURN_FALSE;
-            intval = -intval;
-            size = -size;
-        } else {
-            if (size <= 0)
-                Py_RETURN_FALSE;
-        }
-        uintval = (unsigned long) intval;
-#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 4)) {
-            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 3)) {
-            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 2)) {
-            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 1)) {
-            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
-        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-        double a = PyFloat_AS_DOUBLE(op1);
-        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-    }
-    return (
-        PyObject_RichCompare(op1, op2, Py_EQ));
-}
-
 /* PyUnicode_Substring */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Substring(
             PyObject* text, Py_ssize_t start, Py_ssize_t stop) {
     Py_ssize_t length;
     if (unlikely(__Pyx_PyUnicode_READY(text) == -1)) return NULL;
     length = __Pyx_PyUnicode_GET_LENGTH(text);
     if (start < 0) {
@@ -94810,15 +94920,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
+#if PY_VERSION_HEX >= 0x030C00A6
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+#else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
+#endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
         PyObject *method = NULL;
         int is_method = __Pyx_PyObject_GetMethod(obj, __pyx_n_s_await, &method);
         if (likely(is_method)) {
@@ -94860,15 +94974,15 @@
                  "object %.100s can't be used in 'await' expression",
                  Py_TYPE(obj)->tp_name);
 bad:
     return NULL;
 }
 
 /* CoroutineYieldFrom */
-static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
+  static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
     PyObject *retval;
     PyObject *source_gen = __Pyx__Coroutine_GetAwaitableIter(source);
     if (unlikely(!source_gen)) {
         return NULL;
     }
     if (__Pyx_Coroutine_Check(source_gen)) {
         retval = __Pyx_Generator_Next(source_gen);
@@ -94907,15 +95021,15 @@
         Py_INCREF(source);
         gen->yieldfrom = source;
     }
     return retval;
 }
 
 /* ReturnWithStopIteration */
-static void __Pyx__ReturnWithStopIteration(PyObject* value) {
+  static void __Pyx__ReturnWithStopIteration(PyObject* value) {
     PyObject *exc, *args;
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_PYSTON
     __Pyx_PyThreadState_declare
     if ((PY_VERSION_HEX >= 0x03030000 && PY_VERSION_HEX < 0x030500B1)
             || unlikely(PyTuple_Check(value) || PyExceptionInstance_Check(value))) {
         args = PyTuple_New(1);
         if (unlikely(!args)) return;
@@ -94949,15 +95063,15 @@
     if (unlikely(!exc)) return;
 #endif
     PyErr_SetObject(PyExc_StopIteration, exc);
     Py_DECREF(exc);
 }
 
 /* CythonFunctionShared */
-#include <structmember.h>
+  #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(op->func.m_ml->ml_doc);
@@ -95565,28 +95679,28 @@
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
 /* CythonFunction */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
     PyObject *op = __Pyx_CyFunction_Init(
         PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
         ml, flags, qualname, closure, module, globals, code
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* AsyncIter */
-static PyObject *__Pyx_Coroutine_GetAsyncIter_Generic(PyObject *obj) {
+  static PyObject *__Pyx_Coroutine_GetAsyncIter_Generic(PyObject *obj) {
 #if PY_VERSION_HEX < 0x030500B1
     {
         PyObject *iter = __Pyx_PyObject_CallMethod0(obj, __pyx_n_s_aiter);
         if (likely(iter))
             return iter;
         if (!PyErr_ExceptionMatches(PyExc_AttributeError))
             return NULL;
@@ -95641,15 +95755,15 @@
         }
     }
 #endif
     return __Pyx__Coroutine_AsyncIterNext(obj);
 }
 
 /* StopAsyncIteration */
-#if PY_VERSION_HEX < 0x030500B1
+  #if PY_VERSION_HEX < 0x030500B1
 static PyTypeObject __Pyx__PyExc_StopAsyncIteration_type = {
     PyVarObject_HEAD_INIT(0, 0)
     "StopAsyncIteration",
     sizeof(PyBaseExceptionObject),
     0,
     0,
     0,
@@ -95725,15 +95839,15 @@
     if (builtins && unlikely(PyMapping_SetItemString(builtins, (char*) "StopAsyncIteration", __Pyx_PyExc_StopAsyncIteration) < 0))
         return -1;
 #endif
     return 0;
 }
 
 /* HasAttr */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+  static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
     r = __Pyx_GetAttr(o, n);
@@ -95743,15 +95857,15 @@
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
 
 /* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+  static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -95808,63 +95922,63 @@
     #endif
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+  static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* CallNextTpDealloc */
-static void __Pyx_call_next_tp_dealloc(PyObject* obj, destructor current_tp_dealloc) {
+  static void __Pyx_call_next_tp_dealloc(PyObject* obj, destructor current_tp_dealloc) {
     PyTypeObject* type = Py_TYPE(obj);
     while (type && type->tp_dealloc != current_tp_dealloc)
         type = type->tp_base;
     while (type && type->tp_dealloc == current_tp_dealloc)
         type = type->tp_base;
     if (type)
         type->tp_dealloc(obj);
 }
 
 /* CallNextTpTraverse */
-static int __Pyx_call_next_tp_traverse(PyObject* obj, visitproc v, void *a, traverseproc current_tp_traverse) {
+  static int __Pyx_call_next_tp_traverse(PyObject* obj, visitproc v, void *a, traverseproc current_tp_traverse) {
     PyTypeObject* type = Py_TYPE(obj);
     while (type && type->tp_traverse != current_tp_traverse)
         type = type->tp_base;
     while (type && type->tp_traverse == current_tp_traverse)
         type = type->tp_base;
     if (type && type->tp_traverse)
         return type->tp_traverse(obj, v, a);
     return 0;
 }
 
 /* CallNextTpClear */
-static void __Pyx_call_next_tp_clear(PyObject* obj, inquiry current_tp_clear) {
+  static void __Pyx_call_next_tp_clear(PyObject* obj, inquiry current_tp_clear) {
     PyTypeObject* type = Py_TYPE(obj);
     while (type && type->tp_clear != current_tp_clear)
         type = type->tp_base;
     while (type && type->tp_clear == current_tp_clear)
         type = type->tp_base;
     if (type && type->tp_clear)
         type->tp_clear(obj);
 }
 
 /* SetVTable */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
+  static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
 #if PY_VERSION_HEX >= 0x02070000
     PyObject *ob = PyCapsule_New(vtable, 0, 0);
 #else
     PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
 #endif
     if (!ob)
         goto bad;
@@ -95874,15 +95988,15 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+  static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
@@ -95896,15 +96010,15 @@
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
 }
 
 /* SetupReduce */
-static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
@@ -96000,57 +96114,75 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* PyObject_GenericGetAttr */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+  #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
+  #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -96071,15 +96203,15 @@
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* GetVTable */
-static void* __Pyx_GetVtable(PyObject *dict) {
+  static void* __Pyx_GetVtable(PyObject *dict) {
     void* ptr;
     PyObject *ob = PyObject_GetItem(dict, __pyx_n_s_pyx_vtable);
     if (!ob)
         goto bad;
 #if PY_VERSION_HEX >= 0x02070000
     ptr = PyCapsule_GetPointer(ob, 0);
 #else
@@ -96091,15 +96223,15 @@
     return ptr;
 bad:
     Py_XDECREF(ob);
     return NULL;
 }
 
 /* PatchInspect */
-static PyObject* __Pyx_patch_inspect(PyObject* module) {
+  static PyObject* __Pyx_patch_inspect(PyObject* module) {
 #if defined(__Pyx_Generator_USED) && (!defined(CYTHON_PATCH_INSPECT) || CYTHON_PATCH_INSPECT)
     static int inspect_patched = 0;
     if (unlikely((!inspect_patched) && module)) {
         module = __Pyx_Coroutine_patch_module(
             module, ""
 "old_types = getattr(_module.isgenerator, '_cython_generator_types', None)\n"
 "if old_types is None or not isinstance(old_types, set):\n"
@@ -96116,15 +96248,15 @@
 #else
     if ((0)) return __Pyx_Coroutine_patch_module(module, NULL);
 #endif
     return module;
 }
 
 /* PatchAsyncIO */
-static PyObject* __Pyx_patch_asyncio(PyObject* module) {
+  static PyObject* __Pyx_patch_asyncio(PyObject* module) {
 #if PY_VERSION_HEX < 0x030500B2 &&\
         (defined(__Pyx_Coroutine_USED) || defined(__Pyx_Generator_USED)) &&\
         (!defined(CYTHON_PATCH_ASYNCIO) || CYTHON_PATCH_ASYNCIO)
     PyObject *patch_module = NULL;
     static int asyncio_patched = 0;
     if (unlikely((!asyncio_patched) && module)) {
         PyObject *package;
@@ -96199,15 +96331,15 @@
 #else
     if ((0)) return __Pyx_patch_inspect(__Pyx_Coroutine_patch_module(module, NULL));
 #endif
     return module;
 }
 
 /* CalculateMetaclass */
-static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
+  static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
     Py_ssize_t i, nbases = PyTuple_GET_SIZE(bases);
     for (i=0; i < nbases; i++) {
         PyTypeObject *tmptype;
         PyObject *tmp = PyTuple_GET_ITEM(bases, i);
         tmptype = Py_TYPE(tmp);
 #if PY_MAJOR_VERSION < 3
         if (tmptype == &PyClass_Type)
@@ -96238,15 +96370,15 @@
 #endif
     }
     Py_INCREF((PyObject*) metaclass);
     return (PyObject*) metaclass;
 }
 
 /* Py3ClassCreate */
-static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
+  static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
                                            PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
     PyObject *ns;
     if (metaclass) {
         PyObject *prep = __Pyx_PyObject_GetAttrStr(metaclass, __pyx_n_s_prepare_2);
         if (prep) {
             PyObject *pargs = PyTuple_Pack(2, name, bases);
             if (unlikely(!pargs)) {
@@ -96305,15 +96437,15 @@
         Py_DECREF(margs);
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
-#ifndef CYTHON_CLINE_IN_TRACEBACK
+  #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
@@ -96347,15 +96479,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -96427,15 +96559,15 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-#include "compile.h"
+  #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
@@ -96534,15 +96666,15 @@
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 /* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -96556,15 +96688,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* UnicodeAsUCS4 */
-static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
+  static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
    Py_ssize_t length;
    #if CYTHON_PEP393_ENABLED
    length = PyUnicode_GET_LENGTH(x);
    if (likely(length == 1)) {
        return PyUnicode_READ_CHAR(x, 0);
    }
    #else
@@ -96587,15 +96719,15 @@
    PyErr_Format(PyExc_ValueError,
                 "only single character unicode strings can be converted to Py_UCS4, "
                 "got length %" CYTHON_FORMAT_SSIZE_T "d", length);
    return (Py_UCS4)-1;
 }
 
 /* Declarations */
-#if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -96607,15 +96739,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-#if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -96741,15 +96873,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-#if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -96761,15 +96893,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-#if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -96895,15 +97027,15 @@
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage(enum __pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage(enum __pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -96933,15 +97065,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_AuthenticationMessage),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int32_t(int32_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int32_t(int32_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int32_t neg_one = (int32_t) -1, const_zero = (int32_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -96971,15 +97103,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int32_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int32_t __Pyx_PyInt_As_int32_t(PyObject *x) {
+  static CYTHON_INLINE int32_t __Pyx_PyInt_As_int32_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int32_t neg_one = (int32_t) -1, const_zero = (int32_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97167,15 +97299,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int32_t");
     return (int32_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus(enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus(enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97205,15 +97337,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus(PyObject *x) {
+  static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97401,15 +97533,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus");
     return (enum __pyx_t_7asyncpg_8protocol_8protocol_ConnectionStatus) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ResultType(enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ResultType(enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97439,15 +97571,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ResultType(PyObject *x) {
+  static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ResultType(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97635,15 +97767,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType");
     return (enum __pyx_t_7asyncpg_8protocol_8protocol_ResultType) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ProtocolState(enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ProtocolState(enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97673,15 +97805,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ProtocolState(PyObject *x) {
+  static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ProtocolState(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97869,15 +98001,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState");
     return (enum __pyx_t_7asyncpg_8protocol_8protocol_ProtocolState) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus(enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus(enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -97907,15 +98039,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus(PyObject *x) {
+  static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98103,15 +98235,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus");
     return (enum __pyx_t_7asyncpg_8protocol_8protocol_TransactionStatus) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint64_t neg_one = (uint64_t) -1, const_zero = (uint64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98141,15 +98273,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(uint64_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *x) {
+  static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint64_t neg_one = (uint64_t) -1, const_zero = (uint64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98337,15 +98469,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint64_t");
     return (uint64_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE uint32_t __Pyx_PyInt_As_uint32_t(PyObject *x) {
+  static CYTHON_INLINE uint32_t __Pyx_PyInt_As_uint32_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint32_t neg_one = (uint32_t) -1, const_zero = (uint32_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98533,15 +98665,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint32_t");
     return (uint32_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat(PyObject *x) {
+  static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98729,15 +98861,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat");
     return (enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat(enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat(enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98767,15 +98899,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_ServerDataFormat),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -98963,15 +99095,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99159,15 +99291,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat(enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat(enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99197,15 +99329,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_CodecType(enum __pyx_t_7asyncpg_8protocol_8protocol_CodecType value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_7asyncpg_8protocol_8protocol_CodecType(enum __pyx_t_7asyncpg_8protocol_8protocol_CodecType value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_CodecType neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_CodecType) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_CodecType) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99235,15 +99367,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_7asyncpg_8protocol_8protocol_CodecType),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint32_t neg_one = (uint32_t) -1, const_zero = (uint32_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99273,15 +99405,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(uint32_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99311,15 +99443,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99349,15 +99481,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat(PyObject *x) {
+  static CYTHON_INLINE enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat __Pyx_PyInt_As_enum____pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat neg_one = (enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat) -1, const_zero = (enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99545,15 +99677,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat");
     return (enum __pyx_t_7asyncpg_8protocol_8protocol_ClientExchangeFormat) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
+  static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99741,15 +99873,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int64_t");
     return (int64_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99779,15 +99911,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int64_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_ptrdiff_t(ptrdiff_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_ptrdiff_t(ptrdiff_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const ptrdiff_t neg_one = (ptrdiff_t) -1, const_zero = (ptrdiff_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99817,15 +99949,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(ptrdiff_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99855,15 +99987,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(char),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int16_t(int16_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int16_t(int16_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int16_t neg_one = (int16_t) -1, const_zero = (int16_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -99893,15 +100025,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int16_t),
                                      little, !is_unsigned);
     }
 }
 
 /* ObjectAsUCS4 */
-static Py_UCS4 __Pyx__PyObject_AsPy_UCS4_raise_error(long ival) {
+  static Py_UCS4 __Pyx__PyObject_AsPy_UCS4_raise_error(long ival) {
    if (ival < 0) {
        if (!PyErr_Occurred())
            PyErr_SetString(PyExc_OverflowError,
                            "cannot convert negative value to Py_UCS4");
    } else {
        PyErr_SetString(PyExc_OverflowError,
                        "value too large to convert to Py_UCS4");
@@ -99914,15 +100046,15 @@
    if (unlikely(!__Pyx_is_valid_index(ival, 1114111 + 1))) {
        return __Pyx__PyObject_AsPy_UCS4_raise_error(ival);
    }
    return (Py_UCS4)ival;
 }
 
 /* Generator */
-static PyMethodDef __pyx_Generator_methods[] = {
+  static PyMethodDef __pyx_Generator_methods[] = {
     {"send", (PyCFunction) __Pyx_Coroutine_Send, METH_O,
      (char*) PyDoc_STR("send(arg) -> send 'arg' into generator,\nreturn next yielded value or raise StopIteration.")},
     {"throw", (PyCFunction) __Pyx_Coroutine_Throw, METH_VARARGS,
      (char*) PyDoc_STR("throw(typ[,val[,tb]]) -> raise exception in generator,\nreturn next yielded value or raise StopIteration.")},
     {"close", (PyCFunction) __Pyx_Coroutine_Close_Method, METH_NOARGS,
      (char*) PyDoc_STR("close() -> raise GeneratorExit inside generator.")},
     {0, 0, 0, 0}
@@ -100017,15 +100149,15 @@
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* IterableCoroutine */
-static PyTypeObject __pyx_IterableCoroutineType_type = {
+  static PyTypeObject __pyx_IterableCoroutineType_type = {
     PyVarObject_HEAD_INIT(0, 0)
     "iterable_coroutine",
     sizeof(__pyx_CoroutineObject),
     0,
     (destructor) __Pyx_Coroutine_dealloc,
     0,
     0,
@@ -100099,15 +100231,15 @@
     __pyx_IterableCoroutineType = __Pyx_FetchCommonType(&__pyx_IterableCoroutineType_type);
     if (unlikely(!__pyx_IterableCoroutineType))
         return -1;
     return 0;
 }
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
+  static int __Pyx_check_binary_version(void) {
     char ctversion[5];
     int same=1, i, found_dot;
     const char* rt_from_call = Py_GetVersion();
     PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     found_dot = 0;
     for (i = 0; i < 4; i++) {
         if (!ctversion[i]) {
@@ -100137,15 +100269,15 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrExport */
-static int __Pyx_ExportVoidPtr(PyObject *name, void *p, const char *sig) {
+  static int __Pyx_ExportVoidPtr(PyObject *name, void *p, const char *sig) {
     PyObject *d;
     PyObject *cobj = 0;
     d = PyDict_GetItem(__pyx_d, __pyx_n_s_pyx_capi);
     Py_XINCREF(d);
     if (!d) {
         d = PyDict_New();
         if (!d)
@@ -100168,15 +100300,15 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction
+  #ifndef __PYX_HAVE_RT_ImportFunction
 #define __PYX_HAVE_RT_ImportFunction
 static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
@@ -100222,15 +100354,15 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* InitStrings */
-static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
```

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/protocol.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/protocol.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/record/recordobj.c` & `asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.c`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/record/recordobj.h` & `asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/scram.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/scram.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/settings.pxd` & `asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/protocol/settings.pyx` & `asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/rkt.py` & `asyncpg-rkt-0.27.1/asyncpg/rkt.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/serverversion.py` & `asyncpg-rkt-0.27.1/asyncpg/serverversion.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/transaction.py` & `asyncpg-rkt-0.27.1/asyncpg/transaction.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/types.py` & `asyncpg-rkt-0.27.1/asyncpg/types.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg/utils.py` & `asyncpg-rkt-0.27.1/asyncpg/utils.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/PKG-INFO` & `asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-rkt
-Version: 0.27.0
+Version: 0.27.1
 Summary: An asyncio PostgreSQL driver that returns numpy arrays
 Home-page: https://github.com/MagicStack/asyncpg
 Author: MagicStack Inc
 Author-email: hello@magic.io
 License: Apache License, Version 2.0
 Platform: macOS
 Platform: POSIX
```

### Comparing `asyncpg-rkt-0.27.0/asyncpg_rkt.egg-info/SOURCES.txt` & `asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/Makefile` & `asyncpg-rkt-0.27.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/api/index.rst` & `asyncpg-rkt-0.27.1/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/conf.py` & `asyncpg-rkt-0.27.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/faq.rst` & `asyncpg-rkt-0.27.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/index.rst` & `asyncpg-rkt-0.27.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/installation.rst` & `asyncpg-rkt-0.27.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/docs/usage.rst` & `asyncpg-rkt-0.27.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/performance.png` & `asyncpg-rkt-0.27.1/performance.png`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/pyproject.toml` & `asyncpg-rkt-0.27.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/setup.py` & `asyncpg-rkt-0.27.1/setup.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/__init__.py` & `asyncpg-rkt-0.27.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/ca.cert.pem` & `asyncpg-rkt-0.27.1/tests/certs/ca.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/ca.crl.pem` & `asyncpg-rkt-0.27.1/tests/certs/ca.crl.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/ca.key.pem` & `asyncpg-rkt-0.27.1/tests/certs/ca.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/client.cert.pem` & `asyncpg-rkt-0.27.1/tests/certs/client.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/client.csr.pem` & `asyncpg-rkt-0.27.1/tests/certs/client.csr.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/client.key.pem` & `asyncpg-rkt-0.27.1/tests/certs/client.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/client.key.protected.pem` & `asyncpg-rkt-0.27.1/tests/certs/client.key.protected.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/client_ca.cert.pem` & `asyncpg-rkt-0.27.1/tests/certs/client_ca.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/client_ca.key.pem` & `asyncpg-rkt-0.27.1/tests/certs/client_ca.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/gen.py` & `asyncpg-rkt-0.27.1/tests/certs/gen.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/server.cert.pem` & `asyncpg-rkt-0.27.1/tests/certs/server.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/certs/server.key.pem` & `asyncpg-rkt-0.27.1/tests/certs/server.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/histogram.py` & `asyncpg-rkt-0.27.1/tests/histogram.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test__environment.py` & `asyncpg-rkt-0.27.1/tests/test__environment.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test__sourcecode.py` & `asyncpg-rkt-0.27.1/tests/test__sourcecode.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_adversity.py` & `asyncpg-rkt-0.27.1/tests/test_adversity.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_cache_invalidation.py` & `asyncpg-rkt-0.27.1/tests/test_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_cancellation.py` & `asyncpg-rkt-0.27.1/tests/test_cancellation.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_codecs.py` & `asyncpg-rkt-0.27.1/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_connect.py` & `asyncpg-rkt-0.27.1/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_copy.py` & `asyncpg-rkt-0.27.1/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_cursor.py` & `asyncpg-rkt-0.27.1/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_exceptions.py` & `asyncpg-rkt-0.27.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_execute.py` & `asyncpg-rkt-0.27.1/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_introspection.py` & `asyncpg-rkt-0.27.1/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_listeners.py` & `asyncpg-rkt-0.27.1/tests/test_listeners.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_numpy.py` & `asyncpg-rkt-0.27.1/tests/test_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         dtype, baseline, value_strs, nulls, _ = \
             self.setup_standard_codecs(True)
         for length in (0, 1, 512, 513, 1024):
             query = f"SELECT {', '.join(value_strs)}\n" \
                     f"FROM generate_series(1, {length}) i"
 
             stmt = await self.con.prepare(
-                set_query_dtype(query, dtype)
+                f"--skip\n{set_query_dtype(query, dtype)}"
             )
             with self.subTest(length=length):
                 fetched_array, fetched_nulls = await stmt.fetch()
 
                 self.assertIsInstance(fetched_nulls, list)
                 self.assertEqual(len(fetched_nulls), len(nulls) * length)
                 if length > 0:
```

### Comparing `asyncpg-rkt-0.27.0/tests/test_numpy_benchmark.py` & `asyncpg-rkt-0.27.1/tests/test_numpy_benchmark.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_pool.py` & `asyncpg-rkt-0.27.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_prepare.py` & `asyncpg-rkt-0.27.1/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_record.py` & `asyncpg-rkt-0.27.1/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_rkt.py` & `asyncpg-rkt-0.27.1/tests/test_rkt.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_test.py` & `asyncpg-rkt-0.27.1/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_timeout.py` & `asyncpg-rkt-0.27.1/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_transaction.py` & `asyncpg-rkt-0.27.1/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_types.py` & `asyncpg-rkt-0.27.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.0/tests/test_utils.py` & `asyncpg-rkt-0.27.1/tests/test_utils.py`

 * *Files identical despite different names*

