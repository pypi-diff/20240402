# Comparing `tmp/smadi-0.2.4.tar.gz` & `tmp/smadi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smadi-0.2.4.tar", last modified: Sat Mar 30 22:46:21 2024, max compression
+gzip compressed data, was "smadi-0.2.5.tar", last modified: Tue Apr  2 00:50:29 2024, max compression
```

## Comparing `smadi-0.2.4.tar` & `smadi-0.2.5.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.054018 smadi-0.2.4/
--rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.4/.coveragerc
--rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.4/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.4/.readthedocs.yml
--rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.4/AUTHORS.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.4/CHANGELOG.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.4/CONTRIBUTING.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.4/LICENSE.txt
--rw-r--r--   0 m294      (1000) m294      (1000)     2982 2024-03-30 22:46:21.054018 smadi-0.2.4/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)     1591 2024-03-30 14:53:43.000000 smadi-0.2.4/README.rst
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.050018 smadi-0.2.4/docs/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/Makefile
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.050018 smadi-0.2.4/docs/_static/
--rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/_static/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/authors.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/changelog.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     9724 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/conf.py
--rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/contributing.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/index.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/license.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/readme.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.4/docs/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.4/pyproject.toml
--rw-rw-r--   0 m294      (1000) m294      (1000)     1479 2024-03-30 22:46:21.054018 smadi-0.2.4/setup.cfg
--rw-rw-r--   0 m294      (1000) m294      (1000)      667 2024-03-30 22:45:18.000000 smadi-0.2.4/setup.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.046018 smadi-0.2.4/src/
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.050018 smadi-0.2.4/src/smadi/
--rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.4/src/smadi/__init__.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    17750 2024-03-30 15:08:06.000000 smadi-0.2.4/src/smadi/anomaly_detectors.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    15269 2024-03-30 15:08:13.000000 smadi-0.2.4/src/smadi/climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-03-29 20:29:27.000000 smadi-0.2.4/src/smadi/data_reader.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8775 2024-03-29 20:29:06.000000 smadi-0.2.4/src/smadi/indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     5258 2024-03-30 14:57:24.000000 smadi-0.2.4/src/smadi/map.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     1724 2024-03-30 14:57:33.000000 smadi-0.2.4/src/smadi/metadata.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     7461 2024-03-30 14:58:05.000000 smadi-0.2.4/src/smadi/plot.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8623 2024-03-29 20:28:21.000000 smadi-0.2.4/src/smadi/preprocess.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4011 2024-03-29 20:27:47.000000 smadi-0.2.4/src/smadi/utils.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    11088 2024-03-30 14:58:24.000000 smadi-0.2.4/src/smadi/workflow.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.054018 smadi-0.2.4/src/smadi.egg-info/
--rw-r--r--   0 m294      (1000) m294      (1000)     2982 2024-03-30 22:46:21.000000 smadi-0.2.4/src/smadi.egg-info/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)      862 2024-03-30 22:46:21.000000 smadi-0.2.4/src/smadi.egg-info/SOURCES.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-03-30 22:46:21.000000 smadi-0.2.4/src/smadi.egg-info/dependency_links.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-03-30 15:01:49.000000 smadi-0.2.4/src/smadi.egg-info/not-zip-safe
--rw-rw-r--   0 m294      (1000) m294      (1000)      315 2024-03-30 22:46:21.000000 smadi-0.2.4/src/smadi.egg-info/requires.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-03-30 22:46:21.000000 smadi-0.2.4/src/smadi.egg-info/top_level.txt
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-03-30 22:46:21.054018 smadi-0.2.4/tests/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.4/tests/conftest.py
--rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.4/tests/data_sample.csv
--rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.4/tests/test_climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.4/tests/test_indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.4/tox.ini
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.946805 smadi-0.2.5/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.5/.coveragerc
+-rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.5/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.5/.readthedocs.yml
+-rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.5/AUTHORS.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.5/CHANGELOG.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.5/CONTRIBUTING.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.5/LICENSE.txt
+-rw-r--r--   0 m294      (1000) m294      (1000)     2982 2024-04-02 00:50:29.946805 smadi-0.2.5/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1591 2024-03-30 14:53:43.000000 smadi-0.2.5/README.rst
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.898804 smadi-0.2.5/docs/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/Makefile
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.898804 smadi-0.2.5/docs/_static/
+-rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/_static/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/authors.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/changelog.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9724 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/conf.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/contributing.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/index.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/license.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/readme.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.5/pyproject.toml
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1479 2024-04-02 00:50:29.950805 smadi-0.2.5/setup.cfg
+-rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-02 00:50:00.000000 smadi-0.2.5/setup.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.878804 smadi-0.2.5/src/
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.902804 smadi-0.2.5/src/smadi/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.5/src/smadi/__init__.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    19649 2024-04-01 23:41:33.000000 smadi-0.2.5/src/smadi/anomaly_detectors.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    15269 2024-03-30 15:08:13.000000 smadi-0.2.5/src/smadi/climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-03-29 20:29:27.000000 smadi-0.2.5/src/smadi/data_reader.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8775 2024-03-29 20:29:06.000000 smadi-0.2.5/src/smadi/indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     5258 2024-03-30 14:57:24.000000 smadi-0.2.5/src/smadi/map.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1813 2024-04-01 23:41:33.000000 smadi-0.2.5/src/smadi/metadata.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     7461 2024-03-30 14:58:05.000000 smadi-0.2.5/src/smadi/plot.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8623 2024-03-29 20:28:21.000000 smadi-0.2.5/src/smadi/preprocess.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4522 2024-04-01 23:09:32.000000 smadi-0.2.5/src/smadi/utils.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    14711 2024-04-01 23:41:33.000000 smadi-0.2.5/src/smadi/workflow.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.946805 smadi-0.2.5/src/smadi.egg-info/
+-rw-r--r--   0 m294      (1000) m294      (1000)     2982 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)      898 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/entry_points.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-03-30 15:01:49.000000 smadi-0.2.5/src/smadi.egg-info/not-zip-safe
+-rw-rw-r--   0 m294      (1000) m294      (1000)      315 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/requires.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/top_level.txt
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.946805 smadi-0.2.5/tests/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.5/tests/conftest.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.5/tests/data_sample.csv
+-rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.5/tests/test_climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.5/tests/test_indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.5/tox.ini
```

### Comparing `smadi-0.2.4/.coveragerc` & `smadi-0.2.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/.gitignore` & `smadi-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/.readthedocs.yml` & `smadi-0.2.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/CONTRIBUTING.rst` & `smadi-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/LICENSE.txt` & `smadi-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/PKG-INFO` & `smadi-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smadi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Add a short description here!
 Home-page: https://github.com/MuhammedM294/smadi
 Author: MuhammedM294
 Author-email: muhammedaabdelaal@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/MuhammedM294/smadi
```

### Comparing `smadi-0.2.4/README.rst` & `smadi-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/docs/Makefile` & `smadi-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/docs/conf.py` & `smadi-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/docs/index.rst` & `smadi-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/setup.cfg` & `smadi-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/setup.py` & `smadi-0.2.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,22 @@
     Learn more under: https://pyscaffold.org/
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
-        setup(version="0.2.4")
+        setup(
+            version="0.2.5",
+            entry_points={
+                "console_scripts": [
+                    "run = smadi.workflow:main",
+                ]
+            },
+        )
 
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
```

### Comparing `smadi-0.2.4/src/smadi/__init__.py` & `smadi-0.2.5/src/smadi/__init__.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/anomaly_detectors.py` & `smadi-0.2.5/src/smadi/anomaly_detectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,66 @@
 
         """
         self.clim_df = self._preprocess().copy()
 
         return filter_df(self.clim_df, **kwargs)
 
 
+class AbsoluteAnomaly(AnomalyDetector):
+    """
+    A class for detecting anomalies in time series data based on the absolute deviation value from the climate normal.
+
+    SMA = x - ref
+
+        where:
+        x: the average value of the variable in the time series data. It can be any of the following:
+        Daily average, weekly average, monthly average, etc.
+        ref: the long-term mean (μ) or median (η) of the variable(the climate normal).
+
+    """
+
+    def __init__(
+        self,
+        df: pd.DataFrame,
+        variable: str,
+        fillna: bool = False,
+        fillna_window_size: int = None,
+        smoothing=False,
+        smooth_window_size=None,
+        timespan: List[str] = None,
+        time_step: str = "month",
+        normal_metrics: List[str] = ["mean"],
+    ):
+        super().__init__(
+            df,
+            variable,
+            fillna,
+            fillna_window_size,
+            smoothing,
+            smooth_window_size,
+            timespan,
+            time_step,
+            normal_metrics,
+        )
+
+    def _preprocess(self, **kwargs) -> pd.DataFrame:
+        super()._preprocess(**kwargs)
+        return self.clim_df
+
+    def detect_anomaly(self, **kwargs) -> pd.DataFrame:
+        super().detect_anomaly(**kwargs)
+
+        for metric in self.normal_metrics:
+            self.clim_df[f"abs-{metric}"] = (
+                self.clim_df[f"{self.var}-avg"] - self.clim_df[f"norm-{metric}"]
+            )
+
+        return filter_df(self.clim_df, **kwargs)
+
+
 class ZScore(AnomalyDetector):
     """
     A class for detecting anomalies in time series data based on the Z-Score method.
 
     z_score = (x - μ) / σ
 
         where:
@@ -607,7 +659,23 @@
         super().detect_anomaly(**kwargs)
         for dist in self.dist:
             self.clim_df[f"{dist}"] = self.clim_df.groupby(self.groupby_param)[
                 f"{self.var}-avg"
             ].transform(para_dis, dist=dist)
 
         return filter_df(self.clim_df, **kwargs)
+
+
+if __name__ == "__main__":
+
+    from pathlib import Path
+    from smadi.data_reader import extract_obs_ts
+
+    ascat_path = Path("/home/m294/VSA/Code/datasets")
+
+    po = 4854801
+    sm_ts = extract_obs_ts(po, ascat_path, obs_type="sm", read_bulk=False)
+    df = AbsoluteAnomaly(
+        sm_ts, "sm", time_step="month", normal_metrics=["mean", "median"]
+    ).detect_anomaly()
+
+    print(df)
```

### Comparing `smadi-0.2.4/src/smadi/climatology.py` & `smadi-0.2.5/src/smadi/climatology.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/data_reader.py` & `smadi-0.2.5/src/smadi/data_reader.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/indicators.py` & `smadi-0.2.5/src/smadi/indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/map.py` & `smadi-0.2.5/src/smadi/map.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/metadata.py` & `smadi-0.2.5/src/smadi/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,21 @@
     SMDI,
     SMCA,
     SMAD,
     SMCI,
     SMDS,
     ESSMI,
     ParaDis,
+    AbsoluteAnomaly,
 )
 
 # Supported anomaly detection methods
 _Detectors = {
+    "abs-mean": AbsoluteAnomaly,
+    "abs-median": AbsoluteAnomaly,
     "zscore": ZScore,
     "smapi-mean": SMAPI,
     "smapi-median": SMAPI,
     "smdi": SMDI,
     "smca-mean": SMCA,
     "smca-median": SMCA,
     "smad": SMAD,
```

### Comparing `smadi-0.2.4/src/smadi/plot.py` & `smadi-0.2.5/src/smadi/plot.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/preprocess.py` & `smadi-0.2.5/src/smadi/preprocess.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/src/smadi/utils.py` & `smadi-0.2.5/src/smadi/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import requests
 from functools import wraps
 from time import time
 from io import StringIO
 import pycountry
 import pandas as pd
 
+from fibgrid.realization import FibLandGrid
+
 
 def create_logger(name, level=logging.DEBUG):
     """
     Create a logger with the given name and level
 
     parameters:
     ----------
@@ -126,15 +128,15 @@
         country = pycountry.countries.lookup(country_name)
         return country.alpha_3
     except LookupError:
         print("Country name not found.")
         return None
 
 
-def load_gpis_by_country(country, grid="fibgrid_n6600000", format="csv"):
+def load_gpis_by_country(country, res=6.25, format="csv"):
     """
     Load the GPIS based on the country name from the DGG API
     Source: https://dgg.geo.tuwien.ac.at/
 
     parameters:
     ----------
     country: str
@@ -151,23 +153,41 @@
         format of the data to be returned. Default is "csv". Supported formats are:
         - csv
         - json
     """
 
     country = get_country_code(country)
 
+    if res == 6.25:
+        grid = "fibgrid_n6600000"
+    elif res == 12.5:
+        grid = "fibgrid_n1650000"
+    elif res == 25:
+        grid = "fibgrid_n430000"
+
     # Construct the URL based on the provided country name, grid, and format
-    url = f"https://dgg.geo.tuwien.ac.at/get_points/?grid={grid}&country={country.upper()}&format=csv"
+    url = f"https://dgg.geo.tuwien.ac.at/get_points/?grid={grid}&country={country.upper()}&format={format}"
 
     try:
         response = requests.get(url)
 
         if response.status_code == 200:
             csv_data = response.content.decode("utf-8")
             df = pd.read_csv(StringIO(csv_data))
             return df
         else:
             print(f"Failed to download CSV file. Status code: {response.status_code}")
             return None
     except Exception as e:
         print(f"An error occurred: {str(e)}")
         return None
+
+
+def get_gpis_from_bbox(bbox, res=6.25):
+
+    lonmin, lonmax, latmin, latmax = bbox
+    grid = FibLandGrid(res)
+    gpis = grid.get_bbox_grid_points(
+        lonmin=lonmin, lonmax=lonmax, latmin=latmin, latmax=latmax, both=True
+    )
+
+    return pd.DataFrame({"point": gpis[0], "lon": gpis[1], "lat": gpis[2]})
```

### Comparing `smadi-0.2.4/src/smadi.egg-info/PKG-INFO` & `smadi-0.2.5/src/smadi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smadi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Add a short description here!
 Home-page: https://github.com/MuhammedM294/smadi
 Author: MuhammedM294
 Author-email: muhammedaabdelaal@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/MuhammedM294/smadi
```

### Comparing `smadi-0.2.4/src/smadi.egg-info/SOURCES.txt` & `smadi-0.2.5/src/smadi.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/smadi/plot.py
 src/smadi/preprocess.py
 src/smadi/utils.py
 src/smadi/workflow.py
 src/smadi.egg-info/PKG-INFO
 src/smadi.egg-info/SOURCES.txt
 src/smadi.egg-info/dependency_links.txt
+src/smadi.egg-info/entry_points.txt
 src/smadi.egg-info/not-zip-safe
 src/smadi.egg-info/requires.txt
 src/smadi.egg-info/top_level.txt
 tests/conftest.py
 tests/data_sample.csv
 tests/test_climatology.py
 tests/test_indicators.py
```

### Comparing `smadi-0.2.4/tests/conftest.py` & `smadi-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/tests/data_sample.csv` & `smadi-0.2.5/tests/data_sample.csv`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/tests/test_climatology.py` & `smadi-0.2.5/tests/test_climatology.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/tests/test_indicators.py` & `smadi-0.2.5/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.4/tox.ini` & `smadi-0.2.5/tox.ini`

 * *Files identical despite different names*

