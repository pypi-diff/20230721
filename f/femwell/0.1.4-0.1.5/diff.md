# Comparing `tmp/femwell-0.1.4.tar.gz` & `tmp/femwell-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.1.4.tar", max compression
+gzip compressed data, was "femwell-0.1.5.tar", max compression
```

## Comparing `femwell-0.1.4.tar` & `femwell-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-07-10 14:54:59.990798 femwell-0.1.4/LICENSE
--rw-r--r--   0        0        0     2480 2023-07-10 14:54:59.990798 femwell-0.1.4/README.md
--rw-r--r--   0        0        0      255 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/eme.py.bak
--rw-r--r--   0        0        0        0 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/examples/__init__.py
--rw-r--r--   0        0        0     4820 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5762 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/fefd.py
--rw-r--r--   0        0        0     3173 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/fefd_2d.py
--rw-r--r--   0        0        0     1304 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/fiber.py
--rw-r--r--   0        0        0     1782 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/laplace.py
--rw-r--r--   0        0        0    17333 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/maxwell/waveguide.py
--rw-r--r--   0        0        0      224 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    26893 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7900 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21359 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh.py
--rw-r--r--   0        0        0     1033 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2922 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4224 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     1243 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_schrodinger.py
--rw-r--r--   0        0        0     8799 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/pn_analytical.py
--rw-r--r--   0        0        0     6453 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5880 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/thermal.py
--rw-r--r--   0        0        0     8803 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2655 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/utils.py
--rw-r--r--   0        0        0     1123 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/visualization.py
--rw-r--r--   0        0        0     2089 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/waveguide.py
--rw-r--r--   0        0        0      974 2023-07-10 14:55:11.575044 femwell-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-20 21:59:40.301303 femwell-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2480 2023-07-20 21:59:40.301303 femwell-0.1.5/README.md
+-rw-r--r--   0        0        0      255 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5762 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/fefd.py
+-rw-r--r--   0        0        0     3173 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/fefd_2d.py
+-rw-r--r--   0        0        0     1304 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/laplace.py
+-rw-r--r--   0        0        0    20309 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7900 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4224 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/waveguide.py
+-rw-r--r--   0        0        0      974 2023-07-20 21:59:53.825421 femwell-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.5/PKG-INFO
```

### Comparing `femwell-0.1.4/LICENSE` & `femwell-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/README.md` & `femwell-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/culomb.py` & `femwell-0.1.5/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/eme.py.bak` & `femwell-0.1.5/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.5/femwell/examples/coplanar_waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/fefd.py` & `femwell-0.1.5/femwell/fefd.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/fefd_2d.py` & `femwell-0.1.5/femwell/fefd_2d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/fiber.py` & `femwell-0.1.5/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/laplace.py` & `femwell-0.1.5/femwell/laplace.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/maxwell/waveguide.py` & `femwell-0.1.5/femwell/maxwell/waveguide.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Waveguide analysis based on https://doi.org/10.1080/02726340290084012."""
 from dataclasses import dataclass
 from functools import cached_property
-from typing import List
+from typing import List, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.constants
 import scipy.sparse.linalg
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
 from numpy.typing import NDArray
 from scipy.constants import epsilon_0, speed_of_light
 from skfem import (
     Basis,
     BilinearForm,
     ElementDG,
     ElementTriN1,
@@ -144,28 +146,84 @@
             self.n_eff
             + self.calculate_coupling_coefficient(self, delta_epsilon)
             * scipy.constants.epsilon_0
             * scipy.constants.speed_of_light
             * 0.5
         )
 
+    def calculate_intensity(self) -> Tuple[NDArray, Basis]:
+        """Calculates the intensity of a mode.
+
+        The intensity is calculated from the cross-product between the electric and magnetic field, as
+        described in https://doi.org/10.1364/OE.16.016659.
+
+        The calculation is performed as follows:
+        1) The electric and magnetic fields are interpolated on the quadrature points with the simulation basis;
+        2) The intensity is calculated directly on the quadrature points;
+        3) The intensity is projected on a new discontinuous, piecewise linear triangular basis.
+
+        Returns:
+            Basis, NDArray: Plot-ready basis and intensity array
+        """
+        (Ex, Ey), _ = self.basis.interpolate(self.E)
+        (Hx, Hy), _ = self.basis.interpolate(np.conj(self.H))
+        intensity = 0.5 * np.real(Ex * Hy - Ey * Hx)
+        basis2 = self.basis.with_element(ElementDG(ElementTriP1()))
+        intensity2 = basis2.project(intensity)
+
+        return basis2, intensity2
+
     def plot(self, field, plot_vectors=False, colorbar=True, direction="y", title="E"):
         return plot_mode(
             self.basis,
             field,
             plot_vectors=plot_vectors,
             colorbar=colorbar,
             title=title,
             direction=direction,
         )
 
     def show(self, field, **kwargs):
         self.plot(field=field, **kwargs)
         plt.show()
 
+    def plot_intensity(
+        self,
+        ax: Axes = None,
+        colorbar: bool = True,
+        normalize: bool = True,
+    ) -> Tuple[Figure, Axes]:
+        """Plots the intensity of a mode as outlined in `calculate_intensity`.
+
+        Args:
+            ax (Axes, optional): Axes onto which the plot is drawn. Defaults to None.
+            colorbar (bool, optional): Adds a colorbar to the plot. Defaults to True.
+            normalize (bool, optional): Normalizes the intensity by its maximum value. Defaults to True.
+
+        Returns:
+            Tuple[Figure, Axes]: Figure and axes of the plot.
+        """
+        intensity_basis, intensity = self.calculate_intensity()
+        if normalize:
+            intensity = intensity / intensity.max()
+
+        if ax is None:
+            fig, ax = plt.subplots()
+        else:
+            fig = plt.gcf()
+
+        for subdomain in self.basis.mesh.subdomains.keys() - {"gmsh:bounding_entities"}:
+            self.basis.mesh.restrict(subdomain).draw(ax=ax, boundaries_only=True, color="w")
+        intensity_basis.plot(intensity, ax=ax, cmap="inferno")
+
+        if colorbar:
+            plt.colorbar(ax.collections[-1])
+
+        return fig, ax
+
 
 @dataclass(frozen=True)
 class Modes:
     modes: List
 
     def __getitem__(self, idx) -> Mode:
         return self.modes[idx]
@@ -328,15 +386,38 @@
         return e * v
 
     b_operator = bform.assemble(basis_energy)
 
     return basis_energy, scipy.sparse.linalg.spsolve(b_operator, a_operator)
 
 
-def calculate_overlap(basis_i, E_i, H_i, basis_j, E_j, H_j):
+def calculate_overlap(
+    basis_i: Basis,
+    E_i: np.ndarray,
+    H_i: np.ndarray,
+    basis_j: Basis,
+    E_j: np.ndarray,
+    H_j: np.ndarray,
+) -> np.complex64:
+    """Calculates the fully vectorial overlap between two modes.
+
+    If the modes do not share the basis, interpolation is performed automatically.
+
+    Args:
+        basis_i (Basis): Basis of the first mode
+        E_i (np.ndarray): Electric field of the first mode
+        H_i (np.ndarray): Magnetic field of the first mode
+        basis_j (Basis): Basis of the second mode
+        E_j (np.ndarray): Electric field of the first mode
+        H_j (np.ndarray): Magnetic field of the first mode
+
+    Returns:
+        np.complex64: Complex overlap between the two modes
+    """
+
     @Functional(dtype=np.complex64)
     def overlap(w):
         return cross(np.conj(w["E_i"][0]), w["H_j"][0]) + cross(w["E_j"][0], np.conj(w["H_i"][0]))
 
     if basis_i == basis_j:
         return 0.5 * overlap.assemble(
             basis_i,
```

### Comparing `femwell-0.1.4/femwell/mesh/mesh.py` & `femwell-0.1.5/femwell/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mesh/meshtracker.py` & `femwell-0.1.5/femwell/mesh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mesh/slice.py` & `femwell-0.1.5/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mesh.py` & `femwell-0.1.5/femwell/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mode_solver_1d.py` & `femwell-0.1.5/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.5/femwell/mode_solver_2d_periodic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.5/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mode_solver_inplane.py` & `femwell-0.1.5/femwell/mode_solver_inplane.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/mode_solver_schrodinger.py` & `femwell-0.1.5/femwell/mode_solver_schrodinger.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/pn_analytical.py` & `femwell-0.1.5/femwell/pn_analytical.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/solver.py` & `femwell-0.1.5/femwell/solver.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/tcad.py` & `femwell-0.1.5/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/tests/test_mesh.py` & `femwell-0.1.5/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/thermal.py` & `femwell-0.1.5/femwell/thermal.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/thermal_transient.py` & `femwell-0.1.5/femwell/thermal_transient.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/utils.py` & `femwell-0.1.5/femwell/utils.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/visualization.py` & `femwell-0.1.5/femwell/visualization.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/femwell/waveguide.py` & `femwell-0.1.5/femwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.4/pyproject.toml` & `femwell-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "femwell"
-version = "0.1.4"
+version = "0.1.5"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
```

### Comparing `femwell-0.1.4/PKG-INFO` & `femwell-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.1.4
+Version: 0.1.5
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
```

