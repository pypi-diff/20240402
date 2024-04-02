# Comparing `tmp/casioplot-2.2.1.tar.gz` & `tmp/casioplot-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casioplot-2.2.1.tar", last modified: Thu Mar 28 20:29:40 2024, max compression
+gzip compressed data, was "casioplot-3.0.0.tar", last modified: Tue Apr  2 09:14:18 2024, max compression
```

## Comparing `casioplot-2.2.1.tar` & `casioplot-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:29:40.290151 casioplot-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-28 20:29:28.000000 casioplot-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-28 20:29:28.000000 casioplot-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-03-28 20:29:40.290151 casioplot-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-28 20:29:28.000000 casioplot-2.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:29:40.290151 casioplot-2.2.1/casioplot/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/casioplot.py
--rw-r--r--   0 runner    (1001) docker     (127)   126571 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/configuration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/get_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:29:40.290151 casioplot-2.2.1/casioplot/images/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/images/blanck.png
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-28 20:29:28.000000 casioplot-2.2.1/casioplot/images/calculator.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:29:40.290151 casioplot-2.2.1/casioplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-03-28 20:29:40.000000 casioplot-2.2.1/casioplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-28 20:29:40.000000 casioplot-2.2.1/casioplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:29:40.000000 casioplot-2.2.1/casioplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 20:29:40.000000 casioplot-2.2.1/casioplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 20:29:40.000000 casioplot-2.2.1/casioplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-28 20:29:28.000000 casioplot-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 20:29:40.290151 casioplot-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:14:18.476820 casioplot-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 09:14:13.000000 casioplot-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 09:14:13.000000 casioplot-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-02 09:14:18.476820 casioplot-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-02 09:14:13.000000 casioplot-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:14:18.476820 casioplot-3.0.0/casioplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 09:14:13.000000 casioplot-3.0.0/casioplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-02 09:14:13.000000 casioplot-3.0.0/casioplot/casioplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126546 2024-04-02 09:14:13.000000 casioplot-3.0.0/casioplot/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-04-02 09:14:13.000000 casioplot-3.0.0/casioplot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-02 09:14:13.000000 casioplot-3.0.0/casioplot/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:14:18.476820 casioplot-3.0.0/casioplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-02 09:14:18.000000 casioplot-3.0.0/casioplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 09:14:18.000000 casioplot-3.0.0/casioplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:14:18.000000 casioplot-3.0.0/casioplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 09:14:18.000000 casioplot-3.0.0/casioplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 09:14:18.000000 casioplot-3.0.0/casioplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 09:14:13.000000 casioplot-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:14:18.476820 casioplot-3.0.0/setup.cfg
```

### Comparing `casioplot-2.2.1/LICENSE` & `casioplot-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casioplot-2.2.1/PKG-INFO` & `casioplot-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 2.2.1
+Version: 3.0.0
 Summary: Use casioplot module on a computer
 Author: Miguel Torrinha Pereira
 Author-email: Uniwix <uniwixu@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
@@ -97,38 +97,38 @@
 * show_screen is slower in the computer
 
 For example, the following codes draw a black square of 100 by 100 pixels.
 
 .. code-block:: python3
 
     for x in range(100):
-        for y in raange(100):
+        for y in range(100):
             set_pixel(x, y)
     show_screen()
 
 Is faster on the computer, but
 
 .. code-block:: python3
 
     for x in range(100):
-        for y in raange(100):
+        for y in range(100):
             set_pixel(x, y)
             show_screen()
 
 Is slower.
 
 Development setup
 -----------------
 
 Nothing needed.
 
 Release history
 ---------------
 
-See `CHANGELOG <./CHANGELOG.md>`_.
+See `CHANGELOG.md <https://github.com/uniwix/casioplot/blob/master/CHANGELOG.md>`_.
 
 Meta
 ----
 
 Uniwix - `uniwixu@gmail.com <uniwixu@gmail.com>`_
 
 Distributed under the MIT license. See `LICENSE <https://github.com/uniwix/casioplot/blob/master/LICENSE>`_ for more information.
@@ -141,8 +141,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 2.2.1 - Uniwix
+v 3.0.0 - Uniwix
```

### Comparing `casioplot-2.2.1/README.rst` & `casioplot-3.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,38 +55,38 @@
 * show_screen is slower in the computer
 
 For example, the following codes draw a black square of 100 by 100 pixels.
 
 .. code-block:: python3
 
     for x in range(100):
-        for y in raange(100):
+        for y in range(100):
             set_pixel(x, y)
     show_screen()
 
 Is faster on the computer, but
 
 .. code-block:: python3
 
     for x in range(100):
-        for y in raange(100):
+        for y in range(100):
             set_pixel(x, y)
             show_screen()
 
 Is slower.
 
 Development setup
 -----------------
 
 Nothing needed.
 
 Release history
 ---------------
 
-See `CHANGELOG <./CHANGELOG.md>`_.
+See `CHANGELOG.md <https://github.com/uniwix/casioplot/blob/master/CHANGELOG.md>`_.
 
 Meta
 ----
 
 Uniwix - `uniwixu@gmail.com <uniwixu@gmail.com>`_
 
 Distributed under the MIT license. See `LICENSE <https://github.com/uniwix/casioplot/blob/master/LICENSE>`_ for more information.
@@ -99,8 +99,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 2.2.1 - Uniwix
+v 3.0.0 - Uniwix
```

### Comparing `casioplot-2.2.1/casioplot/characters.py` & `casioplot-3.0.0/casioplot/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 Every size has it's one dictionary there is a key for every character
 and the values are tuples of strings that represent the character in
 a sort of character map, every string corresonds to a row.
 
 :py:func:`_get_char` gets the correct character from the dictionarys,
 serves as an interface for casioplot.py to get the characters it needs.
 """
-
-from typing import Literal
+# TODO: change how characters are drawn to be more efficient and faster
 
 
 large = {
     " ": (
         "                  ",
         "                  ",
         "                  ",
@@ -5338,22 +5337,20 @@
         "        ",
         "        ",
         "        ",
     ),
 }
 
 
-def _get_char(char: str, size: Literal["small", "medium", "large"] = "medium") -> tuple:
+_size_to_dict = {"small": small, "medium": medium, "large": large}
+
+
+def _get_char(char: str, size: str = "medium") -> tuple:
     """Gets the char_map of a character in a given size
 
     :param char: The character
     :param size: The size of the character
     """
     if char not in small.keys():
         raise ValueError(f"character {char} not implemented")
 
-    if size == "small":
-        return small[char]
-    elif size == "medium":
-        return medium[char]
-    else:
-        return large[char]
+    return _size_to_dict[size][char]
```

### Comparing `casioplot-2.2.1/casioplot/configuration_type.py` & `casioplot-3.0.0/casioplot/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-"""This file contains the type `configuration`
+"""This file contains the type `configuration` and the type `COLOR`.
 
 This type makes it possible to representing all settings and configs in a dictionary but still
 have type annotations for every settings.
 """
 
 from typing import TypedDict
 
-from PIL import Image
-
 
 # the option `total=False` makes it possible for a configuration
 # to not have a corresponding value for all settings
-class configuration(TypedDict, total=False):
+class Configuration(TypedDict, total=False):
     # canvas size
     width: int  # canvas width in pixels
     height: int  # canvas height in pixels
 
     # margins
     left_margin: int
     right_margin: int
     top_margin: int
     bottom_margin: int
 
     # background Image
     bg_image_is_set: bool  # is used when changing settings, if it is False the background_image
     # will be ignored
-    background_image: Image.Image  # some configs like casio_graph_90_plus_e
+    background_image: str  # some configs like casio_graph_90_plus_e
     # have a special background image
-    #
+
     # Output settings
     show_screen: bool  # Show the screen, do not mistake for the function show_screen()
     save_screen: bool  # Save the screen as an image
 
     # Saving settings
     filename: str
     image_format: str
     save_multiple: bool  # save multiple images so that the user can examine better the screen
     save_rate: int  # if save_multiple is True a new image will be saved
     # every `save_rate` times show_screen is called
+
+
+# color type
+Color = tuple[int, int, int]
```

### Comparing `casioplot-2.2.1/casioplot.egg-info/PKG-INFO` & `casioplot-3.0.0/casioplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 2.2.1
+Version: 3.0.0
 Summary: Use casioplot module on a computer
 Author: Miguel Torrinha Pereira
 Author-email: Uniwix <uniwixu@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
@@ -97,38 +97,38 @@
 * show_screen is slower in the computer
 
 For example, the following codes draw a black square of 100 by 100 pixels.
 
 .. code-block:: python3
 
     for x in range(100):
-        for y in raange(100):
+        for y in range(100):
             set_pixel(x, y)
     show_screen()
 
 Is faster on the computer, but
 
 .. code-block:: python3
 
     for x in range(100):
-        for y in raange(100):
+        for y in range(100):
             set_pixel(x, y)
             show_screen()
 
 Is slower.
 
 Development setup
 -----------------
 
 Nothing needed.
 
 Release history
 ---------------
 
-See `CHANGELOG <./CHANGELOG.md>`_.
+See `CHANGELOG.md <https://github.com/uniwix/casioplot/blob/master/CHANGELOG.md>`_.
 
 Meta
 ----
 
 Uniwix - `uniwixu@gmail.com <uniwixu@gmail.com>`_
 
 Distributed under the MIT license. See `LICENSE <https://github.com/uniwix/casioplot/blob/master/LICENSE>`_ for more information.
@@ -141,8 +141,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 2.2.1 - Uniwix
+v 3.0.0 - Uniwix
```

### Comparing `casioplot-2.2.1/pyproject.toml` & `casioplot-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Pillow"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "casioplot"
-version = "2.2.1"
+version = "3.0.0"
 description = "Use casioplot module on a computer"
 readme = "README.rst"
 authors = [
     { name = "Uniwix", email = "uniwixu@gmail.com" },
     { name = "Miguel Torrinha Pereira" }
 ]
 license = { file = "LICENSE" }
```

