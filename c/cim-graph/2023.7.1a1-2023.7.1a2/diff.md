# Comparing `tmp/cim_graph-2023.7.1a1.tar.gz` & `tmp/cim_graph-2023.7.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_graph-2023.7.1a1.tar", max compression
+gzip compressed data, was "cim_graph-2023.7.1a2.tar", max compression
```

## Comparing `cim_graph-2023.7.1a1.tar` & `cim_graph-2023.7.1a2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     5141 2023-07-14 22:30:43.656078 cim_graph-2023.7.1a1/README.md
--rw-r--r--   0        0        0        0 2023-07-14 22:30:43.656078 cim_graph-2023.7.1a1/cimgraph/__init__.py
--rw-r--r--   0        0        0      105 2023-07-14 22:30:43.656078 cim_graph-2023.7.1a1/cimgraph/data_profile/__init__.py
--rw-r--r--   0        0        0     9401 2023-07-14 22:30:43.656078 cim_graph-2023.7.1a1/cimgraph/data_profile/cimext_2022/__init__.py
--rw-r--r--   0        0        0   370766 2023-07-14 22:30:43.660078 cim_graph-2023.7.1a1/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
--rw-r--r--   0        0        0    24601 2023-07-14 22:30:43.660078 cim_graph-2023.7.1a1/cimgraph/data_profile/rc4_2021/__init__.py
--rw-r--r--   0        0        0   835023 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
--rw-r--r--   0        0        0     1063 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/__init__.py
--rw-r--r--   0        0        0      353 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/blazegraph/__init__.py
--rw-r--r--   0        0        0     9099 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/blazegraph/blazegraph.py
--rw-r--r--   0        0        0     2887 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/blazegraph/query_parsers.py
--rw-r--r--   0        0        0     9877 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/gridappsd/__init__.py
--rw-r--r--   0        0        0     4429 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/__init__.py
--rw-r--r--   0        0        0     1492 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
--rw-r--r--   0        0        0     3711 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
--rw-r--r--   0        0        0     3156 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
--rw-r--r--   0        0        0     2646 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/analog.py
--rw-r--r--   0        0        0     1483 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/asset.py
--rw-r--r--   0        0        0      885 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/asset_info.py
--rw-r--r--   0        0        0     1491 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
--rw-r--r--   0        0        0     3141 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
--rw-r--r--   0        0        0     3046 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/breaker.py
--rw-r--r--   0        0        0     2795 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/cable_info.py
--rw-r--r--   0        0        0     5482 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
--rw-r--r--   0        0        0     2350 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py
--rw-r--r--   0        0        0     2672 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/disconnector.py
--rw-r--r--   0        0        0     2650 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/discrete.py
--rw-r--r--   0        0        0     3155 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
--rw-r--r--   0        0        0     2176 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
--rw-r--r--   0        0        0     2799 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/fuse.py
--rw-r--r--   0        0        0      995 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
--rw-r--r--   0        0        0     3961 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
--rw-r--r--   0        0        0     3392 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator_phase.py
--rw-r--r--   0        0        0     2973 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
--rw-r--r--   0        0        0     2881 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
--rw-r--r--   0        0        0     3615 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
--rw-r--r--   0        0        0     2446 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
--rw-r--r--   0        0        0     2585 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
--rw-r--r--   0        0        0     2444 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
--rw-r--r--   0        0        0     2831 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
--rw-r--r--   0        0        0     3956 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
--rw-r--r--   0        0        0     2101 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
--rw-r--r--   0        0        0     3294 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
--rw-r--r--   0        0        0     4090 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
--rw-r--r--   0        0        0     2366 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
--rw-r--r--   0        0        0     4137 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
--rw-r--r--   0        0        0     2813 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/recloser.py
--rw-r--r--   0        0        0     2668 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
--rw-r--r--   0        0        0     3314 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
--rw-r--r--   0        0        0     3132 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/shunt_compensator_phase.py
--rw-r--r--   0        0        0     2801 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
--rw-r--r--   0        0        0     3015 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
--rw-r--r--   0        0        0     3688 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
--rw-r--r--   0        0        0     4996 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
--rw-r--r--   0        0        0     3020 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/terminal.py
--rw-r--r--   0        0        0     2415 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
--rw-r--r--   0        0        0     4453 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
--rw-r--r--   0        0        0     2648 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
--rw-r--r--   0        0        0     3158 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
--rw-r--r--   0        0        0     3764 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
--rw-r--r--   0        0        0     2604 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
--rw-r--r--   0        0        0     2280 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/wire_position.py
--rw-r--r--   0        0        0     2687 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
--rw-r--r--   0        0        0      386 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/models/__init__.py
--rw-r--r--   0        0        0     4116 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/models/distributed_model.py
--rw-r--r--   0        0        0     1715 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/models/model_parsers.py
--rw-r--r--   0        0        0     3171 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/models/secondary_area.py
--rw-r--r--   0        0        0     3738 2023-07-14 22:30:43.668078 cim_graph-2023.7.1a1/cimgraph/models/switch_area.py
--rw-r--r--   0        0        0      747 2023-07-14 22:31:34.525183 cim_graph-2023.7.1a1/pyproject.toml
--rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 cim_graph-2023.7.1a1/PKG-INFO
+-rw-r--r--   0        0        0     5141 2023-07-21 18:13:24.252384 cim_graph-2023.7.1a2/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 18:13:24.252384 cim_graph-2023.7.1a2/cimgraph/__init__.py
+-rw-r--r--   0        0        0      105 2023-07-21 18:13:24.252384 cim_graph-2023.7.1a2/cimgraph/data_profile/__init__.py
+-rw-r--r--   0        0        0     9401 2023-07-21 18:13:24.252384 cim_graph-2023.7.1a2/cimgraph/data_profile/cimext_2022/__init__.py
+-rw-r--r--   0        0        0   370766 2023-07-21 18:13:24.256384 cim_graph-2023.7.1a2/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
+-rw-r--r--   0        0        0    24601 2023-07-21 18:13:24.256384 cim_graph-2023.7.1a2/cimgraph/data_profile/rc4_2021/__init__.py
+-rw-r--r--   0        0        0   835023 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
+-rw-r--r--   0        0        0     1063 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/blazegraph/__init__.py
+-rw-r--r--   0        0        0     9099 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/blazegraph/blazegraph.py
+-rw-r--r--   0        0        0     2887 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/blazegraph/query_parsers.py
+-rw-r--r--   0        0        0     9877 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4429 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/__init__.py
+-rw-r--r--   0        0        0     1492 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
+-rw-r--r--   0        0        0     3711 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
+-rw-r--r--   0        0        0     3156 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
+-rw-r--r--   0        0        0     2646 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/analog.py
+-rw-r--r--   0        0        0     1483 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/asset.py
+-rw-r--r--   0        0        0      885 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/asset_info.py
+-rw-r--r--   0        0        0     1491 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
+-rw-r--r--   0        0        0     3141 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
+-rw-r--r--   0        0        0     3046 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/breaker.py
+-rw-r--r--   0        0        0     2795 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/cable_info.py
+-rw-r--r--   0        0        0     5482 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
+-rw-r--r--   0        0        0     2350 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py
+-rw-r--r--   0        0        0     2672 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/disconnector.py
+-rw-r--r--   0        0        0     2650 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/discrete.py
+-rw-r--r--   0        0        0     3155 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
+-rw-r--r--   0        0        0     2176 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
+-rw-r--r--   0        0        0     2799 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/fuse.py
+-rw-r--r--   0        0        0      995 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
+-rw-r--r--   0        0        0     3961 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
+-rw-r--r--   0        0        0     3392 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator_phase.py
+-rw-r--r--   0        0        0     2973 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
+-rw-r--r--   0        0        0     2881 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
+-rw-r--r--   0        0        0     3615 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
+-rw-r--r--   0        0        0     2446 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
+-rw-r--r--   0        0        0     2585 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
+-rw-r--r--   0        0        0     2433 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
+-rw-r--r--   0        0        0     2831 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
+-rw-r--r--   0        0        0     3956 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
+-rw-r--r--   0        0        0     2101 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
+-rw-r--r--   0        0        0     3294 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
+-rw-r--r--   0        0        0     4090 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
+-rw-r--r--   0        0        0     2366 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
+-rw-r--r--   0        0        0     4137 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
+-rw-r--r--   0        0        0     2813 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/recloser.py
+-rw-r--r--   0        0        0     2668 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
+-rw-r--r--   0        0        0     3314 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
+-rw-r--r--   0        0        0     3132 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/shunt_compensator_phase.py
+-rw-r--r--   0        0        0     2801 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
+-rw-r--r--   0        0        0     3015 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
+-rw-r--r--   0        0        0     3688 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
+-rw-r--r--   0        0        0     4996 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
+-rw-r--r--   0        0        0     3020 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/terminal.py
+-rw-r--r--   0        0        0     2415 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
+-rw-r--r--   0        0        0     4453 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
+-rw-r--r--   0        0        0     2648 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
+-rw-r--r--   0        0        0     3158 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
+-rw-r--r--   0        0        0     3764 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
+-rw-r--r--   0        0        0     2604 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
+-rw-r--r--   0        0        0     2280 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/wire_position.py
+-rw-r--r--   0        0        0     2687 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
+-rw-r--r--   0        0        0      386 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/models/__init__.py
+-rw-r--r--   0        0        0     4116 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/models/distributed_model.py
+-rw-r--r--   0        0        0     1715 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/models/model_parsers.py
+-rw-r--r--   0        0        0     3171 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/models/secondary_area.py
+-rw-r--r--   0        0        0     3738 2023-07-21 18:13:24.264385 cim_graph-2023.7.1a2/cimgraph/models/switch_area.py
+-rw-r--r--   0        0        0      747 2023-07-21 18:14:24.173678 cim_graph-2023.7.1a2/pyproject.toml
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 cim_graph-2023.7.1a2/PKG-INFO
```

### Comparing `cim_graph-2023.7.1a1/README.md` & `cim_graph-2023.7.1a2/README.md`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/data_profile/cimext_2022/__init__.py` & `cim_graph-2023.7.1a2/cimgraph/data_profile/cimext_2022/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py` & `cim_graph-2023.7.1a2/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/data_profile/rc4_2021/__init__.py` & `cim_graph-2023.7.1a2/cimgraph/data_profile/rc4_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py` & `cim_graph-2023.7.1a2/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/__init__.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/blazegraph/blazegraph.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/blazegraph/blazegraph.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/blazegraph/query_parsers.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/blazegraph/query_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/gridappsd/__init__.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/__init__.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/analog.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/analog.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/asset.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/asset.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/asset_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/asset_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/base_voltage.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/base_voltage.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/battery_unit.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/battery_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/breaker.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/breaker.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/cable_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/disconnector.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/disconnector.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/discrete.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/discrete.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/fuse.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/fuse.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/get_class_type.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/get_class_type.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator_phase.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/no_load_test.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/no_load_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         PREFIX r:  <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
         PREFIX cim:  <http://iec.ch/TC57/CIM100#>
         SELECT ?mRID ?name ?PhaseImpedance ?row ?column ?r ?x ?b 
 
         WHERE {          
           ?eq r:type cim:PhaseImpedanceData.
           VALUES ?fdrid {"%s"}
-          VALUES ?mRID {"""%feeder_mrid
+          """%feeder_mrid
     # add all equipment mRID
-    for mrid in mrid_list:
-        query_message += ' "%s" \n'%mrid
+#     for mrid in mrid_list:
+#         query_message += ' "%s" \n'%mrid
         
     # add all assets
-    query_message += """               }
+    query_message += """               
         VALUES ?ACLineSegment {"""
     for asset_mrid in asset_list:
         query_message += ' "%s" \n' % asset_mrid
         
     # add all attributes
     query_message += """               } 
         ?eq cim:PhaseImpedanceData.PhaseImpedance ?pli.
```

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_transformer.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     mrid_list = list(typed_catalog[cim.PowerTransformer].keys())
 
     
     query_message = """
         PREFIX r:  <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
         PREFIX cim:  <http://iec.ch/TC57/CIM100#>
         SELECT ?mRID ?name ?Location ?vectorGroup ?aggregate ?inService
-        (group_concat(distinct ?PowerTransformerEnd; separator=";") as ?PowerTransformerEnd) 
-        (group_concat(distinct ?TransformerTank; separator=';') as ?TransformerTanks)
-        (group_concat(distinct ?Terminal; separator=';') as ?Terminals)
+        (group_concat(distinct ?PowerTransformerE; separator=";") as ?PowerTransformerEnd) 
+        (group_concat(distinct ?TransformerTank; separator=";") as ?TransformerTanks)
+        (group_concat(distinct ?Terminal; separator=";") as ?Terminals)
         (group_concat(distinct ?Measurement; separator=";") as ?Measurements) 
         (group_concat(distinct ?Asset; separator=";") as ?Assets) 
         
         WHERE {          
           ?eq r:type cim:PowerTransformer.
           VALUES ?fdrid {"%s"}
           VALUES ?mRID {"""%feeder_mrid
     # add all equipment mRID
     for mrid in mrid_list:
-        query_message += ' "%s" \n'%mrid
+        query_message += """ "%s" \n"""%mrid
     # add all attributes
     query_message += """               } 
          ?eq cim:Equipment.EquipmentContainer ?fdr.
         ?fdr cim:IdentifiedObject.mRID ?fdrid.
 
         ?eq cim:IdentifiedObject.mRID ?mRID.
         ?eq cim:IdentifiedObject.name ?name.
@@ -56,15 +56,15 @@
         OPTIONAL {?asset cim:Asset.PowerSystemResources ?eq.
                   ?asset cim:IdentifiedObject.mRID ?Asset.}
 
         OPTIONAL {?tank cim:TransformerTank.PowerTransformer ?eq.
                   ?tank cim:IdentifiedObject.mRID ?TransformerTank.}
 
         OPTIONAL {?end cim:PowerTransformerEnd.PowerTransformer ?eq.
-                  ?end cim:IdentifiedObject.mRID ?PowerTransformerEnd.}
+                  ?end cim:IdentifiedObject.mRID ?PowerTransformerE.}
                   
         OPTIONAL {?t cim:Terminal.ConductingEquipment ?eq.
                   ?t cim:IdentifiedObject.mRID ?Terminal.}
         OPTIONAL {?meas cim:Measurement.PowerSystemResource ?eq.
             ?meas cim:IdentifiedObject.mRID ?meas_id.
             ?meas a ?meas_cls.
             bind(concat(str(?meas_id),",",strafter(str(?meas_cls),"CIM100#")) as ?Measurement).}
```

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/recloser.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/recloser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/shunt_compensator_phase.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/shunt_compensator_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/switch_phase.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/switch_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/terminal.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/wire_position.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/wire_position.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py` & `cim_graph-2023.7.1a2/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/models/distributed_model.py` & `cim_graph-2023.7.1a2/cimgraph/models/distributed_model.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/models/model_parsers.py` & `cim_graph-2023.7.1a2/cimgraph/models/model_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/models/secondary_area.py` & `cim_graph-2023.7.1a2/cimgraph/models/secondary_area.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/cimgraph/models/switch_area.py` & `cim_graph-2023.7.1a2/cimgraph/models/switch_area.py`

 * *Files identical despite different names*

### Comparing `cim_graph-2023.7.1a1/PKG-INFO` & `cim_graph-2023.7.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-graph
-Version: 2023.7.1a1
+Version: 2023.7.1a2
 Summary: CIM Graph
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

