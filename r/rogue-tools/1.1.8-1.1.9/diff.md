# Comparing `tmp/rogue_tools-1.1.8.tar.gz` & `tmp/rogue_tools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.1.8.tar", last modified: Tue Oct 17 02:42:16 2023, max compression
+gzip compressed data, was "rogue_tools-1.1.9.tar", last modified: Tue Oct 17 03:26:11 2023, max compression
```

## Comparing `rogue_tools-1.1.8.tar` & `rogue_tools-1.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-10-17 02:42:16.575877 rogue_tools-1.1.8/
--rw-rw-rw-   0        0        0      517 2023-10-17 02:42:16.575877 rogue_tools-1.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-10-17 02:42:16.565212 rogue_tools-1.1.8/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.1.8/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     8429 2023-10-17 01:13:32.000000 rogue_tools-1.1.8/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6558 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4070 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0     2868 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/install_tools.py
--rw-rw-rw-   0        0        0    13395 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     3380 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      588 2023-10-17 01:48:35.000000 rogue_tools-1.1.8/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1788 2023-10-13 06:19:54.000000 rogue_tools-1.1.8/rogue_tools/thread_tool.py
--rw-rw-rw-   0        0        0     2087 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     5266 2023-10-17 02:36:25.000000 rogue_tools-1.1.8/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     2300 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3860 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-10-13 02:26:52.000000 rogue_tools-1.1.8/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-10-17 02:42:16.573882 rogue_tools-1.1.8/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-10-17 02:42:16.000000 rogue_tools-1.1.8/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-10-17 02:42:16.000000 rogue_tools-1.1.8/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-17 02:42:16.000000 rogue_tools-1.1.8/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-10-17 02:42:16.000000 rogue_tools-1.1.8/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-17 02:42:16.000000 rogue_tools-1.1.8/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-10-17 02:42:16.000000 rogue_tools-1.1.8/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-10-17 02:42:16.576874 rogue_tools-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-10-17 02:41:53.000000 rogue_tools-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-17 03:26:11.934820 rogue_tools-1.1.9/
+-rw-rw-rw-   0        0        0      517 2023-10-17 03:26:11.933822 rogue_tools-1.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-10-17 03:26:11.920961 rogue_tools-1.1.9/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.1.9/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     8429 2023-10-17 01:13:32.000000 rogue_tools-1.1.9/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6558 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4070 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0     2868 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/install_tools.py
+-rw-rw-rw-   0        0        0    13395 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     3380 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      588 2023-10-17 01:48:35.000000 rogue_tools-1.1.9/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1788 2023-10-13 06:19:54.000000 rogue_tools-1.1.9/rogue_tools/thread_tool.py
+-rw-rw-rw-   0        0        0     2087 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     6278 2023-10-17 03:24:46.000000 rogue_tools-1.1.9/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     2300 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3860 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-10-13 02:26:52.000000 rogue_tools-1.1.9/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-10-17 03:26:11.931828 rogue_tools-1.1.9/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-10-17 03:26:11.000000 rogue_tools-1.1.9/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-10-17 03:26:11.000000 rogue_tools-1.1.9/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-17 03:26:11.000000 rogue_tools-1.1.9/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-10-17 03:26:11.000000 rogue_tools-1.1.9/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-10-17 03:26:11.000000 rogue_tools-1.1.9/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-10-17 03:26:11.000000 rogue_tools-1.1.9/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-10-17 03:26:11.934820 rogue_tools-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-10-17 03:26:03.000000 rogue_tools-1.1.9/setup.py
```

### Comparing `rogue_tools-1.1.8/PKG-INFO` & `rogue_tools-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.1.8
+Version: 1.1.9
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.1.8/rogue_tools/android_tool.py` & `rogue_tools-1.1.9/rogue_tools/android_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/excel_tool.py` & `rogue_tools-1.1.9/rogue_tools/excel_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/file_tool.py` & `rogue_tools-1.1.9/rogue_tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/filter_tool.py` & `rogue_tools-1.1.9/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/ini_tool.py` & `rogue_tools-1.1.9/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/install_tools.py` & `rogue_tools-1.1.9/rogue_tools/install_tools.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/path_tool.py` & `rogue_tools-1.1.9/rogue_tools/path_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/robot_tool.py` & `rogue_tools-1.1.9/rogue_tools/robot_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/show_tool.py` & `rogue_tools-1.1.9/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/string_tool.py` & `rogue_tools-1.1.9/rogue_tools/string_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/thread_tool.py` & `rogue_tools-1.1.9/rogue_tools/thread_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/time_tool.py` & `rogue_tools-1.1.9/rogue_tools/time_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/ui_tool.py` & `rogue_tools-1.1.9/rogue_tools/ui_tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,48 +42,54 @@
     
     def add_label(self,line_index,title, start_pos = (0,0),obj_w=200,obj_h=20):
         label = QLabel(self.windows)
         label.setAlignment(QtCore.Qt.AlignTop | QtCore.Qt.AlignLeft)
         label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w , obj_h))
         label.setText(title)
 
-    def add_btn(self,line_index,title, start_pos = (0,0),call_func=None,obj_w=100,obj_h=20):
+    def add_btn(self,line_index,title, start_pos = (0,0),obj_w=100,obj_h=20,call_func=None,is_thread=True,func_parms=[]):
         '''竖着放按钮'''
         #设置按钮并给按钮命名
-        btn = QPushButton(title,self.windows)
-        btn.setGeometry(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w , obj_h)
-        if call_func:
-            btn.clicked.connect(call_func)
+        btn = self._add_btn(title,start_pos[0] , obj_h * line_index+start_pos[1] , obj_w , obj_h,call_func,is_thread,func_parms)
         return btn
 
-    def add_btn_horizontal(self,line_index,title, start_pos = (0,0),call_func=None,obj_w=100,obj_h=20):
+    def add_btn_horizontal(self,line_index,title, start_pos = (0,0),obj_w=100,obj_h=20,call_func=None,is_thread=True, func_parms=[]):
         '''横着放按钮'''
         #设置按钮并给按钮命名
+        btn = self._add_btn(title,obj_w * line_index+start_pos[0],start_pos[1] , obj_w , obj_h,call_func,is_thread,func_parms)
+        return btn
+
+    def _add_btn(self,title,x,y,w,h,call_func,is_thread,func_parms):
+        def run():
+            if is_thread:
+                self.pool.add_task(title,call_func,*func_parms)
+            else:
+                call_func(*func_parms)
         btn = QPushButton(title,self.windows)
-        btn.setGeometry(obj_w * line_index+start_pos[0],start_pos[1] , obj_w , obj_h)
+        btn.setGeometry(x,y,w,h)
         if call_func:
-            btn.clicked.connect(call_func)
+            btn.clicked.connect(run)
         return btn
 
-    def add_input_editor(self,line_index,title, start_pos = (0,0) ,edit_text='',edit_tips='',obj_w_1=70,obj_w_2=200,obj_h = 20):
+    def add_input_editor(self,line_index,title, start_pos = (0,0),obj_w_1=70,obj_w_2=200,obj_h = 20 ,edit_text='',edit_tips=''):
         input_str = self.save_dic.get(title,'') if edit_text=='' else edit_text
         # 显示标签
         label = QLabel(self.windows)
         label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_1 , obj_h))
         label.setText(title)
         # 输入框
         edit = QLineEdit(self.windows)
         edit.setPlaceholderText(str(edit_tips))
         edit.setText(str(input_str))
         edit.setGeometry(QtCore.QRect(obj_w_1+start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_2 , obj_h))
         # 管理内容
         self.editor_dic[title] = edit.text
         return edit
     
-    def add_combo_box(self,line_index,title, start_pos = (0,0),item_list=[],obj_w_1=70,obj_w_2=200,obj_h = 20):
+    def add_combo_box(self,line_index,title, start_pos = (0,0),obj_w_1=70,obj_w_2=200,obj_h = 20,item_list=[]):
         currentText = self.save_dic.get(title,'')
         # 显示标签
         label = QLabel(self.windows)
         label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_1 , obj_h))
         label.setText(title)
         # 下拉框
         comb_box = QComboBox(self.windows)
@@ -117,15 +123,29 @@
         for line in lines:
             temp  = line.split('=')
             if len(temp)==2:
                 rs_dic[temp[0]]=temp[1]
         return rs_dic
 
 if __name__ == '__main__':
-    main_ui = mainUI(400,400)
-    main_ui.add_btn((10,10),1,'test1')
-    main_ui.add_btn((10,10),2,'test2')
-    main_ui.add_input_editor((160,10),1,'测试一下','test1')
-    main_ui.add_input_editor((160,10),2,'测试一下','test2')
-    main_ui.add_label((10,100),1,'test1')
-    main_ui.add_label((10,100),2,'test2')
-    main_ui.show()
+    from rogue_tools import string_tool
+    def test(k):
+        # 示范多线程
+        key =f'{string_tool.rnd_str(5), k, input.text(), box.currentText()}'
+        print(f'3秒后输出{key}')
+        time.sleep(3)
+        print(key)
+
+    ui = mainUI(300,600)
+    start_pos=(10,10)
+    btn1     = ui.add_btn(0,'竖着放1',start_pos, call_func= test, func_parms=['竖着放1111'])
+    btn2     = ui.add_btn(1,'竖着放2',start_pos, call_func= test, func_parms=['竖着放2222'])
+
+    start_pos=(10,60)
+    btn3     = ui.add_btn_horizontal(0,'横着放1',start_pos, call_func= test, func_parms=['横着放1111'])
+    btn4     = ui.add_btn_horizontal(1,'横着放2',start_pos, call_func= test, func_parms=['横着放2222'])
+
+    start_pos=(10,110)
+    input   = ui.add_input_editor(0,'input0',start_pos,edit_text='删掉显示提示',edit_tips='提示')
+    box     = ui.add_combo_box(1,'box0',start_pos,item_list=['box_str_1','box_str_2','box_str_3'])
+    label   = ui.add_label(2,'label0',start_pos)
+    ui.show()
```

### Comparing `rogue_tools-1.1.8/rogue_tools/web_tool.py` & `rogue_tools-1.1.9/rogue_tools/web_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/win_tool.py` & `rogue_tools-1.1.9/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/yaml_tool.py` & `rogue_tools-1.1.9/rogue_tools/yaml_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools/zip_tool.py` & `rogue_tools-1.1.9/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.1.9/rogue_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.1.8
+Version: 1.1.9
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.1.8/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.1.9/rogue_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.8/setup.py` & `rogue_tools-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 path_tool.del_('rogue_tools.egg-info')
 time.sleep(3)
 
 
 setup(
     name='rogue_tools',  # 包的名字
     author='luohao',  # 作者
-    version='1.1.8',  # 版本号
+    version='1.1.9',  # 版本号
     license='MIT',
 
     description='private tools',  # 描述
     long_description='''long description''',
     author_email='luohao@aobi.com',  # 你的邮箱**
     url='',  # 可以写github上的地址，或者其他地址
     # 包内需要引用的文件夹
```

