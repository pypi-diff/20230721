# Comparing `tmp/cipher_parse-0.5.1a0.tar.gz` & `tmp/cipher_parse-0.5.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipher_parse-0.5.1a0.tar", max compression
+gzip compressed data, was "cipher_parse-0.5.1a1.tar", max compression
```

## Comparing `cipher_parse-0.5.1a0.tar` & `cipher_parse-0.5.1a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/LICENSE
--rw-r--r--   0        0        0      807 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/README.md
--rw-r--r--   0        0        0      280 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/__init__.py
--rw-r--r--   0        0        0       24 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/_version.py
--rw-r--r--   0        0        0    28011 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/cipher_input.py
--rw-r--r--   0        0        0    36114 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/cipher_output.py
--rw-r--r--   0        0        0      384 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/derived_outputs.py
--rw-r--r--   0        0        0    11603 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/discrete_voronoi.py
--rw-r--r--   0        0        0      603 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/errors.py
--rw-r--r--   0        0        0        0 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/example_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/__init__.py
--rw-r--r--   0        0        0   807612 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d
--rw-r--r--   0        0        0    19811 2023-06-01 12:37:35.726376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json
--rw-r--r--   0        0        0     2154 2023-06-01 12:37:35.726376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf
--rw-r--r--   0        0        0        0 2023-06-01 12:37:35.726376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/__init__.py
--rw-r--r--   0        0        0 10104120 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d
--rw-r--r--   0        0        0    19811 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json
--rw-r--r--   0        0        0     2160 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf
--rw-r--r--   0        0        0    47897 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/geometry.py
--rw-r--r--   0        0        0     5726 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/interface.py
--rw-r--r--   0        0        0     9770 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/material.py
--rw-r--r--   0        0        0     7286 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/quats.py
--rw-r--r--   0        0        0    20955 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/utilities.py
--rw-r--r--   0        0        0    12404 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/voxel_map.py
--rw-r--r--   0        0        0     1612 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/pyproject.toml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 cipher_parse-0.5.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-21 14:33:23.955546 cipher_parse-0.5.1a1/LICENSE
+-rw-r--r--   0        0        0      807 2023-07-21 14:33:23.955546 cipher_parse-0.5.1a1/README.md
+-rw-r--r--   0        0        0      280 2023-07-21 14:33:23.955546 cipher_parse-0.5.1a1/cipher_parse/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-21 14:33:23.955546 cipher_parse-0.5.1a1/cipher_parse/_version.py
+-rw-r--r--   0        0        0    28011 2023-07-21 14:33:23.955546 cipher_parse-0.5.1a1/cipher_parse/cipher_input.py
+-rw-r--r--   0        0        0    36114 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/cipher_output.py
+-rw-r--r--   0        0        0      384 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/derived_outputs.py
+-rw-r--r--   0        0        0    11603 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/discrete_voronoi.py
+-rw-r--r--   0        0        0      603 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/errors.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/example_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/__init__.py
+-rw-r--r--   0        0        0   807612 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d
+-rw-r--r--   0        0        0    19811 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json
+-rw-r--r--   0        0        0     2154 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf
+-rw-r--r--   0        0        0        0 2023-07-21 14:33:23.959546 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/__init__.py
+-rw-r--r--   0        0        0 10104120 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d
+-rw-r--r--   0        0        0    19811 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json
+-rw-r--r--   0        0        0     2160 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf
+-rw-r--r--   0        0        0    47158 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/geometry.py
+-rw-r--r--   0        0        0     5726 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/interface.py
+-rw-r--r--   0        0        0     9770 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/material.py
+-rw-r--r--   0        0        0     8453 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/quats.py
+-rw-r--r--   0        0        0    20955 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/utilities.py
+-rw-r--r--   0        0        0    12404 2023-07-21 14:33:23.987547 cipher_parse-0.5.1a1/cipher_parse/voxel_map.py
+-rw-r--r--   0        0        0     1631 2023-07-21 14:33:23.991547 cipher_parse-0.5.1a1/pyproject.toml
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 cipher_parse-0.5.1a1/PKG-INFO
```

### Comparing `cipher_parse-0.5.1a0/LICENSE` & `cipher_parse-0.5.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/README.md` & `cipher_parse-0.5.1a1/README.md`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/cipher_input.py` & `cipher_parse-0.5.1a1/cipher_parse/cipher_input.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/cipher_output.py` & `cipher_parse-0.5.1a1/cipher_parse/cipher_output.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/discrete_voronoi.py` & `cipher_parse-0.5.1a1/cipher_parse/discrete_voronoi.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/errors.py` & `cipher_parse-0.5.1a1/cipher_parse/errors.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d` & `cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json` & `cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf` & `cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d` & `cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json` & `cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf` & `cipher_parse-0.5.1a1/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/geometry.py` & `cipher_parse-0.5.1a1/cipher_parse/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     GeometryExcessTargetVolumeFractionError,
     GeometryMissingPhaseAssignmentError,
     GeometryNonUnitTargetVolumeFractionError,
     GeometryUnassignedPhasePairInterfaceError,
     GeometryVoxelPhaseError,
 )
 from cipher_parse.utilities import generate_interface_energies_plot
-from cipher_parse.quats import quat_angle_between
+from cipher_parse.quats import compute_misorientation_matrix, quat_angle_between
 
 
 class CIPHERGeometry:
     def __init__(
         self,
         materials,
         interfaces,
@@ -375,15 +375,14 @@
             self._assign_phases_by_volume_fractions(is_mat_vol_frac, random_seed)
 
     def _check_interface_phase_pairs(self):
         """If interfaces have phase-pairs specified, check these are consistent with
         the specified phases of associated material."""
 
         for i in self.interfaces:
-
             # assign materials as well as phase_types if materials not assigned to
             # interface:
             if not i.materials:
                 i_mats = []
                 # find which material each referenced phase type belongs to:
                 for j in i.phase_types:
                     mat_j = [k.material.name for k in self.phase_types if k.name == j][0]
@@ -518,15 +517,14 @@
         ints_by_phase_type_pair = {}
         for int_def in self.interfaces:
             if int_def.phase_types not in ints_by_phase_type_pair:
                 ints_by_phase_type_pair[int_def.phase_types] = []
             ints_by_phase_type_pair[int_def.phase_types].append(int_def)
 
         for pt_pair, int_defs in ints_by_phase_type_pair.items():
-
             names = [i.name for i in int_defs]
             if len(set(names)) < len(names):
                 raise ValueError(
                     f"Multiple interface definitions for phase-type pair "
                     f"{pt_pair} have the same `type_label`."
                 )
             type_fracs = [i.type_fraction for i in int_defs]
@@ -666,42 +664,24 @@
 
         if self.misorientation_matrix is not None and not overwrite:
             print(
                 "Misorientation matrix is already set. Use `overwrite=True` to recompute."
             )
             return
 
-        misori_matrix = np.zeros((self.num_phases, self.num_phases), dtype=float)
         all_oris = np.ones((self.num_phases, 4)) * np.nan
         for i in self.phase_types:
             all_oris[i.phases] = i.orientations
 
         if np.any(np.isnan(all_oris)):
             raise RuntimeError(
                 "Not all orientations are accounted for in the phase type definitions."
             )
 
-        all_oris = Orientation(all_oris, family="cubic")  # TODO: generalise symmetry
-
-        misori_matrix = np.zeros((self.num_phases, self.num_phases), dtype=float)
-        for idx in range(self.num_phases):
-            print(
-                f"Finding misorientation for orientation {idx + 1}/{len(all_oris)}",
-                flush=True,
-            )
-            ori_i = all_oris[idx : idx + 1]
-            other_oris = all_oris[idx + 1 :]
-            if other_oris.size:
-                disori_i = ori_i.disorientation(other_oris).as_axis_angle()[..., -1]
-                misori_matrix[idx, idx + 1 :] = disori_i
-                misori_matrix[idx + 1 :, idx] = disori_i
-
-        if degrees:
-            misori_matrix = np.rad2deg(misori_matrix)
-
+        misori_matrix = compute_misorientation_matrix(all_oris, degrees)
         self._misorientation_matrix = misori_matrix
         self._misorientation_matrix_is_degrees = degrees
 
         return misori_matrix
 
     def get_pyvista_grid(self):
         """Experimental!"""
@@ -724,15 +704,14 @@
     @staticmethod
     def assign_phase_material_randomly(
         num_materials,
         num_phases,
         volume_fractions,
         random_seed=None,
     ):
-
         print(
             "Randomly assigning phases to materials according to volume_fractions...",
             end="",
         )
         rng = np.random.default_rng(seed=random_seed)
         phase_material = rng.choice(
             a=num_materials,
@@ -750,15 +729,14 @@
         grid_size,
         size,
         seeds=None,
         num_phases=None,
         random_seed=None,
         is_periodic=False,
     ):
-
         if sum(i is not None for i in (seeds, num_phases)) != 1:
             raise ValueError(f"Specify exactly one of `seeds` and `num_phases`")
 
         if seeds is None:
             vor_map = DiscreteVoronoi.from_random(
                 num_regions=num_phases,
                 grid_size=grid_size,
@@ -876,15 +854,14 @@
         self,
         slice_index=0,
         normal_dir="z",
         data_label="phase",
         include=None,
         misorientation_matrix=None,
     ):
-
         allowed_data = [
             "phase",
             "material",
             "interface",
             "interface_idx",
             "phase_neighbours",
             "grain_boundaries",
@@ -935,15 +912,14 @@
         data_label="phase",
         include=None,
         phase_centroids=False,
         discrete_colours=None,
         layout_args=None,
         **kwargs,
     ):
-
         if "misorientation_matrix" in kwargs:
             slice_dat = self.get_slice(
                 slice_index,
                 normal_dir,
                 data_label,
                 include,
                 misorientation_matrix=kwargs.pop("misorientation_matrix"),
@@ -992,15 +968,14 @@
 
         # TODO: fix plotter to show multiple cell data
         pl = pv.Plotter(notebook=True)
         pl.add_mesh(grid)
         pl.show()
 
     def write_VTK(self, path):
-
         grid = self.get_pyvista_grid()
 
         grid.cell_data["interface_idx"] = self.voxel_interface_idx_3D.flatten(order="F")
         grid.cell_data["material"] = self.voxel_material_3D.flatten(order="F")
         grid.cell_data["phase"] = self.voxel_phase_3D.flatten(order="F")
 
         grid.save(path)
```

### Comparing `cipher_parse-0.5.1a0/cipher_parse/interface.py` & `cipher_parse-0.5.1a1/cipher_parse/interface.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/material.py` & `cipher_parse-0.5.1a1/cipher_parse/material.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/quats.py` & `cipher_parse-0.5.1a1/cipher_parse/quats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 
+from defdap.quat import Quat
+
 
 def quat_conjugate(quats_arr):
     quats_copy = np.copy(quats_arr)
     quats_copy[..., 1] *= -1
     quats_copy[..., 2] *= -1
     quats_copy[..., 3] *= -1
     return quats_copy
@@ -260,7 +262,43 @@
             np.sqrt(1 - rand_nums[:, 0]) * np.cos(2 * np.pi * rand_nums[:, 1]),
             np.sqrt(rand_nums[:, 0]) * np.sin(2 * np.pi * rand_nums[:, 2]),
             np.sqrt(rand_nums[:, 0]) * np.cos(2 * np.pi * rand_nums[:, 2]),
         ]
     ).T
 
     return quats
+
+
+def compute_misorientation_matrix(quat_comps, degrees=False, quiet=False):
+    """Use DefDAP to calculate an N-by-N symmetric matrix of disorientation angles between
+    an array of N quaternions.
+
+    Parameter
+    ---------
+    degrees
+        If True, return the misorientation array in degrees rather than radians.
+
+    """
+
+    num_quats = len(quat_comps)
+    quat_objs = np.empty(num_quats, dtype=Quat)
+
+    for i in range(len(quat_comps)):
+        quat_objs[i] = Quat(quat_comps[i])
+
+    quat_comps_sym = Quat.calcSymEqvs(quat_objs, "cubic")
+
+    misori_matrix = np.zeros((num_quats, num_quats))
+    for idx, ref_ori in enumerate(quat_objs):
+        if not quiet and idx % 100 == 0:
+            print(f"Finding misorientations {idx}/{num_quats}", flush=True)
+        misori, _ = Quat.calcMisOri(quat_comps_sym, ref_ori)
+        misori_matrix[:, idx] = 2 * np.arccos(misori)
+
+    # make precisely symmetric
+    misori_matrix = np.triu(misori_matrix)
+    misori_matrix = misori_matrix + misori_matrix.T - np.diag(np.diag(misori_matrix))
+
+    if degrees:
+        misori_matrix = np.rad2deg(misori_matrix)
+
+    return misori_matrix
```

### Comparing `cipher_parse-0.5.1a0/cipher_parse/utilities.py` & `cipher_parse-0.5.1a1/cipher_parse/utilities.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/cipher_parse/voxel_map.py` & `cipher_parse-0.5.1a1/cipher_parse/voxel_map.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.1a0/pyproject.toml` & `cipher_parse-0.5.1a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cipher-parse"
-version = "0.5.1a0"
+version = "0.5.1a1"
 description = "Pre- and post-processing for the phase-field code CIPHER."
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d",
     "cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d",
@@ -25,14 +25,15 @@
 notebook = {version = "^6.5.1", optional = true}
 pandas = "^1.5.1"
 parse = "^1.19.0"
 ipywidgets = "<8.0.0"
 sqlalchemy = {version = "<2.0.0", optional = true}
 pyvista = "^0.39.0"
 trame = "^2.4.2"
+defdap = "^0.93.5"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.12.2"
 ipykernel = "^6.6.1"
 pytest = "^6.2.5"
 commitizen = "^2.20.3"
 pre-commit = "^2.16.0"
@@ -45,15 +46,15 @@
 [tool.poetry.extras]
 hickle = ["hickle"]
 matflow = ["hickle", "matflow", "sqlalchemy"]
 notebook = ["notebook"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.1a0"
+version = "0.5.1a1"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "cipher_parse/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `cipher_parse-0.5.1a0/PKG-INFO` & `cipher_parse-0.5.1a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cipher-parse
-Version: 0.5.1a0
+Version: 0.5.1a1
 Summary: Pre- and post-processing for the phase-field code CIPHER.
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: hickle
 Provides-Extra: matflow
 Provides-Extra: notebook
 Requires-Dist: damask (>=3.0.0-alpha.6,<4.0.0)
+Requires-Dist: defdap (>=0.93.5,<0.94.0)
 Requires-Dist: h5py (==2.10.0)
 Requires-Dist: hickle (==4.0.4) ; extra == "hickle" or extra == "matflow"
 Requires-Dist: ipywidgets (<8.0.0)
 Requires-Dist: itkwidgets (>=0.25.2)
 Requires-Dist: matflow (>=0.2.26,<0.3.0) ; extra == "matflow"
 Requires-Dist: nbformat (>=5.4.0,<6.0.0)
 Requires-Dist: notebook (>=6.5.1,<7.0.0) ; extra == "notebook"
```

