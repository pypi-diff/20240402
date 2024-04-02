# Comparing `tmp/dsplus-0.3.7.tar.gz` & `tmp/dsplus-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.3.7.tar", last modified: Fri Mar 29 03:05:43 2024, max compression
+gzip compressed data, was "dsplus-0.3.8.tar", last modified: Tue Apr  2 19:19:49 2024, max compression
```

## Comparing `dsplus-0.3.7.tar` & `dsplus-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 03:05:43.288040 dsplus-0.3.7/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.3.7/LICENSE
--rw-rw-rw-   0        0        0      690 2024-03-29 03:05:43.287187 dsplus-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 03:05:43.264238 dsplus-0.3.7/dsplus/
--rw-rw-rw-   0        0        0      171 2024-03-29 03:05:16.000000 dsplus-0.3.7/dsplus/__init__.py
--rw-rw-rw-   0        0        0    22326 2024-03-29 02:59:04.000000 dsplus-0.3.7/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    41986 2024-03-29 02:59:14.000000 dsplus-0.3.7/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    29517 2024-03-29 02:27:40.000000 dsplus-0.3.7/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    44406 2024-03-29 03:03:20.000000 dsplus-0.3.7/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-03-29 03:05:43.276327 dsplus-0.3.7/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-03-29 03:05:43.000000 dsplus-0.3.7/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-03-29 03:05:43.000000 dsplus-0.3.7/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 03:05:43.000000 dsplus-0.3.7/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 03:05:43.000000 dsplus-0.3.7/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 03:05:43.288040 dsplus-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 03:05:43.281453 dsplus-0.3.7/tests/
--rw-rw-rw-   0        0        0    12163 2024-03-29 02:59:04.000000 dsplus-0.3.7/tests/test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.470435 dsplus-0.3.8/
+-rw-rw-rw-   0        0        0     1084 2024-03-29 14:28:34.000000 dsplus-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-04-02 19:19:49.469864 dsplus-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2024-03-29 14:28:34.000000 dsplus-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.429272 dsplus-0.3.8/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-04-02 19:19:36.000000 dsplus-0.3.8/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24320 2024-04-02 19:06:51.000000 dsplus-0.3.8/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    41986 2024-03-29 14:28:34.000000 dsplus-0.3.8/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56679 2024-04-01 14:08:05.000000 dsplus-0.3.8/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    44406 2024-03-29 14:28:34.000000 dsplus-0.3.8/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.454275 dsplus-0.3.8/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:19:49.470955 dsplus-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1693 2024-03-29 18:38:45.000000 dsplus-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.468300 dsplus-0.3.8/tests/
+-rw-rw-rw-   0        0        0    12143 2024-03-29 16:50:11.000000 dsplus-0.3.8/tests/Test_pandas.py
```

### Comparing `dsplus-0.3.7/LICENSE` & `dsplus-0.3.8/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `dsplus-0.3.7/PKG-INFO` & `dsplus-0.3.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.3.7
+Version: 0.3.8
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.3.7/dsplus/pb_functions_general.py` & `dsplus-0.3.8/dsplus/pb_functions_general.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,38 @@
 
     return (value_numeric)
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: File
 
 #%%
+def os_path(path: str|list|np.ndarray|pd.Series) -> str|pd.Series:
+    '''Replace forward slash by back slash in path.
+
+    Args:
+        path (str | list | np.ndarray | pd.Series): Vector of pathnames.
+
+    Returns:
+        str|pd.Series: Pathname(s) with only back slashes. If 'path' is string literal, string literal is returned. Otherwise, Series is returned.
+
+    Examples:
+        >>> os_path(r'd:\try.txt')
+        >>> os_path('d:\\try.txt')
+        >>> os_path([r'd:\try.txt', 'd:\\try.txt'])
+    '''
+    v_path = pd_to_series(path)
+
+    v_path = v_path.str.replace('\\', '/').str.replace('//', '/')
+
+    if isinstance(path, str):
+        return v_path.iloc[0]
+    else:
+        return v_path
+
+#%%
 def os_path_join(folders: str|list|np.ndarray|pd.Series,
                  files: str|list|np.ndarray|pd.Series,
                  extensions: str|list|np.ndarray|pd.Series= None) -> pd.Series:
     '''Vectorized function for joining folder and file paths.
 
     Args:
         folders (str | list | np.ndarray | pd.Series): Vector of folder paths.
@@ -67,19 +91,19 @@
     Returns:
         Series: Series of full paths.
 
     Noted:
         - The length of the files, folders, and extensions can be: (a) all 1, (b) 1 for one and same for the other two, or (c) same for all three.
 
     Examples:
-        >>> path_join(r'd:\folder', 'file')
-        >>> path_join(r'd:\folder', 'file', 'txt')
-        >>> path_join(r'd:\folder', ['file1', 'file2'], 'txt')
-        >>> path_join([r'd:\folder1', r'd:/folder2'], 'file')
-        >>> path_join([r'd:\folder1', r'd:/folder2'], ['file1', 'file2'], ['txt', 'csv'])
+        >>> os_path_join(r'd:\folder', 'file')
+        >>> os_path_join(r'd:\folder', 'file', 'txt')
+        >>> os_path_join(r'd:\folder', ['file1', 'file2'], 'txt')
+        >>> os_path_join([r'd:\folder1', r'd:/folder2'], 'file')
+        >>> os_path_join([r'd:\folder1', r'd:/folder2'], ['file1', 'file2'], ['txt', 'csv'])
     '''
     v_folders = pd_to_series(folders)
     v_files = pd_to_series(files)
     v_extensions = pd_to_series(extensions)
 
     len_max = np.max([len(v_folders), len(v_files), len(v_extensions)])
 
@@ -99,31 +123,69 @@
 
     if extensions is not None:
         v_path = v_path.str.cat(v_extensions, sep = r'.')
 
     return (v_path)
 
 #%%
+def os_filename(v_pathnames: str|list|np.ndarray|pd.Series) -> pd.Series:
+    '''Remove extension from pathnames.
+
+    Args:
+        v_pathnames (str | list | np.ndarray | pd.Series): Vector of pathnames.
+
+    Returns:
+        pd.Series: Series of filenames with extensions removed.
+
+    Examples:
+        >>> os_filename('try.txt')
+        >>> os_filename(['try.txt.jpg', 'try2.txt'])
+    '''
+    v_pathnames = pd.Series([os.path.splitext(v_pathname)[0] for v_pathname in pd_to_series(v_pathnames)])
+
+    return v_pathnames
+
+#%%
+def os_extension(v_pathnames: str|list|np.ndarray|pd.Series) -> pd.Series:
+    '''Get extension from pathnames.
+
+    Args:
+        v_pathnames (str | list | np.ndarray | pd.Series): Vector of pathnames.
+
+    Returns:
+        pd.Series: Series of extensions.
+
+    Examples:
+        >>> os_extension(r'D:\try.txt')
+        >>> os_extension([r'D:\try.txt.jpg', r'D:\try2.txt'])
+    '''
+    v_pathnames = pd.Series([os.path.splitext(v_pathname)[1] for v_pathname in pd_to_series(v_pathnames)]).str.replace(r'.', '')
+
+    return v_pathnames
+
+#%%
 def os_basename(v_pathnames: str|list|np.ndarray|pd.Series, keep_extension = True) -> pd.Series:
     '''Get basenames from pathnames. Wrapper around 'os.path.basename()'.
 
     Args:
         v_pathnames (str | list | np.ndarray | pd.Series): Vector of pathnames.
+        keep_extension (bool, True): If False, extensions are removed. Defaults to True.
 
     Returns:
         pd.Series: Series of basenames.
 
     Examples:
         >>> os_basename('D:\try.txt')
-        >>> os_basename(['D:\try.txt', 'D:\try2.txt'])
+        >>> os_basename([r'D:\try.txt', r'D:\try2.txt'])
     '''
     v_pathnames = pd.Series([os.path.basename(v_pathname) for v_pathname in pd_to_series(v_pathnames)])
 
     if not keep_extension:
-        v_pathnames = pd.Series([os.path.splitext(v_pathname)[0] for v_pathname in pd_to_series(v_pathnames)])
+        # v_pathnames = pd.Series([os.path.splitext(v_pathname)[0] for v_pathname in pd_to_series(v_pathnames)])
+        v_pathnames = os_filename(v_pathnames)
 
     return (v_pathnames)
 
 #%%
 def os_dirname(v_pathnames: str|list|np.ndarray|pd.Series) -> pd.Series:
     '''Get dirnames from pathnames. Wrapper around 'os.path.dirname()'.
```

### Comparing `dsplus-0.3.7/dsplus/pb_functions_pandas.py` & `dsplus-0.3.8/dsplus/pb_functions_pandas.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.3.7/dsplus/pb_functions_spatial.py` & `dsplus-0.3.8/dsplus/pb_functions_spatial.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.3.7/dsplus.egg-info/PKG-INFO` & `dsplus-0.3.8/dsplus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.3.7
+Version: 0.3.8
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.3.7/setup.py` & `dsplus-0.3.8/setup.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from setuptools import setup, find_packages
-from dsplus.__init__ import __version__
-
-setup(
-    name='dsplus',
-    version=__version__,
-    author='Prashana Bajracharya',
-    author_email='pajracharya713@gmail.com',
-    description='Helper functions for data science applications.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    # author=httpimport.__author__,
-    # license='MIT',
-    # url=httpimport.__github__,
-    # py_modules=['dsplus'],
-    packages=find_packages(),
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    # python_requires='>=3.6',
-    # classifiers=[
-    #     'Development Status :: 6 - Mature',
-    #     'Programming Language :: Python :: 3.4',
-    #     'Programming Language :: Python :: 3.7',
-    #     'Programming Language :: Python :: 3.9',
-    #     'Programming Language :: Python :: 3.11',
-    #     'Programming Language :: Python :: Implementation :: CPython',
-    #     'Programming Language :: Python :: Implementation :: PyPy',
-    #     'Intended Audience :: Developers',
-    #     'Intended Audience :: Information Technology',
-    #     'Topic :: Software Development :: Libraries :: Python Modules',
-    #     'Topic :: Software Development :: Build Tools',
-    #     'Topic :: Software Development :: Testing',
-    # ],
-    keywords=[
-        'data science',
-        'pandas'],
-)
+from setuptools import setup, find_packages
+from dsplus.__init__ import __version__
+
+setup(
+    name='dsplus',
+    version=__version__,
+    author='Prashana Bajracharya',
+    author_email='pajracharya713@gmail.com',
+    description='Helper functions for data science applications.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    # author=httpimport.__author__,
+    # license='MIT',
+    # url=httpimport.__github__,
+    # py_modules=['dsplus'],
+    packages=find_packages(),
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    # python_requires='>=3.6',
+    # classifiers=[
+    #     'Development Status :: 6 - Mature',
+    #     'Programming Language :: Python :: 3.4',
+    #     'Programming Language :: Python :: 3.7',
+    #     'Programming Language :: Python :: 3.9',
+    #     'Programming Language :: Python :: 3.11',
+    #     'Programming Language :: Python :: Implementation :: CPython',
+    #     'Programming Language :: Python :: Implementation :: PyPy',
+    #     'Intended Audience :: Developers',
+    #     'Intended Audience :: Information Technology',
+    #     'Topic :: Software Development :: Libraries :: Python Modules',
+    #     'Topic :: Software Development :: Build Tools',
+    #     'Topic :: Software Development :: Testing',
+    # ],
+    keywords=[
+        'data science',
+        'pandas'],
+)
```

### Comparing `dsplus-0.3.7/tests/test_pandas.py` & `dsplus-0.3.8/tests/Test_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,31 +61,31 @@
 
     assert v == [0,1,2]
 
 #endregion -----------------------------------------------------------------------------------------
 #region Type Conversion
 
 #%%
-def test_vector_to_series_1():
+def test_pd_to_series_1():
     assert ds.pd_to_series([1,2,3]).equals(pd.Series([1,2,3]))
 
 #%%
-def test_vector_to_series_2():
+def test_pd_to_series_2():
     assert ds.pd_to_series([]).equals(pd.Series([]))
 
 #%%
-def test_vector_to_series_3():
+def test_pd_to_series_3():
     assert ds.pd_to_series(np.array([1,2,3])).equals(pd.Series(np.array([1,2,3])))
 
 #%%
-def test_vector_to_series_4():
+def test_pd_to_series_4():
     assert ds.pd_to_series(pd.Series([1,2,3])).equals(pd.Series([1,2,3]))
 
 #%%
-def test_vector_to_series_5():
+def test_pd_to_series_5():
     assert ds.pd_to_series(pd.Series([1,2,3]).index).equals(pd.Series([0,1,2]))
 
 #endregion -----------------------------------------------------------------------------------------
 #region Slice
 
 #%%
 def test_pd_select_1():
```

