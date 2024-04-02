# Comparing `tmp/robotframework_creartramas-2.1.1.tar.gz` & `tmp/robotframework_creartramas-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.1.1.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.2.1.tar", max compression
```

## Comparing `robotframework_creartramas-2.1.1.tar` & `robotframework_creartramas-2.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.1/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.1/LICENSE
--rw-r--r--   0        0        0      670 2024-03-27 10:02:51.933985 robotframework_creartramas-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.1/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2095 2024-03-27 10:03:25.664168 robotframework_creartramas-2.1.1/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.2.1/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.2.1/LICENSE
+-rw-r--r--   0        0        0      670 2024-04-02 07:26:47.128801 robotframework_creartramas-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.2.1/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2128 2024-04-02 07:22:03.522637 robotframework_creartramas-2.2.1/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.2.1/PKG-INFO
```

### Comparing `robotframework_creartramas-2.1.1/docs/README.md` & `robotframework_creartramas-2.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.1/LICENSE` & `robotframework_creartramas-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.1/pyproject.toml` & `robotframework_creartramas-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.1.1"
+version = "2.2.1"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.1.1/TRAMAS/creartramas.py` & `robotframework_creartramas-2.2.1/TRAMAS/creartramas.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,17 +24,16 @@
     def crear_trama(chek,direccion_destino, numero_bits, direccion_origen, comando, datos):
         """
         Esta funcion construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
         Hay que tener en cuenta que los datos que se introducen deben estar en formate hexadecimal 0XAB.
         También a la hora de introducir datos, estso deben estar en forma de lista datos=[0x00,0x00,..]
         Finalmente, se devuelve la trama creada.
         """
-        # Construye la trama según la estructura proporcionada
-        trama = f"{direccion_destino:02X} {numero_bits:02X} {direccion_origen:02X} {comando:02X} "
+         # Construye la trama según la estructura proporcionada
+        trama = " ".join([f"{direccion_destino:02X}", f"{numero_bits:02X}", f"{direccion_origen:02X}", f"{comando:02X}"]) 
         # Agregar cada elemento de la lista datos a la trama en formato hexadecimal
-        for dato in datos:
-            trama += f"{dato:02X} "
+        trama +=" " + " ".join([f"{dato:02X}" for dato in datos]) + " "
         # Calcula el checksum de la trama
         checksum = calcular_checksum(trama)
         # Agrega el checksum a la trama
         trama += f"{checksum:02X}\n"  # Asegura que el checksum esté representado por dos caracteres hexadecimales
         return trama
```

### Comparing `robotframework_creartramas-2.1.1/PKG-INFO` & `robotframework_creartramas-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.1.1
+Version: 2.2.1
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

