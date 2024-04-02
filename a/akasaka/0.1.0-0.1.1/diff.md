# Comparing `tmp/akasaka-0.1.0.tar.gz` & `tmp/akasaka-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akasaka-0.1.0.tar", last modified: Mon Apr  1 22:30:13 2024, max compression
+gzip compressed data, was "akasaka-0.1.1.tar", last modified: Tue Apr  2 00:34:35 2024, max compression
```

## Comparing `akasaka-0.1.0.tar` & `akasaka-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:13.375286 akasaka-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-01 22:30:02.000000 akasaka-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-01 22:30:13.375286 akasaka-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 22:30:02.000000 akasaka-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:13.371286 akasaka-0.1.0/akasaka/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 22:30:02.000000 akasaka-0.1.0/akasaka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-01 22:30:02.000000 akasaka-0.1.0/akasaka/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-01 22:30:02.000000 akasaka-0.1.0/akasaka/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-01 22:30:02.000000 akasaka-0.1.0/akasaka/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:13.375286 akasaka-0.1.0/akasaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-01 22:30:13.000000 akasaka-0.1.0/akasaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-01 22:30:13.000000 akasaka-0.1.0/akasaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:30:13.000000 akasaka-0.1.0/akasaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 22:30:13.000000 akasaka-0.1.0/akasaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 22:30:13.000000 akasaka-0.1.0/akasaka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 22:30:13.000000 akasaka-0.1.0/akasaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:30:13.375286 akasaka-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-01 22:30:02.000000 akasaka-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:34:35.589683 akasaka-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 00:34:26.000000 akasaka-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-02 00:34:35.589683 akasaka-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-02 00:34:26.000000 akasaka-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:34:35.589683 akasaka-0.1.1/akasaka/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 00:34:26.000000 akasaka-0.1.1/akasaka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-02 00:34:26.000000 akasaka-0.1.1/akasaka/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-02 00:34:26.000000 akasaka-0.1.1/akasaka/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-02 00:34:26.000000 akasaka-0.1.1/akasaka/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:34:35.589683 akasaka-0.1.1/akasaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-02 00:34:35.000000 akasaka-0.1.1/akasaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-02 00:34:35.000000 akasaka-0.1.1/akasaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:34:35.000000 akasaka-0.1.1/akasaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 00:34:35.000000 akasaka-0.1.1/akasaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 00:34:35.000000 akasaka-0.1.1/akasaka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 00:34:35.000000 akasaka-0.1.1/akasaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:34:35.589683 akasaka-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-02 00:34:26.000000 akasaka-0.1.1/setup.py
```

### Comparing `akasaka-0.1.0/LICENSE` & `akasaka-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.0/PKG-INFO` & `akasaka-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasaka
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic mutiprocess preprocessing task loader and dispatcher
 Home-page: https://github.com/JeffersonQin/akasaka
 Author: Haoyun Qin
 Author-email: qhy.cis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `akasaka-0.1.0/README.md` & `akasaka-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.0/akasaka/loader.py` & `akasaka-0.1.1/akasaka/loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import importlib.util
 
 
 def load_class(module_path):
     try:
         module_name, class_name = module_path.rsplit('.', 1)
-        print(module_name)
-        print(class_name)
         spec = importlib.util.find_spec(module_name)
         if spec is None:
             raise ImportError(f"Module '{module_name}' not found.")
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         if not hasattr(module, class_name):
             raise AttributeError(f"Class '{class_name}' not found in module '{module_name}'.")
```

### Comparing `akasaka-0.1.0/akasaka/main.py` & `akasaka-0.1.1/akasaka/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,40 +31,36 @@
     
     module_path = args.module_path
     num_process = args.num_process
     
     if args.help:
         remaining_args += ["-h"]
 
-    try:
-        # Add the current working directory to the sys.path so that the module can be found
-        sys.path.append(os.getcwd())
-        # Load the class from the module
-        loaded_class = load_class(module_path)
-        print(f"Successfully loaded class '{loaded_class.__name__}' from module '{args.module_path}'.")
-        # Check if the loaded class is a subclass of 'AkasakaTask'
-        if not issubclass(loaded_class, AkasakaTask):
-            raise ValueError("The loaded class should be a subclass of 'AkasakaTask'.")
-
-        # Initialize the task with the remaining command line arguments
-        akasaka_task = loaded_class(args=remaining_args)
-
-        # Generate a list of tasks to be executed
-        tasks = akasaka_task.generate_tasks()
-        tasks = list(tasks)
-        print(f"Generated {len(tasks)} tasks to be executed.")
-
-        pool = multiprocessing.Pool(processes=num_process)
-
-        # using the chunksize for better performance
-        # this implementation is taken from the official implementation of multiprocessing.Pool.map
-        chunksize, extra = divmod(len(tasks), num_process * 4)
-        if extra:
-            chunksize += 1
+    # Add the current working directory to the sys.path so that the module can be found
+    sys.path.append(os.getcwd())
+    # Load the class from the module
+    loaded_class = load_class(module_path)
+    print(f"Successfully loaded class '{loaded_class.__name__}' from module '{args.module_path}'.")
+    # Check if the loaded class is a subclass of 'AkasakaTask'
+    if not issubclass(loaded_class, AkasakaTask):
+        raise ValueError("The loaded class should be a subclass of 'AkasakaTask'.")
+
+    # Initialize the task with the remaining command line arguments
+    akasaka_task = loaded_class(args=remaining_args)
+
+    # Generate a list of tasks to be executed
+    tasks = akasaka_task.generate_tasks()
+    tasks = list(tasks)
+    print(f"Generated {len(tasks)} tasks to be executed.")
+
+    pool = multiprocessing.Pool(processes=num_process)
+
+    # using the chunksize for better performance
+    # this implementation is taken from the official implementation of multiprocessing.Pool.map
+    chunksize, extra = divmod(len(tasks), num_process * 4)
+    if extra:
+        chunksize += 1
 
-        _ = list(tqdm(pool.imap_unordered(execute, tasks, chunksize=chunksize), total=len(tasks)))
+    _ = list(tqdm(pool.imap_unordered(execute, tasks, chunksize=chunksize), total=len(tasks)))
 
-        pool.close()
-        pool.join()
-
-    except (ImportError, AttributeError, ValueError) as e:
-        print(f"Error: {e}")
+    pool.close()
+    pool.join()
```

### Comparing `akasaka-0.1.0/akasaka/task.py` & `akasaka-0.1.1/akasaka/task.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.0/akasaka.egg-info/PKG-INFO` & `akasaka-0.1.1/akasaka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasaka
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic mutiprocess preprocessing task loader and dispatcher
 Home-page: https://github.com/JeffersonQin/akasaka
 Author: Haoyun Qin
 Author-email: qhy.cis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `akasaka-0.1.0/setup.py` & `akasaka-0.1.1/setup.py`

 * *Files identical despite different names*

