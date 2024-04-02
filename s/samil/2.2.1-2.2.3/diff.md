# Comparing `tmp/samil-2.2.1.tar.gz` & `tmp/samil-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samil-2.2.1.tar", last modified: Sat Aug 27 13:15:09 2022, max compression
+gzip compressed data, was "samil-2.2.3.tar", last modified: Tue Apr  2 21:44:31 2024, max compression
```

## Comparing `samil-2.2.1.tar` & `samil-2.2.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 13:15:09.847562 samil-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-27 13:15:02.000000 samil-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9438 2022-08-27 13:15:09.847562 samil-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9017 2022-08-27 13:15:02.000000 samil-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 13:15:09.847562 samil-2.2.1/samil/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-27 13:15:02.000000 samil-2.2.1/samil/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15239 2022-08-27 13:15:02.000000 samil-2.2.1/samil/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-08-27 13:15:02.000000 samil-2.2.1/samil/influx.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16381 2022-08-27 13:15:02.000000 samil-2.2.1/samil/inverter.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-08-27 13:15:02.000000 samil-2.2.1/samil/inverterutil.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3513 2022-08-27 13:15:02.000000 samil-2.2.1/samil/pvoutput.py
--rw-r--r--   0 runner    (1001) docker     (121)     7223 2022-08-27 13:15:02.000000 samil-2.2.1/samil/statustypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 13:15:09.847562 samil-2.2.1/samil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9438 2022-08-27 13:15:09.000000 samil-2.2.1/samil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-08-27 13:15:09.000000 samil-2.2.1/samil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 13:15:09.000000 samil-2.2.1/samil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-27 13:15:09.000000 samil-2.2.1/samil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-27 13:15:09.000000 samil-2.2.1/samil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-27 13:15:09.000000 samil-2.2.1/samil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 13:15:09.847562 samil-2.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1091 2022-08-27 13:15:02.000000 samil-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:44:31.497039 samil-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 21:44:23.000000 samil-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-02 21:44:31.497039 samil-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-02 21:44:23.000000 samil-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:44:31.493039 samil-2.2.3/samil/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 21:44:23.000000 samil-2.2.3/samil/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15248 2024-04-02 21:44:23.000000 samil-2.2.3/samil/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-02 21:44:23.000000 samil-2.2.3/samil/influx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16477 2024-04-02 21:44:23.000000 samil-2.2.3/samil/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 21:44:23.000000 samil-2.2.3/samil/inverterutil.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3513 2024-04-02 21:44:23.000000 samil-2.2.3/samil/pvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-02 21:44:23.000000 samil-2.2.3/samil/statustypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:44:31.497039 samil-2.2.3/samil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-02 21:44:31.000000 samil-2.2.3/samil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 21:44:31.000000 samil-2.2.3/samil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:44:31.000000 samil-2.2.3/samil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 21:44:31.000000 samil-2.2.3/samil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 21:44:31.000000 samil-2.2.3/samil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 21:44:31.000000 samil-2.2.3/samil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:44:31.497039 samil-2.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1091 2024-04-02 21:44:23.000000 samil-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:44:31.493039 samil-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-04-02 21:44:23.000000 samil-2.2.3/tests/test_inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-02 21:44:23.000000 samil-2.2.3/tests/test_pvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-02 21:44:23.000000 samil-2.2.3/tests/test_statustypes.py
```

### Comparing `samil-2.2.1/LICENSE` & `samil-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `samil-2.2.1/PKG-INFO` & `samil-2.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: samil
-Version: 2.2.1
-Summary: Samil Power inverter tool
-Home-page: https://github.com/mhvis/solar
-Author: Maarten Visscher
-Author-email: mail@maartenvisscher.nl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Samil Power inverter tool
 
 [![PyPI](https://img.shields.io/pypi/v/samil)](https://pypi.org/project/samil/)
 
 Get model and status data from Samil Power inverters over the network.
 
 If you just need PVOutput.org uploading, you can also try the
@@ -34,14 +20,15 @@
 [semonet/solar](https://github.com/semonet/solar)
 
 ## Features
 
 * View inverter data
 * Upload to PVOutput.org
 * Publish to MQTT broker
+* Write to an InfluxDB database
 
 The following features are not implemented but can be easily implemented upon request:
 
 * Filter inverter based on IP or serial number
 * Support for multiple PVOutput.org systems
 
 ## Getting started
@@ -120,14 +107,18 @@
 The command `samil pvoutput` gathers status data from 1 or more inverters and uploads it to your PVOutput.org system.
 If you have multiple inverters, the data of each inverter is aggregated before uploading.
 
 For full usage info, run `samil pvoutput --help`.
 
 By default, the script uploads once and then stops. You can use cron to execute the script every 5 minutes.
 
+#### InfluxDB
+
+See CLI reference below.
+
 #### Fetch historical data
 
 *Todo*
 
 ## Run command at boot
 
 Follow the instructions here to run the MQTT or PVOutput command automatically at startup.
@@ -297,14 +288,46 @@
                           upload.
 
   --dry-run               Do not upload data to PVOutput.org.
   --interface TEXT        IP address of local network interface to bind to.
   --help                  Show this message and exit.
 ```
 
+```
+$ samil influx --help
+Usage: samil influx [OPTIONS] BUCKET
+
+  Writes system status data to an InfluxDB database.
+
+  The InfluxDB instance can be specified using environment variables or a
+  configuration file. See https://github.com/influxdata/influxdb-client-
+  python#client-configuration. Use the option -c to point to a configuration
+  file. Specify the bucket to write to in the BUCKET argument. Each
+  measurement will have the name 'samil'.
+
+  Do you have multiple inverters? This command only supports 1 inverter
+  because I am lazy and only need 1, but if you need more, create an issue on
+  the GitHub project page. It is trivial to add.
+
+  This command has no built-in restart mechanism and will crash for instance
+  when the Influx or inverter connection is lost. (This is again because I am
+  lazy, use systemd or Docker to restart on failure.)
+
+  Status is not written when the inverter is powered off at night.
+
+Options:
+  -c TEXT             InfluxDB client configuration file.
+  --interval FLOAT    Interval between status writes in seconds.  [default:
+                      10.0]
+  --interface TEXT    IP address of local network interface to bind to.
+  --gzip              Use GZip compression for the InfluxDB writes.
+  --measurement TEXT  InfluxDB measurement name.  [default: samil]
+  --help              Show this message and exit.
+```
+
 ## Development info
 
 Development installation (usually in a virtual environment):
 ```commandline
 pip install -e .
 pip install -r dev-requirements.txt
 ```
```

### Comparing `samil-2.2.1/README.md` & `samil-2.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: samil
+Version: 2.2.3
+Summary: Samil Power inverter tool
+Home-page: https://github.com/mhvis/solar
+Author: Maarten Visscher
+Author-email: mail@maartenvisscher.nl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: paho-mqtt>=1.5.0
+Requires-Dist: click>=7.1.2
+Requires-Dist: influxdb-client>=1.32.0
+
 # Samil Power inverter tool
 
 [![PyPI](https://img.shields.io/pypi/v/samil)](https://pypi.org/project/samil/)
 
 Get model and status data from Samil Power inverters over the network.
 
 If you just need PVOutput.org uploading, you can also try the
@@ -20,14 +37,15 @@
 [semonet/solar](https://github.com/semonet/solar)
 
 ## Features
 
 * View inverter data
 * Upload to PVOutput.org
 * Publish to MQTT broker
+* Write to an InfluxDB database
 
 The following features are not implemented but can be easily implemented upon request:
 
 * Filter inverter based on IP or serial number
 * Support for multiple PVOutput.org systems
 
 ## Getting started
@@ -106,14 +124,18 @@
 The command `samil pvoutput` gathers status data from 1 or more inverters and uploads it to your PVOutput.org system.
 If you have multiple inverters, the data of each inverter is aggregated before uploading.
 
 For full usage info, run `samil pvoutput --help`.
 
 By default, the script uploads once and then stops. You can use cron to execute the script every 5 minutes.
 
+#### InfluxDB
+
+See CLI reference below.
+
 #### Fetch historical data
 
 *Todo*
 
 ## Run command at boot
 
 Follow the instructions here to run the MQTT or PVOutput command automatically at startup.
@@ -283,14 +305,46 @@
                           upload.
 
   --dry-run               Do not upload data to PVOutput.org.
   --interface TEXT        IP address of local network interface to bind to.
   --help                  Show this message and exit.
 ```
 
+```
+$ samil influx --help
+Usage: samil influx [OPTIONS] BUCKET
+
+  Writes system status data to an InfluxDB database.
+
+  The InfluxDB instance can be specified using environment variables or a
+  configuration file. See https://github.com/influxdata/influxdb-client-
+  python#client-configuration. Use the option -c to point to a configuration
+  file. Specify the bucket to write to in the BUCKET argument. Each
+  measurement will have the name 'samil'.
+
+  Do you have multiple inverters? This command only supports 1 inverter
+  because I am lazy and only need 1, but if you need more, create an issue on
+  the GitHub project page. It is trivial to add.
+
+  This command has no built-in restart mechanism and will crash for instance
+  when the Influx or inverter connection is lost. (This is again because I am
+  lazy, use systemd or Docker to restart on failure.)
+
+  Status is not written when the inverter is powered off at night.
+
+Options:
+  -c TEXT             InfluxDB client configuration file.
+  --interval FLOAT    Interval between status writes in seconds.  [default:
+                      10.0]
+  --interface TEXT    IP address of local network interface to bind to.
+  --gzip              Use GZip compression for the InfluxDB writes.
+  --measurement TEXT  InfluxDB measurement name.  [default: samil]
+  --help              Show this message and exit.
+```
+
 ## Development info
 
 Development installation (usually in a virtual environment):
 ```commandline
 pip install -e .
 pip install -r dev-requirements.txt
 ```
```

### Comparing `samil-2.2.1/samil/cli.py` & `samil-2.2.3/samil/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,23 +303,23 @@
     """Writes system status data to an InfluxDB database.
 
     The InfluxDB instance can be specified using environment variables or a
     configuration file. See
     https://github.com/influxdata/influxdb-client-python#client-configuration.
     Use the option -c to point to a configuration file. Specify the bucket to
     write to in the BUCKET argument. Each measurement will have the name
-    'samil'.
+    'samil' by default.
 
     Do you have multiple inverters? This command only supports 1 inverter
     because I am lazy and only need 1, but if you need more, create an issue on
     the GitHub project page. It is trivial to add.
 
     This command has no built-in restart mechanism and will crash for instance
-    when the Influx or inverter connection is lost. (This is again because I am
-    lazy, use systemd or Docker to restart on failure.)
+    when the Influx or inverter connection is lost. This is again because I am
+    lazy, use systemd or Docker to restart on failure.
 
     Status is not written when the inverter is powered off at night.
     """
     # Print info messages (at least)
     if logging.root.level > logging.INFO:
         logging.basicConfig(level=logging.INFO)
```

### Comparing `samil-2.2.1/samil/influx.py` & `samil-2.2.3/samil/influx.py`

 * *Files identical despite different names*

### Comparing `samil-2.2.1/samil/inverter.py` & `samil-2.2.3/samil/inverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,16 @@
 
             for i in range(advertisements):
                 logger.debug('Sending server broadcast message')
                 bc.sendto(message, ('<broadcast>', 1300))
                 try:
                     sock, addr = self.listen_sock.accept()
                     logger.info('Connected with inverter on address %s', addr)
+                    # Wait before sending identification request
+                    sleep(1.0)
                     return sock, addr
                 except socket.timeout:
                     pass
         raise InverterNotFoundError
 
 
 def decode_string(val: bytes) -> str:
```

### Comparing `samil-2.2.1/samil/inverterutil.py` & `samil-2.2.3/samil/inverterutil.py`

 * *Files identical despite different names*

### Comparing `samil-2.2.1/samil/pvoutput.py` & `samil-2.2.3/samil/pvoutput.py`

 * *Files identical despite different names*

### Comparing `samil-2.2.1/samil/statustypes.py` & `samil-2.2.3/samil/statustypes.py`

 * *Files identical despite different names*

### Comparing `samil-2.2.1/samil.egg-info/PKG-INFO` & `samil-2.2.3/samil.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: samil
-Version: 2.2.1
+Version: 2.2.3
 Summary: Samil Power inverter tool
 Home-page: https://github.com/mhvis/solar
 Author: Maarten Visscher
 Author-email: mail@maartenvisscher.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: paho-mqtt>=1.5.0
+Requires-Dist: click>=7.1.2
+Requires-Dist: influxdb-client>=1.32.0
 
 # Samil Power inverter tool
 
 [![PyPI](https://img.shields.io/pypi/v/samil)](https://pypi.org/project/samil/)
 
 Get model and status data from Samil Power inverters over the network.
 
@@ -34,14 +37,15 @@
 [semonet/solar](https://github.com/semonet/solar)
 
 ## Features
 
 * View inverter data
 * Upload to PVOutput.org
 * Publish to MQTT broker
+* Write to an InfluxDB database
 
 The following features are not implemented but can be easily implemented upon request:
 
 * Filter inverter based on IP or serial number
 * Support for multiple PVOutput.org systems
 
 ## Getting started
@@ -120,14 +124,18 @@
 The command `samil pvoutput` gathers status data from 1 or more inverters and uploads it to your PVOutput.org system.
 If you have multiple inverters, the data of each inverter is aggregated before uploading.
 
 For full usage info, run `samil pvoutput --help`.
 
 By default, the script uploads once and then stops. You can use cron to execute the script every 5 minutes.
 
+#### InfluxDB
+
+See CLI reference below.
+
 #### Fetch historical data
 
 *Todo*
 
 ## Run command at boot
 
 Follow the instructions here to run the MQTT or PVOutput command automatically at startup.
@@ -297,14 +305,46 @@
                           upload.
 
   --dry-run               Do not upload data to PVOutput.org.
   --interface TEXT        IP address of local network interface to bind to.
   --help                  Show this message and exit.
 ```
 
+```
+$ samil influx --help
+Usage: samil influx [OPTIONS] BUCKET
+
+  Writes system status data to an InfluxDB database.
+
+  The InfluxDB instance can be specified using environment variables or a
+  configuration file. See https://github.com/influxdata/influxdb-client-
+  python#client-configuration. Use the option -c to point to a configuration
+  file. Specify the bucket to write to in the BUCKET argument. Each
+  measurement will have the name 'samil'.
+
+  Do you have multiple inverters? This command only supports 1 inverter
+  because I am lazy and only need 1, but if you need more, create an issue on
+  the GitHub project page. It is trivial to add.
+
+  This command has no built-in restart mechanism and will crash for instance
+  when the Influx or inverter connection is lost. (This is again because I am
+  lazy, use systemd or Docker to restart on failure.)
+
+  Status is not written when the inverter is powered off at night.
+
+Options:
+  -c TEXT             InfluxDB client configuration file.
+  --interval FLOAT    Interval between status writes in seconds.  [default:
+                      10.0]
+  --interface TEXT    IP address of local network interface to bind to.
+  --gzip              Use GZip compression for the InfluxDB writes.
+  --measurement TEXT  InfluxDB measurement name.  [default: samil]
+  --help              Show this message and exit.
+```
+
 ## Development info
 
 Development installation (usually in a virtual environment):
 ```commandline
 pip install -e .
 pip install -r dev-requirements.txt
 ```
```

### Comparing `samil-2.2.1/setup.py` & `samil-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="samil",
-    version="2.2.1",
+    version="2.2.3",
     author="Maarten Visscher",
     author_email="mail@maartenvisscher.nl",
     description="Samil Power inverter tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mhvis/solar",
     packages=["samil"],
```

