# Comparing `tmp/PyMPDATA-1.0.8.tar.gz` & `tmp/PyMPDATA-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMPDATA-1.0.8.tar", last modified: Sun Feb 12 14:44:54 2023, max compression
+gzip compressed data, was "PyMPDATA-1.0.9.tar", last modified: Thu Feb 23 18:21:33 2023, max compression
```

## Comparing `PyMPDATA-1.0.8.tar` & `PyMPDATA-1.0.9.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.214824 PyMPDATA-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.202823 PyMPDATA-1.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.202823 PyMPDATA-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/workflows/joss.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/workflows/readme_julia.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/workflows/readme_matlab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/workflows/readme_python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.github/workflows/stale_issues.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31252 2023-02-12 14:44:54.214824 PyMPDATA-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.202823 PyMPDATA-1.0.8/PyMPDATA/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.206824 PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/extrapolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/polar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.206824 PyMPDATA-1.0.8/PyMPDATA/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/domain_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/formulae_antidiff.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/formulae_axpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/formulae_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/formulae_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/formulae_nonoscillatory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/formulae_upwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/indexers.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/traversals.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/traversals_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/traversals_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/impl/traversals_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/scalar_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/PyMPDATA/vector_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.206824 PyMPDATA-1.0.8/PyMPDATA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31252 2023-02-12 14:44:54.000000 PyMPDATA-1.0.8/PyMPDATA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-12 14:44:54.000000 PyMPDATA-1.0.8/PyMPDATA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 14:44:54.000000 PyMPDATA-1.0.8/PyMPDATA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-12 14:44:54.000000 PyMPDATA-1.0.8/PyMPDATA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-12 14:44:54.000000 PyMPDATA-1.0.8/PyMPDATA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/paper/
--rw-r--r--   0 runner    (1001) docker     (123)    36415 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/paper/fig-crop.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    35759 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/paper/fig-perf.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 14:44:54.214824 PyMPDATA-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/test-time-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/devops_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/devops_tests/test_todos_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/arabas_and_farhat_2020/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/arabas_and_farhat_2020/test_black_scholes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/jarecka_et_al_2015/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/jarecka_et_al_2015/test_just_do_it.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/jaruga_et_al_2015/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/jaruga_et_al_2015/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/jaruga_et_al_2015/test_libmpdata_refdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/kinematic_2d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/kinematic_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/kinematic_2d/test_single_timestep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/convergence_refdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/test_moment_of_r_integral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/test_wall_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/smolarkiewicz_1983/
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/smolarkiewicz_1983/test_against_libmpdata_refdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/smolarkiewicz_2006/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/smolarkiewicz_2006/test_run_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.210824 PyMPDATA-1.0.8/tests/smoke_tests/timing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/timing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/timing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/timing/test_timing_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/timing/test_timing_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/smoke_tests/timing/test_timing_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.214824 PyMPDATA-1.0.8/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:54.214824 PyMPDATA-1.0.8/tests/unit_tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/fixtures/n_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_boundary_condition_extrapolated_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_boundary_condition_periodic_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_boundary_condition_polar_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_diffusion_only_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_domain_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_dpdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_formulae_upwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_mpdata_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_scalar_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_shared_advector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_traversals.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_upwind_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-02-12 14:44:39.000000 PyMPDATA-1.0.8/tests/unit_tests/test_upwind_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.964912 PyMPDATA-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.940912 PyMPDATA-1.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.944912 PyMPDATA-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/workflows/joss.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/workflows/readme_julia.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/workflows/readme_matlab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/workflows/readme_python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.github/workflows/stale_issues.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30258 2023-02-23 18:21:33.964912 PyMPDATA-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.944912 PyMPDATA-1.0.9/PyMPDATA/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.948912 PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/extrapolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/polar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/PyMPDATA/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/domain_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/formulae_antidiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/formulae_axpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/formulae_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/formulae_laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/formulae_nonoscillatory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/formulae_upwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/indexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/traversals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/traversals_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/traversals_halos_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/traversals_halos_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/traversals_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/impl/traversals_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/scalar_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/PyMPDATA/vector_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.948912 PyMPDATA-1.0.9/PyMPDATA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30258 2023-02-23 18:21:33.000000 PyMPDATA-1.0.9/PyMPDATA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-02-23 18:21:33.000000 PyMPDATA-1.0.9/PyMPDATA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 18:21:33.000000 PyMPDATA-1.0.9/PyMPDATA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 18:21:33.000000 PyMPDATA-1.0.9/PyMPDATA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 18:21:33.000000 PyMPDATA-1.0.9/PyMPDATA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29075 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    36415 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/paper/fig-crop.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    35759 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/paper/fig-perf.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 18:21:33.964912 PyMPDATA-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/test-time-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/tests/devops_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/devops_tests/test_todos_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/tests/smoke_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/tests/smoke_tests/arabas_and_farhat_2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/arabas_and_farhat_2020/test_black_scholes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.956912 PyMPDATA-1.0.9/tests/smoke_tests/jarecka_et_al_2015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/jarecka_et_al_2015/test_just_do_it.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.960912 PyMPDATA-1.0.9/tests/smoke_tests/jaruga_et_al_2015/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/jaruga_et_al_2015/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/jaruga_et_al_2015/test_libmpdata_refdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.960912 PyMPDATA-1.0.9/tests/smoke_tests/kinematic_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/kinematic_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/kinematic_2d/test_single_timestep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.960912 PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/convergence_refdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/test_moment_of_r_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/test_wall_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.960912 PyMPDATA-1.0.9/tests/smoke_tests/smolarkiewicz_1983/
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/smolarkiewicz_1983/test_against_libmpdata_refdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.960912 PyMPDATA-1.0.9/tests/smoke_tests/smolarkiewicz_2006/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/smolarkiewicz_2006/test_run_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.960912 PyMPDATA-1.0.9/tests/smoke_tests/timing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/timing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/timing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/timing/test_timing_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/timing/test_timing_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/smoke_tests/timing/test_timing_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.964912 PyMPDATA-1.0.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:33.964912 PyMPDATA-1.0.9/tests/unit_tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/fixtures/n_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_boundary_condition_extrapolated_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_boundary_condition_periodic_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_boundary_condition_polar_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_diffusion_only_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_domain_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_dpdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_formulae_upwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_mpdata_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_scalar_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_shared_advector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_traversals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_upwind_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-02-23 18:21:17.000000 PyMPDATA-1.0.9/tests/unit_tests/test_upwind_2d.py
```

### Comparing `PyMPDATA-1.0.8/.github/workflows/joss.yml` & `PyMPDATA-1.0.9/.github/workflows/joss.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.github/workflows/main.yml` & `PyMPDATA-1.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.github/workflows/readme_julia.yml` & `PyMPDATA-1.0.9/.github/workflows/readme_julia.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.github/workflows/readme_matlab.yml` & `PyMPDATA-1.0.9/.github/workflows/readme_matlab.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.github/workflows/readme_python.yml` & `PyMPDATA-1.0.9/.github/workflows/readme_python.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.github/workflows/stale_issues.yml` & `PyMPDATA-1.0.9/.github/workflows/stale_issues.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.gitignore` & `PyMPDATA-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/.zenodo.json` & `PyMPDATA-1.0.9/.zenodo.json`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/LICENSE` & `PyMPDATA-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PKG-INFO` & `PyMPDATA-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMPDATA
-Version: 1.0.8
+Version: 1.0.9
 Summary: Numba-accelerated Pythonic implementation of MPDATA with examples in Python, Julia and Matlab
 Author: https://github.com/open-atmos/PyMPDATA/graphs/contributors
 Author-email: sylwester.arabas@uj.edu.pl
 License: GPL-3.0
 Project-URL: Tracker, https://github.com/open-atmos/PyMPDATA/issues
 Project-URL: Documentation, https://open-atmos.github.io/PyMPDATA
 Project-URL: Source, https://github.com/open-atmos/PyMPDATA
@@ -27,30 +27,25 @@
 [![Python 3](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3)](https://www.python.org/)
 [![LLVM](https://img.shields.io/static/v1?label=LLVM&logo=LLVM&color=gold&message=Numba)](https://www.numba.org)
 [![Linux OK](https://img.shields.io/static/v1?label=Linux&logo=Linux&color=yellow&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Linux)
 [![macOS OK](https://img.shields.io/static/v1?label=macOS&logo=Apple&color=silver&message=%E2%9C%93)](https://en.wikipedia.org/wiki/macOS)
 [![Windows OK](https://img.shields.io/static/v1?label=Windows&logo=Windows&color=white&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Windows)
 [![Jupyter](https://img.shields.io/static/v1?label=Jupyter&logo=Jupyter&color=f37626&message=%E2%9C%93)](https://jupyter.org/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/open-atmos/PyMPDATA/graphs/commit-activity)
-[![OpenHub](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA/widgets/project_thin_badge?format=gif)](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA)
+[![OpenHub](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA/widgets/project_thin_badge?format=gif)](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA)   
 [![status](https://joss.theoj.org/papers/10e7361e43785dbb1b3d659c5b01757a/status.svg)](https://joss.theoj.org/papers/10e7361e43785dbb1b3d659c5b01757a)
 [![DOI](https://zenodo.org/badge/225610671.svg)](https://zenodo.org/badge/latestdoi/225610671)     
 [![EU Funding](https://img.shields.io/static/v1?label=EU%20Funding%20by&color=103069&message=FNP&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAC4AAAAeCAYAAABTwyyaAAAEzklEQVRYw9WYS2yUVRiGn3P5ZzozpZ3aUsrNgoKlKBINmkhpCCwwxIAhsDCpBBIWhmCMMYTEhSJ4i9EgBnSBEm81MRrFBhNXEuUSMCopiRWLQqEGLNgr085M5//POS46NNYFzHQ6qGc1i5nzP/P973m/9ztCrf7A8T9csiibCocUbvTzfxLcAcaM3cY3imXz25lT3Y34G7gQYAKV3+bFAHcATlBTPogJNADG92iY28FHW97kyPbnuW/W7xgzAhukQ9xe04PJeOT0HkQRwK0TlEeGWb/kOO9v3kdD3a8YK9GhDMfa6mg9fxunOm/lWPtcpDI4K7n/jnN8+uQbrFrUSiwU/DtSEUB/MsKKBT+zYslJqiYNgVE4JwhHkzy86wlWvrKVWDSZ/YFjZlU39yw4y/rGoyQGowWB67zl4QQue+jssMdXrQvZ/00jyeHwqCgDKwnsiJjSvkYAxsG5K9WsenYbJdqAtAjhCIxCSZt/4fK1w5A2WCvxrUAKCHwNVoA2aGmvq11jJQQapEXrgMBKqmJJugejKGWLIxXrBPFoigfv/omd675gRkU/xgqUDlAhH3UDaAAlLSqUQekAYyVTyhLs3tDMsvntlIYzOFcEcOcEGd9jx9oDbGs6QO0t/Tijxi9S4bhzxiWaVh5m94Zm0n7oui4ybo0raUlcncQnxx+g+WgDF/vLoYDmoqSl/dJUnt7XRCoTZjij0Z6Pc2LiNS4EBBkNvoeOJXN+yPWWSZeANOhwJq/98nKVwNdoL8B5AROxBKBL0gjh8DMhdCh3eJnrA0yqhLpplwmyup6IajvAOIGfKGVx3VmCRGnOMpe5QAdG0bT8CAeeep0d6z6nqjSJnQiZWEllLMWrmz6k+fE9rGk8MVqYgsGv5ZH2i1Opr+9kajzB5d74hKQ+KS3d/WVMLhtgdu1lriRiOR/4nDVunaR24x7qp3UV5Cb/fJvC83nv26W81LIK58SYNFmwq4hsGx/5BwKlzYRma2NUthgOJSew4i7ru9nJYCQF5tApb2yvjiDQKJV/IfJKh0o6qssSLKv/jcAoRKHQQzE2Lj2OMV5OkWFc4MZIpsev8uXWXRx6ZicbGk8QZLxxgwe+x/rlR3h3816+f2E7lbEU+ZDn3vKVpePCdFovzCISHqbl5EIoQOteKMPB1rto65zNyfOz+KOrGl06lHPQyi/WOohH0/T0l1MZH6A3GUEKl7Pmr2la6wBrBWWRDP2DUcqjKVKBGom9RZmABAykwnglafpSJSPQvsfiOR0EQ7ExVmazA8cY6N4K1iw6RdAXRwi4mgrheT5Dvs4LeuS81a15Ll/3dQisFVSVpnj7sf1sX/sZvhAc+6UOrQyBVUQ8gx/orFmDsZqtaw/y1qZ9zKjp5vDpenyjcNe+cLNmTiUdf/bEOddVQ0VpgsOn54ET+EYxvWKALSu+5tGG76it7MNaiZKGQ23zCIcMfUMxBnrjN3fmHHvCAlp+vJcXWx6itqoXpAEnUNLx8iMfo5Xh1i17R3PJYCpC2cZ3qK3sQ8WGEDDuXlAQuFKGHzpmopXhTNfk0bmxs7uC1w6uJul79AxFkMIiBJy5UoUWjrZLU5DCFdTARDHuDqVw+OkSwI0MCEW4gtNF2BPrBCo8fKNbtILWX9aUDqFqHnn7AAAAAElFTkSuQmCC)](https://www.fnp.org.pl/en/)
 [![PL Funding](https://img.shields.io/static/v1?label=PL%20Funding%20by&color=d21132&message=NCN&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAANCAYAAACpUE5eAAAABmJLR0QA/wD/AP+gvaeTAAAAKUlEQVQ4jWP8////fwYqAiZqGjZqIHUAy4dJS6lqIOMdEZvRZDPcDQQAb3cIaY1Sbi4AAAAASUVORK5CYII=)](https://www.ncn.gov.pl/?language=en)
-[![Copyright](https://img.shields.io/static/v1?label=Copyright&color=249fe2&message=Jagiellonian%20University&)](https://en.uj.edu.pl/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA/actions)
 [![Appveyor Build status](http://ci.appveyor.com/api/projects/status/github/open-atmos/PyMPDATA?branch=main&svg=true)](https://ci.appveyor.com/project/slayoo/pympdata/branch/main)
 [![Coverage Status](https://codecov.io/gh/open-atmos/PyMPDATA/branch/main/graph/badge.svg)](https://codecov.io/github/open-atmos/PyMPDATA?branch=main)
-[![Github Actions Status](https://github.com/open-atmos/PyMPDATA/actions/workflows/pylint.yml/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA/actions/workflows/pylint.yml)    
-[![GitHub issues](https://img.shields.io/github/issues-pr/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/pulls?q=)
-[![GitHub issues](https://img.shields.io/github/issues-pr-closed/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/pulls?q=is:closed)    
-[![GitHub issues](https://img.shields.io/github/issues/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/issues?q=)
-[![GitHub issues](https://img.shields.io/github/issues-closed/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/issues?q=)    
+
 [![PyPI version](https://badge.fury.io/py/PyMPDATA.svg)](https://pypi.org/project/PyMPDATA)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA/)
 
 PyMPDATA is a high-performance Numba-accelerated Pythonic implementation of the MPDATA 
   algorithm of Smolarkiewicz et al. used in geophysical fluid dynamics and beyond.
 MPDATA numerically solves generalised transport equations -
   partial differential equations used to model conservation/balance laws, scalar-transport problems,
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/__init__.py` & `PyMPDATA-1.0.9/PyMPDATA/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/constant.py` & `PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """ boundary condition filling halos with a constant value """
+# pylint: disable=too-many-arguments
 from functools import lru_cache
 
 import numba
 
+from PyMPDATA.impl.traversals_common import make_fill_halos_loop
+
 
 class Constant:
     """class which instances are to be passed in boundary_conditions tuple to the
     `PyMPDATA.scalar_field.ScalarField` and
     `PyMPDATA.vector_field.VectorField` __init__ methods"""
 
     def __init__(self, value):
         self.value = value
 
-    def make_scalar(self, ats, halo, dtype, jit_flags):
+    def make_scalar(self, ats, set_value, halo, dtype, jit_flags):
         """returns (lru-cached) Numba-compiled scalar halo-filling callable"""
-        return _make_scalar_constant(self.value, ats, halo, dtype, jit_flags)
+        return _make_scalar_constant(self.value, ats, set_value, halo, dtype, jit_flags)
 
-    def make_vector(self, ats, halo, dtype, jit_flags):
+    def make_vector(self, ats, set_value, halo, dtype, jit_flags):
         """returns (lru-cached) Numba-compiled vector halo-filling callable"""
-        return _make_scalar_constant(self.value, ats, halo, dtype, jit_flags)
+        return _make_scalar_constant(self.value, ats, set_value, halo, dtype, jit_flags)
 
 
 @lru_cache()
-def _make_scalar_constant(value, _, __, ___, jit_flags):
+def _make_scalar_constant(value, _, set_value, __, ___, jit_flags):
     @numba.njit(**jit_flags)
     def fill_halos(_1, _2, _3):
         return value
 
-    return fill_halos
+    return make_fill_halos_loop(jit_flags, set_value, fill_halos)
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/extrapolated.py` & `PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/extrapolated.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """ boundary condition extrapolating values from the edge to the halo """
+# pylint: disable=too-many-arguments
 from functools import lru_cache
 
 import numba
 
 from PyMPDATA.impl.enumerations import (
     ARG_FOCUS,
     INNER,
     META_AND_DATA_DATA,
     META_AND_DATA_META,
     SIGN_LEFT,
 )
+from PyMPDATA.impl.traversals_common import make_fill_halos_loop
 
 
 class Extrapolated:
     """class which instances are to be passed in boundary_conditions tuple to the
     `PyMPDATA.scalar_field.ScalarField` and
     `PyMPDATA.vector_field.VectorField` __init__ methods"""
 
     def __init__(self, dim=INNER, eps=1e-10):
         self.eps = eps
         self.dim = dim
 
-    def make_scalar(self, ats, halo, dtype, jit_flags):
+    def make_scalar(self, ats, set_value, halo, dtype, jit_flags):
         """returns (lru-cached) Numba-compiled scalar halo-filling callable"""
         return _make_scalar_extrapolated(
-            self.dim, self.eps, ats, halo, dtype, jit_flags
+            self.dim, self.eps, ats, set_value, halo, dtype, jit_flags
         )
 
-    def make_vector(self, ats, halo, dtype, jit_flags):
+    def make_vector(self, ats, set_value, halo, dtype, jit_flags):
         """returns (lru-cached) Numba-compiled vector halo-filling callable"""
-        return _make_vector_extrapolated(self.dim, ats, halo, dtype, jit_flags)
+        return _make_vector_extrapolated(
+            self.dim, ats, set_value, halo, dtype, jit_flags
+        )
 
 
 @lru_cache()
 # pylint: disable=too-many-arguments
-def _make_scalar_extrapolated(dim, eps, ats, halo, dtype, jit_flags):
+def _make_scalar_extrapolated(dim, eps, ats, set_value, halo, dtype, jit_flags):
     @numba.njit(**jit_flags)
     def impl(psi, span, sign):
         if sign == SIGN_LEFT:
             edg = halo - psi[ARG_FOCUS][dim]
             nom = ats(*psi, edg + 1) - ats(*psi, edg)
             den = ats(*psi, edg + 2) - ats(*psi, edg + 1)
             cnst = nom / den if abs(den) > eps else 0
@@ -64,17 +68,17 @@
 
     else:
 
         @numba.njit(**jit_flags)
         def fill_halos_scalar(psi, span, sign):
             return impl(psi, span, sign)
 
-    return fill_halos_scalar
+    return make_fill_halos_loop(jit_flags, set_value, fill_halos_scalar)
 
 
 @lru_cache()
-def _make_vector_extrapolated(_, ats, __, ___, jit_flags):
+def _make_vector_extrapolated(_, ats, set_value, __, ___, jit_flags):
     @numba.njit(**jit_flags)
     def fill_halos(psi, ____, sign):
         return ats(*psi, sign)
 
-    return fill_halos
+    return make_fill_halos_loop(jit_flags, set_value, fill_halos)
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/periodic.py` & `PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/periodic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """ periodic/cyclic boundary condition logic """
 from functools import lru_cache
 
 import numba
 
 from PyMPDATA.impl.enumerations import SIGN_LEFT, SIGN_RIGHT
+from PyMPDATA.impl.traversals_common import make_fill_halos_loop
 
 
 class Periodic:
     """class which instances are to be passed in boundary_conditions tuple to the
     `PyMPDATA.scalar_field.ScalarField` and
     `PyMPDATA.vector_field.VectorField` __init__ methods"""
 
     def __init__(self):
         assert SIGN_RIGHT == -1
         assert SIGN_LEFT == +1
 
     @staticmethod
-    def make_scalar(ats, _, __, jit_flags):
+    def make_scalar(ats, set_value, _, __, jit_flags):
         """returns (lru-cached) Numba-compiled scalar halo-filling callable"""
-        return _make_scalar_periodic(ats, jit_flags)
+        return _make_scalar_periodic(ats, set_value, jit_flags)
 
     @staticmethod
-    def make_vector(ats, _, __, jit_flags):
+    def make_vector(ats, set_value, _, __, jit_flags):
         """returns (lru-cached) Numba-compiled vector halo-filling callable"""
-        return _make_vector_periodic(ats, jit_flags)
+        return _make_vector_periodic(ats, set_value, jit_flags)
 
 
 @lru_cache()
-def _make_scalar_periodic(ats, jit_flags):
+def _make_scalar_periodic(ats, set_value, jit_flags):
     @numba.njit(**jit_flags)
-    def fill_halos(psi, span, sign):
-        return ats(*psi, sign * span)
+    def fill_halos(focus_psi, span, sign):
+        return ats(*focus_psi, sign * span)
 
-    return fill_halos
+    return make_fill_halos_loop(jit_flags, set_value, fill_halos)
 
 
 @lru_cache()
-def _make_vector_periodic(ats, jit_flags):
+def _make_vector_periodic(ats, set_value, jit_flags):
     @numba.njit(**jit_flags)
-    def fill_halos(psi, span, sign):
-        return ats(*psi, sign * span)
+    def fill_halos(focus_psi, span, sign):
+        return ats(*focus_psi, sign * span)
 
-    return fill_halos
+    return make_fill_halos_loop(jit_flags, set_value, fill_halos)
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/boundary_conditions/polar.py` & `PyMPDATA-1.0.9/PyMPDATA/boundary_conditions/polar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ polar boundary condition for use in with spherical coordinates """
 from functools import lru_cache
 
 import numba
 
 from PyMPDATA.impl.enumerations import ARG_FOCUS, SIGN_LEFT, SIGN_RIGHT
+from PyMPDATA.impl.traversals_common import make_fill_halos_loop
 
 
 class Polar:
     """class which instances are to be passed in boundary_conditions tuple to the
     `ScalarField` and `VectorField` __init__ methods"""
 
     def __init__(self, grid, longitude_idx, latitude_idx):
@@ -18,15 +19,15 @@
         self.nlat = grid[latitude_idx]
         assert self.nlon % 2 == 0
 
         self.nlon_half = self.nlon // 2
         self.lon_idx = longitude_idx
         self.lat_idx = latitude_idx
 
-    def make_scalar(self, ats, halo, _, jit_flags):
+    def make_scalar(self, ats, set_value, halo, _, jit_flags):
         """returns (lru-cached) Numba-compiled scalar halo-filling callable"""
         nlon_half = self.nlon_half
         nlat = self.nlat
         lon_idx = self.lon_idx
         lat_idx = self.lat_idx
         left_edge_idx = halo - 1
         right_edge_idx = nlat + halo
@@ -39,22 +40,22 @@
                 step = (left_edge_idx - lat) * 2 + 1
             else:
                 step = (lat - right_edge_idx) * 2 + 1
 
             val = nlon_half * (-1 if lon > nlon_half else 1)
             return ats(*psi, sign * step, val)
 
-        return fill_halos
+        return make_fill_halos_loop(jit_flags, set_value, fill_halos)
 
     @staticmethod
-    def make_vector(ats, _, __, jit_flags):
+    def make_vector(ats, set_value, _, __, jit_flags):
         """returns (lru-cached) Numba-compiled vector halo-filling callable"""
-        return _make_vector_polar(ats, jit_flags)
+        return _make_vector_polar(ats, set_value, jit_flags)
 
 
 @lru_cache()
-def _make_vector_polar(ats, jit_flags):
+def _make_vector_polar(ats, set_value, jit_flags):
     @numba.njit(**jit_flags)
     def fill_halos(psi, ___, ____):
         return ats(*psi, 0)  # TODO #120
 
-    return fill_halos
+    return make_fill_halos_loop(jit_flags, set_value, fill_halos)
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/domain_decomposition.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/domain_decomposition.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/enumerations.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/enumerations.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/field.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         if traversals.jit_flags != self.__jit_flags:
             method = {"ScalarField": "make_scalar", "VectorField": "make_vector"}[
                 self.__class__.__name__
             ]
             self.__impl = (self.__properties.meta, *self._impl_data), tuple(
                 getattr(fill_halos, method)(
                     traversals.indexers[self.n_dims].ats[i],
+                    traversals.indexers[self.n_dims].set,
                     self.halo,
                     self.dtype,
                     traversals.jit_flags,
                 )
                 for i, fill_halos in enumerate(self.fill_halos)
             )
         self.__jit_flags = traversals.jit_flags
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/formulae_antidiff.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/formulae_antidiff.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/formulae_axpy.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/formulae_axpy.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/formulae_flux.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/formulae_flux.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/formulae_laplacian.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/formulae_laplacian.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/formulae_nonoscillatory.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/formulae_nonoscillatory.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/formulae_upwind.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/formulae_upwind.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/grid.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/grid.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/indexers.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/indexers.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/meta.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/meta.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/impl/traversals.py` & `PyMPDATA-1.0.9/PyMPDATA/impl/traversals.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from pathlib import Path
 
 from ..scalar_field import ScalarField
 from ..vector_field import VectorField
 from .enumerations import INNER, MID3D, OUTER
 from .grid import make_chunk, make_domain
 from .indexers import make_indexers
-from .traversals_scalar import _make_apply_scalar, _make_fill_halos_scalar
-from .traversals_vector import _make_apply_vector, _make_fill_halos_vector
+from .traversals_halos_scalar import _make_fill_halos_scalar
+from .traversals_halos_vector import _make_fill_halos_vector
+from .traversals_scalar import _make_apply_scalar
+from .traversals_vector import _make_apply_vector
 
 
 class Traversals:
     """groups njit-ted traversals for a given grid, halo, jit_flags and threading settings"""
 
     def __init__(self, *, grid, halo, jit_flags, n_threads, left_first):
         assert not (n_threads > 1 and len(grid) == 1)
@@ -34,15 +36,14 @@
             Path(__file__).stem + "NullFields", ("scalar", "vector")
         )(
             scalar=ScalarField.make_null(self.n_dims, self).impl,
             vector=VectorField.make_null(self.n_dims, self).impl,
         )
 
         common_kwargs = {
-            "indexers": self.indexers,
             "jit_flags": jit_flags,
             "halo": halo,
             "n_dims": self.n_dims,
             "chunker": chunk,
             "spanner": domain,
         }
         self._code = {
@@ -53,14 +54,15 @@
             "fill_halos_vector": _make_fill_halos_vector(
                 left_first=left_first,
                 **common_kwargs,
             ),
         }
         common_kwargs = {
             **common_kwargs,
+            "indexers": self.indexers,
             **{
                 "boundary_cond_vector": self._code["fill_halos_vector"],
                 "boundary_cond_scalar": self._code["fill_halos_scalar"],
                 "n_threads": n_threads,
             },
         }
         self._code = {
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA/options.py` & `PyMPDATA-1.0.9/PyMPDATA/options.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/scalar_field.py` & `PyMPDATA-1.0.9/PyMPDATA/scalar_field.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/solver.py` & `PyMPDATA-1.0.9/PyMPDATA/solver.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/stepper.py` & `PyMPDATA-1.0.9/PyMPDATA/stepper.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA/vector_field.py` & `PyMPDATA-1.0.9/PyMPDATA/vector_field.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/PyMPDATA.egg-info/PKG-INFO` & `PyMPDATA-1.0.9/PyMPDATA.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMPDATA
-Version: 1.0.8
+Version: 1.0.9
 Summary: Numba-accelerated Pythonic implementation of MPDATA with examples in Python, Julia and Matlab
 Author: https://github.com/open-atmos/PyMPDATA/graphs/contributors
 Author-email: sylwester.arabas@uj.edu.pl
 License: GPL-3.0
 Project-URL: Tracker, https://github.com/open-atmos/PyMPDATA/issues
 Project-URL: Documentation, https://open-atmos.github.io/PyMPDATA
 Project-URL: Source, https://github.com/open-atmos/PyMPDATA
@@ -27,30 +27,25 @@
 [![Python 3](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3)](https://www.python.org/)
 [![LLVM](https://img.shields.io/static/v1?label=LLVM&logo=LLVM&color=gold&message=Numba)](https://www.numba.org)
 [![Linux OK](https://img.shields.io/static/v1?label=Linux&logo=Linux&color=yellow&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Linux)
 [![macOS OK](https://img.shields.io/static/v1?label=macOS&logo=Apple&color=silver&message=%E2%9C%93)](https://en.wikipedia.org/wiki/macOS)
 [![Windows OK](https://img.shields.io/static/v1?label=Windows&logo=Windows&color=white&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Windows)
 [![Jupyter](https://img.shields.io/static/v1?label=Jupyter&logo=Jupyter&color=f37626&message=%E2%9C%93)](https://jupyter.org/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/open-atmos/PyMPDATA/graphs/commit-activity)
-[![OpenHub](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA/widgets/project_thin_badge?format=gif)](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA)
+[![OpenHub](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA/widgets/project_thin_badge?format=gif)](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA)   
 [![status](https://joss.theoj.org/papers/10e7361e43785dbb1b3d659c5b01757a/status.svg)](https://joss.theoj.org/papers/10e7361e43785dbb1b3d659c5b01757a)
 [![DOI](https://zenodo.org/badge/225610671.svg)](https://zenodo.org/badge/latestdoi/225610671)     
 [![EU Funding](https://img.shields.io/static/v1?label=EU%20Funding%20by&color=103069&message=FNP&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAC4AAAAeCAYAAABTwyyaAAAEzklEQVRYw9WYS2yUVRiGn3P5ZzozpZ3aUsrNgoKlKBINmkhpCCwwxIAhsDCpBBIWhmCMMYTEhSJ4i9EgBnSBEm81MRrFBhNXEuUSMCopiRWLQqEGLNgr085M5//POS46NNYFzHQ6qGc1i5nzP/P973m/9ztCrf7A8T9csiibCocUbvTzfxLcAcaM3cY3imXz25lT3Y34G7gQYAKV3+bFAHcATlBTPogJNADG92iY28FHW97kyPbnuW/W7xgzAhukQ9xe04PJeOT0HkQRwK0TlEeGWb/kOO9v3kdD3a8YK9GhDMfa6mg9fxunOm/lWPtcpDI4K7n/jnN8+uQbrFrUSiwU/DtSEUB/MsKKBT+zYslJqiYNgVE4JwhHkzy86wlWvrKVWDSZ/YFjZlU39yw4y/rGoyQGowWB67zl4QQue+jssMdXrQvZ/00jyeHwqCgDKwnsiJjSvkYAxsG5K9WsenYbJdqAtAjhCIxCSZt/4fK1w5A2WCvxrUAKCHwNVoA2aGmvq11jJQQapEXrgMBKqmJJugejKGWLIxXrBPFoigfv/omd675gRkU/xgqUDlAhH3UDaAAlLSqUQekAYyVTyhLs3tDMsvntlIYzOFcEcOcEGd9jx9oDbGs6QO0t/Tijxi9S4bhzxiWaVh5m94Zm0n7oui4ybo0raUlcncQnxx+g+WgDF/vLoYDmoqSl/dJUnt7XRCoTZjij0Z6Pc2LiNS4EBBkNvoeOJXN+yPWWSZeANOhwJq/98nKVwNdoL8B5AROxBKBL0gjh8DMhdCh3eJnrA0yqhLpplwmyup6IajvAOIGfKGVx3VmCRGnOMpe5QAdG0bT8CAeeep0d6z6nqjSJnQiZWEllLMWrmz6k+fE9rGk8MVqYgsGv5ZH2i1Opr+9kajzB5d74hKQ+KS3d/WVMLhtgdu1lriRiOR/4nDVunaR24x7qp3UV5Cb/fJvC83nv26W81LIK58SYNFmwq4hsGx/5BwKlzYRma2NUthgOJSew4i7ru9nJYCQF5tApb2yvjiDQKJV/IfJKh0o6qssSLKv/jcAoRKHQQzE2Lj2OMV5OkWFc4MZIpsev8uXWXRx6ZicbGk8QZLxxgwe+x/rlR3h3816+f2E7lbEU+ZDn3vKVpePCdFovzCISHqbl5EIoQOteKMPB1rto65zNyfOz+KOrGl06lHPQyi/WOohH0/T0l1MZH6A3GUEKl7Pmr2la6wBrBWWRDP2DUcqjKVKBGom9RZmABAykwnglafpSJSPQvsfiOR0EQ7ExVmazA8cY6N4K1iw6RdAXRwi4mgrheT5Dvs4LeuS81a15Ll/3dQisFVSVpnj7sf1sX/sZvhAc+6UOrQyBVUQ8gx/orFmDsZqtaw/y1qZ9zKjp5vDpenyjcNe+cLNmTiUdf/bEOddVQ0VpgsOn54ET+EYxvWKALSu+5tGG76it7MNaiZKGQ23zCIcMfUMxBnrjN3fmHHvCAlp+vJcXWx6itqoXpAEnUNLx8iMfo5Xh1i17R3PJYCpC2cZ3qK3sQ8WGEDDuXlAQuFKGHzpmopXhTNfk0bmxs7uC1w6uJul79AxFkMIiBJy5UoUWjrZLU5DCFdTARDHuDqVw+OkSwI0MCEW4gtNF2BPrBCo8fKNbtILWX9aUDqFqHnn7AAAAAElFTkSuQmCC)](https://www.fnp.org.pl/en/)
 [![PL Funding](https://img.shields.io/static/v1?label=PL%20Funding%20by&color=d21132&message=NCN&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAANCAYAAACpUE5eAAAABmJLR0QA/wD/AP+gvaeTAAAAKUlEQVQ4jWP8////fwYqAiZqGjZqIHUAy4dJS6lqIOMdEZvRZDPcDQQAb3cIaY1Sbi4AAAAASUVORK5CYII=)](https://www.ncn.gov.pl/?language=en)
-[![Copyright](https://img.shields.io/static/v1?label=Copyright&color=249fe2&message=Jagiellonian%20University&)](https://en.uj.edu.pl/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA/actions)
 [![Appveyor Build status](http://ci.appveyor.com/api/projects/status/github/open-atmos/PyMPDATA?branch=main&svg=true)](https://ci.appveyor.com/project/slayoo/pympdata/branch/main)
 [![Coverage Status](https://codecov.io/gh/open-atmos/PyMPDATA/branch/main/graph/badge.svg)](https://codecov.io/github/open-atmos/PyMPDATA?branch=main)
-[![Github Actions Status](https://github.com/open-atmos/PyMPDATA/actions/workflows/pylint.yml/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA/actions/workflows/pylint.yml)    
-[![GitHub issues](https://img.shields.io/github/issues-pr/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/pulls?q=)
-[![GitHub issues](https://img.shields.io/github/issues-pr-closed/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/pulls?q=is:closed)    
-[![GitHub issues](https://img.shields.io/github/issues/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/issues?q=)
-[![GitHub issues](https://img.shields.io/github/issues-closed/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/issues?q=)    
+
 [![PyPI version](https://badge.fury.io/py/PyMPDATA.svg)](https://pypi.org/project/PyMPDATA)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA/)
 
 PyMPDATA is a high-performance Numba-accelerated Pythonic implementation of the MPDATA 
   algorithm of Smolarkiewicz et al. used in geophysical fluid dynamics and beyond.
 MPDATA numerically solves generalised transport equations -
   partial differential equations used to model conservation/balance laws, scalar-transport problems,
```

### Comparing `PyMPDATA-1.0.8/PyMPDATA.egg-info/SOURCES.txt` & `PyMPDATA-1.0.9/PyMPDATA.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 PyMPDATA/impl/formulae_nonoscillatory.py
 PyMPDATA/impl/formulae_upwind.py
 PyMPDATA/impl/grid.py
 PyMPDATA/impl/indexers.py
 PyMPDATA/impl/meta.py
 PyMPDATA/impl/traversals.py
 PyMPDATA/impl/traversals_common.py
+PyMPDATA/impl/traversals_halos_scalar.py
+PyMPDATA/impl/traversals_halos_vector.py
 PyMPDATA/impl/traversals_scalar.py
 PyMPDATA/impl/traversals_vector.py
 paper/fig-crop.pdf
 paper/fig-perf.pdf
 paper/paper.bib
 paper/paper.md
 tests/__init__.py
@@ -56,19 +58,19 @@
 tests/smoke_tests/__init__.py
 tests/smoke_tests/arabas_and_farhat_2020/test_black_scholes.py
 tests/smoke_tests/jarecka_et_al_2015/test_just_do_it.py
 tests/smoke_tests/jaruga_et_al_2015/__init__.py
 tests/smoke_tests/jaruga_et_al_2015/test_libmpdata_refdata.py
 tests/smoke_tests/kinematic_2d/__init__.py
 tests/smoke_tests/kinematic_2d/test_single_timestep.py
-tests/smoke_tests/olesik_et_al_2020/__init__.py
-tests/smoke_tests/olesik_et_al_2020/convergence_refdata.txt
-tests/smoke_tests/olesik_et_al_2020/test_moment_of_r_integral.py
-tests/smoke_tests/olesik_et_al_2020/test_simulation.py
-tests/smoke_tests/olesik_et_al_2020/test_wall_time.py
+tests/smoke_tests/olesik_et_al_2022/__init__.py
+tests/smoke_tests/olesik_et_al_2022/convergence_refdata.txt
+tests/smoke_tests/olesik_et_al_2022/test_moment_of_r_integral.py
+tests/smoke_tests/olesik_et_al_2022/test_simulation.py
+tests/smoke_tests/olesik_et_al_2022/test_wall_time.py
 tests/smoke_tests/smolarkiewicz_1983/test_against_libmpdata_refdata.py
 tests/smoke_tests/smolarkiewicz_2006/test_run_all.py
 tests/smoke_tests/timing/__init__.py
 tests/smoke_tests/timing/fixtures.py
 tests/smoke_tests/timing/test_timing_1d.py
 tests/smoke_tests/timing/test_timing_2d.py
 tests/smoke_tests/timing/test_timing_3d.py
```

### Comparing `PyMPDATA-1.0.8/README.md` & `PyMPDATA-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 [![Python 3](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3)](https://www.python.org/)
 [![LLVM](https://img.shields.io/static/v1?label=LLVM&logo=LLVM&color=gold&message=Numba)](https://www.numba.org)
 [![Linux OK](https://img.shields.io/static/v1?label=Linux&logo=Linux&color=yellow&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Linux)
 [![macOS OK](https://img.shields.io/static/v1?label=macOS&logo=Apple&color=silver&message=%E2%9C%93)](https://en.wikipedia.org/wiki/macOS)
 [![Windows OK](https://img.shields.io/static/v1?label=Windows&logo=Windows&color=white&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Windows)
 [![Jupyter](https://img.shields.io/static/v1?label=Jupyter&logo=Jupyter&color=f37626&message=%E2%9C%93)](https://jupyter.org/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/open-atmos/PyMPDATA/graphs/commit-activity)
-[![OpenHub](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA/widgets/project_thin_badge?format=gif)](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA)
+[![OpenHub](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA/widgets/project_thin_badge?format=gif)](https://www.openhub.net/p/atmos-cloud-sim-uj-PyMPDATA)   
 [![status](https://joss.theoj.org/papers/10e7361e43785dbb1b3d659c5b01757a/status.svg)](https://joss.theoj.org/papers/10e7361e43785dbb1b3d659c5b01757a)
 [![DOI](https://zenodo.org/badge/225610671.svg)](https://zenodo.org/badge/latestdoi/225610671)     
 [![EU Funding](https://img.shields.io/static/v1?label=EU%20Funding%20by&color=103069&message=FNP&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAC4AAAAeCAYAAABTwyyaAAAEzklEQVRYw9WYS2yUVRiGn3P5ZzozpZ3aUsrNgoKlKBINmkhpCCwwxIAhsDCpBBIWhmCMMYTEhSJ4i9EgBnSBEm81MRrFBhNXEuUSMCopiRWLQqEGLNgr085M5//POS46NNYFzHQ6qGc1i5nzP/P973m/9ztCrf7A8T9csiibCocUbvTzfxLcAcaM3cY3imXz25lT3Y34G7gQYAKV3+bFAHcATlBTPogJNADG92iY28FHW97kyPbnuW/W7xgzAhukQ9xe04PJeOT0HkQRwK0TlEeGWb/kOO9v3kdD3a8YK9GhDMfa6mg9fxunOm/lWPtcpDI4K7n/jnN8+uQbrFrUSiwU/DtSEUB/MsKKBT+zYslJqiYNgVE4JwhHkzy86wlWvrKVWDSZ/YFjZlU39yw4y/rGoyQGowWB67zl4QQue+jssMdXrQvZ/00jyeHwqCgDKwnsiJjSvkYAxsG5K9WsenYbJdqAtAjhCIxCSZt/4fK1w5A2WCvxrUAKCHwNVoA2aGmvq11jJQQapEXrgMBKqmJJugejKGWLIxXrBPFoigfv/omd675gRkU/xgqUDlAhH3UDaAAlLSqUQekAYyVTyhLs3tDMsvntlIYzOFcEcOcEGd9jx9oDbGs6QO0t/Tijxi9S4bhzxiWaVh5m94Zm0n7oui4ybo0raUlcncQnxx+g+WgDF/vLoYDmoqSl/dJUnt7XRCoTZjij0Z6Pc2LiNS4EBBkNvoeOJXN+yPWWSZeANOhwJq/98nKVwNdoL8B5AROxBKBL0gjh8DMhdCh3eJnrA0yqhLpplwmyup6IajvAOIGfKGVx3VmCRGnOMpe5QAdG0bT8CAeeep0d6z6nqjSJnQiZWEllLMWrmz6k+fE9rGk8MVqYgsGv5ZH2i1Opr+9kajzB5d74hKQ+KS3d/WVMLhtgdu1lriRiOR/4nDVunaR24x7qp3UV5Cb/fJvC83nv26W81LIK58SYNFmwq4hsGx/5BwKlzYRma2NUthgOJSew4i7ru9nJYCQF5tApb2yvjiDQKJV/IfJKh0o6qssSLKv/jcAoRKHQQzE2Lj2OMV5OkWFc4MZIpsev8uXWXRx6ZicbGk8QZLxxgwe+x/rlR3h3816+f2E7lbEU+ZDn3vKVpePCdFovzCISHqbl5EIoQOteKMPB1rto65zNyfOz+KOrGl06lHPQyi/WOohH0/T0l1MZH6A3GUEKl7Pmr2la6wBrBWWRDP2DUcqjKVKBGom9RZmABAykwnglafpSJSPQvsfiOR0EQ7ExVmazA8cY6N4K1iw6RdAXRwi4mgrheT5Dvs4LeuS81a15Ll/3dQisFVSVpnj7sf1sX/sZvhAc+6UOrQyBVUQ8gx/orFmDsZqtaw/y1qZ9zKjp5vDpenyjcNe+cLNmTiUdf/bEOddVQ0VpgsOn54ET+EYxvWKALSu+5tGG76it7MNaiZKGQ23zCIcMfUMxBnrjN3fmHHvCAlp+vJcXWx6itqoXpAEnUNLx8iMfo5Xh1i17R3PJYCpC2cZ3qK3sQ8WGEDDuXlAQuFKGHzpmopXhTNfk0bmxs7uC1w6uJul79AxFkMIiBJy5UoUWjrZLU5DCFdTARDHuDqVw+OkSwI0MCEW4gtNF2BPrBCo8fKNbtILWX9aUDqFqHnn7AAAAAElFTkSuQmCC)](https://www.fnp.org.pl/en/)
 [![PL Funding](https://img.shields.io/static/v1?label=PL%20Funding%20by&color=d21132&message=NCN&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAANCAYAAACpUE5eAAAABmJLR0QA/wD/AP+gvaeTAAAAKUlEQVQ4jWP8////fwYqAiZqGjZqIHUAy4dJS6lqIOMdEZvRZDPcDQQAb3cIaY1Sbi4AAAAASUVORK5CYII=)](https://www.ncn.gov.pl/?language=en)
-[![Copyright](https://img.shields.io/static/v1?label=Copyright&color=249fe2&message=Jagiellonian%20University&)](https://en.uj.edu.pl/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA/actions)
 [![Appveyor Build status](http://ci.appveyor.com/api/projects/status/github/open-atmos/PyMPDATA?branch=main&svg=true)](https://ci.appveyor.com/project/slayoo/pympdata/branch/main)
 [![Coverage Status](https://codecov.io/gh/open-atmos/PyMPDATA/branch/main/graph/badge.svg)](https://codecov.io/github/open-atmos/PyMPDATA?branch=main)
-[![Github Actions Status](https://github.com/open-atmos/PyMPDATA/actions/workflows/pylint.yml/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA/actions/workflows/pylint.yml)    
-[![GitHub issues](https://img.shields.io/github/issues-pr/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/pulls?q=)
-[![GitHub issues](https://img.shields.io/github/issues-pr-closed/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/pulls?q=is:closed)    
-[![GitHub issues](https://img.shields.io/github/issues/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/issues?q=)
-[![GitHub issues](https://img.shields.io/github/issues-closed/open-atmos/PyMPDATA.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA/issues?q=)    
+
 [![PyPI version](https://badge.fury.io/py/PyMPDATA.svg)](https://pypi.org/project/PyMPDATA)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA/)
 
 PyMPDATA is a high-performance Numba-accelerated Pythonic implementation of the MPDATA 
   algorithm of Smolarkiewicz et al. used in geophysical fluid dynamics and beyond.
 MPDATA numerically solves generalised transport equations -
   partial differential equations used to model conservation/balance laws, scalar-transport problems,
```

### Comparing `PyMPDATA-1.0.8/appveyor.yml` & `PyMPDATA-1.0.9/appveyor.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/paper/fig-crop.pdf` & `PyMPDATA-1.0.9/paper/fig-crop.pdf`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/paper/fig-perf.pdf` & `PyMPDATA-1.0.9/paper/fig-perf.pdf`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/paper/paper.bib` & `PyMPDATA-1.0.9/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/paper/paper.md` & `PyMPDATA-1.0.9/paper/paper.md`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/setup.py` & `PyMPDATA-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/devops_tests/test_todos_annotated.py` & `PyMPDATA-1.0.9/tests/devops_tests/test_todos_annotated.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/jarecka_et_al_2015/test_just_do_it.py` & `PyMPDATA-1.0.9/tests/smoke_tests/jarecka_et_al_2015/test_just_do_it.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/jaruga_et_al_2015/test_libmpdata_refdata.py` & `PyMPDATA-1.0.9/tests/smoke_tests/jaruga_et_al_2015/test_libmpdata_refdata.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/kinematic_2d/test_single_timestep.py` & `PyMPDATA-1.0.9/tests/smoke_tests/kinematic_2d/test_single_timestep.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/test_moment_of_r_integral.py` & `PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/test_moment_of_r_integral.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
 import numpy as np
 import pint
 import pytest
-from PyMPDATA_examples.Olesik_et_al_2020.coordinates import x_id, x_log_of_pn, x_p2
+from PyMPDATA_examples.Olesik_et_al_2022.coordinates import x_id, x_log_of_pn, x_p2
 
 si = pint.UnitRegistry()
 
 
 @pytest.mark.parametrize("k", [0, 1, 2, 3])
 @pytest.mark.parametrize("coord", [x_id(), x_log_of_pn(r0=1 * si.um, n=1), x_p2()])
 def test_moment_of_r_integral(k, coord):
```

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/olesik_et_al_2020/test_simulation.py` & `PyMPDATA-1.0.9/tests/smoke_tests/olesik_et_al_2022/test_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
 import warnings
 
 import numpy as np
 import pytest
 from numba.core.errors import NumbaExperimentalFeatureWarning
-from PyMPDATA_examples.Olesik_et_al_2020.analysis import compute_figure_data
-from PyMPDATA_examples.Olesik_et_al_2020.coordinates import x_id, x_log_of_pn, x_p2
-from PyMPDATA_examples.Olesik_et_al_2020.settings import (
+from PyMPDATA_examples.Olesik_et_al_2022.analysis import compute_figure_data
+from PyMPDATA_examples.Olesik_et_al_2022.coordinates import x_id, x_log_of_pn, x_p2
+from PyMPDATA_examples.Olesik_et_al_2022.settings import (
     Settings,
     default_GC_max,
     default_nr,
 )
-from PyMPDATA_examples.Olesik_et_al_2020.simulation import Simulation
+from PyMPDATA_examples.Olesik_et_al_2022.simulation import Simulation
 
 from PyMPDATA.options import Options
 
 settings = Settings()
 grid_layout_set = (x_id(), x_p2(), x_log_of_pn(r0=1, n=1))
 opt_set = (
     {"n_iters": 1},
```

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/smolarkiewicz_1983/test_against_libmpdata_refdata.py` & `PyMPDATA-1.0.9/tests/smoke_tests/smolarkiewicz_1983/test_against_libmpdata_refdata.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/smolarkiewicz_2006/test_run_all.py` & `PyMPDATA-1.0.9/tests/smoke_tests/smolarkiewicz_2006/test_run_all.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/timing/fixtures.py` & `PyMPDATA-1.0.9/tests/smoke_tests/timing/fixtures.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/timing/test_timing_1d.py` & `PyMPDATA-1.0.9/tests/smoke_tests/timing/test_timing_1d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/timing/test_timing_2d.py` & `PyMPDATA-1.0.9/tests/smoke_tests/timing/test_timing_2d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/smoke_tests/timing/test_timing_3d.py` & `PyMPDATA-1.0.9/tests/smoke_tests/timing/test_timing_3d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_boundary_condition_extrapolated_1d.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_boundary_condition_extrapolated_1d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_boundary_condition_periodic_nd.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_boundary_condition_periodic_nd.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_boundary_condition_polar_2d.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_boundary_condition_polar_2d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_clock.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_clock.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_diffusion_only_2d.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_diffusion_only_2d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_domain_decomposition.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_domain_decomposition.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_dpdc.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_dpdc.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_formulae_upwind.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_formulae_upwind.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_grid.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_mpdata_2d.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_mpdata_2d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_scalar_field.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_scalar_field.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_shared_advector.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_shared_advector.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_solver.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_stepper.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_stepper.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_traversals.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_traversals.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_upwind_1d.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_upwind_1d.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-1.0.8/tests/unit_tests/test_upwind_2d.py` & `PyMPDATA-1.0.9/tests/unit_tests/test_upwind_2d.py`

 * *Files identical despite different names*

