# Comparing `tmp/news-signals-0.1.8.tar.gz` & `tmp/news-signals-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.1.8.tar", last modified: Tue Mar 14 22:43:12 2023, max compression
+gzip compressed data, was "news-signals-0.1.9.tar", last modified: Wed Mar 15 22:09:25 2023, max compression
```

## Comparing `news-signals-0.1.8.tar` & `news-signals-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:12.614008 news-signals-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-14 22:43:02.000000 news-signals-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-14 22:43:02.000000 news-signals-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-14 22:43:12.614008 news-signals-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-14 22:43:02.000000 news-signals-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-14 22:43:02.000000 news-signals-0.1.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:12.610008 news-signals-0.1.8/news_signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-14 22:43:02.000000 news-signals-0.1.8/news_signals/yfinance_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:12.610008 news-signals-0.1.8/news_signals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-14 22:43:12.000000 news-signals-0.1.8/news_signals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-14 22:43:12.000000 news-signals-0.1.8/news_signals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 22:43:12.000000 news-signals-0.1.8/news_signals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-14 22:43:12.000000 news-signals-0.1.8/news_signals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-14 22:43:12.000000 news-signals-0.1.8/news_signals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:12.606008 news-signals-0.1.8/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:12.610008 news-signals-0.1.8/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/elon_musk_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100.small.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:43:12.614008 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/politics_china_australia_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/sample_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-03-14 22:43:02.000000 news-signals-0.1.8/resources/test/tesla_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 22:43:12.614008 news-signals-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-14 22:43:02.000000 news-signals-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.170960 news-signals-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-15 22:09:15.000000 news-signals-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-15 22:09:15.000000 news-signals-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-15 22:09:25.170960 news-signals-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-15 22:09:15.000000 news-signals-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 22:09:15.000000 news-signals-0.1.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.162960 news-signals-0.1.9/news_signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36759 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/yfinance_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.162960 news-signals-0.1.9/news_signals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.158960 news-signals-0.1.9/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.166960 news-signals-0.1.9/resources/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/elon_musk_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100.small.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.170960 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/politics_china_australia_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/sample_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/tesla_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:09:25.170960 news-signals-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-15 22:09:15.000000 news-signals-0.1.9/setup.py
```

### Comparing `news-signals-0.1.8/LICENSE` & `news-signals-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/PKG-INFO` & `news-signals-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
-Check out this [colab notebook](https://drive.google.com/file/d/1iTjjeSt1S5WF0jJItH31DRe2C3IkZvz5/view?usp=sharing) to see some of the things you can do with the news-signals library.
+Check out this [colab notebook](https://drive.google.com/file/d/1zM4J3jFA9v2LDTFKOpaa3EUUGhOdQieo/view?usp=share_link) to see some of the things you can do with the news-signals library.
 
 
 ## Quickstart
 
 
 #### Install news-signals in a new environment
 ```
```

### Comparing `news-signals-0.1.8/README.md` & `news-signals-0.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # News Signals
 
-Check out this [colab notebook](https://drive.google.com/file/d/1iTjjeSt1S5WF0jJItH31DRe2C3IkZvz5/view?usp=sharing) to see some of the things you can do with the news-signals library.
+Check out this [colab notebook](https://drive.google.com/file/d/1zM4J3jFA9v2LDTFKOpaa3EUUGhOdQieo/view?usp=share_link) to see some of the things you can do with the news-signals library.
 
 
 ## Quickstart
 
 
 #### Install news-signals in a new environment
 ```
```

### Comparing `news-signals-0.1.8/news_signals/anomaly_detection.py` & `news-signals-0.1.9/news_signals/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/aql_builder.py` & `news-signals-0.1.9/news_signals/aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/data.py` & `news-signals-0.1.9/news_signals/data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/dataset_transformations.py` & `news-signals-0.1.9/news_signals/dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/exogenous_signals.py` & `news-signals-0.1.9/news_signals/exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/newsapi.py` & `news-signals-0.1.9/news_signals/newsapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,22 @@
     pass
 
 
 class TooManyRequestsError(Exception):
     pass
 
 
+def set_headers(app_id, app_key):
+    """
+    set global headers for newsapi requests
+    """
+    HEADERS['X-AYLIEN-NewsAPI-Application-ID'] = app_id
+    HEADERS['X-AYLIEN-NewsAPI-Application-Key'] = app_key
+
+
 @sleep_and_retry
 @limits(calls=NEWSAPI_CALLS_PER_MINUTE, period=60)
 def make_newsapi_request(
         endpoint,
         params,
         headers,
         trials=10,
```

### Comparing `news-signals-0.1.8/news_signals/plotting.py` & `news-signals-0.1.9/news_signals/plotting.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/representative_story.py` & `news-signals-0.1.9/news_signals/representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/signals.py` & `news-signals-0.1.9/news_signals/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -720,14 +720,25 @@
     def create_aylien_dataset(self, start, end):
         _ = self.__call__(start, end)
         _ = self.sample_stories_in_window(
             start, end, sample_per_tick=True
         )
         return self.to_dict()
 
+    @staticmethod
+    def normalize_aylien_story(story):
+        """
+        stories is a list of dicts, each dict is a story
+        """
+        # this is needed because arrow cannot serialize empty dicts
+        for e in story['entities']:
+            if 'external_ids' in e and len(e['external_ids']) == 0:
+                del e['external_ids']
+        return story
+
     def sample_stories_in_window(self, start, end,
                                  num_stories=20,
                                  sample_per_tick=True,
                                  overwrite_existing=False,
                                  stories_column='stories',
                                  freq='D'):
         """
@@ -755,19 +766,19 @@
                 # the polymorphic .isna check in pandas is weird
                 if type(self.feeds_df.loc[start][stories_column]) is list and not overwrite_existing:
                     logger.info(f'Already have stories for {start} to {end}')
                     continue
                 else:
                     logger.info(f'Getting stories for {start} to {end}')
                     params = self.make_query(start, end)
-                    stories = self.stories_endpoint(params)
+                    stories = [self.normalize_aylien_story(s) for s in self.stories_endpoint(params)]
                     story_bucket_records.append({'timestamp': start, stories_column: stories})
         else:
             params = self.make_query(start, end)
-            stories = self.stories_endpoint(params)
+            stories = [self.normalize_aylien_story(s) for s in self.stories_endpoint(params)]
             records = defaultdict(list)
             for story in stories:
                 ts = self.normalize_timestamp(story['published_at'], freq)
                 records[ts].append(story)
             for ts, stories in records.items():
                 story_bucket_records.append({'timestamp': ts, stories_column: stories})
```

### Comparing `news-signals-0.1.8/news_signals/signals_dataset.py` & `news-signals-0.1.9/news_signals/signals_dataset.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/summarization.py` & `news-signals-0.1.9/news_signals/summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_anomaly_detection.py` & `news-signals-0.1.9/news_signals/test_anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_aql_builder.py` & `news-signals-0.1.9/news_signals/test_aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_data.py` & `news-signals-0.1.9/news_signals/test_data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_dataset_transformations.py` & `news-signals-0.1.9/news_signals/test_dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_exogenous_signals.py` & `news-signals-0.1.9/news_signals/test_exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_newsapi.py` & `news-signals-0.1.9/news_signals/test_newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_representative_story.py` & `news-signals-0.1.9/news_signals/test_representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_signals.py` & `news-signals-0.1.9/news_signals/test_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_signals_dataset.py` & `news-signals-0.1.9/news_signals/test_signals_dataset.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/test_summarization.py` & `news-signals-0.1.9/news_signals/test_summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals/yfinance_timeseries.py` & `news-signals-0.1.9/news_signals/yfinance_timeseries.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/news_signals.egg-info/PKG-INFO` & `news-signals-0.1.9/news_signals.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
-Check out this [colab notebook](https://drive.google.com/file/d/1iTjjeSt1S5WF0jJItH31DRe2C3IkZvz5/view?usp=sharing) to see some of the things you can do with the news-signals library.
+Check out this [colab notebook](https://drive.google.com/file/d/1zM4J3jFA9v2LDTFKOpaa3EUUGhOdQieo/view?usp=share_link) to see some of the things you can do with the news-signals library.
 
 
 ## Quickstart
 
 
 #### Install news-signals in a new environment
 ```
```

### Comparing `news-signals-0.1.8/news_signals.egg-info/SOURCES.txt` & `news-signals-0.1.9/news_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/elon_musk_timeseries.json` & `news-signals-0.1.9/resources/test/elon_musk_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/politics_china_australia_timeseries.json` & `news-signals-0.1.9/resources/test/politics_china_australia_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/sample_stories.json` & `news-signals-0.1.9/resources/test/sample_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/resources/test/tesla_stories.json` & `news-signals-0.1.9/resources/test/tesla_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.8/setup.py` & `news-signals-0.1.9/setup.py`

 * *Files identical despite different names*

