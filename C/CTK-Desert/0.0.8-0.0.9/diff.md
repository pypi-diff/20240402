# Comparing `tmp/CTK_Desert-0.0.8.tar.gz` & `tmp/CTK_Desert-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTK_Desert-0.0.8.tar", last modified: Tue Mar 19 21:23:06 2024, max compression
+gzip compressed data, was "CTK_Desert-0.0.9.tar", last modified: Wed Mar 20 20:28:01 2024, max compression
```

## Comparing `CTK_Desert-0.0.8.tar` & `CTK_Desert-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 21:23:06.592802 CTK_Desert-0.0.8/
--rw-rw-rw-   0        0        0    35821 2024-03-19 14:55:39.000000 CTK_Desert-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    42109 2024-03-19 21:23:06.591806 CTK_Desert-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      135 2024-03-19 14:50:59.000000 CTK_Desert-0.0.8/README.md
--rw-rw-rw-   0        0        0     1109 2024-03-19 21:22:58.000000 CTK_Desert-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 21:23:06.592802 CTK_Desert-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-19 21:23:06.559913 CTK_Desert-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-19 21:23:06.574862 CTK_Desert-0.0.8/src/CTK_Desert/
--rw-rw-rw-   0        0        0     4489 2024-03-19 14:16:39.000000 CTK_Desert-0.0.8/src/CTK_Desert/AddPage.py
--rw-rw-rw-   0        0        0     1054 2024-03-19 14:21:19.000000 CTK_Desert-0.0.8/src/CTK_Desert/Page_EX_Code.py
--rw-rw-rw-   0        0        0     3577 2024-02-11 15:30:28.000000 CTK_Desert-0.0.8/src/CTK_Desert/Page_base_model.py
--rw-rw-rw-   0        0        0     4342 2024-03-19 14:40:19.000000 CTK_Desert-0.0.8/src/CTK_Desert/Settings.py
--rw-rw-rw-   0        0        0    13818 2024-03-16 19:16:59.000000 CTK_Desert-0.0.8/src/CTK_Desert/Tab_Page_Frame.py
--rw-rw-rw-   0        0        0     1004 2024-03-16 20:20:22.000000 CTK_Desert-0.0.8/src/CTK_Desert/Theme.py
--rw-rw-rw-   0        0        0     8389 2024-03-19 20:24:09.000000 CTK_Desert-0.0.8/src/CTK_Desert/Widgits.py
--rw-rw-rw-   0        0        0     2056 2024-03-19 21:22:46.000000 CTK_Desert-0.0.8/src/CTK_Desert/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 21:23:06.584830 CTK_Desert-0.0.8/src/CTK_Desert/images/
-drwxrwxrwx   0        0        0        0 2024-03-19 21:23:06.589813 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/
--rw-rw-rw-   0        0        0     1582 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_d.png
--rw-rw-rw-   0        0        0     1706 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_d_s.png
--rw-rw-rw-   0        0        0     1563 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_l.png
--rw-rw-rw-   0        0        0     1689 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_l_s.png
--rw-rw-rw-   0        0        0    28973 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_d.png
--rw-rw-rw-   0        0        0    29351 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_d_s.png
--rw-rw-rw-   0        0        0    26984 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_l.png
--rw-rw-rw-   0        0        0    27191 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_l_s.png
--rw-rw-rw-   0        0        0    14942 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/images/empty.ico
--rw-rw-rw-   0        0        0       27 2024-03-18 17:59:29.000000 CTK_Desert-0.0.8/src/CTK_Desert/preferences.json
--rw-rw-rw-   0        0        0     1669 2023-10-06 06:31:48.000000 CTK_Desert-0.0.8/src/CTK_Desert/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-19 21:23:06.590809 CTK_Desert-0.0.8/src/CTK_Desert.egg-info/
--rw-rw-rw-   0        0        0    42109 2024-03-19 21:23:06.000000 CTK_Desert-0.0.8/src/CTK_Desert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2024-03-19 21:23:06.000000 CTK_Desert-0.0.8/src/CTK_Desert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 21:23:06.000000 CTK_Desert-0.0.8/src/CTK_Desert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-03-19 21:23:06.000000 CTK_Desert-0.0.8/src/CTK_Desert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 21:23:06.000000 CTK_Desert-0.0.8/src/CTK_Desert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-20 20:28:01.018695 CTK_Desert-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2024-03-19 14:55:39.000000 CTK_Desert-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    42109 2024-03-20 20:28:01.017695 CTK_Desert-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2024-03-19 14:50:59.000000 CTK_Desert-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1109 2024-03-20 20:27:28.000000 CTK_Desert-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-20 20:28:01.018695 CTK_Desert-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-20 20:28:00.974696 CTK_Desert-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-20 20:28:00.990695 CTK_Desert-0.0.9/src/CTK_Desert/
+-rw-rw-rw-   0        0        0     4489 2024-03-19 14:16:39.000000 CTK_Desert-0.0.9/src/CTK_Desert/AddPage.py
+-rw-rw-rw-   0        0        0     1054 2024-03-19 14:21:19.000000 CTK_Desert-0.0.9/src/CTK_Desert/Page_EX_Code.py
+-rw-rw-rw-   0        0        0     3577 2024-02-11 15:30:28.000000 CTK_Desert-0.0.9/src/CTK_Desert/Page_base_model.py
+-rw-rw-rw-   0        0        0     4342 2024-03-19 14:40:19.000000 CTK_Desert-0.0.9/src/CTK_Desert/Settings.py
+-rw-rw-rw-   0        0        0    13754 2024-03-20 20:06:59.000000 CTK_Desert-0.0.9/src/CTK_Desert/Tab_Page_Frame.py
+-rw-rw-rw-   0        0        0     1004 2024-03-16 20:20:22.000000 CTK_Desert-0.0.9/src/CTK_Desert/Theme.py
+-rw-rw-rw-   0        0        0     8389 2024-03-19 20:24:09.000000 CTK_Desert-0.0.9/src/CTK_Desert/Widgits.py
+-rw-rw-rw-   0        0        0     2056 2024-03-19 21:22:46.000000 CTK_Desert-0.0.9/src/CTK_Desert/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-20 20:28:01.009699 CTK_Desert-0.0.9/src/CTK_Desert/images/
+drwxrwxrwx   0        0        0        0 2024-03-20 20:28:01.015700 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/
+-rw-rw-rw-   0        0        0     1582 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_d.png
+-rw-rw-rw-   0        0        0     1706 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_d_s.png
+-rw-rw-rw-   0        0        0     1563 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_l.png
+-rw-rw-rw-   0        0        0     1689 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_l_s.png
+-rw-rw-rw-   0        0        0    28973 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_d.png
+-rw-rw-rw-   0        0        0    29351 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_d_s.png
+-rw-rw-rw-   0        0        0    26984 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_l.png
+-rw-rw-rw-   0        0        0    27191 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_l_s.png
+-rw-rw-rw-   0        0        0    14942 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/images/empty.ico
+-rw-rw-rw-   0        0        0       27 2024-03-18 17:59:29.000000 CTK_Desert-0.0.9/src/CTK_Desert/preferences.json
+-rw-rw-rw-   0        0        0     1669 2023-10-06 06:31:48.000000 CTK_Desert-0.0.9/src/CTK_Desert/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-20 20:28:01.016697 CTK_Desert-0.0.9/src/CTK_Desert.egg-info/
+-rw-rw-rw-   0        0        0    42109 2024-03-20 20:28:00.000000 CTK_Desert-0.0.9/src/CTK_Desert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      893 2024-03-20 20:28:00.000000 CTK_Desert-0.0.9/src/CTK_Desert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-20 20:28:00.000000 CTK_Desert-0.0.9/src/CTK_Desert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-03-20 20:28:00.000000 CTK_Desert-0.0.9/src/CTK_Desert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-20 20:28:00.000000 CTK_Desert-0.0.9/src/CTK_Desert.egg-info/top_level.txt
```

### Comparing `CTK_Desert-0.0.8/LICENSE` & `CTK_Desert-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/PKG-INFO` & `CTK_Desert-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTK_Desert
-Version: 0.0.8
+Version: 0.0.9
 Summary: A GUI that uses the customtkinter library to create GUIs based on your need, so that you focus on the functionality of your application and not the design.
 Author-email: Morad Sayed <Morad.S.Singer@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CTK_Desert-0.0.8/pyproject.toml` & `CTK_Desert-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CTK_Desert"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
   "customtkinter>=5.2.0,<6.0.0", 
   "Pillow>=9.4.0,<10.0.0", 
   "numpy>=1.23.5,<2.0.0"
 ]
 requires-python = ">=3.8,<4.0"
 license = {file = "LICENSE"} # "LICENSE" is name of the license file, which must be in root of project folder
```

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/AddPage.py` & `CTK_Desert-0.0.9/src/CTK_Desert/AddPage.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/Page_EX_Code.py` & `CTK_Desert-0.0.9/src/CTK_Desert/Page_EX_Code.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/Page_base_model.py` & `CTK_Desert-0.0.9/src/CTK_Desert/Page_base_model.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/Settings.py` & `CTK_Desert-0.0.9/src/CTK_Desert/Settings.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/Tab_Page_Frame.py` & `CTK_Desert-0.0.9/src/CTK_Desert/Tab_Page_Frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         self.menu_frame.place(relx=self.menu_relx, rely=0, anchor="nw", relheight = 1-(25/self.window_height), relwidth = self.menu_relwidth)
 
     def page(self):
         self.page_frame = ctk.CTkFrame(self, fg_color="transparent")
         for name in self.tabs:
             self.pages_dict[name[0]] = eval(name[0] + "(self.window, self, self.page_frame)")    #calls all the contents of the tabs (but not displaying them) and passing the arguments, while saving them in a dict for later use
             if self.pages_dict[name[0]].scrollable:
-                Last_widget = ctk.CTkFrame(self.pages_dict[name[0]].Scrollable_frame, fg_color=(hvr_clr_g(LIGHT_MODE["background"], "l"), hvr_clr_g(DARK_MODE["background"], "d")), bg_color=(hvr_clr_g(LIGHT_MODE["background"], "l"), hvr_clr_g(DARK_MODE["background"], "d"))) #created to locate the y position for the edge of the frame
+                Last_widget = ctk.CTkFrame(self.pages_dict[name[0]].Scrollable_frame, fg_color=self.pages_dict[name[0]].Scrollable_frame._fg_color, bg_color=self.pages_dict[name[0]].Scrollable_frame._fg_color) #created to locate the y position for the edge of the frame
                 Last_widget.pack(fill="x", pady=10) 
         self.pages_dict["Workspace"].pages_path = self.U_Pages_dir
 
 
         self.pages_dict[self.page_choise].pack(expand=True, fill="both")                        #display the default page
         directory = self.original_icons_dir if self.page_choise == "Workspace" or self.page_choise == "Settings" else self.user_icons_dir
         self.buttons[self.page_choise].configure(image=ctk.CTkImage(Image.open(f"{directory}{self.page_choise}_l_s.png"), Image.open(f"{directory}{self.page_choise}_d_s.png"), (45,45) if self.page_choise == "Workspace" else (30,30)))
```

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/Theme.py` & `CTK_Desert-0.0.9/src/CTK_Desert/Theme.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/Widgits.py` & `CTK_Desert-0.0.9/src/CTK_Desert/Widgits.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/__init__.py` & `CTK_Desert-0.0.9/src/CTK_Desert/__init__.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_d.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_d.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_d_s.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_d_s.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_l.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_l.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/settings_l_s.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/settings_l_s.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_d.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_d.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_d_s.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_d_s.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_l.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_l.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/Icons/workspace_l_s.png` & `CTK_Desert-0.0.9/src/CTK_Desert/images/Icons/workspace_l_s.png`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/images/empty.ico` & `CTK_Desert-0.0.9/src/CTK_Desert/images/empty.ico`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert/utils.py` & `CTK_Desert-0.0.9/src/CTK_Desert/utils.py`

 * *Files identical despite different names*

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert.egg-info/PKG-INFO` & `CTK_Desert-0.0.9/src/CTK_Desert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTK_Desert
-Version: 0.0.8
+Version: 0.0.9
 Summary: A GUI that uses the customtkinter library to create GUIs based on your need, so that you focus on the functionality of your application and not the design.
 Author-email: Morad Sayed <Morad.S.Singer@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CTK_Desert-0.0.8/src/CTK_Desert.egg-info/SOURCES.txt` & `CTK_Desert-0.0.9/src/CTK_Desert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

