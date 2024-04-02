# Comparing `tmp/icalreporting-0.1.1.tar.gz` & `tmp/icalreporting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icalreporting-0.1.1.tar", last modified: Tue Oct 10 18:27:48 2023, max compression
+gzip compressed data, was "icalreporting-0.1.2.tar", last modified: Tue Apr  2 14:28:55 2024, max compression
```

## Comparing `icalreporting-0.1.1.tar` & `icalreporting-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 j.gressier (2084770372) 706199157        0 2023-10-10 18:27:48.665854 icalreporting-0.1.1/
--rw-r--r--   0 j.gressier (2084770372) 706199157     1074 2023-10-10 17:01:32.000000 icalreporting-0.1.1/LICENSE
--rw-r--r--   0 j.gressier (2084770372) 706199157     3731 2023-10-10 18:27:48.665403 icalreporting-0.1.1/PKG-INFO
--rw-r--r--   0 j.gressier (2084770372) 706199157     1458 2023-10-10 18:23:47.000000 icalreporting-0.1.1/README.md
-drwxr-xr-x   0 j.gressier (2084770372) 706199157        0 2023-10-10 18:27:48.658658 icalreporting-0.1.1/icalreporting/
--rw-r--r--   0 j.gressier (2084770372) 706199157       22 2023-10-10 18:27:28.000000 icalreporting-0.1.1/icalreporting/__init__.py
--rw-r--r--   0 j.gressier (2084770372) 706199157     5558 2023-10-10 17:46:27.000000 icalreporting-0.1.1/icalreporting/reporting.py
-drwxr-xr-x   0 j.gressier (2084770372) 706199157        0 2023-10-10 18:27:48.663990 icalreporting-0.1.1/icalreporting.egg-info/
--rw-r--r--   0 j.gressier (2084770372) 706199157     3731 2023-10-10 18:27:48.000000 icalreporting-0.1.1/icalreporting.egg-info/PKG-INFO
--rw-r--r--   0 j.gressier (2084770372) 706199157      269 2023-10-10 18:27:48.000000 icalreporting-0.1.1/icalreporting.egg-info/SOURCES.txt
--rw-r--r--   0 j.gressier (2084770372) 706199157        1 2023-10-10 18:27:48.000000 icalreporting-0.1.1/icalreporting.egg-info/dependency_links.txt
--rw-r--r--   0 j.gressier (2084770372) 706199157       99 2023-10-10 18:27:48.000000 icalreporting-0.1.1/icalreporting.egg-info/requires.txt
--rw-r--r--   0 j.gressier (2084770372) 706199157       14 2023-10-10 18:27:48.000000 icalreporting-0.1.1/icalreporting.egg-info/top_level.txt
--rw-r--r--   0 j.gressier (2084770372) 706199157     1693 2023-10-10 18:27:28.000000 icalreporting-0.1.1/pyproject.toml
--rw-r--r--   0 j.gressier (2084770372) 706199157       38 2023-10-10 18:27:48.665946 icalreporting-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:28:55.787813 icalreporting-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 14:28:40.000000 icalreporting-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-02 14:28:55.787813 icalreporting-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-02 14:28:40.000000 icalreporting-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:28:55.787813 icalreporting-0.1.2/icalreporting/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 14:28:40.000000 icalreporting-0.1.2/icalreporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-02 14:28:40.000000 icalreporting-0.1.2/icalreporting/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:28:55.787813 icalreporting-0.1.2/icalreporting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-02 14:28:55.000000 icalreporting-0.1.2/icalreporting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 14:28:55.000000 icalreporting-0.1.2/icalreporting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:28:55.000000 icalreporting-0.1.2/icalreporting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 14:28:55.000000 icalreporting-0.1.2/icalreporting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 14:28:55.000000 icalreporting-0.1.2/icalreporting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-02 14:28:40.000000 icalreporting-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:28:55.787813 icalreporting-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:28:55.787813 icalreporting-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-02 14:28:40.000000 icalreporting-0.1.2/tests/test_icalimport.py
```

### Comparing `icalreporting-0.1.1/LICENSE` & `icalreporting-0.1.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Jérémie GRESSIER
+Copyright (c) 2023 Jérémie GRESSIER
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `icalreporting-0.1.1/PKG-INFO` & `icalreporting-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: icalreporting
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reporting tools from ical files
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
-        Copyright (c) 2022 Jérémie GRESSIER
+        Copyright (c) 2023 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -57,17 +57,33 @@
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d32cf67a5fa242c88bb1568277f1d60e)](https://app.codacy.com/gh/jgressier/icalreporting/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)[![Doc](https://readthedocs.org/projects/icalreporting/badge/?version=latest)](https://readthedocs.org/projects/icalreporting/)
 [![Slack](https://img.shields.io/static/v1?logo=slack&label=slack&message=contact&style=flat)](https://join.slack.com/t/isae-opendev/shared_invite/zt-obqywf6r-UUuHR4_hc5iTzyL5bFCwpw
 )
 
 ### Features
 
+- able to load ical files and fill a pandas database
+- parse the pandas database to identify project and creates a worksheet tables
+- export to open document XLSX file
 
-### Installation and usage
+### Installation
 
 ```bash
 pip install --upgrade icalreporting
 ```
+This automatic installation will get needed dependencies. 
 
 ### Requirements
 
 see [requirements.txt](https://github.com/jgressier/icalreporting/blob/master/requirements.txt)
+
+### Usage
+
+When installed, you just need to put a set a ical files in a folder for a project. You will be able to create a reporting file with the following lines.
+
+```python
+from icalreporting.reporting import Project
+prj = Project(name="Big-Project", folder="examples/projectA", start="2023-01-01", end="2024-01-01")
+prj.load_ics()  # read files
+wb = prj.workbook()  # create workbook
+wb.save("projectA.xlsx")  # save it to file
+```
```

### Comparing `icalreporting-0.1.1/README.md` & `icalreporting-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -9,17 +9,33 @@
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d32cf67a5fa242c88bb1568277f1d60e)](https://app.codacy.com/gh/jgressier/icalreporting/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)[![Doc](https://readthedocs.org/projects/icalreporting/badge/?version=latest)](https://readthedocs.org/projects/icalreporting/)
 [![Slack](https://img.shields.io/static/v1?logo=slack&label=slack&message=contact&style=flat)](https://join.slack.com/t/isae-opendev/shared_invite/zt-obqywf6r-UUuHR4_hc5iTzyL5bFCwpw
 )
 
 ### Features
 
+- able to load ical files and fill a pandas database
+- parse the pandas database to identify project and creates a worksheet tables
+- export to open document XLSX file
 
-### Installation and usage
+### Installation
 
 ```bash
 pip install --upgrade icalreporting
 ```
+This automatic installation will get needed dependencies. 
 
 ### Requirements
 
-see [requirements.txt](https://github.com/jgressier/icalreporting/blob/master/requirements.txt)
+see [requirements.txt](https://github.com/jgressier/icalreporting/blob/master/requirements.txt)
+
+### Usage
+
+When installed, you just need to put a set a ical files in a folder for a project. You will be able to create a reporting file with the following lines.
+
+```python
+from icalreporting.reporting import Project
+prj = Project(name="Big-Project", folder="examples/projectA", start="2023-01-01", end="2024-01-01")
+prj.load_ics()  # read files
+wb = prj.workbook()  # create workbook
+wb.save("projectA.xlsx")  # save it to file
+```
```

### Comparing `icalreporting-0.1.1/icalreporting/reporting.py` & `icalreporting-0.1.2/icalreporting/reporting.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,29 @@
 from datetime import datetime, timedelta
 from ical.calendar_stream import IcsCalendarStream
 import pandas as pd
 from pathlib import Path
 import openpyxl as xl
 from openpyxl.utils.dataframe import dataframe_to_rows
 
+_default_startdate = "2020-01-01"
+_default_enddate = "2030-01-01"
 
 def ical_to_dframe(filename: Path, startdate: datetime, enddate: datetime):
+    """read a file in ICAL format and create events between 2 dates
+    can handle recurrent events
+
+    Args:
+        filename (Path): path name of ICAL file
+        startdate (datetime): starting date for events
+        enddate (datetime): ending date (included) for events
+
+    Returns:
+        DataFrame: as member of the class (date, year, month, h_begin, duration, name, description, begin) properties
+    """
     with filename.open() as ics_file:
         calendar = IcsCalendarStream.calendar_from_ics(ics_file.read())
     return pd.DataFrame(
         [
             {
                 "date": event.dtstart,
                 "year": event.dtstart.year,
@@ -37,43 +50,48 @@
                 "begin": event.dtstart,
             }
             for event in calendar.timeline.included(startdate, enddate)
         ]
     )
 
 
-class Project:
+class Project():
+    """Class Project, can read ICAL file, define tags and create worksheet 
+    """
     def __init__(
-        self, name: str, folder=None, start: str = "2020-01-01", end: str = "2030-01-01", default_WP="No_WP"
+        self, name: str, folder=None, start: str = _default_startdate, end: str = _default_enddate, default_WP="No_WP"
     ):
         self._name = name
         self._folder = name if folder is None else folder
         self._start = datetime.fromisoformat(start)
         self._end = datetime.fromisoformat(end) + timedelta(days=1)
         self._default_WP = default_WP
         print(self._end)
         print(f"> init project {self._name} in folder {self._folder}")
-        print(f"    will include {self._start.date()} to {self._end.date()}")
+        print(f"    will include {self._start.date()} to {self._end.date()} (not included)")
 
     def load_ics(self):
         framedict = {}
-        # print(Path(self._folder), Path(self._folder).exists(), Path(self._folder).is_dir())
-        # print(list(Path(self._folder).glob("*.ics")))
-        for filename in list(Path(self._folder).glob("*.ics")):
+        filelist = list(Path(self._folder).glob("*.ics"))
+        for filename in filelist:
             print(f"- reading {filename}")
             framedict[filename.stem] = ical_to_dframe(filename, self._start, self._end)
             framedict[filename.stem]["Member"] = filename.stem  # file name without path nor extension
+        if len(filelist) == 0:
+            raise FileNotFoundError("no *.ics file found")
         self._dframe = pd.concat(tuple(framedict.values()))
         self._set_wp(default=self._default_WP)
         self._clean_wp()
 
     def members(self):
+        """returns set (unordered list) of members"""
         return set(self._dframe["Member"])
 
     def work_packages(self):
+        """returns set (unordered list) of Work Packages"""
         return set(self._dframe["WP"])
 
     def _df_to_tab(self, wb: xl.Workbook, df, title=None):
         ws = wb.create_sheet(title=title)
         for row in dataframe_to_rows(df, header=True):
             ws.append(row)
         return ws
@@ -91,14 +109,15 @@
 
     def _clean_wp(self):
         rewp = re.compile(r"WP. *-* *")
         self._dframe["name"] = self._dframe["name"].apply(lambda s: rewp.sub("", s))
         return
 
     def filter(self, start: str, end: str):
+        """replace DataFrame with selected dates"""
         self._dframe = self._df_slot(start, end)
 
     def add_tabdetail_member(self, wb, member: str):
         df = self._dframe[self._dframe["Member"] == member].loc[:, ["date", "duration", "WP", "name"]]
         df["date"] = df["date"].apply(lambda d: d.strftime("%d/%m/%Y"))
         ws = self._df_to_tab(wb, df, member)
         ws.delete_cols(1)
@@ -136,12 +155,12 @@
                 print(f"- create WP worksheet {wp}")
                 self.add_tab_workpackage(wb, wp)
         wb.remove(ws_empty)
         return wb
 
 
 if __name__ == "__main__":
-    prj = Project(name="mambo", folder="examples/projetA", start="2023-01-01", end="2024-01-01")
+    prj = Project(name="mambo", folder="examples/projectA", start="2023-01-01", end="2024-01-01")
     prj.load_ics()  # lecture des .ics
     # prj.filter(start="2023-01-01", end="2023-12-31") # filtre des dates
     wb = prj.workbook()  # création du tableur
     wb.save("projetA.xlsx")  # sauvegarde du fichier
```

### Comparing `icalreporting-0.1.1/icalreporting.egg-info/PKG-INFO` & `icalreporting-0.1.2/icalreporting.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: icalreporting
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reporting tools from ical files
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
-        Copyright (c) 2022 Jérémie GRESSIER
+        Copyright (c) 2023 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -57,17 +57,33 @@
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d32cf67a5fa242c88bb1568277f1d60e)](https://app.codacy.com/gh/jgressier/icalreporting/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)[![Doc](https://readthedocs.org/projects/icalreporting/badge/?version=latest)](https://readthedocs.org/projects/icalreporting/)
 [![Slack](https://img.shields.io/static/v1?logo=slack&label=slack&message=contact&style=flat)](https://join.slack.com/t/isae-opendev/shared_invite/zt-obqywf6r-UUuHR4_hc5iTzyL5bFCwpw
 )
 
 ### Features
 
+- able to load ical files and fill a pandas database
+- parse the pandas database to identify project and creates a worksheet tables
+- export to open document XLSX file
 
-### Installation and usage
+### Installation
 
 ```bash
 pip install --upgrade icalreporting
 ```
+This automatic installation will get needed dependencies. 
 
 ### Requirements
 
 see [requirements.txt](https://github.com/jgressier/icalreporting/blob/master/requirements.txt)
+
+### Usage
+
+When installed, you just need to put a set a ical files in a folder for a project. You will be able to create a reporting file with the following lines.
+
+```python
+from icalreporting.reporting import Project
+prj = Project(name="Big-Project", folder="examples/projectA", start="2023-01-01", end="2024-01-01")
+prj.load_ics()  # read files
+wb = prj.workbook()  # create workbook
+wb.save("projectA.xlsx")  # save it to file
+```
```

### Comparing `icalreporting-0.1.1/pyproject.toml` & `icalreporting-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "icalreporting"
-version = "0.1.1"
+version = "0.1.2"
 description = "Reporting tools from ical files"
 authors = [{name="J. Gressier", email="jeremie.gressier@isae-supaero.fr"}]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
@@ -41,15 +41,15 @@
 minversion = "6.0"
 addopts = "--cov -v"
 testpaths = [
     "tests"
 ]
 
 [tool.bumpver]
-current_version = "v0.1.1"
+current_version = "v0.1.2"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

