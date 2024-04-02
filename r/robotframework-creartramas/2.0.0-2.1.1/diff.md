# Comparing `tmp/robotframework_creartramas-2.0.0.tar.gz` & `tmp/robotframework_creartramas-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.0.0.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.1.1.tar", max compression
```

## Comparing `robotframework_creartramas-2.0.0.tar` & `robotframework_creartramas-2.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.0.0/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.0.0/LICENSE
--rw-r--r--   0        0        0      670 2024-04-02 10:16:52.099439 robotframework_creartramas-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.0.0/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2123 2024-04-02 10:11:24.189274 robotframework_creartramas-2.0.0/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.1/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.1/LICENSE
+-rw-r--r--   0        0        0      670 2024-03-27 10:02:51.933985 robotframework_creartramas-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.1/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2095 2024-03-27 10:03:25.664168 robotframework_creartramas-2.1.1/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.1/PKG-INFO
```

### Comparing `robotframework_creartramas-2.0.0/docs/README.md` & `robotframework_creartramas-2.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.0.0/LICENSE` & `robotframework_creartramas-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.0.0/pyproject.toml` & `robotframework_creartramas-2.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.0.0"
+version = "2.1.1"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.0.0/TRAMAS/creartramas.py` & `robotframework_creartramas-2.1.1/TRAMAS/creartramas.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,24 @@
         # Devuelve el checksum módulo 256, comprobando que si check > 256 , el cheksum es 256 menos la diferencia que hay entre ambos
         if check >= 256:
             checksum = 256 - (abs(256-check))
         else:
             checksum = abs(256-check)
         return checksum # valor absoluto por si checksum es mayor que 256
         
-    def crear_trama(direccion_destino, numero_bits, direccion_origen, comando, datos):
+    def crear_trama(chek,direccion_destino, numero_bits, direccion_origen, comando, datos):
         """
         Esta funcion construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
         Hay que tener en cuenta que los datos que se introducen deben estar en formate hexadecimal 0XAB.
         También a la hora de introducir datos, estso deben estar en forma de lista datos=[0x00,0x00,..]
         Finalmente, se devuelve la trama creada.
         """
-         # Construye la trama según la estructura proporcionada
-        trama = " ".join([f"{direccion_destino:02X}", f"{numero_bits:02X}", f"{direccion_origen:02X}", f"{comando:02X}"]) 
+        # Construye la trama según la estructura proporcionada
+        trama = f"{direccion_destino:02X} {numero_bits:02X} {direccion_origen:02X} {comando:02X} "
         # Agregar cada elemento de la lista datos a la trama en formato hexadecimal
-        trama +=" " + " ".join([f"{dato:02X}" for dato in datos]) + " "
+        for dato in datos:
+            trama += f"{dato:02X} "
         # Calcula el checksum de la trama
         checksum = calcular_checksum(trama)
         # Agrega el checksum a la trama
         trama += f"{checksum:02X}\n"  # Asegura que el checksum esté representado por dos caracteres hexadecimales
         return trama
```

### Comparing `robotframework_creartramas-2.0.0/PKG-INFO` & `robotframework_creartramas-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.0.0
+Version: 2.1.1
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

