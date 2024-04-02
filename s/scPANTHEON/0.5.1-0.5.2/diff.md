# Comparing `tmp/scPANTHEON-0.5.1.tar.gz` & `tmp/scPANTHEON-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.5.1.tar", last modified: Sun Mar 24 09:49:47 2024, max compression
+gzip compressed data, was "scPANTHEON-0.5.2.tar", last modified: Tue Apr  2 14:48:46 2024, max compression
```

## Comparing `scPANTHEON-0.5.1.tar` & `scPANTHEON-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 09:49:47.801265 scPANTHEON-0.5.1/
--rw-rw-rw-   0        0        0      238 2024-03-24 09:49:47.800265 scPANTHEON-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-01-02 19:33:04.000000 scPANTHEON-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 09:49:47.756985 scPANTHEON-0.5.1/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      238 2024-03-24 09:49:47.000000 scPANTHEON-0.5.1/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2024-03-24 09:49:47.000000 scPANTHEON-0.5.1/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 09:49:47.000000 scPANTHEON-0.5.1/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-03-24 09:49:47.000000 scPANTHEON-0.5.1/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-03-24 09:49:47.000000 scPANTHEON-0.5.1/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-24 09:49:47.000000 scPANTHEON-0.5.1/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-24 09:49:47.765001 scPANTHEON-0.5.1/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.1/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 09:49:47.782034 scPANTHEON-0.5.1/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.1/scpantheon/app/__init__.py
--rw-rw-rw-   0        0        0     2978 2024-03-23 11:36:17.000000 scPANTHEON-0.5.1/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2024-03-24 09:49:47.797266 scPANTHEON-0.5.1/scpantheon/front_end/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.1/scpantheon/front_end/__init__.py
--rw-rw-rw-   0        0        0    11831 2024-03-24 05:48:52.000000 scPANTHEON-0.5.1/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     4227 2024-03-24 05:48:52.000000 scPANTHEON-0.5.1/scpantheon/front_end/extensions_qt.py
--rw-rw-rw-   0        0        0     4567 2024-03-23 11:36:17.000000 scPANTHEON-0.5.1/scpantheon/front_end/load_qt.py
--rw-rw-rw-   0        0        0     4899 2024-03-23 11:36:17.000000 scPANTHEON-0.5.1/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1314 2024-03-24 09:48:50.000000 scPANTHEON-0.5.1/scpantheon/main.py
--rw-rw-rw-   0        0        0    66606 2024-03-24 09:20:45.000000 scPANTHEON-0.5.1/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2024-03-24 09:49:47.802266 scPANTHEON-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-03-24 09:49:06.000000 scPANTHEON-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:48:46.000270 scPANTHEON-0.5.2/
+-rw-rw-rw-   0        0        0      238 2024-04-02 14:48:45.999271 scPANTHEON-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-01-02 19:33:04.000000 scPANTHEON-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 14:48:45.971272 scPANTHEON-0.5.2/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      238 2024-04-02 14:48:45.000000 scPANTHEON-0.5.2/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-02 14:48:45.000000 scPANTHEON-0.5.2/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:48:45.000000 scPANTHEON-0.5.2/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-02 14:48:45.000000 scPANTHEON-0.5.2/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-02 14:48:45.000000 scPANTHEON-0.5.2/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 14:48:45.000000 scPANTHEON-0.5.2/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 14:48:45.978270 scPANTHEON-0.5.2/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.2/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:48:45.983271 scPANTHEON-0.5.2/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.2/scpantheon/app/__init__.py
+-rw-rw-rw-   0        0        0     2978 2024-03-23 11:36:17.000000 scPANTHEON-0.5.2/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:48:45.995273 scPANTHEON-0.5.2/scpantheon/front_end/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.2/scpantheon/front_end/__init__.py
+-rw-rw-rw-   0        0        0    12912 2024-04-02 10:22:19.000000 scPANTHEON-0.5.2/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     4227 2024-03-24 05:48:52.000000 scPANTHEON-0.5.2/scpantheon/front_end/extensions_qt.py
+-rw-rw-rw-   0        0        0     4567 2024-03-23 11:36:17.000000 scPANTHEON-0.5.2/scpantheon/front_end/load_qt.py
+-rw-rw-rw-   0        0        0     4899 2024-03-23 11:36:17.000000 scPANTHEON-0.5.2/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1309 2024-04-02 10:28:00.000000 scPANTHEON-0.5.2/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66684 2024-04-02 11:00:55.000000 scPANTHEON-0.5.2/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:48:46.001271 scPANTHEON-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-02 14:48:33.000000 scPANTHEON-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:48:45.997273 scPANTHEON-0.5.2/tests/
+-rw-rw-rw-   0        0        0      294 2024-04-02 14:13:56.000000 scPANTHEON-0.5.2/tests/test_data.py
```

### Comparing `scPANTHEON-0.5.1/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.5.2/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.1/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.5.2/scpantheon/front_end/data_qt.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,35 +31,43 @@
     my_signal = pyqtSignal(str)
 
     def __init__(self):
         super(Ui_Dialog, self).__init__()
     
     def setupUi(self, Dialog):
         Dialog.setObjectName("Data Panel")
-        Dialog.resize(750, 300)
+        Dialog.resize(750, 400)
         self.cwd = os.getcwd()
         font = QtGui.QFont()
         font.setPointSize(20)
         font.setWeight(20)
         # render help text
         self.text_brow = QTextBrowser()
 
         '''# Choose path button
         self.btn_Extensions = QPushButton("Choose New Extensions folder",self)  
         self.btn_Extensions.setObjectName("btn_Extensions")  
         self.btn_Extensions.clicked.connect(self.slot_btn_Extensions)
         self.btn_Extensions.setFont(font)
         self.btn_Extensions.setMinimumSize(750, 100)
         # self.btn_Extensions.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)'''
-        # Choose file button
-        self.btn_Data = QPushButton("Choose New Data File",self)  
-        self.btn_Data.setObjectName("btn_Data")  
-        self.btn_Data.clicked.connect(self.slot_btn_Data)
-        self.btn_Data.setFont(font)
-        self.btn_Data.setMinimumSize(750, 100)
+        # Choose Data File Button
+        self.btn_Data_File = QPushButton("Choose New Data File",self)  
+        self.btn_Data_File.setObjectName("btn_Data_File")  
+        self.btn_Data_File.clicked.connect(self.slot_btn_Data_file)
+        self.btn_Data_File.setFont(font)
+        self.btn_Data_File.setMinimumSize(750, 100)
+        # self.btn_Data.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+
+        # Choose Data Folder Button
+        self.btn_Data_Folder = QPushButton("Choose New Data Folder",self)  
+        self.btn_Data_Folder.setObjectName("btn_Data_Folder")  
+        self.btn_Data_Folder.clicked.connect(self.slot_btn_Data_folder)
+        self.btn_Data_Folder.setFont(font)
+        self.btn_Data_Folder.setMinimumSize(750, 100)
         # self.btn_Data.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         # Start scpantheon
         self.btn_Start = QPushButton("Data Not Found",self)
         self.btn_Start.setObjectName("btn_Start")
         self.btn_Start.clicked.connect(lambda : self.Run(Dialog))
         self.btn_Start.setFont(font)
@@ -72,61 +80,75 @@
 
         self.buttonBox = QDialogButtonBox(Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
         self.buttonBox.setObjectName("buttonBox")
         self.layout.addWidget(self.buttonBox)
 
         '''self.layout.addWidget(self.btn_Extensions)'''
-        self.layout.addWidget(self.btn_Data)
+        self.layout.addWidget(self.btn_Data_File)
+        self.layout.addWidget(self.btn_Data_Folder)
         self.layout.addWidget(self.btn_Start)
 
         # self.retranslateUi(Dialog) 
         # self.buttonBox.accepted.connect(self.accepted)
         self.buttonBox.rejected.connect(self.rejected)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
         
         try:
             '''extensions_path, data_file = read_path(dir) '''
-            extensions_file, data_file = read_path(dir) 
-            if data_file != '':
+            extensions_file, data = read_path(dir) 
+            if data != '':
                 self.btn_Start.setText("Run Previous Data")
-                self.text_brow.setText("\t\t\tPrevious Data File Path:\n\t" + data_file)
+                self.text_brow.setText("\t\t\tPrevious Data Path:\n\t" + data)
             else:
                 self.btn_Data.setText("Choose A Data File!")
-                self.text_brow.setText("\t\t\tData File Not Found...")
+                self.text_brow.setText("\t\t\tData Not Found...")
             '''auto_pip_install(extensions_path) '''
         except:
-            self.btn_Data.setText("Choose A Data File!")
-            self.text_brow.setText("\t\t\tData File Not Found...")
+            self.btn_Data.setText("Choose A Data File Or Folder!")
+            self.text_brow.setText("\t\t\tData Not Found...")
 
     def event(self, event):
         if event.type()==QtCore.QEvent.EnterWhatsThisMode:
             QWhatsThis.leaveWhatsThisMode()
             # self.text_brow.setText("Choose your extension packages and your data") 
         return QDialog.event(self,event)
 
     '''def slot_btn_Extensions(self):
         global Extensions
         Extensions = QFileDialog.getExistingDirectory(self," ",self.cwd) # 起始路径
         # write extension into user_data_dir
         if Extensions != '':
            write_msg('extensions_path', Extensions)'''
 
-    def slot_btn_Data(self):
+    def slot_btn_Data_file(self):
         global Data
         Data, file_type = QFileDialog.getOpenFileName(self, " ", self.cwd)   # 设置文件扩展名过滤,用双分号间隔
         if Data == "":
             # print("\nchoose canceled")
             return
         # write Data into user_data_dir
         write_msg('data_file', Data)
         # print("Data:",Data)
         # self.text_brow.append("new data path:"+Data)
         self.btn_Start.setText("Run New Data!")
         self.text_brow.setText("\t\t\tNew Data File Path:\n\t" + Data)
+    
+    def slot_btn_Data_folder(self):
+        global Data
+        Data = QFileDialog.getExistingDirectory(self, " ", self.cwd)   # 设置文件扩展名过滤,用双分号间隔
+        if Data == "":
+            # print("\nchoose canceled")
+            return
+        # write Data into user_data_dir
+        write_msg('data_file', Data)
+        # print("Data:",Data)
+        # self.text_brow.append("new data path:"+Data)
+        self.btn_Start.setText("Run New Data!")
+        self.text_brow.setText("\t\t\tNew Data Folder Path:\n\t" + Data)
 
     def Run(self, Dialog):
         global check_code
         check_code = 'app closed'
         Dialog.reject() 
 
 # extract online extension zip
```

### Comparing `scPANTHEON-0.5.1/scpantheon/front_end/extensions_qt.py` & `scPANTHEON-0.5.2/scpantheon/front_end/extensions_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.1/scpantheon/front_end/load_qt.py` & `scPANTHEON-0.5.2/scpantheon/front_end/load_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.1/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.5.2/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.1/scpantheon/main.py` & `scPANTHEON-0.5.2/scpantheon/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from multiprocessing import freeze_support
 
 import multiprocessing
 import pkg_resources, subprocess
 try:
-    from scpantheon import source
+    # !!!
+    import source
     from scpantheon.app import bokeh_qt
-    from scpantheon.front_end import data_qt
+    # !!!
+    from front_end import data_qt
     version = pkg_resources.get_distribution("scpantheon").version
 except:
     print("pip install scpantheon")
     subprocess.check_call(['pip', 'install', "scpantheon"])
     from scpantheon import source
     from scpantheon.app import bokeh_qt
     from scpantheon.front_end import data_qt
```

### Comparing `scPANTHEON-0.5.1/scpantheon/source.py` & `scPANTHEON-0.5.2/scpantheon/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 TOOLTIPS = [
         ("(x,y)", "($x, $y)"),
         ("color", "@color"),
 ]
 
 class FlowPlot:
-    global data_file
+    global data_path
     def __init__(self, data=None, color_map=None, x_init_idx = 0, y_init_idx = 1, allow_select = True, select_color_change = True, main_plot = None,title=None): # - legend=None
         self.adata = data
         self.data_df = self.adata.to_df()
         self.data_log = np.log1p(self.data_df)    
         # For real-valued input, log1p is accurate also for x so small that 1 + x == 1 in floating-point accuracy.
         self.label_existed, view_existed = False, False # group_label_existed
         # personalized
@@ -577,15 +577,15 @@
             color_js = ''
             '''print('\ntext_color: color===')
             print(self.adata.uns['category_dict'][self.group.value]['color'])'''
             try:
                 length = len(self.adata.uns['category_dict'][self.group.value]['color']) 
                 for i in range(length):
                     color_js = color_js + self.adata.uns['category_dict'][self.group.value]['color'][i] + ' '
-                    print("color_js", color_js)
+                    # print("color_js", color_js)
                 self.para_color.text = color_js + color_list[18]
             except:
                 print('====text color failed===')
                 length = 1
                 # color_js = [color_list[18]]
                 self.para_color.text = str(color_list[18])
             # trigger js_on_change
@@ -979,15 +979,15 @@
         return to_json
 
         
 color_list = d3['Category20c'][20]
 Main_plot = FlowPlot
 
 class connection:
-    global extensions_path, data_file
+    global extensions_path, data_path
     def __init__(self):
         self.Figure = Main_plot
     
     def get_attributes(self):
         if self.Figure.view.filters == []:
             remain_cells = list(range(self.Figure.data_df.shape[0]))
         else:
@@ -1096,16 +1096,16 @@
         view_list = list(obsm.keys())+['generic_columns']
         self.Figure.adata.obsm = obsm
         self.Figure.choose_panel.options = view_list
         self.Figure.choose_panel.value = view_list[-2]
         self.Figure.s_x.value = view_list[-2] + str(0)
         self.Figure.s_y.value = view_list[-2] + str(1)
     
-    def get_data_file(self):
-        return data_file
+    def get_data_path(self):
+        return data_path
 
     def get_extension_file(self):
         return extensions_path
 
 
 class plot_function:
     def __init__(self):
@@ -1219,16 +1219,18 @@
             print('new_buttons:', new_buttons)
             new_buttons.sizing_mode = 'scale_height'
             new_buttons.name = name
             new_buttons.children.append(div)
             curdoc().add_root(new_buttons)
             layouts = column(layouts, new_buttons)
         else:
-            if but != None:
-                but.visible = False
+            if but is not None:
+                curdoc().remove_root(but)
+            '''if but != None:
+                but.visible = False'''
         ind = ind + 1
     buttons = layouts
     if curdoc().get_model_by_name('module_buttons') == None:
         buttons.name = 'module_buttons'
     # curdoc().add_root(buttons)
 
 def add_to_buttons_group(buttons, buttons_group):
@@ -1270,40 +1272,42 @@
     print(curdoc().get_model_by_name(option))
     load_module(module_checkbox.value)
     # models.visible = False
     # module_checkbox.active.remove(int(ind))
 
 def upload_callback(): 
 
-    global data_file
+    global data_path
     global Main_plot
 
     # path_, file_name = fetch()
     loading_remind = Div(text='Loading data……')
     curdoc().add_root(loading_remind) 
     print('===loading finished=====')
-    filename = os.path.split(data_file)[1]   
+    filename = os.path.split(data_path)[1]   
 
     def load():
         global Main_plot
-        filetype = os.path.splitext(filename)[-1][1:] # split the filename and the type
-                                                      # [-1] means the last tuple: the type 
+        filetype = os.path.splitext(filename)[-1][1:] # split the filename and the type, [-1] means the last tuple: the type 
+        # !!!
+        print('filetype:', filetype)
         if filetype == 'csv':
-            adata = sc.read_csv(data_file) 
+            adata = sc.read_csv(data_path) 
             print('csv data')
         elif filetype == 'h5ad':
-            adata = sc.read_h5ad(data_file)
-            # adata = anndata.read(data_file, backed='r')  
+            adata = sc.read_h5ad(data_path)
+            # adata = anndata.read(data_path, backed='r')  
             print('h5ad data')
-        elif filetype == 'mtx':
+        elif filetype == '':
+            print("read_10x")
             adata = sc.read_10x_mtx(
-                'data/hg19/',  # the directory with the `.mtx` file
+                data_path,# the directory with the `.mtx` file
                 var_names='gene_symbols',                # use gene symbols for the variable names (variables-axis index)
                 cache=True)                              # write a cache file for faster subsequent reading
-        # print(data_file)
+
         # Figure, layout
         mainplot, panel1 = CreateTool(adata=adata).base_tool() # Mainplot: figure, layout
         print('===mainplot finished=====')
         Main_plot = mainplot
         # Highlight Gene Figure
         hl_figure, panel2 = CreateTool(adata=adata).highlight_gene(mainplot)
         print('====highlight finished=====')
@@ -1322,18 +1326,18 @@
         f.truncate(0)
         f.close()
     file = open(path, 'w')
     file.write(msg)
     file.close()
 
 def main(doc):
-    global Main_plot, extensions_path, data_file, module_select_id
+    global Main_plot, extensions_path, data_path, module_select_id
     module_select_id = 1999
     # read path_ and file from user_data_dir
-    extensions_path, data_file = read_path(dir)
+    extensions_path, data_path = read_path(dir)
     # auto_pip_install(extensions_path)    
     doc.add_next_tick_callback(upload_callback)                                                     
     
     '''
     global mycursor
     try: myconnect()
     except:
```

### Comparing `scPANTHEON-0.5.1/setup.py` & `scPANTHEON-0.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.5.1',#版本
+    version='0.5.2',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
-    install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5==5.15.6','PyQtWebEngine',
-                       'appdirs','requests','leidenalg'], # 依赖包,如果没有,可以不要 rpy2
+    install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
+                       'appdirs','requests','leidenalg', 'setuptools_scm'], # 依赖包,如果没有,可以不要 rpy2
     extras_require={
         
     }, # 依赖包,深度使用需手动安装
     entry_points={
         'console_scripts': [
             'sc-pantheon = scpantheon.main:main' # scripts -> multiprocessing
         ]
```

