# Comparing `tmp/pyplate-hte-0.3.1.tar.gz` & `tmp/pyplate-hte-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplate-hte-0.3.1.tar", last modified: Thu Mar 14 20:39:54 2024, max compression
+gzip compressed data, was "pyplate-hte-0.4.tar", last modified: Tue Apr  2 16:58:44 2024, max compression
```

## Comparing `pyplate-hte-0.3.1.tar` & `pyplate-hte-0.4.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-03-14 20:39:54.678194 pyplate-hte-0.3.1/
--rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-01-28 17:38:34.000000 pyplate-hte-0.3.1/LICENSE.txt
--rw-r--r--   0 marvinj    (502) staff       (20)    14954 2024-03-14 20:39:54.676796 pyplate-hte-0.3.1/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)     2139 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/README.md
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-03-14 20:39:54.642004 pyplate-hte-0.3.1/pyplate/
--rw-r--r--   0 marvinj    (502) staff       (20)     1633 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/pyplate/__init__.py
--rw-r--r--   0 marvinj    (502) staff       (20)    13085 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/pyplate/experiment_design.py
--rw-r--r--   0 marvinj    (502) staff       (20)   103267 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/pyplate/pyplate.py
--rw-r--r--   0 marvinj    (502) staff       (20)    14316 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/pyplate/slicer.py
--rw-r--r--   0 marvinj    (502) staff       (20)    11981 2023-12-15 17:29:48.000000 pyplate-hte-0.3.1/pyplate/slicer_bak.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-03-14 20:39:54.675437 pyplate-hte-0.3.1/pyplate_hte.egg-info/
--rw-r--r--   0 marvinj    (502) staff       (20)    14954 2024-03-14 20:39:54.000000 pyplate-hte-0.3.1/pyplate_hte.egg-info/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)      731 2024-03-14 20:39:54.000000 pyplate-hte-0.3.1/pyplate_hte.egg-info/SOURCES.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-03-14 20:39:54.000000 pyplate-hte-0.3.1/pyplate_hte.egg-info/dependency_links.txt
--rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-03-14 20:39:54.000000 pyplate-hte-0.3.1/pyplate_hte.egg-info/requires.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-03-14 20:39:54.000000 pyplate-hte-0.3.1/pyplate_hte.egg-info/top_level.txt
--rw-r--r--   0 marvinj    (502) staff       (20)      690 2024-03-14 20:39:43.000000 pyplate-hte-0.3.1/pyproject.toml
--rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-03-14 20:39:54.678402 pyplate-hte-0.3.1/setup.cfg
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-03-14 20:39:54.674023 pyplate-hte-0.3.1/tests/
--rw-r--r--   0 marvinj    (502) staff       (20)    10643 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/tests/test_Container.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1975 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_Experiment.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6029 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_ExperimentalSpace.py
--rw-r--r--   0 marvinj    (502) staff       (20)      987 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_Factor.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5193 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/tests/test_Plate.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6666 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/tests/test_Recipe.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_Slicer.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3477 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/tests/test_Substance.py
--rw-r--r--   0 marvinj    (502) staff       (20)     2827 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_convert.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3702 2024-03-14 20:33:06.000000 pyplate-hte-0.3.1/tests/test_create_solution.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1340 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_dilute.py
--rw-r--r--   0 marvinj    (502) staff       (20)      927 2024-02-05 17:19:38.000000 pyplate-hte-0.3.1/tests/test_eugene.py
--rw-r--r--   0 marvinj    (502) staff       (20)    24056 2024-03-14 20:33:07.000000 pyplate-hte-0.3.1/tests/test_recipe_amount_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)    10202 2024-03-14 20:33:07.000000 pyplate-hte-0.3.1/tests/test_recipe_volume_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5701 2024-03-13 22:47:19.000000 pyplate-hte-0.3.1/tests/test_transfers.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1149 2024-03-08 21:34:49.000000 pyplate-hte-0.3.1/tests/test_volume_used_Plate_transfer.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.520273 pyplate-hte-0.4/
+-rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-02-29 20:48:18.000000 pyplate-hte-0.4/LICENSE.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)    15332 2024-04-02 16:58:44.518910 pyplate-hte-0.4/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)     2582 2024-04-02 16:53:28.000000 pyplate-hte-0.4/README.md
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.429279 pyplate-hte-0.4/pyplate/
+-rw-r--r--   0 marvinj    (502) staff       (20)     1531 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyplate/__init__.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    13085 2024-02-29 20:48:18.000000 pyplate-hte-0.4/pyplate/experiment_design.py
+-rw-r--r--   0 marvinj    (502) staff       (20)   105779 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyplate/pyplate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      815 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyplate/pyplate.yaml
+-rw-r--r--   0 marvinj    (502) staff       (20)    14316 2024-02-29 20:48:18.000000 pyplate-hte-0.4/pyplate/slicer.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.517501 pyplate-hte-0.4/pyplate_hte.egg-info/
+-rw-r--r--   0 marvinj    (502) staff       (20)    15332 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)      668 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/SOURCES.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/dependency_links.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/requires.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/top_level.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)      687 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyproject.toml
+-rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-04-02 16:58:44.520513 pyplate-hte-0.4/setup.cfg
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.515740 pyplate-hte-0.4/tests/
+-rw-r--r--   0 marvinj    (502) staff       (20)    10643 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Container.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1975 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_Experiment.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6029 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_ExperimentalSpace.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      987 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_Factor.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5193 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Plate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6666 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Recipe.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_Slicer.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3477 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Substance.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     2827 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_convert.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3702 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_create_solution.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1340 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_dilute.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    24056 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_recipe_amount_used.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    10202 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_recipe_volume_used.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5701 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_transfers.py
```

### Comparing `pyplate-hte-0.3.1/LICENSE.txt` & `pyplate-hte-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/PKG-INFO` & `pyplate-hte-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.3.1
+Version: 0.4
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -192,24 +192,27 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Repository, https://github.com/ekwan/PyPlate
-Project-URL: Documentation, https://pyplate-hte.readthedocs.io
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 
 # PyPlate
 
+[![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
+[![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
+
 An open-source Python tool for high-throughput chemistry.
 
 ### Introduction
 
 PyPlate provides tools for the design and implementation of high-throughput chemistry experiments (in particular, reaction screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
 
 ### Installation
@@ -252,11 +255,13 @@
 
 recipe.visualize(what=plate, mode='final', unit='uL', timeframe=0)
 
 ```
 
 ![img.png](images/simple_visualization.png)
 
+Documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).
+
 ## License
 
 Licensed under the Apache License, Version 2.0 (the "License")
 You may obtain a copy of the License at https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyplate-hte-0.3.1/README.md` & `pyplate-hte-0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # PyPlate
 
+[![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
+[![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
+
 An open-source Python tool for high-throughput chemistry.
 
 ### Introduction
 
 PyPlate provides tools for the design and implementation of high-throughput chemistry experiments (in particular, reaction screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
 
 ### Installation
@@ -46,11 +50,13 @@
 
 recipe.visualize(what=plate, mode='final', unit='uL', timeframe=0)
 
 ```
 
 ![img.png](images/simple_visualization.png)
 
+Documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).
+
 ## License
 
 Licensed under the Apache License, Version 2.0 (the "License")
 You may obtain a copy of the License at https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyplate-hte-0.3.1/pyplate/__init__.py` & `pyplate-hte-0.4/pyplate/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from pathlib import Path
 import os
 import yaml
 
-
 # import pyplate
 
+
 class Config:
     def __init__(self):
         file_path = None
-        environ_path = Path(os.environ.get('PYPLATE_CONFIG', ''))
-        if environ_path.is_dir():
-            environ_path.joinpath("pyplate.yaml")
-        for path in [environ_path, Path("pyplate.yaml"), Path("../pyplate.yaml"), Path.home() / "pyplate.yaml"]:
+        for path in [Path(os.environ.get('PYPLATE_CONFIG', '')), Path.home(), Path(os.path.dirname(__file__))]:
+            path = path.joinpath('pyplate.yaml')
             if path.is_file():
                 file_path = path
                 break
 
         if file_path is None:
             raise RuntimeError("pyplate.yaml not found.")
```

### Comparing `pyplate-hte-0.3.1/pyplate/experiment_design.py` & `pyplate-hte-0.4/pyplate/experiment_design.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/pyplate/pyplate.py` & `pyplate-hte-0.4/pyplate/pyplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -654,25 +654,28 @@
                 substance, quantity = entry
                 if not isinstance(substance, Substance) or not isinstance(quantity, str):
                     raise TypeError("Element in initial_contents must be a (Substance, str) tuple.")
                 self._self_add(substance, quantity)
             contents = []
             for substance, quantity in self.contents.items():
                 quantity, unit = Unit.convert_from_storage_to_standard_format(substance, quantity)
-                contents.append(f"{quantity} {unit} of {substance.name}")
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                contents.append(f"{round(quantity, precision)} {unit} of {substance.name}")
             self.instructions = f"Add {', '.join(contents)}"
             if self.max_volume != float('inf'):
                 max_volume, unit = Unit.convert_from_storage_to_standard_format(self, self.max_volume)
-                self.instructions += f" to a {max_volume} {unit} container."
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                self.instructions += f" to a {round(max_volume, precision)} {unit} container."
             else:
                 self.instructions += " to a container."
         else:
             if self.max_volume != float('inf'):
                 max_volume, unit = Unit.convert_from_storage_to_standard_format(self, self.max_volume)
-                self.instructions = f"Create a {max_volume} {unit} container."
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                self.instructions = f"Create a {round(max_volume, precision)} {unit} container."
             else:
                 self.instructions = "Create a container."
 
     def __eq__(self, other):
         if not isinstance(other, Container):
             return False
         return self.name == other.name and self.contents == other.contents and \
@@ -761,16 +764,16 @@
             transfer = Unit.convert_from_storage(ratio * source_container.volume, 'L')
             transfer, unit = Unit.get_human_readable_unit(transfer, 'L')
         else:
             # total mass in source container times ratio
             mass = sum(Unit.convert(substance, f"{amount} {config.moles_prefix if not substance.is_enzyme() else 'U'}",
                                     "mg") for substance, amount in source_container.contents.items())
             transfer, unit = Unit.get_human_readable_unit(mass * ratio, 'mg')
-
-        to.instructions += f"\nTransfer {transfer} {unit} of {source_container.name} to {to.name}"
+        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+        to.instructions += f"\nTransfer {round(transfer, precision)} {unit} of {source_container.name} to {to.name}"
         to.volume = round(sum(Unit.convert(substance, f"{amount} {config.moles_prefix}", config.volume_prefix) for
                               substance, amount in to.contents.items()), config.internal_precision)
         if to.volume > to.max_volume:
             raise ValueError(f"Exceeded maximum volume in {to.name}.")
         source_container.volume = sum(Unit.convert(substance, f"{amount} {config.moles_prefix}", config.volume_prefix)
                                       for substance, amount in source_container.contents.items())
         source_container.volume = round(source_container.volume, config.internal_precision)
@@ -989,15 +992,16 @@
             concentration = Unit.calculate_concentration_ratio(solute, kwargs['concentration'], solvent)
             quantity = Unit.convert(solute, kwargs['quantity'], concentration[1])
             result = Container(name, initial_contents=[(solute, kwargs['quantity'])])
             result._self_add(solvent, f"{quantity / concentration[0]} {concentration[1]}")
         contents = []
         for substance, value in result.contents.items():
             value, unit = Unit.convert_from_storage_to_standard_format(substance, value)
-            contents.append(f"{value} {unit} of {substance.name}")
+            precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+            contents.append(f"{round(value, precision)} {unit} of {substance.name}")
         result.instructions = "Add " + ", ".join(contents) + " to a container."
         return result
 
     @staticmethod
     def create_solution_from(source: Container, solute: Substance, concentration: str, solvent: Substance,
                              quantity: str, name=None) -> Tuple[Container, Container]:
         # TODO: consider case of different solvent
@@ -1059,17 +1063,22 @@
 
         residual, solution = Container.transfer(source, solution, f"{source.volume * ratio} {config.volume_prefix}")
         solution = solution.fill_to(solvent, quantity)
 
         contents = [(*Unit.convert_from_storage_to_standard_format(solution, solution.volume), source.name),
                     (*Unit.convert_from_storage_to_standard_format(solvent, solution.contents[solvent]), solvent.name)]
         max_volume, unit = Unit.convert_from_storage_to_standard_format(solution, solution.max_volume)
+        sub_instructions = []
+        for value, sub_unit, substance in contents:
+            precision = config.precisions[sub_unit] if sub_unit in config.precisions else config.precisions['default']
+            sub_instructions.append(f"{round(value, precision)} {sub_unit} of {substance}")
+        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
         solution.instructions = ("Add "
-                                 + ", ".join(f"{value} {unit} of {substance}" for value, unit, substance in contents)
-                                 + f" to a {max_volume} {unit} container.")
+                                 + ", ".join(sub_instructions)
+                                 + f" to a {round(max_volume, precision)} {unit} container.")
 
         return residual, solution.fill_to(solvent, quantity)
 
     def remove(self, what: (Substance | int) = Substance.LIQUID) -> Container:
         """
         Removes substances from `Container`
 
@@ -1149,15 +1158,16 @@
             destination = deepcopy(self)
             destination.name = name
         else:
             destination = self
         needed_umoles = f"{required_umoles} umol"
         result = destination._add(solvent, needed_umoles)
         needed_volume, unit = Unit.get_human_readable_unit(Unit.convert(solvent, needed_umoles, 'umol'), 'L')
-        result.instructions += f"Dilute with {needed_volume} {unit} of {solvent.name}."
+        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+        result.instructions += f"Dilute with {round(needed_volume, precision)} {unit} of {solvent.name}."
         return result
 
     def fill_to(self, solvent: Substance, quantity: str) -> Container:
         """
         Fills container with `solvent` up to `quantity`.
 
         Args:
@@ -1181,15 +1191,16 @@
         current_quantity = sum(Unit.convert(substance, f"{value} {config.moles_prefix}", quantity_unit)
                                for substance, value in self.contents.items() if not substance.is_enzyme())
 
         required_quantity = quantity - current_quantity
         result = self._add(solvent, f"{required_quantity} {quantity_unit}")
         required_volume = Unit.convert(solvent, f"{required_quantity} {quantity_unit}", 'L')
         required_volume, unit = Unit.get_human_readable_unit(required_volume, 'L')
-        result.instructions += f"Fill with {required_volume} {unit} of {solvent.name}."
+        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+        result.instructions += f"Fill with {round(required_volume, precision)} {unit} of {solvent.name}."
         return result
 
 
 class Plate:
     """
     A spatially ordered collection of Containers, like a 96 well plate.
     The spatial arrangement must be rectangular. Immutable.
@@ -1761,15 +1772,15 @@
                 source = step.frm[0]
                 source_name = source.plate.name if isinstance(source, PlateSlicer) else source.name
                 dest = step.to[0]
                 dest_name = dest.plate.name if isinstance(dest, PlateSlicer) else dest.name
                 quantity, = step.operands
 
                 step.instructions = f"""Transfer {quantity} from {str(source) if isinstance(source, PlateSlicer) else
-                source_name} to {dest_name}."""
+                source_name} to {str(dest) if isinstance(dest, PlateSlicer) else dest_name}."""
 
                 self.used.add(source_name)
                 self.used.add(dest_name)
 
                 # containers and such can change while baking the recipe
                 if isinstance(source, PlateSlicer):
                     source = deepcopy(source)
@@ -1867,26 +1878,36 @@
             elif operator == 'dilute':
                 dest = step.to[0]
                 dest_name = dest.name
                 solute, concentration, solvent, new_name = step.operands
                 step.frm.append(None)
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
-                step.instructions = f"Dilute {solute.name} in {dest_name} to {concentration} with {solvent.name}."
                 self.results[dest_name] = self.results[dest_name].dilute(solute, concentration, solvent, new_name)
+                amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
+                amount_added = Unit.convert_from(solvent, amount_added, config.moles_prefix, 'L')
+                amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                step.instructions = (f"Dilute {solute.name} in {dest_name} to {concentration}" +
+                                     f" by adding {round(amount_added, precision)} {unit} of {solvent.name}.")
                 step.substances_used.add(solvent)
                 step.to.append(self.results[dest_name])
             elif operator == 'fill_to':
                 dest = step.to[0]
                 dest_name = dest.plate.name if isinstance(dest, PlateSlicer) else dest.name
                 solvent, quantity = step.operands
                 step.frm.append(None)
                 step.to[0] = self.results[dest_name]
-                step.instructions = f"Fill {dest.name} with {solvent.name} up to {quantity}."
                 self.used.add(dest_name)
+                amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
+                amount_added = Unit.convert_from(solvent, amount_added, config.moles_prefix, 'L')
+                amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                step.instructions = (f"Fill {dest.name} with {solvent.name} up to {quantity}"
+                                     f" by adding {round(amount_added, precision)} {unit}.")
 
                 if isinstance(dest, PlateSlicer):
                     dest = deepcopy(dest)
                     dest.plate = self.results[dest_name]
                 else:
                     dest = self.results[dest_name]
 
@@ -2057,14 +2078,18 @@
             else:
                 substance_unit = 'U' if substance.is_enzyme() else config.moles_prefix
                 return Unit.convert_from(substance, elem.contents.get(substance, 0), substance_unit, unit)
 
         if isinstance(timeframe, str):
             start_index = self.stages[timeframe].start
             end_index = self.stages[timeframe].stop
+            if start_index is None:
+                start_index = 0
+            if end_index is None:
+                end_index = len(self.steps)
         else:
             if timeframe >= len(self.steps):
                 raise ValueError("Invalid step number.")
             if timeframe < 0:
                 timeframe = max(0, len(self.steps) + timeframe)
             start_index = timeframe
             end_index = timeframe + 1
@@ -2103,14 +2128,15 @@
             if what.name == self.steps[end].frm[1].name:
                 data = self.steps[end].frm[1][:].get_dataframe()
             elif what.name == self.steps[end].to[1].name:
                 data = self.steps[end].to[1][:].get_dataframe()
             df = data.applymap(numpy.vectorize(helper, cache=True, otypes='d'))
 
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+        df = df.round(precision)
         vmin, vmax = df.min().min(), df.max().max()
         styler = df.style.format(precision=precision).background_gradient(cmap, vmin=vmin, vmax=vmax)
         return styler
 
 
 class PlateSlicer(Slicer):
     """ @private """
@@ -2310,43 +2336,44 @@
         Returns:
             numpy.ndarray of volumes for each well in uL
 
         """
         if unit is None:
             unit = config.default_volume_unit
 
+        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+
         if substance is None:
             return numpy.vectorize(lambda elem: Unit.convert_from_storage(elem.volume, unit), cache=True,
-                                   otypes='d')(self.get())
+                                   otypes='d')(self.get()).round(precision)
 
         if isinstance(substance, Substance):
             substance = [substance]
 
         if not (substance is None or
                 (isinstance(substance, Iterable) and all(isinstance(x, Substance) for x in substance))):
             raise TypeError("Substance must be a Substance or an Iterable of Substances.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
-        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
 
         def helper(elem):
             amount = 0
             """ Returns volume of elem. """
             if substance is None:
                 for subs, quantity in elem.contents.items():
                     substance_unit = 'U' if subs.is_enzyme() else config.moles_prefix
                     amount += Unit.convert_from(subs, quantity, substance_unit, unit)
             else:
                 for subs in substance:
                     substance_unit = 'U' if subs.is_enzyme() else config.moles_prefix
                     amount += Unit.convert_from(subs, elem.contents.get(subs, 0), substance_unit, unit)
-            return round(amount, precision)
+            return amount
 
-        return numpy.vectorize(helper, cache=True, otypes='d')(self.get())
+        return numpy.vectorize(helper, cache=True, otypes='d')(self.get()).round(precision)
 
     def substances(self) -> set[Substance]:
         """
 
         Returns: A set of substances present in the plate.
 
         """
@@ -2375,17 +2402,17 @@
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
 
         def helper(elem):
             amount = 0
             for subs in substance:
                 if not subs.is_enzyme():
                     amount += Unit.convert_from(subs, elem.contents.get(subs, 0), config.moles_prefix, unit)
-            return round(amount, precision)
+            return amount
 
-        return numpy.vectorize(helper, cache=True, otypes='d')(self.get())
+        return numpy.vectorize(helper, cache=True, otypes='d')(self.get()).round(precision)
 
     def remove(self, what: (Substance | int) = Substance.LIQUID):
         """
         Removes substances from slice
 
         Arguments:
             what: What to remove. Can be a type of substance or a specific substance. Defaults to LIQUID.
```

### Comparing `pyplate-hte-0.3.1/pyplate/slicer.py` & `pyplate-hte-0.4/pyplate/slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/pyplate_hte.egg-info/PKG-INFO` & `pyplate-hte-0.4/pyplate_hte.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.3.1
+Version: 0.4
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -192,24 +192,27 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Repository, https://github.com/ekwan/PyPlate
-Project-URL: Documentation, https://pyplate-hte.readthedocs.io
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 
 # PyPlate
 
+[![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
+[![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
+
 An open-source Python tool for high-throughput chemistry.
 
 ### Introduction
 
 PyPlate provides tools for the design and implementation of high-throughput chemistry experiments (in particular, reaction screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
 
 ### Installation
@@ -252,11 +255,13 @@
 
 recipe.visualize(what=plate, mode='final', unit='uL', timeframe=0)
 
 ```
 
 ![img.png](images/simple_visualization.png)
 
+Documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).
+
 ## License
 
 Licensed under the Apache License, Version 2.0 (the "License")
 You may obtain a copy of the License at https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyplate-hte-0.3.1/pyplate_hte.egg-info/SOURCES.txt` & `pyplate-hte-0.4/pyplate_hte.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 pyplate/__init__.py
 pyplate/experiment_design.py
 pyplate/pyplate.py
+pyplate/pyplate.yaml
 pyplate/slicer.py
-pyplate/slicer_bak.py
 pyplate_hte.egg-info/PKG-INFO
 pyplate_hte.egg-info/SOURCES.txt
 pyplate_hte.egg-info/dependency_links.txt
 pyplate_hte.egg-info/requires.txt
 pyplate_hte.egg-info/top_level.txt
 tests/test_Container.py
 tests/test_Experiment.py
@@ -18,12 +18,10 @@
 tests/test_Plate.py
 tests/test_Recipe.py
 tests/test_Slicer.py
 tests/test_Substance.py
 tests/test_convert.py
 tests/test_create_solution.py
 tests/test_dilute.py
-tests/test_eugene.py
 tests/test_recipe_amount_used.py
 tests/test_recipe_volume_used.py
-tests/test_transfers.py
-tests/test_volume_used_Plate_transfer.py
+tests/test_transfers.py
```

### Comparing `pyplate-hte-0.3.1/pyproject.toml` & `pyplate-hte-0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplate-hte"
-version = "0.3.1"
+version = "0.4"
 description = "A Python tool for designing chemistry experiments in plate format"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Eugene Kwan and James Marvin"},
     {email = "ekwan16@gmail.com"}
 ]
@@ -23,8 +23,10 @@
 
 
 [tool.setuptools]
 packages = ["pyplate"]
 
 [project.urls]
 Repository = "https://github.com/ekwan/PyPlate"
-Documentation = "https://pyplate-hte.readthedocs.io"
+
+[tool.setuptools.package-data]
+pyplate = ["*.yaml"]
```

### Comparing `pyplate-hte-0.3.1/tests/test_Container.py` & `pyplate-hte-0.4/tests/test_Container.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_Experiment.py` & `pyplate-hte-0.4/tests/test_Experiment.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_ExperimentalSpace.py` & `pyplate-hte-0.4/tests/test_ExperimentalSpace.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_Factor.py` & `pyplate-hte-0.4/tests/test_Factor.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_Plate.py` & `pyplate-hte-0.4/tests/test_Plate.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_Recipe.py` & `pyplate-hte-0.4/tests/test_Recipe.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_Slicer.py` & `pyplate-hte-0.4/tests/test_Slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_Substance.py` & `pyplate-hte-0.4/tests/test_Substance.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_convert.py` & `pyplate-hte-0.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_create_solution.py` & `pyplate-hte-0.4/tests/test_create_solution.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_dilute.py` & `pyplate-hte-0.4/tests/test_dilute.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_recipe_amount_used.py` & `pyplate-hte-0.4/tests/test_recipe_amount_used.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_recipe_volume_used.py` & `pyplate-hte-0.4/tests/test_recipe_volume_used.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.3.1/tests/test_transfers.py` & `pyplate-hte-0.4/tests/test_transfers.py`

 * *Files identical despite different names*

