# Comparing `tmp/kqcircuits-4.6.21.tar.gz` & `tmp/kqcircuits-4.6.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kqcircuits-4.6.21.tar", last modified: Fri Jul 21 14:11:24 2023, max compression
+gzip compressed data, was "kqcircuits-4.6.9rc1.tar", last modified: Tue Mar  7 09:28:44 2023, max compression
```

## Comparing `kqcircuits-4.6.21.tar` & `kqcircuits-4.6.9rc1.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.179694 kqcircuits-4.6.21/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 14:11:24.179694 kqcircuits-4.6.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.135694 kqcircuits-4.6.21/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/console_scripts/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.179694 kqcircuits-4.6.21/kqcircuits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 14:11:24.179694 kqcircuits-4.6.21/kqcircuits/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.143694 kqcircuits-4.6.21/kqcircuits/chips/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/airbridge_crossings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/airbridge_dc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30195 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/crossing_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/daisy_woven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/dc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/demo_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/junction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/junction_test2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/lithography_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/lithography_test_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/quality_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/quality_factor_twoface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/sample_holder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/single_xmons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/stripes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/tsv_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/chips/xmons_direct_coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.147694 kqcircuits-4.6.21/kqcircuits/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/airbridge_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.151694 kqcircuits-4.6.21/kqcircuits/elements/airbridges/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/airbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/airbridges/airbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/airbridges/airbridge_multi_face.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/airbridges/airbridge_rectangular.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/chip_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/circular_capacitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/daisy_woven.oas
--rw-r--r--   0 runner    (1001) docker     (123)    28848 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/finger_capacitor_square.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/finger_capacitor_taper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.151694 kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.151694 kqcircuits-4.6.21/kqcircuits/elements/fluxlines/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/fluxlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/fluxlines/fluxline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/fluxlines/fluxline_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/fluxlines/fluxline_straight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/launcher_dc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.155694 kqcircuits-4.6.21/kqcircuits/elements/markers/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/markers/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/markers/marker_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/mask_marker_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/meander.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/smooth_capacitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26823 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/spiral_resonator_polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.155694 kqcircuits-4.6.21/kqcircuits/elements/tsvs/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/tsvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/tsvs/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/tsvs/tsv_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/tsvs/tsv_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)    42923 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/waveguide_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_curved.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_straight.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_taper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.155694 kqcircuits-4.6.21/kqcircuits/junctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/junction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/manhattan_single_junction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/no_squid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/junctions/squid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/klayout_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/layer_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.159694 kqcircuits-4.6.21/kqcircuits/layer_config/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/layer_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/layer_config/default_layer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/layer_config/default_layer_props.lyp
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/layer_config/example_layer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.159694 kqcircuits-4.6.21/kqcircuits/masks/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/masks/mask_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/masks/mask_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/masks/mask_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/pya_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.159694 kqcircuits-4.6.21/kqcircuits/qubits/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/qubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/qubits/double_pads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/qubits/double_pads_splines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/qubits/qubit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/qubits/swissmon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.163694 kqcircuits-4.6.21/kqcircuits/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/airbridges_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/circular_capacitor_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/cross_section_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/double_pads_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/empty_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.167694 kqcircuits-4.6.21/kqcircuits/simulations/export/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.167694 kqcircuits-4.6.21/kqcircuits/simulations/export/ansys/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/ansys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/ansys/ansys_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.167694 kqcircuits-4.6.21/kqcircuits/simulations/export/elmer/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/elmer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/elmer/elmer_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/export_and_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/simulation_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.167694 kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/sonnet_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/template.son
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.167694 kqcircuits-4.6.21/kqcircuits/simulations/export/xsection/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/xsection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/export/xsection/xsection_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/finger_capacitor_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/flip_chip_connector_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    46731 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/single_xmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/single_xmons_full_chip_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/waveguides_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/simulations/xmons_direct_coupling_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.171694 kqcircuits-4.6.21/kqcircuits/test_structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/airbridge_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/cross_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.171694 kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/stripes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/test_structures/tsv_test_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.179694 kqcircuits-4.6.21/kqcircuits/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/count_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/coupler_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/deep_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/edit_node_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/export_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/geometry_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/geometry_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/groundgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/gui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/import_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/layout_to_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/library_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/log_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/netlist_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/netlist_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/plugin_startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/refpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/replace_squids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/kqcircuits/util/symmetric_polygons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:11:24.135694 kqcircuits-4.6.21/kqcircuits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 14:11:24.000000 kqcircuits-4.6.21/kqcircuits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-21 14:11:24.000000 kqcircuits-4.6.21/kqcircuits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:11:24.000000 kqcircuits-4.6.21/kqcircuits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 14:11:24.000000 kqcircuits-4.6.21/kqcircuits.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-21 14:11:24.000000 kqcircuits-4.6.21/kqcircuits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 14:11:24.000000 kqcircuits-4.6.21/kqcircuits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:11:24.179694 kqcircuits-4.6.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-21 14:11:05.000000 kqcircuits-4.6.21/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      206 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      528 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)       96 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.364674 kqcircuits-4.6.9rc1/console_scripts/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/console_scripts/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2819 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/console_scripts/run.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/kqcircuits/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1347 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       64 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/kqcircuits/_static_version.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6540 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/_version.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.372674 kqcircuits-4.6.9rc1/kqcircuits/chips/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1448 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6212 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_crossings.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3481 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_dc_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    29396 2023-02-20 16:40:40.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/chip.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6954 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/crossing_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3976 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/daisy_woven.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1216 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/dc_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11053 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/demo.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9794 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/demo_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2114 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/empty.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3381 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5588 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test2.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1535 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/launchers.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6092 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4930 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10434 2023-02-27 12:33:15.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12878 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor_twoface.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/sample_holder_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16609 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/shaping.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3462 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/simple.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18962 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/single_xmons.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5103 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/stripes.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3527 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/tsv_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11979 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/chips/xmons_direct_coupling.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10119 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/defaults.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.380674 kqcircuits-4.6.9rc1/kqcircuits/elements/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1921 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4504 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridge_connection.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.380674 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1238 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3723 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2932 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_multi_face.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2436 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_rectangular.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10793 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/chip_frame.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6556 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/circular_capacitor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3709 2023-01-25 07:43:18.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/daisy_woven.oas
+-rw-rw-r--   0 dave      (1000) dave      (1000)    28708 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/element.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9307 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_square.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5183 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_taper.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.384674 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1154 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2617 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1375 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6647 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.384674 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1167 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3424 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2805 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_standard.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_straight.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3528 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/launcher.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2149 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/launcher_dc.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.388674 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1124 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4691 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1302 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker_standard.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5221 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/mask_marker_fc.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9555 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/meander.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9970 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/smooth_capacitor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    26823 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/spiral_resonator_polygon.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.388674 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1134 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1751 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2729 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_ellipse.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1663 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_standard.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    38661 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_composite.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12973 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6696 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_curved.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7614 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_splitter.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2657 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_straight.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3661 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_taper.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.388674 kqcircuits-4.6.9rc1/kqcircuits/junctions/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1504 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2695 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/junction.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13878 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8937 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan_single_junction.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1653 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/no_squid.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3131 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1660 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/junctions/squid.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    19990 2023-02-20 16:40:40.000000 kqcircuits-4.6.9rc1/kqcircuits/klayout_view.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1845 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_cluster.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.392674 kqcircuits-4.6.9rc1/kqcircuits/layer_config/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12093 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_config.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    35168 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_props.lyp
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5157 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/layer_config/example_layer_config.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.396674 kqcircuits-4.6.9rc1/kqcircuits/masks/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1543 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17237 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/mask_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    22122 2023-03-03 12:22:03.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/mask_layout.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21747 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/masks/mask_set.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3012 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/pya_resolver.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.400674 kqcircuits-4.6.9rc1/kqcircuits/qubits/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1219 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10373 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5784 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads_splines.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5535 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/qubit.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8489 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/qubits/swissmon.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1270 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2122 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/airbridges_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1815 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/circular_capacitor_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6786 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/cross_section_simulation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3231 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/double_pads_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1170 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/empty_simulation.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1220 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18084 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/ansys_export.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9050 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/cross_section_elmer_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15549 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/elmer_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2735 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/export_and_run.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3291 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/simulation_export.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.404674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1092 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6954 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/parser.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9707 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/sonnet_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1173 2023-01-25 07:43:18.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/template.son
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4332 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/util.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.408674 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1039 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    22849 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/xsection_export.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1933 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/finger_capacitor_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2141 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/flip_chip_connector_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5226 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/port.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    46731 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/simulation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2629 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmon.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3914 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmons_full_chip_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4333 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/waveguides_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11433 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5213 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_sim.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.408674 kqcircuits-4.6.9rc1/kqcircuits/test_structures/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1248 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6820 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/airbridge_dc.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3086 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/cross_test.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.408674 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1157 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11388 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1613 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2651 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/stripes_test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6489 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/test_structure.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2719 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/test_structures/tsv_test_pattern.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/kqcircuits/util/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1108 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3227 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/area.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2099 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/count_instances.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3141 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/coupler_lib.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1256 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/deep_delete.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2766 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/dependencies.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7786 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/edit_node_plugin.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8451 2023-02-23 15:09:46.000000 kqcircuits-4.6.9rc1/kqcircuits/util/export_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15818 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/geometry_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1960 2023-02-15 17:44:05.000000 kqcircuits-4.6.9rc1/kqcircuits/util/geometry_json_encoder.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3261 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/groundgrid.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8992 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/gui_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1579 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/import_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3995 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/label.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    19976 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/layout_to_code.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14347 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/kqcircuits/util/library_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2708 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/log_router.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4700 2023-02-20 16:40:40.000000 kqcircuits-4.6.9rc1/kqcircuits/util/merge.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13273 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/netlist_extraction.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5443 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/netlist_graph.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10538 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/parameter_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6705 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/parameters.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1560 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/plugin_startup.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3615 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/refpoints.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9090 2023-02-15 08:13:12.000000 kqcircuits-4.6.9rc1/kqcircuits/util/replace_squids.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2244 2023-02-13 14:44:04.000000 kqcircuits-4.6.9rc1/kqcircuits/util/symmetric_polygons.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-07 09:28:44.364674 kqcircuits-4.6.9rc1/kqcircuits.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      528 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6424 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       48 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      344 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       27 2023-03-07 09:28:44.000000 kqcircuits-4.6.9rc1/kqcircuits.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-03-07 09:28:44.412674 kqcircuits-4.6.9rc1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3038 2023-03-03 10:53:16.000000 kqcircuits-4.6.9rc1/setup.py
```

### Comparing `kqcircuits-4.6.21/console_scripts/__init__.py` & `kqcircuits-4.6.9rc1/console_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/console_scripts/run.py` & `kqcircuits-4.6.9rc1/console_scripts/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,62 +13,43 @@
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 import argparse
 import logging
 import sys
-import subprocess
 from pathlib import Path
 from kqcircuits.simulations.export.export_and_run import export_and_run
-from kqcircuits.defaults import TMP_PATH, SCRIPTS_PATH
+from kqcircuits.defaults import TMP_PATH, SIM_SCRIPT_PATH
 
 logging.basicConfig(level=logging.WARN, stream=sys.stdout)
 
+
 def run():
     parser = argparse.ArgumentParser(description='KQC console scripts')
 
     subparser = parser.add_subparsers(dest="command")
 
     simulate_parser = subparser.add_parser('simulate', help='KQC simulation \
             export and run script. Run and export with a single command!')
-    mask_parser = subparser.add_parser('mask', help='Build KQC Mask.')
 
     simulate_parser.add_argument('export_script', type=str, help='Name of the export script')
     simulate_parser.add_argument('--export-path-basename', type=str, default=None,
                                  help='The export folder will be `TMP_PATH / Path(export_path_basename)`, \
                                        if not given, then it will be `TMP_PATH / Path(args.export_script).stem`')
     simulate_parser.add_argument('-q', '--quiet', action="store_true", help='Quiet mode: No GUI')
 
-    mask_parser.add_argument('mask_script', type=str, help='Name of the mask script')
-    mask_parser.add_argument('-d', '--debug', action="store_true", help="Debug mode. Use a single process and "
-                             "print logs to standard output too.")
-    mask_parser.add_argument('-c N', action="store_true", help="Limit the number of used CPUs to 'N'")
-
     args, args_for_script = parser.parse_known_args()
 
     if args.command == "simulate":
         script_file = Path(args.export_script)
         if not script_file.is_file():
-            script_file = Path(SCRIPTS_PATH / "simulations" / args.export_script)
+            script_file = Path(SIM_SCRIPT_PATH / args.export_script)
             if not script_file.is_file():
-                logging.error(f"Export script not found at {args.export_script} or {script_file}")
+                logging.error(
+                        f"Export script not found at {args.export_script} or {SIM_SCRIPT_PATH / args.export_script}")
                 return
         if args.export_path_basename is not None:
             export_path = TMP_PATH / args.export_path_basename
         else:
             export_path = TMP_PATH / Path(args.export_script).stem
         export_and_run(script_file, export_path, args.quiet, args_for_script)
-    elif args.command == "mask":
-        script_file = Path(args.mask_script)
-        if not script_file.is_file():
-            script_file = Path(SCRIPTS_PATH / "masks" / args.mask_script)
-            if not script_file.is_file():
-                logging.error(f"Mask script not found at {args.mask_script} or {script_file}")
-                return
-        if args.debug:
-            subprocess.call([sys.executable, script_file, '-d'])
-        else:  # Windows needs this for multiprocessing
-            with open(script_file) as mask_file:
-                exec(mask_file.read())  # pylint: disable=exec-used
-    else:
-        parser.print_usage()
```

### Comparing `kqcircuits-4.6.21/kqcircuits/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,13 @@
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 import sys
 
 from kqcircuits.util.dependencies import install_kqc_dependencies
 
-# pylint: disable=undefined-variable
 from ._version import __version__
 if hasattr(sys.modules[__name__], "_version"):
     del _version  # remove to avoid confusion with __version__
 
 # Check for needed dependencies and install if missing.
 install_kqc_dependencies()
```

### Comparing `kqcircuits-4.6.21/kqcircuits/_version.py` & `kqcircuits-4.6.9rc1/kqcircuits/_version.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/airbridge_crossings.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_crossings.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,75 +38,68 @@
     crossings = Param(pdt.TypeInt, "Number of double crossings", 10,
         docstring="Number of pairs of airbridge crossings")
     b_number = Param(pdt.TypeInt, "Number of bridges", 5,
         docstring="Number of airbridges in one element of the mechanical test array")
 
     def build(self):
 
-        launchers = self.produce_launchers("SMA8",
-            launcher_assignments={
-                1: "PL-1-IN", 2: "PL-2-IN",
-                3: "PL-4-IN", 4: "PL-4-OUT",
-                5: "PL-2-OUT", 6: "PL-1-OUT",
-                7: "PL-3-OUT", 8: "PL-3-IN"
-            }
-        )
+        launchers = self.produce_launchers("SMA8")
         self._produce_transmission_lines(launchers)
         self._produce_mechanical_test_array()
 
     def _produce_transmission_lines(self, launchers):
 
         # Left transmission line
         self.insert_cell(WaveguideCoplanar,
             path=pya.DPath([
-                launchers["PL-1-IN"][0],
-                launchers["PL-1-OUT"][0]
+                launchers["NW"][0],
+                launchers["SW"][0]
             ], 1)
         )
 
         # Right transmission line
         self.insert_cell(WaveguideCoplanar,
             path=pya.DPath([
-                launchers["PL-2-IN"][0],
-                launchers["PL-2-OUT"][0]
+                launchers["NE"][0],
+                launchers["SE"][0]
             ], 1)
         )
 
         # Crossing transmission line
-        nodes = [Node(launchers["PL-3-IN"][0])]
-        ref_x = launchers["PL-1-IN"][0].x
-        last_y = launchers["PL-3-IN"][0].y
+        nodes = [Node(launchers["WN"][0])]
+        ref_x = launchers["NW"][0].x
+        last_y = launchers["WN"][0].y
         crossings = self.crossings  # must be even
-        step = (launchers["PL-3-IN"][0].y - launchers["PL-3-OUT"][0].y) / (crossings - 0.5) / 2
+        step = (launchers["WN"][0].y - launchers["WS"][0].y) / (crossings - 0.5) / 2
         wiggle = 250
         for _ in range(crossings):
             nodes.append(Node((ref_x - wiggle, last_y)))
             nodes.append(Node((ref_x, last_y), AirbridgeConnection))
             nodes.append(Node((ref_x + wiggle, last_y)))
             last_y -= step
             nodes.append(Node((ref_x + wiggle, last_y)))
             nodes.append(Node((ref_x, last_y), AirbridgeConnection))
             nodes.append(Node((ref_x - wiggle, last_y)))
             last_y -= step
-        nodes.append(Node(launchers["PL-3-OUT"][0]))
+        nodes.append(Node(launchers["WS"][0]))
         waveguide_cell = self.add_element(WaveguideComposite, nodes=nodes)
         self.insert_cell(waveguide_cell)
 
         # TL without crossings
-        nodes = [Node(launchers["PL-4-IN"][0])]
-        ref_x = launchers["PL-2-IN"][0].x + 2 * wiggle + 50
-        last_y = launchers["PL-4-IN"][0].y
+        nodes = [Node(launchers["EN"][0])]
+        ref_x = launchers["NE"][0].x + 2 * wiggle + 50
+        last_y = launchers["EN"][0].y
         for _ in range(crossings):
             nodes.append(Node((ref_x + wiggle, last_y)))
             nodes.append(Node((ref_x - wiggle, last_y)))
             last_y -= step
             nodes.append(Node((ref_x - wiggle, last_y)))
             nodes.append(Node((ref_x + wiggle, last_y)))
             last_y -= step
-        nodes.append(Node(launchers["PL-4-OUT"][0]))
+        nodes.append(Node(launchers["ES"][0]))
         waveguide_cell = self.add_element(WaveguideComposite, nodes=nodes)
         self.insert_cell(waveguide_cell)
 
     def _produce_mechanical_test_array(self):
 
         p_test_origin = pya.DPoint(3600, 9650)
         v_distance_step = pya.DVector(0, -2350)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/airbridge_dc_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/airbridge_dc_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/chip.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/chip.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 #
 # You should have received a copy of the GNU General Public License along with this program. If not, see
 # https://www.gnu.org/licenses/gpl-3.0.html.
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
-# pylint: disable=R0904
-# TODO: Consider refactoring to reduce number of public methods
+
 
 import numpy
 from autologging import logged
 
 from kqcircuits.defaults import default_layers, default_junction_type, default_sampleholders, default_mask_parameters, \
     default_bump_parameters, default_marker_type
 from kqcircuits.elements.chip_frame import ChipFrame
@@ -34,15 +33,14 @@
 from kqcircuits.util.groundgrid import make_grid
 from kqcircuits.elements.tsvs.tsv import Tsv
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector_dc import FlipChipConnectorDc
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector_rf import FlipChipConnectorRf
 
 
 @logged
-@add_parameters_from(Tsv, "tsv_type")
 @add_parameters_from(FlipChipConnectorRf, "connector_type")
 @add_parameter(ChipFrame, "box", hidden=True)
 @add_parameters_from(ChipFrame, "name_mask", "name_chip", "name_copy", "name_brand",
                      "dice_grid_margin", marker_types=[default_marker_type] * 8)
 class Chip(Element):
     """Base PCell declaration for chips.
 
@@ -269,15 +267,15 @@
                 frame_trans = pya.DTrans(0, 0)
             self.produce_frame(frame_parameters, frame_trans)
 
         if self.with_gnd_tsvs:
             self._produce_ground_tsvs(face_id=[0, 2])
         if self.with_face1_gnd_tsvs:
             tsv_box = self.get_box(1).enlarged(pya.DVector(-self.edge_from_tsv, -self.edge_from_tsv))
-            self._produce_ground_tsvs(face_id=[3, 1], tsv_box=tsv_box)
+            self._produce_ground_tsvs(face_id=[1, 3], tsv_box=tsv_box)
 
         if self.with_gnd_bumps:
             self._produce_ground_bumps()
 
     def get_box(self, face=0):
         """
         Get the chip frame box for the specified face, correctly resolving defaults.
@@ -377,42 +375,40 @@
                 # optionally apply relative transformation to the label
                 rel_label_trans_str = inst.property("label_trans")
                 if rel_label_trans_str is not None:
                     rel_label_trans = pya.DCplxTrans.from_s(rel_label_trans_str)
                     label_trans = label_trans * rel_label_trans
                 self.insert_cell(cell, label_trans)
 
-    def produce_launchers(self, sampleholder_type, launcher_assignments=None, enabled=None, face_id=0):
+    def produce_launchers(self, sampleholder_type, launcher_assignments=None, enabled=None):
         """Produces launchers for typical sample holders and sets chip size (``self.box``) accordingly.
 
         This is a wrapper around ``produce_n_launchers()`` to generate typical launcher configurations.
 
         Args:
             sampleholder_type: name of the sample holder type
             launcher_assignments: dictionary of (port_id: name) that assigns a name to some of the launchers
             enabled: list of enabled launchers, empty means all
-            face_id: index of face_ids in which to insert the launchers
 
         Returns:
             launchers as a dictionary :code:`{name: (point, heading, distance from chip edge)}`
 
         """
 
         if sampleholder_type == "SMA8":  # this is special: it has default launcher assignments
             if not launcher_assignments:
                 launcher_assignments = {1: "NW", 2: "NE", 3: "EN", 4: "ES", 5: "SE", 6: "SW", 7: "WS", 8: "WN"}
 
         if sampleholder_type in default_sampleholders:
             return self.produce_n_launchers(**default_sampleholders[sampleholder_type],
-                                            launcher_assignments=launcher_assignments, enabled=enabled, face_id=face_id)
+                                            launcher_assignments=launcher_assignments, enabled=enabled)
         return {}
 
     def produce_n_launchers(self, n, launcher_type, launcher_width, launcher_gap, launcher_indent, pad_pitch,
-                            launcher_assignments=None, launcher_frame_gap=None, enabled=None, chip_box=None,
-                            face_id=0):
+                            launcher_assignments=None, launcher_frame_gap=None, enabled=None, chip_box=None):
         """Produces n launchers at default locations and optionally changes the chip size.
 
         Launcher pads are equally distributed around the chip. This may be overridden by specifying
         the number of pads desired per chip side if ``n`` is an array of 4 numbers.
 
         Pads not in ``launcher_assignments`` are disabled by default. The ``enabled`` argument may
         override this. If neither argument is defined then all pads are enabled with default names.
@@ -424,32 +420,31 @@
             launcher_gap: pad to ground gap of the launchers
             launcher_indent: distance between the chip edge and pad port
             pad_pitch: distance between pad centers
             launcher_frame_gap: gap of the launcher pad at the frame
             launcher_assignments: dictionary of (port_id: name) that assigns a name to some of the launchers
             enabled: optional list of enabled launchers
             chip_box: optionally changes the chip size (``self.box``)
-            face_id: index of face_ids in which to insert the launchers
 
         Returns:
             launchers as a dictionary :code:`{name: (point, heading, distance from chip edge)}`
         """
 
         if launcher_frame_gap is None:
             launcher_frame_gap = launcher_gap
 
         if chip_box is not None:
             self.box = chip_box
 
         if launcher_type == "DC":
-            launcher_cell = self.add_element(LauncherDC, width=launcher_width, face_ids=[self.face_ids[face_id]])
+            launcher_cell = self.add_element(LauncherDC, width=launcher_width)
         else:
             launcher_cell = self.add_element(Launcher, s=launcher_width, l=launcher_width,
                                              a_launcher=launcher_width, b_launcher=launcher_gap,
-                                             launcher_frame_gap=launcher_frame_gap, face_ids=[self.face_ids[face_id]])
+                                             launcher_frame_gap=launcher_frame_gap)
 
         pads_per_side = n
         if not isinstance(n, tuple):
             n = int((n + n % 4) / 4)
             pads_per_side = [n, n, n, n]
 
         dirs = (90, 0, -90, 180)
@@ -457,45 +452,39 @@
                  pya.DTrans(2, 0, self.box.p2.x, self.box.p2.y),
                  pya.DTrans(1, 0, self.box.p2.x, self.box.p1.y),
                  pya.DTrans(0, 0, self.box.p1.x, self.box.p1.y))
         _w = self.box.p2.x - self.box.p1.x
         _h = self.box.p2.y - self.box.p1.y
         sides = [_w, _h, _w, _h]
 
-        return self._insert_launchers(dirs, enabled, launcher_assignments, launcher_cell, launcher_indent,
-                                      launcher_width, pad_pitch, pads_per_side, sides, trans)
-
-    def _insert_launchers(self, dirs, enabled, launcher_assignments, launcher_cell, launcher_indent, launcher_width,
-                          pad_pitch, pads_per_side, sides, trans):
-
-        """Inserts launcher cell at predefined parameters and returns launcher cells
+        launchers = {}  # dictionary of point, heading, distance from chip edge
 
-        """
-        port_id, launchers = 0, {}
+        port_id = 0
         for np, dr, tr, si in zip(pads_per_side, dirs, trans, sides):
             for i in range(np):
                 port_id += 1
                 if launcher_assignments:
-                    if port_id not in launcher_assignments:
+                    if port_id in launcher_assignments:
+                        name = launcher_assignments[port_id]
+                    else:
                         continue
-                    name = launcher_assignments[port_id]
-
                 else:
                     name = str(port_id)
 
                 if enabled and name not in enabled:
                     continue
 
                 loc = tr * pya.DPoint(launcher_indent, si / 2 + pad_pitch * (i + 0.5 - np / 2))
                 launchers[name] = (loc, dr, launcher_width)
 
                 transf = pya.DCplxTrans(1, dr, False, loc)
                 launcher_inst, launcher_refpoints = self.insert_cell(launcher_cell, transf, name)
                 launcher_inst.set_property("port_id", port_id)
                 self.add_port(name, launcher_refpoints["port"])
+
         return launchers
 
     def make_grid_locations(self, box, delta_x=100, delta_y=100):  # pylint: disable=no-self-use
         """
         Define the locations for a grid. This method returns the full grid.
 
         Args:
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/crossing_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/crossing_twoface.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,92 +35,85 @@
     crossing_length = Param(pdt.TypeDouble, "Crossing waveguide length", 400, unit="μm",
         docstring="Length of the crossing on the top face (μm)")
     cross_talk_distance = Param(pdt.TypeDouble, "Transmission line distance from meander", 300, unit="μm",
         docstring="Distance between the right straight transmission line and meander on the right (μm)")
     meander_face = Param(pdt.TypeString, "Meander face on right side", "single", choices=["Single", "Two Face"])
 
     def build(self):
-        launchers = self.produce_launchers("SMA8",
-            launcher_assignments={
-                1: "PL-1-IN", 2: "PL-2-IN",
-                3: "PL-4-IN", 4: "PL-4-OUT",
-                5: "PL-2-OUT", 6: "PL-1-OUT",
-                7: "PL-3-OUT", 8: "PL-3-IN"
-            }
-        )
+        launchers = self.produce_launchers("SMA8")
         self._produce_transmission_lines(launchers)
 
     def _produce_transmission_lines(self, launchers):
         distance = 700
         right_tr_x = 5000 + distance
         left_tr_x = 5000 - distance
         face1_box = self.get_box(1)
 
         # Left transmission line
-        nodes = [Node(self.refpoints["PL-1-IN_port"]),
-                 Node(self.refpoints["PL-1-IN_port_corner"] + pya.DPoint(0, - 2 * self.r)),
-                 Node((left_tr_x, self.refpoints["PL-1-IN_port_corner"].y - 2 * self.r)),
+        nodes = [Node(self.refpoints["NW_port"]),
+                 Node(self.refpoints["NW_port_corner"] + pya.DPoint(0, - 2 * self.r)),
+                 Node((left_tr_x, self.refpoints["NW_port_corner"].y - 2 * self.r)),
                  Node((left_tr_x, face1_box.p2.y), a=self.a_capped, b=self.b_capped),
                  Node((left_tr_x, face1_box.p1.y + 100), a=self.a, b=self.b),
-                 Node((left_tr_x, self.refpoints["PL-1-OUT_port_corner"].y + 2 * self.r)),
-                 Node(self.refpoints["PL-1-OUT_port_corner"] + pya.DPoint(0, 2 * self.r)),
-                 Node(self.refpoints["PL-1-OUT_port"])
+                 Node((left_tr_x, self.refpoints["SW_port_corner"].y + 2 * self.r)),
+                 Node(self.refpoints["SW_port_corner"] + pya.DPoint(0, 2 * self.r)),
+                 Node(self.refpoints["SW_port"])
                  ]
 
         self.insert_cell(WaveguideComposite, nodes=nodes)
 
         # Right transmission line
-        nodes = [Node(self.refpoints["PL-2-IN_port"]),
-                 Node(self.refpoints["PL-2-IN_port_corner"] + pya.DPoint(0, - 2 * self.r)),
-                 Node((right_tr_x, self.refpoints["PL-2-IN_port_corner"].y - 2 * self.r)),
+        nodes = [Node(self.refpoints["NE_port"]),
+                 Node(self.refpoints["NE_port_corner"] + pya.DPoint(0, - 2 * self.r)),
+                 Node((right_tr_x, self.refpoints["NE_port_corner"].y - 2 * self.r)),
                  Node((right_tr_x, face1_box.p2.y),
                       a=self.a_capped, b=self.b_capped),
                  Node((right_tr_x, face1_box.p1.y + 100), a=self.a, b=self.b),
-                 Node((right_tr_x, self.refpoints["PL-2-OUT_port_corner"].y + 2 * self.r)),
-                 Node(self.refpoints["PL-2-OUT_port_corner"] + pya.DPoint(0, 2 * self.r)),
-                 Node(self.refpoints["PL-2-OUT_port"])
+                 Node((right_tr_x, self.refpoints["SE_port_corner"].y + 2 * self.r)),
+                 Node(self.refpoints["SE_port_corner"] + pya.DPoint(0, 2 * self.r)),
+                 Node(self.refpoints["SE_port"])
                  ]
 
         self.insert_cell(WaveguideComposite, nodes=nodes)
 
         # Crossing transmission line
-        nodes = [Node(self.refpoints["PL-3-IN_port"]),
-                 Node((face1_box.p1.x, self.refpoints["PL-3-IN_port"].y),
+        nodes = [Node(self.refpoints["WN_port"]),
+                 Node((face1_box.p1.x, self.refpoints["WN_port"].y),
                       a=self.a_capped, b=self.b_capped)]
         ref_x = left_tr_x
         ref_x_1 = ref_x - self.crossing_length / 2.
         ref_x_2 = ref_x + self.crossing_length / 2.
 
-        last_y = launchers["PL-3-IN"][0].y
+        last_y = launchers["WN"][0].y
         crossings = self.crossings  # must be even
-        step = (launchers["PL-3-IN"][0].y - launchers["PL-3-OUT"][0].y) / (crossings - 0.5) / 2
+        step = (launchers["WN"][0].y - launchers["WS"][0].y) / (crossings - 0.5) / 2
         wiggle = self.crossing_length / 2. + 250
 
         for i in range(crossings):
             nodes.append(Node((ref_x - wiggle, last_y)))
             nodes.append(Node((ref_x_1, last_y), face_id=self.face_ids[1]))
             nodes.append(Node((ref_x_2, last_y), face_id=self.face_ids[0]))
             nodes.append(Node((ref_x + wiggle, last_y)))
             last_y -= step
             nodes.append(Node((ref_x + wiggle, last_y)))
             nodes.append(Node((ref_x_2, last_y), face_id=self.face_ids[1]))
             nodes.append(Node((ref_x_1, last_y), face_id=self.face_ids[0]))
             nodes.append(Node((ref_x - wiggle, last_y)))
             last_y -= step
-        nodes.append(Node((face1_box.p1.x + 100, self.refpoints["PL-3-OUT_port"].y), a=self.a, b=self.b))
-        nodes.append(Node(self.refpoints["PL-3-OUT_port_corner"]))
-        nodes.append(Node(self.refpoints["PL-3-OUT_port"]))
+        nodes.append(Node((face1_box.p1.x + 100, self.refpoints["WS_port"].y), a=self.a, b=self.b))
+        nodes.append(Node(self.refpoints["WS_port_corner"]))
+        nodes.append(Node(self.refpoints["WS_port"]))
         self.insert_cell(WaveguideComposite, nodes=nodes)
 
         # cross_talk
         ref_x = right_tr_x + self.cross_talk_distance + wiggle
-        last_y = self.refpoints["PL-4-IN_port"].y
-        nodes = [Node(self.refpoints["PL-4-IN_port"]),
-                 Node(self.refpoints["PL-4-IN_port_corner"]),
-                 Node((face1_box.p2.x, self.refpoints["PL-4-IN_port"].y),
+        last_y = self.refpoints["EN_port"].y
+        nodes = [Node(self.refpoints["EN_port"]),
+                 Node(self.refpoints["EN_port_corner"]),
+                 Node((face1_box.p2.x, self.refpoints["EN_port"].y),
                       a=self.a_capped, b=self.b_capped)]
         for i in range(crossings):
             if i == 0 and self.meander_face == "Two Face":
                 nodes.append(
                     Node((ref_x + wiggle, last_y), face_id=self.face_ids[1]))
             else:
                 nodes.append(Node((ref_x + wiggle, last_y)))
@@ -128,12 +121,12 @@
             last_y -= step
             nodes.append(Node((ref_x - wiggle, last_y)))
             if i == range(crossings)[-1] and self.meander_face == "Two Face":
                 nodes.append(Node((ref_x + wiggle, last_y), face_id=self.face_ids[0]))
             else:
                 nodes.append(Node((ref_x + wiggle, last_y)))
             last_y -= step
-        nodes.append(Node((face1_box.p2.x - 100, self.refpoints["PL-4-OUT_port"].y),
+        nodes.append(Node((face1_box.p2.x - 100, self.refpoints["ES_port"].y),
                           a=self.a, b=self.b))
-        nodes.append(Node(self.refpoints["PL-4-OUT_port_corner"]))
-        nodes.append(Node(self.refpoints["PL-4-OUT_port"]))
+        nodes.append(Node(self.refpoints["ES_port_corner"]))
+        nodes.append(Node(self.refpoints["ES_port"]))
         self.insert_cell(WaveguideComposite, nodes=nodes)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/daisy_woven.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/daisy_woven.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/dc_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/dc_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/demo.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,24 +40,24 @@
     include_couplers = Param(pdt.TypeBoolean, "Include couplers between qubits", True)
 
     def build(self):
 
         launcher_assignments = {
             # N
             2: "FL-QB1",
-            3: "PL-1-IN",
-            4: "PL-1-OUT",
+            3: "PL-A-IN",
+            4: "PL-A-OUT",
             5: "FL-QB2",
             # E
             7: "DL-QB2",
             12: "DL-QB4",
             # S
             14: "FL-QB4",
-            15: "PL-2-IN",
-            16: "PL-2-OUT",
+            15: "PL-B-IN",
+            16: "PL-B-OUT",
             17: "FL-QB3",
             # W
             19: "DL-QB3",
             24: "DL-QB1",
         }
         self.produce_launchers("ARD24", launcher_assignments)
 
@@ -172,16 +172,16 @@
 
         self.insert_cell(WaveguideCoplanarSplitter, pya.DTrans(tcross_rot, False, 0, 0),
                          inst_name="PL{}".format(qubit_nr),
                          label_trans=pya.DCplxTrans(0.2), align_to=cap_ref_abs["port_b"], align="port_bottom",
                          **t_cross_parameters(a=self.a, b=self.b, a2=self.a, b2=self.b, length_extra_side=30))
 
     def produce_probelines(self):
-        self.produce_probeline("PL-1", 1, 2, False, 6)
-        self.produce_probeline("PL-2", 4, 3, True, 3)
+        self.produce_probeline("PL-A", 1, 2, False, 6)
+        self.produce_probeline("PL-B", 4, 3, True, 3)
 
     def produce_probeline(self, probeline_name, qubit_a_nr, qubit_b_nr, mirrored, cap_finger_nr):
 
         if mirrored:
             cap_rot = 1
             cap_pos_shift = pya.DPoint(0, -2000)
         else:
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/demo_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/demo_twoface.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,24 @@
     name_chip = Param(pdt.TypeString, "Name of the chip", "DT")
 
     def build(self):
 
         launcher_assignments = {
             # N
             2: "FL-QB1",
-            3: "PL-1-IN",
-            4: "PL-2-IN",
+            3: "PL-A-IN",
+            4: "PL-B-IN",
             5: "FL-QB2",
             # E
             7: "DL-QB2",
             12: "DL-QB4",
             # S
             14: "FL-QB4",
-            15: "PL-2-OUT",
-            16: "PL-1-OUT",
+            15: "PL-B-OUT",
+            16: "PL-A-OUT",
             17: "FL-QB3",
             # W
             19: "DL-QB3",
             24: "DL-QB1",
         }
         self.produce_launchers("ARD24", launcher_assignments)
 
@@ -168,16 +168,16 @@
         tcross_cell = self.add_element(WaveguideCoplanarSplitter, **t_cross_parameters(
             a=self.a, b=self.b, a2=self.a, b2=self.b, length_extra_side=30, face_ids=[self.face_ids[1]]))
         tcross_ref_rel = self.get_refpoints(tcross_cell, pya.DTrans(tcross_rot, False, 0, 0))
         tcross_trans = pya.DTrans(tcross_rot, False, cap_ref_abs["port_b"] - tcross_ref_rel["port_bottom"])
         self.insert_cell(tcross_cell, tcross_trans, inst_name="PL{}".format(qubit_nr), label_trans=pya.DCplxTrans(0.2))
 
     def produce_probelines(self):
-        self.produce_probeline("PL-1", 1, 3, True, 4)
-        self.produce_probeline("PL-2", 2, 4, False, 6)
+        self.produce_probeline("PL-A", 1, 3, True, 4)
+        self.produce_probeline("PL-B", 2, 4, False, 6)
 
     def produce_probeline(self, probeline_name, qubit_a_nr, qubit_b_nr, mirrored, cap_finger_nr):
 
         cap_cell = self.add_element(FingerCapacitorTaper,
             finger_number=cap_finger_nr,
             taper_length=20,
             face_ids=[self.face_ids[1]]
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/empty.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/empty.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/junction_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/junction_test2.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/junction_test2.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/launchers.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/launchers.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/lithography_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/lithography_test_twoface.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/lithography_test_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/quality_factor.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/quality_factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,39 +79,39 @@
         if self.resonators_both_sides:
             wg_top_y = chip_side / 2
         else:
             wg_top_y = (chip_side + max_res_len) / 2
 
         # Non-standard Launchers mimicking SMA8 at 1cm chip size, but keeping fixed distance from top
         launchers = self.produce_n_launchers(8, "RF", 300, 180, self.launcher_indent,
-                                             chip_side - 2 * self.launcher_top_dist, {8: "PL-1-IN", 3: "PL-1-OUT"})
+                                             chip_side - 2 * self.launcher_top_dist, {8: "PL-IN", 3: "PL-OUT"})
 
         # Define start and end of feedline
-        points_fl = [launchers["PL-1-IN"][0]]
-        if abs(launchers["PL-1-IN"][0].y - wg_top_y) > 1:
+        points_fl = [launchers["PL-IN"][0]]
+        if abs(launchers["PL-IN"][0].y - wg_top_y) > 1:
             # Bend in the feedline needed
             points_fl += [
-                launchers["PL-1-IN"][0] + pya.DVector(self.r + self.marker_safety, 0),
-                pya.DPoint(launchers["PL-1-IN"][0].x + self.r + self.feedline_bend_distance + self.marker_safety,
+                launchers["PL-IN"][0] + pya.DVector(self.r + self.marker_safety, 0),
+                pya.DPoint(launchers["PL-IN"][0].x + self.r + self.feedline_bend_distance + self.marker_safety,
                            wg_top_y)
             ]
             points_fl_end = [
-                pya.DPoint(launchers["PL-1-OUT"][0].x - self.r - self.feedline_bend_distance - self.marker_safety,
+                pya.DPoint(launchers["PL-OUT"][0].x - self.r - self.feedline_bend_distance - self.marker_safety,
                            wg_top_y),
-                launchers["PL-1-OUT"][0] + pya.DVector(-self.r - self.marker_safety, 0),
+                launchers["PL-OUT"][0] + pya.DVector(-self.r - self.marker_safety, 0),
             ]
         elif self.marker_safety > 0:
-            points_fl += [launchers["PL-1-IN"][0] + pya.DVector(self.marker_safety, 0)]
+            points_fl += [launchers["PL-IN"][0] + pya.DVector(self.marker_safety, 0)]
             points_fl_end = [
-                launchers["PL-1-OUT"][0] + pya.DVector(-self.marker_safety, 0),
+                launchers["PL-OUT"][0] + pya.DVector(-self.marker_safety, 0),
             ]
         else:
             points_fl_end = []
 
-        points_fl_end += [launchers["PL-1-OUT"][0]]
+        points_fl_end += [launchers["PL-OUT"][0]]
 
         tl_start = points_fl[-1]
         tl_end = points_fl_end[0]
 
         resonators = len(self.res_lengths)
         v_res_step = (tl_end - tl_start) * (1. / resonators)
         cell_cross = self.add_element(WaveguideCoplanarSplitter, **t_cross_parameters(
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/sample_holder_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/sample_holder_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,40 +35,30 @@
     n_launchers = Param(pdt.TypeInt, "Number of launchers", 40, unit="")
     launcher_pitch = Param(pdt.TypeDouble, "Launcher pitch", 635, unit="μm")
     launcher_width = Param(pdt.TypeDouble, "Launcher width", 160, unit="μm")
     launcher_gap = Param(pdt.TypeDouble, "Launcher gap", 96, unit="μm")
     launcher_indent = Param(pdt.TypeDouble, "Launcher indent from edge", 520, unit="μm")
 
     def build(self):
-        nr_pads_per_side = int(self.n_launchers / 4.)
-
-        # North edge
-        launcher_assigments = {i: f"PL-{i}-IN" for i in range(1, nr_pads_per_side + 1)}
-        # East edge
-        launcher_assigments.update({pin: f"PL-{pl+1}-OUT" for pl, pin in
-                                    enumerate(range(2 * nr_pads_per_side, nr_pads_per_side, -1))})
-        # South edge
-        launcher_assigments.update({pin: f"PL-{pl + nr_pads_per_side + 1}-OUT" for pl, pin in
-                                    enumerate(range(2 * nr_pads_per_side + 1, 3 * nr_pads_per_side + 1))})
-        # West edge
-        launcher_assigments.update({pin: f"PL-{pl + nr_pads_per_side + 1}-IN" for pl, pin in
-                                    enumerate(range(4 * nr_pads_per_side, 3 * nr_pads_per_side, -1))})
-
         self.produce_n_launchers(self.n_launchers, "RF", self.launcher_width, self.launcher_gap, self.launcher_indent,
-                                 self.launcher_pitch, launcher_assignments=launcher_assigments)
+                                 self.launcher_pitch)
 
-        def _produce_waveguide(i, straight_distance, first_port, second_port):
+        nr_pads_per_side = int(self.n_launchers / 4.)
+
+        def _produce_waveguide(i, j, straight_distance):
             cell = self.add_element(WaveguideComposite, nodes=[
-                Node(self.refpoints[f'PL-{i}-{first_port}_port']),
-                Node(self.refpoints[f'PL-{i}-{first_port}_port_corner'] + pya.DVector(0, straight_distance)),
-                Node(self.refpoints[f'PL-{i}-{second_port}_port_corner'] + pya.DVector(straight_distance, 0)),
-                Node(self.refpoints[f'PL-{i}-{second_port}_port']),
+                Node(self.refpoints[f'{i}_port']),
+                Node(self.refpoints[f'{i}_port_corner'] + pya.DVector(0, straight_distance)),
+                Node(self.refpoints[f'{j}_port_corner'] + pya.DVector(straight_distance, 0)),
+                Node(self.refpoints[f'{j}_port']),
             ])
             self.insert_cell(cell)
 
-            self.__log.info(f"{self.name_chip}: Waveguide PL-{i} length: {cell.length()}")
-
-        for i in range(1, nr_pads_per_side + 1):
-            _produce_waveguide(i, -1200, first_port="IN", second_port="OUT")
+            self.__log.info("%s: Waveguide %d-%d length: %s", self.name_chip, i, j, cell.length())
 
-        for i in range(nr_pads_per_side + 1, nr_pads_per_side * 2 + 1):
-            _produce_waveguide(i, 1200, first_port="OUT", second_port="IN")
+        for i, j in zip(range(1, nr_pads_per_side + 1),
+                        range(2 * nr_pads_per_side, nr_pads_per_side, -1)):
+            _produce_waveguide(i, j, -1200)
+
+        for i, j in zip(range(2 * nr_pads_per_side + 1, 3 * nr_pads_per_side + 1),
+                        range(4 * nr_pads_per_side, 3 * nr_pads_per_side, -1)):
+            _produce_waveguide(i, j, 1200)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/shaping.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/shaping.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/simple.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/simple.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/single_xmons.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/single_xmons.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/stripes.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/stripes.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/tsv_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/tsv_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/chips/xmons_direct_coupling.py` & `kqcircuits-4.6.9rc1/kqcircuits/chips/xmons_direct_coupling.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/defaults.py` & `kqcircuits-4.6.9rc1/kqcircuits/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 default_fluxline_type = "Fluxline Standard"
 default_marker_type = "Marker Standard"
 default_junction_test_pads_type = "Junction Test Pads Simple"
 default_tsv_type = "Tsv Standard"
 
 default_drc_runset = "example.lydrc"
 
-# Default list of Elements to break down before netlist export.
+# default elements to breakdown before netlist export
+# list of strings
 default_netlist_breakdown = [
     "Waveguide Composite",
     "Meander",
 ]
 
 default_netlist_ignore_connections = [
     ("drive", "drive"), # Don't connect two overlapping qubit drive ports
@@ -176,17 +177,14 @@
 # an instance of each PCell which is clumsy to run at startup.
 # In the list below basic waveguide elements are omitted since they can be better generated by other node parameters
 node_editor_valid_elements = [
     'Airbridge', 'AirbridgeConnection', 'AirbridgeMultiFace', 'AirbridgeRectangular', 'CircularCapacitor',
     'FingerCapacitorSquare', 'FingerCapacitorTaper', 'FlipChipConnectorRf', 'SmoothCapacitor',
     'WaveguideCoplanarSplitter']
 
-node_editor_layer_changing_elements = ['FlipChipConnectorRf']
-
-
 # Path to the layer configuration file, which defines layer/face related defaults.
 # The path can be either absolute or relative.
 layer_config_path = Path(__file__).parent/"layer_config"/"default_layer_config.py"
 
 # Load layer/face related defaults from the layer config file
 
 layer_config_module = module_from_file(layer_config_path)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/airbridge_connection.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridge_connection.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/airbridges/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/airbridges/airbridge.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/airbridges/airbridge_multi_face.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_multi_face.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/airbridges/airbridge_rectangular.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/airbridges/airbridge_rectangular.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/chip_frame.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/chip_frame.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/circular_capacitor.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/circular_capacitor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/daisy_woven.oas` & `kqcircuits-4.6.9rc1/kqcircuits/elements/daisy_woven.oas`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/element.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,19 +419,18 @@
         return get_refpoints(self.layout.layer(default_layers["refpoints"]), cell, cell_transf, rec_levels)
 
     def get_layer(self, layer_name, face_id=0):
         """Returns the specified Layer object.
 
         Args:
             layer_name: layer name text
-            face_id: Name or index of the face to use, default=0
+            face_id: index of the face id, default=0
+
         """
-        if isinstance(face_id, str):
-            return self.layout.layer(self.face(self.face_ids.index(face_id))[layer_name])
-        elif (face_id == 0) and (layer_name not in self.face(0)):
+        if (face_id == 0) and (layer_name not in self.face(0)):
             return self.layout.layer(default_layers[layer_name])
         else:
             return self.layout.layer(self.face(face_id)[layer_name])
 
     @staticmethod
     def _create_cell(elem_cls, layout, library=None, **parameters) -> pya.Cell:
         """Create cell for elem_cls in layout.
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/finger_capacitor_square.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_square.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/finger_capacitor_taper.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/finger_capacitor_taper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 from autologging import logged
 
-from kqcircuits.elements.finger_capacitor_square import FingerCapacitorSquare
 from kqcircuits.elements.flip_chip_connectors import connector_type_choices
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector import FlipChipConnector
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector_dc import FlipChipConnectorDc
 from kqcircuits.elements.launcher import Launcher
 from kqcircuits.pya_resolver import pya
-from kqcircuits.util.parameters import Param, pdt, add_parameters_from
+from kqcircuits.util.parameters import Param, pdt
 
 
-@add_parameters_from(FingerCapacitorSquare, "a2", "b2")
 @logged
 class FlipChipConnectorRf(FlipChipConnector):
     """PCell declaration for an inter-chip rf connector.
 
     Flip chip connector with two coplanar waveguide connections and different ground bump configurations.
     The input port is on the first face and on the left. The output port is on the second face and rotated as chosen.
 
@@ -48,88 +46,63 @@
     output_rotation = Param(pdt.TypeDouble, "Rotation of output port w.r.t. input port", 180, unit="degrees")
     connector_a = Param(pdt.TypeDouble, "Conductor width at the connector area", 40, unit="μm")
     connector_b = Param(pdt.TypeDouble, "Gap width at the connector area", 40, unit="μm")
     round_connector = Param(pdt.TypeBoolean, "Use round connector shape", False)
     n_center_bumps = Param(pdt.TypeInt, "Number of center bumps in series", 1)
 
     def build(self):
-
         # Flip-chip bump
-        bump = self.add_element(FlipChipConnectorDc, face_ids=self.face_ids)
+        bump = self.add_element(FlipChipConnectorDc)
         for i in range(self.n_center_bumps):
             self.insert_cell(bump, pya.DTrans((i - (self.n_center_bumps - 1) / 2) * self.inter_bump_distance, 0))
         bump_ref = self.get_refpoints(bump)
         self.__log.debug("bump_ref: %s", bump_ref)
 
-        a2 = self.a2 if self.a2 >= 0 else self.a
-        b2 = self.b2 if self.b2 >= 0 else self.b
-
+        tt = pya.DCplxTrans(1, self.output_rotation, False, 0, 0)  # top transformation
         if self.round_connector:
             # Rounded geometry
-            def rounded_plate(center_x, width, length):
-                reg = pya.Region(pya.DBox(center_x - length / 2, -width / 2,
-                                          center_x + length / 2, width / 2).to_itype(self.layout.dbu))
-                return reg.rounded_corners(0, min(width, length) / (2 * self.layout.dbu), self.n)
-
-            def trace(start_x, width, length):
-                return pya.Region(pya.DBox(start_x, -width / 2, start_x + length, width / 2).to_itype(self.layout.dbu))
+            def rounded_plate_with_trace(trace_x, plate_x, trace_width, plate_width, plate_length):
+                reg = pya.Region(pya.DBox(plate_x - plate_length / 2, -plate_width / 2,
+                                          plate_x + plate_length / 2, plate_width / 2).to_itype(self.layout.dbu))
+                reg.round_corners(0, min(plate_width, plate_length) / (2 * self.layout.dbu), self.n)
+                reg += pya.Region(pya.DBox(trace_x, -trace_width / 2,
+                                           plate_x, trace_width / 2).to_itype(self.layout.dbu))
+                return reg
 
             w = self.connector_a + 2 * self.connector_b
-            bumps_length = (self.n_center_bumps - 1) * self.inter_bump_distance
-            length = w + bumps_length
-
-            def produce_shape(face, a, b, rotation, trace_rotation):
-                # Base metal gap outline
-                trace_dtrans = pya.DCplxTrans(1, trace_rotation, False, - bumps_length / 2, 0)
-                trace_itrans = trace_dtrans.to_itrans(self.layout.dbu)
-                region = rounded_plate(0, w, length) + trace(0, a + 2 * b, - w / 2).transformed(trace_itrans)
-                self.__log.info(f'{str(trace_itrans)=}')
-
-                # Ground grid avoidance
-                avoid_region = region.sized(self.margin / self.layout.dbu, self.margin / self.layout.dbu, 2)
-
-                # Subtract circles under bumps
-                for i in range(self.n_center_bumps):
-                    region -= rounded_plate((i - (self.n_center_bumps - 1) / 2) * self.inter_bump_distance,
-                                            self.connector_a, self.connector_a)
-
-                # Subtract input trace with possible rotation
-                region -= trace(0, a, - w / 2).transformed(trace_itrans)
-
-                # Subtract trace connecting the series bumps
-                region -= trace(- bumps_length / 2, a, bumps_length)
-
-                dtrans = pya.DCplxTrans(1, rotation, False, 0, 0)
-                itrans = dtrans.to_itrans(self.layout.dbu)
-                self.cell.shapes(self.get_layer("base_metal_gap_wo_grid", face)).insert(region.transformed(itrans))
-                self.add_protection(avoid_region.transformed(itrans), face, 0)
-                self.add_port("{}_port".format(self.face_ids[face]),
-                              dtrans * pya.DPoint(-bumps_length/2, 0) + trace_dtrans * dtrans * pya.DVector(-w/2, 0),
-                              trace_dtrans * dtrans * pya.DVector(-1, 0), face)
-
-            produce_shape(0, self.a, self.b, 0, 0)
-            produce_shape(1, a2, b2, 180, self.output_rotation - 180)
-
+            l = w + (self.n_center_bumps - 1) * self.inter_bump_distance
+            region = rounded_plate_with_trace(-l/2, 0, self.a + 2 * self.b, w, l)
+            avoid_region = region.sized(self.margin / self.layout.dbu, self.margin / self.layout.dbu, 2)
+            for i in range(self.n_center_bumps):
+                region -= rounded_plate_with_trace(-l/2, (i - (self.n_center_bumps - 1) / 2) * self.inter_bump_distance,
+                                                   self.a, self.connector_a, self.connector_a)
+
+            self.cell.shapes(self.get_layer("base_metal_gap_wo_grid")).insert(region)
+            self.cell.shapes(self.get_layer("base_metal_gap_wo_grid", 1)).insert(region.transformed(pya.ICplxTrans(tt)))
+            self.add_protection(avoid_region)
+            self.add_protection(avoid_region.transformed(pya.ICplxTrans(tt)), 1, 0)
+
+            # add reference point
+            self.add_port("{}_port".format(self.face_ids[0]), pya.DPoint(-l/2, 0), pya.DVector(-1, 0), 0)
+            self.add_port("{}_port".format(self.face_ids[1]), tt * pya.DPoint(-l/2, 0), tt * pya.DVector(-1, 0), 1)
         else:
             # Taper geometry
             s = self.ubm_diameter + (self.n_center_bumps - 1) * self.inter_bump_distance
             trans = pya.DCplxTrans(1, 0, False, bump_ref["base"] + pya.DPoint(- self.ubm_diameter - s / 2, 0))
-            tt = pya.DCplxTrans(1, self.output_rotation, False, 0, 0)
             self.insert_cell(Launcher, trans, self.face_ids[0], s=s, l=self.ubm_diameter,
                              a_launcher=self.connector_a, b_launcher=self.connector_b,
                              launcher_frame_gap=self.connector_b)
             self.insert_cell(Launcher, tt * trans, self.face_ids[1], s=s, l=self.ubm_diameter,
                              a_launcher=self.connector_a, b_launcher=self.connector_b,
-                             launcher_frame_gap=self.connector_b, face_ids=[self.face_ids[1], self.face_ids[0]],
-                             a=a2, b=b2)
+                             launcher_frame_gap=self.connector_b, face_ids=[self.face_ids[1], self.face_ids[0]])
 
         # Insert ground bumps
         if self.connector_type == "GSG":
-            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, 0, self.inter_bump_distance))
-            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, 0, -self.inter_bump_distance))
+            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, pya.DPoint(0, self.inter_bump_distance)))
+            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, pya.DPoint(0, -self.inter_bump_distance)))
         elif self.connector_type == "Coax":
             dist_y = 0.5**0.5 * self.inter_bump_distance
             dist_x = dist_y + self.inter_bump_distance * (self.n_center_bumps - 1) / 2
-            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, dist_x, dist_y))
-            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, -dist_x, dist_y))
-            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, dist_x, -dist_y))
-            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, -dist_x, -dist_y))
+            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, pya.DPoint(dist_x, dist_y)))
+            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, pya.DPoint(-dist_x, dist_y)))
+            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, pya.DPoint(dist_x, -dist_y)))
+            self.insert_cell(bump, pya.DCplxTrans(1, 0, False, pya.DPoint(-dist_x, -dist_y)))
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/fluxlines/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/fluxlines/fluxline.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/fluxlines/fluxline_standard.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/fluxlines/fluxline_straight.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/fluxlines/fluxline_straight.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/launcher.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/launcher.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/launcher_dc.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/launcher_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/markers/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/markers/marker.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/markers/marker_standard.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/markers/marker_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/mask_marker_fc.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/mask_marker_fc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/meander.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/meander.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/smooth_capacitor.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/smooth_capacitor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/spiral_resonator_polygon.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/spiral_resonator_polygon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/tsvs/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/tsvs/tsv.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/tsvs/tsv_ellipse.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_ellipse.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,29 +39,26 @@
         """
         Generate elliptical TSV
         """
         # shorthand
         r = self.tsv_diameter / 2
         w = self.tsv_elliptical_width / 2
         m = self.margin
-        n = self.n
 
         # parametric representation is taken from https://en.wikipedia.org/wiki/Superellipse
         p1 = 6
         p2 = 2
         # Protection layer
         tsv_pts_avoidance = [pya.DPoint(
             numpy.abs(math.cos(a)) ** (2 / p1) * (w + m) * numpy.sign(math.cos(a)),
             numpy.abs(math.sin(a)) ** (2 / p2) * (r + m) * numpy.sign(math.sin(a))) for a in
-            (x / n * 2 * math.pi for x in range(0, n + 1))]
+            (x / 32 * math.pi for x in range(0, 65))]
 
         tsv_pts = [
             pya.DPoint(numpy.abs(math.cos(a)) ** (2 / p1) * w * numpy.sign(math.cos(a)),
                        numpy.abs(math.sin(a)) ** (2 / p2) * r * numpy.sign(math.sin(a))) for
-            a in (x / n * 2 * math.pi for x in range(0, n + 1))]
+            a in (x / 32 * math.pi for x in range(0, 65))]
 
         shape = pya.DPolygon(tsv_pts_avoidance)
         # ground avoidance layer 1t1 face
         self.cell.shapes(self.get_layer("ground_grid_avoidance")).insert(shape)
-        self.cell.shapes(self.get_layer("ground_grid_avoidance", 1)).insert(shape)
-        self.cell.shapes(self.get_layer("through_silicon_via")).insert(pya.DPolygon(tsv_pts))
-        self.cell.shapes(self.get_layer("through_silicon_via", 1)).insert(pya.DPolygon(tsv_pts))
+        self.cell.shapes(self.get_layer("through_silicon_via")).insert(pya.DPolygon(tsv_pts))  # TSV only on 1t1 face
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/tsvs/tsv_standard.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/tsvs/tsv_standard.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,12 @@
 
     Origin is at the geometric center. Geometry es circular.
 
     .. MARKERS_FOR_PNG 0,0
     """
 
     def build(self):
-        tsv = circle_polygon(self.tsv_diameter / 2, self.n)
+        tsv = circle_polygon(self.tsv_diameter / 2)
         self.cell.shapes(self.get_layer("through_silicon_via")).insert(tsv)
-        self.cell.shapes(self.get_layer("through_silicon_via", 1)).insert(tsv)
-        margin = circle_polygon(self.tsv_diameter / 2 + self.margin, self.n)
+        margin = circle_polygon(self.tsv_diameter / 2 + self.margin)
         self.cell.shapes(self.get_layer("ground_grid_avoidance")).insert(margin)
-        self.cell.shapes(self.get_layer("ground_grid_avoidance", 1)).insert(margin)
         del self.refpoints['base']
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/waveguide_composite.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_composite.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from itertools import zip_longest
 from typing import Tuple
 from math import pi, tan
 from autologging import logged
 
 from scipy.optimize import root_scalar
 
-from kqcircuits.defaults import node_editor_layer_changing_elements
 from kqcircuits.pya_resolver import pya
 from kqcircuits.util.parameters import Param, pdt, add_parameters_from
 from kqcircuits.util.library_helper import element_by_class_name
 from kqcircuits.util.geometry_helper import vector_length_and_direction, point_shift_along_vector, \
     get_cell_path_length, get_angle, get_direction
 from kqcircuits.elements.element import Element
 from kqcircuits.elements.airbridges.airbridge import Airbridge
@@ -172,16 +171,16 @@
         node_list = ast.literal_eval(nlas + ",")
 
         return [Node.deserialize(node) for node in node_list]
 
 
 @add_parameters_from(WaveguideCoplanarTaper, taper_length=100)
 @add_parameters_from(Airbridge, "airbridge_type")
-@add_parameters_from(WaveguideCoplanar, "term1", "term2", "add_metal")
 @add_parameters_from(FlipChipConnectorRf)
+@add_parameters_from(WaveguideCoplanar, "term1", "term2")
 @logged
 class WaveguideComposite(Element):
     """A composite waveguide made of waveguides and other elements.
 
     From the user's perspective this is a WaveguideCoplanar that is extended with Airbridge,
     WaveguideCoplanarTaper and FlipChipConnector, so that a signal can be routed over other
     waveguides and several chip faces. As a bonus feature other arbitrary elements like coplanar
@@ -204,18 +203,14 @@
     parameter puts N airbridges evenly distributed across the preceding edge.
 
     The ``length_before`` parameter of a node can be specified to automatically set the length of
     the waveguide between that node and the previous one. It will in fact create a Meander element
     instead of a normal waveguide between those nodes to achieve the correct length. Alternative parameter
     ``length_increment`` sets the waveguide length increment compared to normal waveguide.
 
-    If ``add_metal`` parameter is set to ``True`` for a node then the specified WaveguideCoplanar
-    segment will also use the "base metal addition" layer so that a waveguide trace may continue
-    inside a metal gap region.
-
     A notable implementation detail is that every Airbridge (sub)class is done as AirbridgeConnection.
     This way a waveguide taper is automatically inserted before and after the airbridge so the user
     does not have to manually add these. Other Node types do not have this feature.
 
     A WaveguideComposite cell has a method ``segment_lengths`` that returns a list of lengths of each individual
     regular waveguide segment. Segments are bounded by any element that is not a standard waveguide, such as Airbridge,
     flip chip, taper or any custom element.
@@ -246,79 +241,24 @@
 
         cell = super().create(layout, library, **parameters)
         setattr(cell, "segment_lengths", lambda: WaveguideComposite.get_segment_lengths(cell))
 
         return cell
 
     @staticmethod
-    def get_segment_cells(cell):
-        """Get the subcells of a ``WaveguideComposite`` cell, ordered by node index.
-
-        The subcells include ``WaveguideCoplanar``, ``WaveguideCoplanarTaper`` and ``Meander`` cells for straight,
-        tapered and meandering segments, respectively, and any element cells that were inserted explicitly
-        (``element`` argument) or implicitly (changing ``a``, ``b`` or ``face_id``) at any ``Node``.
-
-        The ``node_index`` returned with each subcell is an index to the ``nodes`` parameter of the
-        ``WaveguideComposite`` cell. It points to the node that _created_ the subcell, which is the node following a
-        segment for regular ``WaveguideCoplanar`` segments, and the node that specified the element or parameter change
-        otherwise.
-
-        Note that there may be multiple subcells per node, and some nodes may not have associated subcells (in
-        particular, regular ``WaveguideCoplanar`` segments are merged when possible). Subscells are returned in the
-        order in which they appear in the waveguide.
-
-        Args:
-            cell: A WaveguideComposite cell. Can be a PCell or static cell created from a PCell.
-
-        Returns: A list of tuples (node_index: int, subcell: pya.Cell) ordered by node_index.
-        """
-        layout = cell.layout()
-
-        segment_data = []
-
-        for inst in cell.each_inst():
-            # Note: Using layout.cell(inst.cell_index) instead of inst.cell to work around KLayout issue #235
-            child_cell = layout.cell(inst.cell_index)
-
-            node_index = inst.property("waveguide_composite_node_index")
-            if node_index is not None:
-                segment_data.append((node_index, child_cell))
-
-        return list(sorted(reversed(segment_data), key=lambda x: x[0]))
-
-    @staticmethod
     def get_segment_lengths(cell):
-        """ Retrieves the segment lengths of each waveguide segment in a WaveguideComposite cell.
-
-        Waveguide segments are ``WaveguideCoplanar``, ``WaveguideCoplanarTaper`` and ``Meander`` subcells.
-        This method returns a list with the same length as the ``nodes`` parameter, where each element is the total
-        length of all waveguides directly preceding and/or defined in that node. For example, for a taper node both the
-        preceding regular waveguide and the taper itself are counted.
-
-        Note that ``WaveguideComposite`` merges consecutive waveguide segments if they have no special elements. As
-        a consequence, the corresponding waveguide lengths all accumulate in the next index which has a taper, meander
-        or other element, and the length for nodes that contain ony ``WaveguideCoplanar`` is reported as 0.
-
-        Args:
-            cell: A WaveguideComposite cell. Can be a PCell or static cell created from a PCell.
-
-        Returns: A list waveguide lengths per node
+        """ Retreives the segment lengths of each waveguide segment in a WaveguideComposite cell
         """
 
         # Measure segment lengths, counting only "regular waveguides"
-        waveguide_segment_types = {"Waveguide Coplanar", "Waveguide Coplanar Taper", "Meander"}
-
-        segment_data = WaveguideComposite.get_segment_cells(cell)
-        if len(segment_data) == 0:
-            return []
-
-        segment_lengths = [0] * (segment_data[-1][0] + 1)
-        for node_index, child_cell in segment_data:
-            if child_cell.name.split('$')[0] in waveguide_segment_types:
-                segment_lengths[node_index] += get_cell_path_length(child_cell)
+        layout = cell.layout()
+        # Note: Using layout.cell(inst.cell_index) instead of inst.cell to work around KLayout issue #235
+        child_cells = [layout.cell(inst.cell_index) for inst in cell.each_inst()]
+        segment_lengths = [get_cell_path_length(child_cell) for child_cell in child_cells
+                           if child_cell.name.split('$')[0] == "Waveguide Coplanar"]
 
         return segment_lengths
 
     @staticmethod
     def produce_fixed_length_waveguide(chip, route_function, initial_guess=0.0, length=0.0, **waveguide_params):
         """
         Produce a waveguide composite with fixed length. `route_function` should be a single-argument function that
@@ -427,50 +367,48 @@
     def build(self):
         """Produce the composite waveguide.
 
         In practice this becomes an alternating chain of WaveguideCoplanar and some other Element
         subclass. Elements are oriented collinear to the preceding Node and an automatic bend is
         inserted after if the next Node is not collinear.
         """
-
         self._nodes = Node.nodes_from_string(self.nodes)
         self._child_refpoints = {}
         if len(self._nodes) < 2:
             self.raise_error_on_cell("Need at least 2 Nodes for a WaveguideComposite.",
                                      self._nodes[0].position if len(self._nodes) == 1 else pya.DPoint())
 
         self._wg_start_idx = 0      # next waveguide starts here
         self._wg_start_pos = self._nodes[0].position
         self._wg_start_dir = self._node_entrance_direction(0)
 
-        self.old_id = self.face_ids[0]
-
         for i, node in enumerate(self._nodes):
             self.__log.debug(f' Node #{i}: ({node.position.x:.2f}, {node.position.y:.2f}), {node.element.__class__},'
                              f' {node.params}')
-            if 'face_id' in node.params:
-                self.new_id = node.params['face_id']
-            else:
-                self.new_id = self.old_id
-
-            if 'add_metal' in node.params:
-                self.add_metal = node.params['add_metal']
-
             if node.element is None:
-                if self.new_id != self.old_id:
-                    self._add_layer_changing_element(i)
-                elif 'a' in node.params or 'b' in node.params:
+                if 'a' in node.params or 'b' in node.params:
                     self._add_taper(i)
+                elif 'face_id' in node.params:
+                    self._add_fc_bump(i)
             else:
-                self.check_node_type(node, i)
+                if node.element is AirbridgeConnection:
+                    self._add_airbridge(i)
+                elif issubclass(node.element, Airbridge):
+                    if node.element is not Airbridge:   # change default if specific type is used
+                        self.airbridge_type = node.element.default_type
+                    self._add_airbridge(i, with_side_airbridges=False)
+                elif node.element is WaveguideCoplanarTaper:
+                    self._add_taper(i)
+                elif node.element is FlipChipConnectorRf:
+                    self._add_fc_bump(i)
+                else:
+                    self._add_simple_element(i)
 
                 self._terminator(i)
 
-            self.old_id = self.new_id
-
         # pylint: disable=undefined-loop-variable
         if node.element is None:
             self._add_waveguide(i)
 
         # Create airbridge on each node that has `ab_across=True` in params
         for i, node in enumerate(self._nodes):
             if "ab_across" in node.params and node.params["ab_across"]:
@@ -479,30 +417,14 @@
 
         # Reference points
         self.refpoints.update(self._child_refpoints)
         self.add_port("a", self._nodes[0].position, -self._node_entrance_direction(0))
         self.add_port("b", self._wg_start_pos, self._wg_start_dir)
 
 
-    def check_node_type(self, node, i):
-        """Iterate over supported Node types and run approriate function"""
-
-        if node.element is AirbridgeConnection:
-            self._add_airbridge(i)
-        elif issubclass(node.element, Airbridge):
-            if node.element is not Airbridge:  # change default if specific type is used
-                self.airbridge_type = node.element.default_type
-            self._add_airbridge(i, with_side_airbridges=False)
-        elif node.element is WaveguideCoplanarTaper:
-            self._add_taper(i)
-        elif node.element in [element_by_class_name(el) for el in node_editor_layer_changing_elements]:
-            self._add_layer_changing_element(i, node.element)
-        else:
-            self._add_simple_element(i)
-
     def _add_taper(self, ind):
         """Create a WaveguideCoplanarTaper and change default a/b."""
 
         node = self._nodes[ind]
 
         params = {**self.pcell_params_by_name(WaveguideCoplanarTaper), **node.params}
         a, b = params.pop('a', self.a), params.pop('b', self.b)
@@ -511,36 +433,31 @@
 
         taper_cell = self.add_element(WaveguideCoplanarTaper, **{**params, 'a2': a, 'b2': b, 'm2': self.margin})
         self._insert_cell_and_waveguide(ind, taper_cell)
 
         self.a = a
         self.b = b
 
-    def _add_layer_changing_element(self, ind, element=FlipChipConnectorRf):
-        """Add element which changes face_id and change default face_id."""
+    def _add_fc_bump(self, ind):
+        """Add FlipChipConnectorRF and change default face_id."""
         node = self._nodes[ind]
-        params = {**self.pcell_params_by_name(element), **node.params}
-
-        if self.new_id == self.old_id:  # no change, just a Node
+        if "face_id" not in node.params:
+            node.params["face_id"] = self.face_ids[1]
+        params = {**self.pcell_params_by_name(FlipChipConnectorRf), **node.params}
+        new_id = node.params.pop("face_id")
+        old_id = self.face_ids[0]
+        if new_id == old_id:  # no change, just a Node
             return
+        # TODO support vias?
 
-        params['face_ids'] = [self.old_id, self.new_id]
-
-        # Allow face changing elements to change waveguide widths
-        new_a, new_b = params.get('a', self.a), params.get('b', self.b)
-        if not (new_a == self.a and new_b == self.b):
-            params['a2'], params['b2'] = new_a, new_b
-            params['a'], params['b'] = self.a, self.b
-
-        fc_cell = self.add_element(element, **params)
-
-        self._insert_cell_and_waveguide(ind, fc_cell, before=f'{self.old_id}_port', after=f'{self.new_id}_port')
+        fc_cell = self.add_element(FlipChipConnectorRf, **params)
+        self._insert_cell_and_waveguide(ind, fc_cell, before=f'{old_id}_port', after=f'{new_id}_port')
 
-        self.a, self.b = new_a, new_b
-        self.face_ids = [self.new_id] + [a for a in self.face_ids if a != self.new_id]
+        self.face_ids[0] = new_id
+        self.face_ids[1] = old_id
 
     def _add_airbridge(self, ind, **kwargs):
         """Add an airbridge with tapers at both sides and change default a/b if required."""
 
         node = self._nodes[ind]
         params = {**self.pcell_params_by_name(AirbridgeConnection), **kwargs,
                   'a2': self.a, 'b2': self.b, 'm2': self.margin,
@@ -596,16 +513,15 @@
         # Compute transformation for the cell
         waveguide_dir = self._node_entrance_direction(ind)
         trans = pya.DCplxTrans(1, get_angle(waveguide_dir) - get_angle(element_dir), False, self._nodes[ind].position)
         if ind in (0, len(self._nodes) - 1):
             trans *= pya.DTrans(-rel_ref[before if ind == 0 else after])
 
         # Insert element cell with computed transformation
-        cell_inst, ref = self.insert_cell(cell, trans)
-        cell_inst.set_property("waveguide_composite_node_index", ind)
+        _, ref = self.insert_cell(cell, trans)
         if inst_name is not None:
             for name, value in ref.items():
                 self._child_refpoints[f'{inst_name}_{name}'] = value
 
         # Add waveguide from previous element until this element
         self._add_waveguide(ind, ref[before], waveguide_dir)
 
@@ -631,16 +547,15 @@
             return
         params = {**self.pcell_params_by_name(WaveguideCoplanar), "path": points}
         if start_index != 0 or self._nodes[start_index].element:
             params['term1'] = 0
         if end_index != len(self._nodes) - 1 or self._nodes[end_index].element:
             params['term2'] = 0
         wg_cell = self.add_element(WaveguideCoplanar, **params)
-        cell_inst, _ = self.insert_cell(wg_cell)
-        cell_inst.set_property("waveguide_composite_node_index", end_index)
+        self.insert_cell(wg_cell)
 
     def _add_waveguide(self, end_index, end_pos=None, end_dir=None):
         """Creates waveguide from `self._wg_start_idx` until `end_index`.
 
         Args:
             end_index: the last node index taken into account in the waveguide
             end_pos: endpoint position of the waveguide (optional, overwrites `self._nodes[end_index].position`)
@@ -753,18 +668,16 @@
                     if n1 - 1 == start_index:
                         meander_len -= start_len + (points[0] - turn_start).length()
                     elif self._nodes[n1-1].angle is None:
                         meander_len -= start_len / 2
                     else:
                         meander_len -= start_len + (self._nodes[n1-1].position - turn_start).length()
 
-                params = {**node1.params, "a": self.a, "b": self.b}
-                cell_inst, _ = self.insert_cell(Meander, start=[meander_start.x, meander_start.y],
-                                                end=[meander_end.x, meander_end.y], length=meander_len, **params)
-                cell_inst.set_property("waveguide_composite_node_index", end_index)
+                self.insert_cell(Meander, start=[meander_start.x, meander_start.y], end=[meander_end.x, meander_end.y],
+                                 length=meander_len, **node1.params)
                 wg_points = point0 + points[p0:p1] + ([] if start_len < 1e-4 else [meander_start])
                 self._insert_wg_cell(wg_points, n0, n1)
                 n0 = n1
                 p0 = p1
                 point0 = [] if end_len < 1e-4 else [meander_end]
             elif "n_bridges" in node1.params and node1.params["n_bridges"] > 0:
                 ab_len = node1.params['bridge_length'] if "bridge_length" in node1.params else None
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import math
 
 from kqcircuits.pya_resolver import pya
-from kqcircuits.util.parameters import Param, pdt, add_parameters_from
+from kqcircuits.util.parameters import Param, pdt
 
 from kqcircuits.elements.element import Element
 from kqcircuits.elements.waveguide_coplanar_straight import WaveguideCoplanarStraight
 from kqcircuits.elements.waveguide_coplanar_curved import WaveguideCoplanarCurved
 
 
-@add_parameters_from(WaveguideCoplanarStraight, "add_metal")
 class WaveguideCoplanar(Element):
     """The PCell declaration for an arbitrary coplanar waveguide.
 
     Coplanar waveguide defined by the width of the center conductor and gap. It can follow any segmented lines with
     predefined bending radios. It actually consists of straight and bent PCells. Termination lengths are lengths of
     extra ground gaps for opened transmission lines
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_curved.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_curved.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
 
 from math import pi, sin, cos
 
 from kqcircuits.elements.element import Element
 from kqcircuits.pya_resolver import pya
 from kqcircuits.util.geometry_helper import vector_length_and_direction
-from kqcircuits.util.parameters import Param, pdt, add_parameters_from
-from kqcircuits.elements.waveguide_coplanar_straight import WaveguideCoplanarStraight
+from kqcircuits.util.parameters import Param, pdt
 
 
 def arc(r, start, stop, n):
     """ Returns list of points of an arc
 
     Args:
         r: radius
@@ -44,15 +43,14 @@
     for i in range(n_steps):
         alpha = start + step * (i + 0.5)
         pts.append(pya.DPoint(r_corner * cos(alpha), r_corner * sin(alpha)))
     pts.append(pya.DPoint(r * cos(stop), r * sin(stop)))
     return pts
 
 
-@add_parameters_from(WaveguideCoplanarStraight, "add_metal")
 class WaveguideCoplanarCurved(Element):
     """The PCell declaration of a curved segment of a coplanar waveguide.
 
     Coordinate origin is left at the center of the arc.
     """
 
     alpha = Param(pdt.TypeDouble, "Curve angle (rad)", pi)
@@ -78,16 +76,14 @@
         # Protection layer
         pts = left_protection_arc + right_protection_arc
         self.add_protection(pya.DPolygon(pts))
         # Waveguide lenght
         pts = annotation_arc
         shape = pya.DPath(pts, self.a)
         self.cell.shapes(self.get_layer("waveguide_path")).insert(shape)
-        if self.add_metal:
-            self.cell.shapes(self.get_layer("base_metal_addition")).insert(shape)
 
     @staticmethod
     def create_curve_arcs(elem, angle):
         """Creates arcs of points for a curved waveguide.
 
         Args:
             elem: Element from which the waveguide parameters for the arc are taken
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_splitter.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_splitter.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_straight.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_straight.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 class WaveguideCoplanarStraight(Element):
     """The PCell declaration of a straight segment of a coplanar waveguide.
 
    .. MARKERS_FOR_PNG 15,8 15,0
     """
 
     l = Param(pdt.TypeDouble, "Length", 30)
-    add_metal = Param(pdt.TypeBoolean, "Add trace in base metal addition too", False)
 
     def build(self):
         # Refpoint in the first end
         # Left gap
         pts = [
             pya.DPoint(0, self.a / 2 + 0),
             pya.DPoint(self.l, self.a / 2 + 0),
@@ -62,9 +61,7 @@
         # Waveguide length
         pts = [
             pya.DPoint(0, 0),
             pya.DPoint(self.l, 0),
         ]
         shape = pya.DPath(pts, self.a)
         self.cell.shapes(self.get_layer("waveguide_path")).insert(shape)
-        if self.add_metal:
-            self.cell.shapes(self.get_layer("base_metal_addition")).insert(shape)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/elements/waveguide_coplanar_taper.py` & `kqcircuits-4.6.9rc1/kqcircuits/elements/waveguide_coplanar_taper.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,16 @@
 
 import math
 
 from kqcircuits.elements.element import Element
 from kqcircuits.pya_resolver import pya
 from kqcircuits.util.parameters import Param, pdt, add_parameters_from
 from kqcircuits.elements.finger_capacitor_square import FingerCapacitorSquare
-from kqcircuits.elements.waveguide_coplanar_straight import WaveguideCoplanarStraight
 
 
-@add_parameters_from(WaveguideCoplanarStraight, "add_metal")
 @add_parameters_from(FingerCapacitorSquare, a2=Element.a*2, b2=Element.b*2)
 class WaveguideCoplanarTaper(Element):
     """The PCell declaration of a taper segment of a coplanar waveguide.
 
     .. MARKERS_FOR_PNG 0,0,31.2,0 0,5,0,-5 31.2,-10,31.2,10
     """
 
@@ -69,20 +67,16 @@
             pya.DPoint(0, self.a / 2),
             pya.DPoint(self.taper_length, self.a2 / 2),
             pya.DPoint(self.taper_length, -self.a2 / 2),
             pya.DPoint(0, -self.a / 2)
         ]
         shape = pya.DPolygon(pts)
         self.cell.shapes(self.get_layer("waveguide_path")).insert(shape)
-        if self.add_metal:
-            self.cell.shapes(self.get_layer("base_metal_addition")).insert(shape)
         pts = [
             pya.DPoint(0, 0),
             pya.DPoint(self.taper_length, 0),
         ]
         shape = pya.DPath(pts, min(self.a, self.a2))
         self.cell.shapes(self.get_layer("waveguide_path")).insert(shape)
-        if self.add_metal:
-            self.cell.shapes(self.get_layer("base_metal_addition")).insert(shape)
         # refpoints for connecting to waveguides
         self.add_port("a", pya.DPoint(0, 0), pya.DVector(-1, 0))
         self.add_port("b", pya.DPoint(self.taper_length, 0), pya.DVector(1, 0))
```

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/junction.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/junction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/manhattan.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/manhattan_single_junction.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/manhattan_single_junction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/no_squid.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/no_squid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/junctions/squid.py` & `kqcircuits-4.6.9rc1/kqcircuits/junctions/squid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/klayout_view.py` & `kqcircuits-4.6.9rc1/kqcircuits/klayout_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 
         if filename is None:
             filename = cell.name
         if layers_set is None:
             layers_set = [resolve_default_layer_info(layer_name) for layer_name in mask_bitmap_export_layers]
 
         if len(layers_set) == 1:
-            layer_str = "-" + layers_set[0].name
+            layer_str = " " + layers_set[0].name
         else:
             layer_str = ""
         cell_png_name = path / "{}{}.png".format(filename, layer_str)
 
         def export_callback():
             self.layout_view.save_image(str(cell_png_name), pngsize[0], pngsize[1])
```

### Comparing `kqcircuits-4.6.21/kqcircuits/layer_cluster.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_cluster.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/layer_config/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/layer_config/default_layer_config.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 # Top face layers
 _face_layers['2b1'] = {
     **_shift_layers(_common_b_t_layers, 0, 1),    # common layers at the "top"
 }
 
 # Ceiling face layers
 _face_layers['2t1'] = {
-    **_shift_layers(_common_b_t_layers, 128, 1),     # same common layers at the "ceiling"
+    **_shift_layers(_common_layers, 128, 1),     # same common layers at the "ceiling"
 }
 
 # Other auxiliary layers [Layer 220-229]
 _aux_layers_dict = {
     "annotations": (220, 0),
     "annotations_2": (221, 0),
     "instance_names": (222, 0),
@@ -135,23 +135,23 @@
 # default_faces[face_id] contains the face dictionary for the face determined by face_id.
 #
 # Each face dictionary should contain:
 #   - key "id" with value face_id (string)
 #   - for all the available layers in that face: key "Layer_name", value pya.LayerInfo object for that layer
 #
 default_faces = {}
-for f in ('1t1', '2b1', '1b1', '2t1'):
+for f in ('1b1', '1t1', '2b1', '2t1'):
     default_faces[f] = {n: pya.LayerInfo(i[0], i[1], f'{f}_{n}') for n, i in _face_layers[f].items()}
 
 # pya layer information
 default_layers = {n: pya.LayerInfo(i[0], i[1], n) for n, i in _aux_layers_dict.items()}
 for face, layers in default_faces.items():
     default_layers.update({f'{face}_{name}': li for name, li in layers.items()})
 
-for f in ('1t1', '2b1', '1b1', '2t1'):
+for f in ('1b1', '1t1', '2b1', '2t1'):
     default_faces[f]['id'] = f
 
 default_face_id = "1t1"  # face_id of the face that is used by default in some contexts
 
 # Layer names (without face prefix) for layers exported as individual .oas files during mask layout export.
 default_mask_export_layers = [
     "base_metal_gap",
@@ -203,27 +203,27 @@
 ]
 
 # Layer clusters used for exporting only certain layers together in the same file, when exporting individual chips
 # during mask layout export.
 # Dictionary with items "cluster name: LayerCluster".
 chip_export_layer_clusters = {
     # 1b1-face
-    "SIS-1b1": LayerCluster(["1b1_SIS_junction", "1b1_SIS_shadow", "1b1_SIS_junction_2"],
+    "SIS 1b1": LayerCluster(["1b1_SIS_junction", "1b1_SIS_shadow", "1b1_SIS_junction_2"],
                             ["1b1_base_metal_gap_for_EBL"], "1b1"),
-    "airbridges-1b1": LayerCluster(["1b1_airbridge_pads", "1b1_airbridge_flyover"],
+    "airbridges 1b1": LayerCluster(["1b1_airbridge_pads", "1b1_airbridge_flyover"],
                                    ["1b1_base_metal_gap_wo_grid"], "1b1"),
     # 1t1-face
-    "SIS-1t1": LayerCluster(["1t1_SIS_junction", "1t1_SIS_shadow", "1t1_SIS_junction_2"],
+    "SIS 1t1": LayerCluster(["1t1_SIS_junction", "1t1_SIS_shadow", "1t1_SIS_junction_2"],
                             ["1t1_base_metal_gap_for_EBL"], "1t1"),
-    "airbridges-1t1": LayerCluster(["1t1_airbridge_pads", "1t1_airbridge_flyover"],
+    "airbridges 1t1": LayerCluster(["1t1_airbridge_pads", "1t1_airbridge_flyover"],
                                    ["1t1_base_metal_gap_wo_grid"], "1t1"),
     # 2b1-face
-    "SIS-2b1": LayerCluster(["2b1_SIS_junction", "2b1_SIS_shadow", "2b1_SIS_junction_2"],
+    "SIS 2b1": LayerCluster(["2b1_SIS_junction", "2b1_SIS_shadow", "2b1_SIS_junction_2"],
                             ["2b1_base_metal_gap_for_EBL"], "2b1"),
-    "airbridges-2b1": LayerCluster(["2b1_airbridge_pads", "2b1_airbridge_flyover"],
+    "airbridges 2b1": LayerCluster(["2b1_airbridge_pads", "2b1_airbridge_flyover"],
                                    ["2b1_base_metal_gap_wo_grid"], "2b1"),
 }
 
 # default layers to use for calculating cell path lengths with get_cell_path_length()
 default_path_length_layers = [
     "1b1_waveguide_path",
     "1t1_waveguide_path",
```

### Comparing `kqcircuits-4.6.21/kqcircuits/layer_config/default_layer_props.lyp` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_props.lyp`

 * *Files 8% similar despite different names*

#### Comparing `kqcircuits-4.6.21/kqcircuits/layer_config/default_layer_props.lyp` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/default_layer_props.lyp`

```diff
@@ -1015,235 +1015,14 @@
       <width>2</width>
       <marked>false</marked>
       <xfill>false</xfill>
       <animation>0</animation>
       <name/>
       <source>'2t1 ground grid avoidance' 133/2@1</source>
     </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 base metal gap for EBL' 134/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 waveguide path' 135/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 SIS junction' 136/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 SIS shadow' 137/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 SIS junction 2' 139/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 airbridge pads' 146/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 airbridge flyover' 147/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 chip dicing' 158/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 underbump metallization' 148/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 indium bump' 149/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 through silicon via' 150/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 through silicon via avoidance' 153/2@1</source>
-    </group-members>
-    <group-members>
-      <frame-color>#FFFFFF</frame-color>
-      <fill-color>#FF0000</fill-color>
-      <frame-brightness>0</frame-brightness>
-      <fill-brightness>0</fill-brightness>
-      <dither-pattern>I0</dither-pattern>
-      <line-style/>
-      <valid>true</valid>
-      <visible>true</visible>
-      <transparent>false</transparent>
-      <width>1</width>
-      <marked>false</marked>
-      <xfill>false</xfill>
-      <animation>0</animation>
-      <name/>
-      <source>'2t1 ports' 154/2@1</source>
-    </group-members>
   </properties>
   <properties>
     <frame-color/>
     <fill-color/>
     <frame-brightness>0</frame-brightness>
     <fill-brightness>0</fill-brightness>
     <dither-pattern/>
```

### Comparing `kqcircuits-4.6.21/kqcircuits/layer_config/example_layer_config.py` & `kqcircuits-4.6.9rc1/kqcircuits/layer_config/example_layer_config.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/masks/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/masks/mask_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/mask_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 """Functions for exporting mask sets."""
 import json
 import os
 import subprocess
 from importlib import import_module
-from math import pi
 
 from autologging import logged
 
 from kqcircuits.chips.chip import Chip
 from kqcircuits.defaults import mask_bitmap_export_layers, chip_export_layer_clusters, default_layers, \
     default_mask_parameters, default_drc_runset, DRC_PATH, STARTUPINFO
 from kqcircuits.elements.flip_chip_connectors.flip_chip_connector_dc import FlipChipConnectorDc
 from kqcircuits.klayout_view import resolve_default_layer_info
 from kqcircuits.pya_resolver import pya, klayout_executable_command
 from kqcircuits.util.area import get_area_and_density
 from kqcircuits.util.count_instances import count_instances_in_cell
-from kqcircuits.util.geometry_helper import circle_polygon
 from kqcircuits.util.geometry_json_encoder import GeometryJsonEncoder
 from kqcircuits.util.netlist_extraction import export_cell_netlist
+from kqcircuits.util.geometry_helper import circle_polygon
 
 
 @logged
 def export_mask_set(mask_set):
     """Exports the designs, bitmap and documentation for the mask_set."""
 
     export_bitmaps(mask_set)
@@ -50,39 +49,39 @@
 def export_designs(mask_set):
     """Exports .oas and .gds files of the mask_set."""
     # export mask layouts
     for mask_layout in mask_set.mask_layouts:
         export_masks_of_face(mask_set._mask_set_dir, mask_layout, mask_set)
 
 
-def export_chip(chip_cell, chip_name, chip_dir, layout, export_drc, alt_netlists=None):
+def export_chip(chip_cell, chip_name, chip_dir, layout, export_drc):
     """Exports a chip used in a maskset."""
 
     is_pcell = chip_cell.pcell_declaration() is not None
 
     # save data that is only available in pcell, not static cell
     if is_pcell:
         chip_class = type(chip_cell.pcell_declaration())
         chip_params = chip_cell.pcell_parameters_by_name()
 
     # export .oas file with pcells (requires exporting a cell one hierarchy level above chip pcell)
     dummy_cell = layout.create_cell(chip_name)
     dummy_cell.insert(pya.DCellInstArray(chip_cell.cell_index(), pya.DTrans()))
-    _export_cell(chip_dir / f"{chip_name}_with_pcells.oas", dummy_cell, "all")
+    _export_cell(chip_dir/f"{chip_name}_with_pcells.oas", dummy_cell, "all")
     dummy_cell.delete()
     static_cell = layout.cell(layout.convert_cell_to_static(chip_cell.cell_index()))
 
     # save the chip .oas file with all layers and only containing static cells
     save_opts = pya.SaveLayoutOptions()
     save_opts.format = "OASIS"
     save_opts.write_context_info = False  # to save all cells as static cells
-    static_cell.write(str(chip_dir / f"{chip_name}.oas"), save_opts)
+    static_cell.write(str(chip_dir/f"{chip_name}.oas"), save_opts)
 
     # export netlist
-    export_cell_netlist(static_cell, chip_dir / f"{chip_name}-netlist.json", chip_cell, alt_netlists)
+    export_cell_netlist(static_cell, chip_dir/f"{chip_name}-netlist.json", chip_cell)
     # calculate flip-chip bump count
     bump_count = count_instances_in_cell(chip_cell, FlipChipConnectorDc)
     # find layer areas and densities
     layer_areas_and_densities = {}
     for layer, area, density in zip(*get_area_and_density(static_cell)):
         if area != 0.0:
             layer_areas_and_densities[layer] = {"area": f"{area:.2f}", "density": f"{density * 100:.2f}"}
@@ -92,15 +91,15 @@
         "Chip class module": chip_class.__module__ if is_pcell else None,
         "Chip class name": chip_class.__name__ if is_pcell else None,
         "Chip parameters": chip_params if is_pcell else None,
         "Bump count": bump_count,
         "Layer areas and densities": layer_areas_and_densities
     }
 
-    with open(chip_dir / (chip_name + ".json"), "w") as f:
+    with open(chip_dir/(chip_name + ".json"), "w") as f:
         json.dump(chip_json, f, cls=GeometryJsonEncoder, sort_keys=True, indent=4)
 
     # export .gds files for EBL or laser writer
     for cluster_name, layer_cluster in chip_export_layer_clusters.items():
         # If the chip has no shapes in the main layers of the layer cluster, should not export the chip with
         # that layer cluster.
         export_layer_cluster = False
@@ -113,15 +112,15 @@
             # To transform the exported layer cluster chip correctly (e.g. mirroring for top chip),
             # an instance of the cell is inserted to a temporary cell with the correct transformation.
             # Was not able to get this working by just using static_cell.transform_into().
             temporary_cell = layout.create_cell(chip_name)
             temporary_cell.insert(pya.DCellInstArray(static_cell.cell_index(), default_mask_parameters[
                 layer_cluster.face_id]["chip_trans"]))
             layers_to_export = {name: layout.layer(default_layers[name]) for name in layer_cluster.all_layers()}
-            path = chip_dir / f"{chip_name}-{cluster_name}.gds"
+            path = chip_dir / "{} {}.gds".format(chip_name, cluster_name)
             _export_cell(path, temporary_cell, layers_to_export)
             temporary_cell.delete()
 
     # export drc report for the chip
     if export_drc:
         export_drc_report(chip_name, chip_dir)
 
@@ -143,31 +142,14 @@
     # export .oas file with all layers
     path = export_dir_for_face / f"{_get_mask_layout_full_name(mask_set, mask_layout)}.oas"
     _export_cell(path, mask_layout.top_cell, "all")
     # export .oas files for individual optical lithography layers
     for layer_name in mask_layout.mask_export_layers:
         export_mask(export_dir_for_face, layer_name, mask_layout, mask_set)
 
-    # Find area and density for the layers defined in mask_layout.mask_export_density_layers
-    layer_infos = [resolve_default_layer_info(layer_name, mask_layout.face_id)
-                   for layer_name in mask_layout.mask_export_density_layers]
-    area_data = get_area_and_density(mask_layout.top_cell, layer_infos)
-
-    wafer_area = pi * mask_layout.wafer_rad ** 2  # Use circular wafer area instead of rectangular bounding boxes
-    layer_areas_and_densities = {name: {
-        "area": round(area, 2),
-        "density": round(area / wafer_area * 100, 2)
-    } for name, area, _ in zip(*area_data)}
-
-    mask_json = {
-        "layer_areas_and_densities": layer_areas_and_densities,
-    }
-    with open(export_dir_for_face / (subdir_name_for_face + ".json"), "w") as f:
-        json.dump(mask_json, f, cls=GeometryJsonEncoder, sort_keys=True, indent=4)
-
 
 def export_mask(export_dir, layer_name, mask_layout, mask_set):
     """ Exports a mask from a single layer of a single face of a mask set.
 
     Args:
         export_dir: directory for the files
         layer_name: name of the layer exported as a mask, if starts with '-' then it will be inverted
@@ -189,37 +171,36 @@
         wafer = pya.Region(top_cell.begin_shapes_rec(layer)).merged()
         disc = pya.Region([circle_polygon(mask_layout.wafer_rad).to_itype(layout.dbu)])
         layout.copy_layer(layer, tmp_layer)
         layout.clear_layer(layer)
         top_cell.shapes(layer).insert(wafer ^ disc)
 
     layers_to_export = {layer_info.name: layer}
-    path = export_dir / (_get_mask_layout_full_name(mask_set, mask_layout) + f"-{layer_info.name}.oas")
+    path = export_dir / (_get_mask_layout_full_name(mask_set, mask_layout) + f" {layer_info.name}.oas")
     _export_cell(path, top_cell, layers_to_export)
 
     if invert:
         layout.clear_layer(layer)
         layout.copy_layer(tmp_layer, layer)
     layout.delete_layer(tmp_layer)
 
-
 @logged
 def export_docs(mask_set, filename="Mask_Documentation.md"):
     """Exports mask documentation containing mask layouts and parameters of all chips in the mask_set."""
-    file_location = str(mask_set._mask_set_dir / filename)
+    file_location = str(mask_set._mask_set_dir/filename)
 
     with open(file_location, "w+", encoding="utf-8") as f:
         f.write("# Mask Set Name: {}\n".format(mask_set.name))
         f.write("Version: {}\n".format(mask_set.version))
 
         for mask_layout in mask_set.mask_layouts:
 
             f.write("## Mask Layout {}:\n".format(mask_layout.face_id + mask_layout.extra_id))
-            mask_layout_str = _get_mask_layout_full_name(mask_set, mask_layout)
-            f.write(f"![alt text]({mask_layout_str}/{mask_layout_str}-mask_graphical_rep.png)\n")
+            mask_layout_str = _get_mask_layout_full_name(mask_set, mask_layout).replace(" ", "%20")
+            f.write(f"![alt text]({mask_layout_str}/{mask_layout_str}%20mask_graphical_rep.png)\n")
 
             f.write("### Number of Chips in Mask Layout {}\n".format(mask_layout.face_id + mask_layout.extra_id))
 
             chip_counts = {}
 
             def count_chips(mlayout, counts):
 
@@ -271,16 +252,16 @@
                 cls = getattr(import_module(cls_mod), cls_name)
                 # get defaults and update ones with input
                 params = cls().pcell_params_by_name()
                 params.update(params_input)
                 params_schema = cls.get_schema()
                 for param_name, param_declaration in params_schema.items():
                     f.write("| **{}** | {} |\n".format(
-                        param_declaration.description.replace("|", "&#124;"),
-                        str(params[param_name])))
+                            param_declaration.description.replace("|", "&#124;"),
+                            str(params[param_name])))
             f.write("\n")
 
             f.write("### Other Chip Information\n")
             f.write("| | |\n")
             f.write("| :--- | :--- |\n")
 
             # launcher assignments
@@ -311,45 +292,49 @@
         for mask_layout in mask_set.mask_layouts:
             mask_layout_str = _get_mask_layout_full_name(mask_set, mask_layout)
             mask_layout_path = mask_set._mask_set_dir / mask_layout_str
 
             f.write("### Mask Files:\n")
             for file_name in os.listdir(mask_layout_path):
                 if file_name.endswith(".oas"):
-                    f.write(" + [{}]({})\n".format(file_name, os.path.join(mask_layout_str, file_name)))
+                    # the spaces are replaced by "%20" to make links to filenames with spaces work
+                    f.write(" + [{}]({})\n".format(file_name,
+                                                   os.path.join(mask_layout_str, file_name).replace(" ", "%20")))
             f.write("\n")
 
             f.write("### Mask Images:\n")
             for file_name in os.listdir(mask_layout_path):
                 if file_name.endswith(".png"):
-                    f.write("+ [{}]({})\n".format(file_name, os.path.join(mask_layout_str, file_name)))
+                    # the spaces are replaced by "%20" to make links to filenames with spaces work
+                    f.write("+ [{}]({})\n".format(file_name,
+                                                  os.path.join(mask_layout_str, file_name).replace(" ", "%20")))
 
         f.close()
 
 
 @logged
 def export_bitmaps(mask_set, spec_layers=mask_bitmap_export_layers):
     """Exports bitmaps for the mask_set."""
     # pylint: disable=dangerous-default-value
 
     # export bitmaps for mask layouts
     for mask_layout in mask_set.mask_layouts:
         mask_layout_dir_name = _get_mask_layout_full_name(mask_set, mask_layout)
-        mask_layout_dir = _get_directory(mask_set._mask_set_dir / str(mask_layout_dir_name))
+        mask_layout_dir = _get_directory(mask_set._mask_set_dir/str(mask_layout_dir_name))
         filename = _get_mask_layout_full_name(mask_set, mask_layout)
         view = mask_set.view
         if view:
             view.focus(mask_layout.top_cell)
             view.export_all_layers_bitmap(mask_layout_dir, mask_layout.top_cell, filename=filename)
             view.export_layers_bitmaps(mask_layout_dir, mask_layout.top_cell, filename=filename,
                                        layers_set=spec_layers, face_id=mask_layout.face_id)
     # export bitmaps for chips
-    chips_dir = _get_directory(mask_set._mask_set_dir / "Chips")
+    chips_dir = _get_directory(mask_set._mask_set_dir/"Chips")
     for name, cell in mask_set.used_chips.items():
-        chip_dir = _get_directory(chips_dir / name)
+        chip_dir = _get_directory(chips_dir/name)
         if view:
             view.export_all_layers_bitmap(chip_dir, cell, filename=name)
     if view:
         view.focus(mask_set.mask_layouts[0].top_cell)
 
 
 @logged
@@ -402,8 +387,8 @@
 def _get_directory(directory):
     if not os.path.exists(str(directory)):
         os.mkdir(str(directory))
     return directory
 
 
 def _get_mask_layout_full_name(mask_set, mask_layout):
-    return f"{mask_set.name}_v{mask_set.version}-{mask_layout.face_id}{mask_layout.extra_id}"
+    return f"{mask_set.name}_v{mask_set.version} {mask_layout.face_id}{mask_layout.extra_id}"
```

### Comparing `kqcircuits-4.6.21/kqcircuits/masks/mask_layout.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/mask_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,24 +47,22 @@
         wafer_center: Wafer center as a pya.DVector
         chips_map_offset: Offset to make chips_map centered on wafer
         wafer_top_flat_length: length of flat edge at the top of the wafer
         wafer_bottom_flat_length: length of flat edge at the bottom of the wafer
         dice_width: Dicing width for this mask layout
         text_margin: Text margin for this mask layout
         chip_size: side width of the chips (assuming square chips)
-        edge_clearance: minimum clearance of outer chips from the edge of the mask
+        edge_clearance: minimum clearance of outer chips from the edge of the mask, measured from the chip center
         chip_box_offset: Offset (pya.DVector) from chip origin of the chip frame boxes for this face
         chip_trans: DTrans applied to all chips
         mask_name_offset: mask name label offset from default position (DPoint)
         mask_name_scale: text scaling factor for mask name label (float)
         mask_text_scale: text scaling factor for graphical representation layer (float)
         mask_marker_offset: offset of mask markers from wafer center in horizontal and vertical directions (float)
         mask_export_layers: list of layer names (without face_ids) to be exported as individual mask `.oas` files
-        mask_export_density_layers: list of layer names (without face_ids) for which we want to calculate the coverage
-         density
         submasks: list of submasks, each element is a tuple (submask mask_layout, submask position)
         extra_id: extra string used to create unique name for mask layouts with the same face_id
         extra_chips: List of tuples (name, position, trans) for chips placed outside chips_map, trans is an optional
             transformation to use in place of self.chip_trans
         top_cell: Top cell of this mask layout
         added_chips: List of (chip name, chip position, chip bounding box, chip dtrans) populated by chips added during
             build()
@@ -78,36 +76,35 @@
         self.with_grid = with_grid
         self.face_id = face_id
         self.chips_map = chips_map
         self.chips_map_legend = None
 
         self.layers_to_mask = kwargs.get("layers_to_mask", default_layers_to_mask)
         self.covered_region_excluded_layers = kwargs.get("covered_region_excluded_layers",
-                                                        default_covered_region_excluded_layers) + ["mask_edge"]
+                                                        default_covered_region_excluded_layers)
         self.wafer_rad = kwargs.get("wafer_rad", default_mask_parameters[self.face_id]["wafer_rad"])
         self.wafer_center = (pya.DVector(0, 0))
         self.chips_map_offset = kwargs.get("chips_map_offset",
                                               default_mask_parameters[self.face_id]["chips_map_offset"])
         self.wafer_top_flat_length = kwargs.get("wafer_top_flat_length", 0)
         self.wafer_bottom_flat_length = kwargs.get("wafer_bottom_flat_length", 0)
         self.dice_width = kwargs.get("dice_width", default_mask_parameters[self.face_id]["dice_width"])
         self.text_margin = kwargs.get("text_margin", default_mask_parameters[self.face_id]["text_margin"])
         self.chip_size = kwargs.get("chip_size", default_mask_parameters[self.face_id]["chip_size"])
-        self.edge_clearance = kwargs.get("edge_clearance", self.chip_size / 2)
+        self.edge_clearance = kwargs.get("edge_clearance", self.chip_size)
         self.chip_box_offset = kwargs.get("chip_box_offset", default_mask_parameters[self.face_id]["chip_box_offset"])
         self.chip_trans = kwargs.get("chip_trans", default_mask_parameters[self.face_id]["chip_trans"])
         self.mask_name_offset = kwargs.get("mask_name_offset", default_mask_parameters[self.face_id][
             "mask_name_offset"])
         self.mask_name_scale = kwargs.get("mask_name_scale", 1)
         self.mask_text_scale = kwargs.get("mask_text_scale", default_mask_parameters[self.face_id]["mask_text_scale"])
         self.mask_markers_type = kwargs.get("mask_markers_type", "all")
         self.mask_marker_offset = kwargs.get("mask_marker_offset", default_mask_parameters[self.face_id][
             "mask_marker_offset"])
         self.mask_export_layers = kwargs.get("mask_export_layers", default_mask_export_layers)
-        self.mask_export_density_layers = kwargs.get("mask_export_density_layers", [])
         self.submasks = kwargs.get("submasks", [])
         self.extra_id = kwargs.get("extra_id", "")
         self.extra_chips = kwargs.get("extra_chips", [])
 
         self.top_cell = self.layout.create_cell(f"{self.name} {self.face_id}")
         self.added_chips = []
 
@@ -151,41 +148,37 @@
                                     print("error occurs at %s at %s" % (name, face_id))
 
                             for shapes_to_remove in shapes:
                                 shapes_to_remove.delete()
 
                 self.chips_map_legend[name] = new_cell
 
+        step_ver = pya.DVector(0, -self.chip_size)
+        step_hor = pya.DVector(self.chip_size, 0)
+
         region_covered = self._mask_create_geometry()
         if len(self.submasks) > 0:
             region_covered = pya.Region()  # don't fill with metal gap layer if using submasks
             for submask_layout, submask_pos in self.submasks:
                 self.top_cell.insert(
                     pya.DCellInstArray(submask_layout.top_cell.cell_index(),
                                        pya.DTrans(submask_pos - submask_layout.wafer_center + self.wafer_center))
                 )
 
         # add chips from chips_map
         for (i, row) in enumerate(tqdm(self.chips_map, desc='Adding chips to mask', bar_format=default_bar_format)):
             for (j, chip_name) in enumerate(row):
-                if chip_name == "---":
-                    continue
-                position = pya.DPoint(self.chip_size * j, -self.chip_size * (i + 1)) - self.chips_map_offset + \
-                           pya.DVector(-self.wafer_rad, self.wafer_rad)
-                pos = position - self.wafer_center
-                test_x = self.chip_size if pos.x + self.chip_size / 2 > 0 else 0
-                test_y = self.chip_size if pos.y + self.chip_size / 2 > 0 else 0
-                d_edge = self.wafer_rad - (pos + pya.DVector(test_x, test_y)).abs()
-                if  d_edge > self.edge_clearance:
+                position = pya.DPoint(step_ver * (i + 1) + step_hor * j) - self.chips_map_offset \
+                           + pya.DVector(-self.wafer_rad, self.wafer_rad)
+                if (position - step_ver*0.5 + step_hor*0.5 - self.wafer_center).abs() - self.wafer_rad < \
+                        -self.edge_clearance:
                     added_chip, region_chip = self._add_chip(chip_name, position, self.chip_trans)
-                    region_covered -= region_chip
                 else:
-                    print(f" Warning, dropping chip {chip_name} at ({i}, {j}), '{self.face_id}' - too close to edge:"
-                          f" {d_edge:.2f} < {self.edge_clearance}")
-                    added_chip = False
+                    added_chip, region_chip = False, pya.Region()
+                region_covered -= region_chip
                 if not added_chip:
                     self.chips_map[i][j] = "---"
 
         # add chips outside chips_map
         for name, pos, *trans in self.extra_chips:  # trans is optional
             if name in chips_map_legend:
                 region_covered -= self._add_chip(name, pos, trans[0] if trans else self.chip_trans)[1]
```

### Comparing `kqcircuits-4.6.21/kqcircuits/masks/mask_set.py` & `kqcircuits-4.6.9rc1/kqcircuits/masks/mask_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,51 +13,46 @@
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 import copy
 import os
-import logging
-from sys import argv
+import subprocess
 from time import perf_counter
+from string import Template
 from inspect import isclass
-from multiprocessing import Pool
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
 
 from autologging import logged
 from tqdm import tqdm
 
-from kqcircuits.util.log_router import route_log
-from kqcircuits.pya_resolver import pya, is_standalone_session
-from kqcircuits.defaults import default_bar_format, TMP_PATH, default_face_id
+from kqcircuits.pya_resolver import pya, is_standalone_session, klayout_executable_command
+from kqcircuits.defaults import default_bar_format, TMP_PATH, STARTUPINFO, default_face_id
 from kqcircuits.masks.mask_export import export_chip, export_mask_set
 from kqcircuits.masks.mask_layout import MaskLayout
 from kqcircuits.klayout_view import KLayoutView
 
 
 @logged
 class MaskSet:
     """Class representing a set of masks for different chip faces.
 
     A mask set consists of one or more MaskLayouts, each of which is for a certain face.
 
     To create a mask, add mask layouts to the mask set using add_mask_layout() and add chips to these mask layouts using
-    add_chip(). These functions also export some files for each chip. Then call build() to create the
+    add_chips() or add_chip(). These functions also export some files for each chip. Then call build() to create the
     cell hierarchy of the entire mask, and finally export mask files by calling export().
 
-    Chips are created in parallel in separate processes but the user may choose to use a ``-d`` switch on
-    the command line for debugging with a single process. It is also possible to manually limit the number of
-    concurrently used CPUs for resource management purposes with the ``-c 4`` switch (to 4 in this example).
-
     Example:
         mask = MaskSet(...)
         mask.add_mask_layout(...)
         mask.add_mask_layout(...)
-        mask.add_chip(...)
+        mask.add_chips(...)
         mask.build()
         mask.export()
 
     Attributes:
         layout: pya.Layout of this mask set
         name: Name of the mask set
         version: Version of the mask set
@@ -83,27 +78,20 @@
         self.version = version
         self.with_grid = with_grid
         self.export_drc = export_drc
         self.chips_map_legend = {}
         self.mask_layouts = []
         self.mask_export_layers = mask_export_layers if mask_export_layers is not None else []
         self.used_chips = {}
-        self._extra_params = {}
+        self.template_imports = []
+        self._thread_create_chip_parameters = {}
         self._mask_set_dir = Path(export_path)/f"{name}_v{version}"
 
         self._mask_set_dir.mkdir(parents=True, exist_ok=True)
 
-        self._extra_params["enable_debug"] = '-d' in argv
-        self._single_process = self._extra_params["enable_debug"] or not is_standalone_session()
-
-        self._cpu_override = 0
-        if '-c' in argv and len(argv) > argv.index('-c') + 1:
-            self._cpu_override = int(argv[argv.index('-c') + 1])
-
-
     def add_mask_layout(self, chips_map, face_id=default_face_id, mask_layout_type=MaskLayout, **kwargs):
         """Creates a mask layout from chips_map and adds it to self.mask_layouts.
 
         Args:
             chips_map: List of lists (2D-array) of strings, each string is a chip name (or --- for no chip)
             face_id: face_id of the mask layout
             mask_layout_type: type of the mask layout (MaskLayout or a child class of it)
@@ -116,101 +104,197 @@
             kwargs["mask_export_layers"] = self.mask_export_layers
 
         mask_layout = mask_layout_type(self.layout, self.name, self.version, self.with_grid, chips_map, face_id,
                                        **kwargs)
         self.mask_layouts.append(mask_layout)
         return mask_layout
 
-    def add_chip(self, chips, variant_name=None, cpus=None, **parameters):
-        """Adds a chip (or list of chips) with parameters to self.chips_map_legend and exports the files for each chip.
+    def load_cell_from_file(self, file_name):
+        """Load GDS or OASIS cell from file.
 
-        Note the complex polymorphism used here: ``chips`` is either a single chip class or a list of ``(chip, variant,
-        parameters)`` tuples. In the latter case the rest of the arguments (except ``cpus``) are ignored. Also,
-        ``chips`` (or the individual chip part of tuples) may be a simple file name to load a static .oas file instead.
+        Load a cell (usually a chip) from the specified file.
+
+        Args:
+            file_name: name of the file (with path) to be loaded
+
+        Returns:
+            the loaded cell
+        """
+        load_opts = pya.LoadLayoutOptions()
+        if hasattr(pya.LoadLayoutOptions, "CellConflictResolution"):
+            load_opts.cell_conflict_resolution = pya.LoadLayoutOptions.CellConflictResolution.RenameCell
+        self.layout.read(file_name, load_opts)
+        return self.layout.top_cells()[-1]
 
-        The chip's parameters dictionary may also contain an ``alt_netlists`` dictionary to specify alternative ways of
-        generating netlists. See ``export_cell_netlist()`` or the ``quick_demo.py`` mask for further information.
+    def add_chips(self, chips, threads=None):
+        """Adds a list of chips with parameters to self.chips_map_legend and exports the files for each chip.
 
         Args:
-            chip: A chip class. Or a list of tuples, like ``[(QualityFactor, "QDG", parameters),...]``,
-                  parameters are optional.
-            variant_name: Name for specific variant, the same as in the mask layout.
-            cpus: Number of parallel processes to use for chip generation. By default uses ``os.cpu_count()``
-                  or the number of chips, whichever is smaller.
-            **parameters: Any parameters passed to the a single chip PCell.
+            chips: List of tuples that ``add_chip`` uses. Parameters are optional.
+                For example, ``(QualityFactor, "QDG", parameters)``.
+            threads: Number of parallel threads to use for generation. By default uses ``os.cpu_count()`` threads.
+                Uses subprocesses and consequently a lot of memory. In standalone python mode always uses 1 thread.
+
+        Warning:
+            It is advised to lower the thread number if your system has a lot of CPU cores but not a lot of memory.
+            The same applies for exporting large and complex geometry.
         """
         self._time['ADD_CHIPS'] = perf_counter()
 
-        if not isinstance(chips, list):  # only one chip
-            cpus = 1
-            chips = [(chips, variant_name, parameters)]
-
-        if cpus is None:
-            cpus = min(len(chips), os.cpu_count())
-        if self._cpu_override > 0:
-            cpus = self._cpu_override
-
-        # Pool.map() needs all arguments packed into a single list
-        xargs = (self.name, self.with_grid, self._mask_set_dir, self.export_drc, self._extra_params)
-        chip_args = ((chip, xargs) for chip in chips)
-
-        file_names = []
-        if cpus == 1 or self._single_process:
-            file_names += map(self._create_chip, chip_args)
+        if threads is None:
+            threads = os.cpu_count()
+        if threads is None or threads < 1 or is_standalone_session():
+            threads = 1
+
+        if threads == 1:
+            for chip_class, variant_name, *params in tqdm(chips, desc='Building variants',
+                                                          bar_format=default_bar_format):
+                self.add_chip(chip_class, variant_name, **(params[0] if params else {}))
         else:
-            print(f"Building chip variants in parallel using {cpus} processes...")
-            with Pool(cpus) as pool:
-                file_names += pool.map(self._create_chip, chip_args)
-
-        # import chip cells exported by the parallel processes into the mask
-        for variant, file_name in tqdm(file_names, desc='Add chips into mask', bar_format=default_bar_format):
-            self._load_chip_into_mask(file_name, variant)
+            print(f"Building chip variants in parallel using {threads} threads...")
 
-    @staticmethod
-    def _create_chip(chip_arg):
-        """Create chip, possibly in a separate process."""
+            template = self._get_template()
 
-        chip, xargs = chip_arg
-        name, with_grid, _mask_set_dir, export_drc, _extra_params = xargs
-        chip_class, variant_name, *chip_params = chip
-        chip_params = chip_params[0] if chip_params else {}
-        alt_netlists = chip_params.pop("alt_netlists", None)
+            class ChipSubprocessException(Exception):
+                def __init__(self, err, chip_variant):
+                    super().__init__()
+                    self.err = err
+                    self.chip_variant = chip_variant
+                def __str__(self):
+                    return f'Building the {self.chip_variant} chip variant caused the following error:'\
+                    f'{os.linesep}{self.err}'
+
+            def _subprocess_worker(args):
+                with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                                      startupinfo=STARTUPINFO) as proc:
+                    _, errs = proc.communicate()
+                    # Process has error return code, return error stream
+                    if proc.returncode > 0:
+                        return errs.decode('UTF-8')
+                return None
+
+            def _params_to_str(params):  # flatten a parameters dictionary to a string
+                ps = ""
+                for n, v in params.items():
+                    if isinstance(v, str):
+                        ps += f",{n}={repr(v)}"
+                    elif isinstance(v, pya.DBox):
+                        ps += f",{n}=pya.DBox({v.p1.x}, {v.p1.y}, {v.p2.x}, {v.p2.y})"
+                    elif isinstance(v, pya.DVector):
+                        ps += f",{n}=pya.DVector({v.x}, {v.y})"
+                    elif isinstance(v, pya.DPoint):
+                        ps += f",{n}=pya.DPoint({v.x}, {v.y})"
+                    else:
+                        ps += f",{n}={v}"
+                return ps
+
+            tp = ThreadPool(threads)
+            file_names = []
+            processes = {}
+            for chip_class, variant_name, *param_list in chips:
+                # create the script for generating this chip with the correct parameters and exporting the chip files
+                params = {
+                    'name_chip': variant_name,
+                    'name_mask': self.name,
+                    'with_grid': self.with_grid,
+                    'merge_base_metal_gap': True,
+                    }
+                if param_list:
+                    params.update(param_list[0])
+
+                element_import = f'from {chip_class.__module__} import {chip_class.__name__}'
+                create_element = f'cell = {chip_class.__name__}.create(layout {_params_to_str(params)})'
+                chip_path = self._mask_set_dir/"Chips"/f"{variant_name}"
+                chip_path.mkdir(parents=True, exist_ok=True)
+                script_name = str(chip_path / f"{variant_name}.py")
+                file_names.append((variant_name, str(chip_path / f"{variant_name}.oas"), script_name))
+
+                substitution_parameters = {
+                    'name_mask': self.name,
+                    'chip_path': str(chip_path),
+                    'variant_name': variant_name,
+                    'chip_class': chip_class.__name__,
+                    'element_import': element_import,
+                    'create_element': create_element,
+                    'export_drc': self.export_drc
+                }
+                substitution_parameters.update(self._thread_create_chip_parameters)
+                result = template.substitute(**substitution_parameters)
+                with open(script_name, "w") as f:
+                    f.write(result)
+
+                # launch klayout process that runs the created script
+                try:  # pylint: disable=consider-using-with
+                    processes[variant_name] = tp.apply_async(_subprocess_worker,
+                                   ([klayout_executable_command(), "-e", "-z", "-nc", "-rm", script_name],)
+                                   )
+                except subprocess.CalledProcessError as e:
+                    self.__log.error(e.output)
+
+            # wait for processes to end
+            tp.close()
+            for variant_name, process in processes.items():
+                process_error = process.get()
+                if process_error is not None:
+                    raise ChipSubprocessException(process_error, variant_name)
+            tp.join()
+
+            # import chip cells exported by the parallel processes into the mask
+            for variant_name, file_name, script_name in tqdm(file_names, desc='Building variants (parallel)',
+                                                             bar_format=default_bar_format):
+                self._load_chip_into_mask(file_name, variant_name)
+                # remove the script that was used to generate the chip
+                if os.path.exists(script_name):
+                    os.remove(script_name)
 
-        chip_path = _mask_set_dir/"Chips"/f"{variant_name}"
+    def add_chip(self, chip, variant_name, **kwargs):
+        """Adds a chip with the given name and parameters to self.chips_map_legend and exports chip files.
+
+        Args:
+            chip: the chip type class (for PCell chip), or a chip cell (for manually designed chip)
+            variant_name: name for specific variant, the same as in the mask layout
+            **kwargs: any parameters passed to the chip PCell
+        """
+
+        chip_path = self._mask_set_dir/"Chips"/f"{variant_name}"
         chip_path.mkdir(parents=True, exist_ok=True)
 
-        logging.basicConfig(level=logging.DEBUG)  # this level is NOT actually used
-        route_log(filename=chip_path/f"{variant_name}.log", stdout=_extra_params["enable_debug"])
+        if isclass(chip):
+            cell = self.variant_definition(chip, variant_name, **kwargs)[variant_name]
+            export_chip(cell, variant_name, chip_path, self.layout, self.export_drc)
+            self.layout.delete_cell_rec(cell.cell_index())
+        else:
+            export_chip(chip, variant_name, chip_path, self.layout, self.export_drc)
 
-        view = KLayoutView()
-        layout = view.layout
+        self._load_chip_into_mask(str(chip_path / f"{variant_name}.oas"), variant_name)
 
-        if isclass(chip_class):
-            params = {
-                'name_chip': variant_name,
-                'name_mask': name,
-                'with_grid': with_grid,
-                'merge_base_metal_gap': True,
-                'display_name': variant_name,
-                'name_copy': None,
-            }
-            if chip_params:
-                params.update(chip_params)
-            cell = chip_class.create(layout, **params)
-        else:  # its a file name, load it
-            load_opts = pya.LoadLayoutOptions()
-            if hasattr(pya.LoadLayoutOptions, "CellConflictResolution"):
-                load_opts.cell_conflict_resolution = pya.LoadLayoutOptions.CellConflictResolution.RenameCell
-            layout.read(chip_class, load_opts)
-            cell = layout.top_cells()[-1]
+    def variant_definition(self, chip_class, variant_name, **kwargs):
+        """Returns chip variant definition with default mask specific parameters.
 
-        export_chip(cell, variant_name, chip_path, layout, export_drc, alt_netlists)
-        view.close()
+        Args:
+            chip_class: the chip type class
+            variant_name: name for specific variant, the same as in the mask layout
+            **kwargs: any parameters passed to the chip PCell
 
-        return variant_name, str(chip_path / f"{variant_name}.oas")
+        Returns:
+            dictionary compatible with mask map structure
+        """
+        self.__log.info("Resolving %s", variant_name)
+
+        chip_parameters = {
+            "merge_base_metal_gap": True,
+            "name_chip": variant_name,
+            "display_name": variant_name,
+            "name_mask": self.name,
+            "name_copy": None,
+            "with_grid": self.with_grid,
+            **kwargs
+        }
+
+        return {variant_name: chip_class.create(self.layout, **chip_parameters)}
 
     def build(self, remove_guiding_shapes=True):
         """Builds the mask set.
 
         Creates cells for the mask based on self.mask_layouts and self.chips_map_legend. Optionally removes
         guiding shapes from the layout. Populates self.used_chips with the chips used in the mask layouts.
 
@@ -332,7 +416,60 @@
 
     def _load_chip_into_mask(self, file_name, variant_name):
         """Loads a chip from file_name to self.layout and adds it into self.chips_map_legend["variant_name"]"""
         load_opts = pya.LoadLayoutOptions()
         load_opts.cell_conflict_resolution = pya.LoadLayoutOptions.CellConflictResolution.RenameCell
         self.layout.read(file_name, load_opts)
         self.chips_map_legend.update({variant_name: self.layout.top_cells()[-1]})
+
+    def _get_template(self):
+        """Returns an updated template string."""
+
+        temp = _CREATE_CHIP_TEMPLATE
+        for i in self.template_imports:
+            temp = temp.replace('#TEMPLATE_IMPORT#', i, 1)
+        return Template(temp)
+
+
+# Template for creating and exporting a chip during mask generation.
+#
+# This is used in _get_template() to create a template used in add_chips() to create chips in
+# parallel. The "#TEMPLATE_IMPORT#" strings in it will be replaced by "template_imports" elements
+# to update the template itself.
+
+_CREATE_CHIP_TEMPLATE = """
+
+import logging
+import sys
+import traceback
+#TEMPLATE_IMPORT#
+from pathlib import Path
+from kqcircuits.masks.mask_export import export_chip
+from kqcircuits.pya_resolver import pya
+from kqcircuits.klayout_view import KLayoutView
+from kqcircuits.util.log_router import route_log
+${element_import}
+
+try:
+    logging.basicConfig(level=logging.DEBUG)  # this level is NOT actually used
+    chip_path = Path(r"${chip_path}")
+    route_log(filename=chip_path/"${variant_name}.log")
+
+    view = KLayoutView()
+    layout, top_cell = view.layout, view.top_cell
+
+    # cell definition and arbitrary code here
+    ${create_element}
+
+    top_cell.insert(pya.DCellInstArray(cell.cell_index(), pya.DTrans()))
+
+    # export chip files
+    export_chip(cell, "${variant_name}", chip_path, layout, ${export_drc})
+
+#TEMPLATE_IMPORT#
+
+except Exception as err:
+    print(traceback.format_exc(), file=sys.stderr)
+    pya.Application.instance().exit(1)
+pya.Application.instance().exit(0)
+
+"""
```

### Comparing `kqcircuits-4.6.21/kqcircuits/pya_resolver.py` & `kqcircuits-4.6.9rc1/kqcircuits/pya_resolver.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/qubits/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/qubits/double_pads.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,86 +16,81 @@
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import math
 
 from kqcircuits.elements.element import Element
 from kqcircuits.junctions.squid import Squid
-from kqcircuits.junctions.manhattan import Manhattan
 from kqcircuits.util.parameters import Param, pdt, add_parameters_from
 from kqcircuits.qubits.qubit import Qubit
 from kqcircuits.pya_resolver import pya
 
-
-@add_parameters_from(Squid, junction_type="Manhattan")
-@add_parameters_from(Manhattan)
+@add_parameters_from(Squid, junction_type="Manhattan Single Junction")
 class DoublePads(Qubit):
     """A two-island qubit, consisting of two rounded rectangles shunted by a junction, with one capacitive coupler.
 
     Contains a coupler on the north edge and two separate qubit islands in the center
     joined by a junction or SQUID loaded from another library.
     Refpoint for a readout line at the opening to the coupler and a modifiable refpoint for
-    a driveline.
+    a driveline outside of the rectangle.
     """
 
     ground_gap = Param(pdt.TypeList, "Width, height of the ground gap (µm, µm)", [700, 700])
     ground_gap_r = Param(pdt.TypeDouble, "Ground gap rounding radius", 50, unit="μm")
     coupler_extent = Param(pdt.TypeList, "Width, height of the coupler (µm, µm)", [150, 20])
     coupler_r = Param(pdt.TypeDouble, "Coupler rounding radius", 10, unit="μm")
     coupler_a = Param(pdt.TypeDouble, "Width of the coupler waveguide center conductor", Element.a, unit="μm")
     coupler_offset = Param(pdt.TypeDouble, "Distance from first qubit island to coupler", 20, unit="μm")
     squid_offset = Param(pdt.TypeDouble, "Offset between SQUID center and qubit center", 0, unit="μm")
     island1_extent = Param(pdt.TypeList, "Width, height of the first qubit island (µm, µm)", [500, 100])
     island1_r = Param(pdt.TypeDouble, "First qubit island rounding radius", 50, unit="μm")
     island2_extent = Param(pdt.TypeList, "Width, height of the second qubit island (µm, µm)", [500, 100])
     island2_r = Param(pdt.TypeDouble, "Second qubit island rounding radius", 50, unit="μm")
     drive_position = Param(pdt.TypeList, "Coordinate for the drive port (µm, µm)", [-450, 0])
-    island1_taper_width = Param(pdt.TypeDouble, "First qubit island tapering width on the island side", 10, unit="µm")
+    island1_taper_width = Param(pdt.TypeDouble, "First qubit island tapering width on the island side", 50, unit="µm")
     island1_taper_junction_width = Param(pdt.TypeDouble,
-                                         "First qubit island tapering width on the junction side", 10, unit="µm")
-    island2_taper_width = Param(pdt.TypeDouble, "Second qubit island tapering width on the island side", 10, unit="µm")
+        "First qubit island tapering width on the junction side", 10, unit="µm")
+    island1_taper_height = Param(pdt.TypeDouble, "First qubit island tapering height", 10, unit="µm")
+    island2_taper_width = Param(pdt.TypeDouble, "Second qubit island tapering width on the island side", 50, unit="µm")
     island2_taper_junction_width = Param(pdt.TypeDouble,
-                                         "Second qubit island tapering width on the junction side", 10, unit="µm")
-
-    island_island_gap = Param(pdt.TypeDouble, "Island to island gap distance", 70, unit="µm")
+        "Second qubit island tapering width on the junction side", 10, unit="µm")
+    island2_taper_height = Param(pdt.TypeDouble, "Second qubit island tapering height", 10, unit="µm")
 
     def build(self):
 
         # Qubit base
         ground_gap_points = [
-            pya.DPoint(float(self.ground_gap[0]) / 2,  float(self.ground_gap[1]) / 2),
-            pya.DPoint(float(self.ground_gap[0]) / 2, -float(self.ground_gap[1]) / 2),
+            pya.DPoint( float(self.ground_gap[0]) / 2,  float(self.ground_gap[1]) / 2),
+            pya.DPoint( float(self.ground_gap[0]) / 2, -float(self.ground_gap[1]) / 2),
             pya.DPoint(-float(self.ground_gap[0]) / 2, -float(self.ground_gap[1]) / 2),
             pya.DPoint(-float(self.ground_gap[0]) / 2,  float(self.ground_gap[1]) / 2),
         ]
         ground_gap_polygon = pya.DPolygon(ground_gap_points)
         ground_gap_region = pya.Region(ground_gap_polygon.to_itype(self.layout.dbu))
         ground_gap_region.round_corners(self.ground_gap_r / self.layout.dbu,
-                                        self.ground_gap_r / self.layout.dbu, self.n)
+            self.ground_gap_r / self.layout.dbu, self.n)
 
         # SQUID
         # Create temporary SQUID cell to calculate SQUID height
         temp_squid_cell = self.add_element(Squid, junction_type=self.junction_type)
         temp_squid_ref = self.get_refpoints(temp_squid_cell)
         squid_height = temp_squid_ref["port_common"].distance(pya.DPoint(0, 0))
         # Now actually add SQUID
         squid_transf = pya.DCplxTrans(1, 0, False, pya.DVector(0, self.squid_offset - squid_height / 2))
         self.produce_squid(squid_transf)
 
-        taper_height = (self.island_island_gap - squid_height)/2
-
         # First island
-        island1_region = self._build_island1(squid_height, taper_height)
+        island1_region = self._build_island1(squid_height)
 
         # Second island
-        island2_region = self._build_island2(squid_height, taper_height)
+        island2_region = self._build_island2(squid_height)
 
         # Coupler gap
         coupler_region = self._build_coupler((self.squid_offset + squid_height / 2)
-                                             + taper_height + float(self.island1_extent[1]))
+            + self.island1_taper_height + float(self.island1_extent[1]))
 
         self.cell.shapes(self.get_layer("base_metal_gap_wo_grid")).insert(
             ground_gap_region - coupler_region - island1_region - island2_region
         )
 
         # Protection
         protection_polygon = pya.DPolygon([
@@ -110,72 +105,74 @@
             (self.ground_gap_r + self.margin) / self.layout.dbu,
             self.n
         )
         self.cell.shapes(self.get_layer("ground_grid_avoidance")).insert(protection_region)
 
         # Coupler port
         self.add_port("cplr", pya.DPoint(0, float(self.ground_gap[1]) / 2),
-                      direction=pya.DVector(pya.DPoint(0, float(self.ground_gap[1]))))
+            direction=pya.DVector(pya.DPoint(0, float(self.ground_gap[1]))))
 
         # Drive port
         self.add_port("drive", pya.DPoint(float(self.drive_position[0]), float(self.drive_position[1])),
-                      direction=pya.DVector(float(self.drive_position[0]), float(self.drive_position[1])))
+            direction=pya.DVector(float(self.drive_position[0]), float(self.drive_position[1])))
+
 
     def _build_coupler(self, first_island_top_edge):
         coupler_top_edge = first_island_top_edge + self.coupler_offset + float(self.coupler_extent[1])
         coupler_polygon = pya.DPolygon([
             pya.DPoint(-float(self.coupler_extent[0]) / 2, coupler_top_edge),
             pya.DPoint(-float(self.coupler_extent[0]) / 2, first_island_top_edge + self.coupler_offset),
-            pya.DPoint(float(self.coupler_extent[0]) / 2, first_island_top_edge + self.coupler_offset),
-            pya.DPoint(float(self.coupler_extent[0]) / 2, coupler_top_edge),
+            pya.DPoint( float(self.coupler_extent[0]) / 2, first_island_top_edge + self.coupler_offset),
+            pya.DPoint( float(self.coupler_extent[0]) / 2, coupler_top_edge),
         ])
         coupler_region = pya.Region(coupler_polygon.to_itype(self.layout.dbu))
         coupler_region.round_corners(self.coupler_r / self.layout.dbu, self.coupler_r / self.layout.dbu, self.n)
         coupler_path_polygon = pya.DPolygon([
             pya.DPoint(-self.coupler_a / 2, (float(self.ground_gap[1]) / 2)),
-            pya.DPoint(self.coupler_a / 2, (float(self.ground_gap[1]) / 2)),
-            pya.DPoint(self.coupler_a / 2, coupler_top_edge),
+            pya.DPoint( self.coupler_a / 2, (float(self.ground_gap[1]) / 2)),
+            pya.DPoint( self.coupler_a / 2, coupler_top_edge),
             pya.DPoint(-self.coupler_a / 2, coupler_top_edge),
         ])
         coupler_path = pya.Region(coupler_path_polygon.to_itype(self.layout.dbu))
         return coupler_region + coupler_path
 
-    def _build_island1(self, squid_height, taper_height):
+
+    def _build_island1(self, squid_height):
         island1_bottom = self.squid_offset + squid_height / 2
         island1_polygon = pya.DPolygon([
             pya.DPoint(-float(self.island1_extent[0]) / 2,
-                       island1_bottom + taper_height + float(self.island1_extent[1])),
-            pya.DPoint(float(self.island1_extent[0]) / 2,
-                       island1_bottom + taper_height + float(self.island1_extent[1])),
-            pya.DPoint(float(self.island1_extent[0]) / 2, island1_bottom + taper_height),
-            pya.DPoint(-float(self.island1_extent[0]) / 2, island1_bottom + taper_height),
+                island1_bottom + self.island1_taper_height + float(self.island1_extent[1])),
+            pya.DPoint( float(self.island1_extent[0]) / 2,
+                island1_bottom + self.island1_taper_height + float(self.island1_extent[1])),
+            pya.DPoint( float(self.island1_extent[0]) / 2, island1_bottom + self.island1_taper_height),
+            pya.DPoint(-float(self.island1_extent[0]) / 2, island1_bottom + self.island1_taper_height),
         ])
         island1_region = pya.Region(island1_polygon.to_itype(self.layout.dbu))
         island1_region.round_corners(self.island1_r / self.layout.dbu, self.island1_r / self.layout.dbu, self.n)
         island1_taper = pya.Region(pya.DPolygon([
-            pya.DPoint(self.island1_taper_width / 2, island1_bottom + taper_height),
-            pya.DPoint(self.island1_taper_junction_width / 2, island1_bottom),
+            pya.DPoint( self.island1_taper_width / 2, island1_bottom + self.island1_taper_height),
+            pya.DPoint( self.island1_taper_junction_width / 2, island1_bottom),
             pya.DPoint(-self.island1_taper_junction_width / 2, island1_bottom),
-            pya.DPoint(-self.island1_taper_width / 2, island1_bottom + taper_height),
+            pya.DPoint(-self.island1_taper_width / 2, island1_bottom + self.island1_taper_height),
         ]).to_itype(self.layout.dbu))
-
         return island1_region + island1_taper
 
-    def _build_island2(self, squid_height, taper_height):
+
+    def _build_island2(self, squid_height):
         island2_top = self.squid_offset - squid_height / 2
         island2_polygon = pya.DPolygon([
             pya.DPoint(-float(self.island2_extent[0]) / 2,
-                       island2_top - taper_height - float(self.island2_extent[1])),
-            pya.DPoint(float(self.island2_extent[0]) / 2,
-                       island2_top - taper_height - float(self.island2_extent[1])),
-            pya.DPoint(float(self.island2_extent[0]) / 2, island2_top - taper_height),
-            pya.DPoint(-float(self.island2_extent[0]) / 2, island2_top - taper_height),
+                island2_top - self.island2_taper_height - float(self.island2_extent[1])),
+            pya.DPoint( float(self.island2_extent[0]) / 2,
+                island2_top - self.island2_taper_height - float(self.island2_extent[1])),
+            pya.DPoint( float(self.island2_extent[0]) / 2, island2_top - self.island2_taper_height),
+            pya.DPoint(-float(self.island2_extent[0]) / 2, island2_top - self.island2_taper_height),
         ])
         island2_region = pya.Region(island2_polygon.to_itype(self.layout.dbu))
         island2_region.round_corners(self.island2_r / self.layout.dbu, self.island2_r / self.layout.dbu, self.n)
         island2_taper = pya.Region(pya.DPolygon([
-            pya.DPoint(self.island2_taper_width / 2, island2_top - taper_height),
-            pya.DPoint(self.island2_taper_junction_width / 2, island2_top),
+            pya.DPoint( self.island2_taper_width / 2, island2_top - self.island2_taper_height),
+            pya.DPoint( self.island2_taper_junction_width / 2, island2_top),
             pya.DPoint(-self.island2_taper_junction_width / 2, island2_top),
-            pya.DPoint(-self.island2_taper_width / 2, island2_top - taper_height),
+            pya.DPoint(-self.island2_taper_width / 2, island2_top - self.island2_taper_height),
         ]).to_itype(self.layout.dbu))
         return island2_region + island2_taper
```

### Comparing `kqcircuits-4.6.21/kqcircuits/qubits/double_pads_splines.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/double_pads_splines.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,57 +34,57 @@
     island_spline = Param(pdt.TypeList, "Control points of a B-Spline that defines left half of the island",
         [-250, 20, -250, 80, -100, 100, 0, 100])
     island_spline_samples = Param(pdt.TypeInt, "Number of samples taken from each island spline", 100,
         docstring=( "Number of samples taken from each island spline. "
                     "There is a spline for each consequent series of four control points"))
 
 
-    def _build_island1(self, squid_height, taper_height):
+    def _build_island1(self, squid_height):
         island1_bottom = self.squid_offset + squid_height / 2
-        curve_start = pya.DPoint(0, island1_bottom + taper_height)
+        curve_start = pya.DPoint(0, island1_bottom + self.island1_taper_height)
         island1_control_points = [curve_start + pya.DPoint(-self.island1_taper_width / 2, 0)] + \
             [curve_start + pya.DPoint(float(self.island_spline[idx]), float(self.island_spline[idx+1]))
                 for idx in range(0, len(self.island_spline), 2)]
         island1_control_points += [pya.DPoint(-p.x, p.y) for p in reversed(island1_control_points[:-1])]
         for i, p in enumerate(island1_control_points):
             self.refpoints[f"island1_control_point_{i}"] = p
         island1_polygon = pya.DPolygon(bspline_points(island1_control_points,
                                                         self.island_spline_samples,
                                                         startpoint=True, endpoint=True))
         island1_region = pya.Region(island1_polygon.to_itype(self.layout.dbu))
         island1_taper = pya.Region(pya.DPolygon([
             #pertrude taper into island in case of precision errors
-            pya.DPoint( self.island1_taper_width / 2, island1_bottom + taper_height + 1),
-            pya.DPoint( self.island1_taper_width / 2, island1_bottom + taper_height),
+            pya.DPoint( self.island1_taper_width / 2, island1_bottom + self.island1_taper_height + 1),
+            pya.DPoint( self.island1_taper_width / 2, island1_bottom + self.island1_taper_height),
             pya.DPoint( self.island1_taper_junction_width / 2, island1_bottom),
             pya.DPoint(-self.island1_taper_junction_width / 2, island1_bottom),
-            pya.DPoint(-self.island1_taper_width / 2, island1_bottom + taper_height),
+            pya.DPoint(-self.island1_taper_width / 2, island1_bottom + self.island1_taper_height),
             #pertrude taper into island in case of precision errors
-            pya.DPoint(-self.island1_taper_width / 2, island1_bottom + taper_height + 1),
+            pya.DPoint(-self.island1_taper_width / 2, island1_bottom + self.island1_taper_height + 1),
         ]).to_itype(self.layout.dbu))
         return island1_region + island1_taper
 
 
-    def _build_island2(self, squid_height, taper_height):
+    def _build_island2(self, squid_height):
         island2_top = self.squid_offset - squid_height / 2
-        curve_start = pya.DPoint(0, island2_top - taper_height)
+        curve_start = pya.DPoint(0, island2_top - self.island2_taper_height)
         island2_control_points = [curve_start + pya.DPoint(-self.island2_taper_width / 2, 0)] + \
             [curve_start + pya.DPoint(float(self.island_spline[idx]), -float(self.island_spline[idx+1]))
                 for idx in range(0, len(self.island_spline), 2)]
         island2_control_points += [pya.DPoint(-p.x, p.y) for p in reversed(island2_control_points[:-1])]
         for i, p in enumerate(island2_control_points):
             self.refpoints[f"island2_control_point_{i}"] = p
         island2_polygon = pya.DPolygon(bspline_points(island2_control_points,
                                                         self.island_spline_samples,
                                                         startpoint=True, endpoint=True))
         island2_region = pya.Region(island2_polygon.to_itype(self.layout.dbu))
         island2_taper = pya.Region(pya.DPolygon([
             #pertrude taper into island in case of precision errors
-            pya.DPoint( self.island2_taper_width / 2, island2_top - taper_height - 1),
-            pya.DPoint( self.island2_taper_width / 2, island2_top - taper_height),
+            pya.DPoint( self.island2_taper_width / 2, island2_top - self.island2_taper_height - 1),
+            pya.DPoint( self.island2_taper_width / 2, island2_top - self.island2_taper_height),
             pya.DPoint( self.island2_taper_junction_width / 2, island2_top),
             pya.DPoint(-self.island2_taper_junction_width / 2, island2_top),
-            pya.DPoint(-self.island2_taper_width / 2, island2_top - taper_height),
+            pya.DPoint(-self.island2_taper_width / 2, island2_top - self.island2_taper_height),
             #pertrude taper into island in case of precision errors
-            pya.DPoint(-self.island2_taper_width / 2, island2_top - taper_height - 1),
+            pya.DPoint(-self.island2_taper_width / 2, island2_top - self.island2_taper_height - 1),
         ]).to_itype(self.layout.dbu))
         return island2_region + island2_taper
```

### Comparing `kqcircuits-4.6.21/kqcircuits/qubits/qubit.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/qubit.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,35 +94,30 @@
             # add parts of qubit to the layer needed for EBL
             region = pya.Region(cell.shapes(self.get_layer("base_metal_gap_wo_grid")))
             region.transform(inst.cplx_trans)
             self.cell.shapes(self.get_layer("base_metal_gap_for_EBL")).insert(region)
 
         return refpoints_rel
 
-    def produce_fluxline(self, rot=0, trans=pya.DVector(), **parameters):
+    def produce_fluxline(self, **parameters):
         """Produces the fluxline.
 
         Creates the fluxline cell and inserts it as a subcell. The "flux" and "flux_corner" ports
-        are made available for the qubit. By default, fluxlines align their "origin_fluxline" refpoint to
-        "origin_squid" refpoint in the direction of "port_common". However, the user might tweak the alignment direction
-        by using the argument rot and the relative position by an extra pya.DVector(x, y) allowing to tune the position
-        to achieve the desired design parameters.
+        are made available for the qubit.
 
         Args:
-            rot: Extra rotation of the fluxline, in degrees
-            trans (DVector): fluxline x/y translation
             parameters: parameters for the fluxline to overwrite default and subclass parameters
         """
 
         if self.fluxline_type == "none":
             return
 
         cell = self.add_element(Fluxline, **parameters)
 
         refpoints_so_far = self.get_refpoints(self.cell)
         squid_edge = refpoints_so_far["origin_squid"]
         a = (squid_edge - refpoints_so_far['port_common'])
         rotation = math.atan2(a.y, a.x) / math.pi * 180 + 90
-        total_transformation = pya.DCplxTrans(1, rotation + rot, False, squid_edge - self.refpoints["base"] + trans)
+        transf = pya.DCplxTrans(1, rotation, False, squid_edge - self.refpoints["base"])
 
-        cell_inst, _ = self.insert_cell(cell, total_transformation)
+        cell_inst, _ = self.insert_cell(cell, transf)
         self.copy_port("flux", cell_inst)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/qubits/swissmon.py` & `kqcircuits-4.6.9rc1/kqcircuits/qubits/swissmon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/airbridges_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/airbridges_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/circular_capacitor_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/circular_capacitor_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/cross_section_simulation.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/cross_section_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/double_pads_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/double_pads_sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,8 +54,8 @@
                 InternalPort((port_i := port_i + 1), *self.etched_line(refp["port_squid_a"], refp["port_squid_b"]),
                     face=port_face, inductance=self.junction_inductance, capacitance=self.junction_capacitance,
                     junction=True
                 )
             )
 
         self.produce_waveguide_to_port(refp["port_cplr"], refp["port_cplr_corner"], (port_i := port_i + 1),
-            "top", waveguide_length=self.waveguide_length, face=port_face)
+            "top", waveguide_length=200, face=port_face)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/empty_simulation.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/empty_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/ansys/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/ansys/ansys_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/ansys/ansys_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/elmer/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/elmer/elmer_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/elmer/elmer_export.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from pathlib import Path
 from distutils.dir_util import copy_tree
 
 from kqcircuits.simulations.export.util import export_layers
 from kqcircuits.util.export_helper import write_commit_reference_file
 from kqcircuits.defaults import ELMER_SCRIPT_PATHS
 from kqcircuits.simulations.simulation import Simulation
-from kqcircuits.simulations.cross_section_simulation import CrossSectionSimulation
 from kqcircuits.util.geometry_json_encoder import GeometryJsonEncoder
 
 
 def copy_elmer_scripts_to_directory(path: Path):
     """
     Copies Elmer scripts into directory path.
 
@@ -41,88 +40,61 @@
         path: Location where to copy scripts folder.
     """
     if path.exists() and path.is_dir():
         for script_path in ELMER_SCRIPT_PATHS:
             copy_tree(str(script_path), str(path), update=1)
 
 
-def export_elmer_json(simulation,
+def export_elmer_json(simulation: Simulation,
                       path: Path,
                       tool='capacitance',
                       linear_system_method='bicgstab',
                       p_element_order=1,
                       frequency=5,
                       mesh_size=None,
-                      workflow=None,
-                      dielectric_surfaces=None,
-                      is_axisymmetric=False):
+                      workflow=None):
     """
     Export Elmer simulation into json and gds files.
 
     Args:
         simulation: The simulation to be exported.
         path: Location where to write json.
-        tool(str): Available: "capacitance", "wave_equation" and "cross-section" (Default: capacitance)
+        tool(str): Available: "capacitance" and "wave_equation" (Default: capacitance)
         linear_system_method(str): Available: 'bicgstab', 'mg' (Default: bicgstab)
         p_element_order(int): polynomial order of p-elements (Default: 1)
         frequency: Units are in GHz. To set up multifrequency analysis, use list of numbers.
         mesh_size(dict): Parameters to determine mesh element sizes
         workflow(dict): Parameters for simulation workflow
-        dielectric_surfaces: Loss tangents for dielectric interfaces, thickness and permittivity should be specified in
-            the simulation. The loss tangent is post-processed to the participation to get the quality factor.
-            Default is None. Input is of the form::
-
-                'substrate': {
-                    'tan_delta_surf': 5e-7
-                },
-                'layerMA': {  # metal–vacuum
-                    'tan_delta_surf': 0.001,  # loss tangent
-                },
-                'layerMS': { # metal–substrate
-                    'tan_delta_surf': 0.001,
-                },
-                'layerSA': { # substrate–vacuum
-                    'tan_delta_surf': 0.001,
-                }
-        is_axisymmetric(bool): Simulate with Axi Symmetric coordinates along :math:`y\\Big|_{x=0}` (Default: False)
 
     Returns:
          Path to exported json file.
     """
-    is_cross_section = isinstance(simulation, CrossSectionSimulation)
-
-    if simulation is None or not isinstance(simulation, (Simulation, CrossSectionSimulation)):
+    if simulation is None or not isinstance(simulation, Simulation):
         raise ValueError("Cannot export without simulation")
 
     # collect data for .json file
-    if is_cross_section:
-        layers = simulation.layer_dict
-
     json_data = {
         'tool': tool,
+        'linear_system_method': linear_system_method,
+        'p_element_order': p_element_order,
         **simulation.get_simulation_data(),
-        **({'layers': {k: (v.layer, v.datatype) for k, v in layers.items()}} if is_cross_section else {}),
         'mesh_size': {} if mesh_size is None else mesh_size,
         'workflow': {} if workflow is None else workflow,
         'frequency': frequency,
-        **({} if dielectric_surfaces is None else {'dielectric_surfaces': dielectric_surfaces}),
-        'linear_system_method': linear_system_method,
-        'p_element_order': p_element_order,
-        'is_axisymmetric': is_axisymmetric,
     }
 
     # write .json file
     json_filename = str(path.joinpath(simulation.name + '.json'))
     with open(json_filename, 'w') as fp:
         json.dump(json_data, fp, cls=GeometryJsonEncoder, indent=4)
 
     # write .gds file
     gds_filename = str(path.joinpath(simulation.name + '.gds'))
     export_layers(gds_filename, simulation.layout, [simulation.cell], output_format='GDS2',
-                  layers=layers.values() if is_cross_section else simulation.get_layers())
+                  layers=simulation.get_layers())
 
     return json_filename
 
 
 def export_elmer_script(json_filenames, path: Path, workflow=None, file_prefix='simulation',
         script_file='scripts/run.py'):
     """
@@ -283,55 +255,36 @@
     return main_script_filename
 
 
 def export_elmer(simulations: [],
                  path: Path,
                  tool='capacitance',
                  linear_system_method='bicgstab',
-                 p_element_order=3,
+                 p_element_order=1,
                  frequency=5,
                  file_prefix='simulation',
                  script_file='scripts/run.py',
                  mesh_size=None,
                  workflow=None,
-                 dielectric_surfaces=None,
-                 is_axisymmetric=False,
                  skip_errors=False):
     """
     Exports an elmer simulation model to the simulation path.
 
     Args:
 
         simulations(list(Simulation)): list of all the simulations
         path(Path): Location where to output the simulation model
-        tool(str): Available: "capacitance", "wave_equation" and "cross-section" (Default: capacitance)
+        tool(str): Available: "capacitance" and "wave_equation" (Default: capacitance)
         linear_system_method(str): Available: 'bicgstab', 'mg' (Default: bicgstab)
         p_element_order(int): polynomial order of p-elements (Default: 1)
         frequency: Units are in GHz. To set up multifrequency analysis, use list of numbers.
         file_prefix: File prefix of the script file to be created.
         script_file: Name of the script file to run.
         mesh_size(dict): Parameters to determine mesh element sizes
         workflow(dict): Parameters for simulation workflow
-        dielectric_surfaces: Loss tangents for dielectric interfaces, thickness and permittivity should be specified in
-            the simulation. The loss tangent is post-processed to the participation to get the quality factor.
-            Default is None. Input is of the form::
-
-                'substrate': {
-                    'tan_delta_surf': 5e-7
-                },
-                'layerMA': {  # metal–vacuum
-                    'tan_delta_surf': 0.001,  # loss tangent
-                },
-                'layerMS': { # metal–substrate
-                    'tan_delta_surf': 0.001,
-                },
-                'layerSA': { # substrate–vacuum
-                    'tan_delta_surf': 0.001,
-                }
-        is_axisymmetric(bool): Simulate with Axi Symmetric coordinates along :math:`y\\Big|_{x=0}` (Default: False)
         skip_errors(bool): Skip simulations that cause errors. (Default: False)
 
             .. warning::
 
                **Use this carefully**, some of your simulations might not make sense physically and
                you might end up wasting time on bad simulations.
 
@@ -353,24 +306,16 @@
             })
 
     write_commit_reference_file(path)
     copy_elmer_scripts_to_directory(path)
     json_filenames = []
     for simulation in simulations:
         try:
-            json_filenames.append(export_elmer_json(simulation=simulation,
-                                                    path=path,
-                                                    tool=tool,
-                                                    linear_system_method=linear_system_method,
-                                                    p_element_order=p_element_order,
-                                                    frequency=frequency,
-                                                    mesh_size=mesh_size,
-                                                    workflow=workflow,
-                                                    dielectric_surfaces=dielectric_surfaces,
-                                                    is_axisymmetric=is_axisymmetric))
+            json_filenames.append(export_elmer_json(simulation, path, tool, linear_system_method,
+                                                    p_element_order, frequency, mesh_size, workflow))
         except (IndexError, ValueError, Exception) as e:  # pylint: disable=broad-except
             if skip_errors:
                 logging.warning(
                     f'Simulation {simulation.name} skipped due to {e.args}. '\
                     'Some of your other simulations might not make sense geometrically. '\
                     'Disable `skip_errors` to see the full traceback.'
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/export_and_run.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/export_and_run.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/simulation_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/simulation_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/parser.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/parser.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/sonnet_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/sonnet_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/sonnet/template.son` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/sonnet/template.son`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/util.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # https://www.gnu.org/licenses/gpl-3.0.html.
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
-import math
 from typing import List
 from kqcircuits.pya_resolver import pya
 from kqcircuits.defaults import default_output_format
 
 
 def export_layers(filename, layout, cells=None, layers=None, output_format=default_output_format):
 
@@ -43,52 +42,29 @@
 def find_edge_from_point_in_cell(cell: pya.Cell, layer: int, point: pya.DPoint, dbu, tolerance=0.01):
     """
     Finds the edge closest to a point, and returns the edge as well as it's polygon and edge index
     """
     return find_edge_from_point_in_polygons(cell.shapes(layer).each(pya.Shapes.SPolygons), point, dbu, tolerance)
 
 
-def _dist(edge: pya.Edge, point: pya.Point):
-    """
-    If point projected to line by edge is in edge then use `distance_abs`
-    but otherwise take the minimum distance to end points
-    """
-    v_edge = pya.Vector(edge.p2-edge.p1)
-    if v_edge.sprod(v_edge) > 0:
-        v_point_start = pya.Vector(point-edge.p1)
-        v_point_end = pya.Vector(point-edge.p2)
-
-        v_point_start_projection = v_edge.sprod(v_point_start)/math.sqrt(v_edge.sprod(v_edge))
-        v_point_end_projection = v_edge.sprod(v_point_end)/math.sqrt(v_edge.sprod(v_edge))
-
-        if edge.length() >= abs(v_point_start_projection+v_point_end_projection):
-            out = edge.distance_abs(point)
-        else:
-            out = min(point.distance(edge.p1), point.distance(edge.p2))
-    else:
-        out = min(point.distance(edge.p1), point.distance(edge.p2))
-    return out
-
-
 def find_edge_from_point_in_polygons(polygons: List[pya.Polygon], point: pya.DPoint, dbu, tolerance=0.01):
     """
     Finds the edge closest to a point, and returns the edge as well as it's polygon and edge index
     """
-
     # Find closest edge to point
     edges = [(i, j, edge.to_dtype(dbu))
              for (i, polygon) in enumerate(polygons)
              for (j, edge) in enumerate(polygon.each_edge())
              ]
-    (distance, i, j, nearest_edge) = \
-        sorted([(_dist(edge, point), i, j, edge) for (i, j, edge) in edges])[0]
-    if distance < tolerance:
+    (sq_distance, i, j, nearest_edge) = \
+        sorted([(((edge.p1 + edge.p2)/2).sq_distance(point), i, j, edge) for (i, j, edge) in edges])[0]
+    if sq_distance < tolerance**2:
         return i, j, nearest_edge
     else:
-        raise ValueError(f"No edge found at {point=}, {nearest_edge=}, {distance=}")
+        raise ValueError(f"No edge found at {point=}, {nearest_edge=}, {sq_distance=}")
 
 
 def get_enclosing_polygon(points: List[List[float]]):
     """
     Order points in such a way that they form a polygon without intersecting
     lines. The ordering is clockwise starting from the left-most point.
```

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/xsection/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/export/xsection/xsection_export.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/export/xsection/xsection_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import ast
 import json
+import logging
 import os
 import subprocess
 from pathlib import Path
 from typing import Callable, List, Tuple, Union
 from kqcircuits.defaults import STARTUPINFO, XSECTION_PROCESS_PATH
 from kqcircuits.pya_resolver import pya, klayout_executable_command
 from kqcircuits.simulations.export.util import export_layers
@@ -47,31 +48,28 @@
         klayout_dir_name = "KLayout"
     elif os.name == "posix":
         klayout_dir_name = ".klayout"
     else:
         raise SystemError("Error: unsupported operating system")
     xsection_plugin_path = os.path.join(os.path.expanduser("~"), klayout_dir_name, "salt/xsection/macros/xsection.lym")
     cut_string = f"{cut1.x},{cut1.y};{cut2.x},{cut2.y}"
-
-    if not klayout_executable_command():
-        raise Exception("Can't find klayout executable command!")
-    if not Path(xsection_plugin_path).is_file():
-        raise Exception("The 'xsection' plugin is missing in KLayout! Go to 'Tools->Manage Packages' to install it.")
-
-    # Hack: Weird prefix keeps getting added when path is converted to string which breaks the ruby plugin
-    xs_run = str(process_path).replace("\\\\?\\", "")
-    xs_params = str(parameters_path).replace("\\\\?\\", "")
-    # When debugging, remove '-z' argument to see ruby error messages
-    subprocess.run([klayout_executable_command(), input_oas.absolute(), '-z', '-nc', '-rx',
-                    '-r', xsection_plugin_path,
-                    '-rd', f'xs_run={xs_run}',
-                    '-rd', f'xs_params={xs_params}',
-                    '-rd', f'xs_cut={cut_string}',
-                    '-rd', f'xs_out={output_oas.absolute()}'],
-        check=True, startupinfo=STARTUPINFO)
+    try:
+        # Hack: Weird prefix keeps getting added when path is converted to string which breaks the ruby plugin
+        xs_run = str(process_path).replace("\\\\?\\", "")
+        xs_params = str(parameters_path).replace("\\\\?\\", "")
+        # When debugging, remove '-z' argument to see ruby error messages
+        subprocess.run([klayout_executable_command(), input_oas.absolute(), '-z', '-nc', '-rx',
+                        '-r', xsection_plugin_path,
+                        '-rd', f'xs_run={xs_run}',
+                        '-rd', f'xs_params={xs_params}',
+                        '-rd', f'xs_cut={cut_string}',
+                        '-rd', f'xs_out={output_oas.absolute()}'],
+            check=True, startupinfo=STARTUPINFO)
+    except FileNotFoundError:
+        logging.warning("Klayout executable not found.")
 
 
 # pylint: disable=dangerous-default-value
 def create_xsections_from_simulations(simulations: List[Simulation],
                                       output_path: Path,
                                       cuts: Union[Tuple[pya.DPoint, pya.DPoint], List[Tuple[pya.DPoint, pya.DPoint]]],
                                       process_path: Path = XSECTION_PROCESS_PATH,
```

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/finger_capacitor_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/finger_capacitor_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/flip_chip_connector_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/flip_chip_connector_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/port.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/port.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/simulation.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/single_xmon.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/single_xmons_full_chip_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/single_xmons_full_chip_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/waveguides_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/waveguides_sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     cpw_length = Param(pdt.TypeDouble, "Waveguide length", 100, unit="μm")
     n_guides = Param(pdt.TypeInt, "Number of guides", 5)
     spacing = Param(pdt.TypeDouble, "Parallel spacing", 100, unit="μm")
     guide_face_id = Param(pdt.TypeString, "Guide face id", '1t1')
     add_bumps = Param(pdt.TypeBoolean, "Add ground bumps", False)
     port_termination_end = Param(pdt.TypeBoolean, "Port termination end", True)
     use_edge_ports = Param(pdt.TypeBoolean, "Use edge ports", True)
-    etch_opposite_face = Param(pdt.TypeBoolean, "Remove the whole opposite face metal if flip chip", False)
-
 
     def build(self):
         self.produce_guides()
         if self.add_bumps:
             self.produce_ground_bumps()
 
     def produce_guides(self):
@@ -74,18 +72,14 @@
                 else:
                     self.produce_waveguide_to_port(p0, p1, i, waveguide_length=cpw_length/2.,
                                                    a=a, b=b, face=face_id[guide_face_id])
                     wg_cell = self.add_element(WaveguideCoplanar, path=pya.DPath([p0, p2], 0), term1=0,
                                                term2=self.b, face_ids=[guide_face_id])
                     self.insert_cell(wg_cell)
 
-            if self.etch_opposite_face:
-                region = pya.Region(self.box.to_itype(self.layout.dbu))
-                self.cell.shapes(self.get_layer("base_metal_gap_wo_grid", face_id=1)).insert(region)
-
     def produce_ground_bumps(self):
         n_guides = self.n_guides
         spacing = self.spacing
         tot_y = (n_guides-1)*spacing
         bump = self.add_element(FlipChipConnectorDc)
 
         for i in range(n_guides-1):
```

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/simulations/xmons_direct_coupling_sim.py` & `kqcircuits-4.6.9rc1/kqcircuits/simulations/xmons_direct_coupling_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/airbridge_dc.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/airbridge_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/cross_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/cross_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/stripes_test.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/stripes_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/test_structure.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/test_structure.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/test_structures/tsv_test_pattern.py` & `kqcircuits-4.6.9rc1/kqcircuits/test_structures/tsv_test_pattern.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/__init__.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/area.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/refpoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,79 @@
 # This code is part of KQCircuits
-# Copyright (C) 2021 IQM Finland Oy
+# Copyright (C) 2022 IQM Finland Oy
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public
 # License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 # warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with this program. If not, see
 # https://www.gnu.org/licenses/gpl-3.0.html.
 #
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
-import logging
-from os import cpu_count
-from time import perf_counter
-
-from autologging import logged
-
 from kqcircuits.pya_resolver import pya
 
 
-@logged
-class AreaReceiver(pya.TileOutputReceiver):
-    """ Class for handling and storing output from :class:`TilingProcessor` """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.area = 0.0
-
-    def put(self, ix, iy, tile, obj, dbu, clip):
-        """ Function called by :class:`TilingProcessor` on output """
-        #pylint: disable=unused-argument
-        self.__log.debug(f"Area for tile {ix},{iy}: {obj} ({dbu})")
-        self.area = obj * (dbu * dbu)  # report as um^2
-
-
-def get_area_and_density(cell: pya.Cell, layer_infos=None):
-    """ Get total area and density :math:`\\rho=\\frac{area}{bbox.area}` of all layers.
-
-    Args:
-        cell: target cell to get area from
-        layer_infos: list of ``LayerInfo`` to get area for, or None to get area for all layers.
-
-    Returns:
-        tuple: tuple containing lists of
-
-          * layer names as str
-          * total area as float
-          * density between 0 and 1 as float
+class Refpoints:
+    """Helper class for extracting reference points from given layer and cell.
 
-    """
-    start_time = perf_counter()
-    layout = cell.layout()
+    Once Refpoints is initialized, it can be used similar way as dictionary, where reference point text (string) field
+    is the key and reference point position (pya.DPoint) is the value.
 
-    tp = pya.TilingProcessor()
-    tp.threads = cpu_count()
-    tp.tile_size = (2000, 2000)  # microns
-    if layer_infos is None:
-        layer_infos = list(layout.layer_infos())
-    layer_areas = [AreaReceiver() for _ in layer_infos]
-    layer_bboxes = [AreaReceiver() for _ in layer_infos]
-
-    for layer_info, area_receiver, bbox_receiver in zip(layer_infos, layer_areas, layer_bboxes):
-        name = f"_{layer_info.name}"  # if `name` starts with a number, tp.execute() fails, so we add an underscore
-        area, bbox = name + '_area', name + '_bbox'
-        tp.input(name, cell.begin_shapes_rec(layout.layer(layer_info)))
-        tp.output(area, area_receiver)
-        tp.output(bbox, bbox_receiver)
-        tp.queue(f"_output({area}, {name}.area)")
-        tp.queue(f"_output({bbox}, {name}.bbox.area)")
-    tp.execute("Calculate polygon and bounding box area")
-
-    areas = [area.area for area in layer_areas]
-    bboxes = [bbox.area for bbox in layer_bboxes]
-    layer_names = [layer_info.name for layer_info in layer_infos]
-    densities = [area / bbox if bbox != 0.0 else 0.0 for area, bbox in zip(areas, bboxes)]
-    if len(areas) > 0:
-        logging.info(f'For cell {cell.name} got layer areas: {areas}')
-        logging.info(f'Area calculation took {perf_counter() - start_time:.1f} seconds')
-
-    return layer_names, areas, densities
+    Refpoints is implemented such that the dictionary is extracted from given layer and cell only when it's used for the
+    first time. Extracting the dictionary can be relatively time-demanding process, so this way we can speed up the
+    element creation process in KQC.
+
+    Attributes:
+        layer: layer specification for source of reference points
+        cell: cell containing the reference points
+        trans: transform for converting reference points into target coordinate system
+        rec_levels: recursion level when looking for reference points from subcells. Set to 0 to disable recursion.
+    """
+    def __init__(self, layer, cell, trans, rec_levels):
+        self.layer = layer
+        self.cell = cell
+        self.trans = trans
+        self.rec_levels = rec_levels
+        self.refpoints = None
+
+    def dict(self):
+        """Extracts and returns reference points as dictionary, where text is the key and position is the value."""
+        if self.refpoints is None:
+            self.refpoints = {}
+            shapes_iter = pya.RecursiveShapeIterator(self.cell.layout(), self.cell, self.layer)
+            if self.rec_levels is not None:
+                shapes_iter.max_depth = self.rec_levels
+            while not shapes_iter.at_end():
+                shape = shapes_iter.shape()
+                if shape.type() in (pya.Shape.TText, pya.Shape.TTextRef):
+                    self.refpoints[shape.text_string] = self.trans * (shapes_iter.dtrans()*pya.DPoint(shape.text_dpos))
+                shapes_iter.next()
+        return self.refpoints
+
+    def __iter__(self):
+        """Returns iterator"""
+        return iter(self.dict())
+
+    def __getitem__(self, item):
+        """The [] operator to return position for given reference point text."""
+        return self.dict()[item]
+
+    def __setitem__(self, item, value):
+        """The [] operator to set a new reference point."""
+        self.dict()[item] = value
+
+    def items(self):
+        """Returns a list of text-position pairs."""
+        return self.dict().items()
+
+    def keys(self):
+        """Returns a list of texts."""
+        return self.dict().keys()
+
+    def values(self):
+        """Returns a list of positions."""
+        return self.dict().values()
```

### Comparing `kqcircuits-4.6.21/kqcircuits/util/count_instances.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/count_instances.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/coupler_lib.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/coupler_lib.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/deep_delete.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/deep_delete.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/dependencies.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/edit_node_plugin.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/edit_node_plugin.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/export_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/export_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,18 +191,29 @@
     """
     Tries to open file with Klayout. If Klayout is not found, opens file with operating system's default application.
     Implementation supports Windows, macOS, and Linux.
     """
     if argv[-1] == "-q":  # quiet mode, do not run viewer
         return
 
-    exe = klayout_executable_command()
-    if not exe:
+    try:
+        subprocess.call((klayout_executable_command(), filepath))
+        return
+    except FileNotFoundError:
         logging.warning("Klayout executable not found.")
-    else:
-        subprocess.call((exe, filepath))
+
+    try:
+        if platform.system() == 'Windows':  # Windows
+            subprocess.call(filepath, shell=True, startupinfo=STARTUPINFO)
+        elif platform.system() == 'Darwin':  # macOS
+            subprocess.call(('open', filepath))
+        else:  # Linux
+            subprocess.call(('xdg-open', filepath))
+    except FileNotFoundError:
+        logging.warning("Unable to open file %s.", filepath)
+
 
 def get_klayout_version():
     if is_standalone_session():
         return f"KLayout {importlib.metadata.version('klayout')}"
     else:
         return pya.Application.instance().version()
```

### Comparing `kqcircuits-4.6.21/kqcircuits/util/geometry_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/groundgrid.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/groundgrid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/gui_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/gui_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/import_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/import_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/label.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/label.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/layout_to_code.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/layout_to_code.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/library_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/library_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/log_router.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/log_router.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import logging
 import sys
 
 
-def route_log(lowest_visible_level="INFO", remove_old_handlers=True, filename="", stdout=True):
-    """Routes the log output to stdout and/or the specified logfile.
+def route_log(lowest_visible_level="INFO", remove_old_handlers=True, filename=""):
+    """Routes the log output to stdout and to an optional file
 
     Enables monitoring the log in KLayout console. If requested it also appends logs to the
     specified file. By default removes old handlers from root logger to avoid output to other places
     than defined here.
 
     Arguments:
         lowest_visible_level (String): one of DEBUG, INFO, WARNING, ERROR, CRITICAL
         remove_old_handlers (Boolean): determines if old handlers are removed from the root logger
         filename: name of the file to append logs to
-        stdout: enable printing logs to standard output
     """
 
     root_logger = logging.getLogger()
 
     # To make sure that the logs are only output to the place defined here, old handlers must be removed from the
     # logger. This is needed for example if you want to set a different lowest_visible_level by re-running this.
     # Otherwise the old handlers would cause output with the old lowest_visible_level.
@@ -43,18 +42,18 @@
         while root_logger.hasHandlers():
             root_logger.removeHandler(root_logger.handlers[0])
 
     message_format = "%(asctime)s:%(levelname)s:%(name)s:%(funcName)s:%(message)s"
     date_format = "%Y-%m-%d %H:%M:%S"
     formatter = logging.Formatter(message_format, date_format)
 
-    if stdout:
-        handler = logging.StreamHandler(stream=sys.stdout)
-        handler.setFormatter(formatter)
-        handler.setLevel(lowest_visible_level)
-        root_logger.addHandler(handler)
+    handler = logging.StreamHandler(stream=sys.stdout)
+    handler.setFormatter(formatter)
+    handler.setLevel(lowest_visible_level)
+
+    root_logger.addHandler(handler)
 
     if filename:
         fh = logging.FileHandler(filename)
         fh.setFormatter(formatter)
         fh.setLevel(lowest_visible_level)
         root_logger.addHandler(fh)
```

### Comparing `kqcircuits-4.6.21/kqcircuits/util/merge.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/merge.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/netlist_extraction.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/netlist_extraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 # The software distribution should follow IQM trademark policy for open-source software
 # (meetiqm.com/developers/osstmpolicy). IQM welcomes contributions to the code. Please see our contribution agreements
 # for individuals (meetiqm.com/developers/clas/individual) and organizations (meetiqm.com/developers/clas/organization).
 
 
 import json
 import logging
-import os.path
 from os import cpu_count
 
 from kqcircuits.defaults import default_layers, default_netlist_breakdown, default_faces
 from kqcircuits.pya_resolver import pya
 from kqcircuits.util.geometry_helper import get_cell_path_length
 from kqcircuits.util.geometry_json_encoder import GeometryJsonEncoder
 
 log = logging.getLogger(__name__)
 
 
-def export_cell_netlist(cell, filename, pcell=None, alt_netlists=None):
-    """Exports netlist(s) in JSON into file(s).
+def export_cell_netlist(cell, filename, pcell=None):
+    """ Exports netlist into `filename` in JSON
 
     The file will have four sections:
     ``{"nets": {...}, "subcircuits": {...}, "circuits": {...}, "chip": {...}}``
 
     KLayout's `terminology <https://www.klayout.de/doc-qt5/manual/lvs_overview.html>`__ differs
     from the one used in typical EDA tools where we have components (resistors, capacitors, etc.),
     pins (the endpoints of components) and nets (i.e. wires between pins). Components are PCell
@@ -43,51 +42,31 @@
     The main conceptual difference is that waveguides, that would be analogous to wires, are also
     treated as components. Consequently, a net in the ``nets`` section usually contains exactly two
     overlapping pins that belong to two different components each identified by a unique
     ``subcircuit_id``. One of these is almost always a waveguide. Unconnected pins are not shown
     except for Launchers.
 
     The ``subcircuits`` section is a dictionary of the used cells: ``<subcircuit_id>: {"cell_name":
-    "...", "subcircuit_location": {"_pya_type": "DPoint", "x": <x>, "y": <y>}, ...}``.
-    Where ``cell_name`` is the name of the used Element optionally appended with ``$<n>`` if there
-    are more than one Elements of the same type. Different instances of the same cell will have
-    different ``subcircuit_id`` but identical ``cell_name``. ``subcircuit_location`` defines the
-    center of the bounding box of the subcircuit's geometry in ``base_metal_gap_wo_grid`` layer,
-    while ``subcircuit_origin`` defines the center of the bounding box of netlist ports of the cell.
+    "...", "subcircuit_location": [<x>, <y>]}``. Where ``cell_name`` is the name of the used Element
+    optionally appended with ``$<n>`` if there are more than one Elements of the same type.
+    Different instances of the same cell will have different ``subcircuit_id`` but identical
+    ``cell_name``.
 
     The ``circuits`` section maps ``cell_name`` to a dictionary of the named Element's parameters.
 
     If the Cell object is a Chip, the ``chip`` section contains bounding boxes of each face in the chip.
 
-    This function may generate alternative netlists too as specified in the ``alt_netlists``
-    dictionary. The keys should be tags that get added to the generated netlist filenames and the
-    values are the corresponding Element breakdown lists used to generate them. The default netlist
-    is generated regadless of this parameter.
-
     Args:
         cell: pya Cell object
         filename: absolute path as convertible to string
         pcell: pya PCell object. If None, an attempt is made to treat cell as pcell
-        alt_netlists: optional dictionary of file name postfixes and element breakdown lists
     """
     if pcell is None:
         pcell = cell
 
-    _export_cell_netlist_breakdown(cell, filename, pcell, default_netlist_breakdown)
-
-    if isinstance(alt_netlists, dict):
-        fn, ext = os.path.splitext(filename)
-        for tag, breakdown in alt_netlists.items():
-            fnt = f"{fn}_{tag}{ext}"
-            _export_cell_netlist_breakdown(cell, fnt, pcell, breakdown)
-
-
-def _export_cell_netlist_breakdown(cell, filename, pcell, breakdown_list):
-    """A helper function of ``export_cell_netlist``, processes a single breakdown list."""
-
     # get LayoutToNetlist object
     layout = cell.layout()
     faces_with_ports = [face_id for face_id in default_faces if f"{face_id}_ports" in default_layers]
     port_layers = [layout.layer(default_layers[f"{face_id}_ports"]) for face_id in faces_with_ports]
     shapes_iter = pya.RecursiveShapeIterator(layout, cell, port_layers)
     ltn = pya.LayoutToNetlist(shapes_iter)
     # text_enlargement>0 converts the texts into boxes so that their overlaps are detected as connections
@@ -103,39 +82,38 @@
     # extract cell to circuit map for finding the netlist of interest
     cm = ltn.const_cell_mapping_into(layout, cell)
     reverse_cell_map = {v: k for k, v in cm.table().items()}
     # export the circuit of interest
     circuit = ltn.netlist().circuit_by_cell_index(reverse_cell_map[cell.cell_index()])
     if circuit:
         log.info(f"Exporting netlist to {filename}")
-        _export_netlist(circuit, filename, ltn.internal_layout(), layout, cm, pcell, breakdown_list)
+        export_netlist(circuit, filename, ltn.internal_layout(), layout, cm, pcell)
     else:
         log.info(f"No circuit found for {cell.display_title()}")
 
 
-def _export_netlist(circuit, filename, internal_layout, original_layout, cell_mapping, pcell, breakdown_list):
-    """A helper function of ``export_cell_netlist``,  exports ``circuit`` into ``filename``.
+def export_netlist(circuit, filename, internal_layout, original_layout, cell_mapping, pcell=None):
+    """ Exports `circuit` into `filename` in JSON
 
     Args:
         circuit: pya Circuit object
         filename: absolute path as convertible to string
         internal_layout: pya layout object where the netlist cells are registered
         original_layout: pya Layout object where the original cells and pcells are registered
         cell_mapping: CellMapping object as given by pya LayoutToNetlist object
-        pcell: pya PCell object from which circuit was extracted
-        breakdown_list: a list of Elements to break down for the netlist
-    """
+        pcell: pya PCell object from which circuit was extracted, if available
 
+    """
     # first flatten subcircuits mentioned in elements to breakdown
     # TODO implement an efficient depth first search or similar solution
     for _ in range(internal_layout.top_cell().hierarchy_levels()):
         subcircuits = list(circuit.each_subcircuit())
         for subcircuit in subcircuits:
             internal_cell = internal_layout.cell(subcircuit.circuit_ref().cell_index)
-            if internal_cell.name.split('$')[0].replace('*', ' ') in breakdown_list:
+            if internal_cell.name.split('$')[0] in default_netlist_breakdown:
                 circuit.flatten_subcircuit(subcircuit)
 
     nets_for_export = {}
     for net in circuit.each_net():
         nets_for_export[net.expanded_name()] = extract_nets(net)
 
     subcircuits_for_export = {}
@@ -163,15 +141,15 @@
     for subcircuit in circuit.each_subcircuit():
         internal_cell = internal_layout.cell(subcircuit.circuit_ref().cell_index)
         if cell_mapping.has_mapping(internal_cell.cell_index()):
             original_cell_index = cell_mapping.cell_mapping(internal_cell.cell_index())
             possible_instances = [(i,i_trans) for i,i_trans in original_instances
                                                 if i.cell.cell_index() == original_cell_index]
         else:
-            log.info(('%s element has no cell mapping in %s between circuit layout and orignal layout,'
+            log.warning(('%s element has no cell mapping in %s between circuit layout and orignal layout,'
                     ' using subcircuit center point as subcircuit_location instead'), internal_cell.name, circuit.name)
             possible_instances = []
 
         used_internal_cells.add(internal_cell)
 
         if hasattr(subcircuit, "trans"):
             subcircuit_trans = subcircuit.trans
@@ -203,19 +181,19 @@
             if len(bboxes) > 0:
                 combined_bbox = pya.DBox(min([bbox.p1.x for bbox in bboxes]), min([bbox.p1.y for bbox in bboxes]),
                                          max([bbox.p2.x for bbox in bboxes]), max([bbox.p2.y for bbox in bboxes]))
                 # subcircuit_location is the center of geometry of all *_base_metal_gap_wo_grid layers in the cell
                 # we also transform the point by instance's predecessors' transformation
                 subcircuit_location = correct_instance_trans * combined_bbox.center()
             else:
-                log.info(('%s element has no bounding boxes in *_base_metal_gap_wo_grid layers in %s,'
+                log.warning(('%s element has no bounding boxes in *_base_metal_gap_wo_grid layers in %s,'
                     ' using subcircuit center point as subcircuit_location instead'),
                     internal_cell.name, circuit.name)
         elif possible_instances:
-            log.info(('Could not find a matching element for %s subcircuit in the orignal layout of %s,'
+            log.warning(('Could not find a matching element for %s subcircuit in the orignal layout of %s,'
                     ' using subcircuit center point as subcircuit_location instead'), internal_cell.name, circuit.name)
 
         subcircuits_for_export[subcircuit.id()] = {
             "cell_name": internal_cell.name,
             "instance_name": correct_instance.property('id') if correct_instance else None,
             "subcircuit_origin": subcircuit_trans.disp,
             "subcircuit_location": subcircuit_location,
@@ -223,15 +201,15 @@
         }
 
     circuits_for_export = {}
     for internal_cell in sorted(used_internal_cells, key=lambda cell: cell.name):
         circuits_for_export[internal_cell.name] = extract_circuits(cell_mapping, internal_cell, original_layout)
 
     chip_for_export = {}
-    if pcell.pcell_declaration() is not None:
+    if pcell is not None and pcell.pcell_declaration() is not None:
         chip_params = pcell.pcell_parameters_by_name()
         if {'frames_enabled', 'face_boxes', 'face_ids', 'box'} <= set(chip_params.keys()):
             for face in chip_params['frames_enabled']:
                 face_box = chip_params['face_boxes'][int(face)]
                 if face_box is None:
                     face_box = chip_params['box']
                 face_id = chip_params['face_ids'][int(face)]
```

### Comparing `kqcircuits-4.6.21/kqcircuits/util/netlist_graph.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/netlist_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,16 @@
     graph = nx.Graph()
     graph.add_edges_from(edges)
 
     # Add data to the nodes
     for subcircuit_id in used_subcircuit_ids:
         subcircuit = network["subcircuits"][str(subcircuit_id)]
         graph.nodes[subcircuit_id]["cell_name"] = subcircuit["cell_name"]
-        graph.nodes[subcircuit_id]["cell_type"] = subcircuit["cell_name"].split('$')[0].replace('*', ' ')
-        graph.nodes[subcircuit_id]["location"] = [  subcircuit["subcircuit_location"]["x"],
-                                                    subcircuit["subcircuit_location"]["y"]]
+        graph.nodes[subcircuit_id]["cell_type"] = subcircuit["cell_name"].split('$')[0]
+        graph.nodes[subcircuit_id]["location"] = subcircuit["subcircuit_location"]
         if "instance_name" in subcircuit and subcircuit["instance_name"] is not None:
             instance_name = subcircuit["instance_name"]
         else:
             instance_name = ""
         base_name = instance_name if instance_name != "" else str(subcircuit_id)
 
         # Define a unique name by suffixing with a number if needed
```

### Comparing `kqcircuits-4.6.21/kqcircuits/util/parameter_helper.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/parameter_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/parameters.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/parameters.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/plugin_startup.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/plugin_startup.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/replace_squids.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/replace_squids.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits/util/symmetric_polygons.py` & `kqcircuits-4.6.9rc1/kqcircuits/util/symmetric_polygons.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.6.21/kqcircuits.egg-info/SOURCES.txt` & `kqcircuits-4.6.9rc1/kqcircuits.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 kqcircuits/simulations/export/__init__.py
 kqcircuits/simulations/export/export_and_run.py
 kqcircuits/simulations/export/simulation_export.py
 kqcircuits/simulations/export/util.py
 kqcircuits/simulations/export/ansys/__init__.py
 kqcircuits/simulations/export/ansys/ansys_export.py
 kqcircuits/simulations/export/elmer/__init__.py
+kqcircuits/simulations/export/elmer/cross_section_elmer_export.py
 kqcircuits/simulations/export/elmer/elmer_export.py
 kqcircuits/simulations/export/sonnet/__init__.py
 kqcircuits/simulations/export/sonnet/parser.py
 kqcircuits/simulations/export/sonnet/sonnet_export.py
 kqcircuits/simulations/export/sonnet/template.son
 kqcircuits/simulations/export/xsection/__init__.py
 kqcircuits/simulations/export/xsection/xsection_export.py
```

### Comparing `kqcircuits-4.6.21/setup.py` & `kqcircuits-4.6.9rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,29 +40,28 @@
     author="IQM Finland Oy",
     author_email="kqcircuits@meetiqm.com",
     url="https://iqm-finland.github.io/KQCircuits/",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.9",
     install_requires=[                # Record dependencies in kqcircuits/util/dependencies.py too
-        "klayout>=0.28",
+        "klayout>=0.26",
         "numpy>=1.16",
         "Autologging~=1.3",
         "scipy>=1.2",
         "tqdm>=4.61",
         # psutil was considered when cpu_count(logical=False), was implemented in an alternative way
         # in elmer_export.py and gmsh_helpers.py, consider adding if more features are needed.
     ],
     extras_require={
         "docs": ["sphinx~=4.4", "sphinx-rtd-theme~=0.4", "networkx>=2.7", "matplotlib>=3.5.1"],
         "tests": ["pytest>=6.0.2", "pytest-cov~=2.8", "pytest-xdist>=2.1", "tox>=3.18", "pylint==2.9",
-                  "networkx>=2.7", "matplotlib>=3.5.1"],
+                  "networkx>=2.7", "matplotlib>=3.5.1", "nbqa~=1.3"],
         "notebooks": ["jupyter~=1.0.0", "klayout>=0.28"],
         "graphs": ["networkx>=2.7", "matplotlib>=3.5.1"],
-        "simulations": ["gmsh>=4.11.1", "pandas>=1.5.3"],
     },
     entry_points={
         'console_scripts':[
             'kqc = console_scripts.run:run',
             ]
         }
 )
```

