# Comparing `tmp/ftrack_framework_qt-2.0.0.tar.gz` & `tmp/ftrack_framework_qt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_framework_qt-2.0.0.tar", max compression
+gzip compressed data, was "ftrack_framework_qt-2.1.0.tar", max compression
```

## Comparing `ftrack_framework_qt-2.0.0.tar` & `ftrack_framework_qt-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10176 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0       70 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/README.md
--rw-r--r--   0        0        0     1185 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      463 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/__init__.py
--rw-r--r--   0        0        0      199 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/dialogs/__init__.py
--rw-r--r--   0        0        0     6898 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/dialogs/base_context_dialog.py
--rw-r--r--   0        0        0     4538 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/dialogs/base_dialog.py
--rw-r--r--   0        0        0      121 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/widgets/__init__.py
--rw-r--r--   0        0        0     1095 2024-02-12 12:20:35.512473 ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/widgets/base_widget.py
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 ftrack_framework_qt-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      167 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/README.md
+-rw-r--r--   0        0        0     1164 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      463 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/__init__.py
+-rw-r--r--   0        0        0     3295 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/base_context_dialog.py
+-rw-r--r--   0        0        0     5521 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/base_dialog.py
+-rw-r--r--   0        0        0      121 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/widgets/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/widgets/base_widget.py
+-rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 ftrack_framework_qt-2.1.0/PKG-INFO
```

### Comparing `ftrack_framework_qt-2.0.0/LICENSE.txt` & `ftrack_framework_qt-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_framework_qt-2.0.0/pyproject.toml` & `ftrack_framework_qt-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-framework-qt"
-version = "2.0.0"
+version = "2.1.0"
 description='ftrack framework qt library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_framework_qt", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/framework-qt"
@@ -24,15 +24,15 @@
 
 [tool.poetry.dependencies]
 python = ">= 3.7, < 3.12"
 "Qt.py" = ">=1.0.0, < 2"
 #ftrack
 ftrack-constants= {  version = "^2.0.0", optional = true }
 ftrack-utils = {  version = "^2.0.0", optional = true }
-ftrack-qt = {  version = "^2.0.0", extras = ["pyside"], optional = true }
+ftrack-qt = {  version = "^2.0.0", optional = true }
 #framework
 ftrack-framework-core = {  version = "^2.0.0", optional = true }
 
 [tool.poetry.extras]
 ftrack-libs = ["ftrack-constants", "ftrack-utils", "ftrack-qt"]
 framework-libs = ["ftrack-framework-core"]
```

### Comparing `ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/dialogs/base_dialog.py` & `ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/base_dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,44 @@
 # :copyright: Copyright (c) 2024 ftrack
 
 from Qt import QtWidgets, QtCore
 
 from ftrack_framework_core.widget.dialog import FrameworkDialog
 
 from ftrack_qt.widgets.dialogs import StyledDialog
+from ftrack_qt.widgets.headers import SessionHeader
 
 from ftrack_qt.utils.layout import recursive_clear_layout
 
 
 class BaseDialog(FrameworkDialog, StyledDialog):
     '''Default Framework dialog'''
 
     name = 'base_dialog'
     tool_config_type_filter = None
+    run_button_title = 'run'
     ui_type = 'qt'
-    docked = True
+
+    @property
+    def header(self):
+        return self._header
 
     @property
     def tool_widget(self):
         return self._tool_widget
 
+    @property
+    def run_button(self):
+        return self._run_button
+
+    @property
+    def tool_config_names(self):
+        '''Return tool config names if passed in the dialog options.'''
+        return self.dialog_options.get('tool_config_names')
+
     def __init__(
         self,
         event_manager,
         client_id,
         connect_methods_callback,
         connect_setter_property_callback,
         connect_getter_property_callback,
@@ -47,58 +61,77 @@
         *dialog_options*: Dictionary of arguments passed to configure the
         current dialog.
         '''
         # As a mixing class we have to initialize the parents separately
         StyledDialog.__init__(
             self,
             background_style=None,
-            docked=self.docked,
+            docked=dialog_options.get("docked", False),
             parent=parent,
         )
         FrameworkDialog.__init__(
             self,
             event_manager,
             client_id,
             connect_methods_callback,
             connect_setter_property_callback,
             connect_getter_property_callback,
             dialog_options,
-            parent=parent,
+            parent,
         )
+        self._header = None
         self._tool_widget = None
+        self._run_button = None
 
         self.pre_build()
         self.build()
         self.post_build()
 
     def pre_build(self):
         main_layout = QtWidgets.QVBoxLayout()
         self.setLayout(main_layout)
 
     def build(self):
+        # Create the header
+        self._header = SessionHeader(self.event_manager.session)
+
         self._tool_widget = QtWidgets.QWidget()
         _tool_widget_layout = QtWidgets.QVBoxLayout()
         self._tool_widget.setLayout(_tool_widget_layout)
 
+        self._run_button = QtWidgets.QPushButton(self.run_button_title)
+
+        self.layout().addWidget(self._header)
         self.layout().addWidget(self._tool_widget)
+        self.layout().addWidget(self._run_button)
 
     def post_build(self):
         '''Set up all the signals'''
         self._on_client_context_changed_callback()
+        # Connect run_tool_config button
+        self._run_button.clicked.connect(self._on_run_button_clicked)
 
     def _on_client_context_changed_callback(self, event=None):
         '''Client context has been changed'''
         super(BaseDialog, self)._on_client_context_changed_callback(event)
         # Clean the UI every time a new context is set as the current tool
         # config might not be available anymore
         self.clean_ui()
         self.pre_build_ui()
         self.build_ui()
         self.post_build_ui()
 
+    def _on_run_button_clicked(self):
+        '''
+        Run button from the UI has been clicked.
+        Tell client to run the current tool config
+        '''
+
+        self.run_tool_config(self.tool_config['reference'])
+
     # FrameworkDialog overrides
     def show_ui(self):
         '''Override Show method of the base framework dialog'''
         StyledDialog.show(self)
         self.raise_()
         self.activateWindow()
         self.setWindowState(
@@ -137,13 +170,10 @@
 
     def build_ui(self):
         raise NotImplementedError
 
     def post_build_ui(self):
         raise NotImplementedError
 
-    def _on_run_button_clicked(self):
-        raise NotImplementedError
-
     def closeEvent(self, event):
         self.ui_closed()
         super(BaseDialog, self).closeEvent(event)
```

### Comparing `ftrack_framework_qt-2.0.0/source/ftrack_framework_qt/widgets/base_widget.py` & `ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/widgets/base_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_qt-2.0.0/PKG-INFO` & `ftrack_framework_qt-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-framework-qt
-Version: 2.0.0
+Version: 2.1.0
 Summary: ftrack framework qt library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,16 +15,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: framework-libs
 Provides-Extra: ftrack-libs
 Requires-Dist: Qt.py (>=1.0.0,<2)
 Requires-Dist: ftrack-constants (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-framework-core (>=2.0.0,<3.0.0) ; extra == "framework-libs"
-Requires-Dist: ftrack-qt[pyside] (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
+Requires-Dist: ftrack-qt (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-utils (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Project-URL: Repository, https://github.com/ftrackhq/integrations/tree/main/libs/framework-qt
 Description-Content-Type: text/markdown
 
 # Framework Qt
 
-This is the ftrack integrations framework-qt library.
+This is the ftrack integrations framework-qt library. 
+Base dialogs and widgets mixins used in the ftrack integrations framework should be found here.
```

