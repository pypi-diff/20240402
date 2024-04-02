# Comparing `tmp/lidia-0.9.1.tar.gz` & `tmp/lidia-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidia-0.9.1.tar", last modified: Fri Oct 27 13:17:45 2023, max compression
+gzip compressed data, was "lidia-0.9.2.tar", last modified: Mon Dec  4 13:53:43 2023, max compression
```

## Comparing `lidia-0.9.1.tar` & `lidia-0.9.2.tar`

### file list

```diff
@@ -1,53 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.726858 lidia-0.9.1/
--rw-rw-rw-   0        0        0     1097 2023-02-17 08:50:04.000000 lidia-0.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0      114 2023-03-01 12:02:42.000000 lidia-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2712 2023-10-27 13:17:45.725857 lidia-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2052 2023-10-27 12:37:29.000000 lidia-0.9.1/README.md
--rw-rw-rw-   0        0        0       88 2022-12-15 16:52:24.000000 lidia-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      858 2023-10-27 13:17:45.728860 lidia-0.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.102883 lidia-0.9.1/src/
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.399856 lidia-0.9.1/src/lidia/
--rw-rw-rw-   0        0        0       23 2023-10-27 12:38:20.000000 lidia-0.9.1/src/lidia/__init__.py
--rw-rw-rw-   0        0        0       35 2022-06-02 23:11:14.000000 lidia-0.9.1/src/lidia/__main__.py
--rw-rw-rw-   0        0        0    14247 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/aircraft.py
--rw-rw-rw-   0        0        0     3584 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/approach.html
--rw-rw-rw-   0        0        0     5293 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/cas.html
--rw-rw-rw-   0        0        0     4862 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/config.py
--rw-rw-rw-   0        0        0     1061 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/info.html
--rw-rw-rw-   0        0        0     5165 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/lidia.py
--rw-rw-rw-   0        0        0     2540 2023-04-17 19:44:22.000000 lidia-0.9.1/src/lidia/mytypes.py
--rw-rw-rw-   0        0        0    38852 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/pfd.html
--rw-rw-rw-   0        0        0    15774 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/rpctask.html
--rw-rw-rw-   0        0        0     2312 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/server.py
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.585859 lidia-0.9.1/src/lidia/sources/
--rw-rw-rw-   0        0        0        0 2022-06-13 10:57:36.000000 lidia-0.9.1/src/lidia/sources/__init__.py
--rw-rw-rw-   0        0        0     2236 2022-12-19 19:16:52.000000 lidia-0.9.1/src/lidia/sources/approach.py
--rw-rw-rw-   0        0        0     1551 2023-02-17 08:50:04.000000 lidia-0.9.1/src/lidia/sources/confighelp.md
--rw-rw-rw-   0        0        0     2416 2023-03-01 11:21:48.000000 lidia-0.9.1/src/lidia/sources/confighelp.py
--rw-rw-rw-   0        0        0     6390 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/sources/demo.py
--rw-rw-rw-   0        0        0     2937 2023-03-01 11:21:48.000000 lidia-0.9.1/src/lidia/sources/flightgear.py
--rw-rw-rw-   0        0        0     6600 2022-12-19 19:16:52.000000 lidia-0.9.1/src/lidia/sources/mytypes.py
--rw-rw-rw-   0        0        0     3623 2023-03-01 11:21:48.000000 lidia-0.9.1/src/lidia/sources/rpctask.py
--rw-rw-rw-   0        0        0     2255 2023-10-27 12:37:53.000000 lidia-0.9.1/src/lidia/sources/smol.py
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.700859 lidia-0.9.1/src/lidia/static/
--rw-rw-rw-   0        0        0     1761 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/LICENSE.txt
--rw-rw-rw-   0        0        0    87008 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    87788 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    87592 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    86820 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    86908 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87076 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    87872 2022-11-28 17:12:51.000000 lidia-0.9.1/src/lidia/static/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0     7073 2022-12-09 17:51:17.000000 lidia-0.9.1/src/lidia/static/controls.js
--rw-rw-rw-   0        0        0   121824 2022-06-02 22:10:07.000000 lidia-0.9.1/src/lidia/static/socket.io.js
--rw-rw-rw-   0        0        0     1853 2023-03-01 11:21:48.000000 lidia-0.9.1/src/lidia/static/style.css
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.723857 lidia-0.9.1/src/lidia/utils/
--rw-rw-rw-   0        0        0     3654 2023-04-17 19:44:22.000000 lidia-0.9.1/src/lidia/utils/pack_lidia.m
--rw-rw-rw-   0        0        0    22361 2023-10-27 12:37:29.000000 lidia-0.9.1/src/lidia/utils/pack_maker.py
-drwxrwxrwx   0        0        0        0 2023-10-27 13:17:45.444857 lidia-0.9.1/src/lidia.egg-info/
--rw-rw-rw-   0        0        0     2712 2023-10-27 13:17:45.000000 lidia-0.9.1/src/lidia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-10-27 13:17:45.000000 lidia-0.9.1/src/lidia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-27 13:17:45.000000 lidia-0.9.1/src/lidia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-10-27 13:17:45.000000 lidia-0.9.1/src/lidia.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-10-27 13:17:45.000000 lidia-0.9.1/src/lidia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-10-27 13:17:45.000000 lidia-0.9.1/src/lidia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.962784 lidia-0.9.2/
+-rw-rw-rw-   0        0        0     1097 2023-02-17 08:50:04.000000 lidia-0.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      114 2023-03-01 12:02:42.000000 lidia-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2835 2023-12-04 13:53:43.961772 lidia-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2023-10-27 13:20:42.000000 lidia-0.9.2/README.md
+-rw-rw-rw-   0        0        0       88 2022-12-15 16:52:24.000000 lidia-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      858 2023-12-04 13:53:43.971772 lidia-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.816769 lidia-0.9.2/src/
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.846771 lidia-0.9.2/src/lidia/
+-rw-rw-rw-   0        0        0       23 2023-12-04 13:52:03.000000 lidia-0.9.2/src/lidia/__init__.py
+-rw-rw-rw-   0        0        0       35 2022-06-02 23:11:14.000000 lidia-0.9.2/src/lidia/__main__.py
+-rw-rw-rw-   0        0        0    14506 2023-10-27 13:20:42.000000 lidia-0.9.2/src/lidia/aircraft.py
+-rw-rw-rw-   0        0        0     4770 2023-10-27 13:20:42.000000 lidia-0.9.2/src/lidia/config.py
+-rw-rw-rw-   0        0        0     5186 2023-10-27 13:20:42.000000 lidia-0.9.2/src/lidia/lidia.py
+-rw-rw-rw-   0        0        0     2540 2023-04-17 19:44:22.000000 lidia-0.9.2/src/lidia/mytypes.py
+-rw-rw-rw-   0        0        0     2539 2023-12-04 13:47:26.000000 lidia-0.9.2/src/lidia/server.py
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.916771 lidia-0.9.2/src/lidia/sources/
+-rw-rw-rw-   0        0        0        0 2022-06-13 10:57:36.000000 lidia-0.9.2/src/lidia/sources/__init__.py
+-rw-rw-rw-   0        0        0     2236 2022-12-19 19:16:52.000000 lidia-0.9.2/src/lidia/sources/approach.py
+-rw-rw-rw-   0        0        0     1551 2023-02-17 08:50:04.000000 lidia-0.9.2/src/lidia/sources/confighelp.md
+-rw-rw-rw-   0        0        0     2416 2023-03-01 11:21:48.000000 lidia-0.9.2/src/lidia/sources/confighelp.py
+-rw-rw-rw-   0        0        0     6523 2023-10-27 13:20:42.000000 lidia-0.9.2/src/lidia/sources/demo.py
+-rw-rw-rw-   0        0        0     2937 2023-03-01 11:21:48.000000 lidia-0.9.2/src/lidia/sources/flightgear.py
+-rw-rw-rw-   0        0        0     6600 2022-12-19 19:16:52.000000 lidia-0.9.2/src/lidia/sources/mytypes.py
+-rw-rw-rw-   0        0        0     3623 2023-03-01 11:21:48.000000 lidia-0.9.2/src/lidia/sources/rpctask.py
+-rw-rw-rw-   0        0        0     2491 2023-10-27 13:20:09.000000 lidia-0.9.2/src/lidia/sources/smol.py
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.950786 lidia-0.9.2/src/lidia/static/
+-rw-rw-rw-   0        0        0     1761 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/LICENSE.txt
+-rw-rw-rw-   0        0        0    87008 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    87788 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    87592 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    86820 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    86908 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87076 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    87872 2022-11-28 17:12:51.000000 lidia-0.9.2/src/lidia/static/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0     7073 2022-12-09 17:51:17.000000 lidia-0.9.2/src/lidia/static/controls.js
+-rw-rw-rw-   0        0        0   121824 2022-06-02 22:10:07.000000 lidia-0.9.2/src/lidia/static/socket.io.js
+-rw-rw-rw-   0        0        0     1853 2023-03-01 11:21:48.000000 lidia-0.9.2/src/lidia/static/style.css
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.954769 lidia-0.9.2/src/lidia/utils/
+-rw-rw-rw-   0        0        0     3654 2023-04-17 19:44:22.000000 lidia-0.9.2/src/lidia/utils/pack_lidia.m
+-rw-rw-rw-   0        0        0    22331 2023-10-27 13:20:42.000000 lidia-0.9.2/src/lidia/utils/pack_maker.py
+drwxrwxrwx   0        0        0        0 2023-12-04 13:53:43.959774 lidia-0.9.2/src/lidia.egg-info/
+-rw-rw-rw-   0        0        0     2835 2023-12-04 13:53:43.000000 lidia-0.9.2/src/lidia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1119 2023-12-04 13:53:43.000000 lidia-0.9.2/src/lidia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-04 13:53:43.000000 lidia-0.9.2/src/lidia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-12-04 13:53:43.000000 lidia-0.9.2/src/lidia.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-12-04 13:53:43.000000 lidia-0.9.2/src/lidia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-12-04 13:53:43.000000 lidia-0.9.2/src/lidia.egg-info/top_level.txt
```

### Comparing `lidia-0.9.1/LICENSE.txt` & `lidia-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/PKG-INFO` & `lidia-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidia
-Version: 0.9.1
+Version: 0.9.2
 Summary: serve an aircraft instruments panel as a web page
 Home-page: https://gitlab.com/Maarrk/lidia
 Author: Marek S. Lukasiewicz
 Author-email: marek@lukasiewicz.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -75,14 +75,15 @@
 ## Contributing
 
 - Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
 - Python code should be formatted with autopep8
 - Other source files should be formatted with Prettier
 - Install packages for development with `pip install -r requirements.txt`
 - To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
+- APIs deprecated in previous versions, waiting to be changed in next major release are marked with `@deprecated` comment
 
 ## Acknowledgements
 
 This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
 
 Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
```

### Comparing `lidia-0.9.1/README.md` & `lidia-0.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 ## Contributing
 
 - Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
 - Python code should be formatted with autopep8
 - Other source files should be formatted with Prettier
 - Install packages for development with `pip install -r requirements.txt`
 - To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
+- APIs deprecated in previous versions, waiting to be changed in next major release are marked with `@deprecated` comment
 
 ## Acknowledgements
 
 This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
 
 Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
```

### Comparing `lidia-0.9.1/setup.cfg` & `lidia-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/aircraft.py` & `lidia-0.9.2/src/lidia/aircraft.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,18 @@
             (XYZ, 'v_body'),
             (XYZ, 'a_body'),
             (Controls, 'ctrl'),
             (HelicopterRPM, 'hrpm'),
         ]:
             if name in smol:
                 setattr(state, name, VectorType.from_list(smol[name]))
-        # TODO: Borders
+        if 'brdr' in smol:
+            state.brdr = Borders()
+            state.brdr.low = Controls.from_list(smol['brdr']['low'])
+            state.brdr.high = Controls.from_list(smol['brdr']['high'])
         if 'btn' in smol:
             state.btn = Buttons.from_list(smol['btn'])
         if 'instr' in smol:
             state.instr = Instruments()
             for name in ['ias', 'gs', 'alt', 'qnh', 'ralt']:
                 if name in smol['instr']:
                     setattr(state.instr, name, smol['instr'][name])
@@ -352,17 +355,16 @@
         return data
 
     @classmethod
     def from_smol(cls, smol: dict) -> 'AircraftState':
         state = cls(**super().from_smol(smol).dict())
         for name in ['trgt', 'trim']:
             if name in smol:
-                # For backwards compatibility
+                # @deprecated
                 if smol[name] is List:
-                    # TODO: Some warning when logging setup available
                     smol[name] = {'ctrl': {name: smol[name]}}
                 setattr(state, name, AircraftData.from_smol(smol[name]))
 
         return state
 
 
 if __name__ == '__main__':
@@ -383,14 +385,17 @@
     state.t_boot = 0x10000000
     state.model_instruments(config)
     state.instr.tcas = []
     state.instr.tcas.append(TrafficObject(
         vol=TrafficVolume.PROXIMATE_TRAFFIC,
         brg=0.5, dist=5000.0, alt=10.0, vsi=0
     ))
+    state.brdr = Borders()
+    state.brdr.low = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
+    state.brdr.high = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
     print(state.smol())
     import msgpack
     packer = msgpack.Packer(use_single_float=False)
     data_double = packer.pack(state.smol())
     packer = msgpack.Packer(use_single_float=True)
     data_float = packer.pack(state.smol())
     data = data_double[:0x21] + data_float[0x15:]
```

### Comparing `lidia-0.9.1/src/lidia/config.py` & `lidia-0.9.2/src/lidia/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,31 +33,30 @@
     """Show flightpath vector (FPV) indicator on ADI"""
     show_retrograde: bool = False
     """Show reverse flight path vector on ADI"""
     move_roll_ticks: bool = False
     """Move roll angle scale with horizon, keeping sideslip triangle in place"""
     sideslip_max: float = 15.0
     """Maximal displayed sideslip angle, in degrees"""
-    # TODO: Rewrite docstrings to reference terms like "safe", "warning", "desired" etc. instead of colors
     rpm_e_good_low: float = 0.97
-    """Engine RPM green tape lower limit"""
+    """Engine RPM safe region lower limit"""
     rpm_e_good_high: float = 1.03
-    """Engine RPM green tape upper limit"""
+    """Engine RPM safe region upper limit"""
     rpm_e_warn_low: float = 0.97
-    """Engine RPM yellow tape lower limit"""
+    """Engine RPM warning region lower limit"""
     rpm_e_warn_high: float = 1.03
-    """Engine RPM yellow tape upper limit"""
+    """Engine RPM warning region upper limit"""
     rpm_r_good_low: float = 0.97
-    """Rotor RPM green tape lower limit"""
+    """Rotor RPM safe region lower limit"""
     rpm_r_good_high: float = 1.03
-    """Rotor RPM green tape upper limit"""
+    """Rotor RPM safe region upper limit"""
     rpm_r_warn_low: float = 0.90
-    """Rotor RPM yellow tape lower limit"""
+    """Rotor RPM warning region lower limit"""
     rpm_r_warn_high: float = 1.10
-    """Rotor RPM yellow tape upper limit"""
+    """Rotor RPM warning region upper limit"""
     traffic_range: float = 18520.0
     """Range of displayed traffic information, in meters"""
 
 
 class ApproachConfig(NestingModel):
     """Ship approach configuration"""
     nominal_alt: float = 3
```

### Comparing `lidia-0.9.1/src/lidia/lidia.py` & `lidia-0.9.2/src/lidia/lidia.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     queue = Queue()
     server_process = Process(target=run_server, args=(queue, args, config))
     server_process.start()
 
     if args.verbosity >= 0 and not args.source.endswith('help'):
         print(f"""\
 Lidia GUIs driven by '{args.source}' source served on:
-    - RPC task: http://localhost:{args.http_port}/rpctask
+    - Controls View (aka RPC task): http://localhost:{args.http_port}/controls
     - Primary Flight Display: http://localhost:{args.http_port}/pfd
     - Ship Approach: http://localhost:{args.http_port}/approach
 
 (see this list and configuration at http://localhost:{args.http_port}/info)""")
         if args.passthrough_port is not None:
             print(
                 f'State in SMOL forwarded via UDP to {args.passthrough_host}:{args.passthrough_port}')
```

### Comparing `lidia-0.9.1/src/lidia/mytypes.py` & `lidia-0.9.2/src/lidia/mytypes.py`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/server.py` & `lidia-0.9.2/src/lidia/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,20 +34,24 @@
             pass
         eventlet.sleep(0.02)
 
 
 def run_server(q: Queue, args: Namespace, config: Config):
     # specifying just local path breaks when run as a module
     root_path = path.abspath(path.dirname(__file__))
+    pages_path = path.join(root_path, 'pages')
     static_files = {
-        '/': {'content_type': 'text/html', 'filename': path.join(root_path, 'rpctask.html')},
-        '/info': {'content_type': 'text/html', 'filename': path.join(root_path, 'info.html')},
-        '/rpctask': {'content_type': 'text/html', 'filename': path.join(root_path, 'rpctask.html')},
-        '/pfd': {'content_type': 'text/html', 'filename': path.join(root_path, 'pfd.html')},
-        '/approach': {'content_type': 'text/html', 'filename': path.join(root_path, 'approach.html')},
+        # @deprecated: change to info.html
+        '/': {'content_type': 'text/html', 'filename': path.join(pages_path, 'controls.html')},
+        '/info': {'content_type': 'text/html', 'filename': path.join(pages_path, 'info.html')},
+        '/controls': {'content_type': 'text/html', 'filename': path.join(pages_path, 'controls.html')},
+        # @deprecated
+        '/rpctask': {'content_type': 'text/html', 'filename': path.join(pages_path, 'controls.html')},
+        '/pfd': {'content_type': 'text/html', 'filename': path.join(pages_path, 'pfd.html')},
+        '/approach': {'content_type': 'text/html', 'filename': path.join(pages_path, 'approach.html')},
         '/static': path.join(root_path, 'static'),
     }
 
     sio = socketio.Server()
 
     @sio.on('config_request')
     def config_request(_sid, _environ):
```

### Comparing `lidia-0.9.1/src/lidia/sources/approach.py` & `lidia-0.9.2/src/lidia/sources/approach.py`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/sources/confighelp.md` & `lidia-0.9.2/src/lidia/sources/confighelp.md`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/sources/confighelp.py` & `lidia-0.9.2/src/lidia/sources/confighelp.py`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/sources/demo.py` & `lidia-0.9.2/src/lidia/sources/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,10 +155,13 @@
             vol=TrafficVolume.TRAFFIC_ADVISORY,
             brg=-0.3, dist=10000, alt=-10, vsi=1
         ))
         state.instr.tcas.append(TrafficObject(
             vol=TrafficVolume.RESOLUTION_ADVISORY,
             brg=-0.5, dist=5000, alt=-120, vsi=0
         ))
+        # Keep traffic objects fixed in world space
+        for trobj in state.instr.tcas:
+            trobj.brg += state.att.yaw
 
         q.put(('smol', state.smol()))
         sleep(1 / args.frequency)
```

### Comparing `lidia-0.9.1/src/lidia/sources/flightgear.py` & `lidia-0.9.2/src/lidia/sources/flightgear.py`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/sources/mytypes.py` & `lidia-0.9.2/src/lidia/sources/mytypes.py`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/sources/rpctask.py` & `lidia-0.9.2/src/lidia/sources/rpctask.py`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/sources/smol.py` & `lidia-0.9.2/src/lidia/sources/smol.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,13 +53,17 @@
                     except Exception as e:
                         print(e)
 
                 if decoded is not None:
                     try:
                         state = AircraftState.from_smol(decoded)
                         state.model_instruments(config)
+                        if state.trgt is not None:
+                            state.trgt.model_instruments(config)
+                        if state.trim is not None:
+                            state.trim.model_instruments(config)
                         q.put(('smol', state.smol()))
                     except Exception as e:
                         print(e)
 
             except socket.timeout:
                 continue
```

### Comparing `lidia-0.9.1/src/lidia/static/LICENSE.txt` & `lidia-0.9.2/src/lidia/static/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-Bold.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-ExtraLight.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-Light.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-Medium.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-Regular.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-SemiBold.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/RobotoMono-Thin.ttf` & `lidia-0.9.2/src/lidia/static/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/controls.js` & `lidia-0.9.2/src/lidia/static/controls.js`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/socket.io.js` & `lidia-0.9.2/src/lidia/static/socket.io.js`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/static/style.css` & `lidia-0.9.2/src/lidia/static/style.css`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/utils/pack_lidia.m` & `lidia-0.9.2/src/lidia/utils/pack_lidia.m`

 * *Files identical despite different names*

### Comparing `lidia-0.9.1/src/lidia/utils/pack_maker.py` & `lidia-0.9.2/src/lidia/utils/pack_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
     with open(output + '.elm', 'w') as out_elm:
         out_elm.write('''##### Generated with pack_maker.py
 # output stream definition
 # include it in your model **inside the elements block** like this:
 #
 # include: "./{}.elm";
-# 
+#
 # you also need to increase the number of output elements in the control data block:
 # begin: control data;
 #     output elements: +1;
 # end: control data;
 
 ### output stream definition
 stream output: {}{},
@@ -410,19 +410,19 @@
                         main_fields, trgt_fields, trim_fields)
 
         out_elm.write('\tvalues, {},\n'.format(values.getvalue().count('\n')))
         out_elm.write(values.getvalue())
         out_elm.write('''
 \tmodifier, copy cast,
 \t\tswap, f, d, i,
-''')  # TODO: verify swapped types
+''')
         type_out = StringIO()
         pack_fieldlists(Generator.MBDYN_TYPE, type_out, infos,
                         main_fields, trgt_fields, trim_fields)
-        out_elm.write(type_out.getvalue()[:-2]) # strip ending ',\n'
+        out_elm.write(type_out.getvalue()[:-2])  # strip ending ',\n'
         out_elm.write('''
 \t;
 
 # vim:ft=mbd
 ''')
```

### Comparing `lidia-0.9.1/src/lidia.egg-info/PKG-INFO` & `lidia-0.9.2/src/lidia.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidia
-Version: 0.9.1
+Version: 0.9.2
 Summary: serve an aircraft instruments panel as a web page
 Home-page: https://gitlab.com/Maarrk/lidia
 Author: Marek S. Lukasiewicz
 Author-email: marek@lukasiewicz.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -75,14 +75,15 @@
 ## Contributing
 
 - Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
 - Python code should be formatted with autopep8
 - Other source files should be formatted with Prettier
 - Install packages for development with `pip install -r requirements.txt`
 - To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
+- APIs deprecated in previous versions, waiting to be changed in next major release are marked with `@deprecated` comment
 
 ## Acknowledgements
 
 This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
 
 Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
```

### Comparing `lidia-0.9.1/src/lidia.egg-info/SOURCES.txt` & `lidia-0.9.2/src/lidia.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,17 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/lidia/__init__.py
 src/lidia/__main__.py
 src/lidia/aircraft.py
-src/lidia/approach.html
-src/lidia/cas.html
 src/lidia/config.py
-src/lidia/info.html
 src/lidia/lidia.py
 src/lidia/mytypes.py
-src/lidia/pfd.html
-src/lidia/rpctask.html
 src/lidia/server.py
 src/lidia.egg-info/PKG-INFO
 src/lidia.egg-info/SOURCES.txt
 src/lidia.egg-info/dependency_links.txt
 src/lidia.egg-info/entry_points.txt
 src/lidia.egg-info/requires.txt
 src/lidia.egg-info/top_level.txt
```

