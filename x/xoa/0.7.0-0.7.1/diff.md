# Comparing `tmp/xoa-0.7.0.tar.gz` & `tmp/xoa-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-0.7.0.tar", last modified: Mon Jul 17 11:31:22 2023, max compression
+gzip compressed data, was "xoa-0.7.1.tar", last modified: Fri Jul 21 14:52:45 2023, max compression
```

## Comparing `xoa-0.7.0.tar` & `xoa-0.7.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.473256 xoa-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/workflows/python-package-conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-17 11:31:04.000000 xoa-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 11:31:04.000000 xoa-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-17 11:31:04.000000 xoa-0.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 11:31:04.000000 xoa-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 11:31:04.000000 xoa-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 11:31:22.473256 xoa-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-17 11:31:04.000000 xoa-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-17 11:31:04.000000 xoa-0.7.0/ROADMAP.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-07-17 11:31:04.000000 xoa-0.7.0/bin/xoa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/.nojekill
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_static/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     2678 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.457254 xoa-0.7.0/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/doc/_templates/autosummary/
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_templates/autosummary/class.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/accessors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/doc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/appendix.cf.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/appendix.options.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/appendix.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/doc/binder/
--rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/binder/apt.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/binder/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/binder/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/configure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/doc/ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/ext/gencfspecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4758 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/ext/genfortran.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2296 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/ext/genoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/howtostart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.cf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.cfgm.cfg2rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.cfgm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/env/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-17 11:31:04.000000 xoa-0.7.0/env/environment.rtd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 11:31:04.000000 xoa-0.7.0/env/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 11:31:04.000000 xoa-0.7.0/env/requirements-doc.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/plot_croco_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/plot_hycom_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/plot_mercator_argo.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 11:31:04.000000 xoa-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 11:31:04.000000 xoa-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 11:31:22.473256 xoa-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-17 11:31:04.000000 xoa-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.469255 xoa-0.7.0/xoa/
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.469255 xoa-0.7.0/xoa/_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    94162 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/argo-7900573.nc
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/argo.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.south-africa.meridional.nc
--rw-r--r--   0 runner    (1001) docker     (123)   194356 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.south-africa.surf.nc
--rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.south-africa.zonal.nc
--rw-r--r--   0 runner    (1001) docker     (123)    43153 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/gdp-6203641.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/gdp.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   177500 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.gdp.h.nc
--rw-r--r--   0 runner    (1001) docker     (123)   176804 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.gdp.u.nc
--rw-r--r--   0 runner    (1001) docker     (123)   176804 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.gdp.v.nc
--rw-r--r--   0 runner    (1001) docker     (123)    71836 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/ibi-argo-7900573.nc
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/mercator.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cf.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cf.ini
--rw-r--r--   0 runner    (1001) docker     (123)   121868 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    68086 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cfgm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/dyn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/krig.py
--rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/num.py
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/sigma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.473256 xoa-0.7.0/xoa/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35220 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_dyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_sigma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_thermdyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/thermdyn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.469255 xoa-0.7.0/xoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.849114 xoa-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.833114 xoa-0.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-21 14:52:27.000000 xoa-0.7.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 14:52:27.000000 xoa-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-21 14:52:27.000000 xoa-0.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.833114 xoa-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-21 14:52:27.000000 xoa-0.7.1/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 14:52:27.000000 xoa-0.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-21 14:52:27.000000 xoa-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-21 14:52:27.000000 xoa-0.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-07-21 14:52:27.000000 xoa-0.7.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 14:52:27.000000 xoa-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 14:52:27.000000 xoa-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-21 14:52:45.849114 xoa-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-21 14:52:27.000000 xoa-0.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-21 14:52:27.000000 xoa-0.7.1/ROADMAP.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.833114 xoa-0.7.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-07-21 14:52:27.000000 xoa-0.7.1/bin/xoa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/.nojekill
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/_static/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2678 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.829114 xoa-0.7.1/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/doc/_templates/autosummary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/_templates/autosummary/class.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/accessors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/appendix.cf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/appendix.options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/appendix.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/doc/binder/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/binder/apt.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/binder/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/binder/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/configure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/doc/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/ext/gencfspecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4758 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/ext/genfortran.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2296 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/ext/genoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/howtostart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/uses.cf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/uses.cfgm.cfg2rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/uses.cfgm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 14:52:27.000000 xoa-0.7.1/doc/uses.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 14:52:27.000000 xoa-0.7.1/env/environment.rtd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-21 14:52:27.000000 xoa-0.7.1/env/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 14:52:27.000000 xoa-0.7.1/env/requirements-doc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.837114 xoa-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-21 14:52:27.000000 xoa-0.7.1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-21 14:52:27.000000 xoa-0.7.1/examples/plot_croco_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-21 14:52:27.000000 xoa-0.7.1/examples/plot_hycom_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-21 14:52:27.000000 xoa-0.7.1/examples/plot_mercator_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 14:52:27.000000 xoa-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 14:52:27.000000 xoa-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-21 14:52:45.849114 xoa-0.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-21 14:52:27.000000 xoa-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.841114 xoa-0.7.1/xoa/
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.849114 xoa-0.7.1/xoa/_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    94162 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/argo-7900573.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/argo.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/croco.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/croco.south-africa.meridional.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   194356 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/croco.south-africa.surf.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/croco.south-africa.zonal.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    43153 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/gdp-6203641.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/gdp.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/hycom.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   177500 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/hycom.gdp.h.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   176804 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/hycom.gdp.u.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   176804 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/hycom.gdp.v.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    71836 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/ibi-argo-7900573.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/_samples/mercator.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/cf.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/cf.ini
+-rw-r--r--   0 runner    (1001) docker     (123)   121868 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68086 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/cfgm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23445 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/dyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/krig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23456 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/sigma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.849114 xoa-0.7.1/xoa/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35220 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_dyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_sigma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/tests/test_thermdyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-21 14:52:27.000000 xoa-0.7.1/xoa/thermdyn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:52:45.845114 xoa-0.7.1/xoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-21 14:52:45.000000 xoa-0.7.1/xoa.egg-info/top_level.txt
```

### Comparing `xoa-0.7.0/.github/dependabot.yml` & `xoa-0.7.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/.github/workflows/python-package-conda.yml` & `xoa-0.7.1/.github/workflows/python-package-conda.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Python Package using Conda
+name: CI
 
 on: [push]
 
 jobs:
   build-linux:
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `xoa-0.7.0/.github/workflows/python-publish.yml` & `xoa-0.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/.gitignore` & `xoa-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/CHANGES.rst` & `xoa-0.7.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,95 +1,87 @@
 What's new
 ##########
 
 
+0.7.1 (2023-07-21)
+==================
+
+New features
+------------
+- Add support for not creating multi-indexes in :func:`xoa.coords.geo_stack`.
+
+Bug fixes
+---------
+- Fix :func:`xoa.geo.get_distances` that was not able to handle multi-indexes from :func:`xoa.coords.geo_stack`.
+- Fix doc generation [:pull:`83`].
+- Fix :func:`xoa.sigma.get_cs` to keep it compatible with pure numpy arrays
+
+
+Documentation
+-------------
+- Add a link to the github repository.
+
+
 0.7.0 (2023-07-17)
 ==================
 
 New features
 ------------
 - Add issue and pull request templates.
 - Add the :func:`xoa.filter.smooth` function [:pull:`76`].
-- Improved the default `sig` and `std` parameter values for filter windows
-  that accept them [:pull:`76`].
-- Add the :func:`xoa.plot.plot_minimap` and :func:`xoa.plot.plot_double_minimap`
-  functions to display the
-  geographic situation of a set of coordinates [:pull:`73`].
+- Improved the default `sig` and `std` parameter values for filter windows that accept them [:pull:`76`].
+- Add the :func:`xoa.plot.plot_minimap` and :func:`xoa.plot.plot_double_minimap` functions to display the geographic situation of a set of coordinates [:pull:`73`].
 - Add support for the `min_extent` keyword to :func:`xoa.geo.get_extent` [:pull:`73`]
 - Add dask support to :mod:`xoa.sigma` sigma to depth converters [:pull:`72`].
 - Add the :mod:`xoa.num` module that contains low level numeric utilities.
-- Add the :func:`xoa.thermdyn.mixed_layer_depth` function to compute
-  the mixed layer depth with three different methods [:pull:`67`, :pull:`75`].
-- Add the :func:`xoa.thermdyn.is_temp`, :func:`xoa.thermdyn.is_sal`
-  and :func:`xoa.thermdyn.is_dens` functions
-  to infer if an array of temperature, salinity or density type,
-  and added the related :func:`xoa.thermdyn.get_temp`,
-  :func:`xoa.thermdyn.get_sal` and :func:`xoa.thermdyn.get_dens`
-  function to search in datasets[:pull:`67`, :pull:`79`].
-- Add `kernel_kwargs` keyword to :func:`xoa.filter.convolve` to better control
-  the kernel generation by :func:`xoa.filter.generate_kernel` [:pull:`64`].
-- Add inference of parameters for some window functions, like the gaussian
-  shape, in :func:`xoa.filter.get_window_func` [:pull:`64`].
-- Add :func:`xoa.regrid.isoslice` based on :func:`xoa.interp.isoslice` core function
-  [:pull:`63`].
+- Add the :func:`xoa.thermdyn.mixed_layer_depth` function to compute the mixed layer depth with three different methods [:pull:`67`, :pull:`75`].
+- Add the :func:`xoa.thermdyn.is_temp`, :func:`xoa.thermdyn.is_sal` and :func:`xoa.thermdyn.is_dens` functions to infer if an array of temperature, salinity or density type, and added the related :func:`xoa.thermdyn.get_temp`, :func:`xoa.thermdyn.get_sal` and :func:`xoa.thermdyn.get_dens` function to search in datasets[:pull:`67`, :pull:`79`].
+- Add `kernel_kwargs` keyword to :func:`xoa.filter.convolve` to better control the kernel generation by :func:`xoa.filter.generate_kernel` [:pull:`64`].
+- Add inference of parameters for some window functions, like the gaussian shape, in :func:`xoa.filter.get_window_func` [:pull:`64`].
+- Add :func:`xoa.regrid.isoslice` based on :func:`xoa.interp.isoslice` core function [:pull:`63`].
 
 Breaking changes
 ----------------
-- func:`~xoa.filter.get_window_func` accepts now only one positional argument
-  and all other arguments must be named.
+- :func:`~xoa.filter.get_window_func` now accepts only one positional argument and all other arguments must be named.
 
 Bug fixes
 ---------
 - Fix :func:`xoa.cfgm.is_boolstr` which now supports the new :mod:`configobj`.
 - Fix broadcasting :mod:`xoa.interp` 1d interpolation routines [:issue:`69`].
-- Fix :func:`xoa.sigma.get_sigma_terms` so that it works in case of multiple
-  levels coordinates [:pull:`60`].
+- Fix :func:`xoa.sigma.get_sigma_terms` so that it works in case of multiple levels coordinates [:pull:`60`].
 - Fix :func:`xoa.grid.to_rect` that now infers coordinates and can emit a warning or raise an error.
 
 Documentation
 -------------
-- Add an example of `xoa.plot.plot_double_minimap` to
-  :ref:`sphx_glr_examples_plot_mercator_argo.py`
-  and :ref:`sphx_glr_examples_plot_hycom_gdp.py` examples [:pull:`73`].
-- Add an example of `xoa.thermdyn.mixed_layer_depth` to
-  :ref:`sphx_glr_examples_plot_croco_section.py` example [:pull:`67`].
+- Add an example of `xoa.plot.plot_double_minimap` to :ref:`sphx_glr_examples_plot_mercator_argo.py` and :ref:`sphx_glr_examples_plot_hycom_gdp.py` examples [:pull:`73`].
+- Add an example of `xoa.thermdyn.mixed_layer_depth` to :ref:`sphx_glr_examples_plot_croco_section.py` example [:pull:`67`].
 
 
 0.6.1 (2022-02-24)
 ==================
 
 New features
 ------------
-- Add a warning to :func:`xoa.open_data_sample` that is emitted when the request edfile
-  is not an internal data sample [:pull:`47`].
-- Add the :func:`xoa.plot.add_shadow`, :func:`xoa.plot.add_glow` and
-  :func:`xoa.plot.add_lightshading` function to add path effects to plots [:pull:`44`].
+- Add a warning to :func:`xoa.open_data_sample` that is emitted when the requested file is not an internal data sample [:pull:`47`].
+- Add the :func:`xoa.plot.add_shadow`, :func:`xoa.plot.add_glow` and :func:`xoa.plot.add_lightshading` function to add path effects to plots [:pull:`44`].
 - Add the :func:`xoa.plot.plot_ts` function to make T-S diagrams [:pull:`43`].
-- Add the :func:`xoa.filter.demerliac` function to apply a Dermerliac filter
-  to time serie [:pull:`41`].
-- Add support for fine tuning masking in :func:`xoa.filter.convolve` through the `na_thres`
-  parameter [:pull:`41`].
-- Add the :func:`xoa.geo.cdist` and :func:`xoa.geo.pdist` functions to compute
-  haversine distances respectively between two dataset and with a dataset  [:pull:`40`].
-- Add the :func:`xoa.coords.geo_stack` function to stack longitudes and latitudes
-  into another dimension, in a dataset or data array  [:pull:`40`].
-- Add the :func:`xoa.filter.decimate` function to crudely undersample a geographic
-  dataset or data array with a radius of proximity [:pull:`40`].
-- Add the :func:`xoa.geo.get_distances` to compute the Haversine distances between
-  locations inside a single dataset or between txo datasets [:pull:`40`].
+- Add the :func:`xoa.filter.demerliac` function to apply a Dermerliac filter to time serie [:pull:`41`].
+- Add support for fine tuning masking in :func:`xoa.filter.convolve` through the `na_thres` parameter [:pull:`41`].
+- Add the :func:`xoa.geo.cdist` and :func:`xoa.geo.pdist` functions to compute haversine distances respectively between two dataset and with a dataset  [:pull:`40`].
+- Add the :func:`xoa.coords.geo_stack` function to stack longitudes and latitudes into another dimension, in a dataset or data array  [:pull:`40`].
+- Add the :func:`xoa.filter.decimate` function to crudely undersample a geographic dataset or data array with a radius of proximity [:pull:`40`].
+- Add the :func:`xoa.geo.get_distances` to compute the Haversine distances between locations inside a single dataset or between txo datasets [:pull:`40`].
 - Add the :func:`xoa.krig.empirical_variogram` function to estimate variogram parameters.
 - Add the :class:`xoa.krig.VariogramModel` to manage a variogram model [:pull:`40`].
 - Add the :class:`xoa.krig.Kriger` and :func:`xoa.krig.krig` to perform kriging [:pull:`40`].
-- Add the `exclude` option to data var and coordinate specifications of
-  :class:`xoa.cf.CFSpecs` instances [:pull:`38`].
+- Add the `exclude` option to data var and coordinate specifications of :class:`xoa.cf.CFSpecs` instances [:pull:`38`].
 
 Breaking changes
 ----------------
-- A single Nan now contaminates the data over the kernel emprise in :func:`xoa.filter.convolve`
-  since `na_thres` is set to zero by default  [:pull:`40`].
+- A single Nan now contaminates the data over the kernel emprise in :func:`xoa.filter.convolve` since `na_thres` is set to zero by default  [:pull:`40`].
 - xoa now requires the :mod:`gsw` package.
 
 Bug fixes
 ---------
 - Fix :func:`xoa.regrid.regrid1d` so that it works now with time coordinates [:pull:`48`].
 - Fix :func:`xoa.regrid.grid2loc` so that it works with scalar output coordinates.
 - Fix :func:`xoa.regrid.regrid1d` to prevent conflict in the presence of MultiIndexes.
@@ -119,129 +111,97 @@
 
 
 0.5.0 (2021-10-12)
 ==================
 
 New features
 ------------
-- Add the `hlocs` argument to :func:`xoa.sigma.get_sigma_terms`
-  and :func:`xoa.sigma.decode_cf_sigma` to decode at several horizontal
-  staggered grid locations  [:pull:`34`].
-- Add the `edges` argument to :func:`xoa.regrid.regrid1d` to manually specify
-  the edges that are used by the "cellave" regridding method  [:pull:`34`].
-- Add back the `loc` argument to the formatting methods of :mod:`xoa.cf`
-   [:pull:`34`].
-- Add dimension checking and support for dask arrays in :mod:`xoa.sigma`
-   [:pull:`34`].
-- Expose a few options of :meth:`xoa.cfgm.ConfigManager` to the
-  :func:`xoa.cfgm.cfgargparse` function.
-- Add the :confval:`cfgm_cfg_file` sphinx configuration option
-  to save the default configuration of a :meth:`xoa.cfgm.ConfigManager`.
+- Add the `hlocs` argument to :func:`xoa.sigma.get_sigma_terms` and :func:`xoa.sigma.decode_cf_sigma` to decode at several horizontal staggered grid locations  [:pull:`34`].
+- Add the `edges` argument to :func:`xoa.regrid.regrid1d` to manually specify the edges that are used by the "cellave" regridding method  [:pull:`34`].
+- Add back the `loc` argument to the formatting methods of :mod:`xoa.cf` [:pull:`34`].
+- Add dimension checking and support for dask arrays in :mod:`xoa.sigma` [:pull:`34`].
+- Expose a few options of :meth:`xoa.cfgm.ConfigManager` to the :func:`xoa.cfgm.cfgargparse` function.
+- Add the :confval:`cfgm_cfg_file` sphinx configuration option to save the default configuration of a :meth:`xoa.cfgm.ConfigManager`.
 
 Bug fixes
 ---------
 - Fix :func:`xoa.regrid.regrid1d` with "cellave" method  [:pull:`34`].
-- Fix :meth:`xoa.cf.CFSpecs.get_location_mapping` for coordinates that have
-  no axis attribute specifications  [:pull:`34`].
-- Fix :func:`xoa.grid.dz2depth` that was not working properly with 4D+ arrays
-  [:pull:`34`].
+- Fix :meth:`xoa.cf.CFSpecs.get_location_mapping` for coordinates that have no axis attribute specifications  [:pull:`34`].
+- Fix :func:`xoa.grid.dz2depth` that was not working properly with 4D+ arrays [:pull:`34`].
 
 
 Breaking changes
 ----------------
-- The `loc` argument of :func:`xoa.sigma.get_sigma_terms` is renamed `vloc`
-   [:pull:`34`].
+- The `loc` argument of :func:`xoa.sigma.get_sigma_terms` is renamed `vloc` [:pull:`34`].
 
 
 0.4.0 (2021-09-02)
 ==================
 
 New features
 ------------
 - :meth:`xoa.cf.CFSpecs.decode` better supports staggered grids.
-- :meth:`xoa.cf.CFSpecs.search_dim` supports generic names in addition
-  to dimension types as second argument.
-- Add the :meth:`xoa.cf.CFSpecs.match_dim` method to check if a given
-  dimension name is known.
-- Add the :meth:`~xoa.cf.CFSpecs.reloc` and :meth:`~xoa.cf.CFSpecs.to_loc` methods
-  to :class:`xoa.cf.CFSpecs` for quickly changing the staggered grid indicators
-  in names.
-- Add the :meth:`xoa.cf.SGLocator.add_loc` method to quickly change the location
-  markers in a data array.
+- :meth:`xoa.cf.CFSpecs.search_dim` supports generic names in addition to dimension types as second argument.
+- Add the :meth:`xoa.cf.CFSpecs.match_dim` method to check if a given dimension name is known.
+- Add the :meth:`~xoa.cf.CFSpecs.reloc` and :meth:`~xoa.cf.CFSpecs.to_loc` methods to :class:`xoa.cf.CFSpecs` for quickly changing the staggered grid indicators in names.
+- Add the :meth:`xoa.cf.SGLocator.add_loc` method to quickly change the location markers in a data array.
 
 Breaking changes
 ----------------
 - :func:`xoa.coords.get_dims` is renamed to :func:`xoa.coords.get_cf_dims`.
-- The `name` argument of :class:`xoa.cf.CFSpecs` methods is renamed to `cf_name`,
-  and the `dim_type(s)` argument is renamed to `cf_arg(s)`.
-- :meth:`xoa.cf.SGLocator.get_location` is renamed to
-  :meth:`~xoa.cf.SGLocator.get_loc_from_da` and the :meth:`~xoa.cf.SGLocator.get_loc` is added.
+- The `name` argument of :class:`xoa.cf.CFSpecs` methods is renamed to `cf_name`, and the `dim_type(s)` argument is renamed to `cf_arg(s)`.
+- :meth:`xoa.cf.SGLocator.get_location` is renamed to :meth:`~xoa.cf.SGLocator.get_loc_from_da` and the :meth:`~xoa.cf.SGLocator.get_loc` is added.
 
 Bug fixes
 ---------
 - Fix the output formatting of :func:`xoa.grid.dz2depth`.
 
 Documentation
 -------------
-- The :ref:`uses.cf` section and :ref:`sphx_glr_examples_plot_hycom_gdp.py` example
-  are adapted to reflect changes.
+- The :ref:`uses.cf` section and :ref:`sphx_glr_examples_plot_hycom_gdp.py` example are adapted to reflect changes.
 
 
 v0.3.1 (2021-05-21)
 ===================
 
 New features
 ------------
-
-- Add an `autolim` keyword to :func:`xoa.plot.plot_flow` to speedup
-  the processing with cartopy maps.
+- Add an `autolim` keyword to :func:`xoa.plot.plot_flow` to speedup the processing with cartopy maps.
 
 Breaking changes
 ----------------
-
-- Rename the `cf` and `sigma` keyword of :func:`xoa.register_accessors`
-  respectively to `xcf` and `decode_sigma` to match the default
-  name of accessors.
+- Rename the `cf` and `sigma` keyword of :func:`xoa.register_accessors` respectively to `xcf` and `decode_sigma` to match the default name of accessors.
 - Rename the `sigma` accessor to `decode_sigma`.
 
 Bug fixes
 ---------
-
 - Fix the access to the xoa executable on windows.
 - Fix the minimal version for xarray [:pull:`23`].
 
 Documentation
 -------------
-
 - Add a "How to start" section.
-- Accessors are now documented separately with `sphinx-autosummary-accessors`
-  [:pull:`20`].
+- Accessors are now documented separately with `sphinx-autosummary-accessors` [:pull:`20`].
 - The Hycom-GDP example now uses :func:`xoa.plot.plot_flow`.
 
 
 v0.3.0 (2021-05-12)
 ===================
 
 New features
 ------------
-
 - Add the :func:`xoa.plot.plot_flow` function [:pull:`9`].
-- Improve :func:`xoa.coords.get_depth` so that it can compute
-  depth from sigma coordinates or layer thinknesses [:pull:`8`].
+- Improve :func:`xoa.coords.get_depth` so that it can compute depth from sigma coordinates or layer thinknesses [:pull:`8`].
 - Add the :func:`xoa.dyn.flow2d` function [:pull:`7`].
 - Add the :func:`xoa.regrid.extrap1d` function.
-- Add the :func:`xoa.filter.erode_coast` function which is specialized version
-  of the :func:`xoa.filter.erode_mask` for horizontal data.
-- Add the :func:`xoa.coords.get_xdim`, :func:`~xoa.coords.get_ydim`,
-  :func:`~xoa.coords.get_zdim`, :func:`~xoa.coords.get_tdim` and
-  :func:`~xoa.coords.get_fdim` for quickly finding standard dimensions.
+- Add the :func:`xoa.filter.erode_coast` function which is specialized version of the :func:`xoa.filter.erode_mask` for horizontal data.
+- Add the :func:`xoa.coords.get_xdim`, :func:`~xoa.coords.get_ydim`, :func:`~xoa.coords.get_zdim`, :func:`~xoa.coords.get_tdim` and :func:`~xoa.coords.get_fdim` for quickly finding standard dimensions.
 
 Bug fixes
 ---------
-
 - Fix u and v CF config [:pull:`6`]
 
 
 0.2.0
 =====
 
 New features
```

### Comparing `xoa-0.7.0/LICENSE` & `xoa-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/PKG-INFO` & `xoa-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa
-Version: 0.7.0
+Version: 0.7.1
 Summary: xarray-based ocean analysis library
 Home-page: https://github.com/vacumm/xoa
 Author: Shom
 Author-email: stephane.raynaud@shom.fr
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,38 +22,41 @@
 License-File: LICENSE
 
 xoa - xarray-based ocean analysis library
 =========================================
 
 .. image:: https://github.com/shom-fr/xoa/actions/workflows/python-package-conda.yml/badge.svg
     :alt: Install, linting and tests
-.. image:: https://anaconda.org/conda-forge/xoa/badges/version.svg
+.. image:: https://img.shields.io/conda/vn/conda-forge/xoa.svg
     :alt: Available on conda-forge
     :target: https://conda.anaconda.org/conda-forge/xoa
+.. image:: https://img.shields.io/pypi/v/xoa.svg
+    :alt: Available on pypi
+    :target: ttps://pypi.python.org/pypi/xoa/
 .. image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :target: https://xoa.readthedocs.io/en/latest/
 .. image:: https://anaconda.org/conda-forge/xoa/badges/downloads.svg
     :alt: Number of downloads on anaconda.org/conda-forge
     :target: https://anaconda.org/conda-forge/xoa/
 .. image:: https://pepy.tech/badge/xoa
     :alt: Number of downloads on pypi
     :target: https://pypi.org/project/xoa
+.. image:: https://img.shields.io/badge/code%20style-black-black
+    :alt: Black code style
 .. image:: https://anaconda.org/conda-forge/xoa/badges/platforms.svg
     :alt: noarch
     :target: https://anaconda.org/conda-forge/xoa
 .. image:: https://anaconda.org/conda-forge/xoa/badges/license.svg
     :alt: Apache 2.0
     :target: https://anaconda.org/conda-forge/xoa
 
 xoa is intended to help reading and manipulating observed
 and simulated ocean data.
 It is heavily based on `xarray <http://xarray.pydata.org/en/stable/>`_.
-For those who know it, it is the successor of
-`vacumm <https://github.com/VACUMM/vacumm>`_.
 
 Installation
 ------------
 
 From conda::
 
    conda install -c conda-forge xoa
```

### Comparing `xoa-0.7.0/README.rst` & `xoa-0.7.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 xoa - xarray-based ocean analysis library
 =========================================
 
 .. image:: https://github.com/shom-fr/xoa/actions/workflows/python-package-conda.yml/badge.svg
     :alt: Install, linting and tests
-.. image:: https://anaconda.org/conda-forge/xoa/badges/version.svg
+.. image:: https://img.shields.io/conda/vn/conda-forge/xoa.svg
     :alt: Available on conda-forge
     :target: https://conda.anaconda.org/conda-forge/xoa
+.. image:: https://img.shields.io/pypi/v/xoa.svg
+    :alt: Available on pypi
+    :target: ttps://pypi.python.org/pypi/xoa/
 .. image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :target: https://xoa.readthedocs.io/en/latest/
 .. image:: https://anaconda.org/conda-forge/xoa/badges/downloads.svg
     :alt: Number of downloads on anaconda.org/conda-forge
     :target: https://anaconda.org/conda-forge/xoa/
 .. image:: https://pepy.tech/badge/xoa
     :alt: Number of downloads on pypi
     :target: https://pypi.org/project/xoa
+.. image:: https://img.shields.io/badge/code%20style-black-black
+    :alt: Black code style
 .. image:: https://anaconda.org/conda-forge/xoa/badges/platforms.svg
     :alt: noarch
     :target: https://anaconda.org/conda-forge/xoa
 .. image:: https://anaconda.org/conda-forge/xoa/badges/license.svg
     :alt: Apache 2.0
     :target: https://anaconda.org/conda-forge/xoa
 
 xoa is intended to help reading and manipulating observed
 and simulated ocean data.
 It is heavily based on `xarray <http://xarray.pydata.org/en/stable/>`_.
-For those who know it, it is the successor of
-`vacumm <https://github.com/VACUMM/vacumm>`_.
 
 Installation
 ------------
 
 From conda::
 
    conda install -c conda-forge xoa
```

### Comparing `xoa-0.7.0/ROADMAP.rst` & `xoa-0.7.1/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/Makefile` & `xoa-0.7.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/_static/custom.css` & `xoa-0.7.1/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/_templates/autosummary/class.rst` & `xoa-0.7.1/doc/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/_templates/autosummary/module.rst` & `xoa-0.7.1/doc/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/accessors.rst` & `xoa-0.7.1/doc/accessors.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/appendix.cf.rst` & `xoa-0.7.1/doc/appendix.cf.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/cli.rst` & `xoa-0.7.1/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/conf.py` & `xoa-0.7.1/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 import xoa.cf
 
 cfgm_get_cfgm_func = xoa.cf._get_cfgm_
 cfgm_rst_file = "cf.txt"
 
 # %% Extlinks
 extlinks = {
-    "issue": ("https://github.com/shom-fr/xoa/issues/%s", "GH"),
-    "pull": ("https://github.com/shom-fr/xoa/pulls/%s", "PR"),
+    "issue": ("https://github.com/shom-fr/xoa/issues/%s", "GH%s"),
+    "pull": ("https://github.com/shom-fr/xoa/pulls/%s", "PR%s"),
 }
 
 # %% Nbsphinx
 # nbsphinx_timeout = 120  # in seconds
 
 # %% Sphinx gallery
 warnings.simplefilter("ignore", MatplotlibDeprecationWarning)
@@ -137,19 +137,21 @@
         'binderhub_url': 'https://mybinder.org',
         'dependencies': ['./binder/environment.yml', './binder/apt.txt', './binder/setup.py'],
         'notebooks_dir': 'notebooks',
         'use_jupyter_lab': True,
     },
 }
 
+# %% IPython
+ipython_warning_is_error = False
+
 # %% User directives
 
 
 def setup(app):
-
     app.add_css_file('custom.css')
 
     app.add_object_type(
         'confopt',
         'confopt',
         objname='configuration option',
         indextemplate='pair: %s; configuration option',
```

### Comparing `xoa-0.7.0/doc/configure.rst` & `xoa-0.7.1/doc/configure.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/ext/gencfspecs.py` & `xoa-0.7.1/doc/ext/gencfspecs.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/ext/genfortran.py` & `xoa-0.7.1/doc/ext/genfortran.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/ext/genoptions.py` & `xoa-0.7.1/doc/ext/genoptions.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/howtostart.rst` & `xoa-0.7.1/doc/howtostart.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/install.rst` & `xoa-0.7.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/uses.cf.rst` & `xoa-0.7.1/doc/uses.cf.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/uses.cfgm.cfg2rst.txt` & `xoa-0.7.1/doc/uses.cfgm.cfg2rst.txt`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/doc/uses.cfgm.rst` & `xoa-0.7.1/doc/uses.cfgm.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 Config management with  :mod:`xoa.cfgm`
 #######################################
 
 
 Introduction
 ============
 
-The :mod:`xoa.cfgm` module facilitates and extends the functionality
-offered by the excellent
+The :mod:`xoa.cfgm` module simplifies and extends the functionality
+provided by the excellent
 `configobj <https://configobj.readthedocs.io/en/latest/index.html>`_
-configuration file reading and validation package.
-It makes the global usage slightly easier and adds support for
+configuration file reader and validator package.
+It makes global usage a little easier and adds support for
 plurals forms and for exporting the specifications
-to a commandline options and rst declarations.
+to commandline options and rst declarations.
 
 
 Loading and validating
 ======================
 
 
 Let's define the configuration specifications:
@@ -41,16 +41,16 @@
 
 .. ipython:: python
 
     from xoa import cfgm
     CFGM = cfgm.ConfigManager(cfgspecs_lines)
 
 .. note:: To configure a library, the `cfgspecs_lines` argument is typically the name
-    of a static file placed in the same directory as the module that will
-    initializes an instance of the `~xoa.cfg.ConfigManager` class.
+    of a static file placed in the same directory as the module, which will
+    initialize an instance of the :class:`~xoa.cfg.ConfigManager` class.
 
 And finally, load and validate the user configuration:
 
 .. ipython:: python
 
     cfg = CFGM.load(cfg_lines)
```

### Comparing `xoa-0.7.0/examples/plot_croco_section.py` & `xoa-0.7.1/examples/plot_croco_section.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/examples/plot_hycom_gdp.py` & `xoa-0.7.1/examples/plot_hycom_gdp.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """
 # %%
 # Initialisations
 # ---------------
 
 import numpy as np
+import pandas as pd
 import xarray as xr
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 import xoa
 from xoa.grid import dz2depth, shift
 from xoa.regrid import grid2loc, regrid1d
 import xoa.cf as xcf
@@ -104,16 +105,17 @@
 
 # %%
 # GDP drifter
 # ~~~~~~~~~~~
 #
 # The drifter comes as a `csv` file and we read it as :class:`pandas.DataFrame` instance.
 
-drifter = xoa.open_data_sample(
-    "gdp-6203641.csv", header=0, skiprows=[1], parse_dates=[2], index_col=2
+csv_name = xoa.get_data_sample("gdp-6203641.csv")
+drifter = pd.read_csv(
+    csv_name, header=0, skiprows=[1], parse_dates=[0], index_col=0, usecols=[2, 3, 4, 5, 6, 7]
 )
 
 # %%
 # Since the sampling is not that nice, we resample it to 3-hour intervals.
 
 drifter = drifter.resample("3H").mean()
 
@@ -200,14 +202,14 @@
     color="C1",
     label="Drifter",
     width=2,
     **kwqv,
 )
 plt.quiverkey(qv, 0.1, 1.06, 0.1, r"0.1 $m\,s^{-1}$", color="k", alpha=1, labelpos="E")
 plt.legend()
-plot_double_minimap(drifter);
+plot_double_minimap(drifter)
 
 # %%
 # The discrepancies between the lagrangian and mean eulerian currents highlight
 # the variability due to the mesocale activity.
 # The differences between the observed and modeled currents are partly due to
 # the lack of data assimilation in the model.
```

### Comparing `xoa-0.7.0/examples/plot_mercator_argo.py` & `xoa-0.7.1/examples/plot_mercator_argo.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/setup.cfg` & `xoa-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/setup.py` & `xoa-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/__init__.py` & `xoa-0.7.1/xoa/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/argo-7900573.nc` & `xoa-0.7.1/xoa/_samples/argo-7900573.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/croco.cfg` & `xoa-0.7.1/xoa/_samples/croco.cfg`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/croco.south-africa.meridional.nc` & `xoa-0.7.1/xoa/_samples/croco.south-africa.meridional.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/croco.south-africa.surf.nc` & `xoa-0.7.1/xoa/_samples/croco.south-africa.surf.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/croco.south-africa.zonal.nc` & `xoa-0.7.1/xoa/_samples/croco.south-africa.zonal.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/gdp-6203641.csv` & `xoa-0.7.1/xoa/_samples/gdp-6203641.csv`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/hycom.gdp.h.nc` & `xoa-0.7.1/xoa/_samples/hycom.gdp.h.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/hycom.gdp.u.nc` & `xoa-0.7.1/xoa/_samples/hycom.gdp.u.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/hycom.gdp.v.nc` & `xoa-0.7.1/xoa/_samples/hycom.gdp.v.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/_samples/ibi-argo-7900573.nc` & `xoa-0.7.1/xoa/_samples/ibi-argo-7900573.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/accessors.py` & `xoa-0.7.1/xoa/accessors.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/cf.cfg` & `xoa-0.7.1/xoa/cf.cfg`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/cf.ini` & `xoa-0.7.1/xoa/cf.ini`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/cf.py` & `xoa-0.7.1/xoa/cf.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/cfgm.py` & `xoa-0.7.1/xoa/cfgm.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/cli.py` & `xoa-0.7.1/xoa/cli.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/color.py` & `xoa-0.7.1/xoa/color.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/coords.py` & `xoa-0.7.1/xoa/coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,15 +897,17 @@
         coord = coord.name
     out = [da for da in ds if coord in da.coords]
     if as_names:
         out = [da.name for da in out]
     return out
 
 
-def geo_stack(obj, stack_dim="npts", rename=False, drop=False, reset_index=False):
+def geo_stack(
+    obj, stack_dim="npts", rename=False, drop=False, reset_index=False, create_index=False
+):
     """Stack the dimensions of longitude and latitude coordinates
 
     .. note:: If already stacked or similar, a simple copy is returned,
         except if `rename` is True.
 
     Parameters
     ----------
@@ -914,14 +916,18 @@
     stack_dim: str
         Name of the new stack dimension
     rename: False
         Rename longitude to `lon` and latitude to `lat` for convenience.
         If no need to stack, rename the single dimension to `stack_dim`.
     drop: bool
         Drop all variables and coordinates that does not contain final stack dimension
+    reset_index: bool
+        Remove MultiIndexes that contains lon and lat dimensions before any operations
+    create_index: bool
+        Create a MultiIndex when calling :meth:`~xarray.DataArray.stack`
 
     Return
     ------
     xarray.DataArray, xarray.Dataset
         Array or dataset with lon and lat stacked.
         Its "geo_stack" :attr:`~xarray.DataArray.encoding` attribute value is set
         to `(stack_dim, lon_dim, lat_dim)`.
@@ -959,15 +965,15 @@
     elif lon.ndim == 1 and lat.ndim == 1 and lon.dims == lat.dims:
         if rename:
             obj = obj.rename({dims[0]: stack_dim})
         else:
             stack_dim = dims[0]
             obj = obj.copy()
     else:
-        obj = obj.stack({stack_dim: dims})
+        obj = obj.stack({stack_dim: dims}, create_index=create_index)
 
     # No multiindex?
     if not singleton and reset_index and lon.name not in obj.coords:
         obj = obj.reset_index(stack_dim)
 
     # Drop variables with no stacked coordinates
     if drop and hasattr(obj, "data_vars"):
```

### Comparing `xoa-0.7.0/xoa/dyn.py` & `xoa-0.7.1/xoa/dyn.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/filter.py` & `xoa-0.7.1/xoa/filter.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/geo.py` & `xoa-0.7.1/xoa/geo.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/grid.py` & `xoa-0.7.1/xoa/grid.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/interp.py` & `xoa-0.7.1/xoa/interp.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/krig.py` & `xoa-0.7.1/xoa/krig.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/misc.py` & `xoa-0.7.1/xoa/misc.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/num.py` & `xoa-0.7.1/xoa/num.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/plot.py` & `xoa-0.7.1/xoa/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         `axes`, `linecollection`, `step`, `duration`.
         `linecollection` refere to the :class:`matplotlib.collections.LineCollection` instance.
         The duration and step are also stored in the output.
 
     Example
     ------
     .. ipython:: python
+        :okwarning:
 
         @suppress
         import numpy as np, xarray as xr
         @suppress
         from xoa.plot import plot_flow
         # Setup data
         x = np.linspace(0, 2*np.pi, 20)
@@ -442,14 +443,15 @@
     ------
     cartopy.mpl.geoaxes.GeoAxes
         An instance of cartopy geographic axes
 
     Example
     -------
     .. ipython:: python
+        :okwarning:
 
         @suppress
         import xarray as xr, numpy as np, matplotlib.pyplot as plt
         @suppress
         from xoa.plot import plot_minimap
         ds = xr.Dataset(coords={{"lon": ("station", [-7, -5, -5]), "lat": ("station", [44, 44, 46])}})
         plt.plot([0, 2], [0, 2])
```

### Comparing `xoa-0.7.0/xoa/regrid.py` & `xoa-0.7.1/xoa/regrid.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/sigma.py` & `xoa-0.7.1/xoa/sigma.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,16 @@
     -------
     xarray.DataArray
         Stretching curve (:math:`C` | ``C``)
     """
     s, a, b = sig, thetas, thetab
     cs = np.sinh(s * a) * (1 - b) / np.sinh(a)
     cs = cs + b * (np.tanh(a * (s + 0.5)) / (2 * np.tanh(0.5 * a)) - 0.5)
-    cs.name = None
     if hasattr(cs, "coords"):
+        cs.name = None
         cs = cf.get_cf_specs(sig).format_data_var(cs, "cs", format_coords=False, rename_dims=False)
     return cs
 
 
 def ocean_s_coordinate(
     sig,
     ssh,
@@ -624,15 +624,14 @@
     vsingle = vloc not in ("any", None)
     hsingle = not isinstance(hlocs, list)
     if hsingle:
         hlocs = [hlocs]
     sigs = cfspecs.search(ds, 'sig', loc=vloc, single=False)
     terms = {}
     for sig in sigs:
-
         # Check standard_name and get loc
         if "standard_name" not in sig.attrs:
             raise XoaSigmaError(
                 "No standard_name attribute found in sigma/s " "variable name: " + sig.name
             )
         standard_name, loc = cfspecs.sglocator.parse_attr("standard_name", sig.standard_name)
         # skip this one
@@ -644,19 +643,17 @@
                 f"Sigma/s type variable {sig.name} " "has no formula_term attribute"
             )
         formula_terms = decode_formula_terms(sig.formula_terms)
 
         # Loop in horizontal locations
         subterms = terms[loc] = {}
         for hloc in hlocs:
-
             # Check terms
             subsubterms = subterms[hloc] = {sig.name: "sig", "type": standard_name}
             for fname, fvname in formula_terms.items():
-
                 # xoa.cf name
                 # TODO: handle mising cs and fallback with thetas and thetab
                 if fname.lower() not in FORMULA_TERMS_TO_CF_NAMES:
                     raise XoaSigmaError("Unknown formula term name: " + fname)
                 cf_name = FORMULA_TERMS_TO_CF_NAMES[fname.lower()]
 
                 # Real name
@@ -738,17 +735,15 @@
     from . import sigma as sigma_module
 
     sigma_type = None
     hsingle = not isinstance(hlocs, (list, tuple))
     if hsingle:
         hlocs = [hlocs]
     for vloc, vterms in all_terms.items():
-
         for hloc in hlocs:
-
             terms = vterms if hsingle else vterms[hloc]
             hloc = cfspecs.sglocator.parse_loc_arg(hloc)
             sigma_type = terms.pop("type")
 
             # Args: keys are cf names, values are dataarrays
             kwargs = {}
             for vname, cf_name in terms.items():
```

### Comparing `xoa-0.7.0/xoa/tests/test_cf.py` & `xoa-0.7.1/xoa/tests/test_cf.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_coords.py` & `xoa-0.7.1/xoa/tests/test_coords.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_dyn.py` & `xoa-0.7.1/xoa/tests/test_dyn.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_filter.py` & `xoa-0.7.1/xoa/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_geo.py` & `xoa-0.7.1/xoa/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_grid.py` & `xoa-0.7.1/xoa/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_interp.py` & `xoa-0.7.1/xoa/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_misc.py` & `xoa-0.7.1/xoa/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_regrid.py` & `xoa-0.7.1/xoa/tests/test_regrid.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_sigma.py` & `xoa-0.7.1/xoa/tests/test_sigma.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/tests/test_thermdyn.py` & `xoa-0.7.1/xoa/tests/test_thermdyn.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa/thermdyn.py` & `xoa-0.7.1/xoa/thermdyn.py`

 * *Files identical despite different names*

### Comparing `xoa-0.7.0/xoa.egg-info/PKG-INFO` & `xoa-0.7.1/xoa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa
-Version: 0.7.0
+Version: 0.7.1
 Summary: xarray-based ocean analysis library
 Home-page: https://github.com/vacumm/xoa
 Author: Shom
 Author-email: stephane.raynaud@shom.fr
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,38 +22,41 @@
 License-File: LICENSE
 
 xoa - xarray-based ocean analysis library
 =========================================
 
 .. image:: https://github.com/shom-fr/xoa/actions/workflows/python-package-conda.yml/badge.svg
     :alt: Install, linting and tests
-.. image:: https://anaconda.org/conda-forge/xoa/badges/version.svg
+.. image:: https://img.shields.io/conda/vn/conda-forge/xoa.svg
     :alt: Available on conda-forge
     :target: https://conda.anaconda.org/conda-forge/xoa
+.. image:: https://img.shields.io/pypi/v/xoa.svg
+    :alt: Available on pypi
+    :target: ttps://pypi.python.org/pypi/xoa/
 .. image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :target: https://xoa.readthedocs.io/en/latest/
 .. image:: https://anaconda.org/conda-forge/xoa/badges/downloads.svg
     :alt: Number of downloads on anaconda.org/conda-forge
     :target: https://anaconda.org/conda-forge/xoa/
 .. image:: https://pepy.tech/badge/xoa
     :alt: Number of downloads on pypi
     :target: https://pypi.org/project/xoa
+.. image:: https://img.shields.io/badge/code%20style-black-black
+    :alt: Black code style
 .. image:: https://anaconda.org/conda-forge/xoa/badges/platforms.svg
     :alt: noarch
     :target: https://anaconda.org/conda-forge/xoa
 .. image:: https://anaconda.org/conda-forge/xoa/badges/license.svg
     :alt: Apache 2.0
     :target: https://anaconda.org/conda-forge/xoa
 
 xoa is intended to help reading and manipulating observed
 and simulated ocean data.
 It is heavily based on `xarray <http://xarray.pydata.org/en/stable/>`_.
-For those who know it, it is the successor of
-`vacumm <https://github.com/VACUMM/vacumm>`_.
 
 Installation
 ------------
 
 From conda::
 
    conda install -c conda-forge xoa
```

### Comparing `xoa-0.7.0/xoa.egg-info/SOURCES.txt` & `xoa-0.7.1/xoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

