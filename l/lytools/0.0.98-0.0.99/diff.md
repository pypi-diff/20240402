# Comparing `tmp/lytools-0.0.98.tar.gz` & `tmp/lytools-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytools-0.0.98.tar", last modified: Thu Oct 12 12:57:20 2023, max compression
+gzip compressed data, was "lytools-0.0.99.tar", last modified: Fri Oct 27 13:40:35 2023, max compression
```

## Comparing `lytools-0.0.98.tar` & `lytools-0.0.99.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 liyang     (501) staff       (20)        0 2023-10-12 12:57:20.595340 lytools-0.0.98/
--rw-r--r--   0 liyang     (501) staff       (20)     1063 2022-11-11 17:55:32.000000 lytools-0.0.98/LICENSE
--rw-r--r--   0 liyang     (501) staff       (20)      319 2023-10-12 12:57:20.595203 lytools-0.0.98/PKG-INFO
--rw-r--r--   0 liyang     (501) staff       (20)       81 2022-11-28 04:33:42.000000 lytools-0.0.98/README.md
-drwxr-xr-x   0 liyang     (501) staff       (20)        0 2023-10-12 12:57:20.593711 lytools-0.0.98/lytools/
--rw-r--r--   0 liyang     (501) staff       (20)      288 2023-10-12 12:57:20.000000 lytools-0.0.98/lytools/__init__.py
--rw-r--r--   0 liyang     (501) staff       (20)   166523 2023-10-12 12:55:40.000000 lytools-0.0.98/lytools/_lytools.py
-drwxr-xr-x   0 liyang     (501) staff       (20)        0 2023-10-12 12:57:20.595037 lytools-0.0.98/lytools.egg-info/
--rw-r--r--   0 liyang     (501) staff       (20)      319 2023-10-12 12:57:20.000000 lytools-0.0.98/lytools.egg-info/PKG-INFO
--rw-r--r--   0 liyang     (501) staff       (20)      220 2023-10-12 12:57:20.000000 lytools-0.0.98/lytools.egg-info/SOURCES.txt
--rw-r--r--   0 liyang     (501) staff       (20)        1 2023-10-12 12:57:20.000000 lytools-0.0.98/lytools.egg-info/dependency_links.txt
--rw-r--r--   0 liyang     (501) staff       (20)       87 2023-10-12 12:57:20.000000 lytools-0.0.98/lytools.egg-info/requires.txt
--rw-r--r--   0 liyang     (501) staff       (20)        8 2023-10-12 12:57:20.000000 lytools-0.0.98/lytools.egg-info/top_level.txt
--rw-r--r--   0 liyang     (501) staff       (20)       38 2023-10-12 12:57:20.595379 lytools-0.0.98/setup.cfg
--rw-r--r--   0 liyang     (501) staff       (20)      593 2023-10-12 12:57:20.000000 lytools-0.0.98/setup.py
+drwxr-xr-x   0 liyang     (501) staff       (20)        0 2023-10-27 13:40:35.571576 lytools-0.0.99/
+-rw-r--r--   0 liyang     (501) staff       (20)     1063 2022-11-11 17:55:32.000000 lytools-0.0.99/LICENSE
+-rw-r--r--   0 liyang     (501) staff       (20)      319 2023-10-27 13:40:35.571420 lytools-0.0.99/PKG-INFO
+-rw-r--r--   0 liyang     (501) staff       (20)       81 2022-11-28 04:33:42.000000 lytools-0.0.99/README.md
+drwxr-xr-x   0 liyang     (501) staff       (20)        0 2023-10-27 13:40:35.570051 lytools-0.0.99/lytools/
+-rw-r--r--   0 liyang     (501) staff       (20)      288 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools/__init__.py
+-rw-r--r--   0 liyang     (501) staff       (20)   166524 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools/_lytools.py
+drwxr-xr-x   0 liyang     (501) staff       (20)        0 2023-10-27 13:40:35.571193 lytools-0.0.99/lytools.egg-info/
+-rw-r--r--   0 liyang     (501) staff       (20)      319 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools.egg-info/PKG-INFO
+-rw-r--r--   0 liyang     (501) staff       (20)      220 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools.egg-info/SOURCES.txt
+-rw-r--r--   0 liyang     (501) staff       (20)        1 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools.egg-info/dependency_links.txt
+-rw-r--r--   0 liyang     (501) staff       (20)       87 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools.egg-info/requires.txt
+-rw-r--r--   0 liyang     (501) staff       (20)        8 2023-10-27 13:40:35.000000 lytools-0.0.99/lytools.egg-info/top_level.txt
+-rw-r--r--   0 liyang     (501) staff       (20)       38 2023-10-27 13:40:35.571637 lytools-0.0.99/setup.cfg
+-rw-r--r--   0 liyang     (501) staff       (20)      593 2023-10-27 13:40:35.000000 lytools-0.0.99/setup.py
```

### Comparing `lytools-0.0.98/LICENSE` & `lytools-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `lytools-0.0.98/lytools/_lytools.py` & `lytools-0.0.99/lytools/_lytools.py`

 * *Files 1% similar despite different names*

```diff
@@ -3770,38 +3770,37 @@
         polys = m.fillcontinents(color='#B1B0B1', lake_color='#EFEFEF')
         for poly in polys:
             poly.set_clip_path(clip_circle.get_path(), clip_circle.get_transform())
         if is_plot_colorbar:
             cbar = plt.colorbar(ret, ax=ax, shrink=0.5, location='bottom', pad=0.0)
         return m, ret
 
-    def plot_ortho_significance_scatter(self, m, fpath_p, temp_root, sig_level=0.05, ax=None, linewidths=0.5, s=20,
+    def plot_Robinson_significance_scatter(self, m, fpath_p, temp_root, sig_level=0.05, ax=None, linewidths=0.5, s=20,
                                         c='k', marker='x',
                                         zorder=100, res=2):
+
         fpath_clip = fpath_p + 'clip.tif'
-        fpath_spatial_dict = DIC_and_TIF().spatial_tif_to_dic(fpath_p)
+        fpath_spatial_dict = DIC_and_TIF(tif_template=fpath_p).spatial_tif_to_dic(fpath_p)
         D_clip = DIC_and_TIF(tif_template=fpath_p)
         D_clip_lon_lat_pix_dict = D_clip.spatial_tif_to_lon_lat_dic(temp_root)
         fpath_clip_spatial_dict_clipped = {}
         for pix in fpath_spatial_dict:
             lon, lat = D_clip_lon_lat_pix_dict[pix]
-            if lat <= 30 + res:
-                continue
             fpath_clip_spatial_dict_clipped[pix] = fpath_spatial_dict[pix]
-        DIC_and_TIF().pix_dic_to_tif(fpath_clip_spatial_dict_clipped, fpath_clip)
+        DIC_and_TIF(tif_template=fpath_p).pix_dic_to_tif(fpath_clip_spatial_dict_clipped, fpath_clip)
         fpath_resample = fpath_clip + 'resample.tif'
         ToRaster().resample_reproj(fpath_clip, fpath_resample, res=res)
-        fpath_resample_ortho = fpath_resample + 'ortho.tif'
-        self.ortho_reproj(fpath_resample, fpath_resample_ortho, res=res * 100000)
+        fpath_resample_ortho = fpath_resample + 'Robinson.tif'
+        self.Robinson_reproj(fpath_resample, fpath_resample_ortho, res=res * 10000)
         arr, originX, originY, pixelWidth, pixelHeight = ToRaster().raster2array(fpath_resample_ortho)
 
         arr = Tools().mask_999999_arr(arr, warning=False)
         arr[arr > sig_level] = np.nan
         D_resample = DIC_and_TIF(tif_template=fpath_resample_ortho)
-
+        #
         os.remove(fpath_clip)
         os.remove(fpath_resample_ortho)
         os.remove(fpath_resample)
 
         spatial_dict = D_resample.spatial_arr_to_dic(arr)
         lon_lat_pix_dict = D_resample.spatial_tif_to_lon_lat_dic(temp_root)
```

### Comparing `lytools-0.0.98/setup.py` & `lytools-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding='utf-8'
 
 from setuptools import setup
 long_description = open('README.md').read()
 setup(
     name='lytools',
-    version='0.0.98',
+    version='0.0.99',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Yang Li',
     author_email='leeyang1991@gmail.com',
     packages=['lytools'],
     url='https://github.com/leeyang1991/lytools',
     python_requires='>=3',
```

