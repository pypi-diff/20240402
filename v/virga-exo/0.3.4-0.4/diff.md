# Comparing `tmp/virga-exo-0.3.4.tar.gz` & `tmp/virga-exo-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/virga-exo-0.3.4.tar", last modified: Sat Dec 11 01:27:01 2021, max compression
+gzip compressed data, was "virga-exo-0.4.tar", last modified: Tue Apr  2 05:54:21 2024, max compression
```

## Comparing `virga-exo-0.3.4.tar` & `virga-exo-0.4.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2021-12-11 01:27:01.000000 virga-exo-0.3.4/
--rw-r--r--   0 nbatalh1   (503) staff       (20)      706 2021-12-11 01:27:01.000000 virga-exo-0.3.4/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)      321 2020-04-22 00:32:37.000000 virga-exo-0.3.4/README.rst
--rw-r--r--   0 nbatalh1   (503) staff       (20)       38 2021-12-11 01:27:01.000000 virga-exo-0.3.4/setup.cfg
--rw-r--r--   0 nbatalh1   (503) staff       (20)     3095 2021-12-11 01:09:34.000000 virga-exo-0.3.4/setup.py
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga/
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)      261 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/__init__.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    17860 2020-02-01 00:56:36.000000 virga-exo-0.3.4/virga/calc_mie.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     2952 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/cloudy_retrieval.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    13526 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/compare_plots.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    18398 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/direct_mmr_solver.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    10584 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/gas_properties.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    65909 2021-12-11 00:46:46.000000 virga-exo-0.3.4/virga/justdoit.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    25425 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/justplotit.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     2830 2020-01-30 05:56:47.000000 virga-exo-0.3.4/virga/optics.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     8893 2021-08-11 06:47:51.000000 virga-exo-0.3.4/virga/pvaps.py
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga/reference/
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/reference/__init__.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    14244 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/root_functions.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     6708 2021-08-24 21:22:36.000000 virga-exo-0.3.4/virga/run_virga.py
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga_exo.egg-info/
--rw-r--r--   0 nbatalh1   (503) staff       (20)      706 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga_exo.egg-info/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)      491 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga_exo.egg-info/SOURCES.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga_exo.egg-info/dependency_links.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2020-04-21 22:13:16.000000 virga-exo-0.3.4/virga_exo.egg-info/not-zip-safe
--rw-r--r--   0 nbatalh1   (503) staff       (20)       61 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga_exo.egg-info/requires.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        6 2021-12-11 01:27:01.000000 virga-exo-0.3.4/virga_exo.egg-info/top_level.txt
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 05:54:21.105039 virga-exo-0.4/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      855 2024-04-02 05:54:21.104216 virga-exo-0.4/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      321 2020-04-22 00:32:37.000000 virga-exo-0.4/README.rst
+-rw-r--r--   0 nbatalh1   (503) staff       (20)       38 2024-04-02 05:54:21.105236 virga-exo-0.4/setup.cfg
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     3093 2024-04-02 05:52:22.000000 virga-exo-0.4/setup.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 05:54:21.093900 virga-exo-0.4/virga/
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)      261 2022-02-05 02:08:04.000000 virga-exo-0.4/virga/__init__.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    17860 2020-02-01 00:56:36.000000 virga-exo-0.4/virga/calc_mie.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     2952 2022-02-05 02:08:04.000000 virga-exo-0.4/virga/cloudy_retrieval.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    13376 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/compare_plots.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    18398 2021-08-24 21:22:36.000000 virga-exo-0.4/virga/direct_mmr_solver.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    15436 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/gas_properties.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    19875 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/ior_factory.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    76788 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/justdoit.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    26699 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/justplotit.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     2818 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/optics.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    16351 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/pvaps.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 05:54:21.098241 virga-exo-0.4/virga/reference/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     1192 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/reference/196.csv
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2022-02-05 02:08:04.000000 virga-exo-0.4/virga/reference/__init__.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    12120 2021-08-24 21:22:36.000000 virga-exo-0.4/virga/reference/hj.pt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     3413 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/reference/particle_sizes.csv
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     5934 2021-08-24 21:22:36.000000 virga-exo-0.4/virga/reference/t1000g100nc_m0.0.dat
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    18429 2024-04-02 05:52:22.000000 virga-exo-0.4/virga/root_functions.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     6708 2022-02-05 02:08:04.000000 virga-exo-0.4/virga/run_virga.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 05:54:21.103191 virga-exo-0.4/virga_exo.egg-info/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      855 2024-04-02 05:54:20.000000 virga-exo-0.4/virga_exo.egg-info/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      630 2024-04-02 05:54:20.000000 virga-exo-0.4/virga_exo.egg-info/SOURCES.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2024-04-02 05:54:20.000000 virga-exo-0.4/virga_exo.egg-info/dependency_links.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2023-03-18 00:33:59.000000 virga-exo-0.4/virga_exo.egg-info/not-zip-safe
+-rw-r--r--   0 nbatalh1   (503) staff       (20)       61 2024-04-02 05:54:20.000000 virga-exo-0.4/virga_exo.egg-info/requires.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        6 2024-04-02 05:54:20.000000 virga-exo-0.4/virga_exo.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `virga-exo-0.3.4/PKG-INFO` & `virga-exo-0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: virga-exo
-Version: 0.3.4
+Version: 0.4
 Summary: exoplanet code for compute cloud structure
 Home-page: https://natashabatalha.github.io/virga
+Download-URL: https://github.com/natashabatalha/virga
 Author: Natasha E. Batalha
 Author-email: natasha.e.batalha@gmail.com
 License: GPL-3.0
-Download-URL: https://github.com/natashabatalha/virga
-Description: README.rst
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: bokeh
+Requires-Dist: joblib
+Requires-Dist: photutils
+Requires-Dist: astropy
+Requires-Dist: scipy
+Requires-Dist: PyMieScatt
+
+README.rst
```

### Comparing `virga-exo-0.3.4/setup.py` & `virga-exo-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # from the setup.cfg file.
 #
 # use_2to3 and zip_safe are common options support by setuptools; these can
 # also be placed in the setup.cfg, as will be demonstrated in a future update
 # to this sample package.
 setup(
     name='virga-exo', 
-    version = '0.3.4',
+    version = '0.4',
     description = 'exoplanet code for compute cloud structure',
     long_description = 'README.rst',
     author = 'Natasha E. Batalha',
     author_email = 'natasha.e.batalha@gmail.com',
     url = 'https://natashabatalha.github.io/virga',
     license = 'GPL-3.0',
     download_url = 'https://github.com/natashabatalha/virga',
```

### Comparing `virga-exo-0.3.4/virga/calc_mie.py` & `virga-exo-0.4/virga/calc_mie.py`

 * *Files identical despite different names*

### Comparing `virga-exo-0.3.4/virga/cloudy_retrieval.py` & `virga-exo-0.4/virga/cloudy_retrieval.py`

 * *Files identical despite different names*

### Comparing `virga-exo-0.3.4/virga/compare_plots.py` & `virga-exo-0.4/virga/compare_plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import astropy.units as u
 import numpy as np
 
 from . import justdoit as pyeddy
 
 def plot_pt(out, labels, lines, **kwargs):
 
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',600)
+    kwargs['height'] = kwargs.get('height',300)
+    kwargs['width'] = kwargs.get('width',600)
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','Temperature (K)')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     
 
     cols = viridis(len(out))
@@ -38,16 +38,16 @@
         fig.line(temperature, pressure, legend_label=labels[i], color=cols[i],line_width=5, line_dash=lines[i])
 
     plot_format(fig)
     return fig
 
 def plot_cumsum(out,labels,lines,**kwargs):
 
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',600)
+    kwargs['height'] = kwargs.get('height',300)
+    kwargs['width'] = kwargs.get('width',600)
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
 
     cols = viridis(len(out))
     pressure = out[0]['pressure']
     kwargs['y_range'] = kwargs.get('y_range',[np.max(pressure), np.min(pressure)])
@@ -62,16 +62,16 @@
     plot_format(fig)
     return fig
 
 def plot_output(out,attribute,attribute_label,gas,labels,lines,legend_on=True,
                     color_indx=0,**kwargs):
 
     condensibles = out[0]['condensibles']
-    kwargs['plot_height'] = kwargs.get('plot_height',400)
-    kwargs['plot_width'] = kwargs.get('plot_width',350)
+    kwargs['height'] = kwargs.get('height',400)
+    kwargs['width'] = kwargs.get('width',350)
     kwargs['x_axis_label'] = kwargs.get('x_axis_label',attribute_label)
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     kwargs['x_range'] = kwargs.get('x_range', [1e-2, 1e4])
 
     cols = viridis(len(out))
@@ -104,16 +104,16 @@
         Dictionary output from pyeddy run
     color : method
         Method from bokeh.palletes. e.g. bokeh.palletes.virids, bokeh.palletes.magma
     **kwargs : kwargs 
         Kwargs for bokeh.figure() 
     """
 
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',400)
+    kwargs['height'] = kwargs.get('height',300)
+    kwargs['width'] = kwargs.get('width',400)
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','Column Optical Depth')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')    
 
     ngas = len(out['condensibles'])
     temperature = out['temperature']
@@ -142,16 +142,16 @@
         Dictionary output from pyeddy run
     color : method
         Method from bokeh.palletes. e.g. bokeh.palletes.virids, bokeh.palletes.magma
     **kwargs : kwargs 
         Kwargs for bokeh.figure() 
     """
 
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',400)
+    kwargs['height'] = kwargs.get('height',300)
+    kwargs['width'] = kwargs.get('width',400)
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','Condensate MMR')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')    
 
     ngas = len(out[0]['condensibles'])
     temperature = out['temperature']
@@ -202,15 +202,15 @@
 
     #PLOT W0
     scat01 = np.flip(np.reshape(dat01['w0'].values,(nlayer,nwno)),0)
     xr, yr = scat01.shape
     f01a = figure(x_range=[0, yr], y_range=[0,xr],
                            x_axis_label=wavelength_label, y_axis_label=pressure_label,
                            title="Single Scattering Albedo",
-                          plot_width=300, plot_height=300)
+                          width=300, height=300)
 
 
     f01a.image(image=[scat01],  color_mapper=color_mapper, x=0,y=0,dh=xr,dw =yr )
 
     color_bar = ColorBar(color_mapper=color_mapper, #ticker=LogTicker(),
                        label_standoff=12, border_line_color=None, location=(0,0))
 
@@ -224,15 +224,15 @@
     cols = colfun2(200)[::-1]
     color_mapper = LogColorMapper(palette=cols, low=1e-3, high=10)
 
 
     f01 = figure(x_range=[0, yr], y_range=[0,xr],
                            x_axis_label=wavelength_label, y_axis_label=pressure_label,
                            title="Cloud Optical Depth Per Layer",
-                          plot_width=320, plot_height=300)
+                          width=320, height=300)
 
     f01.image(image=[scat01],  color_mapper=color_mapper, x=0,y=0,dh=xr,dw =yr )
 
     color_bar = ColorBar(color_mapper=color_mapper, ticker=LogTicker(),
                        label_standoff=12, border_line_color=None, location=(0,0))
     f01.add_layout(color_bar, 'left')
 
@@ -243,15 +243,15 @@
     cols = colfun3(200)[::-1]
     color_mapper = LinearColorMapper(palette=cols, low=0, high=1)
 
 
     f01b = figure(x_range=[0, yr], y_range=[0,xr],
                            x_axis_label=wavelength_label, y_axis_label=pressure_label,
                            title="Assymetry Parameter",
-                          plot_width=300, plot_height=300)
+                          width=300, height=300)
 
     f01b.image(image=[scat01],  color_mapper=color_mapper, x=0,y=0,dh=xr,dw =yr )
 
     color_bar = ColorBar(color_mapper=color_mapper, ticker=BasicTicker(),
                        label_standoff=12, border_line_color=None, location=(0,0))
     f01b.add_layout(color_bar, 'left')
 
@@ -303,16 +303,16 @@
     df.yaxis.major_label_text_font='times'
     df.xaxis.axis_label_text_font_style = 'bold'
     df.yaxis.axis_label_text_font_style = 'bold'
 
 
 def plot_fsed(out,labels,y_axis='pressure',color_indx=0,cld_bounds=False,gas_indx=None,**kwargs):
 
-    kwargs['plot_height'] = kwargs.get('plot_height',400)
-    kwargs['plot_width'] = kwargs.get('plot_width',700)
+    kwargs['height'] = kwargs.get('height',400)
+    kwargs['width'] = kwargs.get('width',700)
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','fsed')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     #kwargs['x_range'] = kwargs.get('x_range', [1e-2, 2e1])
     if gas_indx is not None:
         title = 'Condensible = ' + str(out[0]['condensibles'][gas_indx])
```

### Comparing `virga-exo-0.3.4/virga/direct_mmr_solver.py` & `virga-exo-0.4/virga/direct_mmr_solver.py`

 * *Files identical despite different names*

### Comparing `virga-exo-0.3.4/virga/justdoit.py` & `virga-exo-0.4/virga/justdoit.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,24 +74,25 @@
     
     #### First we need to either grab or compute Mie coefficients #### 
     for i, igas in zip(range(ngas),condensibles) : 
 
         #Get gas properties including gas mean molecular weight,
         #gas mixing ratio, and the density
         run_gas = getattr(gas_properties, igas)
-        gas_mw[i], gas_mmr[i], rho_p[i] = run_gas(mmw, mh=mh, gas_mmr=atmo.gas_mmr)
+        gas_mw[i], gas_mmr[i], rho_p[i] = run_gas(mmw, mh=mh, gas_mmr=atmo.gas_mmr[igas])
 
         #Get mie files that are already saved in 
         #directory
         #eventually we will replace this with nice database 
         qext_gas, qscat_gas, cos_qscat_gas, nwave, radius,wave_in = get_mie(igas,directory)
 
         if i==0: 
             nradii = len(radius)
             rmin = np.min(radius)
+
             radius, rup, dr = get_r_grid(rmin, n_radii=nradii)
             qext = np.zeros((nwave,nradii,ngas))
             qscat = np.zeros((nwave,nradii,ngas))
             cos_qscat = np.zeros((nwave,nradii,ngas))
 
         #add to master matrix that contains the per gas Mie stuff
         qext[:,:,i], qscat[:,:,i], cos_qscat[:,:,i] = qext_gas, qscat_gas, cos_qscat_gas
@@ -184,15 +185,15 @@
         'mixing_length_unit':'cm',
         'kz':kz, 
         'kz_unit':'cm^2/s',
         'scale_height':scale_h,
         'cloud_deck':z_cld
     }
 
-def calc_optics(nwave, qc, qt, rg, reff, ndz,radius,dr,qext, qscat,cos_qscat,sig, rmin, nrad,verbose):
+def calc_optics(nwave, qc, qt, rg, reff, ndz,radius,dr,qext, qscat,cos_qscat,sig, rmin, nrad,verbose=False):
     """
     Calculate spectrally-resolved profiles of optical depth, single-scattering
     albedo, and asymmetry parameter.
 
     Parameters
     ----------
     nwave : int 
@@ -258,38 +259,59 @@
                     warning0 = f'Take caution in analyzing results. There have been a calculated particle radii off the Mie grid, which has a min radius of {rmin}cm and distribution of {sig}. The following errors:'
                     warning+='{0}cm for the {1}th gas at the {2}th grid point; '.format(str(rg[iz,igas]),str(igas),str(iz))
 
                 r2 = rg[iz,igas]**2 * np.exp( 2*np.log( sig)**2 )
                 opd_layer[iz,igas] = 2.*PI*r2*ndz[iz,igas]
 
                 #  Calculate normalization factor (forces lognormal sum = 1.0)
-                rsig = sig
+                rsig = sig #the log normal particle size distribution 
                 norm = 0.
                 for irad in range(nrad):
                     rr = radius[irad]
                     arg1 = dr[irad] / ( np.sqrt(2.*PI)*rr*np.log(rsig) )
                     arg2 = -np.log( rr/rg[iz,igas] )**2 / ( 2*np.log(rsig)**2 )
                     norm = norm + arg1*np.exp( arg2 )
                     #print (rr, rg[iz,igas],rsig,arg1,arg2)
 
                 # normalization
-                norm = ndz[iz,igas] / norm
+                norm = ndz[iz,igas] / norm #number density distribution
 
                 for irad in range(nrad):
                     rr = radius[irad]
-                    arg1 = dr[irad] / ( np.sqrt(2.*PI)*np.log(rsig) )
+                    arg1 = dr[irad] / ( np.sqrt(2.*PI)*np.log(rsig) ) # log normal distribution is the rsig
                     arg2 = -np.log( rr/rg[iz,igas] )**2 / ( 2*np.log(rsig)**2 )
                     pir2ndz = norm*PI*rr*arg1*np.exp( arg2 )         
                     for iwave in range(nwave): 
                         scat_gas[iz,iwave,igas] = scat_gas[iz,iwave,igas]+qscat[iwave,irad,igas]*pir2ndz
                         ext_gas[iz,iwave,igas] = ext_gas[iz,iwave,igas]+qext[iwave,irad,igas]*pir2ndz
                         cqs_gas[iz,iwave,igas] = cqs_gas[iz,iwave,igas]+cos_qscat[iwave,irad,igas]*pir2ndz
 
                     #TO DO ADD IN CLOUD SUBLAYER KLUGE LATER 
+    
+    for igas in range(ngas):
+        for iz in range(nz-1,-1,-1):
 
+            if np.sum(ext_gas[iz,:,igas]) > 0:
+                ibot = iz
+                break
+            if iz == 0:
+                ibot=0
+        #print(igas,ibot)
+        if ibot >= nz -2:
+            print("Not doing sublayer as cloud deck at the bottom of pressure grid")
+            
+        else:
+            opd_layer[ibot+1,igas] = opd_layer[ibot,igas]*0.1
+            scat_gas[ibot+1,:,igas] = scat_gas[ibot,:,igas]*0.1
+            ext_gas[ibot+1,:,igas] = ext_gas[ibot,:,igas]*0.1
+            cqs_gas[ibot+1,:,igas] = cqs_gas[ibot,:,igas]*0.1
+            opd_layer[ibot+2,igas] = opd_layer[ibot,igas]*0.05
+            scat_gas[ibot+2,:,igas] = scat_gas[ibot,:,igas]*0.05
+            ext_gas[ibot+2,:,igas] = ext_gas[ibot,:,igas]*0.05
+            cqs_gas[ibot+2,:,igas] = cqs_gas[ibot,:,igas]*0.05
     #Sum over gases and compute spectral optical depth profile etc
     for iz in range(nz):
         for iwave in range(nwave): 
             opd_scat = 0.
             opd_ext = 0.
             cos_qs = 0.
             for igas in range(ngas):
@@ -311,19 +333,115 @@
         opd_gas[0,igas] = opd_layer[0,igas]
 
         for iz in range(1,nz):
             opd_gas[iz,igas] = opd_gas[iz-1,igas] + opd_layer[iz,igas]
     if ((warning!='') & (verbose)): print(warning0+warning+' Turn off warnings by setting verbose=False.')
     return opd, w0, g0, opd_gas
 
+def calc_optics_user_r_dist(wave_in, ndz, 
+    radius, radius_unit, r_distribution, 
+    qext, qscat ,cos_qscat,  verbose=False):
+    """
+    Calculate spectrally-resolved profiles of optical depth, single-scattering
+    albedo, and asymmetry parameter for a user-input particle radius distribution
+
+    Parameters
+    ----------
+    wave_in : ndarray
+        your wavelength grid in microns
+    ndz : float
+        Column density of total particle concentration (#/cm^2) 
+            Note: set to whatever, it's your free knob 
+            ---- this does not directly translate to something physical because it's for all particles in your slab
+            May have to use values of 1e8 or so
+    radius : ndarray
+        Radius bin values - the range of particle sizes of interest. Maybe measured in the lab, 
+        Ensure radius_unit is specified 
+    radius_unit : astropy.unit.Units
+        Astropy compatible unit
+    qscat : ndarray
+        Scattering efficiency
+    qext : ndarray
+        Extinction efficiency
+    cos_qscat : ndarray
+        qscat-weighted <cos (scattering angle)>
+    r_distribution : ndarray
+        the radius distribution in each bin. Maybe measured from the lab, generated from microphysics, etc.
+        Should integrate to 1. 
+    verbose: bool 
+        print out warnings or not
+
+
+    Returns
+    -------
+    opd : ndarray 
+        extinction optical depth due to all condensates in layer
+    w0 : ndarray 
+        single scattering albedo
+    g0 : ndarray 
+        asymmetry parameter = Q_scat wtd avg of <cos theta>
+    """
+
+    radius = (radius*radius_unit).to(u.cm)
+    radius = radius.value
+    
+    wavenumber_grid = 1e4/wave_in
+    wavenumber_grid = np.array([item[0] for item in wavenumber_grid])
+    nwave = len(wavenumber_grid)
+    PI=np.pi
+    nrad = len(radius) ## where radius is the radius grid of the particle size distribution
+    
+    scat= np.zeros((nwave))
+    ext = np.zeros((nwave))
+    cqs = np.zeros((nwave))
+    
+    opd = np.zeros((nwave))
+    w0 = np.zeros((nwave))
+    g0 = np.zeros((nwave))
+    
+    opd_scat = 0.
+    opd_ext = 0.
+    cos_qs = 0.
+                    
+        #  Calculate normalization factor 
+    for irad in range(nrad):
+            rr = radius[irad] # the get the radius at each grid point, this is in nanometers 
+    
+            each_r_bin = ndz * (r_distribution[irad]) # weight the radius bin by the distribution 
+            pir2ndz = PI * rr**2 * each_r_bin # find the weighted cross section
+            
+            for iwave in range(nwave): 
+                scat[iwave] = scat[iwave] + qscat[iwave,irad]*pir2ndz 
+                ext[iwave] = ext[iwave] + qext[iwave,irad]*pir2ndz
+                cqs[iwave] = cqs[iwave] + cos_qscat[iwave,irad]*pir2ndz
+                
+                
+                    # calculate the spectral optical depth profile etc
+    for iwave in range(nwave): 
+            opd_scat = 0.
+            opd_ext = 0.
+            cos_qs = 0.
+            
+            opd_scat = opd_scat + scat[iwave]
+            opd_ext = opd_ext + ext[iwave]
+            cos_qs = cos_qs + cqs[iwave]
+   
+                    
+            if( opd_scat > 0. ):
+                            opd[iwave] = opd_ext 
+                            w0[iwave] = opd_scat / opd_ext
+                            g0[iwave] = cos_qs / opd_scat
+                    
+    return opd, w0, g0, wavenumber_grid
+
 def eddysed(t_top, p_top,t_mid, p_mid, condensibles, 
     gas_mw, gas_mmr,rho_p,mw_atmos,gravity, kz,mixl,
     fsed, b, eps, scale_h, z_top, z_alpha, z_min, param,
     mh,sig, rmin, nrad,d_molecule,eps_k,c_p_factor,
-    og_vfall=True,do_virtual=True, supsat=0, verbose=True):
+    og_vfall=True,do_virtual=True, supsat=0, verbose=False):
     """
     Given an atmosphere and condensates, calculate size and concentration
     of condensates in balance between eddy diffusion and sedimentation.
 
     Parameters
     ----------
     t_top : ndarray
@@ -428,15 +546,15 @@
         q_below = gas_mmr[i]
 
         #include decrease in condensate mixing ratio below model domain
         if do_virtual: 
             z_cld=None
             qvs_factor = (supsat+1)*gas_mw[i]/mw_atmos
             get_pvap = getattr(pvaps, igas)
-            if igas == 'Mg2SiO4':
+            if igas in ['Mg2SiO4','CaTiO3','CaAl12O19','FakeHaze','H2SO4','KhareHaze','SteamHaze300K','SteamHaze400K']:
                 pvap = get_pvap(t_bot, p_bot, mh=mh)
             else:
                 pvap = get_pvap(t_bot, mh=mh)
 
             qvs = qvs_factor*pvap/p_bot   
             if qvs <= q_below :   
 
@@ -809,43 +927,39 @@
     reff_layer : float
         droplet effective radius (second moment of size distrib, cm)
     ndz_layer : float 
         number column density of condensate (cm^-3)
     """
 
     get_pvap = getattr(pvaps, gas_name)
-    if gas_name == 'Mg2SiO4':
+    if gas_name in ['Mg2SiO4','CaTiO3','CaAl12O19','FakeHaze','H2SO4','KhareHaze','SteamHaze300K','SteamHaze400K']:
         pvap = get_pvap(t_layer, p_layer,mh=mh)
     else:
         pvap = get_pvap(t_layer,mh=mh)
 
     fs = supsat + 1 
 
     #   atmospheric density (g/cm^3)
     rho_atmos = p_layer / ( r_atmos * t_layer )    
 
     #   mass mixing ratio of saturated vapor (g/g)
     qvs = fs*pvap / ( (r_cloud) * t_layer ) / rho_atmos
 
     #   --------------------------------------------------------------------
-    #   Layer is cloud free
-
+    #   Layer is cloud free -neb-
     if( q_below < qvs ):
-
         qt_layer = q_below
         qt_top   = q_below
         qc_layer = 0.
         rg_layer = 0.
         reff_layer = 0.
         ndz_layer = 0.
         z_cld = z_cld
         fsed_mid = 0
-
     else:
-
         #   --------------------------------------------------------------------
         #   Cloudy layer: first calculate qt and qc at top of layer,
         #   then calculate layer averages
         if isinstance(z_cld,type(None)):
             z_cld = z_bot
         else:
             z_cld = z_cld
@@ -966,15 +1080,15 @@
         ndz_layer = (3*rho_atmos*qc_layer*dz_layer /
                     ( 4*np.pi*rho_p*rg_layer**3 ) * np.exp( -9*lnsig2 ))
 
     return qt_top, qc_layer,qt_layer, rg_layer,reff_layer,ndz_layer, z_cld, fsed_mid 
 
 class Atmosphere():
     def __init__(self,condensibles, fsed=0.5, b=1, eps=1e-2, mh=1, mmw=2.2, sig=2.0,
-                    param='const', verbose=True, supsat=0, gas_mmr=None):
+                    param='const', verbose=False, supsat=0, gas_mmr=None):
         """
         Parameters
         ----------
         condensibles : list of str
             list of gases for which to consider as cloud species 
         fsed : float 
             Sedimentation efficiency coefficient. Jupiter ~3-6. Hot Jupiters ~ 0.1-1.
@@ -1003,15 +1117,18 @@
         self.sig = sig
         self.param = param
         self.eps = eps
         self.verbose = verbose 
         #grab constants
         self.constants()
         self.supsat = supsat
-        self.gas_mmr = gas_mmr
+        if isinstance(gas_mmr, type(None)):
+            self.gas_mmr = {igas:None for igas in condensibles}
+        else: 
+            self.gas_mmr = gas_mmr
 
     def constants(self):
         #   Depth of the Lennard-Jones potential well for the atmosphere 
         # Used in the viscocity calculation (units are K) (Rosner, 2000)
         #   (78.6 for air, 71.4 for N2, 59.7 for H2)
         self.eps_k = 59.7
         #   diameter of atmospheric molecule (cm) (Rosner, 2000)
@@ -1066,15 +1183,15 @@
         Teff : float, optional
             Effective temperature. If None (default), Teff set to temperature at 1 bar
         alpha_pressure : float
             Pressure at which we want fsed=alpha for variable fsed calculation
         pd_kwargs : kwargs
             Pandas key words for file read in. 
             If reading old style eddysed files, you would need: 
-            skiprows=3, delim_whitespace=True, header=None, names=["ind","pressure","temperature","kz"]
+            skiprows=3, sep='\s+', header=None, names=["ind","pressure","temperature","kz"]
         """
         #first read in dataframe, dict or file and sort by pressure
         if not isinstance(df, type(None)):
             if isinstance(df, dict): df = pd.DataFrame(df)
             df = df.sort_values('pressure')
         elif not isinstance(filename, type(None)):
             df = pd.read_csv(filename, **pd_kwargs)
@@ -1361,34 +1478,33 @@
         opd, w0, g0
             Extinction per layer, single scattering abledo, asymmetry parameter, 
             All are ndarrays that are nlayer by nwave
         """
         run = compute(self, directory = directory, as_dict = as_dict)
         return run
 
-def calc_mie_db(gas_name, dir_refrind, dir_out, rmin = 1e-8, nradii = 60):
+def calc_mie_db(gas_name, dir_refrind, dir_out, rmin = 1e-8, rmax = 5.4239131e-2, nradii = 60,fort_calc_mie = False):
     """
     Function that calculations new Mie database using PyMieScatt. 
-
     Parameters
     ----------
     gas_name : list, str
         List of names of gasses. Or a single gas name. 
         See pyeddy.available() to see which ones are currently available. 
     dir_refrind : str 
         Directory where you store optical refractive index files that will be created. 
     dir_out: str 
         Directory where you want to store Mie parameter files. Will be stored as gas_name.Mieff. 
         BEWARE FILE OVERWRITES. 
     rmin : float , optional
-        (Default=1e-5) Units of cm. The minimum radius to compute Mie parameters for. 
+        (Default=1e-8) Units of cm. The minimum radius to compute Mie parameters for. 
         Usually 0.1 microns is small enough. However, if you notice your mean particle radius 
         is on the low end, you may compute your grid to even lower particle sizes. 
     nradii : int, optional
-        (Default=40) number of radii points to compute grid on. 40 grid points for exoplanets/BDs
+        (Default=60) number of radii points to compute grid on. 40 grid points for exoplanets/BDs
         is generally sufficient. 
 
     Returns 
     -------
     Q extinction, Q scattering,  asymmetry * Q scattering, radius grid (cm), wavelength grid (um)
 
     The Q "efficiency factors" are = cross section / geometric cross section of particle
@@ -1404,55 +1520,71 @@
         #files will be saved in `directory`
         # obtaining refractive index data for each gas
         wave_in,nn,kk = get_refrind(gas_name[i],dir_refrind)
         nwave = len(wave_in)
 
         if i==0:
             #all these files need to be on the same grid
-            radius, rup, dr = get_r_grid(r_min = rmin, n_radii = nradii)
+            #radius, rup, dr = get_r_grid(r_min = rmin, n_radii = nradii)
+            radius, rup, dr = get_r_grid_w_max(r_min=rmin, r_max=rmax, n_radii=nradii)
 
             qext_all=np.zeros(shape=(nwave,nradii,ngas))
             qscat_all = np.zeros(shape=(nwave,nradii,ngas))
             cos_qscat_all=np.zeros(shape=(nwave,nradii,ngas))
 
         #get extinction, scattering, and asymmetry
         #all of these are  [nwave by nradii]
-        qext_gas, qscat_gas, cos_qscat_gas = calc_new_mieff(wave_in, nn,kk, radius, rup, fort_calc_mie = False)
+        qext_gas, qscat_gas, cos_qscat_gas = calc_new_mieff(wave_in, nn,kk, radius, rup, fort_calc_mie = fort_calc_mie)
 
         #add to master matrix that contains the per gas Mie stuff
         qext_all[:,:,i], qscat_all[:,:,i], cos_qscat_all[:,:,i] = qext_gas, qscat_gas, cos_qscat_gas 
 
         #prepare format for old ass style
         wave = [nwave] + sum([[r]+list(wave_in) for r in radius],[])
         qscat = [nradii]  + sum([[np.nan]+list(iscat) for iscat in qscat_gas.T],[])
         qext = [np.nan]  + sum([[np.nan]+list(iext) for iext in qext_gas.T],[])
         cos_qscat = [np.nan]  + sum([[np.nan]+list(icos) for icos in cos_qscat_gas.T],[])
-
+        print(os.path.join(dir_out,gas_name[i]+".mieff"))
         pd.DataFrame({'wave':wave,'qscat':qscat,'qext':qext,'cos_qscat':cos_qscat}).to_csv(os.path.join(dir_out,gas_name[i]+".mieff"),
                                                                                    sep=' ',
                                                                                   index=False,header=None)
     return qext_all, qscat_all, cos_qscat_all, radius,wave_in
 
 def get_mie(gas, directory):
     """
     Get Mie parameters from old ass formatted files
     """
-    df = pd.read_csv(os.path.join(directory,gas+".mieff"),names=['wave','qscat','qext','cos_qscat'], delim_whitespace=True)
+    df = pd.read_csv(os.path.join(directory,gas+".mieff"),names=['wave','qscat','qext','cos_qscat'], sep='\s+')
 
     nwave = int( df.iloc[0,0])
     nradii = int(df.iloc[0,1])
 
     #get the radii (all the rows where there the last three rows are nans)
     radii = df.loc[np.isnan(df['qscat'])]['wave'].values
 
     df = df.dropna()
 
     assert len(radii) == nradii , "Number of radii specified in header is not the same as number of radii."
     assert nwave*nradii == df.shape[0] , "Number of wavelength specified in header is not the same as number of waves in file"
 
+    # check if incoming wavegrid is in correct order
+    sub_array = df['wave'].values[:196]  # Extract the first 196 values
+    is_ascending = np.all(np.diff(sub_array) >= 0) # check if going from short to long wavelength
+
+    if is_ascending == False:
+        flipped_wave = np.flip(df['wave'].values.reshape(nradii, -1, nwave), axis=2).flatten()
+        flipped_qscat = np.flip(df['qscat'].values.reshape(nradii, -1, nwave), axis=2).flatten()
+        flipped_qext = np.flip(df['qext'].values.reshape(nradii, -1, nwave), axis=2).flatten()
+        flipped_cos_qscat = np.flip(df['cos_qscat'].values.reshape(nradii, -1, nwave), axis=2).flatten()
+
+        df['wave'] = flipped_wave
+        df['qscat'] = flipped_qscat
+        df['qext'] = flipped_qext
+        df['cos_qscat'] = flipped_cos_qscat
+
     wave = df['wave'].values.reshape((nradii,nwave)).T
     qscat = df['qscat'].values.reshape((nradii,nwave)).T
     qext = df['qext'].values.reshape((nradii,nwave)).T
     cos_qscat = df['cos_qscat'].values.reshape((nradii,nwave)).T
 
     return qext,qscat, cos_qscat, nwave, radii,wave
 
@@ -1464,20 +1596,30 @@
 
     Parameters
     ----------
     igas : str 
         Gas name 
     directory : str 
         Directory were reference files are located. 
+
+    Returns
+    -------
+    wavelength, real part, imaginary part 
     """
     filename = os.path.join(directory ,igas+".refrind")
     #put skiprows=1 in loadtxt to skip first line
-    idummy, wave_in, nn, kk = np.loadtxt(open(filename,'rt').readlines(), unpack=True, usecols=[0,1,2,3])#[:-1]
-
-    return wave_in,nn,kk
+    try:
+        idummy, wave_in, nn, kk = np.loadtxt(open(filename,'rt').readlines(), unpack=True, usecols=[0,1,2,3])#[:-1]
+        return wave_in,nn,kk
+    except: 
+        df = pd.read_csv(filename)
+        wave_in = df['micron'].values 
+        nn = df['real'].values
+        kk = df['imaginary'].values
+        return wave_in,nn,kk
 
 def get_r_grid_w_max(r_min=1e-8, r_max=5.4239131e-2, n_radii=60):
     """
     Get spacing of radii to run Mie code
 
     r_min : float 
             Minimum radius to compute (cm)
@@ -1519,42 +1661,151 @@
     radius = r_min * vrat**(np.linspace(0,n_radii-1,n_radii)/3.)
     rup = f1*radius
     dr = f2*radius
 
     return radius, rup, dr
 
 
-def picaso_format(opd, w0, g0 ):
-    df = pd.DataFrame(index=[ i for i in range(opd.shape[0]*opd.shape[1])], columns=['lvl','w','opd','w0','g0'])
+def picaso_format(opd, w0, g0, pressure=None, wavenumber=None ):
+    """
+    Gets virga output to picaso format 
+
+    Parameters
+    ----------
+    opd : ndarray 
+        array from virga of extinction optical depths per layer 
+    w0 : ndarray 
+        array from virga of single scattering albedo 
+    g0 : ndarray
+        array from virga of asymmetry 
+    pressure : array 
+        pressure array in bars 
+    wavenumber: array 
+        wavenumber arry in cm^(-1)
+
+    """
+    df = pd.DataFrame(
+                dict(opd = opd.flatten(), 
+                     w0 = w0.flatten(), 
+                     g0 = g0.flatten()))
+                     
+    if not isinstance(pressure,type(None)):
+        df['pressure'] = np.concatenate([[i]*len(wavenumber) for i in pressure])
+    if  not isinstance(wavenumber,type(None)):
+        df['wavenumber'] = np.concatenate([wavenumber]*len(pressure))
+    return df
+
+def picaso_format_custom_wavenumber_grid(opd, w0, g0, wavenumber_grid ):
+    """
+    This is currently redundant with picaso_format now that picaso_format 
+    reads in wavenumber grid. 
+    Keeping for now, but will discontinue soon. 
+    """
+    df = pd.DataFrame(index=[ i for i in range(opd.shape[0]*opd.shape[1])], columns=['pressure','wavenumber','opd','w0','g0'])
     i = 0 
     LVL = []
     WV,OPD,WW0,GG0 =[],[],[],[]
     for j in range(opd.shape[0]):
            for w in range(opd.shape[1]):
-                LVL +=[j+1]
-                WV+=[w+1]
+                LVL+=[j+1]
+                WV+=[wavenumber_grid[w]]
                 OPD+=[opd[j,w]]
                 WW0+=[w0[j,w]]
                 GG0+=[g0[j,w]]
     df.iloc[:,0 ] = LVL
     df.iloc[:,1 ] = WV
     df.iloc[:,2 ] = OPD
     df.iloc[:,3 ] = WW0
     df.iloc[:,4 ] = GG0
     return df
 
+def picaso_format_slab(p_bottom,  opd, w0, g0, 
+    wavenumber_grid, pressure_grid ,p_top=None,p_decay=None):
+    """
+    Sets up a PICASO-readable dataframe that inserts a wavelength dependent aerosol layer at the user's 
+    given pressure bounds, i.e., a wavelength-dependent slab of clouds or haze.
+    
+    Parameters
+    ----------
+    p_bottom : float 
+        the cloud/haze base pressure
+        the upper bound of pressure (i.e., lower altitude bound) to set the aerosol layer. (Bars)
+    opd : ndarray
+        wavelength-dependent optical depth of the aerosol
+    w0 : ndarray
+        wavelength-dependent single scattering albedo of the aerosol
+    g0 : ndarray
+        asymmetry parameter = Q_scat wtd avg of <cos theta>
+    wavenumber_grid : ndarray
+        wavenumber grid in (cm^-1) 
+    pressure_grid : ndarray
+        bars, user-defined pressure grid for the model atmosphere
+    p_top : float
+         bars, the cloud/haze-top pressure
+         This cuts off the upper cloud region as a step function. 
+         You must specify either p_top or p_decay. 
+    p_decay : ndarray
+        noramlized to 1, unitless
+        array the same size as pressure_grid which specifies a 
+        height dependent optical depth. The usual format of p_decay is 
+        a fsed like exponential decay ~np.exp(-fsed*z/H)
+
+
+    Returns
+    -------
+    Dataframe of aerosol layer with pressure (in levels - non-physical units!), wavenumber, opd, w0, and g0 to be read by PICASO
+    """
+    if (isinstance(p_top, type(None)) & isinstance(p_decay, type(None))): 
+        raise Exception("Must specify cloud top pressure via p_top, or the vertical pressure decay via p_decay")
+    elif (isinstance(p_top, type(None)) & (~isinstance(p_decay, type(None)))): 
+        p_top = 1e-10#arbitarily small pressure to make sure float comparison doest break
+
+
+    df = pd.DataFrame(index=[ i for i in range(pressure_grid.shape[0]*opd.shape[0])], columns=['pressure','wavenumber','opd','w0','g0'])
+    i = 0 
+    LVL = []
+    WV,OPD,WW0,GG0 =[],[],[],[]
+    
+    # this loops the opd, w0, and g0 between p and dp bounds and put zeroes for them everywhere else
+    for j in range(pressure_grid.shape[0]):
+           for w in range(opd.shape[0]):
+                #stick in pressure bounds for the aerosol layer:
+                if p_top <= pressure_grid[j] <= p_bottom:
+                    LVL+=[j+1]
+                    WV+=[wavenumber_grid[w]]
+                    if isinstance(p_decay,type(None)):
+                        OPD+=[opd[w]]
+                    else: 
+                        OPD+=[p_decay[j]/np.max(p_decay)*opd[w]]
+                    WW0+=[w0[w]]
+                    GG0+=[g0[w]]
+                else:
+                    LVL+=[j+1]
+                    WV+=[wavenumber_grid[w]]
+                    OPD+=[opd[w]*0]
+                    WW0+=[w0[w]*0]
+                    GG0+=[g0[w]*0]       
+                    
+    df.iloc[:,0 ] = LVL
+    df.iloc[:,1 ] = WV
+    df.iloc[:,2 ] = OPD
+    df.iloc[:,3 ] = WW0
+    df.iloc[:,4 ] = GG0
+    return df
+
+
 def available():
     """
     Print all available gas condensates 
     """
     pvs = [i for i in dir(pvaps) if i != 'np' and '_' not in i]
     gas_p = [i for i in dir(gas_properties) if i != 'np' and '_' not in i]
     return list(np.intersect1d(gas_p, pvs))
 
-def recommend_gas(pressure, temperature, mh, mmw, plot=False, legend='inside',**plot_kwargs):
+def recommend_gas(pressure, temperature, mh, mmw, plot=False, returnplot = False, legend='inside', **plot_kwargs):
     """
     Recommends condensate species for a users calculation. 
 
     Parameters
     ----------
     pressure : ndarray, list
         Pressure grid for user's pressure-temperature profile. Unit=bars
@@ -1576,16 +1827,18 @@
         pressure (bars), condensation temperature (Kelvin)
     """    
     if plot: 
         from bokeh.plotting import figure, show
         from bokeh.models import Legend
         from bokeh.palettes import magma   
         plot_kwargs['y_range'] = plot_kwargs.get('y_range',[1e2,1e-3])
-        plot_kwargs['plot_height'] = plot_kwargs.get('plot_height',400)
-        plot_kwargs['plot_width'] = plot_kwargs.get('plot_width',600)
+        plot_kwargs['height'] = plot_kwargs.get('plot_height',plot_kwargs.get('height',400))
+        plot_kwargs['width'] = plot_kwargs.get('plot_width', plot_kwargs.get('width',600))
+        if 'plot_width' in plot_kwargs.keys() : plot_kwargs.pop('plot_width')
+        if 'plot_height' in plot_kwargs.keys() : plot_kwargs.pop('plot_height')
         plot_kwargs['x_axis_label'] = plot_kwargs.get('x_axis_label','Temperature (K)')
         plot_kwargs['y_axis_label'] = plot_kwargs.get('y_axis_label','Pressure (bars)')
         plot_kwargs['y_axis_type'] = plot_kwargs.get('y_axis_type','log')        
         fig = figure(**plot_kwargs)
 
     all_gases = available()
     cond_ts = []
@@ -1623,21 +1876,27 @@
                 f = fig.line(cond_ts[i],cond_p ,color=cols[i],line_width=line_widths[i])
                 legend_it.append((all_gases[i], [f]))
 
         if legend == 'outside':
             legend = Legend(items=legend_it, location=(0, 0))
             legend.click_policy="mute"
             fig.add_layout(legend, 'right')   
-        
+            
         plot_format(fig)
-        show(fig) 
+        
+        if returnplot:
+            return recommend, fig
+        else:
+            show(fig)
+    
+    return recommend
 
-    return recommend 
+    
 
-def condensation_t(gas_name, mh, mmw, pressure =  np.logspace(-6, 2, 20)):
+def condensation_t(gas_name, mh, mmw, pressure =  np.logspace(-6, 2, 20), gas_mmr=None):
     """
     Find condensation curve for any planet given a pressure. These are computed 
     based on pressure vapor curves defined in pvaps.py. 
 
     Default is to compute condensation temperature on a pressure grid 
 
     Parameters
@@ -1654,35 +1913,48 @@
         Default = np.logspace(-3,2,20)
 
     Returns
     -------
     ndarray, ndarray
         pressure (bars), condensation temperature (Kelvin)
     """
+
     if isinstance(pressure,(float,int)):
         pressure = [pressure]
     temps = []
     for p in pressure: 
         temp = optimize.root_scalar(find_cond_t, 
                         bracket=[10, 10000], method='brentq', 
-                        args=(p, mh, mmw, gas_name))
+                        args=(p, mh, mmw, gas_name, gas_mmr))
         temps += [temp.root]
     return np.array(pressure), np.array(temps)
 
 def hot_jupiter():
     directory = os.path.join(os.path.dirname(__file__), "reference",
                                    "hj.pt")
 
-    df = pd.read_csv(directory,delim_whitespace=True, usecols=[1,2,3],
+    df = pd.read_csv(directory,sep='\s+', usecols=[1,2,3],
                   names = ['pressure','temperature','kz'],skiprows=1)
     df.loc[df['pressure']>12.8,'temperature'] = np.linspace(1822,2100,df.loc[df['pressure']>12.8].shape[0])
     return df
 
 def brown_dwarf(): 
     directory = os.path.join(os.path.dirname(__file__), "reference",
                                    "t1000g100nc_m0.0.dat")
 
-    df  = pd.read_csv(directory,skiprows=1,delim_whitespace=True,
+    df  = pd.read_csv(directory,skiprows=1,sep='\s+',
                  header=None, usecols=[1,2,3],
                  names=['pressure','temperature','chf'])
     return df
 
+def warm_neptune(): 
+    directory = os.path.join(os.path.dirname(__file__), "reference",
+                                   "wn.pt")
+def temperate_neptune(): 
+    directory = os.path.join(os.path.dirname(__file__), "reference",
+                                   "temperate_neptune.pt")
+
+    df  = pd.read_csv(directory,skiprows=0,sep='\s+',
+                 header=None,
+                 names=['pressure','temperature','kz'])
+    return df
+
```

### Comparing `virga-exo-0.3.4/virga/justplotit.py` & `virga-exo-0.4/virga/justplotit.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bokeh.models import LinearColorMapper, LogTicker,BasicTicker, ColorBar,LogColorMapper,Legend
 from bokeh.palettes import magma as colfun1
 from bokeh.palettes import Colorblind8
 from bokeh.palettes import viridis as colfun2
 from bokeh.palettes import gray as colfun3
 from bokeh.palettes import Colorblind8
 import bokeh.palettes as colpals
+from bokeh.io import output_notebook 
 import astropy.units as u
 import numpy as np
 
 from . import justdoit as pyeddy
 
 def pt(out, with_condensation=True,return_condensation=False, **kwargs):
     """
@@ -34,17 +35,18 @@
         Kwargs for bokeh.figure() 
 
     Returns
     -------
     if return_condensation: fig, cond temperature curves, ,cond pressure grid , name of all available gases
     else: fig
     """
-
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',600)
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',600))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','Temperature (K)')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     
 
     ngas = len(out['condensibles'])
     temperature = out['temperature']
@@ -162,20 +164,22 @@
         dndr = {}
         for i in gas_name:
             dndr[i]= N[nl,gas_name.index(i)]/r/np.sqrt(2*np.pi)*np.log(sig)*np.exp(
                         - np.log(r/(r_g[nl,gas_name.index(i)]*1e-4))**2/(2*np.log(sig)**2)) #1e-4 is microns to cm
         dndr['r'] = r*1e4 #convert to microns
 
         if j==0:
-            p1 = figure(plot_width=p1w, plot_height=p1h, title="Select Pressure Level", 
+            p1 = figure(width=p1w, height=p1h, title="Select Pressure Level", 
                 x_axis_type='log',y_axis_type='log',y_axis_label='Pressure (bars)',x_axis_label='Mean Particle Radius (um)',
                 y_range=[np.max(pressure),np.min(pressure)])
 
-            p2 = figure(plot_width=p2w, plot_height=p2h, title="Particle Distribution at %.0e bars" %at_pressure,
-                         x_axis_type='log', y_axis_type='log', y_axis_label='dn/dr (cm-3)',x_axis_label='Particle Radius (um)')
+            p2 = figure(width=p2w, height=p2h, title="Particle Distribution at %.0e bars" %at_pressure,
+                         x_axis_type='log', y_axis_type='log', y_axis_label='dn/dr (cm-3)',
+                         x_axis_label='Particle Radius (um)', 
+                         y_range=[np.max([np.min(dndr[i]), 1e-50]), np.max(dndr[i])])
 
         #add to r_g for that plot 
         df_r_g['average'] = [pressure[nl]]*len(pressure)
         df_r_g['horizontal'] = np.linspace(np.amin(r_g[r_g>0]), np.amax(r_g) , len(pressure))
             
 
         s1 = ColumnDataSource(data=dict(df_r_g))
@@ -243,16 +247,18 @@
         Dictionary output from pyeddy run
     color : method
         Method from bokeh.palletes. e.g. bokeh.palletes.virids, bokeh.palletes.magma
     **kwargs : kwargs 
         Kwargs for bokeh.figure() 
     """
 
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',400)
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',400))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','Column Optical Depth')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')    
 
     if type(out)==dict:
         out=[out]
@@ -309,17 +315,18 @@
     out : dict 
         Dictionary output from pyeddy run
     color : method
         Method from bokeh.palletes. e.g. bokeh.palletes.virids, bokeh.palletes.magma
     **kwargs : kwargs 
         Kwargs for bokeh.figure() 
     """
-
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',400)
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',400))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','Condensate MMR')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')    
 
     if type(out)==dict:
         out=[out]
@@ -401,15 +408,15 @@
 
     #PLOT W0
     scat01 = np.flip(np.reshape(dat01['w0'].values,(nlayer,nwno)),0)
     xr, yr = scat01.shape
     f01a = figure(x_range=[0, yr], y_range=[0,xr],
                            x_axis_label=wavelength_label, y_axis_label=pressure_label,
                            title="Single Scattering Albedo",
-                          plot_width=300, plot_height=300)
+                          width=300, height=300)
 
 
     f01a.image(image=[scat01],  color_mapper=color_mapper, x=0,y=0,dh=xr,dw =yr )
 
     color_bar = ColorBar(color_mapper=color_mapper, #ticker=LogTicker(),
                        label_standoff=12, border_line_color=None, location=(0,0))
 
@@ -423,15 +430,15 @@
     cols = colfun2(200)[::-1]
     color_mapper = LogColorMapper(palette=cols, low=1e-3, high=10)
 
 
     f01 = figure(x_range=[0, yr], y_range=[0,xr],
                            x_axis_label=wavelength_label, y_axis_label=pressure_label,
                            title="Cloud Optical Depth Per Layer",
-                          plot_width=320, plot_height=300)
+                          width=320, height=300)
 
     f01.image(image=[scat01],  color_mapper=color_mapper, x=0,y=0,dh=xr,dw =yr )
 
     color_bar = ColorBar(color_mapper=color_mapper, ticker=LogTicker(),
                        label_standoff=12, border_line_color=None, location=(0,0))
     f01.add_layout(color_bar, 'left')
 
@@ -442,15 +449,15 @@
     cols = colfun3(200)[::-1]
     color_mapper = LinearColorMapper(palette=cols, low=0, high=1)
 
 
     f01b = figure(x_range=[0, yr], y_range=[0,xr],
                            x_axis_label=wavelength_label, y_axis_label=pressure_label,
                            title="Asymmetry Parameter",
-                          plot_width=300, plot_height=300)
+                          width=300, height=300)
 
     f01b.image(image=[scat01],  color_mapper=color_mapper, x=0,y=0,dh=xr,dw =yr )
 
     color_bar = ColorBar(color_mapper=color_mapper, ticker=BasicTicker(),
                        label_standoff=12, border_line_color=None, location=(0,0))
     f01b.add_layout(color_bar, 'left')
 
@@ -499,17 +506,18 @@
         Default is just to return a figure but you can also 
         return all the 1d profiles 
     legend : bool 
         Default is none. Legend for each component of out 
     **kwargs : keyword arguments
         Key word arguments will be supplied to each bokeh figure function
     """
-
-    kwargs['plot_height'] = kwargs.get('plot_height',300)
-    kwargs['plot_width'] = kwargs.get('plot_width',300)
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',300))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
 
     if not isinstance(out, list):
         out = [out]
 
     pressure = out[0]['pressure']
 
@@ -522,53 +530,57 @@
     opd = figure(x_axis_label='Optical Depth',y_axis_label='Pressure (bars)',
         x_axis_type='log',**kwargs)
 
     
     for i,results in enumerate(out): 
         inds = np.where((results['wave']>wave_range[0]) & 
             (results['wave']<wave_range[1]))
-
-        opd.line(np.mean(results['opd_per_layer'][:,inds],axis=2)[:,0], 
+        opd_dat = np.mean(results['opd_per_layer'][:,inds],axis=2)[:,0]
+        opd.line(opd_dat, 
                  results['pressure'], color=colors[np.mod(i, len(colors))],line_width=3)
-        
-        g0.line(np.mean(results['asymmetry'][:,inds],axis=2)[:,0], 
+        g0_dat = np.mean(results['asymmetry'][:,inds],axis=2)[:,0]
+        g0.line(g0_dat, 
                  results['pressure'], color=colors[np.mod(i, len(colors))],line_width=3)
         
         if isinstance(legend, type(None)):
-            ssa.line(np.mean(results['single_scattering'][:,inds],axis=2)[:,0], 
+            ssa_dat = np.mean(results['single_scattering'][:,inds],axis=2)[:,0]
+            ssa.line(ssa_dat, 
                  results['pressure'], color=colors[np.mod(i, len(colors))],line_width=3)
         else:
-            ssa.line(np.mean(results['single_scattering'][:,inds],axis=2)[:,0], 
+            ssa_dat = np.mean(results['single_scattering'][:,inds],axis=2)[:,0]
+            ssa.line(ssa_dat, 
                  results['pressure'], color=colors[np.mod(i, len(colors))],line_width=3,
                  legend_label=legend[i])
             ssa.legend.location='top_left'
 
     if return_output:   
-        return gridplot([[opd,ssa,g0]]), [opd,ssa,g0]
+        return gridplot([[opd,ssa,g0]]), [opd_dat,ssa_dat,g0_dat]
     else:   
         return gridplot([[opd,ssa,g0]])
 
 def find_nearest_1d(array,value):
     #small program to find the nearest neighbor in a matrix
     ar , iar ,ic = np.unique(array,return_index=True,return_counts=True)
     idx = (np.abs(ar-value)).argmin(axis=0)
     if ic[idx]>1: 
         idx = iar[idx] + (ic[idx]-1)
     else: 
         idx = iar[idx]
     return idx
 
-def pressure_fig(**plot_kwargs):
-    plot_kwargs['y_range'] = plot_kwargs.get('y_range',[1e2,1e-6])
-    plot_kwargs['plot_height'] = plot_kwargs.get('plot_height',400)
-    plot_kwargs['plot_width'] = plot_kwargs.get('plot_width',600)
-    plot_kwargs['x_axis_label'] = plot_kwargs.get('x_axis_label','Temperature (K)')
-    plot_kwargs['y_axis_label'] = plot_kwargs.get('y_axis_label','Pressure (bars)')
-    plot_kwargs['y_axis_type'] = plot_kwargs.get('y_axis_type','log')        
-    fig = figure(**plot_kwargs)
+def pressure_fig(**kwargs):
+    kwargs['y_range'] = kwargs.get('y_range',[1e2,1e-6])
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',400))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',600))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
+    kwargs['x_axis_label'] = kwargs.get('x_axis_label','Temperature (K)')
+    kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
+    kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')        
+    fig = figure(**kwargs)
     return fig
 
 def plot_format(df):
     """Function to reformat plots"""
     df.xaxis.axis_label_text_font='times'
     df.yaxis.axis_label_text_font='times'
     df.xaxis.major_label_text_font_size='14pt'
@@ -578,16 +590,18 @@
     df.xaxis.major_label_text_font='times'
     df.yaxis.major_label_text_font='times'
     df.xaxis.axis_label_text_font_style = 'bold'
     df.yaxis.axis_label_text_font_style = 'bold'
 
 def plot_fsed(pressure, z, scale_height, alpha, beta, epsilon=1e-2, pres_alpha=None, **kwargs):
 
-    kwargs['plot_height'] = kwargs.get('plot_height',400)
-    kwargs['plot_width'] = kwargs.get('plot_width',700)
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',700))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','fsed')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
 
     if type(alpha) is int:
         alpha = [alpha]
@@ -620,16 +634,18 @@
     return fig
 
 def fsed_from_output(out,labels,y_axis='pressure',color_indx=0,cld_bounds=False,gas_indx=None,**kwargs):
 
     if type(out)==dict:
         out=[out]
 
-    kwargs['plot_height'] = kwargs.get('plot_height',400)
-    kwargs['plot_width'] = kwargs.get('plot_width',700)
+    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',700))
+    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
     kwargs['x_axis_label'] = kwargs.get('x_axis_label','fsed')
     kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure (bars)')
     kwargs['x_axis_type'] = kwargs.get('x_axis_type','log')
     kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
     #kwargs['x_range'] = kwargs.get('x_range', [1e-2, 2e1])
     if gas_indx is not None:
         title = 'Condensible = ' + str(out[0]['condensibles'][gas_indx])
@@ -642,17 +658,17 @@
     fig = figure(**kwargs)
 
     min_id=[]; max_id=[]
     for i in range(len(out)):
         if gas_indx is None: x = out[i]['fsed']
         else: x = out[i]['fsed'][:,gas_indx]
 
-        if y_axis is 'pressure':
+        if y_axis == 'pressure':
             y = out[i]['pressure']
-        elif y_axis is 'z':
+        elif y_axis == 'z':
             y = out[i]['altitude']
         col = Colorblind8[np.mod(i+color_indx, 8)]
         fig.line(x, y, legend_label=labels[i], color=col, line_width=5)
         if cld_bounds and gas_indx is not None:
             low_clds = []; high_clds = []
             ndz = out[i]['column_density'][:,gas_indx]
             nonzero = np.where(ndz>1e-3)[0]
```

### Comparing `virga-exo-0.3.4/virga/optics.py` & `virga-exo-0.4/virga/optics.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 		Condensible name (e.g. Al2O3)
 
 	Returns
 	-------
 	micron_wave, nn, kk as ndarrays
 	"""
 	df = pd.read_csv(os.path.join(directory,condensible+'.refrind'),
-		skiprows=2, header=None,delim_whitespace=True,
+		skiprows=2, header=None,sep='\s+',
                 names=['i', 'wavelength', 'nn', 'kk'])
 	micron_wave=df['wavelength'].values
 	nn = df['nn'].values
 	kk = df['kk'].values
 	return micron_wave, nn, kk
```

### Comparing `virga-exo-0.3.4/virga/root_functions.py` & `virga-exo-0.4/virga/root_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,22 +39,22 @@
 
     Returns
     -------
     ad_qc : float 
         mixing ratio of condensed condensate (g/g)
     """
     #   All vapor in excess of saturation condenses
-    if param is 'const':
+    if param == 'const':
         ad_qc = np.max([ 0., qt - ad_qvs ])
 
         # Eqn. 7 in A & M 
         #   Difference from advective-diffusive balance 
         advdif = ad_qbelow*np.exp( - ad_rainf*ad_qc*ad_dz / ( qt*ad_mixl ) )
         #print(advdif, ad_qc, ad_dz ,ad_mixl,qt )
-    elif param is 'exp':
+    elif param == 'exp':
         fsed = ad_rainf; mixl = ad_mixl; z = ad_dz
         qc = (ad_qbelow - ad_qvs) * np.exp( - b * fsed / mixl * np.exp(zb/b) 
                             * (np.exp(z/b) -1) + eps*z/b)
         advdif = qc + ad_qvs
 
     advdif = advdif - qt
     return advdif
@@ -167,14 +167,127 @@
         #when Reynolds is greater than 1000, we can just use 
         #an asymptotic value that is independent of Reynolds number
         #Eqn. B3 from A&M 01
         vfall_r = beta_slip*np.sqrt( 8.*drho*r*grav / (3.*cdrag*rho_atmos) )
 
     return vfall_r 
 
+
+def vfall_aggregrates(r, grav, mw_atmos, t, p, rhop, D=2, Ragg=1):
+    """
+    Calculate fallspeed for a particle at one layer in an
+    atmosphere, assuming low Reynolds number and in the molecular regime (Epstein drag), 
+    i.e., where Knudsen number (mfp/r) is high (>>1). 
+
+    User chooses whether particle is spherical or an aggregate.
+    If aggregrate, the monomer size is given by r and the outer effective radius of the aggregrate is Ragg.
+    
+    all units are cgs
+    
+    Parameters
+    ----------
+    r : float
+        monomer particle radius (cm)
+    mw_atmos : float 
+        atmospheric molecular weight (g/mol)
+    t : float 
+        atmospheric temperature (K)
+    p  : float
+        atmospheric pressure (dyne/cm^2)
+    rhop : float 
+        density of particle (g/cm^3)
+    grav : float 
+        acceleration of gravity (cm/s^2)
+    Ragg : float
+        aggregate particle effective radius (cm). (Defaults to 1 for spherical monomers).
+    D : float
+        fractal number (Default is 2 because function reduces to monomers at this value).
+    """
+    R_GAS = 8.3143e7  #universial gas constant; cgs units cm3-bar/mole-K
+    k = 1.38e-16  #boltzmann contant in cgs units -  cm2 g s-2 K-1 (ergs/K)
+    
+    N_avo = 6.022e23
+    
+    mass = mw_atmos/N_avo 
+    
+    rho_atmos = (mw_atmos*p) / (R*t) #atmospheric density
+    drho = rhop - rho_atmos
+    v_thermal = np.sqrt((3*k*t)/mass) #root mean speed of the gas 
+    
+    #the stopping time of the particle
+    t_stop_epstein_r = (2.0/3.0) * (r*drho) / (rho_atmos*v_thermal) 
+    
+    vfall_epstein_agg_r = t_stop_epstein_r * grav * (Ragg/r)**(D-2)
+
+    return vfall_epstein_agg_r
+
+def vfall_aggregrates_ohno(r, grav,mw_atmos,mfp, t, p, rhop, ad_qc, D=2):
+    """
+    Calculates fallspeed for a fractal aggegrate particle as performed
+    by Ohno et al., 2020, with an outer 
+    effective radius of R_agg made up of monomers of size r, at one layer in an
+    atmosphere. ***Requires characteristic radius ragg to have D > or equal 2, i.e., not very fluffy aggregrates.
+
+    Essentially a more explicit version of the regular "vfall_aggregates" function, 
+    and is not dependent on being in free molecular (Esptein) regime
+    
+    all units are cgs
+    
+    Parameters
+    ----------
+    r : float
+        monomer particle radius (cm)
+    grav : float 
+        acceleration of gravity (cm/s^2)
+    rhop : float
+        density of aggregrate particle (g/cm^3)
+    t : float 
+        atmospheric temperature (K)
+    p  : float
+        atmospheric pressure (dyne/cm^2)
+    mw_atmos : float 
+        atmospheric molecular weight (g/mol)
+    mfp : float 
+        atmospheric molecular mean free path (cm)
+    ad_qc : float 
+        mixing ratio of condensed condensate (g/g)
+    D : float
+        fractal number (Default is 2).
+    gas_mw : float
+        condensate gas mean molecular weight (g/mol)
+    """
+    #Define some constants
+    R_GAS = 8.3143e7  #universial gas constant; cgs units cm3-bar/mole-K
+    k = 1.38e-16  #boltzmann contant in cgs units -  cm2 g s-2 K-1 (ergs/K)
+    N_avo = 6.022e23 #avogadro's number
+
+    #determine the number density of monomer particles
+    N = ad_qc * N_avo/ gas_mw
+
+    #calculate the aggregrate radius based on the fractal dimension, monomer radius, and number density of monomers
+    Ragg = r * N**(1/D) 
+
+    mass = mw_atmos/N_avo
+    rho_atmos = (mw_atmos*p) / (R*t) #atmospheric density
+    drho = rho_agg - rho_atmos
+
+    kn = mfp / Ragg #Knudsen number
+    beta = 1.0 + (1.26*kn) #Cunningham correction (slip factor for gas kinetic effects)
+    v_thermal = np.sqrt((8*k*t)/(mass*np.pi)) #thermal speed of the gas 
+
+    #visc = (1.0/3.0)*rho_atmos*v_thermal*mfp #viscosity of the atmosphere, appropriate for large Kn (Esptein)
+    visc = 5.877e-6 * np.sqrt(t) #in dyne/cm^2 with t in K (via Woitke & Helling 2003)
+
+    vfall_stokes = (2.0/9.0) * beta * grav * ((Ragg)**2) * (drho/visc) 
+    v_bracket = (1.0 + (((0.45/54.0) * (grav/((visc)**2)) * ((Ragg)**3) * rho_atmos * rho_agg)**(2./5.)))**(-5.0/4.0)
+    
+    vfall_r_ohno = vfall_stokes  * v_bracket
+   
+    return vfall_r_ohno
+
 def vfall_find_root(r, grav=None,mw_atmos=None,mfp=None,visc=None,
               t=None,p=None, rhop=None,w_convect=None ):
     """
     This is used to find F(X)-y=0 where F(X) is the fall speed for 
     a spherical particle and `y` is the convective velocity scale. 
     When the two are balanced we arrive at our correct particle radius.
 
@@ -283,17 +396,17 @@
     Returns
     ______
     soln.root : float
         the value of the parameter solve_for
     """
 
     def force_balance_new(u):
-        if solve_for is "vfall":
+        if solve_for == "vfall":
             return force_balance(u, temp, grav, mw_atmos, mfp, visc, t, p, rhop) 
-        elif solve_for is "rw":
+        elif solve_for == "rw":
             return force_balance(temp, u, grav, mw_atmos, mfp, visc, t, p, rhop) 
 
     soln = optimize.root_scalar(force_balance_new, bracket=[lo, hi], method='brentq') 
 
     return soln.root
 
 def qvs_below_model(p_test, qv_dtdlnp=None, qv_p=None, 
@@ -306,24 +419,24 @@
     """
     #  Extrapolate temperature lapse rate to test pressure
 
     t_test = qv_t + np.log( qv_p / p_test )*qv_dtdlnp
     
     #  Compute saturation mixing ratio
     get_pvap = getattr(pvaps, qv_gas_name)
-    if qv_gas_name == 'Mg2SiO4':
+    if qv_gas_name in ['Mg2SiO4','CaTiO3','CaAl12O19']:
         pvap_test = get_pvap(t_test, p_test, mh=mh)
     else:
         pvap_test = get_pvap(t_test,mh=mh)
 
     fx = qv_factor * pvap_test / p_test 
     return np.log(fx) - np.log(q_below)
 
 
-def find_cond_t(t_test, p_test = None, mh=None, mmw=None, gas_name=None):    
+def find_cond_t(t_test, p_test = None, mh=None, mmw=None, gas_name=None, gas_mmr=None):    
     """
     Root function used used to find condenstation temperature. E.g. 
     the temperature when  
 
     log p_vap = log partial pressure of gas 
 
     Parameters
@@ -338,17 +451,17 @@
         mean molecular weight (2.2 for solar)
     gas_name : str 
         gas name, case sensitive 
     """
     pvap_fun = getattr(pvaps, gas_name)
     gas_p_fun = getattr(gas_properties, gas_name)
     #get gas mixing ratio 
-    gas_mw, gas_mmr ,rho = gas_p_fun(mmw,mh=mh)
+    gas_mw, gas_mmr ,rho = gas_p_fun(mmw,mh=mh , gas_mmr=gas_mmr)
     #get vapor pressure and correct for masses of atmo and gas 
-    if gas_name == 'Mg2SiO4':
+    if gas_name in ['Mg2SiO4','CaTiO3','CaAl12O19']:
         pv = gas_mw/mmw*pvap_fun(t_test,p_test, mh=mh)/1e6 #dynes to bars 
     else:
         pv = gas_mw/mmw*pvap_fun(t_test, mh=mh)/1e6 #dynes to bars 
     #get partial pressure
     partial_p = gas_mmr*p_test*mh 
     if pv == 0:
         pv = 1e-30 #dummy small
```

### Comparing `virga-exo-0.3.4/virga/run_virga.py` & `virga-exo-0.4/virga/run_virga.py`

 * *Files identical despite different names*

### Comparing `virga-exo-0.3.4/virga_exo.egg-info/PKG-INFO` & `virga-exo-0.4/virga_exo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: virga-exo
-Version: 0.3.4
+Version: 0.4
 Summary: exoplanet code for compute cloud structure
 Home-page: https://natashabatalha.github.io/virga
+Download-URL: https://github.com/natashabatalha/virga
 Author: Natasha E. Batalha
 Author-email: natasha.e.batalha@gmail.com
 License: GPL-3.0
-Download-URL: https://github.com/natashabatalha/virga
-Description: README.rst
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: bokeh
+Requires-Dist: joblib
+Requires-Dist: photutils
+Requires-Dist: astropy
+Requires-Dist: scipy
+Requires-Dist: PyMieScatt
+
+README.rst
```

