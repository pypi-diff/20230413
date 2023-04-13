# Comparing `tmp/shexer-2.1.1.tar.gz` & `tmp/shexer-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.1.1.tar", last modified: Fri Apr  7 09:41:47 2023, max compression
+gzip compressed data, was "shexer-2.1.2.tar", last modified: Thu Apr 13 17:30:01 2023, max compression
```

## Comparing `shexer-2.1.1.tar` & `shexer-2.1.2.tar`

### file list

```diff
@@ -1,237 +1,238 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.650612 shexer-2.1.1/
--rw-rw-rw-   0        0        0    11558 2019-11-23 19:24:24.000000 shexer-2.1.1/LICENSE
--rw-rw-rw-   0        0        0    25803 2023-04-07 09:41:47.651611 shexer-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    24887 2023-04-06 19:41:11.000000 shexer-2.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-07 09:41:47.659609 shexer-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1392 2023-04-07 09:41:11.000000 shexer-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.025611 shexer-2.1.1/shexer/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/__init__.py
--rw-rw-rw-   0        0        0      644 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/consts.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.060626 shexer-2.1.1/shexer/core/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.079611 shexer-2.1.1/shexer/core/instances/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/core/instances/__init__.py
--rw-rw-rw-   0        0        0      713 2021-10-25 09:34:37.000000 shexer-2.1.1/shexer/core/instances/abstract_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.108607 shexer-2.1.1/shexer/core/instances/annotators/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/core/instances/annotators/__init__.py
--rw-rw-rw-   0        0        0      383 2021-01-14 17:50:11.000000 shexer-2.1.1/shexer/core/instances/annotators/annotator_func.py
--rw-rw-rw-   0        0        0     1817 2021-01-14 17:50:11.000000 shexer-2.1.1/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-rw-rw-   0        0        0     3198 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/instances/annotators/base_annotator.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.173608 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/
--rw-rw-rw-   0        0        0        0 2021-01-14 17:50:11.000000 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-rw-rw-   0        0        0      688 2021-10-25 09:34:37.000000 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-rw-rw-   0        0        0      592 2021-01-14 17:50:11.000000 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-rw-rw-   0        0        0      807 2021-01-14 17:50:11.000000 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-rw-rw-   0        0        0     1793 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0      830 2021-10-25 09:34:37.000000 shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-rw-rw-   0        0        0     4260 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/instances/instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.184608 shexer-2.1.1/shexer/core/instances/mappings/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/core/instances/mappings/__init__.py
--rw-rw-rw-   0        0        0     1081 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.195608 shexer-2.1.1/shexer/core/instances/mix/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/core/instances/mix/__init__.py
--rw-rw-rw-   0        0        0     2652 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-rw-rw-   0        0        0       22 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/core/instances/pconsts.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.214610 shexer-2.1.1/shexer/core/profiling/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/profiling/__init__.py
--rw-rw-rw-   0        0        0     8614 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/profiling/class_profiler.py
--rw-rw-rw-   0        0        0      182 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/profiling/consts.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.233608 shexer-2.1.1/shexer/core/profiling/strategy/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/profiling/strategy/__init__.py
--rw-rw-rw-   0        0        0     6976 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-rw-rw-   0        0        0     1349 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-rw-rw-   0        0        0     7395 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.244608 shexer-2.1.1/shexer/core/shexing/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/shexing/__init__.py
--rw-rw-rw-   0        0        0     6110 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/class_shexer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.270608 shexer-2.1.1/shexer/core/shexing/strategy/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/core/shexing/strategy/__init__.py
--rw-rw-rw-   0        0        0    16882 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-rw-rw-   0        0        0     5685 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-rw-rw-   0        0        0     2804 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.290628 shexer-2.1.1/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-rw-rw-   0        0        0        0 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-rw-rw-   0        0        0      118 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-rw-rw-   0        0        0     1088 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-rw-rw-   0        0        0      412 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.309609 shexer-2.1.1/shexer/io/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/__init__.py
--rw-rw-rw-   0        0        0      103 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/io/file.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.311613 shexer-2.1.1/shexer/io/graph/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.407649 shexer-2.1.1/shexer/io/graph/yielder/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/graph/yielder/__init__.py
--rw-rw-rw-   0        0        0     1431 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/base_triples_yielder.py
--rw-rw-rw-   0        0        0    16303 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.419648 shexer-2.1.1/shexer/io/graph/yielder/filter/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/graph/yielder/filter/__init__.py
--rw-rw-rw-   0        0        0      862 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-rw-rw-   0        0        0     1131 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-rw-rw-   0        0        0     1132 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1757 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-rw-rw-   0        0        0     1166 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     2674 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-rw-rw-   0        0        0     5686 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-rw-rw-   0        0        0     6817 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.430610 shexer-2.1.1/shexer/io/graph/yielder/remote/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/graph/yielder/remote/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-04-03 18:35:42.000000 shexer-2.1.1/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-rw-rw-   0        0        0     4724 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.440649 shexer-2.1.1/shexer/io/json/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/json/__init__.py
--rw-rw-rw-   0        0        0      207 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/json/json_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.477609 shexer-2.1.1/shexer/io/line_reader/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/line_reader/__init__.py
--rw-rw-rw-   0        0        0      285 2021-01-14 17:50:12.000000 shexer-2.1.1/shexer/io/line_reader/file_line_reader.py
--rw-rw-rw-   0        0        0      332 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/line_reader/gz_line_reader.py
--rw-rw-rw-   0        0        0      260 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/line_reader/raw_string_line_reader.py
--rw-rw-rw-   0        0        0      353 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/io/line_reader/zip_file_line_reader.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.480621 shexer-2.1.1/shexer/io/profile/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.489608 shexer-2.1.1/shexer/io/profile/formater/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/profile/formater/__init__.py
--rw-rw-rw-   0        0        0      409 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.491609 shexer-2.1.1/shexer/io/shacl/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/io/shacl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.504609 shexer-2.1.1/shexer/io/shacl/formater/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/io/shacl/formater/__init__.py
--rw-rw-rw-   0        0        0    15833 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/io/shacl/formater/shacl_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.517629 shexer-2.1.1/shexer/io/shape_map/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shape_map/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.549615 shexer-2.1.1/shexer/io/shape_map/label/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shape_map/label/__init__.py
--rw-rw-rw-   0        0        0     1410 2021-01-14 17:50:12.000000 shexer-2.1.1/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.561611 shexer-2.1.1/shexer/io/shape_map/node_selector/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shape_map/node_selector/__init__.py
--rw-rw-rw-   0        0        0     6755 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-rw-rw-   0        0        0     4966 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shape_map/shape_map_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.563611 shexer-2.1.1/shexer/io/shex/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.577614 shexer-2.1.1/shexer/io/shex/formater/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shex/formater/__init__.py
--rw-rw-rw-   0        0        0      244 2021-01-14 17:50:12.000000 shexer-2.1.1/shexer/io/shex/formater/consts.py
--rw-rw-rw-   0        0        0     7006 2023-04-07 09:41:11.000000 shexer-2.1.1/shexer/io/shex/formater/shex_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.631629 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-rw-rw-   0        0        0     6014 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-rw-rw-   0        0        0     2287 2023-02-03 19:09:46.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.675612 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-rw-rw-   0        0        0        0 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-rw-rw-   0        0        0      383 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-rw-rw-   0        0        0      171 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-rw-rw-   0        0        0      887 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-rw-rw-   0        0        0     1278 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-rw-rw-   0        0        0     1500 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-rw-rw-   0        0        0     3211 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.687612 shexer-2.1.1/shexer/io/sparql/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/io/sparql/__init__.py
--rw-rw-rw-   0        0        0     4538 2022-07-15 19:02:46.000000 shexer-2.1.1/shexer/io/sparql/query.py
--rw-rw-rw-   0        0        0      469 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/io/wikidata.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.804610 shexer-2.1.1/shexer/model/
--rw-rw-rw-   0        0        0      552 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/IRI.py
--rw-rw-rw-   0        0        0      280 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/Literal.py
--rw-rw-rw-   0        0        0      810 2021-01-14 17:50:12.000000 shexer-2.1.1/shexer/model/Macro.py
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/__init__.py
--rw-rw-rw-   0        0        0      502 2021-10-04 17:33:25.000000 shexer-2.1.1/shexer/model/bnode.py
--rw-rw-rw-   0        0        0      100 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/const_elem_types.py
--rw-rw-rw-   0        0        0     1119 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/model/fixed_prop_choice_statement.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.839610 shexer-2.1.1/shexer/model/graph/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/graph/__init__.py
--rw-rw-rw-   0        0        0     6186 2022-07-15 19:02:46.000000 shexer-2.1.1/shexer/model/graph/abstract_sgraph.py
--rw-rw-rw-   0        0        0     7633 2023-04-04 10:53:17.000000 shexer-2.1.1/shexer/model/graph/endpoint_sgraph.py
--rw-rw-rw-   0        0        0     6201 2023-04-04 17:24:52.000000 shexer-2.1.1/shexer/model/graph/rdflib_sgraph.py
--rw-rw-rw-   0        0        0     4173 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/hierarchy_tree.py
--rw-rw-rw-   0        0        0     2527 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/node_selector.py
--rw-rw-rw-   0        0        0      427 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/property.py
--rw-rw-rw-   0        0        0     3361 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/model/shape.py
--rw-rw-rw-   0        0        0      858 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/model/shape_map.py
--rw-rw-rw-   0        0        0     2716 2023-02-02 16:28:05.000000 shexer-2.1.1/shexer/model/statement.py
--rw-rw-rw-   0        0        0    23678 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/shaper.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.925612 shexer-2.1.1/shexer/utils/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/__init__.py
--rw-rw-rw-   0        0        0      621 2022-08-11 11:37:45.000000 shexer-2.1.1/shexer/utils/compression.py
--rw-rw-rw-   0        0        0       94 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/dict.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.011611 shexer-2.1.1/shexer/utils/factories/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/factories/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/utils/factories/class_profiler_factory.py
--rw-rw-rw-   0        0        0     2226 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/utils/factories/class_shexer_factory.py
--rw-rw-rw-   0        0        0      728 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/factories/h_tree.py
--rw-rw-rw-   0        0        0    12215 2023-04-04 10:53:17.000000 shexer-2.1.1/shexer/utils/factories/instance_tracker_factory.py
--rw-rw-rw-   0        0        0      437 2021-10-03 10:32:18.000000 shexer-2.1.1/shexer/utils/factories/iri_factory.py
--rw-rw-rw-   0        0        0      286 2021-01-14 17:50:12.000000 shexer-2.1.1/shexer/utils/factories/remote_graph_factory.py
--rw-rw-rw-   0        0        0     1985 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/utils/factories/shape_map_factory.py
--rw-rw-rw-   0        0        0      616 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/factories/shape_map_parser_factory.py
--rw-rw-rw-   0        0        0     1723 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/utils/factories/shape_serializer_factory.py
--rw-rw-rw-   0        0        0    18627 2023-04-04 10:53:17.000000 shexer-2.1.1/shexer/utils/factories/triple_yielders_factory.py
--rw-rw-rw-   0        0        0      123 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/file.py
--rw-rw-rw-   0        0        0      397 2021-10-04 17:33:25.000000 shexer-2.1.1/shexer/utils/log.py
--rw-rw-rw-   0        0        0      803 2021-01-14 17:50:12.000000 shexer-2.1.1/shexer/utils/namespaces.py
--rw-rw-rw-   0        0        0      967 2019-11-23 19:24:28.000000 shexer-2.1.1/shexer/utils/obj_references.py
--rw-rw-rw-   0        0        0     2008 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/utils/shapes.py
--rw-rw-rw-   0        0        0     1397 2022-03-28 20:28:03.000000 shexer-2.1.1/shexer/utils/target_elements.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.022612 shexer-2.1.1/shexer/utils/translators/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.1/shexer/utils/translators/__init__.py
--rw-rw-rw-   0        0        0     2881 2021-04-26 09:52:52.000000 shexer-2.1.1/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-rw-rw-   0        0        0     3026 2023-04-03 15:39:42.000000 shexer-2.1.1/shexer/utils/triple_yielders.py
--rw-rw-rw-   0        0        0     5511 2023-04-06 19:32:13.000000 shexer-2.1.1/shexer/utils/uri.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:46.057610 shexer-2.1.1/shexer.egg-info/
--rw-rw-rw-   0        0        0    25803 2023-04-07 09:41:45.000000 shexer-2.1.1/shexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7726 2023-04-07 09:41:45.000000 shexer-2.1.1/shexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:41:45.000000 shexer-2.1.1/shexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-07 09:41:45.000000 shexer-2.1.1/shexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-07 09:41:45.000000 shexer-2.1.1/shexer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.561611 shexer-2.1.1/test/
--rw-rw-rw-   0        0        0        0 2021-01-14 17:50:12.000000 shexer-2.1.1/test/__init__.py
--rw-rw-rw-   0        0        0     1903 2021-11-20 10:36:36.000000 shexer-2.1.1/test/const.py
--rw-rw-rw-   0        0        0     8963 2023-04-03 18:35:42.000000 shexer-2.1.1/test/t_utils.py
--rw-rw-rw-   0        0        0     1488 2022-08-10 11:13:26.000000 shexer-2.1.1/test/test_all_classes_mode.py
--rw-rw-rw-   0        0        0     1525 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_allow_opt_cardinality.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.574610 shexer-2.1.1/test/test_bugs/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.1/test/test_bugs/__init__.py
--rw-rw-rw-   0        0        0      796 2022-03-28 20:28:03.000000 shexer-2.1.1/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-rw-rw-   0        0        0     9920 2022-08-11 11:37:45.000000 shexer-2.1.1/test/test_compression_mode.py
--rw-rw-rw-   0        0        0     2171 2023-02-02 16:28:05.000000 shexer-2.1.1/test/test_decimals.py
--rw-rw-rw-   0        0        0     5564 2023-04-03 18:13:21.000000 shexer-2.1.1/test/test_depth_for_building_subgraph.py
--rw-rw-rw-   0        0        0     3526 2023-04-06 19:32:13.000000 shexer-2.1.1/test/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0     1388 2023-02-02 16:28:05.000000 shexer-2.1.1/test/test_disable_comments.py
--rw-rw-rw-   0        0        0     2922 2023-04-04 10:53:17.000000 shexer-2.1.1/test/test_disable_endpoint_cache.py
--rw-rw-rw-   0        0        0     1491 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_disable_exact_cardinality.py
--rw-rw-rw-   0        0        0     2552 2023-04-03 18:35:42.000000 shexer-2.1.1/test/test_disable_or_statements.py
--rw-rw-rw-   0        0        0     3786 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_discard_and_compliant.py
--rw-rw-rw-   0        0        0     2090 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_file_target_classes.py
--rw-rw-rw-   0        0        0     1677 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_graph_file_input.py
--rw-rw-rw-   0        0        0     3456 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_graph_list_of_file_inputs.py
--rw-rw-rw-   0        0        0     1951 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_infer_numeric_types_for_untyped_literals.py
--rw-rw-rw-   0        0        0     7818 2023-02-02 16:28:05.000000 shexer-2.1.1/test/test_input_format.py
--rw-rw-rw-   0        0        0     3367 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_instances_file_input.py
--rw-rw-rw-   0        0        0     3852 2023-02-02 16:28:05.000000 shexer-2.1.1/test/test_instances_report.py
--rw-rw-rw-   0        0        0     3548 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_instantiation_property.py
--rw-rw-rw-   0        0        0     1964 2022-03-28 20:28:03.000000 shexer-2.1.1/test/test_inverse_paths.py
--rw-rw-rw-   0        0        0     3594 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_keep_less_specific.py
--rw-rw-rw-   0        0        0     4051 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_list_of_url_input.py
--rw-rw-rw-   0        0        0     4106 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_namespaces_dict.py
--rw-rw-rw-   0        0        0     2082 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_namespaces_to_ignore.py
--rw-rw-rw-   0        0        0     5000 2021-01-14 17:50:12.000000 shexer-2.1.1/test/test_raw_graph.py
--rw-rw-rw-   0        0        0     4300 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_raw_shape_map.py
--rw-rw-rw-   0        0        0     1711 2022-07-15 19:02:46.000000 shexer-2.1.1/test/test_rdflib_graph.py
--rw-rw-rw-   0        0        0     2930 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_remove_empty_sahpes.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.625611 shexer-2.1.1/test/test_shacl/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.1/test/test_shacl/__init__.py
--rw-rw-rw-   0        0        0     2225 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_shacl/test_annotation.py
--rw-rw-rw-   0        0        0     2242 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_shacl/test_class_selection.py
--rw-rw-rw-   0        0        0     3291 2023-04-06 19:32:13.000000 shexer-2.1.1/test/test_shacl/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0      910 2022-03-28 20:28:03.000000 shexer-2.1.1/test/test_shacl/test_literal_types.py
--rw-rw-rw-   0        0        0     4313 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_shape_map_file.py
--rw-rw-rw-   0        0        0     6086 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_shape_map_format.py
--rw-rw-rw-   0        0        0     2307 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0     2889 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_shapes_namespaces.py
--rw-rw-rw-   0        0        0     2452 2022-03-28 20:28:03.000000 shexer-2.1.1/test/test_sort.py
--rw-rw-rw-   0        0        0     2058 2021-10-24 17:07:37.000000 shexer-2.1.1/test/test_target_classes.py
--rw-rw-rw-   0        0        0     3120 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_threshold.py
--rw-rw-rw-   0        0        0     2578 2023-04-03 18:13:27.000000 shexer-2.1.1/test/test_url_endpoint.py
--rw-rw-rw-   0        0        0     1867 2022-07-15 19:02:46.000000 shexer-2.1.1/test/test_url_graph.py
--rw-rw-rw-   0        0        0     1900 2021-10-03 10:32:18.000000 shexer-2.1.1/test/test_wikidata_annotation.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:41:47.649613 shexer-2.1.1/ws/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.1/ws/__init__.py
--rw-rw-rw-   0        0        0    19884 2022-03-28 20:28:03.000000 shexer-2.1.1/ws/shexer_rest.py
--rw-rw-rw-   0        0        0       28 2019-11-23 19:24:29.000000 shexer-2.1.1/ws/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.958874 shexer-2.1.2/
+-rw-rw-rw-   0        0        0    11558 2019-11-23 19:24:24.000000 shexer-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0    25803 2023-04-13 17:30:01.958874 shexer-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    24887 2023-04-06 19:41:11.000000 shexer-2.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-13 17:30:01.961871 shexer-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-04-13 17:29:20.000000 shexer-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:29:59.985873 shexer-2.1.2/shexer/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/consts.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.027882 shexer-2.1.2/shexer/core/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.111872 shexer-2.1.2/shexer/core/instances/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/__init__.py
+-rw-rw-rw-   0        0        0      713 2021-10-25 09:34:37.000000 shexer-2.1.2/shexer/core/instances/abstract_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.190873 shexer-2.1.2/shexer/core/instances/annotators/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/annotators/__init__.py
+-rw-rw-rw-   0        0        0      383 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/annotator_func.py
+-rw-rw-rw-   0        0        0     1817 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-rw-rw-   0        0        0     3198 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/annotators/base_annotator.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.297873 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/
+-rw-rw-rw-   0        0        0        0 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-rw-rw-   0        0        0      688 2021-10-25 09:34:37.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-rw-rw-   0        0        0      592 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-rw-rw-   0        0        0      807 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-rw-rw-   0        0        0     1793 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0      830 2021-10-25 09:34:37.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-rw-rw-   0        0        0     4260 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.309874 shexer-2.1.2/shexer/core/instances/mappings/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/mappings/__init__.py
+-rw-rw-rw-   0        0        0     1081 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.330873 shexer-2.1.2/shexer/core/instances/mix/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/mix/__init__.py
+-rw-rw-rw-   0        0        0     2652 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-rw-rw-   0        0        0       22 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/pconsts.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.364914 shexer-2.1.2/shexer/core/profiling/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/profiling/__init__.py
+-rw-rw-rw-   0        0        0     8614 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/class_profiler.py
+-rw-rw-rw-   0        0        0      182 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/profiling/consts.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.431928 shexer-2.1.2/shexer/core/profiling/strategy/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/profiling/strategy/__init__.py
+-rw-rw-rw-   0        0        0     6976 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-rw-rw-   0        0        0     1349 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-rw-rw-   0        0        0     7395 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.436872 shexer-2.1.2/shexer/core/shexing/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/shexing/__init__.py
+-rw-rw-rw-   0        0        0     6110 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/class_shexer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.480914 shexer-2.1.2/shexer/core/shexing/strategy/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/shexing/strategy/__init__.py
+-rw-rw-rw-   0        0        0    16882 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-rw-rw-   0        0        0     5685 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-rw-rw-   0        0        0     2804 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.530870 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-rw-rw-   0        0        0        0 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-rw-rw-   0        0        0     1088 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-rw-rw-   0        0        0      412 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.551875 shexer-2.1.2/shexer/io/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/__init__.py
+-rw-rw-rw-   0        0        0      103 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.553876 shexer-2.1.2/shexer/io/graph/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.750869 shexer-2.1.2/shexer/io/graph/yielder/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/__init__.py
+-rw-rw-rw-   0        0        0     1431 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-rw-rw-   0        0        0    16303 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.775871 shexer-2.1.2/shexer/io/graph/yielder/filter/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/filter/__init__.py
+-rw-rw-rw-   0        0        0      862 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-rw-rw-   0        0        0     1131 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-rw-rw-   0        0        0     1132 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1757 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-rw-rw-   0        0        0     1166 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     2674 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-rw-rw-   0        0        0     5686 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     6817 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.806873 shexer-2.1.2/shexer/io/graph/yielder/remote/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/remote/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-04-03 18:35:42.000000 shexer-2.1.2/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-rw-rw-   0        0        0     4724 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.817871 shexer-2.1.2/shexer/io/json/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/json/__init__.py
+-rw-rw-rw-   0        0        0      207 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/json/json_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.875872 shexer-2.1.2/shexer/io/line_reader/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/line_reader/__init__.py
+-rw-rw-rw-   0        0        0      285 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/io/line_reader/file_line_reader.py
+-rw-rw-rw-   0        0        0      332 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/line_reader/gz_line_reader.py
+-rw-rw-rw-   0        0        0      260 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/line_reader/raw_string_line_reader.py
+-rw-rw-rw-   0        0        0      353 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/line_reader/zip_file_line_reader.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.877873 shexer-2.1.2/shexer/io/profile/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.889871 shexer-2.1.2/shexer/io/profile/formater/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/profile/formater/__init__.py
+-rw-rw-rw-   0        0        0      409 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.892879 shexer-2.1.2/shexer/io/shacl/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/shacl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.913872 shexer-2.1.2/shexer/io/shacl/formater/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/shacl/formater/__init__.py
+-rw-rw-rw-   0        0        0    15833 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/io/shacl/formater/shacl_serializer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.934870 shexer-2.1.2/shexer/io/shape_map/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.961871 shexer-2.1.2/shexer/io/shape_map/label/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/label/__init__.py
+-rw-rw-rw-   0        0        0     1410 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.978913 shexer-2.1.2/shexer/io/shape_map/node_selector/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/node_selector/__init__.py
+-rw-rw-rw-   0        0        0     6755 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-rw-rw-   0        0        0     4966 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/shape_map_parser.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.981871 shexer-2.1.2/shexer/io/shex/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.012871 shexer-2.1.2/shexer/io/shex/formater/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shex/formater/__init__.py
+-rw-rw-rw-   0        0        0      244 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/io/shex/formater/consts.py
+-rw-rw-rw-   0        0        0     7006 2023-04-07 09:41:11.000000 shexer-2.1.2/shexer/io/shex/formater/shex_serializer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.100872 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-rw-rw-   0        0        0     6083 2023-04-13 17:29:20.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-rw-rw-   0        0        0     2287 2023-02-03 19:09:46.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.161871 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-rw-rw-   0        0        0        0 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-rw-rw-   0        0        0      171 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-rw-rw-   0        0        0      887 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-rw-rw-   0        0        0     1278 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-rw-rw-   0        0        0     1500 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-rw-rw-   0        0        0     3211 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.182871 shexer-2.1.2/shexer/io/sparql/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/sparql/__init__.py
+-rw-rw-rw-   0        0        0     4538 2022-07-15 19:02:46.000000 shexer-2.1.2/shexer/io/sparql/query.py
+-rw-rw-rw-   0        0        0      469 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/wikidata.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.348910 shexer-2.1.2/shexer/model/
+-rw-rw-rw-   0        0        0      552 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/IRI.py
+-rw-rw-rw-   0        0        0      280 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/Literal.py
+-rw-rw-rw-   0        0        0      810 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/model/Macro.py
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/__init__.py
+-rw-rw-rw-   0        0        0      502 2021-10-04 17:33:25.000000 shexer-2.1.2/shexer/model/bnode.py
+-rw-rw-rw-   0        0        0      100 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/const_elem_types.py
+-rw-rw-rw-   0        0        0     1119 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/model/fixed_prop_choice_statement.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.437878 shexer-2.1.2/shexer/model/graph/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/graph/__init__.py
+-rw-rw-rw-   0        0        0     6186 2022-07-15 19:02:46.000000 shexer-2.1.2/shexer/model/graph/abstract_sgraph.py
+-rw-rw-rw-   0        0        0     7633 2023-04-04 10:53:17.000000 shexer-2.1.2/shexer/model/graph/endpoint_sgraph.py
+-rw-rw-rw-   0        0        0     6201 2023-04-04 17:24:52.000000 shexer-2.1.2/shexer/model/graph/rdflib_sgraph.py
+-rw-rw-rw-   0        0        0     4173 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/hierarchy_tree.py
+-rw-rw-rw-   0        0        0     2527 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/node_selector.py
+-rw-rw-rw-   0        0        0      427 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/property.py
+-rw-rw-rw-   0        0        0     3361 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/model/shape.py
+-rw-rw-rw-   0        0        0      858 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/shape_map.py
+-rw-rw-rw-   0        0        0     2716 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/model/statement.py
+-rw-rw-rw-   0        0        0    23678 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/shaper.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.583874 shexer-2.1.2/shexer/utils/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/__init__.py
+-rw-rw-rw-   0        0        0      621 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/utils/compression.py
+-rw-rw-rw-   0        0        0       94 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/dict.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.760872 shexer-2.1.2/shexer/utils/factories/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/factories/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/utils/factories/class_profiler_factory.py
+-rw-rw-rw-   0        0        0     2226 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/utils/factories/class_shexer_factory.py
+-rw-rw-rw-   0        0        0      728 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/factories/h_tree.py
+-rw-rw-rw-   0        0        0    12215 2023-04-04 10:53:17.000000 shexer-2.1.2/shexer/utils/factories/instance_tracker_factory.py
+-rw-rw-rw-   0        0        0      437 2021-10-03 10:32:18.000000 shexer-2.1.2/shexer/utils/factories/iri_factory.py
+-rw-rw-rw-   0        0        0      286 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/utils/factories/remote_graph_factory.py
+-rw-rw-rw-   0        0        0     1985 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/utils/factories/shape_map_factory.py
+-rw-rw-rw-   0        0        0      616 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/factories/shape_map_parser_factory.py
+-rw-rw-rw-   0        0        0     1723 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/utils/factories/shape_serializer_factory.py
+-rw-rw-rw-   0        0        0    18627 2023-04-04 10:53:17.000000 shexer-2.1.2/shexer/utils/factories/triple_yielders_factory.py
+-rw-rw-rw-   0        0        0      123 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/file.py
+-rw-rw-rw-   0        0        0      397 2021-10-04 17:33:25.000000 shexer-2.1.2/shexer/utils/log.py
+-rw-rw-rw-   0        0        0      803 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/utils/namespaces.py
+-rw-rw-rw-   0        0        0      967 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/obj_references.py
+-rw-rw-rw-   0        0        0     2008 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/utils/shapes.py
+-rw-rw-rw-   0        0        0     1397 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/utils/target_elements.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.789874 shexer-2.1.2/shexer/utils/translators/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.2/shexer/utils/translators/__init__.py
+-rw-rw-rw-   0        0        0     2881 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-rw-rw-   0        0        0     3026 2023-04-03 15:39:42.000000 shexer-2.1.2/shexer/utils/triple_yielders.py
+-rw-rw-rw-   0        0        0     5708 2023-04-13 17:29:20.000000 shexer-2.1.2/shexer/utils/uri.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.025872 shexer-2.1.2/shexer.egg-info/
+-rw-rw-rw-   0        0        0    25803 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7785 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.899875 shexer-2.1.2/test/
+-rw-rw-rw-   0        0        0        0 2021-01-14 17:50:12.000000 shexer-2.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0     1903 2021-11-20 10:36:36.000000 shexer-2.1.2/test/const.py
+-rw-rw-rw-   0        0        0     8963 2023-04-03 18:35:42.000000 shexer-2.1.2/test/t_utils.py
+-rw-rw-rw-   0        0        0     1488 2022-08-10 11:13:26.000000 shexer-2.1.2/test/test_all_classes_mode.py
+-rw-rw-rw-   0        0        0     1525 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_allow_opt_cardinality.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.906875 shexer-2.1.2/test/test_bugs/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_bugs/__init__.py
+-rw-rw-rw-   0        0        0      796 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-rw-rw-   0        0        0     1192 2023-04-13 17:29:20.000000 shexer-2.1.2/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-rw-rw-   0        0        0     9920 2022-08-11 11:37:45.000000 shexer-2.1.2/test/test_compression_mode.py
+-rw-rw-rw-   0        0        0     2171 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_decimals.py
+-rw-rw-rw-   0        0        0     5564 2023-04-03 18:13:21.000000 shexer-2.1.2/test/test_depth_for_building_subgraph.py
+-rw-rw-rw-   0        0        0     3526 2023-04-13 15:42:15.000000 shexer-2.1.2/test/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0     1388 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_disable_comments.py
+-rw-rw-rw-   0        0        0     2922 2023-04-04 10:53:17.000000 shexer-2.1.2/test/test_disable_endpoint_cache.py
+-rw-rw-rw-   0        0        0     1491 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_disable_exact_cardinality.py
+-rw-rw-rw-   0        0        0     2552 2023-04-03 18:35:42.000000 shexer-2.1.2/test/test_disable_or_statements.py
+-rw-rw-rw-   0        0        0     3786 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_discard_and_compliant.py
+-rw-rw-rw-   0        0        0     2090 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_file_target_classes.py
+-rw-rw-rw-   0        0        0     1677 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_graph_file_input.py
+-rw-rw-rw-   0        0        0     3456 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_graph_list_of_file_inputs.py
+-rw-rw-rw-   0        0        0     1951 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-rw-rw-   0        0        0     7818 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_input_format.py
+-rw-rw-rw-   0        0        0     3367 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_instances_file_input.py
+-rw-rw-rw-   0        0        0     3852 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_instances_report.py
+-rw-rw-rw-   0        0        0     3548 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_instantiation_property.py
+-rw-rw-rw-   0        0        0     1964 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_inverse_paths.py
+-rw-rw-rw-   0        0        0     3594 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_keep_less_specific.py
+-rw-rw-rw-   0        0        0     4051 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_list_of_url_input.py
+-rw-rw-rw-   0        0        0     4106 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_namespaces_dict.py
+-rw-rw-rw-   0        0        0     2082 2023-04-13 17:23:12.000000 shexer-2.1.2/test/test_namespaces_to_ignore.py
+-rw-rw-rw-   0        0        0     5000 2021-01-14 17:50:12.000000 shexer-2.1.2/test/test_raw_graph.py
+-rw-rw-rw-   0        0        0     4300 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_raw_shape_map.py
+-rw-rw-rw-   0        0        0     1711 2022-07-15 19:02:46.000000 shexer-2.1.2/test/test_rdflib_graph.py
+-rw-rw-rw-   0        0        0     2930 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_remove_empty_sahpes.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.917874 shexer-2.1.2/test/test_shacl/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.2/test/test_shacl/__init__.py
+-rw-rw-rw-   0        0        0     2225 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shacl/test_annotation.py
+-rw-rw-rw-   0        0        0     2242 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shacl/test_class_selection.py
+-rw-rw-rw-   0        0        0     3291 2023-04-06 19:32:13.000000 shexer-2.1.2/test/test_shacl/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0      910 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_shacl/test_literal_types.py
+-rw-rw-rw-   0        0        0     4313 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shape_map_file.py
+-rw-rw-rw-   0        0        0     6086 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shape_map_format.py
+-rw-rw-rw-   0        0        0     2307 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0     2889 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shapes_namespaces.py
+-rw-rw-rw-   0        0        0     2452 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_sort.py
+-rw-rw-rw-   0        0        0     2058 2021-10-24 17:07:37.000000 shexer-2.1.2/test/test_target_classes.py
+-rw-rw-rw-   0        0        0     3120 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_threshold.py
+-rw-rw-rw-   0        0        0     2578 2023-04-03 18:13:27.000000 shexer-2.1.2/test/test_url_endpoint.py
+-rw-rw-rw-   0        0        0     1867 2022-07-15 19:02:46.000000 shexer-2.1.2/test/test_url_graph.py
+-rw-rw-rw-   0        0        0     1900 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_wikidata_annotation.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.956872 shexer-2.1.2/ws/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.2/ws/__init__.py
+-rw-rw-rw-   0        0        0    19884 2022-03-28 20:28:03.000000 shexer-2.1.2/ws/shexer_rest.py
+-rw-rw-rw-   0        0        0       28 2019-11-23 19:24:29.000000 shexer-2.1.2/ws/wsgi.py
```

### Comparing `shexer-2.1.1/LICENSE` & `shexer-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/PKG-INFO` & `shexer-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.1.1
+Version: 2.1.2
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.1.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.2.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `shexer-2.1.1/README.md` & `shexer-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/setup.py` & `shexer-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.1.1',
+  version = '2.1.2',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.1.1.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.1.2.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `shexer-2.1.1/shexer/consts.py` & `shexer-2.1.2/shexer/consts.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.1.2/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.1.2/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.1.2/shexer/core/instances/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py` & `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/instance_tracker.py` & `shexer-2.1.2/shexer/core/instances/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/mappings/shape_map_instance_tracker.py` & `shexer-2.1.2/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.1.2/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/profiling/class_profiler.py` & `shexer-2.1.2/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.1.2/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.1.2/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.1.2/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/shexing/class_shexer.py` & `shexer-2.1.2/shexer/core/shexing/class_shexer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.1.2/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.1.2/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.1.2/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.1.2/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.1.2/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.1.2/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.1.2/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.1.2/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.1.2/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,16 +78,18 @@
         :param uri:
         :param namespaces_dict:
         :return:
         """
         best_match = None
         for a_namespace in namespaces_dict:  # Prefixed element (all literals are prefixed elements)
             if uri.startswith(a_namespace):
-                if best_match is None or len(best_match) < len(a_namespace):
+                if "/" not in uri[len(a_namespace):] and \
+                        "#" not in uri[len(a_namespace):]:
                     best_match = a_namespace
+                    break
 
         return None if best_match is None else uri.replace(best_match, namespaces_dict[best_match] + ":")
 
 
     def probability_representation(self, statement):
         return COMMENT_INI + self._frequency_serializer.serialize_frequency(statement)
```

### Comparing `shexer-2.1.1/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/io/sparql/query.py` & `shexer-2.1.2/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/IRI.py` & `shexer-2.1.2/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/Macro.py` & `shexer-2.1.2/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.1.2/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/graph/abstract_sgraph.py` & `shexer-2.1.2/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.1.2/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.1.2/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/hierarchy_tree.py` & `shexer-2.1.2/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/node_selector.py` & `shexer-2.1.2/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/shape.py` & `shexer-2.1.2/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/shape_map.py` & `shexer-2.1.2/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/model/statement.py` & `shexer-2.1.2/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/shaper.py` & `shexer-2.1.2/shexer/shaper.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/compression.py` & `shexer-2.1.2/shexer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.1.2/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.1.2/shexer/utils/factories/class_shexer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/h_tree.py` & `shexer-2.1.2/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.1.2/shexer/utils/factories/instance_tracker_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/shape_map_factory.py` & `shexer-2.1.2/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.1.2/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.1.2/shexer/utils/factories/shape_serializer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.1.2/shexer/utils/factories/triple_yielders_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/namespaces.py` & `shexer-2.1.2/shexer/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/obj_references.py` & `shexer-2.1.2/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/shapes.py` & `shexer-2.1.2/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/target_elements.py` & `shexer-2.1.2/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.1.2/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/triple_yielders.py` & `shexer-2.1.2/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/shexer/utils/uri.py` & `shexer-2.1.2/shexer/utils/uri.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,20 @@
 
 
 def prefixize_uri_if_possible(target_uri, namespaces_prefix_dict):
     best_match = None
     candidate_uri = remove_corners(target_uri)
     for a_namespace in namespaces_prefix_dict:  # Prefixed element (all literals are prefixed elements)
         if candidate_uri.startswith(a_namespace):
-            if best_match is None or len(best_match) < len(a_namespace):
+            if "/" not in candidate_uri[len(a_namespace):] and \
+                "#" not in candidate_uri[len(a_namespace):]:
                 best_match = a_namespace
+                break
+            # if best_match is None or len(best_match) < len(a_namespace):
+            #     best_match = a_namespace
 
     return target_uri if best_match is None else candidate_uri.replace(best_match, namespaces_prefix_dict[best_match] + ":")
```

### Comparing `shexer-2.1.1/shexer.egg-info/PKG-INFO` & `shexer-2.1.2/shexer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.1.1
+Version: 2.1.2
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.1.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.2.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `shexer-2.1.1/shexer.egg-info/SOURCES.txt` & `shexer-2.1.2/shexer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 test/test_target_classes.py
 test/test_threshold.py
 test/test_url_endpoint.py
 test/test_url_graph.py
 test/test_wikidata_annotation.py
 test/test_bugs/__init__.py
 test/test_bugs/test_no_sharp_in_auto_shape_names.py
+test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
 test/test_shacl/__init__.py
 test/test_shacl/test_annotation.py
 test/test_shacl/test_class_selection.py
 test/test_shacl/test_detect_minimal_iri.py
 test/test_shacl/test_literal_types.py
 ws/__init__.py
 ws/shexer_rest.py
```

### Comparing `shexer-2.1.1/test/const.py` & `shexer-2.1.2/test/const.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/t_utils.py` & `shexer-2.1.2/test/t_utils.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_all_classes_mode.py` & `shexer-2.1.2/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_allow_opt_cardinality.py` & `shexer-2.1.2/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.1.2/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_compression_mode.py` & `shexer-2.1.2/test/test_compression_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_decimals.py` & `shexer-2.1.2/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_depth_for_building_subgraph.py` & `shexer-2.1.2/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_detect_minimal_iri.py` & `shexer-2.1.2/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_disable_comments.py` & `shexer-2.1.2/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_disable_endpoint_cache.py` & `shexer-2.1.2/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_disable_exact_cardinality.py` & `shexer-2.1.2/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_disable_or_statements.py` & `shexer-2.1.2/test/test_disable_or_statements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_discard_and_compliant.py` & `shexer-2.1.2/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_file_target_classes.py` & `shexer-2.1.2/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_graph_file_input.py` & `shexer-2.1.2/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_graph_list_of_file_inputs.py` & `shexer-2.1.2/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.1.2/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_input_format.py` & `shexer-2.1.2/test/test_input_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_instances_file_input.py` & `shexer-2.1.2/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_instances_report.py` & `shexer-2.1.2/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_instantiation_property.py` & `shexer-2.1.2/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_inverse_paths.py` & `shexer-2.1.2/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_keep_less_specific.py` & `shexer-2.1.2/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_list_of_url_input.py` & `shexer-2.1.2/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_namespaces_dict.py` & `shexer-2.1.2/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_namespaces_to_ignore.py` & `shexer-2.1.2/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_raw_graph.py` & `shexer-2.1.2/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_raw_shape_map.py` & `shexer-2.1.2/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_rdflib_graph.py` & `shexer-2.1.2/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_remove_empty_sahpes.py` & `shexer-2.1.2/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shacl/test_annotation.py` & `shexer-2.1.2/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shacl/test_class_selection.py` & `shexer-2.1.2/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.1.2/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shacl/test_literal_types.py` & `shexer-2.1.2/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shape_map_file.py` & `shexer-2.1.2/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shape_map_format.py` & `shexer-2.1.2/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shape_qualifiers_mode.py` & `shexer-2.1.2/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_shapes_namespaces.py` & `shexer-2.1.2/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_sort.py` & `shexer-2.1.2/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_target_classes.py` & `shexer-2.1.2/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_threshold.py` & `shexer-2.1.2/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_url_endpoint.py` & `shexer-2.1.2/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_url_graph.py` & `shexer-2.1.2/test/test_url_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/test/test_wikidata_annotation.py` & `shexer-2.1.2/test/test_wikidata_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.1/ws/shexer_rest.py` & `shexer-2.1.2/ws/shexer_rest.py`

 * *Files identical despite different names*

