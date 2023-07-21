# Comparing `tmp/pytearcat-0.0.5.tar.gz` & `tmp/pytearcat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytearcat-0.0.5.tar", last modified: Thu Jun 16 15:11:30 2022, max compression
+gzip compressed data, was "pytearcat-0.0.6.tar", last modified: Fri Jul 21 21:38:43 2023, max compression
```

## Comparing `pytearcat-0.0.5.tar` & `pytearcat-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 joaquin    (501) staff       (20)        0 2022-06-16 15:11:30.298653 pytearcat-0.0.5/
--rw-r--r--   0 joaquin    (501) staff       (20)     5593 2022-06-16 15:11:30.298488 pytearcat-0.0.5/PKG-INFO
--rw-r--r--   0 joaquin    (501) staff       (20)     4708 2022-06-02 17:45:43.000000 pytearcat-0.0.5/README.md
--rw-r--r--   0 joaquin    (501) staff       (20)     4958 2022-06-02 17:35:44.000000 pytearcat-0.0.5/README.rst
-drwxr-xr-x   0 joaquin    (501) staff       (20)        0 2022-06-16 15:11:30.291497 pytearcat-0.0.5/pytearcat/
--rw-r--r--   0 joaquin    (501) staff       (20)      432 2022-05-31 16:23:44.000000 pytearcat-0.0.5/pytearcat/__init__.py
-drwxr-xr-x   0 joaquin    (501) staff       (20)        0 2022-06-16 15:11:30.293629 pytearcat-0.0.5/pytearcat/gr/
--rw-r--r--   0 joaquin    (501) staff       (20)      343 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/__init__.py
--rw-r--r--   0 joaquin    (501) staff       (20)     7622 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/christoffel.py
--rw-r--r--   0 joaquin    (501) staff       (20)     2617 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/einstein.py
--rw-r--r--   0 joaquin    (501) staff       (20)     1693 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/geodesic.py
--rw-r--r--   0 joaquin    (501) staff       (20)     9158 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/metric.py
--rw-r--r--   0 joaquin    (501) staff       (20)     3187 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/ricci.py
--rw-r--r--   0 joaquin    (501) staff       (20)     6754 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/gr/riemann.py
-drwxr-xr-x   0 joaquin    (501) staff       (20)        0 2022-06-16 15:11:30.294889 pytearcat-0.0.5/pytearcat/tensor/
--rw-r--r--   0 joaquin    (501) staff       (20)      289 2022-05-31 16:23:44.000000 pytearcat-0.0.5/pytearcat/tensor/__init__.py
-drwxr-xr-x   0 joaquin    (501) staff       (20)        0 2022-06-16 15:11:30.298109 pytearcat-0.0.5/pytearcat/tensor/core/
--rw-r--r--   0 joaquin    (501) staff       (20)       28 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/__init__.py
--rw-r--r--   0 joaquin    (501) staff       (20)     4020 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/config.py
--rw-r--r--   0 joaquin    (501) staff       (20)     1270 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/core.py
--rw-r--r--   0 joaquin    (501) staff       (20)     4749 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/display.py
--rw-r--r--   0 joaquin    (501) staff       (20)    18856 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/distribute.py
--rw-r--r--   0 joaquin    (501) staff       (20)      229 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/error.py
--rw-r--r--   0 joaquin    (501) staff       (20)        8 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/fun.py
--rw-r--r--   0 joaquin    (501) staff       (20)     9471 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/gpwrap.py
--rw-r--r--   0 joaquin    (501) staff       (20)     1208 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/greek.py
--rw-r--r--   0 joaquin    (501) staff       (20)     9584 2022-06-01 12:24:15.000000 pytearcat-0.0.5/pytearcat/tensor/core/interp.py
--rw-r--r--   0 joaquin    (501) staff       (20)       63 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/core/ptseries.py
--rw-r--r--   0 joaquin    (501) staff       (20)    14431 2022-06-13 21:13:45.000000 pytearcat-0.0.5/pytearcat/tensor/core/tdata.py
--rw-r--r--   0 joaquin    (501) staff       (20)    22296 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/kdelta.py
--rw-r--r--   0 joaquin    (501) staff       (20)    22124 2021-12-04 22:06:18.000000 pytearcat-0.0.5/pytearcat/tensor/lcivita.py
--rw-r--r--   0 joaquin    (501) staff       (20)     9634 2022-06-01 12:45:08.000000 pytearcat-0.0.5/pytearcat/tensor/misc.py
--rw-r--r--   0 joaquin    (501) staff       (20)    64636 2022-06-15 15:41:51.000000 pytearcat-0.0.5/pytearcat/tensor/tensor.py
-drwxr-xr-x   0 joaquin    (501) staff       (20)        0 2022-06-16 15:11:30.292307 pytearcat-0.0.5/pytearcat.egg-info/
--rw-r--r--   0 joaquin    (501) staff       (20)     5593 2022-06-16 15:11:30.000000 pytearcat-0.0.5/pytearcat.egg-info/PKG-INFO
--rw-r--r--   0 joaquin    (501) staff       (20)      908 2022-06-16 15:11:30.000000 pytearcat-0.0.5/pytearcat.egg-info/SOURCES.txt
--rw-r--r--   0 joaquin    (501) staff       (20)        1 2022-06-16 15:11:30.000000 pytearcat-0.0.5/pytearcat.egg-info/dependency_links.txt
--rw-r--r--   0 joaquin    (501) staff       (20)       92 2022-06-16 15:11:30.000000 pytearcat-0.0.5/pytearcat.egg-info/requires.txt
--rw-r--r--   0 joaquin    (501) staff       (20)       10 2022-06-16 15:11:30.000000 pytearcat-0.0.5/pytearcat.egg-info/top_level.txt
--rw-r--r--   0 joaquin    (501) staff       (20)       38 2022-06-16 15:11:30.298712 pytearcat-0.0.5/setup.cfg
--rw-r--r--   0 joaquin    (501) staff       (20)      862 2022-06-16 15:10:23.000000 pytearcat-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:43.637910 pytearcat-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 21:38:39.000000 pytearcat-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-21 21:38:43.633910 pytearcat-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-21 21:38:39.000000 pytearcat-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:43.629910 pytearcat-0.0.6/pytearcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:43.633910 pytearcat-0.0.6/pytearcat/gr/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/christoffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/einstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/ricci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/gr/riemann.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:43.633910 pytearcat-0.0.6/pytearcat/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:43.633910 pytearcat-0.0.6/pytearcat/tensor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/gpwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/greek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/ptseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/core/tdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/kdelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/lcivita.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67103 2023-07-21 21:38:39.000000 pytearcat-0.0.6/pytearcat/tensor/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:43.629910 pytearcat-0.0.6/pytearcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-21 21:38:43.000000 pytearcat-0.0.6/pytearcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-21 21:38:43.000000 pytearcat-0.0.6/pytearcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:38:43.000000 pytearcat-0.0.6/pytearcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-21 21:38:43.000000 pytearcat-0.0.6/pytearcat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 21:38:43.000000 pytearcat-0.0.6/pytearcat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 21:38:43.637910 pytearcat-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 21:38:42.000000 pytearcat-0.0.6/setup.py
```

### Comparing `pytearcat-0.0.5/PKG-INFO` & `pytearcat-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,54 @@
-Metadata-Version: 2.1
-Name: pytearcat
-Version: 0.0.5
-Summary: A package to perform tensor algebra calculations.
-Home-page: https://github.com/pytearcat/pytearcat
-Author: Joaquin Sureda
-Author-email: jmsureda@uc.cl
-License: LICENCE
-Description: # Pytearcat: PYthon TEnsor AlgebRa calCulATor - A python package for general relativity and tensor calculus
-        
-        Pytearcat is an open-source Python package created to work with general tensor operations, either in the field of General Relativity (GR) or others that need to use tensor calculus. It provides the basic GR tensors built in the package and uses a standard syntax for the Einstein notation. 
-        
-        ## Installation
-        
-        As a Python package, Pytearcat can be installed through pip using
-        
-        ```bash
-        pip install pytearcat
-        ```
-        To use the Giacpy core in Pytearcat, the user must explicitly indicate during the package installation that the installer must include the Giacpy module in the process. This is done through
-        
-        ```bash
-        pip install pytearcat[giapy]
-        ```
-        
-        ## File structure summary
-        Inside the Pytearcat package, there are two sub-packages named _gr_ and _tensor_. Inside the first one, there are six modules related to GR expressions. These libraries allow calculating quantities that are very common in GR, such as the Christoffel symbols (first and the second kind, _christoffel.py_), the Ricci tensor and the Ricci scalar (_ricci.py_), the Riemann tensor (_riemann.py_) and the Einstein tensor (_einstein.py_). Also, there is a module to define the metric (_metric.py_) and another to calculate the geodesics (_geodesic.py_).
-        The second sub-package named _tensor_ contains modules that allow to define tensors and operate with them. The _misc.py_ module contains functions that allow defining symbolic functions, variables, and constants. It also contains other functions to work with series expansions and to simplify expressions. The _kdelta.py_ and _lcivita.py_ modules contain the data classes which define the Kronecker Delta symbol and the Levi-Civita symbol, respectively. 
-        The _tensor.py_ module contains the code related with the class _tensor_ and many functions that are useful to define a tensor, operate tensors, recognise the contravariant and covariant indices, lower and raise indices and expand a tensor like a series up to a specific order. Inside this sub-package, there is another one named _core_ which contains essential information that the program needs to operate tensors. All the functions required by the user are located at the top level of the package. 
-        
-        ## Usage
-        
-        Pytearcat works using Jupyter Notebooks to give the outputs in mathematical form. To use the package the user should import Pytearcat within a Jypyter Notebook
-        
-        ```python
-        import pytearcat as pt
-        ```
-        
-        Later, it is possible to access the functions and methods of the package within the notebook. Different usage examples can be found in the top directory of the GitHub repository.
-        
-        ## How to cite this work
-        
-        To cite this work, please refer to Pytearcat's release paper [San Martin & Sureda (2021)](https://doi.org/10.1016/j.ascom.2022.100572) (also available on [arXiv](https://arxiv.org/abs/2106.15016)) and use the following Bibtex citation:
-        
-        
-        ```
-        @article{pytearcat2022,
-        	abstract = {This paper introduces the first release of Pytearcat, a Python package developed to compute tensor algebra operations in the context of theoretical physics, for instance, in general relativity. Given that working with tensors can become a complex task, people often rely on computational tools to perform tensor calculations. We aim to build a tensor calculator based on Python, which benefits from being free and easy to use. Pytearcat syntax resembles the usual physics notation for tensor calculus, such as the Einstein notation for index contraction. This version allows the user to perform many tensor operations, including derivatives and series expansions, along with routines to obtain the typical General Relativity tensors. A particular concern was put in the execution times, leading to incorporate an alternative core for the symbolic calculations, enabling to reach much faster execution times. The syntax and the versatility of Pytearcat are the most important features of this package, where the latter can be used to extend Pytearcat to other areas of theoretical physics.},
-        	author = {M. San Mart\'in and J. Sureda},
-        	doi = {https://doi.org/10.1016/j.ascom.2022.100572},
-        	issn = {2213-1337},
-        	journal = {Astronomy and Computing},
-        	keywords = {Software, Public release, General relativity, Tensor algebra, Computer algebra system},
-        	pages = {100572},
-        	title = {Pytearcat: PYthon TEnsor AlgebRa calCulATor A python package for general relativity and tensor calculus},
-        	url = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
-        	year = {2022},
-        	Bdsk-Url-1 = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
-        	Bdsk-Url-2 = {https://doi.org/10.1016/j.ascom.2022.100572}}
-        
-        ```
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-Provides-Extra: giacpy
+# Pytearcat: PYthon TEnsor AlgebRa calCulATor - A python package for general relativity and tensor calculus
+
+Pytearcat is an open-source Python package created to work with general tensor operations, either in the field of General Relativity (GR) or others that need to use tensor calculus. It provides the basic GR tensors built in the package and uses a standard syntax for the Einstein notation. 
+
+## Installation
+
+As a Python package, Pytearcat can be installed through pip using
+
+```bash
+pip install pytearcat
+```
+To use the Giacpy core in Pytearcat, the user must explicitly indicate during the package installation that the installer must include the Giacpy module in the process. This is done through
+
+```bash
+pip install pytearcat[giapy]
+```
+
+## File structure summary
+Inside the Pytearcat package, there are two sub-packages named _gr_ and _tensor_. Inside the first one, there are six modules related to GR expressions. These libraries allow calculating quantities that are very common in GR, such as the Christoffel symbols (first and the second kind, _christoffel.py_), the Ricci tensor and the Ricci scalar (_ricci.py_), the Riemann tensor (_riemann.py_) and the Einstein tensor (_einstein.py_). Also, there is a module to define the metric (_metric.py_) and another to calculate the geodesics (_geodesic.py_).
+The second sub-package named _tensor_ contains modules that allow to define tensors and operate with them. The _misc.py_ module contains functions that allow defining symbolic functions, variables, and constants. It also contains other functions to work with series expansions and to simplify expressions. The _kdelta.py_ and _lcivita.py_ modules contain the data classes which define the Kronecker Delta symbol and the Levi-Civita symbol, respectively. 
+The _tensor.py_ module contains the code related with the class _tensor_ and many functions that are useful to define a tensor, operate tensors, recognise the contravariant and covariant indices, lower and raise indices and expand a tensor like a series up to a specific order. Inside this sub-package, there is another one named _core_ which contains essential information that the program needs to operate tensors. All the functions required by the user are located at the top level of the package. 
+
+## Usage
+
+Pytearcat works using Jupyter Notebooks to give the outputs in mathematical form. To use the package the user should import Pytearcat within a Jypyter Notebook
+
+```python
+import pytearcat as pt
+```
+
+Later, it is possible to access the functions and methods of the package within the notebook. Different usage examples can be found in the top directory of the GitHub repository.
+
+## How to cite this work
+
+To cite this work, please refer to Pytearcat's release paper [San Martin & Sureda (2021)](https://doi.org/10.1016/j.ascom.2022.100572) (also available on [arXiv](https://arxiv.org/abs/2106.15016)) and use the following Bibtex citation:
+
+
+```
+@article{pytearcat2022,
+	abstract = {This paper introduces the first release of Pytearcat, a Python package developed to compute tensor algebra operations in the context of theoretical physics, for instance, in general relativity. Given that working with tensors can become a complex task, people often rely on computational tools to perform tensor calculations. We aim to build a tensor calculator based on Python, which benefits from being free and easy to use. Pytearcat syntax resembles the usual physics notation for tensor calculus, such as the Einstein notation for index contraction. This version allows the user to perform many tensor operations, including derivatives and series expansions, along with routines to obtain the typical General Relativity tensors. A particular concern was put in the execution times, leading to incorporate an alternative core for the symbolic calculations, enabling to reach much faster execution times. The syntax and the versatility of Pytearcat are the most important features of this package, where the latter can be used to extend Pytearcat to other areas of theoretical physics.},
+	author = {M. San Mart\'in and J. Sureda},
+	doi = {https://doi.org/10.1016/j.ascom.2022.100572},
+	issn = {2213-1337},
+	journal = {Astronomy and Computing},
+	keywords = {Software, Public release, General relativity, Tensor algebra, Computer algebra system},
+	pages = {100572},
+	title = {Pytearcat: PYthon TEnsor AlgebRa calCulATor A python package for general relativity and tensor calculus},
+	url = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
+	year = {2022},
+	Bdsk-Url-1 = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
+	Bdsk-Url-2 = {https://doi.org/10.1016/j.ascom.2022.100572}}
+
+```
+
```

### Comparing `pytearcat-0.0.5/README.md` & `pytearcat-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pytearcat
+Version: 0.0.6
+Summary: A package to perform tensor algebra calculations.
+Home-page: https://github.com/pytearcat/pytearcat
+Author: Joaquin Sureda
+Author-email: jmsureda@uc.cl
+License: LICENCE
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Description-Content-Type: text/markdown
+Provides-Extra: giacpy
+License-File: LICENSE
+
 # Pytearcat: PYthon TEnsor AlgebRa calCulATor - A python package for general relativity and tensor calculus
 
 Pytearcat is an open-source Python package created to work with general tensor operations, either in the field of General Relativity (GR) or others that need to use tensor calculus. It provides the basic GR tensors built in the package and uses a standard syntax for the Einstein notation. 
 
 ## Installation
 
 As a Python package, Pytearcat can be installed through pip using
```

### Comparing `pytearcat-0.0.5/pytearcat/gr/christoffel.py` & `pytearcat-0.0.6/pytearcat/gr/christoffel.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,41 @@
 
             raise SyntaxError("Christoffel can be only first or second kind.")
 
 
 
 
 def calculate_christoffel(First_kind=True,Second_kind=True):
+
+    r"""Christoffel
+
+    Computes the Christoffel symbol
+
+    Parameters
+    ----------
+    First_kind : Boolean, optional
+        This boolean indicates if the first kind Christoffel symbol should be calculated. (Default = True)
+    Second_kind : Boolean, optional
+        This boolean indicates if the second kind Christoffel symbol should be calculated. (Default = True)
+
+    Raises
+    ------
+    ValueError
+        If both arguments are False.
+    
+    Examples
+    --------
+        Computing the Christoffel symbols
+        
+        >>> Chr = pt.christoffel()
+
+        Christoffel :math:`\Gamma_{\alpha \beta \gamma}` and :math:`\Gamma^{\alpha}_{\beta \gamma}`
+            0%|          | 0/64 [00:00<?, ?it/s]
+
+    """
     
     global Christoffel
     
     g = config.g
     var = list(config.coords.values())
     dim = config.dim
     ord_status = config.ord_status
```

### Comparing `pytearcat-0.0.5/pytearcat/gr/einstein.py` & `pytearcat-0.0.6/pytearcat/gr/einstein.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/gr/geodesic.py` & `pytearcat-0.0.6/pytearcat/gr/geodesic.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/gr/metric.py` & `pytearcat-0.0.6/pytearcat/gr/metric.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,52 @@
     import io
     from contextlib import redirect_stdout
     from pytearcat.tensor.core.display import gp_pretty_latex
 
 
 def create_metric(ds2 = ''):
 
+    r'''
+    It defines the metric. 
+
+    Parameters
+    ----------
+    ds2 : str
+        string indicating line element representing the metric to be used
+
+    Raises
+    ------
+    TypeError
+        If the argument received is not a string.
+
+    Examples
+    --------
+    
+    >>> # Define the coordinates to be used
+    >>> t,x,y,z = pt.coords('t,x,y,z')
+    >>> # Define any constant (more than one constant can be defined at the same time)
+    >>> a = pt.fun('a','t')
+    >>> g = pt.metric('ds2 = -dt**2 + a**2*(dx**2 + dy**2 + dz**2)')
+
+    Remember that the time coordinate must be the first coordinate.
+
+    Dimension = 4
+
+    Coordinates = t,x,y,z
+    
+    Metric defined successfully: 
+
+    .. math::
+        ds^2 = -1 \cdot dt^2+a^{2}{\left(t \right)} \cdot dx^2+a^{2}{\left(t \right)} \cdot dy^2+a^{2}{\left(t \right)} \cdot dz^2
+
+    .. math::
+        \displaystyle \left[\begin{matrix}-1 & 0 & 0 & 0\\0 & a^{2}{\left(t \right)} & 0 & 0\\0 & 0 & a^{2}{\left(t \right)} & 0\\0 & 0 & 0 & a^{2}{\left(t \right)}\end{matrix}\right]
+    
+    '''
+
     global g
 
     if config.g_status == True:
 
         answer = input('The metric has already been defined. Do you want to overwrite it? (yes/no)')
 
         if answer == 'yes' or answer == 'y' or answer == 'Y' or answer == 'YES':
@@ -345,15 +383,31 @@
     return dict(zip(a,b))
 
 def def_coords(coords):
 
     '''
     It defines the coordinates of the manifold. 
 
-    coords = 't,x,y,z'
+    Parameters
+    ----------
+    coords : str
+        string indicating the indices combination used to start the complete method
+
+    Raises
+    ------
+    TypeError
+        If the argument received is not a string.
+
+    Examples
+    --------
+    Assuming you have defined a tensor A with indices '_i,^j', i.e. $A_{i}^{j}$, we can calculate the other indices combinations by writting 
+
+    >>> t,x,y,z = pt.coords('t,x,y,z')
+    
+    Remember that the time coordinate must be the first coordinate.
     
     '''
 
     if not isinstance(coords,str):
 
         raise TypeError("The argument must be a string.")
```

### Comparing `pytearcat-0.0.5/pytearcat/gr/ricci.py` & `pytearcat-0.0.6/pytearcat/gr/ricci.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/gr/riemann.py` & `pytearcat-0.0.6/pytearcat/gr/riemann.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,37 @@
 from pytearcat.tensor.core import config
 from pytearcat.tensor.tensor import construct, tensor_series, Tensor
 
 from .christoffel import calculate_christoffel, D
 
 def calculate_riemann(default = True, All = False):
 
+    r"""Riemann Tensor
+
+    Computes the Riemann tensor
+
+    Parameters
+    ----------
+    default : Boolean, optional
+        This boolean indicates only the component :math: `R^{\alpha}_{\beta \gamma \delta}`should be calculated. (Default = True)
+    All : Boolean, optional
+        This boolean indicates if all the tensor components should be calculated. (Default = True)
+
+    
+    Examples
+    --------
+        Computing the Christoffel symbols
+        
+        >>> Chr = pt.christoffel()
+
+        Christoffel :math:`\Gamma_{\alpha \beta \gamma}` and :math:`\Gamma^{\alpha}_{\beta \gamma}`
+            0%|          | 0/64 [00:00<?, ?it/s]
+
+    """
+
     # Riemann (_,_,_,_)
 
     global Riemann
 
     dim = config.dim
 
     if config.riemann is None:
```

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/config.py` & `pytearcat-0.0.6/pytearcat/tensor/core/config.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/core.py` & `pytearcat-0.0.6/pytearcat/tensor/core/core.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/display.py` & `pytearcat-0.0.6/pytearcat/tensor/core/display.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/distribute.py` & `pytearcat-0.0.6/pytearcat/tensor/core/distribute.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/gpwrap.py` & `pytearcat-0.0.6/pytearcat/tensor/core/gpwrap.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/greek.py` & `pytearcat-0.0.6/pytearcat/tensor/core/greek.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/interp.py` & `pytearcat-0.0.6/pytearcat/tensor/core/interp.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/core/tdata.py` & `pytearcat-0.0.6/pytearcat/tensor/core/tdata.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/kdelta.py` & `pytearcat-0.0.6/pytearcat/tensor/kdelta.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/lcivita.py` & `pytearcat-0.0.6/pytearcat/tensor/lcivita.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/misc.py` & `pytearcat-0.0.6/pytearcat/tensor/misc.py`

 * *Files identical despite different names*

### Comparing `pytearcat-0.0.5/pytearcat/tensor/tensor.py` & `pytearcat-0.0.6/pytearcat/tensor/tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,19 +74,25 @@
 
         else:
             pass
 
 
 def bajarindice(tensor,i,kstring,kstring2):
 
-    # i: primera posicion que tiene un indice arriba ej: en un string de indices '_,^,^' -> i = 1 (contando desde 0)
+    '''
+    tensor: Tensor object for which we want to lower their indices
+
+    i: first position that has an upper index i.e. in a string of indices '_,^,^' -> i = 1 (counting from 0)
 
-    # kstring: string original de los indices tensor ej: '_,^,^'
+    kstring: original string containing the tensor indices e.g. '_,^,^'
 
-    # kstring2: string objetivo (con el indice i abajo) de los indices del tencor ej: '_,_,^'
+    kstring2: target string (with the i string down) for the tensor indices e.g.  '_,_,^'
+
+    TODO: This function should be implemented as a method of the tensor class
+    '''
 
     index = compare(tensor.n,kstring)
 
     index2 = compare(tensor.n,kstring2)
 
     dim = config.dim
 
@@ -156,29 +162,28 @@
 
             bla = 'tensor.tensor[index2]%s = temporal'%iterstring2       # Esto asigna a los indices que queremos llegar
 
         exec(bla,globals(),locals())
 
     tensor.indices[index2] = True
 
-    # hasta aqui todo okidoki uwu
-
-    # ESTA FUNCION SE TENDRA QUE LLAMAR CUANTAS VECES SEA NECESARIA HASTA LLEGAR A TENER TODO ABAJO _ _ _
-
-    # REVISAR EL RESULTADO DE LA PRIMERA BAJADA DE INDICES COMPARAR CON GRTENSOR
-
 
 
 def subirindice(tensor,kstring):
 
-    # Recibe:
+    '''
+    Receives 
 
-    # 1) Nombre de la variable de clase Tensor al cual queremos subir los indices
+    1) Tensor object for which we want to raise their indices
 
-    # 2) string de la forma '_,^,_'
+    2) string like '_,^,_'
+    
+
+    TODO: This function should be implemented as a method of the tensor class
+    '''
 
     index = compare(tensor.n,kstring)
 
     klista = kstring.split(',') # ['_','^','_']
 
     NAME = tensor.name
 
@@ -270,18 +275,23 @@
 
                     tensor.indices[index2] = True
 
             subirindice(tensor,kstring2)
 
 def createfirstindex(tensor,kstring):
 
-    # kstring: string original de los indices ej: '^,_,_' ...
-    # tensor: tensor de la clase Tensor
+    '''
+    tensor: object of tensor class for which we want get the full covariant form
+
+    kstring: original string of the current indices of the tensor e.g. '^,_,_'
+
+    TODO: This function should be implemented as a method of the tensor class
+    '''
 
-    N = tensor.n # Number of index
+    N = tensor.n # Number of indices
 
     objetivo = tensor.sequence[0].split(',') # ['_','_','_']
 
     lista = kstring.split(',')  # ['^','_','_']
 
     for i in range(len(lista)):
 
@@ -691,16 +701,23 @@
                     var += eval('self.%s[Nindex]%s'%(ten_call,old_string),locals(),globals())
 
                 return var 
 
     def space(self):
         
         '''
-        Saves the spatial components of the Tensor on the attribut tensor_sp.
+        Saves the spatial components of the Tensor on the attribute tensor_sp.
+
+
+        Examples
+        --------
+        Assuming you have defined a tensor A it is possible to store its spatial by doing
 
+        >>> A.space()
+        
         '''
         
         for k in range(2**self.n):
             
             index = k
         
             iterstring = ''
@@ -715,23 +732,43 @@
 
                 exec_str = 'self.tensor_sp[%d]%s = self.tensor[%d]%s'%(index,iterstring,index,iterstring2)
 
                 exec(exec_str,locals(),globals())
 
     def series(self,index = None):
 
-        '''
-        Expands each element of the tensor at the given indices.
+        '''Expand each element of the tensor at the corresponding index.
+
+        This method explicitly applies the series expansion up to the order defined.
+
+        Parameters
+        ----------
+            index : str, optional
+                string indicating the indices combination used to start the complete method
+                If not given it applies the method to the tensor with all its covariant indices, i.e, '_i,_j,_...'
+
+        Raises
+        ------
+            ValueError
+                If the 'index' specified does not correspond to any possible indices combination.
+
+        See Also
+        ------
+            misc.setorder()
         
         '''
 
         if index is None:
 
             index = self.sequence[0]
 
+        if (index not in self.sequence) or index == '':
+
+            raise ValueError('Bad index definition')
+
         dim = config.dim
 
         k = 0
         for i in self.sequence:
             if i == index:
                 break 
             k += 1
@@ -752,22 +789,30 @@
 
         '''Calculates the missing indices combintation of the tensor
 
         Calculates the missing indices combintation of the tensor using the metric to raise and lower the indices, starting from the given indices combination
 
         Parameters
         ----------
-        index : str, optional
+        index : str
             string indicating the indices combination used to start the complete method
 
         Raises
         ------
         ValueError
             If the 'index' specified does not correspond to any possible indices combination.
-        - string indicating the starting indices combination i.e., '_,^,_' for a 3-rank tensor.
+
+        Examples
+        --------
+        Assuming you have defined a tensor A with indices '_i,^j', i.e. $A_{i}^{j}$, we can calculate the other indices combinations by writting 
+
+        >>> A.complete('_i,^j)
+        
+        All other indices of A Tensor $A$  already calculated.
+        >>> A.assign(elements, '_i,_j')
         
         '''
 
         if (index not in self.sequence and index is not None) or index == '':
 
             raise ValueError('Bad index definition')
 
@@ -1863,34 +1908,45 @@
 
                 print('All components are zero')
 
 
 
 def D(a,b):
 
-    '''
-    Derivative of a tensor "a" with respect to the index "b".
+    """Derivative
 
-    a is an object of class Tdata
-    b is a string that indicates the index, written as "_index"
+    Computes the derivative for the Tensor 'a' with respect to the index 'b'.
 
-    It returns an object of class Tdata. 
+    Parameters
+    ----------
+    a : Tdata
+        Tdata instance corresponding to the Tensor for which the derivative will be applied.
+    b : str
+        string corresponding to the index for the covariant derivative.
 
-    -------------
-    Example:
+    Raises
+    ------
+    TensorSyntaxError
+        If the arguments passed have syntax errors.
+    
+    Examples
+    --------
+    Assigning a nested list to a 'Tensor'
 
-    A = D(G("^a, ^b"), "_c")
+    >>> A = D(G("^a, ^b"), "_c")
 
     We suggest to save this into a Tensor object as
 
-    B = ten("B", 3)
+    >>> B = ten("B", 3)
 
-    B.assign(A, "^a, ^b, _c")
+    >>> B.assign(A, "^a, ^b, _c")
 
-    '''
+    >>> Elements assigned correctly to the ^a,^b,_j components
+
+    """
 
     der_examine(b)
 
     if config.space_time == True:
 
         dim = config.dim
 
@@ -2050,34 +2106,44 @@
 
             exec(string,locals(),globals())
         
         return Tdata(string_return, temp)
 
 def C(a,b):
 
-    '''
-    Covariant derivative of a tensor "a" with respect to the index "b".
+    """Covariant derivative
 
-    a is an object of class Tdata
-    b is a string that indicates the index, written as "_index"
+    Computes the covariant derivative for the Tensor 'a' with respect to the index 'b'.
 
-    It returns an object of class Tdata. 
-
-    -------------
-    Example:
+    Parameters
+    ----------
+    a : Tdata
+        Tdata instance corresponding to the Tensor for wich the covariant derivative will be applied.
+    b : str
+        string corresponding to the index for the covariant derivative.
 
-    A = C(G("^a, ^b"), "_c")
+    Raises
+    ------
+    TensorSyntaxError
+        If the arguments passed have syntax errors.
+    
+    Examples
+    --------
+    Assigning a nested list to a 'Tensor'
 
+    >>> A = C(G("^a, ^b"), "_c")
     We suggest to save this into a Tensor object as
 
-    B = ten("B", 3)
+    >>> B = ten("B", 3)
 
-    B.assign(A, "^a, ^b, _c")
+    >>> B.assign(A, "^a, ^b, _c")
 
-    '''
+    Elements assigned correctly to the ^a,^b,_j components
+
+    """
 
     der_examine(b)
 
     if config.space_time == True:
 
         dim = config.dim
 
@@ -2245,14 +2311,44 @@
     
     T.factor((',').join(TD.updn))
     
     return T
 
 def determinant(T):
 
+    """Determinant
+
+    Utility to compute the determinant of a rank 2 'Tensor' T
+
+    Parameters
+    ----------
+    T : Tensor
+        Rank 2 'Tensor' instance.
+
+    Raises
+    ------
+    ValueError
+        If it receives anything else than a 'Tensor' object.
+        If it is not a rank 2 tensor.
+    
+    Examples
+    --------
+    Assigning a nested list to a 'Tensor'
+
+    >>>  = C(G("^a, ^b"), "_c")
+    We suggest to save this into a Tensor object as
+
+    >>> B = ten("B", 3)
+
+    >>> B.assign(A, "^a, ^b, _c")
+
+    Elements assigned correctly to the ^a,^b,_j components
+
+    """
+
     if not isinstance(T,Tdata):
 
         raise(ValueError("T must ve a Tdata instance."))
     
     if len(T.updn) != 2: 
         
         raise(ValueError("Must be a rank 2 tensor"))
```

### Comparing `pytearcat-0.0.5/pytearcat.egg-info/PKG-INFO` & `pytearcat-0.0.6/pytearcat.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 Metadata-Version: 2.1
 Name: pytearcat
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to perform tensor algebra calculations.
 Home-page: https://github.com/pytearcat/pytearcat
 Author: Joaquin Sureda
 Author-email: jmsureda@uc.cl
 License: LICENCE
-Description: # Pytearcat: PYthon TEnsor AlgebRa calCulATor - A python package for general relativity and tensor calculus
-        
-        Pytearcat is an open-source Python package created to work with general tensor operations, either in the field of General Relativity (GR) or others that need to use tensor calculus. It provides the basic GR tensors built in the package and uses a standard syntax for the Einstein notation. 
-        
-        ## Installation
-        
-        As a Python package, Pytearcat can be installed through pip using
-        
-        ```bash
-        pip install pytearcat
-        ```
-        To use the Giacpy core in Pytearcat, the user must explicitly indicate during the package installation that the installer must include the Giacpy module in the process. This is done through
-        
-        ```bash
-        pip install pytearcat[giapy]
-        ```
-        
-        ## File structure summary
-        Inside the Pytearcat package, there are two sub-packages named _gr_ and _tensor_. Inside the first one, there are six modules related to GR expressions. These libraries allow calculating quantities that are very common in GR, such as the Christoffel symbols (first and the second kind, _christoffel.py_), the Ricci tensor and the Ricci scalar (_ricci.py_), the Riemann tensor (_riemann.py_) and the Einstein tensor (_einstein.py_). Also, there is a module to define the metric (_metric.py_) and another to calculate the geodesics (_geodesic.py_).
-        The second sub-package named _tensor_ contains modules that allow to define tensors and operate with them. The _misc.py_ module contains functions that allow defining symbolic functions, variables, and constants. It also contains other functions to work with series expansions and to simplify expressions. The _kdelta.py_ and _lcivita.py_ modules contain the data classes which define the Kronecker Delta symbol and the Levi-Civita symbol, respectively. 
-        The _tensor.py_ module contains the code related with the class _tensor_ and many functions that are useful to define a tensor, operate tensors, recognise the contravariant and covariant indices, lower and raise indices and expand a tensor like a series up to a specific order. Inside this sub-package, there is another one named _core_ which contains essential information that the program needs to operate tensors. All the functions required by the user are located at the top level of the package. 
-        
-        ## Usage
-        
-        Pytearcat works using Jupyter Notebooks to give the outputs in mathematical form. To use the package the user should import Pytearcat within a Jypyter Notebook
-        
-        ```python
-        import pytearcat as pt
-        ```
-        
-        Later, it is possible to access the functions and methods of the package within the notebook. Different usage examples can be found in the top directory of the GitHub repository.
-        
-        ## How to cite this work
-        
-        To cite this work, please refer to Pytearcat's release paper [San Martin & Sureda (2021)](https://doi.org/10.1016/j.ascom.2022.100572) (also available on [arXiv](https://arxiv.org/abs/2106.15016)) and use the following Bibtex citation:
-        
-        
-        ```
-        @article{pytearcat2022,
-        	abstract = {This paper introduces the first release of Pytearcat, a Python package developed to compute tensor algebra operations in the context of theoretical physics, for instance, in general relativity. Given that working with tensors can become a complex task, people often rely on computational tools to perform tensor calculations. We aim to build a tensor calculator based on Python, which benefits from being free and easy to use. Pytearcat syntax resembles the usual physics notation for tensor calculus, such as the Einstein notation for index contraction. This version allows the user to perform many tensor operations, including derivatives and series expansions, along with routines to obtain the typical General Relativity tensors. A particular concern was put in the execution times, leading to incorporate an alternative core for the symbolic calculations, enabling to reach much faster execution times. The syntax and the versatility of Pytearcat are the most important features of this package, where the latter can be used to extend Pytearcat to other areas of theoretical physics.},
-        	author = {M. San Mart\'in and J. Sureda},
-        	doi = {https://doi.org/10.1016/j.ascom.2022.100572},
-        	issn = {2213-1337},
-        	journal = {Astronomy and Computing},
-        	keywords = {Software, Public release, General relativity, Tensor algebra, Computer algebra system},
-        	pages = {100572},
-        	title = {Pytearcat: PYthon TEnsor AlgebRa calCulATor A python package for general relativity and tensor calculus},
-        	url = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
-        	year = {2022},
-        	Bdsk-Url-1 = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
-        	Bdsk-Url-2 = {https://doi.org/10.1016/j.ascom.2022.100572}}
-        
-        ```
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 Provides-Extra: giacpy
+License-File: LICENSE
+
+# Pytearcat: PYthon TEnsor AlgebRa calCulATor - A python package for general relativity and tensor calculus
+
+Pytearcat is an open-source Python package created to work with general tensor operations, either in the field of General Relativity (GR) or others that need to use tensor calculus. It provides the basic GR tensors built in the package and uses a standard syntax for the Einstein notation. 
+
+## Installation
+
+As a Python package, Pytearcat can be installed through pip using
+
+```bash
+pip install pytearcat
+```
+To use the Giacpy core in Pytearcat, the user must explicitly indicate during the package installation that the installer must include the Giacpy module in the process. This is done through
+
+```bash
+pip install pytearcat[giapy]
+```
+
+## File structure summary
+Inside the Pytearcat package, there are two sub-packages named _gr_ and _tensor_. Inside the first one, there are six modules related to GR expressions. These libraries allow calculating quantities that are very common in GR, such as the Christoffel symbols (first and the second kind, _christoffel.py_), the Ricci tensor and the Ricci scalar (_ricci.py_), the Riemann tensor (_riemann.py_) and the Einstein tensor (_einstein.py_). Also, there is a module to define the metric (_metric.py_) and another to calculate the geodesics (_geodesic.py_).
+The second sub-package named _tensor_ contains modules that allow to define tensors and operate with them. The _misc.py_ module contains functions that allow defining symbolic functions, variables, and constants. It also contains other functions to work with series expansions and to simplify expressions. The _kdelta.py_ and _lcivita.py_ modules contain the data classes which define the Kronecker Delta symbol and the Levi-Civita symbol, respectively. 
+The _tensor.py_ module contains the code related with the class _tensor_ and many functions that are useful to define a tensor, operate tensors, recognise the contravariant and covariant indices, lower and raise indices and expand a tensor like a series up to a specific order. Inside this sub-package, there is another one named _core_ which contains essential information that the program needs to operate tensors. All the functions required by the user are located at the top level of the package. 
+
+## Usage
+
+Pytearcat works using Jupyter Notebooks to give the outputs in mathematical form. To use the package the user should import Pytearcat within a Jypyter Notebook
+
+```python
+import pytearcat as pt
+```
+
+Later, it is possible to access the functions and methods of the package within the notebook. Different usage examples can be found in the top directory of the GitHub repository.
+
+## How to cite this work
+
+To cite this work, please refer to Pytearcat's release paper [San Martin & Sureda (2021)](https://doi.org/10.1016/j.ascom.2022.100572) (also available on [arXiv](https://arxiv.org/abs/2106.15016)) and use the following Bibtex citation:
+
+
+```
+@article{pytearcat2022,
+	abstract = {This paper introduces the first release of Pytearcat, a Python package developed to compute tensor algebra operations in the context of theoretical physics, for instance, in general relativity. Given that working with tensors can become a complex task, people often rely on computational tools to perform tensor calculations. We aim to build a tensor calculator based on Python, which benefits from being free and easy to use. Pytearcat syntax resembles the usual physics notation for tensor calculus, such as the Einstein notation for index contraction. This version allows the user to perform many tensor operations, including derivatives and series expansions, along with routines to obtain the typical General Relativity tensors. A particular concern was put in the execution times, leading to incorporate an alternative core for the symbolic calculations, enabling to reach much faster execution times. The syntax and the versatility of Pytearcat are the most important features of this package, where the latter can be used to extend Pytearcat to other areas of theoretical physics.},
+	author = {M. San Mart\'in and J. Sureda},
+	doi = {https://doi.org/10.1016/j.ascom.2022.100572},
+	issn = {2213-1337},
+	journal = {Astronomy and Computing},
+	keywords = {Software, Public release, General relativity, Tensor algebra, Computer algebra system},
+	pages = {100572},
+	title = {Pytearcat: PYthon TEnsor AlgebRa calCulATor A python package for general relativity and tensor calculus},
+	url = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
+	year = {2022},
+	Bdsk-Url-1 = {https://www.sciencedirect.com/science/article/pii/S221313372200018X},
+	Bdsk-Url-2 = {https://doi.org/10.1016/j.ascom.2022.100572}}
+
+```
+
```

### Comparing `pytearcat-0.0.5/pytearcat.egg-info/SOURCES.txt` & `pytearcat-0.0.6/pytearcat.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+LICENSE
 README.md
-README.rst
 setup.py
 pytearcat/__init__.py
 pytearcat.egg-info/PKG-INFO
 pytearcat.egg-info/SOURCES.txt
 pytearcat.egg-info/dependency_links.txt
 pytearcat.egg-info/requires.txt
 pytearcat.egg-info/top_level.txt
```

### Comparing `pytearcat-0.0.5/setup.py` & `pytearcat-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
-requirements = ["jupyter>=1.0.0", "numpy==1.19.0", "sympy>=1.7.1", "tqdm>=4.55.0", "jedi==0.17.2"]
+requirements = ["jupyter>=1.0.0", "numpy>=1.22.0", "sympy>=1.7.1", "tqdm>=4.55.0", "jedi>=0.17.2"]
 
 ext_requirements = {"giacpy" : ["giacpy>=0.7.0"]}
 
 setup(
     name="pytearcat",
-    version="0.0.5",
+    version="0.0.6",
     author="Joaquin Sureda",
     author_email="jmsureda@uc.cl",
     description="A package to perform tensor algebra calculations.",
     long_description=readme,
     long_description_content_type="text/markdown",
     licence="LICENCE",
     url="https://github.com/pytearcat/pytearcat",
     packages=find_packages(),
     install_requires=requirements,
     extras_require=ext_requirements,
     classifiers=[
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

