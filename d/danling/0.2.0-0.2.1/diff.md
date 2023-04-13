# Comparing `tmp/danling-0.2.0.tar.gz` & `tmp/danling-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.2.0.tar", last modified: Tue Apr 11 13:46:07 2023, max compression
+gzip compressed data, was "danling-0.2.1.tar", last modified: Thu Apr 13 10:33:52 2023, max compression
```

## Comparing `danling-0.2.0.tar` & `danling-0.2.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.849398 danling-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-11 13:46:03.000000 danling-0.2.0/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-11 13:46:03.000000 danling-0.2.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 13:46:03.000000 danling-0.2.0/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-11 13:46:03.000000 danling-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-11 13:46:07.849398 danling-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-11 13:46:03.000000 danling-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-11 13:46:03.000000 danling-0.2.0/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-11 13:46:03.000000 danling-0.2.0/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 13:46:07.000000 danling-0.2.0/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 13:46:03.000000 danling-0.2.0/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-11 13:46:03.000000 danling-0.2.0/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-11 13:46:03.000000 danling-0.2.0/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 13:46:03.000000 danling-0.2.0/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 13:46:03.000000 danling-0.2.0/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-11 13:46:03.000000 danling-0.2.0/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-11 13:46:03.000000 danling-0.2.0/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/runner_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 13:46:03.000000 danling-0.2.0/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-11 13:46:03.000000 danling-0.2.0/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 13:46:03.000000 danling-0.2.0/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 13:46:03.000000 danling-0.2.0/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 13:46:03.000000 danling-0.2.0/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 13:46:03.000000 danling-0.2.0/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 13:46:03.000000 danling-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-11 13:46:03.000000 danling-0.2.0/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 13:46:03.000000 danling-0.2.0/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:46:03.000000 danling-0.2.0/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 13:46:03.000000 danling-0.2.0/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/runner_base.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-11 13:46:03.000000 danling-0.2.0/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 13:46:03.000000 danling-0.2.0/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 13:46:03.000000 danling-0.2.0/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 13:46:03.000000 danling-0.2.0/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 13:46:03.000000 danling-0.2.0/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 13:46:03.000000 danling-0.2.0/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 13:46:03.000000 danling-0.2.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.845398 danling-0.2.0/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.845398 danling-0.2.0/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.845398 danling-0.2.0/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 13:46:03.000000 danling-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 13:46:03.000000 danling-0.2.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 13:46:03.000000 danling-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:46:07.849398 danling-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:46:03.000000 danling-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.849398 danling-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-11 13:46:03.000000 danling-0.2.0/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.336945 danling-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 10:33:46.000000 danling-0.2.1/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 10:33:46.000000 danling-0.2.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-13 10:33:46.000000 danling-0.2.1/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-13 10:33:46.000000 danling-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 10:33:52.336945 danling-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-13 10:33:46.000000 danling-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-13 10:33:46.000000 danling-0.2.1/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-13 10:33:46.000000 danling-0.2.1/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 10:33:51.000000 danling-0.2.1/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 10:33:46.000000 danling-0.2.1/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-13 10:33:46.000000 danling-0.2.1/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-13 10:33:46.000000 danling-0.2.1/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:33:46.000000 danling-0.2.1/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:33:46.000000 danling-0.2.1/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-13 10:33:46.000000 danling-0.2.1/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-13 10:33:46.000000 danling-0.2.1/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 10:33:46.000000 danling-0.2.1/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-13 10:33:46.000000 danling-0.2.1/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 10:33:46.000000 danling-0.2.1/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:33:46.000000 danling-0.2.1/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 10:33:46.000000 danling-0.2.1/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 10:33:46.000000 danling-0.2.1/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-13 10:33:46.000000 danling-0.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 10:33:46.000000 danling-0.2.1/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 10:33:46.000000 danling-0.2.1/docs/metrics/average_meter.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:33:46.000000 danling-0.2.1/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:33:46.000000 danling-0.2.1/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:33:46.000000 danling-0.2.1/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:33:46.000000 danling-0.2.1/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 10:33:46.000000 danling-0.2.1/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:33:46.000000 danling-0.2.1/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:33:46.000000 danling-0.2.1/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:33:46.000000 danling-0.2.1/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-13 10:33:46.000000 danling-0.2.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.316945 danling-0.2.1/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 10:33:46.000000 danling-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 10:33:46.000000 danling-0.2.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:33:46.000000 danling-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:33:52.336945 danling-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:33:46.000000 danling-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-13 10:33:46.000000 danling-0.2.1/tests/test_runner.py
```

### Comparing `danling-0.2.0/.github/workflows/docs.yaml` & `danling-0.2.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/.github/workflows/push.yaml` & `danling-0.2.1/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/.gitignore` & `danling-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.Apache2` & `danling-0.2.1/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.BSD2` & `danling-0.2.1/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.BSD3` & `danling-0.2.1/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.BSD4` & `danling-0.2.1/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.GPL2` & `danling-0.2.1/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.GPL3` & `danling-0.2.1/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.MIT` & `danling-0.2.1/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/LICENSES/LICENSE.Unlicense` & `danling-0.2.1/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/PKG-INFO` & `danling-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.0
+Version: 0.2.1
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.0/README.md` & `danling-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/anaconda-project.yml` & `danling-0.2.1/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/__init__.py` & `danling-0.2.1/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/metrics/average_meter.py` & `danling-0.2.1/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/metrics/average_meters.py` & `danling-0.2.1/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/__init__.py` & `danling-0.2.1/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/mlp/dense.py` & `danling-0.2.1/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/mlp/mlp.py` & `danling-0.2.1/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/__init__.py` & `danling-0.2.1/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.1/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.1/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/decoder.py` & `danling-0.2.1/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/encoder.py` & `danling-0.2.1/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.1/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.1/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.2.1/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/registry.py` & `danling-0.2.1/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/runner/README.md` & `danling-0.2.1/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/runner/base_runner.py` & `danling-0.2.1/danling/runner/base_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     """
 
     # pylint: disable=R0902
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.init_distributed()
-        if self.seed is not None:
+        if self.state.seed is not None:
             self.set_seed()
-        if self.deterministic:
+        if self.state.deterministic:
             self.set_deterministic()
-        if self.log:
+        if self.state.log:
             self.init_logging()
         self.init_print()
-        if self.tensorboard:
+        if self.state.tensorboard:
             self.init_tensorboard()
 
     @on_main_process
     def init_logging(self) -> None:
         r"""
         Set up logging.
         """
@@ -64,15 +64,15 @@
                         "class": "logging.StreamHandler",
                         "stream": "ext://sys.stdout",
                     },
                     "logfile": {
                         "level": "DEBUG",
                         "formatter": "standard",
                         "class": "logging.FileHandler",
-                        "filename": self.log_path,
+                        "filename": self.state.log_path,
                         "mode": "a",
                     },
                 },
                 "loggers": {
                     "": {
                         "handlers": ["stdout", "logfile"],
                         "level": "DEBUG",
@@ -92,27 +92,27 @@
         Only print on a specific `process` or when `force = True`.
 
         Args:
             process: The process to `print` on.
 
         Notes
         -----
-        If `self.log = True`, the default `print` function will be override by `logging.info`.
+        If `self.state.log = True`, the default `print` function will be override by `logging.info`.
         """
 
         logger = logging.getLogger("print")
         logger.flush = lambda: [h.flush for h in logger.handlers]  # type: ignore
         import builtins as __builtin__  # pylint: disable=C0415
 
         builtin_print = __builtin__.print
 
         @catch
         def print(*args, force=False, end="\n", file=None, flush=False, **kwargs):  # pylint: disable=W0622
             if self.rank == process or force:
-                if self.log:
+                if self.state.log:
                     logger.info(*args, **kwargs)
                 else:
                     builtin_print(*args, end=end, file=file, flush=flush, **kwargs)
 
         __builtin__.print = print
 
     @on_main_process
@@ -124,27 +124,27 @@
 
     def set_seed(self, seed: Optional[int] = None, bias: Optional[int] = None) -> None:
         r"""
         Set up random seed.
 
         Args:
             seed: Random seed to set.
-                Defaults to `self.seed` (`config.seed`).
+                Defaults to `self.state.seed` (`config.seed`).
 
             bias: Make the seed different for each processes.
 
                 This avoids same data augmentation are applied on every processes.
 
                 Defaults to `self.rank`.
 
                 Set to `False` to disable this feature.
         """
 
         if seed is None:
-            seed = self.seed
+            seed = self.state.seed
         if bias is None:
             bias = self.rank
         if bias:
             seed += bias
         np.random.seed(seed)
         random.seed(seed)
 
@@ -180,87 +180,95 @@
                 RuntimeWarning,
             )
         lr = lr * lr_scale_factor  # pylint: disable=C0103, E1101
         lr_final = lr_final * lr_scale_factor  # pylint: disable=E1101
         self.lr_scale_factor = lr_scale_factor
         return lr, lr_final
 
-    def step(self, zero_grad: bool = True) -> None:
+    def step(self, zero_grad: bool = True, batch_size: Optional[int] = None) -> None:
         r"""
         Step optimizer and scheduler.
 
-        This method also increment the `self.steps` attribute.
+        This method increment `self.state.steps`.
+
+        This method also increment `self.state.iters` when `batch_size` is specified.
 
         Args:
             zero_grad: Whether to zero the gradients.
         """
 
         if self.optimizer is not None:
             self.optimizer.step()
             if zero_grad:
                 self.optimizer.zero_grad()
         if self.scheduler is not None:
             self.scheduler.step()
         self.state.steps += 1
+        if batch_size is not None:
+            self.state.iters += batch_size
         # TODO: Support `drop_last = False`
-        self.state.iters += self.batch_size_equivalent
+        # self.state.iters += self.batch_size_equivalent
 
     def state_dict(self, cls: Callable = dict) -> Mapping:
         r"""
         Return dict of all attributes for checkpoint.
         """
 
         raise NotImplementedError
 
     @catch
     @on_main_process
     def save_checkpoint(self) -> None:
         r"""
-        Save checkpoint to `runner.checkpoint_dir`.
+        Save checkpoint to `self.state.checkpoint_dir`.
 
-        The checkpoint will be saved to `runner.checkpoint_dir/latest.pth`.
+        The checkpoint will be saved to `self.state.checkpoint_dir/latest.pth`.
 
-        If `save_interval` is positive and `self.epochs + 1` is a multiple of `save_interval`,
-        the checkpoint will also be copied to `runner.checkpoint_dir/epoch-{self.epochs}.pth`.
+        If `self.state.save_interval` is positive and `self.state.epochs + 1` is a multiple of `save_interval`,
+        the checkpoint will also be copied to `self.state.checkpoint_dir/epoch-{self.state.epochs}.pth`.
 
-        If `self.is_best` is `True`, the checkpoint will also be copied to `runner.checkpoint_dir/best.pth`.
+        If `self.state.is_best` is `True`, the checkpoint will also be copied to `self.state.checkpoint_dir/best.pth`.
         """
 
-        latest_path = os.path.join(self.checkpoint_dir, "latest.pth")
+        latest_path = os.path.join(self.state.checkpoint_dir, "latest.pth")
         self.save(self.state_dict(), latest_path)
-        if hasattr(self, "save_interval") and self.save_interval > 0 and (self.epochs + 1) % self.save_interval == 0:
-            save_path = os.path.join(self.checkpoint_dir, f"epoch-{self.epochs}.pth")
+        if (
+            hasattr(self, "save_interval")
+            and self.save_interval > 0
+            and (self.state.epochs + 1) % self.save_interval == 0
+        ):
+            save_path = os.path.join(self.state.checkpoint_dir, f"epoch-{self.state.epochs}.pth")
             shutil.copy(latest_path, save_path)
         if self.is_best:
-            best_path = os.path.join(self.checkpoint_dir, "best.pth")
+            best_path = os.path.join(self.state.checkpoint_dir, "best.pth")
             shutil.copy(latest_path, best_path)
 
     def load_checkpoint(  # pylint: disable=W1113
         self, checkpoint: Optional[Union[Mapping, str]] = None, override_config: bool = True, *args, **kwargs
     ) -> None:
         """
         Load info from checkpoint.
 
         Args:
             checkpoint: Checkpoint (or its path) to load.
-                Defaults to `runner.checkpoint_dir/latest.pth`.
+                Defaults to `self.state.checkpoint_dir/latest.pth`.
             override_config: If True, override runner config with checkpoint config.
-            *args: Additional arguments to pass to `runner.load`.
-            **kwargs: Additional keyword arguments to pass to `runner.load`.
+            *args: Additional arguments to pass to `self.load`.
+            **kwargs: Additional keyword arguments to pass to `self.load`.
 
         Raises:
             FileNotFoundError: If `checkpoint` does not exists.
 
         See Also:
             [`from_checkpoint`][danling.BaseRunner.from_checkpoint]: Build runner from checkpoint.
             [`load_pretrained`][danling.BaseRunner.load_pretrained]: Load parameters from pretrained checkpoint.
         """
 
         if checkpoint is None:
-            checkpoint = os.path.join(self.checkpoint_dir, "latest.pth")  # type: ignore
+            checkpoint = os.path.join(self.state.checkpoint_dir, "latest.pth")  # type: ignore
         # TODO: Support loading checkpoints in other format
         if isinstance(checkpoint, str):
             if not os.path.exists(checkpoint):
                 raise FileNotFoundError(f"checkpoint is set to {checkpoint} but does not exist.")
             self.checkpoint = checkpoint  # pylint: disable=W0201
             checkpoint: Mapping = self.load(checkpoint, *args, **kwargs)  # type: ignore
         # TODO: Wrap state_dict in a dataclass
@@ -275,16 +283,16 @@
 
     def load_pretrained(self, checkpoint: Union[Mapping, str], *args, **kwargs) -> None:
         """
         Load parameters from pretrained checkpoint.
 
         Args:
             checkpoint: Pretrained checkpoint (or its path) to load.
-            *args: Additional arguments to pass to `runner.load`.
-            **kwargs: Additional keyword arguments to pass to `runner.load`.
+            *args: Additional arguments to pass to `self.load`.
+            **kwargs: Additional keyword arguments to pass to `self.load`.
 
         Raises:
             FileNotFoundError: If `checkpoint` does not exists.
 
         See Also:
             [`load_checkpoint`][danling.BaseRunner.load_checkpoint]: Load info from checkpoint.
         """
@@ -303,63 +311,63 @@
     @classmethod
     def from_checkpoint(cls, checkpoint: Union[Mapping, str], *args, **kwargs) -> BaseRunner:
         r"""
         Build BaseRunner from checkpoint.
 
         Args:
             checkpoint: Checkpoint (or its path) to load.
-                Defaults to `runner.checkpoint_dir/latest.pth`.
-            *args: Additional arguments to pass to `runner.load`.
-            **kwargs: Additional keyword arguments to pass to `runner.load`.
+                Defaults to `self.state.checkpoint_dir/latest.pth`.
+            *args: Additional arguments to pass to `self.load`.
+            **kwargs: Additional keyword arguments to pass to `self.load`.
 
         Returns:
             (BaseRunner):
         """
 
         if isinstance(checkpoint, str):
             checkpoint = cls.load(checkpoint, *args, **kwargs)
         runner = cls(**checkpoint["runner"])  # type: ignore
         runner.load_checkpoint(checkpoint, override_config=False)
         return runner
 
     def append_result(self, result) -> None:
         r"""
-        Append result to `self.results`.
+        Append result to `self.state.results`.
 
         Warnings:
-            `self.results` is heavily relied upon for computing metrics.
+            `self.state.results` is heavily relied upon for computing metrics.
 
             Failed to use this method may lead to unexpected behavior.
         """
 
-        self.results.append(result)
+        self.state.results.append(result)
 
     def print_result(self) -> None:
         r"""
         Print latest and best result.
         """
 
-        print(f"results: {self.results}")
-        print(f"latest result: {self.latest_result}")
-        print(f"best result: {self.best_result}")
+        print(f"results: {self.state.results}")
+        print(f"latest result: {self.state.latest_result}")
+        print(f"best result: {self.state.best_result}")
 
     @catch
     @on_main_process
     def save_result(self) -> None:
         r"""
-        Save result to `runner.dir`.
+        Save result to `self.state.dir`.
 
         This method will save latest and best result to
-        `runner.dir/latest.json` and `runner.dir/best.json` respectively.
+        `self.state.dir/latest.json` and `self.state.dir/best.json` respectively.
         """
 
-        results_path = os.path.join(self.dir, "results.json")
-        self.save({"id": self.id, "name": self.name, "results": self.results}, results_path, indent=4)
-        ret = {"id": self.id, "name": self.name}
-        result = self.latest_result  # type: ignore
+        results_path = os.path.join(self.state.dir, "results.json")
+        self.save({"id": self.state.id, "name": self.state.name, "results": self.state.results}, results_path, indent=4)
+        ret = {"id": self.state.id, "name": self.state.name}
+        result = self.state.latest_result  # type: ignore
         if isinstance(result, FlatDict):
             result = result.dict()  # type: ignore
         # This is slower but ensure id is the first key
         if result is not None:
             ret.update(result)  # type: ignore
         latest_path = os.path.join(self.dir, "latest.json")
         self.save(ret, latest_path, indent=4)
```

### Comparing `danling-0.2.0/danling/runner/runner_base.py` & `danling-0.2.1/danling/runner/runner_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,18 @@
             If `train` is in `dataloaders`, then `batch_size` is the batch size of `train`.
             Otherwise, `batch_size` is the batch size of the first dataloader.
 
         Returns:
             (int):
         """
 
-        loader = self.dataloaders["train"] if "train" in self.dataloaders else next(iter(self.dataloaders.values()))
-        return loader.batch_size
+        if self.dataloaders:
+            loader = self.dataloaders["train"] if "train" in self.dataloaders else next(iter(self.dataloaders.values()))
+            return loader.batch_size
+        raise AttributeError("batch_size could not be inferred, since no dataloaedr found.")
 
     @property
     def batch_size_equivalent(self) -> int:
         r"""
         Actual batch size.
 
         Returns:
```

### Comparing `danling-0.2.0/danling/runner/runner_state.py` & `danling-0.2.1/danling/runner/runner_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 from datetime import datetime
 from random import randint
 from typing import IO, Callable, List, Optional, Union
 from uuid import UUID, uuid5
 from warnings import warn
 
 from chanfig import NestedDict
-from git.exc import InvalidGitRepositoryError
-from git.repo import Repo
+
+try:
+    from git.exc import InvalidGitRepositoryError
+    from git.repo import Repo
+except ImportError:
+    warn("gitpython not installed, git hash will not be available")
+    Repo = None
 
 from danling.utils import base62, ensure_dir
 
 PathStr = Union[os.PathLike, str, bytes]
 File = Union[PathStr, IO]
 
 DEFAULT_EXPERIMENT_NAME = "DanLing"
@@ -123,14 +128,18 @@
     In practice, `checkpoint_dir_name` is rarely called.
 
     Attributes: logging:
         log (bool): Whether to log the outputs.
             Defaults to `True`.
         tensorboard (bool): Whether to use `tensorboard`.
             Defaults to `False`.
+        print_interval (int): Interval of printing logs.
+            Defaults to -1.
+        save_interval (int): Interval of saving intermediate checkpoints.
+            Defaults to -1, never save intermediate checkpoints.
 
     Notes:
         `RunnerState` is a `NestedDict`, so you can access its attributes by `state["name"]` or `state.name`.
 
     See Also:
         [`RunnerBase`][danling.runner.runner_base.RunnerBase]: The runeer state that stores critical information.
         [`BaseRunner`][danling.runner.BaseRunner]: The base runner class.
@@ -163,22 +172,27 @@
     index_set: Optional[str]
     index: str
 
     project_root: str = "experiments"
     checkpoint_dir_name: str = "checkpoints"
     log: bool = True
     tensorboard: bool = False
+    print_interval: int = -1
+    save_interval: int = -1
 
     def __init__(self, *args, **kwargs):
-        try:
-            self.experiment_id = Repo(search_parent_directories=True).head.object.hexsha
-        except ImportError:
+        if Repo is not None:
+            try:
+                self.experiment_id = Repo(search_parent_directories=True).head.object.hexsha
+            except ImportError:
+                warn("GitPython is not installed, using default experiment id.")
+            except InvalidGitRepositoryError:
+                warn("Git reporitory is invalid, using default experiment id.")
+        else:
             warn("GitPython is not installed, using default experiment id.")
-        except InvalidGitRepositoryError:
-            warn("Git reporitory is invalid, using default experiment id.")
         self.deterministic = False
         self.seed = randint(0, 2**32 - 1)
         self.iters = 0
         self.steps = 0
         self.epochs = 0
         self.results = []
         self.index_set = None
```

### Comparing `danling-0.2.0/danling/runner/torch_runner.py` & `danling-0.2.1/danling/runner/torch_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,23 @@
         accelerate: Defaults to `{}`.
             if is `None`, will not use `accelerate`.
     """
 
     # pylint: disable=R0902
 
     accelerator: Accelerator = None  # type: ignore
-    accelerate: Mapping[str, Any] = None  # type: ignore
+    accelerate: Mapping[str, Any]
+
+    def __init__(self, *args, **kwargs) -> None:
+        self.accelerate = {}
+        if len(args) == 1 and isinstance(args[0], dict):
+            self.accelerate.update(args[0].pop("accelerate", {}))
+        if "accelerate" in kwargs:
+            self.accelerate.update(kwargs.pop("accelerate"))
+        super().__init__(*args, **kwargs)
 
     def init_distributed(self) -> None:
         r"""
         Set up distributed training.
 
         Initialise process group and set up DDP variables.
         """
@@ -60,27 +68,27 @@
 
     def set_seed(self, seed: int = None, bias: Optional[int] = None) -> None:  # type: ignore
         r"""
         Set up random seed.
 
         Args:
             seed: Random seed to set.
-                Defaults to `self.seed` (`config.seed`).
+                Defaults to `self.state.seed` (`config.seed`).
 
             bias: Make the seed different for each processes.
 
                 This avoids same data augmentation are applied on every processes.
 
                 Defaults to `self.rank`.
 
                 Set to `False` to disable this feature.
         """
 
         if seed is None:
-            seed = self.seed
+            seed = self.state.seed
         if self.distributed:
             object_list = [seed]
             dist.broadcast_object_list(object_list)
             seed = object_list[0]
         if bias is None:
             bias = self.rank
         if bias:
@@ -164,17 +172,19 @@
             If `train` is in `dataloaders`, then `batch_size` is the batch size of `train`.
             Otherwise, `batch_size` is the batch size of the first dataloader.
 
         Returns:
             (int):
         """
 
-        loader = self.dataloaders["train"] if "train" in self.dataloaders else next(iter(self.dataloaders.values()))
-        batch_sampler = loader.sampler if isinstance(loader.sampler, BatchSampler) else loader.batch_sampler
-        return batch_sampler.batch_size
+        if self.dataloaders:
+            loader = self.dataloaders["train"] if "train" in self.dataloaders else next(iter(self.dataloaders.values()))
+            batch_sampler = loader.sampler if isinstance(loader.sampler, BatchSampler) else loader.batch_sampler
+            return batch_sampler.batch_size
+        raise AttributeError("batch_size could not be inferred, since no dataloaedr found.")
 
     @property
     def accum_steps(self) -> int:
         r"""
         Gradient accumulation steps.
 
         Returns:
```

### Comparing `danling-0.2.0/danling/runner/utils.py` & `danling-0.2.1/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/tensors/nested_tensor.py` & `danling-0.2.1/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/tensors/torch_func_registry.py` & `danling-0.2.1/danling/tensors/torch_func_registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/utils/basex.py` & `danling-0.2.1/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/utils/decorators.py` & `danling-0.2.1/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling/utils/io.py` & `danling-0.2.1/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/danling.egg-info/PKG-INFO` & `danling-0.2.1/danling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.0
+Version: 0.2.1
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.0/danling.egg-info/SOURCES.txt` & `danling-0.2.1/danling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/mkdocs.yml` & `danling-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.1/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.1/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.1/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.1/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/assets/images/favicon.ico` & `danling-0.2.1/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/assets/images/logo.png` & `danling-0.2.1/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/overrides/main.html` & `danling-0.2.1/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/pyproject.toml` & `danling-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.2.0/tests/test_runner.py` & `danling-0.2.1/tests/test_runner.py`

 * *Files identical despite different names*

