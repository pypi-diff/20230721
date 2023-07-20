# Comparing `tmp/hist-2.7.0.tar.gz` & `tmp/hist-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Thu Jul 20 21:59:49 2023, max compression
```

## Comparing `hist-2.7.0.tar` & `hist-2.7.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 hist-2.7.0/.all-contributorsrc
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hist-2.7.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 hist-2.7.0/.gitattributes
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hist-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 hist-2.7.0/.readthedocs.yml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hist-2.7.0/CITATION.cff
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hist-2.7.0/dev-environment.yml
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 hist-2.7.0/noxfile.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 hist-2.7.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hist-2.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hist-2.7.0/.github/labeler.yml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/docs-improvements.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/support.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hist-2.7.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 hist-2.7.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hist-2.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hist-2.7.0/.github/workflows/pr.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hist-2.7.0/binder/postBuild
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 hist-2.7.0/docs/Makefile
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 hist-2.7.0/docs/banner_slides.md
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 hist-2.7.0/docs/changelog.md
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 hist-2.7.0/docs/conf.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hist-2.7.0/docs/contributing.md
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 hist-2.7.0/docs/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hist-2.7.0/docs/make.bat
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 hist-2.7.0/docs/support.rst
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_category.png
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_circular.png
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_integer.png
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_regular.png
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_variable.png
--rw-r--r--   0        0        0   278047 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/banner.gif
--rw-r--r--   0        0        0    21774 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/ex_hist_density.png
--rw-r--r--   0        0        0    62092 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/fullplot_example.png
--rw-r--r--   0        0        0    18389 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/histlogo.png
--rw-r--r--   0        0        0    94683 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/histlogo.svg
--rw-r--r--   0        0        0    17543 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/histogram_design.png
--rw-r--r--   0        0        0   301669 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/pieplot_example.png
--rw-r--r--   0        0        0   114661 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/ratioplot_example.png
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/stackplot_example.png
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/.gitignore
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/Makefile
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_category.tex
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_circular.tex
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_integer.tex
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_regular.tex
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_variable.tex
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 hist-2.7.0/docs/examples/HistDemo.ipynb
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.accumulators.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.axestuple.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.axis.rst
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.axis.transform.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.basehist.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.classichist.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.dask.hist.rst
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.dask.namedhist.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.dask.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.hist.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.intervals.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.namedhist.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.numpy.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.plot.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.quick_construct.rst
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.stack.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.storage.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.svgplots.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.svgutils.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.tag.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.version.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/modules.rst
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/accumulators.rst
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/analyses.rst
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/axes.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/cli.rst
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/indexing.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/installation.rst
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/numpy.rst
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/quickstart.rst
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/storages.rst
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/subclassing.rst
--rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Histogram.ipynb
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Interpolation.ipynb
--rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Plots.ipynb
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Reprs.ipynb
--rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/SVGHistogram.ipynb
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Stack.ipynb
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Transform.ipynb
--rw-r--r--   0        0        0    50203 2020-02-02 00:00:00.000000 hist-2.7.0/notebooks/HistLogo.ipynb
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hist-2.7.0/notebooks/axestuple-setattr.ipynb
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/accumulators.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axestuple.py
--rw-r--r--   0        0        0    22056 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/basehist.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/classichist.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/hist.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/interop.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/intervals.py
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/namedhist.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/numpy.py
--rw-r--r--   0        0        0    23008 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/py.typed
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/quick_construct.py
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/stack.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/storage.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/svgplots.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/svgutils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/tag.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/version.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/_compat/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/_compat/builtins.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/_compat/typing.py
--rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axis/py.typed
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axis/transform.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/dask/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/dask/hist.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/dask/namedhist.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 hist-2.7.0/tests/conftest.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_axestuple.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_axis.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_bh.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_dask.py
--rw-r--r--   0        0        0    28170 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_general.py
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_interop.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_intervals.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_mock_plot.py
--rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_named.py
--rw-r--r--   0        0        0    19787 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_plot.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_profile.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_reprs.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_stacks.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_version.py
--rw-r--r--   0        0        0    20789 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_image_plot_pull.png
--rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_image_plot_ratio_callable.png
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_image_plot_ratio_hist.png
--rw-r--r--   0        0        0    19403 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_plot1d_auto_handling.png
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 hist-2.7.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 hist-2.7.0/LICENSE
--rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 hist-2.7.0/README.md
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 hist-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    16961 2020-02-02 00:00:00.000000 hist-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3319 2023-07-20 21:59:49.000000 hist-2.7.1/.all-contributorsrc
+-rw-r--r--   0        0        0      125 2023-07-20 21:59:49.000000 hist-2.7.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-07-20 21:59:49.000000 hist-2.7.1/.gitattributes
+-rw-r--r--   0        0        0     1755 2023-07-20 21:59:49.000000 hist-2.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2023-07-20 21:59:49.000000 hist-2.7.1/.readthedocs.yml
+-rw-r--r--   0        0        0      789 2023-07-20 21:59:49.000000 hist-2.7.1/CITATION.cff
+-rw-r--r--   0        0        0      412 2023-07-20 21:59:49.000000 hist-2.7.1/dev-environment.yml
+-rw-r--r--   0        0        0     2530 2023-07-20 21:59:49.000000 hist-2.7.1/noxfile.py
+-rw-r--r--   0        0        0     2543 2023-07-20 21:59:49.000000 hist-2.7.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-07-20 21:59:49.000000 hist-2.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      169 2023-07-20 21:59:49.000000 hist-2.7.1/.github/labeler.yml
+-rw-r--r--   0        0        0      268 2023-07-20 21:59:49.000000 hist-2.7.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      343 2023-07-20 21:59:49.000000 hist-2.7.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      399 2023-07-20 21:59:49.000000 hist-2.7.1/.github/ISSUE_TEMPLATE/docs-improvements.md
+-rw-r--r--   0        0        0      537 2023-07-20 21:59:49.000000 hist-2.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      227 2023-07-20 21:59:49.000000 hist-2.7.1/.github/ISSUE_TEMPLATE/support.md
+-rw-r--r--   0        0        0      668 2023-07-20 21:59:49.000000 hist-2.7.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      684 2023-07-20 21:59:49.000000 hist-2.7.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1328 2023-07-20 21:59:49.000000 hist-2.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      229 2023-07-20 21:59:49.000000 hist-2.7.1/.github/workflows/pr.yml
+-rw-r--r--   0        0        0       76 2023-07-20 21:59:49.000000 hist-2.7.1/binder/postBuild
+-rw-r--r--   0        0        0      633 2023-07-20 21:59:49.000000 hist-2.7.1/docs/Makefile
+-rw-r--r--   0        0        0     2785 2023-07-20 21:59:49.000000 hist-2.7.1/docs/banner_slides.md
+-rw-r--r--   0        0        0     8422 2023-07-20 21:59:49.000000 hist-2.7.1/docs/changelog.md
+-rw-r--r--   0        0        0     2707 2023-07-20 21:59:49.000000 hist-2.7.1/docs/conf.py
+-rw-r--r--   0        0        0       44 2023-07-20 21:59:49.000000 hist-2.7.1/docs/contributing.md
+-rw-r--r--   0        0        0     4205 2023-07-20 21:59:49.000000 hist-2.7.1/docs/index.rst
+-rw-r--r--   0        0        0      794 2023-07-20 21:59:49.000000 hist-2.7.1/docs/make.bat
+-rw-r--r--   0        0        0      752 2023-07-20 21:59:49.000000 hist-2.7.1/docs/support.rst
+-rw-r--r--   0        0        0     3093 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/axis_category.png
+-rw-r--r--   0        0        0     5696 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/axis_circular.png
+-rw-r--r--   0        0        0     2349 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/axis_integer.png
+-rw-r--r--   0        0        0     2352 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/axis_regular.png
+-rw-r--r--   0        0        0     2599 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/axis_variable.png
+-rw-r--r--   0        0        0   278047 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/banner.gif
+-rw-r--r--   0        0        0    21774 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/ex_hist_density.png
+-rw-r--r--   0        0        0    62092 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/fullplot_example.png
+-rw-r--r--   0        0        0    18389 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/histlogo.png
+-rw-r--r--   0        0        0    94683 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/histlogo.svg
+-rw-r--r--   0        0        0    17543 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/histogram_design.png
+-rw-r--r--   0        0        0   301669 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/pieplot_example.png
+-rw-r--r--   0        0        0   114661 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/ratioplot_example.png
+-rw-r--r--   0        0        0    14396 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_images/stackplot_example.png
+-rw-r--r--   0        0        0       12 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/.gitignore
+-rw-r--r--   0        0        0      257 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/Makefile
+-rw-r--r--   0        0        0      979 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/axis_category.tex
+-rw-r--r--   0        0        0      983 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/axis_circular.tex
+-rw-r--r--   0        0        0      888 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/axis_integer.tex
+-rw-r--r--   0        0        0      912 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/axis_regular.tex
+-rw-r--r--   0        0        0      947 2023-07-20 21:59:49.000000 hist-2.7.1/docs/_src/images/axis_variable.tex
+-rw-r--r--   0        0        0     5913 2023-07-20 21:59:49.000000 hist-2.7.1/docs/examples/HistDemo.ipynb
+-rw-r--r--   0        0        0      139 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.accumulators.rst
+-rw-r--r--   0        0        0      130 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.axestuple.rst
+-rw-r--r--   0        0        0      194 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.axis.rst
+-rw-r--r--   0        0        0      145 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.axis.transform.rst
+-rw-r--r--   0        0        0      127 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.basehist.rst
+-rw-r--r--   0        0        0      136 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.classichist.rst
+-rw-r--r--   0        0        0      130 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.dask.hist.rst
+-rw-r--r--   0        0        0      145 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.dask.namedhist.rst
+-rw-r--r--   0        0        0      212 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.dask.rst
+-rw-r--r--   0        0        0      115 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.hist.rst
+-rw-r--r--   0        0        0      130 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.intervals.rst
+-rw-r--r--   0        0        0      130 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.namedhist.rst
+-rw-r--r--   0        0        0      118 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.numpy.rst
+-rw-r--r--   0        0        0      115 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.plot.rst
+-rw-r--r--   0        0        0      150 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.quick_construct.rst
+-rw-r--r--   0        0        0      506 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.rst
+-rw-r--r--   0        0        0      118 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.stack.rst
+-rw-r--r--   0        0        0      124 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.storage.rst
+-rw-r--r--   0        0        0      127 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.svgplots.rst
+-rw-r--r--   0        0        0      127 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.svgutils.rst
+-rw-r--r--   0        0        0      112 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.tag.rst
+-rw-r--r--   0        0        0      124 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/hist.version.rst
+-rw-r--r--   0        0        0       49 2023-07-20 21:59:49.000000 hist-2.7.1/docs/reference/modules.rst
+-rw-r--r--   0        0        0     5217 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/accumulators.rst
+-rw-r--r--   0        0        0     1318 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/analyses.rst
+-rw-r--r--   0        0        0     7451 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/axes.rst
+-rw-r--r--   0        0        0      134 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/cli.rst
+-rw-r--r--   0        0        0     1264 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/indexing.rst
+-rw-r--r--   0        0        0      603 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/installation.rst
+-rw-r--r--   0        0        0     3915 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/numpy.rst
+-rw-r--r--   0        0        0     5662 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/quickstart.rst
+-rw-r--r--   0        0        0     3586 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/storages.rst
+-rw-r--r--   0        0        0     2784 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/subclassing.rst
+-rw-r--r--   0        0        0    17498 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/Histogram.ipynb
+-rw-r--r--   0        0        0     3908 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/Interpolation.ipynb
+-rw-r--r--   0        0        0     8945 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/Plots.ipynb
+-rw-r--r--   0        0        0     1680 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/Reprs.ipynb
+-rw-r--r--   0        0        0    18737 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/SVGHistogram.ipynb
+-rw-r--r--   0        0        0     5882 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/Stack.ipynb
+-rw-r--r--   0        0        0     3853 2023-07-20 21:59:49.000000 hist-2.7.1/docs/user-guide/notebooks/Transform.ipynb
+-rw-r--r--   0        0        0    50203 2023-07-20 21:59:49.000000 hist-2.7.1/notebooks/HistLogo.ipynb
+-rw-r--r--   0        0        0     1717 2023-07-20 21:59:49.000000 hist-2.7.1/notebooks/axestuple-setattr.ipynb
+-rw-r--r--   0        0        0     1159 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/accumulators.py
+-rw-r--r--   0        0        0     2291 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/axestuple.py
+-rw-r--r--   0        0        0    22056 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/basehist.py
+-rw-r--r--   0        0        0     1431 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/classichist.py
+-rw-r--r--   0        0        0      126 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/hist.py
+-rw-r--r--   0        0        0     4130 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/interop.py
+-rw-r--r--   0        0        0     6893 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/intervals.py
+-rw-r--r--   0        0        0     5187 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/namedhist.py
+-rw-r--r--   0        0        0      161 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/numpy.py
+-rw-r--r--   0        0        0    23012 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/plot.py
+-rw-r--r--   0        0        0        0 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/py.typed
+-rw-r--r--   0        0        0    11131 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/quick_construct.py
+-rw-r--r--   0        0        0     5902 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/stack.py
+-rw-r--r--   0        0        0      323 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/storage.py
+-rw-r--r--   0        0        0     5426 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/svgplots.py
+-rw-r--r--   0        0        0     2282 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/svgutils.py
+-rw-r--r--   0        0        0      250 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/tag.py
+-rw-r--r--   0        0        0      160 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/version.py
+-rw-r--r--   0        0        0      118 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/version.pyi
+-rw-r--r--   0        0        0        0 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/_compat/__init__.py
+-rw-r--r--   0        0        0      759 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/_compat/builtins.py
+-rw-r--r--   0        0        0      619 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/_compat/typing.py
+-rw-r--r--   0        0        0     6018 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/axis/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/axis/py.typed
+-rw-r--r--   0        0        0      182 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/axis/transform.py
+-rw-r--r--   0        0        0      392 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/dask/__init__.py
+-rw-r--r--   0        0        0      290 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/dask/hist.py
+-rw-r--r--   0        0        0      325 2023-07-20 21:59:49.000000 hist-2.7.1/src/hist/dask/namedhist.py
+-rw-r--r--   0        0        0      742 2023-07-20 21:59:49.000000 hist-2.7.1/tests/conftest.py
+-rw-r--r--   0        0        0      691 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_axestuple.py
+-rw-r--r--   0        0        0     2078 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_axis.py
+-rw-r--r--   0        0        0      528 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_bh.py
+-rw-r--r--   0        0        0     4217 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_dask.py
+-rw-r--r--   0        0        0    28170 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_general.py
+-rw-r--r--   0        0        0    11430 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_interop.py
+-rw-r--r--   0        0        0     6204 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_intervals.py
+-rw-r--r--   0        0        0      979 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_mock_plot.py
+-rw-r--r--   0        0        0    25239 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_named.py
+-rw-r--r--   0        0        0    19787 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_plot.py
+-rw-r--r--   0        0        0     1040 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_profile.py
+-rw-r--r--   0        0        0     2714 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_reprs.py
+-rw-r--r--   0        0        0    12162 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_stacks.py
+-rw-r--r--   0        0        0      110 2023-07-20 21:59:49.000000 hist-2.7.1/tests/test_version.py
+-rw-r--r--   0        0        0    20789 2023-07-20 21:59:49.000000 hist-2.7.1/tests/baseline/test_image_plot_pull.png
+-rw-r--r--   0        0        0    19242 2023-07-20 21:59:49.000000 hist-2.7.1/tests/baseline/test_image_plot_ratio_callable.png
+-rw-r--r--   0        0        0    13830 2023-07-20 21:59:49.000000 hist-2.7.1/tests/baseline/test_image_plot_ratio_hist.png
+-rw-r--r--   0        0        0    19403 2023-07-20 21:59:49.000000 hist-2.7.1/tests/baseline/test_plot1d_auto_handling.png
+-rw-r--r--   0        0        0     2148 2023-07-20 21:59:49.000000 hist-2.7.1/.gitignore
+-rw-r--r--   0        0        0     1523 2023-07-20 21:59:49.000000 hist-2.7.1/LICENSE
+-rw-r--r--   0        0        0    12956 2023-07-20 21:59:49.000000 hist-2.7.1/README.md
+-rw-r--r--   0        0        0     5735 2023-07-20 21:59:49.000000 hist-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0    17050 2023-07-20 21:59:49.000000 hist-2.7.1/PKG-INFO
```

### Comparing `hist-2.7.0/.all-contributorsrc` & `hist-2.7.1/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/.pre-commit-config.yaml` & `hist-2.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/CITATION.cff` & `hist-2.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/noxfile.py` & `hist-2.7.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/.github/CONTRIBUTING.md` & `hist-2.7.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `hist-2.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/.github/matchers/pylint.json` & `hist-2.7.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/.github/workflows/cd.yml` & `hist-2.7.1/.github/workflows/cd.yml`

 * *Files 20% similar despite different names*

```diff
@@ -13,33 +13,27 @@
   dist:
     runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
-    - name: Build SDist & wheel
-      run: pipx run --spec build pyproject-build
-
-    - name: Check metadata
-      run: pipx run twine check dist/*
-
-    - uses: actions/upload-artifact@v3
-      with:
-        path: dist/*
+    - uses: hynek/build-and-inspect-python-package@v1
 
 
   publish:
     needs: [dist]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
+    environment:
+      name: pypi
+      url: https://pypi.org/p/hist
+    permissions:
+      id-token: write
 
     steps:
     - uses: actions/download-artifact@v3
       with:
-        name: artifact
+        name: Packages
         path: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.pypi_password }}
```

### Comparing `hist-2.7.0/.github/workflows/ci.yml` & `hist-2.7.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/Makefile` & `hist-2.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/banner_slides.md` & `hist-2.7.1/docs/banner_slides.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/changelog.md` & `hist-2.7.1/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/conf.py` & `hist-2.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/index.rst` & `hist-2.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/make.bat` & `hist-2.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/support.rst` & `hist-2.7.1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/axis_category.png` & `hist-2.7.1/docs/_images/axis_category.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/axis_circular.png` & `hist-2.7.1/docs/_images/axis_circular.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/axis_integer.png` & `hist-2.7.1/docs/_images/axis_integer.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/axis_regular.png` & `hist-2.7.1/docs/_images/axis_regular.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/axis_variable.png` & `hist-2.7.1/docs/_images/axis_variable.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/banner.gif` & `hist-2.7.1/docs/_images/banner.gif`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/ex_hist_density.png` & `hist-2.7.1/docs/_images/ex_hist_density.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/fullplot_example.png` & `hist-2.7.1/docs/_images/fullplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/histlogo.png` & `hist-2.7.1/docs/_images/histlogo.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/histlogo.svg` & `hist-2.7.1/docs/_images/histlogo.svg`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/histogram_design.png` & `hist-2.7.1/docs/_images/histogram_design.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/pieplot_example.png` & `hist-2.7.1/docs/_images/pieplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/ratioplot_example.png` & `hist-2.7.1/docs/_images/ratioplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_images/stackplot_example.png` & `hist-2.7.1/docs/_images/stackplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_src/images/axis_category.tex` & `hist-2.7.1/docs/_src/images/axis_category.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_src/images/axis_circular.tex` & `hist-2.7.1/docs/_src/images/axis_circular.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_src/images/axis_integer.tex` & `hist-2.7.1/docs/_src/images/axis_integer.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_src/images/axis_regular.tex` & `hist-2.7.1/docs/_src/images/axis_regular.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/_src/images/axis_variable.tex` & `hist-2.7.1/docs/_src/images/axis_variable.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/examples/HistDemo.ipynb` & `hist-2.7.1/docs/examples/HistDemo.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/accumulators.rst` & `hist-2.7.1/docs/user-guide/accumulators.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/analyses.rst` & `hist-2.7.1/docs/user-guide/analyses.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/axes.rst` & `hist-2.7.1/docs/user-guide/axes.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/indexing.rst` & `hist-2.7.1/docs/user-guide/indexing.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/installation.rst` & `hist-2.7.1/docs/user-guide/installation.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/numpy.rst` & `hist-2.7.1/docs/user-guide/numpy.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/quickstart.rst` & `hist-2.7.1/docs/user-guide/quickstart.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/storages.rst` & `hist-2.7.1/docs/user-guide/storages.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/subclassing.rst` & `hist-2.7.1/docs/user-guide/subclassing.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/Histogram.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/Histogram.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/Interpolation.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/Interpolation.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/Plots.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/Reprs.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/Reprs.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/SVGHistogram.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/SVGHistogram.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/Stack.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/Stack.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/docs/user-guide/notebooks/Transform.ipynb` & `hist-2.7.1/docs/user-guide/notebooks/Transform.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/notebooks/HistLogo.ipynb` & `hist-2.7.1/notebooks/HistLogo.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/notebooks/axestuple-setattr.ipynb` & `hist-2.7.1/notebooks/axestuple-setattr.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/__init__.py` & `hist-2.7.1/src/hist/__init__.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/axestuple.py` & `hist-2.7.1/src/hist/axestuple.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/basehist.py` & `hist-2.7.1/src/hist/basehist.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/classichist.py` & `hist-2.7.1/src/hist/classichist.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/interop.py` & `hist-2.7.1/src/hist/interop.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/intervals.py` & `hist-2.7.1/src/hist/intervals.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/namedhist.py` & `hist-2.7.1/src/hist/namedhist.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/plot.py` & `hist-2.7.1/src/hist/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "plot2d_full",
     "plot_pie",
     "plot_pull_array",
     "plot_ratio_array",
     "plot_stack",
 )
 
-_PLT_MISSING_MSG = "Hist plotting with fitting requires scipy and iminuit. Please install hist[plot] or manually install dependencies."
+_PLT_MISSING_MSG = "Hist plotting with fitting requires scipy and iminuit. Please install hist[plot,fit] or manually install dependencies."
 
 
 class FitResultArtists(NamedTuple):
     line: matplotlib.lines.Line2D
     errorbar: matplotlib.container.ErrorbarContainer
     band: matplotlib.collections.PolyCollection
```

### Comparing `hist-2.7.0/src/hist/quick_construct.py` & `hist-2.7.1/src/hist/quick_construct.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/stack.py` & `hist-2.7.1/src/hist/stack.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/svgplots.py` & `hist-2.7.1/src/hist/svgplots.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/svgutils.py` & `hist-2.7.1/src/hist/svgutils.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/_compat/builtins.py` & `hist-2.7.1/src/hist/_compat/builtins.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/_compat/typing.py` & `hist-2.7.1/src/hist/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/src/hist/axis/__init__.py` & `hist-2.7.1/src/hist/axis/__init__.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/conftest.py` & `hist-2.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_axestuple.py` & `hist-2.7.1/tests/test_axestuple.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_axis.py` & `hist-2.7.1/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_bh.py` & `hist-2.7.1/tests/test_bh.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_dask.py` & `hist-2.7.1/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_general.py` & `hist-2.7.1/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_interop.py` & `hist-2.7.1/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_intervals.py` & `hist-2.7.1/tests/test_intervals.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_mock_plot.py` & `hist-2.7.1/tests/test_mock_plot.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_named.py` & `hist-2.7.1/tests/test_named.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_plot.py` & `hist-2.7.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_profile.py` & `hist-2.7.1/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_reprs.py` & `hist-2.7.1/tests/test_reprs.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/test_stacks.py` & `hist-2.7.1/tests/test_stacks.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/baseline/test_image_plot_pull.png` & `hist-2.7.1/tests/baseline/test_image_plot_pull.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/baseline/test_image_plot_ratio_callable.png` & `hist-2.7.1/tests/baseline/test_image_plot_ratio_callable.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/baseline/test_image_plot_ratio_hist.png` & `hist-2.7.1/tests/baseline/test_image_plot_ratio_hist.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/tests/baseline/test_plot1d_auto_handling.png` & `hist-2.7.1/tests/baseline/test_plot1d_auto_handling.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/.gitignore` & `hist-2.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/LICENSE` & `hist-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hist-2.7.0/README.md` & `hist-2.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 ![Slideshow of features. See docs/banner_slides.md for text if the image is not readable.](https://github.com/scikit-hep/hist/raw/main/docs/_images/banner.gif)
 
 ## Installation
 
 You can install this library from [PyPI](https://pypi.org/project/hist/) with pip:
 
 ```bash
-python3 -m pip install "hist[plot]"
+python3 -m pip install "hist[plot,fit]"
 ```
 
-If you do not need the plotting features, you can skip the `[plot]` extra.
+If you do not need the plotting features, you can skip the `[plot]` and/or
+`[fit]` extras. `[fit]` is not currently supported in WebAssembly.
 
 ## Features
 
 Hist currently provides everything boost-histogram provides, and the following enhancements:
 
 - Hist augments axes with names:
   - `name=` is a unique label describing each axis.
```

### Comparing `hist-2.7.0/pyproject.toml` & `hist-2.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 mpl = [
     "matplotlib >=3.0",
     "mplhep >=0.2.16",
 ]
 plot = [
     "matplotlib >=3.0",
     "mplhep >=0.2.16",
+]
+fit = [
     "scipy >=1.4",
     "iminuit >=2",
 ]
 dask = [
     "dask[dataframe] >=2022; python_version>='3.8'",
     "dask_histogram >=2023.1; python_version>='3.8'"
 ]
```

### Comparing `hist-2.7.0/PKG-INFO` & `hist-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hist
-Version: 2.7.0
+Version: 2.7.1
 Summary: Hist classes and utilities
 Project-URL: Homepage, https://github.com/scikit-hep/hist
 Project-URL: Documentation, https://hist.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/scikit-hep/hist/issues
 Project-URL: Discussions, https://github.com/scikit-hep/hist/discussions
 Project-URL: Changelog, https://hist.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henry.schreiner@cern.ch>
@@ -64,22 +64,23 @@
 Requires-Dist: pytest>=6; extra == 'docs'
 Requires-Dist: scipy>=1.4; extra == 'docs'
 Requires-Dist: sphinx-book-theme>=0.0.38; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=3.0.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Requires-Dist: uncertainties>=3; extra == 'docs'
+Provides-Extra: fit
+Requires-Dist: iminuit>=2; extra == 'fit'
+Requires-Dist: scipy>=1.4; extra == 'fit'
 Provides-Extra: mpl
 Requires-Dist: matplotlib>=3.0; extra == 'mpl'
 Requires-Dist: mplhep>=0.2.16; extra == 'mpl'
 Provides-Extra: plot
-Requires-Dist: iminuit>=2; extra == 'plot'
 Requires-Dist: matplotlib>=3.0; extra == 'plot'
 Requires-Dist: mplhep>=0.2.16; extra == 'plot'
-Requires-Dist: scipy>=1.4; extra == 'plot'
 Provides-Extra: test
 Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'test'
 Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'test'
 Requires-Dist: pytest-mpl>=0.12; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -110,18 +111,19 @@
 ![Slideshow of features. See docs/banner_slides.md for text if the image is not readable.](https://github.com/scikit-hep/hist/raw/main/docs/_images/banner.gif)
 
 ## Installation
 
 You can install this library from [PyPI](https://pypi.org/project/hist/) with pip:
 
 ```bash
-python3 -m pip install "hist[plot]"
+python3 -m pip install "hist[plot,fit]"
 ```
 
-If you do not need the plotting features, you can skip the `[plot]` extra.
+If you do not need the plotting features, you can skip the `[plot]` and/or
+`[fit]` extras. `[fit]` is not currently supported in WebAssembly.
 
 ## Features
 
 Hist currently provides everything boost-histogram provides, and the following enhancements:
 
 - Hist augments axes with names:
   - `name=` is a unique label describing each axis.
```

