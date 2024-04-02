# Comparing `tmp/beatlesalbuns-0.0.4.tar.gz` & `tmp/beatlesalbuns-0.0.5.tar.gz`

## Comparing `beatlesalbuns-0.0.4.tar` & `beatlesalbuns-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.4/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.4/beatlesalbuns.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.4/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/README.MD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/__init__.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/beatlesalbuns.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.5/PKG-INFO
```

### Comparing `beatlesalbuns-0.0.4/beatlesalbuns.py` & `beatlesalbuns-0.0.5/beatlesalbuns.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,30 +18,34 @@
                       '13-Let It Be'],
                     'Year': [1963, 1963, 1964, 1964, 1965, 1965, 1966, 1967, 1967, 1968, 1969, 1969, 1970]}
     # Método que mostra num dataframe os albuns do grupo The Beatles
     def show_albuns(self):
         #Converter dicionário numa Dataframe em Pandas
          print(f"=== Welcome! This is the list of The Beatles's albums ===".center(50))
          print(f"=== I love The Beatles!! ===\n".center(50))
+         print(pd.DataFrame(self.balbums))
          return pd.DataFrame(self.balbums)
     # Método que mostra as estatísticas da lista de albuns, contam quanto albuns/ano
     def stats(self):
         print("Number of albuns per year")
         print(self.show_albuns().groupby("Year").count())
     # Método que apresenta os nome dos elementos da banda
     def band_members(self):
         print("""
             == Band Members ==
             Vocals and Bass - Paul McCartney
             Vocals and Guitar - John Lennon
             Guitar - George Harrison
             Drums - Ringo Starr
         \n""")
+    # def info(self):
+    #     print(self.show_albuns().info())
 
 if __name__ == '__main__':
     #Instancia um objeto do tipo classe BAlbuns do módulo
     ls_albuns = BAlbuns()
     #invoca os métodos show_albuns(), stats(), band_members()
-    print(ls_albuns.show_albuns())
+    ls_albuns.show_albuns()
     ls_albuns.band_members()
     ls_albuns.stats()
+    #ls_albuns.info()
```

### Comparing `beatlesalbuns-0.0.4/LICENSE.txt` & `beatlesalbuns-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beatlesalbuns-0.0.4/PKG-INFO` & `beatlesalbuns-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: beatlesalbuns
-Version: 0.0.4
+Version: 0.0.5
 Summary: Shows a list of The Beatles albuns, stats and the band members
 Author-email: Carla Godinho <carlasoniagodinho44@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
-# Beatles-albums
+# Beatlesalbuns
+==========
 This package is a demo for my Python students and so I decided to give a tribute to The Beatles band, providing a list of their published Albums.
 Enjoy this packge and listen to their masterpieces!
 
+NOTE:
+----------
+To use this beatlesalbuns module it is a requirement import pandas module. Intall pandas modules:
+
+console> pip install pandas
+
+
 Change log
-==========
-0.0.4 (23/02/2024) - It was added new methods to class BAlbuns: stats() and band_members()
+------------
+0.0.5 (02/04/2024) - Small correction in method show_albuns() in order return the datafrane objet and as well printing the list of albuns
+0.0.4 (26/02/2024) - It was added new methods to class BAlbuns: stats() and band_members()
 0.0.3 (16/05/2023) - It was simplified the import of this module. Previous versions were needed to import beatlesalbuns.beatlesalbuns, this version you just need this instruction: import beatlesalbuns
-0.0.2 (8/05/2023) - Added print "I love The Beatles"
------------------
-Pre-requirements pandas module installed
+0.0.2 (8/05/2023) - Added print "I love The Beatles"
```

