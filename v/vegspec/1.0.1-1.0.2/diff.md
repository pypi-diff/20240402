# Comparing `tmp/vegspec-1.0.1.tar.gz` & `tmp/vegspec-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegspec-1.0.1.tar", last modified: Wed Feb  7 20:01:50 2024, max compression
+gzip compressed data, was "vegspec-1.0.2.tar", last modified: Tue Apr  2 13:11:18 2024, max compression
```

## Comparing `vegspec-1.0.1.tar` & `vegspec-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-02-07 20:01:50.087298 vegspec-1.0.1/
--rwx------   0 kthorp    (1000) kthorp    (1000)     1378 2022-01-25 01:01:56.000000 vegspec-1.0.1/LICENSE.md
--rw-r--r--   0 kthorp    (1000) kthorp    (1000)     5077 2024-02-07 20:01:50.087298 vegspec-1.0.1/PKG-INFO
--rwx------   0 kthorp    (1000) kthorp    (1000)     4467 2024-01-25 17:43:44.000000 vegspec-1.0.1/README.md
--rwx------   0 kthorp    (1000) kthorp    (1000)      104 2021-12-03 23:38:41.000000 vegspec-1.0.1/pyproject.toml
--rwx------   0 kthorp    (1000) kthorp    (1000)      725 2024-02-07 20:01:50.087298 vegspec-1.0.1/setup.cfg
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-02-07 20:01:50.083298 vegspec-1.0.1/src/
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-02-07 20:01:50.083298 vegspec-1.0.1/src/vegspec/
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      608 2024-01-24 13:59:01.000000 vegspec-1.0.1/src/vegspec/__init__.py
--rwx------   0 kthorp    (1000) kthorp    (1000)    65638 2024-01-25 16:30:35.000000 vegspec-1.0.1/src/vegspec/vegspec.py
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-02-07 20:01:50.087298 vegspec-1.0.1/src/vegspec.egg-info/
--rw-r--r--   0 kthorp    (1000) kthorp    (1000)     5077 2024-02-07 20:01:50.000000 vegspec-1.0.1/src/vegspec.egg-info/PKG-INFO
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      266 2024-02-07 20:01:50.000000 vegspec-1.0.1/src/vegspec.egg-info/SOURCES.txt
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        1 2024-02-07 20:01:50.000000 vegspec-1.0.1/src/vegspec.egg-info/dependency_links.txt
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)       12 2024-02-07 20:01:50.000000 vegspec-1.0.1/src/vegspec.egg-info/requires.txt
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        8 2024-02-07 20:01:50.000000 vegspec-1.0.1/src/vegspec.egg-info/top_level.txt
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.578197 vegspec-1.0.2/
+-rwx------   0 kthorp    (1000) kthorp    (1000)     1378 2022-01-25 01:01:56.000000 vegspec-1.0.2/LICENSE.md
+-rw-r--r--   0 kthorp    (1000) kthorp    (1000)     5077 2024-04-02 13:11:18.578197 vegspec-1.0.2/PKG-INFO
+-rwx------   0 kthorp    (1000) kthorp    (1000)     4467 2024-01-25 17:43:44.000000 vegspec-1.0.2/README.md
+-rwx------   0 kthorp    (1000) kthorp    (1000)      104 2021-12-03 23:38:41.000000 vegspec-1.0.2/pyproject.toml
+-rwx------   0 kthorp    (1000) kthorp    (1000)      725 2024-04-02 13:11:18.578197 vegspec-1.0.2/setup.cfg
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.574197 vegspec-1.0.2/src/
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.578197 vegspec-1.0.2/src/vegspec/
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      608 2024-01-24 13:59:01.000000 vegspec-1.0.2/src/vegspec/__init__.py
+-rwx------   0 kthorp    (1000) kthorp    (1000)    65864 2024-03-29 14:25:19.000000 vegspec-1.0.2/src/vegspec/vegspec.py
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.578197 vegspec-1.0.2/src/vegspec.egg-info/
+-rw-r--r--   0 kthorp    (1000) kthorp    (1000)     5077 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/PKG-INFO
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      266 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/SOURCES.txt
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        1 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/dependency_links.txt
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)       12 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/requires.txt
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        8 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/top_level.txt
```

### Comparing `vegspec-1.0.1/LICENSE.md` & `vegspec-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vegspec-1.0.1/PKG-INFO` & `vegspec-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegspec
-Version: 1.0.1
+Version: 1.0.2
 Summary: A compilation of vegetative spectral indices and transformations in Python
 Home-page: http://github.com/kthorp/vegspec
 Author: Dr. Kelly R. Thorp
 Author-email: kelly.thorp@usda.gov
 License: Public Domain
 Project-URL: Source, http://github.com/kthorp/vegspec
 Project-URL: Bug Tracker, http://github.com/kthorp/vegspec/issues
```

### Comparing `vegspec-1.0.1/README.md` & `vegspec-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vegspec-1.0.1/setup.cfg` & `vegspec-1.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vegspec
-version = 1.0.1
+version = 1.0.2
 author = Dr. Kelly R. Thorp
 author_email = kelly.thorp@usda.gov
 description = A compilation of vegetative spectral indices and transformations in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/kthorp/vegspec
 project_urls =
```

### Comparing `vegspec-1.0.1/src/vegspec/__init__.py` & `vegspec-1.0.2/src/vegspec/__init__.py`

 * *Files identical despite different names*

### Comparing `vegspec-1.0.1/src/vegspec/vegspec.py` & `vegspec-1.0.2/src/vegspec/vegspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         self.indices.update({'PRI2':   self._PRI2()   })
         self.indices.update({'NDWI':   self._NDWI()   })
         self.indices.update({'GTSR1':  self._GTSR1()  })
         self.indices.update({'GTSR2':  self._GTSR2()  })
         self.indices.update({'GNDVI':  self._GNDVI()  })
         self.indices.update({'OSAVI':  self._OSAVI()  })
         self.indices.update({'WI':     self._WI()     })
+        self.indices.update({'WNR':    self._WNR()    })
         self.indices.update({'PSSRA':  self._PSSRA()  })
         self.indices.update({'PSSRB':  self._PSSRB()  })
         self.indices.update({'PSSRC':  self._PSSRC()  })
         self.indices.update({'PSNDA':  self._PSNDA()  })
         self.indices.update({'PSNDB':  self._PSNDB()  })
         self.indices.update({'PSNDC':  self._PSNDC()  })
         self.indices.update({'DSR1':   self._DSR1()   })
@@ -842,14 +843,20 @@
 
     def _WI(self):
         """Compute the Water Index (WI) (Penuelas et al., 1997)"""
         R900 = np.interp(900.,self.wl,self.rf,self.NaN,self.NaN)
         R970 = np.interp(970.,self.wl,self.rf,self.NaN,self.NaN)
         return R900/R970
 
+    def _WNR(self):
+        """Compute the WI NDVI ratio (Penuelas et al., 1997)"""
+        WI = self._WI()
+        NDVI = self._NDVI()
+        return WI/NDVI
+
     def _PSSRA(self):
         """Compute the Pigment Specific Simple Ratio for chlA (PSSRA)
         (Blackburn, 1998a; 1998b)"""
         R680 = np.interp(680.,self.wl,self.rf,self.NaN,self.NaN)
         R800 = np.interp(800.,self.wl,self.rf,self.NaN,self.NaN)
         return R800/R680
 
@@ -1496,10 +1503,10 @@
         (Sonobe & Wang, 2017)"""
         D522 = np.interp(522.,self.wl,self.rfd1,self.NaN,self.NaN)
         D728 = np.interp(728.,self.wl,self.rfd1,self.NaN,self.NaN)
         return (D522-D728)/(D522+D728)
 
     def _GRSUM(self):
         """Compute the area of the green reflectance peak from 500 nm
-        to 600 nm (GRSUM) (Thorp and Thompson)"""
+        to 600 nm (GRSUM) (Thorp and Thompson, in prep)"""
         widx = np.where(np.logical_and(self.wl>=500.,self.wl<=600.))
         return np.sum(self.rf[widx]*self.bndwdth[widx])
```

### Comparing `vegspec-1.0.1/src/vegspec.egg-info/PKG-INFO` & `vegspec-1.0.2/src/vegspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegspec
-Version: 1.0.1
+Version: 1.0.2
 Summary: A compilation of vegetative spectral indices and transformations in Python
 Home-page: http://github.com/kthorp/vegspec
 Author: Dr. Kelly R. Thorp
 Author-email: kelly.thorp@usda.gov
 License: Public Domain
 Project-URL: Source, http://github.com/kthorp/vegspec
 Project-URL: Bug Tracker, http://github.com/kthorp/vegspec/issues
```

