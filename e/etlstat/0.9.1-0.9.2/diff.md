# Comparing `tmp/etlstat-0.9.1.tar.gz` & `tmp/etlstat-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etlstat-0.9.1.tar", last modified: Mon Apr 10 07:59:28 2023, max compression
+gzip compressed data, was "etlstat-0.9.2.tar", last modified: Wed Apr 12 11:48:52 2023, max compression
```

## Comparing `etlstat-0.9.1.tar` & `etlstat-0.9.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     8667 2021-05-12 11:14:17.000000 etlstat-0.9.1/.pylintrc
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      384 2022-07-14 07:12:25.000000 etlstat-0.9.1/.travis.yml
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1356 2023-04-10 07:56:32.000000 etlstat-0.9.1/CHANGELOG.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11323 2021-05-12 11:14:17.000000 etlstat-0.9.1/LICENSE.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      907 2023-04-10 07:49:18.000000 etlstat-0.9.1/MANIFEST.in
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-10 07:59:28.264006 etlstat-0.9.1/PKG-INFO
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1305 2023-02-16 13:48:24.000000 etlstat-0.9.1/Pipfile
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    57266 2023-04-10 07:46:25.000000 etlstat-0.9.1/Pipfile.lock
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      266 2021-05-12 11:14:17.000000 etlstat-0.9.1/README.rst
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.208006 etlstat-0.9.1/docs/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/docs/source/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7782 2021-10-18 11:25:24.000000 etlstat-0.9.1/docs/source/conf.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      494 2021-05-12 11:14:17.000000 etlstat-0.9.1/docs/source/index.rst
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      225 2021-05-12 11:14:17.000000 etlstat-0.9.1/docs/source/modules.rst
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/etlstat/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/etlstat/database/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     4639 2021-10-28 13:02:54.000000 etlstat-0.9.1/etlstat/database/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/__init__.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11111 2023-02-16 13:39:52.000000 etlstat-0.9.1/etlstat/database/mysql.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    10583 2023-02-16 11:50:51.000000 etlstat-0.9.1/etlstat/database/oracle.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3946 2023-02-16 11:51:00.000000 etlstat-0.9.1/etlstat/database/postgresql.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/database/test/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1846 2021-10-18 11:25:24.000000 etlstat-0.9.1/etlstat/database/test/22350.px
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/__init__.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1079 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/pmh.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/pmh_update.csv
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1271 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/px_01001.csv
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    15093 2023-02-16 13:39:31.000000 etlstat-0.9.1/etlstat/database/test/test_mysql.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     8709 2023-02-16 13:38:55.000000 etlstat-0.9.1/etlstat/database/test/test_oracle.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3249 2021-10-28 13:02:54.000000 etlstat-0.9.1/etlstat/database/test/test_postgresql.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     2640 2023-02-16 13:37:38.000000 etlstat-0.9.1/etlstat/database/test/test_sqlloader.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      332 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/__init__.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    18326 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/extractor.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/test/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.212005 etlstat-0.9.1/etlstat/extractor/test/data/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/test/data/csv/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/AEREO_SER_06_15.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/AEREO_SER_06_15.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1514 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1875 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/test/data/excel/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/excel/excel_prueba.xls
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/excel/prueba_excel.xls
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.236005 etlstat-0.9.1/etlstat/extractor/test/data/positional/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     2982 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3476 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     4994 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    38412 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    26514 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    24900 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    16986 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   259350 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   534625 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      560 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5865 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7680 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    11275 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3699 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52216 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      612 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1412 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    87580 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     6120 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52920 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       36 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/WHITE_SPACES.TXT
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.240005 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      629 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      451 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/ALOJ_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      371 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AUDIOV_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      567 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/CONS_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      983 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/INFOR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      605 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/JURID_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      428 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/LIMPI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      989 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1487 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MENOR_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      382 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/OPIN_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      575 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PERSON_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1082 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/POST_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      581 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      502 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/SSCC_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      686 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TEC_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      639 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TFERR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      506 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TMAR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1139 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TMER_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      592 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TUI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      743 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       72 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/WHITE_SPACES.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.240005 etlstat-0.9.1/etlstat/extractor/test/data/px/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    18192 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/px/o20012.px
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13264 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/px/o20013.px
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      166 2023-02-16 13:50:14.000000 etlstat-0.9.1/etlstat/extractor/test/data/px/pcaxis_urls.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.260005 etlstat-0.9.1/etlstat/extractor/test/data/px_file/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   768984 2021-10-18 11:25:24.000000 etlstat-0.9.1/etlstat/extractor/test/data/px_file/27066.px
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.260005 etlstat-0.9.1/etlstat/extractor/test/data/sql/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1583 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/sql/afiliados.sql
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     3024 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/sql/contratos.sql
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    13618 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/sql/ratios.sql
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/extractor/test/data/xml/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    28811 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Comex.kjb
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26043 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24654 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26252 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24666 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24501 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24796 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26158 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26697 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24643 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)   192858 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    12422 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/test_extractor.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/log/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      112 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       23 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/__init__.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      739 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/logging.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      683 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/timing.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      316 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/README.rst
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/test/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.212005 etlstat-0.9.1/etlstat/text/test/data/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/test/data/jobs/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13315 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      522 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/data/jobs/Uso com_elec.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/test/data/output/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13001 2023-02-16 13:50:15.000000 etlstat-0.9.1/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1621 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/test_utils.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3998 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/utils.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/etlstat.egg-info/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/PKG-INFO
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5186 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/SOURCES.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)        1 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/dependency_links.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      448 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/requires.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)        8 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/top_level.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1271 2023-04-10 07:50:08.000000 etlstat-0.9.1/requirements.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      204 2023-04-10 07:59:28.268005 etlstat-0.9.1/setup.cfg
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1867 2023-04-10 07:56:04.000000 etlstat-0.9.1/setup.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     8667 2021-05-12 11:14:17.000000 etlstat-0.9.2/.pylintrc
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      384 2022-07-14 07:12:25.000000 etlstat-0.9.2/.travis.yml
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1404 2023-04-12 11:37:18.000000 etlstat-0.9.2/CHANGELOG.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11323 2021-05-12 11:14:17.000000 etlstat-0.9.2/LICENSE.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      907 2023-04-10 07:49:18.000000 etlstat-0.9.2/MANIFEST.in
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-12 11:48:52.367405 etlstat-0.9.2/PKG-INFO
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      970 2023-04-12 11:46:04.000000 etlstat-0.9.2/Pipfile
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    57615 2023-04-12 11:46:54.000000 etlstat-0.9.2/Pipfile.lock
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      266 2021-05-12 11:14:17.000000 etlstat-0.9.2/README.rst
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.343405 etlstat-0.9.2/docs/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/docs/source/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7782 2021-10-18 11:25:24.000000 etlstat-0.9.2/docs/source/conf.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      494 2021-05-12 11:14:17.000000 etlstat-0.9.2/docs/source/index.rst
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      225 2021-05-12 11:14:17.000000 etlstat-0.9.2/docs/source/modules.rst
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/etlstat/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/database/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     4639 2021-10-28 13:02:54.000000 etlstat-0.9.2/etlstat/database/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/__init__.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11111 2023-02-16 13:39:52.000000 etlstat-0.9.2/etlstat/database/mysql.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    10583 2023-02-16 11:50:51.000000 etlstat-0.9.2/etlstat/database/oracle.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3946 2023-02-16 11:51:00.000000 etlstat-0.9.2/etlstat/database/postgresql.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/database/test/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1846 2021-10-18 11:25:24.000000 etlstat-0.9.2/etlstat/database/test/22350.px
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/__init__.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1079 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/pmh.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/pmh_update.csv
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1271 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/px_01001.csv
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    15094 2023-04-12 11:16:23.000000 etlstat-0.9.2/etlstat/database/test/test_mysql.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     8709 2023-02-16 13:38:55.000000 etlstat-0.9.2/etlstat/database/test/test_oracle.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3249 2021-10-28 13:02:54.000000 etlstat-0.9.2/etlstat/database/test/test_postgresql.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     2640 2023-02-16 13:37:38.000000 etlstat-0.9.2/etlstat/database/test/test_sqlloader.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/extractor/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      332 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/__init__.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    18326 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/extractor.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/extractor/test/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/etlstat/extractor/test/data/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/extractor/test/data/csv/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/AEREO_SER_06_15.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/AEREO_SER_06_15.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1514 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1875 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.355404 etlstat-0.9.2/etlstat/extractor/test/data/excel/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/excel/excel_prueba.xls
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/excel/prueba_excel.xls
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.359405 etlstat-0.9.2/etlstat/extractor/test/data/positional/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     2982 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3476 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     4994 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    38412 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    26514 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    24900 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    16986 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   259350 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   534625 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      560 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5865 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7680 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    11275 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3699 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52216 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      612 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1412 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    87580 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     6120 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52920 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       36 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/WHITE_SPACES.TXT
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.359405 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      629 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      451 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/ALOJ_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      371 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AUDIOV_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      567 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/CONS_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      983 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/INFOR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      605 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/JURID_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      428 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/LIMPI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      989 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1487 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MENOR_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      382 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/OPIN_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      575 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PERSON_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1082 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/POST_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      581 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      502 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/SSCC_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      686 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TEC_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      639 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TFERR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      506 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TMAR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1139 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TMER_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      592 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TUI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      743 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       72 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/WHITE_SPACES.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/px/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    18192 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/px/o20012.px
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13264 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/px/o20013.px
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      166 2023-04-12 11:48:31.000000 etlstat-0.9.2/etlstat/extractor/test/data/px/pcaxis_urls.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/px_file/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   768984 2021-10-18 11:25:24.000000 etlstat-0.9.2/etlstat/extractor/test/data/px_file/27066.px
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/sql/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1583 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/sql/afiliados.sql
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     3024 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/sql/contratos.sql
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    13618 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/sql/ratios.sql
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/xml/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    28811 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Comex.kjb
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26043 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24654 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26252 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24666 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24501 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24796 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26158 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26697 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24643 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)   192858 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    12422 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/test_extractor.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/log/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      112 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       23 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/__init__.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      739 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/logging.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      683 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/timing.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      316 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/README.rst
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/test/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/etlstat/text/test/data/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/test/data/jobs/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13315 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      522 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/data/jobs/Uso com_elec.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/test/data/output/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13001 2023-04-12 11:48:32.000000 etlstat-0.9.2/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1621 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/test_utils.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3998 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/utils.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat.egg-info/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/PKG-INFO
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5186 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/SOURCES.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)        1 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/dependency_links.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      231 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/requires.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)        8 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/top_level.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1362 2023-04-12 11:19:46.000000 etlstat-0.9.2/requirements.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      204 2023-04-12 11:48:52.367405 etlstat-0.9.2/setup.cfg
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1811 2023-04-12 11:38:40.000000 etlstat-0.9.2/setup.py
```

### Comparing `etlstat-0.9.1/.pylintrc` & `etlstat-0.9.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/CHANGELOG.txt` & `etlstat-0.9.2/CHANGELOG.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v0.9.2:
+    - Fix dependencies.
+    - Fix test.
 v0.9.1:
     - Fix dependencies.
 v0.9.0:
     - Add management for database exceptions.
     - Update dependencies.
 v0.8.2:
     - fix dependencies.
```

### Comparing `etlstat-0.9.1/LICENSE.txt` & `etlstat-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/MANIFEST.in` & `etlstat-0.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/PKG-INFO` & `etlstat-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etlstat
-Version: 0.9.1
+Version: 0.9.2
 Summary: ETL utils for statistical offices data processing
 Home-page: https://github.com/icane/etlstat.git
 Author: Instituto Cántabro de Estadística
 Author-email: icane@cantabria.es
 License: Apache License 2.0
 Keywords: etl,icane,statistics,utils
 Classifier: Development Status :: 4 - Beta
```

### Comparing `etlstat-0.9.1/Pipfile.lock` & `etlstat-0.9.2/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9798181154888471%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'6298ceed25c52c005a96ae43209be463250230fa5101fb2f3b01229ac40b928b'}}",*

 * * "'default'": "{'beautifulsoup4': {'hashes': "*

 * *              "['sha256:9a315ce70049920ea4572a4055bc4bd700c940521d36fc858205ad4fcde149bf', "*

 * *              "'sha256:c23ad23c521d818955a4151a67d81580319d4bf548d3d49f4223ae041ff98891'], "*

 * *              "'version': '==4.10.0', delete: ['version >=']}, 'numpy': {'hashes': "*

 * *              "['sha256:003a9f530e880cb2cd177cba1af7220b9aa42def9c4afc2a2fc […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "b6c9a60d32376d06658aff8e17d02ec4c02a32fee1c67c8086e2e91ed7c65df1"
+            "sha256": "6298ceed25c52c005a96ae43209be463250230fa5101fb2f3b01229ac40b928b"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9.*"
         },
         "sources": [
             {
@@ -14,20 +14,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "beautifulsoup4": {
             "hashes": [
-                "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da",
-                "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"
+                "sha256:9a315ce70049920ea4572a4055bc4bd700c940521d36fc858205ad4fcde149bf",
+                "sha256:c23ad23c521d818955a4151a67d81580319d4bf548d3d49f4223ae041ff98891"
             ],
             "index": "pypi",
-            "version": "==4.12.2",
-            "version >=": "4.10.*"
+            "version": "==4.10.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
@@ -232,45 +231,45 @@
                 "sha256:1733e6ce52a049243de3264f1fbc22a852cb35458c4ad739ba88189285efdf32"
             ],
             "index": "pypi",
             "version": "==2.2.9"
         },
         "numpy": {
             "hashes": [
-                "sha256:01dd17cbb340bf0fc23981e52e1d18a9d4050792e8fb8363cecbf066a84b827d",
-                "sha256:06005a2ef6014e9956c09ba07654f9837d9e26696a0470e42beedadb78c11b07",
-                "sha256:09b7847f7e83ca37c6e627682f145856de331049013853f344f37b0c9690e3df",
-                "sha256:0aaee12d8883552fadfc41e96b4c82ee7d794949e2a7c3b3a7201e968c7ecab9",
-                "sha256:0cbe9848fad08baf71de1a39e12d1b6310f1d5b2d0ea4de051058e6e1076852d",
-                "sha256:1b1766d6f397c18153d40015ddfc79ddb715cabadc04d2d228d4e5a8bc4ded1a",
-                "sha256:33161613d2269025873025b33e879825ec7b1d831317e68f4f2f0f84ed14c719",
-                "sha256:5039f55555e1eab31124a5768898c9e22c25a65c1e0037f4d7c495a45778c9f2",
-                "sha256:522e26bbf6377e4d76403826ed689c295b0b238f46c28a7251ab94716da0b280",
-                "sha256:56e454c7833e94ec9769fa0f86e6ff8e42ee38ce0ce1fa4cbb747ea7e06d56aa",
-                "sha256:58f545efd1108e647604a1b5aa809591ccd2540f468a880bedb97247e72db387",
-                "sha256:5e05b1c973a9f858c74367553e236f287e749465f773328c8ef31abe18f691e1",
-                "sha256:7903ba8ab592b82014713c491f6c5d3a1cde5b4a3bf116404e08f5b52f6daf43",
-                "sha256:8969bfd28e85c81f3f94eb4a66bc2cf1dbdc5c18efc320af34bffc54d6b1e38f",
-                "sha256:92c8c1e89a1f5028a4c6d9e3ccbe311b6ba53694811269b992c0b224269e2398",
-                "sha256:9c88793f78fca17da0145455f0d7826bcb9f37da4764af27ac945488116efe63",
-                "sha256:a7ac231a08bb37f852849bbb387a20a57574a97cfc7b6cabb488a4fc8be176de",
-                "sha256:abdde9f795cf292fb9651ed48185503a2ff29be87770c3b8e2a14b0cd7aa16f8",
-                "sha256:af1da88f6bc3d2338ebbf0e22fe487821ea4d8e89053e25fa59d1d79786e7481",
-                "sha256:b2a9ab7c279c91974f756c84c365a669a887efa287365a8e2c418f8b3ba73fb0",
-                "sha256:bf837dc63ba5c06dc8797c398db1e223a466c7ece27a1f7b5232ba3466aafe3d",
-                "sha256:ca51fcfcc5f9354c45f400059e88bc09215fb71a48d3768fb80e357f3b457e1e",
-                "sha256:ce571367b6dfe60af04e04a1834ca2dc5f46004ac1cc756fb95319f64c095a96",
-                "sha256:d208a0f8729f3fb790ed18a003f3a57895b989b40ea4dce4717e9cf4af62c6bb",
-                "sha256:dbee87b469018961d1ad79b1a5d50c0ae850000b639bcb1b694e9981083243b6",
-                "sha256:e9f4c4e51567b616be64e05d517c79a8a22f3606499941d97bb76f2ca59f982d",
-                "sha256:f063b69b090c9d918f9df0a12116029e274daf0181df392839661c4c7ec9018a",
-                "sha256:f9a909a8bae284d46bbfdefbdd4a262ba19d3bc9921b1e76126b1d21c3c34135"
+                "sha256:003a9f530e880cb2cd177cba1af7220b9aa42def9c4afc2a2fc3ee6be7eb2b22",
+                "sha256:150947adbdfeceec4e5926d956a06865c1c690f2fd902efede4ca6fe2e657c3f",
+                "sha256:2620e8592136e073bd12ee4536149380695fbe9ebeae845b81237f986479ffc9",
+                "sha256:2eabd64ddb96a1239791da78fa5f4e1693ae2dadc82a76bc76a14cbb2b966e96",
+                "sha256:4173bde9fa2a005c2c6e2ea8ac1618e2ed2c1c6ec8a7657237854d42094123a0",
+                "sha256:4199e7cfc307a778f72d293372736223e39ec9ac096ff0a2e64853b866a8e18a",
+                "sha256:4cecaed30dc14123020f77b03601559fff3e6cd0c048f8b5289f4eeabb0eb281",
+                "sha256:557d42778a6869c2162deb40ad82612645e21d79e11c1dc62c6e82a2220ffb04",
+                "sha256:63e45511ee4d9d976637d11e6c9864eae50e12dc9598f531c035265991910468",
+                "sha256:6524630f71631be2dabe0c541e7675db82651eb998496bbe16bc4f77f0772253",
+                "sha256:76807b4063f0002c8532cfeac47a3068a69561e9c8715efdad3c642eb27c0756",
+                "sha256:7de8fdde0003f4294655aa5d5f0a89c26b9f22c0a58790c38fae1ed392d44a5a",
+                "sha256:889b2cc88b837d86eda1b17008ebeb679d82875022200c6e8e4ce6cf549b7acb",
+                "sha256:92011118955724465fb6853def593cf397b4a1367495e0b59a7e69d40c4eb71d",
+                "sha256:97cf27e51fa078078c649a51d7ade3c92d9e709ba2bfb97493007103c741f1d0",
+                "sha256:9a23f8440561a633204a67fb44617ce2a299beecf3295f0d13c495518908e910",
+                "sha256:a51725a815a6188c662fb66fb32077709a9ca38053f0274640293a14fdd22978",
+                "sha256:a77d3e1163a7770164404607b7ba3967fb49b24782a6ef85d9b5f54126cc39e5",
+                "sha256:adbdce121896fd3a17a77ab0b0b5eedf05a9834a18699db6829a64e1dfccca7f",
+                "sha256:c29e6bd0ec49a44d7690ecb623a8eac5ab8a923bce0bea6293953992edf3a76a",
+                "sha256:c72a6b2f4af1adfe193f7beb91ddf708ff867a3f977ef2ec53c0ffb8283ab9f5",
+                "sha256:d0a2db9d20117bf523dde15858398e7c0858aadca7c0f088ac0d6edd360e9ad2",
+                "sha256:e3ab5d32784e843fc0dd3ab6dcafc67ef806e6b6828dc6af2f689be0eb4d781d",
+                "sha256:e428c4fbfa085f947b536706a2fc349245d7baa8334f0c5723c56a10595f9b95",
+                "sha256:e8d2859428712785e8a8b7d2b3ef0a1d1565892367b32f915c4a4df44d0e64f5",
+                "sha256:eef70b4fc1e872ebddc38cddacc87c19a3709c0e3e5d20bf3954c147b1dd941d",
+                "sha256:f64bb98ac59b3ea3bf74b02f13836eb2e24e48e0ab0145bbda646295769bd780",
+                "sha256:f9006288bcf4895917d02583cf3411f98631275bc67cce355a7f39f8c14338fa"
             ],
-            "index": "pypi",
-            "version": "==1.23.5"
+            "markers": "python_version < '3.10' and platform_machine != 'aarch64' and platform_machine != 'arm64'",
+            "version": "==1.24.2"
         },
         "openpyxl": {
             "hashes": [
                 "sha256:0ab6d25d01799f97a9464630abacbb34aafecdcaa0ef3cba6d6b3499867d0355",
                 "sha256:e47805627aebcf860edb4edf7987b1309c1b3632f3750538ed962bbcc3bd7449"
             ],
             "index": "pypi",
@@ -575,15 +574,15 @@
             "version": "==2.0.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
-            "markers": "python_full_version >= '3.8.0'",
+            "markers": "python_version >= '3.8'",
             "version": "==5.12.0"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
                 "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
                 "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
@@ -718,19 +717,19 @@
                 "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
+                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.0"
         },
         "pylint": {
             "hashes": [
                 "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
                 "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
             ],
             "index": "pypi",
@@ -814,17 +813,25 @@
             "version": "==2.2.0"
         },
         "stevedore": {
             "hashes": [
                 "sha256:2c428d2338976279e8eb2196f7a94910960d9f7ba2f41f3988511e95ca447021",
                 "sha256:bd5a71ff5e5e5f5ea983880e4a1dd1bb47f8feebbb3d95b592398e2f02194771"
             ],
-            "markers": "python_full_version >= '3.8.0'",
+            "markers": "python_version >= '3.8'",
             "version": "==5.0.0"
         },
+        "toml": {
+            "hashes": [
+                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
+                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
+            ],
+            "index": "pypi",
+            "version": "==0.10.2"
+        },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
```

### Comparing `etlstat-0.9.1/docs/source/conf.py` & `etlstat-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/README.rst` & `etlstat-0.9.2/etlstat/database/README.rst`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/mysql.py` & `etlstat-0.9.2/etlstat/database/mysql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/oracle.py` & `etlstat-0.9.2/etlstat/database/oracle.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/postgresql.py` & `etlstat-0.9.2/etlstat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/test/22350.px` & `etlstat-0.9.2/etlstat/database/test/22350.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/test/pmh.csv` & `etlstat-0.9.2/etlstat/database/test/pmh.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/test/px_01001.csv` & `etlstat-0.9.2/etlstat/database/test/px_01001.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/test/test_mysql.py` & `etlstat-0.9.2/etlstat/database/test/test_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,28 +310,28 @@
 
     def test_complete_insert_from_pcaxis(self):
         """Check complete cycle by inserting a pcaxis file into a table."""
         my_conn = MySQL(*self.conn_params)
         Base = declarative_base()
         current_dir = os.path.dirname(os.path.abspath(__file__))
         parsed_pcaxis = pyaxis.parse(current_dir + '/22350.px',
-                                     encoding='ISO-8859-2')
+                                     encoding='ISO-8859-1')
         table_data = parsed_pcaxis['DATA']
         table_data = utils.parse_df_columns(table_data)
         table_data.name = 'ipc'
 
         class Ipc(Base):
             """Auxiliary sqlalchemy table model for the tests."""
 
             __tablename__ = 'ipc'
 
             id = Column(Integer, primary_key=True)
             comunidades_y_ciudades_autonomas = Column(String(100))
             grupos_ecoicop = Column(String(100))
-            tipo_de_dato = Column(String(50))
+            tipo_de_dato = Column(String(100))
             periodo = Column(String(50))
             data = Column(Float)
 
         Ipc.__table__.create(bind=my_conn.engine)
         my_conn.insert(table_data, if_exists='append')
         actual = my_conn.engine.scalar(
             select([func.count('*')]).select_from(Ipc)
@@ -342,15 +342,15 @@
 
     def test_insert_selected_columns(self):
         """Check insert method only with selected columns."""
         my_conn = MySQL(*self.conn_params)
         Base = declarative_base()
         current_dir = os.path.dirname(os.path.abspath(__file__))
         parsed_pcaxis = pyaxis.parse(current_dir + '/22350.px',
-                                     encoding='ISO-8859-2')
+                                     encoding='ISO-8859-1')
         table_data = parsed_pcaxis['DATA']
         table_data = utils.parse_df_columns(table_data)
         table_data.name = 'ipc'
 
         class Ipc(Base):
             """Auxiliary sqlalchemy table model for the tests."""
```

### Comparing `etlstat-0.9.1/etlstat/database/test/test_oracle.py` & `etlstat-0.9.2/etlstat/database/test/test_oracle.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/test/test_postgresql.py` & `etlstat-0.9.2/etlstat/database/test/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/database/test/test_sqlloader.py` & `etlstat-0.9.2/etlstat/database/test/test_sqlloader.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/extractor.py` & `etlstat-0.9.2/etlstat/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/excel/excel_prueba.xls` & `etlstat-0.9.2/etlstat/extractor/test/data/excel/excel_prueba.xls`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/excel/prueba_excel.xls` & `etlstat-0.9.2/etlstat/extractor/test/data/excel/prueba_excel.xls`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/CONS_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/CONS_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/INFOR_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/INFOR_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/JURID_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/JURID_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MENOR_COM.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MENOR_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PERSON_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PERSON_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/POST_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/POST_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TEC_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TEC_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TFERR_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TFERR_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TMER_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TMER_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TUI_SER.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TUI_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv` & `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/px/o20012.px` & `etlstat-0.9.2/etlstat/extractor/test/data/px/o20012.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/px/o20013.px` & `etlstat-0.9.2/etlstat/extractor/test/data/px/o20013.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/px_file/27066.px` & `etlstat-0.9.2/etlstat/extractor/test/data/px_file/27066.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/sql/afiliados.sql` & `etlstat-0.9.2/etlstat/extractor/test/data/sql/afiliados.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/sql/contratos.sql` & `etlstat-0.9.2/etlstat/extractor/test/data/sql/contratos.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/sql/ratios.sql` & `etlstat-0.9.2/etlstat/extractor/test/data/sql/ratios.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Comex.kjb` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Comex.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr` & `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/extractor/test/test_extractor.py` & `etlstat-0.9.2/etlstat/extractor/test/test_extractor.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/log/logging.py` & `etlstat-0.9.2/etlstat/log/logging.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/log/timing.py` & `etlstat-0.9.2/etlstat/log/timing.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb` & `etlstat-0.9.2/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/text/test/data/jobs/Uso com_elec.csv` & `etlstat-0.9.2/etlstat/text/test/data/jobs/Uso com_elec.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb` & `etlstat-0.9.2/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/text/test/test_utils.py` & `etlstat-0.9.2/etlstat/text/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat/text/utils.py` & `etlstat-0.9.2/etlstat/text/utils.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/etlstat.egg-info/PKG-INFO` & `etlstat-0.9.2/etlstat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etlstat
-Version: 0.9.1
+Version: 0.9.2
 Summary: ETL utils for statistical offices data processing
 Home-page: https://github.com/icane/etlstat.git
 Author: Instituto Cántabro de Estadística
 Author-email: icane@cantabria.es
 License: Apache License 2.0
 Keywords: etl,icane,statistics,utils
 Classifier: Development Status :: 4 - Beta
```

### Comparing `etlstat-0.9.1/etlstat.egg-info/SOURCES.txt` & `etlstat-0.9.2/etlstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.1/requirements.txt` & `etlstat-0.9.2/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 charset-normalizer==3.1.0; python_version >= '3.7'
 cx-oracle==7.3.0
 defusedxml==0.6.0
 et-xmlfile==1.1.0; python_version >= '3.6'
 greenlet==2.0.2; python_version >= '3' and platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 idna==3.4; python_version >= '3.5'
 mysql-connector==2.2.9
-numpy==1.23.5
+numpy==1.24.2; python_version < '3.10' and platform_machine != 'aarch64' and platform_machine != 'arm64'
 openpyxl==3.0.10
 pandas==1.4.4
 psycopg2==2.8.6
 pyaxis==0.3.4
 pyjstat==2.4.0
 python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-levenshtein==0.12.2
```

