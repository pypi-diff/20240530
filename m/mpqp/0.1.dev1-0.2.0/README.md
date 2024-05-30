# Comparing `tmp/mpqp-0.1.dev1.tar.gz` & `tmp/mpqp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqp-0.1.dev1.tar", last modified: Mon Feb 19 12:23:39 2024, max compression
+gzip compressed data, was "mpqp-0.2.0.tar", last modified: Thu May 30 14:15:37 2024, max compression
```

## Comparing `mpqp-0.1.dev1.tar` & `mpqp-0.2.0.tar`

### file list

```diff
@@ -1,229 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.638386 mpqp-0.1.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.598385 mpqp-0.1.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.606386 mpqp-0.1.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/.github/workflows/mpqp_dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/.github/workflows/mpqp_prod.yml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35152 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-19 12:23:39.634386 mpqp-0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.610386 mpqp-0.1.dev1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.610386 mpqp-0.1.dev1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.610386 mpqp-0.1.dev1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/all-modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/barrier.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/circuit.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/execution-extras.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/execution.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/gates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/instructions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/measures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/qasm.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.610386 mpqp-0.1.dev1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    68563 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/resources/ColibriTD-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/resources/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/resources/mpqp_favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/resources/mpqp_test_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/docs/vqa.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.602385 mpqp-0.1.dev1/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.610386 mpqp-0.1.dev1/example/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    58081 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/notebooks/Notebook_1__Basics_of_circuit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/notebooks/Notebook_2__Execution_Bell_circuit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/notebooks/Notebook_3__Expectation_value_of_observables.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15883 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/notebooks/Notebook_4__Quantum_Fourier_Transform.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/notebooks/Notebook_5__Variational_Quantum_Algorithms.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/notebooks/Notebook_6__From_OpenQASM_2_to_3.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.614385 mpqp-0.1.dev1/example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/CNOT_cascade_v_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/aws_execution_trials.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/bell_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/circuit_to_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/native_gates_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/observable_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/open_qasm_conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.614385 mpqp-0.1.dev1/example/scripts/qasm_files/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/circ_import.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/circ_import2.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/include1.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/include1_converted.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/include2.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/include2_converted.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/main.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/example/scripts/qasm_files/test_qasm.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.614385 mpqp-0.1.dev1/mpqp/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.614385 mpqp-0.1.dev1/mpqp/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33156 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.614385 mpqp-0.1.dev1/mpqp/core/instruction/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/barrier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.618385 mpqp-0.1.dev1/mpqp/core/instruction/gates/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/controlled_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/custom_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/gate_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    19553 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/native_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/gates/parametrized_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/instruction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.618385 mpqp-0.1.dev1/mpqp/core/instruction/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/measurement/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/measurement/basis_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/measurement/expectation_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/instruction/measurement/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.618385 mpqp-0.1.dev1/mpqp/core/noise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/noise/noise_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/core/noise/noise_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.618385 mpqp-0.1.dev1/mpqp/execution/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.622386 mpqp-0.1.dev1/mpqp/execution/connection/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/connection/aws_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/connection/env_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/connection/ibm_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/connection/qlm_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/connection/setup_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.622386 mpqp-0.1.dev1/mpqp/execution/providers_execution/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/providers_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/providers_execution/atos_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/providers_execution/aws_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/providers_execution/ibm_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/remote_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16293 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.622386 mpqp-0.1.dev1/mpqp/execution/vqa/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/vqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/vqa/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/execution/vqa/vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.622386 mpqp-0.1.dev1/mpqp/gates/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/gates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.622386 mpqp-0.1.dev1/mpqp/measures/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/measures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.622386 mpqp-0.1.dev1/mpqp/qasm/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.626386 mpqp-0.1.dev1/mpqp/qasm/header_codes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/braket_custom_include.inc
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/c3sqrtx.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/c3x.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/c4x.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/csx.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/cu3.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/qelib1.inc
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/rc3x.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/rccx.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/rxx.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/rzz.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/std_lib.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/stdgates.inc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/header_codes/u0.qasm
--rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/open_qasm_2_and_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/qasm_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/qasm_to_myqlm.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/qasm/qasm_to_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.626386 mpqp-0.1.dev1/mpqp/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/tools/choice_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/tools/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/tools/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/mpqp/tools/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.634386 mpqp-0.1.dev1/mpqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-19 12:23:39.000000 mpqp-0.1.dev1/mpqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-02-19 12:23:39.000000 mpqp-0.1.dev1/mpqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:23:39.000000 mpqp-0.1.dev1/mpqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-19 12:23:39.000000 mpqp-0.1.dev1/mpqp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-19 12:23:39.000000 mpqp-0.1.dev1/mpqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-19 12:23:39.000000 mpqp-0.1.dev1/mpqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 12:23:39.638386 mpqp-0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.606386 mpqp-0.1.dev1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.626386 mpqp-0.1.dev1/tests/OA_attempt/
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/OA_attempt/OA-mpqp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.626386 mpqp-0.1.dev1/tests/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.626386 mpqp-0.1.dev1/tests/core/instruction/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.626386 mpqp-0.1.dev1/tests/core/instruction/gates/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/gates/test_controlled_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/gates/test_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/gates/test_gate_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/gates/test_native_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.630385 mpqp-0.1.dev1/tests/core/instruction/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/measurement/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/measurement/test_basis_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/measurement/test_expectation_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/measurement/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/instruction/test_instruction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.630385 mpqp-0.1.dev1/tests/core/noise/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/noise/test_noise_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/noise/test_noise_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.630385 mpqp-0.1.dev1/tests/core/test_circuit/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/add-X.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/add-list.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/all.qasm2
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/all.qasm3
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/init-barrier.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/init-cnots.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/init-empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/init-measure.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/lot_of_gates.qasm3
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit/wo_meas-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/core/test_circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.630385 mpqp-0.1.dev1/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/example/test_demonstrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.630385 mpqp-0.1.dev1/tests/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.630385 mpqp-0.1.dev1/tests/execution/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/connection/test_ibm_q_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/connection/test_qlm_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/connection/test_setup_connections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.634386 mpqp-0.1.dev1/tests/execution/providers_execution/
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/providers_execution/test_atos_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/providers_execution/test_aws_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/providers_execution/test_ibm_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/execution/test_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.634386 mpqp-0.1.dev1/tests/qasm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.634386 mpqp-0.1.dev1/tests/qasm/qasm_examples/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep1.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep2.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_a.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_b.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_b_converted.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_c.qasm
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_c_converted.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_d.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/circular_dep_d_converted.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/in_time_gate_def.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/in_time_gate_def_converted.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/included.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/late_gate_def.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/with_include.qasm
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/qasm_examples/without_include.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/test_open_qasm_2_and_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/test_qasm_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/test_qasm_to_myqlm.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/qasm/test_qasm_to_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:23:39.634386 mpqp-0.1.dev1/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-19 12:22:03.000000 mpqp-0.1.dev1/tests/tools/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.242218 mpqp-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 14:14:18.000000 mpqp-0.2.0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.206218 mpqp-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.210218 mpqp-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-30 14:14:18.000000 mpqp-0.2.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-30 14:14:18.000000 mpqp-0.2.0/.github/workflows/pipy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 14:14:18.000000 mpqp-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 14:14:18.000000 mpqp-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-30 14:14:18.000000 mpqp-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 14:14:18.000000 mpqp-0.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35152 2024-05-30 14:14:18.000000 mpqp-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-30 14:15:37.242218 mpqp-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-30 14:14:18.000000 mpqp-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-30 14:14:18.000000 mpqp-0.2.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.214218 mpqp-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.214218 mpqp-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.214218 mpqp-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/all-modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/barrier.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/circuit.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/execution-extras.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/execution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/gates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/instructions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/measures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/noise.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.214218 mpqp-0.2.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/notebooks/1_Basics_of_circuit.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/notebooks/2_Execution_Bell_circuit.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/notebooks/3_Expectation_value_of_observables.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/notebooks/4_Quantum_Fourier_Transform.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/notebooks/5_Variational_Quantum_Algorithms.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/notebooks/6_Noise_Simulation.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/qasm.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.214218 mpqp-0.2.0/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21399 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/job-device_compat.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/mpqp-logo-dark-theme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/mpqp-logo-light-theme.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.218218 mpqp-0.2.0/docs/resources/old/
+-rw-r--r--   0 runner    (1001) docker     (127)    68563 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/ColibriTD-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/favicon-v1.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/favicon-v1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/mpqp_favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/mpqp_test_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/old-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/old/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/resources/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 14:14:18.000000 mpqp-0.2.0/docs/vqa.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.206218 mpqp-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.218218 mpqp-0.2.0/examples/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    62151 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/notebooks/1_Basics_of_circuit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/notebooks/2_Execution_Bell_circuit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/notebooks/3_Expectation_value_of_observables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/notebooks/4_Quantum_Fourier_Transform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/notebooks/5_Variational_Quantum_Algorithms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18786 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/notebooks/6_Noise_Simulation.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.218218 mpqp-0.2.0/examples/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/CNOT_cascade_v_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/aws_execution_trials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/bell_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/circuit_to_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/cirq_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/native_gates_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/observable_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/open_qasm_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.222218 mpqp-0.2.0/examples/scripts/qasm_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/circ_import.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/circ_import2.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/include1.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/include1_converted.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/include2.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/include2_converted.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/main.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 14:14:18.000000 mpqp-0.2.0/examples/scripts/qasm_files/test_qasm.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-30 14:14:18.000000 mpqp-0.2.0/mac-install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.222218 mpqp-0.2.0/mpqp/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.222218 mpqp-0.2.0/mpqp/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46047 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.222218 mpqp-0.2.0/mpqp/core/instruction/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/barrier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.222218 mpqp-0.2.0/mpqp/core/instruction/gates/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/controlled_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/custom_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/gate_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26491 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/native_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/gates/parametrized_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/instruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/core/instruction/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/measurement/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/measurement/basis_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/measurement/expectation_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/measurement/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18334 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/instruction/measurement/pauli_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/core/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/execution/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/aws_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/env_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/google_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/ibm_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/key_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/connection/qlm_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/execution/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30300 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/providers/atos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/providers/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/providers/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/remote_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20016 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/execution/vqa/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/vqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/vqa/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14028 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/execution/vqa/vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/gates/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/gates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/measures/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/measures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.226218 mpqp-0.2.0/mpqp/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/noise/custom_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/noise/noise_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.230218 mpqp-0.2.0/mpqp/qasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.230218 mpqp-0.2.0/mpqp/qasm/header_codes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/braket_custom_include.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/c3sqrtx.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/c3x.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/c4x.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/csx.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/cu3.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/qelib1.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/rc3x.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/rccx.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/rxx.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/rzz.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/std_lib.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/stdgates.inc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/header_codes/u0.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)    23143 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/open_qasm_2_and_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/qasm_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/qasm_to_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/qasm_to_myqlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/qasm/qasm_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.230218 mpqp-0.2.0/mpqp/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/tools/choice_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/tools/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp/tools/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.222218 mpqp-0.2.0/mpqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-30 14:15:36.000000 mpqp-0.2.0/mpqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-05-30 14:15:36.000000 mpqp-0.2.0/mpqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:15:36.000000 mpqp-0.2.0/mpqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 14:15:36.000000 mpqp-0.2.0/mpqp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 14:15:36.000000 mpqp-0.2.0/mpqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 14:15:36.000000 mpqp-0.2.0/mpqp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.230218 mpqp-0.2.0/mpqp_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-30 14:14:18.000000 mpqp-0.2.0/mpqp_scripts/setup_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 14:14:18.000000 mpqp-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 14:14:18.000000 mpqp-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 14:14:18.000000 mpqp-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-30 14:14:18.000000 mpqp-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.230218 mpqp-0.2.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-30 14:14:18.000000 mpqp-0.2.0/resources/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-30 14:14:18.000000 mpqp-0.2.0/resources/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   889744 2024-05-30 14:14:18.000000 mpqp-0.2.0/resources/mpqp-usage.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:15:37.242218 mpqp-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-30 14:14:18.000000 mpqp-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.234218 mpqp-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.234218 mpqp-0.2.0/tests/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.234218 mpqp-0.2.0/tests/core/instruction/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.234218 mpqp-0.2.0/tests/core/instruction/gates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/gates/test_controlled_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/gates/test_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/gates/test_gate_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/gates/test_native_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.234218 mpqp-0.2.0/tests/core/instruction/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/measurement/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/measurement/test_basis_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/measurement/test_expectation_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/measurement/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/measurement/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/measurement/test_pauli_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/instruction/test_instruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.234218 mpqp-0.2.0/tests/core/test_circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/add-X.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/add-list.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/all.qasm2
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/all.qasm3
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/init-barrier.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/init-cnots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/init-empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/init-measure.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/lot_of_gates.qasm3
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit/wo_meas-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/core/test_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.238218 mpqp-0.2.0/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/examples/test_demonstrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.238218 mpqp-0.2.0/tests/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.238218 mpqp-0.2.0/tests/execution/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/connection/test_ibm_q_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/connection/test_qlm_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/connection/test_setup_connections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.238218 mpqp-0.2.0/tests/execution/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/providers/test_atos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/providers/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/providers/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/providers/test_ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/test_validity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/execution/test_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.238218 mpqp-0.2.0/tests/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/noise/test_noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/noise/test_noisy_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.238218 mpqp-0.2.0/tests/qasm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.242218 mpqp-0.2.0/tests/qasm/qasm_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep1.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep2.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_a.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_b.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_b_converted.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_c.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_c_converted.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_d.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/circular_dep_d_converted.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/in_time_gate_def.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/in_time_gate_def_converted.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/included.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/late_gate_def.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/with_include.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/qasm_examples/without_include.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/test_open_qasm_2_and_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/test_qasm_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/test_qasm_to_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/test_qasm_to_myqlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/qasm/test_qasm_to_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/test_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:15:37.242218 mpqp-0.2.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 14:14:18.000000 mpqp-0.2.0/tests/tools/test_math.py
```

### Comparing `mpqp-0.1.dev1/LICENSE` & `mpqp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/docs/_static/custom.js` & `mpqp-0.2.0/docs/_static/custom.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,132 +1,134 @@
 window.onload = () => {
     // detect enums and make sure their description is easily to style
-    document.querySelectorAll(".class").forEach(class_elt => {
+    document.querySelectorAll(".class").forEach((class_elt) => {
         if (isEnum(class_elt)) {
             title = class_elt.querySelector("dt");
             title.innerHTML = title.innerHTML.replace(/, /g, "<span>, </span>");
             class_elt.classList.add("enum");
         }
-    })
+    });
 
     // remove the dark theme watermark added in js
-    footer = document.querySelector("footer")
-    dark_theme_link = (
+    footer = document.querySelector("footer");
+    dark_theme_link =
         '<a href="https://github.com/MrDogeBro/sphinx_rtd_dark_mode">Dark theme</a>' +
-        ' provided by ' +
-        '<a href="http://mrdogebro.com">MrDogeBro</a>.'
-    )
+        " provided by " +
+        '<a href="http://mrdogebro.com">MrDogeBro</a>.';
     whenCondition(
-        () => footer.innerHTML = footer.innerHTML.replace(dark_theme_link, ''),
+        () => (footer.innerHTML = footer.innerHTML.replace(dark_theme_link, "")),
         () => footer.innerHTML.includes(dark_theme_link)
-    )
+    );
 
-    r = document.querySelector(':root')
-    r.style.setProperty('--dark-link-color', '#80cb53');
+    r = document.querySelector(":root");
+    r.style.setProperty("--dark-link-color", "#80cb53");
 
     // t = document.querySelector('html[data-theme="dark"] .wy-side-nav-search')
     // t.style.setProperty('background-color', '#0d0d0d');
 
     // move the attribute and properties of a class to appear first in the class
-    document.querySelectorAll(".py.class").forEach(pythonClass => {
+    document.querySelectorAll(".py.class").forEach((pythonClass) => {
         if (!isEnum(pythonClass)) {
-            appendAfter = getEndOfClassHeader(pythonClass)
-            pythonClass.querySelectorAll(".py.attribute").forEach(attribute => {
-                appendAfter.insertAdjacentElement('afterend', attribute)
-                appendAfter = attribute
-            })
-            pythonClass.querySelectorAll(".py.property").forEach(property => {
-                appendAfter.insertAdjacentElement('afterend', property)
-                appendAfter = property
-            })
+            appendAfter = getEndOfClassHeader(pythonClass);
+            pythonClass.querySelectorAll(".py.attribute").forEach((attribute) => {
+                appendAfter.insertAdjacentElement("afterend", attribute);
+                appendAfter = attribute;
+            });
+            pythonClass.querySelectorAll(".py.property").forEach((property) => {
+                appendAfter.insertAdjacentElement("afterend", property);
+                appendAfter = property;
+            });
         }
-    })
+    });
 
     // move the constants of a module to appear first in the module
-    document.querySelectorAll(".target").forEach(moduleMarker => {
+    document.querySelectorAll(".target").forEach((moduleMarker) => {
         if (moduleMarker.id.startsWith("module-")) {
-            appendAfter = moduleMarker
-            sibling = moduleMarker.nextSibling
+            module_description =
+                moduleMarker.parentElement.querySelectorAll(".target ~ p");
+            if (module_description.length != 0)
+                appendAfter = module_description[module_description.length - 1];
+            else appendAfter = moduleMarker;
+            sibling = moduleMarker.nextSibling;
             for (; sibling;) {
-                next = sibling.nextSibling
+                next = sibling.nextSibling;
                 if (sibling.nodeName === "DL" && sibling.classList.contains("data")) {
-                    appendAfter.insertAdjacentElement('afterend', sibling)
-                    appendAfter = sibling
+                    appendAfter.insertAdjacentElement("afterend", sibling);
+                    appendAfter = sibling;
                 }
-                sibling = next
+                sibling = next;
             }
         }
-    })
+    });
 
     // move the abstract classes of a module to appear first in the module
-    document.querySelectorAll(".section").forEach(section => {
+    document.querySelectorAll(".section").forEach((section) => {
         if (section.id.startsWith("module-")) {
-            descriptionStart = section.querySelector("dl")
-            appendAfter = descriptionStart.previousElementSibling
-            sibling = descriptionStart
+            descriptionStart = section.querySelector("dl");
+            appendAfter = descriptionStart.previousElementSibling;
+            sibling = descriptionStart;
             for (; sibling;) {
-                next = sibling.nextElementSibling
+                next = sibling.nextElementSibling;
                 if (sibling.classList.contains("class") && isAbstract(sibling)) {
-                    appendAfter.insertAdjacentElement('afterend', sibling)
-                    appendAfter = sibling
+                    appendAfter.insertAdjacentElement("afterend", sibling);
+                    appendAfter = sibling;
                 }
-                sibling = next
+                sibling = next;
             }
         }
-    })
-
-
-}
+    });
+};
 
 // const themeButton = document.querySelector('themeSwitcher')
 // themeButton.addEventListener('click', () => {
 //
 // });
 
-
 function getEndOfClassHeader(elt) {
-    admonition = elt.querySelectorAll(".admonition")
-    if (admonition.length != 0) return admonition[admonition.length - 1]
-    examples = elt.querySelectorAll("dd>div.doctest")
-    if (examples.length != 0) return examples[examples.length - 1]
-    return elt.querySelector(".field-list")
+    admonition = elt.querySelectorAll(".admonition");
+    if (admonition.length != 0) return admonition[admonition.length - 1];
+    field_list = elt.querySelector(".class>dd>.field-list");
+    if (field_list !== null) return elt.querySelector(".class>dd>.field-list");
+    examples = elt.querySelectorAll(".class>dd>div.doctest");
+    if (examples.length != 0) return examples[examples.length - 1];
+    return elt;
 }
 
 function isEnum(elt, explored = []) {
-    id = elt.querySelector("dt").id
-    if (explored.includes(id)) return false
+    id = elt.querySelector("dt").id;
+    if (explored.includes(id)) return false;
 
-    explored.push(id)
+    explored.push(id);
 
-    parents = elt.querySelector("dd > p:first-child")
+    parents = elt.querySelector("dd > p:first-child");
     if (parents && parents.innerHTML.includes("Enum")) {
-        return true
+        return true;
     }
 
-    parents_contain_enum = false
-    elt.querySelectorAll("dd > p:first-child > a").forEach(link => {
-        parent_id = link.href.split("#")[1]
-        new_elt = document.querySelector(`.class:has([id='${parent_id}'])`)
-        if (new_elt && isEnum(new_elt, explored)) parents_contain_enum = true
-    })
+    parents_contain_enum = false;
+    elt.querySelectorAll("dd > p:first-child > a").forEach((link) => {
+        parent_id = link.href.split("#")[1];
+        new_elt = document.querySelector(`.class:has([id='${parent_id}'])`);
+        if (new_elt && isEnum(new_elt, explored)) parents_contain_enum = true;
+    });
 
-    return parents_contain_enum
+    return parents_contain_enum;
 }
 
 function isAbstract(elt) {
-    parents = elt.querySelector("dd > p:first-child")
+    parents = elt.querySelector("dd > p:first-child");
     if (parents && parents.innerHTML.includes("ABC")) {
-        return true
+        return true;
     }
-    return false
+    return false;
 }
 
 function whenCondition(action, condition) {
     function watcher() {
         if (condition()) {
-            action()
-            clearInterval(interval)
+            action();
+            clearInterval(interval);
         }
     }
 
     interval = setInterval(watcher, 50);
 }
```

### Comparing `mpqp-0.1.dev1/docs/conf.py` & `mpqp-0.2.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
+
+import os
+import sys
 from typing import Literal
 
+import dotenv
+from pygments.formatters.latex import LatexFormatter
+
 # Configuration file for the Sphinx documentation builder.
 from sphinx.application import Sphinx
 from sphinx.highlighting import PygmentsBridge
-from pygments.formatters.latex import LatexFormatter
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
-import os
-import sys
 
 sys.path.insert(0, os.path.abspath("../"))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "MPQP"
@@ -32,22 +35,53 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.mathjax",
     "sphinx_rtd_dark_mode",
     "sphinx_copybutton",
-    "sphinx_github_changelog",
+    "nbsphinx",  # requires pandoc ?
+    "nbsphinx_link",
 ]
 default_dark_mode = True
 autodoc_typehints = "description"
 autodoc_type_aliases = {"Matrix": "Matrix", "AvailableDevice": "AvailableDevice"}
+autodoc_mock_imports = ["braket.circuits.measure"]
 simplify_optional_unions = True
 typehints_defaults = "comma"
-sphinx_github_changelog_token = "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"
+dotenv.load_dotenv()
+sphinx_github_changelog_token = os.getenv("SPHINX_GITHUB_CHANGELOG_TOKEN")
+if sphinx_github_changelog_token is not None:
+    extensions.append("sphinx_github_changelog")
+
+# {% set docname = env.doc2path(env.docname,base=None).replace("\\", "/").split(".")[0].split("/")[-1] + '.ipynb' %}
+
+# .. raw:: html
+
+#     <div class="admonition note">
+#       This page was generated from the notebook
+#       <a class="reference external" href="{{ docname|e }}">{{ docname|e }}</a>.
+#     </div>
+
+nbsphinx_prolog = r"""
+{% set docname = 'examples/notebooks/' + env.doc2path(env.docname,base=None).split("/")[-1].split("\\")[-1].split(".")[0] + '.ipynb' %}
+
+.. raw:: html
+
+    <div class="admonition note">
+      This page was generated from the notebook
+      <a class="reference external" href="https://github.com/ColibrITD-SAS/mpqp/blob/main/{{ docname|e }}">{{ docname|e }}</a>.
+    </div>
+
+.. raw:: latex
+
+    \nbsphinxstartnotebook{\scriptsize\noindent\strut
+    \textcolor{gray}{The following section was generated from the notebook
+    \sphinxcode{\sphinxupquote{\strut {{ docname | escape_latex }}}} \dotfill}}
+"""
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
@@ -108,17 +142,24 @@
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
+# `html_theme` is not needed since we use a plugin to have the dark theme RTD,
+# so `html_theme` is overridden anyway.
 # html_theme = "alabaster"
-# html_theme = "furo"  # pip install furo
-# html_theme = "sphinx_rtd_theme"  # pip install sphinx-rtd-theme
+html_context = {
+    "display_github": True,
+    "github_user": "ColibrITD-SAS",
+    "github_repo": "mpqp",
+    "github_version": "dev",
+    "conf_py_path": "/docs/",
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
@@ -132,20 +173,20 @@
 # "<project> v<release> documentation".
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 html_short_title = "MPQP"
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-html_logo = "resources/mpqp_test_logo.png"
+html_logo = "resources/mpqp-logo-dark-theme.svg"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-html_favicon = "resources/mpqp_favicon.png"
+html_favicon = "resources/favicon.ico"
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 # html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
@@ -169,15 +210,16 @@
 # If false, no index is generated.
 # html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
 # html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-# html_show_sourcelink = True
+html_show_sourcelink = True
+html_sourcelink_suffix = ""
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 html_show_sphinx = False
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
 # html_show_copyright = True
```

### Comparing `mpqp-0.1.dev1/docs/execution-extras.rst` & `mpqp-0.2.0/docs/execution-extras.rst`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 implemented. Most of them are aimed at internal usage even though you can
 absolutely use them yourself. As a user, the elements of this page of interest
 for you are most likely:
 
 - IBM's :func:`get_all_job_ids<mpqp.execution.connection.ibm_connection.get_all_job_ids>`;
 - Eviden's :func:`get_all_job_ids<mpqp.execution.connection.qlm_connection.get_all_job_ids>`;
 - AWS's :func:`get_all_task_ids<mpqp.execution.connection.aws_connection.get_all_task_ids>`;
+- CIRQ's :func:`get_all_job_ids<mpqp.execution.connection.cirq_connection.get_all_job_ids>`;
 - The :ref:`con-setup` section.
 
 Provider specifics
 ------------------
 
-Even though most of our interfaces use abstractions such that you don't need to
+Even though most of our interfaces use abstractions such that you do not need to
 know on which provider's QPU your code is running, we need at some point to
 tackle the specifics of each providers. Most (hopefully all soon) of it is
 tackle in these modules.
 
 IBM
 ^^^
 
@@ -27,46 +28,71 @@
 __________
 
 .. automodule:: mpqp.execution.connection.ibm_connection
 
 Execution
 __________
 
-.. automodule:: mpqp.execution.providers_execution.ibm_execution
+.. automodule:: mpqp.execution.providers.ibm
 
 Atos/Eviden
 ^^^^^^^^^^^
 
 Connection
 __________
 
 .. automodule:: mpqp.execution.connection.qlm_connection
 
 Execution
 __________
 
-.. automodule:: mpqp.execution.providers_execution.atos_execution
+.. automodule:: mpqp.execution.providers.atos
 
 AWS
 ^^^
 
-.. automodule:: mpqp.execution.providers_execution.aws_execution
-
 Connection
 __________
 
 .. automodule:: mpqp.execution.connection.aws_connection
 
 Execution
 __________
 
+.. automodule:: mpqp.execution.providers.aws
+
+Google
+^^^^^^
+
+Connection
+__________
+
+.. automodule:: mpqp.execution.connection.google_connection
+
+Execution
+__________
+
+.. automodule:: mpqp.execution.providers.google
+
 .. _con-setup:
 
+Connection setup
+^^^^^^^^^^^^^^^^
+
+key Connection
+______________
+
+.. automodule:: mpqp.execution.connection.key_connection
+
 Connection setup script 
 -----------------------
 
-.. automodule:: mpqp.execution.connection.setup_connections
+.. automodule:: mpqp_scripts.setup_connections
+
+The details on how to get these information can be found in the section 
+:ref:`Remote setup`.
 
 On disk configuration manager
 -----------------------------
 
 .. automodule:: mpqp.execution.connection.env_manager
+
```

### Comparing `mpqp-0.1.dev1/docs/gates.rst` & `mpqp-0.2.0/docs/gates.rst`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/docs/measures.rst` & `mpqp-0.2.0/docs/measures.rst`

 * *Files 12% similar despite different names*

```diff
@@ -39,7 +39,11 @@
 
 
 Measuring using an observable
 -----------------------------
 
 .. automodule:: mpqp.core.instruction.measurement.expectation_value
 
+Pauli String
+^^^^^^^^^^^^
+
+.. automodule:: mpqp.core.instruction.measurement.pauli_string
```

### Comparing `mpqp-0.1.dev1/docs/resources/ColibriTD-logo.png` & `mpqp-0.2.0/docs/resources/old/ColibriTD-logo.png`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/docs/resources/favicon.ico` & `mpqp-0.2.0/docs/resources/old/old-favicon.ico`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/docs/resources/mpqp_favicon.png` & `mpqp-0.2.0/docs/resources/old/mpqp_favicon.png`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/docs/resources/mpqp_test_logo.png` & `mpqp-0.2.0/docs/resources/old/mpqp_test_logo.png`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/docs/vqa.rst` & `mpqp-0.2.0/docs/vqa.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _VQA:
+
 Variational Quantum Algorithms
 ==============================
 
 .. code-block:: python
 
     from mpqp.execution.vqa import *
 
@@ -22,15 +24,15 @@
 has ``FreeExpression``, ``qiskit`` has ``Parameter``, ``qlm`` has ``Variable``,
 ``cirq`` uses ``sympy``'s ``Symbol``, etc...
 
 Once you define a circuit with variables, you have two options:
 
 1. either the measure of the circuit is an 
    :class:`ExpectationMeasure<mpqp.core.instruction.measurement.expectation_value.ExpectationMeasure>`
-   can directly feed it in the optimizer;
+   and can directly feed it in the optimizer;
 2. or you can define a custom cost function for more complicated cases.
 
 Detailed example for those two options can be found in our example notebooks.
 
 .. automodule:: mpqp.execution.vqa.vqa
 
 .. automodule:: mpqp.execution.vqa.optimizer
```

### Comparing `mpqp-0.1.dev1/example/notebooks/Notebook_1__Basics_of_circuit.ipynb` & `mpqp-0.2.0/examples/notebooks/1_Basics_of_circuit.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.972976255992366%*

 * *Differences: {"'cells'": "{4: {'execution_count': 4}, 5: {'source': ['Then, one can ``add`` at the end of the "*

 * *            'circuit an instruction or list of instructions. For that, we add the right '*

 * *            "imports.']}, 6: {'execution_count': 2}, 7: {'execution_count': 5}, 8: {'source': ['As "*

 * *            'previously stated, we can also instantiate and initialize the circuit with a list of '*

 * *            "`Instruction` (gates or measurements).']}, 9: {'execution_count': 6, 'source': "*

 * *            "['circ3 = QCirc […]*

```diff
@@ -38,70 +38,81 @@
                 "The first argument taken by the constructor of ``QCircuit`` is either the number of qubits, or a list of ``Instruction``.\n",
                 "\n",
                 "One can instanciate an empty circuit by only giving its number of qubits. The number of classical bits is automatically handled by the class, and thus is optional. We can also attach to a circuit a given label. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "id": "16fbed57",
             "metadata": {},
             "outputs": [],
             "source": [
                 "circ1 = QCircuit(3)\n",
                 "circ2 = QCircuit(5, nb_cbits=2, label=\"Example\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e04832ad",
             "metadata": {},
             "source": [
-                "Then, one can ``add`` at the end of the circuit an instruction or list of instructions. For that, we add some imports."
+                "Then, one can ``add`` at the end of the circuit an instruction or list of instructions. For that, we add the right imports."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "a32e0476",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from mpqp.gates import *\n",
                 "from mpqp.measures import BasisMeasure\n",
                 "from mpqp import Barrier"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "id": "ab1c9ea6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "circ2.add(CNOT(2,3))\n",
                 "circ2.add([H(0), T(1), CNOT(0,1), S(4)])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d2cf3711",
             "metadata": {},
             "source": [
-                "We can also instantiate and initialize the circuit with a list of ``Instruction`` (gates and measurements)."
+                "As previously stated, we can also instantiate and initialize the circuit with a list of `Instruction` (gates or measurements)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "28832987",
             "metadata": {},
             "outputs": [],
             "source": [
-                "circ3 = QCircuit([H(0), X(1), CNOT(1,2), Barrier(), Y(2), Z(0), CZ(1,0), BasisMeasure([0,1,2], shots=1024)])"
+                "circ3 = QCircuit(\n",
+                "    [\n",
+                "        H(0),\n",
+                "        X(1),\n",
+                "        CNOT(1, 2),\n",
+                "        Barrier(),\n",
+                "        Y(2),\n",
+                "        Z(0),\n",
+                "        CZ(1, 0),\n",
+                "        BasisMeasure([0, 1, 2], shots=1024),\n",
+                "    ]\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "97060ed8",
             "metadata": {},
             "source": [
@@ -168,34 +179,34 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fa694b87",
             "metadata": {},
             "source": [
-                "But also use the method ``display`` to render the circuit in different formats. The default one uses matplotlib, but other options can be given in parameters (the same as the ``qiskit`` display function)."
+                "We can also use the method ``display`` to render the circuit in different formats. The default one uses matplotlib, but other options can be given in parameters (the same as the ``qiskit`` display function)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "302ccb5d",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "c:\\users\\hamza\\appdata\\local\\programs\\python\\python39\\lib\\site-packages\\mpqp\\core\\circuit.py:298: UserWarning: Matplotlib is currently using module://ipykernel.pylab.backend_inline, which is a non-GUI backend, so cannot show the figure.\n",
+                        "c:\\Users\\Henri\\anaconda3\\lib\\site-packages\\mpqp\\core\\circuit.py:294: UserWarning: Matplotlib is currently using module://matplotlib_inline.backend_inline, which is a non-GUI backend, so cannot show the figure.\n",
                         "  fig.show()\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 507.997x264.88 with 1 Axes>"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -209,17 +220,17 @@
             "cell_type": "code",
             "execution_count": 9,
             "id": "50e96aae",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAZ0AAACKCAIAAAD+GQBiAAAfl0lEQVR4nO3daVQTSR4A8AI7iXIqoBHkCCAoEt0RiXIMxygiqwijo4DuE+8V8VgVeMtTUXEHxut5uzoe4IK7g6h44TmAosAiKDOIjCJyyS3hjhICSe+HzMuwIYSQo49Qvw88UklX/VPp/NPd1V2tgaIogEjIwcGhoKAA7yggiIg0YF4jKQ0N+NlBkGSaeAcAQRCkZDCvQRCkbmBegyBI3cC8BkGQukHwDgCCSIlCofT29mLWHIIgPT09mDVHdjCvQZA8ent7sRyP1tDQwKwtNUDKvKaKn8ph+HuoxG4chr0HERkp85oqfiqH4e+hErtxGPYeRGRw3ICsPDw88A4BUrLGxsb79+/jHYU6gHmNrJ4+fYp3CJCSRUZG5ubm4h2FOiDlfigEqZ/CwsKHDx+WlJTgHYg6UJ+81tnZ+enTJyqVqqmpiaIon89HUZTBYHz+/Lm+vp5GowmPAfH5fD6fb2VlhXe8xNXe3l5TUzPQs6ampvr6+ljGM0xERETs3btXT08P70DUwR95DUXRmpoaOp1OpVIBADweT/gPWTQ0NFy9ejUzMzMtLU1XVzc0NNTW1nbNmjVsNjspKSknJ+fBgwcjR47csmWLlZVVSEgI3vES182bN1evXk2j0by8vGxsbOh0uvAn4fTp0zU1NdevX//uu+/wjlHd3Lt3r7q6et26dXgHoi5QFEVRNCsry9fXNz4+fu/evenp6Rs3bkxLS0OHiMvlurm5bd68eagLDpUo7P5evnwJAPD19RUrf/fuHQDA09NTjjrV1UBv+dSpUxYWFm/evOlb+OjRIwDA7Nmzh1SVGlPiW+7t7WUymXfv3sWmueEAAQCkpKRERkZmZWWNGzcOABAYGHjz5s0jR44MNUW2t7e/ePGitbVVaUl36EaOHCn6K0s51B+Hw4mOjra3txeVfPnyJSQkZOTIkefOncMxMHV18eJFIyMjX19fvANRH0hDQ8Pq1avPnDkjTGoAAC0trZkzZ2ppaQEAXr58+fDhQ21tbXt7e29vb+l1jRs3rqKiQldXV+VRQ6rE4XB8fHz6luzbt6+ioiImJsbGxgavqAbS3Nzc0tIyceJEkp5Dx+Fw9u/ff+fOHbwDUSuaUVFRAoFg6dKloqLnz58Lz40qKCg4ePBgZGTk9u3bs7Ozf/jhh0GrMzExgXmN7Dw9Pel0uujhr7/+euzYMSaTGRERgWNU/f3222/Ozs5GRka2trZjx469fPky3hHJ49ChQ15eXjNmzMA7EPViYmKyYMEC0X5pdXU1AODx48coirJYLNFRNi6Xq6+v397ejs/u8v8DAx9rePPmDQBgyZIlYuWVlZUAAB8fHznqJKbCwkIFa5DlLfP5fBaLpaGhkZOTo2BVylVfX29gYCC2MsfHx2MWgFLeck1NjaGhYVVVFTbNDR9IXV3d5s2bRWtGRkYGgiAuLi5tbW0vX760trYWltNoNH19/cePHy9ZskTVqVZxeXl5K1as6FvC4XDwCkZFHBwcMJhP4tSpU/n5+aGhoc7Ozqpua0hiYmJaWlrECsPDw1euXEnMHVI+n9/R0dHR0UGj0Wg02pgxYwAAu3fvDgkJMTc3xzs6dYMAAPoeNElLS2OxWNra2nl5eSiKCo+yCWlpaTU0NEivrrW1VUtLi0ajSX+ZpaWlcANKRWbOnJmYmNi3pKqq6tatW9KXUsX3AUEQ1WUfVX+Bq6urd+/ebWJiIsshCCJkk+bmZk1NolxC09vbm5OT8/Tp09zc3JKSkpqaGm1tbX19/e7u7q6uLh6PN2HChOrq6u+///7du3eTJ08etELse1ila6/q2mUwGAiTyWxraxM+fvLkSVJSUlhYGACgu7sb/H9XCgSC9vZ2KdU1NzdbWFjY2dnl5+dLb7iiokLuoIHKPmCUVLdBUfy+LYN246ZNmzgczr/+9a++J4umpqZKHLnDuPd8fHyEp56IYbPZhoaGGAQgpfeKi4t//PHH5ORkc3NzT0/PkJCQKVOmMBgMBPnjdFEOhzN37lxnZ+e3b98eP37cwMDgL3/5y/r164XbcRKRa/3EFxIXFxcWFmZoaPjhwweBQNDT0+Pp6QkAEK7KfbNme3u79DEBLS0tKysrOzs7FccMYeH69et379718/NbvHixqJDH4z19+pQIZyT4+vr2z2suLi7YJLWBFBYW7tmzJz8/PyQkJCcnR8plLc+ePWtra7t48SKFQhEIBDk5OZcuXZo4ceLKlSt3797d/9AhNDQoinK53KKiou7u7oSEBARBOjs7URTt7u4eOXJk34PTNBrt+fPneBwEFAfguIEyApZSQ1tbm7GxsY6OTnV1dd/yoqKi/fv3qyKYoeLz+WInHhkZGb19+xazAMTeckdHx5YtW8aPH3/mzJmuri7pyw50Im5dXV1oaCidTj9//rz05iDpNAEANBqNyWRSqdSnT5/OmDFDR0cHAEClUgMDA0V33q2oqGAwGDNnzsQq30J4ioyMrK+vj42NNTU17VuekJAgZUcJS5qamg8ePDh9+jQAwNnZedu2bcXFxbIcpVKFV69eOTg4cLnc4uLi0NDQQU//HuhEXGNj4zNnzvz888/nz5/39/dns9kqC1ndiTIcn8+3sLAIDw8XlbS2ts6bN+/mzZtZWVmLFy8WjiQQARj4tys7OxsA4O3tLVZeWFgIAHB2dpajTmJSPOCBasjKytLQ0Jg5c6Zw7gAhgUBw7NgxCoWSmJioimDkhlfTonZ/+umncePGXb9+XcYFOzs7TUxMXr58KeU1PB4vIiLC2tq6pKRErDlIFr931p49ezw9PSkUir29/Y4dO0RP9/b25ufnP3v2TLhzShASP+NXr14FBwezWCx9fX0jI6OgoKCoqCgURd+8ebNy5UonJyd9ff0xY8YEBARERETIWCeRqS6vzZ07FwAwbdo0X19fX1/fBQsWuLu7jx07VvhDmJqaqopg5IZvXjt37pyZmVlRUZHsC0ZFRQUHB8vyyri4uPHjx5eVlaEkXD/x9fuYWm9vr2iwpu//xKT4UCA2daqUUsZDlfWWcew9vJoWtpuYmOjh4SH7CWh1dXXTpk0rKCiQcZGCggJbW1sdHR3SrZ/4ImVnwbwGYF7Du2n52v373/8+YsSI2NhYbJobtgi9XQZJQdLLIYe5Xbt29T3XHVIRUv4IwO01pYDbayRqdxiun4ogykUnEARBygLzGgRB6oaUx9cQBFH6JaIEHwJWBSV24zDsPYjISLk69vT04B2COoDdqAhV/LhKbw6zttQAPBgJkRtZDqj3jZMsMZMXPL4GQZC6gXkNgiB1A/MaWQmn/4QgqD+4n09W8BiNEFn6Ad/jaxQKBcsZvREEwXdUipSDLKr4kHD/JCBIdXp7ezG+OgKztiQiZV5TxYeE+ycBQZCywONrEATJQyAQFBcX4x2FZDCvQRAkj/j4+IiICLyjkIwcx1zFwPk8AAkDVhGy9AO+4wZKb7Grq2vy5MnXr19nsVgYNDdUcHsNgqAhO3jwoLu7u8SkRgR/pFUURWtqauh0OpVKBQDweDzhPwQk8degq6urtraWSqUK7/jN4/H09PSMjIwAAFVVVb29vRQKBUVRHo9nZmbW/45BuP/CDBXpAlYRsvSDOm2vNTY2Tp06NT8/38LCAoPm5PD79lp2drafn196enpsbGxGRkZoaOjz58+HWld3d7e7u/uWLVuUHaRMmpubExISVq5caWZmZmZmtmLFCuE9qAAA165dmzFjhoWFRUBAwPnz56XftR6CIOl27dq1du3agZIaIaAoeuPGDRsbm8bGRuGtXAICAigUyufPn4d6D5jGxkYqlcpkMoe64FCBge/Nw+fz//znPwMA4uPj+5Zv2LAhMjJSvjqJSVdXF+8QCIEsH1zfOLGPWYktFhcXjx8/vq2tDZvm5APq6+v19PT63hRy1apVrq6uoof19fUxMTEyVldbW9vR0aHkGPuR3mvV1dX6+voGBgb19fXCksrKyoCAAEXqlBubzX7//r1AIFB6ze3t7Uqvk4wAACrqYeVSm7w2b968U6dOYdacfMC6det0dHS4XK6oyNraeufOnSiK/ve//921a1dwcDCDwcAvQgkG7bWLFy8CAPz8/FAUFQgE3333XW1trYJ1DlVxcbGTk5Nwo9jQ0FBs+xFSHLl6WD3yWnp6+qRJk3g8HjbNyQ2YmJgsWLBA9Li6uhoA8PjxY1HJrVu3SJfXUBT19vYGACQmJp4+ffrf//63UuqUXX19vYGBgdguP8G/eORCuh5Wg7zG5/OnT59+69YtbJpThGZdXZ2rq6tozcjIyEAQxMXFRYFDdoRw4cIFXV3drVu35uXlLV++HOPWY2JiWlpaxArDw8NRMozckQLsYezFxcXp6ur6+/vjHcjgEACAjY2N6HFaWhqLxdLW1pavutbWVi0tLRqNJv1llpaWlZWV8jUhI3Nz88OHD4eEhHR2dsq4iKovEW1ubhaeg6IUCIJgM0MDZg0pTrk9rHQaGhqiziTg9chdXV0vXrzIzs5+9+5dWVkZm83mcDgIglCpVGNjYwaDkZqaevjw4e7u7kG/4ECxN6jgKsdgMACTybxw4YJw4y0jI4NCoYiNG8q+H8pms7W1tR0dHZW9USkOyLaVe/jwYSsrKwBAUlKSsuqU0bx58yT2OJvNVmIrwxnpehgQdT+Ux+OlpKQsXrxYR0fH2dk5IiLi8uXL2dnZpaWldXV1Hz9+LCsry8zM9Pf3nzx5MovF0tfXX758+d27d/l8vhzNYQPk5eW5ubmlpKQcOnTowIEDAICHDx/2fYXsee3Lly9Tp05dsWKFakL9gyy9VlxcvGrVqsrKSh0dHSMjo0+fPilep+xOnTrV/yvn4uKixCaGOdL1MAHzWldX14kTJywsLDw8POLi4qScutHQ0DB27NjKykoURZuams6ePTtr1iwbG5tz58719PTI2ByWAIqiXC63qKiou7s7ISEBQZDOzs6+ryDjuEFPT4+vr6/wp/vs2bMAAIzP8+Dz+cKBCxEjI6O3b98qsYlhjnQ9TLS8lpqaOnHiRH9///z8/EEXX7t2bf/TP7OysubOnTtlypS0tLRBm8PY/zW/Zs2aWbNmib0iJSXF3Nwcw5AGN2ivRUdH3759W/i/QCD45ptvAAA3btxQpM6h4vP5p0+fBgA4Oztv27ZNdNqzsgw61q72hD08f/58FfWwchEnr33+/HnNmjW2trZ9T3uQQvqJuLdv37awsNi6dWtXV5fE5nDxR/N8Pt/CwkI4oiT09u3bPXv2zJkzZ/To0WFhYUePHsUjQgmk91pBQcHatWv7lpSXl2tra9PpdCkHX1T0SajuAx43bpyKaoZUgSB5raKiYsqUKatWreJwODIuO+iJuK2trQEBATNmzBCdCU+UvLZnzx5PT08KhWJvb79jxw58YxqUlF4rLy+X+EMUHR0NAFiyZIlwrt0h1akI1X3AuK860JAQIa+9fv3a1NR00KsF+kpPT7e1tZVl5+D777+3tLQsLy9HCbBy/t5834N/Eg8EEorEXrt27dqcOXMMDAy0tbXHjh3bd6/z0KFDpqamenp6enp6LBYrKCio/9WvMK9BKkWEvHb8+PHk5GTZlxKeiHvz5k0ZX3/jxo03b96gBFg5yTHHixgSzSupuglbcJ8KBhoSMs5TdOXKlQsXLmRmZmLTnBKR8rsB85pKa4ZUgYx5rby8fMSIEXLMR4T7yknK7wbMayqtGVIFMuY1sjTXH3EvOoEgCJIPzGsQBKkbUt4XGUEQpV82jCCk7AoIgvoj5Ze5p6cH7xAgCCIuUuY1CACwatUqvEOASEMVuzjSm8OsLYngmJpq4T4wBBEEvuOhQyUWIfEDFgPHDSAIUjcwr0EQpG7g8TWIKCgUCpYTjiMIAgeg1BXMa8ORijKIgplCONWKEuORjoB3GICUBea14UhFGQRmCogg4PE1SJ2hKAp3NochmNcgdfaPf/xDOKUoNKzAvEZWd+/exTsEoqurqzt58uT69evxDgTCGsxrytfT05OQkLBo0SIzMzMAwOjRo6dPn75z5873798rsRU/Pz8l1qaWoqKi/vrXv8oxfRhEdn+MG6AoWlNTQ6fTqVQqAIDH4wn/gYYkIyNjw4YN1tbWwcHBJ0+eNDc3r6ioeP/+/Z07d9zc3AICAg4fPjxy5Ei8w5Sgqqqqt7eXQqFoamoKBAIul2trayt6tre3t7y8nEajaWpqdnd30+l0XV1dHKMd1OvXr+/du1dSUoJ3IBAehNOBZ2Vl+fr6xsfH7927Nz09fePGjf3vCTgoLpfr5ua2efPmoS6oNi5dujR+/PhHjx6JSkCfid5bWlqWLVvm5OTU2tqqeFtAgSnkJS6bkJCwY8cObW1tAIC5ufnu3bv7PtvR0bF06VIAAJ1O37Bhw7t375QbkuKLi/H29j59+jRmzQ0K4Hp/g6ESi5D4AYsBKIreuHHDxsZGdPvFgIAACoXS/84mg2psbKRSqUwmU8kxksTPP/9sbGxcWlrat1BshRAIBFu3bvXx8eHz+Qo2p/S8JnTt2jUAAIvFEggEYk99/vx58uTJqrtXoRK/PA8ePJg0aZL0uyjBvCYF6fNafX29np5eYmKiqGjVqlWurq7C/+/du7dr167t27ffvHmz/4reX21tbUdHh6qCJTAul2tpaZmeni5W3n+F6O3t/frrr+Pi4hRsUUV5DUXR+fPnAwAuXLggVr5///7nz5+rKCTFFxfp7e2dOnWq6MbYqm5ORjCvYQmsW7dOR0eHy+WKiqytrXfu3ImiaGxs7K1btwQCAZvNdnd3X7ZsGX5xEt2PP/7o5+fXv1ziCpGbm8tgMGT5nZBCdXmtvLx81KhRBgYGTU1NosLS0tKNGzeqLiTFFxc5f/68h4cHZs3JCOY1LAETE5MFCxaIHldXVwMAHj9+3NPTY21tnZ+fLyx/8eIFAKCwsBCnOInO29tb4m0WB1ohpkyZIupb+agur6EoGhMTAwBYvXq1qCQoKKhvmlN6SIovLtTZ2WliYiJL38K8JgXZ85pmXV2dq6uraBghIyMDQRAXFxcEQdzc3EaMGCEsNzIyAgDU19crNEihvl6+fOnu7i776z08PPLz81UXj4LCw8MnT558+fLlrKwsAEBSUpKXl5dwHSC4I0eOzJ4929HREe9AIDwhAAAbGxvR47S0NBaLJRwUi4+PF5U/ePCATqf3zYAStba2amlp0Wg06S+ztLSsrKyUO2jZIQiC2RQRhoaGEsslXjWpq6srEAhCQ0MVaVF112NSqdSzZ89+8803oaGhGRkZ169fF44n4BiSSF1dXV5e3vv37ysrK1tbW7lcLoVC0dLSmjBhgqGh4fHjx1+9eiVjVRhf0KqhoSFaIYl/LW3faAG2ASv4tWUwGAiTyWxraxM+fvLkSVJSUlhYmNjrysrKjh49mpqaqqOjI6W65uZmCwsLOzu7QbdEKioq5A6agAQCwahRozgcDoVCEXtqoIlGt23bpqWlFRsbK3ejwrPM5FtWlnXU09NzxYoViYmJrq6u165dk3G1lvhmlRLVL7/8cuXKldTU1ObmZicnJzs7OyaTaWhoSKPRenp6uFzux48fz507R6VSHRwcPDw8AgIC/P39pZ9kp0i0QwXny8VUXl6em5tbSkrKoUOHDhw4AAB4+PBh3z3Vjx8/ent7v3nzZtB92i9fvkydOnXFihXK310mPCsrq5KSkv7lYIADE0uWLPnPf/6jSIuZmZlyLztQVGLevn0LAPD391dutUNanM/nX7t2zdHR0draOioqqrCwcKDxlsLCQjqd3tbW1tLScuXKlYULFxoaGoaFhX38+FEV0Q4VgMfXMARQFOVyuUVFRd3d3QkJCQiCdHZ2ip6uqqpav359S0sLiqIfPnz49ddfcYuU2EJCQo4cOdK/XOIKweVyx4wZ8+nTJ9XHJZmMq6nwWEFQUJByq5V98aysrK+++srFxeX27duDDh/3PxH348eP4eHhRkZGUVFRHA5HudEOFcxrWPq/cNesWTNr1izRw8rKSn9//4yMjKysrMzMzM2bN0vcJIFQFH3x4oW5ufmXL1/EyiWuEMeOHZN9I0gViJ/Xurq6Nm3aZGZmdvXqVVmWlXIibnV19fLly62trXNzc5UY7VDBvIalP8Ll8/kWFhbh4eHCh1wul8Fg9N1jpVKpwvkIIYkCAwP/9re/iRX2XyFKSkrGjRv322+/YRSWJATPaxUVFX/6058CAwPb29tlWVCWE3FTUlLodPqJEyeUFe1QwbyGpd/D3bNnj6enJ4VCsbe337FjB74xkVRra+ukSZNiYmL6FoqtEKWlpTY2NpcuXcI2NHEyrqaFhYUAAB8fH+VWK33xwsJCU1PTkydPyr6gjCfiVlVV2dvbb9++XXgRG8xrUqhJXuvp6REV9f0fGpKamhoWi+Xn5yfaYRetEDwe78yZM3Q6vf/1SdgbdDV98+bNypUrnZyc9PX1jYyMli1btnfvXsWrlWXxOXPmJCcny76U7Cfioija2toaHBwsPLIJ85oUZM9rZBu+Jbzu7u6TJ08ePnzYxsbG3d39n//857Zt26qqqu7fv+/o6Hjw4MGpU6fiHaOqhu0VrFa+xaOjo0tLS69cuYJNc3KD53lgiWThkkVPT8/Tp09fvXqVlpY2bdq0KVOm+Pj4mJqa4h3X79Qpr8XFxc2bN2/ChAnYNCc3mNewRLJwIaVQp7xGxuaInybIntfgPOBktWjRIrxDgCCCIlkahkQU+QmF22v4Nkf8zR+4vQZBEEQs8H7vwxGCIKqYngFB4OoEEQJcEYcjYt4CXUXZVkpzmLUFYQx+tBBRDDXbkuuIFYQleHwNgiB1A/MaBEHqBuY1CILUDcxrEASpG5jXyEpsdjwIgkTgKBJEVuQaDyVvtP0fEh/Rt9cePHjQ2dmJdxQQBJEJofMaiqLh4eHEv9MihBmBQLBv3z4p2w4oiu7bt0/uOxAqF4wWL4TOa8+fP3dwcJB+01JoWNHU1Ozo6Pjhhx8GekFsbGxnZ6emJiFWbBgtbpQ6+66SrVu37tGjR3hHARELj8f7+uuvnz59CvrNrP3kyZOvv/5a4l2p8KIG0aIoCgAgYLRSEDevdXV12dnZwTtgQf1VVVUxmUyxTNHQ0MBkMge6CzKOyB4tiqIAAGJGOxBZ81ppaemTJ08aGxtVGk1fycnJYWFhmDUHkUtqauqoUaNEN0tmMBheXl737t3DN6qBkDpagUAwatQowkYr0eC7ypmZmSwWKyMjAwBw9uzZqKiogQ4cdnd3u7u7b9myRdF9YwAAAImJicHBwUqpClI/CxYsCAwMvHfvnvDhiRMnzMzM5s+fj29UAyF1tHfv3g0KCiJstJJJT3uZmZkIghQUFAgf3rp1S1tbOy0tTeKLGxsbqVQqk8lUPN02NTXNmDFD8XogNVZSUuLq6ir838XF5f379/jGIx2MFkuD5DV7e/u+t8VNS0v76quv3r17N9Dra2trOzo6Bm0Vs3PlcZ9jS3UBYPbWcO9D6UaMGIF3CEMAo5WFgqscg8GQlteqq6sBALgc5HJycqqtrcW+XYhcXr9+PXfuXC8vr9evX+Mdy+BgtJiRlhc/fPgAABg/frwiuVMOJSUlenp6JiYmGLcLkc7UqVO5XK6mpiYR7jY9KBgtZqTlNRsbGwCAcKsNS4mJiStWrMC4UYikjhw5QqIrUmC02BjkctZp06aNHj362bNnohIej/fo0aOFCxdKfH1ra6uWlhaNRpM7IBRFp02blpubq62tLXclEAQNa9J3U3NzcxEEuX//vqjk5MmT+fn5El/MZrO1tbUdHR0H3fuF4wZErhmvhuRD8PDEwGgxaJfBYAyy/KxZs7KysjZt2pSdnS0cCbW3t3d0dJT4Yi0tLSsrKzs7u0EbrqioGOip9evXBwYGenl5iZW/ePHi7du3AoGgrKzs22+/ZbFYg7YCQdDwJOu0So2NjW1tbba2tird3+7u7nZwcCgqKup/ba2Pj09kZKSnp+fVq1dPnDiRk5OjujAgCCI1Wbf36HQ6nU5XaSgAgDt37vj6+kqcMOCnn37S19cHAKSlpfn7+6s6EgiCyItYU45IGQkdM2ZMWVnZ3r17m5ub16xZg3FgEASRCIGm92Wz2fPnz8/Ly5P+sqysrMWLF3/48EFPTw+bwCAIIhcCba8lJSUFBQVJfIrNZk+YMIHL5QIALCwsmpqampubsY0OgiDSINCoc2pq6uXLlyU+ZWBgMH/+/Dt37hgaGp47dy46OtrS0hLb6CAIIg0C7Yd2dHRI37XkcDilpaUMBmPMmDGYRQURU3Z2dk5OTlNTU1VVVWRk5PTp0/GOSJqGhobk5OTx48c3NTUtXLjQ3Nwc74ikqaioeP78+YULF5KTk42NjfEORy6yXkgKQYTB5/OnT5/+5csXFEVzc3PpdDqfz8c7KGm8vb2F8ziw2ezZs2fjHc4g6urq6uvrmUxmZWUl3rHIiUDH1yBIRpqamqtWrRKelW5sbMxms7u6uvAOakAtLS35+fnCeRwMDQ0/fPhQU1ODd1DSGBsbYz/bhXLBvAaR0tatWykUCgDgwIED+/btI/LVxLW1tX0PsIwePZrgeU0NEGjcAIKGRCAQREdHu7u7DzSMThA6OjocDkf0kMPhwFtHqhrcXoNI6fPnzwcOHAgODg4MDDx06JDwHCBisrS01NbW5vF4AADhzVBkuYYaUgSBxkMhSEY9PT2zZs365ZdfhA9tbW1LSkrwDUm6x48f5+XlLVq06P79+zY2Nt9++y3eEUlTUFCQnp5+9OjRZcuWOTs7L126FO+Ihux/IleGjh4uOTYAAAAASUVORK5CYII=\n",
+                        "image/png": "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",
                         "text/plain": [
-                            "<PIL.Image.Image image mode=RGB size=413x138>"
+                            "<PIL.Image.Image image mode=RGB size=413x138 at 0x251F2C06A90>"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -230,15 +241,15 @@
         {
             "cell_type": "markdown",
             "id": "9865f7d5",
             "metadata": {},
             "source": [
                 "## Retrieve circuit properties\n",
                 "\n",
-                "Depth blabla"
+                "One can also retrieve different properties of the circuit, including the depth, the size (quantum and classical bits), counting (specific) gates and retrieving the attached measurements."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "8e75255d",
             "metadata": {},
@@ -324,20 +335,20 @@
         {
             "cell_type": "markdown",
             "id": "bf37b06b",
             "metadata": {},
             "source": [
                 "## Combination of circuits\n",
                 "\n",
-                "babpabababllba"
+                "We also allow combinations of circuits. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 7,
             "id": "1656b928",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -362,20 +373,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "68ef12e4",
             "metadata": {},
             "source": [
-                "``append``"
+                "One can ``append`` a circuit to another, consisting in concatenating the circuit horizontally at the right of the first one. For more simplicity, the ``+`` realized the same operation. When the size does not match, we automatically adjust the size of the resulting circuit."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 8,
             "id": "ff7fda3c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -393,20 +404,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c70512be",
             "metadata": {},
             "source": [
-                "``tensor``"
+                "One can also take the tensor product of two circuits using the method ``tensor``, or the symbol ``@``, which will concatenate the second circuit vertically under the first."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 9,
             "id": "872b2174",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -426,91 +437,141 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "54598610",
             "metadata": {},
             "source": [
-                "## Translating the circuit"
+                "## Translating the circuit\n",
+                "\n",
+                "MPQP is a multi-platform quantum programming library and handles for the user the translation of circuits. We allow the user to use a function to export the circuit in different objects specific to each SDK using the method ``to_other_language``. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 10,
             "id": "a35b512d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<qiskit.circuit.quantumcircuit.QuantumCircuit at 0x24f83150190>"
+                            "<qiskit.circuit.quantumcircuit.QuantumCircuit at 0x2186bf40a90>"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from mpqp import Language\n",
+                "\n",
                 "circ3.to_other_language(Language.QISKIT)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 11,
             "id": "2869a46e",
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "Circuit(ops=[Op(gate='H', qbits=[0], type=0, cbits=None, formula=None, remap=None), Op(gate='X', qbits=[1], type=0, cbits=None, formula=None, remap=None), Op(gate='CNOT', qbits=[1, 2], type=0, cbits=None, formula=None, remap=None), Op(gate='Y', qbits=[2], type=0, cbits=None, formula=None, remap=None), Op(gate='Z', qbits=[0], type=0, cbits=None, formula=None, remap=None), Op(gate='CSIGN', qbits=[1, 0], type=0, cbits=None, formula=None, remap=None)], name=None, gateDic={'X': GateDefinition(name='X', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='X', parameters=[]), nbctrls=None, circuit_implementation=None), 'Y': GateDefinition(name='Y', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=-0.0, im=-1.0), ComplexNumber(re=0.0, im=1.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='Y', parameters=[]), nbctrls=None, circuit_implementation=None), 'Z': GateDefinition(name='Z', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=-1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='Z', parameters=[]), nbctrls=None, circuit_implementation=None), 'H': GateDefinition(name='H', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=0.7071067811865475, im=0.0), ComplexNumber(re=0.7071067811865475, im=0.0), ComplexNumber(re=0.7071067811865475, im=0.0), ComplexNumber(re=-0.7071067811865475, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='H', parameters=[]), nbctrls=None, circuit_implementation=None), 'CNOT': GateDefinition(name='CNOT', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=True, is_dag=None, is_trans=None, is_conj=None, subgate='X', syntax=GSyntax(name='CNOT', parameters=[]), nbctrls=1, circuit_implementation=None), 'CSIGN': GateDefinition(name='CSIGN', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=-1.0, im=0.0)]), is_ctrl=True, is_dag=None, is_trans=None, is_conj=None, subgate='Z', syntax=GSyntax(name='CSIGN', parameters=[]), nbctrls=1, circuit_implementation=None), 'ISWAP': GateDefinition(name='ISWAP', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=1.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=1.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='ISWAP', parameters=[]), nbctrls=None, circuit_implementation=None), 'SQRTSWAP': GateDefinition(name='SQRTSWAP', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.5, im=0.5), ComplexNumber(re=0.5, im=-0.5), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.5, im=-0.5), ComplexNumber(re=0.5, im=0.5), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='SQRTSWAP', parameters=[]), nbctrls=None, circuit_implementation=None), 'I': GateDefinition(name='I', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='I', parameters=[]), nbctrls=None, circuit_implementation=None), 'SWAP': GateDefinition(name='SWAP', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='SWAP', parameters=[]), nbctrls=None, circuit_implementation=None), 'CCNOT': GateDefinition(name='CCNOT', arity=3, matrix=Matrix(nRows=8, nCols=8, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=True, is_dag=None, is_trans=None, is_conj=None, subgate='CNOT', syntax=GSyntax(name='CCNOT', parameters=[]), nbctrls=1, circuit_implementation=None), 'S': GateDefinition(name='S', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=1.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='S', parameters=[]), nbctrls=None, circuit_implementation=None), 'T': GateDefinition(name='T', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.7071067811865476, im=0.7071067811865476)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='T', parameters=[]), nbctrls=None, circuit_implementation=None)}, nbqbits=3, nbcbits=0, _gate_set=GateSet(gate_signatures={'X': GateSignature(name='X', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_x at 0x0000024FEBF2ABA0>, circuit_generator=None), 'Y': GateSignature(name='Y', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_y at 0x0000024FEBF2AC70>, circuit_generator=None), 'Z': GateSignature(name='Z', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_z at 0x0000024FEBF2AD40>, circuit_generator=None), 'H': GateSignature(name='H', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_h at 0x0000024FEBF2AAD0>, circuit_generator=None), 'CNOT': GateSignature(name='CNOT', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_cnot at 0x0000024FEBF2C110>, circuit_generator=None), 'CSIGN': GateSignature(name='CSIGN', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_csign at 0x0000024FEBF2C1E0>, circuit_generator=None), 'ISWAP': GateSignature(name='ISWAP', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_iswap at 0x0000024FEBF2C450>, circuit_generator=None), 'SQRTSWAP': GateSignature(name='SQRTSWAP', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_sqrtswap at 0x0000024FEBF2C380>, circuit_generator=None), 'I': GateSignature(name='I', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_i at 0x0000024FEBF2AE10>, circuit_generator=None), 'SWAP': GateSignature(name='SWAP', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_swap at 0x0000024FEBF2C2B0>, circuit_generator=None), 'CCNOT': GateSignature(name='CCNOT', parameters=[], arity=3, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_ccnot at 0x0000024FEBF2C520>, circuit_generator=None), 'S': GateSignature(name='S', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_s at 0x0000024FEBF2AEE0>, circuit_generator=None), 'T': GateSignature(name='T', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_t at 0x0000024FEBF2C040>, circuit_generator=None), 'PH': GateSignature(name='PH', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_ph at 0x0000024FEBF2A5F0>, circuit_generator=None), 'RZ': GateSignature(name='RZ', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_rz at 0x0000024FEBF2A6C0>, circuit_generator=None), 'RX': GateSignature(name='RX', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_rx at 0x0000024FEBF2A860>, circuit_generator=None), 'RY': GateSignature(name='RY', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_ry at 0x0000024FEBF2A790>, circuit_generator=None), 'U': AbstractGate(name='U', parameters=[1, 1, 1], arity=1, nb_args=3, arg_types=[<class 'float'>, <class 'float'>, <class 'float'>], arity_generator=None, matrix_generator=<function gen_U at 0x0000024F80B85940>, circuit_generator=None, dag_func=None), 'U1': AbstractGate(name='U1', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<function gen_u1 at 0x0000024F80C6FAF0>, circuit_generator=None, dag_func=None), 'U2': AbstractGate(name='U2', parameters=[1, 1], arity=1, nb_args=2, arg_types=[<class 'float'>, <class 'float'>], arity_generator=None, matrix_generator=<function gen_u2 at 0x0000024F80C6FB80>, circuit_generator=None, dag_func=None), 'U3': AbstractGate(name='U3', parameters=[1, 1, 1], arity=1, nb_args=3, arg_types=[<class 'float'>, <class 'float'>, <class 'float'>], arity_generator=None, matrix_generator=<function gen_U at 0x0000024F80B85940>, circuit_generator=None, dag_func=None)}), has_matrices=True, var_dic={}, qregs=[], ancilla_map=None, _serialized_gate_set=b\"\\x80\\x04\\x95?\\x06\\x00\\x00\\x00\\x00\\x00\\x00\\x8c\\x11qat.core.gate_set\\x94\\x8c\\x07GateSet\\x94\\x93\\x94)\\x81\\x94}\\x94\\x8c\\x0fgate_signatures\\x94}\\x94(\\x8c\\x01X\\x94h\\x00\\x8c\\rGateSignature\\x94\\x93\\x94)\\x81\\x94}\\x94(\\x8c\\x04name\\x94h\\x07\\x8c\\nparameters\\x94]\\x94\\x8c\\x05arity\\x94K\\x01\\x8c\\x07nb_args\\x94K\\x00\\x8c\\targ_types\\x94]\\x94\\x8c\\x0farity_generator\\x94N\\x8c\\x10matrix_generator\\x94\\x8c$qat.core.circuit_builder.matrix_util\\x94\\x8c\\x05gen_x\\x94\\x93\\x94\\x8c\\x11circuit_generator\\x94Nub\\x8c\\x01Y\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch\\x19h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_y\\x94\\x93\\x94h\\x18Nub\\x8c\\x01Z\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_z\\x94\\x93\\x94h\\x18Nub\\x8c\\x01H\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch'h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_h\\x94\\x93\\x94h\\x18Nub\\x8c\\x04CNOT\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch.h\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x08gen_cnot\\x94\\x93\\x94h\\x18Nub\\x8c\\x05CSIGN\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch5h\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\tgen_csign\\x94\\x93\\x94h\\x18Nub\\x8c\\x05ISWAP\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch<h\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\tgen_iswap\\x94\\x93\\x94h\\x18Nub\\x8c\\x08SQRTSWAP\\x94h\\t)\\x81\\x94}\\x94(h\\x0chCh\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x0cgen_sqrtswap\\x94\\x93\\x94h\\x18Nub\\x8c\\x01I\\x94h\\t)\\x81\\x94}\\x94(h\\x0chJh\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_i\\x94\\x93\\x94h\\x18Nub\\x8c\\x04SWAP\\x94h\\t)\\x81\\x94}\\x94(h\\x0chQh\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x08gen_swap\\x94\\x93\\x94h\\x18Nub\\x8c\\x05CCNOT\\x94h\\t)\\x81\\x94}\\x94(h\\x0chXh\\r]\\x94h\\x0fK\\x03h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\tgen_ccnot\\x94\\x93\\x94h\\x18Nub\\x8c\\x01S\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch_h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_s\\x94\\x93\\x94h\\x18Nub\\x8c\\x01T\\x94h\\t)\\x81\\x94}\\x94(h\\x0chfh\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_t\\x94\\x93\\x94h\\x18Nub\\x8c\\x02PH\\x94h\\t)\\x81\\x94}\\x94(h\\x0chmh\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94\\x8c\\ndill._dill\\x94\\x8c\\n_load_type\\x94\\x93\\x94\\x8c\\x05float\\x94\\x85\\x94R\\x94ah\\x13Nh\\x14h\\x15\\x8c\\x06gen_ph\\x94\\x93\\x94h\\x18Nub\\x8c\\x02RZ\\x94h\\t)\\x81\\x94}\\x94(h\\x0chzh\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x15\\x8c\\x06gen_rz\\x94\\x93\\x94h\\x18Nub\\x8c\\x02RX\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch\\x81h\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x15\\x8c\\x06gen_rx\\x94\\x93\\x94h\\x18Nub\\x8c\\x02RY\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch\\x88h\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x15\\x8c\\x06gen_ry\\x94\\x93\\x94h\\x18Nub\\x8c\\x01U\\x94\\x8c\\x14qat.lang.AQASM.gates\\x94\\x8c\\x0cAbstractGate\\x94\\x93\\x94)\\x81\\x94}\\x94(h\\x0ch\\x8fh\\r]\\x94(K\\x01K\\x01K\\x01eh\\x0fK\\x01h\\x10K\\x03h\\x11]\\x94(hwhwhweh\\x13Nh\\x14\\x8c qat.interop.openqasm.qasm_parser\\x94\\x8c\\x05gen_U\\x94\\x93\\x94h\\x18N\\x8c\\x08dag_func\\x94Nub\\x8c\\x02U1\\x94h\\x92)\\x81\\x94}\\x94(h\\x0ch\\x9bh\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x97\\x8c\\x06gen_u1\\x94\\x93\\x94h\\x18Nh\\x9aNub\\x8c\\x02U2\\x94h\\x92)\\x81\\x94}\\x94(h\\x0ch\\xa2h\\r]\\x94(K\\x01K\\x01eh\\x0fK\\x01h\\x10K\\x02h\\x11]\\x94(hwhweh\\x13Nh\\x14h\\x97\\x8c\\x06gen_u2\\x94\\x93\\x94h\\x18Nh\\x9aNub\\x8c\\x02U3\\x94h\\x92)\\x81\\x94}\\x94(h\\x0ch\\xa9h\\r]\\x94(K\\x01K\\x01K\\x01eh\\x0fK\\x01h\\x10K\\x03h\\x11]\\x94(hwhwhweh\\x13Nh\\x14h\\x99h\\x18Nh\\x9aNubusb.\")"
+                            "Circuit(ops=[Op(gate='H', qbits=[0], type=0, cbits=None, formula=None, remap=None), Op(gate='X', qbits=[1], type=0, cbits=None, formula=None, remap=None), Op(gate='CNOT', qbits=[1, 2], type=0, cbits=None, formula=None, remap=None), Op(gate='Y', qbits=[2], type=0, cbits=None, formula=None, remap=None), Op(gate='Z', qbits=[0], type=0, cbits=None, formula=None, remap=None), Op(gate='CSIGN', qbits=[1, 0], type=0, cbits=None, formula=None, remap=None)], name=None, gateDic={'X': GateDefinition(name='X', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='X', parameters=[]), nbctrls=None, circuit_implementation=None), 'Y': GateDefinition(name='Y', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=-0.0, im=-1.0), ComplexNumber(re=0.0, im=1.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='Y', parameters=[]), nbctrls=None, circuit_implementation=None), 'Z': GateDefinition(name='Z', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=-1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='Z', parameters=[]), nbctrls=None, circuit_implementation=None), 'H': GateDefinition(name='H', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=0.7071067811865475, im=0.0), ComplexNumber(re=0.7071067811865475, im=0.0), ComplexNumber(re=0.7071067811865475, im=0.0), ComplexNumber(re=-0.7071067811865475, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='H', parameters=[]), nbctrls=None, circuit_implementation=None), 'CNOT': GateDefinition(name='CNOT', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=True, is_dag=None, is_trans=None, is_conj=None, subgate='X', syntax=GSyntax(name='CNOT', parameters=[]), nbctrls=1, circuit_implementation=None), 'CSIGN': GateDefinition(name='CSIGN', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=-1.0, im=0.0)]), is_ctrl=True, is_dag=None, is_trans=None, is_conj=None, subgate='Z', syntax=GSyntax(name='CSIGN', parameters=[]), nbctrls=1, circuit_implementation=None), 'ISWAP': GateDefinition(name='ISWAP', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=1.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=1.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='ISWAP', parameters=[]), nbctrls=None, circuit_implementation=None), 'SQRTSWAP': GateDefinition(name='SQRTSWAP', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.5, im=0.5), ComplexNumber(re=0.5, im=-0.5), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.5, im=-0.5), ComplexNumber(re=0.5, im=0.5), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='SQRTSWAP', parameters=[]), nbctrls=None, circuit_implementation=None), 'I': GateDefinition(name='I', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='I', parameters=[]), nbctrls=None, circuit_implementation=None), 'SWAP': GateDefinition(name='SWAP', arity=2, matrix=Matrix(nRows=4, nCols=4, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='SWAP', parameters=[]), nbctrls=None, circuit_implementation=None), 'CCNOT': GateDefinition(name='CCNOT', arity=3, matrix=Matrix(nRows=8, nCols=8, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0)]), is_ctrl=True, is_dag=None, is_trans=None, is_conj=None, subgate='CNOT', syntax=GSyntax(name='CCNOT', parameters=[]), nbctrls=1, circuit_implementation=None), 'S': GateDefinition(name='S', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=1.0)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='S', parameters=[]), nbctrls=None, circuit_implementation=None), 'T': GateDefinition(name='T', arity=1, matrix=Matrix(nRows=2, nCols=2, data=[ComplexNumber(re=1.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.0, im=0.0), ComplexNumber(re=0.7071067811865476, im=0.7071067811865476)]), is_ctrl=False, is_dag=None, is_trans=None, is_conj=None, subgate=None, syntax=GSyntax(name='T', parameters=[]), nbctrls=None, circuit_implementation=None)}, nbqbits=3, nbcbits=0, _gate_set=GateSet(gate_signatures={'X': GateSignature(name='X', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_x at 0x000002186CACCA00>, circuit_generator=None), 'Y': GateSignature(name='Y', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_y at 0x000002186CACCAD0>, circuit_generator=None), 'Z': GateSignature(name='Z', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_z at 0x000002186CACCBA0>, circuit_generator=None), 'H': GateSignature(name='H', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_h at 0x000002186CACC930>, circuit_generator=None), 'CNOT': GateSignature(name='CNOT', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_cnot at 0x000002186CACCEE0>, circuit_generator=None), 'CSIGN': GateSignature(name='CSIGN', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_csign at 0x000002186CAD7040>, circuit_generator=None), 'ISWAP': GateSignature(name='ISWAP', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_iswap at 0x000002186CAD72B0>, circuit_generator=None), 'SQRTSWAP': GateSignature(name='SQRTSWAP', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_sqrtswap at 0x000002186CAD71E0>, circuit_generator=None), 'I': GateSignature(name='I', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_i at 0x000002186CACCC70>, circuit_generator=None), 'SWAP': GateSignature(name='SWAP', parameters=[], arity=2, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_swap at 0x000002186CAD7110>, circuit_generator=None), 'CCNOT': GateSignature(name='CCNOT', parameters=[], arity=3, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_ccnot at 0x000002186CAD7380>, circuit_generator=None), 'S': GateSignature(name='S', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_s at 0x000002186CACCD40>, circuit_generator=None), 'T': GateSignature(name='T', parameters=[], arity=1, nb_args=0, arg_types=[], arity_generator=None, matrix_generator=<cyfunction gen_t at 0x000002186CACCE10>, circuit_generator=None), 'PH': GateSignature(name='PH', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_ph at 0x000002186CACC450>, circuit_generator=None), 'RZ': GateSignature(name='RZ', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_rz at 0x000002186CACC520>, circuit_generator=None), 'RX': GateSignature(name='RX', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_rx at 0x000002186CACC6C0>, circuit_generator=None), 'RY': GateSignature(name='RY', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<cyfunction gen_ry at 0x000002186CACC5F0>, circuit_generator=None), 'U': AbstractGate(name='U', parameters=[1, 1, 1], arity=1, nb_args=3, arg_types=[<class 'float'>, <class 'float'>, <class 'float'>], arity_generator=None, matrix_generator=<function gen_U at 0x000002186CD04040>, circuit_generator=None, dag_func=None), 'U1': AbstractGate(name='U1', parameters=[1], arity=1, nb_args=1, arg_types=[<class 'float'>], arity_generator=None, matrix_generator=<function gen_u1 at 0x000002186CDC6670>, circuit_generator=None, dag_func=None), 'U2': AbstractGate(name='U2', parameters=[1, 1], arity=1, nb_args=2, arg_types=[<class 'float'>, <class 'float'>], arity_generator=None, matrix_generator=<function gen_u2 at 0x000002186CDC6700>, circuit_generator=None, dag_func=None), 'U3': AbstractGate(name='U3', parameters=[1, 1, 1], arity=1, nb_args=3, arg_types=[<class 'float'>, <class 'float'>, <class 'float'>], arity_generator=None, matrix_generator=<function gen_U at 0x000002186CD04040>, circuit_generator=None, dag_func=None)}), has_matrices=True, var_dic={}, qregs=[], ancilla_map=None, _serialized_gate_set=b\"\\x80\\x04\\x95?\\x06\\x00\\x00\\x00\\x00\\x00\\x00\\x8c\\x11qat.core.gate_set\\x94\\x8c\\x07GateSet\\x94\\x93\\x94)\\x81\\x94}\\x94\\x8c\\x0fgate_signatures\\x94}\\x94(\\x8c\\x01X\\x94h\\x00\\x8c\\rGateSignature\\x94\\x93\\x94)\\x81\\x94}\\x94(\\x8c\\x04name\\x94h\\x07\\x8c\\nparameters\\x94]\\x94\\x8c\\x05arity\\x94K\\x01\\x8c\\x07nb_args\\x94K\\x00\\x8c\\targ_types\\x94]\\x94\\x8c\\x0farity_generator\\x94N\\x8c\\x10matrix_generator\\x94\\x8c$qat.core.circuit_builder.matrix_util\\x94\\x8c\\x05gen_x\\x94\\x93\\x94\\x8c\\x11circuit_generator\\x94Nub\\x8c\\x01Y\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch\\x19h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_y\\x94\\x93\\x94h\\x18Nub\\x8c\\x01Z\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_z\\x94\\x93\\x94h\\x18Nub\\x8c\\x01H\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch'h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_h\\x94\\x93\\x94h\\x18Nub\\x8c\\x04CNOT\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch.h\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x08gen_cnot\\x94\\x93\\x94h\\x18Nub\\x8c\\x05CSIGN\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch5h\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\tgen_csign\\x94\\x93\\x94h\\x18Nub\\x8c\\x05ISWAP\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch<h\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\tgen_iswap\\x94\\x93\\x94h\\x18Nub\\x8c\\x08SQRTSWAP\\x94h\\t)\\x81\\x94}\\x94(h\\x0chCh\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x0cgen_sqrtswap\\x94\\x93\\x94h\\x18Nub\\x8c\\x01I\\x94h\\t)\\x81\\x94}\\x94(h\\x0chJh\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_i\\x94\\x93\\x94h\\x18Nub\\x8c\\x04SWAP\\x94h\\t)\\x81\\x94}\\x94(h\\x0chQh\\r]\\x94h\\x0fK\\x02h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x08gen_swap\\x94\\x93\\x94h\\x18Nub\\x8c\\x05CCNOT\\x94h\\t)\\x81\\x94}\\x94(h\\x0chXh\\r]\\x94h\\x0fK\\x03h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\tgen_ccnot\\x94\\x93\\x94h\\x18Nub\\x8c\\x01S\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch_h\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_s\\x94\\x93\\x94h\\x18Nub\\x8c\\x01T\\x94h\\t)\\x81\\x94}\\x94(h\\x0chfh\\r]\\x94h\\x0fK\\x01h\\x10K\\x00h\\x11]\\x94h\\x13Nh\\x14h\\x15\\x8c\\x05gen_t\\x94\\x93\\x94h\\x18Nub\\x8c\\x02PH\\x94h\\t)\\x81\\x94}\\x94(h\\x0chmh\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94\\x8c\\ndill._dill\\x94\\x8c\\n_load_type\\x94\\x93\\x94\\x8c\\x05float\\x94\\x85\\x94R\\x94ah\\x13Nh\\x14h\\x15\\x8c\\x06gen_ph\\x94\\x93\\x94h\\x18Nub\\x8c\\x02RZ\\x94h\\t)\\x81\\x94}\\x94(h\\x0chzh\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x15\\x8c\\x06gen_rz\\x94\\x93\\x94h\\x18Nub\\x8c\\x02RX\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch\\x81h\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x15\\x8c\\x06gen_rx\\x94\\x93\\x94h\\x18Nub\\x8c\\x02RY\\x94h\\t)\\x81\\x94}\\x94(h\\x0ch\\x88h\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x15\\x8c\\x06gen_ry\\x94\\x93\\x94h\\x18Nub\\x8c\\x01U\\x94\\x8c\\x14qat.lang.AQASM.gates\\x94\\x8c\\x0cAbstractGate\\x94\\x93\\x94)\\x81\\x94}\\x94(h\\x0ch\\x8fh\\r]\\x94(K\\x01K\\x01K\\x01eh\\x0fK\\x01h\\x10K\\x03h\\x11]\\x94(hwhwhweh\\x13Nh\\x14\\x8c qat.interop.openqasm.qasm_parser\\x94\\x8c\\x05gen_U\\x94\\x93\\x94h\\x18N\\x8c\\x08dag_func\\x94Nub\\x8c\\x02U1\\x94h\\x92)\\x81\\x94}\\x94(h\\x0ch\\x9bh\\r]\\x94K\\x01ah\\x0fK\\x01h\\x10K\\x01h\\x11]\\x94hwah\\x13Nh\\x14h\\x97\\x8c\\x06gen_u1\\x94\\x93\\x94h\\x18Nh\\x9aNub\\x8c\\x02U2\\x94h\\x92)\\x81\\x94}\\x94(h\\x0ch\\xa2h\\r]\\x94(K\\x01K\\x01eh\\x0fK\\x01h\\x10K\\x02h\\x11]\\x94(hwhweh\\x13Nh\\x14h\\x97\\x8c\\x06gen_u2\\x94\\x93\\x94h\\x18Nh\\x9aNub\\x8c\\x02U3\\x94h\\x92)\\x81\\x94}\\x94(h\\x0ch\\xa9h\\r]\\x94(K\\x01K\\x01K\\x01eh\\x0fK\\x01h\\x10K\\x03h\\x11]\\x94(hwhwhweh\\x13Nh\\x14h\\x99h\\x18Nh\\x9aNubusb.\")"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "circ3.to_other_language(Language.MY_QLM)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 12,
             "id": "4dbea0c8",
-            "metadata": {},
+            "metadata": {
+                "scrolled": false
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "This program uses OpenQASM language features that may not be supported on QPUs or on-demand simulators.\n"
+                        "c:\\Users\\JulienCalisto\\Documents\\MPQP_main_repo\\mpqp\\.venv\\lib\\site-packages\\mpqp\\qasm\\qasm_to_braket.py:80: UnsupportedBraketFeaturesWarning: \n",
+                        "This program uses OpenQASM language features that may not be supported on QPUs or on-demand simulators.\n",
+                        "  warnings.warn(\n",
+                        "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "Circuit('instructions': [Instruction('operator': H('qubit_count': 1), 'target': QubitSet([Qubit(0)]), 'control': QubitSet([]), 'control_state': (), 'power': 1), Instruction('operator': X('qubit_count': 1), 'target': QubitSet([Qubit(1)]), 'control': QubitSet([]), 'control_state': (), 'power': 1), Instruction('operator': CNot('qubit_count': 2), 'target': QubitSet([Qubit(1), Qubit(2)]), 'control': QubitSet([]), 'control_state': (), 'power': 1), Instruction('operator': Y('qubit_count': 1), 'target': QubitSet([Qubit(2)]), 'control': QubitSet([]), 'control_state': (), 'power': 1), Instruction('operator': Z('qubit_count': 1), 'target': QubitSet([Qubit(0)]), 'control': QubitSet([]), 'control_state': (), 'power': 1), Instruction('operator': CZ('qubit_count': 2), 'target': QubitSet([Qubit(1), Qubit(0)]), 'control': QubitSet([]), 'control_state': (), 'power': 1)])"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "circ3.to_other_language(Language.BRAKET)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 13,
+            "id": "99135941",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<pre style=\"overflow: auto; white-space: pre;\">q_0: \u2500\u2500\u2500H\u2500\u2500\u2500Z\u2500\u2500\u2500@\u2500\u2500\u2500M(&#x27;c_0&#x27;)\u2500\u2500\u2500\n",
+                            "                \u2502\n",
+                            "q_1: \u2500\u2500\u2500X\u2500\u2500\u2500@\u2500\u2500\u2500@\u2500\u2500\u2500M(&#x27;c_1&#x27;)\u2500\u2500\u2500\n",
+                            "            \u2502\n",
+                            "q_2: \u2500\u2500\u2500\u2500\u2500\u2500\u2500X\u2500\u2500\u2500Y\u2500\u2500\u2500M(&#x27;c_2&#x27;)\u2500\u2500\u2500</pre>"
+                        ],
+                        "text/plain": [
+                            "q_0: \u2500\u2500\u2500H\u2500\u2500\u2500Z\u2500\u2500\u2500@\u2500\u2500\u2500M('c_0')\u2500\u2500\u2500\n",
+                            "                \u2502\n",
+                            "q_1: \u2500\u2500\u2500X\u2500\u2500\u2500@\u2500\u2500\u2500@\u2500\u2500\u2500M('c_1')\u2500\u2500\u2500\n",
+                            "            \u2502\n",
+                            "q_2: \u2500\u2500\u2500\u2500\u2500\u2500\u2500X\u2500\u2500\u2500Y\u2500\u2500\u2500M('c_2')\u2500\u2500\u2500"
+                        ]
+                    },
+                    "execution_count": 13,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "circ3.to_other_language(Language.CIRQ)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b625d414",
+            "metadata": {},
+            "source": [
+                "Since we use OpenQASM as a common standard for circuit translation, we also provide for the user a way to retrive the code of the circuit in OpenQASM 2.0 and 3.0."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 21,
             "id": "c39e3e72",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -534,24 +595,24 @@
             ],
             "source": [
                 "print(circ3.to_qasm2())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 22,
             "id": "0cdb44e5",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "OPENQASM 3.0;\n",
-                        "include 'stdgates.inc';\n",
+                        "include \"stdgates.inc\";\n",
                         "\n",
                         "qubit[3] q;\n",
                         "bit[3] c;\n",
                         "h q[0];\n",
                         "x q[1];\n",
                         "cx q[1],q[2];\n",
                         "barrier q[0],q[1],q[2];\n",
@@ -570,72 +631,99 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9b28dfc3",
             "metadata": {},
             "source": [
-                "## Parametrized circuit"
+                "## Parametrized circuit\n",
+                "\n",
+                "We allow the use and manipulation of symbolic variable to parametrize gates. \n",
+                "\n",
+                "We first declare symbolic variables using `symbols` (yes, we indeed use `sympy`!)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": null,
             "id": "f4c91072",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from mpqp.gates import symbols\n",
-                "import numpy as np"
+                "\n",
+                "theta, k = symbols(\"\u03b8 k\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "f8b64b3a",
+            "metadata": {},
+            "source": [
+                "We can then use these variables to instantiate and add ``ParametrizedGate`` to the circuit."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 49,
+            "execution_count": null,
             "id": "d9ba7734",
             "metadata": {},
             "outputs": [],
             "source": [
-                "theta, k = symbols(\"\u03b8 k\")\n",
-                "\n",
                 "param_circ = QCircuit(\n",
-                "    [Rx(theta, 0), CNOT(1,2), X(2), Rk(2,1), H(0), CRk(k, 0, 2),\n",
+                "    [Rx(theta, 0), CNOT(1,2), X(2), Rk(k,1), H(0), CRk(k, 0, 2),\n",
                 "    BasisMeasure(list(range(3)), shots=1000)]\n",
                 ")"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "779c8b03",
+            "metadata": {},
+            "source": [
+                "One can observe, in the print below, that 3 gates depend on variables.  "
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 50,
+            "execution_count": null,
             "id": "aad43475",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "     \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510   \u250c\u2500\u2500\u2500\u2510                         \u250c\u2500\u2510   \n",
-                        "q_0: \u2524 Rx(\u03b8) \u251c\u2500\u2500\u2500\u2524 H \u251c\u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524M\u251c\u2500\u2500\u2500\n",
-                        "     \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\u250c\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2510 \u2502                 \u250c\u2500\u2510\u2514\u2565\u2518   \n",
-                        "q_1: \u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2500\u2500\u2524 P(pi/2) \u251c\u2500\u253c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524M\u251c\u2500\u256b\u2500\u2500\u2500\u2500\n",
-                        "       \u250c\u2500\u2534\u2500\u2510  \u2514\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2518 \u2502P(2**(1 - k)*pi) \u2514\u2565\u2518 \u2551 \u250c\u2500\u2510\n",
-                        "q_2: \u2500\u2500\u2524 X \u251c\u2500\u2500\u2500\u2500\u2500\u2524 X \u251c\u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u256b\u2500\u2500\u256b\u2500\u2524M\u251c\n",
-                        "       \u2514\u2500\u2500\u2500\u2518     \u2514\u2500\u2500\u2500\u2518                       \u2551  \u2551 \u2514\u2565\u2518\n",
-                        "c: 3/\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2569\u2550\u2550\u2569\u2550\u2550\u2569\u2550\n",
-                        "                                             1  0  2 \n"
+                        "     \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510       \u250c\u2500\u2500\u2500\u2510                              \u250c\u2500\u2510   \n",
+                        "q_0: \u2524 Rx(\u03b8) \u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524 H \u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524M\u251c\u2500\u2500\u2500\n",
+                        "     \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510 \u2502                 \u250c\u2500\u2510\u2514\u2565\u2518   \n",
+                        "q_1: \u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2500\u2500\u2524 P(2**(1 - k)*pi) \u251c\u2500\u253c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524M\u251c\u2500\u256b\u2500\u2500\u2500\u2500\n",
+                        "       \u250c\u2500\u2534\u2500\u2510  \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518 \u2502P(2**(1 - k)*pi) \u2514\u2565\u2518 \u2551 \u250c\u2500\u2510\n",
+                        "q_2: \u2500\u2500\u2524 X \u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524 X \u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u256b\u2500\u2500\u256b\u2500\u2524M\u251c\n",
+                        "       \u2514\u2500\u2500\u2500\u2518         \u2514\u2500\u2500\u2500\u2518                            \u2551  \u2551 \u2514\u2565\u2518\n",
+                        "c: 3/\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2569\u2550\u2550\u2569\u2550\u2550\u2569\u2550\n",
+                        "                                                      1  0  2 \n"
                     ]
                 }
             ],
             "source": [
                 "print(param_circ)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "cfadd9f6",
+            "metadata": {},
+            "source": [
+                "If we want to attribute values to the parameters, one can use the method ``subs`` as follows. This will return a new circuit with the gates' parameters given in ``subs``. One can also choose to substitute symbolic variable with real and complex numbers when call the ``run`` function (at execution)."
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 53,
+            "execution_count": null,
             "id": "bdc7f941",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -648,30 +736,39 @@
                         "        \u2514\u2500\u2500\u2500\u2518     \u2514\u2500\u2500\u2500\u2518             \u2551  \u2551 \u2514\u2565\u2518\n",
                         "c: 3/\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2569\u2550\u2550\u2569\u2550\u2550\u2569\u2550\n",
                         "                                    1  0  2 \n"
                     ]
                 }
             ],
             "source": [
+                "import numpy as np\n",
                 "print(param_circ.subs({theta: np.pi/3, k:2}))"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "95208ea0",
+            "metadata": {},
+            "source": [
+                "One can also retrieve the set of variables in the circuit by calling the ``variables()`` method."
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 54,
+            "execution_count": null,
             "id": "000492f4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{k, \u03b8}"
                         ]
                     },
-                    "execution_count": 54,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "param_circ.variables()"
             ]
@@ -689,13 +786,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.5"
+            "version": "3.9.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpqp-0.1.dev1/example/scripts/CNOT_cascade_v_pairs.py` & `mpqp-0.2.0/examples/scripts/CNOT_cascade_v_pairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from mpqp.gates import CNOT, H, Rx, Ry, Rz
+import numpy as np
+
 from mpqp import QCircuit
 from mpqp.execution import run
 from mpqp.execution.devices import ATOSDevice
-import numpy as np
+from mpqp.gates import CNOT, H, Rx, Ry, Rz
 
 circuit = QCircuit(5)
 
 circuit.add(H(0))
 circuit.add(H(1))
 circuit.add(Rz(np.pi / 3, 1))
 circuit.add(H(2))
@@ -34,9 +35,7 @@
 circuit2.add(CNOT(0, 1))
 circuit2.add(CNOT(2, 3))
 circuit2.add(CNOT(1, 2))
 circuit2.add(CNOT(3, 4))
 circuit2.add(Ry(np.pi / 3, 4))
 
 print(run(circuit2, ATOSDevice.MYQLM_PYLINALG).state_vector)
-
-
```

### Comparing `mpqp-0.1.dev1/example/scripts/aws_execution_trials.py` & `mpqp-0.2.0/examples/scripts/aws_execution_trials.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+import numpy as np
+from braket.devices import LocalSimulator
+
 from mpqp import QCircuit
-from mpqp.core.instruction.measurement import Observable, ExpectationMeasure
-from mpqp.execution.devices import AWSDevice, ATOSDevice
+from mpqp.core.instruction.measurement import ExpectationMeasure, Observable
+from mpqp.execution import run
+from mpqp.execution.devices import ATOSDevice, AWSDevice
 from mpqp.gates import *
 from mpqp.measures import BasisMeasure
-from mpqp.execution import Sample, run
-from mpqp.qasm import qasm3_to_braket_Program, open_qasm_2_to_3
-from braket.devices import LocalSimulator
-from braket.tasks import GateModelQuantumTaskResult
-import numpy as np
 from mpqp.qasm.qasm_to_braket import qasm3_to_braket_Circuit
 
 device = LocalSimulator()
 
 
 qasm_str = """OPENQASM 3.0;
 include 'stdgates.inc';
@@ -89,9 +88,7 @@
 circuit.add(Rx(1.76, 1))
 circuit.add(Ry(1.76, 1))
 circuit.add(Rz(1.987, 0))
 
 # Running the computation on myQLM and on Aer simulator, then retrieving the results
 result = run(circuit, [AWSDevice.BRAKET_LOCAL_SIMULATOR, ATOSDevice.MYQLM_PYLINALG])
 print(result)
-
-
```

### Comparing `mpqp-0.1.dev1/example/scripts/circuit_to_qasm.py` & `mpqp-0.2.0/examples/scripts/circuit_to_qasm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from mpqp.gates import *
 from mpqp import QCircuit
+from mpqp.gates import *
 from mpqp.measures import BasisMeasure
 
 # Declaration of the circuit with the right size
 circuit = QCircuit(4)
 
 # Constructing the circuit by adding gates
 circuit.add(T(0))
```

### Comparing `mpqp-0.1.dev1/example/scripts/demonstration.py` & `mpqp-0.2.0/examples/scripts/demonstration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 """Demonstration MPQP"""
 
 import numpy as np
-from mpqp.gates import *
+
 from mpqp import QCircuit
-from mpqp.measures import BasisMeasure
 from mpqp.execution import run
-from mpqp.execution.devices import ATOSDevice, IBMDevice, AWSDevice
-from mpqp.tools.visualization import plot_results_sample_mode
-import matplotlib.pyplot as plt
-
+from mpqp.execution.devices import ATOSDevice, AWSDevice, GOOGLEDevice, IBMDevice
+from mpqp.gates import *
+from mpqp.measures import BasisMeasure
 
 # Constructing the circuit
 meas = BasisMeasure(list(range(3)), shots=2000)
 c = QCircuit([T(0), CNOT(0, 1), Ry(np.pi / 2, 2), S(1), CZ(2, 1), SWAP(2, 0), meas])
 print(c)
 
 # Run the circuit on a selected device
 results = run(
     c,
     [
         IBMDevice.AER_SIMULATOR,
         ATOSDevice.MYQLM_PYLINALG,
         ATOSDevice.MYQLM_CLINALG,
         AWSDevice.BRAKET_LOCAL_SIMULATOR,
+        GOOGLEDevice.CIRQ_LOCAL_SIMULATOR,
     ],
 )
 
 # Print the results
 print(results)
 
 # Display the circuit
-plot_results_sample_mode(results)
-plt.show()
+results.plot()
 
 c = QCircuit([T(0), CNOT(0, 1), Ry(np.pi / 2, 2), S(1), CZ(2, 1), SWAP(2, 0)])
 res = run(
     c,
     [
         IBMDevice.AER_SIMULATOR_STATEVECTOR,
         ATOSDevice.MYQLM_PYLINALG,
         ATOSDevice.MYQLM_CLINALG,
         AWSDevice.BRAKET_LOCAL_SIMULATOR,
+        GOOGLEDevice.CIRQ_LOCAL_SIMULATOR,
     ],
 )
 # Print the results
 print(res)
```

### Comparing `mpqp-0.1.dev1/example/scripts/native_gates_examples.py` & `mpqp-0.2.0/examples/scripts/native_gates_examples.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Example 3: Using native gates"""
 
-from mpqp.gates import *
 from mpqp import QCircuit
 from mpqp.execution import run
-from mpqp.execution.devices import IBMDevice, AWSDevice, ATOSDevice
+from mpqp.execution.devices import ATOSDevice, AWSDevice, GOOGLEDevice, IBMDevice
+from mpqp.gates import *
 
 # Declaration of the circuit with the right size
 circuit = QCircuit(3, label="Test native gates")
 # Constructing the circuit by adding gates and measurements
 circuit.add([H(0), X(1), Y(2), Z(0), S(1), T(0)])
 circuit.add([Rx(1.2324, 2), Ry(-2.43, 0), Rz(1.04, 1), Rk(-1, 1), P(-323, 2)])
 circuit.add(U(1.2, 2.3, 3.4, 2))
@@ -17,11 +17,17 @@
 
 # no measure, we want the state vector
 
 print(circuit)
 print(circuit.to_qasm2())
 print(circuit.to_qasm3())
 
-result = run(circuit, [ATOSDevice.MYQLM_PYLINALG,
-                       IBMDevice.AER_SIMULATOR_STATEVECTOR,
-                       AWSDevice.BRAKET_LOCAL_SIMULATOR])
+result = run(
+    circuit,
+    [
+        ATOSDevice.MYQLM_PYLINALG,
+        IBMDevice.AER_SIMULATOR_STATEVECTOR,
+        AWSDevice.BRAKET_LOCAL_SIMULATOR,
+        GOOGLEDevice.CIRQ_LOCAL_SIMULATOR,
+    ],
+)
 print(result)
```

### Comparing `mpqp-0.1.dev1/example/scripts/open_qasm_conversions.py` & `mpqp-0.2.0/examples/scripts/open_qasm_conversions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Examples of OpenQASM conversion from 2.0 to 3.0"""
 
-from mpqp.qasm import open_qasm_2_to_3
+from mpqp.qasm import open_qasm_2_to_3, remove_user_gates
 
 print("-------------------------")
 print("-------------------------")
 
 qasm2_1 = """OPENQASM 2.0;
 include "qelib1.inc";
 qreg q[2];
@@ -47,15 +47,16 @@
 include "qasm_files/test_qasm.inc";
 u3(0.3,0.2,0.1) q[0];
 h q[1];
 cx q[1],q[0];
 
 barrier q;"""
 
-print(open_qasm_2_to_3(qasm2_3, path_to_file="mpqp/example"))
+# this exemple should be executed from mpqp root
+print(open_qasm_2_to_3(qasm2_3, path_to_file="examples/scripts"))
 
 print("-------------------------")
 print("-------------------------")
 
 qasm2_4 = """OPENQASM 2.0;
 include "qelib1.inc";
 gate hello(theta) a, b {
@@ -69,7 +70,39 @@
 u3(0.3,0.2,0.1) q[0];
 h q[1];
 cx q[1],q[0];
 
 barrier q;"""
 
 print(open_qasm_2_to_3(qasm2_4))
+
+
+print("-------------------------")
+print("-------------------------")
+
+qasm2_4 = """OPENQASM 2.0;
+include "qelib1.inc";
+gate rxx(theta) a, b {
+    u3(pi/2, theta, 0) a;
+    h b;
+    cx a,
+    b;
+    u1(-theta) b;
+    cx a, b;
+    h b;
+    u2(-pi, pi-theta) a;
+}
+gate rzz(theta) a,b {
+    cx a,b;
+    u1(theta) b;
+    cx a,b;
+}
+
+qubit[3] q;
+bit[1] c0;
+bit[1] c1;
+bit[1] c2;
+rxx(0.4) q[0], q[1];
+rzz(0.2) q[1], q[2];
+c2[0] = measure q[2];"""
+
+print(remove_user_gates(qasm2_4))
```

### Comparing `mpqp-0.1.dev1/mpqp/all.py` & `mpqp-0.2.0/mpqp/all.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 # pyright: reportUnusedImport=false
 import numpy as np
-from . import QCircuit, Barrier, Language, Instruction
+
+from mpqp.execution.providers.atos import get_result_from_qlm_job_id
+
+from . import Barrier, Instruction, Language, QCircuit
+from .execution import (
+    Job,
+    JobStatus,
+    JobType,
+    Result,
+    Sample,
+    StateVector,
+    adjust_measure,
+    get_remote_result,
+    run,
+    submit,
+)
+from .execution.remote_handler import get_all_job_ids
+from .execution.devices import ATOSDevice, AWSDevice, GOOGLEDevice, IBMDevice
+from .execution.vqa import Optimizer, minimize
 from .gates import (
-    X,
-    Y,
-    Z,
-    H,
-    P,
-    S,
-    T,
-    SWAP,
-    U,
-    Rx,
-    Ry,
-    Rz,
-    Rk,
     CNOT,
     CZ,
-    CRk,
+    SWAP,
     TOF,
     ControlledGate,
+    CRk,
+    CustomGate,
     Gate,
-    ParametrizedGate,
-    symbols,
     GateDefinition,
-    KrausRepresentation,
-    PauliDecomposition,
-    CustomGate,
+    H,
+    Id,
+    P,
+    ParametrizedGate,
+    Rk,
+    Rx,
+    Ry,
+    Rz,
+    S,
+    T,
+    U,
     UnitaryMatrix,
+    X,
+    Y,
+    Z,
+    symbols,
 )
 from .measures import (
-    ComputationalBasis,
     Basis,
-    HadamardBasis,
-    VariableSizeBasis,
     BasisMeasure,
+    ComputationalBasis,
     ExpectationMeasure,
-    Observable,
-    Measure,
-)
-from .execution import (
-    Result,
-    StateVector,
-    Sample,
-    run,
-    adjust_measure,
-    submit,
-    Job,
-    JobStatus,
-    JobType,
-)
-from .execution.devices import (
-    ATOSDevice,
-    IBMDevice,
-    AWSDevice,
+    HadamardBasis,
 )
-from .execution.vqa import minimize, Optimizer
-from .execution.connection.qlm_connection import get_all_job_ids
-from mpqp.execution.providers_execution.atos_execution import get_result_from_qlm_job_id
+from .measures import I as Iop
+from .measures import Measure, Observable, VariableSizeBasis
+from .measures import X as Xop
+from .measures import Y as Yop
+from .measures import Z as Zop
 from .qasm import open_qasm_file_conversion_2_to_3, open_qasm_hard_includes
 
+from .noise import Depolarizing
+
 theta, k = symbols("θ k")  # type: ignore
 obs = Observable(np.array([[0, 1], [1, 0]]))
 circ = QCircuit([P(theta, 0), ExpectationMeasure([0], observable=obs, shots=1000)])
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/barrier.py` & `mpqp-0.2.0/mpqp/core/instruction/barrier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """A barrier is a purely cosmetic instruction. In fact, at execution it is
 removed because it could have a negative impact on the execution speed of the
 circuit (since it artificially increases the depth)."""
 
-from typing import Optional
-from qiskit.circuit.library import Barrier as QiskitBarrier
+from typing import TYPE_CHECKING, Optional
 
-from qiskit.circuit import Parameter
+if TYPE_CHECKING:
+    from qiskit.circuit import Parameter
 
 from mpqp.core.languages import Language
+
 from .instruction import Instruction
 
 
 class Barrier(Instruction):
     """Visual indicator of the grouping of circuit sections"""
 
     def __init__(self):
         super().__init__([0])
         self.size = 0
         """Size of the barrier (set to 0 by default)."""
 
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
-        qiskit_parameters: Optional[set[Parameter]] = None,
+        qiskit_parameters: Optional[set["Parameter"]] = None,
     ):
         if language == Language.QISKIT:
+            from qiskit.circuit.library import Barrier as QiskitBarrier
+
             return QiskitBarrier(self.size)
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/gates/controlled_gate.py` & `mpqp-0.2.0/mpqp/core/instruction/gates/controlled_gate.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/gates/custom_gate.py` & `mpqp-0.2.0/mpqp/core/instruction/gates/custom_gate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from typeguard import typechecked
 
+if TYPE_CHECKING:
+    from qiskit.circuit import Parameter
+
 from mpqp.core.instruction.gates.gate import Gate
-from mpqp.core.instruction.gates.gate_definition import (
-    UnitaryMatrix,
-    KrausRepresentation,
-    PauliDecomposition,
-)
+from mpqp.core.instruction.gates.gate_definition import UnitaryMatrix
 from mpqp.core.languages import Language
-from qiskit.circuit import Parameter
 
 
 @typechecked
 class CustomGate(Gate):
     """Custom gates allow you to define your own gates.
 
     Args:
@@ -31,49 +29,23 @@
 
     def to_matrix(self):
         return self.matrix
 
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
-        qiskit_parameters: Optional[set[Parameter]] = None,
+        qiskit_parameters: Optional[set["Parameter"]] = None,
     ):
+        from qiskit.quantum_info.operators import Operator as QiskitOperator
+
         if qiskit_parameters is None:
             qiskit_parameters = set()
-        return super().to_other_language(language, qiskit_parameters)
+        return QiskitOperator(self.matrix)
 
     def decompose(self):
         """Returns the circuit made of native gates equivalent to this gate.
 
         6M-TODO refine this doc and implement
         """
         from mpqp.core.circuit import QCircuit
 
         return QCircuit(self.nb_qubits)
-
-
-@typechecked
-class KrausGate(CustomGate):
-    """6M-TODO"""
-    def __init__(
-        self,
-        definition: KrausRepresentation,
-        targets: list[int],
-        label: Optional[str] = None,
-    ):
-        self.kraus_representation = definition
-        """See parameter description."""
-        CustomGate.__init__(self, UnitaryMatrix(definition.to_matrix()), targets, label)
-
-
-@typechecked
-class PauliDecompositionGate(CustomGate):
-    """6M-TODO"""
-    def __init__(
-        self,
-        definition: PauliDecomposition,
-        targets: list[int],
-        label: Optional[str] = None,
-    ):
-        self.pauli_decomposition = definition
-        """See parameter description."""
-        CustomGate.__init__(self, UnitaryMatrix(definition.to_matrix()), targets, label)
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/gates/gate.py` & `mpqp-0.2.0/mpqp/core/instruction/gates/gate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
-from abc import abstractmethod, ABC
+
+from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Optional
 
 import numpy as np
 from scipy.linalg import fractional_matrix_power
 from typeguard import typechecked
 
-from mpqp.core.instruction.instruction import Instruction
 from mpqp.core.instruction.gates.gate_definition import UnitaryMatrix
+from mpqp.core.instruction.instruction import Instruction
 from mpqp.tools.generics import Matrix
 from mpqp.tools.maths import matrix_eq
 
 
 @typechecked
 class Gate(Instruction, ABC):
     """Represent a unitary operator acting on qubit(s).
@@ -36,14 +37,17 @@
 
     @abstractmethod
     def to_matrix(self) -> Matrix:
         """Return the "base" matricial semantics to this gate. Without
         considering potential column and row permutations needed if the targets
         of the gate are not sorted.
 
+        Returns:
+            A numpy array representing the unitary matrix of the gate.
+
         Example:
             >>> gd = UnitaryMatrix(
             ...     np.array([[0, 0, 0, 1], [0, 1, 0, 0], [1, 0, 0, 0], [0, 0, 1, 0]])
             ... )
             >>> CustomGate(gd, [1, 2]).to_matrix()
             array([[0, 0, 0, 1],
                    [0, 1, 0, 0],
@@ -51,30 +55,29 @@
                    [0, 0, 1, 0]])
             >>> SWAP(0,1).to_matrix()
             array([[1, 0, 0, 0],
                    [0, 0, 1, 0],
                    [0, 1, 0, 0],
                    [0, 0, 0, 1]])
 
-        Returns:
-            A numpy array representing the unitary matrix of the gate.
         """
 
     def inverse(self) -> Gate:
         """Computing the inverse of this gate.
 
-        Examples:
+        Returns:
+            The gate corresponding to the inverse of this gate.
+
+        Example:
             >>> Z(0).inverse()
             Z(0)
             >>> CustomGate(UnitaryMatrix(np.diag([1,1j])),[0]).inverse().to_matrix()
-            array([[1,  0 ],
-                   [0, -1j]])
+            array([[1.-0.j, 0.-0.j],
+                   [0.-0.j, 0.-1.j]])
 
-        Returns:
-            The gate corresponding to the inverse of this gate.
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         return CustomGate(
             UnitaryMatrix(self.to_matrix().transpose().conjugate()),
             self.targets,
             self.label,
@@ -83,84 +86,86 @@
     def is_equivalent(self, other: Gate) -> bool:
         """Determine if the gate in parameter is equivalent to this gate.
 
         The equivalence of two gate is only determined from their matricial
         semantics (and thus ignores all other aspects of the gate such as the
         target qubits, the label, etc....)
 
-        Examples:
-            >>> X(0).is_equivalent(CustomGate(UnitaryMatrix(np.array([[0,1],[1,0]])),[1]))
-            True
-
         Args:
             other: the gate to test if it is equivalent to this gate
 
         Returns:
-            True if the two gates' matrix semantics are equal.
+            ``True`` if the two gates' matrix semantics are equal.
+
+        Example:
+            >>> X(0).is_equivalent(CustomGate(UnitaryMatrix(np.array([[0,1],[1,0]])),[1]))
+            True
+
         """
         return matrix_eq(self.to_matrix(), other.to_matrix())
 
     def power(self, exponent: float) -> Gate:
         """Compute the exponentiation `G^{exponent}` of this gate G.
 
+        Args:
+            exponent: Number representing the exponent.
+
+        Returns:
+            The gate elevated to the exponent in parameter.
+
         Examples:
             >>> swap_gate = SWAP(0,1)
             >>> (swap_gate.power(2)).to_matrix()
             array([[1, 0, 0, 0],
                    [0, 1, 0, 0],
                    [0, 0, 1, 0],
                    [0, 0, 0, 1]])
             >>> (swap_gate.power(-1)).to_matrix()
-            array([[1, 0, 0, 0],
-                   [0, 0, 1, 0],
-                   [0, 1, 0, 0],
-                   [0, 0, 0, 1]])
+            array([[1., 0., 0., 0.],
+                   [0., 0., 1., 0.],
+                   [0., 1., 0., 0.],
+                   [0., 0., 0., 1.]])
             >>> (swap_gate.power(0.75)).to_matrix() # not implemented yet
             array([[1.        +0.j        , 0.        +0.j        ,
                     0.        +0.j        , 0.        +0.j        ],
                    [0.        +0.j        , 0.14644661+0.35355339j,
                     0.85355339-0.35355339j, 0.        +0.j        ],
                    [0.        +0.j        , 0.85355339-0.35355339j,
                     0.14644661+0.35355339j, 0.        +0.j        ],
                    [0.        +0.j        , 0.        +0.j        ,
                     0.        +0.j        , 1.        +0.j        ]])
 
-        Args:
-            exponent: Number representing the exponent.
-
-        Returns:
-            The gate elevated to the exponent in parameter.
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         return CustomGate(
             definition=UnitaryMatrix(
                 fractional_matrix_power(self.to_matrix(), exponent)
             ),
             targets=self.targets,
             label=None if self.label is None else self.label + f"^{exponent}",
         )
 
     def tensor_product(self, other: Gate) -> Gate:
         """Compute the tensor product of the current gate.
 
-        Examples:
-            >>> (X(0).tensor_product(Z(0))).to_matrix()
-            array([[ 0,  0,  1,  0],
-                   [ 0,  0,  0, -1],
-                   [ 1,  0,  0,  0],
-                   [ 0, -1,  0,  0]])
-
         Args:
             other: Second operand of the tensor product.
 
         Returns:
             A Gate representing a tensor product of this gate with the gate in
             parameter.
 
+        Example:
+            >>> (X(0).tensor_product(Z(0))).to_matrix()
+            array([[ 0,  0,  1,  0],
+                   [ 0,  0,  0, -1],
+                   [ 1,  0,  0,  0],
+                   [ 0, -1,  0,  0]])
+
         # 3M-TODO: to be implemented, don't trust the code bellow, it's pure experiments
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         gd = UnitaryMatrix(
             np.kron(self.to_matrix(), other.to_matrix())
         )  # self, gate, type="tensor"
@@ -181,104 +186,107 @@
 
     def _mandatory_label(self, postfix: str = ""):
         return "g" + postfix if self.label is None else self.label
 
     def product(self, other: Gate, targets: Optional[list[int]] = None) -> Gate:
         """Compute the composition of self and the other gate.
 
-        Examples:
-            >>> (X(0).product(Z(0))).to_matrix()
-            array([[ 0, -1],
-                   [ 1,  0]])
-
         Args:
             other: Rhs of the product.
             targets: Qubits on which this new gate will operate. If not given,
                 the targets of the two gates multiplied must be the same and the
                 resulting gate will have this same targets.
 
         Returns:
             The product of the two gates concerned.
+
+        Example:
+            >>> (X(0).product(Z(0))).to_matrix()
+            array([[ 0, -1],
+                   [ 1,  0]])
+
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         return CustomGate(
             definition=UnitaryMatrix(self.to_matrix().dot(other.to_matrix())),  # type: ignore
             targets=self._check_targets_compatibility(other, targets),
             label=f"{self._mandatory_label('1')}×{other._mandatory_label('2')}",
         )
 
     def scalar_product(self, scalar: complex) -> Gate:
         """Multiply this gate by a scalar. It normalizes the subtraction
         to ensure it is unitary.
 
-        Examples:
-            >>> (X(0).scalar_product(1j)).to_matrix()
-            array([[0, 1j],
-                   [1j, 0]])
-
         Args:
             scalar: The number to multiply the gate's matrix by.
 
         Returns:
             The result of the multiplication, the targets of the resulting gate
             will be the same as the ones of the initial gate.
+
+        Example:
+            >>> (X(0).scalar_product(1j)).to_matrix()
+            array([[0.+0.j, 0.+1.j],
+                   [0.+1.j, 0.+0.j]])
+
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         return CustomGate(
             UnitaryMatrix(self.to_matrix() * scalar / abs(scalar)),
             targets=self.targets,
             label=f"{scalar}×{self._mandatory_label()}",
         )
 
     def minus(self, other: Gate, targets: Optional[list[int]] = None) -> Gate:
         """Compute the subtraction of two gates. It normalizes the subtraction
         to ensure it is unitary.
 
-        Examples:
-            >>> (X(0).minus(Z(0))).to_matrix()
-            array([[-0.70710678,  0.70710678],
-                   [ 0.70710678,  0.70710678]])
-
         Args:
             other: The gate to subtract to this gate.
             targets: Qubits on which this new gate will operate. If not given,
                 the targets of the two gates multiplied must be the same and the
                 resulting gate will have this same targets.
 
         Returns:
             The subtraction of ``self`` and ``other``.
 
+        Example:
+            >>> (X(0).minus(Z(0))).to_matrix()
+            array([[-0.70710678,  0.70710678],
+                   [ 0.70710678,  0.70710678]])
+
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         subtraction = self.to_matrix() - other.to_matrix()
         return CustomGate(
             definition=UnitaryMatrix(subtraction / np.linalg.norm(subtraction, 2)),  # type: ignore
             targets=self._check_targets_compatibility(other, targets),
             label=f"{self._mandatory_label('1')}-{other._mandatory_label('2')}",
         )
 
     def plus(self, other: Gate, targets: Optional[list[int]] = None) -> Gate:
         """Compute the sum of two gates. It normalizes the subtraction
         to ensure it is unitary.
 
-        Examples:
-            >>> (X(0).plus(Z(0))).to_matrix()
-            array([[ 0.70710678,  0.70710678],
-                   [ 0.70710678, -0.70710678]])
-
         Args:
             other: The gate to add to this gate.
             targets: Qubits on which this new gate will operate. If not given, the targets of the two gates multiplied
             must be the same and the resulting gate will have this same targets.
 
         Returns:
             The sum of ``self`` and ``other``.
+
+        Example:
+            >>> (X(0).plus(Z(0))).to_matrix()
+            array([[ 0.70710678,  0.70710678],
+                   [ 0.70710678, -0.70710678]])
+
         """
         from mpqp.core.instruction.gates.custom_gate import CustomGate
 
         addition = self.to_matrix() + other.to_matrix()
         return CustomGate(
             definition=UnitaryMatrix(addition / np.linalg.norm(addition, 2)),  # type: ignore
             targets=self._check_targets_compatibility(other, targets),
@@ -335,7 +343,9 @@
     """
 
     def __init__(self, target: int, label: Optional[str] = None):
         Gate.__init__(self, [target], label)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.targets[0]})"
+
+    nb_qubits = 1  # pyright: ignore[reportAssignmentType]
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/gates/gate_definition.py` & `mpqp-0.2.0/mpqp/core/instruction/gates/gate_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,117 +1,94 @@
 from __future__ import annotations
 
-from abc import abstractmethod, ABC
+from abc import ABC, abstractmethod
+from numbers import Complex
 from warnings import warn
 
 import numpy as np
 from sympy import Expr
 from typeguard import typechecked
-from numbers import Complex
 
-from mpqp.tools.maths import is_unitary, matrix_eq
 from mpqp.tools.generics import Matrix, one_lined_repr
+from mpqp.tools.maths import is_unitary, matrix_eq
 
 
 @typechecked
 class GateDefinition(ABC):
     """A class used to handle the definition of a Gate.
 
     A quantum gate can be defined in several ways, and this class allows us to
     define it as we prefer. It also handles the translation from one definition
     to another.
 
     This said, for now only one way of defining the gates is supported, using
     their matricial semantics.
 
-    Examples:
+    Example:
         >>> gate_matrix = np.array([[0, 0, 0, 1], [0, 1, 0, 0], [1, 0, 0, 0], [0, 0, 1, 0]])
         >>> gate_definition = UnitaryMatrix(gate_matrix)
-        >>> custom_gate = CustomGate(gate_definition)
-    """
+        >>> custom_gate = CustomGate(gate_definition, [0])
 
-    """ TODO: put this back once we implement the other definitions
-    This class permit to define a gate in 4 potential ways:
-        1. the unitary matrix defining the gate
-        2. a combination of several other gates
-        3. a combination of Kraus operators
-        4. the decomposition of the gate in the Pauli basis (only possible for LU gates)
     """
 
+    # TODO: put this back once we implement the other definitions
+    # This class permit to define a gate in 4 potential ways:
+    #     1. the unitary matrix defining the gate
+    #     2. a combination of several other gates
+    #     3. a combination of Kraus operators
+    #     4. the decomposition of the gate in the Pauli basis (only possible for LU gates)
+
     @abstractmethod
     def to_matrix(self) -> Matrix:
         """Returns the matrix corresponding to this gate definition."""
 
     @abstractmethod
     def subs(
         self,
         values: dict[Expr | str, Complex],
         remove_symbolic: bool = False,
         disable_symbol_warn: bool = False,
     ) -> GateDefinition:
         pass
 
-    # @abstractmethod
-    def to_kraus_representation(self) -> KrausRepresentation:
-        """6M-TODO"""
-        raise NotImplementedError()
-
-    # @abstractmethod
-    def to_pauli_decomposition(self) -> PauliDecomposition:
-        """6M-TODO"""
-        raise NotImplementedError()
-
     def is_equivalent(self, other: GateDefinition) -> bool:
         """Determines if this definition is equivalent to the other.
 
         Args:
             other: The definition we want to know if it is equivalent.
 
-        Examples:
+        Example:
             >>> d1 = UnitaryMatrix(np.array([[1, 0], [0, -1]]))
             >>> d2 = UnitaryMatrix(np.array([[2, 0], [0, -2.0]]) / 2)
             >>> d1.is_equivalent(d2)
             True
+
         """
         return matrix_eq(self.to_matrix(), other.to_matrix())
 
     def inverse(self) -> GateDefinition:
         """Compute the inverse of the gate.
 
         Returns:
             A GateDefinition representing the inverse of the gate defined.
 
-        Examples:
+        Example:
             >>> UnitaryMatrix(np.array([[1, 0], [0, -1]])).inverse()
-            array([[ 1.,  0.],
-                   [-0., -1.]])
+            UnitaryMatrix(array([[ 1., 0.], [-0., -1.]]))
+
         """
         mat = self.to_matrix()
 
         if not all(
             isinstance(elt.item(), Complex) for elt in np.nditer(mat, ["refs_ok"])  # type: ignore
         ):
             raise ValueError("Cannot invert arbitrary gates using symbolic variables")
         return UnitaryMatrix(np.linalg.inv(mat))  # type:ignore
 
 
-class KrausRepresentation(GateDefinition):
-    """# 6M-TODO : implement and comment"""
-
-    def __init__(self):
-        self.pp = 1
-
-
-class PauliDecomposition(GateDefinition):
-    """# 6M-TODO : implement and comment"""
-
-    def __init__(self):
-        self.pp = 1
-
-
 @typechecked
 class UnitaryMatrix(GateDefinition):
     """Definition of a gate using it's matrix.
 
     Args:
         definition: Matrix defining the unitary gate.
         disable_symbol_warn: Boolean used to enable/disable warning concerning
@@ -130,22 +107,14 @@
             )
         self.matrix = definition
         """See parameter :attr:`definition`'s description."""
 
     def to_matrix(self) -> Matrix:
         return self.matrix
 
-    def to_kraus_representation(self) -> KrausRepresentation:
-        """6M-TODO to implement"""
-        ...
-
-    def to_pauli_decomposition(self) -> PauliDecomposition:
-        """6M-TODO to implement"""
-        ...
-
     def subs(
         self,
         values: dict[Expr | str, Complex],
         remove_symbolic: bool = False,
         disable_symbol_warn: bool = False,
     ):
         """Substitute some symbolic variables in the definition by complex values.
@@ -168,20 +137,20 @@
 
         def mapping(val: Expr | Complex) -> Expr | Complex:
             def caster(v: Expr | Complex) -> Expr | Complex:
                 # problem between pyright and abstract numeric types ?
                 # "complex" cannot be assigned to return type "Complex"
                 return (
                     complex(v) if remove_symbolic else v
-                )  # pyright: ignore[reportGeneralTypeIssues]
+                )  # pyright: ignore[reportReturnType]
 
             # the types in sympy are relatively badly handled
             # Argument of type "Unknown | Basic | Expr" cannot be assigned to parameter "v" of type "Expr | Complex"
             return (
-                caster(val.subs(values))  # pyright: ignore[reportGeneralTypeIssues]
+                caster(val.subs(values))  # pyright: ignore[reportArgumentType]
                 if isinstance(val, Expr)
                 else val
             )
 
         matrix = self.to_matrix()
         otype = (
             complex
@@ -192,7 +161,8 @@
 
         return UnitaryMatrix(
             np.vectorize(mapping, otypes=[otype])(matrix), disable_symbol_warn
         )
 
     def __repr__(self) -> str:
         return f"UnitaryMatrix({one_lined_repr(getattr(self, 'matrix', ''))})"
+
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/gates/native_gates.py` & `mpqp-0.2.0/mpqp/core/instruction/gates/native_gates.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,55 @@
 """Native gates is the set of all gates natively supported in OpenQASM. Since we
 rely on this standard, all of them are indeed implemented. In addition, this
 module contains a few abstract classes used to factorize the behaviors common to
 a lot of gates. Feel free to use them for your own custom gates!"""
 
 from __future__ import annotations
 
-from abc import ABC
 from numbers import Integral
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
+
+if TYPE_CHECKING:
+    from qiskit.circuit import Parameter
 
 import numpy as np
 import numpy.typing as npt
-
-from qiskit.circuit import Parameter
-from qiskit.circuit.library import (
-    ZGate,
-    YGate,
-    CCXGate,
-    PhaseGate,
-    SGate,
-    UGate,
-    TGate,
-    SwapGate,
-    RXGate,
-    RYGate,
-    RZGate,
-    HGate,
-    CXGate,
-    XGate,
-    CPhaseGate,
-    CZGate,
-)
 from sympy import Expr, pi
 
 # pylance doesn't handle well Expr, so a lot of "type:ignore" will happen in
 # this file :/
 from typeguard import typechecked
 
-from mpqp.core.languages import Language
-from mpqp.core.instruction.gates.gate import Gate, InvolutionGate, SingleQubitGate
 from mpqp.core.instruction.gates.controlled_gate import ControlledGate
+from mpqp.core.instruction.gates.gate import Gate, InvolutionGate, SingleQubitGate
 from mpqp.core.instruction.gates.gate_definition import UnitaryMatrix
 from mpqp.core.instruction.gates.parametrized_gate import ParametrizedGate
-from mpqp.tools.generics import Matrix
-from mpqp.tools.maths import cos, sin, exp
+from mpqp.core.languages import Language
+from mpqp.tools.generics import Matrix, SimpleClassReprABC
+from mpqp.tools.maths import cos, exp, sin
 
 
 @typechecked
-def _qiskit_parameter_adder(param: Expr | float, qiskit_parameters: set[Parameter]):
+def _qiskit_parameter_adder(
+    param: Expr | float, qiskit_parameters: set["Parameter"]
+) -> "Parameter | float | int":
     """To avoid having several parameters in qiskit for the same value we keep
     track of them in a set. This function takes care of this, this way you can
     directly call `QiskitGate(_qiskit_parameter_adder(<param>, <q_params_set>))`
     without having to manually take care of the de-duping.
 
+    This process is a form of memoization.
+
     Args:
         param: The parameter you need for your qiskit gate.
         qiskit_parameters: The set of previously set qiskit parameters. This set
         is updated inplace.
 
     Returns:
-
+        The memoized parameter
     """
     if isinstance(param, Expr):
         name = str(param)
         previously_set_param = list(
             filter(lambda elt: elt.name == name, qiskit_parameters)
         )
         if len(previously_set_param) > 1:
@@ -71,50 +57,59 @@
                 "Somehow two parameter got the same name, this shouldn't be "
                 "possible. For help on this error please contact the authors of"
                 " this library"
             )
         elif len(previously_set_param) == 1:
             qiskit_param = previously_set_param[0]
         else:
+            from qiskit.circuit import Parameter
+
             qiskit_param = Parameter(name)
             qiskit_parameters.add(qiskit_param)
     else:
         qiskit_param = param
     return qiskit_param
 
 
 @typechecked
-class NativeGate(Gate, ABC):
+class NativeGate(Gate, SimpleClassReprABC):
     """The standard on which we rely, OpenQASM, comes with a set of gates
     supported by default. More complicated gates can be defined by the user.
     This class represent all those gates supported by default.
 
     Args:
         targets: List of indices referring to the qubits on which the gate will
             be applied.
         label: Label used to identify the gate.
     """
 
     native_gate_options = {"disable_symbol_warn": True}
 
 
 @typechecked
-class RotationGate(NativeGate, ParametrizedGate, ABC):
+class RotationGate(NativeGate, ParametrizedGate, SimpleClassReprABC):
     """Many gates can be classified as a simple rotation gate, around a specific
     axis (and potentially with a control qubit). All those gates have in common
     a single parameter: ``theta``. This class help up factorize this behavior,
-    and simply having to tweak the matricial semantics and qasm translation of
+    and simply having to tweak the matrix semantics and qasm translation of
     the specific gate.
 
     Args:
         theta: Angle of the rotation.
         target: Index referring to the qubits on which the gate will be applied.
     """
 
+    if TYPE_CHECKING:
+        from braket.circuits import gates
+        from qiskit.circuit.library import CPhaseGate, PhaseGate, RXGate, RYGate, RZGate
+
     qiskit_gate: type[RXGate | RYGate | RZGate | PhaseGate | CPhaseGate]
+    braket_gate: type[
+        gates.Rx | gates.Ry | gates.Rz | gates.PhaseShift | gates.CPhaseShift
+    ]
 
     def __init__(self, theta: Expr | float, target: int):
         self.parameters = [theta]
         definition = UnitaryMatrix(self.to_matrix(), **self.native_gate_options)
         ParametrizedGate.__init__(
             self, definition, [target], [self.theta], type(self).__name__.capitalize()
         )
@@ -127,155 +122,270 @@
         return (
             f"{type(self).__name__}({f'{self.theta}'.rstrip('0')}, {self.targets[0]})"
         )
 
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
-        qiskit_parameters: Optional[set[Parameter]] = None,
+        qiskit_parameters: Optional[set["Parameter"]] = None,
     ):
         if qiskit_parameters is None:
             qiskit_parameters = set()
         theta = float(self.theta) if self._numeric_parameters else self.theta
         if language == Language.QISKIT:
             return self.qiskit_gate(_qiskit_parameter_adder(theta, qiskit_parameters))
+        elif language == Language.BRAKET:
+            # TODO: handle symbolic parameters for Braket
+            if isinstance(theta, Expr):
+                raise NotImplementedError(
+                    "Symbolic expressions are not yet supported for braket "
+                    "export, this feature is coming very soon!"
+                )
+            return self.braket_gate(theta)
         else:
             raise NotImplementedError(f"Error: {language} is not supported")
 
 
 @typechecked
-class NoParameterGate(NativeGate, ABC):
+class NoParameterGate(NativeGate, SimpleClassReprABC):
     """Class describing native gates that do not depend on parameters.
 
     Args:
         targets: List of indices referring to the qubits on which the gate will
             be applied.
         label: Label used to identify the gate.
     """
 
+    if TYPE_CHECKING:
+        from braket.circuits import gates
+        from qiskit.circuit.library import (
+            CCXGate,
+            CXGate,
+            CZGate,
+            HGate,
+            IGate,
+            SGate,
+            SwapGate,
+            TGate,
+            XGate,
+            YGate,
+            ZGate,
+        )
+
     qiskit_gate: type[
         XGate
         | YGate
         | ZGate
         | HGate
         | TGate
         | SGate
         | SwapGate
         | CXGate
         | CZGate
         | CCXGate
+        | IGate
+    ]
+    braket_gate: type[
+        gates.X
+        | gates.Y
+        | gates.Z
+        | gates.H
+        | gates.T
+        | gates.S
+        | gates.Swap
+        | gates.CNot
+        | gates.CZ
+        | gates.CCNot
+        | gates.I
     ]
+    qlm_aqasm_keyword: str
+
     """Corresponding ``qiskit``'s gate class."""
     matrix: npt.NDArray[np.complex64]
     """Matricial semantics of the gate."""
 
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
-        qiskit_parameters: Optional[set[Parameter]] = None,
+        qiskit_parameters: Optional[set["Parameter"]] = None,
     ):
         if language == Language.QISKIT:
             return self.qiskit_gate()
+        elif language == Language.BRAKET:
+            return self.braket_gate()
         else:
             raise NotImplementedError(f"Error: {language} is not supported")
 
     def to_matrix(self) -> Matrix:
         return self.matrix
 
 
 @typechecked
-class OneQubitNoParamGate(SingleQubitGate, NoParameterGate, ABC):
+class OneQubitNoParamGate(SingleQubitGate, NoParameterGate, SimpleClassReprABC):
     """Class describing one-qubit native gates that do not depend on parameters.
 
     Args:
         target: Index referring to the qubits on which the gate will be applied.
     """
 
     def __init__(self, target: int):
         SingleQubitGate.__init__(self, target, type(self).__name__)
 
 
+class Id(OneQubitNoParamGate, InvolutionGate):
+    """One qubit identity gate.
+
+    Args:
+        target: Index referring to the qubit on which the gate will be applied.
+
+    Example:
+        >>> Id(0).to_matrix()
+        array([[1.+0.j, 0.+0.j],
+               [0.+0.j, 1.+0.j]], dtype=complex64)
+
+    """
+
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import IGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = IGate
+        self.braket_gate = gates.I
+        self.qlm_aqasm_keyword = "I"
+        self.matrix = np.eye(2, dtype=np.complex64)
+
+
 class X(OneQubitNoParamGate, InvolutionGate):
     """One qubit X (NOT) Pauli gate.
 
     Args:
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> X(0).to_matrix()
         array([[0, 1],
                [1, 0]])
+
     """
 
-    qiskit_gate = XGate
-    matrix = np.array([[0, 1], [1, 0]])
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import XGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = XGate
+        self.braket_gate = gates.X
+        self.qlm_aqasm_keyword = "X"
+        self.matrix = np.array([[0, 1], [1, 0]])
 
 
 class Y(OneQubitNoParamGate, InvolutionGate):
     """One qubit Y Pauli gate.
 
     Args:
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> Y(0).to_matrix()
         array([[ 0.+0.j, -0.-1.j],
                [ 0.+1.j,  0.+0.j]])
+
     """
 
-    qiskit_gate = YGate
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import YGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = YGate
+        self.braket_gate = gates.Y
+        self.qlm_aqasm_keyword = "Y"
+
     matrix = np.array([[0, -1j], [1j, 0]])
 
 
 class Z(OneQubitNoParamGate, InvolutionGate):
     """One qubit Z Pauli gate.
 
     Args:
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> Z(0).to_matrix()
         array([[ 1,  0],
                [ 0, -1]])
+
     """
 
-    qiskit_gate = ZGate
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import ZGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = ZGate
+        self.braket_gate = gates.Z
+        self.qlm_aqasm_keyword = "Z"
+
     matrix = np.array([[1, 0], [0, -1]])
 
 
 class H(OneQubitNoParamGate, InvolutionGate):
     """One qubit Hadamard gate.
 
     Args:
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> H(0).to_matrix()
         array([[ 0.70710678,  0.70710678],
                [ 0.70710678, -0.70710678]])
+
     """
 
-    qiskit_gate = HGate
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import HGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = HGate
+        self.braket_gate = gates.H
+        self.qlm_aqasm_keyword = "H"
+
     matrix = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
 
 
 class P(RotationGate, SingleQubitGate):
     """One qubit parametrized Phase gate. Consist in a rotation around Z axis.
 
     Args:
         theta: Parameter representing the phase to apply.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> P(np.pi/3, 1).to_matrix()
         array([[1. +0.j       , 0. +0.j       ],
                [0. +0.j       , 0.5+0.8660254j]])
+
     """
 
-    qiskit_gate = PhaseGate
+    def __init__(self, theta: Expr | float, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import PhaseGate
+
+        super().__init__(theta, target)
+
+        self.qiskit_gate = PhaseGate
+        self.braket_gate = gates.PhaseShift
+        self.qlm_aqasm_keyword = "PH"
 
     def to_matrix(self) -> Matrix:
         return np.array([[1, 0], [0, exp(self.parameters[0] * 1j)]])  # type:ignore
 
 
 class S(OneQubitNoParamGate):
     """One qubit S gate. It's equivalent to ``P(pi/2)``.
@@ -284,72 +394,105 @@
     Args:
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> S(0).to_matrix()
         array([[1.+0.j, 0.+0.j],
                [0.+0.j, 0.+1.j]])
+
     """
 
-    qiskit_gate = SGate
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import SGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = SGate
+        self.braket_gate = gates.S
+        self.qlm_aqasm_keyword = "S"
+
     matrix = np.array([[1, 0], [0, 1j]])
 
 
 class T(OneQubitNoParamGate):
-    """One qubit T gate. It consists in applying a phase of Pi/4.
-    The T gate can be defined as the fourth-root of the Z (Pauli) gate.
+    r"""One qubit T gate. It is also referred to as the `\pi/4` gate because it
+    consists in applying the phase gate with a phase of `\pi/4`.
+
+    The T gate can also be defined as the fourth-root of the Z (Pauli) gate.
 
     Args:
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> T(0).to_matrix()
-        array([[1.        +0.j        , 0.        +0.j        ],
-               [0.        +0.j        , 0.70710678+0.70710678j]])
+        array([[1, 0],
+               [0, exp(0.25*I*pi)]], dtype=object)
+
     """
 
-    qiskit_gate = TGate
+    def __init__(self, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import TGate
+
+        super().__init__(target)
+
+        self.qiskit_gate = TGate
+        self.braket_gate = gates.T
+        self.qlm_aqasm_keyword = "T"
+
     matrix = np.array([[1, 0], [0, exp((pi / 4) * 1j)]])
 
 
 class SWAP(InvolutionGate, NoParameterGate):
     """Two-qubit SWAP gate.
 
     Args:
         a: First target of the swapping operation.
         b: Second target of the swapping operation.
 
     Example:
-        >>> SWAP(0, 1)
+        >>> SWAP(0, 1).to_matrix()
         array([[1, 0, 0, 0],
                [0, 0, 1, 0],
                [0, 1, 0, 0],
                [0, 0, 0, 1]])
-    """
 
-    qiskit_gate = SwapGate
-    matrix = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
+    """
 
     def __init__(self, a: int, b: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import SwapGate
+
+        self.qiskit_gate = SwapGate
+        self.braket_gate = gates.Swap
+        self.qlm_aqasm_keyword = "SWAP"
+
+        self.matrix = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
         super().__init__([a, b], "SWAP")
 
+    nb_qubits = (  # pyright: ignore[reportAssignmentType,reportIncompatibleMethodOverride]
+        2
+    )
 
-class U(NativeGate, ParametrizedGate):
+
+class U(NativeGate, ParametrizedGate, SingleQubitGate):
     """Generic one qubit unitary gate. It is parametrized by 3 Euler angles.
 
     Args:
         theta: Parameter representing the first angle of the gate U.
         phi: Parameter representing the second angle of the gate U.
         gamma: Parameter representing the third angle of the gate U.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> U(np.pi/3, 0, np.pi/4, 0).to_matrix()
         array([[ 0.8660254 +0.j        , -0.35355339-0.35355339j],
                [ 0.5       +0.j        ,  0.61237244+0.61237244j]])
+
     """
 
     def __init__(
         self,
         theta: Expr | float,
         phi: Expr | float,
         gamma: Expr | float,
@@ -373,51 +516,80 @@
     def gamma(self):
         """See corresponding argument."""
         return self.parameters[2]
 
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
-        qiskit_parameters: Optional[set[Parameter]] = None,
+        qiskit_parameters: Optional[set["Parameter"]] = None,
     ):
-        if qiskit_parameters is None:
-            qiskit_parameters = set()
         if language == Language.QISKIT:
+            from qiskit.circuit.library import UGate
+
+            if qiskit_parameters is None:
+                qiskit_parameters = set()
+
             return UGate(
                 theta=_qiskit_parameter_adder(self.theta, qiskit_parameters),
                 phi=_qiskit_parameter_adder(self.phi, qiskit_parameters),
                 lam=_qiskit_parameter_adder(self.gamma, qiskit_parameters),
             )
+        elif language == Language.BRAKET:
+            from braket.circuits import gates
+
+            # 3M-TODO handle symbolic parameters
+            if (
+                isinstance(self.theta, Expr)
+                or isinstance(self.phi, Expr)
+                or isinstance(self.gamma, Expr)
+            ):
+                raise NotImplementedError(
+                    "Symbolic expressions are not yet supported for braket "
+                    "export, this feature is coming very soon!"
+                )
+
+            return gates.U(self.theta, self.phi, self.gamma)
         else:
             raise NotImplementedError(f"Error: {language} is not supported")
 
     def to_matrix(self) -> Matrix:
         c, s, eg, ep = (
             cos(self.theta / 2),  # type:ignore
             sin(self.theta / 2),  # type:ignore
             exp(self.gamma * 1j),  # type:ignore
             exp(self.phi * 1j),  # type:ignore
         )
         return np.array([[c, -eg * s], [ep * s, eg * ep * c]])  # type:ignore
 
+    qlm_aqasm_keyword = "U"
+
 
 class Rx(RotationGate, SingleQubitGate):
     """One qubit rotation around the X axis
 
     Args:
         theta: Parameter representing the angle of the gate.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> Rx(np.pi/5, 1).to_matrix()
         array([[0.95105652+0.j        , 0.        -0.30901699j],
                [0.        -0.30901699j, 0.95105652+0.j        ]])
+
     """
 
-    qiskit_gate = RXGate
+    def __init__(self, theta: Expr | float, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import RXGate
+
+        super().__init__(theta, target)
+
+        self.qiskit_gate = RXGate
+        self.braket_gate = gates.Rx
+        self.qlm_aqasm_keyword = "RX"
 
     def to_matrix(self) -> Matrix:
         c, s = cos(self.parameters[0] / 2), sin(self.parameters[0] / 2)  # type:ignore
         return np.array([[c, -1j * s], [-1j * s, c]])  # type:ignore
 
 
 class Ry(RotationGate, SingleQubitGate):
@@ -427,59 +599,85 @@
         theta: Parameter representing the angle of the gate.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> Ry(np.pi/5, 1).to_matrix()
         array([[ 0.95105652, -0.30901699],
                [ 0.30901699,  0.95105652]])
+
     """
 
-    qiskit_gate = RYGate
+    def __init__(self, theta: Expr | float, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import RYGate
+
+        super().__init__(theta, target)
+
+        self.qiskit_gate = RYGate
+        self.braket_gate = gates.Ry
+        self.qlm_aqasm_keyword = "RY"
 
     def to_matrix(self) -> Matrix:
         c, s = cos(self.parameters[0] / 2), sin(self.parameters[0] / 2)  # type:ignore
         return np.array([[c, -s], [s, c]])
 
 
 class Rz(RotationGate, SingleQubitGate):
     """One qubit rotation around the Z axis
 
     Args:
         theta: Parameter representing the angle of the gate.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
-        >>> Rz(np.pi/5, 1).to_matrix()
-        array([[0.95105652-0.30901699j, 0.        +0.j        ],
-               [0.        +0.j        , 0.95105652-0.30901699j]])
+        >>> print(clean_matrix(Rz(np.pi/5, 1).to_matrix()))
+        [[0.9510565-0.309017j, 0],
+         [0, 0.9510565+0.309017j]]
+
     """
 
-    qiskit_gate = RZGate
+    def __init__(self, theta: Expr | float, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import RZGate
+
+        super().__init__(theta, target)
+
+        self.qiskit_gate = RZGate
+        self.braket_gate = gates.Rz
+        self.qlm_aqasm_keyword = "RZ"
 
     def to_matrix(self) -> Matrix:
-        e = exp(-1j * self.parameters[0] / 2)  # type:ignore
-        return np.array([[e, 0], [0, e]])
+        e = exp(-1j * self.parameters[0] / 2)  # pyright: ignore[reportOperatorIssue]
+        return np.array(  # pyright: ignore[reportCallIssue]
+            [[e, 0], [0, 1 / e]]  # pyright: ignore[reportOperatorIssue]
+        )
 
 
 class Rk(RotationGate, SingleQubitGate):
     r"""One qubit Phase gate of angle `\frac{2i\pi}{2^k}`.
 
     Args:
         k: Parameter used in the definition of the phase to apply.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
         >>> Rk(5, 0).to_matrix()
         array([[1.        +0.j        , 0.        +0.j        ],
                [0.        +0.j        , 0.98078528+0.19509032j]])
-    """
 
-    qiskit_gate = PhaseGate
+    """
 
     def __init__(self, k: Expr | int, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import PhaseGate
+
+        self.qiskit_gate = PhaseGate
+        self.braket_gate = gates.PhaseShift
+        self.qlm_aqasm_keyword = "PH"
+
         self.parameters = [k]
         definition = UnitaryMatrix(self.to_matrix(), **self.native_gate_options)
         ParametrizedGate.__init__(self, definition, [target], [self.k], "Rk")
 
     @property
     def theta(self) -> Expr | float:
         r"""Value of the rotation angle, parametrized by ``k`` with the relation
@@ -497,83 +695,105 @@
         return np.array([[1, 0], [0, e]])
 
     def __repr__(self):
         return f"{type(self).__name__}({self.k}, {self.targets[0]})"
 
 
 class CNOT(InvolutionGate, NoParameterGate, ControlledGate):
-    """
-    Two-qubit Controlled-NOT gate.
+    """Two-qubit Controlled-NOT gate.
 
     Args:
         control: index referring to the qubit used to control the gate
         target: index referring to the qubit on which the gate will be applied
 
     Example:
         >>> CNOT(0, 1).to_matrix()
         array([[1, 0, 0, 0],
                [0, 1, 0, 0],
                [0, 0, 0, 1],
                [0, 0, 1, 0]])
-    """
 
-    qiskit_gate = CXGate
+    """
 
     def __init__(self, control: int, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import CXGate
+
+        self.qiskit_gate = CXGate
+        self.braket_gate = gates.CNot
+        self.qlm_aqasm_keyword = "CNOT"
         ControlledGate.__init__(self, [control], [target], X(target), "CNOT")
 
     def to_matrix(self) -> Matrix:
         return np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
 
+    nb_qubits = (  # pyright: ignore[reportAssignmentType,reportIncompatibleMethodOverride]
+        2
+    )
+
 
 class CZ(InvolutionGate, NoParameterGate, ControlledGate):
     """Two-qubit Controlled-Z gate.
 
     Args:
         control: Index referring to the qubit used to control the gate.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
-        >>> CZ(0, 1).to_matrix()
-        array([[ 1,  0,  0,  0],
-               [ 0,  1,  0,  0],
-               [ 0,  0,  1,  0],
-               [ 0,  0,  0, -1]])
-    """
+        >>> print(clean_matrix(CZ(0, 1).to_matrix()))
+        [[1, 0, 0, 0],
+         [0, 1, 0, 0],
+         [0, 0, 1, 0],
+         [0, 0, 0, -1]]
 
-    qiskit_gate = CZGate
+    """
 
     def __init__(self, control: int, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import CZGate
+
+        self.qiskit_gate = CZGate
+        self.braket_gate = gates.CZ
+        self.qlm_aqasm_keyword = "CSIGN"
         ControlledGate.__init__(self, [control], [target], Z(target), "CZ")
 
     def to_matrix(self) -> Matrix:
-        m = np.eye(8, dtype=complex)
+        m = np.eye(4, dtype=complex)
         m[-1, -1] = -1
         return m
 
+    nb_qubits = (  # pyright: ignore[reportAssignmentType,reportIncompatibleMethodOverride]
+        2
+    )
+
 
 class CRk(RotationGate, ControlledGate):
     """Two-qubit Controlled-Rk gate.
 
     Args:
         k: Parameter used in the definition of the phase to apply.
         control: Index referring to the qubit used to control the gate.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
-        >>> CRk(4, 0, 1)
-        array([[1.        +0.j        , 0.        +0.j        , 0.        +0.j        , 0.        +0.j        ],
-               [0.        +0.j        , 1.        +0.j        , 0.        +0.j        , 0.        +0.j        ],
-               [0.        +0.j        , 0.        +0.j        , 1.        +0.j        , 1.        +0.j        ],
-               [0.        +0.j        , 0.        +0.j        , 0.        +0.j        , 0.92387953+0.38268343j]])
-    """
+        >>> print(clean_matrix(CRk(4, 0, 1).to_matrix()))
+        [[1, 0, 0, 0],
+         [0, 1, 0, 0],
+         [0, 0, 1, 0],
+         [0, 0, 0, 0.9238795+0.3826834j]]
 
-    qiskit_gate = CPhaseGate
+    """
 
     def __init__(self, k: Expr | int, control: int, target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import CPhaseGate
+
+        self.qiskit_gate = CPhaseGate
+        self.braket_gate = gates.CPhaseShift
+        self.qlm_aqasm_keyword = ["CNOT", "PH"]
         self.parameters = [k]
         ControlledGate.__init__(self, [control], [target], Rk(k, target), "CRk")
         definition = UnitaryMatrix(self.to_matrix(), **self.native_gate_options)
         ParametrizedGate.__init__(self, definition, [target], [k], "CRk")
 
     @property
     def theta(self) -> Expr | float:
@@ -590,38 +810,56 @@
     def to_matrix(self) -> Matrix:
         e = exp(self.theta * 1j)  # type:ignore
         return np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, e]])
 
     def __repr__(self):
         return f"{type(self).__name__}({self.k}, {self.controls[0]}, {self.targets[0]})"
 
+    nb_qubits = (  # pyright: ignore[reportAssignmentType,reportIncompatibleMethodOverride]
+        2
+    )
+
 
 class TOF(InvolutionGate, NoParameterGate, ControlledGate):
     """Three-qubit Controlled-Controlled-NOT gate, also known as Toffoli Gate
 
     Args:
         control: List of indices referring to the qubits used to control the gate.
         target: Index referring to the qubit on which the gate will be applied.
 
     Example:
-        >>> TOF([0, 1], 2).to_matrix()
-        array([[1, 0, 0, 0, 0, 0, 0, 0],
-               [0, 1, 0, 0, 0, 0, 0, 0],
-               [0, 0, 1, 0, 0, 0, 0, 0],
-               [0, 0, 0, 1, 0, 0, 0, 0],
-               [0, 0, 0, 0, 1, 0, 0, 0],
-               [0, 0, 0, 0, 0, 1, 0, 0],
-               [0, 0, 0, 0, 0, 0, 0, 1],
-               [0, 0, 0, 0, 0, 0, 1, 0]])
-    """
+        >>> print(clean_matrix(TOF([0, 1], 2).to_matrix()))
+        [[1, 0, 0, 0, 0, 0, 0, 0],
+         [0, 1, 0, 0, 0, 0, 0, 0],
+         [0, 0, 1, 0, 0, 0, 0, 0],
+         [0, 0, 0, 1, 0, 0, 0, 0],
+         [0, 0, 0, 0, 1, 0, 0, 0],
+         [0, 0, 0, 0, 0, 1, 0, 0],
+         [0, 0, 0, 0, 0, 0, 0, 1],
+         [0, 0, 0, 0, 0, 0, 1, 0]]
 
-    qiskit_gate = CCXGate
+    """
 
     def __init__(self, control: list[int], target: int):
+        from braket.circuits import gates
+        from qiskit.circuit.library import CCXGate
+
+        self.qiskit_gate = CCXGate
+        self.braket_gate = gates.CCNot
+        self.qlm_aqasm_keyword = "CCNOT"
         if len(control) != 2:
             raise ValueError("A Toffoli gate must have exactly 2 control qubits.")
         ControlledGate.__init__(self, control, [target], X(target), "TOF")
 
     def to_matrix(self) -> Matrix:
         m = np.identity(8, dtype=complex)
         m[-2:, -2:] = np.ones(2) - np.identity(2)
         return m
+
+    nb_qubits = (  # pyright: ignore[reportAssignmentType,reportIncompatibleMethodOverride]
+        3
+    )
+
+
+NATIVE_GATES = [CNOT, CRk, CZ, H, Id, P, Rk, Rx, Ry, Rz, S, SWAP, T, TOF, U, X, Y, Z]
+# 3M-TODO : check the possibility to detect when a custom gate can be defined as a native gate, problem with
+#  parametrized gates maybe
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/gates/parametrized_gate.py` & `mpqp-0.2.0/mpqp/core/instruction/gates/parametrized_gate.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 More on the topic of symbolic variable can be found in the `VQA <VQA.html>`_
 page"""
 
 from __future__ import annotations
 
 from abc import ABC
 from copy import deepcopy
-from typing import Optional
 from numbers import Complex
+from typing import Optional
 
 from sympy import Expr, symbols  # pyright: ignore [reportUnusedImport]
 from typeguard import typechecked
 
 from mpqp.core.instruction.gates.gate import Gate
 from mpqp.core.instruction.gates.gate_definition import GateDefinition
 
@@ -25,29 +25,30 @@
 #  initialization of ParametrizedGate. For now this problem is manually tackled
 #  by instantiating self.parameters before the computation of the gates's
 #  definition but this solution looks like a conception problem...
 
 
 @typechecked
 class ParametrizedGate(Gate, ABC):
-    """
-    Define a parametrized gate.
+    """Define a parametrized gate.
 
     Args:
-        definition: Provide a definition of the gate (matrix, gate combination, ...).
+        definition: Provide a definition of the gate (matrix, gate combination,
+            ...).
         targets: List of indices referring to the qubits on which the gate will
             be applied.
         parameters: List of parameters used to define the gate.
         label: Label used to identify the measurement.
 
-    Examples:
+    Example:
         >>> theta = np.pi/3
         >>> c, s = np.cos(theta / 2), np.sin(theta / 2)
         >>> gate_def = UnitaryMatrix(np.array([[c, s], [-s, c]]))
-        >>> parametrized = ParametrizedGate(gate_def, 3, theta)
+        >>> parametrized = ParametrizedGate(gate_def, [3], [theta])
+
     """
 
     def __init__(
         self,
         definition: GateDefinition,
         targets: list[int],
         parameters: list[Expr | float],
@@ -72,7 +73,10 @@
         concrete_gate.parameters = [
             caster(param.subs(values)) if isinstance(param, Expr) else param
             for param in self.parameters
         ]
         concrete_gate._numeric_parameters = True
 
         return concrete_gate
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.parameters},{self.targets})"
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/instruction.py` & `mpqp-0.2.0/mpqp/core/instruction/instruction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """An :class:`Instruction` is the base element for circuits elements, containing
 common methods to all of them."""
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from copy import deepcopy
-from typing import Any, Optional
 from numbers import Complex
+from pickle import dumps
+from typing import TYPE_CHECKING, Any, Optional
 
 from sympy import Expr
-from qiskit.circuit import Parameter
 from typeguard import typechecked
 
+if TYPE_CHECKING:
+    from qiskit.circuit import Parameter
+
 from mpqp.core.languages import Language
-from mpqp.tools.generics import flatten
+from mpqp.tools.generics import SimpleClassReprABC, flatten
 
 
 @typechecked
-class Instruction(ABC):
+class Instruction(SimpleClassReprABC):
     """Abstract class defining an instruction of a quantum circuit.
 
     An Instruction is the elementary component of a
     :class:`QCircuit<mpqp.core.circuit>`. It consists in a manipulation of one
     (or several) qubit(s) of the quantum circuit. It may involve classical bits
     as well, for defining or retrieving the result of the instruction.
 
@@ -29,127 +32,132 @@
 
         - :class:`Gate<mpqp.core.instruction.gates.gate.Gate>`
         - :class:`Measure<mpqp.core.instruction.measurement.measure.Measure>`
         - :class:`Barrier<mpqp.core.instruction.barrier.Barrier>`
 
     Args:
         targets: List of indices referring to the qubits on which the
-            instruction will be applied
-        label: label used to identify the instruction
+            instruction will be applied.
+        label: Label used to identify the instruction.
     """
 
     def __init__(
         self,
         targets: list[int],
         label: Optional[str] = None,
     ):
+        if len(targets) == 0:
+            raise ValueError("Expected non-empty target list")
         if len(set(targets)) != len(targets):
             raise ValueError(f"Duplicate registers in targets: {targets}")
         if not all([t >= 0 for t in targets]):
             raise ValueError(f"Negative index in targets: {targets}")
         self.targets = targets
         """See parameter description."""
         self.label = label
         """See parameter description."""
 
     @property
     def nb_qubits(self) -> int:
-        """Number of qubits of this instruction"""
+        """Number of qubits of this instruction."""
         return len(self.connections())
 
     @property
     def nb_cbits(self) -> int:
-        """Number of cbits of this instruction"""
+        """Number of cbits of this instruction."""
         from mpqp.core.instruction.measurement.basis_measure import BasisMeasure
 
         if isinstance(self, BasisMeasure):
             return len(flatten([self.c_targets]))
         else:
             return 0
 
     @abstractmethod
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
         qiskit_parameters: Optional[set[Parameter]] = None,
     ) -> Any:
-        """Transform this instruction into the corresponding object in the
+        """Transforms this instruction into the corresponding object in the
         language specified in the ``language`` arg.
 
         By default, the instruction is translated to the corresponding one in
         Qiskit, since it is the interface we use to generate the OpenQASM code.
 
         In the future, we will generate the OpenQASM code on our own, and this
         method will be used only for complex objects that are not tractable by
         OpenQASM (like hybrid structures).
 
         Args:
-            language: enum representing the target language.
+            language: Enum representing the target language.
             qiskit_parameters: We need to keep track of the parameters
                 passed to qiskit in order not to define twice the same
                 parameter. Defaults to ``set()``.
 
         Returns:
             The corresponding instruction (gate or measure) in the target
-            language
+            language.
         """
         pass
 
+    def __eq__(self, value: object) -> bool:
+        return dumps(self) == dumps(value)
+
     def __str__(self) -> str:
         from mpqp.core.circuit import QCircuit
 
-        c = QCircuit(
-            (self.targets if isinstance(self.targets, int) else max(self.targets)) + 1
-        )
+        c = QCircuit(max(self.connections()) + 1)
         c.add(self)
         return str(c)
 
     def __repr__(self) -> str:
         from mpqp.core.instruction.gates import ControlledGate
 
         controls = str(self.controls) + "," if isinstance(self, ControlledGate) else ""
         return f"{type(self).__name__}({controls}{self.targets})"
 
     def connections(self) -> set[int]:
         """Returns the indices of the qubits connected to the instruction.
 
+        Returns:
+            The qubits ordered connected to instruction.
+
         Example:
             >>> CNOT(0,1).connections()
-            [0, 1]
+            {0, 1}
 
-        Returns:
-            The qubits ordered connected to instruction.
         """
         from mpqp.core.instruction.gates import ControlledGate
 
         return (
             set(self.controls).union(self.targets)
             if isinstance(self, ControlledGate)
             else set(self.targets)
         )
 
     def subs(
         self, values: dict[Expr | str, Complex], remove_symbolic: bool = False
     ) -> Instruction:
-        r"""Substitute the parameters of the instruction with complex values.
-        Optionally also remove all symbolic variables such as `\pi` (needed for
+        r"""Substitutes the parameters of the instruction with complex values.
+        Optionally also removes all symbolic variables such as `\pi` (needed for
         example for circuit execution).
 
         Since we use ``sympy`` for gates' parameters, ``values`` can in fact be
         anything the ``subs`` method from ``sympy`` would accept.
 
-        Example:
-            >>> theta = symbols("θ")
-            >>> print(Rx(theta, 0).subs({theta: np.pi}))
-               ┌───────┐
-            q: ┤ Rx(π) ├
-               └───────┘
-
         Args:
             values: Mapping between the variables and the replacing values.
             remove_symbolic: If symbolic values should be replaced by their
                 numeric counterpart.
 
         Returns:
             The circuit with the replaced parameters.
+
+        Example:
+            >>> theta = symbols("θ")
+            >>> print(Rx(theta, 0).subs({theta: np.pi}))
+               ┌───────┐
+            q: ┤ Rx(π) ├
+               └───────┘
+
         """
         return deepcopy(self)
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/measurement/basis_measure.py` & `mpqp-0.2.0/mpqp/core/instruction/measurement/basis_measure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """The :class:`BasisMeasure` is used to project the state on a statevector of a
 given :class:`Basis` and returns the corresponding eigenvalue."""
 
 from __future__ import annotations
-from typing import Optional
 
-import qiskit.circuit
-from qiskit.circuit import Parameter
+from typing import TYPE_CHECKING, Optional
+
 from typeguard import typechecked
 
-from .measure import Measure
-from .basis import Basis, ComputationalBasis
+if TYPE_CHECKING:
+    from qiskit.circuit import Parameter
+
 from mpqp.core.languages import Language
 
+from .basis import Basis, ComputationalBasis
+from .measure import Measure
+
 
 @typechecked
 class BasisMeasure(Measure):
     """Class representing a measure of one or several qubits in a specific
     basis.
 
     By default, the computational basis will be used. The user can also precise
@@ -34,17 +37,18 @@
             should be measured.
         basis: Basis in which the measure is performed. Defaults to
             :class:`ComputationalBasis()<mpqp.core.instruction.measurement.basis.ComputationalBasis>`
         label: Label used to identify the measure.
 
     Examples:
         >>> c1 = QCircuit([H(0), H(1), CNOT(0,1)])
-        >>> c1.add(BasisMeasure([0, 1, 2], shots=1024))
+        >>> c1.add(BasisMeasure([0, 1], shots=1024))
         >>> c2 = QCircuit([H(0), H(1), CNOT(0,1)])
-        >>> c2.add(BasisMeasure([0, 1, 2], shots=1024, basis=HadamardBasis()))
+        >>> c2.add(BasisMeasure([0, 1], shots=1024, basis=HadamardBasis()))
+
     """
 
     def __init__(
         self,
         targets: list[int],
         c_targets: Optional[list[int]] = None,
         shots: int = 0,
@@ -63,21 +67,23 @@
         """See parameter description."""
         self.basis = basis
         """See parameter description."""
 
     def to_other_language(
         self,
         language: Language = Language.QISKIT,
-        qiskit_parameters: Optional[set[Parameter]] = None,
+        qiskit_parameters: Optional[set["Parameter"]] = None,
     ):
         if qiskit_parameters is None:
             qiskit_parameters = set()
         if language == Language.QISKIT:
+            from qiskit.circuit import Measure
+
             if isinstance(self.basis, ComputationalBasis):
-                return qiskit.circuit.Measure()
+                return Measure()
             else:
                 raise NotImplementedError(f"{type(self.basis)} not handled")
         else:
             raise NotImplementedError(f"{language} is not supported")
 
     def __repr__(self) -> str:
         options = ""
```

### Comparing `mpqp-0.1.dev1/mpqp/core/instruction/measurement/measure.py` & `mpqp-0.2.0/mpqp/core/instruction/measurement/measure.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/mpqp/execution/connection/aws_connection.py` & `mpqp-0.2.0/mpqp/execution/connection/aws_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 import os
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from botocore.exceptions import NoRegionError
-from braket.aws import AwsDevice, AwsSession
-from braket.devices import LocalSimulator
-from braket.devices.device import Device as BraketDevice
 from termcolor import colored
 from typeguard import typechecked
 
+if TYPE_CHECKING:
+    from braket.devices.device import Device as BraketDevice
+
 from mpqp.execution.connection.env_manager import get_env_variable, save_env_variable
 from mpqp.execution.devices import AWSDevice
 from mpqp.tools.errors import AWSBraketRemoteExecutionError
 
 
 def setup_aws_braket_account() -> tuple[str, list[Any]]:
-    """Set up the connection to an Amazon Braket account using user input.
+    """Setups the connection to an Amazon Braket account using user input.
 
     This function checks whether an Amazon Braket account is already configured
     and prompts the user to update it if needed. It then collects the user's AWS
     access key, AWS secret key (hidden input), and the AWS region for Amazon
     Braket. The function attempts to configure the Amazon Braket account using
     the provided credentials.
 
     Returns:
         A tuple containing a message indicating the result of the setup (e.g.,
         success, cancelled, or error, ...) and an empty list. The list is
         included for consistency with the existing code structure.
     """
+    from braket.aws import AwsSession
 
-    already_configured = get_env_variable("BRAKET_CONFIGURED") == "True"
-
-    if already_configured:
+    if get_env_variable("BRAKET_CONFIGURED") == "True":
         decision = input(
             "An Amazon Braket account is already configured. Do you want to update it? [y/N] "
         )
         if decision.lower().strip() != "y":
             return "Canceled.", []
 
     try:
         os.system("aws configure")
         save_env_variable("BRAKET_CONFIGURED", "True")
+        session = AwsSession()
+        save_env_variable("AWS_DEFAULT_REGION", session.region)
         return "Amazon Braket account correctly configured", []
 
     except Exception as e:
         print(colored("Error configuring Amazon Braket account", "red"))
         print(colored(str(e), "red"))
         input("Press 'Enter' to continue")
         return "", []
 
 
 def get_aws_braket_account_info() -> str:
     """Get AWS Braket credentials information including access key ID,
     obfuscated secret access key, and region.
 
-    Examples:
+    Returns:
+        A formatted string containing AWS credentials information with an
+        obfuscated secret access key.
+
+    Example:
         >>> get_aws_braket_account_info()
             access_key_id: 'AKIA26NYJ***********'
             secret_access_key: 'sMDad***********************************'
             region: 'us-east-1'
 
-    Returns:
-        A formatted string containing AWS credentials information with an
-        obfuscated secret access key.
-
     """
     if get_env_variable("BRAKET_CONFIGURED") == "False":
         raise AWSBraketRemoteExecutionError(
             "Error when trying to get AWS credentials. No AWS Braket account configured."
         )
+    from braket.aws import AwsSession
 
     try:
         session = AwsSession()
 
         # get the AWS Braket user access key, secret key and region
         access_key_id = session.boto_session.get_credentials().access_key
 
@@ -87,78 +88,101 @@
 
     return f"""    access_key_id: '{access_key_id}'
     secret_access_key: '{obfuscate_key}' 
     region: '{region_name}'"""
 
 
 @typechecked
-def get_braket_device(device: AWSDevice) -> BraketDevice:
-    """
-    Returns the AwsDevice device associate with the AWSDevice in parameter.
+def get_braket_device(device: AWSDevice, is_noisy: bool = False) -> "BraketDevice":
+    """Returns the AwsDevice device associate with the AWSDevice in parameter.
 
     Args:
         device: AWSDevice element describing which remote/local AwsDevice we want.
+        is_noisy: If the expected device is noisy or not.
+
+    Raises:
+        AWSBraketRemoteExecutionError: If the device or the region could not be
+            retrieved.
 
-    Examples:
+    Example:
         >>> device = get_braket_device(AWSDevice.BRAKET_RIGETTI_ASPEN_M_3)
         >>> device.properties.action['braket.ir.jaqcd.program'].supportedResultTypes
         [ResultType(name='Sample', observables=['x', 'y', 'z', 'h', 'i'], minShots=10, maxShots=100000),
          ResultType(name='Expectation', observables=['x', 'y', 'z', 'h', 'i'], minShots=10, maxShots=100000),
          ResultType(name='Variance', observables=['x', 'y', 'z', 'h', 'i'], minShots=10, maxShots=100000),
          ResultType(name='Probability', observables=None, minShots=10, maxShots=100000)]
 
     Raises:
-        AWSBraketRemoteExecutionError
+        AWSBraketRemoteExecutionError: If the device or the region could not be
+            retrieved.
     """
+    import boto3
+    from botocore.exceptions import NoRegionError
+    from braket.aws import AwsDevice, AwsSession
+    from braket.devices import LocalSimulator
 
     if not device.is_remote():
-        return LocalSimulator()
+        if is_noisy:
+            return LocalSimulator("braket_dm")
+        else:
+            return LocalSimulator()
 
     try:
-        return AwsDevice(device.get_arn())
+        braket_client = boto3.client("braket", region_name=device.get_region())
+        aws_session = AwsSession(braket_client=braket_client)
+        aws_session.add_braket_user_agent(user_agent="APN/1.0 ColibriTD/1.0 MPQP/1.0")
+        return AwsDevice(device.get_arn(), aws_session=aws_session)
     except ValueError as ve:
         raise AWSBraketRemoteExecutionError(
             "Failed to retrieve remote AWS device. Please check the arn, or if the "
             "device is accessible from your region..\nTrace: " + str(ve)
         )
     except NoRegionError as err:
         raise AWSBraketRemoteExecutionError(
             "Failed to find the region related with your aws credentials. Make sure you"
             "configured correctly your AWS account with 'setup_connections.py' script."
             "\nTrace: " + str(err)
         )
 
 
 def get_all_task_ids() -> list[str]:
-    """Retrieve all the task ids of this account/group from AWS.
+    """Retrieves all the task ids of this account/group from AWS.
 
-    Examples:
+    Example:
         >>> get_all_task_ids()
         ['arn:aws:braket:us-east-1:752542621531:quantum-task/6a46ae9a-d02f-4a23-b46f-eae43471bc22',
          'arn:aws:braket:us-east-1:752542621531:quantum-task/11db7e68-2b17-4b00-a4ec-20f662fd4876',
          'arn:aws:braket:us-east-1:752542621531:quantum-task/292d329f-727c-4b92-83e1-7d4bedd4b243',
          'arn:aws:braket:us-east-1:752542621531:quantum-task/4b94c703-2ce8-480b-b3f3-ecb2580dbb82',
          'arn:aws:braket:us-east-1:752542621531:quantum-task/edc094aa-23e8-4a8c-87be-f2e09281d79d',
          'arn:aws:braket:us-east-1:752542621531:quantum-task/af9e623a-dd1c-4ecb-9db6-dbbd1af08110']
+
     """
-    return [
-        task["quantumTaskArn"]
-        for task in (
-            AwsSession().braket_client.search_quantum_tasks(filters=[])["quantumTasks"]
-        )
-    ]
+    from braket.aws import AwsSession
+
+    if get_env_variable("BRAKET_CONFIGURED") == "True":
+        return [
+            task["quantumTaskArn"]
+            for task in (
+                AwsSession().braket_client.search_quantum_tasks(filters=[])[
+                    "quantumTasks"
+                ]
+            )
+        ]
+    return []
 
 
 def get_all_partial_ids() -> list[str]:
-    """Retrieve all the task ids of this account/group from AWS and extracts the
+    """Retrieves all the task ids of this account/group from AWS and extracts the
     significant part.
 
-    Examples:
+    Example:
         >>> get_all_partial_ids()
         ['6a46ae9a-d02f-4a23-b46f-eae43471bc22',
          '11db7e68-2b17-4b00-a4ec-20f662fd4876',
          '292d329f-727c-4b92-83e1-7d4bedd4b243',
          '4b94c703-2ce8-480b-b3f3-ecb2580dbb82',
          'edc094aa-23e8-4a8c-87be-f2e09281d79d',
          'af9e623a-dd1c-4ecb-9db6-dbbd1af08110']
+
     """
     return [id.split("/")[-1] for id in get_all_task_ids()]
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/connection/env_manager.py` & `mpqp-0.2.0/mpqp/execution/connection/env_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,117 @@
 """This module takes care of saving and loading the configuration of supported
 providers."""
 
 import os
-from dotenv import set_key, load_dotenv
+
+from dotenv import load_dotenv, set_key
 from typeguard import typechecked
 
 MPQP_CONFIG_PATH = os.path.expanduser("~") + "/.mpqp"
 
 
 def _create_config_if_needed():
     """If there is not already a ``.mpqp`` file we create it."""
     if not os.path.exists(MPQP_CONFIG_PATH):
         open(MPQP_CONFIG_PATH, "a").close()
 
 
 def get_existing_config_str() -> str:
-    """Gets the content of the ``.mpqp`` config file
+    """Gets the content of the ``.mpqp`` config file.
 
-    Examples:
-        >>> get_existing_config_str()
-        IBM_TOKEN='e7c9*************'
-        IBM_CONFIGURED='True'
+    Returns:
+        The string with .mpqp file content.
+
+    Example:
+        >>> save_env_variable('QLM_USER', 'hjaffali')
+        True
+        >>> save_env_variable('QLM_PASSWD', '****************')
+        True
+        >>> save_env_variable('QLM_CONFIGURED', 'True')
+        True
+        >>> save_env_variable('BRAKET_CONFIGURED', 'True')
+        True
+        >>> print(get_existing_config_str()) # doctest: +NORMALIZE_WHITESPACE
         QLM_USER='hjaffali'
         QLM_PASSWD='****************'
         QLM_CONFIGURED='True'
         BRAKET_CONFIGURED='True'
 
-    Returns:
-        The string with .mpqp file content.
     """
+    if not os.path.exists(MPQP_CONFIG_PATH):
+        return ""
     with open(MPQP_CONFIG_PATH, "r") as mpqp:
         file_str = mpqp.read()
     return file_str
 
 
 def load_env_variables() -> bool:
-    """Load the variables stored in the ``.mpqp`` file.
+    """Loads the variables stored in the ``.mpqp`` file.
 
-    Examples:
-        >>> os.getenv("IBM_CONFIGURED")
+    Returns:
+        ``True`` if the variables are loaded correctly.
 
+    Example:
+        >>> os.getenv("IBM_CONFIGURED")
+        >>> open(os.path.expanduser("~") + "/.mpqp", "w").write("IBM_CONFIGURED='True'\\n")
+        22
+        >>> os.getenv("IBM_CONFIGURED")
         >>> load_env_variables()
         True
         >>> os.getenv("IBM_CONFIGURED")
         'True'
 
-    Returns:
-        True if the variables are loaded correctly.
     """
     load_dotenv(MPQP_CONFIG_PATH, override=True)
     return True
 
 
 @typechecked
 def get_env_variable(key: str) -> str:
-    """Load the ``.mpqp`` env file and return the value associated with the key
-    in parameter. If the variable doesn't exist, an empty string is returned.
+    """Loads the ``.mpqp`` env file and returns the value associated with the key
+    in parameter. If the variable does not exist, an empty string is returned.
 
-    Examples:
+    Args:
+        key: The key for which we want to get the value.
+
+    Example:
+        >>> save_env_variable("BRAKET_CONFIGURED", 'True')
+        True
         >>> get_env_variable("BRAKET_CONFIGURED")
         'True'
         >>> get_env_variable("RaNdOM")
         ''
 
-    Args:
-        key: The key for which we want to get the value.
     """
     _create_config_if_needed()
     load_env_variables()
     val = os.getenv(key, "")
 
     return val
 
 
 @typechecked
 def save_env_variable(key: str, value: str) -> bool:
     """Adds or updates the ``key`` environment variable in ``.mpqp`` file.
 
+    Args:
+        key: Name of the environment variable.
+        value: Value to be saved.
+
+    Returns:
+        ``True`` if the save was successful.
+
     Examples:
         >>> get_env_variable("RaNdOM")
         ''
         >>> save_env_variable("RaNdOM", "azertyuiop")
         True
         >>> get_env_variable("RaNdOM")
         'azertyuiop'
 
-    Args:
-        key: Name of the environment variable.
-        value: Value to be saved.
-
-    Returns:
-        True if the save was successful.
     """
     _create_config_if_needed()
 
     try:
         a, _, _ = set_key(MPQP_CONFIG_PATH, key, value)
         if a is None:
             raise SystemError(
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/connection/ibm_connection.py` & `mpqp-0.2.0/mpqp/execution/connection/ibm_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from getpass import getpass
+from typing import TYPE_CHECKING
 
-from qiskit.providers import QiskitBackendNotFoundError
-from qiskit.providers.backend import BackendV1
 from qiskit_ibm_provider import IBMProvider
 from qiskit_ibm_provider.accounts import AccountNotFoundError
 from qiskit_ibm_provider.api.exceptions import RequestsApiError
-from qiskit_ibm_runtime import QiskitRuntimeService
 from termcolor import colored
 from typeguard import typechecked
 
-from mpqp.execution.connection.env_manager import (get_env_variable,
-                                                   save_env_variable)
+if TYPE_CHECKING:
+    from qiskit.providers.backend import BackendV1
+    from qiskit_ibm_runtime import QiskitRuntimeService
+
+from mpqp.execution.connection.env_manager import get_env_variable, save_env_variable
 from mpqp.execution.devices import IBMDevice
 from mpqp.tools.errors import IBMRemoteExecutionError
 
 Ibm_Provider = None
 Runtime_Service = None
 
 
 @typechecked
 def config_ibm_account(token: str):
-    """
-    Configure and save locally IBM Quantum account's information.
+    """Configure and save locally IBM Quantum account's information.
 
     Args:
         token: IBM Quantum API token.
 
     Raises:
         IBMRemoteExecutionError
     """
@@ -39,16 +39,15 @@
         save_env_variable("IBM_CONFIGURED", "False")
         raise IBMRemoteExecutionError(
             "Error when saving the account.\nTrace: " + str(err)
         )
 
 
 def setup_ibm_account():
-    """Setup the IBM Q account, by looking at the existing configuration, asking for the token and update
-    the current account."""
+    """Setups and updates the IBM Q account using the existing configuration and by asking for the token ."""
     was_configured = get_env_variable("IBM_CONFIGURED") == "True"
 
     if was_configured:
         decision = input(
             "An IBMQ account is already configured. Do you want to update it? [y/N]"
         )
         if decision.lower().strip() != "y":
@@ -69,46 +68,49 @@
         else:
             save_env_variable("IBM_CONFIGURED", "False")
         getpass("Press 'Enter' to continue")
         return "", []
 
 
 def test_connection() -> bool:
-    """
-    Tests if the connection to the provider works. Returns False if login failed, True otherwise.
+    """Tests if the connection to the provider works.
+
+    Returns:
+        ``False`` if login failed.
     """
     try:
         IBMProvider()
     except RequestsApiError as err:
         if "Login failed" in str(err):
             print(colored("Wrong credentials", "red"))
             return False
         else:
             raise err
     return True
 
 
 def get_IBMProvider() -> IBMProvider:
-    """
-    Returns the IBMProvider needed to get one or several backends for execution
+    """Returns the IBMProvider needed to get one or several backends for
+    execution.
+
+    Raises:
+        IBMRemoteExecutionError
 
-    Examples:
+    Example:
         >>> instance = get_IBMProvider()
         >>> instance.backends()
         [<IBMBackend('ibmq_qasm_simulator')>,
          <IBMBackend('simulator_extended_stabilizer')>,
          <IBMBackend('simulator_mps')>,
          <IBMBackend('simulator_stabilizer')>,
          <IBMBackend('simulator_statevector')>,
          <IBMBackend('ibm_brisbane')>,
          <IBMBackend('ibm_kyoto')>,
          <IBMBackend('ibm_osaka')>]
 
-    Raises:
-        IBMRemoteExecutionError
     """
     global Ibm_Provider
     if Ibm_Provider is None:
         if get_env_variable("IBM_CONFIGURED") == "False":
             raise IBMRemoteExecutionError(
                 "Error when instantiating IBM Provider. No IBM Q account configured."
             )
@@ -123,30 +125,34 @@
             raise IBMRemoteExecutionError(
                 "Error when instantiating IBM Provider. No IBM Q account configured.\nTrace: "
                 + str(err)
             )
     return Ibm_Provider
 
 
-def get_QiskitRuntimeService() -> QiskitRuntimeService:
-    """
-    Returns the QiskitRuntimeService needed for remote connection and execution
+def get_QiskitRuntimeService() -> "QiskitRuntimeService":
+    """Returns the QiskitRuntimeService needed for remote connection and
+    execution.
+
+    Raises:
+        IBMRemoteExecutionError: When the ``qiskit`` runtime is not configured
+            or the configuration cannot be retrieved.
 
-    Examples:
+    Example:
         >>> service = get_QiskitRuntimeService()
         >>> service.jobs()
         [<RuntimeJob('cmdj3b4nktricigarn8g', 'estimator')>,
          <RuntimeJob('cmdj3a74mi97k7j7ujv0', 'sampler')>,
          <RuntimeJob('cmama29054sir2cq94og', 'estimator')>,
          <RuntimeJob('cmama14pduldih1q4ktg', 'sampler')>,
          <RuntimeJob('cm7vds4pduldih1k1mq0', 'sampler')>]
 
-    Raises:
-        IBMRemoteExecutionError
     """
+    from qiskit_ibm_runtime import QiskitRuntimeService
+
     global Runtime_Service
     if Runtime_Service is None:
         if get_env_variable("IBM_CONFIGURED") == "False":
             raise IBMRemoteExecutionError(
                 "Error when instantiating QiskitRuntimeService. No IBM account configured."
             )
         try:
@@ -156,100 +162,103 @@
                 "Error when instantiating QiskitRuntimeService (probably wrong token saved "
                 "in the account).\nTrace: " + str(err)
             )
     return Runtime_Service
 
 
 def get_active_account_info() -> str:
-    """
-    Returns the information concerning the active IBMQ account
+    """Returns the information concerning the active IBMQ account.
 
-    Args:
+    Returns:
+        The description containing the account information.
 
-    Examples:
+    Example:
         >>> print(get_active_account_info())
             Channel: ibm_quantum
             Instance: ibm-q-startup/colibritd/default
             Token: bf5e5*****
             URL: https://auth.quantum-computing.ibm.com/api
             Verify: True
 
-    Returns:
-        a string describin the account info
     """
     provider = get_IBMProvider()
     account = provider.active_account()
     assert account is not None
     return f"""    Channel: {account["channel"]}
     Instance: {account["instance"]}
     Token: {account["token"][:5]}*****
     URL: {account["url"]}
     Verify: {account["verify"]}"""
 
 
 @typechecked
-def get_backend(device: IBMDevice) -> BackendV1:
-    """
-    Retrieve the IBM Q remote device corresponding to the device in parameter
+def get_backend(device: IBMDevice) -> "BackendV1":
+    """Retrieves the IBM Q remote device corresponding to the device in
+    parameter.
 
     Args:
         device: The IBMDevice to get from IBMQ provider.
 
-    Examples:
+    Returns:
+        The requested backend.
+
+    Example:
         >>> brisbane = get_backend(IBMDevice.IBM_BRISBANE)
         >>> brisbane.properties().gates[0].parameters
         [Nduv(datetime.datetime(2024, 1, 9, 11, 3, 18, tzinfo=tzlocal()), gate_error, , 0.00045619997922344296),
          Nduv(datetime.datetime(2024, 1, 9, 15, 41, 39, tzinfo=tzlocal()), gate_length, ns, 60)]
 
-    Returns:
-        a qiskit.providers.backend.Backend object that will be use to execute circuit
-
     Raises:
-        IBMRemoteExecutionError
+        ValueError: If the required backend is a local simulator.
+        IBMRemoteExecutionError: If the device was not found.
     """
     # NOTE:
     #       Question : when a backend is present in several IBMQ instances, which instance does it use to submit jobs
     # on this backend ? Typically if with colibritd instance i have more priority and by default it uses ibmq
     # instance, then i lose something here.
     #       Answer : it takes the default instance attached to the account (the higher plan, usually).
     if not device.is_remote():
         raise ValueError("Expected a remote IBMQ device but got a local simulator.")
+    from qiskit.providers import QiskitBackendNotFoundError
 
     provider = get_IBMProvider()
 
     try:
         backend = provider.get_backend(device.value)
-
     except QiskitBackendNotFoundError as err:
         raise IBMRemoteExecutionError(
             f"Requested device {device} not found. Verify if your instances "
             "allows to access this machine, or the device's name.\n"
             f"Trace: {err}"
         )
 
     return backend
 
 
 def get_all_job_ids() -> list[str]:
-    """
-    Retrieve all the job ids of this account from the several IBM remote providers
-    (IBMProvider, QiskitRuntimeService, ...)
+    """Retrieves all the job ids of this account from the several IBM remote
+    providers (IBMProvider, QiskitRuntimeService, ...).
 
-    Examples:
+    Returns:
+        The list of job ids.
+
+    Example:
         >>> get_all_job_ids()
         ['cm6pp7e879ps6bbo7m30', 'cm6ou0q70abqioeudkd0', 'cm6opgcpduldih1hq7j0', 'cm01vp4pduldih0uoi2g',
         'cnvw8z3b08x0008y3e4g', 'cnvw7qyb08x0008y3e0g', 'cnvw7fdvn4c0008a6ztg', 'cnvw79dvn4c0008a6zt0',
         'cnvw64rb08x0008y3dx0', 'cnvw5z7wsx00008wybcg', 'cmdj3b4nktricigarn8g', 'cmdj3a74mi97k7j7ujv0',
         'cmama29054sir2cq94og', 'cmama14pduldih1q4ktg', 'cm80qmi70abqiof0o170', 'cm80qlkpduldih1k4png',
         'cm80pb1054sir2ck9i3g', 'cm80pa6879ps6bbqg2pg', 'cm7vdugiidfp3m8rg02g', 'cm7vds4pduldih1k1mq0']
+
     """
     all_job_ids = []
-
-    ibm_provider = get_IBMProvider()  # using IBMProvider
-    service = get_QiskitRuntimeService()  # using QiskitRuntimeService
+    if get_env_variable("IBM_CONFIGURED") != "True":
+        return all_job_ids
+    ibm_provider = get_IBMProvider()
+    service = get_QiskitRuntimeService()
 
     if ibm_provider:
         all_job_ids.extend([job.job_id() for job in ibm_provider.jobs()])
 
     if service:
         all_job_ids.extend([job.job_id() for job in service.jobs()])
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/connection/qlm_connection.py` & `mpqp-0.2.0/mpqp/execution/connection/qlm_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import annotations
-from typing import Any
 
-from typeguard import typechecked
-from getpass import getpass
 import os
+from getpass import getpass
+from typing import Any
 
 from termcolor import colored
+from typeguard import typechecked
 
 from mpqp.execution.connection.env_manager import (
-    save_env_variable,
     get_env_variable,
     load_env_variables,
+    save_env_variable,
 )
 from mpqp.tools.errors import QLMRemoteExecutionError
 
 QLM_connection = None
 
 
 @typechecked
 def config_qlm_account(username: str, password: str, global_config: bool) -> bool:
-    """Configure and save locally QLM account's information.
+    """Configures and saves locally QLM account's information.
 
     Args:
         username: QLM username.
         password: QLM password.
         global_config: If True, this QLM account will be configured to work even
             outside MPQP.
 
     Raises:
-        QLMRemoteExecutionError
+        QLMRemoteExecutionError: TODO
     """
     # store the username and password in environment variables QLM_USER and QLM_PASSWD in .mpqp
     prev_user = get_env_variable("QLM_USER")
     prev_pass = get_env_variable("QLM_PASSWD")
     prev_configure = get_env_variable("QLM_CONFIGURED")
     if prev_configure == "":
         prev_configure = "False"
@@ -75,16 +75,16 @@
         raise QLMRemoteExecutionError(
             "Error when saving the account.\nTrace: " + str(err)
         )
     return True
 
 
 def setup_qlm_account() -> tuple[str, list[Any]]:
-    """Setup the QLM account, by looking at the existing configuration, asking
-    for the token and update the current account."""
+    """Setups the QLM account, by looking at the existing configuration, asking
+    for username/password and updating the current account."""
     already_configured = get_env_variable("QLM_CONFIGURED") == "True"
 
     if already_configured:
         decision = input(
             "An QLM account is already configured. Do you want to update it? [y/N] "
         )
         if decision.lower().strip() != "y":
@@ -106,24 +106,30 @@
     else:
         print(colored("Wrong credential", "red"))
         getpass("Press 'Enter' to continue")
         return "", []
 
 
 def get_all_job_ids() -> list[str]:
-    """Retrieve from the remote QLM all the job-ids associated with this account.
+    """Retrieves from the remote QLM all the job-ids associated with this account.
 
-    Examples:
+    Returns:
+        List of all job-ids associated with this account.
+
+    Example:
         >>> get_all_job_ids()
         ['Job144361', 'Job144360', 'Job144359', 'Job144358', 'Job144357', 'Job143334', 'Job143333', 'Job143332',
         'Job141862', 'Job141861', 'Job141722', 'Job141720', 'Job141716', 'Job141715', 'Job141712', 'Job19341']
+
     """
 
-    connection = get_QLMaaSConnection()
-    return [job_info.id for job_info in connection.get_jobs_info()]
+    if get_env_variable("QLM_CONFIGURED") == "True":
+        connection = get_QLMaaSConnection()
+        return [job_info.id for job_info in connection.get_jobs_info()]
+    return []
 
 
 def get_QLMaaSConnection():
     """Connects to the QLM and returns the QLMaaSConnection. If the connection
     was already established, we only return the one stored in global variable,
     otherwise we instantiate a new QLMaaSConnection."""
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/job.py` & `mpqp-0.2.0/mpqp/execution/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,45 @@
+"""
+When you call :func:`run<mpqp.execution.runner.run>` or
+:func:`submit<mpqp.execution.runner.submit>`, a :class:`Job` is created by 
+:func:`generate_job<mpqp.execution.runner.generate_job>`. This job contains all
+the needed information to configure the execution, and eventually retrieve
+remote results.
+
+A :class:`Job` can be of three types, given by the :class:`JobType` enum. In 
+addition, it has a status, given by the :class:`JobStatus` enum.
+
+As described above, a :class:`Job` is generated on circuit submission so you
+would in principle never need to instantiate one yourself.
+"""
+
 from __future__ import annotations
-from typing import Optional, TYPE_CHECKING
+
+from typing import TYPE_CHECKING, Optional
+
 from aenum import Enum, NoAlias
+from typeguard import typechecked
 
 # This is needed because for some reason pyright does not understand that Enum
 # is a class (probably because Enum does weird things to the Enum class)
-from typeguard import typechecked
-
 if TYPE_CHECKING:
     from enum import Enum
 
-from mpqp.core.instruction.measurement import Measure, ExpectationMeasure, BasisMeasure
-from .connection.ibm_connection import get_IBMProvider, get_QiskitRuntimeService
-from .connection.qlm_connection import get_QLMaaSConnection
-from ..core.circuit import QCircuit
-from .devices import AvailableDevice, IBMDevice, AWSDevice, ATOSDevice
-
-from qat.comm.qlmaas.ttypes import JobStatus as QLM_JobStatus, QLMServiceException
-from qiskit.providers import JobStatus as IBM_JobStatus
 from braket.aws import AwsQuantumTask
+from qat.comm.qlmaas.ttypes import JobStatus as QLM_JobStatus
+from qat.comm.qlmaas.ttypes import QLMServiceException
+from qiskit.providers import JobStatus as IBM_JobStatus
+
+from mpqp.core.instruction.measurement import BasisMeasure, ExpectationMeasure, Measure
 
+from ..core.circuit import QCircuit
 from ..tools.errors import IBMRemoteExecutionError, QLMRemoteExecutionError
+from .connection.ibm_connection import get_IBMProvider, get_QiskitRuntimeService
+from .connection.qlm_connection import get_QLMaaSConnection
+from .devices import ATOSDevice, AvailableDevice, AWSDevice, IBMDevice
 
 
 class JobStatus(Enum):
     """Possible states of a Job."""
 
     INIT = "initializing the job"
     """Initializing the job."""
@@ -36,43 +52,41 @@
     ERROR = "an error occurred with the job"
     """An error occurred with the job."""
     DONE = "the job is successfully done"
     """The job is successfully done."""
 
 
 class JobType(Enum):
-    """
-    Possible types of Job to execute.
+    """Possible types of Job to execute.
 
     Each type of job is restricted to some measures (and to some backends, but
     this is tackled by the backends themselves).
     """
 
     _settings_ = NoAlias
     STATE_VECTOR = {BasisMeasure, type(None)}
-    """Retrieve the vector representing the quantum state, this type is *ideal*."""
+    """Retrieves the vector representing the quantum state, this type is *ideal*."""
     SAMPLE = {BasisMeasure}
-    """Measure several times the quantum state in the basis, and retrieve the 
+    """Measures several times the quantum state in the basis, and retrieve the 
     counts. Contrarily to the ``STATE_VECTOR`` job type, this one is *realistic*."""
     OBSERVABLE = {ExpectationMeasure}
-    """Compute the *expectation value* of an observable, using the state_vector 
+    """Computes the *expectation value* of an observable, using the state_vector 
     or the samples. This type is ideal too: it requires some trickery to 
     retrieve the expectation value in an optimal manner."""
 
 
 @typechecked
 class Job:
-    """
-    Representation of a job, an object regrouping all the information about
+    """Representation of a job, an object regrouping all the information about
     the submission of a computation/measure of a quantum circuit on a
     specific hardware.
 
-    A job as a type, and a status, and is affected to a specific device.
+    A job has a type, and a status, and is attached to a specific device.
     Moreover, the job contains also the quantum circuit and the measure to be
-    computed on the circuit.
+    performed on the circuit.
 
     Args:
         job_type: Type of the job (sample, observable, ...).
         circuit: Circuit to execute.
         device: Device (simulator, quantum computer) on which we want to execute
             the job.
         measure: Object representing the measure to perform.
@@ -84,14 +98,15 @@
         >>> circuit.add(BasisMeasure([0, 1], shots=1000))
         >>> job2 = Job(
         ...     JobType.STATE_VECTOR,
         ...     circuit,
         ...     IBMDevice.AER_SIMULATOR,
         ...     circuit.get_measurements()[0],
         ... )
+
     """
 
     # 6M-TODO: decide, when there are several measurements, if we define a
     #  multi-measure job, or if we need several jobs. For the moment, a Job can
     #  handle only one measurement
 
     def __init__(
@@ -111,15 +126,15 @@
         """See parameter description."""
         self.measure = measure
         """See parameter description."""
 
         self.id: Optional[str] = None
         """Contains the id of the remote job, used to retrieve the result from 
         the remote provider.  ``None`` if the job is local. If the job is not 
-        local, it will be set latter on."""
+        local, it will be set later on."""
 
     @property
     def status(self):
         """Update and return the current job status. Mainly relevant for remote jobs."""
         if self._status not in [
             JobStatus.DONE,
             JobStatus.ERROR,
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/providers_execution/atos_execution.py` & `mpqp-0.2.0/mpqp/execution/providers/ibm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,517 +1,471 @@
-from typing import Optional
+from __future__ import annotations
 
-import numpy as np
+import math
+from typing import TYPE_CHECKING, Optional
+
+from qiskit import QuantumCircuit
+from qiskit.compiler import transpile
+from qiskit.primitives import BackendEstimator
+from qiskit.primitives import Estimator as Qiskit_Estimator
+from qiskit.primitives import EstimatorResult, SamplerResult
+from qiskit.providers import BackendV1, BackendV2
+from qiskit.providers import JobStatus as IBM_JobStatus
+from qiskit.quantum_info import Operator
+from qiskit.result import Result as QiskitResult
+from qiskit_aer import Aer, AerSimulator
+from qiskit_ibm_provider.job import IBMJob
+from qiskit_ibm_runtime import Estimator as Runtime_Estimator
+from qiskit_ibm_runtime import RuntimeJob
+from qiskit_ibm_runtime import Sampler as Runtime_Sampler
+from qiskit_ibm_runtime import Session
 from typeguard import typechecked
-from statistics import mean
 
-from mpqp.core.instruction.measurement import ComputationalBasis
-from mpqp.core.instruction.measurement.basis_measure import BasisMeasure
-from mpqp.core.instruction.measurement.expectation_value import (
-    ExpectationMeasure,
-    Observable,
+from mpqp.core.circuit import QCircuit
+from mpqp.core.instruction.measurement import BasisMeasure
+from mpqp.core.instruction.measurement.expectation_value import ExpectationMeasure
+from mpqp.core.languages import Language
+from mpqp.execution.connection.ibm_connection import (
+    get_IBMProvider,
+    get_QiskitRuntimeService,
 )
-from mpqp.execution.devices import ATOSDevice
-from ..connection.qlm_connection import get_QLMaaSConnection
-from ..job import Job, JobType, JobStatus
-from ..result import Result, Sample, StateVector
-from mpqp.qasm import qasm2_to_myqlm_Circuit
-from mpqp import QCircuit, Language
-from ...tools.errors import QLMRemoteExecutionError
-
-from qat.qlmaas.result import AsyncResult
-from qat.core.contexts import QPUContext
-from qat.pylinalg import PyLinalg
-from qat.clinalg.qpu import CLinalg
-from qat.core.wrappers.observable import Observable as QLM_Observable
-from qat.plugins.observable_splitter import ObservableSplitter
-from qat.core.wrappers.result import Result as QLM_Result
-from qat.core.wrappers.circuit import Circuit
-from qat.core.wrappers.job import Job as JobQLM
-from qat.comm.qlmaas.ttypes import JobStatus as QLM_JobStatus, QLMServiceException
+from mpqp.execution.devices import IBMDevice
+from mpqp.execution.job import Job, JobStatus, JobType
+from mpqp.execution.result import Result, Sample, StateVector
+from mpqp.tools.errors import DeviceJobIncompatibleError, IBMRemoteExecutionError
 
 
 @typechecked
-def get_local_qpu(device: ATOSDevice):
-    if device.is_remote():
-        raise ValueError("Excepted a local device, not the remote QLM")
-    if device == ATOSDevice.MYQLM_PYLINALG:
-        return PyLinalg()
-    return CLinalg()
-
+def run_ibm(job: Job) -> Result:
+    """Executes the job on the right IBM Q device precised in the job in
+    parameter.
 
-@typechecked
-def generate_state_vector_job(
-    myqlm_circuit: Circuit, device: ATOSDevice = ATOSDevice.MYQLM_PYLINALG
-) -> tuple[JobQLM, QPUContext]:
-    """Generate a myQLM job from the myQLM circuit and select the right myQLM
-    QPU to run on it.
+    Note:
+        This function is not meant to be used directly, please use
+        ``runner.run(...)`` instead.
 
     Args:
-        myqlm_circuit: MyQLM circuit of the job.
-        device: ATOSDevice on which the user wants to run the job (to know if
-            the run in local of remote).
-
-    Returns:
-        A myQLM Job and the right myQLM QPUHandler on which it will be submitted.
-    """
-
-    if device.is_remote():
-        get_QLMaaSConnection()
-        from qlmaas.qpus import LinAlg  # type: ignore
-
-        qpu = LinAlg()
-    else:
-        qpu = get_local_qpu(device)
-
-    return myqlm_circuit.to_job(job_type="SAMPLE"), qpu
-
-
-@typechecked
-def generate_sample_job(myqlm_circuit: Circuit, job: Job) -> tuple[JobQLM, QPUContext]:
-    """Generate a myQLM job from the myQLM circuit and job sample info (target,
-    shots, ...), and select the right myQLM QPU to run on it.
-
-    Args:
-        myqlm_circuit: MyQLM circuit of the job.
-        job: Original mpqp job used to generate the myQLM job.
-
-    Returns:
-        A myQLM Job and the right myQLM QPUHandler on which it will be submitted.
-    """
-
-    assert job.measure is not None
-
-    myqlm_job = myqlm_circuit.to_job(
-        job_type="SAMPLE",
-        qubits=job.measure.targets,
-        nbshots=job.measure.shots,
-    )
-
-    if job.device.is_remote():
-        get_QLMaaSConnection()
-        from qlmaas.qpus import LinAlg  # type: ignore
-
-        qpu = LinAlg()
-    else:
-        assert isinstance(job.device, ATOSDevice)
-        qpu = get_local_qpu(job.device)
-
-    return myqlm_job, qpu
-
-
-@typechecked
-def generate_observable_job(
-    myqlm_circuit: Circuit, job: Job
-) -> tuple[JobQLM, QPUContext]:
-    """Generate a myQLM job from the myQLM circuit and observable, and select
-    the right myQLM QPU to run on it.
-
-    Args:
-        myqlm_circuit: MyQLM circuit of the job.
-        job: Original mpqp job used to generate the myQLM job.
+        job: Job to be executed.
 
     Returns:
-        A myQLM Job and the right myQLM QPUHandler on which it will be submitted.
+        The result of the job.
     """
-
-    assert job.measure is not None and isinstance(job.measure, ExpectationMeasure)
-
-    myqlm_job = myqlm_circuit.to_job(
-        job_type="OBS",
-        observable=QLM_Observable(
-            job.measure.nb_qubits, matrix=job.measure.observable.matrix
-        ),
-        nbshots=job.measure.shots,
-    )
-    if job.device.is_remote():
-        get_QLMaaSConnection()
-        from qlmaas.qpus import LinAlg  # type: ignore
-
-        qpu = LinAlg()
-    else:
-        assert isinstance(job.device, ATOSDevice)
-        qpu = ObservableSplitter() | get_local_qpu(job.device)
-
-    return myqlm_job, qpu
+    return run_aer(job) if not job.device.is_remote() else run_ibmq(job)
 
 
 @typechecked
-def extract_state_vector_result(
-    myqlm_result: QLM_Result,
-    job: Optional[Job] = None,
-    device: ATOSDevice = ATOSDevice.MYQLM_PYLINALG,
+def compute_expectation_value(
+    ibm_circuit: QuantumCircuit, ibm_backend: Optional[BackendV1 | BackendV2], job: Job
 ) -> Result:
-    """Construct a Result from the result given by the myQLM/QLM run in state
-    vector mode.
+    """Configures observable job and run it locally, and returns the
+    corresponding Result.
+
+    Note:
+        This function is not meant to be used directly, please use
+        ``runner.run(...)`` instead.
 
     Args:
-        myqlm_result: Result return by myQLM/QLM after run of the job.
-        job: Original mpqp job used to generate the run. Used to retrieve more
-            easily info to instantiate the result.
-        device: ATOSDevice on which the job was submitted. Used to know if the
-            run was remote or local.
+        ibm_circuit: QuantumCircuit (already reversed bits)
+        ibm_backend: The IBM backend (local of remote) on which we execute the job.
+        job: Mpqp job describing the observable job to run.
 
     Returns:
-        A Result containing the result info extract from the myQLM/QLM
-        statevector result.
+        The result of the job.
     """
-    if job is None:
-        nb_qubits = (
-            myqlm_result.qregs[0].length
-            if device.is_remote()
-            else sum(len(qreg.qbits) for qreg in myqlm_result.data.qregs)
+    if not isinstance(job.measure, ExpectationMeasure):
+        raise ValueError(
+            "Cannot compute expectation value if measure used in job is not of "
+            "type ExpectationMeasure"
         )
-        job = Job(JobType.STATE_VECTOR, QCircuit(nb_qubits), device, None)
+    nb_shots = job.measure.shots
+    qiskit_observable = job.measure.observable.to_other_language(Language.QISKIT)
+    assert isinstance(qiskit_observable, Operator)
+
+    if nb_shots != 0:
+        assert ibm_backend is not None
+        estimator = BackendEstimator(backend=ibm_backend)
     else:
-        nb_qubits = job.circuit.nb_qubits
+        estimator = Qiskit_Estimator()
 
-    nb_states = 2**nb_qubits
-    amplitudes = np.zeros(nb_states, np.complex64)
-    probas = np.zeros(nb_states, np.float32)
-    for sample in myqlm_result:
-        amplitudes[sample._state] = sample.amplitude
-        probas[sample._state] = sample.probability
+    # 6M-TODO : think of the possibility to compute several expectation values at the same time when the circuit is
+    #  the same apparently the estimator.run() can take several circuits and observables at the same time,
+    #  to verify if putting them all together increases the performance
 
-    return Result(job, StateVector(amplitudes, nb_qubits, probas), 0, 0)
+    job.status = JobStatus.RUNNING
+    job_expectation = estimator.run(
+        [ibm_circuit], [qiskit_observable], shots=nb_shots if nb_shots != 0 else None
+    )
+    estimator_result = job_expectation.result()
+    assert isinstance(job.device, IBMDevice)
+    return extract_result(estimator_result, job, job.device)
 
 
 @typechecked
-def extract_sample_result(
-    myqlm_result: QLM_Result,
-    job: Optional[Job] = None,
-    device: ATOSDevice = ATOSDevice.MYQLM_PYLINALG,
-) -> Result:
-    """Construct a Result from the result given by the myQLM/QLM run in sample
-    mode.
+def check_job_compatibility(job: Job):
+    """Checks whether the job in parameter has coherent and compatible
+    attributes.
 
     Args:
-        myqlm_result: Result return by myQLM/QLM after run of the job.
-        job: Original mpqp job used to generate the run. Used to retrieve more
-            easily info to instantiate the result.
-        device: ATOSDevice on which the job was submitted. Used to know if the
-            run was remote or local.
+        job: Job for which we want to check compatibility.
 
-    Returns:
-        A Result containing the result info extract from the myQLM/QLM sample
-        result.
-    """
-    if job is None:
-        assert isinstance(myqlm_result.qregs[0].length, int)
-        nb_qubits = (
-            myqlm_result.qregs[0].length
-            if device.is_remote()
-            else sum(len(qreg.qbits) for qreg in myqlm_result.raw_data.qregs)
-        )
-        nb_shots = int(myqlm_result.meta_data["nbshots"])
-        job = Job(
-            JobType.SAMPLE,
-            QCircuit(nb_qubits),
-            device,
-            BasisMeasure(targets=list(range(nb_qubits)), shots=nb_shots),
+    Raises:
+        DeviceJobIncompatibleError: If there is a mismatch between information
+            contained in the job (measure and job_type, device and job_type,
+            etc...).
+    """
+    if not type(job.measure) in job.job_type.value:
+        raise DeviceJobIncompatibleError(
+            f"An {job.job_type.name} job is valid only if the corresponding circuit has an measure in "
+            f"{list(map(lambda cls: cls.__name__, job.job_type.value))}. "
+            f"{type(job.measure).__name__} was given instead."
         )
-    else:
-        nb_qubits = job.circuit.nb_qubits
-        if job.measure is None:
-            raise NotImplementedError("We cannot handle job without measure for now")
-        nb_shots = job.measure.shots
-
-    # we here take the average of errors over all samples
-    error = mean([sample.err for sample in myqlm_result])
-    samples = [
-        Sample(
-            nb_qubits,
-            index=sample._state,
-            probability=sample.probability,
-            bin_str=str(sample.state)[1:-1],
+    if (
+        job.job_type == JobType.STATE_VECTOR
+        and job.device != IBMDevice.AER_SIMULATOR_STATEVECTOR
+    ):
+        raise DeviceJobIncompatibleError(
+            "Cannot reconstruct state vector with this device. Please use "
+            f"{IBMDevice.AER_SIMULATOR_STATEVECTOR} instead (or change the job "
+            "type, by for example giving a number of shots to the measure)."
         )
-        for sample in myqlm_result
-    ]
-
-    return Result(job, samples, error, nb_shots)
+    if job.device == IBMDevice.AER_SIMULATOR_STATEVECTOR:
+        if job.job_type == JobType.SAMPLE:
+            raise DeviceJobIncompatibleError(
+                "Cannot use sample mode with the statevector simulator."
+            )
+        if job.job_type == JobType.OBSERVABLE:
+            assert job.measure is not None
+            if job.measure.shots > 0:
+                raise DeviceJobIncompatibleError(
+                    "Cannot compute expectation values with non-zero shots"
+                    f" with {IBMDevice.AER_SIMULATOR_STATEVECTOR}.\nSet the"
+                    " shots to zero to get the exact value, or select "
+                    "another device instead"
+                )
 
 
 @typechecked
-def extract_observable_result(
-    myqlm_result: QLM_Result,
-    job: Optional[Job] = None,
-    device: ATOSDevice = ATOSDevice.MYQLM_PYLINALG,
-) -> Result:
-    """Construct a Result from the result given by the myQLM/QLM run in
-    observable mode.
+def run_aer(job: Job):
+    """Executes the job on the right AER local simulator precised in the job in
+    parameter.
+
+    Note:
+        This function is not meant to be used directly, please use
+        ``runner.run(...)`` instead.
 
     Args:
-        myqlm_result: Result return by myQLM/QLM after run of the job.
-        job: Original mpqp job used to generate the run. Used to retrieve more
-            easily info to instantiate the result.
-        device: ATOSDevice on which the job was submitted. Used to know if the
-            run was remote or local.
+        job: Job to be executed.
 
     Returns:
-        A Result containing the result info extract from the myQLM/QLM
-        observable result.
+        the result of the job.
     """
-    if job is None:
-        if device.is_remote():
-            nb_qubits = myqlm_result.data.qregs[0].length
-        else:
-            nb_qubits = sum(len(qreg.qbits) for qreg in myqlm_result.data.qregs)
-        nb_shots = int(myqlm_result.meta_data["nbshots"])
-        job = Job(
-            JobType.OBSERVABLE,
-            QCircuit(nb_qubits),
-            device,
-            ExpectationMeasure(
-                targets=list(range(nb_qubits)),
-                observable=Observable(
-                    np.zeros((2**nb_qubits, 2**nb_qubits), dtype=np.complex64)
-                ),
-                shots=nb_shots,
-            ),
-        )
-    else:
-        if job.measure is None:
-            raise NotImplementedError("We cannot handle job without measure for now")
-        nb_shots = job.measure.shots
-
-    return Result(job, myqlm_result.value, myqlm_result.error, nb_shots)
-
-
-@typechecked
-def extract_result(
-    myqlm_result: QLM_Result,
-    job: Optional[Job] = None,
-    device: ATOSDevice = ATOSDevice.MYQLM_PYLINALG,
-) -> Result:
-    """
-    Construct a Result from the result given by the myQLM/QLM run.
+    qiskit_circuit = (
+        job.circuit.without_measurements().to_other_language(Language.QISKIT)
+        if (job.job_type == JobType.STATE_VECTOR)
+        else job.circuit.to_other_language(Language.QISKIT)
+    )
+    if TYPE_CHECKING:
+        assert isinstance(qiskit_circuit, QuantumCircuit)
 
-    Args:
-        myqlm_result: Result returned by myQLM/QLM after run of the job.
-        job: Original mpqp job used to generate the run. Used to retrieve more
-            easily info to instantiate the result.
-        device: ATOSDevice on which the job was submitted. Used to know if the
-            run was remote or local.
+    qiskit_circuit = qiskit_circuit.reverse_bits()
+    check_job_compatibility(job)
 
-    Returns:
-        A Result containing the result info extract from the myQLM/QLM result.
-    """
+    # define backend simulator
+    if job.device == IBMDevice.AER_SIMULATOR:
+        backend_sim = AerSimulator()
+        if job.job_type == JobType.SAMPLE:
+            assert job.measure is not None
+            run_input = transpile(qiskit_circuit, backend_sim)
+            job.status = JobStatus.RUNNING
+            job_sim = backend_sim.run(run_input, shots=job.measure.shots)
+            result_sim = job_sim.result()
+            result = extract_result(result_sim, job, IBMDevice.AER_SIMULATOR)
+        elif job.job_type == JobType.OBSERVABLE:
+            result = compute_expectation_value(qiskit_circuit, backend_sim, job)
+        else:
+            raise ValueError(f"Job type {job.job_type} not handled on {job.device}")
 
-    if (job is None) or job.device.is_remote():
-        if myqlm_result.value is None:
-            if list(myqlm_result)[0].amplitude is None:
-                job_type = JobType.SAMPLE
-            else:
-                job_type = JobType.STATE_VECTOR
+    elif job.device == IBMDevice.AER_SIMULATOR_STATEVECTOR:
+        if job.job_type == JobType.STATE_VECTOR:
+            backend_sim = Aer.get_backend(job.device.value)
+            # the save_statevector method is patched on qiskit_aer load, meaning
+            # the type checker can't find it. I hate it but it is what it is.
+            # this explains the `type: ignore`. This method is needed to get a
+            # statevector our of the statevector simulator...
+            qiskit_circuit.save_statevector()  # type: ignore
+            job.status = JobStatus.RUNNING
+            job_sim = backend_sim.run(qiskit_circuit, shots=0)
+            result_sim = job_sim.result()
+            result = extract_result(
+                result_sim, job, IBMDevice.AER_SIMULATOR_STATEVECTOR
+            )
+        elif job.job_type == JobType.OBSERVABLE:
+            result = compute_expectation_value(qiskit_circuit, None, job)
         else:
-            job_type = JobType.OBSERVABLE
-    else:
-        job_type = job.job_type
+            raise ValueError(f"job type {job.job_type} not handled on {job.device}")
 
-    if job_type == JobType.STATE_VECTOR:
-        return extract_state_vector_result(myqlm_result, job, device)
-    elif job_type == JobType.SAMPLE:
-        return extract_sample_result(myqlm_result, job, device)
     else:
-        return extract_observable_result(myqlm_result, job, device)
+        raise ValueError(f"job device {job.device} not handled yet")
 
-
-@typechecked
-def job_pre_processing(job: Job) -> Circuit:
-    """Extract the myQLM circuit and check if ``job.type`` and ``job.measure``
-    are coherent.
-
-    Args:
-        job: Mpqp job used to instantiate the myQLM circuit.
-    """
-
-    if (
-        job.job_type == JobType.STATE_VECTOR
-        and job.measure is not None
-        and not isinstance(job.measure, BasisMeasure)
-    ):
-        raise ValueError("`STATE_VECTOR` jobs require basis measure to be run")
-    if job.job_type == JobType.OBSERVABLE and not isinstance(
-        job.measure, ExpectationMeasure
-    ):
-        raise ValueError("`OBSERVABLE` jobs require `ExpectationMeasure` to be run")
-
-    myqlm_circuit = job.circuit.to_other_language(Language.MY_QLM)
-
-    return myqlm_circuit
+    job.status = JobStatus.DONE
+    return result
 
 
 @typechecked
-def run_atos(job: Job) -> Result:
-    """Execute the job on the right ATOS device precised in the job in parameter.
-    This function is not meant to be used directly, please use
-    ``runner.run(...)`` instead.
-
-    Args:
-        job: Job to be executed.
-
-    Returns:
-        A Result after submission and execution of the job.
-    """
-    return run_myQLM(job) if not job.device.is_remote() else run_QLM(job)
+def submit_ibmq(job: Job) -> tuple[str, RuntimeJob | IBMJob]:
+    """Submits the job on the remote IBM device (quantum computer or simulator).
 
-
-@typechecked
-def run_myQLM(job: Job) -> Result:
-    """Execute the job on the local myQLM simulator. This function is not meant
-    to be used directly, please use ``runner.run(...)`` instead.
+    Note:
+        This function is not meant to be used directly, please use
+        ``runner.submit(...)`` instead.
 
     Args:
         job: Job to be executed.
 
     Returns:
-        A Result after submission and execution of the job.
+        IBM's job id and the ``qiskit`` job itself.
     """
-
-    result = None
-    myqlm_job = None
-    myqlm_result = None
-    qpu = None
-
-    myqlm_circuit = job_pre_processing(job)
-
     if job.job_type == JobType.STATE_VECTOR:
-        myqlm_job, qpu = generate_state_vector_job(myqlm_circuit)
+        raise DeviceJobIncompatibleError(
+            "State vector cannot be computed using IBM remote simulators and"
+            " devices. Please use a local simulator instead."
+        )
 
-    elif job.job_type == JobType.SAMPLE:
-        assert isinstance(job.measure, BasisMeasure)
-        if isinstance(job.measure.basis, ComputationalBasis):
-            myqlm_job, qpu = generate_sample_job(myqlm_circuit, job)
-        else:
-            raise NotImplementedError(
-                "Does not handle other basis than the ComputationalBasis for the moment"
+    if job.job_type == JobType.OBSERVABLE:
+        if not isinstance(job.measure, ExpectationMeasure):
+            raise ValueError(
+                "An observable job must is valid only if the corresponding "
+                "circuit has an expectation measure."
+            )
+        if job.measure.shots == 0:
+            raise DeviceJobIncompatibleError(
+                "Expectation values cannot be computed exactly using IBM remote"
+                " simulators and devices. Please use a local simulator instead."
             )
+    check_job_compatibility(job)
 
-    elif job.job_type == JobType.OBSERVABLE:
+    qiskit_circuit = job.circuit.to_other_language(Language.QISKIT)
+    if TYPE_CHECKING:
+        assert isinstance(qiskit_circuit, QuantumCircuit)
+    qiskit_circuit = qiskit_circuit.reverse_bits()
+
+    service = get_QiskitRuntimeService()
+    backend_str = job.device.value
+    session = Session(service=service, backend=backend_str)
+    if job.job_type == JobType.OBSERVABLE:
         assert isinstance(job.measure, ExpectationMeasure)
-        myqlm_job, qpu = generate_observable_job(myqlm_circuit, job)
+        estimator = Runtime_Estimator(session=session)
+        qiskit_observable = job.measure.observable.to_other_language(Language.QISKIT)
+        assert isinstance(qiskit_observable, Operator)
 
+        ibm_job = estimator.run(
+            qiskit_circuit, qiskit_observable, shots=job.measure.shots
+        )
+    elif job.job_type == JobType.SAMPLE:
+        assert job.measure is not None
+        sampler = Runtime_Sampler(session=session)
+        ibm_job = sampler.run(qiskit_circuit, shots=job.measure.shots)
     else:
-        raise ValueError(f"Job type {job.job_type} not handled")
+        raise NotImplementedError(f"{job.job_type} not handled.")
 
-    job.status = JobStatus.RUNNING
-    myqlm_result = qpu.submit(myqlm_job)
+    job.id = ibm_job.job_id()
 
-    # retrieving the results
-    result = extract_result(myqlm_result, job, job.device)  # type: ignore
-
-    job.status = JobStatus.DONE
-    return result
+    return job.id, ibm_job
 
 
 @typechecked
-def submit_QLM(job: Job) -> tuple[str, AsyncResult]:
-    """Submit the job on the remote QLM machine. This function is not meant to
-    be used directly, please use ``runner.submit(...)`` instead.
+def run_ibmq(job: Job) -> Result:
+    """Submits the job on the right IBMQ remote device, precised in the job in
+    parameter, and waits until the job is completed.
+
+    Note:
+        This function is not meant to be used directly, please use
+        ``runner.run(...)`` instead.
 
     Args:
         job: Job to be executed.
 
     Returns:
-        The job_id and the AsyncResult of the submitted job.
+        A Result after submission and execution of the job.
     """
+    _, remote_job = submit_ibmq(job)
+    ibm_result = remote_job.result()
 
-    myqlm_job = None
-    qpu = None
-
-    myqlm_circuit = job_pre_processing(job)
-
-    if job.device == ATOSDevice.QLM_LINALG:
-        if job.job_type == JobType.STATE_VECTOR:
-            assert isinstance(job.device, ATOSDevice)
-            myqlm_job, qpu = generate_state_vector_job(myqlm_circuit, job.device)
-
-        elif job.job_type == JobType.SAMPLE:
-            assert isinstance(job.measure, BasisMeasure)
-            if isinstance(job.measure.basis, ComputationalBasis):
-                myqlm_job, qpu = generate_sample_job(myqlm_circuit, job)
-            else:
-                raise NotImplementedError(
-                    "Does not handle other basis than the ComputationalBasis for the moment"
-                )
-
-        elif job.job_type == JobType.OBSERVABLE:
-            assert isinstance(job.measure, ExpectationMeasure)
-            myqlm_job, qpu = generate_observable_job(myqlm_circuit, job)
-
-        else:
-            raise ValueError(f"Job type {job.job_type} not handled")
-
-        job.status = JobStatus.RUNNING
-        async_result = qpu.submit(myqlm_job)
-        job_id = async_result.get_info().id
-        job.id = job_id
-    else:
-        raise NotImplementedError(f"Device {job.device} not handled")
-
-    return job_id, async_result
+    assert isinstance(job.device, IBMDevice)
+    return extract_result(ibm_result, job, job.device, remote_job)
 
 
 @typechecked
-def run_QLM(job: Job) -> Result:
-    """Submit the job on the remote QLM machine and wait for it to be done. This
-    function is not meant to be used directly, please use ``runner.run(...)``
-    instead.
+def extract_result(
+    result: QiskitResult | EstimatorResult | SamplerResult,
+    job: Optional[Job] = None,
+    device: IBMDevice = IBMDevice.AER_SIMULATOR,
+    ibm_job: Optional[IBMJob | RuntimeJob] = None,
+) -> Result:
+    """Parses a result from ``IBM`` execution (remote or local) in a ``MPQP``
+    :class:`Result<mpqp.execution.result.Result>`.
 
     Args:
-        job: Job to be executed.
+        result: Result returned by IBM after running of the job.
+        job: ``MPQP`` job used to generate the run. Enables a more complete
+            result.
+        device: IBMDevice on which the job was submitted. Used to know if the
+            run was remote or local
+        ibm_job: IBM or Runtime job used to retrieve info about the circuit and
+            the submitted job (in the remote case).
 
     Returns:
-        A Result after submission and execution of the job.
+        The ``qiskit`` result converted to our format.
     """
 
-    if not isinstance(job.device, ATOSDevice) or not job.device.is_remote():
+    if job is not None and (
+        isinstance(result, EstimatorResult) != (job.job_type == JobType.OBSERVABLE)
+    ):
         raise ValueError(
-            "The job given is not a QLM one, so it cannot be handled by this "
-            "function."
+            "Mismatch between job type and result type: either the result is an"
+            " `EstimatorResult` and the job is od type of both those assertions"
+            " are false."
         )
 
-    _, async_result = submit_QLM(job)
-    qlm_result = async_result.join()
+    if isinstance(result, EstimatorResult):
+        if job is None:
+            job = Job(JobType.OBSERVABLE, QCircuit(0), device)
+        shots = 0 if len(result.metadata[0]) == 0 else result.metadata[0]["shots"]
+        variance = (
+            None if len(result.metadata[0]) == 0 else result.metadata[0]["variance"]
+        )
+        return Result(job, result.values[0], variance, shots)
 
-    return extract_result(qlm_result, job, job.device)
+    elif isinstance(result, SamplerResult):
+        shots = result.metadata[0]["shots"]
+        probas = result.quasi_dists[0]
+        if job is None:
+            if ibm_job is None:
+                #  If we don't have access to the remote Sampler RuntimeJob, we determine the number of qubits by taking
+                #  the max index in the counts and take the upper power of two. Of course this is not a clean way and
+                #  can lead to a lower number of qubit than the real one. We asked IBM support, apparently there is no
+                #  way to retrieve the right nb_qubits with SamplerResult only. That is why we encourage to input the
+                #  ibm_job to this function
+                max_index = max(list(probas.keys()))
+                nb_qubits = math.ceil(math.log2(max_index + 1))
+            else:
+                if isinstance(ibm_job, RuntimeJob):
+                    nb_qubits = len(ibm_job.inputs["circuits"][0].qubits)
+                else:
+                    raise ValueError(
+                        f"Expected a RuntimeJob as optional parameter but got an {type(ibm_job)} instead"
+                    )
+            job = Job(
+                JobType.SAMPLE,
+                QCircuit(nb_qubits),
+                device,
+                BasisMeasure(list(range(nb_qubits)), shots=shots),
+            )
+
+        data = [
+            Sample(
+                index=item, probability=probas[item], nb_qubits=job.circuit.nb_qubits
+            )
+            for item in probas
+        ]
+        return Result(job, data, None, shots)
+
+    elif isinstance(
+        result, QiskitResult
+    ):  # pyright: ignore[reportUnnecessaryIsInstance]
+        if job is None:
+            job_data = result.data()
+            if "statevector" in job_data:
+                job_type = JobType.STATE_VECTOR
+                nb_qubits = int(math.log(len(result.get_statevector()), 2))
+                job = Job(job_type, QCircuit(nb_qubits), device)
+            elif "counts" in job_data:
+                job_type = JobType.SAMPLE
+                nb_qubits = len(list(result.get_counts())[0])
+                shots = result.results[0].shots
+                job = Job(
+                    job_type,
+                    QCircuit(nb_qubits),
+                    device,
+                    BasisMeasure(list(range(nb_qubits)), shots=shots),
+                )
+            else:
+                if len(result.data()) == 0:
+                    raise ValueError(
+                        "Result data is empty, cannot extract anything. Check "
+                        "if the associated job was successfully completed."
+                    )
+                else:
+                    raise ValueError(
+                        f"Data with keys {result.data().keys()} in result not handled."
+                    )
+
+        if job.job_type == JobType.STATE_VECTOR:
+            vector = result.get_statevector()
+            state_vector = StateVector(
+                vector.data,  # pyright: ignore[reportArgumentType]
+                job.circuit.nb_qubits,
+            )
+            return Result(job, state_vector, 0, 0)
+        elif job.job_type == JobType.SAMPLE:
+            assert job.measure is not None
+            counts = result.get_counts()
+            data = [
+                Sample(
+                    bin_str=item, count=counts[item], nb_qubits=job.circuit.nb_qubits
+                )
+                for item in counts
+            ]
+            return Result(job, data, None, job.measure.shots)
+        else:
+            raise NotImplementedError(f"{job.job_type} not handled.")
+
+    else:
+        raise NotImplementedError(f"Result type {type(result)} not handled")
 
 
 @typechecked
-def get_result_from_qlm_job_id(job_id: str) -> Result:
-    """Retrieve the result, described by the job_id in parameter, from the
-    remote QLM and convert it into an mpqp result. If the job is still running,
-    we wait (blocking) until it is DONE.
+def get_result_from_ibm_job_id(job_id: str) -> Result:
+    """Retrieves from IBM remote platform and parse the result of the job_id
+    given in parameter. If the job is still running, we wait (blocking) until it
+    is ``DONE``.
 
     Args:
-        job_id: Id of the remote QLM job.
-
-    Raises:
-        QLMRemoteExecutionError
+        job_id: Id of the remote IBM job.
 
+    Returns:
+        The result converted to our format.
     """
-    connection = get_QLMaaSConnection()
-
-    try:
-        qlm_job = connection.get_job(job_id)
-    except QLMServiceException as e:
-        raise QLMRemoteExecutionError(
-            f"Job with id {job_id} not found.\nTrace: " + str(e)
+    # search for job id in the connector given in parameter first
+    # if not found, try with IBMProvider, then QiskitRuntimeService
+    # if not found, raise an error
+    connector = get_IBMProvider()
+    ibm_job = (
+        connector.retrieve_job(job_id)
+        if job_id in [job.job_id() for job in connector.jobs()]
+        else None
+    )
+    if ibm_job is None:
+        connector = get_QiskitRuntimeService()
+        ibm_job = (
+            connector.job(job_id)
+            if job_id in [job.job_id() for job in connector.jobs()]
+            else None
+        )
+    if ibm_job is None:
+        raise IBMRemoteExecutionError(
+            f"Job with id {job_id} was not found on this account."
         )
 
-    status = qlm_job.get_status()
-    if status in [
-        QLM_JobStatus.CANCELLED,
-        QLM_JobStatus.UNKNOWN_JOB,
-        QLM_JobStatus.DELETED,
-        QLM_JobStatus.FAILED,
-        QLM_JobStatus.STOPPED,
-    ]:
-        raise QLMRemoteExecutionError(
-            f"Trying to retrieve a QLM result for a job in status {status.name}"
+    status = ibm_job.status()
+    if status in [IBM_JobStatus.CANCELLED, IBM_JobStatus.ERROR]:
+        raise IBMRemoteExecutionError(
+            f"Trying to retrieve an IBM result for a job in status {status.name}"
         )
-    elif status in [QLM_JobStatus.WAITING, QLM_JobStatus.RUNNING]:
-        qlm_job.join()
 
-    qlm_result: QLM_Result = qlm_job.get_result()
+    # If the job is finished, it will get the result, if still running it is block until it finishes
+    result = ibm_job.result()
+    backend = ibm_job.backend()
+    assert isinstance(backend, (BackendV1, BackendV2))
+    ibm_device = IBMDevice(backend.name)
 
-    return extract_result(qlm_result, None, ATOSDevice.QLM_LINALG)
+    return extract_result(result, None, ibm_device, ibm_job)
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/remote_handler.py` & `mpqp-0.2.0/mpqp/execution/remote_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,126 @@
 """After the jobs are submitted, one can use the functions of this module to
 retrieve the results from a job_id or the job directly, and list all job
 attached to the configured accounts."""
 
 from __future__ import annotations
 
+from typing import Optional
+
 from typeguard import typechecked
 
 from mpqp.execution import Result
-from mpqp.execution.connection.aws_connection import get_all_task_ids
-from mpqp.execution.connection.qlm_connection import get_all_job_ids as qlm_ids
+from mpqp.execution.connection.aws_connection import get_all_task_ids as aws_ids
 from mpqp.execution.connection.ibm_connection import get_all_job_ids as ibm_ids
-from mpqp.execution.providers_execution.atos_execution import get_result_from_qlm_job_id
-from mpqp.execution.providers_execution.aws_execution import (
-    get_result_from_aws_task_arn,
+from mpqp.execution.connection.qlm_connection import get_all_job_ids as qlm_ids
+from mpqp.execution.connection.google_connection import get_all_job_ids as cirq_ids
+from mpqp.execution.devices import (
+    ATOSDevice,
+    AvailableDevice,
+    AWSDevice,
+    IBMDevice,
+    GOOGLEDevice,
 )
-from mpqp.execution.providers_execution.ibm_execution import get_result_from_ibm_job_id
-
-from mpqp.execution.devices import IBMDevice, AWSDevice, ATOSDevice, AvailableDevice
 from mpqp.execution.job import Job
+from mpqp.execution.providers.atos import get_result_from_qlm_job_id
+from mpqp.execution.providers.aws import get_result_from_aws_task_arn
+from mpqp.execution.providers.ibm import get_result_from_ibm_job_id
 
 
 @typechecked
-def remote_result_from_id(job_id: str, device: AvailableDevice) -> Result:
-    """
-    Retrieve and parse a remote the result from a job_id and device. If the job is still running, it will wait until it
-    is done.
+def get_remote_result(
+    job_data: str | Job, device: Optional[AvailableDevice] = None
+) -> Result:
+    """Retrieve and parse a remote the result from a job_id and device. If the
+    job is still running, it will wait until it is done.
+
+    Args:
+        job_data: Either the :class:`Job<mpqp.execution.job.Job>` object or the
+            job id used to identify the job on the remote device.
+        device: Remote device on which the job was launched, needed only if
+            ``job_data`` is the identifier of the job.
+
+    Returns:
+        The ``Result`` of the desired remote job.
 
     Examples:
-        >>> print(remote_result_from_id('Job141933', ATOSDevice.QLM_LINALG))
+        >>> print(get_remote_result('Job141933', ATOSDevice.QLM_LINALG))
         Result: ATOSDevice, QLM_LINALG
-        Counts: [1017, 0, 0, 0, 983, 0, 0, 0]
-        Probabilities: [0.5085 0.     0.     0.     0.4915 0.     0.     0.    ]
-        State: 000, Index: 0, Count: 1017, Probability: 0.5085
-        State: 100, Index: 4, Count: 983, Probability: 0.4915
-        Error: 0.011181519941139355
-        >>> print(remote_result_from_id(
+         Counts: [1017, 0, 0, 0, 983, 0, 0, 0]
+         Probabilities: [0.5085 0.     0.     0.     0.4915 0.     0.     0.    ]
+          State: 000, Index: 0, Count: 1017, Probability: 0.5085
+          State: 100, Index: 4, Count: 983, Probability: 0.4915
+         Error: 0.011181519941139355
+        >>> print(get_remote_result(
         ...     'cm80pb1054sir2ck9i3g',
         ...     IBMDevice.IBMQ_QASM_SIMULATOR,
         ... ))
         Result: IBMDevice, IBMQ_QASM_SIMULATOR
-        Expectation value: 1.6410799999999999
-        Error/Variance: 1.24570724535
+         Expectation value: 1.6410799999999999
+         Error/Variance: 1.24570724535
         >>> aws_task_id = (
         ...     'arn:aws:braket:us-east-1:752542621531:quantum-task/'
         ...     '6a46ae9a-d02f-4a23-b46f-eae43471bc22'
         ... )
-        >>> print(remote_result_from_id(
+        >>> print(get_remote_result(
         ...     aws_task_id,
         ...     AWSDevice.BRAKET_SV1_SIMULATOR,
         ... ))
         Result: AWSDevice, BRAKET_SV1_SIMULATOR
-        Expectation value: 1.6635202030411578
-        Error/Variance: None
+         Expectation value: 1.6635202030411578
+         Error/Variance: None
 
-    Args:
-        job_id: Id used to identify the job on the remote device.
-        device: Remote device on which the job was launched.
+        >>> circ = QCircuit([H(0), CNOT(0,1)])
+        >>> _, job = submit(circ, ATOSDevice.QLM_LINALG)
+        >>> print(get_remote_result(job))
+        Result: ATOSDevice, QLM_LINALG
+         State vector: [0.7071068, 0, 0, 0.7071068]
+         Probabilities: [0.5, 0, 0, 0.5]
+         Number of qubits: 2
 
-    Returns:
-        A Result of the remote job identified by the job_id in parameter.
     """
+    if isinstance(job_data, Job):
+        if job_data.id is None:
+            raise ValueError("Can't retrieve remote result for a job whose id is None.")
+
+        device = job_data.device
+        job_data = job_data.id
+    else:
+        if device is None:
+            raise ValueError(
+                "To get a remote result from a job it, please also provide the "
+                "device to get the data from."
+            )
 
-    # if the device is not a remote one
     if not device.is_remote():
         raise ValueError(
             "Trying to retrieve a remote result while the device of the job was local."
         )
 
-    # check the type of the device, and call the right job getter
     if isinstance(device, IBMDevice):
-        return get_result_from_ibm_job_id(job_id)
+        return get_result_from_ibm_job_id(job_data)
     elif isinstance(device, ATOSDevice):
-        return get_result_from_qlm_job_id(job_id)
+        return get_result_from_qlm_job_id(job_data)
     elif isinstance(device, AWSDevice):
-        return get_result_from_aws_task_arn(job_id)
+        return get_result_from_aws_task_arn(job_data)
     else:
         raise NotImplementedError(
             f"The device {device.name} is not supported for remote features."
         )
 
 
-@typechecked
-def remote_result_from_job(job: Job) -> Result:
-    """Retrieve and parse a remote the result from an mpqp job. If the job is
-    still running, it will wait until it is done.
-
-    Args:
-        job: MPQP job for which we want to retrieve the result from the remote
-            device.
-
-    Returns:
-        A Result of the remote job in parameter.
-    """
-    if job.id is None:
-        raise ValueError("Can't retrieve remote result for a job whose id is None.")
-    return remote_result_from_id(job.id, job.device)
-
-
 def get_all_job_ids() -> dict[type[AvailableDevice], list[str]]:
     """Retrieve from the remote providers all the job-ids associated with this
     account.
 
     Returns:
         A dictionary of job-ids indexed by the correspond AvailableDevice
         (ATOSDevice, AWSDevice, IBMDevice, ...).
     """
     job_ids: dict[type[AvailableDevice], list[str]] = {
-        AWSDevice: get_all_task_ids(),
+        AWSDevice: aws_ids(),
         ATOSDevice: qlm_ids(),
         IBMDevice: ibm_ids(),
+        GOOGLEDevice: cirq_ids(),
     }
 
     return job_ids
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/runner.py` & `mpqp-0.2.0/mpqp/execution/runner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,67 @@
+"""
+Once the circuit is defined, you can to execute it and retrieve the result using
+the function :func:`run`. You can execute said circuit on one or several devices
+(local or remote). The function will wait (blocking) until the job is completed
+and will return a :class:`Result<mpqp.execution.result.Result>` in only one
+device was given or a :class:`BatchResult<mpqp.execution.result.BatchResult>` 
+otherwise (see :ref:`below<Results>`).
+
+Alternatively, when running jobs on a remote device, you could prefer to
+retrieve the result asynchronously, without having to wait and block the
+application until the computation is completed. In that case, you can use the
+:func:`submit` instead. It will submit the job and
+return the corresponding job id and :class:`Job<mpqp.execution.job.Job>` object.
+
+.. note::
+    Unlike :func:`run`, we can only submit on one device at a time.
+"""
+
 from __future__ import annotations
 
-from typing import Optional, Union
+from numbers import Complex
+from typing import Iterable, Optional, Union
 
 import numpy as np
 from sympy import Expr
 from typeguard import typechecked
-from numbers import Complex
 
 from mpqp.core.circuit import QCircuit
 from mpqp.core.instruction.measurement.basis_measure import BasisMeasure
 from mpqp.core.instruction.measurement.expectation_value import (
     ExpectationMeasure,
     Observable,
 )
-from mpqp.execution.devices import AvailableDevice, IBMDevice, ATOSDevice, AWSDevice
-from mpqp.execution.providers_execution.aws_execution import (
-    run_braket,
-    submit_job_braket,
+from mpqp.execution.devices import (
+    ATOSDevice,
+    AvailableDevice,
+    AWSDevice,
+    GOOGLEDevice,
+    IBMDevice,
 )
-from mpqp.execution.providers_execution.atos_execution import run_atos, submit_QLM
-from mpqp.execution.providers_execution.ibm_execution import run_ibm, submit_ibmq
-from mpqp.execution.result import Result, BatchResult
-from mpqp.execution.job import Job, JobType, JobStatus
-from mpqp.tools.errors import RemoteExecutionError
+from mpqp.execution.job import Job, JobStatus, JobType
+from mpqp.execution.providers.atos import run_atos, submit_QLM
+from mpqp.execution.providers.aws import run_braket, submit_job_braket
+from mpqp.execution.providers.google import run_google
+from mpqp.execution.providers.ibm import run_ibm, submit_ibmq
+from mpqp.execution.result import BatchResult, Result
+from mpqp.tools.errors import DeviceJobIncompatibleError, RemoteExecutionError
+from mpqp.tools.generics import OneOrMany
 
 
 @typechecked
 def adjust_measure(measure: ExpectationMeasure, circuit: QCircuit):
-    """We allow the measure to not span the entire circuit, but none of our
-    providers allow for that. So we patch the measure with this function, with
-    identities on the qubits that no not interest our user.
+    """We allow the measure to not span the entire circuit, but providers
+    usually don't support this behavior. To make this work we tweak the measure
+    this function to match the expected behavior.
+
+    In order to do this, we add identity measures on the qubits not targeted by
+    the measure. In addition of this, some swaps are automatically added so the
+    the qubits measured are ordered and contiguous (though this is done in
+    :func:`generate_job`)
 
     Args:
         measure: The expectation measure, potentially incomplete.
         circuit: The circuit to which will be added the potential swaps allowing
             the user to get the expectation value of the qubits in an arbitrary
             order (this part is not handled by this function).
 
@@ -54,41 +82,42 @@
     return tweaked_measure
 
 
 @typechecked
 def generate_job(
     circuit: QCircuit, device: AvailableDevice, values: dict[Expr | str, Complex] = {}
 ) -> Job:
-    """Create a Job from the circuit and the eventual measurements. If the
-    circuit depends on variables, the values given in parameters are used to do
-    the substitution.
+    """Creates the Job of appropriate type and containing the information needed
+    for the execution of the circuit.
+
+    If the circuit contains symbolic variables (see section :ref:`VQA` for more
+    information on them), the ``values`` parameter is used perform the necessary
+    substitutions.
 
     Args:
         circuit: Circuit to be run.
         device: Device on which the circuit will be run.
         values: Set of values to substitute symbolic variables.
 
     Returns:
         The Job containing information about the execution of the circuit.
     """
     circuit = circuit.subs(values, True)
 
-    # get the measurements of this circuit
     m_list = circuit.get_measurements()
     nb_meas = len(m_list)
 
-    # determine the job type and create the right job
     if nb_meas == 0:
         job = Job(JobType.STATE_VECTOR, circuit, device)
     elif nb_meas == 1:
         measurement = m_list[0]
         if isinstance(measurement, BasisMeasure):
-            # 3M-TODO: handle other basis by adding the right rotation (change of basis) before
-            #       measuring in the computational basis
-            # 3M-TODO: Muhammad circuit.add(CustomGate(UnitaryMatrix(change_of_basis_inverse)))
+            # 3M-TODO: handle other basis by adding the right rotation (change
+            # of basis) before measuring in the computational basis
+            # Muhammad: circuit.add(CustomGate(UnitaryMatrix(change_of_basis_inverse)))
             if measurement.shots <= 0:
                 job = Job(JobType.STATE_VECTOR, circuit, device)
             else:
                 job = Job(JobType.SAMPLE, circuit, device, measurement)
         elif isinstance(measurement, ExpectationMeasure):
             job = Job(
                 JobType.OBSERVABLE,
@@ -98,15 +127,16 @@
             )
         else:
             raise NotImplementedError(
                 f"Measurement type {type(measurement)} not handled"
             )
     else:
         raise NotImplementedError(
-            "Cannot handle several measurement in the current version"
+            "Current version of MPQP do not support multiple measurement in a "
+            "circuit."
         )
 
     return job
 
 
 @typechecked
 def _run_single(
@@ -119,47 +149,68 @@
         circuit: QCircuit to be run.
         device: Device, on which the circuit will be run.
         values: Set of values to substitute symbolic variables. Defaults to ``{}``.
 
     Returns:
         The Result containing information about the measurement required.
 
-    Examples:
+    Raises:
+        DeviceJobIncompatibleError: if a non noisy simulator is given in parameter and the circuit contains noise
+        NotImplementedError: If the device is not handled for noisy simulation or other submissions.
+
+    Example:
         >>> c = QCircuit([H(0), CNOT(0, 1), BasisMeasure([0, 1], shots=1000)], label="Bell pair")
         >>> result = run(c, IBMDevice.AER_SIMULATOR)
-        >>> print(result)
+        >>> print(result) # doctest: +SKIP
         Result: IBMDevice, AER_SIMULATOR
-        Counts: [512, 0, 0, 488]
-        Probabilities: [0.512 0.    0.    0.488]
-        State: 00, Index: 0, Count: 512, Probability: 0.512
-        State: 11, Index: 3, Count: 488, Probability: 0.488
-        Error: None
+         Probabilities: [0.523, 0, 0, 0.477]
+         Counts: [523, 0, 0, 477]
+         Samples:
+          State: 00, Index: 0, Count: 523, Probability: 0.523
+          State: 11, Index: 3, Count: 477, Probability: 0.477
+         Error: None
+
     """
     job = generate_job(circuit, device, values)
     job.status = JobStatus.INIT
 
+    if circuit.noises:
+        if not device.is_noisy_simulator():
+            raise DeviceJobIncompatibleError(
+                f"Device {device} cannot simulate circuits containing NoiseModels."
+            )
+        elif not (isinstance(device, ATOSDevice) or isinstance(device, AWSDevice)):
+            raise NotImplementedError(
+                f"Noisy simulations are not yet available on devices of type {type(device).name}."
+            )
+
     if isinstance(device, IBMDevice):
         return run_ibm(job)
     elif isinstance(device, ATOSDevice):
         return run_atos(job)
     elif isinstance(device, AWSDevice):
         return run_braket(job)
+    elif isinstance(device, GOOGLEDevice):
+        return run_google(job)
     else:
         raise NotImplementedError(f"Device {device} not handled")
 
 
 @typechecked
 def run(
     circuit: QCircuit,
-    device: AvailableDevice | list[AvailableDevice],
+    device: OneOrMany[AvailableDevice],
     values: Optional[dict[Expr | str, Complex]] = None,
 ) -> Union[Result, BatchResult]:
     """Runs the circuit on the backend, or list of backend, provided in
-    parameter. If the circuit depends on variables, the values given in
-    parameters are used to do the substitution.
+    parameter.
+
+    If the circuit contains symbolic variables (see section :ref:`VQA` for more
+    information on them), the ``values`` parameter is used perform the necessary
+    substitutions.
 
     Args:
         circuit: QCircuit to be run.
         device: Device, or list of devices, on which the circuit will be run.
         values: Set of values to substitute symbolic variables. Defaults to ``{}``.
 
     Returns:
@@ -167,82 +218,86 @@
 
     Examples:
         >>> c = QCircuit(
         ...     [H(0), CNOT(0, 1), BasisMeasure([0, 1], shots=1000)],
         ...     label="Bell pair",
         ... )
         >>> result = run(c, IBMDevice.AER_SIMULATOR)
-        >>> print(result)
+        >>> print(result) # doctest: +SKIP
         Result: IBMDevice, AER_SIMULATOR
-        Counts: [512, 0, 0, 488]
-        Probabilities: [0.512 0.    0.    0.488]
-        State: 00, Index: 0, Count: 512, Probability: 0.512
-        State: 11, Index: 3, Count: 488, Probability: 0.488
-        Error: None
+         Counts: [497, 0, 0, 503]
+         Probabilities: [0.497, 0, 0, 0.503]
+         Samples:
+          State: 00, Index: 0, Count: 497, Probability: 0.497
+          State: 11, Index: 3, Count: 503, Probability: 0.503
+         Error: None
         >>> batch_result = run(
         ...     c,
         ...     [ATOSDevice.MYQLM_PYLINALG, AWSDevice.BRAKET_LOCAL_SIMULATOR]
         ... )
-        >>> print(batch_result)
+        >>> print(batch_result) # doctest: +SKIP
         BatchResult: 2 results
-        Result: AWSDevice, BRAKET_LOCAL_SIMULATOR
-        Counts: [492, 0, 0, 508]
-        Probabilities: [0.492 0.    0.    0.508]
-        State: 00, Index: 0, Count: 492, Probability: 0.492
-        State: 11, Index: 3, Count: 508, Probability: 0.508
-        Error: None
         Result: ATOSDevice, MYQLM_PYLINALG
-        Counts: [462, 0, 0, 538]
-        Probabilities: [0.462 0.    0.    0.538]
-        State: 00, Index: 0, Count: 462, Probability: 0.462
-        State: 11, Index: 3, Count: 538, Probability: 0.538
-        Error: 0.015773547629015002
+         Counts: [499, 0, 0, 501]
+         Probabilities: [0.499, 0, 0, 0.501]
+         Samples:
+          State: 00, Index: 0, Count: 499, Probability: 0.499
+          State: 11, Index: 3, Count: 501, Probability: 0.501
+         Error: 0.01581926829057682
+        Result: AWSDevice, BRAKET_LOCAL_SIMULATOR
+         Counts: [502, 0, 0, 498]
+         Probabilities: [0.502, 0, 0, 0.498]
+         Samples:
+          State: 00, Index: 0, Count: 502, Probability: 0.502
+          State: 11, Index: 3, Count: 498, Probability: 0.498
+         Error: None
+
     """
 
     if values is None:
         values = {}
 
-    if isinstance(device, list):
-        # Duplicate devices are removed
-        set_device = list(set(device))
-        if len(set_device) == 1:
-            return _run_single(circuit, set_device[0], values)
-
-        return BatchResult(
-            [_run_single(circuit, dev, values) for dev in set_device]
-        )
+    if isinstance(device, Iterable):
+        return BatchResult([_run_single(circuit, dev, values) for dev in set(device)])
 
     return _run_single(circuit, device, values)
 
 
 @typechecked
 def submit(
     circuit: QCircuit, device: AvailableDevice, values: dict[Expr | str, Complex] = {}
 ) -> tuple[str, Job]:
-    """
-    Submit the job related with the circuit on the remote backend provided in parameter.
-    The submission returns a job_id that can be used to retrieve the Result later.
-    If the circuit depends on variables, the values given in parameters are used to do the substitution.
-    Unlike :meth:`run`, for the moment, one can only submit a circuit to a single device.
+    """Submit the job related with the circuit on the remote backend provided in
+    parameter. The submission returns a ``job_id`` that can be used to retrieve
+    the :class:`Result<mpqp.execution.result.Result>` later, using the
+    :func:`get_remote_result<mpqp.execution.remote_handler.get_remote_result>`
+    function.
+
+    If the circuit contains symbolic variables (see section :ref:`VQA` for more
+    information on them), the ``values`` parameter is used perform the necessary
+    substitutions.
 
-    Examples:
-        >>> circuit = QCircuit([H(0), CNOT(0,1), BasisMeasure([0,1], shots=10)])
-        >>> job_id, job = submit(circuit, ATOSDevice.QLM_LINALG)
-        Logging as user <qlm_user>...
-        Submitted a new batch: Job766
-        >>> print("Status of " +job_id +":", job.job_status)
-        Status of Job766: JobStatus.RUNNING
+    Mind that this function only support single device submissions.
 
     Args:
         circuit: QCircuit to be run.
         device: Remote device on which the circuit will be submitted.
         values: Set of values to substitute symbolic variables.
 
     Returns:
         The job id provided by the remote device after submission of the job.
+
+    Example:
+        >>> circuit = QCircuit([H(0), CNOT(0,1), BasisMeasure([0,1], shots=10)])
+        >>> job_id, job = submit(circuit, ATOSDevice.QLM_LINALG) #doctest: +SKIP
+        Logging as user <qlm_user>...
+        Submitted a new batch: Job766
+        >>> print("Status of " +job_id +":", job.job_status) #doctest: +SKIP
+        Status of Job766: JobStatus.RUNNING
+
     """
     if not device.is_remote():
         raise RemoteExecutionError(
             "submit(...) function is only made for remote device."
         )
 
     job = generate_job(circuit, device, values)
```

### Comparing `mpqp-0.1.dev1/mpqp/execution/vqa/vqa.py` & `mpqp-0.2.0/mpqp/execution/vqa/vqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
-from typing import Any, Collection, TypeVar, Union
-from typing import Callable, Optional
-from scipy.optimize import minimize as scipy_minimize, OptimizeResult
-from sympy import Expr
+from typing import Any, Callable, Collection, Optional, TypeVar, Union
+
 import numpy as np
 import numpy.typing as npt
+from scipy.optimize import OptimizeResult
+from scipy.optimize import minimize as scipy_minimize
+from sympy import Expr
 from typeguard import typechecked
 
 from mpqp.core.circuit import QCircuit
 from mpqp.execution.devices import AvailableDevice
 from mpqp.execution.runner import _run_single  # pyright: ignore[reportPrivateUsage]
 from mpqp.execution.vqa.optimizer import Optimizer
 
@@ -38,18 +39,40 @@
     optimizable: QCircuit | OptimizableFunc,
     method: Optimizer | OptimizerCallable,
     device: Optional[AvailableDevice] = None,
     init_params: Optional[OptimizerInput] = None,
     nb_params: Optional[int] = None,
     optimizer_options: Optional[dict[str, Any]] = None,
 ) -> tuple[float, OptimizerInput]:
-    """This function runs an optimization on the parameters of the circuit, to
-    minimize the expectation value of the measure of the circuit by it's
-    observables. Note that this means that the circuit should contain an
-    expectation measure!
+    """This function runs an optimization on the parameters of the circuit, in order to
+    minimize the measured expectation value of observables associated with the given circuit.
+    Note that this means that the latter should contain an ``ExpectationMeasure``.
+
+    Args:
+        optimizable: Either the circuit, containing symbols and an expectation
+            measure, or the evaluation function.
+        method: The method used to optimize most of those methods come from
+            ``scipy``. If the choices offered in this package are not
+            covering your needs, you can define your own optimizer. This should be
+            a function taking as input a function representing the circuit, with
+            as many inputs as the circuit has parameters, and any optional
+            initialization parameters, and returning the optimal value reached
+            and the parameters used to reach this value.
+        device: The device on which the circuit should be run.
+        init_params: The optional initialization parameters (the value
+            attributed to the symbols in the first loop of the optimizer).
+        nb_params: Number of variables to input in ``optimizable``. It is only
+            useful if ``optimizable`` is a Callable and if ``init_params`` was
+            not given. If not this argument is not taken into account.
+        optimizer_options: Options used to configure the VQA optimizer (maximum
+            iterations, convergence threshold, etc...). These options are passed
+            as is to the minimizer.
+
+    Returns:
+        The optimal value reached and the parameters corresponding to this value.
 
     Examples:
         >>> alpha, beta = symbols("α β")
         >>> circuit = QCircuit([
         ...     H(0),
         ...     Rx(alpha, 1),
         ...     CNOT(1,0),
@@ -80,36 +103,14 @@
         ...     cost_func,
         ...     Optimizer.BFGS,
         ...     nb_params=2,
         ...     optimizer_options={"maxiter":50},
         ... )
         (8.881784197001252e-16, array([0., 0.]))
 
-    Args:
-        optimizable: Either the circuit, containing symbols and an expectation
-            measure, or the evaluation function.
-        method: The method used to optimize most of those methods come from
-            either scipy or cma. If the choice offered in this package are not
-            covering your needs, you can define your own optimizer. It should be
-            a function taking as input a function representing the circuit, with
-            as many inputs as the circuit has parameters, as well as optional
-            initialization parameters, and returning the optimal value reached
-            and the parameters used to reach this value.
-        device: The device on which the circuit should be run.
-        init_params: The optional initialization parameters (the value
-            attributed to the symbols in the first loop of the optimizer).
-        nb_params: Number of variables to input in ``optimizable``. It is only
-            useful if ``optimizable`` is a Callable and if ``init_params`` was
-            not given. If not this argument is not taken into account.
-        optimizer_options: Options used to configure the VQA optimizer (maximum
-            iterations, convergence threshold, etc...). These options are passed
-            as is to the minimizer.
-
-    Returns:
-        The optimal value reached and the parameters used to reach this value.
     """
     if isinstance(optimizable, QCircuit):
         if device is None:
             raise ValueError("A device is needed to optimize a circuit")
         optimizer = _minimize_remote if device.is_remote() else _minimize_local
         return optimizer(optimizable, method, device, init_params, nb_params)
     else:
```

### Comparing `mpqp-0.1.dev1/mpqp/qasm/header_codes/braket_custom_include.inc` & `mpqp-0.2.0/mpqp/qasm/header_codes/braket_custom_include.inc`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/mpqp/qasm/header_codes/qelib1.inc` & `mpqp-0.2.0/mpqp/qasm/header_codes/qelib1.inc`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/mpqp/qasm/header_codes/stdgates.inc` & `mpqp-0.2.0/mpqp/qasm/header_codes/stdgates.inc`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/mpqp/qasm/open_qasm_2_and_3.py` & `mpqp-0.2.0/mpqp/qasm/open_qasm_2_and_3.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,55 @@
+"""The latest version of OpenQASM (3.0, started in 2020) has been released by
+conjoint members of IBM Quantum, AWS Quantum Computing, Zapata Computing, Zurich
+Instruments and University of Oxford. This version extends the 2.0 one, adding
+some advanced features, and modifying parts of syntax and grammar, making some
+part of OpenQASM 2.0 not fully retro-compatible (hence why we need to keep track
+of the instructions requiring custom definitions in :class:`Instr`).
+
+This being said, this "new" version was quite slow to come to SDKs, so to help
+the transition we are making a few conversion functions available. The main one
+being :func:`open_qasm_2_to_3`.
+
+The translation is performed in a two main steps:
+
+1. the OpenQASM 2.0 code is parsed by :func:`parse_openqasm_2_file` (it's a
+   basic parse, separating the instructions),
+2. each instruction is converted to it's OpenQASM 3.0 counterpart by
+   :func:`convert_instruction_2_to_3`,
+
+Since :func:`open_qasm_2_to_3` needs a few tricky parameters to function
+properly, you also have access to a shorthand accepting directly the path of the
+file you want to convert: :func:`open_qasm_file_conversion_2_to_3`.
+
+In some cases, having multiple files to deal with can be cumbersome. You can
+avoid this pain point by uniting all your source files in a single one using
+:func:`open_qasm_hard_includes`.
+
+On the other hand, some providers such as Cirq do not support user defined
+gates, requiring to replace all user gate calls by their definition. This is
+done using :func:`remove_user_gates`.
+"""
+
 import os
-from pathlib import Path
 import re
-from os.path import splitext
 from enum import Enum
-
-from warnings import warn
+from os.path import splitext
+from pathlib import Path
 from textwrap import dedent
+from warnings import warn
+
 from anytree import Node, PreOrderIter
 from typeguard import typechecked
 
 from mpqp.tools.errors import InstructionParsingError
 
 
 class Instr(Enum):
-    """Special instruction of which the definition needs to included in the
-    header of the file."""
+    """Special instruction for which the definition needs to included in the
+    file."""
 
     STD_LIB = 0
     CSX = 1
     U0 = 2
     CU3 = 3
     SXDG = 4
     RZZ = 5
@@ -83,15 +114,15 @@
 @typechecked
 def qasm_code(instr: Instr) -> str:
     """Return the string corresponding of the declaration of the instruction in
     parameter. It is also used to return the whole standard library string when
     we hard include it.
 
     Args:
-        instr: Instr for which we want the corresponding OpenQASM code
+        instr: Instr for which we want the corresponding OpenQASM code.
 
     Returns:
         OpenQASM definition of ``instr``.
     """
 
     # 3M-TODO: if run from outside the mpqp folder, the following line will fuck things up, fix it
     headers_folder = os.path.dirname(__file__) + "/header_codes/"
@@ -111,39 +142,40 @@
 
 
 @typechecked
 def parse_openqasm_2_file(code: str) -> list[str]:
     """Splits a complete OpenQASM2 program into individual instructions.
 
     Args:
-        code: The complete OpenQASM 2.0 program, we do not check for correct syntax, it is assumed that the code is
-        well formed.
+        code: The complete OpenQASM 2.0 program.
 
     Returns:
         List of instructions.
+
+    Note:
+        we do not check for correct syntax, it is assumed that the code is well
+        formed.
     """
     # 6M-TODO: deal with comments, for the moment we remove them all
 
     # removing comment
     cleaned_code = "".join([loc.split("//")[0] for loc in code.split("\n")])
 
     cleaned_code = cleaned_code.replace("\t", " ").strip()
 
-    # gate must be registered as a single instruction
     gate_matches = list(re.finditer(r"gate .*?}", cleaned_code))
-    # we start with adding all the instructions up to the first gate definition
     sanitized_start = (
         cleaned_code[: gate_matches[0].span()[0]] if gate_matches else cleaned_code
     )
     instructions = sanitized_start.split(";")
 
-    # we then add turn by turn the following gate definition, all the
-    # instructions between it and the next one, and so on...
     for i in range(len(gate_matches)):
+        # gates definition are added as a single instruction
         instructions.append(cleaned_code[slice(*(gate_matches[i].span()))])
+        # all instructions between two gate definitions are added individually
         instructions.extend(
             cleaned_code[
                 gate_matches[i].span()[1] : (
                     None
                     if i == len(gate_matches) - 1
                     else gate_matches[i + 1].span()[0]
                 )
@@ -153,29 +185,29 @@
     return list(filter(lambda i: i != "", instructions))
 
 
 @typechecked
 def convert_instruction_2_to_3(
     instr: str,
     included_instr: set[Instr],
-    included_tree_current_node: Node,
+    included_tree_current: Node,
     defined_gates: set[str],
     path_to_main: str = ".",
 ) -> tuple[str, str]:
     """Some instructions changed name from QASM 2 to QASM 3, also the way to
     import files changed slightly. This function operates those changes on a
     single instruction.
 
     Args:
         instr: Instruction to be upgraded.
         included_instr: Some instructions need new imports, in order to keep
-            track of which instruction are already
+            track of which instruction are already.
         imported in the overall scope, a dictionary of already included
             instructions is passed and modified along.
-        included_tree_current_node: Current Node in the file inclusion tree.
+        included_tree_current: Current Node in the file inclusion tree.
         defined_gates: Set of custom gates already defined.
         path_to_main: Path to the main folder from which include paths are
             described.
 
     Returns:
         The upgraded instruction and the potential code to add in the header as
         the second element.
@@ -198,21 +230,23 @@
 
     # If the line is the OpenQASM header
     if instr.startswith("OPENQASM 2.0"):
         header_code += "OPENQASM 3.0;\n"
     elif instr_name == "include":
         path = instr.split(" ")[-1].strip("'\"")
         if path != "qelib1.inc":
-            if is_path_in_ancestors(path, included_tree_current_node):
+            if any(path in node.name for node in included_tree_current.ancestors):
                 raise RuntimeError("Circular dependency detected.")
             # Convert the file included, add it to the inclusion tree,
             # and create a new file and include it in the converted code
-            if not is_path_in_tree(path, included_tree_current_node):
+            if not any(
+                path in node.name for node in PreOrderIter(included_tree_current.root)
+            ):  # checks in the path is not already included
                 with open(f"{path_to_main}/{path}", "r") as f:
-                    child = Node(path, parent=included_tree_current_node)
+                    child = Node(path, parent=included_tree_current)
                     converted_content = open_qasm_2_to_3(
                         f.read(), child, path_to_main, defined_gates
                     )
                 new_path = splitext(path)[0] + "_converted" + splitext(path)[1]
                 with open(f"{path_to_main}/{new_path}", "w") as f:
                     f.write(converted_content)
                 header_code += f"include '{new_path}';\n"
@@ -266,28 +300,28 @@
             instr.split("{")[1].split("}")[0].split(";"),
         )
         for instruction in g_instructions:
             instruction = instruction.strip()
             i_code, h_code = convert_instruction_2_to_3(
                 instruction,
                 included_instr,
-                included_tree_current_node,
+                included_tree_current,
                 defined_gates,
                 path_to_main,
             )
             g_string += " " * 4 + i_code
             header_code += h_code
         instructions_code += g_string + "}\n"
     elif instr_name == "if":
         if_statement = instr.split(")")[0] + ")"
         nested_instr = ")".join(instr.split(")")[1:])
         i_code, h_code = convert_instruction_2_to_3(
             nested_instr,
             included_instr,
-            included_tree_current_node,
+            included_tree_current,
             defined_gates,
             path_to_main,
         )
         instructions_code += if_statement + i_code + ";\n"
         header_code += h_code
     elif instr_name == "opaque":
         raise NotImplementedError("opaque exports not handled yet")
@@ -308,47 +342,49 @@
     code: str,
     included_tree_current_node: Node = Node("initial_code"),
     path_to_file: str = ".",
     defined_gates: set[str] = set(),
 ) -> str:
     """Converts an OpenQASM code from version 2.0 and 3.0.
 
-    It is a partial conversion (mainly circuit structure) for helping building
-    temporary bridges between different platforms that use different versions.
+    This function will also recursively go through the imported files to
+    translate them too. It is a partial conversion (the ``opaque`` keyword is
+    not handled and comments are stripped) for helping building temporary
+    bridges between different platforms that use different versions.
 
     Args:
-        code: string containing the OpenQASM 2.0 code and instructions
+        code: String containing the OpenQASM 2.0 code and instructions.
         included_tree_current_node: Current Node in the file inclusion tree.
         path_to_file: Path to the location of the file from which the code is
             coming (useful for locating imports).
         defined_gates: Set of custom gates already defined.
 
     Returns:
         Converted OpenQASM code in the 3.0 version.
 
-    Examples:
-        >>> qasm2_str = '''\\
-        ... OPENQASM 2.0;
+    Example:
+        >>> qasm2_str = '''OPENQASM 2.0;
         ... qreg q[2];
         ... creg c[2];
         ... h q[0];
         ... cx q[0],q[1];
         ... measure q[0] -> c[0];
         ... measure q[1] -> c[1];
         ... '''
-        >>> open_qasm_2_to_3(qasm2_str)
-        '''OPENQASM 3.0;
-        include 'stdgates.inc';
+        >>> print(open_qasm_2_to_3(qasm2_str)) # doctest: +NORMALIZE_WHITESPACE
+        OPENQASM 3.0;
+        include "stdgates.inc";
         qubit[2] q;
         bit[2] c;
         h q[0];
         cx q[0],q[1];
         c[0] = measure q[0];
         c[1] = measure q[1];
-        '''
+
+
     """
 
     header_code = ""
     instructions_code = ""
 
     instructions = parse_openqasm_2_file(code)
 
@@ -372,67 +408,68 @@
     return target_code
 
 
 @typechecked
 def open_qasm_file_conversion_2_to_3(path: str) -> str:
     """Converts an OpenQASM code in a file from version 2.0 and 3.0.
 
-    It is a partial conversion (mainly circuit structure) for helping building
-    temporary bridges between different platforms that use different versions.
+    This function is a shorthand to initialize :func:`open_qasm_2_to_3` with the
+    correct values.
 
     Args:
         path: Path to the file containing the OpenQASM 2.0 code, and eventual
             imports.
 
     Returns:
         Converted OpenQASM code in the 3.0 version.
 
     Examples:
-        >>> example_dir = "example/qasm_files/"
+        >>> example_dir = "examples/scripts/qasm_files/"
         >>> with open(example_dir + "main.qasm", "r") as f:
-        ...     print(f.read())
-        '''OPENQASM 2.0;
+        ...     print(f.read()) # doctest: +NORMALIZE_WHITESPACE
+        OPENQASM 2.0;
         include "include1.qasm";
         include "include2.qasm";
         qreg q[2];
         creg c[2];
         h q[0];
         cx q[0],q[1];
         gate2 q[0];
         gate3 q[0], q[1];
         measure q[0] -> c[0];
-        measure q[1] -> c[1];'''
-        >>> print(open_qasm_file_conversion_2_to_3(example_dir + "main.qasm"))
-        '''OPENQASM 3.0;
+        measure q[1] -> c[1];
+        >>> print(open_qasm_file_conversion_2_to_3(example_dir + "main.qasm")) # doctest: +NORMALIZE_WHITESPACE
+        OPENQASM 3.0;
         include 'include1_converted.qasm';
         include 'include2_converted.qasm';
-        include 'stdgates.inc';
+        include "stdgates.inc";
         qubit[2] q;
         bit[2] c;
         h q[0];
         cx q[0],q[1];
         gate2 q[0];
         gate3 q[0], q[1];
         c[0] = measure q[0];
-        c[1] = measure q[1];'''
+        c[1] = measure q[1];
         >>> with open(example_dir + "include1_converted.qasm", "r") as f:
-        ...     print(f.read())
-        '''OPENQASM 3.0;
-        include 'stdgates.inc';
+        ...     print(f.read()) # doctest: +NORMALIZE_WHITESPACE
+        OPENQASM 3.0;
+        include "stdgates.inc";
         gate gate2 a {
             u3(pi, -pi/2, pi/2) a;
-        }'''
+        }
         >>> with open(example_dir + "include2_converted.qasm", "r") as f:
-        ...     print(f.read())
-        '''OPENQASM 3.0;
-        include 'stdgates.inc';
+        ...     print(f.read()) # doctest: +NORMALIZE_WHITESPACE
+        OPENQASM 3.0;
+        include "stdgates.inc";
         gate gate3 a, b {
             u3(0, -pi/2, pi/3) a;
             cz a, b;
-        }'''
+        }
+
     """
 
     with open(path, "r") as f:
         code = f.read()
         return open_qasm_2_to_3(code, Node(path), str(Path(path).parent))
 
 
@@ -443,34 +480,35 @@
     path_to_file: str = "./",
     is_openqasm_header_included: bool = False,
 ) -> str:
     r"""Converts an OpenQASM code (2.0 and 3.0) to use no includes, but writes
     every instruction in previously included files, directly in the code
     returned.
 
-    Examples:
-        >>> examples_folder = "tests/qasm/qasm_examples"
-        >>> filename = examples_folder + "/with_include.qasm"
-        >>> with open(filename) as f:
-        ...     print(open_qasm_hard_includes(f.read(), {filename}).strip("\n"))
-        '''gate csx a, b {
-            ctrl @ sx a, b;
-        }'''
-
     Args:
         code: String containing the OpenQASM code and instructions.
         included_files: The set of files already included, used to avoid
             duplicate imports and circular dependencies. This set should be
             initialized with the name of the root file you started with.
-        path_to_file: Path used to localize files that are inputted.
+        path_to_file: Path used to localize files that are included.
         is_openqasm_header_included: Boolean used to only include once the
             OpenQASM header.
 
     Returns:
         Include-less OpenQASM code.
+
+    Example:
+        >>> examples_folder = "tests/qasm/qasm_examples"
+        >>> filename = examples_folder + "/with_include.qasm"
+        >>> with open(filename) as f:
+        ...     print(open_qasm_hard_includes(f.read(), {filename}).strip("\n"))
+        gate csx a, b {
+            ctrl @ sx a, b;
+        }
+
     """
     lines = code.split("\n")
     converted_code = []
 
     for line in lines:
         if "include" in line:
             line_array = line.split()
@@ -501,35 +539,142 @@
         else:
             if not line.startswith("//"):
                 converted_code.append(line)
 
     return "\n".join(converted_code)
 
 
-@typechecked
-def is_path_in_tree(path: str, any_node: Node):
-    """Checks if a path is already present in a node of the tree represented by
-    one of his nodes (in parameter).
+def parse_user_gates(qasm_code: str) -> tuple[dict[str, str], str]:
+    r"""Parses user gate definitions from QASM code.
 
     Args:
-        path: Element to search in the tree.
-        any_node: One node of the tree on which we want to search.
+        qasm_code: The QASM code containing user gate definitions.
 
     Returns:
-        True if the path is the name of one of the nodes of the tree.
+        A tuple containing a dictionary of user gate definitions
+        and the QASM string stripped of it's user gate definitions.
+
+    Example:
+        >>> qasm_str = '''gate rzz(theta) a,b {
+        ...     cx a,b;
+        ...     u1(theta) b;
+        ...     cx a,b;
+        ... }
+        ... qubit[3] q;
+        ... bit[1] c0;
+        ... bit[1] c1;
+        ... rzz(0.2) q[1], q[2];
+        ... c2[0] = measure q[2];'''
+        >>> print(parse_user_gates(qasm_str))
+        ({'rzz': [['theta'], ['a', 'b'], 'cx a,b;', 'u1(theta) b;', 'cx a,b;']}, 'qubit[3] q;\nbit[1] c0;\nbit[1] c1;\nrzz(0.2) q[1], q[2];\nc2[0] = measure q[2];')
     """
-    return any([path in node.name for node in PreOrderIter(any_node.root)])
+    # TODO: for cleaner gate definitions, they could be objects instead of lists
+    user_gate_definitions = {}
 
+    replaced_code = qasm_code
 
-@typechecked
-def is_path_in_ancestors(path: str, node: Node):
-    """Checks if a path is already present in an ancestor of the node in
-    parameter.
+    lines = qasm_code.split("\n")
+
+    in_user_gate = False
+    current_gate_name = ""
+    current_gate_definition = []
+
+    for line in lines:
+        if line.strip().startswith("gate"):
+            in_user_gate = True
+            current_gate_name_parameters = line.split()[1].split("(")
+            current_gate_name = current_gate_name_parameters[0]
+            current_gate_parameters = (
+                current_gate_name_parameters[1][:-1].split(",")
+                if len(current_gate_name_parameters) > 1
+                else ""
+            )
+            current_gate_definition = []
+            current_gate_qubits = ""
+            for elem in line.split()[2:]:
+                current_gate_qubits += elem
+            current_gate_qubits = current_gate_qubits.replace("{", "").split(",")
+
+            current_gate_definition.append(current_gate_parameters)
+            current_gate_definition.append(current_gate_qubits)
+            replaced_code = replaced_code.replace(line + "\n", "")
+        elif in_user_gate:
+            if line.strip().endswith("}"):
+                user_gate_definitions[current_gate_name] = current_gate_definition
+                in_user_gate = False
+            else:
+                current_gate_definition.append(line.strip())
+            replaced_code = replaced_code.replace(line + "\n", "")
+
+    return user_gate_definitions, replaced_code
+
+
+def remove_user_gates(qasm_code: str) -> str:
+    """Replaces instances of user gates with their definitions in the given QASM
+    code. This uses :func:`parse_user_gates` to separate the gate definitions
+    from the rest of the code.
 
     Args:
-        path: Element to search in the tree.
-        node: The node for which we want to search in his ancestors.
+        qasm_code: The QASM code containing user gate calls.
 
     Returns:
-        True if the path is the name of one of the ancestors of the node/
+        The QASM code with user gate calls replaced by their definitions.
+
+    Example:
+        >>> qasm_str = '''gate MyGate a, b {
+        ...      h a;
+        ...      cx a, b;
+        ... }
+        ... qreg q[3];
+        ... creg c[2];
+        ... MyGate q[0], q[1];
+        ... measure q -> c;'''
+        >>> print(remove_user_gates(qasm_str))
+        qreg q[3];
+        creg c[2];
+        h q[0];
+        cx q[0], q[1];
+        measure q -> c;
     """
-    return any([path in node.name for node in node.ancestors])
+    replaced_code = qasm_code
+    user_gate_definitions, replaced_code = parse_user_gates(qasm_code)
+
+    for gate_name in user_gate_definitions:
+
+        lines = qasm_code.split("\n")
+        for line in lines:
+            if line.strip().startswith(gate_name + " ") or line.strip().startswith(
+                gate_name + "("
+            ):
+                current_gate_qubits = [
+                    elem.replace(",", "").replace(";", "") for elem in line.split()[1:]
+                ]
+
+                current_gate_parameters = line.split()[0].split("(")
+                current_gate_parameters = (
+                    current_gate_parameters[1][:-1].split(",")
+                    if len(current_gate_parameters) > 1
+                    else []
+                )
+
+                all_gate = ""
+                for gate in user_gate_definitions[gate_name][2:]:
+                    all_gate += gate + "\n"
+
+                for i, parameter in enumerate(user_gate_definitions[gate_name][1]):
+                    all_gate = (
+                        all_gate.replace(
+                            "," + parameter + ",", ", " + current_gate_qubits[i] + ","
+                        )
+                        .replace(
+                            " " + parameter + ",", " " + current_gate_qubits[i] + ","
+                        )
+                        .replace(parameter + ";", current_gate_qubits[i] + ";")
+                        .replace(parameter + " ;", current_gate_qubits[i] + " ;")
+                    )
+
+                for i, parameter in enumerate(user_gate_definitions[gate_name][0]):
+                    all_gate = all_gate.replace(parameter, current_gate_parameters[i])
+
+                replaced_code = replaced_code.replace(line + "\n", all_gate)
+
+    return replaced_code
```

### Comparing `mpqp-0.1.dev1/mpqp/tools/choice_tree.py` & `mpqp-0.2.0/mpqp/tools/choice_tree.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,96 @@
+"""This module provides functionalities for working with decision trees, 
+allowing for seamless navigation and interaction within a tree structure.
+
+You can define a :class:`QuestionNode`, containing your question and options.
+Each option (:class:`AnswerNode`) contains the description of the option
+together with optional actions and follow up question.
+
+To run your choice tree, just run :func:`run_choice_tree` on your root question.
+"""
+
 from dataclasses import dataclass
 from typing import Any, Callable, Iterable, Optional, TypeVar
+
 from pick import pick
 from typeguard import typechecked
 
 from mpqp.tools.generics import find
 
 T = TypeVar("T")
 
 
 @dataclass
 class AnswerNode:
-    """Represents a node in a decision tree corresponding to an answer to a question. An answer can lead to an action,
-    or to another question."""
+    """Represents a node in a decision tree corresponding to an answer to a
+    question. An answer can lead to an action, or to another question.
+
+    Args:
+        label: See attribute description.
+        action: See attribute description.
+        next_question: See attribute description.
+    """
 
     label: str
     """The label or text associated with the answer."""
     action: Callable[..., tuple[str, Iterable[Any]]]
-    """A callable representing an action function linked to an answer."""
+    """A callable representing an action function linked to an answer. The
+    return value of the action is composed of the text to display after it ran 
+    (something like "Success", "Failure", or "You're a wonderful human being"),
+    and the parameters to pass to the next action to be executed. These
+    parameters to be passed between actions are useful to keep memory of the
+    previous actions for instance."""
     next_question: Optional["QuestionNode"] = None
     """An optional reference to the next question node."""
 
 
 @dataclass
 class QuestionNode:
-    """Represents a node in a decision tree corresponding to a question."""
+    """Represents a node in a decision tree corresponding to a question.
+
+    Args:
+        label: See attribute description.
+        answers: See attribute description.
+    """
+
     label: str
     """The label or text associated with the question."""
     answers: list[AnswerNode]
     """List of possible answers to this question."""
 
 
 @typechecked
 def run_choice_tree(question: QuestionNode):
-    """
-    Execute the choice tree by starting with the question node in parameter.
+    """Execute the choice tree by starting with the question node in parameter.
 
     Args:
         question: Root question from which the choice tree will start
     """
-    # 3M-TODO: allow exit with Ctrl+C and Q
     prev_args = []
     prev_message = ""
     next_question = question
-    while True:
-        option, _ = pick(
-            list(map(lambda a: a.label, next_question.answers)) + ["Exit"],
-            prev_message + "\n\n" + next_question.label,
-            indicator="=>",
-        )
-        if option == "Exit":
-            return
-        selected_answer = find(next_question.answers, lambda a: a.label == option)
-        prev_message, prev_args = selected_answer.action(*prev_args)
-        next_question = selected_answer.next_question
-        if next_question is None:
-            pick(["Press 'Enter' to continue"], prev_message, indicator="")
-            return
+    try:
+        while True:
+            option, _ = pick(
+                list(map(lambda a: a.label, next_question.answers)) + ["Exit"],
+                prev_message + "\n\n" + next_question.label,
+                indicator="=>",
+            )
+            if option == "Exit":
+                return
+            selected_answer = find(next_question.answers, lambda a: a.label == option)
+            prev_message, prev_args = selected_answer.action(*prev_args)
+            next_question = selected_answer.next_question
+            if next_question is None:
+                pick(["Press 'Enter' to continue"], prev_message, indicator="")
+                return
+
+    except KeyboardInterrupt:
+        print()
+        pass
 
 
 # Example:
 if __name__ == "__main__":
 
     def date_name_picker():
         name = input("What's your name?\n\t")
```

### Comparing `mpqp-0.1.dev1/pytest.ini` & `mpqp-0.2.0/pytest.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 [pytest]
 ; culprits packages added as comments
 filterwarnings = 
     ; pkg_resources
     ignore:Deprecated call to `pkg_resources.declare_namespace.*:DeprecationWarning 
+    ;  a package has a version called 'qp' which does not respect PEP440 
+    ignore:!!\n\n.*:DeprecationWarning 
     ; qat (myqlm)
     ignore:pkg_resources is deprecated as an API.*:DeprecationWarning
     ignore:.*scipy.*:DeprecationWarning
     ignore:.*MessageStream size changed.*:RuntimeWarning
     ; qiskit
     ignore:.*qiskit.opflow.*:DeprecationWarning
     ignore:.*qiskit.utils.algorithm_globals.*:DeprecationWarning
     ignore:.*qiskit.circuit.quantumcircuit.QuantumCircuit.i.*:DeprecationWarning
     ignore:Setting metadata to None.*:DeprecationWarning
     ignore:divide by zero.*:RuntimeWarning
     ignore:The qiskit.extensions module is pending deprecation.*:PendingDeprecationWarning
-    ignore:Building a flow controller with keyword arguments is going to be deprecated.*:PendingDeprecationWarning
+    ignore:Building a flow controller with keyword arguments is going to be deprecated.*:PendingDeprecationWarning
+    ignore:.*OpenQASM language features that m.*
+    ignore:.*OpenQASMTranslationWarning.*
+    ; others
+    ;  pyreadline
+    ignore:Using or importing the ABCs from 'collections'.*:DeprecationWarning
+    ;  backports
+    ignore:Implicit None on return values is deprecated.*:DeprecationWarning
```

### Comparing `mpqp-0.1.dev1/tests/core/instruction/gates/test_controlled_gate.py` & `mpqp-0.2.0/tests/core/instruction/gates/test_controlled_gate.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/tests/core/instruction/gates/test_gate.py` & `mpqp-0.2.0/tests/core/instruction/gates/test_gate.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/tests/core/instruction/gates/test_gate_definition.py` & `mpqp-0.2.0/tests/core/instruction/gates/test_gate_definition.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/tests/core/instruction/gates/test_native_gates.py` & `mpqp-0.2.0/tests/core/instruction/gates/test_native_gates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import pytest
-
 import numpy as np
+import pytest
 from sympy import Expr, symbols
 
 from mpqp.gates import *
-from mpqp.tools.maths import matrix_eq, cos, sin, exp, I, pi
 from mpqp.tools.generics import Matrix
+from mpqp.tools.maths import I, cos, exp, matrix_eq, pi, sin
 
 theta: Expr
 k: Expr
 theta, k = symbols("θ k")  # pyright: ignore[reportAssignmentType]
 c, s, e = cos(theta), sin(theta), exp(1.0 * I * theta)
 c2, s2, e2 = (
     cos(theta / 2),  # pyright: ignore[reportOperatorIssue]
@@ -104,17 +103,17 @@
     assert matrix_eq(Ry(angle, 0).to_matrix(), result_matrix)
 
 
 @pytest.mark.parametrize(
     "angle, result_matrix",
     [
         (0, np.eye(2)),
-        (np.pi, np.diag([-1j] * 2)),
-        (np.pi / 5, np.diag([0.95105652 - 0.30901699j] * 2)),
-        (theta, np.diag([1 / e2] * 2)),  # pyright: ignore
+        (np.pi, np.diag([-1j, 1j])),
+        (np.pi / 5, np.diag([0.95105652 - 0.30901699j, 0.95105652 + 0.30901699j])),
+        (theta, np.diag([1 / e2, e2])),  # pyright: ignore
     ],
 )
 def test_Rz(angle: float, result_matrix: Matrix):
     assert matrix_eq(Rz(angle, 0).to_matrix(), result_matrix)
 
 
 @pytest.mark.parametrize(
```

### Comparing `mpqp-0.1.dev1/tests/core/instruction/measurement/test_basis.py` & `mpqp-0.2.0/tests/core/instruction/measurement/test_basis.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,48 +46,48 @@
     [
         (
             ComputationalBasis,
             3,
             True,
             (
                 "Basis: [\n"
-                "    [1.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 1.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 1.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 0.+0.j 1.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 0.+0.j 0.+0.j 1.+0.j 0.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 1.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 1.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 1.+0.j]\n"
+                "    [1, 0, 0, 0, 0, 0, 0, 0],\n"
+                "    [0, 1, 0, 0, 0, 0, 0, 0],\n"
+                "    [0, 0, 1, 0, 0, 0, 0, 0],\n"
+                "    [0, 0, 0, 1, 0, 0, 0, 0],\n"
+                "    [0, 0, 0, 0, 1, 0, 0, 0],\n"
+                "    [0, 0, 0, 0, 0, 1, 0, 0],\n"
+                "    [0, 0, 0, 0, 0, 0, 1, 0],\n"
+                "    [0, 0, 0, 0, 0, 0, 0, 1]\n"
                 "]\n"
             ),
         ),
         (
             ComputationalBasis,
             2,
             False,
             (
                 "Basis: [\n"
-                "    [1.+0.j 0.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 1.+0.j 0.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 1.+0.j 0.+0.j],\n"
-                "    [0.+0.j 0.+0.j 0.+0.j 1.+0.j]\n"
+                "    [1, 0, 0, 0],\n"
+                "    [0, 1, 0, 0],\n"
+                "    [0, 0, 1, 0],\n"
+                "    [0, 0, 0, 1]\n"
                 "]\n"
             ),
         ),
         (
             HadamardBasis,
             2,
             True,
             (
                 "Basis: [\n"
-                "    [0.5+0.j 0.5+0.j 0.5+0.j 0.5+0.j],\n"
-                "    [ 0.5+0.j -0.5+0.j  0.5+0.j -0.5+0.j],\n"
-                "    [ 0.5+0.j  0.5+0.j -0.5+0.j -0.5+0.j],\n"
-                "    [ 0.5+0.j -0.5+0.j -0.5+0.j  0.5-0.j]\n"
+                "    [0.5, 0.5, 0.5, 0.5],\n"
+                "    [0.5, -0.5, 0.5, -0.5],\n"
+                "    [0.5, 0.5, -0.5, -0.5],\n"
+                "    [0.5, -0.5, -0.5, 0.5]\n"
                 "]\n"
             ),
         ),
     ],
 )
 def test_basis_implementations(
     basis: type[VariableSizeBasis],
```

### Comparing `mpqp-0.1.dev1/tests/core/instruction/measurement/test_basis_measure.py` & `mpqp-0.2.0/tests/core/instruction/measurement/test_basis_measure.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def test_basis_measure_init_fails_duplicate_c_targets():
     with pytest.raises(ValueError, match="Duplicate registers in targets"):
         BasisMeasure(targets=[0, 1], c_targets=[2, 2, 3], shots=1024)
 
 
 def test_basis_measure_to_other_language_not_implemented():
-    measure = BasisMeasure([0], basis=HadamardBasis)
+    measure = BasisMeasure([0], basis=HadamardBasis())
     with pytest.raises(NotImplementedError):
         measure.to_other_language(language=Language.QISKIT)
 
 
 def test_basis_measure_repr():
     measure = BasisMeasure([0, 1], shots=1024)
     representation = repr(measure)
```

### Comparing `mpqp-0.1.dev1/tests/core/instruction/measurement/test_measure.py` & `mpqp-0.2.0/tests/core/instruction/measurement/test_measure.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/tests/core/test_circuit.py` & `mpqp-0.2.0/tests/core/test_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from __future__ import annotations
+
 from typing import Optional, Sequence
 
-import pytest
 import numpy as np
+import pytest
 from qiskit import QuantumCircuit
 from typeguard import TypeCheckError
 
-from mpqp import QCircuit, Instruction, Barrier, Language
-from mpqp.gates import Gate, CNOT, X, Y, Z, CZ, SWAP, T, H, Rx, S, Ry, Rz
+from mpqp import Barrier, Instruction, Language, QCircuit
+from mpqp.gates import CNOT, CZ, SWAP, Gate, H, Rx, Ry, Rz, S, T, X, Y, Z
 from mpqp.measures import BasisMeasure, ExpectationMeasure, Observable
-from mpqp.tools.generics import ListOrSingle, one_lined_repr
-
-# 3M-TODO: a lot of these tests use str to test circuit equivalence, it would be
-# preferable to define a __eq__ in the QCircuit class, or at least an
-# `equivalent` method
+from mpqp.tools.generics import OneOrMany, one_lined_repr
 
 
 @pytest.mark.parametrize(
     "init_param, printed_result_filename",
     [
         (0, "empty"),
         ([], "empty"),
@@ -55,15 +52,15 @@
             [CNOT(0, 1), BasisMeasure([0, 1], shots=100)],
             "list",
         ),
     ],
 )
 def test_add(
     init_circuit: QCircuit,
-    added_gates: ListOrSingle[Instruction],
+    added_gates: OneOrMany[Instruction],
     printed_result_filename: str,
 ):
     with open(
         f"tests/core/test_circuit/add-{printed_result_filename}.txt",
         "r",
         encoding="utf-8",
     ) as f:
```

### Comparing `mpqp-0.1.dev1/tests/example/test_demonstrations.py` & `mpqp-0.2.0/tests/examples/test_demonstrations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,29 @@
+from typing import Any, Callable
+
+import numpy as np
 import pytest
+from braket.devices import LocalSimulator
+
 from mpqp import QCircuit
-from mpqp.core.instruction.measurement import Observable, ExpectationMeasure
-from mpqp.execution.devices import AWSDevice, ATOSDevice, IBMDevice
+from mpqp.core.instruction.measurement import ExpectationMeasure, Observable
+from mpqp.execution import run
+from mpqp.execution.devices import ATOSDevice, AvailableDevice, AWSDevice, IBMDevice
 from mpqp.gates import *
 from mpqp.measures import BasisMeasure
-from mpqp.execution import run
-from braket.devices import LocalSimulator
-import numpy as np
 from mpqp.qasm.qasm_to_braket import qasm3_to_braket_Circuit
+from mpqp.tools.errors import UnsupportedBraketFeaturesWarning
+
+
+def warn_guard(device: AvailableDevice, run: Callable[[], Any]):
+    if isinstance(device, AWSDevice):
+        with pytest.warns(UnsupportedBraketFeaturesWarning):
+            return run()
+    else:
+        return run()
 
 
 def test_sample_demo():
     # Declaration of the circuit with the right size
     circuit = QCircuit(4)
 
     # Constructing the circuit by adding gates
@@ -30,24 +42,26 @@
     circuit.add(CNOT(3, 0))
     circuit.add(Rz(3.14, 0))
 
     # Add measurement
     circuit.add(BasisMeasure([0, 1, 2, 3], shots=2000))
 
     # Run the circuit on a selected device
-    run(
+    runner = lambda: run(
         circuit,
         [
             IBMDevice.AER_SIMULATOR,
             ATOSDevice.MYQLM_PYLINALG,
             ATOSDevice.MYQLM_CLINALG,
             AWSDevice.BRAKET_LOCAL_SIMULATOR,
         ],
     )
 
+    warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
+
     assert True
 
 
 def test_statevector_demo():
     # Declaration of the circuit with the right size
     circuit = QCircuit(4)
 
@@ -64,38 +78,42 @@
     circuit.add(H(3))
     circuit.add(CNOT(1, 2))
     circuit.add(Rx(3.14, 1))
     circuit.add(CNOT(3, 0))
     circuit.add(Rz(3.14, 0))
 
     # when no measure in the circuit, must run in statevector mode
-    run(
+    runner = lambda: run(
         circuit,
         [
             IBMDevice.AER_SIMULATOR_STATEVECTOR,
             ATOSDevice.MYQLM_PYLINALG,
             ATOSDevice.MYQLM_CLINALG,
             AWSDevice.BRAKET_LOCAL_SIMULATOR,
         ],
     )
 
+    warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
+
     # same when we add a BasisMeasure with 0 shots
     circuit.add(BasisMeasure([0, 1, 2, 3], shots=0))
 
     # Run the circuit on a selected device
-    run(
+    runner = lambda: run(
         circuit,
         [
             IBMDevice.AER_SIMULATOR_STATEVECTOR,
             ATOSDevice.MYQLM_PYLINALG,
             ATOSDevice.MYQLM_CLINALG,
             AWSDevice.BRAKET_LOCAL_SIMULATOR,
         ],
     )
 
+    warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
+
     assert True
 
 
 def test_observable_demo():
     obs = Observable(
         np.array(
             [
@@ -117,31 +135,32 @@
 
     # Running the computation on myQLM and on Aer simulator, then retrieving the results
     run(circuit, [ATOSDevice.MYQLM_PYLINALG, IBMDevice.AER_SIMULATOR])
 
     assert True
 
 
-def test_aws_executions():
+def test_aws_qasm_executions():
     device = LocalSimulator()
 
     qasm_str = """OPENQASM 3.0;
     include 'stdgates.inc';
     qubit[2] q;
     bit c;
     h q[0];
     cx q[0],q[1];
     c[0] = measure q[0];
     c[1] = measure q[1];"""
 
-    circuit = qasm3_to_braket_Circuit(qasm_str)
-
+    runner = lambda: qasm3_to_braket_Circuit(qasm_str)
+    circuit = warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
     device.run(circuit, shots=100).result()
 
-    #####################################################
+
+def test_aws_mpqp_executions():
 
     # Declaration of the circuit with the right size
     circuit = QCircuit(4)
 
     # Constructing the circuit by adding gates
     circuit.add(T(0))
     circuit.add(CNOT(0, 1))
@@ -157,15 +176,17 @@
     circuit.add(CNOT(1, 2))
     circuit.add(Rx(3.14, 1))
     circuit.add(CNOT(3, 0))
     circuit.add(Rz(3.14, 0))
     # Add measurement
     circuit.add(BasisMeasure([0, 1, 2, 3], shots=2000))
 
-    run(circuit, AWSDevice.BRAKET_LOCAL_SIMULATOR)
+    runner = lambda: run(circuit, AWSDevice.BRAKET_LOCAL_SIMULATOR)
+
+    warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
 
     #####################################################
 
     obs = Observable(
         np.array(
             [
                 [0.63, 0.5, 1, 1],
@@ -181,25 +202,31 @@
     circuit = QCircuit(2, label="Observable test")
     # Constructing the circuit by adding gates and measurements
     circuit.add(H(0))
     circuit.add(Rx(1.76, 1))
     circuit.add(ExpectationMeasure([0, 1], observable=obs, shots=0))
 
     # Running the computation on myQLM and on Braket simulator, then retrieving the results
-    run(circuit, [AWSDevice.BRAKET_LOCAL_SIMULATOR, ATOSDevice.MYQLM_PYLINALG])
+    runner = lambda: run(
+        circuit, [AWSDevice.BRAKET_LOCAL_SIMULATOR, ATOSDevice.MYQLM_PYLINALG]
+    )
+    warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
 
     #####################################################
 
     # Declaration of the circuit with the right size
     circuit = QCircuit(
         [H(0), Rx(1.76, 1), Ry(1.76, 1), Rz(1.987, 0)], label="StateVector test"
     )
 
     # Running the computation on myQLM and on Aer simulator, then retrieving the results
-    run(circuit, [AWSDevice.BRAKET_LOCAL_SIMULATOR, ATOSDevice.MYQLM_PYLINALG])
+    runner = lambda: run(
+        circuit, [AWSDevice.BRAKET_LOCAL_SIMULATOR, ATOSDevice.MYQLM_PYLINALG]
+    )
+    warn_guard(AWSDevice.BRAKET_LOCAL_SIMULATOR, runner)
 
 
 def test_all_native_gates():
     # Declaration of the circuit with the right size
     circuit = QCircuit(3, label="Test native gates")
     # Constructing the circuit by adding gates and measurements
     circuit.add([H(0), X(1), Y(2), Z(0), S(1), T(0)])
```

### Comparing `mpqp-0.1.dev1/tests/execution/connection/test_ibm_q_connection.py` & `mpqp-0.2.0/tests/execution/connection/test_ibm_q_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,7 +93,9 @@
 #
 # def test_mock_ibm_provider(mock_ibm_provider):
 #     with patch(
 #         "mpqp.execution.connection.ibm_connection.IBMProvider", mock_ibm_provider
 #     ):
 #         with pytest.raises(RequestsApiError, match="401 Client Error: Unauthorized"):
 #             IBMProvider()
+
+# TODO
```

### Comparing `mpqp-0.1.dev1/tests/execution/providers_execution/test_atos_execution.py` & `mpqp-0.2.0/tests/execution/providers/test_atos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""add -l or --long to the cli args to run this test (disabled by default 
-because too slow)"""
+"""Add ``--long`` to the cli args to run this test (disabled by default because 
+too slow)"""
+
+import sys
 
 # 3M-TODO test everything
 import numpy as np
 import pytest
 
-from mpqp.core.instruction.measurement import Observable, ExpectationMeasure
-from mpqp.gates import *
 from mpqp import QCircuit
-from mpqp.measures import BasisMeasure
+from mpqp.core.instruction.measurement import ExpectationMeasure, Observable
 from mpqp.execution import run
 from mpqp.execution.devices import ATOSDevice
-
-import sys
+from mpqp.gates import *
+from mpqp.measures import BasisMeasure
 
 
 @pytest.mark.parametrize(
     "circuit",
     [
         # SAMPLE JOB
         QCircuit(
@@ -65,9 +65,9 @@
         ),
     ],
 )
 def running_remote_QLM_without_error(circuit: QCircuit):
     run(circuit, ATOSDevice.QLM_LINALG)
 
 
-if "-l" in sys.argv or "--long" in sys.argv:
+if "--long" in sys.argv:
     test_running_remote_QLM_without_error = running_remote_QLM_without_error
```

### Comparing `mpqp-0.1.dev1/tests/execution/providers_execution/test_ibm_execution.py` & `mpqp-0.2.0/tests/execution/providers/test_ibm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""Add ``-l`` or ``--long`` to the cli args to run this test (disable by default 
-because too slow)"""
+"""Add ``--long`` to the cli args to run this test (disabled by default because 
+too slow)"""
+
+import sys
 
 # 3M-TODO test everything
 import numpy as np
 import pytest
-from mpqp.core.instruction.measurement import Observable, ExpectationMeasure
-from mpqp.gates import *
+
 from mpqp import QCircuit
-from mpqp.measures import BasisMeasure
+from mpqp.core.instruction.measurement import ExpectationMeasure, Observable
 from mpqp.execution import run
 from mpqp.execution.devices import IBMDevice
-
-import sys
+from mpqp.gates import *
+from mpqp.measures import BasisMeasure
 
 
 @pytest.mark.parametrize(
     "circuit",
     [
         # SAMPLE JOB
         QCircuit(
@@ -50,12 +51,15 @@
                     shots=1000,
                 ),
             ]
         ),
     ],
 )
 def running_remote_IBM_without_error(circuit: QCircuit):
-    run(circuit, IBMDevice.IBMQ_QASM_SIMULATOR)
+    run(circuit, IBMDevice.AER_SIMULATOR)
 
 
-if "-l" in sys.argv or "--long" in sys.argv:
+if "--long" in sys.argv:
+    # in fact this is not slow anymore, because IBM disabled their remote
+    # simulator, so this is a local one. Because of this, this test is not super
+    # useful anymore. TODO: can we do better ?
     test_running_remote_IBM_without_error = running_remote_IBM_without_error
```

### Comparing `mpqp-0.1.dev1/tests/execution/test_runner.py` & `mpqp-0.2.0/tests/execution/test_runner.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/tests/execution/test_vqa.py` & `mpqp-0.2.0/tests/execution/test_vqa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typing import Any
+
 import numpy as np
 import pytest
 from sympy import Expr
 
 from mpqp import QCircuit
 from mpqp.core.instruction.measurement.expectation_value import (
     ExpectationMeasure,
     Observable,
 )
-from mpqp.gates import *
-from mpqp.execution.devices import AWSDevice, AvailableDevice, IBMDevice, ATOSDevice
-from mpqp.execution.vqa import minimize, Optimizer
-from mpqp.execution.vqa.vqa import OptimizableFunc
+from mpqp.execution.devices import ATOSDevice, AvailableDevice, AWSDevice, IBMDevice
 from mpqp.execution.runner import _run_single  # pyright: ignore[reportPrivateUsage]
+from mpqp.execution.vqa import Optimizer, minimize
+from mpqp.execution.vqa.vqa import OptimizableFunc
+from mpqp.gates import *
+from mpqp.tools.errors import UnsupportedBraketFeaturesWarning
 
 # the symbols function is a bit wacky, so some manual type definition is needed here
 theta: Expr = symbols("θ")  # type: ignore
 
 
 def with_local_devices(args: tuple[Any, ...]):
     return (
@@ -37,16 +39,23 @@
                 ]
             ),
             0,
         )
     ),
 )
 def test_optimizer_circuit(circ: QCircuit, minimum: float, device: AvailableDevice):
-    try:
+    def run():
         assert minimize(circ, Optimizer.BFGS, device)[0] - minimum < 0.05
+
+    try:
+        if isinstance(device, AWSDevice):
+            with pytest.warns(UnsupportedBraketFeaturesWarning):
+                run()
+        else:
+            run()
     except (ValueError, NotImplementedError) as err:
         if "not handled" not in str(err):
             raise
 
 
 @pytest.mark.parametrize(
     "eval_f, minimum, device",
```

### Comparing `mpqp-0.1.dev1/tests/qasm/test_open_qasm_2_and_3.py` & `mpqp-0.2.0/tests/qasm/test_open_qasm_2_and_3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from mpqp.qasm import open_qasm_file_conversion_2_to_3, open_qasm_hard_includes
 
 qasm_folder = "tests/qasm/qasm_examples/"
 
 
 def test_qasm_hard_import():
     with_include_fn = qasm_folder + "with_include.qasm"
@@ -27,14 +28,14 @@
     with pytest.raises(RuntimeError) as e:
         open_qasm_file_conversion_2_to_3(
             qasm_folder + "circular_dep1.qasm",
         )
     assert "Circular dependency" in str(e.value)
 
 
-def test_circular_dependency_detection_2():
+def test_circular_dependency_detection_false_positive():
     try:
         open_qasm_file_conversion_2_to_3(
             qasm_folder + "circular_dep_a.qasm",
         )
     except RuntimeError:
         assert False, f"Circular dependency raised while it shouldn't"
```

### Comparing `mpqp-0.1.dev1/tests/qasm/test_qasm_to_myqlm.py` & `mpqp-0.2.0/tests/qasm/test_qasm_to_myqlm.py`

 * *Files identical despite different names*

### Comparing `mpqp-0.1.dev1/tests/qasm/test_qasm_to_qiskit.py` & `mpqp-0.2.0/tests/qasm/test_qasm_to_qiskit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from mpqp.qasm.qasm_to_qiskit import qasm2_to_QuantumCircuit
+from mpqp.qasm.qasm_to_qiskit import qasm2_to_Qiskit_Circuit
 from qiskit import QuantumCircuit
 
 
 @pytest.mark.parametrize(
     "qasm_code, gate_names",
     [
         (
@@ -25,12 +25,12 @@
             [
                 "h",
                 "cx",
             ],
         ),
     ],
 )
-def test_qasm2_to_QuantumCircuit(qasm_code: str, gate_names: list[str]):
-    circ = qasm2_to_QuantumCircuit(qasm_code)
+def test_qasm2_to_Qiskit_Circuit(qasm_code: str, gate_names: list[str]):
+    circ = qasm2_to_Qiskit_Circuit(qasm_code)
     assert isinstance(circ, QuantumCircuit)
     for instr, expected_gate in zip(circ.data, gate_names):
         assert instr.operation.name == expected_gate
```

### Comparing `mpqp-0.1.dev1/tests/tools/test_math.py` & `mpqp-0.2.0/tests/tools/test_math.py`

 * *Files identical despite different names*

