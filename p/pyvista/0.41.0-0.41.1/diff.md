# Comparing `tmp/pyvista-0.41.0.tar.gz` & `tmp/pyvista-0.41.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-0.41.0.tar", last modified: Wed Jul 19 22:35:15 2023, max compression
+gzip compressed data, was "pyvista-0.41.1.tar", last modified: Fri Jul 21 15:58:03 2023, max compression
```

## Comparing `pyvista-0.41.0.tar` & `pyvista-0.41.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.335841 pyvista-0.41.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-19 22:16:56.000000 pyvista-0.41.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-07-19 22:16:56.000000 pyvista-0.41.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-07-19 22:16:56.000000 pyvista-0.41.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-07-19 22:35:15.335841 pyvista-0.41.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-07-19 22:16:56.000000 pyvista-0.41.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.311840 pyvista-0.41.0/pyvista/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2752 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9834 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.315840 pyvista-0.41.0/pyvista/core/
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/_typing_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    11188 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/_vtk_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    15161 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/cell.py
--rw-r--r--   0 runner    (1001) docker     (122)     4818 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/celltype.py
--rw-r--r--   0 runner    (1001) docker     (122)    41117 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/composite.py
--rw-r--r--   0 runner    (1001) docker     (122)    21474 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (122)   104875 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    44167 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/datasetattributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.315840 pyvista-0.41.0/pyvista/core/filters/
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/composite.py
--rw-r--r--   0 runner    (1001) docker     (122)   214933 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/data_set.py
--rw-r--r--   0 runner    (1001) docker     (122)    29701 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/image_data.py
--rw-r--r--   0 runner    (1001) docker     (122)   133756 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/poly_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/rectilinear_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/structured_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/filters/unstructured_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    28301 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    10033 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)   100028 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4156 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/pyvista_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.319841 pyvista-0.41.0/pyvista/core/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21123 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/cell_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     7695 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    16425 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    20591 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)    51282 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     8697 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8747 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/observers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36453 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/parametric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    11670 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (122)    74674 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     9442 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/utilities/transformations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/core/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.319841 pyvista-0.41.0/pyvista/demos/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15906 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/demos/demos.py
--rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/demos/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.323840 pyvista-0.41.0/pyvista/examples/
--rw-r--r--   0 runner    (1001) docker     (122)   463087 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/2k_earth_daymap.jpg
--rwxr-xr-x   0 runner    (1001) docker     (122)      157 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    74547 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/airplane.ply
--rw-r--r--   0 runner    (1001) docker     (122)    17941 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/ant.ply
--rw-r--r--   0 runner    (1001) docker     (122)    21542 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)   522284 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/channels.vti
--rw-r--r--   0 runner    (1001) docker     (122)   150564 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/downloads.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11928 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (122)    37447 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/globe.vtk
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/gltf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/hexbeam.vtk
--rw-r--r--   0 runner    (1001) docker     (122)    20128 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/nut.ply
--rw-r--r--   0 runner    (1001) docker     (122)    27139 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/planets.py
--rw-r--r--   0 runner    (1001) docker     (122)   228473 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/rectilinear.vtk
--rw-r--r--   0 runner    (1001) docker     (122)    16237 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/sphere.ply
--rw-r--r--   0 runner    (1001) docker     (122)    14094 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/uniform.vtk
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/examples/vrml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.323840 pyvista-0.41.0/pyvista/ext/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16136 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/ext/coverage.py
--rw-r--r--   0 runner    (1001) docker     (122)    18247 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/ext/plot_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/ext/viewer_directive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.323840 pyvista-0.41.0/pyvista/jupyter/
--rw-r--r--   0 runner    (1001) docker     (122)     7442 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5210 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/jupyter/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/jupyter/pv_ipygany.py
--rw-r--r--   0 runner    (1001) docker     (122)    22787 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/jupyter/pv_pythreejs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.327840 pyvista-0.41.0/pyvista/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)    34433 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/_property.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/_vtk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/_vtk_gl.py
--rw-r--r--   0 runner    (1001) docker     (122)    12924 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/actor_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)    14662 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/background_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/camera.py
--rw-r--r--   0 runner    (1001) docker     (122)   140615 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/charts.py
--rw-r--r--   0 runner    (1001) docker     (122)    38863 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)    28732 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/composite_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/cube_axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3993 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    41365 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/lights.py
--rw-r--r--   0 runner    (1001) docker     (122)    34948 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    35265 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/opts.py
--rw-r--r--   0 runner    (1001) docker     (122)    70008 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/picking.py
--rw-r--r--   0 runner    (1001) docker     (122)   251604 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.331841 pyvista-0.41.0/pyvista/plotting/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6584 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/prop3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     9135 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/render_passes.py
--rw-r--r--   0 runner    (1001) docker     (122)    40862 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/render_window_interactor.py
--rw-r--r--   0 runner    (1001) docker     (122)   122642 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)    21771 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    19509 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/scalar_bars.py
--rw-r--r--   0 runner    (1001) docker     (122)    21106 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/texture.py
--rw-r--r--   0 runner    (1001) docker     (122)    87822 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/themes.py
--rw-r--r--   0 runner    (1001) docker     (122)    20170 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.331841 pyvista-0.41.0/pyvista/plotting/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11491 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)     3413 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/cubemap.py
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/gl_checks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6012 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     4507 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/utilities/xvfb.py
--rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/volume.py
--rw-r--r--   0 runner    (1001) docker     (122)    12571 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/volume_property.py
--rw-r--r--   0 runner    (1001) docker     (122)    87428 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.331841 pyvista-0.41.0/pyvista/trame/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/trame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11359 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/trame/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (122)    18755 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/trame/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     8439 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/trame/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.335841 pyvista-0.41.0/pyvista/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/cell_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/features.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/parametric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/transformations.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-19 22:16:57.000000 pyvista-0.41.0/pyvista/utilities/xvfb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.311840 pyvista-0.41.0/pyvista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-07-19 22:35:15.000000 pyvista-0.41.0/pyvista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4540 2023-07-19 22:35:15.000000 pyvista-0.41.0/pyvista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 22:35:15.000000 pyvista-0.41.0/pyvista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-07-19 22:35:15.000000 pyvista-0.41.0/pyvista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-19 22:35:15.000000 pyvista-0.41.0/pyvista.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 22:35:15.335841 pyvista-0.41.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-19 22:16:57.000000 pyvista-0.41.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 22:35:15.335841 pyvista-0.41.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-19 22:16:57.000000 pyvista-0.41.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-07-19 22:16:57.000000 pyvista-0.41.0/tests/test_meshio.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-19 22:16:57.000000 pyvista-0.41.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-19 22:16:57.000000 pyvista-0.41.0/tests/test_tinypages.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.669719 pyvista-0.41.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-21 15:37:40.000000 pyvista-0.41.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-07-21 15:37:40.000000 pyvista-0.41.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-07-21 15:37:40.000000 pyvista-0.41.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-07-21 15:58:03.669719 pyvista-0.41.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-07-21 15:37:40.000000 pyvista-0.41.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.605719 pyvista-0.41.1/pyvista/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2752 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9834 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.613719 pyvista-0.41.1/pyvista/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/_typing_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11188 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/_vtk_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15161 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/cell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4818 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/celltype.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41117 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21474 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104875 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44167 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/datasetattributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.617719 pyvista-0.41.1/pyvista/core/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)   214933 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29701 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/image_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)   133756 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/poly_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/rectilinear_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/structured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/filters/unstructured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28301 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10033 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)   100028 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4156 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/pyvista_ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.625719 pyvista-0.41.1/pyvista/core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21123 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/cell_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7695 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16425 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20591 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51282 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8697 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8747 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/observers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36453 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/parametric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11670 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74674 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9442 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/utilities/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/core/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.625719 pyvista-0.41.1/pyvista/demos/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15906 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/demos/demos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/demos/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.633719 pyvista-0.41.1/pyvista/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)   463087 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/2k_earth_daymap.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      157 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74547 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/airplane.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    17941 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/ant.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    21542 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)   522284 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/channels.vti
+-rw-r--r--   0 runner    (1001) docker     (122)   150564 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/downloads.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11928 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37447 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/globe.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/hexbeam.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)    20128 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/nut.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    27139 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/planets.py
+-rw-r--r--   0 runner    (1001) docker     (122)   228473 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/rectilinear.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)    16237 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/sphere.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    14094 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/uniform.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/examples/vrml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.637719 pyvista-0.41.1/pyvista/ext/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16136 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/ext/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18247 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/ext/plot_directive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/ext/viewer_directive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.637719 pyvista-0.41.1/pyvista/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (122)     7442 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5210 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/jupyter/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/jupyter/pv_ipygany.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22787 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/jupyter/pv_pythreejs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.653719 pyvista-0.41.1/pyvista/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34433 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/_vtk_gl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12924 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/actor_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14662 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/background_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)   140615 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/charts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38863 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28732 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/composite_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/cube_axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3993 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41365 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/lights.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34948 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35265 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/opts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70008 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/picking.py
+-rw-r--r--   0 runner    (1001) docker     (122)   251613 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.657719 pyvista-0.41.1/pyvista/plotting/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6584 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/prop3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9135 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/render_passes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40862 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/render_window_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (122)   122642 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21771 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19509 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/scalar_bars.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21106 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/texture.py
+-rw-r--r--   0 runner    (1001) docker     (122)    87822 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/themes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20170 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.657719 pyvista-0.41.1/pyvista/plotting/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11491 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3413 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/cubemap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/gl_checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6012 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4507 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/utilities/xvfb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12571 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/volume_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)    87428 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.661719 pyvista-0.41.1/pyvista/trame/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/trame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11338 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/trame/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18755 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/trame/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8663 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/trame/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.669719 pyvista-0.41.1/pyvista/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/cell_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/parametric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-21 15:37:41.000000 pyvista-0.41.1/pyvista/utilities/xvfb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.605719 pyvista-0.41.1/pyvista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-07-21 15:58:03.000000 pyvista-0.41.1/pyvista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4540 2023-07-21 15:58:03.000000 pyvista-0.41.1/pyvista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:58:03.000000 pyvista-0.41.1/pyvista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-07-21 15:58:03.000000 pyvista-0.41.1/pyvista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-21 15:58:03.000000 pyvista-0.41.1/pyvista.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 15:58:03.669719 pyvista-0.41.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-21 15:37:41.000000 pyvista-0.41.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:58:03.669719 pyvista-0.41.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-21 15:37:41.000000 pyvista-0.41.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-07-21 15:37:41.000000 pyvista-0.41.1/tests/test_meshio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-21 15:37:41.000000 pyvista-0.41.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-21 15:37:41.000000 pyvista-0.41.1/tests/test_tinypages.py
```

### Comparing `pyvista-0.41.0/AUTHORS.rst` & `pyvista-0.41.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/LICENSE` & `pyvista-0.41.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/PKG-INFO` & `pyvista-0.41.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.41.0
+Version: 0.41.1
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.41.0/README.rst` & `pyvista-0.41.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyproject.toml` & `pyvista-0.41.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,22 @@
 jupyter = [
     'ipyvtklink',
     'ipywidgets',
     'jupyter-server-proxy',
     'nest_asyncio',
     'panel',
     'pythreejs',
-    'trame>=2.5.0',
-    'trame-client>=2.9.4',
-    'trame-server>=2.11.4',
-    'trame-vtk>=2.5.3',
+    'trame>=2.5.2',
+    'trame-vuetify>=2.3.1',
+    'trame-vtk>=2.5.8',
 ]
 trame = [
-    'trame>=2.5.0',
-    'trame-client>=2.9.4',
-    'trame-server>=2.11.4',
-    'trame-vtk>=2.5.3',
+    'trame>=2.5.2',
+    'trame-vuetify>=2.3.1',
+    'trame-vtk>=2.5.8',
 ]
 
 [project.urls]
 Documentation = 'https://docs.pyvista.org/'
 "Bug Tracker" = 'https://github.com/pyvista/pyvista/issues'
 "Source Code" = 'https://github.com/pyvista/pyvista'
```

### Comparing `pyvista-0.41.0/pyvista/__init__.py` & `pyvista-0.41.1/pyvista/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/_plot.py` & `pyvista-0.41.1/pyvista/_plot.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/__init__.py` & `pyvista-0.41.1/pyvista/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/_vtk_core.py` & `pyvista-0.41.1/pyvista/core/_vtk_core.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/cell.py` & `pyvista-0.41.1/pyvista/core/cell.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/celltype.py` & `pyvista-0.41.1/pyvista/core/celltype.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/composite.py` & `pyvista-0.41.1/pyvista/core/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/dataobject.py` & `pyvista-0.41.1/pyvista/core/dataobject.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/dataset.py` & `pyvista-0.41.1/pyvista/core/dataset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/datasetattributes.py` & `pyvista-0.41.1/pyvista/core/datasetattributes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/errors.py` & `pyvista-0.41.1/pyvista/core/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/__init__.py` & `pyvista-0.41.1/pyvista/core/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/composite.py` & `pyvista-0.41.1/pyvista/core/filters/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/data_set.py` & `pyvista-0.41.1/pyvista/core/filters/data_set.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/image_data.py` & `pyvista-0.41.1/pyvista/core/filters/image_data.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/poly_data.py` & `pyvista-0.41.1/pyvista/core/filters/poly_data.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/rectilinear_grid.py` & `pyvista-0.41.1/pyvista/core/filters/rectilinear_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/structured_grid.py` & `pyvista-0.41.1/pyvista/core/filters/structured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/filters/unstructured_grid.py` & `pyvista-0.41.1/pyvista/core/filters/unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/grid.py` & `pyvista-0.41.1/pyvista/core/grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/objects.py` & `pyvista-0.41.1/pyvista/core/objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/pointset.py` & `pyvista-0.41.1/pyvista/core/pointset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/pyvista_ndarray.py` & `pyvista-0.41.1/pyvista/core/pyvista_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/__init__.py` & `pyvista-0.41.1/pyvista/core/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/arrays.py` & `pyvista-0.41.1/pyvista/core/utilities/arrays.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/cell_type_helper.py` & `pyvista-0.41.1/pyvista/core/utilities/cell_type_helper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/cells.py` & `pyvista-0.41.1/pyvista/core/utilities/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/docs.py` & `pyvista-0.41.1/pyvista/core/utilities/docs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/features.py` & `pyvista-0.41.1/pyvista/core/utilities/features.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/fileio.py` & `pyvista-0.41.1/pyvista/core/utilities/fileio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/geometric_objects.py` & `pyvista-0.41.1/pyvista/core/utilities/geometric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/helpers.py` & `pyvista-0.41.1/pyvista/core/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/misc.py` & `pyvista-0.41.1/pyvista/core/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/observers.py` & `pyvista-0.41.1/pyvista/core/utilities/observers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/parametric_objects.py` & `pyvista-0.41.1/pyvista/core/utilities/parametric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/points.py` & `pyvista-0.41.1/pyvista/core/utilities/points.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/reader.py` & `pyvista-0.41.1/pyvista/core/utilities/reader.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/utilities/transformations.py` & `pyvista-0.41.1/pyvista/core/utilities/transformations.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/core/wrappers.py` & `pyvista-0.41.1/pyvista/core/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/demos/demos.py` & `pyvista-0.41.1/pyvista/demos/demos.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/demos/logo.py` & `pyvista-0.41.1/pyvista/demos/logo.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/errors.py` & `pyvista-0.41.1/pyvista/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/2k_earth_daymap.jpg` & `pyvista-0.41.1/pyvista/examples/2k_earth_daymap.jpg`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/airplane.ply` & `pyvista-0.41.1/pyvista/examples/airplane.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/ant.ply` & `pyvista-0.41.1/pyvista/examples/ant.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/cells.py` & `pyvista-0.41.1/pyvista/examples/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/channels.vti` & `pyvista-0.41.1/pyvista/examples/channels.vti`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/downloads.py` & `pyvista-0.41.1/pyvista/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/examples.py` & `pyvista-0.41.1/pyvista/examples/examples.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/globe.vtk` & `pyvista-0.41.1/pyvista/examples/globe.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/gltf.py` & `pyvista-0.41.1/pyvista/examples/gltf.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/hexbeam.vtk` & `pyvista-0.41.1/pyvista/examples/hexbeam.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/nut.ply` & `pyvista-0.41.1/pyvista/examples/nut.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/planets.py` & `pyvista-0.41.1/pyvista/examples/planets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/rectilinear.vtk` & `pyvista-0.41.1/pyvista/examples/rectilinear.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/sphere.ply` & `pyvista-0.41.1/pyvista/examples/sphere.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/uniform.vtk` & `pyvista-0.41.1/pyvista/examples/uniform.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/examples/vrml.py` & `pyvista-0.41.1/pyvista/examples/vrml.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/ext/coverage.py` & `pyvista-0.41.1/pyvista/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/ext/plot_directive.py` & `pyvista-0.41.1/pyvista/ext/plot_directive.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/ext/viewer_directive.py` & `pyvista-0.41.1/pyvista/ext/viewer_directive.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/jupyter/__init__.py` & `pyvista-0.41.1/pyvista/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/jupyter/notebook.py` & `pyvista-0.41.1/pyvista/jupyter/notebook.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/jupyter/pv_ipygany.py` & `pyvista-0.41.1/pyvista/jupyter/pv_ipygany.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/jupyter/pv_pythreejs.py` & `pyvista-0.41.1/pyvista/jupyter/pv_pythreejs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/__init__.py` & `pyvista-0.41.1/pyvista/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/_plotting.py` & `pyvista-0.41.1/pyvista/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/_property.py` & `pyvista-0.41.1/pyvista/plotting/_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/_typing.py` & `pyvista-0.41.1/pyvista/plotting/_typing.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/_vtk.py` & `pyvista-0.41.1/pyvista/plotting/_vtk.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/_vtk_gl.py` & `pyvista-0.41.1/pyvista/plotting/_vtk_gl.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/actor.py` & `pyvista-0.41.1/pyvista/plotting/actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/actor_properties.py` & `pyvista-0.41.1/pyvista/plotting/actor_properties.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/axes.py` & `pyvista-0.41.1/pyvista/plotting/axes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/axes_actor.py` & `pyvista-0.41.1/pyvista/plotting/axes_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/background_renderer.py` & `pyvista-0.41.1/pyvista/plotting/background_renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/camera.py` & `pyvista-0.41.1/pyvista/plotting/camera.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/charts.py` & `pyvista-0.41.1/pyvista/plotting/charts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/colors.py` & `pyvista-0.41.1/pyvista/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/composite_mapper.py` & `pyvista-0.41.1/pyvista/plotting/composite_mapper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/cube_axes_actor.py` & `pyvista-0.41.1/pyvista/plotting/cube_axes_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/errors.py` & `pyvista-0.41.1/pyvista/plotting/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/helpers.py` & `pyvista-0.41.1/pyvista/plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/lights.py` & `pyvista-0.41.1/pyvista/plotting/lights.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/lookup_table.py` & `pyvista-0.41.1/pyvista/plotting/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/mapper.py` & `pyvista-0.41.1/pyvista/plotting/mapper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/opts.py` & `pyvista-0.41.1/pyvista/plotting/opts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/picking.py` & `pyvista-0.41.1/pyvista/plotting/picking.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/plotter.py` & `pyvista-0.41.1/pyvista/plotting/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,18 +554,17 @@
         Returns
         -------
         str
             The exported filename.
 
         """
         try:
-            from trame.app import get_server
-
             from pyvista.trame import PyVistaLocalView
             from pyvista.trame.jupyter import elegantly_launch
+            from pyvista.trame.views import get_server
         except ImportError:  # pragma: no cover
             raise ImportError('Please install trame to export')
 
         # Ensure trame server is launched
         server = get_server(pyvista.global_theme.trame.jupyter_server_name)
         if not server.running:
             elegantly_launch(pyvista.global_theme.trame.jupyter_server_name)
```

### Comparing `pyvista-0.41.0/pyvista/plotting/plotting/__init__.py` & `pyvista-0.41.1/pyvista/plotting/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/prop3d.py` & `pyvista-0.41.1/pyvista/plotting/prop3d.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/render_passes.py` & `pyvista-0.41.1/pyvista/plotting/render_passes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/render_window_interactor.py` & `pyvista-0.41.1/pyvista/plotting/render_window_interactor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/renderer.py` & `pyvista-0.41.1/pyvista/plotting/renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/renderers.py` & `pyvista-0.41.1/pyvista/plotting/renderers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/scalar_bars.py` & `pyvista-0.41.1/pyvista/plotting/scalar_bars.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/texture.py` & `pyvista-0.41.1/pyvista/plotting/texture.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/themes.py` & `pyvista-0.41.1/pyvista/plotting/themes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/tools.py` & `pyvista-0.41.1/pyvista/plotting/tools.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/__init__.py` & `pyvista-0.41.1/pyvista/plotting/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/algorithms.py` & `pyvista-0.41.1/pyvista/plotting/utilities/algorithms.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/cubemap.py` & `pyvista-0.41.1/pyvista/plotting/utilities/cubemap.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/gl_checks.py` & `pyvista-0.41.1/pyvista/plotting/utilities/gl_checks.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/regression.py` & `pyvista-0.41.1/pyvista/plotting/utilities/regression.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/sphinx_gallery.py` & `pyvista-0.41.1/pyvista/plotting/utilities/sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/utilities/xvfb.py` & `pyvista-0.41.1/pyvista/plotting/utilities/xvfb.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/volume.py` & `pyvista-0.41.1/pyvista/plotting/volume.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/volume_property.py` & `pyvista-0.41.1/pyvista/plotting/volume_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/plotting/widgets.py` & `pyvista-0.41.1/pyvista/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/report.py` & `pyvista-0.41.1/pyvista/report.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/trame/jupyter.py` & `pyvista-0.41.1/pyvista/trame/jupyter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Trame utilities for running in Jupyter."""
 import asyncio
 import logging
 import os
 import warnings
 
-from trame.app import get_server
 from trame.ui.vuetify import VAppLayout
 from trame.widgets import html as html_widgets, vtk as vtk_widgets, vuetify as vuetify_widgets
 
 try:
     from ipywidgets.widgets import HTML
 except ImportError:
     HTML = object
 
 
 import pyvista
 from pyvista.trame.ui import UI_TITLE, get_or_create_viewer
-from pyvista.trame.views import CLOSED_PLOTTER_ERROR
+from pyvista.trame.views import CLOSED_PLOTTER_ERROR, get_server
 
 SERVER_DOWN_MESSAGE = """Trame server has not launched.
 
 You must start the trame server before attempting to `show()`
 with PyVista.
 
 You can use the following snippet to launch the server:
```

### Comparing `pyvista-0.41.0/pyvista/trame/ui.py` & `pyvista-0.41.1/pyvista/trame/ui.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista/trame/views.py` & `pyvista-0.41.1/pyvista/trame/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 """Trame view interface for PyVista."""
 import io
 import weakref
 
+from trame.app import get_server as trame_get_server
 from trame.widgets.vtk import VtkLocalView, VtkRemoteLocalView, VtkRemoteView
 from trame_vtk.tools.vtksz2html import write_html
 
 CLOSED_PLOTTER_ERROR = "The render window for this plotter has been destroyed. Do not call `show()` for the plotter before passing to trame."
 
 
+def get_server(*args, **kwargs):
+    """Override trame's get_server."""
+    server = trame_get_server(*args, **kwargs)
+    server.client_type = 'vue2'
+    return server
+
+
 class _BasePyVistaView:
     def __init__(self, plotter):
         self._plotter = weakref.ref(plotter)
         self.pyvista_initialize()
         self._plotter_render_callback = lambda *args: self.update()
 
     def pyvista_initialize(self):
```

### Comparing `pyvista-0.41.0/pyvista/utilities/__init__.py` & `pyvista-0.41.1/pyvista/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/pyvista.egg-info/PKG-INFO` & `pyvista-0.41.1/pyvista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.41.0
+Version: 0.41.1
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.41.0/pyvista.egg-info/SOURCES.txt` & `pyvista-0.41.1/pyvista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/tests/test_init.py` & `pyvista-0.41.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/tests/test_meshio.py` & `pyvista-0.41.1/tests/test_meshio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.41.0/tests/test_tinypages.py` & `pyvista-0.41.1/tests/test_tinypages.py`

 * *Files identical despite different names*

