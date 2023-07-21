# Comparing `tmp/sarracen-1.2.1.tar.gz` & `tmp/sarracen-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarracen-1.2.1.tar", last modified: Tue May 23 17:30:14 2023, max compression
+gzip compressed data, was "sarracen-1.2.2.tar", last modified: Fri Jul 21 11:48:40 2023, max compression
```

## Comparing `sarracen-1.2.1.tar` & `sarracen-1.2.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      679 2023-05-23 17:25:45.049573 sarracen-1.2.1/.github/workflows/joss_paper.yml
--rw-r--r--   0        0        0       76 2023-05-23 17:25:45.049661 sarracen-1.2.1/.gitignore
--rw-r--r--   0        0        0      125 2023-05-23 17:25:45.049741 sarracen-1.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     5493 2023-05-23 17:25:45.049850 sarracen-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    35149 2023-05-23 17:25:45.050092 sarracen-1.2.1/LICENCE
--rw-r--r--   0        0        0     2264 2023-05-23 17:25:45.050225 sarracen-1.2.1/README.md
--rw-r--r--   0        0        0      634 2023-05-23 17:25:45.050343 sarracen-1.2.1/docs/Makefile
--rw-r--r--   0        0        0     1712 2023-05-23 17:25:45.050440 sarracen-1.2.1/docs/api.rst
--rw-r--r--   0        0        0     2153 2023-05-23 17:25:45.050526 sarracen-1.2.1/docs/conf.py
--rw-r--r--   0        0        0     1173 2023-05-23 17:25:45.050624 sarracen-1.2.1/docs/contributing.rst
--rw-r--r--   0        0        0      133 2023-05-23 17:25:45.050699 sarracen-1.2.1/docs/examples.rst
--rw-r--r--   0        0        0     2310 2023-05-23 17:25:45.050830 sarracen-1.2.1/docs/examples/dustydisc.rst
--rw-r--r--   0        0        0   300231 2023-05-23 17:25:45.052392 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-describe.png
--rw-r--r--   0        0        0   577154 2023-05-23 17:25:45.055494 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-dust.png
--rw-r--r--   0        0        0   296363 2023-05-23 17:25:45.057079 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas-sinks.png
--rw-r--r--   0        0        0   296269 2023-05-23 17:25:45.058636 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas.png
--rw-r--r--   0        0        0   152484 2023-05-23 17:25:45.059480 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf-sinks.png
--rw-r--r--   0        0        0   506967 2023-05-23 17:25:45.062017 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf.png
--rw-r--r--   0        0        0    17275 2023-05-23 17:25:45.062189 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-value-counts.png
--rw-r--r--   0        0        0     1121 2023-05-23 17:25:45.062281 sarracen-1.2.1/docs/examples/ot.rst
--rw-r--r--   0        0        0    18453 2023-05-23 17:25:45.062464 sarracen-1.2.1/docs/examples/ot/ot-1d.png
--rw-r--r--   0        0        0   145467 2023-05-23 17:25:45.063212 sarracen-1.2.1/docs/examples/ot/ot-describe.png
--rw-r--r--   0        0        0   178608 2023-05-23 17:25:45.064211 sarracen-1.2.1/docs/examples/ot/ot-sdf.png
--rw-r--r--   0        0        0    70378 2023-05-23 17:25:45.064684 sarracen-1.2.1/docs/examples/ot/ot-streamlines.png
--rw-r--r--   0        0        0    48370 2023-05-23 17:25:45.065025 sarracen-1.2.1/docs/examples/ot/ot.png
--rw-r--r--   0        0        0     1154 2023-05-23 17:25:45.065141 sarracen-1.2.1/docs/index.rst
--rw-r--r--   0        0        0     1648 2023-05-23 17:25:45.065228 sarracen-1.2.1/docs/installation.rst
--rw-r--r--   0        0        0      800 2023-05-23 17:25:45.065311 sarracen-1.2.1/docs/make.bat
--rw-r--r--   0        0        0    95948 2023-05-23 17:25:45.065895 sarracen-1.2.1/docs/paper/main_image.png
--rw-r--r--   0        0        0    14031 2023-05-23 17:25:45.066035 sarracen-1.2.1/docs/paper/paper.bib
--rw-r--r--   0        0        0     5953 2023-05-23 17:25:45.066145 sarracen-1.2.1/docs/paper/paper.md
--rw-r--r--   0        0        0     3484 2023-05-23 17:25:45.066247 sarracen-1.2.1/docs/quick-start.rst
--rw-r--r--   0        0        0     4814 2023-05-23 17:25:45.066335 sarracen-1.2.1/docs/render.rst
--rw-r--r--   0        0        0      527 2023-05-23 17:25:45.066403 sarracen-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       75 2023-05-23 17:25:45.066468 sarracen-1.2.1/requirements.txt
--rw-r--r--   0        0        0      363 2023-05-23 17:29:44.559778 sarracen-1.2.1/sarracen/__init__.py
--rw-r--r--   0        0        0      385 2023-05-23 17:25:45.066665 sarracen-1.2.1/sarracen/interpolate/__init__.py
--rw-r--r--   0        0        0     4766 2023-05-23 17:25:45.066922 sarracen-1.2.1/sarracen/interpolate/base_backend.py
--rw-r--r--   0        0        0    24755 2023-05-23 17:25:45.067067 sarracen-1.2.1/sarracen/interpolate/cpu_backend.py
--rw-r--r--   0        0        0    27110 2023-05-23 17:25:45.067164 sarracen-1.2.1/sarracen/interpolate/gpu_backend.py
--rw-r--r--   0        0        0    55074 2023-05-23 17:25:45.067472 sarracen-1.2.1/sarracen/interpolate/interpolate.py
--rw-r--r--   0        0        0      212 2023-05-23 17:25:45.067578 sarracen-1.2.1/sarracen/kernels/__init__.py
--rw-r--r--   0        0        0     3467 2023-05-23 17:25:45.067665 sarracen-1.2.1/sarracen/kernels/base_kernel.py
--rw-r--r--   0        0        0      562 2023-05-23 17:25:45.067732 sarracen-1.2.1/sarracen/kernels/cubic_spline.py
--rw-r--r--   0        0        0    13535 2023-05-23 17:25:45.067832 sarracen-1.2.1/sarracen/kernels/cubic_spline_exact.py
--rw-r--r--   0        0        0      634 2023-05-23 17:25:45.067901 sarracen-1.2.1/sarracen/kernels/quartic_spline.py
--rw-r--r--   0        0        0      607 2023-05-23 17:25:45.067968 sarracen-1.2.1/sarracen/kernels/quintic_spline.py
--rw-r--r--   0        0        0        1 2023-05-23 17:25:45.068062 sarracen-1.2.1/sarracen/readers/__init__.py
--rw-r--r--   0        0        0      678 2023-05-23 17:25:45.068203 sarracen-1.2.1/sarracen/readers/read_csv.py
--rw-r--r--   0        0        0     8959 2023-05-23 17:25:45.068313 sarracen-1.2.1/sarracen/readers/read_marisa.py
--rw-r--r--   0        0        0     9017 2023-05-23 17:25:45.068426 sarracen-1.2.1/sarracen/readers/read_phantom.py
--rw-r--r--   0        0        0    30051 2023-05-23 17:25:45.068505 sarracen-1.2.1/sarracen/render.py
--rw-r--r--   0        0        0    19956 2023-05-23 17:25:45.068655 sarracen-1.2.1/sarracen/sarracen_dataframe.py
--rw-r--r--   0        0        0        0 2023-05-23 17:25:45.068730 sarracen-1.2.1/sarracen/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 17:25:45.068798 sarracen-1.2.1/sarracen/tests/readers/__init__.py
--rw-r--r--   0        0        0      969 2023-05-23 17:25:45.068868 sarracen-1.2.1/sarracen/tests/readers/test_read_csv.py
--rw-r--r--   0        0        0    84917 2023-05-23 17:25:45.069147 sarracen-1.2.1/sarracen/tests/test_interpolate.py
--rw-r--r--   0        0        0     8159 2023-05-23 17:25:45.069267 sarracen-1.2.1/sarracen/tests/test_kernels.py
--rw-r--r--   0        0        0    11302 2023-05-23 17:25:45.069355 sarracen-1.2.1/sarracen/tests/test_render.py
--rw-r--r--   0        0        0     5514 2023-05-23 17:25:45.069431 sarracen-1.2.1/sarracen/tests/test_sarracen_dataframe.py
--rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 sarracen-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      679 2023-05-23 17:25:45.049573 sarracen-1.2.2/.github/workflows/joss_paper.yml
+-rw-r--r--   0        0        0       76 2023-05-23 17:25:45.049661 sarracen-1.2.2/.gitignore
+-rw-r--r--   0        0        0      125 2023-05-23 17:25:45.049741 sarracen-1.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     5493 2023-05-23 17:25:45.049850 sarracen-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    35149 2023-05-23 17:25:45.050092 sarracen-1.2.2/LICENCE
+-rw-r--r--   0        0        0     2567 2023-07-21 11:28:02.666201 sarracen-1.2.2/README.md
+-rw-r--r--   0        0        0      634 2023-05-23 17:25:45.050343 sarracen-1.2.2/docs/Makefile
+-rw-r--r--   0        0        0     1712 2023-05-23 17:25:45.050440 sarracen-1.2.2/docs/api.rst
+-rw-r--r--   0        0        0     2153 2023-05-23 17:25:45.050526 sarracen-1.2.2/docs/conf.py
+-rw-r--r--   0        0        0     1173 2023-05-23 17:25:45.050624 sarracen-1.2.2/docs/contributing.rst
+-rw-r--r--   0        0        0      133 2023-05-23 17:25:45.050699 sarracen-1.2.2/docs/examples.rst
+-rw-r--r--   0        0        0     2310 2023-05-23 17:25:45.050830 sarracen-1.2.2/docs/examples/dustydisc.rst
+-rw-r--r--   0        0        0   300231 2023-05-23 17:25:45.052392 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-describe.png
+-rw-r--r--   0        0        0   577154 2023-05-23 17:25:45.055494 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-dust.png
+-rw-r--r--   0        0        0   296363 2023-05-23 17:25:45.057079 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-gas-sinks.png
+-rw-r--r--   0        0        0   296269 2023-05-23 17:25:45.058636 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-gas.png
+-rw-r--r--   0        0        0   152484 2023-05-23 17:25:45.059480 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-sdf-sinks.png
+-rw-r--r--   0        0        0   506967 2023-05-23 17:25:45.062017 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-sdf.png
+-rw-r--r--   0        0        0    17275 2023-05-23 17:25:45.062189 sarracen-1.2.2/docs/examples/dustydisc/dustydisc-value-counts.png
+-rw-r--r--   0        0        0     1121 2023-05-23 17:25:45.062281 sarracen-1.2.2/docs/examples/ot.rst
+-rw-r--r--   0        0        0    18453 2023-05-23 17:25:45.062464 sarracen-1.2.2/docs/examples/ot/ot-1d.png
+-rw-r--r--   0        0        0   145467 2023-05-23 17:25:45.063212 sarracen-1.2.2/docs/examples/ot/ot-describe.png
+-rw-r--r--   0        0        0   178608 2023-05-23 17:25:45.064211 sarracen-1.2.2/docs/examples/ot/ot-sdf.png
+-rw-r--r--   0        0        0    70378 2023-05-23 17:25:45.064684 sarracen-1.2.2/docs/examples/ot/ot-streamlines.png
+-rw-r--r--   0        0        0    48370 2023-05-23 17:25:45.065025 sarracen-1.2.2/docs/examples/ot/ot.png
+-rw-r--r--   0        0        0     1154 2023-05-23 17:25:45.065141 sarracen-1.2.2/docs/index.rst
+-rw-r--r--   0        0        0     1648 2023-05-23 17:25:45.065228 sarracen-1.2.2/docs/installation.rst
+-rw-r--r--   0        0        0      800 2023-05-23 17:25:45.065311 sarracen-1.2.2/docs/make.bat
+-rw-r--r--   0        0        0    95948 2023-05-23 17:25:45.065895 sarracen-1.2.2/docs/paper/main_image.png
+-rw-r--r--   0        0        0    14975 2023-07-21 11:28:02.666408 sarracen-1.2.2/docs/paper/paper.bib
+-rw-r--r--   0        0        0     6169 2023-07-21 11:28:02.666585 sarracen-1.2.2/docs/paper/paper.md
+-rw-r--r--   0        0        0     3484 2023-05-23 17:25:45.066247 sarracen-1.2.2/docs/quick-start.rst
+-rw-r--r--   0        0        0     4814 2023-05-23 17:25:45.066335 sarracen-1.2.2/docs/render.rst
+-rw-r--r--   0        0        0      527 2023-05-23 17:25:45.066403 sarracen-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-05-23 17:25:45.066468 sarracen-1.2.2/requirements.txt
+-rw-r--r--   0        0        0      363 2023-07-21 11:28:02.666738 sarracen-1.2.2/sarracen/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-23 17:25:45.066665 sarracen-1.2.2/sarracen/interpolate/__init__.py
+-rw-r--r--   0        0        0     4766 2023-05-23 17:25:45.066922 sarracen-1.2.2/sarracen/interpolate/base_backend.py
+-rw-r--r--   0        0        0    24755 2023-05-23 17:25:45.067067 sarracen-1.2.2/sarracen/interpolate/cpu_backend.py
+-rw-r--r--   0        0        0    27110 2023-05-23 17:25:45.067164 sarracen-1.2.2/sarracen/interpolate/gpu_backend.py
+-rw-r--r--   0        0        0    55899 2023-07-21 11:28:02.667005 sarracen-1.2.2/sarracen/interpolate/interpolate.py
+-rw-r--r--   0        0        0      212 2023-05-23 17:25:45.067578 sarracen-1.2.2/sarracen/kernels/__init__.py
+-rw-r--r--   0        0        0     3467 2023-05-23 17:25:45.067665 sarracen-1.2.2/sarracen/kernels/base_kernel.py
+-rw-r--r--   0        0        0      562 2023-05-23 17:25:45.067732 sarracen-1.2.2/sarracen/kernels/cubic_spline.py
+-rw-r--r--   0        0        0    13535 2023-05-23 17:25:45.067832 sarracen-1.2.2/sarracen/kernels/cubic_spline_exact.py
+-rw-r--r--   0        0        0      634 2023-05-23 17:25:45.067901 sarracen-1.2.2/sarracen/kernels/quartic_spline.py
+-rw-r--r--   0        0        0      607 2023-05-23 17:25:45.067968 sarracen-1.2.2/sarracen/kernels/quintic_spline.py
+-rw-r--r--   0        0        0        1 2023-05-23 17:25:45.068062 sarracen-1.2.2/sarracen/readers/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-23 17:25:45.068203 sarracen-1.2.2/sarracen/readers/read_csv.py
+-rw-r--r--   0        0        0     8959 2023-05-23 17:25:45.068313 sarracen-1.2.2/sarracen/readers/read_marisa.py
+-rw-r--r--   0        0        0     9056 2023-07-21 11:28:02.667212 sarracen-1.2.2/sarracen/readers/read_phantom.py
+-rw-r--r--   0        0        0    30468 2023-07-21 11:28:02.667429 sarracen-1.2.2/sarracen/render.py
+-rw-r--r--   0        0        0    20116 2023-07-21 11:28:02.667629 sarracen-1.2.2/sarracen/sarracen_dataframe.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:25:45.068730 sarracen-1.2.2/sarracen/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:25:45.068798 sarracen-1.2.2/sarracen/tests/readers/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-23 17:25:45.068868 sarracen-1.2.2/sarracen/tests/readers/test_read_csv.py
+-rw-r--r--   0        0        0    84917 2023-05-23 17:25:45.069147 sarracen-1.2.2/sarracen/tests/test_interpolate.py
+-rw-r--r--   0        0        0     8159 2023-05-23 17:25:45.069267 sarracen-1.2.2/sarracen/tests/test_kernels.py
+-rw-r--r--   0        0        0    11302 2023-05-23 17:25:45.069355 sarracen-1.2.2/sarracen/tests/test_render.py
+-rw-r--r--   0        0        0     5514 2023-05-23 17:25:45.069431 sarracen-1.2.2/sarracen/tests/test_sarracen_dataframe.py
+-rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 sarracen-1.2.2/PKG-INFO
```

### Comparing `sarracen-1.2.1/.github/workflows/joss_paper.yml` & `sarracen-1.2.2/.github/workflows/joss_paper.yml`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/CODE_OF_CONDUCT.md` & `sarracen-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/LICENCE` & `sarracen-1.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/README.md` & `sarracen-1.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -41,8 +41,16 @@
 
 Code submissions should be submitted as a pull request. Make sure that all existing unit tests successfully pass, and 
 please add any new unit tests that are relevant. Documentation changes should also be submitted as a pull request.
 
 If you are stuck or need help, [raising an issue](https://github.com/ttricco/sarracen/issues) is a good place to start. 
 This helps us keep common issues in public view. Feel free to also [email](mailto:tstricco@mun.ca) with questions.
 
-Please note that we adhere to a [code of conduct](CODE_OF_CONDUCT.md).
+Please note that we adhere to a [code of conduct](CODE_OF_CONDUCT.md).
+
+Citation
+--------
+
+Please cite the paper if you use Sarracen within your work (DOI: [10.21105/joss.05263](https://doi.org/10.21105/joss.05263)).
+
+*Sarracen: a Python package for analysis and visualization of smoothed particle hydrodynamics data.* Journal of Open Source Software, 8(86), 5263, 2023. 
+
```

### Comparing `sarracen-1.2.1/docs/Makefile` & `sarracen-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/api.rst` & `sarracen-1.2.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/conf.py` & `sarracen-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/contributing.rst` & `sarracen-1.2.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc.rst` & `sarracen-1.2.2/docs/examples/dustydisc.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-describe.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-describe.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-dust.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-dust.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas-sinks.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-gas-sinks.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-gas.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf-sinks.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-sdf-sinks.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-sdf.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-value-counts.png` & `sarracen-1.2.2/docs/examples/dustydisc/dustydisc-value-counts.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/ot.rst` & `sarracen-1.2.2/docs/examples/ot.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/ot/ot-1d.png` & `sarracen-1.2.2/docs/examples/ot/ot-1d.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/ot/ot-describe.png` & `sarracen-1.2.2/docs/examples/ot/ot-describe.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/ot/ot-sdf.png` & `sarracen-1.2.2/docs/examples/ot/ot-sdf.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/ot/ot-streamlines.png` & `sarracen-1.2.2/docs/examples/ot/ot-streamlines.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/examples/ot/ot.png` & `sarracen-1.2.2/docs/examples/ot/ot.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/index.rst` & `sarracen-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/installation.rst` & `sarracen-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/make.bat` & `sarracen-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/paper/main_image.png` & `sarracen-1.2.2/docs/paper/main_image.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/paper/paper.bib` & `sarracen-1.2.2/docs/paper/paper.bib`

 * *Files 8% similar despite different names*

```diff
@@ -142,15 +142,30 @@
 archivePrefix = {arXiv},
        eprint = {1011.3514},
  primaryClass = {astro-ph.IM},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2011ApJS..192....9T},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 
+@BOOK{paraview,
+        title = {The paraview guide: a parallel visualization application},
+       author = {{Ayachit}, Utkarsh},
+         year = {2015},
+    publisher = {Kitware, Inc.}
+}
 
+@INCOLLECTION{visit,
+       author = {{Childs}, Hank and {Brugger}, Eric and {Whitlock}, Brad and {Meredith}, Jeremy and {Ahern}, Sean and {Pugmire}, David and {Biagas}, Kathleen and {Miller}, Mark and {Harrison}, Cyrus and {Weber}, Gunther H. and {Krishnan}, Hari and {Fogal}, Thomas and {Sanderson}, Allen and {Garth}, Christoph and {Bethel}, E. Wes and {Camp}, David and {R\"{u}bel}, Oliver and {Durant}, Marc and {Favre}, Jean M. and {Navr\'{a}til}, Paul},
+          doi = {10.1201/b12985},
+        title = {VisIt: An End-User Tool For Visualizing and Analyzing Very Large Data},
+    booktitle = {High Performance Visualization--Enabling Extreme-Scale Scientific Insight},
+        pages = {357-372},
+        month = {October},
+         year = {2012}
+}
 
 @ARTICLE{swiftsimio,
        author = {{Borrow}, Josh and {Borrisov}, Alexei},
         title = "{swiftsimio: A Python library for reading SWIFT data}",
       journal = {The Journal of Open Source Software},
      keywords = {Python, cosmology, i/o, simulations, astronomy},
          year = 2020,
```

### Comparing `sarracen-1.2.1/docs/paper/paper.md` & `sarracen-1.2.2/docs/paper/paper.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,25 +42,28 @@
 # Statement of need
 
 `Splash` [@splash] is the current standard bearer for visualization of astrophysical
 SPH data. It is an open-source, command-line visualization tool written in Fortran.
 It is comprehensive, highly efficient, and can natively read SPH data from a large 
 number of SPH simulation codes. `Splash` has a large user base for these reasons. The
 significant shortcoming of `Splash` is that it has limited capability for analysis of 
-SPH data. Any complicated analysis requires modification of the Fortran code. 
+SPH data. Any complicated analysis requires modification of the Fortran code.
 
 There are publicly available Python solutions for visualization or analysis of 
 astrophysical SPH data. However, these are often specific to a single code, such as 
 `SWIFTsimIO` [@swiftsimio], which is dedicated to the `Swift` [@swift] cosmological 
 code. `yt` [@yt] is a general purpose analysis and visualization package for 
 volumetric astrophysical data. Originally designed for data from grid-based codes, 
 recent versions have added support to store SPH particle data directly (instead of 
-storing only a mesh interpolation). `Plonk` [@plonk] is the work most similar to 
-ours, but uses custom data structures for storing particle data and is limited to 
-reading HDF5 data from the `Phantom` [@phantom] SPH code.
+storing only a mesh interpolation). `ParaView` [@paraview] and `VisIt` [@visit] are
+two open-source visualization applications that can be used with SPH data and scale 
+to large data sets. `ParaView` and `VisIt` additionally offer scripting in Python. 
+`Plonk` [@plonk] is the work most similar to ours, but uses custom data structures 
+for storing particle data and is limited to reading HDF5 data from the `Phantom` 
+[@phantom] SPH code.
 
 Our goal with `Sarracen` is to provide a Python package that implements the robust
 interpolation and visualization of SPH data offered by `Splash`, but which can be
 used for deeper analysis and integrated into a data scientist's Python toolkit. We 
 use `Matplotlib` [@matplotlib] for visualization, and an extension of the `pandas` 
 [@pandas] DataFrame structure for storing particle data. Using `Sarracen` should 
 be familiar for most users. Furthermore, Python has many high-quality scientific
```

### Comparing `sarracen-1.2.1/docs/quick-start.rst` & `sarracen-1.2.2/docs/quick-start.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/docs/render.rst` & `sarracen-1.2.2/docs/render.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/pyproject.toml` & `sarracen-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/interpolate/base_backend.py` & `sarracen-1.2.2/sarracen/interpolate/base_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/interpolate/cpu_backend.py` & `sarracen-1.2.2/sarracen/interpolate/cpu_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/interpolate/gpu_backend.py` & `sarracen-1.2.2/sarracen/interpolate/gpu_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/interpolate/interpolate.py` & `sarracen-1.2.2/sarracen/interpolate/interpolate.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,30 +297,30 @@
         rotated_y if z == data.ycol else \
             rotated_z if z == data.zcol else data[z]
 
     return x_data, y_data, z_data
 
 
 def _get_mass(data: 'SarracenDataFrame'):
-    if data._mcol == None:
+    if data.mcol == None:
         if 'mass' not in data.params:
             raise KeyError("'mass' column does not exist in this SarracenDataFrame.")
         return data.params['mass']
 
-    return data[data._mcol].to_numpy()
+    return data[data.mcol].to_numpy()
 
 
 def _get_density(data: 'SarracenDataFrame'):
-    if data._rhocol == None:
+    if data.rhocol == None:
         if not {data.hcol}.issubset(data.columns) or 'hfact' not in data.params:
             raise KeyError('Density cannot be derived from the columns in this SarracenDataFrame.')
 
-        return ((data.params['hfact'] / data['h']) ** (data.get_dim()) * _get_mass(data)).to_numpy()
+        return ((data.params['hfact'] / data[data.hcol]) ** (data.get_dim()) * _get_mass(data)).to_numpy()
 
-    return data[data._rhocol].to_numpy()
+    return data[data.rhocol].to_numpy()
 
 
 def _get_weight(data: 'SarracenDataFrame', target: Union[str, np.ndarray], dens_weight: bool):
 
     if type(target) is str:
         if target == 'rho':
             target_data = _get_density(data)
@@ -344,17 +344,17 @@
 def _get_smoothing_lengths(data: 'SarracenDataFrame', hmin: float, x_pixels: int, y_pixels: int,
                            xlim: Tuple[float, float], ylim: Tuple[float, float]):
     """ Return the smoothing length data, imposing a minimum length if hmin is True. """
     
     if hmin:
         pix_size = (xlim[1] - xlim[0]) / x_pixels
         pix_size = np.maximum(pix_size, (ylim[1] - ylim[0]) / y_pixels)
-        h_data = np.maximum(data[data._hcol].to_numpy(), 0.5 * pix_size)
+        h_data = np.maximum(data[data.hcol].to_numpy(), 0.5 * pix_size)
     else:
-        h_data = data[data._hcol].to_numpy()
+        h_data = data[data.hcol].to_numpy()
 
     return h_data
 
 
 def interpolate_2d(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, kernel: BaseKernel = None,
                    x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
                    ylim: Tuple[float, float] = None, exact: bool = False, backend: str = None,
@@ -381,15 +381,16 @@
         a consistent aspect ratio.
     xlim, ylim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -463,15 +464,16 @@
         a consistent aspect ratio.
     xlim, ylim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -547,15 +549,16 @@
         Kernel to use for smoothing the target data. Defaults to the kernel specified in `data`.
     pixels: int, optional
         Number of points in the resulting line plot in the x-direction.
     xlim, ylim: tuple of float, optional
         Starting and ending coordinates of the cross-section line (in particle data space). Defaults to
         the minimum and maximum values of `x` and `y`.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -593,17 +596,17 @@
     pixels = pixels if pixels is not None else 512
 
     if pixels <= 0:
         raise ValueError('pixcount must be greater than zero!')
 
     if hmin:
         pix_size = np.sqrt((xlim[1] - xlim[0])**2 + (ylim[1] - ylim[0])**2) / pixels
-        h_data = np.maximum(data[data._hcol].to_numpy(), 0.5 * pix_size)
+        h_data = np.maximum(data[data.hcol].to_numpy(), 0.5 * pix_size)
     else:
-        h_data = data[data._hcol].to_numpy()
+        h_data = data[data.hcol].to_numpy()
 
     grid = get_backend(backend).\
            interpolate_2d_cross(data[x].to_numpy(), data[y].to_numpy(), w_data, h_data, kernel.w,
                                 kernel.get_radius(), pixels, xlim[0], xlim[1], ylim[0], ylim[1])
 
     if normalize:
         w_norm = _get_weight(data, np.array([1] * len(w_data)), dens_weight)
@@ -639,15 +642,16 @@
     pixels: int, optional
         Number of pixels in the output image in the x & y directions. Default values are chosen to keep
         a consistent aspect ratio.
     xlim, ylim, zlim: tuple of float, optional
         Starting and ending coordinates of the cross-section line (in particle data space). Defaults to
         the minimum and maximum values of `x`, `y`, and `z`.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
        If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -695,17 +699,17 @@
     backend = backend if backend is not None else data.backend
 
     if pixels <= 0:
         raise ValueError('pixcount must be greater than zero!')
 
     if hmin:
         pix_size = np.sqrt((xlim[1] - xlim[0])**2 + (ylim[1] - ylim[0])**2 + (zlim[1] - zlim[0])**2) / pixels
-        h_data = np.maximum(data[data._hcol].to_numpy(), 0.5 * pix_size)
+        h_data = np.maximum(data[data.hcol].to_numpy(), 0.5 * pix_size)
     else:
-        h_data = data[data._hcol].to_numpy()
+        h_data = data[data.hcol].to_numpy()
 
     grid = get_backend(backend) \
            .interpolate_3d_line(data[x].to_numpy(), data[y].to_numpy(), data[z].to_numpy(), w_data, h_data,
                                 kernel.w, kernel.get_radius(), pixels, xlim[0], xlim[1], ylim[0], ylim[1], zlim[0],
                                 zlim[1])
 
     if normalize:
@@ -754,15 +758,16 @@
         a consistent aspect ratio.
     xlim, ylim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to True for column-integrated views,
         when the target is not density, and False for everything else.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
@@ -858,15 +863,16 @@
         a consistent aspect ratio.
     xlim, ylim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     exact: bool
         Whether to use exact interpolation of the data.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -963,15 +969,16 @@
     x_pixels, y_pixels: int, optional
         Number of pixels in the output image in the x & y directions. Default values are chosen to keep
         a consistent aspect ratio.
     xlim, ylim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -1062,15 +1069,16 @@
     x_pixels, y_pixels: int, optional
         Number of pixels in the output image in the x & y directions. Default values are chosen to keep
         a consistent aspect ratio.
     xlim, ylim: float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
@@ -1084,14 +1092,15 @@
         If `pixwidthx`, `pixwidthy`, `pixcountx`, or `pixcounty` are less than or equal to zero, or
         if the specified `x` and `y` minimum and maximums result in an invalid region, or
         if the provided data is not 3-dimensional.
     KeyError
         If `target_x`, `target_y`, `target_z`, `x`, `y`, `z`, mass, density, or smoothing length columns do not
         exist in `data`.
     """
+
     _check_dimension(data, 3)
     x, y, z = _default_xyz(data, x, y, z)
     _verify_columns(data, x, y)
 
     # set default slice to be through the data's average z-value.
     if z_slice is None:
         z_slice = _snap(data.loc[:, z].mean())
@@ -1162,15 +1171,16 @@
     x_pixels, y_pixels, z_pixels: int, optional
         Number of pixels in the output image in the x, y & z directions. Default values are chosen to keep
         a consistent aspect ratio.
     xlim, ylim, zlim: tuple of float, optional
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x`, `y` and `z`.
     backend: ['cpu', 'gpu']
-        The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, the target will be multiplied by density. Defaults to False.
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
         contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
 
     Returns
```

### Comparing `sarracen-1.2.1/sarracen/kernels/base_kernel.py` & `sarracen-1.2.2/sarracen/kernels/base_kernel.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/kernels/cubic_spline.py` & `sarracen-1.2.2/sarracen/kernels/cubic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/kernels/cubic_spline_exact.py` & `sarracen-1.2.2/sarracen/kernels/cubic_spline_exact.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/kernels/quartic_spline.py` & `sarracen-1.2.2/sarracen/kernels/quartic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/kernels/quintic_spline.py` & `sarracen-1.2.2/sarracen/kernels/quintic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/readers/read_csv.py` & `sarracen-1.2.2/sarracen/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/readers/read_marisa.py` & `sarracen-1.2.2/sarracen/readers/read_marisa.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/readers/read_phantom.py` & `sarracen-1.2.2/sarracen/readers/read_phantom.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,16 @@
             df_list = []
             for _, group in df.groupby('itype'):
                 itype = int(group["itype"].iloc[0])
                 mass_key = 'massoftype' if itype == 1 else f'massoftype_{itype}'
                 df_list.append(SarracenDataFrame(group.dropna(axis=1),
                                                  params={**header_vars, **{"mass": header_vars[mass_key]}}))
 
-            df_list.append(SarracenDataFrame(df_sinks, params=header_vars))
+            if not df_sinks.empty:
+                df_list.append(SarracenDataFrame(df_sinks, params=header_vars))
 
             return df_list
 
         if (separate_types == 'sinks' or separate_types == 'all') and not df_sinks.empty:
             return [SarracenDataFrame(df, params={**header_vars, **{"mass": header_vars['massoftype']}}),
                     SarracenDataFrame(df_sinks, params=header_vars)]
```

### Comparing `sarracen-1.2.1/sarracen/render.py` & `sarracen-1.2.2/sarracen/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,16 @@
     cbar_ax: Axes
         Axes to draw the colorbar in, if not provided then space will be taken from the main Axes.
     ax: Axes
         The main axes in which to draw the rendered image.
     exact: bool
         Whether to use exact interpolation of the data. For cross-sections this is ignored. Defaults to False.
     backend: ['cpu', 'gpu']
-        The computation backend to use when rendering this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     integral_samples: int, optional
         If using column interpolation, the number of sample points to take when approximating the 2D column kernel.
     rotation: array_like or Rotation, optional
         The rotation to apply to the data before interpolation. If defined as an array, the
         order of rotations is [z, y, x] in degrees. Only applies to 3D datasets.
     rot_origin: array_like, optional
         Point of rotation of the data, in [x, y, z] form. Defaults to the centre
@@ -285,20 +286,21 @@
         ax.set_yticks([])
     else:
         ax.set_xlabel(x)
         ax.set_ylabel(y)
 
     if cbar:
         colorbar = ax.figure.colorbar(graphic, cbar_ax, ax, **cbar_kws)
-        label = target
-        if data.get_dim() == 3 and xsec is None:
-            label = f"column {label}"
-        if log_scale:
-            label = f"log ({label})"
-        colorbar.ax.set_ylabel(label)
+        if 'label' not in cbar_kws :
+            label = target
+            if data.get_dim() == 3 and xsec is None:
+                label = f"column {label}"
+            if log_scale:
+                label = f"log ({label})"
+            colorbar.ax.set_ylabel(label)
 
     return ax
 
 
 def lineplot(data: 'SarracenDataFrame', target: str, x: str = None, y: str = None, z: str = None,
              kernel: BaseKernel = None, pixels: int = 512, xlim: Tuple[float, float] = None,
              ylim: Tuple[float, float] = None, zlim: Tuple[float, float] = None, ax: Axes = None, backend: str = None,
@@ -319,16 +321,16 @@
     pixels: int, optional
         Number of samples taken across the x axis in the final plot.
     xlim, ylim, zlim: tuple of float, optional
         Coordinates of the two points that make up the cross-sectional line.
     ax: Axes
         The main axes in which to draw the final plot.
     backend: ['cpu', 'gpu']
-        The computation backend to use when performing the underlying interpolation. Defaults to the backend
-        specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     log_scale: bool
         Whether to use a logarithmic scale for color coding.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to False.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
     hmin: bool
@@ -447,15 +449,16 @@
         The minimum and maximum values to use in interpolation, in particle data space. Defaults
         to the minimum and maximum values of `x` and `y`.
     ax: Axes
         The main axes in which to draw the rendered image.
     exact: bool
         Whether to use exact interpolation of the data. For cross-sections this is ignored. Defaults to False.
     backend: ['cpu', 'gpu']
-        The computation backend to use when rendering this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to True for column-integrated views
         and False for everything else.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
@@ -578,15 +581,16 @@
     qkey: bool
         Whether to include a quiver key on the final plot.
     qkey_kws: dict
         Keywords to pass through to ax.quiver.
     exact: bool
         Whether to use exact interpolation of the data. For cross-sections this is ignored. Defaults to False.
     backend: ['cpu', 'gpu']
-        The computation backend to use when rendering this data. Defaults to the backend specified in `data`.
+        The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+        'cpu' is used. A manually specified backend in `data` will override the default.
     dens_weight: bool
         If True, will plot the target mutliplied by the density. Defaults to True for column-integrated views
         and False for everything else.
     normalize: bool
         If True, will normalize the interpolation. Defaults to False (this may change in future versions).
     hmin: bool
         If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
```

### Comparing `sarracen-1.2.1/sarracen/sarracen_dataframe.py` & `sarracen-1.2.2/sarracen/sarracen_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Union, Callable, Tuple
 
 from matplotlib.axes import Axes
 from matplotlib.colors import Colormap
 from pandas import DataFrame, Series
+from numba import cuda
 import numpy as np
 
 from .render import streamlines, arrowplot, render, lineplot
 from .interpolate import interpolate_2d, interpolate_3d_grid
 from .kernels import CubicSplineKernel, BaseKernel
 
-from typing import Tuple
 
 def _copy_doc(copy_func: Callable) -> Callable:
     """Copy documentation from another function to this function."""
     def wrapper(func: Callable) -> Callable:
         func.__doc__ = copy_func.__doc__
         return func
     return wrapper
@@ -100,15 +100,15 @@
         self._units = None
         self.units = Series([np.nan for _ in range(len(self.columns))])
 
         self._xcol, self._ycol, self._zcol, self._hcol, self._mcol, self._rhocol = None, None, None, None, None, None
         self._identify_special_columns()
 
         self._kernel = CubicSplineKernel()
-        self._backend = 'cpu'
+        self._backend = 'gpu' if cuda.is_available() else 'cpu'
 
     @property
     def _constructor(self):
         return SarracenDataFrame
 
     def _identify_special_columns(self):
         """
@@ -121,49 +121,49 @@
 
         If the x or y columns cannot be found, they are set to be the first two columns by default.
         If the z, smoothing length, mass, or density columns cannot be sound, the corresponding column
         label is set to `None`.
         """
         # First look for 'x', then 'rx', and then fallback to the first column.
         if 'x' in self.columns:
-            self._xcol = 'x'
+            self.xcol = 'x'
         elif 'rx' in self.columns:
-            self._xcol = 'rx'
-        else:
-            self._xcol = self.columns[0]
+            self.xcol = 'rx'
+        elif len(self.columns) > 0:
+            self.xcol = self.columns[0]
 
         # First look for 'y', then 'ry', and then fallback to the second column.
         if 'y' in self.columns:
-            self._ycol = 'y'
+            self.ycol = 'y'
         elif 'ry' in self.columns:
-            self._ycol = 'ry'
-        else:
-            self._ycol = self.columns[1]
+            self.ycol = 'ry'
+        elif len(self.columns) > 1:
+            self.ycol= self.columns[1]
 
         # First look for 'z', then 'rz', and then assume that data is 2 dimensional.
         if 'z' in self.columns:
-            self._zcol = 'z'
+            self.zcol = 'z'
         elif 'rz' in self.columns:
-            self._zcol = 'rz'
+            self.zcol = 'rz'
 
         # Look for the keyword 'h' in the data.
         if 'h' in self.columns:
-            self._hcol = 'h'
+            self.hcol = 'h'
 
         # Look for the keyword 'm' or 'mass' in the data.
         if 'm' in self.columns:
-            self._mcol = 'm'
+            self.mcol = 'm'
         elif 'mass' in self.columns:
-            self._mcol = 'mass'
+            self.mcol = 'mass'
 
         # Look for the keyword 'rho' or 'density' in the data.
         if 'rho' in self.columns:
-            self._rhocol = 'rho'
+            self.rhocol = 'rho'
         elif 'density' in self.columns:
-            self._rhocol = 'density'
+            self.rhocol = 'density'
 
     def create_mass_column(self):
         """
         Create a new column 'm', copied from the 'massoftype' dataset parameter.
 
         Intended for use with Phantom data dumps.
 
@@ -172,15 +172,15 @@
         KeyError
             If the 'massoftype' column does not exist in `params`.
         """
         if 'mass' not in self.params:
             raise KeyError("'mass' value does not exist in this SarracenDataFrame.")
 
         self['m'] = self.params['mass']
-        self._mcol = 'm'
+        self.mcol = 'm'
 
     def calc_density(self):
         """
         Create a new column 'rho' that contains particle densities.
 
         Density for each particle is calculated according to
 
@@ -201,18 +201,18 @@
             raise KeyError('hfact missing from params in this SarracenDataFrame.')
         if not {self.mcol}.issubset(self.columns) and 'mass' not in self.params:
             raise KeyError('Missing particle mass data in this SarracenDataFrame.')
 
         mass = self.params['mass']
         # prioritize using mass per particle, if present
         if {self.mcol}.issubset(self.columns):
-            mass = self[self._mcol]
+            mass = self[self.mcol]
 
-        self['rho'] = (self.params['hfact'] / self['h']) ** (self.get_dim()) * mass
-        self._rhocol = 'rho'
+        self['rho'] = (self.params['hfact'] / self[self.hcol]) ** (self.get_dim()) * mass
+        self.rhocol = 'rho'
 
     @_copy_doc(render)
     def render(self, target: str, x: str = None, y: str = None, z: str = None, xsec: float = None,
                kernel: BaseKernel = None, x_pixels: int = None, y_pixels: int = None, xlim: Tuple[float, float] = None,
                ylim: Tuple[float, float] = None, cmap: Union[str, Colormap] = 'gist_heat', cbar: bool = True,
                cbar_kws: dict = {}, cbar_ax: Axes = None, ax: Axes = None, exact: bool = None, backend: str = None,
                integral_samples: int = 1000, rotation: np.ndarray = None, rot_origin: np.ndarray = None,
@@ -281,15 +281,16 @@
             a consistent aspect ratio.
         xlim, ylim, zlim: tuple of float, optional
             The minimum and maximum values to use in interpolation, in particle data space. Defaults
             to the minimum and maximum values of `x`, `y` and `z`.
         exact: bool
             Whether to use exact interpolation of the data. Only applies to 2D datasets.
         backend: ['cpu', 'gpu']
-            The computation backend to use when interpolating this data. Defaults to the backend specified in `data`.
+            The computation backend to use when interpolating this data. Defaults to 'gpu' if CUDA is enabled, otherwise
+            'cpu' is used. A manually specified backend in `data` will override the default.
         dens_weight: bool
             If True, the target will be multiplied by density. Defaults to False.
         normalize: bool
             If True, will normalize the interpolation. Defaults to False (this may change in future versions).
         hmin: bool
             If True, a minimum smoothing length of 0.5 * pixel size will be imposed. This ensures each particle
             contributes to at least one grid cell / pixel. Defaults to False (this may change in a future verison).
@@ -475,8 +476,8 @@
         Get the dimensionality of the data in this dataframe.
 
         Returns
         -------
         int
             The number of positional dimensions.
         """
-        return 3 if self._zcol is not None else 2
+        return 3 if self.zcol is not None else 2
```

### Comparing `sarracen-1.2.1/sarracen/tests/readers/test_read_csv.py` & `sarracen-1.2.2/sarracen/tests/readers/test_read_csv.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/tests/test_interpolate.py` & `sarracen-1.2.2/sarracen/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/tests/test_kernels.py` & `sarracen-1.2.2/sarracen/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/tests/test_render.py` & `sarracen-1.2.2/sarracen/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/sarracen/tests/test_sarracen_dataframe.py` & `sarracen-1.2.2/sarracen/tests/test_sarracen_dataframe.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.1/PKG-INFO` & `sarracen-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarracen
-Version: 1.2.1
+Version: 1.2.2
 Summary: SPH analysis and visualization
 Author-email: "Terrence S. Tricco" <tstricco@mun.ca>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: numba>=0.55.1
 Requires-Dist: pandas>=1.4
@@ -57,7 +57,16 @@
 Code submissions should be submitted as a pull request. Make sure that all existing unit tests successfully pass, and 
 please add any new unit tests that are relevant. Documentation changes should also be submitted as a pull request.
 
 If you are stuck or need help, [raising an issue](https://github.com/ttricco/sarracen/issues) is a good place to start. 
 This helps us keep common issues in public view. Feel free to also [email](mailto:tstricco@mun.ca) with questions.
 
 Please note that we adhere to a [code of conduct](CODE_OF_CONDUCT.md).
+
+Citation
+--------
+
+Please cite the paper if you use Sarracen within your work (DOI: [10.21105/joss.05263](https://doi.org/10.21105/joss.05263)).
+
+*Sarracen: a Python package for analysis and visualization of smoothed particle hydrodynamics data.* Journal of Open Source Software, 8(86), 5263, 2023. 
+
+
```

