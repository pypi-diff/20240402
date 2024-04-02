# Comparing `tmp/atap_corpus_loader-1.2.3.tar.gz` & `tmp/atap_corpus_loader-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atap_corpus_loader-1.2.3.tar", max compression
+gzip compressed data, was "atap_corpus_loader-1.3.0.tar", max compression
```

## Comparing `atap_corpus_loader-1.2.3.tar` & `atap_corpus_loader-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
--rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.2.3/LICENSE
--rw-r--r--   0        0        0     1121 2024-03-22 01:49:27.012225 atap_corpus_loader-1.2.3/README.md
--rw-r--r--   0        0        0     2760 2024-03-22 00:20:21.113686 atap_corpus_loader-1.2.3/atap_corpus_loader/CorpusLoader.py
--rw-r--r--   0        0        0       39 2024-01-31 23:37:31.659710 atap_corpus_loader-1.2.3/atap_corpus_loader/__init__.py
--rw-r--r--   0        0        0    14048 2024-03-22 00:20:21.114532 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/Controller.py
--rw-r--r--   0        0        0     1028 2024-02-07 23:36:17.713791 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/CorpusExportService.py
--rw-r--r--   0        0        0    10510 2024-03-22 01:48:35.293559 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/FileLoaderService.py
--rw-r--r--   0        0        0      120 2024-01-31 04:39:45.157422 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/OniAPIService.py
--rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/__init__.py
--rw-r--r--   0        0        0      861 2024-02-01 23:13:09.263334 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/CorpusHeader.py
--rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/DataType.py
--rw-r--r--   0        0        0    10360 2024-03-04 06:07:17.510943 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/FileReference.py
--rw-r--r--   0        0        0     3947 2024-03-22 00:20:21.115530 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
--rw-r--r--   0        0        0      389 2024-03-22 00:20:21.116288 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
--rw-r--r--   0        0        0      243 2024-03-22 00:20:21.116782 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/__init__.py
--rw-r--r--   0        0        0       42 2024-01-31 04:39:45.159548 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/FileLoadError.py
--rw-r--r--   0        0        0     2791 2024-03-22 01:40:16.341437 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py
--rw-r--r--   0        0        0     2333 2024-02-01 00:33:21.789787 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py
--rw-r--r--   0        0        0      141 2024-01-31 04:39:45.160266 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/__init__.py
--rw-r--r--   0        0        0     1264 2024-02-21 22:35:28.868084 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
--rw-r--r--   0        0        0     1379 2024-03-04 06:07:17.512011 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
--rw-r--r--   0        0        0     1301 2024-02-21 22:40:45.349753 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
--rw-r--r--   0        0        0     1480 2024-03-04 06:07:17.512466 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
--rw-r--r--   0        0        0     2126 2024-03-22 00:20:21.117283 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py
--rw-r--r--   0        0        0     1284 2024-02-21 22:40:45.344967 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
--rw-r--r--   0        0        0     1268 2024-03-04 06:07:17.512871 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
--rw-r--r--   0        0        0     1259 2024-02-21 22:40:45.351554 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
--rw-r--r--   0        0        0      392 2024-01-31 04:39:45.162692 atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/__init__.py
--rw-r--r--   0        0        0     2021 2024-03-22 00:20:21.117946 atap_corpus_loader-1.2.3/atap_corpus_loader/view/ViewWrapperWidget.py
--rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.2.3/atap_corpus_loader/view/__init__.py
--rw-r--r--   0        0        0      908 2024-03-22 00:20:21.118599 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/AbstractWidget.py
--rw-r--r--   0        0        0     5158 2024-03-22 00:20:21.119031 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/CorpusInfoWidget.py
--rw-r--r--   0        0        0     6128 2024-03-08 04:13:48.321708 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/FileLoaderWidget.py
--rw-r--r--   0        0        0     5052 2024-03-22 00:20:21.119559 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/FileSelectorWidget.py
--rw-r--r--   0        0        0     7989 2024-03-04 06:07:17.514349 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/MetaEditorWidget.py
--rw-r--r--   0        0        0      368 2024-01-31 04:42:43.574976 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/OniLoaderWidget.py
--rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/__init__.py
--rw-r--r--   0        0        0      884 2024-02-27 01:11:22.657728 atap_corpus_loader-1.2.3/atap_corpus_loader/view/notifications/NotifierService.py
--rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.2.3/atap_corpus_loader/view/notifications/__init__.py
--rw-r--r--   0        0        0      637 2024-03-22 01:51:37.276070 atap_corpus_loader-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 atap_corpus_loader-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1121 2024-03-26 05:34:13.109832 atap_corpus_loader-1.3.0/README.md
+-rw-r--r--   0        0        0     3034 2024-03-28 05:36:33.585396 atap_corpus_loader-1.3.0/atap_corpus_loader/CorpusLoader.py
+-rw-r--r--   0        0        0       39 2024-01-31 23:37:31.659710 atap_corpus_loader-1.3.0/atap_corpus_loader/__init__.py
+-rw-r--r--   0        0        0    15406 2024-04-02 04:38:13.190518 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/Controller.py
+-rw-r--r--   0        0        0     2165 2024-04-02 05:16:29.554696 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/CorpusExportService.py
+-rw-r--r--   0        0        0    10508 2024-03-28 05:07:32.140765 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/FileLoaderService.py
+-rw-r--r--   0        0        0      120 2024-01-31 04:39:45.157422 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/OniAPIService.py
+-rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/__init__.py
+-rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/CorpusHeader.py
+-rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/DataType.py
+-rw-r--r--   0        0        0    10360 2024-03-04 06:07:17.510943 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/FileReference.py
+-rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
+-rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
+-rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/__init__.py
+-rw-r--r--   0        0        0       42 2024-01-31 04:39:45.159548 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/FileLoadError.py
+-rw-r--r--   0        0        0     2791 2024-03-26 05:34:13.113812 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py
+-rw-r--r--   0        0        0     2333 2024-02-01 00:33:21.789787 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py
+-rw-r--r--   0        0        0      141 2024-01-31 04:39:45.160266 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/__init__.py
+-rw-r--r--   0        0        0     1258 2024-03-26 23:51:50.582799 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1375 2024-03-26 23:51:50.593698 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
+-rw-r--r--   0        0        0     1295 2024-03-26 23:51:50.585036 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
+-rw-r--r--   0        0        0     1476 2024-03-26 23:51:50.577320 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
+-rw-r--r--   0        0        0     2120 2024-03-26 23:51:50.591361 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py
+-rw-r--r--   0        0        0     1278 2024-03-26 23:51:50.580377 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1264 2024-03-26 23:51:50.587110 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
+-rw-r--r--   0        0        0     1253 2024-03-26 23:51:50.589179 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
+-rw-r--r--   0        0        0      392 2024-01-31 04:39:45.162692 atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/__init__.py
+-rw-r--r--   0        0        0     2394 2024-03-28 05:27:29.294201 atap_corpus_loader-1.3.0/atap_corpus_loader/view/ViewWrapperWidget.py
+-rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.3.0/atap_corpus_loader/view/__init__.py
+-rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/AbstractWidget.py
+-rw-r--r--   0        0        0     5671 2024-04-02 05:16:29.557860 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/CorpusInfoWidget.py
+-rw-r--r--   0        0        0     6626 2024-04-02 04:47:12.414631 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/FileLoaderWidget.py
+-rw-r--r--   0        0        0     5339 2024-03-28 00:37:16.585867 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/FileSelectorWidget.py
+-rw-r--r--   0        0        0     8527 2024-03-28 03:29:31.348900 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/MetaEditorWidget.py
+-rw-r--r--   0        0        0      368 2024-01-31 04:42:43.574976 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/OniLoaderWidget.py
+-rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/__init__.py
+-rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.3.0/atap_corpus_loader/view/notifications/NotifierService.py
+-rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.3.0/atap_corpus_loader/view/notifications/__init__.py
+-rw-r--r--   0        0        0     1654 2024-03-28 02:23:23.522637 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/TooltipManager.py
+-rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/__init__.py
+-rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/build_button.md
+-rw-r--r--   0        0        0      972 2024-03-28 02:04:53.521402 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
+-rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
+-rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
+-rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
+-rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
+-rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.3.0/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
+-rw-r--r--   0        0        0      637 2024-04-02 05:30:00.294566 atap_corpus_loader-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 atap_corpus_loader-1.3.0/PKG-INFO
```

### Comparing `atap_corpus_loader-1.2.3/LICENSE` & `atap_corpus_loader-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/README.md` & `atap_corpus_loader-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/CorpusLoader.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/CorpusLoader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from typing import Optional, Callable
 
 import panel
 from atap_corpus.corpus.corpus import DataFrameCorpus
+from panel.theme import Fast
 from panel.viewable import Viewer
 
 from atap_corpus_loader.controller import Controller
 from atap_corpus_loader.view import ViewWrapperWidget
 
-panel.extension(notifications=True)
+panel.extension(notifications=True, design=Fast)
 
 
 class CorpusLoader(Viewer):
     """
     Public interface for the CorpusLoader module. Maintains a reference to the logic Controller and the GUI wrapper.
     A CorpusLoader object can be used as a Panel component, i.e. will render in a Panel GUI.
     The build_callback_fn will be called when a corpus is built (can be set using set_build_callback()).
     """
 
-    def __init__(self, root_directory: str, **params):
+    def __init__(self, root_directory: str, include_meta_loader: bool = False, **params):
         """
         :param root_directory: The root directory that the file selector will search for files to load. The argument must be a string. The directory may be non-existent at initialisation time, but no files will be displayed until it exists.
+        :param include_meta_loader: If True, the Corpus Loader will include additional metadata joining functionality. False by default
         :param params: passed onto the panel.viewable.Viewer super-class
         :type root_directory: str
+        :type include_meta_loader: bool
         """
         super().__init__(**params)
         self.controller: Controller = Controller(root_directory)
-        self.view: ViewWrapperWidget = ViewWrapperWidget(self.controller)
+        self.view: ViewWrapperWidget = ViewWrapperWidget(self.controller, include_meta_loader)
 
     def __panel__(self):
         return self.view
 
     def set_build_callback(self, callback: Callable, *args, **kwargs):
         """
         Allows a callback function to be set when a corpus has completed building
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/Controller.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/Controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
         self.corpora: UniqueNameCorpora = UniqueNameCorpora()
 
         self.build_callback_fn: Optional[Callable] = None
         self.build_callback_args: list = []
         self.build_callback_kwargs: dict = {}
 
-        self.tqdm_obj = Tqdm()
-        self.tqdm_obj.visible = False
+        self.build_tqdm = Tqdm(visible=False)
+        self.export_tqdm = Tqdm(visible=False)
 
     @staticmethod
     def setup_logger():
         if Controller.LOGGER is not None:
             return
         formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         log_file_location = abspath(join(dirname(__file__), '..', 'log.txt'))
@@ -103,119 +103,130 @@
             corpora_dict[corpus.name] = corpus
 
         return corpora_dict
 
     def load_corpus_from_filepaths(self, filepath_ls: list[str], include_hidden: bool) -> bool:
         Controller.LOGGER.debug(f"Files loaded as corpus: {filepath_ls}")
         try:
-            self.file_loader_service.add_corpus_files(filepath_ls, include_hidden, self.tqdm_obj)
+            self.file_loader_service.add_corpus_files(filepath_ls, include_hidden, self.build_tqdm)
             self.corpus_headers = self.file_loader_service.get_inferred_corpus_headers()
         except FileLoadError as e:
             self.display_error(str(e))
-            self.unload_filepaths(filepath_ls)
+            self.unload_all()
             return False
 
         return True
 
-
     def load_meta_from_filepaths(self, filepath_ls: list[str], include_hidden: bool) -> bool:
         Controller.LOGGER.debug(f"Files loaded as meta: {filepath_ls}")
         try:
-            self.file_loader_service.add_meta_files(filepath_ls, include_hidden, self.tqdm_obj)
+            self.file_loader_service.add_meta_files(filepath_ls, include_hidden, self.build_tqdm)
             self.meta_headers = self.file_loader_service.get_inferred_meta_headers()
         except FileLoadError as e:
             self.display_error(str(e))
-            self.unload_filepaths(filepath_ls)
+            self.unload_all()
             return False
 
         return True
 
     def build_corpus(self, corpus_name: str) -> bool:
+        Controller.LOGGER.debug(f"build_corpus method: Building corpus with name {corpus_name}")
         if self.is_meta_added():
             if (self.corpus_link_header is None) or (self.meta_link_header is None):
                 self.display_error("Cannot build without link headers set. Select a corpus header and a meta header as linking headers in the dropdowns")
                 return False
 
         if (corpus_name == '') or (corpus_name is None):
             corpus_name = f"Corpus-{datetime.now()}"
+            Controller.LOGGER.debug(f"build_corpus method: No name provided, so corpus name generated: {corpus_name}")
 
-        self.tqdm_obj.visible = True
+        self.build_tqdm.visible = True
         try:
             corpus = self.file_loader_service.build_corpus(corpus_name, self.corpus_headers,
                                                            self.meta_headers, self.text_header,
                                                            self.corpus_link_header, self.meta_link_header,
-                                                           self.tqdm_obj)
+                                                           self.build_tqdm)
+            Controller.LOGGER.debug(f"build_corpus method: corpus built")
         except FileLoadError as e:
             Controller.LOGGER.exception("Exception while building corpus: ")
             self.display_error(str(e))
-            self.tqdm_obj.visible = False
+            self.build_tqdm.visible = False
             return False
         except Exception as e:
             Controller.LOGGER.exception("Exception while building corpus: ")
             self.display_error(f"Unexpected error building corpus: {e}")
-            self.tqdm_obj.visible = False
+            self.build_tqdm.visible = False
             return False
 
         try:
             self.corpora.add(corpus)
+            Controller.LOGGER.debug(f"build_corpus method: corpus added to corpora")
         except Exception as e:
             Controller.LOGGER.exception("Exception while adding corpus to corpora: ")
             self.display_error(str(e))
-            self.tqdm_obj.visible = False
+            self.build_tqdm.visible = False
             return False
 
         try:
             if self.build_callback_fn is not None:
                 self.build_callback_fn(*self.build_callback_args, **self.build_callback_kwargs)
+                Controller.LOGGER.debug(f"build_corpus method: callback function called")
         except Exception as e:
             Controller.LOGGER.exception("Exception while calling build callback: ")
             self.display_error(f"Build callback error: {e}")
-            self.tqdm_obj.visible = False
+            self.build_tqdm.visible = False
             return False
 
-        self.tqdm_obj.visible = False
+        self.build_tqdm.visible = False
+        Controller.LOGGER.debug(f"build_corpus method: corpus building complete")
 
         return True
 
     def get_corpora_info(self) -> list[ViewCorpusInfo]:
         corpora_info: list[ViewCorpusInfo] = []
 
         for corpus in self.corpora.items():
-            corpus_as_df: DataFrame = corpus.to_dataframe()
+            corpus_df: DataFrame = corpus.to_dataframe()
 
             name: Optional[str] = corpus.name
             num_rows: int = len(corpus)
             headers: list[str] = []
             dtypes: list[str] = []
             dtype: str
-            for header_name, dtype_obj in corpus_as_df.dtypes.items():
+            for header_name, dtype_obj in corpus_df.dtypes.items():
                 try:
                     dtype = DataType(str(dtype_obj).lower()).name
                 except ValueError:
                     dtype = DataType.TEXT.name
                 dtypes.append(dtype)
                 headers.append(str(header_name))
+            first_row_data: list[str] = []
+            if not corpus_df.empty:
+                first_row_data = [str(x) for x in corpus_df.iloc[0]]
 
-            corpora_info.append(ViewCorpusInfo(name, num_rows, headers, dtypes))
+            corpora_info.append(ViewCorpusInfo(name, num_rows, headers, dtypes, first_row_data))
 
         return corpora_info
 
     def delete_corpus(self, corpus_name: str):
         self.corpora.remove(corpus_name)
 
     def rename_corpus(self, corpus_name: str, new_name: str):
+        Controller.LOGGER.debug(f"Renaming corpus named '{corpus_name}' to '{new_name}'")
         corpus: Optional[DataFrameCorpus] = self.corpora.get(corpus_name)
         if corpus is None:
             self.display_error(f"No corpus with name {corpus_name} found")
             return
 
         try:
             corpus.rename(new_name)
         except ValueError as e:
             self.display_error(str(e))
+        except Exception as e:
+            self.display_error(f"Unexpected error while renaming: {e}")
 
     def get_loaded_file_counts(self) -> dict[str, int]:
         corpus_file_set = set(self.file_loader_service.get_loaded_corpus_files())
         meta_file_set = set(self.file_loader_service.get_loaded_meta_files())
         file_set = corpus_file_set | meta_file_set
 
         file_counts: dict[str, int] = {"Total files": len(file_set)}
@@ -274,14 +285,17 @@
 
     def get_all_datatypes(self) -> list[str]:
         return [d.name for d in DataType]
 
     def get_valid_filetypes(self) -> list[str]:
         return [ft.name for ft in ValidFileType]
 
+    def get_build_progress_bar(self) -> Tqdm:
+        return self.build_tqdm
+
     def is_corpus_added(self) -> bool:
         return len(self.file_loader_service.get_loaded_corpus_files()) > 0
 
     def is_meta_added(self) -> bool:
         return len(self.file_loader_service.get_loaded_meta_files()) > 0
 
     def update_corpus_header(self, header: CorpusHeader, include: Optional[bool], datatype_name: Optional[str]):
@@ -340,11 +354,20 @@
 
     def export_corpus(self, corpus_name: str, filetype: str) -> Optional[BytesIO]:
         corpus: Optional[DataFrameCorpus] = self.corpora.get(corpus_name)
         if corpus is None:
             self.display_error(f"No corpus with name '{corpus_name}' found")
             return None
 
+        self.export_tqdm.visible = True
         try:
-            return self.corpus_export_service.export(corpus.to_dataframe(), filetype)
+            file_object: BytesIO = self.corpus_export_service.export(corpus.to_dataframe(), filetype, self.export_tqdm)
+            self.export_tqdm.visible = False
+            return file_object
         except ValueError as e:
             self.display_error(str(e))
+        except Exception as e:
+            self.display_error(f"Unexpected error while exporting: {e}")
+        self.export_tqdm.visible = False
+
+    def get_export_progress_bar(self) -> Tqdm:
+        return self.export_tqdm
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/FileLoaderService.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/FileLoaderService.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,14 @@
         elif load_corpus:
             final_df = corpus_df
         elif load_meta:
             final_df = meta_df
         else:
             raise ValueError("No corpus headers or metadata headers provided")
 
-
-
         return DataFrameCorpus.from_dataframe(final_df, text_header.name, corpus_name)
 
     @staticmethod
     def _sanitise_root_dir(root_directory: str) -> str:
         if type(root_directory) is not str:
             raise TypeError(f"root_directory argument: expected string, got {type(root_directory)}")
         sanitised_directory = normpath(root_directory)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/CorpusHeader.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/CorpusHeader.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class CorpusHeader:
     """
     Represents a column before the corpus is built.
     Holds the name, intended datatype, and whether to include the header.
     Also behaves as a Value Object, where the unique value is the name for equality checks and hashing.
     """
-    def __init__(self, name: str, datatype: DataType, include: bool):
+    def __init__(self, name: str, datatype: DataType, include: bool = False):
         self.name: str = name
         self.datatype: DataType = datatype
         self.include: bool = include
 
     def __str__(self):
         return self.name
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/FileReference.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/FileReference.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,42 +31,42 @@
         else:
             raise TypeError(f"Corpora can only store Corpus objects. Got {corpus.__class__.__name__}.")
 
     def _verify_unique_name(self, name: str):
         if name in self._collection:
             raise ValueError(f"Corpus with name '{name}' already exists. Select a different name")
 
-    def _simple_rename(self, name: str):
-        self._name = name
-
-    def _unique_rename(self, name: str):
+    def _unique_rename(self, corpus: TCorpus, name: str):
         self._verify_unique_name(name)
-        self._name = name
+        old_name = corpus.name
+        corpus._name = name
+        self._collection[name] = self._collection.pop(old_name)
 
     def add(self, corpus: TCorpus):
         """ Adds a Corpus into the Corpora. Corpus name is used as the name for get(), remove().
         If a corpus with the same name is added again, a ValueError is raised.
         If a corpus is added with a name that is empty or None, it is renamed to a generated name based on the current time.
         BaseCorpus objects added have their rename method replaced to include a check for name uniqueness.
         """
         if not isinstance(corpus, BaseCorpus):
             raise TypeError(f"Corpora can only store Corpus objects. Got {corpus.__class__.__name__}.")
 
         self._verify_unique_name(corpus.name)
 
-        corpus.rename = self._unique_rename
+        corpus.__ORIG_RENAME = corpus.rename
+        corpus.rename = lambda new_name, corpus_obj=corpus: self._unique_rename(corpus_obj, new_name)
         self._collection[corpus.name] = corpus
 
     def remove(self, name: str):
         """ Remove a Corpus from the Corpora.
         The rename method of the Corpus object has the unique name constraint removed before it is removed from the Corpora.
         If Corpus does not exist, it'll have no effect.
         """
         try:
-            self._collection[name].rename = self._simple_rename
+            self._collection[name].rename = self._collection[name].__ORIG_RENAME
             del self._collection[name]
         except KeyError:
             return
 
     def items(self) -> list[TCorpus]:
         """
         Returns a shallow copy list of the corpus objects in the Corpora, in order of addition.
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
-            headers.append(CorpusHeader(str(header_name), dtype, True))
+            headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         df: DataFrame = read_csv(file_buf, header=0, usecols=included_headers)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType, FileReference
 from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class DOCXLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         headers: list[CorpusHeader] = [
-            CorpusHeader('document', DataType.TEXT, True),
-            CorpusHeader('filename', DataType.TEXT, True),
-            CorpusHeader('filepath', DataType.TEXT, True)
+            CorpusHeader('document', DataType.TEXT, include=True),
+            CorpusHeader('filename', DataType.TEXT),
+            CorpusHeader('filepath', DataType.TEXT)
         ]
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         docx_doc = Document(file_buf)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
-            headers.append(CorpusHeader(str(header_name), dtype, True))
+            headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         df: DataFrame = read_excel(file_buf, engine='odf', header=0, names=included_headers)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType, FileReference
 from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class ODTLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         headers: list[CorpusHeader] = [
-            CorpusHeader('document', DataType.TEXT, True),
-            CorpusHeader('filename', DataType.TEXT, True),
-            CorpusHeader('filepath', DataType.TEXT, True)
+            CorpusHeader('document', DataType.TEXT, include=True),
+            CorpusHeader('filename', DataType.TEXT),
+            CorpusHeader('filepath', DataType.TEXT)
         ]
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         odt_doc = load(file_buf)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         if len(columns) == 0:
             raise FileLoadError(f"No tabular data found. Ensure the file contains tabular data (rows and columns)")
 
         headers: list[CorpusHeader] = []
         dtype: DataType = DataType.TEXT
         for col_name in columns:
-            headers.append(CorpusHeader(col_name, dtype, True))
+            headers.append(CorpusHeader(col_name, dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         real_path: str = self.file_ref.resolve_real_file_path()
 
         try:
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
-            headers.append(CorpusHeader(str(header_name), dtype, True))
+            headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         df: DataFrame = read_csv(file_buf, sep='\t', header=0, usecols=included_headers)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
 from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class TXTLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         headers: list[CorpusHeader] = [
-            CorpusHeader('document', DataType.TEXT, True),
-            CorpusHeader('filename', DataType.TEXT, True),
-            CorpusHeader('filepath', DataType.TEXT, True)
+            CorpusHeader('document', DataType.TEXT, include=True),
+            CorpusHeader('filename', DataType.TEXT),
+            CorpusHeader('filepath', DataType.TEXT)
         ]
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         document = file_buf.read()
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
-            headers.append(CorpusHeader(str(header_name), dtype, True))
+            headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         df: DataFrame = read_excel(file_buf, header=0, names=included_headers)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/ViewWrapperWidget.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/ViewWrapperWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from typing import Optional
+
 from panel import Tabs
+from panel.widgets import TooltipIcon
 
 from atap_corpus_loader.controller import Controller
 from atap_corpus_loader.view.gui import AbstractWidget, FileLoaderWidget, CorpusInfoWidget
+from atap_corpus_loader.view.tooltips import TooltipManager
 
 
 class ViewWrapperWidget(AbstractWidget):
     """
     A wrapper class that holds different loading method interfaces within a Tab
     """
-    def __init__(self, controller: Controller):
+    def __init__(self, controller: Controller, include_meta_loader: bool):
         super().__init__()
         self.controller: Controller = controller
+        self.tooltip_manager: TooltipManager = TooltipManager()
 
-        self.file_loader: FileLoaderWidget = FileLoaderWidget(self, controller)
+        self.file_loader: FileLoaderWidget = FileLoaderWidget(self, controller, include_meta_loader)
         self.corpus_display: CorpusInfoWidget = CorpusInfoWidget(controller)
 
         self.panel = Tabs(("File Loader", self.file_loader),
                           ("Corpus Overview", self.corpus_display))
         self.corpus_info_idx: int = len(self.panel) - 1
         self.children = [self.file_loader, self.corpus_display]
 
@@ -45,7 +50,10 @@
             self.update_displays()
 
             self.panel.active = self.corpus_info_idx
             corpus_name: str = self.controller.get_latest_corpus().name
             self.controller.display_success(f"Corpus {corpus_name} built successfully")
 
         return success
+
+    def get_tooltip(self, tooltip_name: str) -> Optional[TooltipIcon]:
+        return self.tooltip_manager.get_tooltip(tooltip_name)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/AbstractWidget.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/CorpusInfoWidget.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/CorpusInfoWidget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+import re
 from io import BytesIO
 from typing import Optional
 
-import panel
-from panel import Row, Accordion, bind, HSpacer
+from panel import Row, Accordion, bind, HSpacer, Column
+from panel.layout import Divider
 from panel.pane import Markdown
 from panel.widgets import Button, TextInput, FileDownload, Select
 
 from atap_corpus_loader.controller import Controller
 from atap_corpus_loader.controller.data_objects import ViewCorpusInfo
 from atap_corpus_loader.view.gui import AbstractWidget
 
-panel.extension()
-
 
 class CorpusInfoWidget(AbstractWidget):
     def __init__(self, controller: Controller):
         super().__init__()
         self.controller: Controller = controller
 
         self.corpus_controls = Accordion(toggle=True, width=600)
         self.corpus_controls.header_background = "#FFFFFA"
         self.corpus_controls.active_header_background = "#7A8B99"
         self.corpus_controls.param.watch(self._update_corpus_display, 'active', onlychanged=False)
 
         self.corpus_display: Markdown = Markdown()
 
-        self.panel = Row(self.corpus_controls, self.corpus_display)
+        self.panel = Column(
+            self.corpus_controls,
+            Row(self.controller.get_export_progress_bar()),
+            Divider(),
+            self.corpus_display)
 
     @staticmethod
     def _build_corpus_label(corpus_info: ViewCorpusInfo) -> str:
         name: Optional[str] = corpus_info.name
         if name is None:
             name = " "
         row_info: str = f"{corpus_info.num_rows} document"
@@ -39,19 +42,23 @@
         return f"{name} - {row_info}"
 
     @staticmethod
     def _build_header_markdown_table(corpus_info: ViewCorpusInfo) -> str:
         if len(corpus_info.headers) != len(corpus_info.dtypes):
             return " "
 
-        header_row = "| " + " | ".join(corpus_info.headers) + " |"
-        spacer_row = "| :-: " * len(corpus_info.headers) + "|"
-        data_row = "| " + " | ".join(corpus_info.dtypes) + " |"
+        sanitised_first_row: list[str] = [re.sub(r'([\\\`*_{}[\]()#+\-.!])', r'\\\1', x) for x in corpus_info.first_row_data]
+        sanitised_first_row = [re.sub(r'\n', ' ', x) for x in sanitised_first_row]
+
+        header_row = "| Data label " + "| " + " | ".join(corpus_info.headers) + " |"
+        spacer_row = "| :-: " * (len(corpus_info.headers) + 1) + "|"
+        dtype_row = "| **Datatype** " + "| " + " | ".join(corpus_info.dtypes) + " |"
+        data_row = "| **First document** " + "| " + " | ".join(sanitised_first_row) + " |"
 
-        header_table_text = f"{header_row}\n{spacer_row}\n{data_row}"
+        header_table_text = f"**{corpus_info.name}**\n{header_row}\n{spacer_row}\n{dtype_row}\n{data_row}"
         return header_table_text
 
     def export_corpus(self, corpus_name: str, filetype: str) -> Optional[BytesIO]:
         return self.controller.export_corpus(corpus_name, filetype)
 
     def rename_corpus(self, corpus_name: str, name: str):
         self.controller.rename_corpus(corpus_name, name)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/FileLoaderWidget.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/FileLoaderWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 from panel import Row, Spacer, Column, HSpacer
 from panel.pane import Markdown
-from panel.widgets import Button, TextInput
+from panel.widgets import Button, TextInput, TooltipIcon
 
 from atap_corpus_loader.controller import Controller
 from atap_corpus_loader.view import ViewWrapperWidget
 from atap_corpus_loader.view.gui import AbstractWidget
 from atap_corpus_loader.view.gui.FileSelectorWidget import FileSelectorWidget
 from atap_corpus_loader.view.gui.MetaEditorWidget import MetaEditorWidget
 
 
 class FileLoaderWidget(AbstractWidget):
-    def __init__(self, view_handler: ViewWrapperWidget, controller: Controller):
+    LOADER_WIDTH: int = 600
+
+    def __init__(self, view_handler: ViewWrapperWidget, controller: Controller, include_meta_loader: bool):
         super().__init__()
         self.view_handler: ViewWrapperWidget = view_handler
         self.controller: Controller = controller
         
-        self.load_as_corpus_button: Button = Button(name='Load as corpus', width=130,
-                                                    button_style='outline', button_type='success')
+        self.load_as_corpus_button: Button = Button(name='Load as corpus', width=130, button_style='outline', button_type='success')
         self.load_as_corpus_button.on_click(self.load_as_corpus)
-        self.load_as_meta_button: Button = Button(name='Load as metadata', width=130,
-                                                  button_style='outline', button_type='success')
+        load_corpus_tooltip = self.view_handler.get_tooltip('load_corpus_button')
+        load_corpus_tooltip.visible = not include_meta_loader
+        self.load_as_corpus_row: Row = Row(self.load_as_corpus_button, load_corpus_tooltip)
+        self.load_as_meta_button: Button = Button(name='Load as metadata', width=130, button_style='outline', button_type='success')
         self.load_as_meta_button.on_click(self.load_as_meta)
+        load_buttons_tooltip = self.view_handler.get_tooltip('load_buttons')
+        self.load_as_meta_row: Row = Row(self.load_as_meta_button, load_buttons_tooltip, visible=include_meta_loader)
 
-        self.unload_all_button: Button = Button(name="Unload all", width=100, button_style='solid',
-                                                button_type='danger', disabled=True)
-        self.unload_all_button.on_click(self.unload_all)
-        self.unload_selected_button: Button = Button(name="Unload selected", width=100, button_style='outline',
-                                                     button_type='danger', disabled=True)
+        self.unload_selected_button: Button = Button(name="Unload selected", width=120, button_style='outline', button_type='danger', disabled=True, align='end')
         self.unload_selected_button.on_click(self.unload_selected)
+        self.unload_all_button: Button = Button(name="Unload all", width=120, button_style='solid', button_type='danger', disabled=True, align='end')
+        self.unload_all_button.on_click(self.unload_all)
+        self.unload_col: Column = Column(self.unload_selected_button, self.unload_all_button)
 
         self.loaded_file_info = Markdown()
         
-        self.corpus_name_input = TextInput(placeholder='Corpus name', width=150, visible=False)
-        self.build_button = Button(name='Build corpus', button_style='solid', button_type='success', visible=False)
+        self.corpus_name_input = TextInput(placeholder='Corpus name', width=150)
+        self.build_button: Button = Button(name='Build corpus', button_style='solid', button_type='success')
         self.build_button.on_click(self.build_corpus)
+        build_tool_tip: TooltipIcon = self.view_handler.get_tooltip('build_button')
+        self.build_button_row: Row = Row(self.corpus_name_input, self.build_button, build_tool_tip, visible=False, align='end')
 
-        self.file_selector = FileSelectorWidget(view_handler, controller)
+        self.file_selector = FileSelectorWidget(view_handler, controller, width=self.LOADER_WIDTH)
         self.file_selector.set_button_operation_fn(self._set_button_status_on_operation)
         self.meta_editor = MetaEditorWidget(view_handler, controller)
 
         self.panel = Row(
             Column(
                 self.file_selector,
                 Row(Column(
-                    Row(self.load_as_corpus_button,
-                        self.load_as_meta_button),
-                    Row(self.corpus_name_input,
-                        self.build_button),
-                    Row(self.controller.tqdm_obj)
+                    Row(self.load_as_corpus_row,
+                        self.load_as_meta_row),
+                    self.build_button_row
                 ),
                     self.loaded_file_info,
                     HSpacer(),
-                    self.unload_selected_button,
-                    self.unload_all_button,
-                    width=700)
+                    self.unload_col,
+                    width=self.LOADER_WIDTH),
+                Row(self.controller.get_build_progress_bar())
             ),
             Spacer(width=50),
             self.meta_editor)
         self.children = [self.file_selector, self.meta_editor]
         self.update_display()
 
     def update_display(self):
@@ -70,18 +74,17 @@
         for filetype in file_counts:
             count_str += f"{filetype}: {file_counts[filetype]}\n"
 
         return count_str
 
     def _set_build_buttons_status(self, *_):
         files_added: bool = self.controller.is_meta_added() or self.controller.is_corpus_added()
-        self.corpus_name_input.visible = files_added
-        self.build_button.visible = files_added
-        self.unload_all_button.disabled = not files_added
+        self.build_button_row.visible = files_added
         self.unload_selected_button.disabled = not files_added
+        self.unload_all_button.disabled = not files_added
 
     def _set_button_status_on_operation(self, curr_loading: bool, *_):
         self.file_selector.selector_widget.disabled = curr_loading
         self.file_selector.show_hidden_files_checkbox.disabled = curr_loading
         self.file_selector.expand_archive_checkbox.disabled = curr_loading
         self.file_selector.select_all_button.disabled = curr_loading
         self.file_selector.file_type_filter.disabled = curr_loading
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/FileSelectorWidget.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/FileSelectorWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,55 +3,60 @@
 
 import panel
 from panel import Row, Column
 from panel.widgets import Button, MultiSelect, TextInput, Select, Checkbox
 
 from atap_corpus_loader.controller import Controller
 from atap_corpus_loader.controller.data_objects import FileReference
+from atap_corpus_loader.view import ViewWrapperWidget
 from atap_corpus_loader.view.gui import AbstractWidget
 
 
 class FileSelectorWidget(AbstractWidget):
-    def __init__(self, view_handler: AbstractWidget, controller: Controller):
+    def __init__(self, view_handler: ViewWrapperWidget, controller: Controller, width: int):
         super().__init__()
-        self.view_handler: AbstractWidget = view_handler
+        self.view_handler: ViewWrapperWidget = view_handler
         self.controller: Controller = controller
         # The function will be set by an instance method, but must be callable until then
         self._set_button_status_on_operation: Callable = lambda curr_loading: None
 
         self.select_all_button = Button(name="Select all", width=95,
                                         button_style="solid", button_type="primary")
         self.select_all_button.on_click(self.select_all)
 
-        self.filter_input = TextInput(placeholder="Filter displayed files (supports wildcard syntax)",
+        self.filter_input = TextInput(placeholder="Filter displayed files\t\t\t\N{DOWNWARDS ARROW WITH CORNER LEFTWARDS}",
                                       sizing_mode='stretch_width')
         self.filter_input.param.watch(self._on_filter_change, ['value'])
+        filter_input_tooltip = self.view_handler.get_tooltip('file_filter_input')
+        self.filter_row: Row = Row(self.filter_input, filter_input_tooltip)
 
         self.show_hidden_files_checkbox = Checkbox(name="Show hidden", value=False, align="start")
         self.show_hidden_files_checkbox.param.watch(self._on_filter_change, ['value'])
 
         self.expand_archive_checkbox = Checkbox(name="Expand archives", value=False, align="start")
         self.expand_archive_checkbox.param.watch(self._on_filter_change, ['value'])
 
         self.file_type_filter = Select(name='Filter by filetype', width=150)
         self.file_type_filter.options = ['All valid filetypes'] + self.controller.get_valid_filetypes()
         self.file_type_filter.param.watch(self._on_filter_change, ['value'])
 
-        self.selector_widget = MultiSelect(size=20, sizing_mode='stretch_width')
+        self.selector_widget = MultiSelect(size=10, sizing_mode='stretch_width')
 
         self.panel = Column(
-            Row(self.select_all_button),
-            Row(self.filter_input,
+            Row(Column(
+                self.filter_row,
+                self.select_all_button
+            ),
                 Column(
                     self.show_hidden_files_checkbox,
                     self.expand_archive_checkbox
                 ),
                 self.file_type_filter),
             Row(self.selector_widget),
-            width=700)
+            width=width)
 
         panel.state.add_periodic_callback(self.update_display, period=2000)
         self.update_display()
 
     def set_button_operation_fn(self, _set_button_status_on_operation: Callable):
         self._set_button_status_on_operation = _set_button_status_on_operation
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/gui/MetaEditorWidget.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/gui/MetaEditorWidget.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,57 +2,65 @@
 
 from panel import Column, GridBox, bind, Row, Spacer
 from panel.pane import Markdown, Str
 from panel.widgets import Select, Checkbox
 
 from atap_corpus_loader.controller import Controller
 from atap_corpus_loader.controller.data_objects.CorpusHeader import CorpusHeader
+from atap_corpus_loader.view import ViewWrapperWidget
 from atap_corpus_loader.view.gui import AbstractWidget
 
 
 class MetaEditorWidget(AbstractWidget):
     TABLE_BORDER_STYLE = {'border': '1px dashed black', 'border-radius': '5px'}
     ERROR_BORDER_STYLE = {'border': '1px solid red', 'border-radius': '5px'}
     HEADER_STYLE = {'margin-top': '0', 'margin-bottom': '0'}
 
-    def __init__(self, view_handler: AbstractWidget, controller: Controller):
+    def __init__(self, view_handler: ViewWrapperWidget, controller: Controller):
         super().__init__()
-        self.view_handler: AbstractWidget = view_handler
+        self.view_handler: ViewWrapperWidget = view_handler
         self.controller: Controller = controller
 
         self.corpus_table_container = GridBox(styles=MetaEditorWidget.TABLE_BORDER_STYLE)
         self.meta_table_container = GridBox(styles=MetaEditorWidget.TABLE_BORDER_STYLE)
 
-        self.corpus_table_title = Markdown("## Corpus editor")
-        self.meta_table_title = Markdown("## Metadata editor")
+        corpus_table_title = Markdown("## Corpus editor")
+        corpus_table_tooltip = self.view_handler.get_tooltip('corpus_editor')
+        self.corpus_table_row: Row = Row(corpus_table_title, corpus_table_tooltip)
+
+        meta_table_title = Markdown("## Metadata editor")
+        meta_table_tooltip = self.view_handler.get_tooltip('meta_editor')
+        self.meta_table_row: Row = Row(meta_table_title, meta_table_tooltip)
 
         self.text_header_dropdown = Select(name='Select document label', width=200)
         text_header_fn = bind(self._set_text_header, self.text_header_dropdown)
 
         self.link_row = Row(visible=False, styles=MetaEditorWidget.ERROR_BORDER_STYLE)
-        self.corpus_link_dropdown = Select(name='Select corpus linking label', width=200)
+        link_row_tooltip = self.view_handler.get_tooltip('linking_selectors')
+        self.corpus_link_dropdown = Select(name='Select corpus linking label', width=180)
         corpus_link_fn = bind(self._set_corpus_link_header, self.corpus_link_dropdown)
-        self.meta_link_dropdown = Select(name='Select metadata linking label', width=200)
+        self.meta_link_dropdown = Select(name='Select metadata linking label', width=180)
         meta_link_fn = bind(self._set_meta_link_header, self.meta_link_dropdown)
         link_emoji = '\U0001F517'
         self.link_markdown = Str(link_emoji, styles={"font-size": "2em", "margin": "auto"})
-        self.link_row.objects = [self.corpus_link_dropdown,
-                                 self.link_markdown,
+        self.link_row.objects = [link_row_tooltip,
+                                 self.corpus_link_dropdown,
+                                 self.link_markdown.clone(),
                                  self.meta_link_dropdown,
                                  Column(corpus_link_fn, visible=False),
                                  Column(meta_link_fn, visible=False)]
 
         self.panel = Column(
-            self.corpus_table_title,
+            self.corpus_table_row,
             Row(self.text_header_dropdown, text_header_fn),
             self.corpus_table_container,
             Spacer(height=20),
             self.link_row,
             Spacer(height=20),
-            self.meta_table_title,
+            self.meta_table_row,
             self.meta_table_container
         )
         self.update_display()
 
     def update_display(self):
         self._build_corpus_table()
         self._build_meta_table()
@@ -91,48 +99,48 @@
             table_cells.append(Markdown(header.name, align='start', styles=MetaEditorWidget.HEADER_STYLE))
 
             datatype_selector = Select(options=all_datatypes, value=header.datatype.name, width=120, disabled=is_text)
             if is_meta_table:
                 dtype_fn = bind(self.controller.update_meta_header, header, None, datatype_selector)
             else:
                 dtype_fn = bind(self.controller.update_corpus_header, header, None, datatype_selector)
-            table_cells.append(Row(datatype_selector, dtype_fn))
+            table_cells.append(Row(datatype_selector, Column(dtype_fn, visible=False)))
 
             include_checkbox = Checkbox(value=header.include, align='center', disabled=(is_text or is_link))
             if is_meta_table:
                 include_fn = bind(self.controller.update_meta_header, header, include_checkbox, None)
             else:
                 include_fn = bind(self.controller.update_corpus_header, header, include_checkbox, None)
-            table_cells.append(Row(include_checkbox, include_fn))
+            table_cells.append(Row(include_checkbox, Column(include_fn, visible=False)))
 
             if self.controller.is_meta_added():
                 if is_link:
                     link_identifier = self.link_markdown.clone()
                 else:
                     link_identifier = ' '
                 table_cells.append(link_identifier)
 
         return ncols, table_cells
 
     def _build_corpus_table(self):
         is_corpus_added = self.controller.is_corpus_added()
-        self.corpus_table_title.visible = is_corpus_added
+        self.corpus_table_row.visible = is_corpus_added
         self.corpus_table_container.visible = is_corpus_added
 
         corpus_headers: list[CorpusHeader] = self.controller.get_corpus_headers()
         link_header: Optional[CorpusHeader] = self.controller.get_corpus_link_header()
 
         ncols, corpus_table_cells = self._get_table_cells_list(corpus_headers, link_header, False)
 
         self.corpus_table_container.objects = corpus_table_cells
         self.corpus_table_container.ncols = ncols
 
     def _build_meta_table(self):
         is_meta_added = self.controller.is_meta_added()
-        self.meta_table_title.visible = is_meta_added
+        self.meta_table_row.visible = is_meta_added
         self.meta_table_container.visible = is_meta_added
 
         meta_headers: list[CorpusHeader] = self.controller.get_meta_headers()
         link_header: Optional[CorpusHeader] = self.controller.get_meta_link_header()
 
         ncols, meta_table_cells = self._get_table_cells_list(meta_headers, link_header, True)
```

### Comparing `atap_corpus_loader-1.2.3/atap_corpus_loader/view/notifications/NotifierService.py` & `atap_corpus_loader-1.3.0/atap_corpus_loader/view/notifications/NotifierService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.2.3/pyproject.toml` & `atap_corpus_loader-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "atap-corpus-loader"
-version = "1.2.3"
+version = "1.3.0"
 description = " A GUI loader for atap_corpus using the Panel library."
 authors = ["Hamish Croser <hamish.croser@sydney.edu.au>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "atap_corpus_loader"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.12.0"
 pandas = "~=2.1.0"
-atap_corpus = "~=0.1.12"
+atap_corpus = "~=0.1.13"
 odfpy = "~=1.4.0"
-panel = "~=1.3.0"
+panel = "~=1.4.0"
 pyreadr = "~=0.5.0"
 python-docx = "~=1.1.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `atap_corpus_loader-1.2.3/PKG-INFO` & `atap_corpus_loader-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: atap-corpus-loader
-Version: 1.2.3
+Version: 1.3.0
 Summary:  A GUI loader for atap_corpus using the Panel library.
 License: MIT
 Author: Hamish Croser
 Author-email: hamish.croser@sydney.edu.au
 Requires-Python: >=3.10.0,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: atap_corpus (>=0.1.12,<0.2.0)
+Requires-Dist: atap_corpus (>=0.1.13,<0.2.0)
 Requires-Dist: odfpy (>=1.4.0,<1.5.0)
 Requires-Dist: pandas (>=2.1.0,<2.2.0)
-Requires-Dist: panel (>=1.3.0,<1.4.0)
+Requires-Dist: panel (>=1.4.0,<1.5.0)
 Requires-Dist: pyreadr (>=0.5.0,<0.6.0)
 Requires-Dist: python-docx (>=1.1.0,<1.2.0)
 Description-Content-Type: text/markdown
 
 # Corpus Loader
 
 A GUI loader for atap_corpus using the Panel library. Provides a single Panel-compatible widget in which a user can construct a corpus object for use by the client code.
```

