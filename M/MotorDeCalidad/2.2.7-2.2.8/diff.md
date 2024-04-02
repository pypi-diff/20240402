# Comparing `tmp/MotorDeCalidad-2.2.7.tar.gz` & `tmp/MotorDeCalidad-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MotorDeCalidad-2.2.7.tar", last modified: Mon Jan  8 19:18:28 2024, max compression
+gzip compressed data, was "MotorDeCalidad-2.2.8.tar", last modified: Thu Jan 25 14:15:43 2024, max compression
```

## Comparing `MotorDeCalidad-2.2.7.tar` & `MotorDeCalidad-2.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 19:18:28.445862 MotorDeCalidad-2.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 19:18:28.445862 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-08 19:18:28.000000 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-08 19:18:28.000000 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 19:18:28.000000 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 19:18:28.000000 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-08 19:18:28.000000 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-08 19:18:28.000000 MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-08 19:18:28.445862 MotorDeCalidad-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 19:18:28.445862 MotorDeCalidad-2.2.7/motordecalidad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/motordecalidad/_init_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/motordecalidad/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/motordecalidad/field.py
--rw-r--r--   0 runner    (1001) docker     (127)    46657 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/motordecalidad/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27399 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/motordecalidad/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/motordecalidad/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 19:18:28.445862 MotorDeCalidad-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 19:18:28.445862 MotorDeCalidad-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-01-08 19:18:11.000000 MotorDeCalidad-2.2.7/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:15:43.204079 MotorDeCalidad-2.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:15:43.204079 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-25 14:15:43.000000 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-25 14:15:43.000000 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 14:15:43.000000 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 14:15:42.000000 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-25 14:15:43.000000 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-25 14:15:43.000000 MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-25 14:15:43.204079 MotorDeCalidad-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:15:43.200079 MotorDeCalidad-2.2.8/motordecalidad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/motordecalidad/_init_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/motordecalidad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/motordecalidad/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46354 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/motordecalidad/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27399 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/motordecalidad/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/motordecalidad/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 14:15:43.204079 MotorDeCalidad-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:15:43.200079 MotorDeCalidad-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-01-25 14:15:18.000000 MotorDeCalidad-2.2.8/tests/test_utilities.py
```

### Comparing `MotorDeCalidad-2.2.7/MotorDeCalidad.egg-info/PKG-INFO` & `MotorDeCalidad-2.2.8/MotorDeCalidad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MotorDeCalidad
-Version: 2.2.7
+Version: 2.2.8
 Summary: Paquete demo de Motor de Calidad
 Author: Enzo Ipanaque
 Author-email: enzo.ipanaque@ms-peru.com
 License: Management Solutions
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: typing-extensions==4.5.0
```

### Comparing `MotorDeCalidad-2.2.7/PKG-INFO` & `MotorDeCalidad-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MotorDeCalidad
-Version: 2.2.7
+Version: 2.2.8
 Summary: Paquete demo de Motor de Calidad
 Author: Enzo Ipanaque
 Author-email: enzo.ipanaque@ms-peru.com
 License: Management Solutions
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: typing-extensions==4.5.0
```

### Comparing `MotorDeCalidad-2.2.7/README.md` & `MotorDeCalidad-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-2.2.7/motordecalidad/constants.py` & `MotorDeCalidad-2.2.8/motordecalidad/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MotorVersion = "2.2.7"
+MotorVersion = "2.2.8"
 ##Definición de clase Rules que contiene los datos de las reglas
 class Rules:
     class Pre_Requisites:
         name  = "Prerequisitos de Validación"
         property = "Integridad de Data"
         code = "100"
     class NullRule:
```

### Comparing `MotorDeCalidad-2.2.7/motordecalidad/field.py` & `MotorDeCalidad-2.2.8/motordecalidad/field.py`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-2.2.7/motordecalidad/functions.py` & `MotorDeCalidad-2.2.8/motordecalidad/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,32 +87,27 @@
         with open("output.txt", "w") as archivo:
             archivo.write(informs_str)
         blob_client = container_client.get_blob_client(f"/log/{datetime.now()}/otput.txt")
         with open("output.txt", "rb") as data:
             blob_client.upload_blob(data)
         os.remove("output.txt")
         return finalrequisitesDf
-    except Exception:
-        inform("Error en ejecución")
-        informs_str = "\n".join(lista_informs)
-        with open("output.txt", "w") as archivo:
-            archivo.write(informs_str)
-        blob_client = container_client.get_blob_client(f"/log/{datetime.now()}/otput.txt")
-        with open("output.txt", "rb") as data:
-            blob_client.upload_blob(data)
-        os.remove("output.txt")
 
 
 
 # Function that extracts the information from de JSON File
 def extractParamsFromJson(config):
     try:
-        with open(config, 'r', encoding='latin-1') as archivo_entrada:
+        try:
+            with open(config, 'r', encoding='latin-1') as archivo_entrada:
             # Cargar el JSON
-            data = json.load(archivo_entrada)
+                data = json.load(archivo_entrada)
+        except:
+            file = open(config)
+            data = json.load(file)
         inform("---> Se abre el json")
         input = data.get(JsonParts.Input)
         output = data.get(JsonParts.Output)
         country:str = input.get(JsonParts.Country)
         project:str = input.get(JsonParts.Project)
         entity:str = input.get(JsonParts.Entity)
         domain: str = input.get(JsonParts.Domain)
```

### Comparing `MotorDeCalidad-2.2.7/motordecalidad/rules.py` & `MotorDeCalidad-2.2.8/motordecalidad/rules.py`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-2.2.7/motordecalidad/utilities.py` & `MotorDeCalidad-2.2.8/motordecalidad/utilities.py`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-2.2.7/tests/test_rules.py` & `MotorDeCalidad-2.2.8/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-2.2.7/tests/test_utilities.py` & `MotorDeCalidad-2.2.8/tests/test_utilities.py`

 * *Files identical despite different names*

