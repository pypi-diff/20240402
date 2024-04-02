# Comparing `tmp/py_ballisticcalc-2.0.0b1.tar.gz` & `tmp/py_ballisticcalc-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc-2.0.0b1.tar", last modified: Tue Mar 26 09:01:35 2024, max compression
+gzip compressed data, was "py_ballisticcalc-2.0.0b2.tar", last modified: Tue Apr  2 04:25:27 2024, max compression
```

## Comparing `py_ballisticcalc-2.0.0b1.tar` & `py_ballisticcalc-2.0.0b2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:35.334640 py_ballisticcalc-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-03-26 09:01:35.334640 py_ballisticcalc-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:35.334640 py_ballisticcalc-2.0.0b1/py_ballisticcalc/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/drag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22165 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/drag_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/multiple_bc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/munition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/trajectory_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:35.334640 py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-03-26 09:01:35.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-26 09:01:35.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 09:01:35.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 09:01:35.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 09:01:35.000000 py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 09:01:35.334640 py_ballisticcalc-2.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:35.334640 py_ballisticcalc-2.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_danger_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_mbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-03-26 09:01:24.000000 py_ballisticcalc-2.0.0b1/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.645088 py_ballisticcalc-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-04-02 04:25:27.645088 py_ballisticcalc-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.641088 py_ballisticcalc-2.0.0b2/py_ballisticcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22165 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/multiple_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/munition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.641088 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:25:27.645088 py_ballisticcalc-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.641088 py_ballisticcalc-2.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_danger_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_mbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.0b1/LICENSE` & `py_ballisticcalc-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/PKG-INFO` & `py_ballisticcalc-2.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,15 +185,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b1; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b2; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.0b1/README.md` & `py_ballisticcalc-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/__init__.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/conditions.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/conditions.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 cStandardPressure: float = 29.92          # InHg
 cSpeedOfSoundImperial: float = 49.0223    # Mach1 in fps = cSpeedOfSound * sqrt(°R)
 cStandardDensity: float = 0.076474        # lb/ft^3
 
 @dataclass
 class Atmo(TypedUnits):  # pylint: disable=too-many-instance-attributes
     """Atmospheric conditions and density calculations"""
-    altitude: [float, Distance] = field(default_factory=lambda: Set.Units.distance)
-    pressure: [float, Pressure] = field(default_factory=lambda: Set.Units.pressure)
-    temperature: [float, Temperature] = field(default_factory=lambda: Set.Units.temperature)
+    altitude: [float, Distance] = field(default_factory=Set.Units.distance)
+    pressure: [float, Pressure] = field(default_factory=Set.Units.pressure)
+    temperature: [float, Temperature] = field(default_factory=Set.Units.temperature)
     humidity: float = 0.0           # Relative humidity [0% to 100%]
     density_ratio: float = field(init=False)  # Density / cStandardDensity
     mach: Velocity = field(init=False)  # Mach 1 in reference atmosphere
     _mach1: float = field(init=False)  # Mach 1 in reference atmosphere in fps
     _a0: float = field(init=False)  # Initial reference altitude (ft)
     _t0: float = field(init=False)  # Temperature given at reference altitude °F
     _p0: float = field(init=False)  # Barometric pressure (sea level)
@@ -190,17 +190,17 @@
 @dataclass
 class Wind(TypedUnits):
     """
     Wind direction and velocity by down-range distance.
     direction_from = 0 is blowing from behind shooter. 
     direction_from = 90 degrees is blowing from shooter's left towards right.
     """
-    velocity: [float, Velocity] = field(default_factory=lambda: Set.Units.velocity)
-    direction_from: [float, Angular] = field(default_factory=lambda: Set.Units.angular)
-    until_distance: [float, Distance] = field(default_factory=lambda: Set.Units.distance)
+    velocity: [float, Velocity] = field(default_factory=Set.Units.velocity)
+    direction_from: [float, Angular] = field(default_factory=Set.Units.angular)
+    until_distance: [float, Distance] = field(default_factory=Set.Units.distance)
     MAX_DISTANCE_FEET = 1e8
 
     def __post_init__(self):
         if not self.until_distance:
             self.until_distance = Distance.Foot(Wind.MAX_DISTANCE_FEET)
         if not self.direction_from or not self.velocity:
             self.direction_from = 0
@@ -217,17 +217,17 @@
             With target_distance = sight distance to a target (i.e., as through a rangefinder):
                 * Horizontal distance X to target = cos(look_angle) * target_distance
                 * Vertical distance Y to target = sin(look_angle) * target_distance
     :param relative_angle: Elevation adjustment added to weapon.zero_elevation for a particular shot.
     :param cant_angle: Tilt of gun from vertical, which shifts any barrel elevation
         from the vertical plane into the horizontal plane by sine(cant_angle)
     """
-    look_angle: [float, Angular] = field(default_factory=lambda: Set.Units.angular)
-    relative_angle: [float, Angular] = field(default_factory=lambda: Set.Units.angular)
-    cant_angle: [float, Angular] = field(default_factory=lambda: Set.Units.angular)
+    look_angle: [float, Angular] = field(default_factory=Set.Units.angular)
+    relative_angle: [float, Angular] = field(default_factory=Set.Units.angular)
+    cant_angle: [float, Angular] = field(default_factory=Set.Units.angular)
 
     weapon: Weapon = field(default=None)
     ammo: Ammo = field(default=None)
     atmo: Atmo = field(default=None)
     winds: list[Wind] = field(default=None)
     # NOTE: Calculator assumes that winds are sorted by Wind.until_distance (ascending)
```

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/drag_model.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_model.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/drag_tables.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_tables.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/example.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/example.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/interface.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/interface.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/multiple_bc.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/multiple_bc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/munition.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/munition.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     """
     :param sight_height: Vertical distance from center of bore line to center of sight line.
     :param twist: Distance for barrel rifling to complete one complete turn.
         Positive value => right-hand twist, negative value => left-hand twist.
     :param zero_elevation: Angle of barrel relative to sight line when sight is set to "zero."
         (Typically computed by ballistic Calculator.)
     """
-    sight_height: [float, Distance] = field(default_factory=lambda: Set.Units.sight_height)
-    twist: [float, Distance] = field(default_factory=lambda: Set.Units.twist)
-    zero_elevation: [float, Angular] = field(default_factory=lambda: Set.Units.angular)
+    sight_height: [float, Distance] = field(default_factory=Set.Units.sight_height)
+    twist: [float, Distance] = field(default_factory=Set.Units.twist)
+    zero_elevation: [float, Angular] = field(default_factory=Set.Units.angular)
 
     def __post_init__(self):
         if not self.sight_height:
             self.sight_height = 0
         if not self.twist:
             self.twist = 0
         if not self.zero_elevation:
@@ -38,16 +38,16 @@
     :param mv: Muzzle Velocity
     :param powder_temp: Baseline temperature that produces the given mv
     :param temp_modifier: Change in velocity w temperature: % per 15°C.
         Can be computed with .calc_powder_sens().  Only applies if:
             Settings.USE_POWDER_SENSITIVITY = True
     """
     dm: DragModel = field(default=None)
-    mv: [float, Velocity] = field(default_factory=lambda: Set.Units.velocity)
-    powder_temp: [float, Temperature] = field(default_factory=lambda: Set.Units.temperature)
+    mv: [float, Velocity] = field(default_factory=Set.Units.velocity)
+    powder_temp: [float, Temperature] = field(default_factory=Set.Units.temperature)
     temp_modifier: float = field(default=0)
 
     def __post_init__(self):
         if not self.powder_temp:
             self.powder_temp = Temperature.Celsius(15)
 
     def calc_powder_sens(self, other_velocity: [float, Velocity],
```

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/settings.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/settings.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/trajectory_calc.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_calc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/trajectory_data.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_data.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc/unit.py` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,20 +86,23 @@
         :return: short symbol of the unit of measure in CI
         """
         return UnitPropsDict[self].symbol
 
     def __repr__(self) -> str:
         return UnitPropsDict[self].name
 
-    def __call__(self: 'Unit', value: [int, float, 'AbstractUnit']) -> 'AbstractUnit':
+    def __call__(self: 'Unit', value: [int, float, 'AbstractUnit'] = None) -> ['AbstractUnit', 'Unit']:
         """Creates new unit instance by dot syntax
         :param self: unit as Unit enum
         :param value: numeric value of the unit
         :return: AbstractUnit instance
         """
+        if value is None:
+            return self
+
         if isinstance(value, AbstractUnit):
             return value << self
         if 0 <= self < 10:
             obj = Angular(value, self)
         elif 10 <= self < 20:
             obj = Distance(value, self)
         elif 30 <= self < 40:
```

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/PKG-INFO` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,15 +185,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b1; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b2; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.0b1/py_ballisticcalc.egg-info/SOURCES.txt` & `py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/pyproject.toml` & `py_ballisticcalc-2.0.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc"
-version = "2.0.0b1"
+version = "2.0.0b2"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
@@ -54,10 +54,10 @@
 
 
 #[tool.setuptools.dynamic]
 #version = {attr = "py_ballisticcalc.__version__"}
 
 
 [project.optional-dependencies]
-exts = ['py_ballisticcalc.exts==2.0.0b1']
+exts = ['py_ballisticcalc.exts==2.0.0b2']
 lint = ['pylint', 'flake8']
 charts = ['matplotlib', 'pandas']
```

### Comparing `py_ballisticcalc-2.0.0b1/tests/test_atmosphere.py` & `py_ballisticcalc-2.0.0b2/tests/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/tests/test_computer.py` & `py_ballisticcalc-2.0.0b2/tests/test_computer.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/tests/test_danger_space.py` & `py_ballisticcalc-2.0.0b2/tests/test_danger_space.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/tests/test_mbc.py` & `py_ballisticcalc-2.0.0b2/tests/test_mbc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/tests/test_trajectory.py` & `py_ballisticcalc-2.0.0b2/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b1/tests/test_units.py` & `py_ballisticcalc-2.0.0b2/tests/test_units.py`

 * *Files identical despite different names*

