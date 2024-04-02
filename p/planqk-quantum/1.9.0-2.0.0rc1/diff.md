# Comparing `tmp/planqk-quantum-1.9.0.tar.gz` & `tmp/planqk-quantum-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-1.9.0.tar", last modified: Thu Jul  6 17:03:35 2023, max compression
+gzip compressed data, was "planqk-quantum-2.0.0rc1.tar", last modified: Tue Apr  2 16:32:20 2024, max compression
```

## Comparing `planqk-quantum-1.9.0.tar` & `planqk-quantum-2.0.0rc1.tar`

### file list

```diff
@@ -1,32 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/planqk/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/client/client_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/planqk/qiskit/providers/helper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/providers/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/providers/helper/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/planqk/qiskit/providers/helper/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 17:03:35.000000 planqk-quantum-1.9.0/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-06 17:03:35.000000 planqk-quantum-1.9.0/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 17:03:35.000000 planqk-quantum-1.9.0/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-06 17:03:35.000000 planqk-quantum-1.9.0/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 17:03:35.000000 planqk-quantum-1.9.0/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 17:03:35.772210 planqk-quantum-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 17:03:24.000000 planqk-quantum-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/dwave/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/dwave/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/dto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/job_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/planqk_runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcp_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcz_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/runtime_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/setup.py
```

### Comparing `planqk-quantum-1.9.0/LICENSE` & `planqk-quantum-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.9.0/planqk/qiskit/backend.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-from braket.circuits.circuit_helpers import validate_circuit_and_shots
-from qiskit.circuit import Measure
-from qiskit.transpiler import Target, InstructionProperties
-from qiskit_braket_provider.exception import QiskitBraketException
-
-
 import datetime
 from abc import ABC
-from typing import Union, List, Optional, Tuple, Dict
-
-from qiskit.providers import BackendV2, Provider, Options
-from qiskit_braket_provider.providers.adapter import wrap_circuits_in_verbatim_box
+from copy import copy
 
+from qiskit.circuit import Measure
+from qiskit.providers import BackendV2, Provider
+from qiskit.providers.models import QasmBackendConfiguration, GateConfig
+from qiskit.transpiler import Target
 
-from qiskit.circuit import Instruction as QiskitInstruction
-from .client.backend_dtos import ConfigurationDto, TYPE, BackendDto, ConnectivityDto
-from .client.client_dtos import JobDto, INPUT_FORMAT
+from .client.backend_dtos import ConfigurationDto, TYPE, BackendDto, ConnectivityDto, PROVIDER, HARDWARE_PROVIDER
+from .client.job_dtos import JobDto
 from .job import PlanqkJob
-from planqk.qiskit.providers.helper.adapter import _op_to_instruction, convert_qiskit_to_planqk_circuit, transform_to_qasm_3_program
-from .providers.helper.job_input_converter import convert_circuit_to_backend_input
-
-TASK_ID_DIVIDER = ";"
-
-
-# class PlanqkBackend(BackendV2, ABC):
-#     """BraketBackend."""
-#
-#     def __repr__(self):
-#         return f"PlanqkBraketBackend[{self.name}]"
+from .options import OptionsV2
+from .providers.adapter import ProviderAdapterFactory
 
 
 class PlanqkBackend(BackendV2, ABC):
 
     def __init__(  # pylint: disable=too-many-arguments
             self,
             backend_info: BackendDto,
@@ -40,190 +25,214 @@
             online_date: datetime.datetime = None,
             backend_version: str = None,
             **fields,
     ):
         """PlanqkBackend for execution circuits against PlanQK devices.
 
         Example:
-            >>> provider = PlanqkProvider()
-            >>> backend = provider.get_backend("SV1")
-            >>> transpiled_circuit = transpile(input, backend=backend)
-            >>> backend.run(transpiled_circuit, shots=10).result().get_counts()
+            provider = PlanqkProvider()
+            actual = provider.get_backend("azure.ionq.simulator")
+            transpiled_circuit = transpile(input, actual=actual)
+            actual.run(transpiled_circuit, shots=10).result().get_counts()
             {"100": 10, "001": 10}
 
         Args:
-            backend_info: PlanQK backend infos
-            provider: Qiskit provider for this backend
-            name: name of backend
-            description: description of backend
+            backend_info: PlanQK actual infos
+            provider: Qiskit provider for this actual
+            name: name of actual
+            description: description of actual
             online_date: online date
-            backend_version: backend version
+            backend_version: actual version
             **fields: other arguments
         """
+
         super().__init__(
             provider=provider,
             name=name,
             description=description,
             online_date=online_date,
             backend_version=backend_version,
             **fields,
         )
         self._backend_info = backend_info
         self._target = self._planqk_backend_to_target()
+        self._configuration = self._planqk_backend_dto_to_configuration()
+        self._instance = None
 
     def _planqk_backend_to_target(self) -> Target:
-        """Converts properties of a PlanQK backend into Qiskit Target object.
-
-        Args:
-            planqk_backend: PlanQK backend
+        """Converts properties of a PlanQK actual into Qiskit Target object.
 
         Returns:
-            target for Qiskit backend
+            target for Qiskit actual
         """
         # building target
-        target = Target(description=f"Target for PlanQK backend {self.name}")
-
         configuration: ConfigurationDto = self._backend_info.configuration
         qubit_count: int = configuration.qubit_count
-        # gate model devices
-        if self._backend_info.type == TYPE.QPU:
+        target = Target(description=f"Target for PlanQK actual {self.name}", num_qubits=qubit_count)
 
-            connectivity: ConnectivityDto = self._backend_info.configuration.connectivity
-            instructions: List[QiskitInstruction] = []
+        is_simulator = self._backend_info.type == TYPE.SIMULATOR
+        qubits = configuration.qubits
+        connectivity: ConnectivityDto = self._backend_info.configuration.connectivity
+
+        adapter = ProviderAdapterFactory.get_adapter(self._backend_info.provider)
+
+        single_qubit_props = adapter.single_qubit_gate_props(qubits, is_simulator)
+        multi_qubit_props = adapter.multi_qubit_gate_props(qubits, connectivity, is_simulator)
+        gates_names = {gate.name.lower() for gate in configuration.gates}
+        for gate in gates_names:
+            gate = adapter.to_gate(gate, is_simulator)
+
+            if gate is None:
+                continue
+
+            if gate.num_qubits == 1:
+                target.add_instruction(instruction=gate, properties=single_qubit_props)
+            elif gate.num_qubits > 1:
+                target.add_instruction(instruction=gate, properties=multi_qubit_props)
+            elif gate.num_qubits == 0 and single_qubit_props == {None: None}:
+                # For gates without qubit number qargs can not be determined
+                target.add_instruction(instruction=gate, properties={None: None})
+
+        target.add_instruction(Measure(), single_qubit_props)
+
+        non_gate_instructions = set(configuration.instructions).difference(gates_names).difference({'measure'})
+        for non_gate_instruction_name in non_gate_instructions:
+            instruction = adapter.to_non_gate_instruction(non_gate_instruction_name, is_simulator)
+            if instruction is not None:
+                if instruction.has_single_gate_props:
+                    target.add_instruction(instruction, single_qubit_props)
+                else:
+                    target.add_instruction(instruction=instruction, name=non_gate_instruction_name)
 
-            for operation in configuration.gates:
-                instruction = _op_to_instruction(operation.name) #TODO cchek if finction impl
-                if instruction is not None:
-                    # TODO: remove when target will be supporting > 2 qubit gates  # pylint:disable=fixme
-                    if instruction.num_qubits <= 2:
-                        instructions.append(instruction)
-
-            # add measurement instructions
-            target.add_instruction(
-                Measure(), {(i,): None for i in range(qubit_count)}
-            )
+        return target
 
-            for instruction in instructions:
-                instruction_props: Optional[
-                    Dict[
-                        Union[Tuple[int], Tuple[int, int]], Optional[InstructionProperties]
-                    ]
-                ] = {}
-                # adding 1 qubit instructions
-                if instruction.num_qubits == 1:
-                    for i in range(qubit_count):
-                        instruction_props[(i,)] = None
-                # adding 2 qubit instructions
-                elif instruction.num_qubits == 2:
-                    # building coupling map for fully connected device
-                    if connectivity.fully_connected:
-                        for src in range(qubit_count):
-                            for dst in range(qubit_count):
-                                if src != dst:
-                                    instruction_props[(src, dst)] = None
-                                    instruction_props[(dst, src)] = None
-                    # building coupling map for device with connectivity graph
-                    else:
-                        for src, connections in connectivity.graph.items():
-                            for dst in connections:
-                                instruction_props[(int(src), int(dst))] = None
-                # for more than 2 qubits
-                else:
-                    instruction_props = None
-                # TODO other architcture not inoq
-                target.add_instruction(instruction, instruction_props)
-
-        # gate model simulators
-        elif self._backend_info.type == TYPE.SIMULATOR:
-            instructions = []
-
-            for operation in configuration.gates:
-                instruction = _op_to_instruction(operation.name)
-                if instruction is not None:
-                    # TODO: remove when target will be supporting > 2 qubit gates  # pylint:disable=fixme
-                    if instruction.num_qubits <= 2:
-                        instructions.append(instruction)
-
-            # add measurement instructions
-            target.add_instruction(
-                Measure(), {(i,): None for i in range(qubit_count)}
-            )
+    def _planqk_backend_dto_to_configuration(self) -> QasmBackendConfiguration:
+        basis_gates = [self._get_gate_config_from_target(basis_gate.name)
+                       for basis_gate in self._backend_info.configuration.gates if basis_gate.native_gate
+                       and self._get_gate_config_from_target(basis_gate.name) is not None]
+        gates = [self._get_gate_config_from_target(gate.name)
+                 for gate in self._backend_info.configuration.gates if not gate.native_gate
+                 and self._get_gate_config_from_target(gate.name) is not None]
+
+        return QasmBackendConfiguration(
+            backend_name=self.name,
+            backend_version=self.backend_version,
+            n_qubits=self._backend_info.configuration.qubit_count,
+            basis_gates=basis_gates,
+            gates=gates,
+            local=False,
+            simulator=self._backend_info.type == TYPE.SIMULATOR,
+            conditional=False,
+            open_pulse=False,
+            memory=self._backend_info.configuration.memory_result_supported,
+            max_shots=self._backend_info.configuration.shots_range.max,
+            coupling_map=self.coupling_map,
+            supported_instructions=self._target.instructions,
+            max_experiments=self._backend_info.configuration.shots_range.max,  # Only one circuit is supported per job
+            description=self._backend_info.documentation.description,
+            min_shots=self._backend_info.configuration.shots_range.min,
+        )
 
-            for instruction in instructions:
-                simulator_instruction_props: Optional[
-                    Dict[
-                        Union[Tuple[int], Tuple[int, int]],
-                        Optional[InstructionProperties],
-                    ]
-                ] = {}
-                # adding 1 qubit instructions
-                if instruction.num_qubits == 1:
-                    for i in range(qubit_count):
-                        simulator_instruction_props[(i,)] = None
-                # adding 2 qubit instructions
-                elif instruction.num_qubits == 2:
-                    # building coupling map for fully connected device
-                    for src in range(qubit_count):
-                        for dst in range(qubit_count):
-                            if src != dst:
-                                simulator_instruction_props[(src, dst)] = None
-                                simulator_instruction_props[(dst, src)] = None
-                target.add_instruction(instruction, simulator_instruction_props)
-
-        else:
-            raise QiskitBraketException(
-                "Cannot create target from PlanQK backend information."
+    def _get_gate_config_from_target(self, name) -> GateConfig:
+        operations = [operation for operation in self._target.operations
+                      if isinstance(operation.name, str)  # Filters out the IBM conditional instructions having no name
+                      and operation.name.casefold() == name.casefold()]
+        if len(operations) == 1:
+            operation = operations[0]
+            return GateConfig(
+                name=name,
+                parameters=operation.params,
+                qasm_def='',
             )
 
-        return target
-
     @property
     def target(self):
         return self._target
 
     @property
     def max_circuits(self):
         return None
 
+    @property
+    def min_shots(self):
+        return self._backend_info.configuration.shots_range.min
+
+    @property
+    def max_shots(self):
+        return self._backend_info.configuration.shots_range.max
+
     @classmethod
     def _default_options(cls):
-        return Options()
+        return OptionsV2()
 
-    def run(self, circuit, **kwargs):
-        if isinstance(circuit, (list, tuple)):
-            if len(circuit) > 1:
-                raise RuntimeError("Multi-experiment jobs are not supported")
-            circuit = circuit[0]
+    def run(self, circuit, **kwargs) -> PlanqkJob:
+        """Run a circuit on the backend as job.
 
-        shots = kwargs.get('shots', 1)  # TODO externalize - use backen min default
+        Args:
+            circuit (QuantumCircuit): circuit to run. Currently only a single circuit can be executed per job.
+            **kwargs: additional arguments for the execution (see below)
+        Returns:
+            PlanqkJob: The job instance for the circuit that was run.
+        """
+        from planqk.qiskit.providers.job_input_converter import convert_to_backend_input, convert_to_backend_params
 
-        # TODO input params
+        self._validate_provider_for_backend()
 
-        input = convert_circuit_to_backend_input(self._backend_info.configuration.supported_input_formats, circuit)
+        if isinstance(circuit, (list, tuple)):
+            if len(circuit) > 1:
+                raise ValueError("Multi-experiment jobs are not supported")
+            circuit = circuit[0]
 
-        # import qiskit.qasm3 as q3  TODO try in verbatim box
-        # qasm_circuit_ibm = q3.dumps(input)
-        # qasm_circuit_ibm = qasm_circuit_ibm.replace('\ninclude "stdgates.inc";', '')
-        #TODO this is braket backend specific -> move
-        input_params = {'disable_qubit_rewiring': False,
-                        'qubit_count': circuit.num_qubits}  # TODO determine QuBit count in backend
+        # PennyLane-Qiskit Plugin identifies the result based on the circuit name which must be "circ0"
+        circuit.name = "circ0"
+        shots = kwargs.get('shots', self._backend_info.configuration.shots_range.min)
+
+        # add kwargs, if defined as options, to a copy of the options
+        options = copy(self.options)
+        if kwargs:
+            for field in kwargs:
+                if field in options.data:
+                    options[field] = kwargs[field]
+
+        supported_input_formats = self._backend_info.configuration.supported_input_formats
+        backend_input = convert_to_backend_input(supported_input_formats, circuit, self, options)
+        input_params = convert_to_backend_params(self._backend_info.provider, circuit, options)
 
-        job_request = JobDto(self._backend_info.id,
+        job_request = JobDto(backend_id=self._backend_info.id,
                              provider=self._backend_info.provider.name,
-                             input_format=input[0],
-                             input=input[1],
+                             input_format=backend_input[0],
+                             input=backend_input[1],
                              shots=shots,
                              input_params=input_params)
 
         return PlanqkJob(backend=self, job_details=job_request)
 
+    def _validate_provider_for_backend(self):
+        from planqk.qiskit.runtime_provider import PlanqkQiskitRuntimeService
+        if (self._backend_info.hardware_provider == HARDWARE_PROVIDER.IBM
+                and not isinstance(self.provider, PlanqkQiskitRuntimeService)):
+            raise ValueError(f"Jobs for IBM backends must not be created with {self.provider.__class__.__name__}. "
+                             f"Use {PlanqkQiskitRuntimeService.__name__} instead.")
+
     def retrieve_job(self, job_id: str) -> PlanqkJob:
-        """Return a single job submitted to the backend.
+        """Return a single job.
 
         Args:
-            job_id: ID of the job to retrieve.
+            job_id: id of the job to retrieve.
 
         Returns:
-            The job with the given ID.
+            The job with the given id.
         """
+        return PlanqkJob(backend=self, job_id=job_id)
+
+    def configuration(self) -> QasmBackendConfiguration:
+        """Return the actual configuration.
 
-        return PlanqkJob(backend=self, job_id=job_id)
+        Returns:
+            QasmBackendConfiguration: the configuration for the actual.
+        """
+        return self._configuration
+
+    @property
+    def backend_provider(self) -> PROVIDER:
+        """Return the provider offering the quantum backend resource."""
+        return self._backend_info.provider
```

### Comparing `planqk-quantum-1.9.0/planqk/qiskit/client/client_dtos.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/client/job_dtos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,58 @@
-from dataclasses import dataclass, asdict
-from typing import Optional, Dict, Set, Union
 import json
 from enum import Enum
+from typing import Optional, Dict, Set, Union
+
+from pydantic import BaseModel
 
 
 class INPUT_FORMAT(str, Enum):
     OPEN_QASM_V3 = "OPEN_QASM_V3"
     IONQ_CIRCUIT_V1 = "IONQ_CIRCUIT_V1"
+    QISKIT_PRIMITIVE = "QISKIT_PRIMITIVE"
+    QOQO = "QOQO"
 
 
 class JOB_STATUS(str, Enum):
     COMPLETED = "COMPLETED"
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     FAILED = "FAILED"
     CANCELLING = "CANCELLING"
     CANCELLED = "CANCELLED"
 
 
-@dataclass
-class JobDto:
-    backend_id: str
+class JobDto(BaseModel):
     provider: str
     shots: int = 1
+    backend_id: str = None
     id: Optional[str] = None
+    session_id: Optional[str] = None
     input: Optional[Union[str, Dict]] = None
     input_format: Optional[INPUT_FORMAT] = None
     input_params: Optional[Dict] = None
     begin_execution_time: Optional[str] = None
     cancellation_time: Optional[str] = None
     creation_time: Optional[str] = None
     end_execution_time: Optional[str] = None
     error_data: Optional[dict] = None
     metadata: Optional[Dict[str, str]] = None
     name: Optional[str] = None
     status: Optional[JOB_STATUS] = None
     tags: Optional[Set[str]] = None
 
-    #TODO make me extensible
-
     def __post_init__(self):
         if self.error_data is not None and isinstance(self.error_data, str):
             self.error_data = json.loads(self.error_data)
         if self.input_params is not None and isinstance(self.input_params, str):
             self.input_params = json.loads(self.input_params)
 
-    @classmethod
-    def from_dict(cls, data: Dict):
-        return cls(**data)
 
-    def to_dict(self):
-        return asdict(self)
+class RuntimeJobParamsDto(BaseModel):
+    program_id: str
+    image: Optional[str]
+    hgp: Optional[str]
+    log_level: Optional[str]
+    session_id: Optional[str]
+    max_execution_time: Optional[int] = None
+    start_session: Optional[bool] = False
+    session_time: Optional[int] = None
```

### Comparing `planqk-quantum-1.9.0/planqk/qiskit/job.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,93 @@
 from typing import Optional
 
+from planqk.qiskit.client.client import _PlanqkClient
+from planqk.qiskit.client.job_dtos import JobDto
 from qiskit.providers import JobV1, JobStatus, Backend
+from qiskit.qobj import QobjExperimentHeader
 from qiskit.result import Result
 from qiskit.result.models import ExperimentResult, ExperimentResultData
 
-from planqk.qiskit.client.client import _PlanqkClient
-from planqk.qiskit.client.client_dtos import JobDto
-
-
-class ErrorData(object):
-    def __init__(self, code: str, message: str):
-        self.code = code
-        self.message = message
-
-
 JobStatusMap = {
     "CREATED": JobStatus.INITIALIZING,
     "PENDING": JobStatus.QUEUED,
     "RUNNING": JobStatus.RUNNING,
     "COMPLETED": JobStatus.DONE,
     "FAILED": JobStatus.ERROR,
     "CANCELLING": JobStatus.RUNNING,
     "CANCELLED": JobStatus.CANCELLED,
+    "UNKNOWN": JobStatus.INITIALIZING,
 }
 
 
 class PlanqkJob(JobV1):
     version = 1
 
     def __init__(self, backend: Optional[Backend], job_id: Optional[str] = None, job_details: Optional[JobDto] = None):
 
         if job_id is None and job_details is None:
-            raise ValueError("Either 'job_id' or 'job_details' must be provided.")
-        if job_id is not None and job_details is not None:
-            raise ValueError("Only one of 'job_id' or 'job_details' can be provided.")
+            raise ValueError("Either 'job_id', 'job_details' or both must be provided.")
 
         self._result = None
         self._backend = backend
         self._job_details = job_details
 
-        if job_id is not None:
+        if job_id is not None and job_details is None:
             self._job_id = job_id
             self._refresh()
-            # TODO get backend from job details bakcend id
-
-        else:
+        elif job_id is None and job_details is not None:
             self.submit()
+        else:
+            self._job_id = job_id
+            self._job_details = job_details
 
-        job_details_dict = self._job_details.to_dict()
+        job_details_dict = self._job_details.dict()
         super().__init__(backend=backend, job_id=self._job_id, **job_details_dict)
 
     def submit(self):
         """
         Submits the job for execution.
         """
 
         if self._job_details is None:
             raise RuntimeError("Cannot submit job as no job details are set.")
 
-        self._job_id = _PlanqkClient.submit_job(self._job_details)
+        self._job_details = _PlanqkClient.submit_job(self._job_details)
+        self._job_id = self._job_details.id
 
     def result(self) -> Result:
         """
         Return the result of the job.
         """
         if self._result is not None:
             return self._result
 
         if not self.in_final_state():
             self.wait_for_final_state()
 
         status = JobStatusMap[self._job_details.status]
         if not status == JobStatus.DONE:
             raise RuntimeError(
-                f'{"Cannot retrieve results as job execution failed"}'
+                f'{"Cannot retrieve results as job execution did not complete successfully. "}'
                 + f"(status: {self.status}."
                 + f"error: {self.error_data})"
             )
 
-        result_data = _PlanqkClient.get_job_result(self._job_id)
+        result_data = _PlanqkClient.get_job_result(self._job_id, self.backend().backend_provider)
 
         experiment_result = ExperimentResult(
             shots=self._job_details.shots,
             success=True,
             status=status,
             data=ExperimentResultData(
-                counts=result_data.get("counts", {}),
-                memory=result_data.get("memory", []))
+                counts=result_data.get("counts") or {},
+                memory=result_data.get("memory") or []
+            ),
+            # Header required for PennyLane-Qiskit Plugin as it identifies the result based on the circuit name which is always "circ0"
+            header=QobjExperimentHeader(name="circ0")
         )
 
         self._result = Result(
             backend_name=self._backend.name,
             backend_version=self._backend.version,
             job_id=self._job_id,
             qobj_id=0,
@@ -104,25 +101,25 @@
 
     def _refresh(self):
         """
         Refreshes the job details from the server.
         """
         if self.job_id is None:
             raise ValueError("Job Id is not set.")
-        self._job_details = _PlanqkClient.get_job(self._job_id)
+        self._job_details = _PlanqkClient.get_job(self._job_id, self.backend().backend_provider)
 
     def cancel(self):
         """
         Attempt to cancel the job.
         """
-        _PlanqkClient.cancel_job(self._job_id)
+        _PlanqkClient.cancel_job(self._job_id, self.backend().backend_provider)
 
     def status(self) -> JobStatus:
         """
-        Return the status of the job if it has reached the state DONE. If it is still running, it polls for the result.
+        Return the status of the job.
         """
         self._refresh()
         return JobStatusMap[self._job_details.status]
 
     @property
     def id(self):
         """
@@ -131,7 +128,13 @@
         return self._job_id
 
     def to_dict(self) -> dict:
         """
         Return a dictionary representation of the job.
         """
         return {key: value for key, value in vars(self).items() if not key.startswith('_')}
+
+    def queue_position(self):
+        """
+        Return the position of the job in the server queue.
+        """
+        return None
```

### Comparing `planqk-quantum-1.9.0/planqk/qiskit/providers/helper/adapter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_converters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """Util function for provider."""
-import json
 from typing import Callable, Dict, Optional
 
 from braket.circuits import Circuit, Instruction, gates, result_types
 from braket.circuits.compiler_directives import StartVerbatimBox
 from braket.circuits.gates import PulseGate
 from braket.circuits.serialization import QubitReferenceType, OpenQASMSerializationProperties, IRType
-from braket.device_schema import (
-    DeviceCapabilities,
-)
 from braket.ir.openqasm import Program as OpenQASMProgram
-from braket.schema_common import BraketSchemaBase
 from numpy import pi
 from qiskit import QuantumCircuit
 from qiskit.circuit import Instruction as QiskitInstruction
 from qiskit.circuit import Parameter
 from qiskit.circuit.library import (
     CCXGate,
     CPhaseGate,
@@ -75,15 +70,14 @@
     "cswap": "cswap",
     "cp": "cphaseshift",
     "rxx": "xx",
     "ryy": "yy",
     "ecr": "ecr",
 }
 
-
 qiskit_gate_names_to_braket_gates: Dict[str, Callable] = {
     "u1": lambda lam: [gates.Rz(lam)],
     "u2": lambda phi, lam: [gates.Rz(lam), gates.Ry(pi / 2), gates.Rz(phi)],
     "u3": lambda theta, phi, lam: [
         gates.Rz(lam),
         gates.Rx(pi / 2),
         gates.Rz(theta),
@@ -115,15 +109,15 @@
     "cswap": lambda: [gates.CSwap()],
     "rxx": lambda angle: [gates.XX(angle)],
     "ryy": lambda angle: [gates.YY(angle)],
     "ecr": lambda: [gates.ECR()],
 }
 
 # TODP mark add copyright from braket
-qiskit_gate_name_to_planqk_gate_mapping: Dict[str, Optional[QiskitInstruction]] = {
+qiskit_gate_name_to_braket_gate_mapping: Dict[str, Optional[QiskitInstruction]] = {
     "u1": U1Gate(Parameter("theta")),
     "u2": U2Gate(Parameter("theta"), Parameter("lam")),
     "u3": U3Gate(Parameter("theta"), Parameter("phi"), Parameter("lam")),
     "h": HGate(),
     "ccnot": CCXGate(),
     "cnot": CXGate(),
     "cphaseshift": CPhaseGate(Parameter("theta")),
@@ -148,27 +142,14 @@
     "yy": RYYGate(Parameter("theta")),
     "z": ZGate(),
     "zz": RZZGate(Parameter("theta")),
     "ecr": ECRGate(),
 }
 
 
-def _op_to_instruction(operation: str) -> Optional[QiskitInstruction]:
-    """Converts PlanQK operation to Qiskit Instruction.
-
-    Args:
-        operation: operation
-
-    Returns:
-        Circuit Instruction
-    """
-    operation = operation.lower()
-    return qiskit_gate_name_to_planqk_gate_mapping.get(operation, None)
-
-
 # TODO metnion copyrigtht
 def convert_qiskit_to_planqk_circuit(circuit: QuantumCircuit) -> Circuit:
     """Return a PlanQK quantum input (bases on AWS Braket input) from a Qiskit quantum input.
      Args:
             circuit (QuantumCircuit): PlanQK Quantum Cricuit
 
     Returns:
@@ -214,14 +195,57 @@
     Returns:
            Circuit wrapped in verbatim box, comprising the same instructions
            as the original one and with result types preserved.
     """
     return Circuit(circuit.result_types).add_verbatim_box(Circuit(circuit.instructions))
 
 
+def convert_continuous_qubit_indices(connectivity_graph: dict, ) -> dict:
+    """
+    This function was copied from the following source:
+    https://github.com/qiskit-community/qiskit-braket-provider/blob/984101cec132777c2559a41e9fc4f9ef208e391e/qiskit_braket_provider/providers/adapter.py#L306
+
+    Aspen qubit indices are discontinuous (label between x0 and x7, x being
+    the number of the octagon) while the Qiskit transpiler creates and/or
+    handles coupling maps with continuous indices. This function converts the
+    discontinous connectivity graph from Aspen to a continuous one.
+
+    Args:
+        connectivity_graph (dict): connectivity graph from Aspen. For example
+        4 qubit system, the connectivity graph will be:
+            {"0": ["1", "2", "7"], "1": ["0","2","7"], "2": ["0","1","7"],
+            "7": ["0","1","2"]}
+
+    Returns:
+        dict: Connectivity graph with continuous indices. For example for an
+        input connectivity graph with discontinuous indices (qubit 0, 1, 2 and
+        then qubit 7) as shown here:
+            {"0": ["1", "2", "7"], "1": ["0","2","7"], "2": ["0","1","7"],
+            "7": ["0","1","2"]}
+        the qubit index 7 will be mapped to qubit index 3 for the qiskit
+        transpilation step. Thereby the resultant continous qubit indices
+        output will be:
+            {"0": ["1", "2", "3"], "1": ["0","2","3"], "2": ["0","1","3"],
+            "3": ["0","1","2"]}
+    """
+    # Creates list of existing qubit indices which are discontinuous.
+    indices = [int(key) for key in connectivity_graph.keys()]
+    indices.sort()
+    # Creates a list of continuous indices for number of qubits.
+    map_list = list(range(len(indices)))
+    # Creates a dictionary to remap the discountinous indices to continuous.
+    mapper = dict(zip(indices, map_list))
+    # Performs the remapping from the discontinous to the continuous indices.
+    continous_connectivity_graph = {
+        mapper[int(k)]: [mapper[int(v)] for v in val]
+        for k, val in connectivity_graph.items()
+    }
+    return continous_connectivity_graph
+
+
 def transform_to_qasm_3_program(braket_circuit: Circuit,
                                 disable_qubit_rewiring: bool,
                                 inputs: Dict[str, float]) -> str:
     """Transforms a Braket input to a QASM 3 program."""
 
     qubit_reference_type = QubitReferenceType.VIRTUAL
```

### Comparing `planqk-quantum-1.9.0/setup.py` & `planqk-quantum-2.0.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="1.9.0",
-    author='StoneOne AG',
-    author_email='info@stoneone.de',
+    version="2.0.0rc1",
+    author='Anaqor AG',
+    author_email='info@anaqor.io',
     url='https://github.com/planqk/planqk-quantum',
-    description='Python library for the PlanQK Quantum Platform',
+    description='Python SDK for the PlanQK Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
     license='apache-2.0',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
```

