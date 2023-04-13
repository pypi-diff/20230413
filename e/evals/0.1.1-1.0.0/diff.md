# Comparing `tmp/evals-0.1.1.tar.gz` & `tmp/evals-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-0.1.1.tar", last modified: Tue Mar 14 15:50:32 2023, max compression
+gzip compressed data, was "evals-1.0.0.tar", last modified: Wed Apr 12 23:44:06 2023, max compression
```

## Comparing `evals-0.1.1.tar` & `evals-1.0.0.tar`

### file list

```diff
@@ -1,61 +1,505 @@
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.440159 evals-0.1.1/
--rw-r--r--   0 marvin     (502) staff       (20)     1063 2023-03-14 15:34:49.000000 evals-0.1.1/LICENSE
--rw-r--r--   0 marvin     (502) staff       (20)       90 2023-03-14 15:34:49.000000 evals-0.1.1/MANIFEST.in
--rw-r--r--   0 marvin     (502) staff       (20)       94 2023-03-14 15:50:32.439821 evals-0.1.1/PKG-INFO
--rw-r--r--   0 marvin     (502) staff       (20)     5029 2023-03-14 15:34:49.000000 evals-0.1.1/README.md
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.380931 evals-0.1.1/evals/
--rw-r--r--   0 marvin     (502) staff       (20)      217 2023-03-14 15:34:49.000000 evals-0.1.1/evals/__init__.py
--rw-r--r--   0 marvin     (502) staff       (20)     8435 2023-03-14 15:34:49.000000 evals-0.1.1/evals/api.py
--rw-r--r--   0 marvin     (502) staff       (20)     3985 2023-03-14 15:34:49.000000 evals-0.1.1/evals/base.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.389399 evals-0.1.1/evals/cli/
--rw-r--r--   0 marvin     (502) staff       (20)     7768 2023-03-14 15:34:49.000000 evals-0.1.1/evals/cli/oaieval.py
--rw-r--r--   0 marvin     (502) staff       (20)     3060 2023-03-14 15:34:49.000000 evals-0.1.1/evals/cli/oaievalset.py
--rw-r--r--   0 marvin     (502) staff       (20)     6318 2023-03-14 15:34:49.000000 evals-0.1.1/evals/data.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.394490 evals-0.1.1/evals/elsuite/
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.400681 evals-0.1.1/evals/elsuite/basic/
--rw-r--r--   0 marvin     (502) staff       (20)     1544 2023-03-14 15:34:49.000000 evals-0.1.1/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 marvin     (502) staff       (20)     1085 2023-03-14 15:34:49.000000 evals-0.1.1/evals/elsuite/basic/includes.py
--rw-r--r--   0 marvin     (502) staff       (20)     1516 2023-03-14 15:34:49.000000 evals-0.1.1/evals/elsuite/basic/match.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.403376 evals-0.1.1/evals/elsuite/modelgraded/
--rw-r--r--   0 marvin     (502) staff       (20)    14214 2023-03-14 15:34:49.000000 evals-0.1.1/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 marvin     (502) staff       (20)     2504 2023-03-14 15:34:49.000000 evals-0.1.1/evals/elsuite/translate.py
--rw-r--r--   0 marvin     (502) staff       (20)     4706 2023-03-14 15:34:49.000000 evals-0.1.1/evals/elsuite/utils.py
--rw-r--r--   0 marvin     (502) staff       (20)     4703 2023-03-14 15:34:49.000000 evals-0.1.1/evals/eval.py
--rw-r--r--   0 marvin     (502) staff       (20)     1137 2023-03-14 15:34:49.000000 evals-0.1.1/evals/formatting.py
--rw-r--r--   0 marvin     (502) staff       (20)     2455 2023-03-14 15:34:49.000000 evals-0.1.1/evals/metrics.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.405958 evals-0.1.1/evals/prompt/
--rw-r--r--   0 marvin     (502) staff       (20)     4182 2023-03-14 15:34:49.000000 evals-0.1.1/evals/prompt/base.py
--rw-r--r--   0 marvin     (502) staff       (20)    17028 2023-03-14 15:34:49.000000 evals-0.1.1/evals/record.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.353278 evals-0.1.1/evals/registry/
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.412439 evals-0.1.1/evals/registry/eval_sets/
--rw-r--r--   0 marvin     (502) staff       (20)       71 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      352 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 marvin     (502) staff       (20)       81 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      312 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.420027 evals-0.1.1/evals/registry/evals/
--rw-r--r--   0 marvin     (502) staff       (20)      897 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      247 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/evals/logic.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      881 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 marvin     (502) staff       (20)     1292 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 marvin     (502) staff       (20)     2976 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/evals/test-modelgraded.yaml
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.430459 evals-0.1.1/evals/registry/modelgraded/
--rw-r--r--   0 marvin     (502) staff       (20)      445 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 marvin     (502) staff       (20)     1010 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      237 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 marvin     (502) staff       (20)     1109 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      193 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 marvin     (502) staff       (20)      202 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry/modelgraded/humor_likert.yaml
--rw-r--r--   0 marvin     (502) staff       (20)     5409 2023-03-14 15:34:49.000000 evals-0.1.1/evals/registry.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.439296 evals-0.1.1/evals/utils/
--rw-r--r--   0 marvin     (502) staff       (20)     1505 2023-03-14 15:34:49.000000 evals-0.1.1/evals/utils/api_utils.py
--rw-r--r--   0 marvin     (502) staff       (20)      713 2023-03-14 15:34:49.000000 evals-0.1.1/evals/utils/misc.py
--rw-r--r--   0 marvin     (502) staff       (20)     3991 2023-03-14 15:34:49.000000 evals-0.1.1/evals/utils/snowflake.py
-drwxr-xr-x   0 marvin     (502) staff       (20)        0 2023-03-14 15:50:32.383968 evals-0.1.1/evals.egg-info/
--rw-r--r--   0 marvin     (502) staff       (20)       94 2023-03-14 15:50:32.000000 evals-0.1.1/evals.egg-info/PKG-INFO
--rw-r--r--   0 marvin     (502) staff       (20)     1287 2023-03-14 15:50:32.000000 evals-0.1.1/evals.egg-info/SOURCES.txt
--rw-r--r--   0 marvin     (502) staff       (20)        1 2023-03-14 15:50:32.000000 evals-0.1.1/evals.egg-info/dependency_links.txt
--rw-r--r--   0 marvin     (502) staff       (20)       90 2023-03-14 15:50:32.000000 evals-0.1.1/evals.egg-info/entry_points.txt
--rw-r--r--   0 marvin     (502) staff       (20)      184 2023-03-14 15:50:32.000000 evals-0.1.1/evals.egg-info/requires.txt
--rw-r--r--   0 marvin     (502) staff       (20)        6 2023-03-14 15:50:32.000000 evals-0.1.1/evals.egg-info/top_level.txt
--rw-r--r--   0 marvin     (502) staff       (20)      514 2023-03-14 15:34:49.000000 evals-0.1.1/pyproject.toml
--rw-r--r--   0 marvin     (502) staff       (20)       38 2023-03-14 15:50:32.440230 evals-0.1.1/setup.cfg
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:06.136079 evals-1.0.0/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1063 2023-03-18 03:40:27.000000 evals-1.0.0/LICENSE
+-rw-r--r--   0 kondrich   (502) staff       (20)      136 2023-04-12 23:41:29.000000 evals-1.0.0/MANIFEST.in
+-rw-r--r--   0 kondrich   (502) staff       (20)       94 2023-04-12 23:44:06.135526 evals-1.0.0/PKG-INFO
+-rw-r--r--   0 kondrich   (502) staff       (20)     5239 2023-04-11 16:48:30.000000 evals-1.0.0/README.md
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.664395 evals-1.0.0/evals/
+-rw-r--r--   0 kondrich   (502) staff       (20)      316 2023-04-11 16:48:30.000000 evals-1.0.0/evals/__init__.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2964 2023-04-11 16:48:30.000000 evals-1.0.0/evals/api.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1900 2023-04-11 16:48:30.000000 evals-1.0.0/evals/base.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.669237 evals-1.0.0/evals/cli/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.628534 evals-1.0.0/evals/cli/content/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.628713 evals-1.0.0/evals/cli/content/evallogs/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.629944 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:04.103409 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/
+-rw-r--r--   0 kondrich   (502) staff       (20)   160001 2023-03-20 22:58:43.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/aba_mrpc_true_false.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   961478 2023-03-20 23:01:34.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/actors-sequence.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    98646 2023-03-20 23:01:04.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/advice-multi-type-categorization.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    62020 2023-03-20 22:48:28.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/base64-decode.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   100496 2023-03-20 22:53:59.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/bigrams.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1004 2023-03-20 22:55:26.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/bubble-sort.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      993 2023-03-20 22:58:39.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/chess-match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   136290 2023-03-20 22:50:19.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/complex-replace-characters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1105 2023-03-20 22:54:54.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/compute-max-node-degree.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   186641 2023-03-20 23:02:24.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/convert-hex-hsl-lightness.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    99654 2023-03-20 22:48:16.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/fibonacci-letter-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    76773 2023-03-20 22:49:42.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/first-letters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    89863 2023-03-20 23:00:22.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/general-knowledge.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    95505 2023-03-20 22:48:10.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/generate-json.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    53761 2023-03-20 22:49:44.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/identify-capitals.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1144 2023-03-20 22:57:00.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/imperative-extraction.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   915534 2023-03-20 22:59:48.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/index_list.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   186040 2023-03-20 22:57:22.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/infiniteloop-match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   105375 2023-03-20 22:48:44.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/int-addition.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    46622 2023-03-20 22:47:46.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/integer-multiplication.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   147085 2023-03-20 22:48:19.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/invoices.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   184068 2023-03-20 22:49:40.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/knights-and-knaves.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    84221 2023-03-20 22:49:57.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/largest_country.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    69229 2023-03-20 22:48:27.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/last-word-nth.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   168412 2023-03-20 22:49:04.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/lat_long_identify.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    93555 2023-03-20 22:55:18.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/letter-count-logic.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    72136 2023-03-20 22:48:30.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/letter-counting.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   104392 2023-03-20 22:49:39.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/linear-equations.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    22866 2023-03-20 22:48:59.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/lisp-paren-check.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   106312 2023-03-20 22:58:26.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/logic-derive-sentences.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    70469 2023-03-20 22:48:18.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/logic-statements.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    83123 2023-03-20 22:54:52.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/mass-weight-conversion.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    66122 2023-03-20 22:49:59.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/next-val-series.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   101380 2023-03-20 22:49:42.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/number-pattern.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   544596 2023-03-20 23:00:50.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/ordered-history-events.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    98448 2023-03-20 22:49:13.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/palindromic-substring.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1147 2023-03-20 22:58:05.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/partially_solved_crossword_clues.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1039 2023-03-20 22:55:06.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/points-on-line.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    79891 2023-03-20 22:48:19.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/population-standard-deviation.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    76022 2023-03-20 23:01:33.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/prime-number.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   103585 2023-03-20 22:50:27.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/probability-questions.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)  1635378 2023-03-20 22:48:17.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/qa.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   177896 2023-03-20 22:59:21.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/quadratic-from-three-points.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      965 2023-03-20 22:59:35.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/quotes.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    56982 2023-03-20 23:01:45.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/recursive-functions.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   309312 2023-03-20 22:54:18.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/relative-dates.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1031 2023-03-20 22:54:57.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/repeat-vowels.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1039 2023-03-20 22:49:07.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/reverse-string.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    88645 2023-03-20 22:48:07.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/rewrite-second-letter-capital.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   106765 2023-03-20 22:52:17.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/rocstory.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    71327 2023-03-20 23:02:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/rot13.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1030 2023-03-20 22:57:35.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/rucola.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1022 2023-03-20 22:48:04.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/russe.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1042 2023-03-20 22:55:02.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/russian-nlp-tasks.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   303395 2023-03-20 22:59:20.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/search-paper.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   124062 2023-03-20 22:50:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/sexagenary_cycle_calculation.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    70902 2023-03-20 23:01:28.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/slope_intercept.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    80559 2023-03-20 22:49:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/sort-numbers.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   135242 2023-03-20 23:03:31.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/stock-options.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   164438 2023-03-20 22:54:31.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/substitution-cipher.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   121120 2023-03-20 22:49:14.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/sudoku-solver.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    74936 2023-03-20 22:50:14.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/swap-neighboring-characters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    97545 2023-03-20 22:58:01.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/swap-words.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    80414 2023-03-20 23:02:58.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/test-match-string-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   111993 2023-03-20 22:48:17.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/test-match-unsigned-number.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    63123 2023-03-20 22:48:56.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/unix_timestamp.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    62465 2023-03-20 23:02:00.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-3.5-turbo/word-count.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:04.817311 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/
+-rw-r--r--   0 kondrich   (502) staff       (20)    66277 2023-03-20 23:03:31.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/aba_mrpc_true_false.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   325313 2023-03-20 23:00:08.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/actors-sequence.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1173 2023-03-20 22:55:26.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/advice-multi-type-categorization.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    81769 2023-03-20 23:01:16.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/base64-decode.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    54075 2023-03-20 22:53:39.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/bigrams.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      956 2023-03-20 22:59:54.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/bubble-sort.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      945 2023-03-20 23:00:12.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/chess-match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    92539 2023-03-20 22:53:40.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/complex-replace-characters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1057 2023-03-20 22:57:48.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/compute-max-node-degree.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    95433 2023-03-20 23:02:10.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/convert-hex-hsl-lightness.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   147088 2023-03-20 22:55:00.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/fibonacci-letter-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    53094 2023-03-20 22:52:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/first-letters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    47088 2023-03-20 23:03:13.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/general-knowledge.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   186669 2023-03-20 22:58:00.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/generate-json.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    36478 2023-03-20 22:51:44.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/identify-capitals.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1096 2023-03-20 23:00:55.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/imperative-extraction.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      948 2023-03-20 22:53:00.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/index_list.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    71960 2023-03-20 22:59:56.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/infiniteloop-match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   123538 2023-03-20 22:54:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/int-addition.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    44966 2023-03-20 22:48:00.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/integer-multiplication.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   159857 2023-03-20 22:56:47.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/invoices.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   308910 2023-03-20 23:01:15.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/knights-and-knaves.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    90001 2023-03-20 22:57:51.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/largest_country.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    92154 2023-03-20 23:01:50.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/last-word-nth.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   131573 2023-03-20 22:49:47.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/lat_long_identify.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    54561 2023-03-20 22:59:41.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/letter-count-logic.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    48581 2023-03-20 22:49:11.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/letter-counting.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    74720 2023-03-20 22:51:45.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/linear-equations.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    20693 2023-03-20 22:58:04.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/lisp-paren-check.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1113 2023-03-20 22:54:18.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/logic-derive-sentences.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    45499 2023-03-20 22:53:10.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/logic-statements.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    45212 2023-03-20 22:59:35.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/mass-weight-conversion.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    91129 2023-03-20 23:02:22.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/next-val-series.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    67035 2023-03-20 22:51:49.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/number-pattern.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   195291 2023-03-20 22:57:38.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/ordered-history-events.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    72076 2023-03-20 22:51:14.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/palindromic-substring.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1099 2023-03-20 23:02:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/partially_solved_crossword_clues.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      991 2023-03-20 22:57:51.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/points-on-line.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   110266 2023-03-20 22:53:59.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/population-standard-deviation.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      959 2023-03-20 22:53:59.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/prime-number.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    71496 2023-03-20 22:53:23.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/probability-questions.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)  2456997 2023-03-20 22:52:30.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/qa.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   149142 2023-03-20 22:54:38.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/quadratic-from-three-points.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      917 2023-03-20 23:01:14.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/quotes.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     1031 2023-03-20 22:55:03.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/recursive-functions.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   179288 2023-03-20 22:53:20.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/relative-dates.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      983 2023-03-20 22:58:43.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/repeat-vowels.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   248942 2023-03-20 23:03:26.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/reverse-string.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   114874 2023-03-20 22:53:25.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/rewrite-second-letter-capital.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   129055 2023-03-20 22:58:37.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/rocstory.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      919 2023-03-20 22:59:08.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/rot13.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      982 2023-03-20 23:00:36.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/rucola.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   184168 2023-03-20 23:01:44.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/russe.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      994 2023-03-20 22:56:10.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/russian-nlp-tasks.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   107011 2023-03-20 22:58:57.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/search-paper.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   161687 2023-03-20 22:53:38.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/sexagenary_cycle_calculation.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      980 2023-03-20 22:54:12.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/slope_intercept.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   102084 2023-03-20 22:58:58.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/sort-numbers.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    67680 2023-03-20 23:01:39.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/stock-options.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   182186 2023-03-20 23:02:23.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/substitution-cipher.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   136125 2023-03-20 22:57:34.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/sudoku-solver.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    49350 2023-03-20 22:52:51.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/swap-neighboring-characters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    48769 2023-03-20 22:59:07.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/swap-words.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    43691 2023-03-20 22:57:48.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/test-match-string-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   122863 2023-03-20 22:54:22.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/test-match-unsigned-number.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    35361 2023-03-20 22:53:05.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/unix_timestamp.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    37471 2023-03-20 23:01:32.000000 evals-1.0.0/evals/cli/content/evallogs/2023-03-20_22-45/gpt-4/word-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5645 2023-04-11 16:48:30.000000 evals-1.0.0/evals/cli/oaieval.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     3294 2023-03-28 05:28:29.000000 evals-1.0.0/evals/cli/oaievalset.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.631094 evals-1.0.0/evals/cli/tmp/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.459765 evals-1.0.0/evals/cli/tmp/evallogs/
+-rw-r--r--   0 kondrich   (502) staff       (20)    23661 2023-03-19 18:06:56.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319180651FVXPXVXP_gpt-4_infiniteloop-match.s1.simple-v0.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    29813 2023-03-19 18:07:00.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191806582H2AI7HQ_gpt-4_russe.test.v0.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    21758 2023-03-19 18:07:07.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319180701L6S4VAAX_gpt-4_slope_intercept.dev.v0.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      945 2023-03-19 18:07:09.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319180709LSOLXOCO_gpt-4_counting.dev.v0.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    23648 2023-03-19 18:25:10.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182508GWUO4EFH_gpt-4_infiniteloop-match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    29805 2023-03-19 18:25:17.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182512IZZRD77S_gpt-4_russe.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    21755 2023-03-19 18:25:22.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182519WUDMDTIG_gpt-4_slope_intercept.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      938 2023-03-19 18:25:24.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182524K75HYGM5_gpt-4_counting.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    18814 2023-03-19 18:25:31.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182526ZLLJIBC2_gpt-4_fr-paraphrase-detection.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    18476 2023-03-19 18:25:35.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191825327OQLXUYG_gpt-4_mnemonic.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    24095 2023-03-19 18:26:04.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182537NHCP5GSA_gpt-4_biomolecules.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    35222 2023-03-19 18:26:34.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182606N7YN2K7W_gpt-4_knights-and-knaves.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16453 2023-03-19 18:26:39.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182635LBR7GITU_gpt-4_bigrams.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    15705 2023-03-19 18:26:44.000000 evals-1.0.0/evals/cli/tmp/evallogs/23031918264037CUQYB6_gpt-4_swap-words.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    12798 2023-03-19 18:26:47.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191826464XJ5QR7R_gpt-4_regex-match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    14176 2023-03-19 18:26:54.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182649OI5WJVTH_gpt-4_logical_counting.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     4700 2023-03-19 18:26:57.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182656MMUR4KCT_gpt-4_lisp-paren-check.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    60857 2023-03-19 18:31:11.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319182659BTA6DYON_gpt-4_advice-multi-type-categorization.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    28648 2023-03-19 18:31:17.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183113W4U4NWOJ_gpt-4_convert-hex-hsl-lightness.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    78882 2023-03-19 18:31:23.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183118ILTFI554_gpt-4_us-tort-law.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5200 2023-03-19 18:31:25.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191831257X23MAMJ_gpt-4_positive-binary-operations.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    20353 2023-03-19 18:31:31.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183127IAMXWANO_gpt-4_palindromic-substring.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16699 2023-03-19 18:31:42.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183132MCQ3MMGY_gpt-4_repeat-vowels.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   258450 2023-03-19 18:31:45.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191831443PGE2LHJ_gpt-4_quality.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    17592 2023-03-19 18:31:55.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191831502WC3AU7P_gpt-4_recursive-functions.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    28486 2023-03-19 18:31:59.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191831562LDJPFOP_gpt-4_rucola.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    17038 2023-03-19 18:32:16.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183200KMP5JFEY_gpt-4_unix_timestamp.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    28439 2023-03-19 18:32:27.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183218ZWZJL55Q_gpt-4_complex-replace-characters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    27659 2023-03-19 18:32:40.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183229CO3WZW6M_gpt-4_actors-sequence.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    18209 2023-03-19 18:32:47.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183241I4C3RIZA_gpt-4_substitution-cipher.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    17919 2023-03-19 18:32:50.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183249NLF77YCA_gpt-4_largest_country.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    15045 2023-03-19 18:32:54.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183252ZPUDOPZB_gpt-4_letter-counting.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    26582 2023-03-19 18:33:42.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191832567V65MRIJ_gpt-4_quadratic-from-three-points.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    15667 2023-03-19 18:33:51.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183344ZEQ7FGSU_gpt-4_swap-neighboring-characters.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    87817 2023-03-19 18:34:48.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191833527IL4RX5R_gpt-4_imperative-extraction.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    50683 2023-03-19 18:34:55.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183449FJUHU2YB_gpt-4_relative-dates.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    38337 2023-03-19 18:35:00.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183457C5XM62JK_gpt-4_invoices.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    14506 2023-03-19 18:35:12.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183502CDR3I7VI_gpt-4_test-match-string-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16313 2023-03-19 18:35:17.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191835144T5SQAZI_gpt-4_population-standard-deviation.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    18891 2023-03-19 18:35:26.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191835184XJRYMLW_gpt-4_rewrite-second-letter-capital.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    21373 2023-03-19 18:35:30.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183527GF4MO3L7_gpt-4_linear-equations.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    58963 2023-03-19 18:36:07.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183532BXCOWS7B_gpt-4_ordered-history-events.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    36285 2023-03-19 18:36:44.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183609YZKJFKTU_gpt-4_jee-math.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    19201 2023-03-19 18:36:53.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183646PF6GZF67_gpt-4_number-pattern.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    34620 2023-03-19 18:36:56.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183654POKL72IP_gpt-4_lat_long_identify.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    12817 2023-03-19 18:37:04.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183658CMYAKVVZ_gpt-4_base64-decode.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    31011 2023-03-19 18:37:08.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191837056VNCOZ2R_gpt-4_compute-max-node-degree.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   327587 2023-03-19 18:37:12.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191837107NF455X4_gpt-4_qa.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    21067 2023-03-19 18:37:17.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183714MCZHAX5A_gpt-4_russian-nlp-tasks.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    20013 2023-03-19 18:37:24.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183719JXKJKBKC_gpt-4_crepe.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5236 2023-03-19 18:37:26.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183726XLYALPGE_gpt-4_indices.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    20973 2023-03-19 18:37:34.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183728AZRV45WY_gpt-4_rocstory.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    46675 2023-03-19 18:37:50.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183736FHC4OXGV_gpt-4_event-categories.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    21399 2023-03-19 18:37:58.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183752VU6DVQES_gpt-4_points-on-line.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    15934 2023-03-19 18:38:10.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183807DRBTRW5K_gpt-4_multiplication_evaluation.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     9774 2023-03-19 18:38:16.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191838126IRGK2BU_gpt-4_integer-multiplication.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    12794 2023-03-19 18:38:23.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191838184NYHGGGB_gpt-4_binary_count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    47549 2023-03-19 18:44:08.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319183825PTQZYJNU_gpt-4_sort-alphabetically.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    13155 2023-03-19 18:44:12.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184410TCYPKM3X_gpt-4_python-docstring.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    25897 2023-03-19 18:44:18.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184414YTBKZG5I_gpt-4_decrypt-caesar-cipher.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     7253 2023-03-19 18:44:22.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184419X7JBCI7I_gpt-4_generate-json.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16062 2023-03-19 18:44:29.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184423OJ6KBYCX_gpt-4_imperial_date_to_string.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    20350 2023-03-19 18:44:34.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184431NARDZMPK_gpt-4_anagrams.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    20653 2023-03-19 18:44:38.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184436V7FHN7ZJ_gpt-4_fibonacci-letter-count.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    45652 2023-03-19 18:44:42.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191844403TULQHLH_gpt-4_diagrammatic_logic.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    29897 2023-03-19 18:45:19.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191844443TCGPCE2_gpt-4_bubble-sort.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    14448 2023-03-19 18:45:25.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184521DV46APYE_gpt-4_last-word-nth.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    17170 2023-03-19 18:45:30.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184526LQ64DWXK_gpt-4_letter-count-logic.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    21534 2023-03-19 18:45:41.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184532CBJE4BVH_gpt-4_sudoku-solver.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    14865 2023-03-19 18:45:47.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184543PQQ4PPHA_gpt-4_general-knowledge.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    12099 2023-03-19 18:45:52.000000 evals-1.0.0/evals/cli/tmp/evallogs/2303191845497PQB7OUM_gpt-4_prime-number.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    39982 2023-03-19 18:46:00.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184553AE2AF4UE_gpt-4_ukraine-eit.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    13973 2023-03-19 18:46:05.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184602HO2R4BFU_gpt-4_mass-weight-conversion.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    22806 2023-03-19 18:46:15.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184611NRS736C2_gpt-4_sarcasm.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    13548 2023-03-19 18:46:22.000000 evals-1.0.0/evals/cli/tmp/evallogs/230319184617G4O2U7QW_gpt-4_determinant.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.469653 evals-1.0.0/evals/completion_fns/
+-rw-r--r--   0 kondrich   (502) staff       (20)        0 2023-04-11 16:48:30.000000 evals-1.0.0/evals/completion_fns/__init__.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2678 2023-04-11 20:40:46.000000 evals-1.0.0/evals/completion_fns/cot.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1245 2023-04-11 20:40:46.000000 evals-1.0.0/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1068 2023-04-11 20:40:46.000000 evals-1.0.0/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     4941 2023-04-11 20:40:46.000000 evals-1.0.0/evals/completion_fns/openai.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     4422 2023-04-12 23:38:05.000000 evals-1.0.0/evals/completion_fns/retrieval.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     5699 2023-04-05 21:17:17.000000 evals-1.0.0/evals/data.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.472421 evals-1.0.0/evals/elsuite/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.475989 evals-1.0.0/evals/elsuite/basic/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1655 2023-04-11 16:48:30.000000 evals-1.0.0/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1241 2023-04-12 23:38:05.000000 evals-1.0.0/evals/elsuite/basic/includes.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1831 2023-04-11 16:48:30.000000 evals-1.0.0/evals/elsuite/basic/match.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.478231 evals-1.0.0/evals/elsuite/modelgraded/
+-rw-r--r--   0 kondrich   (502) staff       (20)     6719 2023-04-11 00:03:54.000000 evals-1.0.0/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     9342 2023-04-11 16:48:30.000000 evals-1.0.0/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     3805 2023-04-11 00:03:54.000000 evals-1.0.0/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2682 2023-04-11 16:48:30.000000 evals-1.0.0/evals/elsuite/translate.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     5958 2023-04-12 23:38:05.000000 evals-1.0.0/evals/elsuite/utils.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     5497 2023-04-11 16:48:30.000000 evals-1.0.0/evals/eval.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1137 2023-03-18 03:40:27.000000 evals-1.0.0/evals/formatting.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2455 2023-03-18 03:40:27.000000 evals-1.0.0/evals/metrics.py
+-rw-r--r--   0 kondrich   (502) staff       (20)      453 2023-04-06 22:47:11.000000 evals-1.0.0/evals/mycompletionfn.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.478989 evals-1.0.0/evals/prompt/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4093 2023-04-11 16:48:30.000000 evals-1.0.0/evals/prompt/base.py
+-rw-r--r--   0 kondrich   (502) staff       (20)    17219 2023-04-11 16:48:30.000000 evals-1.0.0/evals/record.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.655567 evals-1.0.0/evals/registry/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.551074 evals-1.0.0/evals/registry/completion_fns/
+-rw-r--r--   0 kondrich   (502) staff       (20)      391 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      103 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      524 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.655055 evals-1.0.0/evals/registry/data/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.554139 evals-1.0.0/evals/registry/data/aba_mrpc_true_false/
+-rw-r--r--   0 kondrich   (502) staff       (20)    40248 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/aba_mrpc_true_false/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.559220 evals-1.0.0/evals/registry/data/actors-sequence/
+-rw-r--r--   0 kondrich   (502) staff       (20)    65813 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/actors-sequence/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.564719 evals-1.0.0/evals/registry/data/anagrams/
+-rw-r--r--   0 kondrich   (502) staff       (20)      748 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/anagrams/fewshot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    60081 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/anagrams/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.567964 evals-1.0.0/evals/registry/data/balance_chemical_equation/
+-rw-r--r--   0 kondrich   (502) staff       (20)    45027 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/balance_chemical_equation/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.572055 evals-1.0.0/evals/registry/data/belarusian_lexicon/
+-rw-r--r--   0 kondrich   (502) staff       (20)    62852 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/belarusian_lexicon/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.575988 evals-1.0.0/evals/registry/data/bigrams/
+-rw-r--r--   0 kondrich   (502) staff       (20)    72408 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/bigrams/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.579356 evals-1.0.0/evals/registry/data/born_first/
+-rw-r--r--   0 kondrich   (502) staff       (20)    22392 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/born_first/born_first.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.582978 evals-1.0.0/evals/registry/data/brazilian-lexicon/
+-rw-r--r--   0 kondrich   (502) staff       (20)  8355773 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/brazilian-lexicon/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.597685 evals-1.0.0/evals/registry/data/bulgarian-lexicon/
+-rw-r--r--   0 kondrich   (502) staff       (20)   154565 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/bulgarian-lexicon/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.604448 evals-1.0.0/evals/registry/data/chess/
+-rw-r--r--   0 kondrich   (502) staff       (20)    48775 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/chess/match.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.607422 evals-1.0.0/evals/registry/data/chess_piece_count/
+-rw-r--r--   0 kondrich   (502) staff       (20)   155059 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/chess_piece_count/fuzzy_match.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.610374 evals-1.0.0/evals/registry/data/complex_replace_characters/
+-rw-r--r--   0 kondrich   (502) staff       (20)    71392 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/complex_replace_characters/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.613931 evals-1.0.0/evals/registry/data/connect4/
+-rw-r--r--   0 kondrich   (502) staff       (20)   271001 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/connect4/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.617541 evals-1.0.0/evals/registry/data/convert-hex-hsl-lightness/
+-rw-r--r--   0 kondrich   (502) staff       (20)   219903 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/convert-hex-hsl-lightness/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.626078 evals-1.0.0/evals/registry/data/coqa/
+-rw-r--r--   0 kondrich   (502) staff       (20)    16912 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/coqa/match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    33337 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/coqa/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.628271 evals-1.0.0/evals/registry/data/crepe/
+-rw-r--r--   0 kondrich   (502) staff       (20)   795920 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/crepe/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.632492 evals-1.0.0/evals/registry/data/cube-pack/
+-rw-r--r--   0 kondrich   (502) staff       (20)    45998 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/cube-pack/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.636410 evals-1.0.0/evals/registry/data/decrypt_caesar_cipher/
+-rw-r--r--   0 kondrich   (502) staff       (20)  9361003 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/decrypt_caesar_cipher/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.649502 evals-1.0.0/evals/registry/data/determinant/
+-rw-r--r--   0 kondrich   (502) staff       (20)    95681 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/determinant/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.652958 evals-1.0.0/evals/registry/data/diagrammatic_logic/
+-rw-r--r--   0 kondrich   (502) staff       (20)  1924826 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/diagrammatic_logic/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.657663 evals-1.0.0/evals/registry/data/emotional-intelligence/
+-rw-r--r--   0 kondrich   (502) staff       (20)   117966 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/emotional-intelligence/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.660414 evals-1.0.0/evals/registry/data/first-letters/
+-rw-r--r--   0 kondrich   (502) staff       (20)    34457 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/first-letters/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.662600 evals-1.0.0/evals/registry/data/formal_logic/
+-rw-r--r--   0 kondrich   (502) staff       (20) 84600957 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/formal_logic/formal_logic_expressions.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.735489 evals-1.0.0/evals/registry/data/forth_stack_sim/
+-rw-r--r--   0 kondrich   (502) staff       (20)   122005 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/forth_stack_sim/basic_samples.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   322293 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/forth_stack_sim/detailed_samples.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    25750 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/forth_stack_sim/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.738693 evals-1.0.0/evals/registry/data/heart-disease/
+-rw-r--r--   0 kondrich   (502) staff       (20)   698130 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/heart-disease/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.743292 evals-1.0.0/evals/registry/data/hebrew_rhyme/
+-rw-r--r--   0 kondrich   (502) staff       (20)    14045 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/hebrew_rhyme/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.746189 evals-1.0.0/evals/registry/data/illinois-law/
+-rw-r--r--   0 kondrich   (502) staff       (20)   310186 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/illinois-law/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.749570 evals-1.0.0/evals/registry/data/imperial_date_to_string/
+-rw-r--r--   0 kondrich   (502) staff       (20)   337028 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/imperial_date_to_string/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.775395 evals-1.0.0/evals/registry/data/infiniteloop-match/
+-rw-r--r--   0 kondrich   (502) staff       (20)    79881 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/infiniteloop-match/infiniteloop-match.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.778194 evals-1.0.0/evals/registry/data/last_word_nth/
+-rw-r--r--   0 kondrich   (502) staff       (20)    30971 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/last_word_nth/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.780893 evals-1.0.0/evals/registry/data/lat_long_identify/
+-rw-r--r--   0 kondrich   (502) staff       (20)   186974 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/lat_long_identify/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.784622 evals-1.0.0/evals/registry/data/logic/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4833 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/logic/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.786901 evals-1.0.0/evals/registry/data/logic-statements/
+-rw-r--r--   0 kondrich   (502) staff       (20)    55936 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/logic-statements/logic-statements.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.791575 evals-1.0.0/evals/registry/data/logiqa/
+-rw-r--r--   0 kondrich   (502) staff       (20)  2192544 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/logiqa/logiqa.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.807779 evals-1.0.0/evals/registry/data/manga-translation/
+-rw-r--r--   0 kondrich   (502) staff       (20)   636299 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/manga-translation/bubbles.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   227677 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/manga-translation/pages.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   622876 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/manga-translation/panels.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.811698 evals-1.0.0/evals/registry/data/map-electronic-component-part-to-fact/
+-rw-r--r--   0 kondrich   (502) staff       (20)    32339 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/map-electronic-component-part-to-fact/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.813909 evals-1.0.0/evals/registry/data/mendelian_inheritance/
+-rw-r--r--   0 kondrich   (502) staff       (20)    14338 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/mendelian_inheritance/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.816557 evals-1.0.0/evals/registry/data/moral_exceptQA/
+-rw-r--r--   0 kondrich   (502) staff       (20)    87418 2023-04-12 22:03:03.000000 evals-1.0.0/evals/registry/data/moral_exceptQA/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.857205 evals-1.0.0/evals/registry/data/naughty_strings/
+-rw-r--r--   0 kondrich   (502) staff       (20)   102512 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/naughty_strings/samples.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    61312 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/naughty_strings/security.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.859988 evals-1.0.0/evals/registry/data/number_pattern/
+-rw-r--r--   0 kondrich   (502) staff       (20)    51330 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/number_pattern/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.863376 evals-1.0.0/evals/registry/data/number_reading/
+-rw-r--r--   0 kondrich   (502) staff       (20)    22951 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/number_reading/number_reading.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.865606 evals-1.0.0/evals/registry/data/partially_solved_crossword_clues/
+-rw-r--r--   0 kondrich   (502) staff       (20)    30125 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/partially_solved_crossword_clues/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.867759 evals-1.0.0/evals/registry/data/pattern_identification/
+-rw-r--r--   0 kondrich   (502) staff       (20)   172000 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/pattern_identification/samples.v0.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.872055 evals-1.0.0/evals/registry/data/poker_hand_ranks/
+-rw-r--r--   0 kondrich   (502) staff       (20)  2510549 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/poker_hand_ranks/full_samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.878614 evals-1.0.0/evals/registry/data/reasoning/
+-rw-r--r--   0 kondrich   (502) staff       (20)    19951 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/reasoning/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.881297 evals-1.0.0/evals/registry/data/regex-match/
+-rw-r--r--   0 kondrich   (502) staff       (20)    87293 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/regex-match/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.884589 evals-1.0.0/evals/registry/data/reverse_string/
+-rw-r--r--   0 kondrich   (502) staff       (20)     7178 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/reverse_string/reverse_string.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.886879 evals-1.0.0/evals/registry/data/rot13/
+-rw-r--r--   0 kondrich   (502) staff       (20)    49168 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/rot13/rot13.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.893123 evals-1.0.0/evals/registry/data/rucola/
+-rw-r--r--   0 kondrich   (502) staff       (20)     2746 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/rucola/few_shot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    75375 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/rucola/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.896451 evals-1.0.0/evals/registry/data/russian-nlp-tasks/
+-rw-r--r--   0 kondrich   (502) staff       (20)    96677 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/russian-nlp-tasks/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.901191 evals-1.0.0/evals/registry/data/sarcasm/
+-rw-r--r--   0 kondrich   (502) staff       (20)      963 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/sarcasm/few_shot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)  6906270 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/sarcasm/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.936891 evals-1.0.0/evals/registry/data/stock_options/
+-rw-r--r--   0 kondrich   (502) staff       (20)     5742 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_option_terms_bear_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     3824 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_option_terms_bull_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    11195 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_option_terms_inverse_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    11103 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_option_terms_inverse_iron_condor_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    10995 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_option_terms_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    11019 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_option_terms_iron_condor_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     9092 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_options_bear_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     6062 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_options_bull_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16822 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_options_inverse_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16745 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_options_inverse_iron_condor_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16688 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_options_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16741 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/stock_options/stock_options_iron_condor_spread.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.938970 evals-1.0.0/evals/registry/data/swedish-spelling/
+-rw-r--r--   0 kondrich   (502) staff       (20)    32883 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/swedish-spelling/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.941628 evals-1.0.0/evals/registry/data/taxes/
+-rw-r--r--   0 kondrich   (502) staff       (20)    80167 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/taxes/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.944617 evals-1.0.0/evals/registry/data/test_comp_sci/
+-rw-r--r--   0 kondrich   (502) staff       (20)    14311 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_comp_sci/questions.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.946715 evals-1.0.0/evals/registry/data/test_fuzzy_match/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1503 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_fuzzy_match/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.948233 evals-1.0.0/evals/registry/data/test_match/
+-rw-r--r--   0 kondrich   (502) staff       (20)      499 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_match/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.950273 evals-1.0.0/evals/registry/data/test_metaeval/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1712 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_metaeval/joke_fruits_labeled.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.953685 evals-1.0.0/evals/registry/data/test_modelgraded/
+-rw-r--r--   0 kondrich   (502) staff       (20)    19232 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_modelgraded/humor_people_jp.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      522 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_modelgraded/joke_fruits.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.654535 evals-1.0.0/evals/registry/data/test_multiio/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.961927 evals-1.0.0/evals/registry/data/test_multiio/battles/
+-rw-r--r--   0 kondrich   (502) staff       (20)      858 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_multiio/battles/joke_animals_vs_fruits.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     4863 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_multiio/battles/rap_animals_vs_fruits.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5043 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_multiio/battles/rap_people_vs_fruits.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5187 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/test_multiio/battles/rap_people_vs_people.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.964161 evals-1.0.0/evals/registry/data/ukraine_eit/
+-rw-r--r--   0 kondrich   (502) staff       (20) 13814472 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/ukraine_eit/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.980770 evals-1.0.0/evals/registry/data/us_tort_law/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4406 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/us_tort_law/few_shot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   474865 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/us_tort_law/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:05.985073 evals-1.0.0/evals/registry/data/which_is_heavier/
+-rw-r--r--   0 kondrich   (502) staff       (20)    37434 2023-04-12 22:02:57.000000 evals-1.0.0/evals/registry/data/which_is_heavier/which_is_heavier.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:06.001198 evals-1.0.0/evals/registry/eval_sets/
+-rw-r--r--   0 kondrich   (502) staff       (20)       99 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      119 2023-04-10 23:31:52.000000 evals-1.0.0/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      560 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      291 2023-04-11 16:55:22.000000 evals-1.0.0/evals/registry/eval_sets/subset.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      412 2023-04-12 23:38:05.000000 evals-1.0.0/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      113 2023-04-12 23:38:05.000000 evals-1.0.0/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      312 2023-04-11 00:03:54.000000 evals-1.0.0/evals/registry/eval_sets/test-modelgraded.yaml
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:06.120392 evals-1.0.0/evals/registry/evals/
+-rw-r--r--   0 kondrich   (502) staff       (20)      215 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      297 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      229 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      310 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      159 2023-03-20 23:45:34.000000 evals-1.0.0/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      246 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      288 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      305 2023-04-10 23:31:52.000000 evals-1.0.0/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      309 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/chess.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      250 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      160 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      335 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1287 2023-04-10 23:31:52.000000 evals-1.0.0/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      151 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      167 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      214 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      175 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      202 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      387 2023-04-11 20:40:46.000000 evals-1.0.0/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      183 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      276 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      928 2023-04-10 23:31:52.000000 evals-1.0.0/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      258 2023-04-11 20:40:46.000000 evals-1.0.0/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      250 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      265 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      222 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      347 2023-03-20 23:45:34.000000 evals-1.0.0/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      327 2023-03-20 23:45:34.000000 evals-1.0.0/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      198 2023-03-20 23:45:34.000000 evals-1.0.0/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      214 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      242 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/logic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      153 2023-04-11 20:40:46.000000 evals-1.0.0/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      674 2023-04-10 23:31:52.000000 evals-1.0.0/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      278 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      215 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)    24917 2023-03-30 00:42:10.000000 evals-1.0.0/evals/registry/evals/mmlu.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      329 2023-04-12 22:03:01.000000 evals-1.0.0/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1193 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      186 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      292 2023-04-10 23:31:52.000000 evals-1.0.0/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      258 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      221 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      188 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      175 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      378 2023-03-18 03:40:27.000000 evals-1.0.0/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      255 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      236 2023-04-11 00:03:54.000000 evals-1.0.0/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      199 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      274 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     4472 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      272 2023-04-11 20:40:46.000000 evals-1.0.0/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      150 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1218 2023-04-12 23:38:05.000000 evals-1.0.0/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      400 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1273 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      347 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     3046 2023-04-11 00:03:54.000000 evals-1.0.0/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      174 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      329 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      365 2023-03-29 23:16:30.000000 evals-1.0.0/evals/registry/evals/which-is-heavier.yaml
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:06.134179 evals-1.0.0/evals/registry/modelgraded/
+-rw-r--r--   0 kondrich   (502) staff       (20)      492 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      291 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1070 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      274 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1157 2023-03-28 05:28:29.000000 evals-1.0.0/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     2564 2023-04-11 00:03:54.000000 evals-1.0.0/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     9600 2023-04-11 16:48:30.000000 evals-1.0.0/evals/registry.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:06.135214 evals-1.0.0/evals/utils/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1504 2023-04-11 16:48:30.000000 evals-1.0.0/evals/utils/api_utils.py
+-rw-r--r--   0 kondrich   (502) staff       (20)      713 2023-03-18 03:40:27.000000 evals-1.0.0/evals/utils/misc.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     3991 2023-03-18 03:40:27.000000 evals-1.0.0/evals/utils/snowflake.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-12 23:44:03.668520 evals-1.0.0/evals.egg-info/
+-rw-r--r--   0 kondrich   (502) staff       (20)       94 2023-04-12 23:44:03.000000 evals-1.0.0/evals.egg-info/PKG-INFO
+-rw-r--r--   0 kondrich   (502) staff       (20)    25018 2023-04-12 23:44:03.000000 evals-1.0.0/evals.egg-info/SOURCES.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)        1 2023-04-12 23:44:03.000000 evals-1.0.0/evals.egg-info/dependency_links.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)       90 2023-04-12 23:44:03.000000 evals-1.0.0/evals.egg-info/entry_points.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)      207 2023-04-12 23:44:03.000000 evals-1.0.0/evals.egg-info/requires.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)        6 2023-04-12 23:44:03.000000 evals-1.0.0/evals.egg-info/top_level.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)      546 2023-04-11 16:48:30.000000 evals-1.0.0/pyproject.toml
+-rw-r--r--   0 kondrich   (502) staff       (20)       38 2023-04-12 23:44:06.136136 evals-1.0.0/setup.cfg
```

### Comparing `evals-0.1.1/LICENSE` & `evals-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-0.1.1/README.md` & `evals-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # Evals
 
-Evals is a framework for evaluating OpenAI models and an open-source registry of benchmarks.
+Evals is a framework for evaluating LLMs (large language models) or systems built using LLMs as components. It also includes an open-source registry of challenging evals.
 
-You can use Evals to create and run evaluations that:
-- use datasets to generate prompts,
-- measure the quality of completions provided by an OpenAI model, and
-- compare performance across different datasets and models.
-
-With Evals, we aim to make it as simple as possible to build an eval while writing as little code as possible. To get started, we recommend that you follow these steps **in order**:
-1. Read through this doc and follow the [setup instructions below](README.md#Setup).
-2. Learn how to run existing evals: [run-evals.md](docs/run-evals.md).
-3. Familiarize yourself with the existing eval templates: [eval-templates.md](docs/eval-templates.md).
-4. Walk through the process for building an eval: [build-eval.md](docs/build-eval.md)
-5. See an example of implementing custom eval logic: [custom-eval.md](docs/custom-eval.md).
+We now support evaluating the behavior of any system including prompt chains or tool-using agents, via the [Completion Function Protocol](docs/completion-fns.md).
+
+With Evals, we aim to make it as simple as possible to build an eval while writing as little code as possible. An "eval" is a task used to evaluate the quality of a system's behavior. To get started, we recommend that you follow these steps:
+
+To get set up with evals, follow the [setup instructions below](README.md#Setup).
+
+#### Running evals
+- Learn how to run existing evals: [run-evals.md](docs/run-evals.md).
+- Familiarize yourself with the existing eval templates: [eval-templates.md](docs/eval-templates.md).
+
+#### Writing evals
+- Walk through the process for building an eval: [build-eval.md](docs/build-eval.md)
+- See an example of implementing custom eval logic: [custom-eval.md](docs/custom-eval.md).
+
+#### Writing CompletionFns
+- Write your own completion functions: [completion-fns.md](docs/completion-fns.md)
 
 If you think you have an interesting eval, please open a PR with your contribution. OpenAI staff actively review these evals when considering improvements to upcoming models.
 
 ____________________
 🚨 For a limited time, we will be granting GPT-4 access to those who contribute high quality evals. Please follow the instructions mentioned above and note that spam or low quality submissions will be ignored❗️
 
 Access will be granted to the email address associated with an accepted Eval. Due to high volume, we are unable to grant access to any email other than the one used for the pull request.
 ____________________
 
 ## Setup
 
-To run evals, you will need to set up and specify your OpenAI API key to run evals. If you need to generate an API key, you can do so at [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys). After you obtain an API key, specify it using the `OPENAI_API_KEY` environment variable. **Please be aware of the [costs](https://openai.com/pricing) associated with using the API when running evals.**
+To run evals, you will need to set up and specify your OpenAI API key. You can generate one at <https://platform.openai.com/account/api-keys>. After you obtain an API key, specify it using the `OPENAI_API_KEY` environment variable. **Please be aware of the [costs](https://openai.com/pricing) associated with using the API when running evals.**
+
+**Minimal Required Version: Python 3.9**
 
 ### Downloading evals
 
 Our Evals registry is stored using [Git-LFS](https://git-lfs.com/). Once you have downloaded and installed LFS, you can fetch the evals with:
 ```sh
 git lfs fetch --all
 git lfs pull
@@ -66,17 +73,17 @@
 
 - Yes! These are in the `examples` folder. We recommend that you also read through [build-eval.md](docs/build-eval.md) in order to gain a deeper understanding of what is happening in these examples.
 
 Do you have any examples of evals implemented in multiple different ways?
 
 - Yes! In particular, see `evals/registry/evals/coqa.yaml`. We have implemented small subsets of the [CoQA](https://stanfordnlp.github.io/coqa/) dataset for various eval templates to help illustrate the differences.
 
-I changed my data but this isn't reflected when running my eval, what's going on?
+When I run an eval, it sometimes hangs at the very end (after the final report). What's going on?
 
-- Your data may have been cached to `/tmp/filecache`. Try removing this cache and rerunning your eval.
+- This is a known issue, but you should be able to interrupt it safely and the eval should finish immediately after.
 
 There's a lot of code, and I just want to spin up a quick eval. Help? OR,
 
 I am a world-class prompt engineer. I choose not to code. How can I contribute my wisdom?
 
 - If you follow an existing [eval template](docs/eval-templates.md) to build a basic or model-graded eval, you don't need to write any evaluation code at all! Just provide your data in JSON format and specify your eval parameters in YAML. [build-eval.md](docs/build-eval.md) walks you through these steps, and you can supplement these instructions with the Jupyter notebooks in the `examples` folder to help you get started quickly. Keep in mind, though, that a good eval will inevitably require careful thought and rigorous experimentation!
```

### Comparing `evals-0.1.1/evals/cli/oaievalset.py` & `evals-1.0.0/evals/cli/oaievalset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This file defines the `oaievalset` CLI for running eval sets.
 """
 import argparse
 import json
 import subprocess
 from pathlib import Path
+from typing import Optional
 
 from evals.registry import Registry
 
 Task = list[str]
 
 
 class Progress:
@@ -37,15 +38,15 @@
             print(highlight(f"Saved progress to {self.file}"))
 
 
 def highlight(str: str) -> str:
     return f"\033[1;32m>>> {str}\033[0m"
 
 
-def main() -> None:
+def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="Run eval sets through the API")
     parser.add_argument("model", type=str, help="Name of a completion model.")
     parser.add_argument("eval_set", type=str, help="Name of eval set. See registry.")
     parser.add_argument(
         "--resume",
         action=argparse.BooleanOptionalAction,
         default=True,
@@ -53,17 +54,19 @@
     )
     parser.add_argument(
         "--exit-on-error",
         action=argparse.BooleanOptionalAction,
         default=True,
         help="Exit if any oaieval command fails.",
     )
-    args, unknown_args = parser.parse_known_args()
+    return parser
 
-    registry = Registry()
+
+def run(args, unknown_args, registry: Optional[Registry] = None) -> None:
+    registry = registry or Registry()
     commands: list[Task] = []
     eval_set = registry.get_eval_set(args.eval_set)
     for eval in registry.get_evals(eval_set.evals):
         command = ["oaieval", args.model, eval.key] + unknown_args
         if command in commands:
             continue
         commands.append(command)
@@ -88,9 +91,15 @@
         print(highlight("Running command: " + " ".join(command) + f" ({real_idx+1}/{num_evals})"))
         subprocess.run(command, stdout=subprocess.PIPE, check=args.exit_on_error)
         progress.add(command)
 
     print(highlight("All done!"))
 
 
+def main() -> None:
+    parser = get_parser()
+    args, unknown_args = parser.parse_known_args()
+    run(args, unknown_args)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `evals-0.1.1/evals/data.py` & `evals-1.0.0/evals/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """
 This file defines utilities for working with data and files of various types.
 """
 import csv
 import dataclasses
 import gzip
-import hashlib
 import itertools
 import json
 import logging
 import os
-import pickle
 import urllib
 from collections.abc import Iterator
 from functools import partial
-from pathlib import Path
 from typing import Any, Sequence, Union
 
 import blobfile as bf
 import lz4.frame
 import pydantic
 import pyzstd
 
@@ -89,44 +86,22 @@
 def _stream_jsonl_file(path) -> Iterator:
     logger.info(f"Streaming {path}")
     with bf.BlobFile(path, "r", streaming=True) as f:
         for line in f:
             yield json.loads(line)
 
 
-def filecache(func):
-    DIR = "/tmp/filecache"
-    name = func.__name__
-
-    def wrapper(*args, **kwargs):
-        md5 = hashlib.md5((name + ":" + str((args, kwargs))).encode("utf-8")).hexdigest()
-        pkl_path = f"{DIR}/{md5}.pkl"
-        if os.path.exists(pkl_path):
-            logger.debug(f"Loading from file cache: {pkl_path}")
-            with open(pkl_path, "rb") as f:
-                return pickle.load(f)
-        result = func(*args, **kwargs)
-        Path(DIR).mkdir(parents=True, exist_ok=True)
-        with open(pkl_path, "wb") as f:
-            pickle.dump(result, f)
-        return result
-
-    return wrapper
-
-
-@filecache
 def get_lines(path) -> list[dict]:
     """
     Get a list of lines from a file.
     """
     with open_by_file_pattern(path, mode="r") as f:
         return f.readlines()
 
 
-@filecache
 def get_jsonl(path: str) -> list[dict]:
     """
     Extract json lines from the given path.
     If the path is a directory, look in subpaths recursively.
 
     Return all lines from all jsonl files as a single list.
     """
@@ -135,20 +110,18 @@
         for filename in bf.listdir(path):
             if filename.endswith(".jsonl"):
                 result += get_jsonl(os.path.join(path, filename))
         return result
     return _get_jsonl_file(path)
 
 
-@filecache
 def get_jsonls(paths: Sequence[str], line_limit=None) -> list[dict]:
     return list(iter_jsonls(paths, line_limit))
 
 
-@filecache
 def get_json(path) -> dict:
     if bf.isdir(path):
         raise ValueError("Path is a directory, only files are supported")
     return _get_json_file(path)
 
 
 def iter_jsonls(paths: Union[str, list[str]], line_limit=None) -> Iterator[dict]:
@@ -196,20 +169,20 @@
 
 
 class EnhancedJSONEncoder(json.JSONEncoder):
     def default(self, o: Any) -> str:
         return _to_py_types(o)
 
 
-def jsondumps(o: Any, **kwargs: Any) -> str:
-    return json.dumps(o, cls=EnhancedJSONEncoder, **kwargs)
+def jsondumps(o: Any, ensure_ascii: bool = False, **kwargs: Any) -> str:
+    return json.dumps(o, cls=EnhancedJSONEncoder, ensure_ascii=ensure_ascii, **kwargs)
 
 
-def jsondump(o: Any, fp: Any, **kwargs: Any) -> None:
-    json.dump(o, fp, cls=EnhancedJSONEncoder, **kwargs)
+def jsondump(o: Any, fp: Any, ensure_ascii: bool = False, **kwargs: Any) -> None:
+    json.dump(o, fp, cls=EnhancedJSONEncoder, ensure_ascii=ensure_ascii, **kwargs)
 
 
 def jsonloads(s: str, **kwargs: Any) -> Any:
     return json.loads(s, **kwargs)
 
 
 def jsonload(fp: Any, **kwargs: Any) -> Any:
```

### Comparing `evals-0.1.1/evals/elsuite/basic/fuzzy_match.py` & `evals-1.0.0/evals/elsuite/basic/fuzzy_match.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-import evals
 import numpy as np
+
+import evals
+from evals.api import CompletionFn
 from evals.elsuite import utils
 from evals.record import RecorderBase
 
 
 class FuzzyMatch(evals.Eval):
     def __init__(
         self,
-        model_specs: evals.ModelSpecs,
+        completion_fns: list[CompletionFn],
         samples_jsonl: str,
         *args,
         max_tokens: int = 500,
         **kwargs,
     ):
-        super().__init__(model_specs, *args, **kwargs)
+        super().__init__(completion_fns, *args, **kwargs)
+        assert len(completion_fns) == 1, "FuzzyMatch only supports one completion fn"
         self.max_tokens = max_tokens
         self.samples_jsonl = samples_jsonl
 
     def eval_sample(self, test_sample, rng):
+        del rng
         prompt, correct_answers = test_sample["input"], test_sample["ideal"]
-        generated_answer = evals.sample_freeform(
-            self.model_spec,
-            prompt,
-            temperature=0.0,
+        result = self.completion_fn(
+            prompt=prompt,
+            temperature=0.0,  # Q: why are these hardcoded?
             max_tokens=16,
         )
-        matches = [
-            utils.fuzzy_match(generated_answer, correct_answer)
-            for correct_answer in correct_answers
-        ]
+        sampled = result.get_completions()[0]
+
+        matches = [utils.fuzzy_match(sampled, correct_answer) for correct_answer in correct_answers]
         evals.record.record_match(
             True in matches,
             expected=correct_answers,
-            picked=[generated_answer for i in range(len(correct_answers)) if matches[i]],
+            picked=[sampled for i in range(len(correct_answers)) if matches[i]],
         )
         evals.record.record_metrics(
             accuracy=float(True in matches),
-            f1_score=utils.f1_score(generated_answer, correct_answers),
+            f1_score=utils.f1_score(sampled, correct_answers),
         )
 
     def run(self, recorder: RecorderBase):
-        samples = evals.get_jsonl(self.samples_jsonl)
+        samples = self.get_samples()
         self.eval_all_samples(recorder, samples)
 
         return {
             "accuracy": np.mean(recorder.get_scores("accuracy")),
             "f1_score": np.mean(recorder.get_scores("f1_score")),
         }
```

### Comparing `evals-0.1.1/evals/elsuite/basic/includes.py` & `evals-1.0.0/evals/elsuite/basic/includes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 from typing import Any
 
+import numpy as np
+
 import evals
-import evals.elsuite.utils
 import evals.metrics
-import numpy as np
+from evals.api import CompletionFn
+from evals.elsuite import utils
 
 
 class Includes(evals.Eval):
     def __init__(
         self,
-        model_specs: evals.ModelSpecs,
+        completion_fns: list[CompletionFn],
         samples_jsonl: str,
+        ignore_case: bool = False,
         *args,
-        max_tokens: int = 500,
         **kwargs,
     ):
-        super().__init__(model_specs, *args, **kwargs)
-        self.max_tokens = max_tokens
+        super().__init__(completion_fns, *args, **kwargs)
+        assert len(completion_fns) == 1, "Includes only supports one completion fn"
         self.samples_jsonl = samples_jsonl
+        self.ignore_case = ignore_case
 
     def eval_sample(self, sample: Any, *_):
-        sampled = evals.sample_freeform(
-            self.model_spec, sample["input"], max_tokens=self.max_tokens
+        prompt = sample["input"]
+        result = self.completion_fn(
+            prompt=prompt,
         )
+        sampled = result.get_completions()[0]
+
         includes_answer = any(
-            [evals.elsuite.utils.get_answer(sampled, ref) for ref in sample["ideal"]]
+            [utils.get_answer(sampled, ref, self.ignore_case) for ref in sample["ideal"]]
         )
         evals.record.record_metrics(accuracy=float(includes_answer))
         return includes_answer
 
     def run(self, recorder):
-        samples = evals.get_jsonl(self.samples_jsonl)
+        samples = self.get_samples()
         self.eval_all_samples(recorder, samples)
         events = recorder.get_scores("accuracy")
         return {
             "accuracy": np.mean(events),
         }
```

### Comparing `evals-0.1.1/evals/elsuite/utils.py` & `evals-1.0.0/evals/elsuite/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import copy
-import os
 import re
 import string
 from collections import Counter, defaultdict
+from typing import Optional, Union
 
-import yaml
+from evals import CompletionFn
+from evals.prompt.base import (
+    OpenAICreateChatPrompt,
+    OpenAICreatePrompt,
+    Prompt,
+    chat_prompt_to_text_prompt,
+    is_chat_prompt,
+)
 
-from evals.api import sample_freeform
-from evals.prompt.base import chat_prompt_to_text_prompt, is_chat_prompt
-
-
-def load_modelgraded_specs(spec_file: str) -> str:
-    current_dir = os.path.dirname(os.path.abspath(__file__))
-    yaml_path = os.path.join(current_dir, "../registry/modelgraded", f"{spec_file}.yaml")
-    return yaml.load(open(yaml_path, "r"), Loader=yaml.FullLoader)
 
+def get_answer(text, answer_prompt, ignore_case=False):
+    if ignore_case:
+        idx = text.lower().rfind(answer_prompt.lower())
+    else:
+        idx = text.rfind(answer_prompt)
 
-def get_answer(text, answer_prompt):
-    idx = text.rfind(answer_prompt)
     if idx == -1:
         return None
     return text[idx + len(answer_prompt) :]
 
 
 def get_consensus(answers):
     counts = defaultdict(int)
@@ -98,28 +100,63 @@
         scrubbed_prompt = scrubbed_prompt.replace("{", "{{").replace("}", "}}")
     return scrubbed_prompt
 
 
 def format_necessary(template: str, **kwargs: dict[str, str]) -> str:
     """Format a template string with only necessary kwargs."""
     keys = [k[1] for k in string.Formatter().parse(template) if k[1]]
-    assert all(k in kwargs for k in keys), f"Required: {keys}, got: {sorted(kwargs)}"
+    assert all(
+        k in kwargs for k in keys
+    ), f"Required: {keys}, got: {sorted(kwargs)}.\nTemplate:\n{template}"
     cur_keys = {k: kwargs[k] for k in keys}
     return template.format(**cur_keys)
 
 
-class PromptFn:
-    """Wrap calls to model with prompt"""
+def format_prompt(prompt: OpenAICreatePrompt, **kwargs: dict[str, str]) -> OpenAICreatePrompt:
+    """Format a prompt with only necessary kwargs."""
+    # if any input kwargs is chat prompt, convert to text prompt
+    kwargs = {
+        k: chat_prompt_to_text_prompt(v, for_completion=False) if is_chat_prompt(v) else v
+        for k, v in kwargs.items()
+    }
+    if is_chat_prompt(prompt):
+        new_prompt = []
+        for msg in prompt:
+            formatted_msg = copy.copy(msg)
+            if "content" in formatted_msg:
+                formatted_msg["content"] = format_necessary(formatted_msg["content"], **kwargs)
+            new_prompt.append(formatted_msg)
+        prompt = new_prompt
+    else:
+        # Prompt is a string
+        prompt = format_necessary(prompt, **kwargs)
+    return prompt
 
-    def __init__(self, prompt, model_spec, max_tokens, temperature=0, completion_kwargs=None):
+
+class PromptFn:
+    """
+    Wrap calls to a completion_fn with a prompt template with applicable keyword args.
+    This will pass many args relevant to OpenAI Completion API, may be ignored by other completion_fn.
+    """
+
+    def __init__(
+        self,
+        prompt: Union[OpenAICreatePrompt, OpenAICreateChatPrompt, Prompt],
+        completion_fn: CompletionFn,
+        max_tokens: int,
+        temperature: int = 0,
+        n_samples: Optional[int] = None,
+        completion_kwargs: Optional[dict] = {},
+    ):
         self.prompt = prompt
         self.max_tokens = max_tokens
-        self.model_spec = model_spec
+        self.completion_fn = completion_fn
         self.temperature = temperature
-        self.completion_kwargs = completion_kwargs or {}
+        self.completion_kwargs = completion_kwargs
+        self.n_samples = n_samples
 
     def __call__(self, **kwargs):
         # if any input kwargs is chat prompt, convert to text prompt
         kwargs = {
             k: chat_prompt_to_text_prompt(v) if is_chat_prompt(v) else v for k, v in kwargs.items()
         }
         if is_chat_prompt(self.prompt):
@@ -129,18 +166,19 @@
                 if "content" in formatted_msg:
                     formatted_msg["content"] = format_necessary(formatted_msg["content"], **kwargs)
                 prompt.append(formatted_msg)
         else:
             # Prompt is a string
             prompt = format_necessary(self.prompt, **kwargs)
 
-        completion = sample_freeform(
-            self.model_spec,
-            prompt,
+        result = self.completion_fn(
+            prompt=prompt,
             max_tokens=self.max_tokens,
             temperature=self.temperature,
             top_p=1,
             frequency_penalty=0,
             presence_penalty=0,
+            n=(1 if self.n_samples is None else self.n_samples),
             **self.completion_kwargs,
         )
-        return completion, prompt
+        sampled = result.get_completions()[0]
+        return sampled, prompt
```

### Comparing `evals-0.1.1/evals/eval.py` & `evals-1.0.0/evals/eval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """
 This file defines the base class for evals.
 """
 import abc
 import asyncio
+import concurrent.futures
 import logging
 import os
 import random
 from multiprocessing.pool import ThreadPool
-from typing import Any, Awaitable, Callable, Dict, List, Tuple
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple
 
 from tqdm import tqdm
 
-from .base import ModelSpec, ModelSpecs
-from .record import Recorder, RecorderBase
+from evals.api import CompletionFn
+
+from .record import RecorderBase
+from .registry import Registry
+from .data import get_jsonl
 
 logger = logging.getLogger(__name__)
 
 
 SHUFFLE_SEED = 123
 _MAX_SAMPLES = None
 
@@ -45,38 +49,37 @@
     `run`: Takes in a recorder and runs the evaluation. Generally, most `run`
         methods will follow this same pattern: loading the data, calling
         `eval_all_samples`, and aggregating the recorded results.
     """
 
     def __init__(
         self,
-        model_specs: ModelSpecs,
+        completion_fns: list[CompletionFn],
         seed: int = 20220722,
         name: str = "no_name_eval.default",
+        registry: Optional[Registry] = None,
+        samples_jsonl: Optional[str] = None,
     ):
         splits = name.split(".")
         if len(splits) < 2:
             raise ValueError(f"Eval name must at least have <base_eval>.<split>. Got name {name}")
 
-        self.model_specs = model_specs
+        self.completion_fns = completion_fns
         self.seed = seed
         self.name = name
+        self.registry = registry or Registry()
+        self.samples_jsonl = samples_jsonl
 
     def eval_sample(self, sample: Any, rng: random.Random):
         raise NotImplementedError()
 
-    @classmethod
-    def create_and_run(cls, model_specs: ModelSpecs, *args, **kwargs) -> Dict[str, float]:
-        logging.info(f"Running {cls.__name__} with {model_specs}, args: {args}, kwargs: {kwargs}")
-        return cls(model_specs).run(*args, **kwargs)
-
     @property
-    def model_spec(self) -> ModelSpec:
-        """Helper for more ergonomic access to a single model."""
-        return self.model_specs.completion
+    def completion_fn(self) -> CompletionFn:
+        """Helper for more ergonomic access to a single CompletionFn."""
+        return self.completion_fns[0]
 
     @abc.abstractmethod
     def run(self, recorder: RecorderBase) -> Dict[str, float]:
         """Run the evaluation with the corresponding recorder."""
         raise NotImplementedError()
 
     async def async_eval_all_samples(
@@ -101,39 +104,59 @@
             await future
 
     def eval_all_samples(
         self,
         recorder: RecorderBase,
         samples,
         show_progress=True,
+        record_raw_sample=True,
     ):
         """
         Evaluate all provided samples in parallel.
         """
         work_items = _index_samples(samples)
         threads = int(os.environ.get("EVALS_THREADS", "10"))
-
         show_progress = bool(os.environ.get("EVALS_SHOW_EVAL_PROGRESS", show_progress))
+        timeout = float(os.environ.get("EVALS_THREAD_TIMEOUT", "40"))
 
-        with ThreadPool(threads) as pool:
-
-            def eval_sample(args):
-                """
-                Evaluate a single sample.
-                """
-                sample, idx = args
-                base_name, split = self.name.split(".")[0:2]
-                sample_id = f"{base_name}.{split}.{idx}"
-                with recorder.as_default_recorder(sample_id):
-                    recorder.record_raw(sample)
-                    seed = f"{sample_id}:{self.seed}".encode("utf-8")
-                    rng = random.Random(seed)
-                    return idx, self.eval_sample(sample, rng)
+        def eval_sample(args):
+            """
+            Evaluate a single sample.
+            """
+            sample, idx = args
+            base_name, split = self.name.split(".")[0:2]
+            sample_id = f"{base_name}.{split}.{idx}"
+            with recorder.as_default_recorder(sample_id):
+                seed = f"{sample_id}:{self.seed}".encode("utf-8")
+                rng = random.Random(seed)
+                return idx, self.eval_sample(sample, rng)
+
+        def worker_thread(args):
+            """
+            Worker thread for evaluating a single sample.
+            """
+            while True:
+                executor = concurrent.futures.ThreadPoolExecutor(max_workers=1)
+                future = executor.submit(eval_sample, args=args)
+                try:
+                    result = future.result(timeout=timeout)
+                    return result
+                except concurrent.futures.TimeoutError as e:
+                    executor.shutdown(wait=False)
 
+        with ThreadPool(threads) as pool:
             if os.environ.get("EVALS_SEQUENTIAL", "0") in {"1", "true", "yes"}:
-                logger.info(f"Running in sequential mode with {threads} threads!")
+                logger.info(f"Running in sequential mode!")
                 iter = map(eval_sample, work_items)
             else:
                 logger.info(f"Running in threaded mode with {threads} threads!")
-                iter = pool.imap_unordered(eval_sample, work_items)
+                iter = pool.imap_unordered(worker_thread, work_items)
             idx_and_result = list(tqdm(iter, total=len(work_items), disable=not show_progress))
         return [r for _, r in sorted(idx_and_result)]
+
+    def get_samples(self):
+        if self.samples_jsonl is None:
+            raise ValueError(
+                    "To use `get_samples`, you must provide a `samples_jsonl` path."
+                    "Got `None`.")
+
+        return get_jsonl(self.samples_jsonl)
```

### Comparing `evals-0.1.1/evals/formatting.py` & `evals-1.0.0/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-0.1.1/evals/metrics.py` & `evals-1.0.0/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-0.1.1/evals/prompt/base.py` & `evals-1.0.0/evals/prompt/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 OpenAICreatePrompt = Union[str, list[str], list[int], list[list[int]]]
 
 # This is the type accepted as the `prompt` field to `openai.ChatCompletion.create` calls
 OpenAIChatMessage = Dict[str, str]  # A message is a dictionary with "role" and "content" keys
 OpenAICreateChatPrompt = List[OpenAIChatMessage]  # A chat log is a list of messages
 
 
-def chat_prompt_to_text_prompt(prompt: OpenAICreateChatPrompt) -> str:
+def chat_prompt_to_text_prompt(prompt: OpenAICreateChatPrompt, for_completion: bool = True) -> str:
     """
     Render a chat prompt as a text prompt. User and assistant messages are separated by newlines
     and prefixed with "User: " and "Assistant: ", respectively, unless there is only one message.
     System messages have no prefix.
     """
     assert is_chat_prompt(prompt), f"Expected a chat prompt, got {prompt}"
     chat_to_prefixes = {
@@ -40,57 +40,57 @@
 
     text = ""
     for msg in prompt:
         role = msg["name"] if "name" in msg else msg["role"]
         prefix = chat_to_prefixes.get(role, role.capitalize() + ": ")
         content = msg["content"]
         text += f"{prefix}{content}\n"
-    text += "Assistant: "
+    if for_completion:
+        text += "Assistant: "
     return text.lstrip()
 
 
-def text_prompt_to_chat_prompt(prompt: str) -> OpenAICreateChatPrompt:
+def text_prompt_to_chat_prompt(prompt: str, role: str = "system") -> OpenAICreateChatPrompt:
     assert isinstance(prompt, str), f"Expected a text prompt, got {prompt}"
     return [
-        {"role": "system", "content": prompt},
+        {"role": role, "content": prompt},
     ]
 
 
 @dataclass
 class Prompt(ABC):
     """
     A `Prompt` encapsulates everything required to present the `raw_prompt` in different formats,
     e.g., a normal unadorned format vs. a chat format.
     """
 
     @abstractmethod
-    def to_openai_create_prompt(self):
+    def to_formatted_prompt(self):
         """
-        Return the actual data to be passed as the `prompt` field to either `openai.ChatCompletion.create`,
-        if the model is a chat model, or `openai.Completion.create` otherwise.
+        Return the actual data to be passed as the `prompt` field to your model.
         See the above types to see what each API call is able to handle.
         """
 
 
 def is_chat_prompt(prompt: Prompt) -> bool:
     return isinstance(prompt, list) and all(isinstance(msg, dict) for msg in prompt)
 
 
 @dataclass
 class CompletionPrompt(Prompt):
     """
     A `Prompt` object that wraps prompts to be compatible with non chat models, which use `openai.Completion.create`.
     """
 
-    raw_prompt: Union[OpenAICreatePrompt, OpenAICreateChatPrompt]
+    raw_prompt: Union[str, OpenAICreateChatPrompt]
 
-    def _render_chat_prompt_as_text(self, prompt: OpenAICreateChatPrompt) -> OpenAICreatePrompt:
+    def _render_chat_prompt_as_text(self, prompt: OpenAICreateChatPrompt) -> str:
         return chat_prompt_to_text_prompt(prompt)
 
-    def to_openai_create_prompt(self) -> OpenAICreatePrompt:
+    def to_formatted_prompt(self) -> str:
         if is_chat_prompt(self.raw_prompt):
             return self._render_chat_prompt_as_text(self.raw_prompt)
         return self.raw_prompt
 
 
 @dataclass
 class ChatCompletionPrompt(Prompt):
@@ -105,11 +105,11 @@
     def _render_text_as_chat_prompt(self, prompt: str) -> OpenAICreateChatPrompt:
         """
         Render a text string as a chat prompt. The default option we adopt here is to simply take the full prompt
         and treat it as a system message.
         """
         return text_prompt_to_chat_prompt(prompt)
 
-    def to_openai_create_prompt(self) -> OpenAICreateChatPrompt:
+    def to_formatted_prompt(self) -> OpenAICreateChatPrompt:
         if is_chat_prompt(self.raw_prompt):
             return self.raw_prompt
         return self._render_text_as_chat_prompt(self.raw_prompt)
```

### Comparing `evals-0.1.1/evals/record.py` & `evals-1.0.0/evals/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,76 +288,77 @@
     This is the default recorder used by `oaieval`.
     """
 
     def __init__(self, log_path: Optional[str], run_spec: RunSpec):
         super().__init__(run_spec)
         self.event_file_path = log_path
         if log_path is not None:
-            with bf.BlobFile(log_path, "w") as f:
-                f.write(jsondumps({"spec": dataclasses.asdict(run_spec)}) + "\n")
+            with bf.BlobFile(log_path, "wb") as f:
+                f.write((jsondumps({"spec": dataclasses.asdict(run_spec)}) + "\n").encode("utf-8"))
 
     def _flush_events_internal(self, events_to_write: Sequence[Event]):
         start = time.time()
         try:
             lines = [jsondumps(event) + "\n" for event in events_to_write]
         except TypeError as e:
             logger.error(f"Failed to serialize events: {events_to_write}")
             raise e
 
-        with bf.BlobFile(self.event_file_path, "a") as f:
-            f.writelines(lines)
+        with bf.BlobFile(self.event_file_path, "ab") as f:
+            f.write(b"".join([l.encode("utf-8") for l in lines]))
 
         logger.info(
             f"Logged {len(lines)} rows of events to {self.event_file_path}: insert_time={t(time.time()-start)}"
         )
 
         self._last_flush_time = time.time()
         self._flushes_done += 1
 
     def record_final_report(self, final_report: Any):
-        with bf.BlobFile(self.event_file_path, "a") as f:
-            f.write(jsondumps({"final_report": final_report}) + "\n")
+        with bf.BlobFile(self.event_file_path, "ab") as f:
+            f.write((jsondumps({"final_report": final_report}) + "\n").encode("utf-8"))
 
         logging.info(f"Final report: {final_report}. Logged to {self.event_file_path}")
 
 
 class Recorder(RecorderBase):
     """
     A recorder which logs events to Snowflake.
     Can be used by passing `--no-local-run` when invoking `oaieval`.
     """
 
     def __init__(
         self,
         log_path: Optional[str],
-        run_spec: evals.base.RunSpec,
+        run_spec: RunSpec,
         snowflake_connection: Optional[SnowflakeConnection] = None,
     ) -> None:
         super().__init__(run_spec)
         self.event_file_path = log_path
         self._writing_lock = threading.Lock()
 
         if snowflake_connection is None:
             snowflake_connection = SnowflakeConnection()
         self._conn = snowflake_connection
 
         if log_path is not None:
-            with bf.BlobFile(log_path, "w") as f:
-                f.write(jsondumps({"spec": dataclasses.asdict(run_spec)}) + "\n")
+            with bf.BlobFile(log_path, "wb") as f:
+                f.write((jsondumps({"spec": dataclasses.asdict(run_spec)}) + "\n").encode("utf-8"))
 
         query = """
             INSERT ALL INTO runs (run_id, model_name, eval_name, base_eval, split, run_config, settings, created_by, created_at)
             VALUES (%(run_id)s, %(model_name)s, %(eval_name)s, %(base_eval)s, %(split)s, run_config, settings, %(created_by)s, %(created_at)s)
             SELECT PARSE_JSON(%(run_config)s) AS run_config, PARSE_JSON(%(settings)s) AS settings
         """
         self._conn.robust_query(
             command=query,
             params={
                 "run_id": run_spec.run_id,
-                "model_name": jsondumps(run_spec.model_names),
+                # TODO: model_name -> completion_fns
+                "model_name": jsondumps(run_spec.completion_fns),
                 "eval_name": run_spec.eval_name,
                 "base_eval": run_spec.base_eval,
                 "split": run_spec.split,
                 "run_config": jsondumps(run_spec.run_config),
                 "settings": jsondumps(run_spec.run_config.get("initial_settings", {})),
                 "created_by": run_spec.created_by,
                 "created_at": run_spec.created_at,
@@ -403,23 +404,23 @@
                 """
                 self._conn.robust_query(command=query, seqparams=buffer, many=True)
                 logger.info(
                     f"Logged {len(buffer)} rows of events to Snowflake: insert_time={t(time.time()-start)}"
                 )
                 idx_l = idx_r
 
-            with bf.BlobFile(self.event_file_path, "a") as f:
-                f.writelines(lines)
+            with bf.BlobFile(self.event_file_path, "ab") as f:
+                f.write(b"".join([l.encode("utf-8") for l in lines]))
             self._last_flush_time = time.time()
             self._flushes_done += 1
 
     def record_final_report(self, final_report: Any):
         with self._writing_lock:
-            with bf.BlobFile(self.event_file_path, "a") as f:
-                f.write(jsondumps({"final_report": final_report}) + "\n")
+            with bf.BlobFile(self.event_file_path, "ab") as f:
+                f.write((jsondumps({"final_report": final_report}) + "\n").encode("utf-8"))
             query = """
                 UPDATE runs
                 SET final_report = PARSE_JSON(%(final_report)s)
                 WHERE run_id = %(run_id)s
             """
             self._conn.robust_query(
                 command=query,
```

### Comparing `evals-0.1.1/evals/registry/evals/test-basic.yaml` & `evals-1.0.0/evals/registry/evals/test-basic.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -21,7 +21,17 @@
   id: test-includes.s1.simple-v0
   description: Example eval that uses fuzzy matching to score completions.
   metrics: [accuracy]
 test-includes.s1.simple-v0:
   class: evals.elsuite.basic.includes:Includes
   args:
     samples_jsonl: test_fuzzy_match/samples.jsonl
+
+test-includes-ignore-case:
+  id: test-includes-ignore-case.s1.simple-v0
+  description: Example eval that uses fuzzy matching to score completions.
+  metrics: [accuracy]
+test-includes-ignore-case.s1.simple-v0:
+  class: evals.elsuite.basic.includes:Includes
+  args:
+    samples_jsonl: test_fuzzy_match/samples.jsonl
+    ignore_case: true
```

### Comparing `evals-0.1.1/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-1.0.0/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -4,38 +4,39 @@
   id: joke-animals-vs-fruits.dev.v0
   metrics: [accuracy]
 joke-animals-vs-fruits.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_multiio/battles/joke_animals_vs_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: battle
+    modelgraded_spec: battle
 
 rap-people-vs-people:
   id: rap-people-vs-people.dev.v0
   metrics: [accuracy]
 rap-people-vs-people.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_multiio/battles/rap_people_vs_people.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: battle
+    modelgraded_spec: battle
 
 rap-animals-vs-fruits:
   id: rap-animals-vs-fruits.dev.v0
   metrics: [accuracy]
 rap-animals-vs-fruits.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_multiio/battles/rap_animals_vs_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: battle
+    modelgraded_spec: battle
 
 rap-people-vs-fruits:
   id: rap-people-vs-fruits.dev.v0
   metrics: [accuracy]
 rap-people-vs-fruits.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_multiio/battles/rap_people_vs_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: battle
+    modelgraded_spec: battle
+
```

### Comparing `evals-0.1.1/evals/registry/evals/test-modelgraded.yaml` & `evals-1.0.0/evals/registry/evals/test-modelgraded.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,96 @@
 # a simple modelgraded eval checking if a completion is funny or not
-joke-animals:
-  id: joke-animals.dev.v0
+joke-fruits:
+  id: joke-fruits.dev.v0
   metrics: [accuracy]
-joke-animals.dev.v0:
+joke-fruits.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
-    samples_jsonl: test_multiio/battles/joke_animals_vs_fruits.jsonl
-    samples_renamings:
-      input1: "input"
-      completion1: "completion"
+    samples_jsonl: test_modelgraded/joke_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: humor
+    modelgraded_spec: humor
 
-# (same eval as above, but with likert scale of 1-5)
-joke-animals-likert:
-  id: joke-animals-likert.dev.v0
+# (same eval as above, but with format_type="out_message")
+joke-fruits-v2:
+  id: joke-fruits-v2.dev.v0
   metrics: [accuracy]
-joke-animals-likert.dev.v0:
+joke-fruits-v2.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
-    samples_jsonl: test_multiio/battles/joke_animals_vs_fruits.jsonl
-    samples_renamings:
-      input1: "input"
-      completion1: "completion"
+    samples_jsonl: test_modelgraded/joke_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: humor_likert
+    modelgraded_spec: humor_out_message
 
-# a simple modelgraded eval checking if a completion is funny or not
-# this example uses a labeled dataset, but ignores "completion" and "choice"
-joke-fruits:
-  id: joke-fruits.dev.v0
+# (same eval as above, but with likert scale of 1-5)
+joke-fruits-likert:
+  id: joke-fruits-likert.dev.v0
   metrics: [accuracy]
-joke-fruits.dev.v0:
+joke-fruits-likert.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
-    samples_jsonl: test_metaeval/joke_fruits_labeled.jsonl
+    samples_jsonl: test_modelgraded/joke_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: humor
+    modelgraded_spec: humor_likert
 
 # a meta-evaluation of a modelgraded eval checking if a completion is funny or not
 # this example uses a labeled dataset with "completion" and "choice"
 joke-fruits-meta:
   id: joke-fruits-meta.dev.v0
   metrics: [accuracy]
 joke-fruits-meta.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_metaeval/joke_fruits_labeled.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: humor
+    modelgraded_spec: humor
     metaeval: true
 
 # (above, but with "answer then explain", rather than "reason then answer")
 joke-fruits-expl-meta:
   id: joke-fruits-expl-meta.dev.v0
   metrics: [accuracy]
 joke-fruits-expl-meta.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_metaeval/joke_fruits_labeled.jsonl
     eval_type: classify_cot
-    modelgraded_spec_file: humor
+    modelgraded_spec: humor
     metaeval: true
 
 # (above, but with "answer" only)
 joke-fruits-ans-meta:
   id: joke-fruits-ans-meta.dev.v0
   metrics: [accuracy]
 joke-fruits-ans-meta.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_metaeval/joke_fruits_labeled.jsonl
     eval_type: classify
-    modelgraded_spec_file: humor
+    modelgraded_spec: humor
     metaeval: true
 
 # a simple modelgraded eval checking if 4 completions to the sample prompt is diverse
-# this example uses a labeled dataset, but ignore "completion" and "choice"
 diversity:
   id: diversity.dev.v0
   metrics: [accuracy]
 diversity.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
-    samples_jsonl: test_metaeval/joke_fruits_labeled.jsonl
+    samples_jsonl: test_modelgraded/joke_fruits.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: diversity
+    modelgraded_spec: diversity
     multicomp_n: 4
     multicomp_temperature: 0.4
+
+# a simple modelgraded eval checking which of N completions to the sample prompt is the best response
+# command: `oaleval gpt-3.5-turbo,gpt-4 best`
+best:
+  id: best.dev.v0
+  metrics: [accuracy]
+best.dev.v0:
+  class: evals.elsuite.modelgraded.classify:ModelBasedClassify
+  args:
+    samples_jsonl: test_modelgraded/joke_fruits.jsonl
+    eval_type: cot_classify
+    modelgraded_spec: best
+    multicomp_n: from_models
+    multicomp_temperature: 0.0
```

### Comparing `evals-0.1.1/evals/registry/modelgraded/closedqa.yaml` & `evals-1.0.0/evals/registry/modelgraded/closedqa.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-prompt: |-
-  You are assessing a submitted answer on a given task based on a criterion. Here is the data:
-  [BEGIN DATA]
-  ***
-  [Task]: {input}
-  ***
-  [Submission]: {completion}
-  ***
-  [Criterion]: {criteria}
-  ***
-  [END DATA]
-  Does the submission meet the criterion? First, write out in a step by step manner your reasoning about the criterion to be sure that your conclusion is correct. Avoid simply stating the correct answers at the outset. Then print only the single character "Y" or "N" (without quotes or punctuation) on its own line corresponding to the correct answer. At the end, repeat just the letter again by itself on a new line.
+closedqa:
+  prompt: |-
+    You are assessing a submitted answer on a given task based on a criterion. Here is the data:
+    [BEGIN DATA]
+    ***
+    [Task]: {input}
+    ***
+    [Submission]: {completion}
+    ***
+    [Criterion]: {criteria}
+    ***
+    [END DATA]
+    Does the submission meet the criterion? First, write out in a step by step manner your reasoning about the criterion to be sure that your conclusion is correct. Avoid simply stating the correct answers at the outset. Then print only the single character "Y" or "N" (without quotes or punctuation) on its own line corresponding to the correct answer. At the end, repeat just the letter again by itself on a new line.
 
-  Reasoning:
-eval_type: cot_classify
-choice_scores:
-  "Y": 1.0
-  "N": 0.0
-choice_strings: 'YN'
-args:
-  criteria:
-    relevance: "relevance: Is the submission referring to a real quote from the text?"
-    conciseness: "conciseness: Is the answer concise and to the point?"
-    correct: "correctness: Is the answer correct?"
-input_outputs:
-  input: "completion"
+    Reasoning:
+  eval_type: cot_classify
+  choice_scores:
+    "Y": 1.0
+    "N": 0.0
+  choice_strings: 'YN'
+  args:
+    criteria:
+      relevance: "relevance: Is the submission referring to a real quote from the text?"
+      conciseness: "conciseness: Is the answer concise and to the point?"
+      correct: "correctness: Is the answer correct?"
+  input_outputs:
+    input: "completion"
```

### Comparing `evals-0.1.1/evals/registry/modelgraded/fact.yaml` & `evals-1.0.0/evals/registry/modelgraded/fact.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-prompt: |-
-  You are comparing a submitted answer to an expert answer on a given question. Here is the data:
-  [BEGIN DATA]
-  ************
-  [Question]: {input}
-  ************
-  [Expert]: {ideal}
-  ************
-  [Submission]: {completion}
-  ************
-  [END DATA]
+fact:
+  prompt: |-
+    You are comparing a submitted answer to an expert answer on a given question. Here is the data:
+    [BEGIN DATA]
+    ************
+    [Question]: {input}
+    ************
+    [Expert]: {ideal}
+    ************
+    [Submission]: {completion}
+    ************
+    [END DATA]
 
-  Compare the factual content of the submitted answer with the expert answer. Ignore any differences in style, grammar, or punctuation.
-  The submitted answer may either be a subset or superset of the expert answer, or it may conflict with it. Determine which case applies. Answer the question by selecting one of the following options:
-  (A) The submitted answer is a subset of the expert answer and is fully consistent with it.
-  (B) The submitted answer is a superset of the expert answer and is fully consistent with it.
-  (C) The submitted answer contains all the same details as the expert answer.
-  (D) There is a disagreement between the submitted answer and the expert answer.
-  (E) The answers differ, but these differences don't matter from the perspective of factuality.
-choice_strings: ABCDE
-input_outputs:
-  input: completion
+    Compare the factual content of the submitted answer with the expert answer. Ignore any differences in style, grammar, or punctuation.
+    The submitted answer may either be a subset or superset of the expert answer, or it may conflict with it. Determine which case applies. Answer the question by selecting one of the following options:
+    (A) The submitted answer is a subset of the expert answer and is fully consistent with it.
+    (B) The submitted answer is a superset of the expert answer and is fully consistent with it.
+    (C) The submitted answer contains all the same details as the expert answer.
+    (D) There is a disagreement between the submitted answer and the expert answer.
+    (E) The answers differ, but these differences don't matter from the perspective of factuality.
+  choice_strings: ABCDE
+  input_outputs:
+    input: completion
```

### Comparing `evals-0.1.1/evals/utils/api_utils.py` & `evals-1.0.0/evals/utils/api_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This file defines various helper functions for interacting with the OpenAI API.
 """
 import logging
 
 import backoff
 import openai
 
-
 @backoff.on_exception(
     wait_gen=backoff.expo,
     exception=(
         openai.error.ServiceUnavailableError,
         openai.error.APIError,
         openai.error.RateLimitError,
         openai.error.APIConnectionError,
```

### Comparing `evals-0.1.1/evals/utils/misc.py` & `evals-1.0.0/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-0.1.1/evals/utils/snowflake.py` & `evals-1.0.0/evals/utils/snowflake.py`

 * *Files identical despite different names*

