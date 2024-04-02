# Comparing `tmp/TkEasyGUI-0.2.38.tar.gz` & `tmp/tkeasygui-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TkEasyGUI-0.2.38.tar", last modified: Tue Apr  2 04:22:58 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.4.tar", last modified: Thu Mar 21 03:29:01 2024, max compression
```

## Comparing `TkEasyGUI-0.2.38.tar` & `tkeasygui-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-02 04:22:58.449664 TkEasyGUI-0.2.38/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 TkEasyGUI-0.2.38/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     4996 2024-04-02 04:22:58.449368 TkEasyGUI-0.2.38/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     2567 2024-04-02 01:24:32.000000 TkEasyGUI-0.2.38/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-02 04:22:58.446643 TkEasyGUI-0.2.38/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      285 2024-03-25 13:03:18.000000 TkEasyGUI-0.2.38/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    16967 2024-03-25 13:04:01.000000 TkEasyGUI-0.2.38/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-02 04:22:56.000000 TkEasyGUI-0.2.38/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    96111 2024-04-02 04:19:04.000000 TkEasyGUI-0.2.38/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-02 04:22:58.448742 TkEasyGUI-0.2.38/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     4996 2024-04-02 04:22:58.000000 TkEasyGUI-0.2.38/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      281 2024-04-02 04:22:58.000000 TkEasyGUI-0.2.38/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-02 04:22:58.000000 TkEasyGUI-0.2.38/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        7 2024-04-02 04:22:58.000000 TkEasyGUI-0.2.38/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-02 04:22:58.000000 TkEasyGUI-0.2.38/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1331 2024-04-02 04:22:50.000000 TkEasyGUI-0.2.38/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-02 04:22:58.449886 TkEasyGUI-0.2.38/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-03-21 03:29:01.411888 tkeasygui-0.2.4/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.4/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4619 2024-03-21 03:29:01.411627 tkeasygui-0.2.4/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2207 2024-03-21 01:48:30.000000 tkeasygui-0.2.4/README.md
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1314 2024-03-21 03:28:22.000000 tkeasygui-0.2.4/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-03-21 03:29:01.411945 tkeasygui-0.2.4/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-03-21 03:29:01.410011 tkeasygui-0.2.4/tkeasygui/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      184 2024-03-21 03:28:27.000000 tkeasygui-0.2.4/tkeasygui/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6349 2024-03-20 07:07:30.000000 tkeasygui-0.2.4/tkeasygui/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    58602 2024-03-21 03:26:34.000000 tkeasygui-0.2.4/tkeasygui/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-03-21 03:29:01.411280 tkeasygui-0.2.4/tkeasygui.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4619 2024-03-21 03:29:01.000000 tkeasygui-0.2.4/tkeasygui.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      260 2024-03-21 03:29:01.000000 tkeasygui-0.2.4/tkeasygui.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-03-21 03:29:01.000000 tkeasygui-0.2.4/tkeasygui.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        7 2024-03-21 03:29:01.000000 tkeasygui-0.2.4/tkeasygui.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-03-21 03:29:01.000000 tkeasygui-0.2.4/tkeasygui.egg-info/top_level.txt
```

### Comparing `TkEasyGUI-0.2.38/LICENSE` & `tkeasygui-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TkEasyGUI-0.2.38/PKG-INFO` & `tkeasygui-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: TkEasyGUI
-Version: 0.2.38
-Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
+Name: tkeasygui
+Version: 0.2.4
+Summary: TkEasyGUI is Easy and Simple GUI Library
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,51 +44,45 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 
 # TkEasyGUI
 
-`TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
+**TkEasyGUI** is a Python library that allows for the easy and simple creation of GUI applications.
 In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
 Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
 
 This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
-- [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
-
-## Platform
-
-- Windows / macOS / Linux (tkinter required)
+- [👉日本語のREADME](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md)
 
 ## Install
 
 Install from pypi
 
 
 ```sh
-python -m pip install TkEasyGUI
+python -m pip install tkeasygui
 ```
 
 Install from GitHub Repository
 
 
 ```sh
 python -m pip install git+https://github.com/kujirahand/tkeasygui-python
 ```
 
-- (memo) Updating from older versions (less than 0.2.24) will fail. ([See the solution](https://github.com/kujirahand/tkeasygui-python/blob/main/docs/installation_trouble.md))
-
 ## How to use
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
-import TkEasyGUI as eg
+import tkeasygui as eg
 
 # Create window
 layout = [
     [eg.Text("Hello, World!")],
     [eg.Button("OK")]
 ]
 window = eg.Window("Hello", layout=layout)
@@ -114,17 +108,20 @@
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
 ## About the relationship with PySimpleGUI
 
-- When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
-- The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
-- This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
-- We are not considering full compatibility with PySimpleGUI.
+Fundamentally, it is compatible with PySimpleGUI. Programs can be written using the same event model. 
+It should be noted that while it was developed with reference to PySimpleGUI, it has been reimplemented from scratch.
+Many unique features have been expanded.
+The basic Elements have been given the same names. However, the names of some properties are different.
+
+We are not considering full compatibility with PySimpleGUI.
+
 
 ## Link
 
 - [pypi.org > TkEasyGUI](https://pypi.org/project/tkeasygui/)
 - [GitHub > TkEasyGUI](https://github.com/kujirahand/tkeasygui-python/)
```

### Comparing `TkEasyGUI-0.2.38/README.md` & `tkeasygui-0.2.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 # TkEasyGUI
 
-`TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
+**TkEasyGUI** is a Python library that allows for the easy and simple creation of GUI applications.
 In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
 Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
 
 This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
-- [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
-
-## Platform
-
-- Windows / macOS / Linux (tkinter required)
+- [👉日本語のREADME](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md)
 
 ## Install
 
 Install from pypi
 
 
 ```sh
-python -m pip install TkEasyGUI
+python -m pip install tkeasygui
 ```
 
 Install from GitHub Repository
 
 
 ```sh
 python -m pip install git+https://github.com/kujirahand/tkeasygui-python
 ```
 
-- (memo) Updating from older versions (less than 0.2.24) will fail. ([See the solution](https://github.com/kujirahand/tkeasygui-python/blob/main/docs/installation_trouble.md))
-
 ## How to use
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
-import TkEasyGUI as eg
+import tkeasygui as eg
 
 # Create window
 layout = [
     [eg.Text("Hello, World!")],
     [eg.Button("OK")]
 ]
 window = eg.Window("Hello", layout=layout)
@@ -66,17 +60,20 @@
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
 ## About the relationship with PySimpleGUI
 
-- When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
-- The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
-- This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
-- We are not considering full compatibility with PySimpleGUI.
+Fundamentally, it is compatible with PySimpleGUI. Programs can be written using the same event model. 
+It should be noted that while it was developed with reference to PySimpleGUI, it has been reimplemented from scratch.
+Many unique features have been expanded.
+The basic Elements have been given the same names. However, the names of some properties are different.
+
+We are not considering full compatibility with PySimpleGUI.
+
 
 ## Link
 
 - [pypi.org > TkEasyGUI](https://pypi.org/project/tkeasygui/)
 - [GitHub > TkEasyGUI](https://github.com/kujirahand/tkeasygui-python/)
```

### Comparing `TkEasyGUI-0.2.38/TkEasyGUI/widgets.py` & `tkeasygui-0.2.4/tkeasygui/widgets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,88 @@
 """
 TkEasyGUI Widgets
 """
 import io
 import os
-import sys
 import tkinter as tk
 from datetime import datetime
 from queue import Queue
 from tkinter import ttk
-from typing import Any, Literal, TypeAlias, Union
+from typing import Any, Literal, TypeAlias
 
 from PIL import Image as PILImage
 from PIL import ImageTk
 
-import TkEasyGUI as eg
+import tkeasygui as eg
 
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
 WINDOW_TIMEOUT: str = "-TIMEOUT-"
-LISTBOX_SELECT_MODE_MULTIPLE: str = "multiple"
-LISTBOX_SELECT_MODE_BROWSE: str = "browse"
-LISTBOX_SELECT_MODE_EXTENDED: str = "extended"
-LISTBOX_SELECT_MODE_SINGLE: str = "single"
+LISTBOX_SELECT_MODE_MULTIPLE: str = 'multiple'
+LISTBOX_SELECT_MODE_BROWSE: str = 'browse'
+LISTBOX_SELECT_MODE_EXTENDED: str = 'extended'
+LISTBOX_SELECT_MODE_SINGLE: str = 'single'
 TABLE_SELECT_MODE_NONE: str = tk.NONE
 TABLE_SELECT_MODE_BROWSE: str = tk.BROWSE
 TABLE_SELECT_MODE_EXTENDED: str = tk.EXTENDED
-EG_SWAP_EVENT_NAME: str = "--swap_event_name--"
 
 # type
-WindowType: TypeAlias = "Window"
-ElementType: TypeAlias = "Element"
 TextAlign: TypeAlias = Literal["left", "right", "center"]
 TextVAlign: TypeAlias = Literal["top", "bottom", "center"]
-FontType: TypeAlias = tuple[str, int] | tuple[str, int, str]
+FontType: TypeAlias = tuple[str, int]
 PointType: TypeAlias = tuple[int, int] | tuple[float, float]
+ElementType: TypeAlias = "Element"
 EventMode: TypeAlias = Literal["user", "system"]
 OrientationType: TypeAlias = Literal["v", "h", "vertical", "horizontal"]
 ListboxSelectMode: TypeAlias = Literal["multiple", "browse", "extended", "single"]
-PadType: TypeAlias = int | tuple[int, int] | tuple[tuple[int, int], tuple[int, int]]
-ReliefType: TypeAlias = Literal["flat", "groove", "raised", "ridge", "solid", "sunken"]
-
 # about color (Thanks)
 # https://kuroro.blog/python/YcZ6Yh4PswqUzaQXwnG2/
 
 #------------------------------------------------------------------------------
-# theme
-_tkeasygui_info: dict[str, Any] = {}
-def theme(name: str) -> None:
-    """Set theme"""
-    _tkeasygui_info["theme"] = name
-
-#------------------------------------------------------------------------------
 # Widget wrapper
 #------------------------------------------------------------------------------
 class TkEasyError(Exception):
     def __init__(self, message="TkEasyError"):
         self.message = message
         super().__init__(self.message)
 
-# Prioritize compatibility with PySimpleGUI
-_compatibility: bool = True
-def set_PySimpleGUI_compatibility(flag: bool=True) -> None:
-    """Set compatibility with PySimpleGUI (Default=True)"""
-    global _compatibility
-    _compatibility = flag
-
 # only one root element
-_root_window: tk.Tk|None = None
-_ttk_style: ttk.Style|None = None
+_root_window: tk.Tk | None = None
 def get_root_window() -> tk.Tk:
     """Get root window."""
     global _root_window
     if _root_window is None:
-        _root_window = tk._get_default_root() # tk.Tk()
-        _root_window.eval('tk::PlaceWindow . center')
+        _root_window = tk.Tk()
         _root_window.attributes('-alpha', 0)
-        _root_window.withdraw()
-        # set theme
-        try:
-            if "theme" in _tkeasygui_info:
-                name = _tkeasygui_info["theme"]
-                _ttk_style = get_ttk_style()
-                _ttk_style.theme_use(name)
-        except Exception as e:
-            print(f"TkEasyGUI.theme: failed to set theme {name} {e}", file=sys.stderr)
-            pass
     return _root_window
 
-def get_font_list() -> list[str]:
-    """Get font list"""
-    root = get_root_window()
-    root.withdraw()
-    return list(tk.font.families())
-
-def get_ttk_style() -> ttk.Style:
-    """Get ttk style"""
-    global _ttk_style
-    if _ttk_style is None:
-        _ttk_style = ttk.Style()
-    return _ttk_style
-
 # active window
-_window_list: list[WindowType] = []
+_window_list: list["Window"] = []
 def _get_active_window() -> tk.Toplevel|None:
     """Get the active window."""
     if len(_window_list) == 0:
         return None
     return _window_list[-1].window
 
-def _window_push(win: WindowType) -> None:
+def _window_push(win: "Window") -> None:
     """Push a window to the list."""
     _window_list.append(win)
 
-def _window_pop(win: WindowType) -> None:
+def _window_pop() -> None:
     """Pop a window from the list."""
-    i = _window_list.index(win)
-    if i >= 0:
-        _window_list.pop()
+    _window_list.pop()
 
 class Window:
     """
     Main window object in TkEasyGUI
     """
-    def __init__(
-                self,
-                title: str,
-                layout: list[list[ElementType]],
-                size: tuple[str, int]|None=None, 
-                resizable:bool=False,
-                font:FontType|None=None,
-                modal: bool=False, 
-                keep_on_top:bool=False, # keep on top
-                no_titlebar: bool=False, # hide titlebar
-                grab_anywhere: bool=False, # can move window by dragging anywhere
-                alpha_channel: float=1.0,
-                **kw) -> None:
+    def __init__(self, title: str, layout: list[list[ElementType]], size: (tuple[str, int]|None)=None, resizable:bool=False, modal: bool=False, **kw) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = _get_active_window()
         if active_win is None:
             active_win = get_root_window()
         self.window: tk.Toplevel = tk.Toplevel(master=active_win)
@@ -151,49 +92,27 @@
         self.focus_timer_id: str|None = None
         self.events: Queue = Queue()
         self.key_elements: dict[str, Element] = {}
         self.last_values: dict[str, Any] = {}
         self.flag_alive: bool = True # Pressing the close button will turn this flag to False.
         self.layout: list[list[ElementType]] = layout
         self._event_hooks: dict[str, list[callable]] = {}
-        self.font: FontType|None = font
-        self.radio_group_dict: dict[str, list[tk.IntVar, int]] = {}
-        self.minimized: bool = False
-        self.maximized: bool = False
-        self.is_hidden: bool = False
-        self._keep_on_top: bool = keep_on_top
-        self._no_titlebar: bool = no_titlebar
-        self._grab_anywhere: bool = grab_anywhere
-        self._grab_flag: bool = False
-        self._start_x: int|None = None
-        self._start_y: int|None = None
-        self._mouse_x: int|None = None
-        self._mouse_y: int|None = None
-        self.alpha_channel: float = alpha_channel
         # Frame
         self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         if size is not None:
             self.window.geometry(f"{size[0]}x{size[1]}")
         self.window.resizable(resizable, resizable)
         # create widgets
         self._create_widget(self.frame, layout)
         # pack frame
         self.frame.pack(expand=True, fill="both")
         self.frame.rowconfigure(0, weight=1)
-        if keep_on_top:
-            self.window.attributes("-topmost", True)
-        if no_titlebar:
-            self.hide_titlebar(True)
-        if grab_anywhere:
-            self.set_grab_anywhere(True)
-        if alpha_channel < 1.0:
-            self.set_alpha_channel(alpha_channel)
         # check modal
         if modal:
             # check position
             parent = active_win
             if parent is not None:
                 self.window.geometry(f"+{parent.winfo_x()+20}+{parent.winfo_y()+20}")
             # set modal action
@@ -201,16 +120,15 @@
             # self.window.transient(parent)
             self.window.grab_set()
             self.window.focus_force()
         else:
             if isinstance(self.window, tk.Tk):
                 self.window.eval('tk::PlaceWindow . center')
         # push window
-        if not modal:
-            _window_push(self)
+        _window_push(self)
     
     def register_event_hooks(self, hooks: dict[str, list[callable]]) -> None:
         """
         [Window.register_event_hooks] Register event hooks. (append events)
         **Example**
         ```
         window.register_event_hooks({
@@ -223,114 +141,81 @@
         ```
         **Note**
         - If you specify a function that returns True, it changes the event name to f"{event}-stopped" and then re-collects the values associated with keys that occur afterwards.
         - @see `Window.read`
         """
         for event_name, handle_list in hooks.items():
             for handle in handle_list:
-                if event_name not in self._event_hooks:
+                if not (event_name in self._event_hooks):
                     self._event_hooks[event_name] = []
                 self._event_hooks[event_name].append(handle)
     
     def _create_widget(self, parent: tk.Widget, layout: list[list["Element"]]):
         """create widget from layout"""
         # check layout
         if not (len(layout) > 0 and (isinstance(layout[0], list) or isinstance(layout[0], tuple))):
             raise TkEasyError(f"Invalid layout, should specify a two-dimensional list: {layout}")
         # prepare create
         for widgets in layout:
             for elem in widgets:
                 elem.prepare_create(self)
         # create widgets
         self.need_focus_widget: tk.Widget|None = None
-        for row_no, widgets in enumerate(layout):
-            frame_row = ttk.Frame(parent, padding=5, name=f"tkeasygui_frame_row_{row_no}")
+        for widgets in layout:
+            frame_row = ttk.Frame(parent, padding=5)
             # columns
             prev_element: Element|None = None
-            row_prop: dict[str, Any] = {"expand": False, "fill": "x", "side": "top"}
-            for col_no, elemment in enumerate(widgets):
+            row_prop: dict[str, Any] = {"expand": True, "fill": "x", "side": "top"}
+            for _col, elemment in enumerate(widgets):
                 # create widget
                 elem: Element = elemment
                 # set window and parent
                 elem.window = self
                 elem.parent = frame_row
-                elem.col_no = col_no
-                elem.row_no = row_no
                 # set prev_element and next_element
                 elem.prev_element = prev_element # set prev_element
                 if prev_element is not None:
                     prev_element.next_element = elem
                 prev_element = elem
-                # create widget
                 try:
                     widget: tk.Widget = elem.create(self, frame_row)
-                    widget.__tkeasygui = elem # type : ignore
-                except Exception as e:
-                    print(e.__traceback__, file=sys.stderr)
-                    raise TkEasyError(
-                        f"Window._create_widget.Failed `{elem.element_type}` key=`{elem.get_name()}` {elem.props} reason:{e}"
-                    ) from e
-                # check key
-                if elem.has_value or (elem.key is not None):
+                    # check key
                     self.key_elements[elem.key] = elem
-                # check focus widget
-                if elem.has_value and (self.need_focus_widget is None):
-                    self.need_focus_widget = widget
-                # check specila key
-                if (self.need_focus_widget is None) and (elem.key == "OK" or elem.key == "Yes"):
-                    self.need_focus_widget = widget
-                # create sub widgets
-                try:
+                    # check focus widget
+                    if elem.has_value and (self.need_focus_widget is None):
+                        self.need_focus_widget = widget
+                    # check specila key
+                    if (self.need_focus_widget is None) and (elem.key == "OK" or elem.key == "Yes"):
+                        self.need_focus_widget = widget
                     # has children?
                     if elem.has_children:
                         self._create_widget(widget, elem.layout)
                 except Exception as e:
-                    raise TkEasyError(
-                        f"Window._create_widget.Failed_sub_widgets `{elem.element_type}` key=`{elem.key}` {elem.props} reason:{e}"
-                    ) from e
-                # post create
-                elem.post_create(self, frame_row)
+                    raise Exception(f"Failed to create widget: {elem.element_type} {elem.key} {elem.props}\n{e}") from e
                 # bind event (before create)
                 for event_name, handle_t in elem._bind_dict.items():
                     self.bind(elem, event_name, handle_t[0], handle_t[1], handle_t[2])
-                # menu ?
-                if isinstance(elem, Menu):
-                    continue
                 # pack widget
                 fill_props = elem._get_pack_props()
                 widget.pack(**fill_props)
-                # expand_y?
+                # debug
                 if elem.expand_y:
-                    row_prop["expand"] = True
                     row_prop["fill"] = "both"
             # add row
             frame_row.pack(**row_prop)
         # end of create
         if self.need_focus_widget is not None:
             # print("focus_set", self.need_focus_widget)
             self.need_focus_widget.focus_set()
 
     def move_to_center(self) -> None:
         """Move the window to the center of the screen."""
         if isinstance(self.window, tk.Tk):
             self.window.eval('tk::PlaceWindow . center')
 
-    def get_element_by_key(self, key: str) -> Union[ElementType, None]:
-        """Get an element by its key."""
-        return self.key_elements[key] if key in self.key_elements else None
-    
-    def get_elements_by_type(self, element_type: str) -> list[ElementType]:
-        """Get elements by type."""
-        result: list[ElementType] = []
-        for rows in self.layout:
-            for elem in rows:
-                if elem.element_type.lower() == element_type.lower():
-                    result.append(elem)
-        return result
-
     def read(self, timeout: int|None=None, timeout_key: str="-TIMEOUT-") -> tuple[str, dict[str, Any]]:
         """ [Window.read] Read events from the window."""
         self.timeout = timeout
         self.timeout_key = timeout_key
         time_id = time_checker_start()
         while True:
             # set timeout
@@ -368,53 +253,14 @@
         if key in self._event_hooks:
             for handle in self._event_hooks[key]:
                 result = handle(key, values)
                 if result is True:
                     flag_stop = True
                     break
         return flag_stop
-    
-    def set_title(self, title: str) -> None:
-        """Set the title of the window."""
-        self.window.title(title)
-
-    def minimize(self) -> None:
-        """Minimize the window."""
-        self.window.iconify()
-        self.minimized = True
-
-    def normal(self) -> None:
-        """set normal window."""
-        if self.minimized:
-            self.window.deiconify()
-            self.minimized = False
-        if self.maximized:
-            self.window.state("normal")
-            self.maximized = False
-
-    def hide(self) -> None:
-        """Hide the window."""
-        self.window.withdraw()
-        self.is_hidden = True
-
-    def un_hide(self) -> None:
-        """Un hide the window."""
-        if self.is_hidden:
-            self.window.deiconify()
-            self.is_hidden = False
-
-    def maximize(self) -> None:
-        """Maximize the window. (`resizable` should be set to True)"""
-        self.window.state("zoomed")
-        self.maximized = True
-    
-    def set_alpha_channel(self, alpha: float) -> None:
-        """Set the alpha channel of the window."""
-        self.window.attributes("-alpha", alpha)
-        self.alpha_channel = alpha
 
     def get_values(self) -> dict[str, Any]:
         """Get values from the window."""
         values: dict[str, Any] = {}
         for key,val in self.key_elements.items():
             if not val.has_value:
                 continue
@@ -435,17 +281,14 @@
     def _event_handler(self, key: str, values: dict[str, Any]|None) -> None:
         """Handle an event."""
         # set value
         if values is None:
             values = {}
         for k, v in self.get_values().items():
             values[k] = v
-        # check EG_SWAP_EVENT_NAME
-        if EG_SWAP_EVENT_NAME in values:
-            key = values.pop(EG_SWAP_EVENT_NAME)
         # put event
         self.events.put((key, values))
         _exit_mainloop()
     
     def _exit_main_loop(self) -> None:
         """Exit mainloop"""
         if self.timeout_id is not None:
@@ -454,42 +297,23 @@
 
     def _close_handler(self):
         """Handle a window close event."""
         self.flag_alive = False
         if self.timeout_id is not None:
             self.window.after_cancel(self.timeout_id)
         self._event_handler(WINDOW_CLOSED, None)
-    
-    def keep_on_top(self, flag: bool) -> None:
-        """Set the window to keep on top."""
-        self.window.attributes("-topmost", flag)
-        self._keep_on_top = flag
-    
-    def send_to_back(self) -> None:
-        """Send the window to the back, and make it not keep on top."""
-        self.window.attributes("-topmost", False)
-        self._keep_on_top = False
-        self.window.lower()
-
-    def hide_titlebar(self, flag: bool) -> None:
-        """Hide the titlebar."""
-        try:
-            self.window.overrideredirect(flag)
-            self._no_titlebar = flag
-        except Exception as e:
-            pass
 
     def close(self) -> None:
         """Close the window."""
         global active_window
         try:
+            _window_pop()
             self.flag_alive = False
             self.window.quit()
             self.window.destroy()
-            _window_pop(self)
         except Exception as _:
             pass
 
     def is_alive(self) -> bool:
         """Check if the window is alive."""
         return self.flag_alive
     
@@ -515,53 +339,14 @@
     def refresh(self) -> "Window":
         """Refresh window"""
         try:
             self.window.update()
         except Exception:
             pass
         return self
-
-    def set_grab_anywhere(self, flag: bool) -> None:
-        """Set grab anywhere"""
-        self._grab_anywhere = flag
-        if flag:
-            self.window.bind("<B1-Motion>", self._move_window)
-            self.window.bind("<ButtonPress-1>", self._start_move_window)
-            self.window.bind("<ButtonRelease-1>", self._stop_move_window)
-        else:
-            self.window.unbind("<B1-Motion>")
-            self.window.unbind("<ButtonPress-1>")
-            self.window.unbind("<ButtonRelease-1>")
-    
-    def _move_window(self, event: tk.Event) -> None:
-        """Move window"""
-        if (not self._grab_anywhere) or (self._grab_flag == False):
-            return
-        mouse_x = self.window.winfo_x() + event.x
-        mouse_y = self.window.winfo_y() + event.y
-        move_x = mouse_x - self._mouse_x
-        move_y = mouse_y - self._mouse_y
-        win_x = self._start_x + move_x
-        win_y = self._start_y + move_y
-        self.window.geometry(f"+{win_x}+{win_y}")
-
-    def _start_move_window(self, event: tk.Event) -> None:
-        """Start move window"""
-        self._grab_flag = True
-        loc = self.window.geometry().split("+")
-        self._start_x = int(loc[1])
-        self._start_y = int(loc[2])
-        self._mouse_x = self.window.winfo_x() + event.x
-        self._mouse_y = self.window.winfo_y() + event.y
-        # print(f"_start_xy={self._start_x}x{self._start_y}")
-        # print(f"_mouse_xy={self._mouse_x}x{self._mouse_y}")
-    
-    def _stop_move_window(self, event: tk.Event) -> None:
-        """Stop move window"""
-        self._grab_flag = False
     
     def bind(self, element: "Element", event_name: str, handle_name: str, propagate: bool=True, event_mode: EventMode = "user") -> None:
         """[Window.bind] Bind element event and handler"""
         element._bind_dict[event_name] = (handle_name, propagate, event_mode)
         if element.widget is None:
             return
         # bind to widget
@@ -617,60 +402,35 @@
     "ButtonText": "text",
     "label": "text",
     "caption": "text",
     "justify": "text_align"
 }
 class Element:
     """Element class."""
-    def __init__(
-            self,
-            element_type: str, # element type
-            ttk_style_name: str, # tkinter widget type
-            key: str|None, # key
-            has_value: bool, # has value
-            metadata: dict[str, Any]|None=None, # meta data
-            **kw) -> None:
+    def __init__(self, element_type: str, key: str|None, **kw) -> None:
         """Create an element."""
+        # check key
+        if key is None or key == "":
+            key = generate_element_key(element_type)
         # define properties
-        self.has_value: bool = has_value
-        self.key: str|int|None = key
-        if self.key is not None:
-            register_element_key(self.key) # for checking unique key
-        if self.has_value and (self.key is None or self.key == ""):
-            self.key = generate_element_id()
+        self.key: str = key
         self.element_type: str = element_type
-        self.ttk_style_name: str = ttk_style_name
-        self.use_ttk: bool = True if ttk_style_name != "" else False
-        self.metadata = metadata
-        self.style_name: str = self._generate_style_name(key)
+        self.has_value: bool = False
         self.props: dict[str, Any] = kw
         self.widget: Any|None = None
         self.expand_x: bool = False
         self.expand_y: bool = False
-        self.anchor: str|None = None
         self.has_children: bool = False
         self.prev_element: Element|None = None
         self.next_element: Element|None = None
         self.window: Window|None = None
         self.parent: tk.Widget|None = None
         self._bind_dict: dict[str, tuple[str, bool, EventMode]] = {}
         self.user_bind_event: tk.Event|None = None # when bind event fired then set this value
         self.vertical_alignment: TextVAlign = "center"
-        self.padx: int|tuple[int,int]|None = 1
-        self.pady: int|tuple[int,int]|None = None
-        self.font: FontType|None = None
-        self.has_font_prop: bool = True
-        self.col_no: int = -1
-        self.row_no: int = -1
-    
-    def get_name(self) -> str:
-        """Get element name."""
-        if self.key is None:
-            return "-unknown-"
-        return str(self.key)
     
     def bind(self, event_name: str, handle_name: str, propagate: bool=True, event_mode: EventMode = "user") -> None:
         """
         Bind event. @see `Window.bind`
         """
         self._bind_dict[event_name] = (handle_name, propagate, event_mode)
         if self.window is not None:
@@ -678,132 +438,56 @@
 
     def disptach_event(self, values: dict[str, Any]|None=None) -> None:
         """Dispatch event"""
         if values is None:
             values = {}
         if self.window is not None:
             self.window._event_handler(self.key, values)
-    
-    def _justify_to_anchor(self, justify: TextAlign) -> str:
-        """Convert justify to anchor"""
-        if justify == "left":
-            return "w"
-        if justify == "right":
-            return "e"
-        return "center"
-
-    def _set_pack_props(self,
-                expand_x: bool|None=None,
-                expand_y: bool|None=None,
-                pad: PadType=None) ->None:
-        """Set pack properties"""
-        if expand_x is not None:
-            self.expand_x = expand_x
-        if expand_y is not None:
-            self.expand_y = expand_y
-        if pad is not None:
-            if isinstance(pad, int):
-                self.padx = self.pady = pad
-            elif isinstance(pad, tuple):
-                self.padx = pad[0]
-                self.pady = pad[1]
-            else:
-                self.padx = pad[0][0]
-                self.pady = pad[0][1]
-
-    def _set_text_props(self,
-                font: FontType|None=None,
-                text_align: TextAlign|None=None,
-                color: str|None=None,
-                text_color: str|None=None,
-                background_color: str|None=None) ->None:
-        """set default props style"""
-        if font is not None:
-            self.props["font"] = font
-            self.font = font
-        if text_align is not None:
-            self.props["justify"] = text_align
-        if color is not None:
-            self.props["fg"] = color
-        if text_color is not None:
-            self.props["fg"] = text_color
-        if background_color is not None:
-            self.props["bg"] = background_color
 
     def _get_pack_props(self) -> dict[str, Any]:
         """Get the fill property in `pack` method."""
         props: dict[str, Any] = {"expand": False, "fill": "none", "side": "left"}
         # check expand
         if self.expand_x and self.expand_y:
             props["expand"] = True
             props["fill"] = "both"
         elif self.expand_x:
             props["expand"] = True
             props["fill"] = "x"
         elif self.expand_y:
             props["expand"] = True
             props["fill"] = "y"
-        # padx / pady
-        if self.padx is not None:
-            props["padx"] = self.padx
-        if self.pady is not None:
-            props["pady"] = self.pady
-        # anchor
-        if self.anchor is not None:
-            props["anchor"] = self.anchor
         # print("pack.props=", self.key, props)
         return props
 
-    def convert_props(self, props: dict[str, Any]) -> dict[str, Any]:
-        result = {}
-        # copy
-        for key, val in props.items():
-            result[key] = val
-        # check props
+    def prepare_create(self, win: Window) -> None:
+        # convert properties
         # size
-        if "size" in result:
-            size = result.pop("size", (8, 1))
-            result["width"] = size[0]
-            result["height"] = size[1]
+        if "size" in self.props:
+            size = self.props.pop("size", (8, 1))
+            self.props["width"] = size[0]
+            self.props["height"] = size[1]
         # background_color
-        if "background_color" in result:
-            result["bg"] = result.pop("background_color")
-        if "text_color" in result:
-            result["fg"] = result.pop("text_color")
-        if "color" in result:
-            result["fg"] = result.pop("color")
+        if "background_color" in self.props:
+            self.props["bg"] = self.props.pop("background_color")
+            # self.props["readonlybackground"] = self.props["bg"]
+        if "text_color" in self.props:
+            self.props["fg"] = self.props.pop("text_color")
         # expand_x
-        if "expand_x" in result:
-            self.expand_x = result.pop("expand_x")
-        if "expand_y" in result:
-            self.expand_y = result.pop("expand_y")
-        # padx / pady
-        if "padx" in result:
-            self.padx = result.pop("padx")
-        if "pady" in result:
-            self.pady = result.pop("pady")
-        # anchor
-        if "anchor" in result:
-            self.anchor = result.pop("anchor")
+        if "expand_x" in self.props:
+            self.expand_x = self.props.pop("expand_x")
+        if "expand_y" in self.props:
+            self.expand_y = self.props.pop("expand_y")
         # convert "select_mode" to "selectmode"
-        if "select_mode" in result:
-            result["selectmode"] = result.pop("select_mode")
+        if "select_mode" in self.props:
+            self.props["selectmode"] = self.props.pop("select_mode")
         # user bind events
-        if "bind_events" in result:
-            bind_events = result.pop("bind_events")
+        if "bind_events" in self.props:
+            bind_events = self.props.pop("bind_events")
             self.bind_events(bind_events)
-        # disabled
-        if "disabled" in result:
-            result["state"] = tk.DISABLED if result.pop("disabled") else tk.NORMAL
-        return result
-
-    def set_disabled(self, disabled: bool) -> None:
-        self.disabled = disabled
-        state = tk.DISABLED if disabled else tk.NORMAL
-        self.widget_update(state=state)
 
     def bind_events(self, events: dict[str, str], event_mode: EventMode="user") -> ElementType:
         """
         Bind user events
         **Example**
         ```
         # (1) bind events in the constructor
@@ -815,89 +499,30 @@
         for event_name, handle_name in events.items():
             self.bind(event_name, handle_name, event_mode=event_mode)
         return self
 
     def create(self, win: Window, parent: tk.Widget) -> Any:
         """Create a widget."""
         return None
-
-    def prepare_create(self, win: Window) -> None:
-        # convert properties
-        if (win.font is not None) and (self.font is None) and self.has_font_prop:
-            self.props["font"] = self.font = win.font
-        self.props = self.convert_props(self.props)
-        # check use ttk
-        if not self.use_ttk:
-            return
-        # set style
-        style = get_ttk_style()
-        style_name = self.style_name
-        # set font style
-        font = None
-        if "font" in self.props:
-            font = self.props.pop("font")
-            style.configure(style_name, font=font)
-        # fg / bg
-        if "fg" in self.props:
-            fg = self.props.pop("fg")
-            style.configure(style_name, foreground=fg)
-            if self.ttk_style_name == "TLabelframe":
-                style.configure(f"{style_name}.Label", foreground=fg)
-        if "bg" in self.props:
-            bg = self.props.pop("bg")
-            style.configure(style_name, background=bg)
-            if self.ttk_style_name == "TLabelframe":
-                style.configure(f"{style_name}.Label", background=bg)
-        # set readonlybackground
-        if "readonlybackground" in self.props:
-            readonlybackground = self.props.pop("readonlybackground")
-            style.map(style_name, background=[("readonly", readonlybackground)])
-        # check element type
-        # Button ?
-        if self.ttk_style_name == "TButton" or self.ttk_style_name == "TLabel":
-            if "justify" in self.props:
-                anchor = self._justify_to_anchor(self.props.pop("justify"))
-                style.configure(style_name, anchor=anchor)
-            if "height" in self.props:
-                height = self.props.pop("height")
-                self.pady = (height-1)//2
-    
-    def _generate_style_name(self, style_key: str|None) -> str:
-        """generate style name"""
-        if style_key is None or style_key == "":
-            style_key = generate_element_style_key(self.element_type)
-        if "." in self.ttk_style_name:
-            return f"{self.ttk_style_name}"
-        else:
-            return f"{style_key}.{self.ttk_style_name}"
-
-
-    def post_create(self, win: Window, parent: tk.Widget) -> None:
-        """Post create widget."""
-        pass
-
+    
     def get(self) -> Any:
         """Get the value of the widget."""
         return "-"
     
     def update(self, *args, **kw) -> None:
-        """update widget configuration."""
-        pass
-    
-    def widget_update(self, **kw) -> None:
-        # update element's props
+        """Update the widget props (only change `props`)"""
         for k, v in kw.items():
             self.props[k] = v
-        kw = self.convert_props(kw)
+    
+    def widget_update(self, **kw) -> None:
         try:
-            if (self.widget is not None)and(len(kw) > 0):
+            if self.widget is not None:
                 self.widget.configure(**kw)
         except Exception as e:
-            print(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}", file=sys.stderr)
-            # raise TkEasyError(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}")
+            raise TkEasyError(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}")
 
     def get_prev_widget(self, target_key: str|None=None) -> tk.Widget:
         """Get the previous widget."""
         # check target_key
         target: tk.Widget = None
         if target_key:
             if target_key in self.window.key_elements:
@@ -926,59 +551,26 @@
         if self.widget is not None:
             if name in self.widget:
                 return self.widget[name]
         return None
 
 class Frame(Element):
     """Frame element."""
-    def __init__(
-                self,
-                title: str,
-                layout: list[list[Element]],
-                key: str = "",
-                size: tuple[int, int]|None=None,
-                relief: ReliefType="groove",
-                # text props
-                font: FontType|None=None, # font
-                color: str|None=None,
-                text_color: str|None=None,
-                background_color: str|None=None,
-                label_outside: bool=False,
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                metadata: dict[str, Any]|None=None,
-                use_ttk: bool=False,
-                **kw) -> None:
-        style_name = "TLabelframe" if use_ttk else ""
-        super().__init__("Frame", style_name, key, False, metadata, **kw)
+    def __init__(self, title: str, layout: list[list[Element]], key: str = "", background_color: str|None=None, size: tuple[int, int]|None=None, **kw) -> None:
+        super().__init__("Frame", key, **kw)
         self.has_children = True
         self.layout = layout
-        self.label_outside = label_outside
         self.props["text"] = title
-        self.props["relief"] = relief
-        self._set_text_props(color=color, text_color=text_color, background_color=background_color, font=font)
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
-        self.use_ttk: bool = use_ttk
-
         if size is not None:
             self.props["size"] = size
+        if background_color:
+            self.props["background"] = background_color
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        """Create a Frame widget."""
-        if self.use_ttk:
-            get_ttk_style().configure(self.style_name, labeloutside=self.label_outside)
-            self.widget = ttk.LabelFrame(
-                parent,
-                style=self.style_name,
-                **self.props)
-        else:
-            self.widget = tk.LabelFrame(parent, **self.props)
+        self.widget = tk.LabelFrame(parent, name=self.key, **self.props)
         return self.widget
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
@@ -989,206 +581,59 @@
         """Get unknown attribute."""
         if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
 
 class Column(Element):
     """Frame element."""
-    def __init__(
-                self,
-                layout: list[list[Element]],
-                key: str = "",
-                background_color: str|None=None,
-                vertical_alignment: TextVAlign="top",
-                size: tuple[int, int]|None=None,
-                # text props
-                text_align: TextAlign|None="left", # text align
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                metadata: dict[str, Any]|None=None,
-                **kw) -> None:
-        super().__init__("Column", "TFrame", key, False, metadata, **kw)
+    def __init__(self, layout: list[list[Element]], key: str = "", background_color: str|None=None,
+                 vertical_alignment: TextVAlign="top",
+                 size: tuple[int, int]|None=None, **kw) -> None:
+        super().__init__("Column", key, **kw)
         self.has_children = True
         self.layout = layout
         self.vertical_alignment = vertical_alignment
-        self.has_font_prop = False
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
         if size is not None:
             self.props["size"] = size
-        if background_color is not None:
-            self.props["background_color"] = background_color
-        if text_align is not None:
-            self.props["anchor"] = self._justify_to_anchor(text_align)
+        if background_color:
+            self.props["background"] = background_color
+        # self.props["anchor"] = {"top": "n", "bottom": "s", "center": "center"}[vertical_alignment]
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        # self.widget = tk.Frame(parent, **self.props)
-        self.widget = ttk.Frame(parent, style=self.style_name, **self.props)
+        self.widget = tk.Frame(parent, name=self.key, **self.props)
         return self.widget
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
+        super().update(*args, **kw)
         self.widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
 
 class Text(Element):
     """Text element."""
-    def __init__(
-                self,
-                text: str = "",
-                key: str|None=None,
-                enable_events: bool=False, # enabled events (click)
-                # text props
-                text_align: TextAlign|None="left", # text align
-                font: FontType|None=None, # font
-                color: str|None=None, # text color
-                text_color: str|None=None, # same as color
-                background_color: str|None=None, # background color
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                metadata: dict[str, Any]|None=None, # user metadata
-                **kw
-                ) -> None:
-        key = text if (key is None) or (key == "") else key
-        super().__init__("Text", "", key, False, metadata, **kw)
-        self.props["text"] = text
-        self._set_text_props(font=font, text_align=text_align, color=color, text_color=text_color, background_color=background_color)
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
-        self.enable_events = enable_events
-
-    def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        """Create a Text widget."""
-        if self.use_ttk:
-            self.widget = ttk.Label(parent, style=self.style_name, **self.props)
-        else:
-            self.widget = tk.Label(parent, **self.props)
-        if self.enable_events:
-            self.widget.bind("<Button-1>", lambda e: self.disptach_event({"event_type": "click", "event": e}))
-        return self.widget
-    
-    def get(self) -> Any:
-        """Get the value of the widget."""
-        return self.get_text()
-    
-    def get_text(self) -> str:
-        return self.props["text"]
-    
-    def set_text(self, text: str) -> None:
-        """Set the text of the widget."""
+    def __init__(self, text: str, key: str|None=None, text_align: TextAlign="left", font: FontType|None=None, **kw) -> None:
+        super().__init__("Text", key, **kw)
         self.props["text"] = text
-        self.widget_update(text=text)
-
-    def update(self, text: str|None=None, *args, **kw) -> None:
-        """Update the widget."""
-        if text is not None:
-            self.set_text(text)
-        self.widget_update(**kw)
-
-class Label(Text):
-    """
-    Label element (alias of Text)
-    """
-    pass
-
-class Menu(Element):
-    """
-    Menu element.
-    **Example**
-    ```
-    menu = eg.Menu([
-        ["File", ["Open", "Save", "---","Exit"]],
-        ["Edit", ["Copy", "Paste"]],
-    ])
-    ```
-    **Note**
-    - "!label" is disabled
-    - "label::-event_name-" is set event name
-    - "---" is separator
-    """
-    def __init__(
-                self,
-                items:Any|None=None,
-                menu_definition:list[list[str|list[Any]]]|None=None,
-                key: str|None=None,
-                metadata: dict[str, Any]|None=None,
-                **kw) -> None:
-        super().__init__("Menu", "", key, False, metadata, **kw)
-        self.items = menu_definition
-        if items is not None:
-            self.items = items
+        self.props["justify"] = text_align
+        self.props["font"] = font
     
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """Create a Text widget."""
-        self.widget = tk.Menu(win.window)
-        win.window.config(menu=self.widget)
-        # make items
-        self._create_menu(self.widget, self.items, 0)
+        self.widget = tk.Label(parent, **self.props)
         return self.widget
     
-    def _add_command(self, parent: tk.Menu, label: str) -> None:
-        # is separator?
-        if label == "-" or label == "---":
-            parent.add_separator()
-            return
-        # command
-        key = label
-        state = tk.NORMAL
-        if label.startswith("!"):
-            label = label[1:]
-            state = tk.DISABLED
-        if "::" in label:
-            label, key = label.split("::")
-        parent.add_command(
-            label=label, 
-            state=state,
-            command=lambda : self.disptach_event({EG_SWAP_EVENT_NAME: key}))
-
-    def _create_menu(self, parent: tk.Menu, items: list[list[str|list[Any]]], level:int = 0) -> None:
-        i = 0
-        while i < len(items):
-            item = items[i]
-            # print(f"{'-' * level}[{i}].{item}")
-            if isinstance(item, int) or isinstance(item, float):
-                item = str(item)
-            if isinstance(item, str):
-                # check next item
-                next_item = items[i+1] if i+1 < len(items) else None
-                if (next_item is None) or (not isinstance(next_item, list)):
-                    self._add_command(parent, item)
-                    # print(f"{'-' * level} add_command label={item}")
-                    i += 1
-                    continue
-                else: # if isinstance(next_item, list):
-                    # submenu
-                    submenu = tk.Menu(parent, tearoff=False)
-                    parent.add_cascade(label=item, menu=submenu)
-                    self._create_menu(submenu, next_item, level+1)
-                    i += 2
-                    continue
-            if isinstance(item, list):
-                self._create_menu(parent, item, level+1)
-                i += 1
-                continue
-            # others
-            i += 1
-
     def get(self) -> Any:
         """Get the value of the widget."""
         return self.get_text()
     
     def get_text(self) -> str:
         return self.props["text"]
     
@@ -1197,131 +642,82 @@
         self.props["text"] = text
         self.widget_update(text=text)
 
     def update(self, text: str|None=None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
+        super().update(*args, **kw)
         self.widget_update(**kw)
 
-
 class Button(Element):
     """Button element."""
-    def __init__(
-                self,
-                button_text: str="",
-                key: str|None = None,
-                disabled: bool=None,
-                size: tuple[int, int]|None=None,
-                use_ttk_buttons: bool=False,
-                tooltip: str|None=None, # (TODO) tooltip
-                # text props
-                text_align: TextAlign|None="left", # text align
-                font: FontType|None=None, # font
-                color: str|None=None, # text color
-                text_color: str|None=None, # same as color
-                background_color: str|None=None, # background color
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                metadata: dict[str, Any]|None=None,
-                **kw
-                ) -> None:
-        key = button_text if (key is None) or (key == "") else key
-        super().__init__("Button", "TButton", key, False, metadata, **kw)
-        self.use_ttk = use_ttk_buttons # can select ttk or tk button
-        self.disabled = False
-        if disabled is not None:
-            self.props["disabled"] = self.disabled = disabled
-        if size is not None:
-            self.props["size"] = size
+    def __init__(self, button_text: str="", key: str="", **kw) -> None:
+        if key == "":
+            key = button_text
+        super().__init__("Button", key, **kw)
+        self.has_value = False
         self.props["text"] = button_text
-        if tooltip is not None:
-            pass # self.props["tooltip"] = tooltip
-        self._set_text_props(font=font, text_align=text_align, color=color, text_color=text_color, background_color=background_color)
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
         self.bind_events({
+            "<Button-1>": "click",
             "<Button-3>": "right_click",
             "<Return>": "return",
         }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        if self.use_ttk:
-            self.widget = ttk.Button(
-                parent,
-                command=lambda: self.disptach_event({"event_type": "command"}),
-                **self.props)
-        else:
-            self.widget = tk.Button(
-                parent,
-                command=lambda: self.disptach_event({"event_type": "command"}),
-                **self.props)
+        self.widget = tk.Button(parent, **self.props)
         return self.widget
 
     def get(self) -> Any:
         """Get the value of the widget."""
         return self.get_text()
     
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
         self.widget_update(text=text)
     
     def get_text(self) -> str:
         return self.props["text"]
 
-    def update(self, text: str|None=None, disabled: bool|None=None, **kw) -> None:
+    def update(self, text: str|None=None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.props["text"] = text
             self.widget_update(text=text)
-        if disabled is not None:
-            self.set_disabled(disabled)
-        # other
+        super().update(**kw)
         self.widget_update(**kw)
     
     def __getattr__(self, name: str) -> Any:
         """Get unknown attribute. """
         # Get the text of the button. (compatibility with PySimpleGUI)
         if name == "GetText":
             return self.get_text
         elif name == "ButtonText":
             return self.get_text()
         return super().__getattr__(name)
 
-class Submit(Button):
-    """Subtmi element. (Alias of Button) : todo: add submit event"""
-    pass
-
 class Checkbox(Element):
-    """Checkbox element."""
-    def __init__(
-                self, text: str="",
-                default: bool=False,
-                key: str|None = None,
-                enable_events: bool=False,
-                # other
-                metadata: dict[str, Any]|None=None,
-                **kw) -> None:
-        if key is None or key == "":
+    """Button element."""
+    def __init__(self, text: str="", default: bool=False, key: str="", enable_events: bool=False, **kw) -> None:
+        if key == "":
             key = text
-        super().__init__("Checkbox", "TCheckbutton", key, True, metadata, **kw)
+        super().__init__("Button", key, **kw)
+        self.has_value = False
         self.default_value = default
         self.props["text"] = text
         if enable_events:
             self.bind_events({
+                "<Button-1>": "click",
                 "<Button-3>": "right_click"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         self.checkbox_var = tk.BooleanVar(value=self.default_value)
-        self.checkbox_var.trace_add("write", lambda *args: self.disptach_event({"event_type": "change", "event": args}))
-        self.widget = ttk.Checkbutton(parent, style=self.style_name, variable=self.checkbox_var, **self.props)
+        self.widget = tk.Checkbutton(parent, variable=self.checkbox_var, **self.props)
         return self.widget
     
     def get_value(self) -> Any:
         """Get the value of the widget."""
         return self.checkbox_var.get()
 
     def set_value(self, b: bool) -> None:
@@ -1335,375 +731,204 @@
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
         self.widget_update(text=text)
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
+        super().update(*args, **kw)
         if len(args) >= 1:
             self.set_value(args[0])
         if len(args) >= 2:
             self.set_text(args[1])
         if "text" in kw:
             self.set_text(kw.pop("text"))
         if "value" in kw:
             print("set_value", kw)
             self.set_value(kw.pop("value"))
         self.widget_update(**kw)
 
-class Radio(Element):
-    """Checkbox element."""
-    def __init__(
-                self, text: str="",
-                group_id: int|str="group",
-                default: bool=False,
-                key: str|None = None,
-                enable_events: bool=False,
-                # other
-                metadata: dict[str, Any]|None=None,
-                **kw) -> None:
-        if key is None or key == "":
-            key = text
-        super().__init__("Radio", "TRadiobutton", key, True, metadata, **kw)
-        self.default_value = default
-        self.value: int = 0
-        self.props["text"] = text
-        self.group_id: str = str(group_id)
-        if enable_events:
-            self.bind_events({
-                "<Button-3>": "right_click"
-            }, "system")
-
-    def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        # create radio group
-        if self.group_id not in win.radio_group_dict:
-            win.radio_group_dict[self.group_id] = [tk.IntVar(value=0), 1]
-            win.radio_group_dict[self.group_id][0].trace_add("write", lambda *args: self.disptach_event({"event_type": "change", "event": args}))
-        else:
-            win.radio_group_dict[self.group_id][1] += 1
-        self.value = win.radio_group_dict[self.group_id][1]
-        # create radiobutton
-        self.widget = ttk.Radiobutton(
-            parent,
-            value=self.value,
-            variable=win.radio_group_dict[self.group_id][0],
-            style=self.style_name,
-            **self.props)
-        if self.default_value:
-            self.select()
-        return self.widget
-    
-    def select(self) -> None:
-        """Select the radio button."""
-        self.window.radio_group_dict[self.group_id][0].set(self.value)
-        if self.widget is not None:
-            w: tk.Radiobutton = self.widget
-            # w.flash() # TODO: flash is not defined
-    
-    def is_selected(self) -> bool:
-        """Check if the radio button is selected."""
-        return self.window.radio_group_dict[self.group_id][0].get() == self.value
-
-    def get_value(self) -> bool:
-        """Get the value of the widget."""
-        return self.value
-
-    def get(self) -> Any:
-        """Get the value of the widget."""
-        return self.is_selected()
-
-    def set_text(self, text: str) -> None:
-        """Set the text of the widget."""
-        self.props["text"] = text
-        self.widget_update(text=text)
-
-    def update(self, text: str|None=None, **kw) -> None:
-        """Update the widget."""
-        if text is not None:
-            self.set_text(text)
-        self.widget_update(**kw)
-
 class Input(Element):
-    """
-    Text input element.
-    """
-    def __init__(
-                self,
-                text: str = "", # default text
-                key: str|None = None, # key
-                default_text: str|None = None, # same as text
-                enable_events: bool = False, # enabled events ([enter] or [change])
-                enable_key_events: bool = False,  # enabled key events
-                enable_focus_events: bool = False, # enabled focus events
-                readonly_background_color: str|None = "silver",
-                password_char: str|None = None, # if you want to use it as a password input box, set "*"
-                readonly: bool = False, # read only box
-                # text props
-                text_align: TextAlign|None = "left", # text align
-                font: FontType|None = None, # font
-                color: str|None = None, # text color
-                text_color: str|None = None, # same as color
-                background_color: str|None = None, # background color
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("Input", "TEntry", key, True, metadata, **kw)
+    """Text input element."""
+    def __init__(self, text: str="", key: str="",
+                 enable_events: bool=False,
+                 background_color: str|None=None, color: str|None=None,
+                 text_aligh: TextAlign="left",
+                 readonly: bool=False, readonly_background_color: str="silver", **kw) -> None:
+        super().__init__("Input", key, **kw)
         self.readonly: bool = readonly
-        self.enable_events: bool = enable_events
-        if default_text is not None: # compatibility with PySimpleGUI
-            text = default_text
-        self.default_text = text # default text @see Input.create
-        self._set_text_props(font=font, text_align=text_align, color=color, text_color=text_color, background_color=background_color)
-        if readonly_background_color is not None:
-            self.props["readonlybackground"] = readonly_background_color
-        if password_char is not None:
-            self.props["show"] = password_char
-        # set props
-        self._set_text_props(font=font, text_align=text_align, color=color, text_color=text_color, background_color=background_color)
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
+        self.props["text"] = text # default text @see Input.create
+        if background_color is not None:
+            self.props["background"] = background_color
+        if color is not None:
+            self.props["foreground"] = color
+        self.props["justify"] = text_aligh
+        self.props["readonlybackground"] = readonly_background_color
+        self.has_value = True
         if enable_events:
             self.bind_events({
-                "<Return>": "return",
-            }, "system")
-        if enable_key_events:
-            self.bind_events({
-                "<Key>": "key",
-            }, "system")
-        if enable_focus_events:
-            self.bind_events({
                 "<FocusIn>": "focusin",
                 "<FocusOut>": "focusout",
+                "<Return>": "return",
+                "<Key>": "key",
                 "<Button-1>": "click",
                 "<Button-3>": "right_click"
             }, "system")
     
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """create Input widget"""
         # set default text
-        self.text_var = tk.StringVar(value=self.default_text)
-        print(self.text_var.get())
+        self.props["textvariable"] = tk.StringVar()
         # create
-        self.widget = ttk.Entry(
-            parent,
-            textvariable=self.text_var,
-            style=self.style_name,
-            **self.props)
+        self.widget = tk.Entry(parent, name=self.key, **self.props)
+        # set text
+        self.widget.insert(0, self.props["text"])
         # set readonly
         if self.readonly:
             self.set_readonly(self.readonly)
-        # trace change
-        if self.enable_events:
-            self.text_var.trace_add("write",
-                lambda *args: self.disptach_event({"event_type": "change", "event": args}))
         return self.widget
 
     def get(self) -> Any:
         """Get the value of the widget."""
-        return self.get_text()
-    
-    def set_text(self, text: str) -> None:
-        if self.widget is None:
-            return
-        # change text
-        self.widget.config(textvariable=self.text_var)
-        self.text_var.set(text)
-        #  OR
-        #   self.delete(0, "end")
-        #   self.insert(0, text)
-
-    def get_text(self) -> str:
-        return self.text_var.get()
+        return self.props["textvariable"].get()
 
     def set_readonly(self, readonly: bool) -> None:
         """set readonly"""
         self.readonly = readonly
         state = "readonly" if self.readonly else "normal"
         self.widget_update(state=state)
 
-    def update(self, text: str|None=None, readonly: bool|None=None, **kw) -> None:
+    def update(self, *args, **kw) -> None:
         """Update the widget."""
+        super().update(*args, **kw)
         if self.widget is None:
             return
+        text = self.props["text"]
+        if len(args) >= 1:
+            text = args[0]
         # check readonly
-        if readonly is not None:
-            self.set_readonly(readonly)
-        # text
-        if text is not None:
-            if self.readonly:
-                self.set_readonly(False)
-                self.set_text(text)
-                self.set_readonly(True)
-            else:
-                self.set_text(text)
+        if "readonly" in kw:
+            self.readonly = True if kw.pop("readonly") else False
+            self.set_readonly(self.readonly)
+        # update text
+        # 1. update widget state
+        readonly = self.readonly
+        if readonly:
+            self.set_readonly(False)
+        # 2. update text property
+        self.props["text"] = text
+        self.props["textvariable"].set(text)
+        # 3. update widget text
+        self.widget.delete(0, "end")
+        self.widget.insert(0, text)
+        # update readonly
+        if readonly:
+            self.set_readonly(True)
         # update others
         self.widget_update(**kw)
 
 class InputText(Input):
     """InputText element. (alias of Input)"""
     pass
 
 class Multiline(Element):
     """Multiline text input element."""
-    def __init__(
-                self,
-                text: str = "", # default text
-                default_text: str|None = None, # same as text
-                key: str|None = None, # key
-                readonly: bool = False,
-                enable_events: bool = False, 
-                enable_key_events: bool = False,
-                enable_focus_events: bool = False,
-                size: tuple[int, int] = (50, 10), # element size (unit=character)
-                # text props
-                font: FontType|None = None, # font
-                color: str|None = None, # text color
-                text_color: str|None = None, # same as color
-                background_color: str|None = None, # background color
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                readonly_background_color: str|None = None,
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("Multiline", "", key, True, metadata, **kw)
+    def __init__(self, text: str="", default_text: str|None=None, key: str="",
+                 enable_events: bool=False,
+                 color: str|None=None, background_color: str|None=None,
+                 readonly: bool=False, readonly_background_color: str='silver',
+                 size: tuple[int, int]=(50, 10),
+                 **kw) -> None:
+        super().__init__("Multiline", key, **kw)
         if default_text is not None:
             text = default_text
         self.props["text"] = text
         self.props["size"] = size
-        self._set_text_props(font=font, color=color, text_color=text_color, background_color=background_color)
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
-        if readonly_background_color is not None:
-            self.readonly_background_color = readonly_background_color
+        if color is not None:
+            self.props["foreground"] = color
+        if background_color is not None:
+            self.props["background"] = self.backgound_color = background_color
+        self.readonly_background_color = readonly_background_color
         self.has_value = True
         self.readonly = readonly
         # bind events
         if enable_events:
             self.bind_events({
-                "<Return>": "return",
-            }, "system")
-        if enable_key_events:
-            self.bind_events({
-                "<Key>": "key",
-            }, "system")
-        if enable_focus_events:
-            self.bind_events({
                 "<FocusIn>": "focusin",
                 "<FocusOut>": "focusout",
+                "<Return>": "return",
+                "<Key>": "key",
                 "<Button-1>": "click",
                 "<Button-3>": "right_click"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        # frame
-        self.widget_frame = widget_frame = ttk.Frame(parent)
         # text
         text = self.props.pop("text", "")
-        self.widget = tk.Text(widget_frame, **self.props)
+        self.widget = tk.Text(parent, name=self.key, **self.props)
         self.widget.insert("1.0", text)
         # readonly
         if self.readonly:
             self.set_readonly(self.readonly)
-        # scrollbar
-        self.scrollbar = ttk.Scrollbar(widget_frame, orient="vertical", command=self.widget.yview)
-        self.widget.configure(yscrollcommand=self.scrollbar.set)
-        # pack to frame
-        self.scrollbar.pack(side="right", fill="y")
-        self.widget.pack(side="right", fill="both", expand=True)
-        return self.widget_frame
+        return self.widget
 
     def get(self) -> Any:
         """Get the value of the widget."""
         if self.widget is None:
             return ""
-        return self.get_text()
-    
-    def get_text(self) -> str:
-        if self.widget is None:
-            return ""
         text = self.widget.get("1.0", "end -1c") # get all text
+        self.props["text"] = text
         return text
 
-    def update(self, text: str|None = None, readonly: bool|None = None, **kw) -> None:
+    def update(self, *args, **kw) -> None:
         """Update the widget."""
-        if text is not None:
+        if len(args) >= 1:
+            text = args[0] # get text
             self.set_text(text)
-        if readonly is not None:
-            self.set_readonly(readonly)
+        if "text" in kw:
+            self.set_text(kw["text"])
+        if "readonly" in kw:
+            self.readonly = True if kw.pop("readonly") else False
+            self.set_readonly(self.readonly)
         self.widget_update(**kw)
 
     def set_readonly(self, readonly: bool) -> None:
         """Set readonly"""
         self.readonly = readonly
-        state = tk.DISABLED if readonly else tk.NORMAL
-        self.widget_update(state=state)
+        state = "disabled" if readonly else "normal"
+        bgcolor = self.readonly_background_color if readonly else self.backgound_color
+        self.widget_update(state=state, background=bgcolor)
 
     def set_text(self, text: str) -> None:
         """Set text"""
         if self.widget is None:
             return
         if self.readonly:
-            self.widget_update(state=tk.NORMAL)
+            self.widget_update(state="normal")
         self.props["text"] = text
         self.widget.delete("1.0", "end") # clear text
         self.widget.insert("1.0", text) # set text
         if self.readonly:
-            self.widget_update(state=tk.DISABLED)
-    
-    def print(self, text: str, text_color: str|None=None, background_color: str|None=None, end:str="\n") -> None:
-        """Print text."""
-        text += end
-        if self.widget is None:
-            return
-        tags: list[str] = []
-        if text_color is not None:
-            tag = generate_element_style_key("--multiline-text_color")
-            self.widget.tag_config(tag, foreground=text_color)
-            tags.append(tag)
-        if background_color is not None:
-            tag = generate_element_style_key("--multiline-background_color")
-            self.widget.tag_config(tag, background=background_color)
-            tags.append(tag)
-        print(tags)
-        self.widget.insert("end", text, tags)
+            self.widget_update(state="disabled")
 
 class Textarea(Multiline):
     """Textarea element. (alias of Multiline)"""
     pass
 
-class Output(Multiline):
-    """Output element. (alias of Multiline) TODO: implement"""
-    pass
-
 class Slider(Element):
     """Slider element."""
-    def __init__(
-                self,
-                key: str|None = None,
-                range: tuple[float, float] = (1, 10),
-                orientation: OrientationType = "horizontal",
-                resolution: float|None = None,
-                default_value: float|None = None,
-                enable_events: bool = False,
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        style_name = "Horizontal.TScale" if (orientation == "h" or orientation == "horizontal") else "Vertical.TScale"
-        super().__init__("Slider", style_name, key, True, metadata, **kw)
+    def __init__(self, key: str = "", range: tuple[float, float]=(1, 10),
+                 orientation: OrientationType="horizontal",
+                 resolution: float=1, default_value: float|None=None,
+                 enable_events: bool=False,
+                 **kw) -> None:
+        super().__init__("Slider", key, **kw)
         self.has_value = True
-        self.has_font_prop = False
         self.range = range
-        self.resolution = resolution # dummy @see Slider.create
+        self.resolution = resolution
         self.default_value = default_value if default_value is not None else range[0]
         # check orientation
         self.orientation: OrientationType = orientation
         if orientation == "v":
             self.props["orient"] = "vertical"
         elif orientation == "h":
             self.props["orient"] = "horizontal"
@@ -1714,19 +939,20 @@
             self.bind_events({
                 "<ButtonRelease-1>": "release"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         self.scale_var = tk.DoubleVar()
         self.scale_var.set(self.default_value)
-        self.widget = ttk.Scale(
+        self.widget = tk.Scale(
             parent,
+            name=self.key,
             variable=self.scale_var,
             from_=self.range[0], to=self.range[1],
-            # resolution=self.resolution, # (memo) ttk.Scale does not support resolution
+            resolution=self.resolution,
             **self.props)
         return self.widget
     
     def get(self) -> Any:
         """Return Widget"""
         return self.scale_var.get()
 
@@ -1736,37 +962,28 @@
             self.scale_var.set(value)
             self.disptach_event()
         else:
             self.widget_update(**kw)
 
 class Canvas(Element):
     """Canvas element."""
-    def __init__(
-                self,
-                key: str|None = None,
-                enable_events: bool = False,
-                background_color: str|None = None,
-                size: tuple[int, int] = (300, 300),
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        super().__init__("Canvas", "", key, False, metadata, **kw)
+    def __init__(self, key: str="", enable_events: bool=False, background_color: str|None=None, size: tuple[int, int]=(300, 300), **kw) -> None:
+        super().__init__("Canvas", key, **kw)
         self.props["size"] = size
-        self.has_font_prop = False
         if background_color:
             self.props["background"] = background_color
         if enable_events:
             self.bind_events({
                 "<ButtonPress>": "mousedown",
                 "<ButtonRelease>": "mouseup",
                 "<Motion>": "mousemove"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        self.widget = tk.Canvas(parent, **self.props)
+        self.widget = tk.Canvas(parent, name=self.key, **self.props)
         return self.widget
     
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
@@ -1777,41 +994,35 @@
         """Get unknown attribute."""
         if name in ["Widget", "tk_canvas"]: # compatibility with PySimpleGUI
             return self.widget
         return super().__getattr__(name)
 
 class Graph(Element):
     """Graph element."""
-    def __init__(
-            self, key: str|None = None,
-            background_color: str|None = None,
-            size: tuple[int, int]=(300, 300),
-            canvas_size: tuple[int, int]|None = None,
-            graph_bottom_left: tuple[int, int]|None = None,
-            graph_top_right: tuple[int, int]|None = None,
-            # other
-            metadata: dict[str, Any]|None = None,
+    def __init__(self, key: str="", background_color: str|None=None,
+            size: tuple[int, int]=(300, 300), canvas_size: tuple[int, int]|None=None,
+            graph_bottom_left: tuple[int, int]|None=None, graph_top_right: tuple[int, int]|None=None,
             **kw) -> None:
-        super().__init__("Graph", "", key, False, metadata, **kw)
-        self.has_font_prop = False
+        super().__init__("Graph", key, **kw)
+        self.key = key
         # <Coordinate> graph_Declared for compatibility, but not yet implemented.
         self.graph_bottom_left = graph_bottom_left
         self.graph_top_right = graph_top_right
         # </Coordinate>
         # <size>
         self.props["size"] = size
         if canvas_size is not None:
             self.props["size"] = canvas_size
         # </size>
         if background_color:
             self.props["background"] = background_color
         self.parent_window: Window|None = None
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        self.widget: tk.Canvas = tk.Canvas(parent, **self.props)
+        self.widget: tk.Canvas = tk.Canvas(parent, name=self.key, **self.props)
         self.parent_window = win
         return self.widget
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
@@ -1879,141 +1090,57 @@
         image: tk.PhotoImage|None = get_image_tk(filename=filename, data=data)
         # important
         self.widget.image = image # type: ignore
         return self.widget.create_image(location, image=image, anchor=tk.NW)
 
 class Image(Element):
     """Image element."""
-    def __init__(
-                self,
-                source: bytes|str|None = None, # image source
-                filename = None, # filen ame
-                data: bytes = None, # image data
-                key: str|None = None,
-                background_color: str|None = None,
-                size: tuple[int, int] = (300, 300),
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        super().__init__("Image", "", key, False, metadata, **kw)
-        self.has_font_prop = False
+    def __init__(self, source: bytes|str|None=None, filename=None, data=None, key: str="", background_color: str|None=None, size: tuple[int, int]=(300, 300), **kw) -> None:
+        super().__init__("Image", key, **kw)
         self.source = source
         self.filename = filename
         self.data = data
-        self.size = self.props["size"] = size
+        if size is not None:
+            self.props["size"] = size
         if background_color is not None:
             self.props["background"] = background_color
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """Create a Image widget."""
-        self.widget = tk.Canvas(parent, **self.props)
-        try:
-            self.set_image(self.source, self.filename, self.data)
-        except Exception:
-            pass
+        photo = get_image_tk(self.source, self.filename, self.data)
+        self.widget = tk.Label(parent, image=photo, name=self.key, **self.props)
+        self.widget.image = photo # type: ignore
         return self.widget
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
-    def erase(self) -> None:
-        """Erase image"""
-        self.widget.delete("all")
-
-    def set_image(self, source: bytes|str=None, filename: str|None=None, data: bytes|None=None) -> None:
-        if self.widget is None:
-            return
-        # set 
-        self.filename = filename
-        self.data = data
-        # erase
-        self.erase()
-        # load
-        photo = get_image_tk(source, filename, data, self.size)
-        if photo is not None:
-            self.widget.create_image(0, 0, image=photo, anchor="nw")
-            self.widget.photo = photo # type ignore
-
-    def update(self, source: bytes|str=None, filename: str|None=None, data: bytes|None=None, size: tuple[int,int]|None=None, **kw) -> None:
+    def update(self, source: bytes|str=None, filename: str|None=None, data: bytes|None=None, **kw) -> None:
         """Update the widget."""
-        if size is not None:
-            self.size = size
-            self.widget.configure(width=size[0], height=size[1])
-        if (source is not None) or (filename is not None) or (data is not None):
-            self.set_image(source, filename, data)
+        image = get_image_tk(source, filename, data)
+        self.widget.configure(image=image)
+        self.widget.image = image # type: ignore
         self.widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
-        if name in ["Widget", "tk_canvas", "tktext_label"]:
+        if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
 
-class VSeparator(Element):
-    """VSeparator element."""
-    def __init__(
-                self,
-                key: str|None = None,
-                background_color: str|None = None,
-                pad: PadType = 5,
-                size: tuple[int, int]=(5, 100),
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        super().__init__("VSeparator", "TSeparator", key, False, metadata, **kw)
-        size = (pad, size[1])
-        self.size = self.props["size"] = size
-        self.props["padx"] = pad
-        if background_color is not None:
-            self.props["background"] = background_color
-        self.props["expand_y"] = True
-    
-    def create(self, win: Window, parent: tk.Widget) -> Any:
-        self.widget = ttk.Separator(parent, orient="vertical")
-        return self.widget
-
-class HSeparator(Element):
-    """HSeparator element."""
-    def __init__(
-                self,
-                key: str|None = None,
-                background_color: str|None = None,
-                pad: PadType = 5,
-                size: tuple[int, int] = (100, 5),
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        super().__init__("HSeparator", "TSeparator", key, False, metadata, **kw)
-        size = (size[1], pad)
-        self.size = self.props["size"] = size
-        self.props["pady"] = pad
-        if background_color is not None:
-            self.props["background"] = background_color
-        self.props["expand_x"] = True
-    
-    def create(self, win: Window, parent: tk.Widget) -> Any:
-        self.widget = ttk.Separator(parent, orient="horizontal")
-        return self.widget
-
 
 class Listbox(Element):
     """Listbox element."""
-    def __init__(
-                self,
-                values: list[str] = [],
-                key: str|None = None,
-                enable_events: bool = False,
-                select_mode: ListboxSelectMode = LISTBOX_SELECT_MODE_BROWSE,
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        super().__init__("Listbox", "", key, True, metadata, **kw)
+    def __init__(self, values: list[str]=[], key: str="", enable_events: bool=False, select_mode: ListboxSelectMode="browse", **kw) -> None:
+        super().__init__("Listbox", key, **kw)
         self.values = values
+        self.has_value = True
         self.select_mode = select_mode
+        self.key = key
         # event
         if enable_events:
             self.bind_events({
                 "<<ListboxSelect>>": "select"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
@@ -2056,38 +1183,30 @@
             self.set_values(values)
         if "values" in kw:
             self.set_values(kw.pop("values"))
         self.widget_update(**kw)
 
 class Combo(Element):
     """Combo element."""
-    def __init__(
-                self,
-                values: list[str]=[],
-                default_value: str="",
-                key: str|None = None,
-                enable_events: bool = False,
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
-        super().__init__("Combo", "TCombobox", key, True, metadata, **kw)
+    def __init__(self, values: list[str]=[], default_value: str="", key: str="", enable_events: bool=False, **kw) -> None:
+        super().__init__("Combo", key, **kw)
         self.values = values
         self.value: tk.StringVar|None = None
         self.default_value = default_value
+        self.has_value = True
         # event
         if enable_events:
             self.bind_events({
                 "<<ComboboxSelected>>": "select"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """[Combo.create] create Listbox widget"""
-        self.value = tk.StringVar()
+        self.value = tk.StringVar(value=self.default_value)
         self.widget = ttk.Combobox(parent, values=self.values, textvariable=self.value, **self.props)
-        self.set_value(self.default_value)
         return self.widget
 
     def set_values(self, values: list[str]) -> None:
         """Set values to list"""
         self.values = values
         if self.widget is not None:
             self.widget_update(values=self.values)
@@ -2112,109 +1231,52 @@
             self.set_values(kw.pop("values"))
         if "value" in kw:
             self.set_value(kw.pop("value"))
         self.widget_update(**kw)
 
 class Table(Element):
     """Table element."""
-    def __init__(
-                self,
-                values: list[list[str]] = [],
-                headings: list[str] = [],
-                key: str|None = None,
-                justification: TextAlign = "center",
-                auto_size_columns: bool = True,
-                max_col_width: int = 0,
-                col_widths: list[int]|None = None,
-                enable_events: bool = False,
-                event_returns_values: bool|None = None, # Returns the table value if set to True, otherwise returns the index.
-                select_mode: str="browse",
-                # text props
-                text_align: TextAlign|None = "left", # text align
-                font: FontType|None = None, # font
-                color: str|None = None, # text color
-                text_color: str|None = None, # same as color
-                background_color: str|None = None, # background color
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: PadType|None = None,
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw) -> None:
+    def __init__(self, values: list[list[str]]=[], headings: list[str]=[], key: str="", justification: TextAlign="center",
+                 auto_size_columns: bool = True, max_col_width: int = 0, font: tuple[str, int]|None=None,
+                 enable_events: bool=False, select_mode: str="browse", **kw) -> None:
         """Create a table."""
-        # super().__init__("Table", "Treeview", key, metadata, **kw)
-        super().__init__("Table", "", key, True, metadata, **kw)
+        super().__init__("Table", key, **kw)
         self.values = values
         self.headings = headings
+        self.has_value = True
         self.enable_events = enable_events
         self.select_mode = select_mode
+        self.justification: str = {"": "", "right": "e", "center": "center", "left": "w"}[justification]
         self.auto_size_columns = auto_size_columns
-        self.max_col_width = max_col_width
-        self.col_widths = col_widths
-        self.has_font_prop = False # has, but not widget root
-        # event_returns_values ?
-        self.event_returns_values: bool = not _compatibility
-        if event_returns_values is not None:
-            self.event_returns_values = event_returns_values 
-        # justification
-        if justification is not None:
-            self.justification: str = self._justify_to_anchor(justification)
-        if text_align is not None:
-            self.justification: str = self._justify_to_anchor(justification)
-        # set props
-        self._set_text_props(font=font, color=color, text_color=text_color, background_color=background_color)
-        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
-        # check col_widths
-        if self.col_widths is None:
-            self.col_widths = [len(s) for s in self.headings]
-            for row in self.values:
-                for i, cell in enumerate(row):
-                    v = max(self.col_widths[i], len(str(cell))+1)
-                    if (self.max_col_width is not None) and (self.max_col_width > 0):
-                        v = min(v, self.max_col_width)
-                    self.col_widths[i] = v
+        self.max_col_width = max_col_width # todo
+        self.font = font # todo
     
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """Create a Table widget."""
         self.window: Window = win
         # create treeview
-        # - FRAME
         self.frame = ttk.Frame(parent, padding=1, relief="ridge", borderwidth=1)
         columns = tuple(i+1 for i, _ in enumerate(self.headings))
-        # - TREE (font)
-        font = None
-        if "font" in self.props:
-            font = self.props.pop("font")
-        # - TREE
         tree = self.widget = ttk.Treeview(
             self.frame,
             columns=columns,
             show="headings",
             **self.props)
-        self.props["font"] = font
-        # - SCROLLBAR
+        # scroll bar
         scrollbar = ttk.Scrollbar(self.frame, orient=tk.VERTICAL, command=tree.yview)
-        tree.configure(yscrollcommand=scrollbar.set)
-        # - pack to frame
+        scrollbar.pack(expand=True, fill=tk.Y, side=tk.RIGHT)
         self.widget.pack(expand=True, fill="both", side=tk.LEFT)
-        scrollbar.pack(fill=tk.Y, side=tk.LEFT)
+        tree.configure(yscrollcommand=scrollbar.set)
         # setting for column
         streatch = tk.YES if self.auto_size_columns else tk.NO
         for i, h in enumerate(self.headings):
             self.widget.heading(i+1, text=h, anchor="center")
             kw: dict[str, Any] = {"stretch": streatch}
             if self.justification != "":
                 kw["anchor"] = self.justification
-            if self.col_widths is not None:
-                # get font size
-                font_w = 12
-                if (self.font is not None) and (len(self.font) >= 2):
-                    font_w = self.font[1]
-                kw["width"] = self.col_widths[i % len(self.col_widths)] * font_w
             self.widget.column(i+1, **kw)
         # add data
         self.set_values(self.values, self.headings)
         if self.enable_events:
             self.widget.bind("<<TreeviewSelect>>", lambda e: self._table_events(e))
         return self.frame
     
@@ -2226,28 +1288,23 @@
         self.headings = headings
         # clear
         self.widget.delete(*self.widget.get_children())
         # update heading
         for i, h in enumerate(self.headings):
             self.widget.heading(i+1, text=h, anchor="center")
         # add data
-        for row_no, row in enumerate(self.values):
-            self.widget.insert(parent="", iid=row_no, index="end", values=row)
+        for row in self.values:
+            self.widget.insert(parent="", index="end", values=row)
     
     def get(self) -> Any:
         """Get the value of the widget."""
         if self.widget is None:
             return []
-        record_ids = self.widget.focus()
-        if self.event_returns_values:
-            record_values = self.widget.item(record_ids, "values")
-        else:
-            if isinstance(record_ids, str):
-                record_ids = [record_ids]
-            record_values = list(map(lambda id_s: int(id_s), record_ids))
+        record_id = self.widget.focus()
+        record_values = self.widget.item(record_id, "values")
         return record_values
 
     def _table_events(self, _event: Any) -> None:
         """Handle events."""
         self.window._event_handler(self.key, {})
 
     def update(self, *args, **kw) -> None:
@@ -2268,28 +1325,20 @@
         self.widget_update(**kw)
 
 #------------------------------------------------------------------------------
 # Browse elements
 
 class FileBrowse(Element):
     """FileBrowse element."""
-    def __init__(
-                self, button_text: str="...",
-                key: str|None = None,
-                title: str = "",
-                target_key: str|None = None,
-                file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
-                multiple_files: bool = False,
-                initial_folder: str|None = None,
-                save_as: bool = False,
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("FileBrowse", "", key, False, metadata, **kw)
+    def __init__(self, button_text: str="...", key: str="", target_key: str|None=None,
+            title: str="", file_types: tuple[tuple[str, str]]=(("All Files", "*.*"),),
+            multiple_files: bool=False, initial_folder: str|None=None,
+            save_as: bool=False, **kw) -> None:
+        super().__init__("FileBrowse", key, **kw)
+        self.has_value = False
         self.target_key = target_key
         self.title = title
         self.file_types = file_types
         self.save_as = save_as
         self.multiple_files = multiple_files
         self.initial_folder = initial_folder
         self.props["text"] = button_text
@@ -2307,18 +1356,15 @@
         return self.widget
     
     def _get_initial_directory(self) -> str:
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # get initial directory
         init_dir = self.initial_folder
         if target is not None:
-            try:
-                target_text = str(target.get())
-            except Exception:
-                target_text = ""
+            target_text = target.get()
             if target_text != "":
                 init_dir = os.path.dirname(target_text)
         return init_dir
 
     def show_dialog(self, *args) -> str|None:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
@@ -2339,82 +1385,57 @@
         return result
     
     def set_text(self, text: str) -> None:
         """Set the text of the button."""
         self.props["text"] = text
         self.widget_update(text=text)
 
-    def update(self, text: str|None=None, **kw) -> None:
+    def update(self, text: str|None=None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
-        self.widget_update(**kw)
+        super().update(*args, **kw)
 
 class FilesBrowse(FileBrowse):
     """FilesBrowse element."""
-    def __init__(
-                self,
-                button_text: str = "...",
-                key: str|None = None,
-                target_key: str|None = None,
-                title: str="",
-                file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("FilesBrowse", "", key, False, metadata, **kw)
+    def __init__(self, button_text: str="...", key: str="", target_key: str|None=None,
+            title: str="", file_types: tuple[tuple[str, str]]=(("All Files", "*.*"),), **kw) -> None:
+        super().__init__("FilesBrowse", key, **kw)
         self.target_key = target_key
         self.title = title
         self.file_types = file_types
         self.props["text"] = button_text
         # force set params
         self.multiple_files = True
         self.save_as = False
 
 class FileSaveAsBrowse(FileBrowse):
     """FileSaveAsBrowse element."""
-    def __init__(
-                self,
-                button_text: str="...",
-                key: str|None = None,
-                target_key: str|None = None,
-                title: str = "",
-                file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("FileSaveAsBrowse", "", key, False, metadata, **kw)
+    def __init__(self, button_text: str="...", key: str="", target_key: str|None=None,
+            title: str="", file_types: tuple[tuple[str, str]]=(("All Files", "*.*"),), **kw) -> None:
+        super().__init__("FileSaveAsBrowse", key, **kw)
         self.target_key = target_key
         self.title = title
         self.file_types = file_types
         self.props["text"] = button_text
         # force set params
         self.multiple_files = False
         self.save_as = True
 
 class FileSaveAs(FileBrowse):
     """FileSaveAs element. (alias of FileSaveAsBrowse)"""
     pass
 
 class FolderBrowse(FileBrowse):
     """FolderBrowse element."""
-    def __init__(
-                self,
-                button_text: str="...",
-                key: str|None = None,
-                target_key: str|None = None,
-                default_path: str|None = None,
-                title: str = "",
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("FolderBrowse", "", key, False, metadata, **kw)
+    def __init__(self, button_text: str="...", key: str="", target_key: str|None=None,
+            default_path: str|None=None,
+            title: str="", **kw) -> None:
+        super().__init__("FolderBrowse", key, **kw)
+        self.has_value = False
         self.target_key = target_key
         self.title = title
         self.default_path = default_path
         self.props["text"] = button_text
     
     def show_dialog(self, *args) -> str|None:
         """Show file dialog"""
@@ -2426,26 +1447,19 @@
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
         return result
 
 class ColorBrowse(FileBrowse):
     """FolderBrowse element."""
-    def __init__(
-                self,
-                button_text: str="...",
-                key: str|None = None,
-                target_key: str|None = None,
-                default_color: str|None = None,
-                title: str="",
-                # other
-                metadata: dict[str, Any]|None = None,
-                **kw
-                ) -> None:
-        super().__init__("FolderBrowse", "", key, False, metadata, **kw)
+    def __init__(self, button_text: str="...", key: str="", target_key: str|None=None,
+            default_color: str|None=None,
+            title: str="", **kw) -> None:
+        super().__init__("FolderBrowse", key, **kw)
+        self.has_value = False
         self.target_key = target_key
         self.title = title
         self.default_color = default_color
         self.props["text"] = button_text
     
     def show_dialog(self, *args) -> str|None:
         """Show file dialog"""
@@ -2462,86 +1476,61 @@
 
 #------------------------------------------------------------------------------
 # Utility functions
 #------------------------------------------------------------------------------
 
 # global variables
 # auto generate element key id
-_element_style_key_ids: dict[str, int] = {}
+_element_key_ids: dict[str, int] = {}
 _element_key_names: dict[str, bool] = {}
-def generate_element_style_key(element_type: str) -> int:
+def generate_element_key(element_type: str) -> int:
     """Get a unique id for an element."""
     element_type = element_type.lower()
-    if element_type not in _element_style_key_ids:
-        _element_style_key_ids[element_type] = 0
+    if element_type not in _element_key_ids:
+        _element_key_ids[element_type] = 0
     key: str = ""
     while True:
-        _element_style_key_ids[element_type] += 1
-        element_id = _element_style_key_ids[element_type]
+        _element_key_ids[element_type] += 1
+        element_id = _element_key_ids[element_type]
         key = f"-{element_type}{element_id}-"
         if key not in _element_key_names:
             _element_key_names[key] = True
             break
     return key
 
-def register_element_key(key: str) -> bool:
+def register_element_key(key: str) -> None:
     """Register element key."""
-    if key in _element_key_names:
-        return False
     _element_key_names[key] = True
-    return True
-
-_elements_with_value: int = 0
-def generate_element_id() -> int:
-    """Generate a unique id for a value element."""
-    global _elements_with_value
-    element_id = _elements_with_value
-    _elements_with_value += 1
-    return element_id
 
 def rgb(r: int, g: int, b: int) -> str:
     r = r & 0xFF
     g = g & 0xFF
     b = b & 0xFF
     return f"#{r:02x}{g:02x}{b:02x}"
 
-def image_resize(img: PILImage, size: tuple[int, int]) -> PILImage:
-    if size[0] < size[1]:
-        r = size[0] / img.size[0]
-    else:
-        r = size[1] / img.size[1]
-    w, h = size[0], int(img.size[1] * r)
-    return img.resize(size=(w, h))
-
-def get_image_tk(source: bytes|str|None=None, filename: str|None = None, data: bytes|None = None, size: tuple[int, int]|None = None) -> tk.PhotoImage|None:
+def get_image_tk(source: bytes|str|None=None, filename: str|None = None, data: bytes|None = None) -> tk.PhotoImage|None:
     """Get Image for tk"""
     # if source is bytes, set data
     if source is not None:
         if isinstance(source, str): # is filename
             filename = source
         else: # is data
             data = source
     # load from file?
     if filename is not None:
         try:
-            img: PILImage = PILImage.open(filename)
-            if size is not None:
-                img = image_resize(img, size)
-            return ImageTk.PhotoImage(image=img)
+            return ImageTk.PhotoImage(file=filename)
         except Exception as e:
             raise TkEasyError(f"TkEasyGUI.Image.set_image.Error: filename='{filename}', {e}")
     # load from data
     if data is not None:
         try:
             # check if data is PILImage
             if isinstance(data, PILImage.Image):
-                img: PILImage = data
-                if size is not None:
-                    img = image_resize(img, size)
-                return ImageTk.PhotoImage(image=img)
+                return ImageTk.PhotoImage(image=data)
             return ImageTk.PhotoImage(data=data)
         except Exception as e:
             print("[TkEasyGUI] get_image_tk.Error:", e, stderr=True)
             return data
     return None
 
 def imagedata_to_bytes(image_data: PILImage) -> bytes:
```

### Comparing `TkEasyGUI-0.2.38/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.4/tkeasygui.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: TkEasyGUI
-Version: 0.2.38
-Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
+Name: tkeasygui
+Version: 0.2.4
+Summary: TkEasyGUI is Easy and Simple GUI Library
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,51 +44,45 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 
 # TkEasyGUI
 
-`TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
+**TkEasyGUI** is a Python library that allows for the easy and simple creation of GUI applications.
 In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
 Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
 
 This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
-- [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
-
-## Platform
-
-- Windows / macOS / Linux (tkinter required)
+- [👉日本語のREADME](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md)
 
 ## Install
 
 Install from pypi
 
 
 ```sh
-python -m pip install TkEasyGUI
+python -m pip install tkeasygui
 ```
 
 Install from GitHub Repository
 
 
 ```sh
 python -m pip install git+https://github.com/kujirahand/tkeasygui-python
 ```
 
-- (memo) Updating from older versions (less than 0.2.24) will fail. ([See the solution](https://github.com/kujirahand/tkeasygui-python/blob/main/docs/installation_trouble.md))
-
 ## How to use
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
-import TkEasyGUI as eg
+import tkeasygui as eg
 
 # Create window
 layout = [
     [eg.Text("Hello, World!")],
     [eg.Button("OK")]
 ]
 window = eg.Window("Hello", layout=layout)
@@ -114,17 +108,20 @@
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
 ## About the relationship with PySimpleGUI
 
-- When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
-- The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
-- This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
-- We are not considering full compatibility with PySimpleGUI.
+Fundamentally, it is compatible with PySimpleGUI. Programs can be written using the same event model. 
+It should be noted that while it was developed with reference to PySimpleGUI, it has been reimplemented from scratch.
+Many unique features have been expanded.
+The basic Elements have been given the same names. However, the names of some properties are different.
+
+We are not considering full compatibility with PySimpleGUI.
+
 
 ## Link
 
 - [pypi.org > TkEasyGUI](https://pypi.org/project/tkeasygui/)
 - [GitHub > TkEasyGUI](https://github.com/kujirahand/tkeasygui-python/)
```

### Comparing `TkEasyGUI-0.2.38/pyproject.toml` & `tkeasygui-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "TkEasyGUI"
-version = "0.2.38"
+name = "tkeasygui"
+version = "0.2.4"
 dependencies = [
   "Pillow",
 ]
 requires-python = ">=3.8"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
 ]
 maintainers = [
  { name="kujirahand", email="web@kujirahand.com" },
 ]
-description = "TkEasyGUI is simple GUI Library for Python3 with Tkinter"
+description = "TkEasyGUI is Easy and Simple GUI Library"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["GUI", "Tkinter", "PySimpleGUI"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

