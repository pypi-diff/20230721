# Comparing `tmp/pyquafu-0.2.9-cp39-cp39-win_amd64.whl.zip` & `tmp/pyquafu-0.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,90 @@
-Zip file size: 155069 bytes, number of entries: 30
--rw-rw-rw-  2.0 fat      376 b- defN 22-Nov-30 04:01 quafu/__init__.py
--rw-rw-rw-  2.0 fat      606 b- defN 22-Nov-30 04:01 quafu/exceptions.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/backends/__init__.py
--rw-rw-rw-  2.0 fat     1441 b- defN 22-Nov-30 04:01 quafu/backends/backends.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/circuits/__init__.py
--rw-rw-rw-  2.0 fat      900 b- defN 22-Nov-30 04:01 quafu/circuits/para_circuit.py
--rw-rw-rw-  2.0 fat    26545 b- defN 22-Nov-30 04:01 quafu/circuits/quantum_circuit.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/elements/__init__.py
--rw-rw-rw-  2.0 fat     9370 b- defN 22-Nov-30 04:01 quafu/elements/element_gates.py
--rw-rw-rw-  2.0 fat     8702 b- defN 22-Nov-30 04:01 quafu/elements/quantum_element.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/results/__init__.py
--rw-rw-rw-  2.0 fat     6602 b- defN 22-Nov-30 04:01 quafu/results/results.py
--rw-rw-rw-  2.0 fat        1 b- defN 22-Nov-30 04:01 quafu/simulators/__init__.py
--rw-rw-rw-  2.0 fat     3690 b- defN 22-Nov-30 04:01 quafu/simulators/default_simulator.py
--rw-rw-rw-  2.0 fat   322560 b- defN 22-Nov-30 04:01 quafu/simulators/qfvm.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2875 b- defN 22-Nov-30 04:01 quafu/simulators/simulator.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/tasks/__init__.py
--rw-rw-rw-  2.0 fat    14319 b- defN 22-Nov-30 04:01 quafu/tasks/tasks.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/users/__init__.py
--rw-rw-rw-  2.0 fat       79 b- defN 22-Nov-30 04:01 quafu/users/exceptions.py
--rw-rw-rw-  2.0 fat      646 b- defN 22-Nov-30 04:01 quafu/users/userapi.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-30 04:01 quafu/utils/__init__.py
--rw-rw-rw-  2.0 fat     1020 b- defN 22-Nov-30 04:01 quafu/utils/basis.py
--rw-rw-rw-  2.0 fat     1234 b- defN 22-Nov-30 04:01 quafu/utils/paulis.py
--rw-rw-rw-  2.0 fat      244 b- defN 22-Nov-30 04:01 quafu/utils/platform.py
--rw-rw-rw-  2.0 fat    11556 b- defN 22-Nov-30 04:01 pyquafu-0.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1279 b- defN 22-Nov-30 04:01 pyquafu-0.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 22-Nov-30 04:01 pyquafu-0.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 22-Nov-30 04:01 pyquafu-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2434 b- defN 22-Nov-30 04:01 pyquafu-0.2.9.dist-info/RECORD
-30 files, 416579 bytes uncompressed, 151149 bytes compressed:  63.7%
+Zip file size: 303218 bytes, number of entries: 88
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 pyquafu-0.3.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 pyquafu.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/
+-rw-r--r--  2.0 unx    11556 b- defN 23-Jul-21 06:22 pyquafu-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2302 b- defN 23-Jul-21 06:22 pyquafu-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-21 06:22 pyquafu-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5994 b- defN 23-Jul-21 06:22 pyquafu-0.3.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-21 06:22 pyquafu-0.3.0.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx   168193 b- defN 23-Jul-21 06:22 pyquafu.libs/libgomp-a34b3233.so.1.0.0
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/tasks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/results/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/users/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/simulators/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/dagcircuits/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/circuits/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/elements/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/qfasm/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/backends/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/benchmark/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/exceptions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/visualisation/
+-rw-r--r--  2.0 unx      348 b- defN 23-Jul-21 06:22 quafu/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/tasks/__init__.py
+-rw-r--r--  2.0 unx    11143 b- defN 23-Jul-21 06:22 quafu/tasks/tasks.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/results/__init__.py
+-rw-r--r--  2.0 unx     6578 b- defN 23-Jul-21 06:22 quafu/results/results.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/users/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-21 06:22 quafu/users/exceptions.py
+-rw-r--r--  2.0 unx     2641 b- defN 23-Jul-21 06:22 quafu/users/userapi.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 06:22 quafu/simulators/__init__.py
+-rwxr-xr-x  2.0 unx   504369 b- defN 23-Jul-21 06:22 quafu/simulators/qfvm.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     3824 b- defN 23-Jul-21 06:22 quafu/simulators/simulator.py
+-rw-r--r--  2.0 unx     3725 b- defN 23-Jul-21 06:22 quafu/simulators/default_simulator.py
+-rw-r--r--  2.0 unx    15897 b- defN 23-Jul-21 06:22 quafu/dagcircuits/circuit_dag.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 06:22 quafu/dagcircuits/__init__.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Jul-21 06:22 quafu/dagcircuits/instruction_node.py
+-rw-r--r--  2.0 unx    11833 b- defN 23-Jul-21 06:22 quafu/dagcircuits/dag_circuit.py
+-rw-r--r--  2.0 unx      939 b- defN 23-Jul-21 06:22 quafu/circuits/para_circuit.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/circuits/__init__.py
+-rw-r--r--  2.0 unx    27017 b- defN 23-Jul-21 06:22 quafu/circuits/quantum_circuit.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/elements/element_gates/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/elements/quantum_element/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/elements/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/elements/element_gates/unitary/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/elements/element_gates/matrices/
+-rw-r--r--  2.0 unx      351 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/phase.py
+-rw-r--r--  2.0 unx      930 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/__init__.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/c21.py
+-rw-r--r--  2.0 unx     2683 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/pauli.py
+-rw-r--r--  2.0 unx     1361 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/cm1.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/c12.py
+-rw-r--r--  2.0 unx     1228 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/clifford.py
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/swap.py
+-rw-r--r--  2.0 unx     1626 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/c11.py
+-rw-r--r--  2.0 unx     1989 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/rotation.py
+-rw-r--r--  2.0 unx       43 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/unitary/__init__.py
+-rw-r--r--  2.0 unx    11341 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/unitary/decomposer.py
+-rw-r--r--  2.0 unx     5331 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/matrices/mat_lib.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/matrices/__init__.py
+-rw-r--r--  2.0 unx     3390 b- defN 23-Jul-21 06:22 quafu/elements/element_gates/matrices/mat_utils.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:22 quafu/elements/quantum_element/pulses/
+-rw-r--r--  2.0 unx      280 b- defN 23-Jul-21 06:22 quafu/elements/quantum_element/__init__.py
+-rw-r--r--  2.0 unx     2455 b- defN 23-Jul-21 06:22 quafu/elements/quantum_element/instruction.py
+-rw-r--r--  2.0 unx     6180 b- defN 23-Jul-21 06:22 quafu/elements/quantum_element/quantum_gate.py
+-rw-r--r--  2.0 unx     2676 b- defN 23-Jul-21 06:22 quafu/elements/quantum_element/quantum_element.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Jul-21 06:22 quafu/elements/quantum_element/pulses/__init__.py
+-rw-r--r--  2.0 unx     7221 b- defN 23-Jul-21 06:22 quafu/elements/quantum_element/pulses/quantum_pulse.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/qfasm/__init__.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-21 06:22 quafu/qfasm/qfasm_convertor.py
+-rw-r--r--  2.0 unx     2330 b- defN 23-Jul-21 06:22 quafu/qfasm/qfasmlex.py
+-rw-r--r--  2.0 unx     5812 b- defN 23-Jul-21 06:22 quafu/qfasm/qfasm_parser.py
+-rw-r--r--  2.0 unx      254 b- defN 23-Jul-21 06:22 quafu/utils/platform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/utils/__init__.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-Jul-21 06:22 quafu/utils/basis.py
+-rw-r--r--  2.0 unx     1234 b- defN 23-Jul-21 06:22 quafu/utils/paulis.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/backends/__init__.py
+-rw-r--r--  2.0 unx     4188 b- defN 23-Jul-21 06:22 quafu/backends/backends.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/benchmark/__init__.py
+-rw-r--r--  2.0 unx     1413 b- defN 23-Jul-21 06:22 quafu/benchmark/variational_n4.py
+-rw-r--r--  2.0 unx      255 b- defN 23-Jul-21 06:22 quafu/benchmark/unitary_test.py
+-rw-r--r--  2.0 unx     2035 b- defN 23-Jul-21 06:22 quafu/benchmark/deutsch_jozsa.py
+-rw-r--r--  2.0 unx     2572 b- defN 23-Jul-21 06:22 quafu/benchmark/adder.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jul-21 06:22 quafu/exceptions/quafu_error.py
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 06:22 quafu/exceptions/__init__.py
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-21 06:22 quafu/exceptions/circuit_error.py
+-rw-r--r--  2.0 unx    19215 b- defN 23-Jul-21 06:22 quafu/visualisation/circuitPlot.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:22 quafu/visualisation/__init__.py
+88 files, 871147 bytes uncompressed, 291260 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,91 +1,265 @@
-Filename: quafu/__init__.py
+Filename: pyquafu-0.3.0.dist-info/
 Comment: 
 
-Filename: quafu/exceptions.py
+Filename: pyquafu.libs/
 Comment: 
 
-Filename: quafu/backends/__init__.py
+Filename: quafu/
 Comment: 
 
-Filename: quafu/backends/backends.py
+Filename: pyquafu-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: quafu/circuits/__init__.py
+Filename: pyquafu-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: quafu/circuits/para_circuit.py
+Filename: pyquafu-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: quafu/circuits/quantum_circuit.py
+Filename: pyquafu-0.3.0.dist-info/RECORD
 Comment: 
 
-Filename: quafu/elements/__init__.py
+Filename: pyquafu-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: quafu/elements/element_gates.py
+Filename: pyquafu.libs/libgomp-a34b3233.so.1.0.0
 Comment: 
 
-Filename: quafu/elements/quantum_element.py
+Filename: quafu/tasks/
 Comment: 
 
-Filename: quafu/results/__init__.py
+Filename: quafu/results/
 Comment: 
 
-Filename: quafu/results/results.py
+Filename: quafu/users/
 Comment: 
 
-Filename: quafu/simulators/__init__.py
+Filename: quafu/simulators/
 Comment: 
 
-Filename: quafu/simulators/default_simulator.py
+Filename: quafu/dagcircuits/
 Comment: 
 
-Filename: quafu/simulators/qfvm.cp39-win_amd64.pyd
+Filename: quafu/circuits/
 Comment: 
 
-Filename: quafu/simulators/simulator.py
+Filename: quafu/elements/
+Comment: 
+
+Filename: quafu/qfasm/
+Comment: 
+
+Filename: quafu/utils/
+Comment: 
+
+Filename: quafu/backends/
+Comment: 
+
+Filename: quafu/benchmark/
+Comment: 
+
+Filename: quafu/exceptions/
+Comment: 
+
+Filename: quafu/visualisation/
+Comment: 
+
+Filename: quafu/__init__.py
 Comment: 
 
 Filename: quafu/tasks/__init__.py
 Comment: 
 
 Filename: quafu/tasks/tasks.py
 Comment: 
 
+Filename: quafu/results/__init__.py
+Comment: 
+
+Filename: quafu/results/results.py
+Comment: 
+
 Filename: quafu/users/__init__.py
 Comment: 
 
 Filename: quafu/users/exceptions.py
 Comment: 
 
 Filename: quafu/users/userapi.py
 Comment: 
 
+Filename: quafu/simulators/__init__.py
+Comment: 
+
+Filename: quafu/simulators/qfvm.cpython-38-x86_64-linux-gnu.so
+Comment: 
+
+Filename: quafu/simulators/simulator.py
+Comment: 
+
+Filename: quafu/simulators/default_simulator.py
+Comment: 
+
+Filename: quafu/dagcircuits/circuit_dag.py
+Comment: 
+
+Filename: quafu/dagcircuits/__init__.py
+Comment: 
+
+Filename: quafu/dagcircuits/instruction_node.py
+Comment: 
+
+Filename: quafu/dagcircuits/dag_circuit.py
+Comment: 
+
+Filename: quafu/circuits/para_circuit.py
+Comment: 
+
+Filename: quafu/circuits/__init__.py
+Comment: 
+
+Filename: quafu/circuits/quantum_circuit.py
+Comment: 
+
+Filename: quafu/elements/element_gates/
+Comment: 
+
+Filename: quafu/elements/quantum_element/
+Comment: 
+
+Filename: quafu/elements/__init__.py
+Comment: 
+
+Filename: quafu/elements/element_gates/unitary/
+Comment: 
+
+Filename: quafu/elements/element_gates/matrices/
+Comment: 
+
+Filename: quafu/elements/element_gates/phase.py
+Comment: 
+
+Filename: quafu/elements/element_gates/__init__.py
+Comment: 
+
+Filename: quafu/elements/element_gates/c21.py
+Comment: 
+
+Filename: quafu/elements/element_gates/pauli.py
+Comment: 
+
+Filename: quafu/elements/element_gates/cm1.py
+Comment: 
+
+Filename: quafu/elements/element_gates/c12.py
+Comment: 
+
+Filename: quafu/elements/element_gates/clifford.py
+Comment: 
+
+Filename: quafu/elements/element_gates/swap.py
+Comment: 
+
+Filename: quafu/elements/element_gates/c11.py
+Comment: 
+
+Filename: quafu/elements/element_gates/rotation.py
+Comment: 
+
+Filename: quafu/elements/element_gates/unitary/__init__.py
+Comment: 
+
+Filename: quafu/elements/element_gates/unitary/decomposer.py
+Comment: 
+
+Filename: quafu/elements/element_gates/matrices/mat_lib.py
+Comment: 
+
+Filename: quafu/elements/element_gates/matrices/__init__.py
+Comment: 
+
+Filename: quafu/elements/element_gates/matrices/mat_utils.py
+Comment: 
+
+Filename: quafu/elements/quantum_element/pulses/
+Comment: 
+
+Filename: quafu/elements/quantum_element/__init__.py
+Comment: 
+
+Filename: quafu/elements/quantum_element/instruction.py
+Comment: 
+
+Filename: quafu/elements/quantum_element/quantum_gate.py
+Comment: 
+
+Filename: quafu/elements/quantum_element/quantum_element.py
+Comment: 
+
+Filename: quafu/elements/quantum_element/pulses/__init__.py
+Comment: 
+
+Filename: quafu/elements/quantum_element/pulses/quantum_pulse.py
+Comment: 
+
+Filename: quafu/qfasm/__init__.py
+Comment: 
+
+Filename: quafu/qfasm/qfasm_convertor.py
+Comment: 
+
+Filename: quafu/qfasm/qfasmlex.py
+Comment: 
+
+Filename: quafu/qfasm/qfasm_parser.py
+Comment: 
+
+Filename: quafu/utils/platform.py
+Comment: 
+
 Filename: quafu/utils/__init__.py
 Comment: 
 
 Filename: quafu/utils/basis.py
 Comment: 
 
 Filename: quafu/utils/paulis.py
 Comment: 
 
-Filename: quafu/utils/platform.py
+Filename: quafu/backends/__init__.py
+Comment: 
+
+Filename: quafu/backends/backends.py
+Comment: 
+
+Filename: quafu/benchmark/__init__.py
+Comment: 
+
+Filename: quafu/benchmark/variational_n4.py
+Comment: 
+
+Filename: quafu/benchmark/unitary_test.py
+Comment: 
+
+Filename: quafu/benchmark/deutsch_jozsa.py
+Comment: 
+
+Filename: quafu/benchmark/adder.py
 Comment: 
 
-Filename: pyquafu-0.2.9.dist-info/LICENSE
+Filename: quafu/exceptions/quafu_error.py
 Comment: 
 
-Filename: pyquafu-0.2.9.dist-info/METADATA
+Filename: quafu/exceptions/__init__.py
 Comment: 
 
-Filename: pyquafu-0.2.9.dist-info/WHEEL
+Filename: quafu/exceptions/circuit_error.py
 Comment: 
 
-Filename: pyquafu-0.2.9.dist-info/top_level.txt
+Filename: quafu/visualisation/circuitPlot.py
 Comment: 
 
-Filename: pyquafu-0.2.9.dist-info/RECORD
+Filename: quafu/visualisation/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## quafu/__init__.py

```diff
@@ -1,11 +1,11 @@
 from .circuits.quantum_circuit import QuantumCircuit
-from .results.results import ExecResult, SimuResult 
+from .results.results import ExecResult, SimuResult
 from .tasks.tasks import Task
 from .users.userapi import User
 from .simulators.simulator import simulate
 
 __all__ = ["QuantumCircuit", "ExecResult", "Task", "User", "SimuResult", "simulate"]
 
+
 def get_version():
-    print ("version: 0.2.9\n")
-    return "0.2.9"
+    return "0.2.11"
```

## quafu/backends/backends.py

```diff
@@ -1,43 +1,96 @@
 import requests
 import json
 import re
 import networkx as nx
+import numpy as np
+import matplotlib.pyplot as plt
+from quafu.users.userapi import User
+
 
 class Backend(object):
-    def __init__(self, name):
-        self.name = name
-        self.valid_gates = []
-        
-    def get_info(self, url, api_token):
+    def __init__(self, backend_info: dict):
+        self.name = backend_info['system_name']
+        self._valid_gates = backend_info['valid_gates']
+        self.qubit_num = backend_info['qubits']
+        self.system_id = backend_info['system_id']
+        self.status = backend_info['status']
+        self.qv = backend_info["QV"]
+        # self.task_in_queue = backend_info["task_in_queue"]
+
+    def get_chip_info(self, user=User()):
+        api_token = user.apitoken
+        url = user._url
         data = {"system_name": self.name.lower()}
-        headers={"api_token": api_token}
-        chip_info = requests.post(url = url + "qbackend/scq_get_chip_info/", data=data, 
-        headers=headers)
-        backend_info = json.loads(chip_info.text)
-       
-        return backend_info
+        headers = {"api_token": api_token}
+        chip_info = requests.post(url=url + user.chip_api, data=data,
+                                  headers=headers)
+        chip_info = json.loads(chip_info.text)
+        json_topo_struct = chip_info["topological_structure"]
+        qubits_list = []
+        for gate in json_topo_struct.keys():
+            qubit = gate.split('_')
+            qubits_list.append(qubit[0])
+            qubits_list.append(qubit[1])
+        qubits_list = list(set(qubits_list))
+        qubits_list = sorted(qubits_list, key=lambda x: int(re.findall(r"\d+", x)[0]))
+        int_to_qubit = {k: v for k, v in enumerate(qubits_list)}
+        qubit_to_int = {v: k for k, v in enumerate(qubits_list)}
+
+        directed_weighted_edges = []
+        weighted_edges = []
+        edges_dict = {}
+        clist = []
+        for gate, name_fidelity in json_topo_struct.items():
+            gate_qubit = gate.split('_')
+            qubit1 = qubit_to_int[gate_qubit[0]]
+            qubit2 = qubit_to_int[gate_qubit[1]]
+            gate_name = list(name_fidelity.keys())[0]
+            fidelity = name_fidelity[gate_name]['fidelity']
+            directed_weighted_edges.append([qubit1, qubit2, fidelity])
+            clist.append([qubit1, qubit2])
+            gate_reverse = gate.split('_')[1] + '_' + gate.split('_')[0]
+            if gate not in edges_dict and gate_reverse not in edges_dict:
+                edges_dict[gate] = fidelity
+            else:
+                if fidelity < edges_dict[gate_reverse]:
+                    edges_dict.pop(gate_reverse)
+                    edges_dict[gate] = fidelity
+
+        for gate, fidelity in edges_dict.items():
+            gate_qubit = gate.split('_')
+            qubit1, qubit2 = qubit_to_int[gate_qubit[0]], qubit_to_int[gate_qubit[1]]
+            weighted_edges.append([qubit1, qubit2, np.round(fidelity, 3)])
+
+        # draw topology
+
+        G = nx.Graph()
+        for key, value in int_to_qubit.items():
+            G.add_node(key, name=value)
+
+        G.add_weighted_edges_from(weighted_edges)
+
+        elarge = [(u, v) for (u, v, d) in G.edges(data=True) if d["weight"] >= 0.9]
+        esmall = [(u, v) for (u, v, d) in G.edges(data=True) if d["weight"] < 0.9]
+        elarge_labels = {(u, v): "%.3f" % d["weight"] for (u, v, d) in G.edges(data=True) if d["weight"] >= 0.9}
+        esmall_labels = {(u, v): "%.3f" % d["weight"] for (u, v, d) in G.edges(data=True) if d["weight"] < 0.9}
+
+        pos = nx.spring_layout(G, seed=1)
+        fig, ax = plt.subplots()
+        nx.draw_networkx_nodes(G, pos, node_size=400, ax=ax)
+
+        nx.draw_networkx_edges(G, pos, edgelist=elarge, width=2, ax=ax)
+        nx.draw_networkx_edges(
+            G, pos, edgelist=esmall, width=2, alpha=0.5, style="dashed"
+            , ax=ax)
+
+        nx.draw_networkx_labels(G, pos, font_size=14, font_family="sans-serif", ax=ax)
+        edge_labels = nx.get_edge_attributes(G, "weight")
+        nx.draw_networkx_edge_labels(G, pos, elarge_labels, font_size=12, font_color="green", ax=ax)
+        nx.draw_networkx_edge_labels(G, pos, esmall_labels, font_size=12, font_color="red", ax=ax)
+        fig.set_figwidth(14)
+        fig.set_figheight(14)
+        fig.tight_layout()
+        return {"mapping": int_to_qubit, "topology_diagram": fig, "full_info": chip_info}
 
     def get_valid_gates(self):
-        return self.valid_gates
-
-
-class ScQ_P10(Backend):
-    def __init__(self):
-        super().__init__("ScQ-P10")
-        self.valid_gates = ["cx", "cz", "rx", "ry", "rz", "x", "y", "z", "h", "sx", "sy", "id", "delay", "barrier", "cy", "cnot", "swap"]
-
-class ScQ_P20(Backend):
-    def __init__(self):
-        super().__init__("ScQ-P20")
-        self.valid_gates = ["cx", "cz", "rx", "ry", "rz", "x", "y", "z", "h", "sx", "sy", "id", "delay", "barrier", "cy", "cnot", "swap"]
-        
-class ScQ_P50(Backend):
-    def __init__(self):
-        super().__init__("ScQ-P50")
-        self.valid_gates = ["cx", "cz", "rx", "ry", "rz", "x", "y", "z", "h"]
-
-class ScQ_S41(Backend):
-    def __init__(self):
-        super().__init__("ScQ-S41")
-        self.valid_gates = [ "rx", "ry", "rz", "x", "y", "z", "h", "sx", "sy", "id", "delay", "barrier", "xy"]
-            
+        return self._valid_gates
```

## quafu/circuits/para_circuit.py

```diff
@@ -1,12 +1,11 @@
-
-
 from .quantum_circuit import QuantumCircuit
 from ..transpiler.Qcovercompiler import QcoverCompiler
 
+
 class QAOACircuit(QuantumCircuit):
     def __init__(self, logical_qubits, physical_qubits, nodes, edges, params, p, gate="CNOT"):
         num = logical_qubits
         self.logical_qubits = logical_qubits
         self.physical_qubits = physical_qubits
         self.nodes = nodes
         self.edges = edges
@@ -16,16 +15,13 @@
         super().__init__(num)
 
     def compile_to_IOP(self):
         """
         QASM from qcover directly
         """
         qaoa_compiler = QcoverCompiler()
-        self.qasm = qaoa_compiler.graph_to_qasm(self.logical_qubits, self.physical_qubits, self.nodes, self.edges, self.paras, self.p, gate=self.gate)
+        self.qasm = qaoa_compiler.graph_to_qasm(self.logical_qubits, self.physical_qubits, self.nodes, self.edges,
+                                                self.paras, self.p, gate=self.gate)
 
     def upate_paras(self, paras):
         self.paras = paras
         pass
-
-
-
-
```

## quafu/circuits/quantum_circuit.py

```diff
@@ -1,49 +1,58 @@
-from typing import Iterable
+from typing import List
 import numpy as np
-from ..elements.quantum_element import Barrier, Delay, ControlledGate, MultiQubitGate, ParaMultiQubitGate, QuantumGate, SingleQubitGate, XYResonance
-from ..elements.element_gates import *
+
+import quafu.elements.element_gates.clifford
+import quafu.elements.element_gates.pauli
+from quafu.elements.quantum_element.pulses.quantum_pulse import QuantumPulse
+from ..elements.quantum_element import Barrier, Delay, MultiQubitGate, QuantumGate, ControlledGate, \
+    SingleQubitGate, XYResonance
+import quafu.elements.element_gates as qeg
 from ..exceptions import CircuitError
 
+
 class QuantumCircuit(object):
     def __init__(self, num: int):
         """
         Initialize a QuantumCircuit object
-        
-        Args:   
+
+        Args:
             num (int): Total qubit number used
         """
         self.num = num
         self.gates = []
         self.openqasm = ""
         self.circuit = []
-        self.measures = dict(zip(range(num), range(num)))
+        self.measures = {}
         self._used_qubits = []
 
     @property
     def used_qubits(self) -> List:
         self.layered_circuit()
         return self._used_qubits
 
-    def add_gate(self, gate : QuantumGate):
+    def add_gate(self, gate: QuantumGate):
+        pos = np.array(gate.pos)
+        if np.any(pos >= self.num):
+            raise CircuitError(f"Gate position out of range: {gate.pos}")
         self.gates.append(gate)
 
     def layered_circuit(self) -> np.ndarray:
         """
         Make layered circuit from the gate sequence self.gates.
 
-        Returns: 
+        Returns:
             A layered list with left justed circuit.
         """
         num = self.num
         gatelist = self.gates
         gateQlist = [[] for i in range(num)]
         used_qubits = []
         for gate in gatelist:
-            if isinstance(gate, SingleQubitGate) or isinstance(gate, Delay):
+            if isinstance(gate, SingleQubitGate) or isinstance(gate, Delay) or isinstance(gate, QuantumPulse):
                 gateQlist[gate.pos].append(gate)
                 if gate.pos not in used_qubits:
                     used_qubits.append(gate.pos)
 
             elif isinstance(gate, Barrier) or isinstance(gate, MultiQubitGate) or isinstance(gate, XYResonance):
                 pos1 = min(gate.pos)
                 pos2 = max(gate.pos)
@@ -82,78 +91,78 @@
 
         lc = np.array(new_gateQlist)
         lc = np.vstack((used_qubits, lc.T)).T
         self.circuit = lc
         self._used_qubits = list(used_qubits)
         return self.circuit
 
-    def draw_circuit(self, width : int=4):
+    def draw_circuit(self, width: int = 4, return_str: bool = False):
         """
         Draw layered circuit using ASCII, print in terminal.
 
         Args:
-            width (int): The width of each gate. s
+            width (int): The width of each gate.
+            return_str: Whether return the circuit string.
         """
         self.layered_circuit()
         gateQlist = self.circuit
         num = gateQlist.shape[0]
         depth = gateQlist.shape[1] - 1
         printlist = np.array([[""] * depth for i in range(2 * num)], dtype="<U30")
 
         reduce_map = dict(zip(gateQlist[:, 0], range(num)))
         reduce_map_inv = dict(zip(range(num), gateQlist[:, 0]))
         for l in range(depth):
             layergates = gateQlist[:, l + 1]
             maxlen = 1 + width
             for i in range(num):
                 gate = layergates[i]
-                if isinstance(gate, SingleQubitGate) or isinstance(gate, Delay):
+                if isinstance(gate, SingleQubitGate) or isinstance(gate, Delay) or (isinstance(gate, QuantumPulse)):
                     printlist[i * 2, l] = gate.symbol
                     maxlen = max(maxlen, len(gate.symbol) + width)
 
                 elif isinstance(gate, MultiQubitGate) or isinstance(gate, XYResonance):
                     q1 = reduce_map[min(gate.pos)]
                     q2 = reduce_map[max(gate.pos)]
                     printlist[2 * q1 + 1:2 * q2, l] = "|"
                     printlist[q1 * 2, l] = "#"
                     printlist[q2 * 2, l] = "#"
-                    if isinstance(gate, ControlledGate): #Controlled-Multiqubit gate
+                    if isinstance(gate, ControlledGate):  # Controlled-Multiqubit gate
                         for ctrl in gate.ctrls:
                             printlist[reduce_map[ctrl] * 2, l] = "*"
-                        
+
                         if gate.targ_name == "SWAP":
                             printlist[reduce_map[gate.targs[0]] * 2, l] = "x"
                             printlist[reduce_map[gate.targs[1]] * 2, l] = "x"
                         else:
                             tq1 = reduce_map[min(gate.targs)]
                             tq2 = reduce_map[max(gate.targs)]
                             printlist[tq1 * 2, l] = "#"
                             printlist[tq2 * 2, l] = "#"
                             if tq1 + tq2 in [reduce_map[ctrl] * 2 for ctrl in gate.ctrls]:
                                 printlist[tq1 + tq2, l] = "*" + gate.symbol
                             else:
                                 printlist[tq1 + tq2, l] = gate.symbol
                             maxlen = max(maxlen, len(gate.symbol) + width)
-                                
-                    else: #Multiqubit gate
+
+                    else:  # Multiqubit gate
                         if gate.name == "SWAP":
                             printlist[q1 * 2, l] = "x"
                             printlist[q2 * 2, l] = "x"
 
                         else:
                             printlist[q1 + q2, l] = gate.symbol
                             maxlen = max(maxlen, len(gate.symbol) + width)
 
                 elif isinstance(gate, Barrier):
                     pos = [i for i in gate.pos if i in reduce_map.keys()]
                     q1 = reduce_map[min(pos)]
                     q2 = reduce_map[max(pos)]
                     printlist[2 * q1:2 * q2 + 1, l] = "||"
                     maxlen = max(maxlen, len("||"))
-                
 
             printlist[-1, l] = maxlen
 
         circuitstr = []
         for j in range(2 * num - 1):
             if j % 2 == 0:
                 linestr = ("q[%d]" % (reduce_map_inv[j // 2])).ljust(6) + "".join(
@@ -161,18 +170,26 @@
                 if reduce_map_inv[j // 2] in self.measures.keys():
                     linestr += " M->c[%d]" % self.measures[reduce_map_inv[j // 2]]
                 circuitstr.append(linestr)
             else:
                 circuitstr.append("".ljust(6) + "".join(
                     [printlist[j, l].center(int(printlist[-1, l]), " ") for l in range(depth)]))
         circuitstr = "\n".join(circuitstr)
-        print(circuitstr)
-        return circuitstr
 
-    def from_openqasm(self, openqasm : str):
+        if return_str:
+            return circuitstr
+        else:
+            print(circuitstr)
+
+    def plot_circuit(self, *args, **kwargs):
+        from quafu.visualisation.circuitPlot import CircuitPlotManager
+        cmp = CircuitPlotManager(self)
+        return cmp(*args, **kwargs)
+
+    def from_openqasm(self, openqasm: str):
         """
         Initialize the circuit from openqasm text.
         Args:
             openqasm: input openqasm str.
         """
         from numpy import pi
         import re
@@ -302,438 +319,476 @@
         if not global_valid:
             print("Warning: All operations after measurement will be removed for executing on experiment")
 
     def to_openqasm(self) -> str:
         """
         Convert the circuit to openqasm text.
 
-        Returns: 
+        Returns:
             openqasm text.
         """
         qasm = "OPENQASM 2.0;\ninclude \"qelib1.inc\";\n"
         qasm += "qreg q[%d];\n" % self.num
         qasm += "creg meas[%d];\n" % len(self.measures)
         for gate in self.gates:
-            if isinstance(gate, SingleQubitGate):
-                if isinstance(gate, ParaSingleQubitGate):
-                    if isinstance(gate.paras, Iterable):
-                        qasm += "%s(" %gate.name.lower() + ",".join(["%s" %para for para in gate.paras]) + ") q[%d];\n" % (gate.pos)
-                    else:
-                        qasm += "%s(%s) " %(gate.name.lower(), gate.paras) + "q[%d];\n" % (gate.pos)
-                else:
-                    if gate.name == "SY":
-                        qasm += "ry(pi/2) q[%d];\n" %(gate.pos)
-                    elif gate.name == "W":
-                        qasm += "rz(-pi/4) q[%d];\nrx(pi) q[%d];\nrz(pi/4) q[%d];\n"  %(gate.pos, gate.pos, gate.pos)
-                    elif gate.name == "SW":
-                        qasm += "rz(-pi/4) q[%d];\nrx(pi/2) q[%d];\nrz(pi/4) q[%d];\n"  %(gate.pos, gate.pos, gate.pos)
-                    else:
-                        qasm += "%s q[%d];\n" % (gate.name.lower(), gate.pos)
-
-            elif isinstance(gate, Delay):
-                qasm += "delay(%d%s) q[%d];\n" % (gate.duration, gate.unit, gate.pos)
-            elif isinstance(gate, XYResonance):
-                qasm += "xy(%d%s) " %(gate.duration, gate.unit) + ",".join(["q[%d]" % p for p in range(min(gate.pos), max(gate.pos)+1)]) + ";\n"
-                
-            elif isinstance(gate, Barrier) or isinstance(gate, MultiQubitGate):
-                if isinstance(gate, ParaMultiQubitGate) or (isinstance(gate, ControlledGate) and bool(gate.paras)):
-                    if isinstance(gate.paras, Iterable):
-                        qasm += "%s(" %gate.name.lower() + ",".join(["%s" %para for para in gate.paras]) + ") " + ",".join(["q[%d]" % p for p in gate.pos]) + ";\n"
-                    else:
-                         qasm += "%s(%s) " %(gate.name.lower(), gate.paras) + ",".join(["q[%d]" % p for p in gate.pos]) + ";\n"
-                
-                else:
-                    if gate.name == "CS":
-                        qasm += "cp(pi/2) " + "q[%d],q[%d];\n" % (gate.pos[0], gate.pos[1])
-                    elif gate.name == "CT":
-                        qasm += "cp(pi/4) " + "q[%d],q[%d];\n" % (gate.pos[0], gate.pos[1])
-                    elif gate.name == "barrier":
-                        qasm += "barrier " + ",".join(["q[%d]" % p for p in range(min(gate.pos), max(gate.pos)+1)]) + ";\n"
-                    else:
-                        qasm += "%s " %(gate.name.lower()) + ",".join(["q[%d]" % p for p in gate.pos]) + ";\n"
+            qasm += gate.to_qasm() + ";\n"
 
         for key in self.measures:
             qasm += "measure q[%d] -> meas[%d];\n" % (key, self.measures[key])
 
         self.openqasm = qasm
         return qasm
 
-
     def id(self, pos: int) -> "QuantumCircuit":
         """
         Identity gate.
 
         Args:
             pos (int): qubit the gate act.
-        """ 
-        self.gates.append(IdGate(pos))
+        """
+        gate = qeg.IdGate(pos)
+        self.add_gate(gate)
         return self
 
     def h(self, pos: int) -> "QuantumCircuit":
         """
         Hadamard gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(HGate(pos))
+        gate = quafu.elements.element_gates.clifford.HGate(pos)
+        self.add_gate(gate)
         return self
 
     def x(self, pos: int) -> "QuantumCircuit":
         """
         X gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(XGate(pos))
+        gate = qeg.XGate(pos)
+        self.add_gate(gate)
         return self
 
     def y(self, pos: int) -> "QuantumCircuit":
         """
         Y gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(YGate(pos))
+        gate = qeg.YGate(pos)
+        self.add_gate(gate)
         return self
 
     def z(self, pos: int) -> "QuantumCircuit":
         """
         Z gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(ZGate(pos))
+        self.add_gate(qeg.ZGate(pos))
         return self
 
     def t(self, pos: int) -> "QuantumCircuit":
         """
         T gate. (~Z^(1/4))
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(TGate(pos))
+        self.add_gate(quafu.elements.element_gates.clifford.TGate(pos))
         return self
-    
+
     def tdg(self, pos: int) -> "QuantumCircuit":
         """
         Tdg gate. (Inverse of T gate)
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(TdgGate(pos))
+        self.add_gate(quafu.elements.element_gates.clifford.TdgGate(pos))
+        return self
 
     def s(self, pos: int) -> "QuantumCircuit":
         """
         S gate. (~√Z)
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(SGate(pos))
+        self.add_gate(quafu.elements.element_gates.clifford.SGate(pos))
         return self
 
     def sdg(self, pos: int) -> "QuantumCircuit":
         """
         Sdg gate. (Inverse of S gate)
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(SdgGate(pos))
+        self.add_gate(quafu.elements.element_gates.clifford.SdgGate(pos))
         return self
 
     def sx(self, pos: int) -> "QuantumCircuit":
         """
         √X gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(SXGate(pos))
+        self.add_gate(quafu.elements.element_gates.pauli.SXGate(pos))
+        return self
+
+    def sxdg(self, pos: int) -> "QuantumCircuit":
+        """
+        Inverse of √X gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = quafu.elements.element_gates.pauli.SXdgGate(pos)
+        self.add_gate(gate)
         return self
 
     def sy(self, pos: int) -> "QuantumCircuit":
         """
         √Y gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(SYGate(pos))
+        self.add_gate(quafu.elements.element_gates.pauli.SYGate(pos))
+        return self
+
+    def sydg(self, pos: int) -> "QuantumCircuit":
+        """
+        Inverse of √Y gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = quafu.elements.element_gates.pauli.SYdgGate(pos)
+        self.add_gate(gate)
         return self
 
     def w(self, pos: int) -> "QuantumCircuit":
         """
         W gate. (~(X + Y)/√2)
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(WGate(pos))
+        self.add_gate(qeg.WGate(pos))
         return self
-    
+
     def sw(self, pos: int) -> "QuantumCircuit":
         """
         √W gate.
 
         Args:
             pos (int): qubit the gate act.
         """
-        self.gates.append(SWGate(pos))
+        self.add_gate(qeg.SWGate(pos))
         return self
-    
+
     def rx(self, pos: int, para: float) -> "QuantumCircuit":
         """
         Single qubit rotation Rx gate.
 
         Args:
             pos (int): qubit the gate act.
             para (float): rotation angle
         """
-        self.gates.append(RXGate(pos, para))
+        self.add_gate(qeg.RXGate(pos, para))
         return self
 
     def ry(self, pos: int, para: float) -> "QuantumCircuit":
         """
         Single qubit rotation Ry gate.
-        
+
         Args:
             pos (int): qubit the gate act.
             para (float): rotation angle
         """
-        self.gates.append(RYGate(pos, para))
+        self.add_gate(qeg.RYGate(pos, para))
         return self
 
     def rz(self, pos: int, para: float) -> "QuantumCircuit":
         """
         Single qubit rotation Rz gate.
-        
+
         Args:
             pos (int): qubit the gate act.
             para (float): rotation angle
         """
-        self.gates.append(RZGate(pos, para))
+        self.add_gate(qeg.RZGate(pos, para))
         return self
 
     def p(self, pos: int, para: float) -> "QuantumCircuit":
         """
         Phase gate
-        
+
         Args:
             pos (int): qubit the gate act.
             para (float): rotation angle
         """
-        self.gates.append(PhaseGate(pos, para))
+        self.add_gate(qeg.PhaseGate(pos, para))
+        return self
 
     def cnot(self, ctrl: int, tar: int) -> "QuantumCircuit":
         """
         CNOT gate.
-        
+
         Args:
             ctrl (int): control qubit.
             tar (int): target qubit.
         """
-        self.gates.append(CXGate(ctrl, tar))
+        self.add_gate(qeg.CXGate(ctrl, tar))
         return self
 
+    def cx(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        return self.cnot(ctrl=ctrl, tar=tar)
+
     def cy(self, ctrl: int, tar: int) -> "QuantumCircuit":
         """
         Control-Y gate.
 
         Args:
             ctrl (int): control qubit.
             tar (int): target qubit.
         """
-        self.gates.append(CYGate(ctrl, tar))
+        self.add_gate(qeg.CYGate(ctrl, tar))
         return self
 
     def cz(self, ctrl: int, tar: int) -> "QuantumCircuit":
         """
         Control-Z gate.
-        
+
         Args:
             ctrl (int): control qubit.
             tar (int): target qubit.
         """
-        self.gates.append(CZGate(ctrl, tar))
+        self.add_gate(qeg.CZGate(ctrl, tar))
         return self
 
     def cs(self, ctrl: int, tar: int) -> "QuantumCircuit":
         """
         Control-S gate.
         Args:
             ctrl (int): control qubit.
             tar (int): target qubit.
         """
-        self.gates.append(CSGate(ctrl, tar))
+        self.add_gate(qeg.CSGate(ctrl, tar))
         return self
 
     def ct(self, ctrl: int, tar: int) -> "QuantumCircuit":
         """
         Control-T gate.
         Args:
             ctrl (int): control qubit.
             tar (int): target qubit.
         """
-        
-        self.gates.append(CTGate(ctrl, tar))
+
+        self.add_gate(qeg.CTGate(ctrl, tar))
         return self
 
     def cp(self, ctrl: int, tar: int, para) -> "QuantumCircuit":
         """
         Control-P gate.
 
         Args:
             ctrl (int): control qubit.
             tar (int): target qubit.
         """
-        self.gates.append(CPGate(ctrl, tar, para))
+        self.add_gate(qeg.CPGate(ctrl, tar, para))
         return self
-  
 
     def swap(self, q1: int, q2: int) -> "QuantumCircuit":
         """
         SWAP gate
-        
+
+        Args:
+            q1 (int): qubit the gate act.
+            q2 (int): qubit the gate act.
+        """
+        self.add_gate(qeg.SwapGate(q1, q2))
+        return self
+
+    def iswap(self, q1: int, q2: int) -> "QuantumCircuit":
+        """
+        iSWAP gate
+
         Args:
             q1 (int): qubit the gate act.
             q2 (int): qubit the gate act.
         """
-        self.gates.append(SwapGate(q1, q2))
+        self.add_gate(qeg.ISwapGate(q1, q2))
         return self
 
     def toffoli(self, ctrl1: int, ctrl2: int, targ: int) -> "QuantumCircuit":
         """
         Toffoli gate
 
         Args:
             ctrl1 (int): control qubit
             ctrl2 (int): control qubit
             targ (int): target qubit
         """
-        self.gates.append(ToffoliGate(ctrl1, ctrl2, targ))
+        self.add_gate(qeg.ToffoliGate(ctrl1, ctrl2, targ))
         return self
-    
-    def fredkin(self, ctrl: int, targ1:int , targ2: int) -> "QuantumCircuit":
+
+    def fredkin(self, ctrl: int, targ1: int, targ2: int) -> "QuantumCircuit":
         """
         Fredkin gate
-        
+
         Args:
             ctrl (int):  control qubit
             targ1 (int): target qubit
             targ2 (int): target qubit
         """
-        self.gates.append(FredkinGate(ctrl, targ1, targ2))
+        self.add_gate(qeg.FredkinGate(ctrl, targ1, targ2))
         return self
 
-    def barrier(self, qlist: List[int]) -> "QuantumCircuit":
+    def barrier(self, qlist: List[int] = None) -> "QuantumCircuit":
         """
         Add barrier for qubits in qlist.
-        
+
         Args:
             qlist (list[int]): A list contain the qubit need add barrier. When qlist contain at least two qubit, the barrier will be added from minimum qubit to maximum qubit. For example: barrier([0, 2]) create barrier for qubits 0, 1, 2. To create discrete barrier, using barrier([0]), barrier([2]).
         """
-        self.gates.append(Barrier(qlist))
+        if qlist is None:
+            qlist = list(range(self.num))
+        self.add_gate(Barrier(qlist))
         return self
 
     def delay(self, pos, duration, unit="ns") -> "QuantumCircuit":
         """
         Let the qubit idle for a certain duration.
 
         Args:
             pos (int): qubit need delay.
             duration (int): duration of qubit delay, which represents integer times of unit.
-            unit (str): time unit for the duration. Can be "ns" and "us". 
+            unit (str): time unit for the duration. Can be "ns" and "us".
         """
-        self.gates.append(Delay(pos, duration, unit=unit))
+        self.add_gate(Delay(pos, duration, unit=unit))
         return self
 
-    def xy(self, qs: int, qe: int, duration: int, unit: str="ns") -> "QuantumCircuit":
+    def xy(self, qs: int, qe: int, duration: int, unit: str = "ns") -> "QuantumCircuit":
         """
         XY resonance time evolution for quantum simulator
         Args:
             qs: start position of resonant qubits.
             qe: end position of resonant qubits.
             duration: duration must be integer, which represents integer times of unit.
             unit: time unit of duration.
 
         """
-        self.gates.append(XYResonance(qs, qe, duration, unit=unit))
+        self.add_gate(XYResonance(qs, qe, duration, unit=unit))
         return self
 
     def rxx(self, q1: int, q2: int, theta):
         """
         Rotation about 2-qubit XX axis.
         Args:
             q1 (int): qubit the gate act.
             q2 (int): qubit the gate act.
             theta: rotation angle.
 
         """
-        self.gates.append(RXXGate(q1, q2, theta))
-    
+        self.add_gate(qeg.RXXGate(q1, q2, theta))
+
     def ryy(self, q1: int, q2: int, theta):
         """
         Rotation about 2-qubit YY axis.
         Args:
             q1 (int): qubit the gate act.
             q2 (int): qubit the gate act.
             theta: rotation angle.
 
         """
-        self.gates.append(RYYGate(q1, q2, theta))
+        self.add_gate(qeg.RYYGate(q1, q2, theta))
 
     def rzz(self, q1: int, q2: int, theta):
         """
         Rotation about 2-qubit ZZ axis.
         Args:
             q1 (int): qubit the gate act.
             q2 (int): qubit the gate act.
             theta: rotation angle.
 
         """
-        self.gates.append(RZZGate(q1, q2, theta))
-    
+        self.add_gate(qeg.RZZGate(q1, q2, theta))
+
     def mcx(self, ctrls: List[int], targ: int):
         """
         Multi-controlled X gate.
+        Args:
+            ctrls: A list of control qubits.
+            targ: Target qubits.
         """
-        self.gates.append(MCXGate(ctrls, targ))
-    
+        self.add_gate(qeg.MCXGate(ctrls, targ))
+
     def mcy(self, ctrls: List[int], targ: int):
         """
-        Multi-controlled X gate.
+        Multi-controlled Y gate.
+        Args:
+            ctrls: A list of control qubits.
+            targ: Target qubits.
         """
-        self.gates.append(MCYGate(ctrls, targ))
-    
+        self.add_gate(qeg.MCYGate(ctrls, targ))
+
     def mcz(self, ctrls: List[int], targ: int):
         """
-        Multi-controlled X gate.
+        Multi-controlled Z gate.
+        Args:
+            ctrls: A list of control qubits.
+            targ: Target qubits.
+        """
+        self.add_gate(qeg.MCZGate(ctrls, targ))
+
+    def unitary(self, matrix: np.ndarray, pos: List[int]):
         """
-        self.gates.append(MCZGate(ctrls, targ))
-    
+        Apply unitary to circuit on specified qubits.
 
-    def measure(self, pos: List[int], cbits: List[int] = []) -> None:
+        Args:
+            matrix (np.ndarray): unitary matrix.
+            pos (list[int]): qubits the gate act on.
+        """
+        compiler = qeg.UnitaryDecomposer(array=matrix, qubits=pos)
+        compiler.apply_to_qc(self)
+
+    def measure(self, pos: List[int] = None, cbits: List[int] = None) -> None:
         """
         Measurement setting for experiment device.
-        
+
         Args:
             pos: Qubits need measure.
             cbits: Classical bits keeping the measure results.
         """
-
-        self.measures = dict(zip(pos, range(len(pos))))
+        if pos is None:
+            pos = list(range(self.num))
 
         if cbits:
-            if len(cbits) == len(self.measures):
-                self.measures = dict(zip(pos, cbits))
-            else:
+            if not len(cbits) == len(pos):
                 raise CircuitError("Number of measured bits should equal to the number of classical bits")
+        else:
+            cbits = pos
 
-
-
+        newly_measures = dict(zip(pos, cbits))
+        self.measures = {**self.measures, **newly_measures}
+        if not len(self.measures.values()) == len(set(self.measures.values())):
+            raise ValueError("Measured bits not uniquely assigned.")
+
+    def add_pulse(self,
+                  pulse: QuantumPulse,
+                  pos: int = None) -> "QuantumCircuit":
+        """
+        Add quantum gate from pulse.
+        """
+        if pos is not None:
+            pulse.set_pos(pos)
+        self.add_gate(pulse)
+        return self
```

## quafu/results/results.py

```diff
@@ -1,179 +1,179 @@
-
-import numpy as np
-from functools import reduce
 import copy
-import matplotlib.pyplot as plt
 from collections import OrderedDict
+
+import matplotlib.pyplot as plt
 from ..utils.basis import *
 
+
 class Result(object):
     """Basis class for quantum results"""
-    pass  
+    pass
+
 
 class ExecResult(Result):
     """ 
     Class that save the execute results returned from backend.
     
     Attributes:
         counts (dict): Samples counts on each bitstring.
-        amplitudes (dict): Calculated amplitudes on each bitstring.
+        probabilities (dict): Calculated probabilities on each bitstring.
         taskid (int): Unique task id for the execute result.
         transpiled_circuit (QuantumCircuit): Quantum circuit transpiled on backend.
     """
+
     def __init__(self, input_dict, measures):
-        status_map = {0:"In Queue", 1:"Running", 2:"Completed", "Canceled":3, 4:"Failed"}
+        status_map = {0: "In Queue", 1: "Running", 2: "Completed", "Canceled": 3, 4: "Failed"}
         self.measures = measures
         self.task_status = status_map[input_dict["status"]]
         self.res = eval(input_dict['res'])
         self.counts = OrderedDict(sorted(self.res.items(), key=lambda s: s[0]))
         self.logicalq_res = {}
         cbits = list(self.measures.values())
         for key, values in self.counts.items():
-           newkey = "".join([key[i] for i in cbits])
-           self.logicalq_res[newkey] = values
+            newkey = "".join([key[i] for i in cbits])
+            self.logicalq_res[newkey] = values
 
         self.taskid = input_dict['task_id']
         self.taskname = input_dict['task_name']
         self.transpiled_openqasm = input_dict["openqasm"]
         from ..circuits.quantum_circuit import QuantumCircuit
         self.transpiled_circuit = QuantumCircuit(0)
         self.transpiled_circuit.from_openqasm(self.transpiled_openqasm)
         self.measure_base = []
         total_counts = sum(self.counts.values())
-        self.amplitudes = {} 
+        self.probabilities = {}
         for key in self.counts:
-            self.amplitudes[key] = self.counts[key]/total_counts
-    
+            self.probabilities[key] = self.counts[key] / total_counts
 
     def calculate_obs(self, pos):
         """
-        Calculate observables Z on input position using amplitudes
+        Calculate observables Z on input position using probabilities
 
         Args: 
             pos (list[int]): Positions of observalbes.
         """
-        return measure_obs(pos, self.logicalq_res) 
+        return measure_obs(pos, self.logicalq_res)
 
-    def plot_amplitudes(self):
+    def plot_probabilities(self):
         """
-        Plot the amplitudes from execute results.
+        Plot the probabilities from execute results.
         """
-        bitstrs = list(self.amplitudes.keys())
-        amps = list(self.amplitudes.values())
+        bitstrs = list(self.probabilities.keys())
+        probs = list(self.probabilities.values())
         plt.figure()
-        plt.bar(range(len(amps)), amps, tick_label = bitstrs)
+        plt.bar(range(len(probs)), probs, tick_label=bitstrs)
         plt.xticks(rotation=70)
-        plt.ylabel("amplitudes")
+        plt.ylabel("probabilities")
 
 
 class SimuResult(Result):
     """
     Class that save the execute simulation results returned from classical simulator.
 
     Attributes:
         num (int): Numbers of measured qubits
-        amplitudes (ndarray): Calculated amplitudes on each bitstring.
+        probabilities (ndarray): Calculated probabilities on each bitstring.
         rho (ndarray): Simulated density matrix of measured qubits
     """
+
     def __init__(self, input, input_form):
         self.num = int(np.log2(input.shape[0]))
         if input_form == "density_matrix":
             self.rho = np.array(input)
-            self.amplitudes = np.diag(input)
-        elif input_form == "amplitudes":
-            self.amplitudes = input
+            self.probabilities = np.diag(input)
+        elif input_form == "probabilities":
+            self.probabilities = input
         elif input_form == "state_vector":
-            self.state_vector = input            
-        
-    def plot_amplitudes(self, full: bool=False, reverse_basis: bool=False, sort: bool=None):
+            self.state_vector = input
+
+    def plot_probabilities(self, full: bool = False, reverse_basis: bool = False, sort: bool = None):
         """
-        Plot the amplitudes from simulated results, ordered in big endian convention.
+        Plot the probabilities from simulated results, ordered in big endian convention.
         
         Args:
             full: Whether plot on the full basis of measured qubits.
             reverse_basis: Whether reverse the bitstring of basis. (Little endian convention).
-            sort:  Sort the results by amplitude values. Can be `"ascend"` order or `"descend"` order. 
+            sort:  Sort the results by probabilities values. Can be `"ascend"` order or `"descend"` order. 
         """
 
-        from ..utils.basis import get_basis
-        probs = self.amplitudes
+        probs = self.probabilities
         inds = range(len(probs))
         if not full:
-            inds = np.where(self.amplitudes > 1e-14)[0]
-            probs = self.amplitudes[inds]
+            inds = np.where(self.probabilities > 1e-14)[0]
+            probs = self.probabilities[inds]
 
-        basis=np.array([bin(i)[2:].zfill(self.num) for i in inds])
+        basis = np.array([bin(i)[2:].zfill(self.num) for i in inds])
         if reverse_basis:
-            basis=np.array([bin(i)[2:].zfill(self.num)[::-1] for i in inds])
+            basis = np.array([bin(i)[2:].zfill(self.num)[::-1] for i in inds])
 
         if sort == "ascend":
             orders = np.argsort(probs)
             probs = probs[orders]
             basis = basis[orders]
         elif sort == "descend":
             orders = np.argsort(probs)
             probs = probs[orders][::-1]
             basis = basis[orders][::-1]
 
-
         plt.figure()
         plt.bar(inds, probs, tick_label=basis)
         plt.xticks(rotation=70)
-        plt.ylabel("amplitudes")
+        plt.ylabel("probabilities")
 
     def get_statevector(self):
         return self.state_vector
 
     def calculate_obs(self, pos):
-        "Calculate observables Z on input position using amplitudes"
-        inds = np.where(self.amplitudes > 1e-14)[0]
-        probs = self.amplitudes[inds]
-        basis=np.array([bin(i)[2:].zfill(self.num) for i in inds])
+        "Calculate observables Z on input position using probabilities"
+        inds = np.where(self.probabilities > 1e-14)[0]
+        probs = self.probabilities[inds]
+        basis = np.array([bin(i)[2:].zfill(self.num) for i in inds])
         res_reduced = dict(zip(basis, probs))
         return measure_obs(pos, res_reduced)
 
 
 def intersec(a, b):
     inter = []
     aind = []
     bind = []
     for i in range(len(a)):
         for j in range(len(b)):
             if a[i] == b[j]:
                 inter.append(a[i])
                 aind.append(i)
                 bind.append(j)
-    
+
     return inter, aind, bind
 
+
 def diff(a, b):
     diff = []
     aind = []
     for i in range(len(a)):
         if a[i] not in b:
             diff.append(a[i])
             aind.append(i)
-    
+
     return diff, aind
 
 
 def merge_measure(obslist):
     obslist = copy.deepcopy(obslist)
     measure_basis = []
     targ_basis = []
     for obs in obslist:
         if len(measure_basis) == 0:
             measure_basis.append(obs)
-            targ_basis.append(len(measure_basis)-1)
+            targ_basis.append(len(measure_basis) - 1)
         else:
             added = 0
             for mi in range(len(measure_basis)):
                 measure_base = measure_basis[mi]
-                interset, intobsi, intbasei = intersec(obs[1], measure_base[1]) 
+                interset, intobsi, intbasei = intersec(obs[1], measure_base[1])
                 diffset, diffobsi = diff(obs[1], measure_base[1])
                 if not len(interset) == 0:
                     if all(np.array(list(obs[0]))[intobsi] == np.array(list(measure_base[0]))[intbasei]):
                         measure_base[0] += "".join(np.array(list(obs[0]))[diffobsi])
                         measure_base[1].extend(diffset)
                         targ_basis.append(mi)
                         added = 1
@@ -181,12 +181,12 @@
                 else:
                     measure_base[0] += obs[0]
                     measure_base[1].extend(obs[1])
                     targ_basis.append(mi)
                     added = 1
                     break
 
-            if not added: 
+            if not added:
                 measure_basis.append(obs)
-                targ_basis.append(len(measure_basis)-1)
+                targ_basis.append(len(measure_basis) - 1)
 
-    return measure_basis, targ_basis
+    return measure_basis, targ_basis
```

## quafu/simulators/default_simulator.py

```diff
@@ -1,98 +1,99 @@
-#default circuit simulator for state vector
+# default circuit simulator for state vector
 
 from typing import Iterable, List, Union
 from quafu.circuits.quantum_circuit import QuantumCircuit
 from ..results.results import SimuResult
-from ..elements.quantum_element import Barrier, Delay, QuantumGate, SingleQubitGate,  MultiQubitGate, XYResonance
+from ..elements.quantum_element import Barrier, Delay, QuantumGate, SingleQubitGate, MultiQubitGate, XYResonance
 import numpy as np
 from functools import reduce
 from sparse import COO, SparseArray
 from scipy.sparse import kron, eye, coo_matrix
 
 import copy
 
+
 def global_op(gate: QuantumGate, global_qubits: List) -> coo_matrix:
     """Local operators to global operators"""
-    num  = len(global_qubits)
+    num = len(global_qubits)
     if isinstance(gate, SingleQubitGate):
-        local_mat = coo_matrix(gate.matrix)     
+        local_mat = coo_matrix(gate.matrix)
         pos = global_qubits.index(gate.pos)
-        local_mat = kron(kron(eye(2**pos), local_mat), eye(2**(num - pos-1)))
+        local_mat = kron(kron(eye(2 ** pos), local_mat), eye(2 ** (num - pos - 1)))
         return local_mat
 
     elif isinstance(gate, MultiQubitGate):
-        local_mat =coo_matrix(gate.matrix)
+        local_mat = coo_matrix(gate.matrix)
         pos = [global_qubits.index(p) for p in gate.pos]
         num_left = min(pos)
         num_right = num - max(pos) - 1
         num_center = max(pos) - min(pos) + 1
-        center_mat = kron(local_mat, eye(2**(num_center - len(pos))))
+        center_mat = kron(local_mat, eye(2 ** (num_center - len(pos))))
         origin_order = sorted(pos)
-        origin_order.extend([p for p in range(min(pos), max(pos)+1) if p not in pos])
+        origin_order.extend([p for p in range(min(pos), max(pos) + 1) if p not in pos])
         new_order = np.argsort(origin_order)
         center_mat = COO.from_scipy_sparse(center_mat)
         center_mat = permutebits(center_mat, new_order).to_scipy_sparse()
-        center_mat = kron(kron(eye(2**num_left), center_mat), eye(2**num_right))
+        center_mat = kron(kron(eye(2 ** num_left), center_mat), eye(2 ** num_right))
         return center_mat
 
 
-def permutebits(mat: Union[SparseArray, np.ndarray], order : Iterable)\
-    ->Union[SparseArray, np.ndarray]:
+def permutebits(mat: Union[SparseArray, np.ndarray], order: Iterable) \
+        -> Union[SparseArray, np.ndarray]:
     """permute qubits for operators or states"""
     num = len(order)
     order = np.array(order)
     r = len(mat.shape)
-    mat = np.reshape(mat, [2]*r*num)
-    order = np.concatenate([order+len(order)*i for i  in range(r)]) 
+    mat = np.reshape(mat, [2] * r * num)
+    order = np.concatenate([order + len(order) * i for i in range(r)])
     mat = np.transpose(mat, order)
-    mat = np.reshape(mat, [2**num]*r)
+    mat = np.reshape(mat, [2 ** num] * r)
     return mat
 
-def ptrace(psi, ind_A: List, diag: bool=True) -> np.ndarray:
+
+def ptrace(psi, ind_A: List, diag: bool = True) -> np.ndarray:
     """partial trace on a state vector"""
     num = int(np.log2(psi.shape[0]))
     order = copy.deepcopy(ind_A)
     order.extend([p for p in range(num) if p not in ind_A])
 
     psi = permutebits(psi, order)
     if diag:
-        psi = np.abs(psi)**2
-        psi = np.reshape(psi, [2**len(ind_A), 2**(num-len(ind_A))])
+        psi = np.abs(psi) ** 2
+        psi = np.reshape(psi, [2 ** len(ind_A), 2 ** (num - len(ind_A))])
         psi = np.sum(psi, axis=1)
-        return psi        
+        return psi
     else:
-        psi = np.reshape(psi, [2**len(ind_A), 2**(num-len(ind_A))]) 
+        psi = np.reshape(psi, [2 ** len(ind_A), 2 ** (num - len(ind_A))])
         rho = psi @ np.conj(np.transpose(psi))
         return rho
 
-def py_simulate(qc: QuantumCircuit, 
-             state_ini: np.ndarray = np.array([]), 
-             output: str="amplitudes") -> SimuResult:
+
+def py_simulate(qc: QuantumCircuit,
+                state_ini: np.ndarray = np.array([]),
+                output: str = "amplitudes") -> SimuResult:
     """Simulate quantum circuit
         Args:
             qc: quantum circuit need to be simulated.
             state_ini (numpy.ndarray): Input state vector
             output (str): `"amplitudes"`: Return ampliteds on measured qubits.
                           `"density_matrix"`: Return reduced density_amtrix on measured qubits.
                           `"state_vector`: Return full statevector.
         Returns:
            SimuResult object that contain the results.
     """
 
     used_qubits = qc.used_qubits
     num = len(used_qubits)
     if not state_ini:
-        psi = np.zeros(2**num)
+        psi = np.zeros(2 ** num)
         psi[0] = 1
 
     else:
         psi = state_ini
 
-    for gate in qc.gates:   
-        if not ((isinstance(gate, Delay)) or (isinstance(gate, Barrier)) or isinstance(gate, XYResonance)): 
+    for gate in qc.gates:
+        if not ((isinstance(gate, Delay)) or (isinstance(gate, Barrier)) or isinstance(gate, XYResonance)):
             op = global_op(gate, used_qubits)
             psi = op @ psi
 
     return psi
-
-
```

## quafu/simulators/simulator.py

```diff
@@ -1,69 +1,90 @@
-
 from typing import Union
 from .default_simulator import py_simulate, ptrace, permutebits
 from .qfvm import simulate_circuit, execute
 from quafu import QuantumCircuit
 from ..results.results import SimuResult
 import numpy as np
-import time
+from ..exceptions import QuafuError
+
 
-def simulate(qc : Union[QuantumCircuit, str], psi : np.ndarray= np.array([]), simulator:str="qfvm_circ", output: str="amplitudes")-> SimuResult:
+def simulate(qc: Union[QuantumCircuit, str],
+             psi: np.ndarray = np.array([]),
+             simulator: str = "qfvm_circ",
+             output: str = "probabilities",
+             use_gpu: bool = False,
+             use_custatevec: bool = False) -> SimuResult:
     """Simulate quantum circuit
     Args:
         qc: quantum circuit or qasm string that need to be simulated.
         psi : Input state vector
-        simulator:`"qfvm_circ"`: The high performance C++ circuit simulator. 
+        simulator:`"qfvm_circ"`: The high performance C++ circuit simulator with optional GPU support. 
                 `"py_simu"`: Python implemented simulator by sparse matrix with low performace for large scale circuit.
                 `"qfvm_qasm"`: The high performance C++ qasm simulator with limited gate set.
 
-        output: `"amplitudes"`: Return ampliteds on measured qubits, ordered in big endian convention.
+        output: `"probabilities"`: Return probabilities on measured qubits, ordered in big endian convention.
                 `"density_matrix"`: Return reduced density_amtrix on measured qubits, ordered in big endian convention.
                 `"state_vector`: Return original full statevector. The statevector returned by `qfvm` backend is ordered in little endian convention (same as qiskit), while `py_simu` backend is orderd in big endian convention.
+        use_gpu: Use the GPU version of `qfvm_circ` simulator.
+        use_custatevec: Use cuStateVec-based `qfvm_circ` simulator. The argument `use_gpu` must also be True.
+
     Returns:
         SimuResult object that contain the results.
 """
     qasm = ""
     if simulator == "qfvm_qasm":
         if not isinstance(qc, str):
             raise ValueError("Must input valid qasm str for qfvm_qasm simulator")
 
         qasm = qc
         qc = QuantumCircuit(0)
         qc.from_openqasm(qasm)
-     
+
     measures = [qc.used_qubits.index(i) for i in qc.measures.keys()]
     num = 0
     if simulator == "qfvm_circ":
-        num = max(qc.used_qubits)+1
+        num = max(qc.used_qubits) + 1
         measures = list(qc.measures.keys())
-        psi = simulate_circuit(qc, psi)
-        
-    elif simulator ==  "py_simu":
+        if use_gpu:
+            if use_custatevec:
+                try:
+                    from .qfvm import simulate_circuit_custate
+                except ImportError:
+                    raise QuafuError(" pyquafu is installed with cuquantum support")
+                psi = simulate_circuit_custate(qc, psi)
+            else:
+                try:
+                    from .qfvm import simulate_circuit_gpu
+                except ImportError:
+                    raise QuafuError("you are not using the GPU version of pyquafu")
+                psi = simulate_circuit_gpu(qc, psi)
+        else:
+            psi = simulate_circuit(qc, psi)
+
+    elif simulator == "py_simu":
         psi = py_simulate(qc, psi)
     elif simulator == "qfvm_qasm":
         num = qc.num
         measures = list(qc.measures.keys())
-        psi = execute(qasm)      
+        psi = execute(qasm)
     else:
         raise ValueError("invalid circuit")
 
-    
     if output == "density_matrix":
         if simulator in ["qfvm_circ", "qfvm_qasm"]:
             psi = permutebits(psi, range(num)[::-1])
         rho = ptrace(psi, measures, diag=False)
         rho = permutebits(rho, list(qc.measures.values()))
         return SimuResult(rho, output)
 
-    elif output == "amplitudes":
+    elif output == "probabilities":
         if simulator in ["qfvm_circ", "qfvm_qasm"]:
             psi = permutebits(psi, range(num)[::-1])
-        amplitudes = ptrace(psi, measures)
-        amplitudes = permutebits(amplitudes, list(qc.measures.values()))
-        return SimuResult(amplitudes, output) 
-    
+        probabilities = ptrace(psi, measures)
+        probabilities = permutebits(probabilities, list(qc.measures.values()))
+        return SimuResult(probabilities, output)
+
     elif output == "state_vector":
         return SimuResult(psi, output)
 
     else:
-        raise ValueError("output should in be 'density_matrix', 'amplitudes', or 'state_vector'")
+        raise ValueError("output should in be 'density_matrix', 'probabilities', or 'state_vector'")
```

## quafu/tasks/tasks.py

```diff
@@ -1,191 +1,110 @@
-import os
 from typing import Dict, List, Tuple
-
 from quafu.circuits.quantum_circuit import QuantumCircuit
-from ..utils.platform import get_homedir
 from ..exceptions import CircuitError, ServerError, CompileError
 from ..results.results import ExecResult, merge_measure
-from ..backends.backends import ScQ_P10, ScQ_P20, ScQ_P50, ScQ_S41
 from ..users.exceptions import UserError
 import numpy as np
 import json
 import requests
 from urllib import parse
-import re
+from quafu.users.userapi import User
+from quafu.backends.backends import Backend
 import copy
-import networkx as nx
-import matplotlib.pyplot as plt
 
-class Task(object): 
+class Task(object):
     """
     Class for submitting quantum computation task to the backend.
 
     Attributes:
-        token (str): Apitoken that associate to your Quafu account.
         shots (int): Numbers of single shot measurement.
         compile (bool): Whether compile the circuit on the backend
         tomo (bool): Whether do tomography (Not support yet)
+        user (User): User object corresponding to Quafu account
+        priority (int): priority level of the task
+        submit_history (dict): circuit submitted with this task
+        backend (dict): quantum backend that execute the task.
+
     """
-    def __init__(self):
-        self._backend = ScQ_P10()
-        self.token = ""
+    def __init__(self, user = User()):
+        self.user = user
         self.shots = 1000
         self.tomo = False
         self.compile = True
-        self._url = ""
-        self.priority = 2
+        self.priority = self.user.priority
+        self.runtime_job_id = ""
         self.submit_history = { }
+        self._available_backends = self.user.get_available_backends(print_info=False)
+        self.backend = self._available_backends[list(self._available_backends.keys())[0]]
 
 
-    def load_account(self) -> None:
-        """
-        Load your Quafu account.
-        """
-        homedir = get_homedir()
-        file_dir = homedir + "/.quafu/"
-        try: 
-            f = open(file_dir + "api", "r")
-            data = f.readlines()
-            self.token = data[0].strip("\n")
-            self._url = data[1].strip("\n")
-        except:
-            raise UserError("User configure error. Please set up your token.")  
-
-    def config(self, 
-               backend: str="ScQ-P10", 
-               shots: int=1000, 
+    def config(self,
+               backend: str="ScQ-P10",
+               shots: int=1000,
                compile: bool=True,
                tomo: bool=False,
                priority: int=2) -> None:
         """
         Configure the task properties
 
         Args:
             backend: Select the experimental backend.
             shots: Numbers of single shot measurement.
             compile: Whether compile the circuit on the backend
             tomo:  Whether do tomography (Not support yet)
             priority: Task priority.
         """
-        if backend == "ScQ-P10":
-            self._backend = ScQ_P10()
-        elif backend == "ScQ-P20":
-            self._backend = ScQ_P20()
-        elif backend == "ScQ-P50":
-            self._backend = ScQ_P50()
-        elif backend == "ScQ-S41":
-            self._backend = ScQ_S41()        
+        if backend not in self._available_backends.keys():
+            raise UserError("backend %s is not valid, available backends are "%backend+", ".join(self._available_backends.keys()))
+
+        self.backend = self._available_backends[backend]
         self.shots = shots
         self.tomo = tomo
         self.compile = compile
         self.priority = priority
 
+
     def get_history(self) -> Dict:
         """
         Get the history of submitted task.
         Returns:
-            A dict of history. The key is the group name and the value is a list of task id in the group. 
+            A dict of history. The key is the group name and the value is a list of task id in the group.
         """
         return self.submit_history
 
+
+
     def get_backend_info(self) -> Dict:
         """
         Get the calibration information of the experimental backend.
 
-        Returns: 
+        Returns:
             Backend information dictionary containing the mapping from the indices to the names of physical bits `'mapping'`, backend topology  `'topology_diagram'` and full calibration inforamtion `'full_info'`.
         """
-        backend_info = self._backend.get_info(self._url, self.token)
-        json_topo_struct = backend_info["topological_structure"]
-        qubits_list = []
-        for gate in json_topo_struct.keys():
-            qubit = gate.split('_')
-            qubits_list.append(qubit[0])
-            qubits_list.append(qubit[1])
-        qubits_list = list(set(qubits_list))
-        qubits_list = sorted(qubits_list, key=lambda x: int(re.findall(r"\d+", x)[0]))
-        int_to_qubit = {k: v for k, v in enumerate(qubits_list)}
-        qubit_to_int = {v: k for k, v in enumerate(qubits_list)}
-
-        directed_weighted_edges = []
-        weighted_edges = []
-        edges_dict = {}
-        clist = []
-        for gate, name_fidelity in json_topo_struct.items():
-            gate_qubit = gate.split('_')
-            qubit1 = qubit_to_int[gate_qubit[0]]
-            qubit2 = qubit_to_int[gate_qubit[1]]
-            gate_name = list(name_fidelity.keys())[0]
-            fidelity = name_fidelity[gate_name]['fidelity']
-            directed_weighted_edges.append([qubit1, qubit2, fidelity])
-            clist.append([qubit1, qubit2])
-            gate_reverse = gate.split('_')[1] + '_' + gate.split('_')[0]
-            if gate not in edges_dict and gate_reverse not in edges_dict:
-                edges_dict[gate] = fidelity
-            else:
-                if fidelity < edges_dict[gate_reverse]:
-                    edges_dict.pop(gate_reverse)
-                    edges_dict[gate] = fidelity
-
-        for gate, fidelity in edges_dict.items():
-            gate_qubit = gate.split('_')
-            qubit1, qubit2 = qubit_to_int[gate_qubit[0]], qubit_to_int[gate_qubit[1]]
-            weighted_edges.append([qubit1, qubit2, np.round(fidelity, 3)])
-
-        # draw topology
-
-        G = nx.Graph()
-        for key, value in int_to_qubit.items():
-            G.add_node(key, name=value)
-
-        G.add_weighted_edges_from(weighted_edges)
-
-        elarge = [(u, v) for (u, v, d) in G.edges(data=True) if d["weight"] >= 0.9]
-        esmall = [(u, v) for (u, v, d) in G.edges(data=True) if d["weight"] < 0.9]
-        elarge_labels = {(u, v) : "%.3f" %d["weight"] for (u, v, d) in G.edges(data=True) if d["weight"] >= 0.9}
-        esmall_labels = {(u, v) : "%.3f" %d["weight"] for (u, v, d) in G.edges(data=True) if d["weight"] < 0.9}
-
-        pos = nx.spring_layout(G, seed=1)  
-        fig, ax = plt.subplots()
-        nx.draw_networkx_nodes(G, pos, node_size=400, ax=ax)
-
-        nx.draw_networkx_edges(G, pos, edgelist=elarge, width=2, ax=ax)
-        nx.draw_networkx_edges(
-            G, pos, edgelist=esmall, width=2, alpha=0.5, style="dashed"
-        , ax=ax)
-
-        nx.draw_networkx_labels(G, pos, font_size=14, font_family="sans-serif", ax=ax)
-        edge_labels = nx.get_edge_attributes(G, "weight")
-        nx.draw_networkx_edge_labels(G, pos, elarge_labels, font_size=12, font_color="green", ax=ax)
-        nx.draw_networkx_edge_labels(G, pos, esmall_labels, font_size=12, font_color="red", ax=ax)
-        fig.set_figwidth(14)
-        fig.set_figheight(14)
-        fig.tight_layout()
-        return {"mapping" : int_to_qubit, "topology_diagram": fig, "full_info": backend_info}
+        return self.backend.get_chip_info(self.user)
 
     def submit(self,
                qc: QuantumCircuit,
                obslist: List=[])\
                 -> Tuple[List[ExecResult], List[int]]:
         """
         Execute the circuit with observable expectation measurement task.
         Args:
             qc (QuantumCircuit): Quantum circuit that need to be executed on backend.
             obslist (list[str, list[int]]): List of pauli string and its position.
 
-        Returns: 
+        Returns:
             List of executed results and list of measured observable
 
-        Examples: 
+        Examples:
             1) input [["XYX", [0, 1, 2]], ["Z", [1]]] measure pauli operator XYX at 0, 1, 2 qubit, and Z at 1 qubit.\n
             2) Measure 5-qubit Ising Hamiltonian we can use\n
             obslist = [["X", [i]] for i in range(5)]]\n
             obslist.extend([["ZZ", [i, i+1]] for i in range(4)])\n
-        
+
         For the energy expectation of Ising Hamiltonian \n
         res, obsexp = q.submit_task(obslist)\n
         E = sum(obsexp)
         """
         # save input circuit
         inputs = copy.deepcopy(qc.gates)
         measures = list(qc.measures.keys())
@@ -213,16 +132,16 @@
             for obi in range(len(obslist)):
                 obs = obslist[obi]
                 rpos = [measures.index(p) for p in obs[1]]
                 measure_results.append(exec_res[targlist[obi]].calculate_obs(rpos))
 
         return exec_res, measure_results
 
-    def run(self, 
-            qc: QuantumCircuit, 
+    def run(self,
+            qc: QuantumCircuit,
             measure_base: List=[]) -> ExecResult:
         """Single run for measurement task.
 
         Args:
             qc (QuantumCircuit): Quantum circuit that need to be executed on backend.
             measure_base (list[str, list[int]]): measure base and it position.
         """
@@ -238,97 +157,102 @@
                     qc.rx(pos, np.pi / 2)
 
             res = self.send(qc)
             res.measure_base = measure_base
 
         return res
 
-    def send(self, 
-             qc: QuantumCircuit, 
-             name: str="", 
+    def send(self,
+             qc: QuantumCircuit,
+             name: str="",
              group: str="",
             wait: bool=True) -> ExecResult:
         """
         Run the circuit on experimental device.
 
         Args:
             qc: Quantum circuit that need to be executed on backend.
             name: Task name.
             group: The task belong which group.
             wait: Whether wait until the execution return.
-        Returns: 
+        Returns:
             ExecResult object that contain the dict return from quantum device.
         """
+        from quafu import get_version
+        version = get_version()
+        if qc.num > self.backend.qubit_num:
+            raise CircuitError("The qubit number %d is too large for backend %s which has %d qubits" %(qc.num, self.backend.name, self.backend.qubit_num))
+
         self.check_valid_gates(qc)
         qc.to_openqasm()
-        backends = {"ScQ-P10": 0, "ScQ-P20": 1, "ScQ-P50": 2, "ScQ-S41" : 3}
         data = {"qtasm": qc.openqasm, "shots": self.shots, "qubits": qc.num, "scan": 0,
-                "tomo": int(self.tomo), "selected_server": backends[self._backend.name],
-                "compile": int(self.compile), "priority": self.priority, "task_name": name}
-        
+                "tomo": int(self.tomo), "selected_server": self.backend.system_id,
+                "compile": int(self.compile), "priority": self.priority, "task_name": name,
+                "pyquafu_version": version, "runtime_job_id": self.runtime_job_id}
+
         if wait:
-            url = self._url  + "qbackend/scq_kit/"
+            url = self.user._url  + self.user.exec_api
         else:
-            url = self._url + "qbackend/scq_kit_asyc/"
-            
-        headers = {'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8', 'api_token': self.token}
+            url = self.user._url  + self.user.exec_async_api
+
+        headers = {'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8', 'api_token': self.user.apitoken}
         data = parse.urlencode(data)
         data = data.replace("%27", "'")
         res = requests.post(url, headers=headers, data=data)
         res_dict = json.loads(res.text)
 
         if res.json()["status"] in [201, 205]:
             raise UserError(res_dict["message"])
         elif res.json()["status"] == 5001:
             raise CircuitError(res_dict["message"])
         elif res.json()["status"] == 5003:
             raise ServerError(res_dict["message"])
         elif res.json()["status"] == 5004:
-            raise CompileError(res_dict["message"]) 
+            raise CompileError(res_dict["message"])
         else:
             task_id = res_dict["task_id"]
-     
+
             if not (group in self.submit_history):
                 self.submit_history[group] = [task_id]
             else:
                 self.submit_history[group].append(task_id)
 
             return ExecResult(res_dict, qc.measures)
 
     def retrieve(self, taskid: str) -> ExecResult:
         """
         Retrieve the results of submited task by taskid.
-        
+
         Args:
             taskid: The taskid of the task need to be retrieved.
         """
         data = {"task_id" : taskid}
-        url = self._url  + "qbackend/scq_task_recall/"
+        url = self.user._url  + self.user.exec_recall_api
 
         headers = {'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8', 'api_token': self.token}
         res = requests.post(url, headers=headers, data=data)
 
         res_dict = json.loads(res.text)
         measures = eval(res_dict["measure"])
-        
+
         return ExecResult(res_dict, measures)
 
-    def retrieve_group(self, 
+    def retrieve_group(self,
                        group: str,
-                       history: Dict={}, 
+                       history: Dict={},
                        verbose: bool=True) -> List[ExecResult]:
         """
         Retrieve the results of submited task by group name.
 
         Args:
             group: The group name need to be retrieved.
             history: History from which to retrieve the results. If not provided, the history will be the submit history of saved by current task.
             verbose: Whether print the task status in the group.
         Returns:
-            A list of execution results in the retrieved group. Only completed task will be added. 
+            A list of execution results in the retrieved group. Only completed task will be added.
         """
         history = history if history else self.submit_history
         taskids = history[group]
 
         group_res = []
         if verbose:
             group = group if group else "Untitled group"
@@ -340,29 +264,28 @@
             if verbose:
                 taskname = taskname if taskname else "Untitled"
                 print((" "*5).join([("%s" %res.taskid).ljust(16), ("%s" %taskname).ljust(10), ("%s" %res.task_status).ljust(10)]))
             if res.task_status == "Completed":
                 group_res.append(res)
 
         return group_res
-    
-     
+
+
     def check_valid_gates(self, qc: QuantumCircuit) -> None:
         """
         Check the validity of the quantum circuit.
         Args:
             qc: QuantumCicuit object that need to be checked.
         """
         if not self.compile:
-            valid_gates = self._backend.valid_gates
+            valid_gates = self.backend.get_valid_gates()
             for gate in qc.gates:
                 if gate.name.lower() not in valid_gates:
-                    raise CircuitError("Invalid operations '%s' for backend '%s'" %(gate.name, self._backend.name))
-                    
+                    raise CircuitError("Invalid operations '%s' for backend '%s'" %(gate.name, self.backend.name))
+
         else:
-            if self._backend.name == "ScQ-S41":
+            if self.backend.name == "ScQ-S41":
                 raise CircuitError("Backend ScQ-S41 must be used without compilation")
-            if self._backend.name == "ScQ-P50":
+            if self.backend.name == "ScQ-P136":
                 for gate in qc.gates:
-                    if gate.name.lower() in ["delay", "xy"]:
-                        raise CircuitError("Invalid operations '%s' for backend '%s'" %(gate.name, self._backend.name))
-        
+                    if gate.name.lower() in ["xy"]:
+                        raise CircuitError("Invalid operations '%s' for backend '%s'" %(gate.name, self.backend.name))
```

## quafu/users/userapi.py

```diff
@@ -1,23 +1,75 @@
 from ..utils.platform import get_homedir
 import os
 import requests
 import json
 from urllib import parse
+from .exceptions import UserError
+
 
 class User(object):
     def __init__(self):
         self.apitoken = ""
-        
+        self._url = "http://quafu.baqis.ac.cn/"
+        self.load_account()
+
+        self.backends_api = "qbackend/get_backends/"
+        self.chip_api = "qbackend/scq_get_chip_info/"
+        self.exec_api = "qbackend/scq_kit/"
+        self.exec_async_api = "qbackend/scq_kit_asyc/"
+        self.exec_recall_api = "qbackend/scq_task_recall/"
+        self.priority = 2
+
+
     def save_apitoken(self, apitoken):
         """
         Save your apitoken associate your Quafu account.
         """
         self.apitoken = apitoken
         homedir = get_homedir()
         file_dir = homedir + "/.quafu/"
         if not os.path.exists(file_dir):
             os.mkdir(file_dir)
         with open(file_dir + "api", "w") as f:
             f.write(self.apitoken+"\n")
             f.write("http://quafu.baqis.ac.cn/")
-    
+
+    def load_account(self):
+        """
+        Load Quafu account.
+        """
+        homedir = get_homedir()
+        file_dir = homedir + "/.quafu/"
+        try:
+            f = open(file_dir + "api", "r")
+            data = f.readlines()
+            token = data[0].strip("\n")
+            url = data[1].strip("\n")
+            self.apitoken = token
+            self._url = url
+            return token, url
+        except:
+            raise UserError("User configure error. Please set up your token.")
+
+    def get_backends_info(self):
+        """
+        Get available backends information
+        """
+
+        backends_info = requests.post(url=self._url+self.backends_api, headers={"api_token" : self.apitoken})
+        backends_info_dict = json.loads(backends_info.text)
+        if backends_info_dict["status"] == 201:
+            raise UserError(backends_info_dict["message"])
+        else:
+            return backends_info_dict["data"]
+
+    def get_available_backends(self, print_info=True):
+        from quafu.backends.backends import Backend
+        backends_info = self.get_backends_info()
+        self._available_backends = {info["system_name"]:Backend(info) for info in backends_info}
+
+        if print_info:
+            print((" "*5).join(["system_name".ljust(10), "qubits".ljust(10),   "status".ljust(10)]))
+            for backend in self._available_backends.values():
+                print((" "*5).join([backend.name.ljust(10), str(backend.qubit_num).ljust(10),  backend.status.ljust(10)]))
+
+        return self._available_backends
```

## quafu/utils/platform.py

```diff
@@ -3,8 +3,11 @@
 
 def get_homedir():
     if sys.platform == 'win32':
         homedir = os.environ['USERPROFILE']
     elif sys.platform == 'linux' or sys.platform == 'darwin':
         homedir = os.environ['HOME']
 
-    return homedir
+    return homedir
+
+
+
```

## Comparing `quafu/exceptions.py` & `quafu/exceptions/quafu_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-
-"""
-Exceptions for errors raised while building circuit.
-"""
-
-class QuafuError(Exception):
-    """Base class for errors raised by Quafu."""
-
-    def __init__(self, *message):
-        """Set the error message."""
-        super().__init__(" ".join(message))
-        self.message = " ".join(message)
-
-    def __str__(self):
-        """Return the message."""
-        return repr(self.message)
-
-class CircuitError(QuafuError):
-    """Exceptions for errors raised while building circuit."""
-    pass
-
-class ServerError(QuafuError):
-    pass
-
-class CompileError(QuafuError):
-    pass
-
+"""
+Exceptions for errors raised while building circuit.
+"""
+
+
+class QuafuError(Exception):
+    """Base class for errors raised by Quafu."""
+
+    def __init__(self, *message):
+        """Set the error message."""
+        super().__init__(" ".join(message))
+        self.message = " ".join(message)
+
+    def __str__(self):
+        """Return the message."""
+        return repr(self.message)
+
+
+class CircuitError(QuafuError):
+    """Exceptions for errors raised while building circuit."""
+    pass
+
+
+class ServerError(QuafuError):
+    """ Exceptions for errors raised while connecting to server."""
+    pass
+
+
+class CompileError(QuafuError):
+    """ Exceptions for errors raised while compiling circuit. """
+    pass
```

## Comparing `pyquafu-0.2.9.dist-info/LICENSE` & `pyquafu-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

