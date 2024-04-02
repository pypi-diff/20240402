# Comparing `tmp/pyDSA_gui-1.5.3.tar.gz` & `tmp/pyDSA_gui-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDSA_gui-1.5.3.tar", last modified: Fri Jun  3 18:52:47 2022, max compression
+gzip compressed data, was "pyDSA_gui-1.5.4.tar", last modified: Tue Apr  2 19:49:43 2024, max compression
```

## Comparing `pyDSA_gui-1.5.3.tar` & `pyDSA_gui-1.5.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 18:52:47.879970 pyDSA_gui-1.5.3/
--rw-r--r--   0 root         (0) root         (0)    35147 2019-01-14 19:49:42.000000 pyDSA_gui-1.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3190 2022-06-03 18:52:47.879970 pyDSA_gui-1.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2514 2020-06-07 10:03:20.000000 pyDSA_gui-1.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 18:52:47.879970 pyDSA_gui-1.5.3/pyDSA_gui/
--rw-r--r--   0 root         (0) root         (0)    26420 2021-03-12 20:52:19.000000 pyDSA_gui-1.5.3/pyDSA_gui/MPLWidget.py
--rw-r--r--   0 root         (0) root         (0)     5963 2019-07-05 20:19:35.000000 pyDSA_gui-1.5.3/pyDSA_gui/MainApp.py
--rw-r--r--   0 root         (0) root         (0)      957 2019-05-21 18:39:51.000000 pyDSA_gui-1.5.3/pyDSA_gui/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63682 2019-06-14 17:41:00.000000 pyDSA_gui-1.5.3/pyDSA_gui/design.py
--rw-r--r--   0 root         (0) root         (0)    52001 2022-06-03 18:44:50.000000 pyDSA_gui-1.5.3/pyDSA_gui/dsa_backend.py
--rw-r--r--   0 root         (0) root         (0)     1477 2019-04-12 19:56:19.000000 pyDSA_gui-1.5.3/pyDSA_gui/files_helper.py
--rw-r--r--   0 root         (0) root         (0)     5005 2019-01-22 00:34:47.000000 pyDSA_gui-1.5.3/pyDSA_gui/log.py
--rw-r--r--   0 root         (0) root         (0)    13734 2019-06-06 23:11:55.000000 pyDSA_gui-1.5.3/pyDSA_gui/mpl_handlers.py
--rw-r--r--   0 root         (0) root         (0)     1157 2019-04-17 22:00:47.000000 pyDSA_gui-1.5.3/pyDSA_gui/tab.py
--rw-r--r--   0 root         (0) root         (0)    10389 2019-07-05 20:19:35.000000 pyDSA_gui-1.5.3/pyDSA_gui/tabanalyze.py
--rw-r--r--   0 root         (0) root         (0)     7552 2021-03-20 22:16:42.000000 pyDSA_gui-1.5.3/pyDSA_gui/tabdata.py
--rw-r--r--   0 root         (0) root         (0)     5630 2019-06-23 10:19:11.000000 pyDSA_gui-1.5.3/pyDSA_gui/tabedges.py
--rw-r--r--   0 root         (0) root         (0)     8355 2022-06-03 18:45:12.000000 pyDSA_gui-1.5.3/pyDSA_gui/tabfits.py
--rw-r--r--   0 root         (0) root         (0)    12714 2019-05-31 12:16:51.000000 pyDSA_gui-1.5.3/pyDSA_gui/tabimport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 18:52:47.879970 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3190 2022-06-03 18:52:47.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2022-06-03 18:52:47.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-03 18:52:47.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-06-03 18:52:47.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-04-07 02:47:28.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2022-06-03 18:52:47.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-06-03 18:52:47.000000 pyDSA_gui-1.5.3/pyDSA_gui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-03 18:52:47.879970 pyDSA_gui-1.5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1841 2022-06-03 18:51:36.000000 pyDSA_gui-1.5.3/setup.py
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:49:43.550991 pyDSA_gui-1.5.4/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    35147 2019-01-14 19:49:42.000000 pyDSA_gui-1.5.4/LICENSE
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     3249 2024-04-02 19:49:43.550991 pyDSA_gui-1.5.4/PKG-INFO
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     2439 2024-04-02 19:08:16.000000 pyDSA_gui-1.5.4/README.md
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:49:43.494323 pyDSA_gui-1.5.4/pyDSA_gui/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    26420 2021-03-12 20:52:19.000000 pyDSA_gui-1.5.4/pyDSA_gui/MPLWidget.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     5963 2019-07-05 20:19:35.000000 pyDSA_gui-1.5.4/pyDSA_gui/MainApp.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)      957 2019-05-21 18:39:51.000000 pyDSA_gui-1.5.4/pyDSA_gui/__init__.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    63682 2019-06-14 17:41:00.000000 pyDSA_gui-1.5.4/pyDSA_gui/design.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    52001 2024-04-02 19:45:06.000000 pyDSA_gui-1.5.4/pyDSA_gui/dsa_backend.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     1477 2019-04-12 19:56:19.000000 pyDSA_gui-1.5.4/pyDSA_gui/files_helper.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     5005 2019-01-22 00:34:47.000000 pyDSA_gui-1.5.4/pyDSA_gui/log.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    13734 2019-06-06 23:11:55.000000 pyDSA_gui-1.5.4/pyDSA_gui/mpl_handlers.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     1157 2019-04-17 22:00:47.000000 pyDSA_gui-1.5.4/pyDSA_gui/tab.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    10389 2019-07-05 20:19:35.000000 pyDSA_gui-1.5.4/pyDSA_gui/tabanalyze.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     4960 2024-04-02 19:07:32.000000 pyDSA_gui-1.5.4/pyDSA_gui/tabdata.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     5630 2019-06-23 10:19:11.000000 pyDSA_gui-1.5.4/pyDSA_gui/tabedges.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     8355 2022-06-03 18:45:12.000000 pyDSA_gui-1.5.4/pyDSA_gui/tabfits.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    12714 2019-05-31 12:16:51.000000 pyDSA_gui-1.5.4/pyDSA_gui/tabimport.py
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:49:43.550991 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     3249 2024-04-02 19:49:43.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/PKG-INFO
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)      584 2024-04-02 19:49:43.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)        1 2024-04-02 19:49:43.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       48 2024-04-02 19:49:43.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/entry_points.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)        1 2019-04-07 02:47:28.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/not-zip-safe
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       59 2024-04-02 19:49:43.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/requires.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       10 2024-04-02 19:49:43.000000 pyDSA_gui-1.5.4/pyDSA_gui.egg-info/top_level.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       38 2024-04-02 19:49:43.550991 pyDSA_gui-1.5.4/setup.cfg
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     1819 2024-04-02 19:49:12.000000 pyDSA_gui-1.5.4/setup.py
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:49:43.550991 pyDSA_gui-1.5.4/tests/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    10648 2022-06-03 18:01:59.000000 pyDSA_gui-1.5.4/tests/test_gui.py
```

### Comparing `pyDSA_gui-1.5.3/LICENSE` & `pyDSA_gui-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/PKG-INFO` & `pyDSA_gui-1.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: pyDSA_gui
-Version: 1.5.3
+Version: 1.5.4
 Summary: GUI for pyDSA_core
 Home-page: https://framagit.org/gabylaunay/pyDSA_gui
 Author: Gaby Launay
 Author-email: gaby.launay@protonmail.com
 Keywords: GUI DSA drop shape contact angle hysteresis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyQt5
+Requires-Dist: pyDSA_core==1.4.1
+Requires-Dist: numpy
+Requires-Dist: matplotlib>=2.2.0
+Requires-Dist: xlsxwriter
 
 <div align="center">
   <img width=500px" src="https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/pyDSA_logo_text.svg"><br><br>
 </div>
 
 
 # Drop shape analysis software.
@@ -96,13 +101,13 @@
 }
 
 ```
 
 ## Issues and bugs
 
 PyDSA is hosted on [Framagit](https://framagit.org/gabylaunay/pyDSA_gui).
-If PyDSA crashes or behaves abnormally, you can report [here](https://framagit.org/gabylaunay/pyDSA_gui/issues) or just send me an email at [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com).
+If PyDSA crashes or behaves abnormally, just send me an email at [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com).
 Any of the followings will greatly help me fix the issue:
 
 - A description of the problem
 - The logs from the terminal
 - A test case to reproduce the problem
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1 Name: pyDSA_gui Version: 1.5.3 Summary: GUI for
+Metadata-Version: 2.1 Name: pyDSA_gui Version: 1.5.4 Summary: GUI for
 pyDSA_core Home-page: https://framagit.org/gabylaunay/pyDSA_gui Author: Gaby
 Launay Author-email: gaby.launay@protonmail.com Keywords: GUI DSA drop shape
 contact angle hysteresis Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Operating System :: POSIX ::
-Linux Description-Content-Type: text/markdown License-File: LICENSE
+Linux Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: pyQt5 Requires-Dist: pyDSA_core==1.4.1 Requires-Dist: numpy Requires-
+Dist: matplotlib>=2.2.0 Requires-Dist: xlsxwriter
        [https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/
                              pyDSA_logo_text.svg]
 
 # Drop shape analysis software. PyDSA is a software for drop shape analysis. It
 allows to measure the properties of droplets in contact with solids (contact
 angle, droplet volume, evaporation rate, displacement velocity, ...) through an
 intuitive interface. PyDSA is developed in Python and use Qt5 for it graphical
@@ -35,12 +37,11 @@
 PyDSA have been usefull for you, please consider citing it: ``` Launay G.
 PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/
 pyDSA_core [Online; accessed ]. ``` bibtex entry: ``` bibtex @Misc
 {launay_pydsa_2018, author = {Gaby Launay}, title = {{PyDSA}: Drop shape
 analysis in {Python}}, year = {2018--}, url = "https://framagit.org/gabylaunay/
 pyDSA_core", note = {[Online; accessed ]} } ``` ## Issues and bugs PyDSA is
 hosted on [Framagit](https://framagit.org/gabylaunay/pyDSA_gui). If PyDSA
-crashes or behaves abnormally, you can report [here](https://framagit.org/
-gabylaunay/pyDSA_gui/issues) or just send me an email at
+crashes or behaves abnormally, just send me an email at
 [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com). Any of the
 followings will greatly help me fix the issue: - A description of the problem -
 The logs from the terminal - A test case to reproduce the problem
```

### Comparing `pyDSA_gui-1.5.3/README.md` & `pyDSA_gui-1.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -78,13 +78,13 @@
 }
 
 ```
 
 ## Issues and bugs
 
 PyDSA is hosted on [Framagit](https://framagit.org/gabylaunay/pyDSA_gui).
-If PyDSA crashes or behaves abnormally, you can report [here](https://framagit.org/gabylaunay/pyDSA_gui/issues) or just send me an email at [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com).
+If PyDSA crashes or behaves abnormally, just send me an email at [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com).
 Any of the followings will greatly help me fix the issue:
 
 - A description of the problem
 - The logs from the terminal
 - A test case to reproduce the problem
```

#### html2text {}

```diff
@@ -26,12 +26,11 @@
 PyDSA have been usefull for you, please consider citing it: ``` Launay G.
 PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/
 pyDSA_core [Online; accessed ]. ``` bibtex entry: ``` bibtex @Misc
 {launay_pydsa_2018, author = {Gaby Launay}, title = {{PyDSA}: Drop shape
 analysis in {Python}}, year = {2018--}, url = "https://framagit.org/gabylaunay/
 pyDSA_core", note = {[Online; accessed ]} } ``` ## Issues and bugs PyDSA is
 hosted on [Framagit](https://framagit.org/gabylaunay/pyDSA_gui). If PyDSA
-crashes or behaves abnormally, you can report [here](https://framagit.org/
-gabylaunay/pyDSA_gui/issues) or just send me an email at
+crashes or behaves abnormally, just send me an email at
 [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com). Any of the
 followings will greatly help me fix the issue: - A description of the problem -
 The logs from the terminal - A test case to reproduce the problem
```

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/MPLWidget.py` & `pyDSA_gui-1.5.4/pyDSA_gui/MPLWidget.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/MainApp.py` & `pyDSA_gui-1.5.4/pyDSA_gui/MainApp.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/__init__.py` & `pyDSA_gui-1.5.4/pyDSA_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/design.py` & `pyDSA_gui-1.5.4/pyDSA_gui/design.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/dsa_backend.py` & `pyDSA_gui-1.5.4/pyDSA_gui/dsa_backend.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/files_helper.py` & `pyDSA_gui-1.5.4/pyDSA_gui/files_helper.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/log.py` & `pyDSA_gui-1.5.4/pyDSA_gui/log.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/mpl_handlers.py` & `pyDSA_gui-1.5.4/pyDSA_gui/mpl_handlers.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/tab.py` & `pyDSA_gui-1.5.4/pyDSA_gui/tab.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/tabanalyze.py` & `pyDSA_gui-1.5.4/pyDSA_gui/tabanalyze.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/tabdata.py` & `pyDSA_gui-1.5.4/pyDSA_gui/tabdata.py`

 * *Files 22% similar despite different names*

```diff
@@ -72,34 +72,14 @@
                     continue
             data.append(list(val))
             headers.append(f'{quant.replace(",", "")}'
                            f' [{unit.replace(",", "")}]')
         data = np.array(data, dtype=float).transpose()
         return data, headers
 
-    def _get_edges_to_export(self):
-        data = []
-        headers = ["frame", "time", "x", "y"]
-        for i in len(self.dsa.edges):
-            pass
-        for quant in self.app.plottable_quant:
-            val, _, unit = self.dsa.get_plotable_quantity(quant, smooth=0)
-            # check that length matches
-            if len(data) > 0:
-                if len(data[0]) != len(val):
-                    self.log.log(f"Quantity {quant} does not have the right"
-                                 f" length ({len(val)} instead of"
-                                 f" {len(data[0])})", level=3)
-                    continue
-            data.append(list(val))
-            headers.append(f'{quant.replace(",", "")}'
-                           f' [{unit.replace(",", "")}]')
-        data = np.array(data, dtype=float).transpose()
-        return data, headers
-
     def _get_filepath_to_export(self, filepath, ext):
         # get fiel to save to
         if filepath is None:
             filepath, _ = select_new_file("Save as")
             if filepath == "":
                 return None
         # Add extension
@@ -129,56 +109,14 @@
         import xlsxwriter
         try:
             # Get filepath
             filepath = self._get_filepath_to_export(filepath, ext=".xlsx")
             if filepath is None:
                 return None
             # get and store data
-            data, headers = self._get_data_to_export()
-            date = datetime.now().strftime("%y-%m-%d %I:%M%p")
-            wb = xlsxwriter.Workbook(filepath, {'nan_inf_to_errors': True})
-            ws = wb.add_worksheet()
-            # write headers
-            ws.write('A1', "File")
-            ws.write('A2', "Analysis date")
-            ws.merge_range('B1:H1', f"{self.dsa.filepath}")
-            ws.merge_range('B2:H2', f"{date}")
-            ws.write_row(2, 0, headers)
-            for i, row in enumerate(data):
-                ws.write_row(i+3, 0, row)
-            wb.close()
-            self.log.log(f"Saved data in {filepath}", level=1)
-        except:
-            self.log.log_unknown_exception()
-
-    def export_edges_as_csv(self, toggle, filepath=None):
-        try:
-            # Get filepath
-            filepath = self._get_filepath_to_export(filepath, ext=".csv")
-            if filepath is None:
-                return None
-            # get and store data
-            data, headers = self._get_data_to_export()
-            date = datetime.now().strftime("%y-%m-%d %I:%M%p")
-            np.savetxt(filepath, data, delimiter=', ',
-                       header=f"File: {self.dsa.filepath}\n"
-                       f"Analysis date: {date}\n"
-                       + ", ".join(headers))
-            self.log.log(f"Saved data in {filepath}", level=1)
-        except:
-            self.log.log_unknown_exception()
-
-    def export_edges_as_xlsx(self, toggle, filepath=None):
-        import xlsxwriter
-        try:
-            # Get filepath
-            filepath = self._get_filepath_to_export(filepath, ext=".xlsx")
-            if filepath is None:
-                return None
-            # get and store data
             data, headers = self._get_data_to_export()
             date = datetime.now().strftime("%y-%m-%d %I:%M%p")
             wb = xlsxwriter.Workbook(filepath, {'nan_inf_to_errors': True})
             ws = wb.add_worksheet()
             # write headers
             ws.write('A1', "File")
             ws.write('A2', "Analysis date")
```

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/tabedges.py` & `pyDSA_gui-1.5.4/pyDSA_gui/tabedges.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/tabfits.py` & `pyDSA_gui-1.5.4/pyDSA_gui/tabfits.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui/tabimport.py` & `pyDSA_gui-1.5.4/pyDSA_gui/tabimport.py`

 * *Files identical despite different names*

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui.egg-info/PKG-INFO` & `pyDSA_gui-1.5.4/pyDSA_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
-Name: pyDSA-gui
-Version: 1.5.3
+Name: pyDSA_gui
+Version: 1.5.4
 Summary: GUI for pyDSA_core
 Home-page: https://framagit.org/gabylaunay/pyDSA_gui
 Author: Gaby Launay
 Author-email: gaby.launay@protonmail.com
 Keywords: GUI DSA drop shape contact angle hysteresis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyQt5
+Requires-Dist: pyDSA_core==1.4.1
+Requires-Dist: numpy
+Requires-Dist: matplotlib>=2.2.0
+Requires-Dist: xlsxwriter
 
 <div align="center">
   <img width=500px" src="https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/pyDSA_logo_text.svg"><br><br>
 </div>
 
 
 # Drop shape analysis software.
@@ -96,13 +101,13 @@
 }
 
 ```
 
 ## Issues and bugs
 
 PyDSA is hosted on [Framagit](https://framagit.org/gabylaunay/pyDSA_gui).
-If PyDSA crashes or behaves abnormally, you can report [here](https://framagit.org/gabylaunay/pyDSA_gui/issues) or just send me an email at [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com).
+If PyDSA crashes or behaves abnormally, just send me an email at [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com).
 Any of the followings will greatly help me fix the issue:
 
 - A description of the problem
 - The logs from the terminal
 - A test case to reproduce the problem
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1 Name: pyDSA-gui Version: 1.5.3 Summary: GUI for
+Metadata-Version: 2.1 Name: pyDSA_gui Version: 1.5.4 Summary: GUI for
 pyDSA_core Home-page: https://framagit.org/gabylaunay/pyDSA_gui Author: Gaby
 Launay Author-email: gaby.launay@protonmail.com Keywords: GUI DSA drop shape
 contact angle hysteresis Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Operating System :: POSIX ::
-Linux Description-Content-Type: text/markdown License-File: LICENSE
+Linux Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: pyQt5 Requires-Dist: pyDSA_core==1.4.1 Requires-Dist: numpy Requires-
+Dist: matplotlib>=2.2.0 Requires-Dist: xlsxwriter
        [https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/
                              pyDSA_logo_text.svg]
 
 # Drop shape analysis software. PyDSA is a software for drop shape analysis. It
 allows to measure the properties of droplets in contact with solids (contact
 angle, droplet volume, evaporation rate, displacement velocity, ...) through an
 intuitive interface. PyDSA is developed in Python and use Qt5 for it graphical
@@ -35,12 +37,11 @@
 PyDSA have been usefull for you, please consider citing it: ``` Launay G.
 PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/
 pyDSA_core [Online; accessed ]. ``` bibtex entry: ``` bibtex @Misc
 {launay_pydsa_2018, author = {Gaby Launay}, title = {{PyDSA}: Drop shape
 analysis in {Python}}, year = {2018--}, url = "https://framagit.org/gabylaunay/
 pyDSA_core", note = {[Online; accessed ]} } ``` ## Issues and bugs PyDSA is
 hosted on [Framagit](https://framagit.org/gabylaunay/pyDSA_gui). If PyDSA
-crashes or behaves abnormally, you can report [here](https://framagit.org/
-gabylaunay/pyDSA_gui/issues) or just send me an email at
+crashes or behaves abnormally, just send me an email at
 [gaby.launay@protonmail.com](mailto:gaby.launay@protonmail.com). Any of the
 followings will greatly help me fix the issue: - A description of the problem -
 The logs from the terminal - A test case to reproduce the problem
```

### Comparing `pyDSA_gui-1.5.3/pyDSA_gui.egg-info/SOURCES.txt` & `pyDSA_gui-1.5.4/pyDSA_gui.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 pyDSA_gui/tabimport.py
 pyDSA_gui.egg-info/PKG-INFO
 pyDSA_gui.egg-info/SOURCES.txt
 pyDSA_gui.egg-info/dependency_links.txt
 pyDSA_gui.egg-info/entry_points.txt
 pyDSA_gui.egg-info/not-zip-safe
 pyDSA_gui.egg-info/requires.txt
-pyDSA_gui.egg-info/top_level.txt
+pyDSA_gui.egg-info/top_level.txt
+tests/test_gui.py
```

### Comparing `pyDSA_gui-1.5.3/setup.py` & `pyDSA_gui-1.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyDSA_gui',
-    version='1.5.3',
+    version='1.5.4',
     description='GUI for pyDSA_core',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://framagit.org/gabylaunay/pyDSA_gui',
     author='Gaby Launay',
     author_email='gaby.launay@protonmail.com',
     classifiers=[
@@ -37,16 +37,16 @@
         'Programming Language :: Python :: 3.5',
         'Natural Language :: English',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: POSIX :: Linux',
     ],
     keywords='GUI DSA drop shape contact angle hysteresis',
     packages=find_packages(exclude=['contrib', 'docs', 'tests', 'samples']),
-    install_requires=['pyQt5', 'pyDSA_core==1.4.0', 'IMTreatment==1.2.0',
-                      'numpy', 'matplotlib>=2.2.0', 'xlsxwriter'],
+    install_requires=['pyQt5', 'pyDSA_core==1.4.1', 'numpy',
+                      'matplotlib>=2.2.0', 'xlsxwriter'],
     extras_require={},
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     entry_points={
         'console_scripts': [
             'pyDSA = pyDSA_gui.MainApp:run',
         ],
```

