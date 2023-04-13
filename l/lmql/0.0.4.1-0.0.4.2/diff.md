# Comparing `tmp/lmql-0.0.4.1.tar.gz` & `tmp/lmql-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.4.1.tar", last modified: Wed Apr  5 09:32:44 2023, max compression
+gzip compressed data, was "lmql-0.0.4.2.tar", last modified: Thu Apr 13 08:25:21 2023, max compression
```

## Comparing `lmql-0.0.4.1.tar` & `lmql-0.0.4.2.tar`

### file list

```diff
@@ -1,230 +1,239 @@
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.077558 lmql-0.0.4.1/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.974617 lmql-0.0.4.1/.github/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.984576 lmql-0.0.4.1/.github/workflows/
--rw-r--r--   0 luca       (501) staff       (20)     1659 2023-04-03 10:50:48.000000 lmql-0.0.4.1/.github/workflows/lmql-web.yml
--rw-r--r--   0 luca       (501) staff       (20)     2688 2023-04-03 10:50:48.000000 lmql-0.0.4.1/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)    12820 2023-03-09 18:22:48.000000 lmql-0.0.4.1/LICENSE
--rw-r--r--   0 luca       (501) staff       (20)      140 2023-04-03 11:22:43.000000 lmql-0.0.4.1/MANIFEST.in
--rw-r--r--   0 luca       (501) staff       (20)     4646 2023-04-05 09:32:44.077823 lmql-0.0.4.1/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)     4214 2023-04-03 17:00:59.000000 lmql-0.0.4.1/README.md
--rw-r--r--   0 luca       (501) staff       (20)       75 2023-03-27 17:50:33.000000 lmql-0.0.4.1/TODO.md
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.985773 lmql-0.0.4.1/docs/
--rw-r--r--   0 luca       (501) staff       (20)      638 2023-03-30 17:12:07.000000 lmql-0.0.4.1/docs/Makefile
--rw-r--r--   0 luca       (501) staff       (20)      444 2023-03-10 12:30:21.000000 lmql-0.0.4.1/docs/RELEASE.md
--rw-r--r--   0 luca       (501) staff       (20)      799 2023-03-30 17:12:07.000000 lmql-0.0.4.1/docs/make.bat
--rw-r--r--   0 luca       (501) staff       (20)       81 2023-04-03 10:50:48.000000 lmql-0.0.4.1/docs/requirements.txt
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.987829 lmql-0.0.4.1/docs/source/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.988356 lmql-0.0.4.1/docs/source/_ext/
--rw-r--r--   0 luca       (501) staff       (20)     3182 2023-04-03 10:50:48.000000 lmql-0.0.4.1/docs/source/_ext/lmql_snippets.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.976296 lmql-0.0.4.1/docs/source/_static/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.988754 lmql-0.0.4.1/docs/source/_static/css/
--rw-r--r--   0 luca       (501) staff       (20)     3966 2023-04-05 07:53:26.000000 lmql-0.0.4.1/docs/source/_static/css/lmql-docs.css
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.989071 lmql-0.0.4.1/docs/source/_static/images/
--rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-03 13:53:17.000000 lmql-0.0.4.1/docs/source/_static/images/lmql.svg
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.989438 lmql-0.0.4.1/docs/source/_static/js/
--rw-r--r--   0 luca       (501) staff       (20)     2191 2023-04-03 14:00:24.000000 lmql-0.0.4.1/docs/source/_static/js/lmql-playground.js
--rw-r--r--   0 luca       (501) staff       (20)     1138 2023-04-05 08:13:04.000000 lmql-0.0.4.1/docs/source/conf.py
--rw-r--r--   0 luca       (501) staff       (20)     1293 2023-03-30 17:12:07.000000 lmql-0.0.4.1/docs/source/dev-setup.md
--rw-r--r--   0 luca       (501) staff       (20)     2709 2023-04-05 09:31:26.000000 lmql-0.0.4.1/docs/source/index.rst
--rw-r--r--   0 luca       (501) staff       (20)     2484 2023-04-05 09:27:50.000000 lmql-0.0.4.1/docs/source/installation.md
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.991762 lmql-0.0.4.1/docs/source/language/
--rw-r--r--   0 luca       (501) staff       (20)     7397 2023-04-05 08:00:31.000000 lmql-0.0.4.1/docs/source/language/constraints.md
--rw-r--r--   0 luca       (501) staff       (20)     4065 2023-04-03 17:02:08.000000 lmql-0.0.4.1/docs/source/language/decoders.md
--rw-r--r--   0 luca       (501) staff       (20)     7639 2023-04-03 16:17:34.000000 lmql-0.0.4.1/docs/source/language/functions.md
--rw-r--r--   0 luca       (501) staff       (20)     6520 2023-04-05 09:26:39.000000 lmql-0.0.4.1/docs/source/language/models.md
--rw-r--r--   0 luca       (501) staff       (20)     8444 2023-04-05 08:44:12.000000 lmql-0.0.4.1/docs/source/language/overview.md
--rw-r--r--   0 luca       (501) staff       (20)     3601 2023-04-03 16:56:38.000000 lmql-0.0.4.1/docs/source/language/scripted_prompts.md
--rw-r--r--   0 luca       (501) staff       (20)     3675 2023-03-30 17:12:07.000000 lmql-0.0.4.1/docs/source/lmql.svg
--rw-r--r--   0 luca       (501) staff       (20)    28444 2023-03-30 17:12:07.000000 lmql-0.0.4.1/docs/source/logo.png
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.994209 lmql-0.0.4.1/docs/source/python/
--rw-r--r--   0 luca       (501) staff       (20)       11 2023-04-03 10:50:48.000000 lmql-0.0.4.1/docs/source/python/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)    10629 2023-04-04 16:29:36.000000 lmql-0.0.4.1/docs/source/python/langchain.ipynb
--rw-r--r--   0 luca       (501) staff       (20)    75148 2023-04-03 10:50:48.000000 lmql-0.0.4.1/docs/source/python/lmql.txt
--rw-r--r--   0 luca       (501) staff       (20)     7874 2023-04-05 09:25:54.000000 lmql-0.0.4.1/docs/source/python/python.ipynb
--rw-r--r--   0 luca       (501) staff       (20)     3135 2023-04-05 09:27:31.000000 lmql-0.0.4.1/docs/source/quickstart.md
--rw-r--r--   0 luca       (501) staff       (20)      257 2023-04-03 11:56:36.000000 lmql-0.0.4.1/docs/todo.md
--rw-r--r--   0 luca       (501) staff       (20)      137 2023-03-10 10:04:42.000000 lmql-0.0.4.1/pyproject.toml
--rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-03 11:04:04.000000 lmql-0.0.4.1/requirements.txt
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.995907 lmql-0.0.4.1/scripts/
--rw-r--r--   0 luca       (501) staff       (20)      295 2023-03-29 10:02:20.000000 lmql-0.0.4.1/scripts/activate-dev.sh
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.996821 lmql-0.0.4.1/scripts/conda/
--rw-r--r--   0 luca       (501) staff       (20)      209 2023-03-10 09:32:52.000000 lmql-0.0.4.1/scripts/conda/requirements-no-gpu.yml
--rw-r--r--   0 luca       (501) staff       (20)      343 2023-03-10 09:32:55.000000 lmql-0.0.4.1/scripts/conda/requirements.yml
--rw-r--r--   0 luca       (501) staff       (20)      486 2023-03-09 18:28:10.000000 lmql-0.0.4.1/scripts/pypi-release.sh
--rw-r--r--   0 luca       (501) staff       (20)      817 2023-03-09 18:06:11.000000 lmql-0.0.4.1/scripts/wheel.sh
--rw-r--r--   0 luca       (501) staff       (20)      828 2023-04-05 09:32:44.078594 lmql-0.0.4.1/setup.cfg
--rw-r--r--   0 luca       (501) staff       (20)       37 2023-03-09 15:51:24.000000 lmql-0.0.4.1/setup.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.978362 lmql-0.0.4.1/src/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:43.999808 lmql-0.0.4.1/src/lmql/
--rw-r--r--   0 luca       (501) staff       (20)     4828 2023-04-05 09:15:14.000000 lmql-0.0.4.1/src/lmql/__init__.py
--rwxr-xr-x   0 luca       (501) staff       (20)     7134 2023-03-27 18:15:10.000000 lmql-0.0.4.1/src/lmql/cli.py
--rw-r--r--   0 luca       (501) staff       (20)     1577 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/demo.py
--rw-r--r--   0 luca       (501) staff       (20)      347 2023-03-12 14:41:02.000000 lmql-0.0.4.1/src/lmql/hello-chat.lmq_compiled.py
--rw-r--r--   0 luca       (501) staff       (20)     1229 2023-03-20 20:26:18.000000 lmql-0.0.4.1/src/lmql/http.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.006480 lmql-0.0.4.1/src/lmql/language/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 16:00:33.000000 lmql-0.0.4.1/src/lmql/language/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    17867 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/language/compiler.py
--rw-r--r--   0 luca       (501) staff       (20)    10194 2023-03-27 14:45:55.000000 lmql-0.0.4.1/src/lmql/language/fragment_parser.py
--rw-r--r--   0 luca       (501) staff       (20)      979 2023-03-27 09:20:54.000000 lmql-0.0.4.1/src/lmql/language/qstrings.py
--rw-r--r--   0 luca       (501) staff       (20)     1804 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/language/validator.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.008651 lmql-0.0.4.1/src/lmql/lib/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 16:00:38.000000 lmql-0.0.4.1/src/lmql/lib/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)      775 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/lib/errors.py
--rw-r--r--   0 luca       (501) staff       (20)      810 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/lib/expr_jitter.py
--rw-r--r--   0 luca       (501) staff       (20)     1998 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/lib/scope.py
--rw-r--r--   0 luca       (501) staff       (20)      495 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/lib/state.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.011763 lmql-0.0.4.1/src/lmql/model/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 16:00:56.000000 lmql-0.0.4.1/src/lmql/model/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    24608 2023-04-03 15:28:28.000000 lmql-0.0.4.1/src/lmql/model/async_generation_utils.py
--rw-r--r--   0 luca       (501) staff       (20)    12601 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/model/client.py
--rw-r--r--   0 luca       (501) staff       (20)    17716 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/model/hf_beam_search.py
--rw-r--r--   0 luca       (501) staff       (20)     1299 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/model/local_client.py
--rw-r--r--   0 luca       (501) staff       (20)    17134 2023-03-09 17:17:19.000000 lmql-0.0.4.1/src/lmql/model/serve.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.013871 lmql-0.0.4.1/src/lmql/ops/
--rw-r--r--   0 luca       (501) staff       (20)       93 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ops/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     7565 2023-03-09 15:40:13.000000 lmql-0.0.4.1/src/lmql/ops/follow_map.py
--rw-r--r--   0 luca       (501) staff       (20)    32970 2023-04-04 22:16:55.000000 lmql-0.0.4.1/src/lmql/ops/ops.py
--rw-r--r--   0 luca       (501) staff       (20)    15564 2023-03-28 15:46:40.000000 lmql-0.0.4.1/src/lmql/ops/token_set.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.023398 lmql-0.0.4.1/src/lmql/runtime/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     2554 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/backtracker.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.024669 lmql-0.0.4.1/src/lmql/runtime/bopenai/
--rw-r--r--   0 luca       (501) staff       (20)     1863 2023-03-20 20:26:18.000000 lmql-0.0.4.1/src/lmql/runtime/bopenai/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    25567 2023-04-05 09:31:49.000000 lmql-0.0.4.1/src/lmql/runtime/bopenai/batched_openai.py
--rw-r--r--   0 luca       (501) staff       (20)    17000 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/runtime/bopenai/openai_api.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.027921 lmql-0.0.4.1/src/lmql/runtime/dclib/
--rw-r--r--   0 luca       (501) staff       (20)      467 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    18632 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_array.py
--rw-r--r--   0 luca       (501) staff       (20)      538 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_global.py
--rw-r--r--   0 luca       (501) staff       (20)    23530 2023-04-03 15:32:26.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_model.py
--rw-r--r--   0 luca       (501) staff       (20)    27080 2023-03-28 15:30:40.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_seq.py
--rw-r--r--   0 luca       (501) staff       (20)    20610 2023-03-28 13:44:47.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/decoders.py
--rw-r--r--   0 luca       (501) staff       (20)    10162 2023-03-20 20:26:18.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/lmql_adapter.py
--rw-r--r--   0 luca       (501) staff       (20)     4138 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/dclib/trie_cache.py
--rw-r--r--   0 luca       (501) staff       (20)     3037 2023-03-27 21:51:16.000000 lmql-0.0.4.1/src/lmql/runtime/decoder_head.py
--rw-r--r--   0 luca       (501) staff       (20)     5056 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/hf_integration.py
--rw-r--r--   0 luca       (501) staff       (20)      250 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/interrupt.py
--rw-r--r--   0 luca       (501) staff       (20)     1084 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/runtime/langchain.py
--rw-r--r--   0 luca       (501) staff       (20)     5797 2023-04-03 14:05:19.000000 lmql-0.0.4.1/src/lmql/runtime/lmql_runtime.py
--rw-r--r--   0 luca       (501) staff       (20)     1186 2023-03-27 14:45:55.000000 lmql-0.0.4.1/src/lmql/runtime/maiohttp.py
--rw-r--r--   0 luca       (501) staff       (20)      732 2023-03-27 15:42:18.000000 lmql-0.0.4.1/src/lmql/runtime/model_registry.py
--rw-r--r--   0 luca       (501) staff       (20)     8564 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/multi_head_interpretation.py
--rw-r--r--   0 luca       (501) staff       (20)    44472 2023-03-27 22:16:55.000000 lmql-0.0.4.1/src/lmql/runtime/openai_integration.py
--rw-r--r--   0 luca       (501) staff       (20)     1979 2023-04-03 11:35:58.000000 lmql-0.0.4.1/src/lmql/runtime/openai_secret.py
--rw-r--r--   0 luca       (501) staff       (20)     2021 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/runtime/output_writer.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.028771 lmql-0.0.4.1/src/lmql/runtime/postprocessing/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/postprocessing/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     6163 2023-03-20 20:26:18.000000 lmql-0.0.4.1/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-r--r--   0 luca       (501) staff       (20)      203 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/postprocessing/group_by.py
--rw-r--r--   0 luca       (501) staff       (20)     1543 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/program_state.py
--rw-r--r--   0 luca       (501) staff       (20)    36840 2023-04-03 16:09:14.000000 lmql-0.0.4.1/src/lmql/runtime/prompt_interpreter.py
--rw-r--r--   0 luca       (501) staff       (20)     8367 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/rewriter.py
--rw-r--r--   0 luca       (501) staff       (20)       86 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/runtime.py
--rw-r--r--   0 luca       (501) staff       (20)     1123 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/runtime/stats.py
--rw-r--r--   0 luca       (501) staff       (20)     2150 2023-03-27 14:45:55.000000 lmql-0.0.4.1/src/lmql/runtime/tok.ipynb
--rw-r--r--   0 luca       (501) staff       (20)     7103 2023-03-28 13:45:47.000000 lmql-0.0.4.1/src/lmql/runtime/tokenizer.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.031640 lmql-0.0.4.1/src/lmql/tests/
--rw-r--r--   0 luca       (501) staff       (20)     5015 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/expr_test_utils.py
--rw-r--r--   0 luca       (501) staff       (20)     1611 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/mask_product_test.py
--rw-r--r--   0 luca       (501) staff       (20)     2789 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/monotonicity.py
--rw-r--r--   0 luca       (501) staff       (20)      546 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/one_of_tests.py
--rw-r--r--   0 luca       (501) staff       (20)      758 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/sentences_op.py
--rw-r--r--   0 luca       (501) staff       (20)      984 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/starts_with_op_test.py
--rw-r--r--   0 luca       (501) staff       (20)     1236 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/stops_at.py
--rw-r--r--   0 luca       (501) staff       (20)      537 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/str_in_str_tests.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.031929 lmql-0.0.4.1/src/lmql/tests/system/
--rw-r--r--   0 luca       (501) staff       (20)     3402 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/system/basic_use_cases.py
--rw-r--r--   0 luca       (501) staff       (20)     4738 2023-04-04 17:50:58.000000 lmql-0.0.4.1/src/lmql/tests/test_multi_head.py
--rw-r--r--   0 luca       (501) staff       (20)     3036 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/tests/token_set_test.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.032494 lmql-0.0.4.1/src/lmql/ui/
--rw-r--r--   0 luca       (501) staff       (20)       27 2023-03-09 17:52:07.000000 lmql-0.0.4.1/src/lmql/ui/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 16:01:09.000000 lmql-0.0.4.1/src/lmql/ui/__init__.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.034247 lmql-0.0.4.1/src/lmql/ui/live/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 16:01:19.000000 lmql-0.0.4.1/src/lmql/ui/live/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     6747 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/ui/live/live.js
--rw-r--r--   0 luca       (501) staff       (20)     3299 2023-03-27 22:05:27.000000 lmql-0.0.4.1/src/lmql/ui/live/live.py
--rw-r--r--   0 luca       (501) staff       (20)     3885 2023-03-27 22:14:32.000000 lmql-0.0.4.1/src/lmql/ui/live/livelib.py
--rw-r--r--   0 luca       (501) staff       (20)      349 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/live/package.json
--rw-r--r--   0 luca       (501) staff       (20)    33701 2023-03-09 17:22:13.000000 lmql-0.0.4.1/src/lmql/ui/live/yarn.lock
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.038242 lmql-0.0.4.1/src/lmql/ui/playground/
--rw-r--r--   0 luca       (501) staff       (20)       31 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/.dockerignore
--rw-r--r--   0 luca       (501) staff       (20)       34 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/.env
--rw-r--r--   0 luca       (501) staff       (20)      310 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)      354 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/Dockerfile
--rw-r--r--   0 luca       (501) staff       (20)     3359 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/README.md
--rw-r--r--   0 luca       (501) staff       (20)     1327 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/ui/playground/package.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.041205 lmql-0.0.4.1/src/lmql/ui/playground/public/
--rw-r--r--   0 luca       (501) staff       (20)       90 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/_headers
--rw-r--r--   0 luca       (501) staff       (20)     3870 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/favicon.ico
--rw-r--r--   0 luca       (501) staff       (20)     1678 2023-03-30 17:43:02.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/index.html
--rw-r--r--   0 luca       (501) staff       (20)     2817 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/lmql.svg
--rw-r--r--   0 luca       (501) staff       (20)      306 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/manifest.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.056046 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/
--rw-r--r--   0 luca       (501) staff       (20)  1227728 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/calc.json
--rw-r--r--   0 luca       (501) staff       (20)   295285 2023-03-27 14:56:41.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/chat.json
--rw-r--r--   0 luca       (501) staff       (20)   160153 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/cot.json
--rw-r--r--   0 luca       (501) staff       (20)    81768 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-r--r--   0 luca       (501) staff       (20)     5221 2023-04-03 09:29:58.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/hello.json
--rw-r--r--   0 luca       (501) staff       (20)    89531 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/joke.json
--rw-r--r--   0 luca       (501) staff       (20)  1710847 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/kv.json
--rw-r--r--   0 luca       (501) staff       (20)    52748 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/list.json
--rw-r--r--   0 luca       (501) staff       (20)   628184 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/meta.json
--rw-r--r--   0 luca       (501) staff       (20)   264768 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/translation.json
--rw-r--r--   0 luca       (501) staff       (20)   215050 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-r--r--   0 luca       (501) staff       (20)       67 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/public/robots.txt
--rw-r--r--   0 luca       (501) staff       (20)       62 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/ref.py
--rw-r--r--   0 luca       (501) staff       (20)       80 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/run-in-docker.sh
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.069507 lmql-0.0.4.1/src/lmql/ui/playground/src/
--rw-r--r--   0 luca       (501) staff       (20)    66653 2023-04-04 17:42:00.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/App.jsx
--rw-r--r--   0 luca       (501) staff       (20)      246 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/App.test.js
--rw-r--r--   0 luca       (501) staff       (20)      807 2023-03-10 16:07:08.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/Configuration.js
--rw-r--r--   0 luca       (501) staff       (20)     1174 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/DataListView.js
--rw-r--r--   0 luca       (501) staff       (20)    20059 2023-03-28 16:19:07.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/DecoderGraph.js
--rw-r--r--   0 luca       (501) staff       (20)      329 2023-03-10 13:03:47.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/DecodingTree.js
--rw-r--r--   0 luca       (501) staff       (20)       89 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/Embed.jsx
--rw-r--r--   0 luca       (501) staff       (20)     9568 2023-04-04 17:41:04.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/Explore.jsx
--rw-r--r--   0 luca       (501) staff       (20)      675 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/SharedState.js
--rw-r--r--   0 luca       (501) staff       (20)     3208 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/State.js
--rw-r--r--   0 luca       (501) staff       (20)     5738 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-r--r--   0 luca       (501) staff       (20)     9360 2023-03-27 14:45:55.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/browser_process.js
--rw-r--r--   0 luca       (501) staff       (20)     1163 2023-03-10 12:41:51.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/build_info.js
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.070950 lmql-0.0.4.1/src/lmql/ui/playground/src/editor/
--rw-r--r--   0 luca       (501) staff       (20)     8673 2023-03-10 13:16:28.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-r--r--   0 luca       (501) staff       (20)     4758 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/editor/theme.json
--rw-r--r--   0 luca       (501) staff       (20)      889 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/explore.svg
--rw-r--r--   0 luca       (501) staff       (20)     1345 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/graph-layout.css
--rw-r--r--   0 luca       (501) staff       (20)     1698 2023-03-27 15:55:28.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/index.css
--rw-r--r--   0 luca       (501) staff       (20)      489 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/index.js
--rw-r--r--   0 luca       (501) staff       (20)     2632 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/logo.svg
--rw-r--r--   0 luca       (501) staff       (20)     8078 2023-03-27 16:48:32.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/queries.js
--rw-r--r--   0 luca       (501) staff       (20)     5990 2023-03-27 14:45:55.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/remote_process.js
--rw-r--r--   0 luca       (501) staff       (20)      362 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/reportWebVitals.js
--rw-r--r--   0 luca       (501) staff       (20)      241 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/setupTests.js
--rw-r--r--   0 luca       (501) staff       (20)     3466 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/spinner.svg
--rw-r--r--   0 luca       (501) staff       (20)     2949 2023-03-27 14:45:55.000000 lmql-0.0.4.1/src/lmql/ui/playground/src/tagged-model-result.js
--rw-r--r--   0 luca       (501) staff       (20)   449905 2023-04-03 10:50:48.000000 lmql-0.0.4.1/src/lmql/ui/playground/yarn.lock
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.074167 lmql-0.0.4.1/src/lmql/ui/vscode/
--rw-r--r--   0 luca       (501) staff       (20)       76 2023-03-29 07:50:18.000000 lmql-0.0.4.1/src/lmql/ui/vscode/.gitattributes
--rw-r--r--   0 luca       (501) staff       (20)       19 2023-03-29 07:50:18.000000 lmql-0.0.4.1/src/lmql/ui/vscode/.gitignore
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.074620 lmql-0.0.4.1/src/lmql/ui/vscode/.vscode/
--rw-r--r--   0 luca       (501) staff       (20)      540 2023-03-29 07:50:18.000000 lmql-0.0.4.1/src/lmql/ui/vscode/.vscode/launch.json
--rw-r--r--   0 luca       (501) staff       (20)       66 2023-03-29 07:50:18.000000 lmql-0.0.4.1/src/lmql/ui/vscode/.vscodeignore
--rw-r--r--   0 luca       (501) staff       (20)    12820 2023-03-09 18:22:48.000000 lmql-0.0.4.1/src/lmql/ui/vscode/LICENSE
--rw-r--r--   0 luca       (501) staff       (20)      959 2023-03-29 10:38:29.000000 lmql-0.0.4.1/src/lmql/ui/vscode/language-configuration.json
--rw-r--r--   0 luca       (501) staff       (20)     1073 2023-03-29 10:52:00.000000 lmql-0.0.4.1/src/lmql/ui/vscode/package.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.075785 lmql-0.0.4.1/src/lmql/ui/vscode/syntaxes/
--rw-r--r--   0 luca       (501) staff       (20)      510 2023-03-29 10:40:52.000000 lmql-0.0.4.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-r--r--   0 luca       (501) staff       (20)      642 2023-03-29 09:54:24.000000 lmql-0.0.4.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-r--r--   0 luca       (501) staff       (20)      853 2023-03-29 09:53:39.000000 lmql-0.0.4.1/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.077210 lmql-0.0.4.1/src/lmql/utils/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-03-09 16:01:26.000000 lmql-0.0.4.1/src/lmql/utils/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     5269 2023-03-09 15:38:14.000000 lmql-0.0.4.1/src/lmql/utils/graph.py
--rw-r--r--   0 luca       (501) staff       (20)     1474 2023-03-11 11:04:22.000000 lmql-0.0.4.1/src/lmql/utils/nputil.py
--rw-r--r--   0 luca       (501) staff       (20)      115 2023-04-05 09:32:36.000000 lmql-0.0.4.1/src/lmql/version.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-05 09:32:44.002919 lmql-0.0.4.1/src/lmql.egg-info/
--rw-r--r--   0 luca       (501) staff       (20)     4646 2023-04-05 09:32:43.000000 lmql-0.0.4.1/src/lmql.egg-info/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)     6335 2023-04-05 09:32:43.000000 lmql-0.0.4.1/src/lmql.egg-info/SOURCES.txt
--rw-r--r--   0 luca       (501) staff       (20)        1 2023-04-05 09:32:43.000000 lmql-0.0.4.1/src/lmql.egg-info/dependency_links.txt
--rw-r--r--   0 luca       (501) staff       (20)       39 2023-04-05 09:32:43.000000 lmql-0.0.4.1/src/lmql.egg-info/entry_points.txt
--rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-05 09:32:43.000000 lmql-0.0.4.1/src/lmql.egg-info/requires.txt
--rw-r--r--   0 luca       (501) staff       (20)        5 2023-04-05 09:32:43.000000 lmql-0.0.4.1/src/lmql.egg-info/top_level.txt
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.234514 lmql-0.0.4.2/
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.079098 lmql-0.0.4.2/.github/
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.094689 lmql-0.0.4.2/.github/workflows/
+-rw-r--r--   0 luca       (501) staff       (20)     1659 2023-04-09 19:01:32.000000 lmql-0.0.4.2/.github/workflows/lmql-web.yml
+-rw-r--r--   0 luca       (501) staff       (20)     2701 2023-04-13 08:24:53.000000 lmql-0.0.4.2/.gitignore
+-rw-r--r--   0 luca       (501) staff       (20)    12820 2023-04-09 19:01:32.000000 lmql-0.0.4.2/LICENSE
+-rw-r--r--   0 luca       (501) staff       (20)      140 2023-04-09 19:01:32.000000 lmql-0.0.4.2/MANIFEST.in
+-rw-r--r--   0 luca       (501) staff       (20)     4646 2023-04-13 08:25:21.234813 lmql-0.0.4.2/PKG-INFO
+-rw-r--r--   0 luca       (501) staff       (20)     4214 2023-04-09 19:01:32.000000 lmql-0.0.4.2/README.md
+-rw-r--r--   0 luca       (501) staff       (20)       75 2023-04-09 19:01:32.000000 lmql-0.0.4.2/TODO.md
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.097084 lmql-0.0.4.2/docs/
+-rw-r--r--   0 luca       (501) staff       (20)      638 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/Makefile
+-rw-r--r--   0 luca       (501) staff       (20)      444 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/RELEASE.md
+-rw-r--r--   0 luca       (501) staff       (20)      799 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/make.bat
+-rw-r--r--   0 luca       (501) staff       (20)       81 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/requirements.txt
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.101126 lmql-0.0.4.2/docs/source/
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.101675 lmql-0.0.4.2/docs/source/_ext/
+-rw-r--r--   0 luca       (501) staff       (20)     5526 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/_ext/lmql_snippets.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.080299 lmql-0.0.4.2/docs/source/_static/
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.102258 lmql-0.0.4.2/docs/source/_static/css/
+-rw-r--r--   0 luca       (501) staff       (20)     5777 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/_static/css/lmql-docs.css
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.102849 lmql-0.0.4.2/docs/source/_static/images/
+-rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/_static/images/lmql.svg
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.103384 lmql-0.0.4.2/docs/source/_static/js/
+-rw-r--r--   0 luca       (501) staff       (20)     2191 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/_static/js/lmql-playground.js
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.103920 lmql-0.0.4.2/docs/source/_templates/
+-rw-r--r--   0 luca       (501) staff       (20)      292 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/_templates/layout.html
+-rw-r--r--   0 luca       (501) staff       (20)     1167 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/conf.py
+-rw-r--r--   0 luca       (501) staff       (20)     1293 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/dev-setup.md
+-rw-r--r--   0 luca       (501) staff       (20)     2709 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/index.rst
+-rw-r--r--   0 luca       (501) staff       (20)     2484 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/installation.md
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.107305 lmql-0.0.4.2/docs/source/language/
+-rw-r--r--   0 luca       (501) staff       (20)     7435 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/constraints.md
+-rw-r--r--   0 luca       (501) staff       (20)     4067 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/decoders.md
+-rw-r--r--   0 luca       (501) staff       (20)     7850 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/functions.md
+-rw-r--r--   0 luca       (501) staff       (20)     6566 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/models.md
+-rw-r--r--   0 luca       (501) staff       (20)     8511 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/overview.md
+-rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/scripted_prompts.md
+-rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/lmql.svg
+-rw-r--r--   0 luca       (501) staff       (20)    28444 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/logo.png
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.109818 lmql-0.0.4.2/docs/source/python/
+-rw-r--r--   0 luca       (501) staff       (20)       11 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/python/.gitignore
+-rw-r--r--   0 luca       (501) staff       (20)    10629 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/python/langchain.ipynb
+-rw-r--r--   0 luca       (501) staff       (20)    75148 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/python/lmql.txt
+-rw-r--r--   0 luca       (501) staff       (20)     8583 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/python/python.ipynb
+-rw-r--r--   0 luca       (501) staff       (20)     3135 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/quickstart.md
+-rw-r--r--   0 luca       (501) staff       (20)      257 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/todo.md
+-rw-r--r--   0 luca       (501) staff       (20)      137 2023-04-09 19:01:32.000000 lmql-0.0.4.2/pyproject.toml
+-rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-09 19:01:32.000000 lmql-0.0.4.2/requirements.txt
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.111757 lmql-0.0.4.2/scripts/
+-rw-r--r--   0 luca       (501) staff       (20)      295 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/activate-dev.sh
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.113294 lmql-0.0.4.2/scripts/conda/
+-rw-r--r--   0 luca       (501) staff       (20)      209 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/conda/requirements-no-gpu.yml
+-rw-r--r--   0 luca       (501) staff       (20)      343 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/conda/requirements.yml
+-rw-r--r--   0 luca       (501) staff       (20)      486 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/pypi-release.sh
+-rw-r--r--   0 luca       (501) staff       (20)      817 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/wheel.sh
+-rw-r--r--   0 luca       (501) staff       (20)      828 2023-04-13 08:25:21.235930 lmql-0.0.4.2/setup.cfg
+-rw-r--r--   0 luca       (501) staff       (20)       37 2023-04-09 19:01:32.000000 lmql-0.0.4.2/setup.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.081673 lmql-0.0.4.2/src/
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.116199 lmql-0.0.4.2/src/lmql/
+-rw-r--r--   0 luca       (501) staff       (20)     4985 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/__init__.py
+-rwxr-xr-x   0 luca       (501) staff       (20)     7337 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/cli.py
+-rw-r--r--   0 luca       (501) staff       (20)     1577 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/demo.py
+-rw-r--r--   0 luca       (501) staff       (20)     1229 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/http.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.126283 lmql-0.0.4.2/src/lmql/language/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)    18943 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/language/compiler.py
+-rw-r--r--   0 luca       (501) staff       (20)    10194 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/fragment_parser.py
+-rw-r--r--   0 luca       (501) staff       (20)      979 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/qstrings.py
+-rw-r--r--   0 luca       (501) staff       (20)     1804 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/validator.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.129484 lmql-0.0.4.2/src/lmql/lib/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)      775 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/errors.py
+-rw-r--r--   0 luca       (501) staff       (20)      810 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/expr_jitter.py
+-rw-r--r--   0 luca       (501) staff       (20)     1998 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/scope.py
+-rw-r--r--   0 luca       (501) staff       (20)      495 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/state.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.134975 lmql-0.0.4.2/src/lmql/model/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)    24608 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/async_generation_utils.py
+-rw-r--r--   0 luca       (501) staff       (20)    12601 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/client.py
+-rw-r--r--   0 luca       (501) staff       (20)    17716 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/hf_beam_search.py
+-rw-r--r--   0 luca       (501) staff       (20)     1299 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/local_client.py
+-rw-r--r--   0 luca       (501) staff       (20)    17134 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/serve.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.137285 lmql-0.0.4.2/src/lmql/ops/
+-rw-r--r--   0 luca       (501) staff       (20)       93 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ops/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     7565 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ops/follow_map.py
+-rw-r--r--   0 luca       (501) staff       (20)    32961 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ops/ops.py
+-rw-r--r--   0 luca       (501) staff       (20)    15564 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ops/token_set.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.148146 lmql-0.0.4.2/src/lmql/runtime/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     2554 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/backtracker.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.150270 lmql-0.0.4.2/src/lmql/runtime/bopenai/
+-rw-r--r--   0 luca       (501) staff       (20)     1863 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/bopenai/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)    25702 2023-04-13 08:25:04.000000 lmql-0.0.4.2/src/lmql/runtime/bopenai/batched_openai.py
+-rw-r--r--   0 luca       (501) staff       (20)    17000 2023-04-09 20:15:19.000000 lmql-0.0.4.2/src/lmql/runtime/bopenai/openai_api.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.154659 lmql-0.0.4.2/src/lmql/runtime/dclib/
+-rw-r--r--   0 luca       (501) staff       (20)      467 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)    18632 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_array.py
+-rw-r--r--   0 luca       (501) staff       (20)      538 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_global.py
+-rw-r--r--   0 luca       (501) staff       (20)    23530 2023-04-10 21:23:08.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_model.py
+-rw-r--r--   0 luca       (501) staff       (20)    28796 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_seq.py
+-rw-r--r--   0 luca       (501) staff       (20)    20610 2023-04-10 21:23:36.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/decoders.py
+-rw-r--r--   0 luca       (501) staff       (20)    10602 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/lmql_adapter.py
+-rw-r--r--   0 luca       (501) staff       (20)     4138 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/trie_cache.py
+-rw-r--r--   0 luca       (501) staff       (20)     3037 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/decoder_head.py
+-rw-r--r--   0 luca       (501) staff       (20)     5056 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/hf_integration.py
+-rw-r--r--   0 luca       (501) staff       (20)      250 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/interrupt.py
+-rw-r--r--   0 luca       (501) staff       (20)     1084 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/langchain.py
+-rw-r--r--   0 luca       (501) staff       (20)     5806 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/lmql_runtime.py
+-rw-r--r--   0 luca       (501) staff       (20)     1186 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/maiohttp.py
+-rw-r--r--   0 luca       (501) staff       (20)      732 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/model_registry.py
+-rw-r--r--   0 luca       (501) staff       (20)     8564 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/multi_head_interpretation.py
+-rw-r--r--   0 luca       (501) staff       (20)    44472 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/openai_integration.py
+-rw-r--r--   0 luca       (501) staff       (20)     1979 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/openai_secret.py
+-rw-r--r--   0 luca       (501) staff       (20)     2086 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/output_writer.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.156890 lmql-0.0.4.2/src/lmql/runtime/postprocessing/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/postprocessing/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     6163 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-r--r--   0 luca       (501) staff       (20)      203 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/postprocessing/group_by.py
+-rw-r--r--   0 luca       (501) staff       (20)     1543 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/program_state.py
+-rw-r--r--   0 luca       (501) staff       (20)    36840 2023-04-13 08:04:33.000000 lmql-0.0.4.2/src/lmql/runtime/prompt_interpreter.py
+-rw-r--r--   0 luca       (501) staff       (20)     8367 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/rewriter.py
+-rw-r--r--   0 luca       (501) staff       (20)       86 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/runtime.py
+-rw-r--r--   0 luca       (501) staff       (20)     1123 2023-04-10 20:34:48.000000 lmql-0.0.4.2/src/lmql/runtime/stats.py
+-rw-r--r--   0 luca       (501) staff       (20)     2150 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/tok.ipynb
+-rw-r--r--   0 luca       (501) staff       (20)     8312 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/tokenizer.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.164302 lmql-0.0.4.2/src/lmql/tests/
+-rw-r--r--   0 luca       (501) staff       (20)     5015 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/expr_test_utils.py
+-rw-r--r--   0 luca       (501) staff       (20)     1611 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/mask_product_test.py
+-rw-r--r--   0 luca       (501) staff       (20)     2789 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/monotonicity.py
+-rw-r--r--   0 luca       (501) staff       (20)      546 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/one_of_tests.py
+-rw-r--r--   0 luca       (501) staff       (20)      758 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/sentences_op.py
+-rw-r--r--   0 luca       (501) staff       (20)      984 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/starts_with_op_test.py
+-rw-r--r--   0 luca       (501) staff       (20)     1236 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/stops_at.py
+-rw-r--r--   0 luca       (501) staff       (20)      537 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/str_in_str_tests.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.165080 lmql-0.0.4.2/src/lmql/tests/system/
+-rw-r--r--   0 luca       (501) staff       (20)     3402 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/system/basic_use_cases.py
+-rw-r--r--   0 luca       (501) staff       (20)     4738 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/test_multi_head.py
+-rw-r--r--   0 luca       (501) staff       (20)     3036 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/token_set_test.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.167874 lmql-0.0.4.2/src/lmql/ui/
+-rw-r--r--   0 luca       (501) staff       (20)     6148 2023-04-10 11:59:45.000000 lmql-0.0.4.2/src/lmql/ui/.DS_Store
+-rw-r--r--   0 luca       (501) staff       (20)       27 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/.gitignore
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/__init__.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.171671 lmql-0.0.4.2/src/lmql/ui/live/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     6747 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/live.js
+-rw-r--r--   0 luca       (501) staff       (20)     3299 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/live.py
+-rw-r--r--   0 luca       (501) staff       (20)     3885 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/livelib.py
+-rw-r--r--   0 luca       (501) staff       (20)      349 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/package.json
+-rw-r--r--   0 luca       (501) staff       (20)    33701 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/yarn.lock
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.177348 lmql-0.0.4.2/src/lmql/ui/playground/
+-rw-r--r--   0 luca       (501) staff       (20)       31 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/.dockerignore
+-rw-r--r--   0 luca       (501) staff       (20)       34 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/.env
+-rw-r--r--   0 luca       (501) staff       (20)      310 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/.gitignore
+-rw-r--r--   0 luca       (501) staff       (20)      354 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/Dockerfile
+-rw-r--r--   0 luca       (501) staff       (20)     3359 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/README.md
+-rw-r--r--   0 luca       (501) staff       (20)     1327 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/package.json
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.182529 lmql-0.0.4.2/src/lmql/ui/playground/public/
+-rw-r--r--   0 luca       (501) staff       (20)       90 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/_headers
+-rw-r--r--   0 luca       (501) staff       (20)     3870 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/favicon.ico
+-rw-r--r--   0 luca       (501) staff       (20)     1678 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/index.html
+-rw-r--r--   0 luca       (501) staff       (20)     2817 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/lmql.svg
+-rw-r--r--   0 luca       (501) staff       (20)      306 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/manifest.json
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.203625 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/
+-rw-r--r--   0 luca       (501) staff       (20)  1227728 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-r--r--   0 luca       (501) staff       (20)   295285 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-r--r--   0 luca       (501) staff       (20)   160153 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-r--r--   0 luca       (501) staff       (20)    81768 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-r--r--   0 luca       (501) staff       (20)     5221 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-r--r--   0 luca       (501) staff       (20)    89531 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-r--r--   0 luca       (501) staff       (20)  1710847 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-r--r--   0 luca       (501) staff       (20)    52748 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/list.json
+-rw-r--r--   0 luca       (501) staff       (20)   628184 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-r--r--   0 luca       (501) staff       (20)   264768 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-r--r--   0 luca       (501) staff       (20)   215050 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-r--r--   0 luca       (501) staff       (20)       67 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/robots.txt
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.205833 lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/
+-rw-r--r--   0 luca       (501) staff       (20)   381736 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-r--r--   0 luca       (501) staff       (20)   252806 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-r--r--   0 luca       (501) staff       (20)       62 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/ref.py
+-rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/run-in-docker.sh
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.222161 lmql-0.0.4.2/src/lmql/ui/playground/src/
+-rw-r--r--   0 luca       (501) staff       (20)    67646 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/App.jsx
+-rw-r--r--   0 luca       (501) staff       (20)      246 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/App.test.js
+-rw-r--r--   0 luca       (501) staff       (20)    29983 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-r--r--   0 luca       (501) staff       (20)      807 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/Configuration.js
+-rw-r--r--   0 luca       (501) staff       (20)     1174 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/DataListView.js
+-rw-r--r--   0 luca       (501) staff       (20)    20848 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-r--r--   0 luca       (501) staff       (20)      329 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/DecodingTree.js
+-rw-r--r--   0 luca       (501) staff       (20)       89 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/Embed.jsx
+-rw-r--r--   0 luca       (501) staff       (20)     9601 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/Explore.jsx
+-rw-r--r--   0 luca       (501) staff       (20)      675 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/SharedState.js
+-rw-r--r--   0 luca       (501) staff       (20)     3868 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/State.js
+-rw-r--r--   0 luca       (501) staff       (20)     5738 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-r--r--   0 luca       (501) staff       (20)     9360 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/browser_process.js
+-rw-r--r--   0 luca       (501) staff       (20)     1163 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/build_info.js
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.223378 lmql-0.0.4.2/src/lmql/ui/playground/src/editor/
+-rw-r--r--   0 luca       (501) staff       (20)     8673 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-r--r--   0 luca       (501) staff       (20)     4758 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/editor/theme.json
+-rw-r--r--   0 luca       (501) staff       (20)      889 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/explore.svg
+-rw-r--r--   0 luca       (501) staff       (20)     1345 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/graph-layout.css
+-rw-r--r--   0 luca       (501) staff       (20)     1698 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/index.css
+-rw-r--r--   0 luca       (501) staff       (20)      489 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/index.js
+-rw-r--r--   0 luca       (501) staff       (20)     2632 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/logo.svg
+-rw-r--r--   0 luca       (501) staff       (20)     8077 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/queries.js
+-rw-r--r--   0 luca       (501) staff       (20)     5990 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/remote_process.js
+-rw-r--r--   0 luca       (501) staff       (20)      362 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-r--r--   0 luca       (501) staff       (20)     9520 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/screenshot.css
+-rw-r--r--   0 luca       (501) staff       (20)      241 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/setupTests.js
+-rw-r--r--   0 luca       (501) staff       (20)     3466 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/spinner.svg
+-rw-r--r--   0 luca       (501) staff       (20)     2949 2023-04-10 14:55:16.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-r--r--   0 luca       (501) staff       (20)   449905 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/yarn.lock
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.229927 lmql-0.0.4.2/src/lmql/ui/vscode/
+-rw-r--r--   0 luca       (501) staff       (20)       76 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.gitattributes
+-rw-r--r--   0 luca       (501) staff       (20)       19 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.gitignore
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.230695 lmql-0.0.4.2/src/lmql/ui/vscode/.vscode/
+-rw-r--r--   0 luca       (501) staff       (20)      540 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.vscode/launch.json
+-rw-r--r--   0 luca       (501) staff       (20)       66 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.vscodeignore
+-rw-r--r--   0 luca       (501) staff       (20)    12820 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/LICENSE
+-rw-r--r--   0 luca       (501) staff       (20)      357 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/README.md
+-rw-r--r--   0 luca       (501) staff       (20)      959 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/language-configuration.json
+-rw-r--r--   0 luca       (501) staff       (20)    11532 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/lmql-vscode.png
+-rw-r--r--   0 luca       (501) staff       (20)     1214 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/package.json
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.232551 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/
+-rw-r--r--   0 luca       (501) staff       (20)      518 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-r--r--   0 luca       (501) staff       (20)      642 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-r--r--   0 luca       (501) staff       (20)      853 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.234023 lmql-0.0.4.2/src/lmql/utils/
+-rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/utils/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     5384 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/utils/graph.py
+-rw-r--r--   0 luca       (501) staff       (20)     1474 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/utils/nputil.py
+-rw-r--r--   0 luca       (501) staff       (20)      115 2023-04-13 08:25:13.000000 lmql-0.0.4.2/src/lmql/version.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.122163 lmql-0.0.4.2/src/lmql.egg-info/
+-rw-r--r--   0 luca       (501) staff       (20)     4646 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/PKG-INFO
+-rw-r--r--   0 luca       (501) staff       (20)     6621 2023-04-13 08:25:21.000000 lmql-0.0.4.2/src/lmql.egg-info/SOURCES.txt
+-rw-r--r--   0 luca       (501) staff       (20)        1 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/dependency_links.txt
+-rw-r--r--   0 luca       (501) staff       (20)       39 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/entry_points.txt
+-rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/requires.txt
+-rw-r--r--   0 luca       (501) staff       (20)        5 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/top_level.txt
```

### Comparing `lmql-0.0.4.1/.github/workflows/lmql-web.yml` & `lmql-0.0.4.2/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/.gitignore` & `lmql-0.0.4.2/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -164,7 +164,9 @@
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks
+
+wip-snippets
```

### Comparing `lmql-0.0.4.1/LICENSE` & `lmql-0.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/PKG-INFO` & `lmql-0.0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.4.1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.4.2 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.4.1/README.md` & `lmql-0.0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/Makefile` & `lmql-0.0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/make.bat` & `lmql-0.0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.4.2/docs/source/_static/css/lmql-docs.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .highlight.lmql {
     border: 1pt solid rgb(212, 212, 212);
     position: relative;
 }
 
+html[data-theme="dark"] .highlight.lmql {
+    border: 1pt solid rgb(110, 109, 109);
+}
+
 .highlight.lmql iframe {
     background-color: var(--pst-color-background);
 }
 
 .highlight.lmql.playground {
     border: none;
 }
@@ -91,14 +95,24 @@
     font-size: 10pt;
     font-weight: bold;
     font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
     cursor: pointer;
     color:rgba(0, 0, 0, 0.957)
 }
 
+html[data-theme="dark"] .getting-started>a {
+    background-color: rgb(57, 57, 57) !important;
+    border-color: rgb(75, 75, 75);
+    color: rgb(215, 215, 215);
+}
+
+html[data-theme="dark"] .getting-started>a.primary {
+    background-color: rgb(66, 64, 174) !important;
+}
+
 .getting-started>a:hover {
     background-color: rgb(233, 228, 228);
 }
 
 
 .getting-started .cmd {
     padding: 5pt;
@@ -151,51 +165,113 @@
 .nboutput .highlight pre {
     /* break lines */
     white-space: break-spaces !important;
 }
 
 .highlight-model-output::before {
     content: "Model Output";
+    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
     position: absolute;
-    top: -10pt;
+    top: 4pt;
     font-size: 9pt;
     text-transform: uppercase;
     left: 0pt;
     z-index: 2;
     width: 100%;
     text-align: center;
     color: grey;
 }
 
 .highlight-model-output {
     position: relative;
     padding-left: 5pt;
+    top: -5pt;
     padding-right: 5pt;
     z-index: -1;
-    font-size: 0.95em;
+    font-size: 0.9em;
+    font-family: monospace;
 }
 
 html[data-theme="dark"] .highlight-model-output::before {
     color: rgb(143, 143, 143);
 }
 
 html[data-theme="dark"] .highlight-model-output {
     background: transparent;
 }
 
 .highlight-model-output .highlight, html[data-theme="dark"] .highlight-model-output .highlight {
-    background: transparent !important;
-}
-
-html[data-theme="dark"] .highlight-model-output .highlight pre {
-    background-color: rgb(30, 30, 30);
-    border-color: rgb(68, 68, 68);
+    display: block;
+    white-space: break-spaces !important;
 }
 
 
-.highlight-model-output .highlight pre {
-    background-color: #fbfbfb;
+.highlight-model-output .highlight {
+    background-color: #fbfbfb !important;
+    border: 0.5pt solid grey;
     position: relative;
-    top: -12pt;
+    /* top: -12pt; */
     border-color: rgb(223, 219, 219);
     white-space: break-spaces !important;
+    padding: 10pt;
+    padding-top: 20pt;
+}
+
+html[data-theme="dark"] .highlight-model-output .highlight {
+    background-color: rgb(30, 30, 30) !important;
+    border-color: rgb(68, 68, 68) !important;
+}
+
+.variable {
+    display: inline; 
+    padding: 0.5pt;
+}
+
+.variable .variable-name {
+    font-weight: 700;
+    color: #333;
+    background-color: rgba(0, 0, 0, 0.4);
+    border-radius: 0.2em;
+    font-family: monospace;
+    color: rgba(255, 255, 255, 0.9);
+    display: inline;
+    margin: 0;
+    margin-right: 0.0em;
+    margin-left: 0;
+    font-size: 0.7em;
+    padding: 0.12em;
+    position: relative;
+    top: -0.15em;
+    left: 0.1em;
+
+    transform-origin: 0 50%;
+    overflow: hidden;
+}
+
+.variable .variable-name.visible {
+    opacity: 1.0;
+}
+
+.val1 {
+    background-color: rgba(255, 166, 0, 0.5) !important;
+    cursor: default;
+}
+
+.val1:hover, .val1.hover, .val1-hover .val1 {
+    background-color: rgba(255, 166, 0, 1.0) !important;
+}
+.val2 {
+    background-color: rgba(206, 128, 184, 1.0) !important;
+    cursor: default;
+}
+
+.val2:hover, .val2.hover, .val2-hover .val2 {
+    background-color: rgba(206, 128, 184, 1.0) !important;
+}
+.val3 {
+    background-color: rgb(130, 140, 249) !important;
+    cursor: default;
+}
+
+.val3:hover, .val3.hover, .val3-hover .val3 {
+    background-color: rgba(107, 119, 255, 1.0) !important;
 }
```

### Comparing `lmql-0.0.4.1/docs/source/_static/images/lmql.svg` & `lmql-0.0.4.2/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.4.2/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/conf.py` & `lmql-0.0.4.2/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 source_suffix = {
     '.rst': 'restructuredtext',
     '.txt': 'markdown',
     '.md': 'markdown',
 }
 
+pygments_style = 'one-dark'
+
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
     'sphinx': ('https://www.sphinx-doc.org/en/master/', None),
 }
 intersphinx_disabled_domains = ['std']
 
 templates_path = ['_templates']
```

### Comparing `lmql-0.0.4.1/docs/source/dev-setup.md` & `lmql-0.0.4.2/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/index.rst` & `lmql-0.0.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/installation.md` & `lmql-0.0.4.2/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/language/constraints.md` & `lmql-0.0.4.2/docs/source/language/constraints.md`

 * *Files 9% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 name::number
 argmax
    "A number: [N]"
 from
    'openai/text-ada-001'
 where
     INT(N)
-```
-```model-output
-A number: 2
+
+model-output::
+A number: [N 2]
 ```
 
 **Note:** If multiple variables in the query have the same name, the constraint is applied to all of them.
 
 ## Choice From Set
 LMQL allows to specify that a variable should be a choice from a set of possible values. This can be rephrased as the variable being within a  set of possible values, i.e. `THING in set(["Volleyball", "Sunscreen", "Bathing Suite"])` in the following example
 
@@ -52,42 +52,40 @@
    "- Sunglasses \n"
    for i in range(4):
       "- [THING] \n"
 from
    'openai/text-ada-001'
 where
    THING in set(["Volleyball", "Sunscreen", "Bathing Suite"])
-```
 
-```model-output
+model-output::
 A list of things not to forget when going to the sea (not travelling): ⏎
-- Sunglasses ⏎
-- Sunscreen ⏎
-- Volleyball ⏎
-- Sunscreen ⏎
-- Sunscreen ⏎
+- [THING Sunglasses] ⏎
+- [THING Sunscreen] ⏎
+- [THING Volleyball] ⏎
+- [THING Sunscreen] ⏎
+- [THING Sunscreen] ⏎
 ```
 
 ## Length 
-Similar to Python the `len` function can be used to refer to the length of a variable and can thus be used to add constraints on it's length.
+Similar to Python, the `len` function can be used to refer to the length of a variable and can thus be used to add constraints on it's length.
 
 ```{lmql}
 name::length
 argmax
    "Hello [NAME]"
 from
    'openai/text-3a-001'
 where
     len(NAME) < 10
-```
 
-```model-output
-Hello ⏎
+model-output::
+Hello [NAME ⏎
 ⏎
-I am in
+I am in]
 ```
 
 ## Combining Constraints
 Several constraints can be combined with the `and` and `or` keywords, recovering a Python boolean expression over the variables utilized in the LMQL query.
 
 
 ## Custom Constraints and Theoretical Background
```

### Comparing `lmql-0.0.4.1/docs/source/language/decoders.md` & `lmql-0.0.4.2/docs/source/language/decoders.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 Among other things, this view allows you to track the decoding process, active hypotheses and interpreter state, including the current evaluation result of the `where` clause. For an example, consider the [translation example](https://lmql.ai/playground/#translation) as included in the Playground IDE (make sure to enable `Advanced Mode`).
 
 
 ## Other Decoding Parameters
 
 * `max_len: int` - The maximum length of the generated sequence. If not specified, the default value of `max_len` is `512`. Note if the maximum length is reached, the LMQL runtime will throw an error if the query has not yet come to a valid result, according to the provided `where` clause.
 
-* `openai_chunksize: int` - The chunksize parameter for OpenAI's `Completion` API. If not specified, the default value of `openai_chunksize` is `32`. See also the description of this parameter in the [Models](models.md#configuring-speculative-openai-api-use) chapter.
+* `openai_chunksize: int` - The chunksize parameter for OpenAI's `Completion` API. If not specified, the default value of `openai_chunksize` is `32`. See also the description of this parameter in the [Models](./models.md#configuring-speculative-openai-api-use) chapter.
```

### Comparing `lmql-0.0.4.1/docs/source/language/functions.md` & `lmql-0.0.4.2/docs/source/language/functions.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 argmax
     "A simple math problem for addition (without solution, without words): [MATH]"
     "{eval(MATH[:-1])}"
 from 
     'openai/text-davinci-003'
 where
     STOPS_AT(MATH, "=")
-```
 
-```model-output
+model-output::
 A simple math problem for addition (without solution, without words):
-7 + 8 = 15
+[MATH 7 + 8 =] 15
 ```
 
 
 
 Here, similar to a python [f-string](https://peps.python.org/pep-0498), we use the `{}` syntax to insert the result of the `eval` function into the prompt. The `[:-1]` indexing is used to strip of the trailing `=` sign.
 
 **Note:** While `eval` is handy for the examples in this section and allows to perform simple math, generally it can pose a security risk and should not be used in production.
@@ -58,22 +57,22 @@
       "is[RESULT]"
 from 
       'openai/text-davinci-003'
 where
       STOPS_AT(REASON_OR_CALC, "<<") and
       STOPS_AT(EXPR, "=") and
       STOPS_AT(REASON_OR_CALC, "So the answer")
-```
-```model-output
+
+model-output::
 Q: Josh decides to try flipping a house.  He buys a house for $80,000 and then puts in $50,000 in repairs.  This increased the value of the house by 150%.  How much profit did he make?
 Let's think step by step.
-Josh bought the house for $80,000 and put in $50,000 in repairs.
-The value of the house increased by 150%, so the new value of the house is $80,000 + 150% of $80,000 = << 80,000 + (80,000*1.5) = 200000.0>>$200,000.
-The profit Josh made is the difference between the new value of the house and the amount he spent on it, which is $200,000 - $80,000 - $50,000 = << 200,000 - 80,000 - 50,000 = 70000>>$70,000.
-So the answer is $70,000.
+[REASON_OR_CALC Josh bought the house for $80,000 and put in $50,000 in repairs.
+The value of the house increased by 150%, so the new value of the house is $80,000 + 150% of $80,000 = <<] [EXPR 80,000 + (80,000*1.5) =] 200000.0>> [REASON_OR_CALC $200,000.
+The profit Josh made is the difference between the new value of the house and the amount he spent on it, which is $200,000 - $80,000 - $50,000 = <<] [EXPR 200,000 - 80,000 - 50,000 =] 70000>> [REASON_OR CALC $70,000.
+So the answer] is [RESULT $70,000.]
 ```
 
 ## Beyond Calculators
 Function use is not limited to calculators. In the example bellow we show how text retrieval, using Pythons `async`/`await` [syntax](https://docs.python.org/3/library/asyncio.html), can be used to augment the reasoning capabilities of the large language model. 
 
 ```{lmql}
 name::wikipedia
@@ -92,22 +91,22 @@
    result = await wikipedia(TERM)
    "Result: {result}\n"
    "Final Answer:[ANSWER]"
 from 
    "openai/text-davinci-003"
 where
    STOPS_AT(TERM, "'")
-```
-```model-output
+
+model-output::
 Q: From which countries did the Norse originate?
-Action: Let's search Wikipedia for the term 'Norse'.
+Action: Let's search Wikipedia for the term '[TERM Norse'].
 Result: Norse is a demonym for Norsemen, a Medieval North Germanic ethnolinguistic group ancestral to modern Scandinavians, defined as speakers of Old Norse from about the 9th to the 13th centuries.
 Norse may also refer to:
 
-Final Answer: The Norse originated from North Germanic countries, including Denmark, Norway, Sweden, and Iceland.
+Final Answer: [ANSWER The Norse originated from North Germanic countries, including Denmark, Norway, Sweden, and Iceland.]
 ```
 
 LMQL can also access the state of the surrounding python interpreter. To showcase this, we show how to use the `assign` and `get` functions to store and retrieve values in a simple key-value store.
 
 ```{lmql}
 name::kvstore
 # simple kv storage
@@ -138,39 +137,39 @@
    """Therefore at the end of the game, Alice has the[OBJECT]"""
    assert "blue ball." in OBJECT
 from 
    "openai/text-davinci-003"
 where
    STOPS_AT(REASONING, "# result") and STOPS_AT(REASONING, "Therefore, ") and
    STOPS_AT(OBJECT, ".") and STOPS_AT(OBJECT, ",")            
-```
-```model-output
+
+model-output::
 (...)
 A: Let's think step by step
 
-At the start of the game:
-`assign("Alice", "black") # result {Alice: "black"}`
-`assign("Bob", "brown") # result {Bob: "brown"}`
-`assign("Claire", "blue") # result {Claire: "blue"}`
-
-After Bob and Claire swap balls:
-`assign("Bob", "blue") # result {Bob: "blue"}`
-`assign("Claire", "brown") # result {Claire: "brown"}`
-
-After Alice and Bob swap balls:
-`assign("Alice", "blue") # result {Alice: "blue"}`
-`assign("Bob", "black") # result {Bob: "black"}`
-
-After Claire and Bob swap balls:
-`assign("Claire", "black") # result {Claire: "black"}`
-`assign("Bob", "brown") # result {Bob: "brown"}`
-
-At the end of the game, Alice has a blue ball:
-`get("Alice") # result blue`
-Therefore at the end of the game, Alice has the blue ball.
+[REASONING At the start of the game:
+`assign("Alice", "black") # result] {Alice: "black"}`
+[REASONING `assign("Bob", "brown") # result] {Bob: "brown"}`
+[REASONING `assign("Claire", "blue") # result] {Claire: "blue"}`
+
+[REASONING After Bob and Claire swap balls:
+`assign("Bob", "blue") # result] {Bob: "blue"}`
+[REASONING `assign("Claire", "brown") # result] {Claire: "brown"}`
+
+[REASONING After Alice and Bob swap balls:
+`assign("Alice", "blue") # result] {Alice: "blue"}`
+[REASONING `assign("Bob", "black") # result] {Bob: "black"}`
+
+[REASONING After Claire and Bob swap balls:
+`assign("Claire", "black") # result] {Claire: "black"}`
+[REASONING `assign("Bob", "brown") # result] {Bob: "brown"}`
+
+[REASONING At the end of the game, Alice has a blue ball:
+`get("Alice") # result] blue`
+Therefore at the end of the game, Alice has the [OBJECT blue ball.]
 ```
 
 As shown in the example above, the `assign` and `get` functions can be used to store and retrieve values in a simple key-value store. The model is merely instructed to make use of these functions in its reasoning. The query then implements logic to intercept any function use and insert the result of the function call into the reasoning. This allows the model to incorporate the state of the key-value store into its reasoning.
```

### Comparing `lmql-0.0.4.1/docs/source/language/models.md` & `lmql-0.0.4.2/docs/source/language/models.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 * `openai/gpt-3.5-turbo` also available as `chatgpt`
 * `openai/gpt-4` also available as `gpt-4`
 
 ### OpenAI API Limitations
 
 Unfortunately, the OpenAI API Completions and Chat API are severely limited in terms of token masking and the availability of the token distribution per predicted token. LMQL tries to leverage these APIs as much as possible, but there are some limitations that we have to work around and may affect users:
 
-* The **OpenAI Completion API limits the number of possible logit biases to 300**. This means, if your constraints induce token masks that are larger than 300 tokens, LMQL will automatically truncate the token mask to the first 300 tokens. This may lead to unexpected behavior, e.g., model performance may be worse than expected as the masking. In cases where the 300 biases limit is exceeded, LMQL prints a warning message to the console, indicating the number of biases that were truncated.
+* The **OpenAI Completion API limits the number of possible logit biases to 300**. This means, if your constraints induce token masks that are larger than 300 tokens, LMQL will automatically truncate the token mask to the first 300 tokens. This may lead to unexpected behavior, e.g., model performance may be worse than expected as the masks are truncated to be more restrictive than necessary. In cases where the 300 biases limit is exceeded, LMQL prints a warning message to the console, indicating that the logit biases were truncated.
 
 * The **OpenAI Completions API only provides the top-5 logprobs per predicted token**. This means that decoding algorithms that explore e.g. the top-n probabilities to make decisions like beam search, are limited to a branching factor of 5.
 
 * The **OpenAI Chat API does not provide any way to mask tokens or obtain the token distribution (ChatGPT, GPT-4)**. Simple constraints can still be enforced, as the LMQL runtime optimizes them to fit the OpenAI API. However, more complex constraints may not be enforceable. In these cases, LMQL will print a error message to the console. As a workaround users may then adjust their constraints to fit these API limitations or resort to post-processing and backtracking. Scripted prompting, intermediate instructions and simple constraints are still supported with Chat API models, nonetheless.
 
 ### Configuring OpenAI API Credentials
```

### Comparing `lmql-0.0.4.1/docs/source/language/overview.md` & `lmql-0.0.4.2/docs/source/language/overview.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Overview
 
 LMQL is a declarative, SQL-like programming language for language model interaction. As an example consider the following query, demonstrating the basic syntax of LMQL:
-
+ 
 ```{lmql}
 
 name::overview-query
 argmax
    """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
    Q: What is the underlying sentiment of this review and why?
    A:[ANALYSIS]
    Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
 from 
    "openai/text-davinci-003"
 where
    not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"]
-```
-```model-output
+
+model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
-A: The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.⏎
-Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION]
+A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
+Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION positive]
 ```
 
 In this program, we use the language model `openai/text-davinci-003` (GPT-3.5) to perform a sentiment analysis on a provided user review. We first ask the model to provide some basic analysis of the review, and then we ask the model to classify the overall sentiment as one of `positive`, `neutral`, or `negative`. The model is able to correctly identify the sentiment of the review as `positive`.
 
 Overall, the query consists of four main clauses:
 
 1. **Decoder Clause** First, we specify the decoding algorithm to use for text generation. In this case we use `argmax` decoding, however, LMQL also support branching decoding algorithms like beam search. See [Decoders](./decoders.md) to learn more about this.
@@ -70,19 +70,19 @@
    Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
 from 
    "openai/text-davinci-003"
 where
    not "\n" in ANALYSIS
 distribution
    CLASSIFICATION in [" positive", " neutral", " negative"]
-```
-```model-output
+
+model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
-A: The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.⏎
+A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
 Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION]
 
 P(CLASSIFICATION)
  -  positive (*) 0.9999244826658527
  -  neutral      7.513155848720942e-05
  -  negative     3.8577566019560874e-07
 ```
@@ -115,21 +115,21 @@
       "What is it that could have been improved? [FURTHER_ANALYSIS]"
    elif CLASSIFICATION == " negative":
       "What is it that they did not like about their stay? [FURTHER_ANALYSIS]"
 from
     "openai/text-davinci-003"
 where
     not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"] and STOPS_AT(FURTHER_ANALYSIS, ".")
-```
-```model-output
+
+model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
-A: The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.⏎
-Based on this, the overall sentiment of the message can be considered to be positive⏎
+A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
+Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION positive]⏎
 What is it that they liked about their stay?⏎
 ⏎
-The reviewer liked the hiking in the mountains and the food.
+[FURTHER_ANALYSIS The reviewer liked the hiking in the mountains and the food.]
 ```
 
 As shown here, we can use the `if` statement to dynamically react to the model's output. In this case, we ask the model to provide a more detailed analysis of the review, depending on the overally positive, neutral, or negative sentiment of the review. All intermediate variables like `ANALYSIS`, `CLASSIFICATION` or `FURTHER_ANALYSIS` can be considered the output of query, and may be processed by an surrounding automated system. 
 
 To learn more about the capabilities of such control-flow-guided prompts, see [Scripted Prompting](./scripted_prompts.md).
```

### Comparing `lmql-0.0.4.1/docs/source/language/scripted_prompts.md` & `lmql-0.0.4.2/docs/source/language/scripted_prompts.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,22 +8,21 @@
   
 name::list
 sample(temperature=0.8)
    "A few things not to forget when going to the sea (not travelling): \n"
    "[LIST]"
 from
    'openai/text-ada-001'
-```
 
-```model-output
+model-output::
 A list of things not to forget when going to the sea (not travelling):
-
--A phone with call, texting or tech services
+[LIST -A phone with call, texting or tech services
 -A copy of the local paper
 -A pen or phone Keytar
+]
 ```
 
 This can work well, however, it is unclear if the model will always produce a well-structured list of items. Further, we have to parse the response to separate the various items and process them further.
 
 **Simple Prompt Templates** To address this, we can provide a more rigid prompt template, where we already provide the output format and let the model only fill in the `THING` variable:
 
 ```{lmql}
@@ -36,23 +35,22 @@
    "-[THING]"
    "-[THING]"
    "-[THING]"
 from
    'openai/text-ada-001'
 where
    STOPS_AT(THING, "\n")
-```
 
-```model-output
+model-output::
 A list of things not to forget when going to the sea (not travelling):
--A phone with a/r text
--pletter
--accoon
--Films about/of the sea
--A has been in the Poconos for/ Entered the Poconos
+-[THING A phone with a/r text]
+-[THING pletter]
+-[THING accoon]
+-[THING Films about/of the sea]
+-[THING A has been in the Poconos for/ Entered the Poconos]
 ```
 
 Note how we use a stopping condition on `THING`, such that a new line in the model output leads to a continuation of our provided template. Without the stopping condition, simple template filling would not be possible, as the model would generate more than one items for the first variable already.
 
 **Prompt with Control-Flow** Given this prompt template, we can now leverage control flow in our prompt, to further process results, while also guiding text generation. First, we simplify our query and use a `for` loop instead of repeating the variable ourselves:
 
 ```{lmql}
@@ -65,25 +63,24 @@
       "-[THING]"
       backpack.append(THING.strip())
    print(backpack)
 from
    'openai/text-ada-001'
 where
    STOPS_AT(THING, "\n")
-```
 
-```model-output
+model-output::
 A list of things not to forget when going to the sea (not travelling):
--A good pair of blue/gel saskaers
--A good sun tanner
--A good air freshener
--A good spot forwashing your hands
--A good spot for washing your feet
+-[THING A good pair of blue/gel saskaers]
+-[THING A good sun tanner]
+-[THING A good air freshener]
+-[THING A good spot forwashing your hands]
+-[THING A good spot for washing your feet]
 
-# print output: ['A good pair of blue/gel saskaers', 'A good sun tanner', 'A good air freshener', 'A good spot forwashing your hands', 'A good spot for washing your feet']
+# print output: \['A good pair of blue/gel saskaers', 'A good sun tanner', 'A good air freshener', 'A good spot forwashing your hands', 'A good spot for washing your feet'\]
 ```
 
 Because we decode our list `THING` by `THING`, we can easily access the individual items, without having to think about parsing or validation. We just add them to a `backpack` list of things, which we then can process further.
 
 ## Python Compatibility
 
 Going beyond simple control flow, LMQL supports most valid Python constructs in the prompt clause of a query, where top-level strings like `"-[THING]"` are automatically interpreted as model input and template variables are assigned accordingly. For more advanced usage, also see the [External Functions](functions.md) chaptor.
```

### Comparing `lmql-0.0.4.1/docs/source/lmql.svg` & `lmql-0.0.4.2/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/logo.png` & `lmql-0.0.4.2/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/python/langchain.ipynb` & `lmql-0.0.4.2/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/python/lmql.txt` & `lmql-0.0.4.2/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/docs/source/python/python.ipynb` & `lmql-0.0.4.2/docs/source/python/python.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963942307692308%*

 * *Differences: {"'cells'": "{12: {'source': ['### Syntax Highlighting\\n', '\\n', 'LMQL also provides a syntax "*

 * *            'highlighter for Visual Studio Code. Both `.lmql` files as well as `.py` files with '*

 * *            '`@lmql.query` decorated functions will be highlighted automatically. The syntax '*

 * *            'highlighter is available as a [VSCode '*

 * *            "extension](https://marketplace.visualstudio.com/items?itemName=lmql-team.lmql).\\n', "*

 * *            "'\\n', 'To enable syntax highlighting in Python files,  […]*

```diff
@@ -198,17 +198,26 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This capability of calling arbitrary program logic during query execution, enables powerful use cases like the integration of retrieval, as discussed in the [LangChain Integration](./langchain.ipynb) chapter."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
-            "source": []
+            "source": [
+                "### Syntax Highlighting\n",
+                "\n",
+                "LMQL also provides a syntax highlighter for Visual Studio Code. Both `.lmql` files as well as `.py` files with `@lmql.query` decorated functions will be highlighted automatically. The syntax highlighter is available as a [VSCode extension](https://marketplace.visualstudio.com/items?itemName=lmql-team.lmql).\n",
+                "\n",
+                "To enable syntax highlighting in Python files, make sure to lead the LMQL code in an `@lmql.query` function with the `lmql` code block type:\n",
+                "\n",
+                "<img width=\"528\" alt=\"image\" src=\"https://user-images.githubusercontent.com/17903049/230897738-a676cd6b-bec2-4403-8628-1c10d3da263c.png\">\n"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "lmql",
             "language": "python",
             "name": "python3"
```

### Comparing `lmql-0.0.4.1/docs/source/quickstart.md` & `lmql-0.0.4.2/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/scripts/wheel.sh` & `lmql-0.0.4.2/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/setup.cfg` & `lmql-0.0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.4.1
+version = 0.0.4.2
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.4.1/src/lmql/__init__.py` & `lmql-0.0.4.2/src/lmql/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 __author__ = 'Luca Beurer-Kellner, Marc Fischer and Mark Mueller'
 __email__ = "luca.beurer-kellner@inf.ethz.ch"
 __license__ = "MIT"
 
 from lmql.language.compiler import LMQLCompiler
 import lmql.runtime.lmql_runtime as lmql_runtime
 import tempfile
-from lmql.runtime.output_writer import silent, stream
+from lmql.runtime.output_writer import silent, stream, printing
 from lmql.runtime.model_registry import LMQLModelRegistry
 from lmql.runtime.lmql_runtime import LMQLQueryFunction, FunctionContext
 
+import lmql.runtime.lmql_runtime as runtime_support
+
+# re-export lmql runtime functions
+from lmql.runtime.lmql_runtime import compiled_query, tag
+
 import os
 
 model_registry = LMQLModelRegistry
 
 def connect(server="http://localhost:8080", model_name="EleutherAI/gpt-j-6B"):
     from lmql.runtime.hf_integration import transformers_model
```

### Comparing `lmql-0.0.4.1/src/lmql/cli.py` & `lmql-0.0.4.2/src/lmql/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,23 @@
     os.system("python -m lmql.model.serve " + " ".join(sys.argv[2:]))
 
 def cmd_run():
     """
     emoji:🏃 run a LMQL script (e.g. "lmql run latest/hello.lmql")
     """
     import asyncio
+    import time
+
+    start = time.time()
 
     parser = argparse.ArgumentParser(description="Runs a LMQL program.")
     parser.add_argument("lmql_file", type=str, help="path to the LMQL file to run")
     parser.add_argument("--no-clear", action="store_true", dest="no_clear", help="don't clear inbetween printing results")
     parser.add_argument("--no-realtime", action="store_true", dest="no_realtime", help="don't print text as it's being generated")
+    parser.add_argument("--time", action="store_true", dest="time", help="Time the query.")
 
     args = parser.parse_args(sys.argv[2:])
 
     absolute_path = os.path.abspath(args.lmql_file)
     from lmql.runtime.output_writer import PrintingDebuggerOutputWriter
 
     writer = PrintingDebuggerOutputWriter()
@@ -49,14 +53,17 @@
             max_length = max([len(str(l)) for l in labels])
 
             print(v)
             for (value, prob), label in zip(distribution, labels):
                 label = label.ljust(max_length)
                 print(" - {} {}".format(label, prob))
 
+    if args.time:
+        print("Query took:", time.time() - start)
+
 def ensure_node_install():
     try:
         v = subprocess.check_output("node --version", shell=True, stderr=subprocess.DEVNULL).decode("utf-8").strip()
     except:
         print("""node.js is not installed. Please install it to use the LMQL playground.
 
 If your Python installation is managed by conda, you can install node.js with:
@@ -186,8 +193,8 @@
     if len(command) == 0:
         print("Unknown command: " + sys.argv[1])
         cmd_usage()
         sys.exit(1)
     command[0]()
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `lmql-0.0.4.1/src/lmql/demo.py` & `lmql-0.0.4.2/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/http.py` & `lmql-0.0.4.2/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/language/compiler.py` & `lmql-0.0.4.2/src/lmql/language/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from lmql.ops.ops import lmql_operation_registry
 
 from lmql.language.qstrings import qstring_to_stmts, TemplateVariable
 from lmql.language.validator import LMQLValidator, LMQLValidationError
 from lmql.language.fragment_parser import LMQLDecoderConfiguration, LMQLQuery, LanguageFragmentParser, FragmentParserError
 from lmql.runtime.model_registry import model_name_aliases
 
+OPS_NAMESPACE = "lmql.ops"
+
 class PromptScope(ast.NodeVisitor):
     def scope(self, query: LMQLQuery):
         self.distribution_vars = set([query.distribution.variable_name]) if query.distribution is not None else set()    
         self.defined_vars = set()
 
         # collect set of global query template variables
         self.free_vars = set()
@@ -103,14 +105,17 @@
             elif type(stmt) is TemplateVariable:
                 if stmt.name in self.query.scope.distribution_vars:
                     compiled_qstring += f"[distribution:{stmt.name}]"
                 else:
                     declared_template_vars.add(stmt.name)
                     compiled_qstring += "[" + stmt.name + "]"
 
+        if len(compiled_qstring) == 0:
+            return constant
+
         result_code = f'yield context.query(f"""{compiled_qstring}""")'
 
         for v in declared_template_vars:
             result_code += f"\n{v} = context.get_var('{v}')"
         return ast.parse(result_code)
 
     # def transform_prompt_stmt(self, stmt):
@@ -194,64 +199,69 @@
         if bn is not None: return bn
         # check if variable is distribution variable
         if node.id in self.scope.distribution_vars:
             raise LMQLValidationError("Distribution variable {} cannot be used in where clause.".format(node.id))
 
         # check for template variables
         if node.id in self.scope.defined_vars and not keep_variables:
-            return f"lmql.Var('{node.id}')"
+            return f"lmql.runtime_support.Var('{node.id}')"
 
         return bn or node.id
 
     def transform_node(self, expr, snf):
         if type(expr) is ast.BoolOp:
             if type(expr.op) is ast.And or type(expr.op) is ast.Or:
                 ops = expr.values
                 tops = [self.transform_node(op, snf) for op in ops]
                 tops_list = ",\n  ".join([t.strip() or "None" for t in tops])
                 
-                Op = "lmql.AndOp" if type(expr.op) is ast.And else "lmql.OrOp"
+                Op = "lmql.runtime_support.AndOp" if type(expr.op) is ast.And else "lmql.OrOp"
                 return snf.add(f"{Op}([\n  {tops_list}\n])")
         # elif type(expr) is ast.Call:
         #     tfunc = self.transform_node(expr.func, snf)
         #     targs = [self.transform_node(a, snf) for a in expr.args]
         #     targs_list = ", ".join(targs)
         #     return f"{tfunc}({targs_list})"
         elif type(expr) is ast.Name:
             return self.transform_name(expr)
         elif type(expr) is ast.UnaryOp:
             op = expr.op
             
             Ops = {
-                ast.Not: "lmql.NotOp"
+                ast.Not: f"{OPS_NAMESPACE}.NotOp"
             }
 
             for OpT, impl in Ops.items():
                 if type(op) is OpT:
                     operand = self.transform_node(expr.operand, snf).strip()
                     return snf.add(f"{impl}([{operand}])")
             
             assert False, "unary operator {} not supported.".format(type(expr.op))
         elif type(expr) is ast.Compare:
             op = expr.ops[0]
             assert len(expr.ops) == 1, "compiler currently does not support comparison with more than one operator"
             
             Ops = {
-                ast.Eq: "lmql.EqOp",
-                ast.Lt: "lmql.Lt",
-                ast.Gt: "lmql.Gt",
-                ast.In: "lmql.InOp"
+                ast.Eq: f"{OPS_NAMESPACE}.EqOp",
+                ast.Lt: f"{OPS_NAMESPACE}.Lt",
+                ast.Gt: f"{OPS_NAMESPACE}.Gt",
+                ast.In: f"{OPS_NAMESPACE}.InOp"
             }
 
             for OpT, impl in Ops.items():
                 if type(op) is OpT: 
                     ops = [self.transform_node(c, snf) for c in [expr.left] + expr.comparators]
                     ops_list = ", ".join(ops).strip()
                     return snf.add(f"{impl}([{ops_list}])")
             
+            # if is_type_constraint(expr):
+            #     type_name = expr.comparators[0].id
+            #     var_name = expr.left.args[0].id
+            #     return snf.add(f"{OPS_NAMESPACE}.TypeConstraint([{type_name}, {OPS_NAMESPACE}.Var('{var_name}')])")
+            
             assert False, "operator {} is not supported.".format(astunparse.unparse(expr))
         elif type(expr) is ast.Constant:
             return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.ListComp:
             return self.default_transform_node(expr, snf).strip()
         elif type(expr) is ast.Call:
             bn = get_builtin_name(expr.func)
@@ -282,35 +292,56 @@
 
         def transform_name(node):
             node.id = self.transform_name(node, keep_variables=True, plain_python=True)
             return node
         node = NameTransformer(transform_name).visit(node)
 
         args = (" " + ", ".join(names)) if len(names) > 0 else ""
-        var_ops = (", ".join([f"lmql.Var('{n}')" for n in names])).strip() if len(names) > 0 else ""
+        var_ops = (", ".join([f"{OPS_NAMESPACE}.Var('{n}')" for n in names])).strip() if len(names) > 0 else ""
         fct_code = astunparse.unparse(node).strip()
         
-        return f"lmql.OpaqueLambdaOp([lambda{args}: {fct_code}, {var_ops}])"
+        return f"{OPS_NAMESPACE}.OpaqueLambdaOp([lambda{args}: {fct_code}, {var_ops}])"
 
 def is_allowed_builtin_python_call(node):
     if type(node) is not ast.Name:
         return False
     allowed_builtin_functions = set(["set", "all"])
     return node.id in allowed_builtin_functions
 
 def get_builtin_name(node, plain_python=False):
     if type(node) is not ast.Name:
         return None
     n = node.id
     
     if n in lmql_operation_registry.keys():
-        return lmql_operation_registry[n]
+        return OPS_NAMESPACE + "." + lmql_operation_registry[n]
     
     return None
 
+def is_type_constraint(expr: ast.Expr):
+    if not type(expr.left) is ast.Call:
+        return False
+    if not type(expr.left.func) is ast.Name:
+        return False
+    if not expr.left.func.id == "type":
+        return False
+    if not type(expr.ops[0]) is ast.Is:
+        return False
+    if not len(expr.comparators) == 1:
+        return False
+    right = expr.comparators[0]
+    if not type(right) is ast.Name:
+        return False
+    if not len(expr.left.args) == 1:
+        return False
+    if not type(expr.left.args[0]) is ast.Name:
+        return False
+    
+    return True
+
 class DecodeClauseTransformation:
     def __init__(self, query):
         self.query = query
 
     def transform(self):
         if type(self.query.decode) is ast.Name:
             method = ast.Constant(self.query.decode.id, "str")
@@ -348,15 +379,15 @@
         self.prologue = prologue
         
         self.in_memory_contents = ""
         
         self.file = open(self.filename, "w")
 
         self.indent = "  "
-        self.write("import lmql.runtime.lmql_runtime as lmql\n")
+        self.write("import lmql\n")
         self.write(self.prologue)
         
         if decorators is not None:
             if decorators_args is None:
                 decorators_args = [None] * len(decorators)
             for d,args in zip(decorators, decorators_args):
                 self.write(f"@{d}({args})\n")
@@ -462,15 +493,15 @@
 
             # resulting code
             code = None
             output_variables = "output_variables=[" + ", ".join([f'"{v}"' for v in scope.defined_vars]) + "]"
 
             # generate function that runs query
             with PythonFunctionWriter("query", output_file, list(scope.free_vars) + ["context"], 
-                q.prologue, decorators=["lmql.query"], decorators_args=[output_variables]) as writer:
+                q.prologue, decorators=["lmql.compiled_query"], decorators_args=[output_variables]) as writer:
                 
                 writer.add(f"context.set_model({model_name})")
                 writer.add(f"context.set_decoder({astunparse.unparse(q.decode.method).strip()}, {unparse_list(q.decode.decoding_args)})")
                 writer.add("# where")
                 writer.add(q.where)
                 writer.add(f"context.set_where_clause({q.where_expr})")
                 writer.add("# prompt")
```

### Comparing `lmql-0.0.4.1/src/lmql/language/fragment_parser.py` & `lmql-0.0.4.2/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/language/qstrings.py` & `lmql-0.0.4.2/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/language/validator.py` & `lmql-0.0.4.2/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/lib/errors.py` & `lmql-0.0.4.2/src/lmql/lib/errors.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/lib/expr_jitter.py` & `lmql-0.0.4.2/src/lmql/lib/expr_jitter.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/lib/scope.py` & `lmql-0.0.4.2/src/lmql/lib/scope.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/model/async_generation_utils.py` & `lmql-0.0.4.2/src/lmql/model/async_generation_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/model/client.py` & `lmql-0.0.4.2/src/lmql/model/client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/model/hf_beam_search.py` & `lmql-0.0.4.2/src/lmql/model/hf_beam_search.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/model/local_client.py` & `lmql-0.0.4.2/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/model/serve.py` & `lmql-0.0.4.2/src/lmql/model/serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ops/follow_map.py` & `lmql-0.0.4.2/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ops/ops.py` & `lmql-0.0.4.2/src/lmql/ops/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 lmql_operation_registry = {}
 
 # @LMQLOp('function_name') decorator
 def LMQLOp(name):
     def class_transformer(cls):
         if type(name) is list:
             for n in name:
-                lmql_operation_registry[n] = f"lmql.{cls.__name__}"
+                lmql_operation_registry[n] = f"{cls.__name__}"
             return cls
-        lmql_operation_registry[name] = f"lmql.{cls.__name__}"
+        lmql_operation_registry[name] = f"{cls.__name__}"
         return cls
     return class_transformer
+
 class Node:
     def __init__(self, predecessors):
         assert type(predecessors) is list, "Predecessors must be a list, not {}".format(type(predecessors))
         self.predecessors = predecessors
         self.depends_on_context = False
         
         self.follow_map = None
```

### Comparing `lmql-0.0.4.1/src/lmql/ops/token_set.py` & `lmql-0.0.4.2/src/lmql/ops/token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/backtracker.py` & `lmql-0.0.4.2/src/lmql/runtime/backtracker.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.4.2/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.4.2/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,17 +546,20 @@
     def __del__(self):
         if self.stats_logger is not None:
             self.stats_logger.cancel()
         # cancel the score worker task
         self.complete_api_worker.cancel()
         for worker in self.complete_request_workers:
             worker.cancel()
-        loop = asyncio.get_event_loop()
-        while not all([t.done() for t in (self.complete_request_workers + [self.complete_api_worker])]):
-            loop._run_once()
+        try:
+            loop = asyncio.get_event_loop()
+            while not all([t.done() for t in (self.complete_request_workers + [self.complete_api_worker])]):
+                loop._run_once()
+        except:
+            pass # if no more event loop is around, no need to wait for the workers to finish
 
     async def api_complete_worker(self, queue):
         while True:
             self.futures = set([f for f in self.futures if not f.done()])
             while Capacity.reserved >= Capacity.total * 0.8:
                 # print("wait before queing more requests", flush=True)
                 await asyncio.sleep(0.1)
```

### Comparing `lmql-0.0.4.1/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.4.2/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 from dataclasses import dataclass
 
 from .dclib_global import get_tokenizer
 from .dclib_array import DataArray, Continuation, topk, alpha_length_normalized, alpha_length_normalized_det
 
 detokenize_seqs = True
 
+@dataclass
+class DecoderGraphSnapshot:
+    node_hashes = None
+    step_not_updated_count = None
+
 class DecoderGraph:
     def __init__(self):
         self.nodes = {}
         self.node_ids = {}
         self.edges = []
 
         self.ctr = 0
 
+        self.json_snapshot: DecoderGraphSnapshot = DecoderGraphSnapshot()
+
     def add_node(self, node):
         uid = f"n{self.ctr}"
         self.ctr += 1
         self.node_ids[node] = uid
         self.nodes[uid] = node
         return uid
     
@@ -30,21 +37,47 @@
         if not self.node_ids[node] in self.nodes:
             self.add_node(node)
         self.nodes[self.node_ids[node]]["pool"] = pool_name
     
     def add_edge(self, from_node, to_node):
         self.edges.append((self.node_ids[from_node], self.node_ids[to_node]))
 
-    async def json(self):
+    async def json(self, diff: bool = False):
         nodes = []
+        
+        if self.json_snapshot.node_hashes is None:
+            self.json_snapshot.node_hashes = {}
+        if self.json_snapshot.step_not_updated_count is None:
+            self.json_snapshot.step_not_updated_count = {}
+        
         for k, v in self.nodes.items():
+            hash = None
+            if diff and k in self.json_snapshot.node_hashes:
+                # this will ignore changes to nodes that have not been updated for 3 steps (may miss changes to nodes that 
+                # are not updated for a long time, careful for now)
+                if k in self.json_snapshot.step_not_updated_count and self.json_snapshot.step_not_updated_count[k] > 2:
+                    continue
+                hash = await v.json_hash()
+                if self.json_snapshot.node_hashes[k] == str(hash):
+                    self.json_snapshot.step_not_updated_count[k] = self.json_snapshot.step_not_updated_count.get(k, 0) + 1
+                    continue
+                    
+                # else:
+                #     print("node changed", k, self.json_snapshot.node_hashes[k], hash)
+            if hash is None:
+                hash = await v.json_hash()
+
             nodes.append({
                 "id": k,
                 **await v.json()
             })
+            
+            if diff:
+                self.json_snapshot.node_hashes[k] = str(hash)
+                self.json_snapshot.step_not_updated_count[k] = 0
 
         return {
             "nodes": nodes,
             "edges": self.edges
         }
 
 class DecoderSequence:
@@ -176,14 +209,20 @@
             self.tokenizer_cache = {}
         if name not in self.tokenizer_cache:
             assert name in providers, f"Unknown tokenizer cache provider {name}"
             self.tokenizer_cache[name] = await providers[name]()
         
         return self.tokenizer_cache[name]
 
+    async def json_hash(self):
+        o = await self.json()
+        if type(o["user_data"]) is dict and "openai-continuations" in o["user_data"]:
+            o["user_data"].pop("openai-continuations")
+        return hash(str(o))
+
     async def json(self):
         seqtext = await self.detokenized("seqtext")
         text = await self.detokenized("text")
         if self.epsilon_node: text = [""]
         root = False
         if self.predecessor is None:
             text = await self.detokenized("seqtext")
```

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/decoders.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/lmql_adapter.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/lmql_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,36 +162,46 @@
         decoder_args["dcmodel"] = dcmodel
         dc.set_truncation_threshold(dcmodel.truncation_threshold)
 
         step_budget = decoder_args.get("step_budget", 1024)
         
         async def debug_out(decoder_step):
             if _DCLibDebugPrinter.printer is not None and dc.DecoderSequence.graph is not None:
-                data = await dc.DecoderSequence.graph.json()
+                data = await dc.DecoderSequence.graph.json(diff=True)
                 data = replace_inf_nan_with_str(data)
                 _DCLibDebugPrinter.printer.add_decoder_state(data)
             dcmodel.report_stats(_DCLibDebugPrinter.printer, decoder_step)
 
         try:
+            import time
+
             decoder_step = 0
+            average_step_time = None
+            start = time.time()
             async for _ in decoder_fct(prompt_ids, **decoder_args):
                 await debug_out(decoder_step)
                 decoder_step += 1
 
                 if step_budget is not None and decoder_step >= step_budget:
                     print("warning: step budget exceeded")
                     break
-                
-                if "performance_stats" in decoder_args:
-                    Stats.print_all()
 
                 if interrupt.check():
                     interrupt.clear()
                     raise InterruptedError("lmql.runtime.interrupt")
                 
+                average_step_time = (time.time() - start) if average_step_time is None else (average_step_time * 0.9 + (time.time() - start) * 0.1)
+
+                if "performance_stats" in decoder_args:
+                    if decoder_step % 10 == 0:
+                        Stats.print_all()
+                        print("step", decoder_step, "time", average_step_time)
+
+                start = time.time()
+                
         except dc.FinishException as fe:
             # one last call to debug_out to get the final state
             await debug_out(decoder_step)
             # if dc.finish is used, the decoder sets the sequences it considers 
             # finished (return them to prompt interpreter)
             result_sequences = fe.result_sequences
             
@@ -206,15 +216,15 @@
                 billable_tokens += upper + (1 if has_deterministic_tail else 0)
             
             dcmodel.log_billable_tokens(billable_tokens)
             
             return [self.make_decoder_head(i,n,s) for i,s in enumerate(result_sequences)]
     
     def validate_args(self, decoder_args, decoder_fct):
-        INTERNAL_ARGS = ["decoder", "dcmodel", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats"]
+        INTERNAL_ARGS = ["decoder", "dcmodel", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats"]
 
         # get all arg names and kwarg names of decoder function
         decoder_arg_names = inspect.getfullargspec(decoder_fct).args
         decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
         for k in decoder_args.keys():
             if k not in decoder_arg_names and k not in decoder_kwarg_names and k not in INTERNAL_ARGS:
                 raise ValueError("Unknown decoder argument: {}".format(k))
```

### Comparing `lmql-0.0.4.1/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.4.2/src/lmql/runtime/dclib/trie_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/decoder_head.py` & `lmql-0.0.4.2/src/lmql/runtime/decoder_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/hf_integration.py` & `lmql-0.0.4.2/src/lmql/runtime/hf_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/langchain.py` & `lmql-0.0.4.2/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.4.2/src/lmql/runtime/lmql_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         interpreter.print_stats()
 
         return results
 
 def tag(t):
     return f"<lmql:{t}/>"
 
-def query(output_variables=None, group_by=None):
+def compiled_query(output_variables=None, group_by=None):
     if output_variables is None:
         output_variables = []
     
     postprocessors = []
     
     calling_frame = inspect.stack()[1]
```

### Comparing `lmql-0.0.4.1/src/lmql/runtime/maiohttp.py` & `lmql-0.0.4.2/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/model_registry.py` & `lmql-0.0.4.2/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.4.2/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/openai_integration.py` & `lmql-0.0.4.2/src/lmql/runtime/openai_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/openai_secret.py` & `lmql-0.0.4.2/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/output_writer.py` & `lmql-0.0.4.2/src/lmql/runtime/output_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import termcolor
 
 class DebuggerOutputWriter:
     def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables): pass
     def add_compiler_output(self, code): pass
 
 class PrintingDebuggerOutputWriter:
-    def __init__(self):
-        self.clear = False
+    def __init__(self, clear=False):
+        self.clear = clear
         self.print_output = True
 
     def add_decoder_state(*args, **kwargs): 
         pass
 
     def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
         if head == 0:
@@ -50,8 +50,9 @@
             
             os.system("clear")
             print(f"{prompt}\n", end="\r")
             
     def add_compiler_output(self, code): pass
 
 silent = DebuggerOutputWriter()
-stream = StreamingOutputWriter
+stream = StreamingOutputWriter
+printing = PrintingDebuggerOutputWriter(clear=True)
```

### Comparing `lmql-0.0.4.1/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.4.2/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/program_state.py` & `lmql-0.0.4.2/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/prompt_interpreter.py` & `lmql-0.0.4.2/src/lmql/runtime/prompt_interpreter.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/rewriter.py` & `lmql-0.0.4.2/src/lmql/runtime/rewriter.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/stats.py` & `lmql-0.0.4.2/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/tok.ipynb` & `lmql-0.0.4.2/src/lmql/runtime/tok.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/runtime/tokenizer.py` & `lmql-0.0.4.2/src/lmql/runtime/tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 global reverse_special_token_mappings
 reverse_special_token_mappings = {}
 
 class LMQLTokenizer:
     def __init__(self, tokenizer_impl):
         self.tokenizer_impl = tokenizer_impl
 
+        self.detokenizer_cache = {}
+
     @property
     def vocab_size(self):
         return self.tokenizer_impl.vocab_size
 
     @property
     def bos_token_id(self):
         return self.tokenizer_impl.bos_token_id
@@ -88,20 +90,45 @@
             if s.startswith("lmql:"):
                 tokens.append(s)
             else:
                 tokens += self.tokenizer_impl.tokenize(s)
         return tokens
         
     def decode(self, input_ids):
+        key = str(input_ids)
+        n = len(input_ids)
+        if n in self.detokenizer_cache.keys():
+            if key in self.detokenizer_cache[n].keys():
+                # print("cache hit")
+                return self.detokenizer_cache[n][key]
+        if n-1 in self.detokenizer_cache.keys():
+            key = str(input_ids[:-1])
+            if key in self.detokenizer_cache[n-1].keys():
+                global reverse_special_token_mappings
+                # print("secondary cache hit")
+                if input_ids[-1] >= self.tokenizer_impl.vocab_size:
+                    extended = self.detokenizer_cache[n-1][key] + "<" + reverse_special_token_mappings[input_ids[-1]] + "/>"
+                else:
+                    extended = self.detokenizer_cache[n-1][key] + self.tokenizer_impl.decode([input_ids[-1]])
+                if not n in self.detokenizer_cache.keys():
+                    self.detokenizer_cache[n] = {}
+                self.detokenizer_cache[n][str(input_ids)] = extended
+                return extended
+
         s = ""
         for chunk in self.chunk_out_by_special_ids(input_ids):
             if type(chunk) is str:
                 s += chunk
             else:
                 s += self.tokenizer_impl.decode(chunk)
+
+        if not n in self.detokenizer_cache.keys():
+            self.detokenizer_cache[n] = {}
+        self.detokenizer_cache[n][key] = s
+
         return s
 
     def __call__(self, s: str):
         input_ids = []
         unpack = False
         if type(s) is not list:
             s = [s]
```

### Comparing `lmql-0.0.4.1/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.4.2/src/lmql/tests/expr_test_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/mask_product_test.py` & `lmql-0.0.4.2/src/lmql/tests/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/monotonicity.py` & `lmql-0.0.4.2/src/lmql/tests/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/one_of_tests.py` & `lmql-0.0.4.2/src/lmql/tests/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/sentences_op.py` & `lmql-0.0.4.2/src/lmql/tests/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/starts_with_op_test.py` & `lmql-0.0.4.2/src/lmql/tests/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/stops_at.py` & `lmql-0.0.4.2/src/lmql/tests/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/str_in_str_tests.py` & `lmql-0.0.4.2/src/lmql/tests/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.4.2/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/test_multi_head.py` & `lmql-0.0.4.2/src/lmql/tests/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/tests/token_set_test.py` & `lmql-0.0.4.2/src/lmql/tests/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/live/live.js` & `lmql-0.0.4.2/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/live/live.py` & `lmql-0.0.4.2/src/lmql/ui/live/live.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/live/livelib.py` & `lmql-0.0.4.2/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/live/yarn.lock` & `lmql-0.0.4.2/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/README.md` & `lmql-0.0.4.2/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/package.json` & `lmql-0.0.4.2/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.4.2/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/index.html` & `lmql-0.0.4.2/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.4.2/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.4.2/src/lmql/ui/playground/src/App.jsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import './graph-layout.css';
 
 import styled from 'styled-components';
 import Editor from "@monaco-editor/react";
 import React, { useEffect, useRef, useState } from "react";
 import { registerLmqlLanguage } from "./editor/lmql-monaco-language";
-import { BsSquare, BsFillExclamationSquareFill, BsBoxArrowUpRight, BsArrowRightCircle, BsCheckSquare, BsSendFill, BsFileArrowDownFill, BsKeyFill, BsTerminal, BsFileCode, BsGithub, BsCardList, BsFullscreen, BsXCircle, BsFillChatLeftTextFill, BsGear, BsGridFill } from 'react-icons/bs';
+import { BsSquare, BsFillExclamationSquareFill, BsBoxArrowUpRight, BsArrowRightCircle, BsFillCameraFill, BsCheckSquare, BsSendFill, BsFileArrowDownFill, BsKeyFill, BsTerminal, BsFileCode, BsGithub, BsCardList, BsFullscreen, BsXCircle, BsFillChatLeftTextFill, BsGear, BsGridFill } from 'react-icons/bs';
 import { DecoderGraph } from './DecoderGraph';
 import { BUILD_INFO } from './build_info';
 import exploreIcon from "./explore.svg"
 import { ExploreState, Explore, PromptPopup, Dialog } from './Explore'
+import { CodeScreenshot } from "./CodeScreenshot";
 import { errorState, persistedState, trackingState, displayState} from "./State"
 import { configuration, LMQLProcess, isLocalMode} from './Configuration';
 import { ValidationGraph } from "./ValidationGraph";
 import { DataListView } from "./DataListView";
 
 import {reconstructTaggedModelResult} from "./tagged-model-result"
 
@@ -758,26 +759,26 @@
     margin-top: 10pt;
     margin-bottom: 10pt;
     color: #c0c0c0;
   }
 
   div .tag-assistant {
     display: inline-block;
-    width: 65%;
     border: 1pt solid #5c5c5c;
     margin-top: 5pt;
+    margin-right: 4%;
 
     border-radius: 8pt;
     overflow: hidden;
     padding: 4pt;
   }
 
   div .tag-user {
     display: block;
-    margin-left: 32%;
+    margin-left: 4%;
     position: relative;
     border: 1pt solid #5c5c5c;
     border-radius: 8pt;
     padding: 4pt;
     margin-bottom: 2pt;
     margin-top: 5pt;
   }
@@ -913,16 +914,16 @@
       expandedText: ""
     }
     this.stepper = null
   }
 
   componentDidMount() {
     this.stepper = setInterval(() => {
-      this.setState(s => Object.assign(s, { typingOffset: s.typingOffset + 4 }))
-    }, 10)
+      this.setState(s => Object.assign(s, { typingOffset: s.typingOffset + 16 }))
+    }, 5)
   }
 
   componentWillUnmount() {
     clearInterval(this.stepper)
   }
 
   componentDidUpdate(prevProps) {
@@ -1729,14 +1730,15 @@
   const defaultClass = stretch ? 'stretch' : '';
   const clearTrigger = useState(new TriggerState())[0];
   const [clearOnRun, setClearOnRun] = useState(true);
   const [perVariableColor, setPerVariableColor] = useState(true);
 
   const [trackMostLikly, setTrackMostLiklyInternal] = useState(window.localStorage.getItem("trackMostLikely") === "true");
   trackingState.setTrackMostLikely = setTrackMostLiklyInternal
+  trackingState.getTrackMostLikely = () => trackMostLikly
   const setTrackMostLikly = (value) => {
     setTrackMostLiklyInternal(value)
     window.localStorage.setItem("trackMostLikely", value)
     if (!value && props.mostLikelyNode) {
       trackingState.setSelectedNode(props.mostLikelyNode)
     }
   }
@@ -2334,14 +2336,17 @@
       buildInfo: BUILD_INFO.info(),
       status: LMQLProcess.status,
       processState: "init",
       graphLayout: false,
       topMenuOpen: false,
       // true by default, false if local storage is set
       simpleMode: window.localStorage.getItem("simple-mode") == "true",
+
+      /* show code screenshot overlay */
+      codeScreenshot: false
     }
   }
 
   setSimpleMode(simpleMode) {
     window.localStorage.setItem("simple-mode", simpleMode);
     ResizeObservers.notify();
     this.setState({ simpleMode });
@@ -2477,14 +2482,35 @@
   };
 
   onMostLiklyNode(node) {
     if (node == null) { return }
     this.setMostLikelyNode(node)
   };
 
+  getCodeScreenshotInput() {
+    let modelResult = null;
+    if (trackingState.getTrackMostLikely()) {
+      modelResult = reconstructTaggedModelResult([this.state.mostLikelyNode]);
+    } else {
+      modelResult = reconstructTaggedModelResult(this.state.selectedNodes);
+    }
+    return {
+      "code": persistedState.getItem("lmql-editor-contents"),
+      "model_result": modelResult,
+    }
+  }
+
+  onCodeScreenshot() {
+    this.setState({ codeScreenshot: true })
+  }
+
+  hideCodeScreenshot() {
+    this.setState({ codeScreenshot: false })
+  }
+
   render() {
     trackingState.setSelectedNode = n => {
       this.onSelectNode(n)
       this.state.selectedNodeTrigger.trigger(n)
     };
 
     const simpleModeClassName = this.state.simpleMode ? "" : "simple-mode";
@@ -2513,16 +2539,16 @@
           <Commit>{this.state.buildInfo.commit}</Commit>
           <ToggleButton onClick={() => this.setTopMenuOpen(!this.state.topMenuOpen)} toggled={this.state.topMenuOpen}>
             <BsGear size={14} />
             <TopBarMenu className={this.state.topMenuOpen ? 'visible' : ''}>
               {configuration.BROWSER_MODE && <li onClick={() => OpenAICredentialsState.setOpen(true)}>
               <BsKeyFill/> OpenAI Credentials
               </li>}
-              {configuration.DEV_MODE && <li onClick={() => this.onExportState()}><BsFileArrowDownFill/> Export State
-              </li>}
+              {configuration.DEV_MODE && <li onClick={() => this.onExportState()}><BsFileArrowDownFill/> Export State</li>}
+              {configuration.DEV_MODE && <li onClick={() => this.onCodeScreenshot()}><BsFillCameraFill/> Code Screenshot</li>}
               <li>
                 <a href="https://github.com/eth-sri/lmql" disabled target="_blank" rel="noreferrer"><BsGithub/>LMQL on Github</a>
               </li>
               <span>
                 LMQL {this.state.buildInfo.commit} 
                 {(configuration.BROWSER_MODE && !isLocalMode()) && <> In-Browser</>}
                 {isLocalMode() && <> Self-Hosted</>}
@@ -2540,13 +2566,14 @@
         </Row>
         <Row style={{ flex: 1 }} className={simpleModeClassName}>
           <DecoderPanel onSelectNode={this.onSelectNode.bind(this)} onMostLiklyNode={this.onMostLiklyNode.bind(this)} selectedNodeTrigger={this.state.selectedNodeTrigger} />
           <InspectorPane nodeInfo={this.state.selectedNodeInfo}></InspectorPane>
         </Row>
         <OpenAICredentials />
         {configuration.DEMO_MODE && displayState.mode != "embed" && <Explore />}
+        {this.state.codeScreenshot && <CodeScreenshot hide={this.hideCodeScreenshot.bind(this)} {...this.getCodeScreenshotInput()}/>}
       </ContentContainer>
     );
   }
 }
 
 export default App;
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -575,18 +575,22 @@
                     }
                     let e = {
                         data: {
                             source: from,
                             target: to
                         }
                     };
-                    cy.add({
-                        group: "edges",
-                        ...e
-                    })
+                    try {
+                        cy.add({
+                            group: "edges",
+                            ...e
+                        })
+                    } catch (e) {
+                        console.error("error adding edge", e)
+                    }
                 }))
 
                 let mostLikely = layoutDecoderGraph(cy)
 
                 if (props.onMostLiklyNode) {
                     props.onMostLiklyNode(mostLikely)
                 }
@@ -599,19 +603,34 @@
 
     // on mount
     useEffect(() => {
         // conn is RemotePRocessConnection
         const renderer = {
             add_result: (output) => {
                 if (output.type == "decoder-graph-state") {
-                    // persist decoder graph in local state
-                    const raw = JSON.stringify(output.data)
-                    setRawGraphData(raw)
-                    persistedState.setItem("decoder-graph", raw, onPersistedGraphChange)
-                    setCyData(output.data)
+                    setCyData(cyData => {
+                        // persist decoder graph in local state
+                        let updated = Object.assign({
+                            nodes: [],
+                            edges: []
+                        }, cyData || {})
+                        let nodes = {}
+                        updated.nodes.forEach(n => nodes[n.id] = n)
+                        output.data.nodes.forEach(n => nodes[n.id] = n)
+                        updated.nodes = Array.from(Object.values(nodes))
+
+                        updated.edges = Array.from([...updated.edges, ...output.data.edges])
+
+                        // console.log("updating", output.data.nodes.length)
+
+                        const raw = JSON.stringify(updated)
+                        setRawGraphData(raw)
+                        persistedState.queueSetItem("decoder-graph", raw, onPersistedGraphChange)
+                        return updated
+                    })
                 } else {
                     // nop in this component
                 }
             },
             clear_results: () => setCyData(null),
         }
         LMQLProcess.addRenderer(renderer)
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.4.2/src/lmql/ui/playground/src/Explore.jsx`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import React, { useEffect, useState } from "react";
 import styled from "styled-components";
 import {queries} from "./queries";
-import { persistedState, trackingState } from "./State";
+import { displayState, persistedState, trackingState } from "./State";
 
 export const PromptPopup = styled.div`
   position: absolute;
   top: 0;
   left: 0;
   width: 100vw;
   height: 100vh;
@@ -367,15 +367,15 @@
     useEffect(() => {
         // register listeners
         ExploreState.listeners.push(setVisible);
 
         // check if first visit
         const editorContents = window.localStorage.getItem("lmql-editor-contents");
         if (editorContents === null || (typeof editorContents === "string" && editorContents.trim().length === 0)) {
-          ExploreState.setVisibility(true);
+          ExploreState.setVisibility(!displayState.preloaded);
         }
 
         // check for hash-specified example to load
         if (window.location.hash && !didLoadAnchor) {
           didLoadAnchor = true;
           const anchor = window.location.hash.substring(1);
           let matches = queries.filter(c => c.queries.find(q => q.state.includes(anchor)))
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/State.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/State.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,11 @@
+import {
+    queries
+} from "./queries";
+
 function getSnippet(allow_snippet = true) {
     const url = window.location.href
     if (url.indexOf('?') === -1) {
         return null
     }
     const parameters = url.split('?')[1]
     if (parameters.startsWith('embed=')) {
@@ -12,22 +16,25 @@
         return null
     }
 }
 
 export const displayState = {
     // if ?embed, mode = embed, else playground
     mode: getSnippet(false) ? 'embed' : 'playground',
+    preloaded: getSnippet(true) ? true : false,
     embedFile: null
 }
 
 class PersistedState {
     constructor() {
         this.items = {}
         this.listeners = {}
         this.restore()
+
+        this.saveQueue = {}
     }
 
     persist(k) {
         Object.keys(this.items).forEach(key => {
             if (!key || key === k) {
                 window.localStorage.setItem(key, this.items[key]);
             }
@@ -39,16 +46,21 @@
             this.items[key] = window.localStorage.getItem(key);
         })
 
         // check for snippet or embed
         let snippetFile = getSnippet()
         if (snippetFile) {
             console.log("loading snippet from", snippetFile)
+            let matches = queries.filter(c => c.queries.find(q => q.state == "precomputed/" + snippetFile + ".json"))
+            if (matches.length === 1) {
+                let q = matches[0].queries.find(q => q.state == "precomputed/" + snippetFile + ".json")
+                snippetFile = q.state
+            }
+
             fetch(snippetFile).then(r => r.text()).then(data => {
-                console.log(data)
                 // remove ? from url
                 window.history.replaceState({}, document.title, window.location.pathname);
                 if (data) {
                     displayState.embedFile = snippetFile
                     this.load(data)
                 }
             })
@@ -104,20 +116,30 @@
 
         if (this.listeners[key]) {
             this.listeners[key].forEach(listener => {
                 if (listener !== exclude_listener) listener(value);
             })
         }
     }
+
+    queueSetItem(key, value, exclude_listener = null) {
+        if (this.saveQueue[key]) {
+            clearTimeout(this.saveQueue[key]);
+        }
+        this.saveQueue[key] = setTimeout(() => {
+            this.setItem(key, value, exclude_listener);
+        })
+    }
 }
 
 export const persistedState = new PersistedState();
 
 export const trackingState = {
     setTrackMostLikely: () => {},
+    getTrackMostLikely: () => false,
     setSelectedNode: () => {},
 }
 
 export const errorState = {
     addListener: listener => {
         errorState.listeners.push(listener);
     },
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.4.2/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.4.2/src/lmql/ui/playground/src/editor/theme.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993206521739131%*

 * *Differences: {"'rules'": "{2: {'foreground': '98c379'}}"}*

```diff
@@ -17,15 +17,15 @@
             "token": ""
         },
         {
             "foreground": "6272a4",
             "token": "comment"
         },
         {
-            "foreground": "f1fa8c",
+            "foreground": "98c379",
             "token": "string"
         },
         {
             "foreground": "bd93f9",
             "token": "constant.numeric"
         },
         {
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.4.2/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.4.2/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/index.css` & `lmql-0.0.4.2/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.4.2/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/queries.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -71,15 +71,15 @@
    expert_name = EXPERT.rstrip(".\\n")
    "For instance,{expert_name} would answer[ANSWER]"
 from 
    "openai/text-davinci-001"
 where
    STOPS_AT(EXPERT, ".") and STOPS_AT(EXPERT, "\\n") and STOPS_AT(ANSWER, ".")`,
                 state: 'precomputed/meta.json'
-            }, ]
+            }]
         }, {
             category: "Tool-Augmented Queries",
             queries: [{
                 name: "🧮 Calculator",
                 description: "On-the-fly arithmetic evaluation using Python.",
                 code: `import re
 from lmql.demo import gsm8k_samples
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.4.2/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.4.2/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.4.2/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.4.2/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.4.2/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.4.2/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/vscode/package.json` & `lmql-0.0.4.2/src/lmql/ui/vscode/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6923076923076923%*

 * *Differences: {"'description'": "'Syntax highlighting for .lmql and Python files with embedded LMQL.'",*

 * * "'displayName'": "'Language Model Query Language (LMQL) Syntax Highlighting'",*

 * * "'icon'": "'lmql-vscode.png'",*

 * * "'publisher'": "'lmql-team'",*

 * * "'readme'": "'./README.md'"}*

```diff
@@ -36,17 +36,20 @@
                 "extensions": [
                     ".lmql"
                 ],
                 "id": "lmql"
             }
         ]
     },
-    "description": "Language Model Query Language",
-    "displayName": "Language Model Query Language (LMQL)",
+    "description": "Syntax highlighting for .lmql and Python files with embedded LMQL.",
+    "displayName": "Language Model Query Language (LMQL) Syntax Highlighting",
     "engines": {
         "vscode": "^1.76.0"
     },
     "homepage": "https://lmql.ai",
+    "icon": "lmql-vscode.png",
     "name": "lmql",
+    "publisher": "lmql-team",
+    "readme": "./README.md",
     "repository": "https://github.com/eth-sri/lmql",
     "version": "0.0.1"
 }
```

### Comparing `lmql-0.0.4.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql/utils/graph.py` & `lmql-0.0.4.2/src/lmql/utils/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     def write(self, obj, info=None):
         if hasattr(obj, "to_graph"):
             obj.to_graph(self)
             return True
         elif hasattr(obj, "__dataclass_fields__"):
             self.node(obj, label=str(type(obj)))
             for f in obj.__dataclass_fields__:
+                # handle type references
+                if type(object) is type:
+                    return False
                 vs = obj.__dict__[f]
                 if type(vs) is not list: vs = [vs]
                 for v in vs:
                     if self.write(v, f):
                         self.edge(obj, v)
             return True
         elif isinstance(obj, Node):
```

### Comparing `lmql-0.0.4.1/src/lmql/utils/nputil.py` & `lmql-0.0.4.2/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.1/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.4.2/src/lmql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.4.1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.4.2 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.4.1/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.4.2/src/lmql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/source/lmql.svg
 docs/source/logo.png
 docs/source/quickstart.md
 docs/source/_ext/lmql_snippets.py
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
+docs/source/_templates/layout.html
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/python/.gitignore
@@ -38,15 +39,14 @@
 scripts/pypi-release.sh
 scripts/wheel.sh
 scripts/conda/requirements-no-gpu.yml
 scripts/conda/requirements.yml
 src/lmql/__init__.py
 src/lmql/cli.py
 src/lmql/demo.py
-src/lmql/hello-chat.lmq_compiled.py
 src/lmql/http.py
 src/lmql/version.py
 src/lmql.egg-info/PKG-INFO
 src/lmql.egg-info/SOURCES.txt
 src/lmql.egg-info/dependency_links.txt
 src/lmql.egg-info/entry_points.txt
 src/lmql.egg-info/requires.txt
@@ -112,14 +112,15 @@
 src/lmql/tests/sentences_op.py
 src/lmql/tests/starts_with_op_test.py
 src/lmql/tests/stops_at.py
 src/lmql/tests/str_in_str_tests.py
 src/lmql/tests/test_multi_head.py
 src/lmql/tests/token_set_test.py
 src/lmql/tests/system/basic_use_cases.py
+src/lmql/ui/.DS_Store
 src/lmql/ui/.gitignore
 src/lmql/ui/__init__.py
 src/lmql/ui/live/__init__.py
 src/lmql/ui/live/live.js
 src/lmql/ui/live/live.py
 src/lmql/ui/live/livelib.py
 src/lmql/ui/live/package.json
@@ -146,16 +147,19 @@
 src/lmql/ui/playground/public/precomputed/hello.json
 src/lmql/ui/playground/public/precomputed/joke.json
 src/lmql/ui/playground/public/precomputed/kv.json
 src/lmql/ui/playground/public/precomputed/list.json
 src/lmql/ui/playground/public/precomputed/meta.json
 src/lmql/ui/playground/public/precomputed/translation.json
 src/lmql/ui/playground/public/precomputed/wiki.json
+src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+src/lmql/ui/playground/public/snippets/json-parsing.json
 src/lmql/ui/playground/src/App.jsx
 src/lmql/ui/playground/src/App.test.js
+src/lmql/ui/playground/src/CodeScreenshot.jsx
 src/lmql/ui/playground/src/Configuration.js
 src/lmql/ui/playground/src/DataListView.js
 src/lmql/ui/playground/src/DecoderGraph.js
 src/lmql/ui/playground/src/DecodingTree.js
 src/lmql/ui/playground/src/Embed.jsx
 src/lmql/ui/playground/src/Explore.jsx
 src/lmql/ui/playground/src/SharedState.js
@@ -167,24 +171,27 @@
 src/lmql/ui/playground/src/graph-layout.css
 src/lmql/ui/playground/src/index.css
 src/lmql/ui/playground/src/index.js
 src/lmql/ui/playground/src/logo.svg
 src/lmql/ui/playground/src/queries.js
 src/lmql/ui/playground/src/remote_process.js
 src/lmql/ui/playground/src/reportWebVitals.js
+src/lmql/ui/playground/src/screenshot.css
 src/lmql/ui/playground/src/setupTests.js
 src/lmql/ui/playground/src/spinner.svg
 src/lmql/ui/playground/src/tagged-model-result.js
 src/lmql/ui/playground/src/editor/lmql-monaco-language.js
 src/lmql/ui/playground/src/editor/theme.json
 src/lmql/ui/vscode/.gitattributes
 src/lmql/ui/vscode/.gitignore
 src/lmql/ui/vscode/.vscodeignore
 src/lmql/ui/vscode/LICENSE
+src/lmql/ui/vscode/README.md
 src/lmql/ui/vscode/language-configuration.json
+src/lmql/ui/vscode/lmql-vscode.png
 src/lmql/ui/vscode/package.json
 src/lmql/ui/vscode/.vscode/launch.json
 src/lmql/ui/vscode/syntaxes/lmql.qstring.json
 src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
 src/lmql/ui/vscode/syntaxes/pylmql.json
 src/lmql/utils/__init__.py
 src/lmql/utils/graph.py
```

