# Comparing `tmp/nap-plot-tools-0.0.3.tar.gz` & `tmp/nap-plot-tools-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nap-plot-tools-0.0.3.tar", last modified: Tue Apr  2 07:10:13 2024, max compression
+gzip compressed data, was "nap-plot-tools-0.0.3a0.tar", last modified: Tue Nov 28 14:43:00 2023, max compression
```

## Comparing `nap-plot-tools-0.0.3.tar` & `nap-plot-tools-0.0.3a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:10:13.702258 nap-plot-tools-0.0.3/
--rw-rw-rw-   0        0        0     1526 2023-07-03 07:56:44.000000 nap-plot-tools-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3526 2024-04-02 07:10:13.699761 nap-plot-tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1866 2023-11-28 14:37:34.000000 nap-plot-tools-0.0.3/README.md
--rw-rw-rw-   0        0        0     1670 2024-04-02 07:10:13.722298 nap-plot-tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-10-27 08:08:29.000000 nap-plot-tools-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:10:13.460434 nap-plot-tools-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:10:13.575008 nap-plot-tools-0.0.3/src/nap_plot_tools/
--rw-rw-rw-   0        0        0      201 2024-03-28 15:58:38.000000 nap-plot-tools-0.0.3/src/nap_plot_tools/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-11-28 14:40:07.000000 nap-plot-tools-0.0.3/src/nap_plot_tools/cmap.py
--rw-rw-rw-   0        0        0    14996 2024-03-28 15:58:03.000000 nap-plot-tools-0.0.3/src/nap_plot_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:10:13.693746 nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/
--rw-rw-rw-   0        0        0     3526 2024-04-02 07:10:12.000000 nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-02 07:10:13.000000 nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:10:12.000000 nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-04-02 07:10:12.000000 nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 07:10:12.000000 nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.311799 nap-plot-tools-0.0.3a0/
+-rw-rw-rw-   0        0        0     1526 2023-07-03 07:56:44.000000 nap-plot-tools-0.0.3a0/LICENSE
+-rw-rw-rw-   0        0        0     3528 2023-11-28 14:43:00.310799 nap-plot-tools-0.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1866 2023-11-28 14:37:34.000000 nap-plot-tools-0.0.3a0/README.md
+-rw-rw-rw-   0        0        0     1670 2023-11-28 14:43:00.317385 nap-plot-tools-0.0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-10-27 08:08:29.000000 nap-plot-tools-0.0.3a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.220642 nap-plot-tools-0.0.3a0/src/
+drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.262421 nap-plot-tools-0.0.3a0/src/nap_plot_tools/
+-rw-rw-rw-   0        0        0      207 2023-11-28 14:40:18.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools/__init__.py
+-rw-rw-rw-   0        0        0     7480 2023-11-28 14:40:07.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools/cmap.py
+-rw-rw-rw-   0        0        0    12756 2023-11-28 14:40:07.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools/tools.py
+drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.306799 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/
+-rw-rw-rw-   0        0        0     3528 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/top_level.txt
```

### Comparing `nap-plot-tools-0.0.3/LICENSE` & `nap-plot-tools-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3/PKG-INFO` & `nap-plot-tools-0.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nap-plot-tools
-Version: 0.0.3
+Version: 0.0.3a0
 Summary: A NAPari PLOTter TOOLbar and tools for additional functionalities.
 Home-page: https://github.com/zoccoler/nap-plot-tools
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/zoccoler/nap-plot-tools/issues
 Project-URL: Documentation, https://github.com/zoccoler/nap-plot-tools#README.md
```

### Comparing `nap-plot-tools-0.0.3/README.md` & `nap-plot-tools-0.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3/setup.cfg` & `nap-plot-tools-0.0.3a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3/src/nap_plot_tools/cmap.py` & `nap-plot-tools-0.0.3a0/src/nap_plot_tools/cmap.py`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3/src/nap_plot_tools/tools.py` & `nap-plot-tools-0.0.3a0/src/nap_plot_tools/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from qtpy.QtWidgets import QSpinBox, QToolButton, QToolBar, QVBoxLayout, QWidget, QHBoxLayout, QSizePolicy
 
 import numpy as np
 
 class QtColorBox(QWidget):
     """A widget that shows a square with the current signal class color.
     """
+    
+
     def __init__(self, first_color_transparent=True) -> None:
         super().__init__()
         # TODO: Check why this may be necessary
         # self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
 
         self._height = 24
         self.setFixedWidth(self._height)
@@ -358,69 +360,8 @@
         name : str
             Button name.
         state : bool
             Button checked state.
         """        
         # Set the checked state of the button
         if name in self.buttons and self.buttons[name].isCheckable():
-            self.buttons[name].setChecked(state)
-
-    def disconnect_button_callback(self, name, callback=None):
-        """Disconnect a specific callback for a button, or all callbacks if none is specified.
-
-        Parameters
-        ----------
-        name : str
-            The name of the button whose callback should be disconnected.
-        callback : callable, optional
-            The specific callback function to disconnect. If None, all callbacks are disconnected.
-        """
-        if name in self.buttons:
-            button = self.buttons[name]
-            signal = button.toggled if button.isCheckable() else button.clicked
-            
-            if callback is not None:
-                # Disconnect a specific callback
-                try:
-                    signal.disconnect(callback)
-                except TypeError:
-                    # Callback was not connected
-                    pass
-            else:
-                # Disconnect all callbacks for the signal
-                try:
-                    signal.disconnect()
-                except TypeError:
-                    # No connections to disconnect
-                    pass
-
-    def remove_button(self, name):
-        """Remove a custom button from the toolbar, disconnecting any callbacks.
-
-        Parameters
-        ----------
-        name : str
-            The name of the button to remove.
-        """
-        if name in self.buttons:
-            # Disconnect all callbacks for the button
-            self.disconnect_button_callback(name)
-
-            button = self.buttons[name]
-            # Find the corresponding action and remove it from the toolbar
-            action = self.toolbar.widgetForAction(button.defaultAction())
-            if action:
-                self.toolbar.removeAction(button.defaultAction())
-            
-            # Hide the button as an additional precaution.
-            button.setVisible(False)
-
-            # Delete the button
-            button.deleteLater()
-
-            # Delete the button from the dictionary
-            del self.buttons[name]
-
-            # Adjust toolbar dimensions after removing the button
-            self.update_toolbar_minimum_width()
-            self.update_toolbar_height()
-
+            self.buttons[name].setChecked(state)
```

### Comparing `nap-plot-tools-0.0.3/src/nap_plot_tools.egg-info/PKG-INFO` & `nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nap-plot-tools
-Version: 0.0.3
+Version: 0.0.3a0
 Summary: A NAPari PLOTter TOOLbar and tools for additional functionalities.
 Home-page: https://github.com/zoccoler/nap-plot-tools
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/zoccoler/nap-plot-tools/issues
 Project-URL: Documentation, https://github.com/zoccoler/nap-plot-tools#README.md
```

