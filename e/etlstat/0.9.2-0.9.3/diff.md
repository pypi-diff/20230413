# Comparing `tmp/etlstat-0.9.2.tar.gz` & `tmp/etlstat-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etlstat-0.9.2.tar", last modified: Wed Apr 12 11:48:52 2023, max compression
+gzip compressed data, was "etlstat-0.9.3.tar", last modified: Thu Apr 13 09:31:16 2023, max compression
```

## Comparing `etlstat-0.9.2.tar` & `etlstat-0.9.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     8667 2021-05-12 11:14:17.000000 etlstat-0.9.2/.pylintrc
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      384 2022-07-14 07:12:25.000000 etlstat-0.9.2/.travis.yml
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1404 2023-04-12 11:37:18.000000 etlstat-0.9.2/CHANGELOG.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11323 2021-05-12 11:14:17.000000 etlstat-0.9.2/LICENSE.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      907 2023-04-10 07:49:18.000000 etlstat-0.9.2/MANIFEST.in
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-12 11:48:52.367405 etlstat-0.9.2/PKG-INFO
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      970 2023-04-12 11:46:04.000000 etlstat-0.9.2/Pipfile
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    57615 2023-04-12 11:46:54.000000 etlstat-0.9.2/Pipfile.lock
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      266 2021-05-12 11:14:17.000000 etlstat-0.9.2/README.rst
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.343405 etlstat-0.9.2/docs/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/docs/source/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7782 2021-10-18 11:25:24.000000 etlstat-0.9.2/docs/source/conf.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      494 2021-05-12 11:14:17.000000 etlstat-0.9.2/docs/source/index.rst
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      225 2021-05-12 11:14:17.000000 etlstat-0.9.2/docs/source/modules.rst
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/etlstat/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/database/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     4639 2021-10-28 13:02:54.000000 etlstat-0.9.2/etlstat/database/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/__init__.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11111 2023-02-16 13:39:52.000000 etlstat-0.9.2/etlstat/database/mysql.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    10583 2023-02-16 11:50:51.000000 etlstat-0.9.2/etlstat/database/oracle.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3946 2023-02-16 11:51:00.000000 etlstat-0.9.2/etlstat/database/postgresql.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/database/test/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1846 2021-10-18 11:25:24.000000 etlstat-0.9.2/etlstat/database/test/22350.px
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/__init__.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1079 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/pmh.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/pmh_update.csv
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1271 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/database/test/px_01001.csv
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    15094 2023-04-12 11:16:23.000000 etlstat-0.9.2/etlstat/database/test/test_mysql.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     8709 2023-02-16 13:38:55.000000 etlstat-0.9.2/etlstat/database/test/test_oracle.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3249 2021-10-28 13:02:54.000000 etlstat-0.9.2/etlstat/database/test/test_postgresql.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     2640 2023-02-16 13:37:38.000000 etlstat-0.9.2/etlstat/database/test/test_sqlloader.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/extractor/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      332 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/__init__.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    18326 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/extractor.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/extractor/test/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/etlstat/extractor/test/data/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat/extractor/test/data/csv/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/AEREO_SER_06_15.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/AEREO_SER_06_15.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1514 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1875 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.355404 etlstat-0.9.2/etlstat/extractor/test/data/excel/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/excel/excel_prueba.xls
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/excel/prueba_excel.xls
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.359405 etlstat-0.9.2/etlstat/extractor/test/data/positional/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     2982 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3476 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     4994 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    38412 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    26514 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    24900 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    16986 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   259350 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   534625 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      560 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5865 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7680 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    11275 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3699 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52216 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      612 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1412 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    87580 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     6120 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52920 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       36 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/WHITE_SPACES.TXT
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.359405 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      629 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      451 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/ALOJ_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      371 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AUDIOV_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      567 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/CONS_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      983 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/INFOR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      605 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/JURID_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      428 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/LIMPI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      989 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1487 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MENOR_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      382 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/OPIN_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      575 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PERSON_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1082 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/POST_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      581 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      502 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/SSCC_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      686 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TEC_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      639 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TFERR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      506 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TMAR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1139 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TMER_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      592 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TUI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      743 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       72 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/positional/format/WHITE_SPACES.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/px/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    18192 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/px/o20012.px
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13264 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/data/px/o20013.px
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      166 2023-04-12 11:48:31.000000 etlstat-0.9.2/etlstat/extractor/test/data/px/pcaxis_urls.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/px_file/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   768984 2021-10-18 11:25:24.000000 etlstat-0.9.2/etlstat/extractor/test/data/px_file/27066.px
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/sql/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1583 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/sql/afiliados.sql
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     3024 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/sql/contratos.sql
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    13618 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/sql/ratios.sql
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.363405 etlstat-0.9.2/etlstat/extractor/test/data/xml/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    28811 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Comex.kjb
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26043 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24654 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26252 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24666 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24501 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24796 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26158 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26697 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24643 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)   192858 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    12422 2021-10-29 06:18:59.000000 etlstat-0.9.2/etlstat/extractor/test/test_extractor.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/log/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      112 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       23 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/__init__.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      739 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/logging.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      683 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/log/timing.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      316 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/README.rst
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/test/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.347405 etlstat-0.9.2/etlstat/text/test/data/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/test/data/jobs/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13315 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      522 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/data/jobs/Uso com_elec.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.367405 etlstat-0.9.2/etlstat/text/test/data/output/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13001 2023-04-12 11:48:32.000000 etlstat-0.9.2/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1621 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/test/test_utils.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3998 2021-05-12 11:14:17.000000 etlstat-0.9.2/etlstat/text/utils.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-12 11:48:52.351405 etlstat-0.9.2/etlstat.egg-info/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/PKG-INFO
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5186 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/SOURCES.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)        1 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/dependency_links.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      231 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/requires.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)        8 2023-04-12 11:48:52.000000 etlstat-0.9.2/etlstat.egg-info/top_level.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1362 2023-04-12 11:19:46.000000 etlstat-0.9.2/requirements.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      204 2023-04-12 11:48:52.367405 etlstat-0.9.2/setup.cfg
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1811 2023-04-12 11:38:40.000000 etlstat-0.9.2/setup.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.824845 etlstat-0.9.3/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     8667 2021-05-12 11:14:17.000000 etlstat-0.9.3/.pylintrc
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      384 2022-07-14 07:12:25.000000 etlstat-0.9.3/.travis.yml
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1436 2023-04-13 09:27:37.000000 etlstat-0.9.3/CHANGELOG.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11323 2021-05-12 11:14:17.000000 etlstat-0.9.3/LICENSE.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      907 2023-04-10 07:49:18.000000 etlstat-0.9.3/MANIFEST.in
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-13 09:31:16.824845 etlstat-0.9.3/PKG-INFO
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      932 2023-04-13 09:11:38.000000 etlstat-0.9.3/Pipfile
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    57338 2023-04-13 09:24:54.000000 etlstat-0.9.3/Pipfile.lock
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      266 2021-05-12 11:14:17.000000 etlstat-0.9.3/README.rst
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.796845 etlstat-0.9.3/docs/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.804845 etlstat-0.9.3/docs/source/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7782 2021-10-18 11:25:24.000000 etlstat-0.9.3/docs/source/conf.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      494 2021-05-12 11:14:17.000000 etlstat-0.9.3/docs/source/index.rst
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      225 2021-05-12 11:14:17.000000 etlstat-0.9.3/docs/source/modules.rst
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.804845 etlstat-0.9.3/etlstat/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.804845 etlstat-0.9.3/etlstat/database/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     4639 2021-10-28 13:02:54.000000 etlstat-0.9.3/etlstat/database/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/database/__init__.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11111 2023-04-12 12:01:00.000000 etlstat-0.9.3/etlstat/database/mysql.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    10583 2023-04-12 12:01:00.000000 etlstat-0.9.3/etlstat/database/oracle.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3946 2023-04-12 12:01:00.000000 etlstat-0.9.3/etlstat/database/postgresql.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.808845 etlstat-0.9.3/etlstat/database/test/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1846 2021-10-18 11:25:24.000000 etlstat-0.9.3/etlstat/database/test/22350.px
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/database/test/__init__.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1079 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/database/test/pmh.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/database/test/pmh_update.csv
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1271 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/database/test/px_01001.csv
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    15094 2023-04-12 12:01:00.000000 etlstat-0.9.3/etlstat/database/test/test_mysql.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     8709 2023-04-12 12:01:00.000000 etlstat-0.9.3/etlstat/database/test/test_oracle.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3249 2021-10-28 13:02:54.000000 etlstat-0.9.3/etlstat/database/test/test_postgresql.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     2640 2023-04-12 12:01:00.000000 etlstat-0.9.3/etlstat/database/test/test_sqlloader.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.808845 etlstat-0.9.3/etlstat/extractor/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      332 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/__init__.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    18326 2021-10-29 06:18:59.000000 etlstat-0.9.3/etlstat/extractor/extractor.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.808845 etlstat-0.9.3/etlstat/extractor/test/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.800845 etlstat-0.9.3/etlstat/extractor/test/data/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.808845 etlstat-0.9.3/etlstat/extractor/test/data/csv/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/csv/AEREO_SER_06_15.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/csv/AEREO_SER_06_15.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1514 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1875 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.808845 etlstat-0.9.3/etlstat/extractor/test/data/excel/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/excel/excel_prueba.xls
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/excel/prueba_excel.xls
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.812845 etlstat-0.9.3/etlstat/extractor/test/data/positional/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     2982 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3476 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     4994 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    38412 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    26514 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    24900 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    16986 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   259350 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   534625 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      560 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5865 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7680 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    11275 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3699 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52216 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      612 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1412 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    87580 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     6120 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52920 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       36 2021-10-29 06:18:59.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/WHITE_SPACES.TXT
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.816845 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      629 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      451 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/ALOJ_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      371 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/AUDIOV_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      567 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/CONS_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      983 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/INFOR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      605 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/JURID_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      428 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/LIMPI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      989 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1487 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/MENOR_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      382 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/OPIN_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      575 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/PERSON_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1082 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/POST_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      581 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      502 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/SSCC_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      686 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TEC_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      639 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TFERR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      506 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TMAR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1139 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TMER_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      592 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TUI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      743 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       72 2021-10-29 06:18:59.000000 etlstat-0.9.3/etlstat/extractor/test/data/positional/format/WHITE_SPACES.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.816845 etlstat-0.9.3/etlstat/extractor/test/data/px/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    18192 2021-10-29 06:18:59.000000 etlstat-0.9.3/etlstat/extractor/test/data/px/o20012.px
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13264 2021-10-29 06:18:59.000000 etlstat-0.9.3/etlstat/extractor/test/data/px/o20013.px
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      166 2023-04-13 08:34:59.000000 etlstat-0.9.3/etlstat/extractor/test/data/px/pcaxis_urls.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.820845 etlstat-0.9.3/etlstat/extractor/test/data/px_file/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   768984 2021-10-18 11:25:24.000000 etlstat-0.9.3/etlstat/extractor/test/data/px_file/27066.px
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.820845 etlstat-0.9.3/etlstat/extractor/test/data/sql/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1583 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/sql/afiliados.sql
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     3024 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/sql/contratos.sql
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    13618 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/sql/ratios.sql
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.820845 etlstat-0.9.3/etlstat/extractor/test/data/xml/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    28811 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Comex.kjb
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26043 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24654 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26252 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24666 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24501 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24796 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26158 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26697 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24643 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)   192858 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    12422 2021-10-29 06:18:59.000000 etlstat-0.9.3/etlstat/extractor/test/test_extractor.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.824845 etlstat-0.9.3/etlstat/log/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      112 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/log/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       23 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/log/__init__.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      739 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/log/logging.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      683 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/log/timing.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.824845 etlstat-0.9.3/etlstat/text/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      316 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/README.rst
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.824845 etlstat-0.9.3/etlstat/text/test/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/test/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.800845 etlstat-0.9.3/etlstat/text/test/data/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.824845 etlstat-0.9.3/etlstat/text/test/data/jobs/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13315 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      522 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/test/data/jobs/Uso com_elec.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.824845 etlstat-0.9.3/etlstat/text/test/data/output/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13001 2023-04-13 08:35:00.000000 etlstat-0.9.3/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1621 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/test/test_utils.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3998 2021-05-12 11:14:17.000000 etlstat-0.9.3/etlstat/text/utils.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-13 09:31:16.804845 etlstat-0.9.3/etlstat.egg-info/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-13 09:31:16.000000 etlstat-0.9.3/etlstat.egg-info/PKG-INFO
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5186 2023-04-13 09:31:16.000000 etlstat-0.9.3/etlstat.egg-info/SOURCES.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)        1 2023-04-13 09:31:16.000000 etlstat-0.9.3/etlstat.egg-info/dependency_links.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      212 2023-04-13 09:31:16.000000 etlstat-0.9.3/etlstat.egg-info/requires.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)        8 2023-04-13 09:31:16.000000 etlstat-0.9.3/etlstat.egg-info/top_level.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      217 2023-04-13 09:20:26.000000 etlstat-0.9.3/requirements.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      204 2023-04-13 09:31:16.824845 etlstat-0.9.3/setup.cfg
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1478 2023-04-13 09:20:52.000000 etlstat-0.9.3/setup.py
```

### Comparing `etlstat-0.9.2/.pylintrc` & `etlstat-0.9.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/CHANGELOG.txt` & `etlstat-0.9.3/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+v0.9.3:
+    - Fix dependencies.
 v0.9.2:
     - Fix dependencies.
     - Fix test.
 v0.9.1:
     - Fix dependencies.
 v0.9.0:
     - Add management for database exceptions.
```

### Comparing `etlstat-0.9.2/LICENSE.txt` & `etlstat-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/MANIFEST.in` & `etlstat-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/PKG-INFO` & `etlstat-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etlstat
-Version: 0.9.2
+Version: 0.9.3
 Summary: ETL utils for statistical offices data processing
 Home-page: https://github.com/icane/etlstat.git
 Author: Instituto Cántabro de Estadística
 Author-email: icane@cantabria.es
 License: Apache License 2.0
 Keywords: etl,icane,statistics,utils
 Classifier: Development Status :: 4 - Beta
```

### Comparing `etlstat-0.9.2/Pipfile` & `etlstat-0.9.3/Pipfile`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 flake8-blind-except = {index = "pypi",version = "*"}
 flake8-builtins = {index = "pypi",version = "*"}
 flake8-docstrings = {index = "pypi",version = "*"}
 flake8-import-order = {index = "pypi",version = "*"}
 flake8-logging-format = {index = "pypi",version = "*"}
 more-itertools = {index = "pypi",version = "*"}
 pytest = {index = "pypi",version = "*"}
-toml = {index = "pypi",version = "*"}
 
 [packages]
 SQLAlchemy = "==1.4.*"
 Unidecode = "==1.1.*"
 cx_Oracle = "==7.3.*"
 defusedxml = "==0.6.*"
 mysql-connector = "==2.2.*"
```

### Comparing `etlstat-0.9.2/Pipfile.lock` & `etlstat-0.9.3/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9818832082551595%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'01b4f37f7caa693eac52d43b2bc2222959486bffe8842505593f063fece0dd8a'}}",*

 * * "'default'": '{\'charset-normalizer\': {\'markers\': "python_full_version >= \'3.7.0\'"}, '*

 * *              '\'requests\': {\'markers\': "python_version < \'4\' and python_full_version >= '*

 * *              '\'3.7.0\'"}, \'soupsieve\': {\'markers\': "python_full_version >= \'3.7.0\'"}}',*

 * * "'develop'": '{\'isort\': {\'markers\': "python_full_version >= \'3.8.0\'"}, \'packaging\': '*

 * *              […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "6298ceed25c52c005a96ae43209be463250230fa5101fb2f3b01229ac40b928b"
+            "sha256": "01b4f37f7caa693eac52d43b2bc2222959486bffe8842505593f063fece0dd8a"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9.*"
         },
         "sources": [
             {
@@ -106,15 +106,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
         "cx-oracle": {
             "hashes": [
                 "sha256:052cfd1b49ca20265893bad543f2d0755ec5d726f1f9b43b091ccb819a2912ca",
                 "sha256:10379b49b910b475987f771c43a37f7e94f938d4fa7bd8f88d06e7460a5370ae",
                 "sha256:1b519d3435ac1ca8b186e59626351355e24be050b80936a36065cbf5618b9017",
@@ -359,15 +359,15 @@
             "version": "==2023.3"
         },
         "requests": {
             "hashes": [
                 "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
+            "markers": "python_version < '4' and python_full_version >= '3.7.0'",
             "version": "==2.28.2"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
@@ -375,15 +375,15 @@
             "version": "==1.16.0"
         },
         "soupsieve": {
             "hashes": [
                 "sha256:49e5368c2cda80ee7e84da9dbe3e110b70a4575f196efb74e51b94549d921955",
                 "sha256:e28dba9ca6c7c00173e34e4ba57448f0688bb681b7c5e8bf4971daafc093d69a"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==2.4"
         },
         "sqlalchemy": {
             "hashes": [
                 "sha256:03be6f3cb66e69fb3a09b5ea89d77e4bc942f3bf84b207dba84666a26799c166",
                 "sha256:048509d7f3ac27b83ad82fd96a1ab90a34c8e906e4e09c8d677fc531d12c23c5",
                 "sha256:07764b240645627bc3e82596435bd1a1884646bfc0721642d24c26b12f1df194",
@@ -574,15 +574,15 @@
             "version": "==2.0.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
-            "markers": "python_version >= '3.8'",
+            "markers": "python_full_version >= '3.8.0'",
             "version": "==5.12.0"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
                 "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
                 "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
@@ -653,19 +653,19 @@
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "index": "pypi",
             "version": "==9.1.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pbr": {
             "hashes": [
                 "sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b",
                 "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"
             ],
             "markers": "python_version >= '2.6'",
@@ -787,19 +787,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
+                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==13.3.3"
+            "version": "==13.3.4"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
             "markers": "python_version >= '3.6'",
@@ -813,25 +813,17 @@
             "version": "==2.2.0"
         },
         "stevedore": {
             "hashes": [
                 "sha256:2c428d2338976279e8eb2196f7a94910960d9f7ba2f41f3988511e95ca447021",
                 "sha256:bd5a71ff5e5e5f5ea983880e4a1dd1bb47f8feebbb3d95b592398e2f02194771"
             ],
-            "markers": "python_version >= '3.8'",
+            "markers": "python_full_version >= '3.8.0'",
             "version": "==5.0.0"
         },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "index": "pypi",
-            "version": "==0.10.2"
-        },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
```

### Comparing `etlstat-0.9.2/docs/source/conf.py` & `etlstat-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/README.rst` & `etlstat-0.9.3/etlstat/database/README.rst`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/mysql.py` & `etlstat-0.9.3/etlstat/database/mysql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/oracle.py` & `etlstat-0.9.3/etlstat/database/oracle.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/postgresql.py` & `etlstat-0.9.3/etlstat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/22350.px` & `etlstat-0.9.3/etlstat/database/test/22350.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/pmh.csv` & `etlstat-0.9.3/etlstat/database/test/pmh.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/px_01001.csv` & `etlstat-0.9.3/etlstat/database/test/px_01001.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/test_mysql.py` & `etlstat-0.9.3/etlstat/database/test/test_mysql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/test_oracle.py` & `etlstat-0.9.3/etlstat/database/test/test_oracle.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/test_postgresql.py` & `etlstat-0.9.3/etlstat/database/test/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/database/test/test_sqlloader.py` & `etlstat-0.9.3/etlstat/database/test/test_sqlloader.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/extractor.py` & `etlstat-0.9.3/etlstat/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/excel/excel_prueba.xls` & `etlstat-0.9.3/etlstat/extractor/test/data/excel/excel_prueba.xls`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/excel/prueba_excel.xls` & `etlstat-0.9.3/etlstat/extractor/test/data/excel/prueba_excel.xls`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/CONS_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/CONS_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/INFOR_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/INFOR_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/JURID_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/JURID_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/MENOR_COM.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/MENOR_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PERSON_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/PERSON_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/POST_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/POST_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TEC_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TEC_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TFERR_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TFERR_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TMER_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TMER_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/TUI_SER.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/TUI_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv` & `etlstat-0.9.3/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/px/o20012.px` & `etlstat-0.9.3/etlstat/extractor/test/data/px/o20012.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/px/o20013.px` & `etlstat-0.9.3/etlstat/extractor/test/data/px/o20013.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/px_file/27066.px` & `etlstat-0.9.3/etlstat/extractor/test/data/px_file/27066.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/sql/afiliados.sql` & `etlstat-0.9.3/etlstat/extractor/test/data/sql/afiliados.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/sql/contratos.sql` & `etlstat-0.9.3/etlstat/extractor/test/data/sql/contratos.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/sql/ratios.sql` & `etlstat-0.9.3/etlstat/extractor/test/data/sql/ratios.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Comex.kjb` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Comex.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr` & `etlstat-0.9.3/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/extractor/test/test_extractor.py` & `etlstat-0.9.3/etlstat/extractor/test/test_extractor.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/log/logging.py` & `etlstat-0.9.3/etlstat/log/logging.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/log/timing.py` & `etlstat-0.9.3/etlstat/log/timing.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb` & `etlstat-0.9.3/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/text/test/data/jobs/Uso com_elec.csv` & `etlstat-0.9.3/etlstat/text/test/data/jobs/Uso com_elec.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb` & `etlstat-0.9.3/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/text/test/test_utils.py` & `etlstat-0.9.3/etlstat/text/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat/text/utils.py` & `etlstat-0.9.3/etlstat/text/utils.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.2/etlstat.egg-info/PKG-INFO` & `etlstat-0.9.3/etlstat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etlstat
-Version: 0.9.2
+Version: 0.9.3
 Summary: ETL utils for statistical offices data processing
 Home-page: https://github.com/icane/etlstat.git
 Author: Instituto Cántabro de Estadística
 Author-email: icane@cantabria.es
 License: Apache License 2.0
 Keywords: etl,icane,statistics,utils
 Classifier: Development Status :: 4 - Beta
```

### Comparing `etlstat-0.9.2/etlstat.egg-info/SOURCES.txt` & `etlstat-0.9.3/etlstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

