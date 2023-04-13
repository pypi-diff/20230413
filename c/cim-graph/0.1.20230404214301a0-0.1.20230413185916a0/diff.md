# Comparing `tmp/cim_graph-0.1.20230404214301a0.tar.gz` & `tmp/cim_graph-0.1.20230413185916a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_graph-0.1.20230404214301a0.tar", max compression
+gzip compressed data, was "cim_graph-0.1.20230413185916a0.tar", max compression
```

## Comparing `cim_graph-0.1.20230404214301a0.tar` & `cim_graph-0.1.20230413185916a0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     4896 2023-04-04 21:42:05.662585 cim_graph-0.1.20230404214301a0/README.md
--rw-r--r--   0        0        0        0 2023-04-04 21:42:05.662585 cim_graph-0.1.20230404214301a0/cimgraph/__init__.py
--rw-r--r--   0        0        0      105 2023-04-04 21:42:05.662585 cim_graph-0.1.20230404214301a0/cimgraph/data_profile/__init__.py
--rw-r--r--   0        0        0     9401 2023-04-04 21:42:05.662585 cim_graph-0.1.20230404214301a0/cimgraph/data_profile/cimext_2022/__init__.py
--rw-r--r--   0        0        0   370766 2023-04-04 21:42:05.666585 cim_graph-0.1.20230404214301a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
--rw-r--r--   0        0        0    24601 2023-04-04 21:42:05.666585 cim_graph-0.1.20230404214301a0/cimgraph/data_profile/rc4_2021/__init__.py
--rw-r--r--   0        0        0   835023 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
--rw-r--r--   0        0        0     1063 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/__init__.py
--rw-r--r--   0        0        0      352 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/blazegraph/__init__.py
--rw-r--r--   0        0        0     9111 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/blazegraph/blazegraph.py
--rw-r--r--   0        0        0     2797 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/blazegraph/query_parsers.py
--rw-r--r--   0        0        0    10314 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/gridappsd/__init__.py
--rw-r--r--   0        0        0     4138 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/__init__.py
--rw-r--r--   0        0        0     1492 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
--rw-r--r--   0        0        0     3711 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
--rw-r--r--   0        0        0     3156 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
--rw-r--r--   0        0        0     2646 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/analog.py
--rw-r--r--   0        0        0     1483 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/asset.py
--rw-r--r--   0        0        0      885 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py
--rw-r--r--   0        0        0     1491 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
--rw-r--r--   0        0        0     3141 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
--rw-r--r--   0        0        0     3041 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/breaker.py
--rw-r--r--   0        0        0     2795 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py
--rw-r--r--   0        0        0     5482 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
--rw-r--r--   0        0        0     2667 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py
--rw-r--r--   0        0        0     2650 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/discrete.py
--rw-r--r--   0        0        0     3155 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
--rw-r--r--   0        0        0     2176 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
--rw-r--r--   0        0        0     2794 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/fuse.py
--rw-r--r--   0        0        0      995 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
--rw-r--r--   0        0        0     3961 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
--rw-r--r--   0        0        0     2968 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
--rw-r--r--   0        0        0     2881 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
--rw-r--r--   0        0        0     3615 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
--rw-r--r--   0        0        0     2446 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
--rw-r--r--   0        0        0     2585 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
--rw-r--r--   0        0        0     2444 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
--rw-r--r--   0        0        0     2831 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
--rw-r--r--   0        0        0     3956 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
--rw-r--r--   0        0        0     2101 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
--rw-r--r--   0        0        0     3294 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
--rw-r--r--   0        0        0     4090 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
--rw-r--r--   0        0        0     2366 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
--rw-r--r--   0        0        0     4137 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
--rw-r--r--   0        0        0     2806 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/recloser.py
--rw-r--r--   0        0        0     2661 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
--rw-r--r--   0        0        0     3314 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
--rw-r--r--   0        0        0     2883 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
--rw-r--r--   0        0        0     3015 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
--rw-r--r--   0        0        0     3688 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
--rw-r--r--   0        0        0     4996 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
--rw-r--r--   0        0        0     3020 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/terminal.py
--rw-r--r--   0        0        0     2415 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
--rw-r--r--   0        0        0     4452 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
--rw-r--r--   0        0        0     2648 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
--rw-r--r--   0        0        0     3122 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
--rw-r--r--   0        0        0     3765 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
--rw-r--r--   0        0        0     2604 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
--rw-r--r--   0        0        0     2280 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py
--rw-r--r--   0        0        0     2687 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
--rw-r--r--   0        0        0      386 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/models/__init__.py
--rw-r--r--   0        0        0     4116 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/models/distributed_model.py
--rw-r--r--   0        0        0     1715 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/models/model_parsers.py
--rw-r--r--   0        0        0     3167 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/models/secondary_area.py
--rw-r--r--   0        0        0     3734 2023-04-04 21:42:05.670585 cim_graph-0.1.20230404214301a0/cimgraph/models/switch_area.py
--rw-r--r--   0        0        0      757 2023-04-04 21:43:01.375832 cim_graph-0.1.20230404214301a0/pyproject.toml
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 cim_graph-0.1.20230404214301a0/PKG-INFO
+-rw-r--r--   0        0        0     4900 2023-04-13 18:58:23.560702 cim_graph-0.1.20230413185916a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 18:58:23.560702 cim_graph-0.1.20230413185916a0/cimgraph/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-13 18:58:23.560702 cim_graph-0.1.20230413185916a0/cimgraph/data_profile/__init__.py
+-rw-r--r--   0        0        0     9401 2023-04-13 18:58:23.560702 cim_graph-0.1.20230413185916a0/cimgraph/data_profile/cimext_2022/__init__.py
+-rw-r--r--   0        0        0   370766 2023-04-13 18:58:23.564702 cim_graph-0.1.20230413185916a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
+-rw-r--r--   0        0        0    24601 2023-04-13 18:58:23.564702 cim_graph-0.1.20230413185916a0/cimgraph/data_profile/rc4_2021/__init__.py
+-rw-r--r--   0        0        0   835023 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
+-rw-r--r--   0        0        0     1063 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/__init__.py
+-rw-r--r--   0        0        0      353 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/blazegraph/__init__.py
+-rw-r--r--   0        0        0     9114 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/blazegraph/blazegraph.py
+-rw-r--r--   0        0        0     2797 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/blazegraph/query_parsers.py
+-rw-r--r--   0        0        0    10318 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4142 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/__init__.py
+-rw-r--r--   0        0        0     1492 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
+-rw-r--r--   0        0        0     3711 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
+-rw-r--r--   0        0        0     3156 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
+-rw-r--r--   0        0        0     2646 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/analog.py
+-rw-r--r--   0        0        0     1483 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/asset.py
+-rw-r--r--   0        0        0      885 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py
+-rw-r--r--   0        0        0     1491 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
+-rw-r--r--   0        0        0     3141 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
+-rw-r--r--   0        0        0     3041 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/breaker.py
+-rw-r--r--   0        0        0     2795 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py
+-rw-r--r--   0        0        0     5482 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
+-rw-r--r--   0        0        0     2667 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py
+-rw-r--r--   0        0        0     2650 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/discrete.py
+-rw-r--r--   0        0        0     3155 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
+-rw-r--r--   0        0        0     2176 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
+-rw-r--r--   0        0        0     2794 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/fuse.py
+-rw-r--r--   0        0        0      995 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
+-rw-r--r--   0        0        0     3961 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
+-rw-r--r--   0        0        0     2968 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
+-rw-r--r--   0        0        0     2881 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
+-rw-r--r--   0        0        0     3615 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
+-rw-r--r--   0        0        0     2446 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
+-rw-r--r--   0        0        0     2585 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
+-rw-r--r--   0        0        0     2444 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
+-rw-r--r--   0        0        0     2831 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
+-rw-r--r--   0        0        0     3956 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
+-rw-r--r--   0        0        0     2101 2023-04-13 18:58:23.568702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
+-rw-r--r--   0        0        0     3294 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
+-rw-r--r--   0        0        0     4090 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
+-rw-r--r--   0        0        0     2366 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
+-rw-r--r--   0        0        0     4137 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
+-rw-r--r--   0        0        0     2806 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/recloser.py
+-rw-r--r--   0        0        0     2661 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
+-rw-r--r--   0        0        0     3314 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
+-rw-r--r--   0        0        0     2883 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
+-rw-r--r--   0        0        0     3015 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
+-rw-r--r--   0        0        0     3688 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
+-rw-r--r--   0        0        0     4996 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
+-rw-r--r--   0        0        0     3020 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/terminal.py
+-rw-r--r--   0        0        0     2415 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
+-rw-r--r--   0        0        0     4452 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
+-rw-r--r--   0        0        0     2648 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
+-rw-r--r--   0        0        0     3122 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
+-rw-r--r--   0        0        0     3765 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
+-rw-r--r--   0        0        0     2604 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
+-rw-r--r--   0        0        0     2280 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py
+-rw-r--r--   0        0        0     2687 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
+-rw-r--r--   0        0        0      386 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/models/__init__.py
+-rw-r--r--   0        0        0     4116 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/models/distributed_model.py
+-rw-r--r--   0        0        0     1715 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/models/model_parsers.py
+-rw-r--r--   0        0        0     3167 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/models/secondary_area.py
+-rw-r--r--   0        0        0     3734 2023-04-13 18:58:23.572702 cim_graph-0.1.20230413185916a0/cimgraph/models/switch_area.py
+-rw-r--r--   0        0        0      757 2023-04-13 18:59:16.960516 cim_graph-0.1.20230413185916a0/pyproject.toml
+-rw-r--r--   0        0        0     5569 1970-01-01 00:00:00.000000 cim_graph-0.1.20230413185916a0/PKG-INFO
```

### Comparing `cim_graph-0.1.20230404214301a0/README.md` & `cim_graph-0.1.20230413185916a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 ## Specifying the CIM Profile
 
 The CIM-Graph library supports multiple CIM profiles, which can be exported using CIMtool or Enterprise Architect Schema Composer as a .xsd data profile. The data profiles are ingested using the xsdata python library and saved in the cimgraph/data_profile directory.
 
 When importing the library, the CIM profile must be specified using the gridappsd-python constructor or directly as
 
 ```python
-import cimlab.data_profile.rc4_2021 as cim
+import cimgraph.data_profile.rc4_2021 as cim
 ```
 
 or by using `importlib`:
 
 ```python
 import importlib
 cim_profile = 'rc4_2021'
-cim = importlib.import_module('cimlab.data_profile.' + cim_profile)
+cim = importlib.import_module('cimgraph.data_profile.' + cim_profile)
 ```
 
 ## Model Initialization
 
 The CIM-Graph library creates object instances populated with the attributes of `name` and `mRID` for all addressable and unaddressable equipment in each distributed area. All other attributes are `None` or `[]` by default.
 
 ### Usage with GridAPPS-D Context Manager
```

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/data_profile/cimext_2022/__init__.py` & `cim_graph-0.1.20230413185916a0/cimgraph/data_profile/cimext_2022/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py` & `cim_graph-0.1.20230413185916a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/data_profile/rc4_2021/__init__.py` & `cim_graph-0.1.20230413185916a0/cimgraph/data_profile/rc4_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py` & `cim_graph-0.1.20230413185916a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/__init__.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/blazegraph/blazegraph.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/blazegraph/blazegraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import importlib
 import logging
 import re
 from typing import Dict, List, Optional
 
-from SPARQLWrapper import JSON, POST, SPARQLWrapper
-
 from cimgraph.loaders import (ConnectionInterface, ConnectionParameters,
                               Parameter, QueryResponse)
 from cimgraph.models.model_parsers import add_to_catalog, add_to_typed_catalog
+from SPARQLWrapper import JSON, POST, SPARQLWrapper
 
 _log = logging.getLogger(__name__)
 
 class BlazegraphConnection(ConnectionInterface):
     def __init__(self, connection_params, cim_profile:str):
-        self.sparql = importlib.import_module('cimlab.loaders.sparql.' + cim_profile)
-        self.cim = importlib.import_module('cimlab.data_profile.' + cim_profile)
+        self.sparql = importlib.import_module('cimgraph.loaders.sparql.' + cim_profile)
+        self.cim = importlib.import_module('cimgraph.data_profile.' + cim_profile)
         self.sparql_obj: Optional[SPARQLWrapper] = None
         self.connection_params = connection_params
 
     def connect(self):
         if not self.sparql_obj:
             url = self.connection_params.parameters[0].value
             self.sparql_obj = SPARQLWrapper(url)
```

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/blazegraph/query_parsers.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/blazegraph/query_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/gridappsd/__init__.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/gridappsd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import atexit
 import importlib
 import os
 import re
 import sys
 from typing import Dict, List
 
-from gridappsd import GridAPPSD
-from SPARQLWrapper import JSON, POST, SPARQLWrapper
-
 from cimgraph.data_profile import CIM_PROFILE
 from cimgraph.loaders import (ConnectionInterface, ConnectionParameters,
                               Parameter, QueryResponse)
 from cimgraph.loaders.blazegraph.blazegraph import BlazegraphConnection
 from cimgraph.models import add_to_catalog, add_to_typed_catalog
+from SPARQLWrapper import JSON, POST, SPARQLWrapper
+
+from gridappsd import GridAPPSD
 
 cim = None
 sparql = None
 
 
 def set_cim_profile(cim_profile: CIM_PROFILE):
     global cim
     global sparql
-    cim = importlib.import_module('cimlab.data_profile.' + cim_profile)
-    sparql = importlib.import_module('cimlab.loaders.sparql.' + cim_profile)
+    cim = importlib.import_module('cimgraph.data_profile.' + cim_profile)
+    sparql = importlib.import_module('cimgraph.loaders.sparql.' + cim_profile)
 
 os.environ["GRIDAPPSD_ADDRESS"] = "localhost"
 os.environ["GRIDAPPSD_PORT"] = "61613"
 os.environ['GRIDAPPSD_APPLICATION_ID'] = 'gridappsd-cim-profile'
 os.environ['GRIDAPPSD_APPLICATION_STATUS'] = 'STARTED'
 os.environ['GRIDAPPSD_USER'] = 'app_user'
 os.environ['GRIDAPPSD_PASSWORD'] = '1234App'
```

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/__init__.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import cimgraph.loaders.sparql.rc4_2021.analog as AnalogSPARQL
 import cimgraph.loaders.sparql.rc4_2021.asset as AssetSPARQL
 import cimgraph.loaders.sparql.rc4_2021.asset_info as AssetInfoSPARQL
 #b
 import cimgraph.loaders.sparql.rc4_2021.base_voltage as BaseVoltageSPARQL
 import cimgraph.loaders.sparql.rc4_2021.battery_unit as BatteryUnitSPARQL
 import cimgraph.loaders.sparql.rc4_2021.breaker as BreakerSPARQL
-# import cimlab.loaders.sparql.rc4_2021.bus_bar_section as BusBarSectionSPARQL
-# import cimlab.loaders.sparql.rc4_2021.bus_bar_section_info as BusBarSectionInfoSPARQL
+# import cimgraph.loaders.sparql.rc4_2021.bus_bar_section as BusBarSectionSPARQL
+# import cimgraph.loaders.sparql.rc4_2021.bus_bar_section_info as BusBarSectionInfoSPARQL
 #c
 import cimgraph.loaders.sparql.rc4_2021.cable_info as CableInfoSPARQL
 import cimgraph.loaders.sparql.rc4_2021.concentric_neutral_cable_info as ConcentricNeutralCableInfoSPARQL
 #d
 import cimgraph.loaders.sparql.rc4_2021.disconnector as DisconnectorSPARQL
 import cimgraph.loaders.sparql.rc4_2021.discrete as DiscreteSPARQL
 #e
```

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/analog.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/analog.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/asset.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/asset.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/breaker.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/breaker.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/discrete.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/discrete.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/fuse.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/fuse.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/recloser.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/recloser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/terminal.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py` & `cim_graph-0.1.20230413185916a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/models/distributed_model.py` & `cim_graph-0.1.20230413185916a0/cimgraph/models/distributed_model.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/models/model_parsers.py` & `cim_graph-0.1.20230413185916a0/cimgraph/models/model_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/models/secondary_area.py` & `cim_graph-0.1.20230413185916a0/cimgraph/models/secondary_area.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/cimgraph/models/switch_area.py` & `cim_graph-0.1.20230413185916a0/cimgraph/models/switch_area.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230404214301a0/pyproject.toml` & `cim_graph-0.1.20230413185916a0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cim-graph"
-version = "0.1.20230404214301a0"
+version = "0.1.20230413185916a0"
 description = "CIM Graph"
 authors = ["C. Allwardt <3979063+craig8@users.noreply.github.com>"]
 packages = [
     { include = "cimgraph" }
 ]
 readme = "README.md"
```

### Comparing `cim_graph-0.1.20230404214301a0/PKG-INFO` & `cim_graph-0.1.20230413185916a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-graph
-Version: 0.1.20230404214301a0
+Version: 0.1.20230413185916a0
 Summary: CIM Graph
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -47,23 +47,23 @@
 ## Specifying the CIM Profile
 
 The CIM-Graph library supports multiple CIM profiles, which can be exported using CIMtool or Enterprise Architect Schema Composer as a .xsd data profile. The data profiles are ingested using the xsdata python library and saved in the cimgraph/data_profile directory.
 
 When importing the library, the CIM profile must be specified using the gridappsd-python constructor or directly as
 
 ```python
-import cimlab.data_profile.rc4_2021 as cim
+import cimgraph.data_profile.rc4_2021 as cim
 ```
 
 or by using `importlib`:
 
 ```python
 import importlib
 cim_profile = 'rc4_2021'
-cim = importlib.import_module('cimlab.data_profile.' + cim_profile)
+cim = importlib.import_module('cimgraph.data_profile.' + cim_profile)
 ```
 
 ## Model Initialization
 
 The CIM-Graph library creates object instances populated with the attributes of `name` and `mRID` for all addressable and unaddressable equipment in each distributed area. All other attributes are `None` or `[]` by default.
 
 ### Usage with GridAPPS-D Context Manager
```

