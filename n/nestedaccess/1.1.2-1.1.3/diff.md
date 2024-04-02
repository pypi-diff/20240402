# Comparing `tmp/nestedaccess-1.1.2.tar.gz` & `tmp/nestedaccess-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-1.1.2.tar", last modified: Mon Apr  1 09:05:12 2024, max compression
+gzip compressed data, was "dist/nestedaccess-1.1.3.tar", last modified: Tue Apr  2 02:31:00 2024, max compression
```

## Comparing `nestedaccess-1.1.2.tar` & `nestedaccess-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2024-04-01 09:05:12.901692 nestedaccess-1.1.2/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-1.1.2/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-1.1.2/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     4639 2024-04-01 09:05:12.901454 nestedaccess-1.1.2/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     2970 2024-04-01 09:03:03.000000 nestedaccess-1.1.2/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2024-04-01 09:05:12.899907 nestedaccess-1.1.2/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       41 2024-04-01 08:00:55.000000 nestedaccess-1.1.2/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)      700 2024-04-01 07:41:16.000000 nestedaccess-1.1.2/nestedaccess/lang.py
--rw-r--r--   0 wkl        (501) staff       (20)     2204 2024-04-01 08:00:23.000000 nestedaccess-1.1.2/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2024-04-01 09:05:12.901035 nestedaccess-1.1.2/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     4639 2024-04-01 09:05:12.000000 nestedaccess-1.1.2/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      257 2024-04-01 09:05:12.000000 nestedaccess-1.1.2/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2024-04-01 09:05:12.000000 nestedaccess-1.1.2/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2024-04-01 09:05:12.000000 nestedaccess-1.1.2/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2024-04-01 09:05:12.901799 nestedaccess-1.1.2/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3494 2024-04-01 09:04:32.000000 nestedaccess-1.1.2/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2024-04-02 02:31:00.106986 nestedaccess-1.1.3/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-1.1.3/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-1.1.3/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     4652 2024-04-02 02:31:00.106683 nestedaccess-1.1.3/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     2983 2024-04-01 09:13:45.000000 nestedaccess-1.1.3/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2024-04-02 02:31:00.103391 nestedaccess-1.1.3/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       41 2024-04-01 08:00:55.000000 nestedaccess-1.1.3/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)      700 2024-04-01 07:41:16.000000 nestedaccess-1.1.3/nestedaccess/lang.py
+-rw-r--r--   0 wkl        (501) staff       (20)     2193 2024-04-02 02:28:36.000000 nestedaccess-1.1.3/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2024-04-02 02:31:00.106113 nestedaccess-1.1.3/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     4652 2024-04-02 02:30:59.000000 nestedaccess-1.1.3/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      257 2024-04-02 02:31:00.000000 nestedaccess-1.1.3/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2024-04-02 02:30:59.000000 nestedaccess-1.1.3/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2024-04-02 02:30:59.000000 nestedaccess-1.1.3/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2024-04-02 02:31:00.107101 nestedaccess-1.1.3/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3494 2024-04-02 02:29:27.000000 nestedaccess-1.1.3/setup.py
```

### Comparing `nestedaccess-1.1.2/LICENSE` & `nestedaccess-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-1.1.2/PKG-INFO` & `nestedaccess-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 1.1.2
+Version: 1.1.3
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # README.md
@@ -54,15 +54,15 @@
             "empty_dict": {}
         }
         
         # normal data test.
         print(nestedaccess.get(data, ["foo", "baz", "quux", "grault", 1]))  # Output: 5
         
         test_key = ("empty_list", 0, "baz", "qux")
-        print(get(data, test_key))  # Output: hello
+        print(nestedaccess.get(data, test_key))  # Output: hello
         
         # Field does not exist, return default value data test.
         print(nestedaccess.get(data, ["nonexistent"], default="Not found"))  # Output: Not found
         
         # If the field does not exist, an error message is returned.
         test_key = ["foo", "baz", "quux", "corge", "invalid"]
         res = nestedaccess.get(data, test_key, lang="en")  # Output: ValueError: cannot fetch nested data because object of type bool has no key or index
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestedaccess Version: 1.1.2 Summary: Nestedaccess
+Metadata-Version: 2.1 Name: nestedaccess Version: 1.1.3 Summary: Nestedaccess
 is a simple, elegant way to retrieve nested data from deep dictionaries or
 lists. Home-page: https://github.com/Potato-OvO/nestedaccess Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com License: MIT Description: # README.md
 _ä_¸_­_æ___æ___æ_¡_£ # Nestedaccess Nestedaccess is a simple, elegant way to retrieve
 deeply nested data from a dictionary. Pass in the keys you want to obtain data
 through lists and tuples in sequence, avoiding the use of overly long if-elif-
 else judgment statements and making the code more elegant. In addition, if the
@@ -10,25 +10,25 @@
 is no default value, an error message will be output. The error message can
 specify a specific [language](#yuyan). ```python import nestedaccess data =
 { "foo": { "bar": [1, 2, 3], "baz": { "qux": "hello", "quux": { "corge": True,
 "grault": [4, 5, 6] } } }, "empty_list": [ { "baz": { "qux": "hello", "quux":
 { "grault": [1, 2, 3] } } }, { "baz": { "qux": "hello1", "quux": { "grault":
 [4, 5, 6] } } } ], "empty_dict": {} } # normal data test. print
 (nestedaccess.get(data, ["foo", "baz", "quux", "grault", 1])) # Output: 5
-test_key = ("empty_list", 0, "baz", "qux") print(get(data, test_key)) # Output:
-hello # Field does not exist, return default value data test. print
-(nestedaccess.get(data, ["nonexistent"], default="Not found")) # Output: Not
-found # If the field does not exist, an error message is returned. test_key =
-["foo", "baz", "quux", "corge", "invalid"] res = nestedaccess.get(data,
-test_key, lang="en") # Output: ValueError: cannot fetch nested data because
-object of type bool has no key or index test1_key = ("foo", "bae", "quux",
-"corge") res1 = nestedaccess.get(data, test1_key, lang="en") #Output: KeyError:
-"field 'bae' does not exist" ``` # Installing Nestedaccess and Supported
-Versions ## Nestedaccess is available on PyPI: ```python $ python -m pip
-install nestedaccess ``` Nestedaccess officially supports Python 3.7+. #
+test_key = ("empty_list", 0, "baz", "qux") print(nestedaccess.get(data,
+test_key)) # Output: hello # Field does not exist, return default value data
+test. print(nestedaccess.get(data, ["nonexistent"], default="Not found")) #
+Output: Not found # If the field does not exist, an error message is returned.
+test_key = ["foo", "baz", "quux", "corge", "invalid"] res = nestedaccess.get
+(data, test_key, lang="en") # Output: ValueError: cannot fetch nested data
+because object of type bool has no key or index test1_key = ("foo", "bae",
+"quux", "corge") res1 = nestedaccess.get(data, test1_key, lang="en") #Output:
+KeyError: "field 'bae' does not exist" ``` # Installing Nestedaccess and
+Supported Versions ## Nestedaccess is available on PyPI: ```python $ python -
+m pip install nestedaccess ``` Nestedaccess officially supports Python 3.7+. #
 Supported Features & BestâPractices - Used to obtain nested data. When the
 nested structure is deep, data can be obtained through lists or tuples to avoid
 using overly long if-elif-else judgment statements and make the code more
 elegant. - Takes a nested data object (can be a dictionary or a list), a list
 of keys or indexes, and an optional default value. - It will try to get the
 nested data in the given key or index order, output the non-existent field name
 if the field does not exist, and return the default value if a custom default
```

### Comparing `nestedaccess-1.1.2/README.md` & `nestedaccess-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "empty_dict": {}
 }
 
 # normal data test.
 print(nestedaccess.get(data, ["foo", "baz", "quux", "grault", 1]))  # Output: 5
 
 test_key = ("empty_list", 0, "baz", "qux")
-print(get(data, test_key))  # Output: hello
+print(nestedaccess.get(data, test_key))  # Output: hello
 
 # Field does not exist, return default value data test.
 print(nestedaccess.get(data, ["nonexistent"], default="Not found"))  # Output: Not found
 
 # If the field does not exist, an error message is returned.
 test_key = ["foo", "baz", "quux", "corge", "invalid"]
 res = nestedaccess.get(data, test_key, lang="en")  # Output: ValueError: cannot fetch nested data because object of type bool has no key or index
```

#### html2text {}

```diff
@@ -6,25 +6,25 @@
 value. If there is no default value, an error message will be output. The error
 message can specify a specific [language](#yuyan). ```python import
 nestedaccess data = { "foo": { "bar": [1, 2, 3], "baz": { "qux": "hello",
 "quux": { "corge": True, "grault": [4, 5, 6] } } }, "empty_list": [ { "baz":
 { "qux": "hello", "quux": { "grault": [1, 2, 3] } } }, { "baz": { "qux":
 "hello1", "quux": { "grault": [4, 5, 6] } } } ], "empty_dict": {} } # normal
 data test. print(nestedaccess.get(data, ["foo", "baz", "quux", "grault", 1])) #
-Output: 5 test_key = ("empty_list", 0, "baz", "qux") print(get(data, test_key))
-# Output: hello # Field does not exist, return default value data test. print
-(nestedaccess.get(data, ["nonexistent"], default="Not found")) # Output: Not
-found # If the field does not exist, an error message is returned. test_key =
-["foo", "baz", "quux", "corge", "invalid"] res = nestedaccess.get(data,
-test_key, lang="en") # Output: ValueError: cannot fetch nested data because
-object of type bool has no key or index test1_key = ("foo", "bae", "quux",
-"corge") res1 = nestedaccess.get(data, test1_key, lang="en") #Output: KeyError:
-"field 'bae' does not exist" ``` # Installing Nestedaccess and Supported
-Versions ## Nestedaccess is available on PyPI: ```python $ python -m pip
-install nestedaccess ``` Nestedaccess officially supports Python 3.7+. #
+Output: 5 test_key = ("empty_list", 0, "baz", "qux") print(nestedaccess.get
+(data, test_key)) # Output: hello # Field does not exist, return default value
+data test. print(nestedaccess.get(data, ["nonexistent"], default="Not found"))
+# Output: Not found # If the field does not exist, an error message is
+returned. test_key = ["foo", "baz", "quux", "corge", "invalid"] res =
+nestedaccess.get(data, test_key, lang="en") # Output: ValueError: cannot fetch
+nested data because object of type bool has no key or index test1_key = ("foo",
+"bae", "quux", "corge") res1 = nestedaccess.get(data, test1_key, lang="en")
+#Output: KeyError: "field 'bae' does not exist" ``` # Installing Nestedaccess
+and Supported Versions ## Nestedaccess is available on PyPI: ```python $ python
+-m pip install nestedaccess ``` Nestedaccess officially supports Python 3.7+. #
 Supported Features & BestâPractices - Used to obtain nested data. When the
 nested structure is deep, data can be obtained through lists or tuples to avoid
 using overly long if-elif-else judgment statements and make the code more
 elegant. - Takes a nested data object (can be a dictionary or a list), a list
 of keys or indexes, and an optional default value. - It will try to get the
 nested data in the given key or index order, output the non-existent field name
 if the field does not exist, and return the default value if a custom default
```

### Comparing `nestedaccess-1.1.2/nestedaccess/lang.py` & `nestedaccess-1.1.3/nestedaccess/lang.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-1.1.2/nestedaccess/nestedaccess.py` & `nestedaccess-1.1.3/nestedaccess/nestedaccess.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,24 +14,20 @@
 
 def get(data, keys, default=None, lang="en"):
     """
     get nested data
 
     Args:
         data (dict or list): Nested data objects, which can be dictionaries or lists
-        keys (list): list of keys or indices to fetch nested data
+        keys (list, tuple): Key or index list, tuple for getting nested data
         default (any, optional): The default value, returned when the acquisition fails, the default is None
+        lang (str, optional): If an error occurs, the language of the error message is returned. Defaults to "en"
 
     Returns:
         any: Nested data value, if the acquisition fails, return the default value
-
-    Example:
-        data = {'foo': {'bar': [1, 2, 3]}}
-        value = get(data, ['foo', 'bar', 1])
-        print(value)  # Output: 2
     """
     try:
         for key in keys:
             if isinstance(data, dict):
                 if key in data:
                     data = data[key]
                 else:
```

### Comparing `nestedaccess-1.1.2/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-1.1.3/nestedaccess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 1.1.2
+Version: 1.1.3
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # README.md
@@ -54,15 +54,15 @@
             "empty_dict": {}
         }
         
         # normal data test.
         print(nestedaccess.get(data, ["foo", "baz", "quux", "grault", 1]))  # Output: 5
         
         test_key = ("empty_list", 0, "baz", "qux")
-        print(get(data, test_key))  # Output: hello
+        print(nestedaccess.get(data, test_key))  # Output: hello
         
         # Field does not exist, return default value data test.
         print(nestedaccess.get(data, ["nonexistent"], default="Not found"))  # Output: Not found
         
         # If the field does not exist, an error message is returned.
         test_key = ["foo", "baz", "quux", "corge", "invalid"]
         res = nestedaccess.get(data, test_key, lang="en")  # Output: ValueError: cannot fetch nested data because object of type bool has no key or index
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestedaccess Version: 1.1.2 Summary: Nestedaccess
+Metadata-Version: 2.1 Name: nestedaccess Version: 1.1.3 Summary: Nestedaccess
 is a simple, elegant way to retrieve nested data from deep dictionaries or
 lists. Home-page: https://github.com/Potato-OvO/nestedaccess Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com License: MIT Description: # README.md
 _ä_¸_­_æ___æ___æ_¡_£ # Nestedaccess Nestedaccess is a simple, elegant way to retrieve
 deeply nested data from a dictionary. Pass in the keys you want to obtain data
 through lists and tuples in sequence, avoiding the use of overly long if-elif-
 else judgment statements and making the code more elegant. In addition, if the
@@ -10,25 +10,25 @@
 is no default value, an error message will be output. The error message can
 specify a specific [language](#yuyan). ```python import nestedaccess data =
 { "foo": { "bar": [1, 2, 3], "baz": { "qux": "hello", "quux": { "corge": True,
 "grault": [4, 5, 6] } } }, "empty_list": [ { "baz": { "qux": "hello", "quux":
 { "grault": [1, 2, 3] } } }, { "baz": { "qux": "hello1", "quux": { "grault":
 [4, 5, 6] } } } ], "empty_dict": {} } # normal data test. print
 (nestedaccess.get(data, ["foo", "baz", "quux", "grault", 1])) # Output: 5
-test_key = ("empty_list", 0, "baz", "qux") print(get(data, test_key)) # Output:
-hello # Field does not exist, return default value data test. print
-(nestedaccess.get(data, ["nonexistent"], default="Not found")) # Output: Not
-found # If the field does not exist, an error message is returned. test_key =
-["foo", "baz", "quux", "corge", "invalid"] res = nestedaccess.get(data,
-test_key, lang="en") # Output: ValueError: cannot fetch nested data because
-object of type bool has no key or index test1_key = ("foo", "bae", "quux",
-"corge") res1 = nestedaccess.get(data, test1_key, lang="en") #Output: KeyError:
-"field 'bae' does not exist" ``` # Installing Nestedaccess and Supported
-Versions ## Nestedaccess is available on PyPI: ```python $ python -m pip
-install nestedaccess ``` Nestedaccess officially supports Python 3.7+. #
+test_key = ("empty_list", 0, "baz", "qux") print(nestedaccess.get(data,
+test_key)) # Output: hello # Field does not exist, return default value data
+test. print(nestedaccess.get(data, ["nonexistent"], default="Not found")) #
+Output: Not found # If the field does not exist, an error message is returned.
+test_key = ["foo", "baz", "quux", "corge", "invalid"] res = nestedaccess.get
+(data, test_key, lang="en") # Output: ValueError: cannot fetch nested data
+because object of type bool has no key or index test1_key = ("foo", "bae",
+"quux", "corge") res1 = nestedaccess.get(data, test1_key, lang="en") #Output:
+KeyError: "field 'bae' does not exist" ``` # Installing Nestedaccess and
+Supported Versions ## Nestedaccess is available on PyPI: ```python $ python -
+m pip install nestedaccess ``` Nestedaccess officially supports Python 3.7+. #
 Supported Features & BestâPractices - Used to obtain nested data. When the
 nested structure is deep, data can be obtained through lists or tuples to avoid
 using overly long if-elif-else judgment statements and make the code more
 elegant. - Takes a nested data object (can be a dictionary or a list), a list
 of keys or indexes, and an optional default value. - It will try to get the
 nested data in the given key or index order, output the non-existent field name
 if the field does not exist, and return the default value if a custom default
```

### Comparing `nestedaccess-1.1.2/setup.py` & `nestedaccess-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

