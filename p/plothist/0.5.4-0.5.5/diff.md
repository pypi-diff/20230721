# Comparing `tmp/plothist-0.5.4.tar.gz` & `tmp/plothist-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plothist-0.5.4.tar", last modified: Thu Jul 20 07:02:33 2023, max compression
+gzip compressed data, was "plothist-0.5.5.tar", last modified: Fri Jul 21 04:15:11 2023, max compression
```

## Comparing `plothist-0.5.4.tar` & `plothist-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       42 2023-06-15 09:36:08.999160 plothist-0.5.4/.gitignore
--rw-r--r--   0        0        0     1518 2023-06-15 09:36:08.999160 plothist-0.5.4/LICENSE
--rw-r--r--   0        0        0     2028 2023-07-20 07:00:25.290800 plothist-0.5.4/README.rst
--rw-r--r--   0        0        0     5944 2023-07-20 03:49:45.483385 plothist-0.5.4/docs/advanced/hep_examples.rst
--rw-r--r--   0        0        0     5086 2023-07-20 05:57:18.696807 plothist-0.5.4/docs/basics/1d_hist.rst
--rw-r--r--   0        0        0     3615 2023-07-18 03:51:34.767128 plothist-0.5.4/docs/basics/2d_hist.rst
--rw-r--r--   0        0        0     5480 2023-07-20 07:00:25.290800 plothist-0.5.4/docs/conf.py
--rw-r--r--   0        0        0      431 2023-07-18 03:51:34.767128 plothist-0.5.4/docs/documentation/documentation.rst
--rw-r--r--   0        0        0    53165 2023-07-20 05:57:18.708807 plothist-0.5.4/docs/img/1d_comparison.svg
--rw-r--r--   0        0        0    31213 2023-07-20 05:57:18.712807 plothist-0.5.4/docs/img/1d_elt1.svg
--rw-r--r--   0        0        0    46925 2023-07-20 05:57:18.712807 plothist-0.5.4/docs/img/1d_elt2.svg
--rw-r--r--   0        0        0    50191 2023-07-20 05:57:18.712807 plothist-0.5.4/docs/img/1d_elt3.svg
--rw-r--r--   0        0        0    41788 2023-07-20 05:57:18.712807 plothist-0.5.4/docs/img/1d_hist_simple.svg
--rw-r--r--   0        0        0  1582427 2023-07-20 05:57:18.716807 plothist-0.5.4/docs/img/2d_hist_correlations.svg
--rw-r--r--   0        0        0    50176 2023-07-20 05:57:18.716807 plothist-0.5.4/docs/img/2d_hist_simple.svg
--rw-r--r--   0        0        0    37269 2023-07-20 05:57:18.716807 plothist-0.5.4/docs/img/2d_hist_uneven.svg
--rw-r--r--   0        0        0     3685 2023-07-18 03:51:34.779128 plothist-0.5.4/docs/img/adv_cubehelix.svg
--rw-r--r--   0        0        0    74541 2023-07-20 05:57:18.716807 plothist-0.5.4/docs/img/hep_examples_dataMC_flatten2D.svg
--rw-r--r--   0        0        0    98542 2023-07-20 05:57:18.716807 plothist-0.5.4/docs/img/hep_examples_dataMC_pull.svg
--rw-r--r--   0        0        0   123764 2023-07-20 05:57:18.716807 plothist-0.5.4/docs/img/hep_examples_dataMC_stacked.svg
--rw-r--r--   0        0        0   123717 2023-07-20 07:00:25.290800 plothist-0.5.4/docs/img/hep_examples_dataMC_stacked_small.svg
--rw-r--r--   0        0        0   123940 2023-07-20 05:57:18.720807 plothist-0.5.4/docs/img/hep_examples_dataMC_unstacked.svg
--rw-r--r--   0        0        0  1341490 2023-06-16 05:37:34.365641 plothist-0.5.4/docs/img/intro_2dhist_complexe.svg
--rw-r--r--   0        0        0      210 2023-07-20 07:00:25.290800 plothist-0.5.4/docs/index.rst
--rw-r--r--   0        0        0     1915 2023-07-18 03:51:34.783128 plothist-0.5.4/docs/usage/installation.rst
--rw-r--r--   0        0        0     1710 2023-07-20 07:00:25.290800 plothist-0.5.4/docs/usage/style.rst
--rw-r--r--   0        0        0     1352 2023-07-20 07:00:25.294800 plothist-0.5.4/plothist/__init__.py
--rw-r--r--   0        0        0     1543 2023-07-20 07:00:25.294800 plothist-0.5.4/plothist/default_style.mplstyle
--rw-r--r--   0        0        0      801 2023-06-15 09:36:09.003160 plothist-0.5.4/plothist/generate_dummy_data.py
--rw-r--r--   0        0        0    13931 2023-07-20 03:49:45.503385 plothist-0.5.4/plothist/hep_plotters.py
--rw-r--r--   0        0        0     1021 2023-07-18 03:51:34.783128 plothist-0.5.4/plothist/plothist_style.py
--rw-r--r--   0        0        0    22401 2023-07-20 03:49:45.503385 plothist-0.5.4/plothist/plotters.py
--rw-r--r--   0        0        0     1543 2023-07-20 07:00:25.294800 plothist-0.5.4/plothist/small_style.mplstyle
--rw-r--r--   0        0        0     6402 2023-07-18 03:51:34.783128 plothist-0.5.4/plothist/variable_registry.py
--rw-r--r--   0        0        0      750 2023-07-20 03:49:45.503385 plothist-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      747 2023-07-20 07:00:25.294800 plothist-0.5.4/scripts/install_latin_modern_fonts.sh
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 plothist-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-06-15 09:36:08.999160 plothist-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1518 2023-06-15 09:36:08.999160 plothist-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2028 2023-07-21 04:14:50.091490 plothist-0.5.5/README.rst
+-rw-r--r--   0        0        0     5944 2023-07-21 04:14:46.719473 plothist-0.5.5/docs/advanced/hep_examples.rst
+-rw-r--r--   0        0        0     5086 2023-07-21 04:14:46.719473 plothist-0.5.5/docs/basics/1d_hist.rst
+-rw-r--r--   0        0        0     3615 2023-07-18 03:51:34.767128 plothist-0.5.5/docs/basics/2d_hist.rst
+-rw-r--r--   0        0        0     5480 2023-07-21 04:14:50.091490 plothist-0.5.5/docs/conf.py
+-rw-r--r--   0        0        0      431 2023-07-18 03:51:34.767128 plothist-0.5.5/docs/documentation/documentation.rst
+-rw-r--r--   0        0        0    53165 2023-07-21 04:14:46.723474 plothist-0.5.5/docs/img/1d_comparison.svg
+-rw-r--r--   0        0        0    31213 2023-07-21 04:14:46.723474 plothist-0.5.5/docs/img/1d_elt1.svg
+-rw-r--r--   0        0        0    46925 2023-07-21 04:14:46.727474 plothist-0.5.5/docs/img/1d_elt2.svg
+-rw-r--r--   0        0        0    50191 2023-07-21 04:14:46.727474 plothist-0.5.5/docs/img/1d_elt3.svg
+-rw-r--r--   0        0        0    41788 2023-07-21 04:14:46.727474 plothist-0.5.5/docs/img/1d_hist_simple.svg
+-rw-r--r--   0        0        0  1582427 2023-07-21 04:14:46.731474 plothist-0.5.5/docs/img/2d_hist_correlations.svg
+-rw-r--r--   0        0        0    50176 2023-07-21 04:14:46.731474 plothist-0.5.5/docs/img/2d_hist_simple.svg
+-rw-r--r--   0        0        0    37269 2023-07-21 04:14:46.731474 plothist-0.5.5/docs/img/2d_hist_uneven.svg
+-rw-r--r--   0        0        0     3685 2023-07-18 03:51:34.779128 plothist-0.5.5/docs/img/adv_cubehelix.svg
+-rw-r--r--   0        0        0    74541 2023-07-21 04:14:46.731474 plothist-0.5.5/docs/img/hep_examples_dataMC_flatten2D.svg
+-rw-r--r--   0        0        0    98542 2023-07-21 04:14:46.731474 plothist-0.5.5/docs/img/hep_examples_dataMC_pull.svg
+-rw-r--r--   0        0        0   123764 2023-07-21 04:14:46.735473 plothist-0.5.5/docs/img/hep_examples_dataMC_stacked.svg
+-rw-r--r--   0        0        0   123717 2023-07-21 04:14:46.735473 plothist-0.5.5/docs/img/hep_examples_dataMC_stacked_small.svg
+-rw-r--r--   0        0        0   123940 2023-07-21 04:14:46.735473 plothist-0.5.5/docs/img/hep_examples_dataMC_unstacked.svg
+-rw-r--r--   0        0        0  1341490 2023-06-16 05:37:34.365641 plothist-0.5.5/docs/img/intro_2dhist_complexe.svg
+-rw-r--r--   0        0        0      210 2023-07-20 07:00:25.290800 plothist-0.5.5/docs/index.rst
+-rw-r--r--   0        0        0     1915 2023-07-18 03:51:34.783128 plothist-0.5.5/docs/usage/installation.rst
+-rw-r--r--   0        0        0     1710 2023-07-20 07:00:25.290800 plothist-0.5.5/docs/usage/style.rst
+-rw-r--r--   0        0        0     1352 2023-07-21 04:14:50.091490 plothist-0.5.5/plothist/__init__.py
+-rw-r--r--   0        0        0     1543 2023-07-21 04:14:46.735473 plothist-0.5.5/plothist/default_style.mplstyle
+-rw-r--r--   0        0        0      801 2023-06-15 09:36:09.003160 plothist-0.5.5/plothist/generate_dummy_data.py
+-rw-r--r--   0        0        0    14618 2023-07-21 04:14:50.091490 plothist-0.5.5/plothist/hep_plotters.py
+-rw-r--r--   0        0        0     1021 2023-07-18 03:51:34.783128 plothist-0.5.5/plothist/plothist_style.py
+-rw-r--r--   0        0        0    22430 2023-07-21 04:14:50.091490 plothist-0.5.5/plothist/plotters.py
+-rw-r--r--   0        0        0     1543 2023-07-20 07:00:25.294800 plothist-0.5.5/plothist/small_style.mplstyle
+-rw-r--r--   0        0        0     6402 2023-07-18 03:51:34.783128 plothist-0.5.5/plothist/variable_registry.py
+-rw-r--r--   0        0        0      750 2023-07-20 03:49:45.503385 plothist-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-07-20 07:00:25.294800 plothist-0.5.5/scripts/install_latin_modern_fonts.sh
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 plothist-0.5.5/PKG-INFO
```

### Comparing `plothist-0.5.4/LICENSE` & `plothist-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/README.rst` & `plothist-0.5.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 Installation and documentation: `https://plothist.readthedocs.io/ <https://plothist.readthedocs.io/>`_
 
 |img1| |img2|
 
 .. |img1| image:: https://raw.githubusercontent.com/cyrraz/plothist/main/docs/img/hep_examples_dataMC_stacked.svg
    :alt: Hep example
-   :width: 320
+   :width: 400
 
 .. |img2| image:: https://raw.githubusercontent.com/cyrraz/plothist/main/docs/img/hep_examples_dataMC_flatten2D.svg
    :alt: Hep example
-   :width: 320
+   :width: 400
 
 
 |GitHub Project| |PyPI version| |Docs from latest| |Docs from main| |Code style: black|
 
 
 **Major advantages over other plotting libraries**: scalability, style and user friendly way of managing variables.
 
@@ -39,11 +39,11 @@
 
 .. |GitHub Project| image:: https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub
    :target: https://github.com/cyrraz/plothist
 .. |PyPI version| image:: https://badge.fury.io/py/plothist.svg
    :target: https://badge.fury.io/py/plothist
 .. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
-.. |Docs from latest| image:: https://img.shields.io/badge/docs-v0.5.4-blue.svg
+.. |Docs from latest| image:: https://img.shields.io/badge/docs-v0.5.5-blue.svg
    :target: https://plothist.readthedocs.io/en/latest/
 .. |Docs from main| image:: https://img.shields.io/badge/docs-main-blue.svg
    :target: https://plothist.readthedocs.io/en/main/
```

### Comparing `plothist-0.5.4/docs/advanced/hep_examples.rst` & `plothist-0.5.5/docs/advanced/hep_examples.rst`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/basics/1d_hist.rst` & `plothist-0.5.5/docs/basics/1d_hist.rst`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/basics/2d_hist.rst` & `plothist-0.5.5/docs/basics/2d_hist.rst`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/conf.py` & `plothist-0.5.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 import os
 
 project = "plothist"
 copyright = "2023, Cyrille Praz, Tristan Fillinger"
 author = "Cyrille Praz, Tristan Fillinger"
 
 # The short X.Y version
-version = "0.5.4"
+version = "0.5.5"
 # The full version, including alpha/beta/rc tags
-release = "0.5.4"
+release = "0.5.5"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `plothist-0.5.4/docs/img/1d_comparison.svg` & `plothist-0.5.5/docs/img/1d_comparison.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/1d_elt1.svg` & `plothist-0.5.5/docs/img/1d_elt1.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/1d_elt2.svg` & `plothist-0.5.5/docs/img/1d_elt2.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/1d_elt3.svg` & `plothist-0.5.5/docs/img/1d_elt3.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/1d_hist_simple.svg` & `plothist-0.5.5/docs/img/1d_hist_simple.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/2d_hist_correlations.svg` & `plothist-0.5.5/docs/img/2d_hist_correlations.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/2d_hist_simple.svg` & `plothist-0.5.5/docs/img/2d_hist_simple.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/2d_hist_uneven.svg` & `plothist-0.5.5/docs/img/2d_hist_uneven.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/adv_cubehelix.svg` & `plothist-0.5.5/docs/img/adv_cubehelix.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/hep_examples_dataMC_flatten2D.svg` & `plothist-0.5.5/docs/img/hep_examples_dataMC_flatten2D.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/hep_examples_dataMC_pull.svg` & `plothist-0.5.5/docs/img/hep_examples_dataMC_pull.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/hep_examples_dataMC_stacked.svg` & `plothist-0.5.5/docs/img/hep_examples_dataMC_stacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/hep_examples_dataMC_stacked_small.svg` & `plothist-0.5.5/docs/img/hep_examples_dataMC_stacked_small.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/hep_examples_dataMC_unstacked.svg` & `plothist-0.5.5/docs/img/hep_examples_dataMC_unstacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/img/intro_2dhist_complexe.svg` & `plothist-0.5.5/docs/img/intro_2dhist_complexe.svg`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/usage/installation.rst` & `plothist-0.5.5/docs/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/docs/usage/style.rst` & `plothist-0.5.5/docs/usage/style.rst`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/plothist/__init__.py` & `plothist-0.5.5/plothist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Plot histograms in a scalable way and a beautiful style."""
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 
 from .plotters import (
     create_comparison_figure,
     create_axis,
     make_hist,
     make_2d_hist,
     plot_hist,
```

### Comparing `plothist-0.5.4/plothist/default_style.mplstyle` & `plothist-0.5.5/plothist/default_style.mplstyle`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/plothist/generate_dummy_data.py` & `plothist-0.5.5/plothist/generate_dummy_data.py`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/plothist/hep_plotters.py` & `plothist-0.5.5/plothist/hep_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     xlabel=None,
     ylabel=None,
     mc_labels=None,
     mc_colors=None,
     save_as=None,
     flatten_2d_hist=False,
     stacked=True,
+    mc_uncertainty=True,
     fig=None,
     ax_main=None,
     ax_comparison=None,
     **comparison_kwargs,
 ):
     """
     Compare data to MC simulations. The data uncertainties are computed using the Poisson confidence interval.
@@ -53,14 +54,16 @@
         The colors for the MC simulations. Default is None.
     save_as : str or None, optional
         The file path to save the figure. Default is None.
     flatten_2d_hist : bool, optional
         If True, flatten 2D histograms to 1D before plotting. Default is False.
     stacked : bool, optional
         If True, stack the MC histograms. If False, plot them side by side. Default is True.
+    mc_uncertainty : bool, optional
+        If False, set the MC uncertainties to zeros. Useful for postfit histograms.
     fig : matplotlib.figure.Figure or None, optional
         The figure to use for the plot. If fig, ax_main and ax_comparison are None, a new figure will be created. Default is None.
     ax_main : matplotlib.axes.Axes or None, optional
         The main axes for the histogram comparison. If fig, ax_main and ax_comparison are None, a new axes will be created. Default is None.
     ax_comparison : matplotlib.axes.Axes or None, optional
         The axes for the comparison plot. If fig, ax_main and ax_comparison are None, a new axes will be created. Default is None.
     **comparison_kwargs : optional
@@ -120,16 +123,16 @@
         # Otherwise, use the Gaussian uncertainties
         uncertainties_low = np.sqrt(data_hist.variances())
         uncertainties_high = uncertainties_low
 
     if comparison_kwargs["comparison"] == "pull":
         data_variances = np.where(
             data_hist.values() >= mc_hist_total.values(),
-            uncertainties_low**2,
-            uncertainties_high**2,
+            uncertainties_low ** 2,
+            uncertainties_high ** 2,
         )
         data_hist[:] = np.stack([data_hist.values(), data_variances], axis=-1)
     elif comparison_kwargs["comparison"] == "ratio":
         if comparison_kwargs["ratio_uncertainty"] == "split":
             np.seterr(divide="ignore", invalid="ignore")
             # Compute asymmetrical uncertainties to plot_comparison()
             comparison_kwargs.setdefault(
@@ -139,19 +142,19 @@
                     uncertainties_high / mc_hist_total.values(),
                 ],
             )
             np.seterr(divide="warn", invalid="warn")
         elif comparison_kwargs["ratio_uncertainty"] == "uncorrelated":
             data_hist_high = data_hist.copy()
             data_hist_high[:] = np.stack(
-                [data_hist_high.values(), uncertainties_high**2], axis=-1
+                [data_hist_high.values(), uncertainties_high ** 2], axis=-1
             )
             data_hist_low = data_hist.copy()
             data_hist_low[:] = np.stack(
-                [data_hist_low.values(), uncertainties_low**2], axis=-1
+                [data_hist_low.values(), uncertainties_low ** 2], axis=-1
             )
             # Compute asymmetrical uncertainties to plot_comparison()
             comparison_kwargs.setdefault(
                 "yerr",
                 [
                     np.sqrt(_hist_ratio_variances(data_hist_low, mc_hist_total)),
                     np.sqrt(_hist_ratio_variances(data_hist_high, mc_hist_total)),
@@ -165,37 +168,49 @@
         color="black",
         label="Data",
     )
 
     _ = ax_main.xaxis.set_ticklabels([])
 
     # Plot MC statistical uncertainty
-    mc_uncertainty = np.sqrt(mc_hist_total.variances())
-    ax_main.bar(
-        x=mc_hist_total.axes[0].centers,
-        bottom=mc_hist_total.values() - mc_uncertainty,
-        height=2 * mc_uncertainty,
-        width=mc_hist_total.axes[0].widths,
-        edgecolor="dimgrey",
-        hatch="////",
-        fill=False,
-        lw=0,
-        label="Stat. unc.",
-    )
+    if mc_uncertainty:
+        mc_uncertainty = np.sqrt(mc_hist_total.variances())
+        ax_main.bar(
+            x=mc_hist_total.axes[0].centers,
+            bottom=mc_hist_total.values() - mc_uncertainty,
+            height=2 * mc_uncertainty,
+            width=mc_hist_total.axes[0].widths,
+            edgecolor="dimgrey",
+            hatch="////",
+            fill=False,
+            lw=0,
+            label="Stat. unc.",
+        )
+    else:
+        mc_hist_total[:] = np.stack(
+            [mc_hist_total.values(), np.zeros_like(mc_hist_total.values())], axis=-1
+        )
+        if comparison_kwargs["comparison"] == "pull":
+            comparison_kwargs.setdefault(
+                "comparison_ylabel",
+                rf"$\frac{{ {comparison_kwargs['h1_label']} - {comparison_kwargs['h2_label']} }}{{ \sigma_{{{comparison_kwargs['h1_label']}}} }} $",
+            )
 
     ax_main.legend()
 
     plot_comparison(
         data_hist,
         mc_hist_total,
         ax=ax_comparison,
         xlabel=xlabel,
         **comparison_kwargs,
     )
 
+    fig.align_ylabels()
+
     if save_as is not None:
         fig.savefig(save_as, bbox_inches="tight")
 
     return fig, ax_main, ax_comparison
 
 
 def _get_poisson_uncertainties(data_hist):
```

### Comparing `plothist-0.5.4/plothist/plothist_style.py` & `plothist-0.5.5/plothist/plothist_style.py`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/plothist/plotters.py` & `plothist-0.5.5/plothist/plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,16 @@
         ax_comparison,
         xlabel=xlabel,
         h1_label=h1_label,
         h2_label=h2_label,
         **comparison_kwargs,
     )
 
+    fig.align_ylabels()
+
     if save_as is not None:
         fig.savefig(save_as, bbox_inches="tight")
 
     return fig, ax_main, ax_comparison
 
 
 def _hist_ratio_variances(hist_1, hist_2):
@@ -518,15 +520,15 @@
                 np.nan,
             )
             h2_scaled_uncertainties = np.where(
                 hist_2.values() != 0,
                 np.sqrt(hist_2.variances()) / hist_2.values(),
                 np.nan,
             )
-            comparison_variances = h1_scaled_uncertainties**2
+            comparison_variances = h1_scaled_uncertainties ** 2
         elif ratio_uncertainty == "uncorrelated":
             comparison_variances = _hist_ratio_variances(hist_1, hist_2)
         else:
             raise ValueError("ratio_uncertainty not in ['uncorrelated', 'split'].")
     elif comparison == "pull":
         comparison_values = np.where(
             hist_1.variances() + hist_2.variances() != 0,
@@ -641,15 +643,15 @@
     """
 
     def f(x0, x1):
         # Adapted from matplotlib
         def color(lambda_):
             # emphasise either low intensity values (gamma < 1),
             # or high intensity values (γ > 1)
-            lambda_gamma = lambda_**gamma
+            lambda_gamma = lambda_ ** gamma
 
             # Angle and amplitude for the deviation
             # from the black to white diagonal
             # in the plane of constant perceived intensity
             a = hue * lambda_gamma * (1 - lambda_gamma) / 2
 
             phi = 2 * np.pi * (start / 3 + rotation * lambda_)
```

### Comparing `plothist-0.5.4/plothist/small_style.mplstyle` & `plothist-0.5.5/plothist/small_style.mplstyle`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/plothist/variable_registry.py` & `plothist-0.5.5/plothist/variable_registry.py`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/pyproject.toml` & `plothist-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/scripts/install_latin_modern_fonts.sh` & `plothist-0.5.5/scripts/install_latin_modern_fonts.sh`

 * *Files identical despite different names*

### Comparing `plothist-0.5.4/PKG-INFO` & `plothist-0.5.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plothist
-Version: 0.5.4
+Version: 0.5.5
 Summary: Plot histograms in a scalable way and a beautiful style.
 Author-email: Cyrille Praz <code.cyrraz@protonmail.com>, Tristan Fillinger <tristan.github@gmail.com>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: BSD License
 Requires-Dist: boost-histogram~=1.3.1
 Requires-Dist: numpy>=1.14.5
 Requires-Dist: matplotlib>=3.0
```

