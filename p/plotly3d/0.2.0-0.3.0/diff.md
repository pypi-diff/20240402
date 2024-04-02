# Comparing `tmp/plotly3d-0.2.0.tar.gz` & `tmp/plotly3d-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.2.0.tar", last modified: Mon Apr  1 21:03:19 2024, max compression
+gzip compressed data, was "plotly3d-0.3.0.tar", last modified: Tue Apr  2 03:00:25 2024, max compression
```

## Comparing `plotly3d-0.2.0.tar` & `plotly3d-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-01 21:03:19.755547 plotly3d-0.2.0/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.2.0/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      267 2024-04-01 21:03:19.754708 plotly3d-0.2.0/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.2.0/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-01 21:03:19.750902 plotly3d-0.2.0/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-03-31 02:49:53.000000 plotly3d-0.2.0/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     5478 2024-04-01 20:59:47.000000 plotly3d-0.2.0/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-01 21:03:19.753977 plotly3d-0.2.0/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      267 2024-04-01 21:03:19.751887 plotly3d-0.2.0/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-01 21:03:19.752411 plotly3d-0.2.0/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-01 21:03:19.752960 plotly3d-0.2.0/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       20 2024-04-01 21:03:19.753485 plotly3d-0.2.0/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-01 21:03:19.754035 plotly3d-0.2.0/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-01 21:03:19.755798 plotly3d-0.2.0/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      400 2024-04-01 03:30:58.000000 plotly3d-0.2.0/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 03:00:25.039440 plotly3d-0.3.0/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.0/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-02 03:00:25.038833 plotly3d-0.3.0/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.0/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 03:00:25.034599 plotly3d-0.3.0/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.0/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9389 2024-04-02 02:58:01.000000 plotly3d-0.3.0/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 03:00:25.038269 plotly3d-0.3.0/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-02 03:00:24.000000 plotly3d-0.3.0/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-02 03:00:24.000000 plotly3d-0.3.0/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-02 03:00:24.000000 plotly3d-0.3.0/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-02 03:00:24.000000 plotly3d-0.3.0/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-02 03:00:24.000000 plotly3d-0.3.0/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-02 03:00:25.039617 plotly3d-0.3.0/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-02 02:59:21.000000 plotly3d-0.3.0/setup.py
```

### Comparing `plotly3d-0.2.0/LICENSE` & `plotly3d-0.3.0/LICENSE`

 * *Files identical despite different names*

