# Comparing `tmp/pyLIQTR-0.3.2.tar.gz` & `tmp/pyLIQTR-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLIQTR-0.3.2.tar", last modified: Fri Jul 21 15:39:29 2023, max compression
+gzip compressed data, was "pyLIQTR-0.3.3.tar", last modified: Fri Jul 21 16:02:07 2023, max compression
```

## Comparing `pyLIQTR-0.3.2.tar` & `pyLIQTR-0.3.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.737407 pyLIQTR-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-21 15:39:29.737407 pyLIQTR-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:39:29.737407 pyLIQTR-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.697406 pyLIQTR-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.701406 pyLIQTR-0.3.2/src/pyLIQTR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.705406 pyLIQTR-0.3.2/src/pyLIQTR/GSE/
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/GSE/GSE.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/GSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.705406 pyLIQTR-0.3.2/src/pyLIQTR/GSE/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/GSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/GSE/tests/test_GSE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.709406 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/pe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/pe_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/pe_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.709406 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.713406 pyLIQTR-0.3.2/src/pyLIQTR/QSP/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/Hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/QSP.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/gen_qsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_cirq_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21006 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    20121 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_select_v.py
--rw-r--r--   0 runner    (1001) docker     (123)    39900 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/qspangles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.713406 pyLIQTR-0.3.2/src/pyLIQTR/QSP/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/QSP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.713406 pyLIQTR-0.3.2/src/pyLIQTR/circuits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/circuits/pyLCircuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/circuits/pyLOperator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.717406 pyLIQTR-0.3.2/src/pyLIQTR/circuits/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/circuits/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/circuits/tests/test_pyLCircuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/circuits/tests/test_pyLOperator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.725407 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/cirq_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/clifford_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/decimal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/exact_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/gate_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/grid_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/point_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/rings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/rotation_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/solve_diophantine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_cirq_tranformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_decimal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_exact_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    30480 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_point_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_solve_diophantine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.729407 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20516 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_cirq_tranformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_decimal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.729407 pyLIQTR-0.3.2/src/pyLIQTR/model_simulators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/model_simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/model_simulators/qspsim.py
--rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/model_simulators/vlasovsim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.733407 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/ChebyshevPoly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/__internal__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/angler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/expander.py
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51225 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/quantum_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/simqsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.733407 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/tests/test_simqsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.733407 pyLIQTR-0.3.2/src/pyLIQTR/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/utils/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/utils/printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.737407 pyLIQTR-0.3.2/src/pyLIQTR/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/utils/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-21 15:39:17.000000 pyLIQTR-0.3.2/src/pyLIQTR/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:39:29.705406 pyLIQTR-0.3.2/src/pyLIQTR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-21 15:39:29.000000 pyLIQTR-0.3.2/src/pyLIQTR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-21 15:39:29.000000 pyLIQTR-0.3.2/src/pyLIQTR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:39:29.000000 pyLIQTR-0.3.2/src/pyLIQTR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 15:39:29.000000 pyLIQTR-0.3.2/src/pyLIQTR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 15:39:29.000000 pyLIQTR-0.3.2/src/pyLIQTR.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.217277 pyLIQTR-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 16:02:07.217277 pyLIQTR-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:02:07.217277 pyLIQTR-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.185275 pyLIQTR-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.189275 pyLIQTR-0.3.3/src/pyLIQTR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.193276 pyLIQTR-0.3.3/src/pyLIQTR/GSE/
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/GSE/GSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/GSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.193276 pyLIQTR-0.3.3/src/pyLIQTR/GSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/GSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/GSE/tests/test_GSE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.193276 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/pe_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/pe_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.193276 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.197276 pyLIQTR-0.3.3/src/pyLIQTR/QSP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/Hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/QSP.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/gen_qsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_cirq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21006 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20121 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_select_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39900 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/qspangles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.197276 pyLIQTR-0.3.3/src/pyLIQTR/QSP/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/QSP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.201276 pyLIQTR-0.3.3/src/pyLIQTR/circuits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/circuits/pyLCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/circuits/pyLOperator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.201276 pyLIQTR-0.3.3/src/pyLIQTR/circuits/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/circuits/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/circuits/tests/test_pyLCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/circuits/tests/test_pyLOperator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.209277 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/cirq_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/clifford_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/decimal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/exact_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/gate_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/grid_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/point_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/rings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/rotation_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/solve_diophantine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_cirq_tranformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_decimal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_exact_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30480 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_point_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_solve_diophantine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.209277 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20516 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_cirq_tranformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_decimal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.213277 pyLIQTR-0.3.3/src/pyLIQTR/model_simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/model_simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/model_simulators/qspsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/model_simulators/vlasovsim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.213277 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/ChebyshevPoly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/__internal__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/angler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51225 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/quantum_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/simqsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.217277 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/tests/test_simqsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.217277 pyLIQTR-0.3.3/src/pyLIQTR/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/utils/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/utils/printing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.217277 pyLIQTR-0.3.3/src/pyLIQTR/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-21 16:01:55.000000 pyLIQTR-0.3.3/src/pyLIQTR/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:07.193276 pyLIQTR-0.3.3/src/pyLIQTR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 16:02:07.000000 pyLIQTR-0.3.3/src/pyLIQTR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-21 16:02:07.000000 pyLIQTR-0.3.3/src/pyLIQTR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:02:07.000000 pyLIQTR-0.3.3/src/pyLIQTR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 16:02:07.000000 pyLIQTR-0.3.3/src/pyLIQTR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 16:02:07.000000 pyLIQTR-0.3.3/src/pyLIQTR.egg-info/top_level.txt
```

### Comparing `pyLIQTR-0.3.2/LICENSE.txt` & `pyLIQTR-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/PKG-INFO` & `pyLIQTR-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyLIQTR
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python package for generating quantum circuits using quantum algorithms.
 Author: Kevin Obenland, Justin Elenewski, Arthur Kurlej,  Joe Belarge, John Blue, and Robert Rood
 Author-email: Kevin.Obenland@ll.mit.edu
 License: BDS-2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# pyLIQTR Version 0.3.1
+# pyLIQTR
 _Kevin Obenland, Justin Elenewski, Arthur Kurlej, Joe Belarge, John Blue &  Robert Rood_
 
 ---
 ## Description
 `pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms. Once the circuits have been generated, one can simulate them (if they are small enough), or utilize them for resource estimations. The codebase is actively developed, and currently supports the following algorithms:
 - Hamiltonian Simulation using Quantum Signal Processing (QSP) for real-valued Hamiltonians
```

### Comparing `pyLIQTR-0.3.2/README.md` & `pyLIQTR-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pyLIQTR Version 0.3.1
+# pyLIQTR
 _Kevin Obenland, Justin Elenewski, Arthur Kurlej, Joe Belarge, John Blue &  Robert Rood_
 
 ---
 ## Description
 `pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms. Once the circuits have been generated, one can simulate them (if they are small enough), or utilize them for resource estimations. The codebase is actively developed, and currently supports the following algorithms:
 - Hamiltonian Simulation using Quantum Signal Processing (QSP) for real-valued Hamiltonians
```

### Comparing `pyLIQTR-0.3.2/setup.py` & `pyLIQTR-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "A python package for generating quantum circuits using quantum algorithms."
 )
 THIS_DIRECTORY = Path(__file__).parent
 LONG_DESCRIPTION = (THIS_DIRECTORY / "README.md").read_text()
 
 setup(
     name=DISTNAME,
-    version="0.3.2",
+    version="0.3.3",
     license=LICENSE,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     packages=find_packages(where="src"),
```

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/GSE/GSE.py` & `pyLIQTR-0.3.3/src/pyLIQTR/GSE/GSE.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/GSE/tests/test_GSE.py` & `pyLIQTR-0.3.3/src/pyLIQTR/GSE/tests/test_GSE.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/pe.py` & `pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/pe.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/pe_gates.py` & `pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/pe_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/PhaseEstimation/pe_sim.py` & `pyLIQTR-0.3.3/src/pyLIQTR/PhaseEstimation/pe_sim.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/Hamiltonian.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/Hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/QSP.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/QSP.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/gen_qsp.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/gen_qsp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_cirq_gates.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_cirq_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_helpers.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_helpers.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_prepare.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_prepare.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/qsp_select_v.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/qsp_select_v.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/QSP/qspangles.py` & `pyLIQTR-0.3.3/src/pyLIQTR/QSP/qspangles.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/circuits/pyLCircuit.py` & `pyLIQTR-0.3.3/src/pyLIQTR/circuits/pyLCircuit.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/circuits/pyLOperator.py` & `pyLIQTR-0.3.3/src/pyLIQTR/circuits/pyLOperator.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/circuits/tests/test_pyLCircuit.py` & `pyLIQTR-0.3.3/src/pyLIQTR/circuits/tests/test_pyLCircuit.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/circuits/tests/test_pyLOperator.py` & `pyLIQTR-0.3.3/src/pyLIQTR/circuits/tests/test_pyLOperator.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/cirq_transforms.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/cirq_transforms.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/clifford_gates.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/clifford_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/decimal_utils.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/decimal_utils.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/ellipse.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/ellipse.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/exact_decomp.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/exact_decomp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/gate_approximation.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/gate_approximation.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/grid_operator.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/grid_operator.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/matrices.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/matrices.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/point_enumeration.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/point_enumeration.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/rings.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/rings.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/rotation_gates.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/rotation_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/solve_diophantine.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/solve_diophantine.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_cirq_tranformers.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_cirq_tranformers.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_decimal_utils.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_decimal_utils.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_exact_decomp.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_exact_decomp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_matrices.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_matrices.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_point_enumeration.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_point_enumeration.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/test_solve_diophantine.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/test_solve_diophantine.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_cirq_tranformers.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_cirq_tranformers.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_decimal_utils.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_decimal_utils.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_matrices.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py` & `pyLIQTR-0.3.3/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/model_simulators/qspsim.py` & `pyLIQTR-0.3.3/src/pyLIQTR/model_simulators/qspsim.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/model_simulators/vlasovsim.py` & `pyLIQTR-0.3.3/src/pyLIQTR/model_simulators/vlasovsim.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/ChebyshevPoly.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/ChebyshevPoly.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/__internal__.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/__internal__.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/angler.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/angler.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/expander.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/expander.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/fitter.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/fitter.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/quantum_ops.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/quantum_ops.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/simqsp.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/simqsp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/sim_methods/tests/test_simqsp.py` & `pyLIQTR-0.3.3/src/pyLIQTR/sim_methods/tests/test_simqsp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/utils/plot_helpers.py` & `pyLIQTR-0.3.3/src/pyLIQTR/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/utils/printing.py` & `pyLIQTR-0.3.3/src/pyLIQTR/utils/printing.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/utils/tests/test_utils.py` & `pyLIQTR-0.3.3/src/pyLIQTR/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR/utils/utils.py` & `pyLIQTR-0.3.3/src/pyLIQTR/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR.egg-info/PKG-INFO` & `pyLIQTR-0.3.3/src/pyLIQTR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyLIQTR
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python package for generating quantum circuits using quantum algorithms.
 Author: Kevin Obenland, Justin Elenewski, Arthur Kurlej,  Joe Belarge, John Blue, and Robert Rood
 Author-email: Kevin.Obenland@ll.mit.edu
 License: BDS-2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# pyLIQTR Version 0.3.1
+# pyLIQTR
 _Kevin Obenland, Justin Elenewski, Arthur Kurlej, Joe Belarge, John Blue &  Robert Rood_
 
 ---
 ## Description
 `pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms. Once the circuits have been generated, one can simulate them (if they are small enough), or utilize them for resource estimations. The codebase is actively developed, and currently supports the following algorithms:
 - Hamiltonian Simulation using Quantum Signal Processing (QSP) for real-valued Hamiltonians
```

### Comparing `pyLIQTR-0.3.2/src/pyLIQTR.egg-info/SOURCES.txt` & `pyLIQTR-0.3.3/src/pyLIQTR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

