# Comparing `tmp/commonroad-drivability-checker-2022.2.1.tar.gz` & `tmp/commonroad-drivability-checker-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad-drivability-checker-2022.2.1.tar", last modified: Fri Nov 25 09:09:27 2022, max compression
+gzip compressed data, was "commonroad-drivability-checker-2023.1.tar", last modified: Fri Jul 21 20:30:00 2023, max compression
```

## Comparing `commonroad-drivability-checker-2022.2.1.tar` & `commonroad-drivability-checker-2023.1.tar`

### file list

```diff
@@ -1,2071 +1,563 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.991338 commonroad-drivability-checker-2022.2.1/
--rw-r--r--   0 root         (0) root         (0)     4761 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1570 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      106 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6076 2022-11-25 09:09:26.991338 commonroad-drivability-checker-2022.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5090 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/commonroad_dc/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5795 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/boundary.py
--rw-r--r--   0 root         (0) root         (0)    25688 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/construction.py
--rw-r--r--   0 root         (0) root         (0)    14915 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/lanelet_bounds.py
--rw-r--r--   0 root         (0) root         (0)      362 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/rectangle_builder.py
--rw-r--r--   0 root         (0) root         (0)     1557 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/scenario_bounds.py
--rw-r--r--   0 root         (0) root         (0)     7479 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/triangle_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3429 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/minkowski_sum.py
--rw-r--r--   0 root         (0) root         (0)     3101 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/pycrcc_collision_dispatch.py
--rw-r--r--   0 root         (0) root         (0)     7188 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/trajectory_queries/
--rw-r--r--   0 root         (0) root         (0)    13816 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/trajectory_queries/trajectory_queries.py
--rw-r--r--   0 root         (0) root         (0)    10833 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/trajectory_queries/trajectory_queries_specialized.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/visualization/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/visualization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3528 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/visualization/drawing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9908 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/evaluation.py
--rw-r--r--   0 root         (0) root         (0)    12256 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/partial_cost_functions.py
--rw-r--r--   0 root         (0) root         (0)    34987 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/route_matcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20312 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/feasibility_checker.py
--rw-r--r--   0 root         (0) root         (0)    17321 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/solution_checker.py
--rw-r--r--   0 root         (0) root         (0)    38520 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/vehicle_dynamics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3825 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11980 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/lanelet_ccosy.py
--rw-r--r--   0 root         (0) root         (0)     5436 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6076 2022-11-25 09:09:26.000000 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)   101041 2022-11-25 09:09:26.000000 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 09:09:26.000000 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 09:09:26.000000 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      129 2022-11-25 09:09:26.000000 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-25 09:09:26.000000 commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/cpp/
--rw-r--r--   0 root         (0) root         (0)     9365 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       77 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/Readme.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/cpp/cmake/
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/cmake/DrivabilityCheckerConfig.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.791343 commonroad-drivability-checker-2022.2.1/cpp/collision/
--rw-r--r--   0 root         (0) root         (0)     4610 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.775343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.795343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/
--rw-r--r--   0 root         (0) root         (0)     1165 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/application.h
--rw-r--r--   0 root         (0) root         (0)     1278 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/application_settings.h
--rw-r--r--   0 root         (0) root         (0)     3626 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_checker.h
--rw-r--r--   0 root         (0) root         (0)     2997 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_object.h
--rw-r--r--   0 root         (0) root         (0)     2356 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_object_ex.h
--rw-r--r--   0 root         (0) root         (0)      545 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_object_types.h
--rw-r--r--   0 root         (0) root         (0)      676 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/i_collision_checker.h
--rw-r--r--   0 root         (0) root         (0)      328 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/i_collision_checker_export.h
--rw-r--r--   0 root         (0) root         (0)      480 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/i_collision_container.h
--rw-r--r--   0 root         (0) root         (0)      323 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/i_collision_object_export.h
--rw-r--r--   0 root         (0) root         (0)     1534 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/line_segment.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.795343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.795343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/detail/
--rw-r--r--   0 root         (0) root         (0)      878 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/detail/aabb.h
--rw-r--r--   0 root         (0) root         (0)     2280 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/detail/obb.h
--rw-r--r--   0 root         (0) root         (0)     1143 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/point.h
--rw-r--r--   0 root         (0) root         (0)     3175 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/polygon.h
--rwxr-xr-x   0 root         (0) root         (0)     2931 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/rectangle_aabb.h
--rw-r--r--   0 root         (0) root         (0)     6271 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/rectangle_obb.h
--rw-r--r--   0 root         (0) root         (0)     1851 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/shape.h
--rw-r--r--   0 root         (0) root         (0)     1579 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/sphere.h
--rw-r--r--   0 root         (0) root         (0)     2542 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/triangle.h
--rw-r--r--   0 root         (0) root         (0)     1677 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/utils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.775343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.795343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/plugins/triangulation/
--rw-r--r--   0 root         (0) root         (0)     1186 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/plugins/triangulation/triangulate.h
--rw-r--r--   0 root         (0) root         (0)     1457 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/primitive_collision_checker.h
--rw-r--r--   0 root         (0) root         (0)     1475 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/raytrace_primitive.h
--rw-r--r--   0 root         (0) root         (0)      998 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/raytrace_utils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.795343 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/
--rw-r--r--   0 root         (0) root         (0)      189 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/basic_types.h
--rw-r--r--   0 root         (0) root         (0)      772 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/broadphase_failure_cc_obj_export.h
--rw-r--r--   0 root         (0) root         (0)      523 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/broadphase_failure_export.h
--rw-r--r--   0 root         (0) root         (0)      778 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/broadphase_failure_obj_obj_export.h
--rw-r--r--   0 root         (0) root         (0)      774 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/collision_checker_export.h
--rw-r--r--   0 root         (0) root         (0)      555 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/collision_object_export_s11.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/
--rw-r--r--   0 root         (0) root         (0)      196 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/point_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      198 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/polygon_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      232 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/rectangle_aabb_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      335 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/rectangle_obb_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      215 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/sphere_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      255 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/triangle_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      200 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/tv_object_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      187 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/export_structs/vertex_export_struct.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/final/
--rw-r--r--   0 root         (0) root         (0)      708 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/final/collision_object_export_final.h
--rw-r--r--   0 root         (0) root         (0)      328 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/i_collision_checker_export.h
--rw-r--r--   0 root         (0) root         (0)      323 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/i_collision_object_export.h
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/point_export.h
--rw-r--r--   0 root         (0) root         (0)      850 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/polygon_export.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/public/
--rw-r--r--   0 root         (0) root         (0)     1629 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/public/serialize_public.h
--rw-r--r--   0 root         (0) root         (0)      730 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/rectangle_aabb_export.h
--rw-r--r--   0 root         (0) root         (0)      723 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/rectangle_obb_export.h
--rw-r--r--   0 root         (0) root         (0)      912 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/serialize.h
--rw-r--r--   0 root         (0) root         (0)     3519 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/serialize_reg_impl.h
--rw-r--r--   0 root         (0) root         (0)      304 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/shape_export.h
--rw-r--r--   0 root         (0) root         (0)      687 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/shape_group_export.h
--rw-r--r--   0 root         (0) root         (0)      679 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/sphere_export.h
--rw-r--r--   0 root         (0) root         (0)      693 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/triangle_export.h
--rw-r--r--   0 root         (0) root         (0)      912 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/tv_object_export.h
--rw-r--r--   0 root         (0) root         (0)      250 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/vector2d_export.h
--rw-r--r--   0 root         (0) root         (0)      603 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/vector2d_export_streams.h
--rw-r--r--   0 root         (0) root         (0)     3590 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/shape_group.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/
--rw-r--r--   0 root         (0) root         (0)      393 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/declarations.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/
--rw-r--r--   0 root         (0) root         (0)      799 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/common.h
--rw-r--r--   0 root         (0) root         (0)      463 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/common_impl.h
--rw-r--r--   0 root         (0) root         (0)      449 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_box2d.h
--rw-r--r--   0 root         (0) root         (0)    11002 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_box2d_inl.h
--rw-r--r--   0 root         (0) root         (0)      381 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_fcl.h
--rw-r--r--   0 root         (0) root         (0)    14172 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_fcl_inl.h
--rw-r--r--   0 root         (0) root         (0)      735 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid.h
--rw-r--r--   0 root         (0) root         (0)      456 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid_common.h
--rw-r--r--   0 root         (0) root         (0)    16860 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid_inl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.799342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/
--rw-r--r--   0 root         (0) root         (0)     1798 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_collision_object.h
--rw-r--r--   0 root         (0) root         (0)     1840 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_collision_queries.h
--rw-r--r--   0 root         (0) root         (0)      529 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_entity_type.h
--rw-r--r--   0 root         (0) root         (0)      353 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_geometry_queries.h
--rw-r--r--   0 root         (0) root         (0)      973 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_helpers.h
--rw-r--r--   0 root         (0) root         (0)      239 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_object_internal.h
--rwxr-xr-x   0 root         (0) root         (0)     5926 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_object_polygon.h
--rw-r--r--   0 root         (0) root         (0)      698 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/i_boost_collision_object.h
--rw-r--r--   0 root         (0) root         (0)      689 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/i_solver_entity_boost.h
--rw-r--r--   0 root         (0) root         (0)      713 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost.h
--rw-r--r--   0 root         (0) root         (0)     1115 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost_factory.h
--rw-r--r--   0 root         (0) root         (0)      356 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_queries.h
--rw-r--r--   0 root         (0) root         (0)      780 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_requests.h
--rw-r--r--   0 root         (0) root         (0)     2039 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_solver_fcl.h
--rw-r--r--   0 root         (0) root         (0)     8589 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_solver_primitive.h
--rw-r--r--   0 root         (0) root         (0)     1224 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_solvers.h
--rw-r--r--   0 root         (0) root         (0)      285 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/distance_queries.h
--rw-r--r--   0 root         (0) root         (0)     1222 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/distance_requests.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/
--rw-r--r--   0 root         (0) root         (0)     1084 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_broadphase_manager_factory.h
--rw-r--r--   0 root         (0) root         (0)     4622 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_checker.h
--rw-r--r--   0 root         (0) root         (0)     2522 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object.h
--rw-r--r--   0 root         (0) root         (0)     2657 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object_group.h
--rw-r--r--   0 root         (0) root         (0)    13038 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_queries.h
--rw-r--r--   0 root         (0) root         (0)    13152 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_requests.h
--rw-r--r--   0 root         (0) root         (0)      484 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_decl.h
--rw-r--r--   0 root         (0) root         (0)     1819 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_queries.h
--rw-r--r--   0 root         (0) root         (0)     1419 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_requests.h
--rw-r--r--   0 root         (0) root         (0)      509 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_entity_type.h
--rw-r--r--   0 root         (0) root         (0)     3435 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_helpers.h
--rw-r--r--   0 root         (0) root         (0)     1563 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_transform.h
--rw-r--r--   0 root         (0) root         (0)      907 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object.h
--rw-r--r--   0 root         (0) root         (0)      719 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object_group.h
--rw-r--r--   0 root         (0) root         (0)      435 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/i_solver_entity_fcl.h
--rw-r--r--   0 root         (0) root         (0)     1776 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/performance_timers.h
--rw-r--r--   0 root         (0) root         (0)      584 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl.h
--rw-r--r--   0 root         (0) root         (0)     1194 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl_factory.h
--rw-r--r--   0 root         (0) root         (0)     1552 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/geometry_queries.h
--rwxr-xr-x   0 root         (0) root         (0)     4280 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/primitive_collision_queries.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/
--rw-r--r--   0 root         (0) root         (0)     1366 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/aabb_sat2d.h
--rw-r--r--   0 root         (0) root         (0)     1706 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/obb_sat2d.h
--rw-r--r--   0 root         (0) root         (0)      591 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/sat2d_checks.h
--rw-r--r--   0 root         (0) root         (0)     1453 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/triangle_sat2d.h
--rw-r--r--   0 root         (0) root         (0)     6058 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/trajectory_queries.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/
--rw-r--r--   0 root         (0) root         (0)      609 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/broadphase_failure.h
--rw-r--r--   0 root         (0) root         (0)     4610 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/broadphase_test.h
--rw-r--r--   0 root         (0) root         (0)      181 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/collision_tests.h
--rw-r--r--   0 root         (0) root         (0)     1319 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/test_common.h
--rw-r--r--   0 root         (0) root         (0)     2466 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/time_variant_collision_object.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/
--rw-r--r--   0 root         (0) root         (0)    11203 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/collision_checker.cc
--rw-r--r--   0 root         (0) root         (0)     1516 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/collision_object.cc
--rw-r--r--   0 root         (0) root         (0)     2579 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/collision_object_ex.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/detail/
--rw-r--r--   0 root         (0) root         (0)      297 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/detail/aabb.cc
--rw-r--r--   0 root         (0) root         (0)     1268 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/point.cc
--rw-r--r--   0 root         (0) root         (0)     5821 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/polygon.cc
--rw-r--r--   0 root         (0) root         (0)     4110 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/rectangle_aabb.cc
--rw-r--r--   0 root         (0) root         (0)     4380 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/rectangle_obb.cc
--rw-r--r--   0 root         (0) root         (0)      705 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/shape.cc
--rw-r--r--   0 root         (0) root         (0)     3508 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/sphere.cc
--rw-r--r--   0 root         (0) root         (0)     3829 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/triangle.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.775343 commonroad-drivability-checker-2022.2.1/cpp/collision/src/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.803342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/plugins/triangulation/
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/plugins/triangulation/gpc_wrapper.c
--rw-r--r--   0 root         (0) root         (0)    11865 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/plugins/triangulation/triangulate.cc
--rw-r--r--   0 root         (0) root         (0)     2479 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/primitive_collision_checker.cc
--rw-r--r--   0 root         (0) root         (0)     5984 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/raytrace_primitive.cc
--rw-r--r--   0 root         (0) root         (0)     7973 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/raytrace_utils.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/final/
--rw-r--r--   0 root         (0) root         (0)      904 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/final/collision_object_export_final.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/public/
--rw-r--r--   0 root         (0) root         (0)     9623 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/public/serialize_public.cc
--rw-r--r--   0 root         (0) root         (0)       52 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize.cc
--rw-r--r--   0 root         (0) root         (0)     1727 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_collision_checker.cc
--rw-r--r--   0 root         (0) root         (0)     2425 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_container_cc_obj.cc
--rw-r--r--   0 root         (0) root         (0)     2504 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_container_obj_obj.cc
--rw-r--r--   0 root         (0) root         (0)     1063 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_point.cc
--rw-r--r--   0 root         (0) root         (0)     3052 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_polygon.cc
--rw-r--r--   0 root         (0) root         (0)     1384 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_rectangle_aabb.cc
--rw-r--r--   0 root         (0) root         (0)     2346 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_rectangle_obb.cc
--rw-r--r--   0 root         (0) root         (0)     1747 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_shape_group.cc
--rw-r--r--   0 root         (0) root         (0)     1252 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_sphere.cc
--rw-r--r--   0 root         (0) root         (0)     1708 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_triangle.cc
--rw-r--r--   0 root         (0) root         (0)     2701 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_tv_object.cc
--rw-r--r--   0 root         (0) root         (0)     6465 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/shape_group.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/
--rw-r--r--   0 root         (0) root         (0)      784 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_collision_object.cc
--rw-r--r--   0 root         (0) root         (0)     8762 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_collision_queries.cc
--rw-r--r--   0 root         (0) root         (0)     1717 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_geometry_queries.cc
--rwxr-xr-x   0 root         (0) root         (0)     4470 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_object_polygon.cc
--rw-r--r--   0 root         (0) root         (0)      337 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/solver_entity_boost.cc
--rw-r--r--   0 root         (0) root         (0)     3021 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_queries.cc
--rw-r--r--   0 root         (0) root         (0)    10782 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_solver_default.cc
--rw-r--r--   0 root         (0) root         (0)    12712 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_solver_fcl.cc
--rw-r--r--   0 root         (0) root         (0)    27974 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_solver_primitive.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/detail/
--rw-r--r--   0 root         (0) root         (0)     1140 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/detail/collision_containers.cc
--rw-r--r--   0 root         (0) root         (0)     3923 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/distance_queries.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/
--rw-r--r--   0 root         (0) root         (0)     1001 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_broadphase_manager_factories.cc
--rw-r--r--   0 root         (0) root         (0)    22419 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_checker.cc
--rw-r--r--   0 root         (0) root         (0)     5150 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_object.cc
--rw-r--r--   0 root         (0) root         (0)     5078 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_object_group.cc
--rw-r--r--   0 root         (0) root         (0)      539 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_queries.cc
--rw-r--r--   0 root         (0) root         (0)     4818 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_requests.cc
--rw-r--r--   0 root         (0) root         (0)     7144 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_distance_queries.cc
--rw-r--r--   0 root         (0) root         (0)     4026 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_distance_requests.cc
--rw-r--r--   0 root         (0) root         (0)     1137 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_entity_factory.cc
--rw-r--r--   0 root         (0) root         (0)     5535 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/performance_timers.cc
--rw-r--r--   0 root         (0) root         (0)      323 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/solver_entity_fcl.cc
--rw-r--r--   0 root         (0) root         (0)     9569 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/geometry_queries.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/sat2d/
--rw-r--r--   0 root         (0) root         (0)     1498 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/sat2d/sat2d_checks.cc
--rw-r--r--   0 root         (0) root         (0)    23711 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/trajectory_queries.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.775343 commonroad-drivability-checker-2022.2.1/cpp/collision/src/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/collision/src/tests/online_tests/
--rw-r--r--   0 root         (0) root         (0)    32436 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/tests/online_tests/broadphase_test.cc
--rw-r--r--   0 root         (0) root         (0)     2094 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/tests/online_tests/test_common.cc
--rw-r--r--   0 root         (0) root         (0)     2718 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/collision/src/time_variant_collision_object.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.807342 commonroad-drivability-checker-2022.2.1/cpp/geometry/
--rw-r--r--   0 root         (0) root         (0)     1539 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/
--rw-r--r--   0 root         (0) root         (0)      149 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/application_settings.h
--rw-r--r--   0 root         (0) root         (0)    23701 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/curvilinear_coordinate_system.h
--rw-r--r--   0 root         (0) root         (0)     7909 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/segment.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/
--rw-r--r--   0 root         (0) root         (0)      189 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/basic_types.h
--rw-r--r--   0 root         (0) root         (0)      989 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/curvilinear_coordinate_system_export.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/export_structs/
--rw-r--r--   0 root         (0) root         (0)      239 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/export_structs/curvilinear_coordinate_system_export_struct.h
--rw-r--r--   0 root         (0) root         (0)      369 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/icurvilinear_coordinate_system_export.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/public/
--rw-r--r--   0 root         (0) root         (0)      537 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/public/serialize_public.h
--rw-r--r--   0 root         (0) root         (0)      181 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/serialize.h
--rw-r--r--   0 root         (0) root         (0)      490 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/serialize_reg_impl.h
--rw-r--r--   0 root         (0) root         (0)      250 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/vector2d_export.h
--rw-r--r--   0 root         (0) root         (0)      603 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/vector2d_export_streams.h
--rw-r--r--   0 root         (0) root         (0)     7359 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/
--rw-r--r--   0 root         (0) root         (0)    57532 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/curvilinear_coordinate_system.cc
--rw-r--r--   0 root         (0) root         (0)     7263 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/segment.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/serialize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/serialize/public/
--rw-r--r--   0 root         (0) root         (0)     2915 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/serialize/public/serialize_public.cc
--rw-r--r--   0 root         (0) root         (0)     2910 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/serialize/serialize_curvil_cs.cc
--rw-r--r--   0 root         (0) root         (0)     3954 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/geometry/src/util.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/python_binding/
--rw-r--r--   0 root         (0) root         (0)     3270 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/python_binding/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/
--rw-r--r--   0 root         (0) root         (0)    56533 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/module_collision.cc
--rw-r--r--   0 root         (0) root         (0)    20088 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/module_geometry.cc
--rw-r--r--   0 root         (0) root         (0)       57 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/py_bind.cc
--rw-r--r--   0 root         (0) root         (0)      924 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/submodule_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/tests/
--rw-r--r--   0 root         (0) root         (0)      384 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/cpp/tests/collision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/cpp/tests/collision/offline_tests/
--rw-r--r--   0 root         (0) root         (0)      331 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/tests/collision/offline_tests/collision_stability_tests.cc
--rw-r--r--   0 root         (0) root         (0)     5036 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/tests/collision/offline_tests/collision_tests.cc
--rw-r--r--   0 root         (0) root         (0)      234 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/tests/collision/offline_tests/collision_tests.h
--rw-r--r--   0 root         (0) root         (0)      235 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/cpp/tests/collision/offline_tests/collision_unit_tests.cc
--rw-r--r--   0 root         (0) root         (0)       79 2022-11-25 09:09:26.991338 commonroad-drivability-checker-2022.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7760 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      274 2022-11-25 09:09:10.000000 commonroad-drivability-checker-2022.2.1/setup_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/third_party/box2d/
--rw-r--r--   0 root         (0) root         (0)       45 2022-11-25 09:09:13.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/.git
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.811342 commonroad-drivability-checker-2022.2.1/third_party/box2d/.github/
--rw-r--r--   0 root         (0) root         (0)      732 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/.github/FUNDING.yml
--rw-r--r--   0 root         (0) root         (0)      242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/.github/issue_template.md
--rw-r--r--   0 root         (0) root         (0)      177 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)       68 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/.gitignore
--rw-r--r--   0 root         (0) root         (0)      388 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     2226 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1859 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1066 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3799 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/README.md
--rw-r--r--   0 root         (0) root         (0)      137 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/build.bat
--rwxr-xr-x   0 root         (0) root         (0)      161 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/build.sh
--rw-r--r--   0 root         (0) root         (0)      142 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/build_docs.sh
--rw-r--r--   0 root         (0) root         (0)      106 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/deploy_docs.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.815342 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/
--rw-r--r--   0 root         (0) root         (0)      996 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)   112702 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/Doxyfile.in
--rw-r--r--   0 root         (0) root         (0)     8162 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/FAQ.md
--rw-r--r--   0 root         (0) root         (0)    15823 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/collision.md
--rw-r--r--   0 root         (0) root         (0)     2796 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/common.md
--rw-r--r--   0 root         (0) root         (0)       49 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/copycss.sh
--rw-r--r--   0 root         (0) root         (0)    60190 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/dynamics.md
--rw-r--r--   0 root         (0) root         (0)     8177 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/extra.css
--rw-r--r--   0 root         (0) root         (0)     9312 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/hello.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/
--rw-r--r--   0 root         (0) root         (0)      912 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/body_origin.gif
--rw-r--r--   0 root         (0) root         (0)     4323 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/captured_toi.svg
--rw-r--r--   0 root         (0) root         (0)    15796 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/chain_loop_inwards.svg
--rw-r--r--   0 root         (0) root         (0)    15846 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/chain_loop_outwards.svg
--rw-r--r--   0 root         (0) root         (0)     8972 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/chain_shape.svg
--rw-r--r--   0 root         (0) root         (0)     2303 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/convex_concave.gif
--rw-r--r--   0 root         (0) root         (0)    48950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/debug_draw.png
--rw-r--r--   0 root         (0) root         (0)     6299 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/distance.svg
--rw-r--r--   0 root         (0) root         (0)     2358 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/distance_joint.gif
--rw-r--r--   0 root         (0) root         (0)     2119 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/gear_joint.gif
--rw-r--r--   0 root         (0) root         (0)    10012 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/ghost_collision.svg
--rw-r--r--   0 root         (0) root         (0)    11430 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/ghost_vertices.svg
--rw-r--r--   0 root         (0) root         (0)     4555 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/logo.svg
--rw-r--r--   0 root         (0) root         (0)    10180 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/manifolds.svg
--rw-r--r--   0 root         (0) root         (0)     5579 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/missed_toi.svg
--rw-r--r--   0 root         (0) root         (0)     8748 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/modules.svg
--rw-r--r--   0 root         (0) root         (0)     5038 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/overlap_test.svg
--rw-r--r--   0 root         (0) root         (0)     2298 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/prismatic_joint.gif
--rw-r--r--   0 root         (0) root         (0)     3526 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/pulley_joint.gif
--rw-r--r--   0 root         (0) root         (0)     5445 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/raycast.svg
--rw-r--r--   0 root         (0) root         (0)     1920 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/revolute_joint.gif
--rw-r--r--   0 root         (0) root         (0)     6344 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/self_intersect.svg
--rw-r--r--   0 root         (0) root         (0)     6361 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/skin_collision.svg
--rw-r--r--   0 root         (0) root         (0)     6958 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/skinned_polygon.svg
--rw-r--r--   0 root         (0) root         (0)    42221 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/testbed.png
--rw-r--r--   0 root         (0) root         (0)     6645 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/tunneling1.svg
--rw-r--r--   0 root         (0) root         (0)     5091 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/tunneling2.svg
--rw-r--r--   0 root         (0) root         (0)     7192 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/wheel_joint.svg
--rw-r--r--   0 root         (0) root         (0)     9638 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/images/winding.svg
--rw-r--r--   0 root         (0) root         (0)     8890 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/loose_ends.md
--rw-r--r--   0 root         (0) root         (0)     8925 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/overview.md
--rw-r--r--   0 root         (0) root         (0)      212 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/references.md
--rw-r--r--   0 root         (0) root         (0)      910 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/docs/testbed.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/
--rw-r--r--   0 root         (0) root         (0)      346 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/include/KHR/
--rw-r--r--   0 root         (0) root         (0)    10277 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/include/KHR/khrplatform.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/include/glad/
--rw-r--r--   0 root         (0) root         (0)   110014 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/include/glad/gl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/src/
--rw-r--r--   0 root         (0) root         (0)    58822 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glad/src/gl.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/
--rw-r--r--   0 root         (0) root         (0)     3804 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.819342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/include/GLFW/
--rw-r--r--   0 root         (0) root         (0)   201594 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/include/GLFW/glfw3.h
--rw-r--r--   0 root         (0) root         (0)    16420 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/include/GLFW/glfw3native.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.823342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/
--rw-r--r--   0 root         (0) root         (0)    13530 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_init.m
--rw-r--r--   0 root         (0) root         (0)     1775 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_joystick.h
--rw-r--r--   0 root         (0) root         (0)    14715 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_joystick.m
--rw-r--r--   0 root         (0) root         (0)    16165 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_monitor.m
--rw-r--r--   0 root         (0) root         (0)     5547 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_platform.h
--rw-r--r--   0 root         (0) root         (0)     2063 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_time.c
--rw-r--r--   0 root         (0) root         (0)    56112 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/cocoa_window.m
--rw-r--r--   0 root         (0) root         (0)    25437 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/context.c
--rw-r--r--   0 root         (0) root         (0)    24575 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/egl_context.c
--rw-r--r--   0 root         (0) root         (0)     8417 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/egl_context.h
--rw-r--r--   0 root         (0) root         (0)     2040 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/glfw_config.h
--rw-r--r--   0 root         (0) root         (0)    22364 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/glx_context.c
--rw-r--r--   0 root         (0) root         (0)     7604 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/glx_context.h
--rw-r--r--   0 root         (0) root         (0)     9117 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/init.c
--rw-r--r--   0 root         (0) root         (0)    35859 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/input.c
--rw-r--r--   0 root         (0) root         (0)    27347 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/internal.h
--rw-r--r--   0 root         (0) root         (0)    12305 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/linux_joystick.c
--rw-r--r--   0 root         (0) root         (0)     2178 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/linux_joystick.h
--rw-r--r--   0 root         (0) root         (0)   115245 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/mappings.h
--rw-r--r--   0 root         (0) root         (0)     5071 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/mappings.h.in
--rw-r--r--   0 root         (0) root         (0)    14234 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/monitor.c
--rw-r--r--   0 root         (0) root         (0)     1972 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/nsgl_context.h
--rw-r--r--   0 root         (0) root         (0)    10953 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/nsgl_context.m
--rw-r--r--   0 root         (0) root         (0)     1729 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/null_init.c
--rw-r--r--   0 root         (0) root         (0)     1585 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/null_joystick.c
--rw-r--r--   0 root         (0) root         (0)     1350 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/null_joystick.h
--rw-r--r--   0 root         (0) root         (0)     2205 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/null_monitor.c
--rw-r--r--   0 root         (0) root         (0)     2193 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/null_platform.h
--rw-r--r--   0 root         (0) root         (0)     7710 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/null_window.c
--rw-r--r--   0 root         (0) root         (0)    11362 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/osmesa_context.c
--rw-r--r--   0 root         (0) root         (0)     3768 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/osmesa_context.h
--rw-r--r--   0 root         (0) root         (0)     3172 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/posix_thread.c
--rw-r--r--   0 root         (0) root         (0)     1682 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/posix_thread.h
--rw-r--r--   0 root         (0) root         (0)     2705 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/posix_time.c
--rw-r--r--   0 root         (0) root         (0)     1513 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/posix_time.h
--rw-r--r--   0 root         (0) root         (0)    11391 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/vulkan.c
--rw-r--r--   0 root         (0) root         (0)    24630 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/wgl_context.c
--rw-r--r--   0 root         (0) root         (0)     6646 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/wgl_context.h
--rw-r--r--   0 root         (0) root         (0)    22958 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_init.c
--rw-r--r--   0 root         (0) root         (0)    26159 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_joystick.c
--rw-r--r--   0 root         (0) root         (0)     2012 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_joystick.h
--rw-r--r--   0 root         (0) root         (0)    15616 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_monitor.c
--rw-r--r--   0 root         (0) root         (0)    15060 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_platform.h
--rw-r--r--   0 root         (0) root         (0)     3046 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_thread.c
--rw-r--r--   0 root         (0) root         (0)     2423 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_time.c
--rw-r--r--   0 root         (0) root         (0)    67777 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/win32_window.c
--rw-r--r--   0 root         (0) root         (0)    33005 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/window.c
--rw-r--r--   0 root         (0) root         (0)    46078 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/wl_init.c
--rw-r--r--   0 root         (0) root         (0)     6407 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/wl_monitor.c
--rw-r--r--   0 root         (0) root         (0)    14479 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/wl_platform.h
--rw-r--r--   0 root         (0) root         (0)    57687 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/wl_window.c
--rw-r--r--   0 root         (0) root         (0)    42564 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/x11_init.c
--rw-r--r--   0 root         (0) root         (0)    16047 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/x11_monitor.c
--rw-r--r--   0 root         (0) root         (0)    16251 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/x11_platform.h
--rw-r--r--   0 root         (0) root         (0)    97117 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/x11_window.c
--rw-r--r--   0 root         (0) root         (0)    22832 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/xkb_unicode.c
--rw-r--r--   0 root         (0) root         (0)     1240 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/glfw/src/xkb_unicode.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.827342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/
--rw-r--r--   0 root         (0) root         (0)      440 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5022 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imconfig.h
--rw-r--r--   0 root         (0) root         (0)   456703 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imgui.cpp
--rw-r--r--   0 root         (0) root         (0)   203797 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imgui.h
--rw-r--r--   0 root         (0) root         (0)   212918 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imgui_demo.cpp
--rw-r--r--   0 root         (0) root         (0)   157969 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imgui_draw.cpp
--rw-r--r--   0 root         (0) root         (0)    98383 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imgui_internal.h
--rw-r--r--   0 root         (0) root         (0)   306199 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imgui_widgets.cpp
--rw-r--r--   0 root         (0) root         (0)    20014 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imstb_rectpack.h
--rw-r--r--   0 root         (0) root         (0)    53192 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imstb_textedit.h
--rw-r--r--   0 root         (0) root         (0)   189912 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/imgui/imstb_truetype.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.827342 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/sajson/
--rw-r--r--   0 root         (0) root         (0)      278 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/sajson/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       88 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/sajson/sajson.cpp
--rw-r--r--   0 root         (0) root         (0)    92205 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/extern/sajson/sajson.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.831342 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/
--rw-r--r--   0 root         (0) root         (0)     1727 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_api.h
--rw-r--r--   0 root         (0) root         (0)     1944 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_block_allocator.h
--rw-r--r--   0 root         (0) root         (0)    23406 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_body.h
--rw-r--r--   0 root         (0) root         (0)     6646 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_broad_phase.h
--rw-r--r--   0 root         (0) root         (0)     3545 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_chain_shape.h
--rw-r--r--   0 root         (0) root         (0)     2217 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_circle_shape.h
--rw-r--r--   0 root         (0) root         (0)     9398 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_collision.h
--rw-r--r--   0 root         (0) root         (0)     5042 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_common.h
--rw-r--r--   0 root         (0) root         (0)    10454 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_contact.h
--rw-r--r--   0 root         (0) root         (0)     1758 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_contact_manager.h
--rw-r--r--   0 root         (0) root         (0)     4843 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_distance.h
--rw-r--r--   0 root         (0) root         (0)     5215 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_distance_joint.h
--rw-r--r--   0 root         (0) root         (0)     3213 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_draw.h
--rw-r--r--   0 root         (0) root         (0)     8192 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_dynamic_tree.h
--rw-r--r--   0 root         (0) root         (0)     3073 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_edge_shape.h
--rw-r--r--   0 root         (0) root         (0)    10015 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_fixture.h
--rw-r--r--   0 root         (0) root         (0)     3561 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_friction_joint.h
--rw-r--r--   0 root         (0) root         (0)     3785 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_gear_joint.h
--rw-r--r--   0 root         (0) root         (0)     2154 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_growable_stack.h
--rw-r--r--   0 root         (0) root         (0)     6093 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_joint.h
--rw-r--r--   0 root         (0) root         (0)    16480 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_math.h
--rw-r--r--   0 root         (0) root         (0)     3948 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_motor_joint.h
--rw-r--r--   0 root         (0) root         (0)     4011 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_mouse_joint.h
--rw-r--r--   0 root         (0) root         (0)     3579 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_polygon_shape.h
--rw-r--r--   0 root         (0) root         (0)     6206 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_prismatic_joint.h
--rw-r--r--   0 root         (0) root         (0)     4709 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_pulley_joint.h
--rw-r--r--   0 root         (0) root         (0)     6392 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_revolute_joint.h
--rw-r--r--   0 root         (0) root         (0)     3259 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_rope.h
--rw-r--r--   0 root         (0) root         (0)     3242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_settings.h
--rw-r--r--   0 root         (0) root         (0)     3829 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_shape.h
--rw-r--r--   0 root         (0) root         (0)     1915 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_stack_allocator.h
--rw-r--r--   0 root         (0) root         (0)     2096 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_time_of_impact.h
--rw-r--r--   0 root         (0) root         (0)     1973 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_time_step.h
--rw-r--r--   0 root         (0) root         (0)     1701 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_timer.h
--rw-r--r--   0 root         (0) root         (0)     1335 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_types.h
--rw-r--r--   0 root         (0) root         (0)     4104 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_weld_joint.h
--rw-r--r--   0 root         (0) root         (0)     6754 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_wheel_joint.h
--rw-r--r--   0 root         (0) root         (0)    10826 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_world.h
--rw-r--r--   0 root         (0) root         (0)     6168 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/b2_world_callbacks.h
--rw-r--r--   0 root         (0) root         (0)     1898 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/include/box2d/box2d.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.831342 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/
--rw-r--r--   0 root         (0) root         (0)     4620 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.831342 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/
--rw-r--r--   0 root         (0) root         (0)     3515 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_broad_phase.cpp
--rw-r--r--   0 root         (0) root         (0)     4727 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_chain_shape.cpp
--rw-r--r--   0 root         (0) root         (0)     3291 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_circle_shape.cpp
--rw-r--r--   0 root         (0) root         (0)     4500 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_collide_circle.cpp
--rw-r--r--   0 root         (0) root         (0)    12223 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_collide_edge.cpp
--rw-r--r--   0 root         (0) root         (0)     6731 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_collide_polygon.cpp
--rw-r--r--   0 root         (0) root         (0)     6621 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_collision.cpp
--rw-r--r--   0 root         (0) root         (0)    16654 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_distance.cpp
--rw-r--r--   0 root         (0) root         (0)    17791 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_dynamic_tree.cpp
--rw-r--r--   0 root         (0) root         (0)     3848 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_edge_shape.cpp
--rw-r--r--   0 root         (0) root         (0)    10560 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_polygon_shape.cpp
--rw-r--r--   0 root         (0) root         (0)    11801 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/collision/b2_time_of_impact.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.831342 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/
--rw-r--r--   0 root         (0) root         (0)     5320 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/b2_block_allocator.cpp
--rw-r--r--   0 root         (0) root         (0)     1440 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/b2_draw.cpp
--rw-r--r--   0 root         (0) root         (0)     2918 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/b2_math.cpp
--rw-r--r--   0 root         (0) root         (0)     1979 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/b2_settings.cpp
--rw-r--r--   0 root         (0) root         (0)     2262 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/b2_stack_allocator.cpp
--rw-r--r--   0 root         (0) root         (0)     2964 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/common/b2_timer.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.835342 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/
--rw-r--r--   0 root         (0) root         (0)    12417 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_body.cpp
--rw-r--r--   0 root         (0) root         (0)     2433 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_chain_circle_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1752 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_chain_circle_contact.h
--rw-r--r--   0 root         (0) root         (0)     2448 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_chain_polygon_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1757 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_chain_polygon_contact.h
--rw-r--r--   0 root         (0) root         (0)     2225 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_circle_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1680 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_circle_contact.h
--rw-r--r--   0 root         (0) root         (0)     7507 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     7116 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_contact_manager.cpp
--rw-r--r--   0 root         (0) root         (0)    23070 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_contact_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     2615 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_contact_solver.h
--rw-r--r--   0 root         (0) root         (0)    11203 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_distance_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     2207 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_edge_circle_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1719 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_edge_circle_contact.h
--rw-r--r--   0 root         (0) root         (0)     2221 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_edge_polygon_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1724 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_edge_polygon_contact.h
--rw-r--r--   0 root         (0) root         (0)     8250 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_fixture.cpp
--rw-r--r--   0 root         (0) root         (0)     7030 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_friction_joint.cpp
--rw-r--r--   0 root         (0) root         (0)    11867 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_gear_joint.cpp
--rw-r--r--   0 root         (0) root         (0)    16696 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_island.cpp
--rw-r--r--   0 root         (0) root         (0)     2645 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_island.h
--rw-r--r--   0 root         (0) root         (0)     7091 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     8243 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_motor_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     4903 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_mouse_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     2249 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_polygon_circle_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1725 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_polygon_circle_contact.h
--rw-r--r--   0 root         (0) root         (0)     2245 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_polygon_contact.cpp
--rw-r--r--   0 root         (0) root         (0)     1685 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_polygon_contact.h
--rw-r--r--   0 root         (0) root         (0)    17284 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_prismatic_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     8918 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_pulley_joint.cpp
--rw-r--r--   0 root         (0) root         (0)    13172 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_revolute_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     8862 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_weld_joint.cpp
--rw-r--r--   0 root         (0) root         (0)    16333 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_wheel_joint.cpp
--rw-r--r--   0 root         (0) root         (0)    29179 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_world.cpp
--rw-r--r--   0 root         (0) root         (0)     1803 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/dynamics/b2_world_callbacks.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.835342 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/rope/
--rw-r--r--   0 root         (0) root         (0)    16548 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/src/rope/b2_rope.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.839341 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/
--rw-r--r--   0 root         (0) root         (0)     2234 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1362 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/MacOSXBundleInfo.plist.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.839341 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/data/
--rw-r--r--   0 root         (0) root         (0)   190044 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/data/droid_sans.ttf
--rw-r--r--   0 root         (0) root         (0)    19317 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/draw.cpp
--rw-r--r--   0 root         (0) root         (0)     2903 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/draw.h
--rw-r--r--   0 root         (0) root         (0)    15307 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/imgui_impl_glfw.cpp
--rw-r--r--   0 root         (0) root         (0)     2198 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/imgui_impl_glfw.h
--rw-r--r--   0 root         (0) root         (0)    24551 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/imgui_impl_opengl3.cpp
--rw-r--r--   0 root         (0) root         (0)     2535 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/imgui_impl_opengl3.h
--rw-r--r--   0 root         (0) root         (0)    16356 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/main.cpp
--rw-r--r--   0 root         (0) root         (0)     5538 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/settings.cpp
--rw-r--r--   0 root         (0) root         (0)     2296 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/settings.h
--rw-r--r--   0 root         (0) root         (0)    12595 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/test.cpp
--rw-r--r--   0 root         (0) root         (0)     4262 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/test.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.843341 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/
--rw-r--r--   0 root         (0) root         (0)     2096 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/add_pair.cpp
--rw-r--r--   0 root         (0) root         (0)     5349 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/apply_force.cpp
--rw-r--r--   0 root         (0) root         (0)     3980 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/body_types.cpp
--rw-r--r--   0 root         (0) root         (0)     4152 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/box_stack.cpp
--rw-r--r--   0 root         (0) root         (0)     3967 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/breakable.cpp
--rw-r--r--   0 root         (0) root         (0)     3110 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/bridge.cpp
--rw-r--r--   0 root         (0) root         (0)     3891 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/bullet_test.cpp
--rw-r--r--   0 root         (0) root         (0)     5189 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/cantilever.cpp
--rw-r--r--   0 root         (0) root         (0)     7065 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/car.cpp
--rw-r--r--   0 root         (0) root         (0)     2327 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/chain.cpp
--rw-r--r--   0 root         (0) root         (0)     3148 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/chain_problem.cpp
--rw-r--r--   0 root         (0) root         (0)     6668 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/character_collision.cpp
--rw-r--r--   0 root         (0) root         (0)     2256 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/circle_stack.cpp
--rw-r--r--   0 root         (0) root         (0)     5343 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/collision_filtering.cpp
--rw-r--r--   0 root         (0) root         (0)     5132 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/collision_processing.cpp
--rw-r--r--   0 root         (0) root         (0)     5512 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/compound_shapes.cpp
--rw-r--r--   0 root         (0) root         (0)     3807 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/confined.cpp
--rw-r--r--   0 root         (0) root         (0)     4867 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/continuous_test.cpp
--rw-r--r--   0 root         (0) root         (0)     2705 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/convex_hull.cpp
--rw-r--r--   0 root         (0) root         (0)     2594 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/conveyor_belt.cpp
--rw-r--r--   0 root         (0) root         (0)     3689 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/distance_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     3487 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/distance_test.cpp
--rw-r--r--   0 root         (0) root         (0)     5099 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/dominos.cpp
--rw-r--r--   0 root         (0) root         (0)     2818 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/dump_loader.cpp
--rw-r--r--   0 root         (0) root         (0)     7659 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/dynamic_tree.cpp
--rw-r--r--   0 root         (0) root         (0)     5472 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/edge_shapes.cpp
--rw-r--r--   0 root         (0) root         (0)     6622 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/edge_test.cpp
--rw-r--r--   0 root         (0) root         (0)     3054 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/friction.cpp
--rw-r--r--   0 root         (0) root         (0)     5223 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/gear_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     1933 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/heavy1.cpp
--rw-r--r--   0 root         (0) root         (0)     2566 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/heavy2.cpp
--rw-r--r--   0 root         (0) root         (0)     2891 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/mobile_balanced.cpp
--rw-r--r--   0 root         (0) root         (0)     2802 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/mobile_unbalanced.cpp
--rw-r--r--   0 root         (0) root         (0)     3061 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/motor_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     3951 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/pinball.cpp
--rw-r--r--   0 root         (0) root         (0)     3275 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/platformer.cpp
--rw-r--r--   0 root         (0) root         (0)     3264 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/polygon_collision.cpp
--rw-r--r--   0 root         (0) root         (0)     6106 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/polygon_shapes.cpp
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/prismatic_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     2773 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/pulley_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     2265 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/pyramid.cpp
--rw-r--r--   0 root         (0) root         (0)    11395 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/ray_cast.cpp
--rw-r--r--   0 root         (0) root         (0)     2247 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/restitution.cpp
--rw-r--r--   0 root         (0) root         (0)     4503 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/revolute_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     8077 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/rope.cpp
--rw-r--r--   0 root         (0) root         (0)     4579 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/sensor.cpp
--rw-r--r--   0 root         (0) root         (0)     5081 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/shape_cast.cpp
--rw-r--r--   0 root         (0) root         (0)     2804 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/shape_editing.cpp
--rw-r--r--   0 root         (0) root         (0)     3489 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/skier.cpp
--rw-r--r--   0 root         (0) root         (0)     3139 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/slider_crank_1.cpp
--rw-r--r--   0 root         (0) root         (0)     4262 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/slider_crank_2.cpp
--rw-r--r--   0 root         (0) root         (0)     6730 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/theo_jansen.cpp
--rw-r--r--   0 root         (0) root         (0)     3961 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/tiles.cpp
--rw-r--r--   0 root         (0) root         (0)     3963 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/time_of_impact.cpp
--rw-r--r--   0 root         (0) root         (0)     2737 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/tumbler.cpp
--rw-r--r--   0 root         (0) root         (0)     6406 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/web.cpp
--rw-r--r--   0 root         (0) root         (0)     3552 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/wheel_joint.cpp
--rw-r--r--   0 root         (0) root         (0)     4609 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/testbed/tests/wrecking_ball.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.843341 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/
--rw-r--r--   0 root         (0) root         (0)      449 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3282 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/collision_test.cpp
--rw-r--r--   0 root         (0) root         (0)   266632 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/doctest.h
--rw-r--r--   0 root         (0) root         (0)     3969 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/hello_world.cpp
--rw-r--r--   0 root         (0) root         (0)     3566 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/joint_test.cpp
--rw-r--r--   0 root         (0) root         (0)     1941 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/math_test.cpp
--rw-r--r--   0 root         (0) root         (0)     2307 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/box2d/unit-test/world_test.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/
--rw-r--r--   0 root         (0) root         (0)     2285 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.appveyor.yml
--rw-r--r--   0 root         (0) root         (0)     1737 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1760 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.clang-tidy
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/articulated_model/
--rw-r--r--   0 root         (0) root         (0)    11474 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/articulated_model/joint.h
--rw-r--r--   0 root         (0) root         (0)     5676 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/articulated_model/joint_config.h
--rw-r--r--   0 root         (0) root         (0)     4590 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/articulated_model/link.h
--rw-r--r--   0 root         (0) root         (0)     7231 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/articulated_model/model.h
--rw-r--r--   0 root         (0) root         (0)     5032 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/articulated_model/model_config.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/learning/
--rw-r--r--   0 root         (0) root         (0)     7639 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/learning/classifier.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/
--rw-r--r--   0 root         (0) root         (0)     2581 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/interpolation.cpp
--rw-r--r--   0 root         (0) root         (0)     2857 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/interpolation.h
--rw-r--r--   0 root         (0) root         (0)     2680 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/interpolation_factory.cpp
--rw-r--r--   0 root         (0) root         (0)     2722 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/interpolation_factory.h
--rw-r--r--   0 root         (0) root         (0)     3108 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/interpolation_linear.cpp
--rw-r--r--   0 root         (0) root         (0)     2628 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/math/motion/taylor_model/interpolation/interpolation_linear.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/narrowphase/
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/narrowphase/penetration_depth_request.h
--rw-r--r--   0 root         (0) root         (0)     2154 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/narrowphase/penetration_depth_result.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/simd/
--rw-r--r--   0 root         (0) root         (0)    36653 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/simd/math_simd_details.h
--rw-r--r--   0 root         (0) root         (0)    12032 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.deprecated/simd/simd_intersect.h
--rw-r--r--   0 root         (0) root         (0)     1806 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.editorconfig
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-25 09:09:14.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.git
--rw-r--r--   0 root         (0) root         (0)     1636 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1257 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/.travis.yml
--rw-r--r--   0 root         (0) root         (0)    14241 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    13950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/
--rw-r--r--   0 root         (0) root         (0)     4584 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/CompilerSettings.cmake
--rw-r--r--   0 root         (0) root         (0)     4961 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/Coveralls.cmake
--rw-r--r--   0 root         (0) root         (0)     1367 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/CoverallsClear.cmake
--rw-r--r--   0 root         (0) root         (0)    16893 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/CoverallsGenerateGcov.cmake
--rw-r--r--   0 root         (0) root         (0)      731 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/FCLVersion.cmake
--rw-r--r--   0 root         (0) root         (0)     3185 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/FindEigen3.cmake
--rw-r--r--   0 root         (0) root         (0)      927 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CMakeModules/cmake_uninstall.cmake.in
--rw-r--r--   0 root         (0) root         (0)     1679 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CPPLINT.cfg
--rw-r--r--   0 root         (0) root         (0)     1891 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CTestConfig.cmake
--rw-r--r--   0 root         (0) root         (0)     1796 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/CTestCustom.cmake.in
--rw-r--r--   0 root         (0) root         (0)      979 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/INSTALL
--rw-r--r--   0 root         (0) root         (0)     1647 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9914 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/ci/
--rwxr-xr-x   0 root         (0) root         (0)      331 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/ci/install_linux.sh
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/ci/install_osx.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/doc/
--rw-r--r--   0 root         (0) root         (0)   106113 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/doc/Doxyfile.in
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/fcl-config.cmake.in
--rw-r--r--   0 root         (0) root         (0)      355 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/fcl.pc.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.779343 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.847341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/
--rw-r--r--   0 root         (0) root         (0)     3311 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.851341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/
--rw-r--r--   0 root         (0) root         (0)    18481 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_SSaP-inl.h
--rw-r--r--   0 root         (0) root         (0)     5807 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_SSaP.h
--rw-r--r--   0 root         (0) root         (0)    28561 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_SaP-inl.h
--rw-r--r--   0 root         (0) root         (0)     7774 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_SaP.h
--rw-r--r--   0 root         (0) root         (0)     7619 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_bruteforce-inl.h
--rw-r--r--   0 root         (0) root         (0)     4360 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_bruteforce.h
--rw-r--r--   0 root         (0) root         (0)     4025 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_collision_manager-inl.h
--rw-r--r--   0 root         (0) root         (0)     5876 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_collision_manager.h
--rw-r--r--   0 root         (0) root         (0)     3459 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_continuous_collision_manager-inl.h
--rw-r--r--   0 root         (0) root         (0)     5817 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_continuous_collision_manager.h
--rw-r--r--   0 root         (0) root         (0)    30876 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_dynamic_AABB_tree-inl.h
--rw-r--r--   0 root         (0) root         (0)     5343 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_dynamic_AABB_tree.h
--rw-r--r--   0 root         (0) root         (0)    33511 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_dynamic_AABB_tree_array-inl.h
--rw-r--r--   0 root         (0) root         (0)     5468 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_dynamic_AABB_tree_array.h
--rw-r--r--   0 root         (0) root         (0)    22775 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_interval_tree-inl.h
--rw-r--r--   0 root         (0) root         (0)     6498 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_interval_tree.h
--rw-r--r--   0 root         (0) root         (0)    18971 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_spatialhash-inl.h
--rw-r--r--   0 root         (0) root         (0)     6808 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/broadphase_spatialhash.h
--rw-r--r--   0 root         (0) root         (0)     9380 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/default_broadphase_callbacks.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.851341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/
--rw-r--r--   0 root         (0) root         (0)    33685 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/hierarchy_tree-inl.h
--rw-r--r--   0 root         (0) root         (0)    11355 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/hierarchy_tree.h
--rw-r--r--   0 root         (0) root         (0)    31723 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/hierarchy_tree_array-inl.h
--rw-r--r--   0 root         (0) root         (0)    10026 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/hierarchy_tree_array.h
--rw-r--r--   0 root         (0) root         (0)    14173 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/interval_tree-inl.h
--rw-r--r--   0 root         (0) root         (0)     4537 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/interval_tree.h
--rw-r--r--   0 root         (0) root         (0)     3488 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/interval_tree_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3081 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/interval_tree_node.h
--rw-r--r--   0 root         (0) root         (0)     5796 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/morton-inl.h
--rw-r--r--   0 root         (0) root         (0)     4023 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/morton.h
--rw-r--r--   0 root         (0) root         (0)     2950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/node_base-inl.h
--rw-r--r--   0 root         (0) root         (0)     2521 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/node_base.h
--rw-r--r--   0 root         (0) root         (0)     2429 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/node_base_array-inl.h
--rw-r--r--   0 root         (0) root         (0)     2344 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/node_base_array.h
--rw-r--r--   0 root         (0) root         (0)     4242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/simple_hash_table-inl.h
--rw-r--r--   0 root         (0) root         (0)     2912 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/simple_hash_table.h
--rw-r--r--   0 root         (0) root         (0)     2457 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/simple_interval-inl.h
--rw-r--r--   0 root         (0) root         (0)     2470 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/simple_interval.h
--rw-r--r--   0 root         (0) root         (0)     4412 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/sparse_hash_table-inl.h
--rw-r--r--   0 root         (0) root         (0)     3047 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/sparse_hash_table.h
--rw-r--r--   0 root         (0) root         (0)     3495 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/spatial_hash-inl.h
--rw-r--r--   0 root         (0) root         (0)     2456 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/broadphase/detail/spatial_hash.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.855341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.855341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/detail/
--rw-r--r--   0 root         (0) root         (0)     7939 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/detail/profiler.h
--rw-r--r--   0 root         (0) root         (0)     2298 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/exception.h
--rw-r--r--   0 root         (0) root         (0)     2602 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/profiler.h
--rw-r--r--   0 root         (0) root         (0)     2521 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/time.h
--rw-r--r--   0 root         (0) root         (0)     6032 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/types.h
--rw-r--r--   0 root         (0) root         (0)     1880 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/unused.h
--rw-r--r--   0 root         (0) root         (0)     4369 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/common/warning.h
--rw-r--r--   0 root         (0) root         (0)     3201 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/config.h.in
--rw-r--r--   0 root         (0) root         (0)     1900 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/fcl.h.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.855341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.855341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/
--rw-r--r--   0 root         (0) root         (0)     3759 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BVH_internal.h
--rw-r--r--   0 root         (0) root         (0)    35711 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BVH_model-inl.h
--rw-r--r--   0 root         (0) root         (0)     8085 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BVH_model.h
--rw-r--r--   0 root         (0) root         (0)     5240 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BVH_utility-inl.h
--rw-r--r--   0 root         (0) root         (0)     2677 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BVH_utility.h
--rw-r--r--   0 root         (0) root         (0)     3680 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BV_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     2909 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BV_node.h
--rw-r--r--   0 root         (0) root         (0)     3204 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/BV_node_base.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.855341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/
--rw-r--r--   0 root         (0) root         (0)     2794 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BVH_front.h
--rw-r--r--   0 root         (0) root         (0)    14183 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BV_fitter-inl.h
--rw-r--r--   0 root         (0) root         (0)     3374 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BV_fitter.h
--rw-r--r--   0 root         (0) root         (0)     2794 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BV_fitter_base.h
--rw-r--r--   0 root         (0) root         (0)    20011 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BV_splitter-inl.h
--rw-r--r--   0 root         (0) root         (0)     5565 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BV_splitter.h
--rw-r--r--   0 root         (0) root         (0)     2810 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/bvh/detail/BV_splitter_base.h
--rw-r--r--   0 root         (0) root         (0)     5641 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/collision_geometry-inl.h
--rw-r--r--   0 root         (0) root         (0)     4524 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/collision_geometry.h
--rw-r--r--   0 root         (0) root         (0)    14651 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/geometric_shape_to_BVH_model-inl.h
--rw-r--r--   0 root         (0) root         (0)     8728 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/geometric_shape_to_BVH_model.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.855341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/octree/
--rw-r--r--   0 root         (0) root         (0)     9180 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/octree/octree-inl.h
--rw-r--r--   0 root         (0) root         (0)     4884 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/octree/octree.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.859341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/
--rw-r--r--   0 root         (0) root         (0)     4324 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/box-inl.h
--rw-r--r--   0 root         (0) root         (0)     2973 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/box.h
--rw-r--r--   0 root         (0) root         (0)     5777 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/capsule-inl.h
--rw-r--r--   0 root         (0) root         (0)     2999 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/capsule.h
--rw-r--r--   0 root         (0) root         (0)     4157 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/cone-inl.h
--rw-r--r--   0 root         (0) root         (0)     2990 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/cone.h
--rw-r--r--   0 root         (0) root         (0)     9312 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/convex-inl.h
--rw-r--r--   0 root         (0) root         (0)     8132 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/convex.h
--rw-r--r--   0 root         (0) root         (0)     4222 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/cylinder-inl.h
--rw-r--r--   0 root         (0) root         (0)     3014 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/cylinder.h
--rw-r--r--   0 root         (0) root         (0)     4826 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/ellipsoid-inl.h
--rw-r--r--   0 root         (0) root         (0)     3042 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/ellipsoid.h
--rw-r--r--   0 root         (0) root         (0)     5171 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/halfspace-inl.h
--rw-r--r--   0 root         (0) root         (0)     3577 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/halfspace.h
--rw-r--r--   0 root         (0) root         (0)     5249 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/plane-inl.h
--rw-r--r--   0 root         (0) root         (0)     3042 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/plane.h
--rw-r--r--   0 root         (0) root         (0)     2415 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/shape_base-inl.h
--rw-r--r--   0 root         (0) root         (0)     2315 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/shape_base.h
--rw-r--r--   0 root         (0) root         (0)     4135 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/sphere-inl.h
--rw-r--r--   0 root         (0) root         (0)     2823 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/sphere.h
--rw-r--r--   0 root         (0) root         (0)     3130 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/triangle_p-inl.h
--rw-r--r--   0 root         (0) root         (0)     2989 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/triangle_p.h
--rw-r--r--   0 root         (0) root         (0)    39718 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/utility-inl.h
--rw-r--r--   0 root         (0) root         (0)     4526 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/geometry/shape/utility.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.859341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.859341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/
--rw-r--r--   0 root         (0) root         (0)     9296 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/AABB-inl.h
--rw-r--r--   0 root         (0) root         (0)     4909 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/AABB.h
--rw-r--r--   0 root         (0) root         (0)    17403 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/OBB-inl.h
--rw-r--r--   0 root         (0) root         (0)     5837 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/OBB.h
--rw-r--r--   0 root         (0) root         (0)     5703 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/OBBRSS-inl.h
--rw-r--r--   0 root         (0) root         (0)     5008 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/OBBRSS.h
--rw-r--r--   0 root         (0) root         (0)    49779 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/RSS-inl.h
--rw-r--r--   0 root         (0) root         (0)     7445 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/RSS.h
--rw-r--r--   0 root         (0) root         (0)    11051 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/kDOP-inl.h
--rw-r--r--   0 root         (0) root         (0)     6102 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/kDOP.h
--rw-r--r--   0 root         (0) root         (0)     8722 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/kIOS-inl.h
--rw-r--r--   0 root         (0) root         (0)     5568 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/kIOS.h
--rw-r--r--   0 root         (0) root         (0)    29496 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/utility-inl.h
--rw-r--r--   0 root         (0) root         (0)     2410 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/bv/utility.h
--rw-r--r--   0 root         (0) root         (0)     7044 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/constants.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.859341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/detail/
--rw-r--r--   0 root         (0) root         (0)     5373 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/detail/polysolver-inl.h
--rw-r--r--   0 root         (0) root         (0)     2892 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/detail/polysolver.h
--rw-r--r--   0 root         (0) root         (0)    12043 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/detail/project-inl.h
--rw-r--r--   0 root         (0) root         (0)     3675 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/detail/project.h
--rw-r--r--   0 root         (0) root         (0)     2723 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/detail/seed.h
--rw-r--r--   0 root         (0) root         (0)    40432 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/geometry-inl.h
--rw-r--r--   0 root         (0) root         (0)     6715 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/geometry.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.863341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/
--rw-r--r--   0 root         (0) root         (0)     2606 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/bv_motion_bound_visitor.h
--rw-r--r--   0 root         (0) root         (0)     7823 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/interp_motion-inl.h
--rw-r--r--   0 root         (0) root         (0)     4856 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/interp_motion.h
--rw-r--r--   0 root         (0) root         (0)     3905 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/motion_base-inl.h
--rw-r--r--   0 root         (0) root         (0)     3557 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/motion_base.h
--rw-r--r--   0 root         (0) root         (0)     7137 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/screw_motion-inl.h
--rw-r--r--   0 root         (0) root         (0)     4180 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/screw_motion.h
--rw-r--r--   0 root         (0) root         (0)    12848 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/spline_motion-inl.h
--rw-r--r--   0 root         (0) root         (0)     4229 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/spline_motion.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.863341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/
--rw-r--r--   0 root         (0) root         (0)    11782 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/interval-inl.h
--rw-r--r--   0 root         (0) root         (0)     4276 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/interval.h
--rw-r--r--   0 root         (0) root         (0)    11409 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/interval_matrix-inl.h
--rw-r--r--   0 root         (0) root         (0)     3581 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/interval_matrix.h
--rw-r--r--   0 root         (0) root         (0)    12248 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/interval_vector-inl.h
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/interval_vector.h
--rw-r--r--   0 root         (0) root         (0)    17457 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/taylor_matrix-inl.h
--rw-r--r--   0 root         (0) root         (0)     4845 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/taylor_matrix.h
--rw-r--r--   0 root         (0) root         (0)    20590 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/taylor_model-inl.h
--rw-r--r--   0 root         (0) root         (0)     5040 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/taylor_model.h
--rw-r--r--   0 root         (0) root         (0)    12731 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/taylor_vector-inl.h
--rw-r--r--   0 root         (0) root         (0)     4423 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/taylor_vector.h
--rw-r--r--   0 root         (0) root         (0)     2891 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/time_interval-inl.h
--rw-r--r--   0 root         (0) root         (0)     2571 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/taylor_model/time_interval.h
--rw-r--r--   0 root         (0) root         (0)    10204 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/tbv_motion_bound_visitor-inl.h
--rw-r--r--   0 root         (0) root         (0)     2990 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/tbv_motion_bound_visitor.h
--rw-r--r--   0 root         (0) root         (0)     4317 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/translation_motion-inl.h
--rw-r--r--   0 root         (0) root         (0)     3107 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/translation_motion.h
--rw-r--r--   0 root         (0) root         (0)     8626 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/triangle_motion_bound_visitor-inl.h
--rw-r--r--   0 root         (0) root         (0)     3652 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/motion/triangle_motion_bound_visitor.h
--rw-r--r--   0 root         (0) root         (0)     6798 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/rng-inl.h
--rw-r--r--   0 root         (0) root         (0)     5272 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/rng.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.863341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/
--rw-r--r--   0 root         (0) root         (0)     2047 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_base.h
--rw-r--r--   0 root         (0) root         (0)     3234 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_r-inl.h
--rw-r--r--   0 root         (0) root         (0)     2727 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_r.h
--rw-r--r--   0 root         (0) root         (0)     3647 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se2-inl.h
--rw-r--r--   0 root         (0) root         (0)     2666 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se2.h
--rw-r--r--   0 root         (0) root         (0)     3104 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se2_disk-inl.h
--rw-r--r--   0 root         (0) root         (0)     2497 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se2_disk.h
--rw-r--r--   0 root         (0) root         (0)     3642 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_euler-inl.h
--rw-r--r--   0 root         (0) root         (0)     2614 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_euler.h
--rw-r--r--   0 root         (0) root         (0)     3280 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_euler_ball-inl.h
--rw-r--r--   0 root         (0) root         (0)     2415 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_euler_ball.h
--rw-r--r--   0 root         (0) root         (0)     3515 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_quat-inl.h
--rw-r--r--   0 root         (0) root         (0)     2603 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_quat.h
--rw-r--r--   0 root         (0) root         (0)     3154 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_quat_ball-inl.h
--rw-r--r--   0 root         (0) root         (0)     2402 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/sampler/sampler_se3_quat_ball.h
--rw-r--r--   0 root         (0) root         (0)     2461 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/triangle.h
--rw-r--r--   0 root         (0) root         (0)     3063 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/variance3-inl.h
--rw-r--r--   0 root         (0) root         (0)     2681 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/math/variance3.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.867341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/
--rw-r--r--   0 root         (0) root         (0)     7092 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision-inl.h
--rw-r--r--   0 root         (0) root         (0)     3063 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision.h
--rw-r--r--   0 root         (0) root         (0)     8356 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision_object-inl.h
--rw-r--r--   0 root         (0) root         (0)     5104 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision_object.h
--rw-r--r--   0 root         (0) root         (0)     3133 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision_request-inl.h
--rw-r--r--   0 root         (0) root         (0)     4389 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision_request.h
--rw-r--r--   0 root         (0) root         (0)     4351 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision_result-inl.h
--rw-r--r--   0 root         (0) root         (0)     3268 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/collision_result.h
--rw-r--r--   0 root         (0) root         (0)     3202 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/contact-inl.h
--rw-r--r--   0 root         (0) root         (0)     3332 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/contact.h
--rw-r--r--   0 root         (0) root         (0)     3372 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/contact_point-inl.h
--rw-r--r--   0 root         (0) root         (0)     2769 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/contact_point.h
--rw-r--r--   0 root         (0) root         (0)    16128 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision-inl.h
--rw-r--r--   0 root         (0) root         (0)     3556 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision.h
--rw-r--r--   0 root         (0) root         (0)     5651 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision_object-inl.h
--rw-r--r--   0 root         (0) root         (0)     3781 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision_object.h
--rw-r--r--   0 root         (0) root         (0)     2634 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision_request-inl.h
--rw-r--r--   0 root         (0) root         (0)     3109 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision_request.h
--rw-r--r--   0 root         (0) root         (0)     2328 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision_result-inl.h
--rw-r--r--   0 root         (0) root         (0)     2481 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/continuous_collision_result.h
--rw-r--r--   0 root         (0) root         (0)     3547 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/cost_source-inl.h
--rw-r--r--   0 root         (0) root         (0)     2611 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/cost_source.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.867341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/
--rw-r--r--   0 root         (0) root         (0)    45269 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/collision_func_matrix-inl.h
--rw-r--r--   0 root         (0) root         (0)     3378 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/collision_func_matrix.h
--rw-r--r--   0 root         (0) root         (0)    51551 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/conservative_advancement_func_matrix-inl.h
--rw-r--r--   0 root         (0) root         (0)     2816 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/conservative_advancement_func_matrix.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.871341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/
--rw-r--r--   0 root         (0) root         (0)     1349 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/alloc.h
--rw-r--r--   0 root         (0) root         (0)    11922 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/epa-inl.h
--rw-r--r--   0 root         (0) root         (0)     4224 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/epa.h
--rw-r--r--   0 root         (0) root         (0)     9411 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/gjk-inl.h
--rw-r--r--   0 root         (0) root         (0)     3995 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/gjk.h
--rw-r--r--   0 root         (0) root         (0)   110586 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/gjk_libccd-inl.h
--rw-r--r--   0 root         (0) root         (0)     9443 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/gjk_libccd.h
--rw-r--r--   0 root         (0) root         (0)     3755 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/list.h
--rw-r--r--   0 root         (0) root         (0)     8329 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/minkowski_diff-inl.h
--rw-r--r--   0 root         (0) root         (0)     3696 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/minkowski_diff.h
--rw-r--r--   0 root         (0) root         (0)     8470 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/polytope.h
--rw-r--r--   0 root         (0) root         (0)     2751 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/simplex.h
--rw-r--r--   0 root         (0) root         (0)     1427 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/convexity_based_algorithm/support.h
--rw-r--r--   0 root         (0) root         (0)    38798 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/distance_func_matrix-inl.h
--rw-r--r--   0 root         (0) root         (0)     3265 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/distance_func_matrix.h
--rw-r--r--   0 root         (0) root         (0)     5264 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/failed_at_this_configuration.h
--rwxr-xr-x   0 root         (0) root         (0)    36271 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/gjk_solver_indep-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     7076 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/gjk_solver_indep.h
--rwxr-xr-x   0 root         (0) root         (0)    33469 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/gjk_solver_libccd-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     6507 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/gjk_solver_libccd.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.871341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/
--rw-r--r--   0 root         (0) root         (0)    23841 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/box_box-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     4305 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/box_box.h
--rw-r--r--   0 root         (0) root         (0)    10094 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/capsule_capsule-inl.h
--rw-r--r--   0 root         (0) root         (0)     5244 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/capsule_capsule.h
--rwxr-xr-x   0 root         (0) root         (0)    21992 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/halfspace-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     7616 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/halfspace.h
--rwxr-xr-x   0 root         (0) root         (0)    25482 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/plane-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     6112 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/plane.h
--rw-r--r--   0 root         (0) root         (0)    10108 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_box-inl.h
--rw-r--r--   0 root         (0) root         (0)     6737 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_box.h
--rwxr-xr-x   0 root         (0) root         (0)     5889 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_capsule-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     3054 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_capsule.h
--rw-r--r--   0 root         (0) root         (0)    11977 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_cylinder-inl.h
--rw-r--r--   0 root         (0) root         (0)     6894 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_cylinder.h
--rwxr-xr-x   0 root         (0) root         (0)     4414 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_sphere-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     2590 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_sphere.h
--rwxr-xr-x   0 root         (0) root         (0)    14334 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_triangle-inl.h
--rwxr-xr-x   0 root         (0) root         (0)     3635 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/sphere_triangle.h
--rw-r--r--   0 root         (0) root         (0)    13277 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/triangle_distance-inl.h
--rw-r--r--   0 root         (0) root         (0)     5147 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/primitive_shape_algorithm/triangle_distance.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.871341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.875341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/
--rw-r--r--   0 root         (0) root         (0)     4351 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/bvh_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3521 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/bvh_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3506 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/bvh_shape_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3031 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/bvh_shape_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3492 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/collision_traversal_node_base-inl.h
--rw-r--r--   0 root         (0) root         (0)     3220 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/collision_traversal_node_base.h
--rw-r--r--   0 root         (0) root         (0)    37337 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/intersect-inl.h
--rw-r--r--   0 root         (0) root         (0)    13970 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/intersect.h
--rw-r--r--   0 root         (0) root         (0)    25985 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/mesh_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     9019 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/mesh_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     6489 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/mesh_continuous_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3842 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/mesh_continuous_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    18225 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/mesh_shape_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     7895 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/mesh_shape_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3730 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/shape_bvh_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3123 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/shape_bvh_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     6183 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/shape_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3397 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/shape_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    16142 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/shape_mesh_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     7268 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision/shape_mesh_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     5284 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3520 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/collision_node.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.879341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/
--rw-r--r--   0 root         (0) root         (0)     4352 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/bvh_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3583 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/bvh_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3459 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/bvh_shape_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3029 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/bvh_shape_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     2542 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/conservative_advancement_stack_data-inl.h
--rw-r--r--   0 root         (0) root         (0)     2365 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/conservative_advancement_stack_data.h
--rw-r--r--   0 root         (0) root         (0)     3520 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/distance_traversal_node_base-inl.h
--rw-r--r--   0 root         (0) root         (0)     3105 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/distance_traversal_node_base.h
--rw-r--r--   0 root         (0) root         (0)    23275 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_conservative_advancement_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     8356 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_conservative_advancement_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    21266 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     9116 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    16041 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_shape_conservative_advancement_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     6870 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_shape_conservative_advancement_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    16601 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_shape_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     7432 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/mesh_shape_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3457 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_bvh_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3103 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_bvh_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     4693 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_conservative_advancement_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3207 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_conservative_advancement_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     4724 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3302 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    12798 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_mesh_conservative_advancement_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     5578 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_mesh_conservative_advancement_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    14456 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_mesh_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     6444 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/distance/shape_mesh_distance_traversal_node.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.879341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.879341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/
--rw-r--r--   0 root         (0) root         (0)     3672 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/mesh_octree_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3567 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/mesh_octree_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3674 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/octree_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3586 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/octree_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3672 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/octree_mesh_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3571 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/octree_mesh_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3714 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/octree_shape_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3595 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/octree_shape_collision_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3714 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/shape_octree_collision_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3595 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/collision/shape_octree_collision_traversal_node.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.879341 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/
--rw-r--r--   0 root         (0) root         (0)     3679 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/mesh_octree_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3473 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/mesh_octree_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3689 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/octree_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3491 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/octree_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3679 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/octree_mesh_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3478 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/octree_mesh_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3724 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/octree_shape_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3500 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/octree_shape_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)     3724 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/shape_octree_distance_traversal_node-inl.h
--rw-r--r--   0 root         (0) root         (0)     3500 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/distance/shape_octree_distance_traversal_node.h
--rw-r--r--   0 root         (0) root         (0)    37013 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/octree_solver-inl.h
--rw-r--r--   0 root         (0) root         (0)     8094 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/octree/octree_solver.h
--rw-r--r--   0 root         (0) root         (0)     4019 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/traversal_node_base-inl.h
--rw-r--r--   0 root         (0) root         (0)     3339 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/traversal_node_base.h
--rw-r--r--   0 root         (0) root         (0)    14469 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/traversal_recurse-inl.h
--rw-r--r--   0 root         (0) root         (0)     3883 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/detail/traversal/traversal_recurse.h
--rw-r--r--   0 root         (0) root         (0)     8638 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/distance-inl.h
--rw-r--r--   0 root         (0) root         (0)     2802 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/distance.h
--rw-r--r--   0 root         (0) root         (0)     2889 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/distance_request-inl.h
--rw-r--r--   0 root         (0) root         (0)     4659 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/distance_request.h
--rw-r--r--   0 root         (0) root         (0)     3985 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/distance_result-inl.h
--rw-r--r--   0 root         (0) root         (0)     4136 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/distance_result.h
--rwxr-xr-x   0 root         (0) root         (0)     2002 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/include/fcl/narrowphase/gjk_solver_type.h
--rw-r--r--   0 root         (0) root         (0)      505 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/package.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.879341 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/
--rw-r--r--   0 root         (0) root         (0)     5578 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.879341 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/
--rw-r--r--   0 root         (0) root         (0)     1899 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_SSaP.cpp
--rw-r--r--   0 root         (0) root         (0)     1901 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_SaP.cpp
--rw-r--r--   0 root         (0) root         (0)     1910 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_bruteforce.cpp
--rw-r--r--   0 root         (0) root         (0)     1922 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_collision_manager.cpp
--rw-r--r--   0 root         (0) root         (0)     1943 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_continuous_collision_manager.cpp
--rw-r--r--   0 root         (0) root         (0)     1927 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_dynamic_AABB_tree.cpp
--rw-r--r--   0 root         (0) root         (0)     1939 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_dynamic_AABB_tree_array.cpp
--rw-r--r--   0 root         (0) root         (0)     1920 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_interval_tree.cpp
--rw-r--r--   0 root         (0) root         (0)     2032 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/broadphase_spatialhash.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/detail/
--rw-r--r--   0 root         (0) root         (0)     1985 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/detail/interval_tree.cpp
--rw-r--r--   0 root         (0) root         (0)     1950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/detail/interval_tree_node.cpp
--rw-r--r--   0 root         (0) root         (0)     3367 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/detail/morton.cpp
--rw-r--r--   0 root         (0) root         (0)     1946 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/detail/simple_interval.cpp
--rw-r--r--   0 root         (0) root         (0)     1941 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/broadphase/detail/spatial_hash.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/common/detail/
--rw-r--r--   0 root         (0) root         (0)    12165 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/common/detail/profiler.cpp
--rw-r--r--   0 root         (0) root         (0)     2371 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/common/exception.cpp
--rw-r--r--   0 root         (0) root         (0)     2439 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/common/time.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/bvh/
--rw-r--r--   0 root         (0) root         (0)     2218 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/bvh/BVH_utility.cpp
--rw-r--r--   0 root         (0) root         (0)     2435 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/bvh/BV_node_base.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/bvh/detail/
--rw-r--r--   0 root         (0) root         (0)     2293 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/bvh/detail/BVH_front.cpp
--rw-r--r--   0 root         (0) root         (0)     1900 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/collision_geometry.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/octree/
--rw-r--r--   0 root         (0) root         (0)     2200 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/octree/octree.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/
--rw-r--r--   0 root         (0) root         (0)     1877 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/box.cpp
--rw-r--r--   0 root         (0) root         (0)     1885 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/capsule.cpp
--rw-r--r--   0 root         (0) root         (0)     1879 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/cone.cpp
--rw-r--r--   0 root         (0) root         (0)     1883 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/convex.cpp
--rw-r--r--   0 root         (0) root         (0)     1887 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/cylinder.cpp
--rw-r--r--   0 root         (0) root         (0)     1889 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/ellipsoid.cpp
--rw-r--r--   0 root         (0) root         (0)     1986 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/halfspace.cpp
--rw-r--r--   0 root         (0) root         (0)     2132 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/plane.cpp
--rw-r--r--   0 root         (0) root         (0)     1890 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/shape_base.cpp
--rw-r--r--   0 root         (0) root         (0)     1883 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/sphere.cpp
--rw-r--r--   0 root         (0) root         (0)     1890 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/triangle_p.cpp
--rw-r--r--   0 root         (0) root         (0)     9741 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/geometry/shape/utility.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/
--rw-r--r--   0 root         (0) root         (0)     1872 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/AABB.cpp
--rw-r--r--   0 root         (0) root         (0)     2881 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/OBB.cpp
--rw-r--r--   0 root         (0) root         (0)     2126 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/OBBRSS.cpp
--rw-r--r--   0 root         (0) root         (0)     3296 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/RSS.cpp
--rw-r--r--   0 root         (0) root         (0)     2955 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/kDOP.cpp
--rw-r--r--   0 root         (0) root         (0)     1873 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/kIOS.cpp
--rw-r--r--   0 root         (0) root         (0)     7950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/bv/utility.cpp
--rw-r--r--   0 root         (0) root         (0)     1792 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/constants.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.883340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/detail/
--rw-r--r--   0 root         (0) root         (0)     1979 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/detail/polysolver.cpp
--rw-r--r--   0 root         (0) root         (0)     1974 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/detail/project.cpp
--rw-r--r--   0 root         (0) root         (0)     3888 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/detail/seed.cpp
--rw-r--r--   0 root         (0) root         (0)     6260 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/geometry.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.887340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/
--rw-r--r--   0 root         (0) root         (0)     1893 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/interp_motion.cpp
--rw-r--r--   0 root         (0) root         (0)     1889 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/motion_base.cpp
--rw-r--r--   0 root         (0) root         (0)     1891 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/screw_motion.cpp
--rw-r--r--   0 root         (0) root         (0)     1893 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/spline_motion.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.887340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/
--rw-r--r--   0 root         (0) root         (0)     2436 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/interval.cpp
--rw-r--r--   0 root         (0) root         (0)     2271 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/interval_matrix.cpp
--rw-r--r--   0 root         (0) root         (0)     2454 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/interval_vector.cpp
--rw-r--r--   0 root         (0) root         (0)     3310 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/taylor_matrix.cpp
--rw-r--r--   0 root         (0) root         (0)     3134 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/taylor_model.cpp
--rw-r--r--   0 root         (0) root         (0)     2857 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/taylor_vector.cpp
--rw-r--r--   0 root         (0) root         (0)     2038 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/taylor_model/time_interval.cpp
--rw-r--r--   0 root         (0) root         (0)     1903 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/translation_motion.cpp
--rw-r--r--   0 root         (0) root         (0)     1923 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/motion/triangle_motion_bound_visitor.cpp
--rw-r--r--   0 root         (0) root         (0)     1948 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/rng.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.887340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/
--rw-r--r--   0 root         (0) root         (0)     1888 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_base.cpp
--rw-r--r--   0 root         (0) root         (0)     1890 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_se2.cpp
--rw-r--r--   0 root         (0) root         (0)     1900 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_se2_disk.cpp
--rw-r--r--   0 root         (0) root         (0)     1901 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_se3_euler.cpp
--rw-r--r--   0 root         (0) root         (0)     1911 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_se3_euler_ball.cpp
--rw-r--r--   0 root         (0) root         (0)     1899 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_se3_quat.cpp
--rw-r--r--   0 root         (0) root         (0)     1909 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/sampler/sampler_se3_quat_ball.cpp
--rw-r--r--   0 root         (0) root         (0)     2626 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/triangle.cpp
--rw-r--r--   0 root         (0) root         (0)     1879 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/math/variance3.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.887340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/
--rw-r--r--   0 root         (0) root         (0)     2471 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/collision.cpp
--rw-r--r--   0 root         (0) root         (0)     1899 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/collision_object.cpp
--rw-r--r--   0 root         (0) root         (0)     1902 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/collision_request.cpp
--rw-r--r--   0 root         (0) root         (0)     1900 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/collision_result.cpp
--rw-r--r--   0 root         (0) root         (0)     1883 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/contact.cpp
--rw-r--r--   0 root         (0) root         (0)     2314 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/contact_point.cpp
--rw-r--r--   0 root         (0) root         (0)     3384 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/continuous_collision.cpp
--rw-r--r--   0 root         (0) root         (0)     1920 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/continuous_collision_object.cpp
--rw-r--r--   0 root         (0) root         (0)     1923 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/continuous_collision_request.cpp
--rw-r--r--   0 root         (0) root         (0)     1921 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/continuous_collision_result.cpp
--rw-r--r--   0 root         (0) root         (0)     1890 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/cost_source.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.887340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.887340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/convexity_based_algorithm/
--rw-r--r--   0 root         (0) root         (0)     1950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/convexity_based_algorithm/epa.cpp
--rw-r--r--   0 root         (0) root         (0)     1950 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/convexity_based_algorithm/gjk.cpp
--rw-r--r--   0 root         (0) root         (0)     4206 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/convexity_based_algorithm/gjk_libccd.cpp
--rw-r--r--   0 root         (0) root         (0)     1971 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/convexity_based_algorithm/minkowski_diff.cpp
--rw-r--r--   0 root         (0) root         (0)      489 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/failed_at_this_configuration.cpp
--rwxr-xr-x   0 root         (0) root         (0)     1949 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/gjk_solver_indep.cpp
--rwxr-xr-x   0 root         (0) root         (0)     1951 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/gjk_solver_libccd.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.891340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/
--rwxr-xr-x   0 root         (0) root         (0)     3225 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/box_box.cpp
--rw-r--r--   0 root         (0) root         (0)     2841 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/capsule_capsule.cpp
--rwxr-xr-x   0 root         (0) root         (0)     6062 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/halfspace.cpp
--rw-r--r--   0 root         (0) root         (0)     2005 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/intersect.cpp
--rwxr-xr-x   0 root         (0) root         (0)     5821 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/plane.cpp
--rw-r--r--   0 root         (0) root         (0)     2554 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/sphere_box.cpp
--rwxr-xr-x   0 root         (0) root         (0)     2857 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/sphere_capsule.cpp
--rw-r--r--   0 root         (0) root         (0)     2627 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/sphere_cylinder.cpp
--rwxr-xr-x   0 root         (0) root         (0)     2602 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/sphere_sphere.cpp
--rwxr-xr-x   0 root         (0) root         (0)     3879 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/sphere_triangle.cpp
--rw-r--r--   0 root         (0) root         (0)     2108 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/primitive_shape_algorithm/triangle_distance.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.891340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.891340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/collision/
--rw-r--r--   0 root         (0) root         (0)     1992 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/collision/collision_traversal_node_base.cpp
--rw-r--r--   0 root         (0) root         (0)     4068 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/collision/mesh_collision_traversal_node.cpp
--rw-r--r--   0 root         (0) root         (0)     2004 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/collision/mesh_continuous_collision_traversal_node.cpp
--rw-r--r--   0 root         (0) root         (0)     2803 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/collision_node.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.891340 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/distance/
--rw-r--r--   0 root         (0) root         (0)     2004 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/distance/conservative_advancement_stack_data.cpp
--rw-r--r--   0 root         (0) root         (0)     1989 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/distance/distance_traversal_node_base.cpp
--rw-r--r--   0 root         (0) root         (0)     2942 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/distance/mesh_conservative_advancement_traversal_node.cpp
--rw-r--r--   0 root         (0) root         (0)     3526 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/distance/mesh_distance_traversal_node.cpp
--rw-r--r--   0 root         (0) root         (0)     1963 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/traversal_node_base.cpp
--rw-r--r--   0 root         (0) root         (0)     3426 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/detail/traversal/traversal_recurse.cpp
--rw-r--r--   0 root         (0) root         (0)     2446 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/distance.cpp
--rw-r--r--   0 root         (0) root         (0)     1900 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/distance_request.cpp
--rw-r--r--   0 root         (0) root         (0)     1898 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/src/narrowphase/distance_result.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.895340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/
--rw-r--r--   0 root         (0) root         (0)     3462 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.895340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/broadphase/
--rw-r--r--   0 root         (0) root         (0)      155 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/broadphase/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5827 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/broadphase/test_broadphase_dynamic_AABB_tree.cpp
--rw-r--r--   0 root         (0) root         (0)     6022 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/eigen_matrix_compare.h
--rw-r--r--   0 root         (0) root         (0)     6333 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/expect_throws_message.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.895340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/
--rw-r--r--   0 root         (0) root         (0)     1829 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/config.h.in
--rw-r--r--   0 root         (0) root         (0)   186242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/env.obj
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.895340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/
--rw-r--r--   0 root         (0) root         (0)   401385 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/Model 1.pptx
--rw-r--r--   0 root         (0) root         (0)   728877 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/Model_1.xml
--rw-r--r--   0 root         (0) root         (0)       92 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/Model_1.xmlmodel.txt
--rw-r--r--   0 root         (0) root         (0)   755755 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/Model_4.xml
--rw-r--r--   0 root         (0) root         (0)       92 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/Model_4.xmlmodel.txt
--rw-r--r--   0 root         (0) root         (0)   755757 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/manyframes/Model_5.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.899340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/newdata/
--rw-r--r--   0 root         (0) root         (0)   387128 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/newdata/Model_1_Scenario_3.xml
--rw-r--r--   0 root         (0) root         (0)  1630765 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/newdata/Model_2_Scenario_3.xml
--rw-r--r--   0 root         (0) root         (0)  5928344 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/newdata/Model_3_Scenario_3.xml
--rw-r--r--   0 root         (0) root         (0)    15777 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/rob.obj
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.911340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/
--rw-r--r--   0 root         (0) root         (0)   918435 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Contact model library.pptx
--rw-r--r--   0 root         (0) root         (0)   423089 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_1_Scenario_1.txt
--rw-r--r--   0 root         (0) root         (0)   423090 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_1_Scenario_2.txt
--rw-r--r--   0 root         (0) root         (0)   369223 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_1_Scenario_3.txt
--rw-r--r--   0 root         (0) root         (0)   204754 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_2_Scenario_1.txt
--rw-r--r--   0 root         (0) root         (0)   204752 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_2_Scenario_2.txt
--rw-r--r--   0 root         (0) root         (0)  1612855 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_2_Scenario_3.txt
--rw-r--r--   0 root         (0) root         (0)   852437 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_3_Scenario_1.txt
--rw-r--r--   0 root         (0) root         (0)   852436 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_3_Scenario_2.txt
--rw-r--r--   0 root         (0) root         (0)  5910440 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/fcl_resources/scenario-1-2-3/Model_3_Scenario_3.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.915340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/geometry/
--rw-r--r--   0 root         (0) root         (0)       24 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/geometry/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.915340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/geometry/shape/
--rw-r--r--   0 root         (0) root         (0)      158 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/geometry/shape/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6185 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/geometry/shape/test_capsule.cpp
--rw-r--r--   0 root         (0) root         (0)    19456 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/geometry/shape/test_convex.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.915340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.915340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/cmake/
--rw-r--r--   0 root         (0) root         (0)     9548 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/cmake/internal_utils.cmake
--rw-r--r--   0 root         (0) root         (0)     1700 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/gtest-1.7.0.diff
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.783343 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.915340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/
--rw-r--r--   0 root         (0) root         (0)    11523 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-death-test.h
--rw-r--r--   0 root         (0) root         (0)     9186 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-message.h
--rw-r--r--   0 root         (0) root         (0)    75864 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-param-test.h
--rw-r--r--   0 root         (0) root         (0)    18796 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-param-test.h.pump
--rw-r--r--   0 root         (0) root         (0)    31659 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-printers.h
--rw-r--r--   0 root         (0) root         (0)     9952 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-spi.h
--rw-r--r--   0 root         (0) root         (0)     6509 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-test-part.h
--rw-r--r--   0 root         (0) root         (0)    10292 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-typed-test.h
--rw-r--r--   0 root         (0) root         (0)    88434 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest.h
--rw-r--r--   0 root         (0) root         (0)    15145 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 root         (0) root         (0)     2324 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest_prod.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/
--rw-r--r--   0 root         (0) root         (0)    13429 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 root         (0) root         (0)     9603 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 root         (0) root         (0)    44145 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 root         (0) root         (0)     8101 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-linked_ptr.h
--rw-r--r--   0 root         (0) root         (0)   192176 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-param-util-generated.h
--rw-r--r--   0 root         (0) root         (0)     9416 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-param-util-generated.h.pump
--rw-r--r--   0 root         (0) root         (0)    24191 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 root         (0) root         (0)    68846 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-port.h
--rw-r--r--   0 root         (0) root         (0)     6968 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-string.h
--rw-r--r--   0 root         (0) root         (0)    28223 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-tuple.h
--rw-r--r--   0 root         (0) root         (0)     9226 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-tuple.h.pump
--rw-r--r--   0 root         (0) root         (0)   185666 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-type-util.h
--rw-r--r--   0 root         (0) root         (0)     9317 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/internal/gtest-type-util.h.pump
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/
--rw-r--r--   0 root         (0) root         (0)     2166 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-all.cc
--rw-r--r--   0 root         (0) root         (0)    50953 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-death-test.cc
--rw-r--r--   0 root         (0) root         (0)    14242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-filepath.cc
--rw-r--r--   0 root         (0) root         (0)    46465 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-internal-inl.h
--rw-r--r--   0 root         (0) root         (0)    27470 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-port.cc
--rw-r--r--   0 root         (0) root         (0)    12279 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-printers.cc
--rw-r--r--   0 root         (0) root         (0)     4163 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-test-part.cc
--rw-r--r--   0 root         (0) root         (0)     3766 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest-typed-test.cc
--rw-r--r--   0 root         (0) root         (0)   184196 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest.cc
--rw-r--r--   0 root         (0) root         (0)     1769 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/src/gtest_main.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/libsvm/
--rw-r--r--   0 root         (0) root         (0)    74873 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/libsvm/svm.cpp
--rw-r--r--   0 root         (0) root         (0)     5355 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/libsvm/svm.h
--rw-r--r--   0 root         (0) root         (0)     6939 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/libsvm_classifier.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/
--rw-r--r--   0 root         (0) root         (0)       88 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/convexity_based_algorithm/
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/convexity_based_algorithm/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    65958 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/convexity_based_algorithm/test_gjk_libccd-inl_epa.cpp
--rw-r--r--   0 root         (0) root         (0)    23621 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/convexity_based_algorithm/test_gjk_libccd-inl_extractClosestPoints.cpp
--rw-r--r--   0 root         (0) root         (0)    13789 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/convexity_based_algorithm/test_gjk_libccd-inl_gjk_doSimplex2.cpp
--rw-r--r--   0 root         (0) root         (0)    20610 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/convexity_based_algorithm/test_gjk_libccd-inl_signed_distance.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/primitive_shape_algorithm/
--rw-r--r--   0 root         (0) root         (0)      154 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/primitive_shape_algorithm/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    31022 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/primitive_shape_algorithm/test_sphere_box.cpp
--rw-r--r--   0 root         (0) root         (0)    39404 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/narrowphase/detail/primitive_shape_algorithm/test_sphere_cylinder.cpp
--rw-r--r--   0 root         (0) root         (0)     3983 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_auto_diff.cpp
--rw-r--r--   0 root         (0) root         (0)    20612 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_box_box.cpp
--rw-r--r--   0 root         (0) root         (0)    21028 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_broadphase_collision_1.cpp
--rw-r--r--   0 root         (0) root         (0)    14652 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_broadphase_collision_2.cpp
--rw-r--r--   0 root         (0) root         (0)    24428 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_broadphase_distance.cpp
--rw-r--r--   0 root         (0) root         (0)     6817 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_bvh_models.cpp
--rw-r--r--   0 root         (0) root         (0)     5214 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_capsule_box_1.cpp
--rw-r--r--   0 root         (0) root         (0)     4032 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_capsule_box_2.cpp
--rw-r--r--   0 root         (0) root         (0)    30827 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_capsule_capsule.cpp
--rw-r--r--   0 root         (0) root         (0)    45549 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_collision.cpp
--rw-r--r--   0 root         (0) root         (0)     4870 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_constant_eps.cpp
--rw-r--r--   0 root         (0) root         (0)     4008 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_cylinder_half_space.cpp
--rw-r--r--   0 root         (0) root         (0)    25948 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_distance.cpp
--rw-r--r--   0 root         (0) root         (0)    16808 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_frontlist.cpp
--rw-r--r--   0 root         (0) root         (0)     3856 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_general.cpp
--rw-r--r--   0 root         (0) root         (0)    11787 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_generate_bvh_model_deferred_finalize.cpp
--rwxr-xr-x   0 root         (0) root         (0)   202198 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_geometric_shapes.cpp
--rw-r--r--   0 root         (0) root         (0)     4493 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_math.cpp
--rw-r--r--   0 root         (0) root         (0)    13227 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_octomap_collision.cpp
--rw-r--r--   0 root         (0) root         (0)     8195 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_octomap_cost.cpp
--rw-r--r--   0 root         (0) root         (0)    10547 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_octomap_distance.cpp
--rw-r--r--   0 root         (0) root         (0)     2837 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_profiler.cpp
--rw-r--r--   0 root         (0) root         (0)   112263 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_shape_mesh_consistency.cpp
--rw-r--r--   0 root         (0) root         (0)    24734 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_signed_distance.cpp
--rw-r--r--   0 root         (0) root         (0)    14968 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_simple.cpp
--rw-r--r--   0 root         (0) root         (0)    10263 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_sphere_box.cpp
--rw-r--r--   0 root         (0) root         (0)     9051 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_sphere_capsule.cpp
--rw-r--r--   0 root         (0) root         (0)    10572 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_sphere_cylinder.cpp
--rw-r--r--   0 root         (0) root         (0)     8828 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_sphere_sphere.cpp
--rw-r--r--   0 root         (0) root         (0)     6054 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_utility.cpp
--rw-r--r--   0 root         (0) root         (0)    20884 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/fcl/test/test_fcl_utility.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.919340 commonroad-drivability-checker-2022.2.1/third_party/gpc/
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-25 09:09:15.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/.git
--rw-r--r--   0 root         (0) root         (0)    70585 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/GPC-README.pdf
--rw-r--r--   0 root         (0) root         (0)     1127 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1053 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/README.md
--rw-r--r--   0 root         (0) root         (0)     4784 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/VERSIONS.TXT
--rw-r--r--   0 root         (0) root         (0)    75080 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/gpc.c
--rw-r--r--   0 root         (0) root         (0)     4905 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/gpc/gpc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/
--rw-r--r--   0 root         (0) root         (0)       46 2022-11-25 09:09:16.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/.git
--rw-r--r--   0 root         (0) root         (0)      149 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/.gitignore
--rw-r--r--   0 root         (0) root         (0)      581 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     2070 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/BSD-LICENSE
--rw-r--r--   0 root         (0) root         (0)     2204 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/Makefile.am
--rw-r--r--   0 root         (0) root         (0)     9769 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/README.md
--rwxr-xr-x   0 root         (0) root         (0)       87 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/bootstrap
--rw-r--r--   0 root         (0) root         (0)      401 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/ccd-config.cmake.in
--rw-r--r--   0 root         (0) root         (0)      382 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/ccd.pc.in
--rw-r--r--   0 root         (0) root         (0)     1304 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/configure.ac
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/
--rw-r--r--   0 root         (0) root         (0)     1231 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7606 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/_build/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/_build/.dir
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/_static/.dir
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/_templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/_templates/.dir
--rw-r--r--   0 root         (0) root         (0)     2720 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/compile-and-install.rst
--rw-r--r--   0 root         (0) root         (0)     9814 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     6269 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/examples.rst
--rw-r--r--   0 root         (0) root         (0)      397 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)       88 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/doc/reference.rst
--rwxr-xr-x   0 root         (0) root         (0)      636 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/make-release.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2180 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2353 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/Makefile
--rw-r--r--   0 root         (0) root         (0)      319 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/Makefile.am
--rw-r--r--   0 root         (0) root         (0)     1928 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/Makefile.include
--rw-r--r--   0 root         (0) root         (0)     1349 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/alloc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.923339 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/
--rw-r--r--   0 root         (0) root         (0)     5287 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/ccd.h
--rw-r--r--   0 root         (0) root         (0)      620 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/ccd_export.h
--rw-r--r--   0 root         (0) root         (0)     1672 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/compiler.h
--rw-r--r--   0 root         (0) root         (0)      130 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/config.h.cmake.in
--rw-r--r--   0 root         (0) root         (0)      166 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/config.h.m4
--rw-r--r--   0 root         (0) root         (0)     5621 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/quat.h
--rw-r--r--   0 root         (0) root         (0)     8187 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd/vec3.h
--rw-r--r--   0 root         (0) root         (0)    31674 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/ccd.c
--rw-r--r--   0 root         (0) root         (0)     1713 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/dbg.h
--rw-r--r--   0 root         (0) root         (0)     3750 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/list.h
--rw-r--r--   0 root         (0) root         (0)    18667 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/mpr.c
--rw-r--r--   0 root         (0) root         (0)     7476 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/polytope.c
--rw-r--r--   0 root         (0) root         (0)     8569 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/polytope.h
--rw-r--r--   0 root         (0) root         (0)     2751 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/simplex.h
--rw-r--r--   0 root         (0) root         (0)      928 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/support.c
--rw-r--r--   0 root         (0) root         (0)     1438 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/support.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.927339 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/
--rw-r--r--   0 root         (0) root         (0)       52 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/.gitignore
--rw-r--r--   0 root         (0) root         (0)      847 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1467 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/Makefile
--rw-r--r--   0 root         (0) root         (0)      595 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/Makefile.am
--rw-r--r--   0 root         (0) root         (0)     6499 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/bench.c
--rw-r--r--   0 root         (0) root         (0)     6691 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/bench2.c
--rw-r--r--   0 root         (0) root         (0)    11212 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/boxbox.c
--rw-r--r--   0 root         (0) root         (0)      522 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/boxbox.h
--rw-r--r--   0 root         (0) root         (0)     4600 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/boxcyl.c
--rw-r--r--   0 root         (0) root         (0)      225 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/boxcyl.h
--rw-r--r--   0 root         (0) root         (0)     5345 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/common.c
--rw-r--r--   0 root         (0) root         (0)      438 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.927339 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/.dir
--rw-r--r--   0 root         (0) root         (0)       23 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/.gitignore
--rw-r--r--   0 root         (0) root         (0)      470 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    35147 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/COPYING
--rw-r--r--   0 root         (0) root         (0)     7639 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      853 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/Makefile
--rw-r--r--   0 root         (0) root         (0)       93 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/Makefile.am
--rwxr-xr-x   0 root         (0) root         (0)    13205 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/check-regressions
--rw-r--r--   0 root         (0) root         (0)    10691 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/cu.c
--rw-r--r--   0 root         (0) root         (0)     3902 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/cu.h
--rwxr-xr-x   0 root         (0) root         (0)      274 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cu/latest.sh
--rw-r--r--   0 root         (0) root         (0)     3967 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cylcyl.c
--rw-r--r--   0 root         (0) root         (0)      435 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/cylcyl.h
--rw-r--r--   0 root         (0) root         (0)      637 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/main.c
--rw-r--r--   0 root         (0) root         (0)    12589 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/mpr_boxbox.c
--rw-r--r--   0 root         (0) root         (0)      469 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/mpr_boxbox.h
--rw-r--r--   0 root         (0) root         (0)     4730 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/mpr_boxcyl.c
--rw-r--r--   0 root         (0) root         (0)      242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/mpr_boxcyl.h
--rw-r--r--   0 root         (0) root         (0)     4189 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/mpr_cylcyl.c
--rw-r--r--   0 root         (0) root         (0)      364 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/mpr_cylcyl.h
--rw-r--r--   0 root         (0) root         (0)    12558 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/polytope.c
--rw-r--r--   0 root         (0) root         (0)      334 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/polytope.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.931339 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/.dir
--rw-r--r--   0 root         (0) root         (0)       63 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSBoxBox.err
--rw-r--r--   0 root         (0) root         (0)     1402 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSBoxBox.out
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSBoxCyl.err
--rw-r--r--   0 root         (0) root         (0)      943 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSBoxCyl.out
--rw-r--r--   0 root         (0) root         (0)       33 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSCylCyl.err
--rw-r--r--   0 root         (0) root         (0)      716 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSCylCyl.out
--rw-r--r--   0 root         (0) root         (0)       63 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSMPRBoxBox.err
--rw-r--r--   0 root         (0) root         (0)     1640 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSMPRBoxBox.out
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSMPRBoxCyl.err
--rw-r--r--   0 root         (0) root         (0)      945 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSMPRBoxCyl.out
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSMPRCylCyl.err
--rw-r--r--   0 root         (0) root         (0)      714 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSMPRCylCyl.out
--rw-r--r--   0 root         (0) root         (0)     1725 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSPt.err
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSPt.out
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSSphereSphere.err
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSSphereSphere.out
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSVec3.err
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/regressions/TSVec3.out
--rw-r--r--   0 root         (0) root         (0)     1665 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/spheresphere.c
--rw-r--r--   0 root         (0) root         (0)      446 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/spheresphere.h
--rw-r--r--   0 root         (0) root         (0)     2636 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/support.c
--rw-r--r--   0 root         (0) root         (0)     2514 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/support.h
--rw-r--r--   0 root         (0) root         (0)     8457 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/vec3.c
--rw-r--r--   0 root         (0) root         (0)      328 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/testsuites/vec3.h
--rw-r--r--   0 root         (0) root         (0)     8969 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/libccd/src/vec3.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.931339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/
--rw-r--r--   0 root         (0) root         (0)     2177 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.783343 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.783343 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.935339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/
--rw-r--r--   0 root         (0) root         (0)     5353 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/abstract_creator.hpp
--rw-r--r--   0 root         (0) root         (0)    26130 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/algo.hpp
--rw-r--r--   0 root         (0) root         (0)     5115 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/algo.tpp
--rw-r--r--   0 root         (0) root         (0)     6644 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/classload.hpp
--rw-r--r--   0 root         (0) root         (0)     2315 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/classload.tpp
--rw-r--r--   0 root         (0) root         (0)    14508 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/client_api.hpp
--rw-r--r--   0 root         (0) root         (0)     3141 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/exception.hpp
--rw-r--r--   0 root         (0) root         (0)     1836 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/export.hpp
--rw-r--r--   0 root         (0) root         (0)    18017 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/factory.hpp
--rw-r--r--   0 root         (0) root         (0)     3793 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/factory_reg.hpp
--rw-r--r--   0 root         (0) root         (0)    33111 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/functional.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.935339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/
--rw-r--r--   0 root         (0) root         (0)     5249 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/FlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     3808 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     6997 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/compact_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)    36720 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_format.hpp
--rw-r--r--   0 root         (0) root         (0)    24583 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_io.hpp
--rw-r--r--   0 root         (0) root         (0)    15239 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/expat_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     5806 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     7036 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     7100 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/parens_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     5288 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/reg_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     7979 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/serializers.hpp
--rw-r--r--   0 root         (0) root         (0)     3822 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     7894 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)    14116 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/strtool.hpp
--rw-r--r--   0 root         (0) root         (0)     3808 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     5763 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     5513 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/micro_api.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.935339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/nodeutil/
--rw-r--r--   0 root         (0) root         (0)     7965 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/nodeutil/node_tree.hpp
--rw-r--r--   0 root         (0) root         (0)     8419 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/phoenix.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.935339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/
--rw-r--r--   0 root         (0) root         (0)     6998 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/path_finder.hpp
--rw-r--r--   0 root         (0) root         (0)     4297 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin.hpp
--rw-r--r--   0 root         (0) root         (0)      821 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin_config.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.935339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/
--rw-r--r--   0 root         (0) root         (0)    15091 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.hpp
--rw-r--r--   0 root         (0) root         (0)     7474 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.tpp
--rw-r--r--   0 root         (0) root         (0)    26710 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.hpp
--rw-r--r--   0 root         (0) root         (0)    12955 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.tpp
--rw-r--r--   0 root         (0) root         (0)     1397 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/path_finder_s11n.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.939339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/
--rw-r--r--   0 root         (0) root         (0)      311 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/bool.hpp
--rw-r--r--   0 root         (0) root         (0)      311 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/char.hpp
--rw-r--r--   0 root         (0) root         (0)      321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/double.hpp
--rw-r--r--   0 root         (0) root         (0)      316 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/float.hpp
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/int.hpp
--rw-r--r--   0 root         (0) root         (0)      311 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/long.hpp
--rw-r--r--   0 root         (0) root         (0)      341 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/long_double.hpp
--rw-r--r--   0 root         (0) root         (0)      540 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/size_t.hpp
--rw-r--r--   0 root         (0) root         (0)      326 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/string.hpp
--rw-r--r--   0 root         (0) root         (0)      317 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/uint.hpp
--rw-r--r--   0 root         (0) root         (0)      323 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/ulong.hpp
--rw-r--r--   0 root         (0) root         (0)     1767 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_list_specializations.hpp
--rw-r--r--   0 root         (0) root         (0)     2470 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_map_specializations.hpp
--rw-r--r--   0 root         (0) root         (0)     3583 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_node_type.hpp
--rw-r--r--   0 root         (0) root         (0)     3127 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp
--rw-r--r--   0 root         (0) root         (0)     3408 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp
--rw-r--r--   0 root         (0) root         (0)     3363 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template3.hpp
--rw-r--r--   0 root         (0) root         (0)     3517 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template4.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.939339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/
--rw-r--r--   0 root         (0) root         (0)      316 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/deque.hpp
--rw-r--r--   0 root         (0) root         (0)      312 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/list.hpp
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/map.hpp
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/multimap.hpp
--rw-r--r--   0 root         (0) root         (0)     1331 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/multiset.hpp
--rw-r--r--   0 root         (0) root         (0)     1127 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/pair.hpp
--rw-r--r--   0 root         (0) root         (0)     1342 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/set.hpp
--rw-r--r--   0 root         (0) root         (0)     6690 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/valarray.hpp
--rw-r--r--   0 root         (0) root         (0)      321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/vector.hpp
--rw-r--r--   0 root         (0) root         (0)     6410 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/reg_s11n_traits.hpp
--rw-r--r--   0 root         (0) root         (0)     6751 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n.hpp
--rw-r--r--   0 root         (0) root         (0)     2091 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n_config.hpp
--rw-r--r--   0 root         (0) root         (0)     4798 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n_debuggering_macros.hpp
--rw-r--r--   0 root         (0) root         (0)     7452 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n_node.hpp
--rw-r--r--   0 root         (0) root         (0)    24061 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11nlite.hpp
--rw-r--r--   0 root         (0) root         (0)    18758 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/serialize.hpp
--rw-r--r--   0 root         (0) root         (0)     7697 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/serialize.tpp
--rw-r--r--   0 root         (0) root         (0)     3188 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/simple_config.hpp
--rw-r--r--   0 root         (0) root         (0)     1831 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/tags.hpp
--rw-r--r--   0 root         (0) root         (0)    16445 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/traits.hpp
--rw-r--r--   0 root         (0) root         (0)     2449 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/type_traits.hpp
--rw-r--r--   0 root         (0) root         (0)    16096 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/variant.hpp
--rw-r--r--   0 root         (0) root         (0)       64 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/notes.txt
--rw-r--r--   0 root         (0) root         (0)      140 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/s11nConfig.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.943339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/
--rw-r--r--   0 root         (0) root         (0)     6944 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/Makefile
--rw-r--r--   0 root         (0) root         (0)     4483 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/argv_parser.cpp
--rw-r--r--   0 root         (0) root         (0)      891 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/argv_parser.hpp
--rw-r--r--   0 root         (0) root         (0)    37640 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/compact.flex.cpp
--rw-r--r--   0 root         (0) root         (0)      606 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/compact_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)     2477 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/data_node_io.cpp
--rw-r--r--   0 root         (0) root         (0)     2831 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/exception.cpp
--rw-r--r--   0 root         (0) root         (0)     1625 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/expat_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)     1836 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/export.hpp
--rw-r--r--   0 root         (0) root         (0)    49935 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funtxt.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     1982 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funtxt_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)    39725 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funxml.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     1707 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funxml_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)      239 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/in.sxml
--rw-r--r--   0 root         (0) root         (0)      240 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/in.wes
--rw-r--r--   0 root         (0) root         (0)      416 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/in.xml
--rw-r--r--   0 root         (0) root         (0)    12038 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/main.cpp
--rw-r--r--   0 root         (0) root         (0)    49900 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/parens.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     2483 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/parens_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)     7377 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/path_finder.cpp
--rw-r--r--   0 root         (0) root         (0)     1337 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.cpp
--rw-r--r--   0 root         (0) root         (0)     2619 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.dl.cpp
--rw-r--r--   0 root         (0) root         (0)      784 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.noop.cpp
--rw-r--r--   0 root         (0) root         (0)     1645 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.win32.cpp
--rw-r--r--   0 root         (0) root         (0)     1133 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/s11n.cpp
--rw-r--r--   0 root         (0) root         (0)     4321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/s11n_node.cpp
--rw-r--r--   0 root         (0) root         (0)     5530 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/s11nlite.cpp
--rw-r--r--   0 root         (0) root         (0)    65103 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/simplexml.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     1878 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/simplexml_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)    14302 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/strtool.cpp
--rw-r--r--   0 root         (0) root         (0)    42559 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/wesnoth.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     2139 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/wesnoth_serializer.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.943339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/
--rw-r--r--   0 root         (0) root         (0)     5353 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/abstract_creator.hpp
--rw-r--r--   0 root         (0) root         (0)    24256 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.hpp
--rw-r--r--   0 root         (0) root         (0)     4225 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.tpp
--rw-r--r--   0 root         (0) root         (0)     6605 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.hpp
--rw-r--r--   0 root         (0) root         (0)     2293 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.tpp
--rw-r--r--   0 root         (0) root         (0)    14420 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/client_api.hpp
--rw-r--r--   0 root         (0) root         (0)     1917 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/exception.hpp
--rw-r--r--   0 root         (0) root         (0)      928 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/export.hpp
--rw-r--r--   0 root         (0) root         (0)    18017 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/factory.hpp
--rw-r--r--   0 root         (0) root         (0)     3695 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/factory_reg.hpp
--rw-r--r--   0 root         (0) root         (0)    32992 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/functional.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.947339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/
--rw-r--r--   0 root         (0) root         (0)     5249 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/FlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     3808 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     6405 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)    36761 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_format.hpp
--rw-r--r--   0 root         (0) root         (0)    24423 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_io.hpp
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     5698 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     6910 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     7110 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     5288 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/reg_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     7979 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/serializers.hpp
--rw-r--r--   0 root         (0) root         (0)     3822 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     7885 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)    14091 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/strtool.hpp
--rw-r--r--   0 root         (0) root         (0)     3808 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp
--rw-r--r--   0 root         (0) root         (0)     5782 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_serializer.hpp
--rw-r--r--   0 root         (0) root         (0)     5513 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/micro_api.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.947339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/nodeutil/
--rw-r--r--   0 root         (0) root         (0)     7965 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/nodeutil/node_tree.hpp
--rw-r--r--   0 root         (0) root         (0)     8419 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/phoenix.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.947339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/
--rw-r--r--   0 root         (0) root         (0)     6978 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/path_finder.hpp
--rw-r--r--   0 root         (0) root         (0)     3388 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin.hpp
--rw-r--r--   0 root         (0) root         (0)      821 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin_config.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.947339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/
--rw-r--r--   0 root         (0) root         (0)    15091 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.hpp
--rw-r--r--   0 root         (0) root         (0)     7461 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.tpp
--rw-r--r--   0 root         (0) root         (0)    26710 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.hpp
--rw-r--r--   0 root         (0) root         (0)    12879 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.tpp
--rw-r--r--   0 root         (0) root         (0)     1397 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/path_finder_s11n.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.947339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/
--rw-r--r--   0 root         (0) root         (0)      311 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/bool.hpp
--rw-r--r--   0 root         (0) root         (0)      311 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/char.hpp
--rw-r--r--   0 root         (0) root         (0)      321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/double.hpp
--rw-r--r--   0 root         (0) root         (0)      316 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/float.hpp
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/int.hpp
--rw-r--r--   0 root         (0) root         (0)      311 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/long.hpp
--rw-r--r--   0 root         (0) root         (0)      341 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/long_double.hpp
--rw-r--r--   0 root         (0) root         (0)      321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/size_t.hpp
--rw-r--r--   0 root         (0) root         (0)      326 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/string.hpp
--rw-r--r--   0 root         (0) root         (0)      310 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/uint.hpp
--rw-r--r--   0 root         (0) root         (0)      323 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/ulong.hpp
--rw-r--r--   0 root         (0) root         (0)     1767 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_list_specializations.hpp
--rw-r--r--   0 root         (0) root         (0)     2470 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_map_specializations.hpp
--rw-r--r--   0 root         (0) root         (0)     3583 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_node_type.hpp
--rw-r--r--   0 root         (0) root         (0)     2492 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp
--rw-r--r--   0 root         (0) root         (0)     2607 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.947339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/
--rw-r--r--   0 root         (0) root         (0)      316 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/deque.hpp
--rw-r--r--   0 root         (0) root         (0)      312 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/list.hpp
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/map.hpp
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/multimap.hpp
--rw-r--r--   0 root         (0) root         (0)     1331 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/multiset.hpp
--rw-r--r--   0 root         (0) root         (0)     1127 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/pair.hpp
--rw-r--r--   0 root         (0) root         (0)     1316 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/set.hpp
--rw-r--r--   0 root         (0) root         (0)     6671 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/valarray.hpp
--rw-r--r--   0 root         (0) root         (0)      321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/vector.hpp
--rw-r--r--   0 root         (0) root         (0)     6326 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/reg_s11n_traits.hpp
--rw-r--r--   0 root         (0) root         (0)     6751 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n.hpp
--rw-r--r--   0 root         (0) root         (0)     2084 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_config.hpp
--rw-r--r--   0 root         (0) root         (0)     4556 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_debuggering_macros.hpp
--rw-r--r--   0 root         (0) root         (0)    10398 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_node.hpp
--rw-r--r--   0 root         (0) root         (0)    24317 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11nlite.hpp
--rw-r--r--   0 root         (0) root         (0)    18758 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.hpp
--rw-r--r--   0 root         (0) root         (0)     7707 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.tpp
--rw-r--r--   0 root         (0) root         (0)     3188 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/simple_config.hpp
--rw-r--r--   0 root         (0) root         (0)     1831 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/tags.hpp
--rw-r--r--   0 root         (0) root         (0)    17424 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/traits.hpp
--rw-r--r--   0 root         (0) root         (0)     2449 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/type_traits.hpp
--rw-r--r--   0 root         (0) root         (0)    15859 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/variant.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.951339 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/
--rw-r--r--   0 root         (0) root         (0)     4483 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/argv_parser.cpp
--rw-r--r--   0 root         (0) root         (0)      891 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/argv_parser.hpp
--rw-r--r--   0 root         (0) root         (0)    37690 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/compact.flex.cpp
--rw-r--r--   0 root         (0) root         (0)      606 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/compact_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)     2477 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/data_node_io.cpp
--rw-r--r--   0 root         (0) root         (0)      636 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/exception.cpp
--rw-r--r--   0 root         (0) root         (0)    49906 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funtxt.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     1982 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funtxt_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)    39716 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funxml.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     1707 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funxml_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)    12038 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/main.cpp
--rw-r--r--   0 root         (0) root         (0)    49869 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/parens.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     2483 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/parens_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)     7347 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/path_finder.cpp
--rw-r--r--   0 root         (0) root         (0)     1337 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/plugin.cpp
--rw-r--r--   0 root         (0) root         (0)     1645 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/plugin.win32.cpp
--rw-r--r--   0 root         (0) root         (0)     1133 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/s11n.cpp
--rw-r--r--   0 root         (0) root         (0)     4321 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/s11n_node.cpp
--rw-r--r--   0 root         (0) root         (0)     5029 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/s11nlite.cpp
--rw-r--r--   0 root         (0) root         (0)    65094 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/simplexml.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     1878 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/simplexml_serializer.cpp
--rw-r--r--   0 root         (0) root         (0)    14261 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/strtool.cpp
--rw-r--r--   0 root         (0) root         (0)    42529 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/wesnoth.flex.cpp
--rw-r--r--   0 root         (0) root         (0)     2139 2022-11-25 09:09:11.000000 commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/wesnoth_serializer.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.951339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/
--rw-r--r--   0 root         (0) root         (0)     1304 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.appveyor.yml
--rw-r--r--   0 root         (0) root         (0)      523 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.clang-format
--rw-r--r--   0 root         (0) root         (0)      242 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.clang-tidy
--rw-r--r--   0 root         (0) root         (0)     2196 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.cmake-format.yaml
--rw-r--r--   0 root         (0) root         (0)       48 2022-11-25 09:09:22.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.git
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.955339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/
--rw-r--r--   0 root         (0) root         (0)    14415 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.955339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     1270 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      669 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 root         (0) root         (0)     1180 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 root         (0) root         (0)      559 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      116 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/labeler.yml
--rw-r--r--   0 root         (0) root         (0)       50 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/labeler_merged.yml
--rw-r--r--   0 root         (0) root         (0)      404 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.955339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)    24549 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     2117 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 root         (0) root         (0)     1090 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/workflows/format.yml
--rw-r--r--   0 root         (0) root         (0)      333 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 root         (0) root         (0)     2497 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2460 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)       62 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/.readthedocs.yml
--rw-r--r--   0 root         (0) root         (0)    10364 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8064 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.955339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/
--rw-r--r--   0 root         (0) root         (0)      705 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/Doxyfile
--rw-r--r--   0 root         (0) root         (0)     7417 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.955339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/_static/
--rw-r--r--   0 root         (0) root         (0)      254 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.959339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.959339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/
--rw-r--r--   0 root         (0) root         (0)     3937 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 root         (0) root         (0)     3398 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 root         (0) root         (0)    14288 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 root         (0) root         (0)     3889 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 root         (0) root         (0)     1556 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 root         (0) root         (0)    11680 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 root         (0) root         (0)     9703 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 root         (0) root         (0)     9372 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 root         (0) root         (0)    45877 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 root         (0) root         (0)     8420 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 root         (0) root         (0)    14171 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 root         (0) root         (0)    25078 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 root         (0) root         (0)    12444 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.959339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 root         (0) root         (0)      278 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 root         (0) root         (0)    16538 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 root         (0) root         (0)     7878 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 root         (0) root         (0)     5125 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 root         (0) root         (0)     6366 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 root         (0) root         (0)     9369 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/basics.rst
--rw-r--r--   0 root         (0) root         (0)     2974 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     3168 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/benchmark.rst
--rw-r--r--   0 root         (0) root         (0)    73677 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)    16122 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/classes.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.959339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/cmake/
--rw-r--r--   0 root         (0) root         (0)      273 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/cmake/index.rst
--rw-r--r--   0 root         (0) root         (0)    25511 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/compiling.rst
--rw-r--r--   0 root         (0) root         (0)    12095 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    14592 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      613 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     3277 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/installing.rst
--rw-r--r--   0 root         (0) root         (0)     3062 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/limitations.rst
--rw-r--r--   0 root         (0) root         (0)    58510 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 root         (0) root         (0)    44653 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 root         (0) root         (0)    87708 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 root         (0) root         (0)    41121 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 root         (0) root         (0)    85853 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 root         (0) root         (0)     2113 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/reference.rst
--rw-r--r--   0 root         (0) root         (0)     4028 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/release.rst
--rw-r--r--   0 root         (0) root         (0)      168 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/requirements.txt
--rw-r--r--   0 root         (0) root         (0)    21940 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.959339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/
--rw-r--r--   0 root         (0) root         (0)    21412 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 root         (0) root         (0)     6118 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 root         (0) root         (0)    95557 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 root         (0) root         (0)     8185 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 root         (0) root         (0)      120 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/common.h
--rw-r--r--   0 root         (0) root         (0)     2037 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.959339 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/
--rw-r--r--   0 root         (0) root         (0)    27823 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 root         (0) root         (0)    40452 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 root         (0) root         (0)     3602 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 root         (0) root         (0)    16397 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 root         (0) root         (0)    16375 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 root         (0) root         (0)     1486 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 root         (0) root         (0)    29086 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 root         (0) root         (0)     7843 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 root         (0) root         (0)     5079 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 root         (0) root         (0)     3709 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 root         (0) root         (0)     6084 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 root         (0) root         (0)    69310 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 root         (0) root         (0)     9085 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 root         (0) root         (0)     2049 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/options.h
--rw-r--r--   0 root         (0) root         (0)   111558 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 root         (0) root         (0)    66118 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 root         (0) root         (0)    14136 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 root         (0) root         (0)    23912 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.963338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/
--rw-r--r--   0 root         (0) root         (0)      217 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1158 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/__main__.py
--rw-r--r--   0 root         (0) root         (0)      202 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/_version.py
--rw-r--r--   0 root         (0) root         (0)      137 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/_version.pyi
--rw-r--r--   0 root         (0) root         (0)      663 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/commands.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/py.typed
--rw-r--r--   0 root         (0) root         (0)    15110 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 root         (0) root         (0)     1899 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pybind11/setup_helpers.pyi
--rw-r--r--   0 root         (0) root         (0)      118 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2185 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3499 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/
--rw-r--r--   0 root         (0) root         (0)    15362 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4841 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11157 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/constructor_stats.h
--rw-r--r--   0 root         (0) root         (0)     1819 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 root         (0) root         (0)      376 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/extra_python_package/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 root         (0) root         (0)     7074 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/extra_setuptools/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 root         (0) root         (0)     2581 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 root         (0) root         (0)     2144 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/local_bindings.h
--rw-r--r--   0 root         (0) root         (0)     5389 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/object.h
--rw-r--r--   0 root         (0) root         (0)     5285 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 root         (0) root         (0)     3647 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 root         (0) root         (0)     2733 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 root         (0) root         (0)      626 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/pytest.ini
--rw-r--r--   0 root         (0) root         (0)      736 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      864 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_async.cpp
--rw-r--r--   0 root         (0) root         (0)      558 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_async.py
--rw-r--r--   0 root         (0) root         (0)     8048 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 root         (0) root         (0)     4946 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_buffers.py
--rw-r--r--   0 root         (0) root         (0)    13475 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 root         (0) root         (0)    17214 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 root         (0) root         (0)     3702 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 root         (0) root         (0)     5728 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_call_policies.py
--rw-r--r--   0 root         (0) root         (0)     6600 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 root         (0) root         (0)     4405 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     3406 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 root         (0) root         (0)     6276 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_chrono.py
--rw-r--r--   0 root         (0) root         (0)    21623 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_class.cpp
--rw-r--r--   0 root         (0) root         (0)    14273 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/
--rw-r--r--   0 root         (0) root         (0)     2639 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      656 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 root         (0) root         (0)     1175 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 root         (0) root         (0)     1259 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 root         (0) root         (0)     1653 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      152 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 root         (0) root         (0)     1357 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 root         (0) root         (0)     1126 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 root         (0) root         (0)     1333 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      166 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 root         (0) root         (0)     5346 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 root         (0) root         (0)     1522 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 root         (0) root         (0)     9629 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 root         (0) root         (0)     4645 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_copy_move.py
--rw-r--r--   0 root         (0) root         (0)     5513 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 root         (0) root         (0)     4015 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 root         (0) root         (0)     2514 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 root         (0) root         (0)     1630 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 root         (0) root         (0)    16867 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 root         (0) root         (0)    28282 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.971338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_embed/
--rw-r--r--   0 root         (0) root         (0)     1758 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      637 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 root         (0) root         (0)      554 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 root         (0) root         (0)    10209 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 root         (0) root         (0)      219 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 root         (0) root         (0)     2610 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_enum.cpp
--rw-r--r--   0 root         (0) root         (0)     7694 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_enum.py
--rw-r--r--   0 root         (0) root         (0)     2628 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_eval.cpp
--rw-r--r--   0 root         (0) root         (0)      768 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_eval.py
--rw-r--r--   0 root         (0) root         (0)      143 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_eval_call.py
--rw-r--r--   0 root         (0) root         (0)     7862 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 root         (0) root         (0)     6753 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    16562 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 root         (0) root         (0)    16637 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 root         (0) root         (0)     1760 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 root         (0) root         (0)     3128 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 root         (0) root         (0)     3381 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 root         (0) root         (0)     5799 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_iostream.py
--rw-r--r--   0 root         (0) root         (0)     6489 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 root         (0) root         (0)    10048 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 root         (0) root         (0)     4333 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)     8102 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 root         (0) root         (0)    19446 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 root         (0) root         (0)    17310 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 root         (0) root         (0)     3742 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_modules.cpp
--rw-r--r--   0 root         (0) root         (0)     2841 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_modules.py
--rw-r--r--   0 root         (0) root         (0)     8863 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 root         (0) root         (0)     9495 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 root         (0) root         (0)    17781 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 root         (0) root         (0)    18647 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 root         (0) root         (0)    17721 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 root         (0) root         (0)    13484 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 root         (0) root         (0)     3832 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 root         (0) root         (0)     9709 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 root         (0) root         (0)     2731 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 root         (0) root         (0)     1906 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 root         (0) root         (0)     8431 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 root         (0) root         (0)     4136 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 root         (0) root         (0)     4945 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 root         (0) root         (0)     1191 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_pickling.py
--rw-r--r--   0 root         (0) root         (0)    13347 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 root         (0) root         (0)    13720 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_pytypes.py
--rw-r--r--   0 root         (0) root         (0)    13120 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 root         (0) root         (0)     5966 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 root         (0) root         (0)    17913 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 root         (0) root         (0)     9620 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 root         (0) root         (0)    12793 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_stl.cpp
--rw-r--r--   0 root         (0) root         (0)     8557 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_stl.py
--rw-r--r--   0 root         (0) root         (0)     4403 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 root         (0) root         (0)     7182 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 root         (0) root         (0)     4458 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 root         (0) root         (0)      765 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_union.cpp
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_union.py
--rw-r--r--   0 root         (0) root         (0)    18454 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 root         (0) root         (0)    11646 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 root         (0) root         (0)     2558 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 root         (0) root         (0)     3103 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.975338 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/
--rw-r--r--   0 root         (0) root         (0)     2295 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 root         (0) root         (0)     3105 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 root         (0) root         (0)     9977 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 root         (0) root         (0)     1427 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/check-style.sh
--rw-r--r--   0 root         (0) root         (0)      952 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 root         (0) root         (0)     1121 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/libsize.py
--rwxr-xr-x   0 root         (0) root         (0)     1202 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/make_changelog.py
--rw-r--r--   0 root         (0) root         (0)    14003 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 root         (0) root         (0)     7010 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 root         (0) root         (0)     9172 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 root         (0) root         (0)     7276 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1822 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 root         (0) root         (0)      915 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.975338 commonroad-drivability-checker-2022.2.1/third_party/triangle/
--rw-r--r--   0 root         (0) root         (0)       48 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/.git
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.787343 commonroad-drivability-checker-2022.2.1/third_party/triangle/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.975338 commonroad-drivability-checker-2022.2.1/third_party/triangle/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1254 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/.github/workflows/wheels.yml
--rw-r--r--   0 root         (0) root         (0)       52 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/.gitignore
--rw-r--r--   0 root         (0) root         (0)      240 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     7652 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/LICENSE
--rw-r--r--   0 root         (0) root         (0)      986 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.975338 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/
--rw-r--r--   0 root         (0) root         (0)     1045 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/A.poly
--rw-r--r--   0 root         (0) root         (0)      252 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8727 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/README
--rw-r--r--   0 root         (0) root         (0)     4805 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/makefile
--rw-r--r--   0 root         (0) root         (0)   108795 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/showme.c
--rw-r--r--   0 root         (0) root         (0)   650886 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/triangle.c
--rw-r--r--   0 root         (0) root         (0)    21910 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/triangle.h
--rw-r--r--   0 root         (0) root         (0)    10300 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/c/tricall.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.975338 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/
--rw-r--r--   0 root         (0) root         (0)      265 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/API.rst
--rw-r--r--   0 root         (0) root         (0)      633 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/Makefile
--rw-r--r--   0 root         (0) root         (0)     2339 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1039 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/convex.rst
--rw-r--r--   0 root         (0) root         (0)     6092 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/data.rst
--rw-r--r--   0 root         (0) root         (0)     2542 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/definitions.rst
--rw-r--r--   0 root         (0) root         (0)     2194 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/delaunay.rst
--rw-r--r--   0 root         (0) root         (0)      599 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/examples.rst
--rw-r--r--   0 root         (0) root         (0)     1182 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      204 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/installing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.979338 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/
--rw-r--r--   0 root         (0) root         (0)      121 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/PSLG.py
--rw-r--r--   0 root         (0) root         (0)      254 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/api_convex_hull.py
--rw-r--r--   0 root         (0) root         (0)      252 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/api_delaunay.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/api_triangulate.py
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/api_voronoi.py
--rw-r--r--   0 root         (0) root         (0)      275 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/bndries.py
--rw-r--r--   0 root         (0) root         (0)      143 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/conforming_delaunay.py
--rw-r--r--   0 root         (0) root         (0)      153 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/conforming_delaunay1.py
--rw-r--r--   0 root         (0) root         (0)      143 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/constrained_conforming_delaunay.py
--rw-r--r--   0 root         (0) root         (0)      153 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/constrained_conforming_delaunay1.py
--rw-r--r--   0 root         (0) root         (0)      148 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/constrained_delaunay.py
--rw-r--r--   0 root         (0) root         (0)      147 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/constrained_delaunay1.py
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/convex_hull.py
--rw-r--r--   0 root         (0) root         (0)      140 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/delaunay.py
--rw-r--r--   0 root         (0) root         (0)      154 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/delaunay1.py
--rw-r--r--   0 root         (0) root         (0)      192 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex1.py
--rw-r--r--   0 root         (0) root         (0)      201 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex2.py
--rw-r--r--   0 root         (0) root         (0)      202 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex3.py
--rw-r--r--   0 root         (0) root         (0)      273 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex4.py
--rw-r--r--   0 root         (0) root         (0)      278 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex5.py
--rw-r--r--   0 root         (0) root         (0)      527 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex6.py
--rw-r--r--   0 root         (0) root         (0)      823 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/ex7.py
--rw-r--r--   0 root         (0) root         (0)      124 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/face.py
--rw-r--r--   0 root         (0) root         (0)      150 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/holes_cavities.py
--rw-r--r--   0 root         (0) root         (0)      413 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/quality.py
--rw-r--r--   0 root         (0) root         (0)      175 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/quality1.py
--rw-r--r--   0 root         (0) root         (0)      352 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/quality2.py
--rw-r--r--   0 root         (0) root         (0)      443 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/refine.py
--rw-r--r--   0 root         (0) root         (0)      159 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/refine1.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/refine2.py
--rw-r--r--   0 root         (0) root         (0)      325 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/voronoi.py
--rw-r--r--   0 root         (0) root         (0)      203 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/voronoi1.py
--rw-r--r--   0 root         (0) root         (0)      425 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/plot/voronoi3.py
--rw-r--r--   0 root         (0) root         (0)     1517 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/quality.rst
--rw-r--r--   0 root         (0) root         (0)     2746 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/refine.rst
--rw-r--r--   0 root         (0) root         (0)     1337 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/doc/voronoi.rst
--rw-r--r--   0 root         (0) root         (0)        6 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1040 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.979338 commonroad-drivability-checker-2022.2.1/third_party/triangle/tests/
--rw-r--r--   0 root         (0) root         (0)     1741 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/tests/test_triangle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.979338 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/
--rw-r--r--   0 root         (0) root         (0)      246 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/__init__.py
--rw-r--r--   0 root         (0) root         (0)   971030 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/core.c
--rw-r--r--   0 root         (0) root         (0)     5814 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/core.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 09:09:26.991338 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/
--rw-r--r--   0 root         (0) root         (0)      768 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/A.1.ele
--rw-r--r--   0 root         (0) root         (0)     2071 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/A.1.node
--rw-r--r--   0 root         (0) root         (0)      869 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/A.1.poly
--rw-r--r--   0 root         (0) root         (0)     1045 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/A.poly
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/bbox.1.area
--rw-r--r--   0 root         (0) root         (0)      342 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/bbox.1.ele
--rw-r--r--   0 root         (0) root         (0)      272 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/bbox.1.node
--rw-r--r--   0 root         (0) root         (0)      240 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.1.ele
--rw-r--r--   0 root         (0) root         (0)      190 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.1.node
--rw-r--r--   0 root         (0) root         (0)      282 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.1.poly
--rw-r--r--   0 root         (0) root         (0)     1597 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.2.ele
--rw-r--r--   0 root         (0) root         (0)     1312 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.2.node
--rw-r--r--   0 root         (0) root         (0)      559 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.2.poly
--rw-r--r--   0 root         (0) root         (0)     6324 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.3.ele
--rw-r--r--   0 root         (0) root         (0)     6107 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.3.node
--rw-r--r--   0 root         (0) root         (0)      965 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.3.poly
--rw-r--r--   0 root         (0) root         (0)    24851 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.4.ele
--rw-r--r--   0 root         (0) root         (0)    25313 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.4.node
--rw-r--r--   0 root         (0) root         (0)     1966 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.4.poly
--rw-r--r--   0 root         (0) root         (0)      639 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/box.poly
--rw-r--r--   0 root         (0) root         (0)      358 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/diamond_02_00009.1.ele
--rw-r--r--   0 root         (0) root         (0)      354 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/diamond_02_00009.1.node
--rw-r--r--   0 root         (0) root         (0)      338 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/diamond_02_00009.1.v.edge
--rw-r--r--   0 root         (0) root         (0)      530 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/diamond_02_00009.1.v.node
--rw-r--r--   0 root         (0) root         (0)      611 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/diamond_02_00009.node
--rw-r--r--   0 root         (0) root         (0)     4767 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/dots.1.v.edge
--rw-r--r--   0 root         (0) root         (0)     9497 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/dots.1.v.node
--rw-r--r--   0 root         (0) root         (0)     2493 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/dots.node
--rw-r--r--   0 root         (0) root         (0)     2502 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.1.ele
--rw-r--r--   0 root         (0) root         (0)     3607 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.1.node
--rw-r--r--   0 root         (0) root         (0)     2720 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.1.poly
--rw-r--r--   0 root         (0) root         (0)    23966 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.2.ele
--rw-r--r--   0 root         (0) root         (0)    26468 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.2.node
--rw-r--r--   0 root         (0) root         (0)     2733 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.2.poly
--rw-r--r--   0 root         (0) root         (0)     4893 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex.poly
--rw-r--r--   0 root         (0) root         (0)     1303 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.1.ele
--rw-r--r--   0 root         (0) root         (0)     1790 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.1.node
--rw-r--r--   0 root         (0) root         (0)     1425 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.1.poly
--rw-r--r--   0 root         (0) root         (0)     5967 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.2.ele
--rw-r--r--   0 root         (0) root         (0)     6716 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.2.node
--rw-r--r--   0 root         (0) root         (0)     1438 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.2.poly
--rw-r--r--   0 root         (0) root         (0)     3162 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex2.poly
--rw-r--r--   0 root         (0) root         (0)    24264 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex3.1.ele
--rw-r--r--   0 root         (0) root         (0)    25934 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex3.1.node
--rw-r--r--   0 root         (0) root         (0)     2731 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex3.1.poly
--rw-r--r--   0 root         (0) root         (0)      505 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex3.node
--rw-r--r--   0 root         (0) root         (0)     1848 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/double_hex3.poly
--rw-r--r--   0 root         (0) root         (0)      321 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/ell.ele
--rw-r--r--   0 root         (0) root         (0)      348 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/ell.node
--rw-r--r--   0 root         (0) root         (0)      946 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/face.1.ele
--rw-r--r--   0 root         (0) root         (0)      587 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/face.1.node
--rw-r--r--   0 root         (0) root         (0)      693 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/face.1.poly
--rw-r--r--   0 root         (0) root         (0)     1482 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/face.poly
--rw-r--r--   0 root         (0) root         (0)  1793579 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/greenland.ele
--rw-r--r--   0 root         (0) root         (0)  1659689 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/greenland.node
--rw-r--r--   0 root         (0) root         (0)    39207 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/la.1.ele
--rw-r--r--   0 root         (0) root         (0)    42764 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/la.1.node
--rw-r--r--   0 root         (0) root         (0)    13877 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/la.1.poly
--rw-r--r--   0 root         (0) root         (0)     9061 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/la.poly
--rw-r--r--   0 root         (0) root         (0)      415 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.1.ele
--rw-r--r--   0 root         (0) root         (0)      725 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.1.node
--rw-r--r--   0 root         (0) root         (0)      449 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.node
--rw-r--r--   0 root         (0) root         (0)      616 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.q.1.ele
--rw-r--r--   0 root         (0) root         (0)      983 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.q.1.node
--rw-r--r--   0 root         (0) root         (0)      920 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.r.1.ele
--rw-r--r--   0 root         (0) root         (0)     1338 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/spiral.r.1.node
--rw-r--r--   0 root         (0) root         (0)    37987 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/square_circle_hole.1.ele
--rw-r--r--   0 root         (0) root         (0)    38746 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/square_circle_hole.1.node
--rw-r--r--   0 root         (0) root         (0)    31610 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data/square_circle_hole.poly
--rw-r--r--   0 root         (0) root         (0)     6426 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/data.py
--rw-r--r--   0 root         (0) root         (0)     3738 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/plot.py
--rw-r--r--   0 root         (0) root         (0)     6239 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/tri.py
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-25 09:09:23.000000 commonroad-drivability-checker-2022.2.1/third_party/triangle/triangle/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.289599 commonroad-drivability-checker-2023.1/
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-07-21 20:30:00.289599 commonroad-drivability-checker-2023.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-21 20:29:59.000000 commonroad-drivability-checker-2023.1/commonroad_dc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-21 20:29:59.000000 commonroad-drivability-checker-2023.1/commonroad_dc/__pycache__/__version__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/boundary.py
+-rw-r--r--   0 root         (0) root         (0)    25688 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/construction.py
+-rw-r--r--   0 root         (0) root         (0)    14915 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/lanelet_bounds.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/rectangle_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/scenario_bounds.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/boundary/triangle_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/collision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/minkowski_sum.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/pycrcc_collision_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)     7188 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/collision/trajectory_queries/
+-rw-r--r--   0 root         (0) root         (0)    13816 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/trajectory_queries/trajectory_queries.py
+-rw-r--r--   0 root         (0) root         (0)    10833 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/trajectory_queries/trajectory_queries_specialized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/collision/visualization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/visualization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/collision/visualization/drawing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/costs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/costs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9908 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/costs/evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    12256 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/costs/partial_cost_functions.py
+-rw-r--r--   0 root         (0) root         (0)    34987 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/costs/route_matcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20312 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/feasibility_checker.py
+-rw-r--r--   0 root         (0) root         (0)    17321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/solution_checker.py
+-rw-r--r--   0 root         (0) root         (0)    38520 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/vehicle_dynamics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/commonroad_dc/geometry/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5177 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/geometry/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/geometry/lanelet_ccosy.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/commonroad_dc/geometry/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-07-21 20:29:59.000000 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    27310 2023-07-21 20:30:00.000000 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 20:29:59.000000 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 20:29:59.000000 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-21 20:30:00.000000 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 20:30:00.000000 commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/
+-rw-r--r--   0 root         (0) root         (0)     7648 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/Readme.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/cmake/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/cmake/DrivabilityCheckerConfig.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/collision/
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.253599 commonroad-drivability-checker-2023.1/cpp/collision/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/application.h
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/application_settings.h
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_checker.h
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_object.h
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_object_ex.h
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_object_types.h
+-rw-r--r--   0 root         (0) root         (0)      676 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/i_collision_checker.h
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/i_collision_checker_export.h
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/i_collision_container.h
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/i_collision_object_export.h
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/line_segment.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/detail/
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/detail/aabb.h
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/detail/obb.h
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/point.h
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/polygon.h
+-rwxr-xr-x   0 root         (0) root         (0)     2931 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/rectangle_aabb.h
+-rw-r--r--   0 root         (0) root         (0)     6271 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/rectangle_obb.h
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/shape.h
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/sphere.h
+-rw-r--r--   0 root         (0) root         (0)     2542 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/triangle.h
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.253599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/plugins/triangulation/
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/plugins/triangulation/triangulate.h
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/primitive_collision_checker.h
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/raytrace_primitive.h
+-rw-r--r--   0 root         (0) root         (0)      998 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/raytrace_utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.261599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/basic_types.h
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/broadphase_failure_cc_obj_export.h
+-rw-r--r--   0 root         (0) root         (0)      523 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/broadphase_failure_export.h
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/broadphase_failure_obj_obj_export.h
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/collision_checker_export.h
+-rw-r--r--   0 root         (0) root         (0)      555 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/collision_object_export_s11.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/point_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      198 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/polygon_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      232 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/rectangle_aabb_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/rectangle_obb_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/sphere_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/triangle_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/tv_object_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      187 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/export_structs/vertex_export_struct.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/final/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/final/collision_object_export_final.h
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/i_collision_checker_export.h
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/i_collision_object_export.h
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/point_export.h
+-rw-r--r--   0 root         (0) root         (0)      850 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/polygon_export.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/public/
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/public/serialize_public.h
+-rw-r--r--   0 root         (0) root         (0)      730 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/rectangle_aabb_export.h
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/rectangle_obb_export.h
+-rw-r--r--   0 root         (0) root         (0)      912 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/serialize.h
+-rw-r--r--   0 root         (0) root         (0)     3519 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/serialize_reg_impl.h
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/shape_export.h
+-rw-r--r--   0 root         (0) root         (0)      687 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/shape_group_export.h
+-rw-r--r--   0 root         (0) root         (0)      679 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/sphere_export.h
+-rw-r--r--   0 root         (0) root         (0)      693 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/triangle_export.h
+-rw-r--r--   0 root         (0) root         (0)      912 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/tv_object_export.h
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/vector2d_export.h
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/vector2d_export_streams.h
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/shape_group.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/declarations.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/common.h
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/common_impl.h
+-rw-r--r--   0 root         (0) root         (0)      449 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_box2d.h
+-rw-r--r--   0 root         (0) root         (0)    11002 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_box2d_inl.h
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_fcl.h
+-rw-r--r--   0 root         (0) root         (0)    14172 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_fcl_inl.h
+-rw-r--r--   0 root         (0) root         (0)      735 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid.h
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid_common.h
+-rw-r--r--   0 root         (0) root         (0)    16860 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid_inl.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_collision_object.h
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_collision_queries.h
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_entity_type.h
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_geometry_queries.h
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_helpers.h
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_object_internal.h
+-rwxr-xr-x   0 root         (0) root         (0)     5926 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_object_polygon.h
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/i_boost_collision_object.h
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/i_solver_entity_boost.h
+-rw-r--r--   0 root         (0) root         (0)      713 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost.h
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost_factory.h
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_queries.h
+-rw-r--r--   0 root         (0) root         (0)      780 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_requests.h
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_solver_fcl.h
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_solver_primitive.h
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_solvers.h
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/distance_queries.h
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/distance_requests.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_broadphase_manager_factory.h
+-rw-r--r--   0 root         (0) root         (0)     4622 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_checker.h
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object.h
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object_group.h
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_queries.h
+-rw-r--r--   0 root         (0) root         (0)    13152 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_requests.h
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_decl.h
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_queries.h
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_requests.h
+-rw-r--r--   0 root         (0) root         (0)      509 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_entity_type.h
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_helpers.h
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_transform.h
+-rw-r--r--   0 root         (0) root         (0)      907 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object.h
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object_group.h
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/i_solver_entity_fcl.h
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/performance_timers.h
+-rw-r--r--   0 root         (0) root         (0)      584 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl.h
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl_factory.h
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/geometry_queries.h
+-rwxr-xr-x   0 root         (0) root         (0)     4280 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/primitive_collision_queries.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.265599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/aabb_sat2d.h
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/obb_sat2d.h
+-rw-r--r--   0 root         (0) root         (0)      591 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/sat2d_checks.h
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/triangle_sat2d.h
+-rw-r--r--   0 root         (0) root         (0)     6058 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/trajectory_queries.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/broadphase_failure.h
+-rw-r--r--   0 root         (0) root         (0)     4610 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/broadphase_test.h
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/collision_tests.h
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/test_common.h
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/include/collision/time_variant_collision_object.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/
+-rw-r--r--   0 root         (0) root         (0)    11203 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/collision_checker.cc
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/collision_object.cc
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/collision_object_ex.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/detail/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/detail/aabb.cc
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/point.cc
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/polygon.cc
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/rectangle_aabb.cc
+-rw-r--r--   0 root         (0) root         (0)     4380 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/rectangle_obb.cc
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/shape.cc
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/sphere.cc
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/triangle.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.253599 commonroad-drivability-checker-2023.1/cpp/collision/src/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/plugins/triangulation/
+-rw-r--r--   0 root         (0) root         (0)    11865 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/plugins/triangulation/triangulate.cc
+-rw-r--r--   0 root         (0) root         (0)     2479 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/primitive_collision_checker.cc
+-rw-r--r--   0 root         (0) root         (0)     5984 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/raytrace_primitive.cc
+-rw-r--r--   0 root         (0) root         (0)     7973 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/raytrace_utils.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/final/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/final/collision_object_export_final.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/public/
+-rw-r--r--   0 root         (0) root         (0)     9623 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/public/serialize_public.cc
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize.cc
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_collision_checker.cc
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_container_cc_obj.cc
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_container_obj_obj.cc
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_point.cc
+-rw-r--r--   0 root         (0) root         (0)     3052 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_polygon.cc
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_rectangle_aabb.cc
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_rectangle_obb.cc
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_shape_group.cc
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_sphere.cc
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_triangle.cc
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_tv_object.cc
+-rw-r--r--   0 root         (0) root         (0)     6465 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/shape_group.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_collision_object.cc
+-rw-r--r--   0 root         (0) root         (0)     8762 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_collision_queries.cc
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_geometry_queries.cc
+-rwxr-xr-x   0 root         (0) root         (0)     4470 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_object_polygon.cc
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/solver_entity_boost.cc
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_queries.cc
+-rw-r--r--   0 root         (0) root         (0)    10782 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_solver_default.cc
+-rw-r--r--   0 root         (0) root         (0)    12712 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_solver_fcl.cc
+-rw-r--r--   0 root         (0) root         (0)    27974 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_solver_primitive.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/detail/
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/detail/collision_containers.cc
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/distance_queries.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_broadphase_manager_factories.cc
+-rw-r--r--   0 root         (0) root         (0)    22419 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_checker.cc
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_object.cc
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_object_group.cc
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_queries.cc
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_requests.cc
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_distance_queries.cc
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_distance_requests.cc
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_entity_factory.cc
+-rw-r--r--   0 root         (0) root         (0)     5535 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/performance_timers.cc
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/solver_entity_fcl.cc
+-rw-r--r--   0 root         (0) root         (0)     9569 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/geometry_queries.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/sat2d/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/sat2d/sat2d_checks.cc
+-rw-r--r--   0 root         (0) root         (0)    23711 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/trajectory_queries.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.253599 commonroad-drivability-checker-2023.1/cpp/collision/src/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.269599 commonroad-drivability-checker-2023.1/cpp/collision/src/tests/online_tests/
+-rw-r--r--   0 root         (0) root         (0)    32436 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/tests/online_tests/broadphase_test.cc
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/tests/online_tests/test_common.cc
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/collision/src/time_variant_collision_object.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/cpp/geometry/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/application_settings.h
+-rw-r--r--   0 root         (0) root         (0)    23785 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/curvilinear_coordinate_system.h
+-rw-r--r--   0 root         (0) root         (0)     7909 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/segment.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/basic_types.h
+-rw-r--r--   0 root         (0) root         (0)      989 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/curvilinear_coordinate_system_export.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/export_structs/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/export_structs/curvilinear_coordinate_system_export_struct.h
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/icurvilinear_coordinate_system_export.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/public/
+-rw-r--r--   0 root         (0) root         (0)      537 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/public/serialize_public.h
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/serialize.h
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/serialize_reg_impl.h
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/vector2d_export.h
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/vector2d_export_streams.h
+-rw-r--r--   0 root         (0) root         (0)     7359 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/src/
+-rw-r--r--   0 root         (0) root         (0)    57646 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/src/curvilinear_coordinate_system.cc
+-rw-r--r--   0 root         (0) root         (0)     7263 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/src/segment.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/src/serialize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/geometry/src/serialize/public/
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/src/serialize/public/serialize_public.cc
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/src/serialize/serialize_curvil_cs.cc
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/geometry/src/util.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/python_binding/
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/python_binding/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/python_binding/src/
+-rw-r--r--   0 root         (0) root         (0)    56533 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/python_binding/src/module_collision.cc
+-rw-r--r--   0 root         (0) root         (0)    20274 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/python_binding/src/module_geometry.cc
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/python_binding/src/py_bind.cc
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/python_binding/src/submodule_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/tests/
+-rw-r--r--   0 root         (0) root         (0)      384 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/cpp/tests/collision/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/cpp/tests/collision/offline_tests/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/tests/collision/offline_tests/collision_stability_tests.cc
+-rw-r--r--   0 root         (0) root         (0)     5036 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/tests/collision/offline_tests/collision_tests.cc
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/tests/collision/offline_tests/collision_tests.h
+-rw-r--r--   0 root         (0) root         (0)      235 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/cpp/tests/collision/offline_tests/collision_unit_tests.cc
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-21 20:30:00.289599 commonroad-drivability-checker-2023.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8184 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/setup_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/third_party/
+-rw-r--r--   0 root         (0) root         (0)      483 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/external_box2d.cmake
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/external_gpc.cmake
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/external_libccd_fcl.cmake
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/external_pybind11.cmake
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/external_triangle.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.273599 commonroad-drivability-checker-2023.1/third_party/libs11n/
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/abstract_creator.hpp
+-rw-r--r--   0 root         (0) root         (0)    26130 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/algo.hpp
+-rw-r--r--   0 root         (0) root         (0)     5115 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/algo.tpp
+-rw-r--r--   0 root         (0) root         (0)     6644 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/classload.hpp
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/classload.tpp
+-rw-r--r--   0 root         (0) root         (0)    14508 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/client_api.hpp
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/exception.hpp
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/export.hpp
+-rw-r--r--   0 root         (0) root         (0)    18017 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/factory.hpp
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/factory_reg.hpp
+-rw-r--r--   0 root         (0) root         (0)    33111 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/functional.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/FlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     6997 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/compact_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)    36720 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_format.hpp
+-rw-r--r--   0 root         (0) root         (0)    24583 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_io.hpp
+-rw-r--r--   0 root         (0) root         (0)    15239 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/expat_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7036 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7100 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/parens_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5288 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/reg_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7979 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/serializers.hpp
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7894 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)    14116 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/strtool.hpp
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/micro_api.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/nodeutil/
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/nodeutil/node_tree.hpp
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/phoenix.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/
+-rw-r--r--   0 root         (0) root         (0)     6998 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/path_finder.hpp
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin.hpp
+-rw-r--r--   0 root         (0) root         (0)      821 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin_config.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/
+-rw-r--r--   0 root         (0) root         (0)    15091 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.hpp
+-rw-r--r--   0 root         (0) root         (0)     7474 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.tpp
+-rw-r--r--   0 root         (0) root         (0)    26710 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.hpp
+-rw-r--r--   0 root         (0) root         (0)    12955 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.tpp
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/path_finder_s11n.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/bool.hpp
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/char.hpp
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/double.hpp
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/float.hpp
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/int.hpp
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/long.hpp
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/long_double.hpp
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/size_t.hpp
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/string.hpp
+-rw-r--r--   0 root         (0) root         (0)      317 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/uint.hpp
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/ulong.hpp
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_list_specializations.hpp
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_map_specializations.hpp
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_node_type.hpp
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template3.hpp
+-rw-r--r--   0 root         (0) root         (0)     3517 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template4.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.277599 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/deque.hpp
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/list.hpp
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/map.hpp
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/multimap.hpp
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/multiset.hpp
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/pair.hpp
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/set.hpp
+-rw-r--r--   0 root         (0) root         (0)     6690 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/valarray.hpp
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/vector.hpp
+-rw-r--r--   0 root         (0) root         (0)     6410 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/reg_s11n_traits.hpp
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n.hpp
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n_config.hpp
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n_debuggering_macros.hpp
+-rw-r--r--   0 root         (0) root         (0)     7452 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n_node.hpp
+-rw-r--r--   0 root         (0) root         (0)    24061 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11nlite.hpp
+-rw-r--r--   0 root         (0) root         (0)    18758 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/serialize.hpp
+-rw-r--r--   0 root         (0) root         (0)     7697 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/serialize.tpp
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/simple_config.hpp
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/tags.hpp
+-rw-r--r--   0 root         (0) root         (0)    16445 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/traits.hpp
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/type_traits.hpp
+-rw-r--r--   0 root         (0) root         (0)    16096 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/variant.hpp
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/notes.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/s11nConfig.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.281599 commonroad-drivability-checker-2023.1/third_party/libs11n/src/
+-rw-r--r--   0 root         (0) root         (0)     6944 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/Makefile
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/argv_parser.cpp
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/argv_parser.hpp
+-rw-r--r--   0 root         (0) root         (0)    37640 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/compact.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/compact_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/data_node_io.cpp
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/exception.cpp
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/expat_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/export.hpp
+-rw-r--r--   0 root         (0) root         (0)    49935 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/funtxt.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/funtxt_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)    39725 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/funxml.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/funxml_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/in.sxml
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/in.wes
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/in.xml
+-rw-r--r--   0 root         (0) root         (0)    12038 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/main.cpp
+-rw-r--r--   0 root         (0) root         (0)    49900 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/parens.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/parens_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)     7377 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/path_finder.cpp
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.cpp
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.dl.cpp
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.noop.cpp
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.win32.cpp
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/s11n.cpp
+-rw-r--r--   0 root         (0) root         (0)     4321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/s11n_node.cpp
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/s11nlite.cpp
+-rw-r--r--   0 root         (0) root         (0)    65103 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/simplexml.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/simplexml_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)    14302 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/strtool.cpp
+-rw-r--r--   0 root         (0) root         (0)    42559 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/wesnoth.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/src/wesnoth_serializer.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.257599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.281599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/abstract_creator.hpp
+-rw-r--r--   0 root         (0) root         (0)    24256 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.hpp
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.tpp
+-rw-r--r--   0 root         (0) root         (0)     6605 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.hpp
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.tpp
+-rw-r--r--   0 root         (0) root         (0)    14420 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/client_api.hpp
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/exception.hpp
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/export.hpp
+-rw-r--r--   0 root         (0) root         (0)    18017 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/factory.hpp
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/factory_reg.hpp
+-rw-r--r--   0 root         (0) root         (0)    32992 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/functional.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.285599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/FlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     6405 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)    36761 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_format.hpp
+-rw-r--r--   0 root         (0) root         (0)    24423 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_io.hpp
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     6910 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5288 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/reg_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7979 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/serializers.hpp
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     7885 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)    14091 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/strtool.hpp
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/micro_api.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.285599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/nodeutil/
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/nodeutil/node_tree.hpp
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/phoenix.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.285599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/
+-rw-r--r--   0 root         (0) root         (0)     6978 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/path_finder.hpp
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin.hpp
+-rw-r--r--   0 root         (0) root         (0)      821 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin_config.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.285599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/
+-rw-r--r--   0 root         (0) root         (0)    15091 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.hpp
+-rw-r--r--   0 root         (0) root         (0)     7461 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.tpp
+-rw-r--r--   0 root         (0) root         (0)    26710 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.hpp
+-rw-r--r--   0 root         (0) root         (0)    12879 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.tpp
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/path_finder_s11n.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.285599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/bool.hpp
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/char.hpp
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/double.hpp
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/float.hpp
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/int.hpp
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/long.hpp
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/long_double.hpp
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/size_t.hpp
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/string.hpp
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/uint.hpp
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/pod/ulong.hpp
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_list_specializations.hpp
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_map_specializations.hpp
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_node_type.hpp
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.285599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/deque.hpp
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/list.hpp
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/map.hpp
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/multimap.hpp
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/multiset.hpp
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/pair.hpp
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/set.hpp
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/valarray.hpp
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/vector.hpp
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/reg_s11n_traits.hpp
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n.hpp
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_config.hpp
+-rw-r--r--   0 root         (0) root         (0)     4556 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_debuggering_macros.hpp
+-rw-r--r--   0 root         (0) root         (0)    10398 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_node.hpp
+-rw-r--r--   0 root         (0) root         (0)    24317 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11nlite.hpp
+-rw-r--r--   0 root         (0) root         (0)    18758 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.hpp
+-rw-r--r--   0 root         (0) root         (0)     7707 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.tpp
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/simple_config.hpp
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/tags.hpp
+-rw-r--r--   0 root         (0) root         (0)    17424 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/traits.hpp
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/type_traits.hpp
+-rw-r--r--   0 root         (0) root         (0)    15859 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/variant.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.289599 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/argv_parser.cpp
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/argv_parser.hpp
+-rw-r--r--   0 root         (0) root         (0)    37690 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/compact.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/compact_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/data_node_io.cpp
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/exception.cpp
+-rw-r--r--   0 root         (0) root         (0)    49906 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funtxt.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funtxt_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)    39716 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funxml.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funxml_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)    12038 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/main.cpp
+-rw-r--r--   0 root         (0) root         (0)    49869 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/parens.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/parens_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)     7347 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/path_finder.cpp
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/plugin.cpp
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/plugin.win32.cpp
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/s11n.cpp
+-rw-r--r--   0 root         (0) root         (0)     4321 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/s11n_node.cpp
+-rw-r--r--   0 root         (0) root         (0)     5029 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/s11nlite.cpp
+-rw-r--r--   0 root         (0) root         (0)    65094 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/simplexml.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/simplexml_serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)    14261 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/strtool.cpp
+-rw-r--r--   0 root         (0) root         (0)    42529 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/wesnoth.flex.cpp
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/wesnoth_serializer.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:30:00.289599 commonroad-drivability-checker-2023.1/third_party/patch/
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/patch/fcl-cmake-disable-warnings.patch
+-rw-r--r--   0 root         (0) root         (0)      764 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/patch/fcl-cmake-skip-findpackage-ccd.patch
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-21 20:29:58.000000 commonroad-drivability-checker-2023.1/third_party/patch/libccd-cmake-fix-install-location.patch
```

### Comparing `commonroad-drivability-checker-2022.2.1/LICENSE` & `commonroad-drivability-checker-2023.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/PKG-INFO` & `commonroad-drivability-checker-2023.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: commonroad-drivability-checker
-Version: 2022.2.1
+Version: 2023.1
 Summary: Drivability checker for CommonRoad scenarios.
 Home-page: https://commonroad.in.tum.de/drivability-checker
 Author: Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 License: BSD
-Project-URL: Documentation, https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/
+Project-URL: Documentation, https://cps.pages.gitlab.lrz.de/commonroad-drivability-checker/
 Project-URL: Forum, https://commonroad.in.tum.de/forum/c/commonroad-drivability-checker/
 Project-URL: Source, https://gitlab.lrz.de/tum-cps/commonroad-drivability-checker
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -31,28 +31,47 @@
 algorithms. It is compatible with the CommonRoad benchmark suite, which
 additionally facilitates and drastically reduces the effort of the development
 of motion planning algorithms.
 
 Please post questions, bug reports, etc. related to our tools or website in our [forum](https://commonroad.in.tum.de/forum/).
 
 
+Installation
+------------
+
+We provide two installation options: Installation as a Python package or building from source.
+
+1. **Python Package**: Install the python package via `pip` in your Conda environment:
+
+	```bash
+	pip install commonroad-drivability-checker
+	```
+	**Note for MacOS M1 users**: You need to use the 64-bit Anaconda Installer (graphical or command-line) in order to install the MacOS PyPi package.
+
+2. **Build from source**: To build the drivability checker from source, please refer to the installation description in the 
+[documentation](https://cps.pages.gitlab.lrz.de/commonroad-drivability-checker/).
+
+
 System Requirements
 -------------------
-The software is written in Python 3.6/3.7 and C++11 and tested on MacOS and Linux. The usage of the [Anaconda](http://www.anaconda.com/download/#download9) 
-Python distribution is strongly recommended.  For building the code, the following minimum versions are required:
+The software is written in Python 3.7 and C++11 and tested on MacOS and Linux. 
+
+The usage of the **[Anaconda](http://www.anaconda.com/download/#download9) Python distribution** is strongly recommended. 
+
+For building the code from source, the following minimum versions are required:
   * **GCC and G++**: version 9 or above
   * **CMake**: version 3.10 or above.
   * **Pip**: version 21.3 or above
 
-If you are a Mac user, we additionally recommend you to use Homebrew, allowing you to install required dependencies such as Eigen.
+**Note for MacOS users (M1 or Intel):** we additionally recommend using the Homebrew package manager, to install required dependencies such as Eigen.
 
 
 Third Party Libraries and Packages
 ----------------------------------
-The C++ code depends on the following libraries:
+The following third-party dependencies of the C++ code are only required for building the project from source!
 
 **Essential dependencies**:
 
 Not included as submodules:
 * [Eigen3](https://eigen.tuxfamily.org/dox/)
 * [Boost](https://www.boost.org/)
 * [OpenMP](https://www.openmp.org/)
@@ -73,26 +92,14 @@
 
 **Note**: Please be aware of the specific licensing conditions when including the optional dependencies Triangle and CGAL.
 See also `notes.txt` and the licensing information on the respective package websites for more details.
 
 The Python dependencies are listed in `requirements.txt`.
 
 
-
-Installation
-------------
-To install the Python package of the drivability checker, please run:
-```
-pip install commonroad-drivability-checker
-```
-
-To build the drivability checker package from source, please refer to the installation description in the 
-[documentation](https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/).
-
-
 Documentation
 -------------
 A full documentation as well as tutorials to get started with the tool can be found on our [toolpage](https://commonroad.in.tum.de/tools/drivability-checker).
 
 
 Publication
 -----------
```

### Comparing `commonroad-drivability-checker-2022.2.1/README.md` & `commonroad-drivability-checker-2023.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,47 @@
 algorithms. It is compatible with the CommonRoad benchmark suite, which
 additionally facilitates and drastically reduces the effort of the development
 of motion planning algorithms.
 
 Please post questions, bug reports, etc. related to our tools or website in our [forum](https://commonroad.in.tum.de/forum/).
 
 
+Installation
+------------
+
+We provide two installation options: Installation as a Python package or building from source.
+
+1. **Python Package**: Install the python package via `pip` in your Conda environment:
+
+	```bash
+	pip install commonroad-drivability-checker
+	```
+	**Note for MacOS M1 users**: You need to use the 64-bit Anaconda Installer (graphical or command-line) in order to install the MacOS PyPi package.
+
+2. **Build from source**: To build the drivability checker from source, please refer to the installation description in the 
+[documentation](https://cps.pages.gitlab.lrz.de/commonroad-drivability-checker/).
+
+
 System Requirements
 -------------------
-The software is written in Python 3.6/3.7 and C++11 and tested on MacOS and Linux. The usage of the [Anaconda](http://www.anaconda.com/download/#download9) 
-Python distribution is strongly recommended.  For building the code, the following minimum versions are required:
+The software is written in Python 3.7 and C++11 and tested on MacOS and Linux. 
+
+The usage of the **[Anaconda](http://www.anaconda.com/download/#download9) Python distribution** is strongly recommended. 
+
+For building the code from source, the following minimum versions are required:
   * **GCC and G++**: version 9 or above
   * **CMake**: version 3.10 or above.
   * **Pip**: version 21.3 or above
 
-If you are a Mac user, we additionally recommend you to use Homebrew, allowing you to install required dependencies such as Eigen.
+**Note for MacOS users (M1 or Intel):** we additionally recommend using the Homebrew package manager, to install required dependencies such as Eigen.
 
 
 Third Party Libraries and Packages
 ----------------------------------
-The C++ code depends on the following libraries:
+The following third-party dependencies of the C++ code are only required for building the project from source!
 
 **Essential dependencies**:
 
 Not included as submodules:
 * [Eigen3](https://eigen.tuxfamily.org/dox/)
 * [Boost](https://www.boost.org/)
 * [OpenMP](https://www.openmp.org/)
@@ -50,26 +69,14 @@
 
 **Note**: Please be aware of the specific licensing conditions when including the optional dependencies Triangle and CGAL.
 See also `notes.txt` and the licensing information on the respective package websites for more details.
 
 The Python dependencies are listed in `requirements.txt`.
 
 
-
-Installation
-------------
-To install the Python package of the drivability checker, please run:
-```
-pip install commonroad-drivability-checker
-```
-
-To build the drivability checker package from source, please refer to the installation description in the 
-[documentation](https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/).
-
-
 Documentation
 -------------
 A full documentation as well as tutorials to get started with the tool can be found on our [toolpage](https://commonroad.in.tum.de/tools/drivability-checker).
 
 
 Publication
 -----------
```

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/boundary.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/boundary/boundary.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/construction.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/boundary/construction.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/lanelet_bounds.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/boundary/lanelet_bounds.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/scenario_bounds.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/boundary/scenario_bounds.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/boundary/triangle_builder.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/boundary/triangle_builder.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/minkowski_sum.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/minkowski_sum.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/pycrcc_collision_dispatch.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/pycrcc_collision_dispatch.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/collision_detection/scenario.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/collision/collision_detection/scenario.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/trajectory_queries/trajectory_queries.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/collision/trajectory_queries/trajectory_queries.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/trajectory_queries/trajectory_queries_specialized.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/collision/trajectory_queries/trajectory_queries_specialized.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/collision/visualization/drawing.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/collision/visualization/drawing.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/evaluation.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/costs/evaluation.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/partial_cost_functions.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/costs/partial_cost_functions.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/costs/route_matcher.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/costs/route_matcher.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/feasibility_checker.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/feasibility_checker.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/solution_checker.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/solution_checker.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/feasibility/vehicle_dynamics.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/feasibility/vehicle_dynamics.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/geometry.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/geometry/geometry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from typing import Optional
 import numpy as np
 import commonroad_dc.pycrccosy as pycrccosy
 from commonroad_dc.geometry.util import chaikins_corner_cutting, resample_polyline, compute_polyline_length,\
     compute_pathlength_from_polyline, compute_orientation_from_polyline
+from matplotlib import pyplot as plt
 
 
 class RefPathLengthException(Exception):
     pass
 
 
 class CurvilinearCoordinateSystem(pycrccosy.CurvilinearCoordinateSystem):
@@ -38,23 +40,24 @@
 
         # remove duplicated vertices in reference path
         _, idx = np.unique(ref_path, axis=0, return_index=True)
         ref_path = ref_path[np.sort(idx)]
 
         # initialize Curvilinear Coordinate System
         super().__init__(ref_path, default_projection_domain_limit, eps, eps2)
-        # compute curvature
-        super().compute_and_set_curvature()
 
         # initialize reference attributes
         self._reference = np.asarray(super().reference_path())
         self._ref_pos = compute_pathlength_from_polyline(self.reference)
-        self._ref_curv = np.asarray(super().get_curvature())
-        self._ref_curv_d = np.gradient(self._ref_curv, self._ref_pos)
         self._ref_theta = np.unwrap(compute_orientation_from_polyline(self.reference))
+        self._ref_curv: Optional[np.ndarray] = None
+        self._ref_curv_d: Optional[np.ndarray] = None
+
+        # compute curvature and curvature derivative
+        self.compute_and_set_curvature()
 
     def __getstate__(self):
         return(pycrccosy.CurvilinearCoordinateSystem.__getstate__(self),
                self.__dict__)
 
     def __setstate__(self, state: tuple):
         pycrccosy.CurvilinearCoordinateSystem.__setstate__(self, state[0])
@@ -80,7 +83,41 @@
         """curvature rate along reference path"""
         return self._ref_curv_d
 
     @property
     def ref_theta(self) -> np.ndarray:
         """orientation along reference path"""
         return self._ref_theta
+
+    def compute_and_set_curvature(self, digits: int = 8):
+        """
+        Computes curvature and sets curvature _ref_curv and its derivative _ref_curv_d
+        :param digits: no. of decimal points to round curvature values
+        """
+        # call compute curvature function of C++ class
+        super().compute_and_set_curvature(digits)
+        # set curvature and curvature change
+        self._ref_curv = np.asarray(super().get_curvature())
+        self._ref_curv_d = np.gradient(self._ref_curv, self._ref_pos)
+
+    def plot_reference_states(self):
+        """function plots orientation, curvature and curvature rate of ref path over s position"""
+        plt.figure(figsize=(7, 7.5))
+        plt.suptitle("Reference path states")
+
+        # orientation
+        plt.subplot(3, 1, 1)
+        plt.plot(self.ref_pos, self.ref_theta, color="k")
+        plt.xlabel("s")
+        plt.ylabel("theta_ref")
+        # curvature
+        plt.subplot(3, 1, 2)
+        plt.plot(self.ref_pos, self.ref_curv, color="k")
+        plt.xlabel("s")
+        plt.ylabel("kappa_ref")
+        # curvature rate
+        plt.subplot(3, 1, 3)
+        plt.plot(self.ref_pos, self.ref_curv_d, color="k")
+        plt.xlabel("s")
+        plt.ylabel("kappa_dot_ref")
+        plt.tight_layout()
+        plt.show()
```

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/lanelet_ccosy.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/geometry/lanelet_ccosy.py`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_dc/geometry/util.py` & `commonroad-drivability-checker-2023.1/commonroad_dc/geometry/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     new_polyline = pycrccosy.Util.resample_polyline(polyline, step)
     return np.array(new_polyline)
 
 
 def resample_polyline_with_length_check(polyline, length_to_check: float = 2.0):
     """
     Resamples point with length check.
-    TODO: This is a helper functions to avoid exceptions during creating CurvilinearCoordinateSystem
-
+    TODO: This is a helper function to avoid exceptions during creating CurvilinearCoordinateSystem
+    :param length_to_check: length to be checked
     :param polyline: polyline with 2D points
     :return: resampled polyline
     """
     length = np.linalg.norm(polyline[-1] - polyline[0])
     if length > length_to_check:
         polyline = resample_polyline(polyline, 1.0)
     else:
@@ -63,34 +63,33 @@
 
 def compute_polyline_length(polyline: np.ndarray) -> float:
     """
     Computes the length of a given polyline
     :param polyline: The polyline
     :return: The path length of the polyline
     """
-    assert isinstance(polyline, np.ndarray) and polyline.ndim == 2 and len(
-        polyline[:,
-        0]) > 2, 'Polyline malformed for path length computation p={}'.format(polyline)
+    assert isinstance(polyline, np.ndarray) and polyline.ndim == 2 and len(polyline[:,0]) > 2, \
+        'Polyline malformed for path length computation p={}'.format(polyline)
 
     distance_between_points = np.diff(polyline, axis=0)
     # noinspection PyTypeChecker
     return np.sum(np.sqrt(np.sum(distance_between_points ** 2, axis=1)))
 
 
 def compute_curvature_from_polyline(polyline: np.ndarray) -> np.ndarray:
     """
     Computes the curvature of a given polyline
 
     :param polyline: The polyline for the curvature computation
     :return: The curvature of the polyline
     """
-    assert isinstance(polyline, np.ndarray) and polyline.ndim == 2 and len(
-        polyline[:, 0]) > 2, 'Polyline malformed for curvature computation p={}'.format(polyline)
+    assert isinstance(polyline, np.ndarray) and polyline.ndim == 2 and len(polyline[:, 0]) > 2, \
+        'Polyline malformed for curvature computation p={}'.format(polyline)
 
-    curvature=pycrccosy.Util.compute_curvature(polyline)
+    curvature = pycrccosy.Util.compute_curvature(polyline)
     return curvature
 
 
 def compute_orientation_from_polyline(polyline: np.ndarray) -> np.ndarray:
     """
     Computes the orientation of a given polyline
 
@@ -144,8 +143,8 @@
         else:
             rel = current_position / current_length
             new_polyline.append((1 - rel) * polyline[current_idx] +
                                 rel * polyline[current_idx + 1])
             current_position += step
     if np.linalg.norm(new_polyline[-1] - polyline[-1]) >= 1e-6:
         new_polyline.append(polyline[-1])
-    return np.array(new_polyline)
+    return np.array(new_polyline)
```

### Comparing `commonroad-drivability-checker-2022.2.1/commonroad_drivability_checker.egg-info/PKG-INFO` & `commonroad-drivability-checker-2023.1/commonroad_drivability_checker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: commonroad-drivability-checker
-Version: 2022.2.1
+Version: 2023.1
 Summary: Drivability checker for CommonRoad scenarios.
 Home-page: https://commonroad.in.tum.de/drivability-checker
 Author: Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 License: BSD
-Project-URL: Documentation, https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/
+Project-URL: Documentation, https://cps.pages.gitlab.lrz.de/commonroad-drivability-checker/
 Project-URL: Forum, https://commonroad.in.tum.de/forum/c/commonroad-drivability-checker/
 Project-URL: Source, https://gitlab.lrz.de/tum-cps/commonroad-drivability-checker
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -31,28 +31,47 @@
 algorithms. It is compatible with the CommonRoad benchmark suite, which
 additionally facilitates and drastically reduces the effort of the development
 of motion planning algorithms.
 
 Please post questions, bug reports, etc. related to our tools or website in our [forum](https://commonroad.in.tum.de/forum/).
 
 
+Installation
+------------
+
+We provide two installation options: Installation as a Python package or building from source.
+
+1. **Python Package**: Install the python package via `pip` in your Conda environment:
+
+	```bash
+	pip install commonroad-drivability-checker
+	```
+	**Note for MacOS M1 users**: You need to use the 64-bit Anaconda Installer (graphical or command-line) in order to install the MacOS PyPi package.
+
+2. **Build from source**: To build the drivability checker from source, please refer to the installation description in the 
+[documentation](https://cps.pages.gitlab.lrz.de/commonroad-drivability-checker/).
+
+
 System Requirements
 -------------------
-The software is written in Python 3.6/3.7 and C++11 and tested on MacOS and Linux. The usage of the [Anaconda](http://www.anaconda.com/download/#download9) 
-Python distribution is strongly recommended.  For building the code, the following minimum versions are required:
+The software is written in Python 3.7 and C++11 and tested on MacOS and Linux. 
+
+The usage of the **[Anaconda](http://www.anaconda.com/download/#download9) Python distribution** is strongly recommended. 
+
+For building the code from source, the following minimum versions are required:
   * **GCC and G++**: version 9 or above
   * **CMake**: version 3.10 or above.
   * **Pip**: version 21.3 or above
 
-If you are a Mac user, we additionally recommend you to use Homebrew, allowing you to install required dependencies such as Eigen.
+**Note for MacOS users (M1 or Intel):** we additionally recommend using the Homebrew package manager, to install required dependencies such as Eigen.
 
 
 Third Party Libraries and Packages
 ----------------------------------
-The C++ code depends on the following libraries:
+The following third-party dependencies of the C++ code are only required for building the project from source!
 
 **Essential dependencies**:
 
 Not included as submodules:
 * [Eigen3](https://eigen.tuxfamily.org/dox/)
 * [Boost](https://www.boost.org/)
 * [OpenMP](https://www.openmp.org/)
@@ -73,26 +92,14 @@
 
 **Note**: Please be aware of the specific licensing conditions when including the optional dependencies Triangle and CGAL.
 See also `notes.txt` and the licensing information on the respective package websites for more details.
 
 The Python dependencies are listed in `requirements.txt`.
 
 
-
-Installation
-------------
-To install the Python package of the drivability checker, please run:
-```
-pip install commonroad-drivability-checker
-```
-
-To build the drivability checker package from source, please refer to the installation description in the 
-[documentation](https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/).
-
-
 Documentation
 -------------
 A full documentation as well as tutorials to get started with the tool can be found on our [toolpage](https://commonroad.in.tum.de/tools/drivability-checker).
 
 
 Publication
 -----------
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/CMakeLists.txt` & `commonroad-drivability-checker-2023.1/cpp/CMakeLists.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,13 @@
-# CONF
-project(DrivabilityChecker)
-cmake_minimum_required(VERSION 3.10)
-
-option(BUILD_SHARED_LIBS "Build dc as a shared library" OFF)
-
-
-option(ADD_TESTS "unit tests" OFF)
-option(BUILD_DOC "generate the doc target." OFF)
-option(ADD_MODULE_GEOMETRY "add geometry module" ON)
-option(ADD_MODULE_COLLISION "add collision module" ON)
-option(ADD_PYTHON_BINDINGS "add Python bindings" OFF)
-option(ADD_TRIANGLE "Use a non-free Triangle library" OFF)
-
 if(WIN32)
 set(CMAKE_INTERPROCEDURAL_OPTIMIZATION FALSE)
 endif(WIN32)
 
 # Add modules for discovering Sphinx etc.
-set(CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/../CMakeModules" ${CMAKE_MODULE_PATH})
-
+set(CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/CMakeModules" ${CMAKE_MODULE_PATH})
 
 if(APPLE)
    # do nothing
 else()
 
 message(STATUS "Using full rpaths")
 # use, i.e. don't skip the full RPATH for the build tree
@@ -44,54 +29,51 @@
     set(CMAKE_INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/lib:$ORIGIN/")
 endif("${isSystemDir}" STREQUAL "-1")
 
 endif()
 
 
 if(ADD_PYTHON_BINDINGS)
-    
+
 
 	message(STATUS ${PYTHON_VER})
-	
-	if((PYTHON_VER) AND (PATH_TO_PYTHON_ENVIRONMENT)) 
+
+	if((PYTHON_VER) AND (PATH_TO_PYTHON_ENVIRONMENT))
 		if (${PYTHON_VER} GREATER_EQUAL 3.8)
 			set(PYTHON_INCLUDE_DIR ${PATH_TO_PYTHON_ENVIRONMENT}/include/python${PYTHON_VER})
 			set(PYTHON_LIBRARY ${PATH_TO_PYTHON_ENVIRONMENT}/lib/libpython${PYTHON_VER}.so)
 			set(PYTHON_EXECUTABLE ${PATH_TO_PYTHON_ENVIRONMENT}/bin/python${PYTHON_VER})
 		else()
 			set(PYTHON_INCLUDE_DIR ${PATH_TO_PYTHON_ENVIRONMENT}/include/python${PYTHON_VER}m)
 			set(PYTHON_LIBRARY ${PATH_TO_PYTHON_ENVIRONMENT}/lib/libpython${PYTHON_VER}m.so)
 			set(PYTHON_EXECUTABLE ${PATH_TO_PYTHON_ENVIRONMENT}/bin/python${PYTHON_VER}m)
 		endif()
 	else()
 		if((NOT PYTHON_INCLUDE_DIR) OR (NOT PYTHON_LIBRARY) OR (NOT PYTHON_EXECUTABLE))
 			#find_package(Python3 COMPONENTS Interpreter Development)
 		endif()
 	endif()
-	
 
-	
+
+
 	message(STATUS ${PYTHON_INCLUDE_DIR})
 	message(STATUS ${PYTHON_LIBRARY})
 	message(STATUS ${PYTHON_EXECUTABLE})
-
-    # Specific binary directory required here
-    add_subdirectory(../third_party/pybind11 third_party/pybind11)
 endif()
 
 ### Shared configuration
 
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 ### Discover dependencies
 
 if(NOT WIN32)
-find_package(s11n)
+#find_package(s11n)
 endif(NOT WIN32)
 
 find_package(Eigen3 3.0.5 QUIET CONFIG)
 
 # If Eigen3Config.cmake is not found, use the FindEigen3.cmake module
 if(NOT Eigen3_FOUND)
   find_package(Eigen3 3.0.5 QUIET MODULE)
@@ -143,54 +125,14 @@
 
 # Provides configure_package_config_file
 include(CMakePackageConfigHelpers)
 
 # Includes sane defaults for installation paths (CMAKE_INSTALL_LIBDIR, CMAKE_INSTALL_BINDIR etc.)
 include(GNUInstallDirs)
 
-if(ADD_TRIANGLE)
-  # Static library for triangle sources
-  
-message(STATUS "Building with support for triangulation using a non-free Triangle library")
-
-add_library(triangle STATIC
-    "${CMAKE_CURRENT_SOURCE_DIR}/../third_party/triangle/c/triangle.c"
-    "${CMAKE_CURRENT_SOURCE_DIR}/../third_party/triangle/c/triangle.h")
-
-target_compile_definitions(triangle PRIVATE -DANSI_DECLARATORS=1 -DTRILIBRARY=1 -DREAL=double -DVOID=int)
-
-
-set_property(TARGET triangle PROPERTY POSITION_INDEPENDENT_CODE ON)
-
-target_include_directories(triangle
-    PUBLIC
-        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/../third_party/triangle/c>
-    PRIVATE
-        ${CMAKE_CURRENT_SOURCE_DIR}/../third_party/triangle/c
-    )
-else()
-	message(STATUS "The non-free Triangle library is excluded from build.")
-endif()
-
-
-# Static library for gpc sources
-
-add_library(gpc STATIC
-    "${CMAKE_CURRENT_SOURCE_DIR}/../cpp/collision/src/plugins/triangulation/gpc_wrapper.c"
-    "${CMAKE_CURRENT_SOURCE_DIR}/../third_party/gpc/gpc.h")
-
-set_property(TARGET gpc PROPERTY POSITION_INDEPENDENT_CODE ON)
-
-target_include_directories(gpc
-    PUBLIC
-        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/../third_party/gpc>
-    PRIVATE
-        ${CMAKE_CURRENT_SOURCE_DIR}/../third_party/gpc
-    )
-	
 if(WIN32)
 
 set(S11_SRC_ROOT ${CMAKE_CURRENT_SOURCE_DIR}/../third_party/libs11n/windows/src)
 
 set(S11_SRC 
 
 ${S11_SRC_ROOT}/argv_parser.cpp
@@ -224,23 +166,25 @@
 
 target_include_directories(s11n
     PUBLIC
         $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/../third_party/libs11n/windows/include>
     PRIVATE
         ${CMAKE_CURRENT_SOURCE_DIR}/../third_party/libs11n/windows/include
     )
-	
+
+add_library(s11n::s11n ALIAS s11n)
+
 endif(WIN32)
 
 ### Definition of crcc
 
 if(ADD_MODULE_COLLISION)
     set(COLLISION_ROOT ${CMAKE_CURRENT_SOURCE_DIR}/collision)
     include(${CMAKE_CURRENT_SOURCE_DIR}/collision/CMakeLists.txt)
-    set(INSTALL_MODULES ${INSTALL_MODULES} crcc gpc)
+    set(INSTALL_MODULES ${INSTALL_MODULES} crcc gpc box2d)
     if(ADD_TRIANGLE)
         set(INSTALL_MODULES ${INSTALL_MODULES} triangle)
     endif()
     set(INSTALL_PYTHON_MODULES ${INSTALL_PYTHON_MODULES} pycrcc)
 endif(ADD_MODULE_COLLISION)
 
 if(WIN32)
@@ -254,31 +198,28 @@
     include(${CMAKE_CURRENT_SOURCE_DIR}/geometry/CMakeLists.txt)
 
 
     set(INSTALL_MODULES ${INSTALL_MODULES} crccosy)
     set(INSTALL_PYTHON_MODULES ${INSTALL_PYTHON_MODULES} pycrccosy)
 endif(ADD_MODULE_GEOMETRY)
 
+if(BUILD_S11N)
+    set(INSTALL_MODULES ${INSTALL_MODULES} s11n)
+endif()
+
 if(ADD_PYTHON_BINDINGS)
     set(PYBIND_ROOT ${CMAKE_CURRENT_SOURCE_DIR}/python_binding)
     include(${CMAKE_CURRENT_SOURCE_DIR}/python_binding/CMakeLists.txt)
 
 endif()
 
 if(ADD_TESTS)
     add_subdirectory(tests)
 endif()
 
-if(BUILD_DOC)
-    if(NOT (ADD_PYTHON_BINDINGS AND ADD_MODULE_COLLISION AND ADD_MODULE_GEOMETRY))
-        message(FATAL_ERROR "BUILD_DOC requires ADD_PYTHON_BINDINGS, ADD_MODULE_COLLISION and ADD_MODULE_GEOMETRY")
-    endif()
-    add_subdirectory(../doc doc)
-endif()
-
 if(ADD_PYTHON_BINDINGS)
     install(TARGETS ${INSTALL_PYTHON_MODULES}
         LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}/python
       )
 endif()
 
 install(TARGETS ${INSTALL_MODULES}
@@ -323,7 +264,14 @@
 
 if(ADD_MODULE_GEOMETRY)
   install(
       DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/geometry/include/
       DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}
     )
 endif()
+
+if(BUILD_DOC)
+    if(NOT (ADD_PYTHON_BINDINGS AND ADD_MODULE_COLLISION AND ADD_MODULE_GEOMETRY))
+        message(FATAL_ERROR "BUILD_DOC requires ADD_PYTHON_BINDINGS, ADD_MODULE_COLLISION and ADD_MODULE_GEOMETRY")
+    endif()
+    add_subdirectory(../doc doc)
+endif()
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/CMakeLists.txt` & `commonroad-drivability-checker-2023.1/cpp/collision/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 ### Definition of crcc
 
-find_package(fcl REQUIRED)
-
-find_package(ccd REQUIRED)
-
-find_package(box2d REQUIRED)
-
-find_package( Boost REQUIRED)
+find_package(Boost REQUIRED)
 
 
 set(COLLISION_SRC_ROOT ${COLLISION_ROOT}/src)
 
 set(COLLISION_SRC
 ${COLLISION_SRC_ROOT}/raytrace_primitive.cc
 ${COLLISION_SRC_ROOT}/shape_group.cc
@@ -94,37 +88,33 @@
         $<INSTALL_INTERFACE:include>
         $<BUILD_INTERFACE:${COLLISION_ROOT}/include>
     PRIVATE
         ${COLLISION_ROOT}/include
         ${Boost_INCLUDE_DIRS} 
     )
 
-if(NOT s11n_FOUND)
+if(NOT TARGET s11n::s11n)
     message(STATUS "Serialization and pickling support have been disabled for crcc")
     target_compile_definitions(crcc PRIVATE -DENABLE_SERIALIZER=0)
 else()
     message(STATUS "Serialization and pickling support have been enabled for crcc")
-    if(NOT WIN32)
-		target_link_libraries(crcc PUBLIC s11n::s11n)
-    else()
-		target_link_libraries(crcc PUBLIC s11n)
-	endif()
-	target_compile_definitions(crcc PRIVATE -DENABLE_SERIALIZER=1)
+    target_link_libraries(crcc PUBLIC s11n::s11n)
+    target_compile_definitions(crcc PRIVATE -DENABLE_SERIALIZER=1)
 endif()
 
 if(ADD_TRIANGLE)
     target_compile_definitions(crcc PUBLIC ENABLE_TRIANGLE=1)
 endif()
 
 target_link_libraries(crcc
   PRIVATE
     gpc
   PUBLIC
     fcl
     ccd
     Eigen3::Eigen
-    box2d::box2d
+    box2d
 )
 
 if(ADD_TRIANGLE)
     target_link_libraries(crcc PRIVATE triangle)
 endif()
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/application.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/application.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/application_settings.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/application_settings.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_checker.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_checker.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_object.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_object.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_object_ex.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_object_ex.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/collision_object_types.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/collision_object_types.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/i_collision_checker.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/i_collision_checker.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/line_segment.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/line_segment.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/detail/aabb.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/detail/aabb.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/detail/obb.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/detail/obb.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/point.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/point.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/polygon.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/polygon.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/rectangle_aabb.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/rectangle_aabb.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/rectangle_obb.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/rectangle_obb.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/shape.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/shape.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/sphere.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/sphere.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/triangle.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/triangle.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/narrowphase/utils.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/narrowphase/utils.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/plugins/triangulation/triangulate.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/plugins/triangulation/triangulate.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/primitive_collision_checker.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/primitive_collision_checker.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/raytrace_primitive.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/raytrace_primitive.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/raytrace_utils.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/raytrace_utils.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/broadphase_failure_cc_obj_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/broadphase_failure_cc_obj_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/broadphase_failure_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/broadphase_failure_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/broadphase_failure_obj_obj_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/broadphase_failure_obj_obj_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/collision_checker_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/collision_checker_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/collision_object_export_s11.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/collision_object_export_s11.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/final/collision_object_export_final.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/final/collision_object_export_final.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/point_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/point_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/polygon_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/polygon_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/public/serialize_public.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/public/serialize_public.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/rectangle_aabb_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/rectangle_aabb_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/rectangle_obb_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/rectangle_obb_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/serialize.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/serialize.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/serialize_reg_impl.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/serialize_reg_impl.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/shape_group_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/shape_group_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/sphere_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/sphere_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/triangle_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/triangle_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/tv_object_export.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/tv_object_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/serialize/vector2d_export_streams.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/serialize/vector2d_export_streams.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/shape_group.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/shape_group.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/common.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/common.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_box2d_inl.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_box2d_inl.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_fcl_inl.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_fcl_inl.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid_inl.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/accelerators/detail/container_grid_inl.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_collision_object.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_collision_object.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_collision_queries.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_collision_queries.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_entity_type.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_entity_type.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_helpers.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_helpers.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/boost_object_polygon.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/boost_object_polygon.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/i_boost_collision_object.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/i_boost_collision_object.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/i_solver_entity_boost.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/i_solver_entity_boost.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost_factory.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/boost/solver_entity_boost_factory.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_requests.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_requests.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_solver_fcl.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_solver_fcl.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_solver_primitive.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_solver_primitive.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/collision_solvers.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/collision_solvers.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/distance_requests.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/distance_requests.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_broadphase_manager_factory.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_broadphase_manager_factory.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_checker.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_checker.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object_group.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_object_group.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_queries.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_queries.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_requests.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_collision_requests.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_queries.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_queries.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_requests.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_distance_requests.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_helpers.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_helpers.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/fcl_transform.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/fcl_transform.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object_group.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/i_fcl_collision_object_group.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/performance_timers.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/performance_timers.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl_factory.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/fcl/solver_entity_fcl_factory.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/geometry_queries.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/geometry_queries.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/primitive_collision_queries.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/primitive_collision_queries.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/aabb_sat2d.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/aabb_sat2d.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/obb_sat2d.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/obb_sat2d.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/sat2d_checks.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/sat2d_checks.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/sat2d/triangle_sat2d.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/sat2d/triangle_sat2d.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/solvers/trajectory_queries.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/solvers/trajectory_queries.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/broadphase_failure.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/broadphase_failure.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/broadphase_test.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/broadphase_test.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/tests/test_common.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/tests/test_common.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/include/collision/time_variant_collision_object.h` & `commonroad-drivability-checker-2023.1/cpp/collision/include/collision/time_variant_collision_object.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/collision_checker.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/collision_checker.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/collision_object.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/collision_object.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/collision_object_ex.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/collision_object_ex.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/point.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/point.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/polygon.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/polygon.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/rectangle_aabb.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/rectangle_aabb.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/rectangle_obb.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/rectangle_obb.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/shape.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/shape.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/sphere.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/sphere.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/narrowphase/triangle.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/narrowphase/triangle.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/plugins/triangulation/triangulate.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/plugins/triangulation/triangulate.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/primitive_collision_checker.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/primitive_collision_checker.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/raytrace_primitive.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/raytrace_primitive.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/raytrace_utils.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/raytrace_utils.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/final/collision_object_export_final.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/final/collision_object_export_final.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/public/serialize_public.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/public/serialize_public.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_collision_checker.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_collision_checker.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_container_cc_obj.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_container_cc_obj.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_container_obj_obj.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_container_obj_obj.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_point.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_point.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_polygon.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_polygon.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_rectangle_aabb.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_rectangle_aabb.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_rectangle_obb.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_rectangle_obb.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_shape_group.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_shape_group.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_sphere.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_sphere.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_triangle.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_triangle.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/serialize/serialize_tv_object.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/serialize/serialize_tv_object.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/shape_group.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/shape_group.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_collision_object.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_collision_object.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_collision_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_collision_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_geometry_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_geometry_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/boost/boost_object_polygon.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/boost/boost_object_polygon.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_solver_default.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_solver_default.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_solver_fcl.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_solver_fcl.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/collision_solver_primitive.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/collision_solver_primitive.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/detail/collision_containers.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/detail/collision_containers.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/distance_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/distance_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_broadphase_manager_factories.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_broadphase_manager_factories.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_checker.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_checker.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_object.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_object.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_object_group.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_object_group.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_collision_requests.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_collision_requests.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_distance_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_distance_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_distance_requests.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_distance_requests.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/fcl_entity_factory.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/fcl_entity_factory.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/fcl/performance_timers.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/fcl/performance_timers.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/geometry_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/geometry_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/sat2d/sat2d_checks.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/sat2d/sat2d_checks.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/solvers/trajectory_queries.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/solvers/trajectory_queries.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/tests/online_tests/broadphase_test.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/tests/online_tests/broadphase_test.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/tests/online_tests/test_common.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/tests/online_tests/test_common.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/collision/src/time_variant_collision_object.cc` & `commonroad-drivability-checker-2023.1/cpp/collision/src/time_variant_collision_object.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/CMakeLists.txt` & `commonroad-drivability-checker-2023.1/cpp/geometry/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -42,19 +42,15 @@
     PRIVATE
         ${CRCCOSY_ROOT}
         ${Boost_INCLUDE_DIRS} 
     )
 
 
 
-if(NOT s11n_FOUND)
+if(NOT TARGET s11n::s11n)
     message(STATUS "Serialization and pickling support have been disabled for crccosy")
     target_compile_definitions(crccosy PRIVATE -DENABLE_SERIALIZER=0)
 else()
     message(STATUS "Serialization and pickling support have been enabled for crccosy")
-	if(NOT WIN32)
-		target_link_libraries(crccosy PUBLIC s11n::s11n)
-	else()
-		target_link_libraries(crccosy PUBLIC s11n)
-	endif()
+    target_link_libraries(crccosy PUBLIC s11n::s11n)
     target_compile_definitions(crccosy PRIVATE -DENABLE_SERIALIZER=1)
 endif()
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/curvilinear_coordinate_system.h` & `commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/curvilinear_coordinate_system.h`

 * *Files 0% similar despite different names*

```diff
@@ -191,18 +191,19 @@
    */
 
   static Eigen::VectorXd computeCurvature(const EigenPolyline &polyline);
 
   /**
    *
    * Computes and sets the curvature information for the reference path
+   * @param digits: no. of decimal points for curvature value (default 8)
    *
    */
 
-  int computeAndSetCurvature(void);
+  int computeAndSetCurvature(int digits = 8);
 
   /**
    *
    * Tangent vector at a specific longitudinal coordinate
    *
    * @param s longitudinal coordinate
    * @return tangent vector
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/segment.h` & `commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/segment.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/curvilinear_coordinate_system_export.h` & `commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/curvilinear_coordinate_system_export.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/public/serialize_public.h` & `commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/public/serialize_public.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/serialize/vector2d_export_streams.h` & `commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/serialize/vector2d_export_streams.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/include/geometry/util.h` & `commonroad-drivability-checker-2023.1/cpp/geometry/include/geometry/util.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/src/curvilinear_coordinate_system.cc` & `commonroad-drivability-checker-2023.1/cpp/geometry/src/curvilinear_coordinate_system.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1120,19 +1120,21 @@
       ((x_d.cwiseProduct(y_dd).eval() - x_dd.cwiseProduct(y_d).eval()).array() /
        ((x_d.array().pow(2) + y_d.array().pow(2)).pow(3. / 2.)))
           .eval();
 
   return curvature;
 }
 
-int CurvilinearCoordinateSystem::computeAndSetCurvature(void) {
+int CurvilinearCoordinateSystem::computeAndSetCurvature(int digits) {
   auto curvature = computeCurvature(referencePath());
   std::vector<double> curv;
+  double precision = pow(10.0, digits);
   for (int cc1 = 0; cc1 < curvature.size(); cc1++) {
-    curv.push_back(curvature[cc1]);
+    // round value to precision
+    curv.push_back(std::round(curvature[cc1] * precision) / precision);
   }
   this->setCurvature(curv);
   return 0;
 }
 
 void CurvilinearCoordinateSystem::computeBestProjectionAxisForSegments() {
   for (int i = 0; i < this->segment_list_.size(); i++) {
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/src/segment.cc` & `commonroad-drivability-checker-2023.1/cpp/geometry/src/segment.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/src/serialize/public/serialize_public.cc` & `commonroad-drivability-checker-2023.1/cpp/geometry/src/serialize/public/serialize_public.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/geometry/src/serialize/serialize_curvil_cs.cc` & `commonroad-drivability-checker-2023.1/cpp/geometry/src/serialize/serialize_curvil_cs.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/python_binding/CMakeLists.txt` & `commonroad-drivability-checker-2023.1/cpp/python_binding/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,21 +14,17 @@
 	IF (WIN32)
 		#requires  cmake 3.13
 		target_link_options(pycrcc PRIVATE -static-libgcc -static-libstdc++ -static)
 	ENDIF()
 
     target_link_libraries(pycrcc PUBLIC crcc)
 
-if(s11n_FOUND)
+if(TARGET s11n::s11n)
     target_compile_definitions(pycrcc PRIVATE -DENABLE_SERIALIZER=1)
-	if(NOT WIN32)
-		target_link_libraries(pycrcc PUBLIC s11n::s11n)
-	else()
-	    target_link_libraries(pycrcc PUBLIC s11n)
-	endif(NOT WIN32)
+    target_link_libraries(pycrcc PUBLIC s11n::s11n)
 else()
     target_compile_definitions(pycrcc PRIVATE -DENABLE_SERIALIZER=0)
 endif()
 
 
 
 
@@ -85,21 +81,17 @@
 	IF (WIN32)
 		#requires  cmake 3.13
 		target_link_options(pycrccosy PRIVATE -static-libgcc -static-libstdc++ -static)
 	ENDIF()
 
     target_link_libraries(pycrccosy PUBLIC crccosy)
 
-if(s11n_FOUND)
+if(TARGET s11n::s11n)
     target_compile_definitions(pycrccosy PRIVATE -DENABLE_SERIALIZER=1)
-	if(NOT WIN32)
-		target_link_libraries(pycrccosy PUBLIC s11n::s11n)
-	else()
-		target_link_libraries(pycrccosy PUBLIC s11n)
-	endif()
+    target_link_libraries(pycrccosy PUBLIC s11n::s11n)
 else()
     target_compile_definitions(pycrccosy PRIVATE -DENABLE_SERIALIZER=0)
 endif()
 	
 
     # See note on $ORIGIN above
     if(APPLE)
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/module_collision.cc` & `commonroad-drivability-checker-2023.1/cpp/python_binding/src/module_collision.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/module_geometry.cc` & `commonroad-drivability-checker-2023.1/cpp/python_binding/src/module_geometry.cc`

 * *Files 2% similar despite different names*

```diff
@@ -331,18 +331,21 @@
       .def("convert_list_of_points_to_cartesian_coords",
            &geometry::CurvilinearCoordinateSystem::
                convertListOfPointsToCartesianCoords,
            "Converts list of points to the cartesian coordinate system."
            "\n\n:param points: vector of points in the curvilinear coordinate frame"
            "\n\n:param num_omp_threads: number of OMP threads for computation"
            "\n\n:return: transformed points")
-      .def("compute_and_set_curvature",
-           &geometry::CurvilinearCoordinateSystem::computeAndSetCurvature,
+      .def("compute_and_set_curvature", [](geometry::CurvilinearCoordinateSystem &cosy, const int digits){
+               return cosy.computeAndSetCurvature(digits);
+           },
+           py::arg("digits") = 8,
            "Automatically computes and sets the curvature information for the "
-           "reference path.")
+           "reference path."
+           "\n\n:param digits:  no. of decimal points for curvature value (default 8)")
 
 #if ENABLE_SERIALIZER
       .def(py::pickle(
           [](const geometry::CurvilinearCoordinateSystem
                  &obj) {  // __getstate__
             /* Return a tuple that fully encodes the state of the object */
             py::list ret;
```

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/python_binding/src/submodule_util.h` & `commonroad-drivability-checker-2023.1/cpp/python_binding/src/submodule_util.h`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/cpp/tests/collision/offline_tests/collision_tests.cc` & `commonroad-drivability-checker-2023.1/cpp/tests/collision/offline_tests/collision_tests.cc`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/setup.py` & `commonroad-drivability-checker-2023.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from sysconfig import get_paths
 
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 
 from distutils.version import LooseVersion
 
+from commonroad_dc.__version__ import __version__
+
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), 'r', encoding='utf-8') as f:
     readme = f.read()
 
 
 class CMakeExtension(Extension):
     def __init__(self, name, sourcedir=''):
@@ -50,63 +52,68 @@
         if not extdir.endswith(os.path.sep):
             extdir += os.path.sep
 
         default_python_include_dir = get_paths()['include']
         default_python_library = ""  # find_libpython()
         default_python_executable = sys.executable
 
-        if (setup_options_dict['PYTHON_INCLUDE_DIR'] != ''):
+        if setup_options_dict['PYTHON_INCLUDE_DIR'] != '':
             python_include_dir = setup_options_dict['PYTHON_INCLUDE_DIR']
         else:
             python_include_dir = default_python_include_dir
 
-        if (setup_options_dict['PYTHON_LIBRARY'] != ''):
+        if setup_options_dict['PYTHON_LIBRARY'] != '':
             python_library = setup_options_dict['PYTHON_LIBRARY']
         else:
             python_library = default_python_library
 
-        if (setup_options_dict['PYTHON_EXECUTABLE'] != ''):
+        if setup_options_dict['PYTHON_EXECUTABLE'] != '':
             python_executable = setup_options_dict['PYTHON_EXECUTABLE']
         else:
             python_executable = default_python_executable
 
         cmake_args = [
             "-DPYTHON_INCLUDE_DIR=" + python_include_dir,
             "-DPYTHON_LIBRARY=" + python_library,
             "-DPYTHON_EXECUTABLE=" + python_executable,
         ]
 
         # build documentation
-        if (setup_options_dict['BUILD_DOC'] != ''):
-            cmake_args += ['-DBUILD_DOC=' + setup_options_dict['BUILD_DOC']]
+        build_doc = 'OFF'
+        if 'BUILD_DOC' in os.environ:
+            build_doc = os.environ['BUILD_DOC']
+            cmake_args += ['-DBUILD_DOC=' + build_doc]
+        elif setup_options_dict['BUILD_DOC'] != '':
+            build_doc = setup_options_dict['BUILD_DOC']
+            cmake_args += ['-DBUILD_DOC=' + build_doc]
         else:
             cmake_args += ['-DBUILD_DOC=OFF']
 
         # add tests
-        if (setup_options_dict['ADD_TESTS'] != ''):
+        if setup_options_dict['ADD_TESTS'] != '':
             cmake_args += ['-DADD_TESTS=' + setup_options_dict['ADD_TESTS']]
         else:
             cmake_args += ['-DADD_TESTS=OFF']
 
         # Enable the non-free Triangle library
 
-        if (setup_options_dict['ADD_TRIANGLE'] != ''):
+        if setup_options_dict['ADD_TRIANGLE'] != '':
             cmake_args += ['-DADD_TRIANGLE=' + setup_options_dict['ADD_TRIANGLE']]
         else:
             cmake_args += ['-DADD_TRIANGLE=OFF']
 
         # add python bindings
-        if (setup_options_dict['ADD_PYTHON_BINDINGS'] != ''):
+        if setup_options_dict['ADD_PYTHON_BINDINGS'] != '':
             cmake_args += ['-DADD_PYTHON_BINDINGS=' + setup_options_dict['ADD_PYTHON_BINDINGS']]
         else:
             cmake_args += ['-DADD_PYTHON_BINDINGS=ON']
 
         print(cmake_args)
 
-        if (setup_options_dict['DEBUG'] != ''):
+        if setup_options_dict['DEBUG'] != '':
             self.debug = setup_options_dict['DEBUG']
         else:
             self.debug = False
 
         cfg = 'Debug' if self.debug else 'Release'
         build_args = ['--config', cfg]
 
@@ -120,20 +127,16 @@
 
         for p in [dist_dir, build_dir]:
             if not os.path.exists(p):
                 os.makedirs(p)
 
         cmake_args += ['-DCMAKE_INSTALL_PREFIX:PATH={}'.format(dist_dir)]
 
-        import multiprocessing
-
         build_args += ['--target', 'install']
 
-        # install_args=build_args
-
         if ('BUILD_JOBS' in os.environ):
             build_args += ['--'] + ['-j'] + [os.environ['BUILD_JOBS']]
 
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=build_dir)
         subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=build_dir)
 
         lib_dir = os.path.join(dist_dir, 'lib')
@@ -159,27 +162,32 @@
         shutil.copy(os.path.join(lib_dir, 'libcrccosy.a'), os.path.join(os.getcwd(), 'commonroad_dc'))
         shutil.copy(os.path.join(lib_dir, 'libgpc.a'), os.path.join(os.getcwd(), 'commonroad_dc'))
         try:
             shutil.copy(os.path.join(lib_dir, 'libtriangle.a'), os.path.join(os.getcwd(), 'commonroad_dc'))
         except(Exception):
             pass
 
-        # self.copy_file(os.path.join(lib_dir, 'libcrcc.a'), os.path.join(os.getcwd(), 'commonroad_dc'))
-        # self.copy_file(os.path.join(lib_dir, 'libcrccosy.a'), os.path.join(os.getcwd(), 'commonroad_dc'))
+        # copy documentation files to doc/build if Cmake Flag -DBUILD_DOC=='ON'
+        if build_doc == 'ON':
+            doc_target_dir = os.path.join(os.getcwd(), 'doc/build')
+            if os.path.exists(doc_target_dir):
+                shutil.rmtree(doc_target_dir)
+            doc_source_dir = os.path.join(dist_dir, 'share/doc/DrivabilityChecker')
+            shutil.copytree(doc_source_dir, doc_target_dir)
 
 
 setup(
     name='commonroad-drivability-checker',
-    version='2022.2.1',
+    version=__version__,
     description='Drivability checker for CommonRoad scenarios.',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://commonroad.in.tum.de/drivability-checker',
     project_urls={
-        'Documentation': 'https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/',
+        'Documentation': 'https://cps.pages.gitlab.lrz.de/commonroad-drivability-checker/',
         'Forum': 'https://commonroad.in.tum.de/forum/c/commonroad-drivability-checker/',
         'Source': 'https://gitlab.lrz.de/tum-cps/commonroad-drivability-checker',
     },
 
     author='Technical University of Munich',
     author_email='commonroad@lists.lrz.de',
     license='BSD',
@@ -198,15 +206,17 @@
     install_requires=[
         'commonroad-io>=2022.3',
         'commonroad-vehicle-models>=3.0.0',
         'numpy>=1.19',
         'scipy>=1.4.1',
         'matplotlib>=3.2.2',
         'polygon3>=3.0.8',
-        'shapely>=1.6.4'
+        'shapely>=1.6.4',
+        'setuptools>=62.1.0',
+        'matplotlib>=3.2.2'
     ],
 
     # Additional information
     classifiers=[
         "Programming Language :: C++",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/fcl/test/gtest/include/gtest/gtest-message.h` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_node.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,250 +1,303 @@
-// Copyright 2005, Google Inc.
-// All rights reserved.
-//
-// Redistribution and use in source and binary forms, with or without
-// modification, are permitted provided that the following conditions are
-// met:
-//
-//     * Redistributions of source code must retain the above copyright
-// notice, this list of conditions and the following disclaimer.
-//     * Redistributions in binary form must reproduce the above
-// copyright notice, this list of conditions and the following disclaimer
-// in the documentation and/or other materials provided with the
-// distribution.
-//     * Neither the name of Google Inc. nor the names of its
-// contributors may be used to endorse or promote products derived from
-// this software without specific prior written permission.
-//
-// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-//
-// Author: wan@google.com (Zhanyong Wan)
-//
-// The Google C++ Testing Framework (Google Test)
-//
-// This header file defines the Message class.
-//
-// IMPORTANT NOTE: Due to limitation of the C++ language, we have to
-// leave some internal implementation details in this header file.
-// They are clearly marked by comments like this:
-//
-//   // INTERNAL IMPLEMENTATION - DO NOT USE IN A USER PROGRAM.
-//
-// Such code is NOT meant to be used by a user directly, and is subject
-// to CHANGE WITHOUT NOTICE.  Therefore DO NOT DEPEND ON IT in a user
-// program!
-
-#ifndef GTEST_INCLUDE_GTEST_GTEST_MESSAGE_H_
-#define GTEST_INCLUDE_GTEST_GTEST_MESSAGE_H_
-
-#include <limits>
-
-#include "gtest/internal/gtest-port.h"
-
-// Ensures that there is at least one operator<< in the global namespace.
-// See Message& operator<<(...) below for why.
-void operator<<(const testing::internal::Secret&, int);
-
-namespace testing {
-
-// The Message class works like an ostream repeater.
-//
-// Typical usage:
-//
-//   1. You stream a bunch of values to a Message object.
-//      It will remember the text in a stringstream.
-//   2. Then you stream the Message object to an ostream.
-//      This causes the text in the Message to be streamed
-//      to the ostream.
-//
-// For example;
-//
-//   testing::Message foo;
-//   foo << 1 << " != " << 2;
-//   std::cout << foo;
-//
-// will print "1 != 2".
-//
-// Message is not intended to be inherited from.  In particular, its
-// destructor is not virtual.
-//
-// Note that stringstream behaves differently in gcc and in MSVC.  You
-// can stream a NULL char pointer to it in the former, but not in the
-// latter (it causes an access violation if you do).  The Message
-// class hides this difference by treating a NULL char pointer as
-// "(null)".
-class GTEST_API_ Message {
- private:
-  // The type of basic IO manipulators (endl, ends, and flush) for
-  // narrow streams.
-  typedef std::ostream& (*BasicNarrowIoManip)(std::ostream&);
-
- public:
-  // Constructs an empty Message.
-  Message();
-
-  // Copy constructor.
-  Message(const Message& msg) : ss_(new ::std::stringstream) {  // NOLINT
-    *ss_ << msg.GetString();
-  }
-
-  // Constructs a Message from a C-string.
-  explicit Message(const char* str) : ss_(new ::std::stringstream) {
-    *ss_ << str;
-  }
-
-#if GTEST_OS_SYMBIAN
-  // Streams a value (either a pointer or not) to this object.
-  template <typename T>
-  inline Message& operator <<(const T& value) {
-    StreamHelper(typename internal::is_pointer<T>::type(), value);
-    return *this;
-  }
-#else
-  // Streams a non-pointer value to this object.
-  template <typename T>
-  inline Message& operator <<(const T& val) {
-    // Some libraries overload << for STL containers.  These
-    // overloads are defined in the global namespace instead of ::std.
-    //
-    // C++'s symbol lookup rule (i.e. Koenig lookup) says that these
-    // overloads are visible in either the std namespace or the global
-    // namespace, but not other namespaces, including the testing
-    // namespace which Google Test's Message class is in.
-    //
-    // To allow STL containers (and other types that has a << operator
-    // defined in the global namespace) to be used in Google Test
-    // assertions, testing::Message must access the custom << operator
-    // from the global namespace.  With this using declaration,
-    // overloads of << defined in the global namespace and those
-    // visible via Koenig lookup are both exposed in this function.
-    using ::operator <<;
-    *ss_ << val;
-    return *this;
-  }
-
-  // Streams a pointer value to this object.
-  //
-  // This function is an overload of the previous one.  When you
-  // stream a pointer to a Message, this definition will be used as it
-  // is more specialized.  (The C++ Standard, section
-  // [temp.func.order].)  If you stream a non-pointer, then the
-  // previous definition will be used.
-  //
-  // The reason for this overload is that streaming a NULL pointer to
-  // ostream is undefined behavior.  Depending on the compiler, you
-  // may get "0", "(nil)", "(null)", or an access violation.  To
-  // ensure consistent result across compilers, we always treat NULL
-  // as "(null)".
-  template <typename T>
-  inline Message& operator <<(T* const& pointer) {  // NOLINT
-    if (pointer == NULL) {
-      *ss_ << "(null)";
-    } else {
-      *ss_ << pointer;
-    }
-    return *this;
-  }
-#endif  // GTEST_OS_SYMBIAN
-
-  // Since the basic IO manipulators are overloaded for both narrow
-  // and wide streams, we have to provide this specialized definition
-  // of operator <<, even though its body is the same as the
-  // templatized version above.  Without this definition, streaming
-  // endl or other basic IO manipulators to Message will confuse the
-  // compiler.
-  Message& operator <<(BasicNarrowIoManip val) {
-    *ss_ << val;
-    return *this;
-  }
-
-  // Instead of 1/0, we want to see true/false for bool values.
-  Message& operator <<(bool b) {
-    return *this << (b ? "true" : "false");
-  }
-
-  // These two overloads allow streaming a wide C string to a Message
-  // using the UTF-8 encoding.
-  Message& operator <<(const wchar_t* wide_c_str);
-  Message& operator <<(wchar_t* wide_c_str);
-
-#if GTEST_HAS_STD_WSTRING
-  // Converts the given wide string to a narrow string using the UTF-8
-  // encoding, and streams the result to this Message object.
-  Message& operator <<(const ::std::wstring& wstr);
-#endif  // GTEST_HAS_STD_WSTRING
-
-#if GTEST_HAS_GLOBAL_WSTRING
-  // Converts the given wide string to a narrow string using the UTF-8
-  // encoding, and streams the result to this Message object.
-  Message& operator <<(const ::wstring& wstr);
-#endif  // GTEST_HAS_GLOBAL_WSTRING
-
-  // Gets the text streamed to this object so far as an std::string.
-  // Each '\0' character in the buffer is replaced with "\\0".
-  //
-  // INTERNAL IMPLEMENTATION - DO NOT USE IN A USER PROGRAM.
-  std::string GetString() const;
-
- private:
-
-#if GTEST_OS_SYMBIAN
-  // These are needed as the Nokia Symbian Compiler cannot decide between
-  // const T& and const T* in a function template. The Nokia compiler _can_
-  // decide between class template specializations for T and T*, so a
-  // tr1::type_traits-like is_pointer works, and we can overload on that.
-  template <typename T>
-  inline void StreamHelper(internal::true_type /*is_pointer*/, T* pointer) {
-    if (pointer == NULL) {
-      *ss_ << "(null)";
-    } else {
-      *ss_ << pointer;
-    }
-  }
-  template <typename T>
-  inline void StreamHelper(internal::false_type /*is_pointer*/,
-                           const T& value) {
-    // See the comments in Message& operator <<(const T&) above for why
-    // we need this using statement.
-    using ::operator <<;
-    *ss_ << value;
-  }
-#endif  // GTEST_OS_SYMBIAN
-
-  // We'll hold the text streamed to this object here.
-  const internal::scoped_ptr< ::std::stringstream> ss_;
-
-  // We declare (but don't implement) this to prevent the compiler
-  // from implementing the assignment operator.
-  void operator=(const Message&);
-};
-
-// Streams a Message to an ostream.
-inline std::ostream& operator <<(std::ostream& os, const Message& sb) {
-  return os << sb.GetString();
-}
-
-namespace internal {
-
-// Converts a streamable value to an std::string.  A NULL pointer is
-// converted to "(null)".  When the input value is a ::string,
-// ::std::string, ::wstring, or ::std::wstring object, each NUL
-// character in it is replaced with "\\0".
-template <typename T>
-std::string StreamableToString(const T& streamable) {
-  return (Message() << streamable).GetString();
-}
+#ifndef s11n_S11N_NODE_HPP_INCLUDED
+#define s11n_S11N_NODE_HPP_INCLUDED
 
-}  // namespace internal
-}  // namespace testing
+////////////////////////////////////////////////////////////////////////
+// s11n_node.hpp
+// A reference implementation for s11n's Data Node concept.
+// License: Public Domain
+// Author: stephan@s11n.net
+////////////////////////////////////////////////////////////////////////
+#include <string>
+#include <map>
+
+#include <vector>
+#include <s11n.net/s11n/variant.hpp> // for lexical casting
+#include <s11n.net/s11n/export.hpp>
+
+namespace s11n {
+
+	/**
+	   s11n_node is a slightly lighter-weight replacement for
+	   the data_node type used in s11n 1.0.x. It will become
+	   the standard node type for s11nlite in 1.1/1.2.
+        */
+        class S11N_EXPORT_API s11n_node
+        {
+        public:
+
+                /**
+                   The map type this object uses to store properties.
+                 */
+		typedef std::map < std::string, std::string > map_type;
+
+                /**
+                   A pair type used to store key/value properties
+                   internally.
+                */
+		typedef map_type::value_type value_type;
+
+                /** The type used to store property keys. For
+                    compatibility with std::map.
+                */
+                typedef map_type::key_type key_type; 
+
+                /** The type used to internally store property
+                    values. For compatibility with std::map.
+                */
+                typedef map_type::mapped_type mapped_type;
+
+                /**
+                   The container type used to store this object's children.
+                   It contains (s11n_node *).
+
+                   While the exact type is not guaranteed, it is
+                   guaranteed to obey the most-commonly-used
+                   std::list/vector conventions: push_back(), erase(),
+                   etc.
+                */
+		typedef std::vector<s11n_node *> child_list_type;
+
+
+                /**
+                   Creates a new node with an empty name() and an
+                   class_name() of "s11n::s11n_node". This
+                   node is functionally useless until it's name is
+                   set, as nodes with empty names are not supported by
+                   any current i/o parsers.
+                */
+                s11n_node();
+
+                /**
+                   Creates a new node with the given name() and an
+                   class_name() of "s11n::s11n_node".
+                */
+		explicit s11n_node( const std::string & name );
+
+                /**
+                   Creates a new node with the given name() and and class_name().
+
+                   Does not throw.
+                */
+                s11n_node( const std::string & name, const std::string implclass );
+
+                /**
+                   Destroys all child objects owned by this object, freeing up
+                   their resources.
+
+                   Does not throw.
+                */
+                ~s11n_node();
+
+		/**
+		   Swaps all publically-visible internal state with
+		   rhs. This includes:
+
+		   - class_name()
+		   - name()
+		   - children()
+		   - properties()
+
+		   Complexity is, in theory, constant time.  For all
+		   data we use their member swap() implementations,
+		   which should be constant-time for the
+		   containers. The C++ Standard apparently guarantees
+		   O(1) swap() for strings, too.  (Josuttis, The C++
+		   Standard Library, section 11.2.8, page 490.)
+
+		   Added in version 1.1.3.
+		*/
+		void swap( s11n_node & rhs );
+
+                /**
+                   Copies the properties, name, class name and
+                   children of rhs. If rhs is this object then this
+                   function does nothing.
+
+                   Does not throw.
+                */
+                s11n_node & operator=( const s11n_node & rhs );
+
+                /**
+                   See copy().
+
+                   Does not throw.
+                */
+                s11n_node( const s11n_node & rhs );
+
+		/**
+                   Returns a list of the s11n_node children of this
+                   object. The caller should not delete any pointers
+                   from this list unless he also removes the pointers
+                   from the list, or else they will get double-deleted
+                   later. In practice it is (almost) never necessary
+                   for client code to manipulate this list directly.
+                */
+                child_list_type & children();
+
+                /**
+                   The const form of children().
+                 */
+                const child_list_type & children() const;
+
+
+                /**
+                   Removes all properties and deletes all children from
+                   this object, freeing up their resources.
+                   
+                   Any pointers to children of this object become
+                   invalided by a call to this function (they get
+                   deleted).
+                */
+                void clear();
+
+
+                /**
+                   Defines the class name which should be used as the
+                   implementation class when this node is
+                   deserialize()d.
+
+                   Client Serializable types should call this one time
+                   from their serialize() method, <em>after</em> calling
+                   the parent class' serialize() method (if indeed that
+                   is called at all), passing it the name of their class,
+                   <em>using the name expected by the classloader</em>. By convention
+                   the class name is the same as it's C++ name, thus Serializable
+                   class foo::FooBar should call:
+
+<pre>
+node.class_name( "foo::FooBar" );
+</pre>
+
+		  from it's serialize() function.
+
+
+                  If classes to not set this then the serialized data
+                  will not have a proper implementation class
+                  name. That is likely to break deserialization.
+
+		  TODO: consider returning the old value,
+		  to simplify swap() operations.
+
+		  Added in 1.1.3.
+                */
+		void class_name( const std::string & n );
+
+
+                /**
+                   Returns the implementation class name set via
+                   class_name().
+                */
+                std::string class_name() const;
+
+		/**
+                   The name which should be used as the key for
+                   storing the node. This is normally translated to
+                   something like an XML element name (e.g., &lt;name&gt;),
+                   and should not contain spaces or other characters
+                   which may not be usable as key names. To be safe,
+                   stick to alphanumeric and underscores, starting
+                   with a letter or underscore. (This class does no
+                   enforce any naming conventions, but your data file
+                   parsers very well may.)
+                */
+		void name( const std::string & n );
+
+		/**
+                   Returns this node's name, as set via name(string).
+                */
+		std::string name() const;
+
+		/**
+		   Returns true if this object has no properties
+		   and no children. The name() and class_name()
+		   are *not* considered.
+		*/
+		bool empty() const;
+
+
+		/**
+                   Lexically casts val to a string and stores it as a
+                   property. If this type conversion is not possible
+                   it will fail at compile time. A value-conversion
+                   failure, on the other hand, is not caught at
+                   compile time. T must support complementary
+                   ostream<< and istream>> operators.
+                 */
+                template < typename T >
+                void set( const std::string & key, const T & val )
+		{
+			this->m_map[key] = ::s11n::Detail::variant(val).str();
+		}
+
+		/**
+                   Tries to get a property named key and lexically
+                   cast it to type T. If this type conversion is not
+                   possible it will fail at compile time. A
+                   value-conversion failure, on the other hand, is not
+                   caught at compile time. If value conversion fails,
+                   or if the requested property is not set, then
+                   defaultval is returned. This can be interpretted as
+                   an error value if the client so chooses, and it is
+                   often helpful to pass a known-invalid value here
+                   for that purpose.
+
+                 */
+		template < typename T >
+                T get( const std::string & key, const T & defaultval ) const
+		{
+                        map_type::const_iterator cit = this->m_map.find( key );
+                        return ( this->m_map.end() == cit ) ? defaultval : ::s11n::Detail::variant( (*cit).second ).cast_to(defaultval);
+		}
+
+                /**
+                   Returns true if this object contains the given
+                   property, else false.
+                */
+		bool is_set( const std::string & key ) const;
+
+                /**
+                   Removes the given property from this object.
+                */
+		void unset( const std::string & key );
+
+		/**
+		   Returns the map of properties contained by this
+		   node.
+		*/
+                map_type & properties();
+
+		/** Const overload. */
+                const map_type & properties() const;
+
+        private:
+		std::string m_name; // name of this node
+		std::string m_iname; // class_name name of this node
+		map_type m_map; // stores key/value properties.
+		child_list_type m_children; // holds child pointers
+
+                /**
+                   Copies all properties and child s11n_nodes from
+                   rhs into this object, as well as any other details
+                   which need to be copied.
+
+                   This can be a very expensive operation, and is rarely
+                   necessary.
+                */
+                void copy( const s11n_node & rhs );
+
+		/**
+                   Removes all property entries from this object.
+                 */
+		void clear_properties();
+
+		/**
+                   Removes all children from this object, deleting all
+                   child pointers.
+                 */
+                void clear_children();
 
-#endif  // GTEST_INCLUDE_GTEST_GTEST_MESSAGE_H_
+	}; // class s11n_node
+
+} // namespace s11n
+
+#endif // s11n_S11N_NODE_HPP_INCLUDED
```

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/abstract_creator.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/abstract_creator.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/algo.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/algo.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/algo.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/algo.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/classload.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/classload.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/classload.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/classload.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/client_api.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/client_api.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/exception.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/exception.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/export.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/export.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/factory.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/factory.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/factory_reg.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/factory_reg.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/functional.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/functional.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/FlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/FlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/compact_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/compact_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_format.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_format.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_io.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/data_node_io.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/expat_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/expat_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funtxt_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/funxml_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/parens_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/parens_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/reg_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/reg_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/serializers.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/serializers.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/simplexml_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/strtool.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/strtool.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/io/wesnoth_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/micro_api.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/micro_api.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/nodeutil/node_tree.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/nodeutil/node_tree.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/phoenix.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/phoenix.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/path_finder.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/path_finder.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin_config.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/plugin/plugin_config.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/listish.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/mapish.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/path_finder_s11n.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/path_finder_s11n.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/size_t.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/pod/size_t.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_list_specializations.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_list_specializations.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_map_specializations.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_map_specializations.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_node_type.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_node_type.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template3.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template3.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template4.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/reg_s11n_traits_template4.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/multiset.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/multiset.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/pair.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/pair.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/set.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/set.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/valarray.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/proxy/std/valarray.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/reg_s11n_traits.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/reg_s11n_traits.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n_config.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n_config.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n_debuggering_macros.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n_debuggering_macros.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11n_node.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11n_node.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/s11nlite.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/s11nlite.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/serialize.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/serialize.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/serialize.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/serialize.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/simple_config.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/simple_config.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/tags.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/tags.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/traits.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/traits.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/type_traits.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/include/s11n.net/s11n/variant.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/include/s11n.net/s11n/variant.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/Makefile` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/Makefile`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/argv_parser.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/argv_parser.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/argv_parser.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/argv_parser.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/compact.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/compact.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/compact_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/compact_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/data_node_io.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/data_node_io.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/exception.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/exception.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/expat_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/expat_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/export.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/export.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funtxt.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/funtxt.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funtxt_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/funtxt_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funxml.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/funxml.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/funxml_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/funxml_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/main.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/main.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/parens.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/parens.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/parens_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/parens_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/path_finder.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/path_finder.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.dl.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.dl.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.noop.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.noop.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/plugin.win32.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/plugin.win32.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/s11n.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/s11n.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/s11n_node.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/s11n_node.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/s11nlite.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/s11nlite.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/simplexml.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/simplexml.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/simplexml_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/simplexml_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/strtool.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/strtool.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/wesnoth.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/wesnoth.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/src/wesnoth_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/src/wesnoth_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/abstract_creator.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/abstract_creator.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/algo.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/classload.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/client_api.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/client_api.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/exception.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/exception.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/export.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/export.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/factory.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/factory.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/factory_reg.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/factory_reg.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/functional.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/functional.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/FlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/FlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/compact_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_format.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_format.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_io.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/data_node_io.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funtxt_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/funxml_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/parens_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/reg_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/reg_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/serializers.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/serializers.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/simplexml_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/strtool.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/strtool.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_data_nodeFlexLexer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_serializer.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/io/wesnoth_serializer.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/micro_api.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/micro_api.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/nodeutil/node_tree.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/nodeutil/node_tree.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/phoenix.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/phoenix.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/path_finder.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/path_finder.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin_config.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/plugin/plugin_config.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/listish.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/mapish.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/path_finder_s11n.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/path_finder_s11n.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_list_specializations.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_list_specializations.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_map_specializations.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_map_specializations.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_node_type.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_node_type.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template1.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/reg_s11n_traits_template2.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/multiset.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/multiset.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/pair.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/pair.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/set.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/set.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/valarray.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/proxy/std/valarray.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/reg_s11n_traits.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/reg_s11n_traits.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_config.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_config.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_debuggering_macros.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11n_debuggering_macros.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/s11nlite.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/s11nlite.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.tpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/serialize.tpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/simple_config.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/simple_config.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/tags.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/tags.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/traits.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/traits.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/type_traits.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/include/s11n.net/s11n/variant.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/include/s11n.net/s11n/variant.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/argv_parser.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/argv_parser.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/argv_parser.hpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/argv_parser.hpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/compact.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/compact.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/compact_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/compact_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/data_node_io.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/data_node_io.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/exception.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/exception.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funtxt.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funtxt.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funtxt_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funtxt_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funxml.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funxml.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/funxml_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/funxml_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/main.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/main.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/parens.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/parens.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/parens_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/parens_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/path_finder.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/path_finder.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/plugin.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/plugin.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/plugin.win32.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/plugin.win32.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/s11n.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/s11n.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/s11n_node.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/s11n_node.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/s11nlite.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/s11nlite.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/simplexml.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/simplexml.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/simplexml_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/simplexml_serializer.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/strtool.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/strtool.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/wesnoth.flex.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/wesnoth.flex.cpp`

 * *Files identical despite different names*

### Comparing `commonroad-drivability-checker-2022.2.1/third_party/libs11n/windows/src/wesnoth_serializer.cpp` & `commonroad-drivability-checker-2023.1/third_party/libs11n/windows/src/wesnoth_serializer.cpp`

 * *Files identical despite different names*

