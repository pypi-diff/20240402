# Comparing `tmp/glycogenius-1.1.7.tar.gz` & `tmp/glycogenius-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glycogenius-1.1.7.tar", last modified: Fri Mar 22 00:05:01 2024, max compression
+gzip compressed data, was "glycogenius-1.1.8.tar", last modified: Tue Apr  2 12:31:30 2024, max compression
```

## Comparing `glycogenius-1.1.7.tar` & `glycogenius-1.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 00:05:01.697632 glycogenius-1.1.7/
--rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     5066 2024-03-22 00:05:01.697632 glycogenius-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4405 2024-01-24 20:27:19.000000 glycogenius-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 00:05:01.672610 glycogenius-1.1.7/glycogenius/
--rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.7/glycogenius/LICENSE.py
-drwxrwxrwx   0        0        0        0 2024-03-22 00:05:01.695567 glycogenius-1.1.7/glycogenius/Modules/
--rw-rw-rw-   0        0        0    43397 2024-03-21 20:26:48.000000 glycogenius-1.1.7/glycogenius/Modules/CLI.py
--rw-rw-rw-   0        0        0    18987 2024-03-21 22:50:34.000000 glycogenius-1.1.7/glycogenius/Modules/Config_Handler.py
--rw-rw-rw-   0        0        0   158203 2024-03-21 19:46:16.000000 glycogenius-1.1.7/glycogenius/Modules/Execution_Functions.py
--rw-rw-rw-   0        0        0    40454 2024-03-22 00:04:25.000000 glycogenius-1.1.7/glycogenius/Modules/File_Accessing.py
--rw-rw-rw-   0        0        0    27663 2024-03-20 13:42:42.000000 glycogenius-1.1.7/glycogenius/Modules/General_Functions.py
--rw-rw-rw-   0        0        0    29531 2024-03-09 13:25:43.000000 glycogenius-1.1.7/glycogenius/Modules/Library_Tools.py
--rw-rw-rw-   0        0        0        0 2023-12-15 19:43:14.000000 glycogenius-1.1.7/glycogenius/Modules/__init__.py
--rw-rw-rw-   0        0        0     3698 2024-03-21 20:19:11.000000 glycogenius-1.1.7/glycogenius/Modules/core.py
--rw-rw-rw-   0        0        0    10163 2024-03-21 22:50:47.000000 glycogenius-1.1.7/glycogenius/Parameters_Template.py
--rw-rw-rw-   0        0        0       64 2023-12-24 14:08:40.000000 glycogenius-1.1.7/glycogenius/__init__.py
--rw-rw-rw-   0        0        0       69 2024-03-10 15:11:52.000000 glycogenius-1.1.7/glycogenius/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 00:05:01.696568 glycogenius-1.1.7/glycogenius.egg-info/
--rw-rw-rw-   0        0        0     5066 2024-03-22 00:05:01.000000 glycogenius-1.1.7/glycogenius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-03-22 00:05:01.000000 glycogenius-1.1.7/glycogenius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 00:05:01.000000 glycogenius-1.1.7/glycogenius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-22 00:05:01.000000 glycogenius-1.1.7/glycogenius.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-03-22 00:05:01.000000 glycogenius-1.1.7/glycogenius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-22 00:05:01.000000 glycogenius-1.1.7/glycogenius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 00:05:01.697632 glycogenius-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2038 2024-03-22 00:05:01.000000 glycogenius-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.469316 glycogenius-1.1.8/
+-rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     5066 2024-04-02 12:31:30.469316 glycogenius-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4405 2024-01-24 20:27:19.000000 glycogenius-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.444391 glycogenius-1.1.8/glycogenius/
+-rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.8/glycogenius/LICENSE.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.468303 glycogenius-1.1.8/glycogenius/Modules/
+-rw-rw-rw-   0        0        0    43400 2024-04-01 13:11:42.000000 glycogenius-1.1.8/glycogenius/Modules/CLI.py
+-rw-rw-rw-   0        0        0    19461 2024-04-01 13:33:48.000000 glycogenius-1.1.8/glycogenius/Modules/Config_Handler.py
+-rw-rw-rw-   0        0        0   159861 2024-04-01 18:12:43.000000 glycogenius-1.1.8/glycogenius/Modules/Execution_Functions.py
+-rw-rw-rw-   0        0        0    42498 2024-04-01 01:34:38.000000 glycogenius-1.1.8/glycogenius/Modules/File_Accessing.py
+-rw-rw-rw-   0        0        0    27665 2024-03-25 13:41:16.000000 glycogenius-1.1.8/glycogenius/Modules/General_Functions.py
+-rw-rw-rw-   0        0        0    30178 2024-03-31 01:55:59.000000 glycogenius-1.1.8/glycogenius/Modules/Library_Tools.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 19:43:14.000000 glycogenius-1.1.8/glycogenius/Modules/__init__.py
+-rw-rw-rw-   0        0        0     3667 2024-03-25 20:18:12.000000 glycogenius-1.1.8/glycogenius/Modules/core.py
+-rw-rw-rw-   0        0        0    10155 2024-04-01 13:10:33.000000 glycogenius-1.1.8/glycogenius/Parameters_Template.py
+-rw-rw-rw-   0        0        0       64 2024-03-23 12:11:11.000000 glycogenius-1.1.8/glycogenius/__init__.py
+-rw-rw-rw-   0        0        0       69 2024-03-22 21:56:00.000000 glycogenius-1.1.8/glycogenius/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.468303 glycogenius-1.1.8/glycogenius.egg-info/
+-rw-rw-rw-   0        0        0     5066 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:31:30.470314 glycogenius-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2038 2024-04-02 12:31:29.000000 glycogenius-1.1.8/setup.py
```

### Comparing `glycogenius-1.1.7/LICENSE` & `glycogenius-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.7/PKG-INFO` & `glycogenius-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glycogenius
-Version: 1.1.7
+Version: 1.1.8
 Summary: GlycoGenius is an all-in-one solution for data analysis of glycomics data.
 Author: Hector Franco Loponte
 Author-email: hectorfloponte@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `glycogenius-1.1.7/README.md` & `glycogenius-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.7/glycogenius/LICENSE.py` & `glycogenius-1.1.8/glycogenius/LICENSE.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.7/glycogenius/Modules/CLI.py` & `glycogenius-1.1.8/glycogenius/Modules/CLI.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
                         var2 = dict(mass.Composition(sequence = var2.split('-')[-1]))
                         var2['H'] -= 2
                         var2['O'] -= 1
                 tag_mass = var2
                 break
         lacto_eesterified = False
         while True:
-            var = input("Is the sample lactonized/ethyl-esterified? (y/n): ")
+            var = input("Is the sample aminated/ethyl-esterified? (y/n): ")
             if var == 'y' or var == '':
                 lacto_eesterified = True
                 break
             elif var == 'n':
                 break
             else:
                 input("\nWrong Input. Press Enter to try again.\n")
@@ -994,15 +994,15 @@
         save_path = parameters[2]
         Execution_Functions.generate_cfg_file(save_path, comments)
         
     if save_path != '':
         pathlib.Path(save_path).mkdir(exist_ok = True, parents = True)
         
     #args to execution functions:
-    output_filtered_data_args = [curve_fit_score, iso_fit_score, s_to_n, max_ppm, percentage_auc, reanalysis, reanalysis_path, save_path, analyze_ms2[0], analyze_ms2[2], reporter_ions, plot_metaboanalyst, compositions, align_chromatograms, force_nglycan, ret_time_interval[2], rt_tolerance_frag, iso_fittings, output_plot_data, multithreaded_analysis, number_cores]
+    output_filtered_data_args = [curve_fit_score, iso_fit_score, s_to_n, max_ppm, percentage_auc, reanalysis, reanalysis_path, save_path, analyze_ms2[0], analyze_ms2[2], reporter_ions, plot_metaboanalyst, compositions, align_chromatograms, force_nglycan, ret_time_interval[2], rt_tolerance_frag, iso_fittings, output_plot_data, multithreaded_analysis, number_cores, 0.0]
 
     imp_exp_gen_library_args = [custom_glycans_list, min_max_monos, min_max_hex, min_max_hexnac, min_max_sia, min_max_fuc, min_max_ac, min_max_gc, force_nglycan, max_adducts, adducts_exclusion, max_charges, reducing_end_tag, fast_iso, high_res, imp_exp_library, library_path, exp_lib_name, only_gen_lib, save_path, internal_standard, permethylated, lactonized_ethyl_esterified, reduced]
 
     list_of_data_args = [samples_list]
 
     index_spectra_from_file_ms1_args = [None, 1, multithreaded_analysis, number_cores]
```

### Comparing `glycogenius-1.1.7/glycogenius/Modules/Config_Handler.py` & `glycogenius-1.1.8/glycogenius/Modules/Config_Handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import sys
 import os
 import datetime
 import configparser
 
 
 
-def config_handler():
+def config_handler(from_GUI = False, param_file_path = ''):
     '''A function that handles the input of configs through a pipelined
     parameters .ini file and turns them into arguments for the functions
     used in core module.
     
     Parameters
     ----------
     none
@@ -99,20 +99,26 @@
     iso_fittings = False
     reanalysis = False
     reanalysis_path = ''
     output_plot_data = False
 
     samples_list = []
     samples_names = []
-
+    
     CLI.print_header(False)
     config = configparser.ConfigParser()
     configs = ""
-    for line in sys.stdin:
-        configs+=line
+    if from_GUI:
+        with open(param_file_path, "r") as f:
+            for line in f:
+                configs+=line
+            f.close()
+    else:
+        for line in sys.stdin:
+            configs+=line
     config.read_string(configs)
     
     #working directory
     save_path = config['running_modes']['working_directory']
     save_path = save_path.strip()
     save_path = save_path.strip("'")
     save_path = save_path.strip("\"")
@@ -236,43 +242,35 @@
         
         total_neu5ac = config['library_building_modes']['neu5ac'].split(',')
         min_max_ac = [int(total_neu5ac[0]), int(total_neu5ac[1])]
         
         total_neu5gc = config['library_building_modes']['neu5gc'].split(',')
         min_max_gc = [int(total_neu5gc[0]), int(total_neu5gc[1])]
         
-    if library_mode != 'import_library':
-        imp_exp_library[1] = config['library_building_modes'].getboolean('export_library')
-        if imp_exp_library[1]:
-            exp_lib_name = config['library_building_modes']['exported_library_name'].strip()
-        force_nglycan = config['common_library_building_settings'].getboolean('force_nglycan')
-        max_adducts = General_Functions.form_to_comp(config['common_library_building_settings']['max_adducts'])
-        adducts_exc = config['common_library_building_settings']['adducts_exclusion'].split(",")
-        if len(adducts_exc) > 0:
-            for i in adducts_exc:
-                adducts_exclusion.append(General_Functions.form_to_comp(i.strip()))
-        max_charges = int(config['common_library_building_settings']['max_charges'])
-        try:
-            reducing_end_tag = float(config['common_library_building_settings']['reducing_end_tag'])
-        except:
-            reducing_end_tag = config['common_library_building_settings']['reducing_end_tag']
-            if reducing_end_tag.split('-')[0] == 'pep':
-                reducing_end_tag = dict(mass.Composition(sequence = reducing_end_tag.split('-')[-1]))
-                reducing_end_tag['H'] -= 2
-                reducing_end_tag['O'] -= 1
-        permethylated = config['common_library_building_settings'].getboolean('permethylated')
-        reduced = config['common_library_building_settings'].getboolean('reduced')
-        lactonized_ethyl_esterified = config['common_library_building_settings'].getboolean('lactonized_ethyl_esterified')
-        fast_iso = config['common_library_building_settings'].getboolean('fast_iso')
-        high_res = config['common_library_building_settings'].getboolean('high_resolution_isotopic_dist')
-        internal_standard = config['common_library_building_settings']['internal_standard_mass']
-        if len(internal_standard.strip()) == 0:
-            internal_standard = 0.0
-        else:
-            internal_standard = float(internal_standard)
+    imp_exp_library[1] = config['library_building_modes'].getboolean('export_library')
+    if imp_exp_library[1]:
+        exp_lib_name = config['library_building_modes']['exported_library_name'].strip()
+    force_nglycan = config['common_library_building_settings'].getboolean('force_nglycan')
+    max_adducts = General_Functions.form_to_comp(config['common_library_building_settings']['max_adducts'])
+    adducts_exc = config['common_library_building_settings']['adducts_exclusion'].split(",")
+    if len(adducts_exc) > 0:
+        for i in adducts_exc:
+            adducts_exclusion.append(General_Functions.form_to_comp(i.strip()))
+    max_charges = int(config['common_library_building_settings']['max_charges'])
+    reducing_end_tag = config['common_library_building_settings']['reducing_end_tag']
+    permethylated = config['common_library_building_settings'].getboolean('permethylated')
+    reduced = config['common_library_building_settings'].getboolean('reduced')
+    lactonized_ethyl_esterified = config['common_library_building_settings'].getboolean('aminated_ethyl_esterified')
+    fast_iso = config['common_library_building_settings'].getboolean('fast_iso')
+    high_res = config['common_library_building_settings'].getboolean('high_resolution_isotopic_dist')
+    internal_standard = config['common_library_building_settings']['internal_standard_mass']
+    if len(internal_standard.strip()) == 0:
+        internal_standard = 0.0
+    else:
+        internal_standard = float(internal_standard)
         
         
     #analysis running mode
     if not reanalysis and not only_gen_lib:
         samples_path = config['running_modes']['samples_directory']
         samples_path = samples_path.strip()
         samples_path = samples_path.strip("'")
@@ -333,31 +331,34 @@
                 if len(i) == 0:
                     reporter_ions = reporter_ions[:i_i]+reporter_ions[i_i+1:]
         align_chromatograms = config['post-analysis/reanalysis'].getboolean('align_chromatograms')
         percentage_auc = float(config['post-analysis/reanalysis']['auc_percentage_threshold'])/100
         max_ppm = int(config['post-analysis/reanalysis']['max_ppm_threshold'])
         iso_fit_score = float(config['post-analysis/reanalysis']['isotopic_fitting_score_threshold'])
         curve_fit_score = float(config['post-analysis/reanalysis']['curve_fitting_score_threshold'])
-        s_to_n = int(config['post-analysis/reanalysis']['signal_to_noise_threshold'])
+        s_to_n = float(config['post-analysis/reanalysis']['signal_to_noise_threshold'])
         compositions = config['post-analysis/reanalysis'].getboolean('analyze_compositions')
         plot_metaboanalyst_file = config['post-analysis/reanalysis'].getboolean('output_metaboanalyst_file')
         if plot_metaboanalyst_file:
             metaboanalyst_groups = config['post-analysis/reanalysis']['metaboanalyst_groups'].split(",")
             for i_i in range(len(metaboanalyst_groups)-1, -1, -1):
                 metaboanalyst_groups[i_i] = metaboanalyst_groups[i_i].strip()
                 metaboanalyst_groups[i_i] = metaboanalyst_groups[i_i].strip("'")
                 metaboanalyst_groups[i_i] = metaboanalyst_groups[i_i].strip("\"")
                 if len(metaboanalyst_groups[i_i]) == 0:
                     del metaboanalyst_groups[i_i]
             plot_metaboanalyst = (plot_metaboanalyst_file, metaboanalyst_groups)
         iso_fittings = config['post-analysis/reanalysis'].getboolean('output_fittings_data')
         output_plot_data = config['post-analysis/reanalysis'].getboolean('output_plot_data')
         
+    if from_GUI:
+        return (custom_glycans_list, min_max_monos, min_max_hex, min_max_hexnac, min_max_sia, min_max_fuc, min_max_ac, min_max_gc, force_nglycan, max_adducts, adducts_exclusion, max_charges, reducing_end_tag, permethylated, reduced, lactonized_ethyl_esterified, fast_iso, high_res, internal_standard, imp_exp_library, exp_lib_name, library_path, only_gen_lib), (multithreaded_analysis, number_cores, analyze_ms2, reporter_ions, tolerance, ret_time_interval, rt_tolerance_frag, min_isotopologue_peaks, min_ppp, close_peaks, align_chromatograms, percentage_auc, max_ppm, iso_fit_score, curve_fit_score, s_to_n, custom_noise, samples_path, save_path, plot_metaboanalyst, compositions, iso_fittings, reanalysis, reanalysis_path, output_plot_data)
+        
     #args to execution functions:
-    output_filtered_data_args = [curve_fit_score, iso_fit_score, s_to_n, max_ppm, percentage_auc, reanalysis, reanalysis_path, save_path, analyze_ms2[0], analyze_ms2[2], reporter_ions, plot_metaboanalyst, compositions, align_chromatograms, force_nglycan, ret_time_interval[2], rt_tolerance_frag, iso_fittings, output_plot_data, multithreaded_analysis, number_cores]
+    output_filtered_data_args = [curve_fit_score, iso_fit_score, s_to_n, max_ppm, percentage_auc, reanalysis, reanalysis_path, save_path, analyze_ms2[0], analyze_ms2[2], reporter_ions, plot_metaboanalyst, compositions, align_chromatograms, force_nglycan, ret_time_interval[2], rt_tolerance_frag, iso_fittings, output_plot_data, multithreaded_analysis, number_cores, 0.0]
 
     imp_exp_gen_library_args = [custom_glycans_list, min_max_monos, min_max_hex, min_max_hexnac, min_max_sia, min_max_fuc, min_max_ac, min_max_gc, force_nglycan, max_adducts, adducts_exclusion, max_charges, reducing_end_tag, fast_iso, high_res, imp_exp_library, library_path, exp_lib_name, only_gen_lib, save_path, internal_standard, permethylated, lactonized_ethyl_esterified, reduced]
 
     list_of_data_args = [samples_list]
 
     index_spectra_from_file_ms1_args = [None, 1, multithreaded_analysis, number_cores]
```

### Comparing `glycogenius-1.1.7/glycogenius/Modules/Execution_Functions.py` & `glycogenius-1.1.8/glycogenius/Modules/Execution_Functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,16 +547,16 @@
             df = {'Glycan' : [], 'Hex' : [], 'HexNAc' : [], 'dHex' : [], 'Neu5Ac' : [], 'Neu5Gc' : [], 'Isotopic Distribution' : [], 'Neutral Mass + Tag' : []}
         for i_i, i in enumerate(full_library):
             if lactonized_ethyl_esterified:
                 df['Glycan'].append(i)
                 df['Hex'].append(full_library[i]['Monos_Composition']['H'])
                 df['HexNAc'].append(full_library[i]['Monos_Composition']['N'])
                 df['dHex'].append(full_library[i]['Monos_Composition']['F'])
-                df['a2,3-Neu5Ac'].append(full_library[i]['Monos_Composition']['lS'])
-                df['a2,6-Neu5Ac'].append(full_library[i]['Monos_Composition']['eS'])
+                df['a2,3-Neu5Ac'].append(full_library[i]['Monos_Composition']['Am'])
+                df['a2,6-Neu5Ac'].append(full_library[i]['Monos_Composition']['E'])
                 df['Neu5Gc'].append(full_library[i]['Monos_Composition']['G'])
             else:
                 df['Glycan'].append(i)
                 df['Hex'].append(full_library[i]['Monos_Composition']['H'])
                 df['HexNAc'].append(full_library[i]['Monos_Composition']['N'])
                 df['dHex'].append(full_library[i]['Monos_Composition']['F'])
                 df['Neu5Ac'].append(full_library[i]['Monos_Composition']['S'])
@@ -591,15 +591,15 @@
                     formula = General_Functions.comp_to_formula(General_Functions.sum_atoms(full_library[i]['Atoms_Glycan+Tag'], adduct_comp))
                     list_form = [i, str(formula), '[M+'+adduct+']', str(General_Functions.form_to_charge(j))]
                     f.write(",".join(list_form)+'\n')
             f.close()
         print("Done!")
     if only_gen_lib:
         print('Library length: '+str(len(full_library)))
-        print("Check it in Glycans_Library.xlsx.")
+        print("Check it in "+exp_lib_name+".")
         print("If you wish to analyze files,")
         print("set 'only_gen_lib' to False and input")
         print("remaining parameters.")
         if os.isatty(0):
             input("\nPress Enter to exit.")
             os._exit(1)
         else:
@@ -948,15 +948,17 @@
                          nglycan,
                          rt_tolerance,
                          rt_tolerance_frag,
                          output_isotopic_fittings,
                          output_plot_data,
                          multithreaded,
                          number_cores,
-                         temp_time = 0.0):
+                         temp_time,
+                         from_GUI = False,
+                         metab_groups = []):
     '''This function filters and converts raw results data into human readable
     excel files.
     
     Parameters
     ----------
     curve_fit_score : float
         The minimum curve fitting score to consider when outputting results.
@@ -1036,15 +1038,18 @@
     -------
     nothing
         Creates excel files of processed data.
     '''
     date = datetime.datetime.now()
     begin_time = str(date)[2:4]+str(date)[5:7]+str(date)[8:10]+"_"+str(date)[11:13]+str(date)[14:16]+str(date)[17:19]
     if reanalysis:
-        print("Reanalyzing raw data with new parameters...")
+        if from_GUI:
+            print("Saving results files...")
+        else:
+            print("Reanalyzing raw data with new parameters...")
         temp_path = save_path+begin_time+"_Temp/"
         pathlib.Path(temp_path).mkdir(exist_ok = True, parents = True)
         try:
             General_Functions.open_gg(gg_file, temp_path)
         except:
             print("\nAnalysis file not found. If you're reanalyzing\nan existing analysis result file, check if the\npath in 'analysis_file' is correct, otherwise\nchange 'reanalysis' to 'no' and try again.\n")
             return
@@ -1624,27 +1629,36 @@
     if plot_metaboanalyst[0]: #start of metaboanalyst plot
         print("Creating file for metaboanalyst plotting...", end="", flush=True)
         with open(save_path+begin_time+"_metaboanalyst_data.csv", "w") as f:
             samples_line = ["Sample"]
             for i_i, i in enumerate(df2["File_Name"]):
                 samples_line.append(i)
             groups_line = ["Group"]
-            if len(plot_metaboanalyst[1]) > 0:
-                for i in df2["File_Name"]:
+            if from_GUI:
+                for i in df2['File_Name']:
                     found = False
-                    for j in plot_metaboanalyst[1]:
-                        if j in i:
-                            found = True
-                            groups_line.append(j)
-                            break
+                    if i in metab_groups.keys():
+                        found = True
+                        groups_line.append(metab_groups[i])
                     if not found:
                         groups_line.append("Ungrouped")
             else:
-                for i in df2["File_Name"]:
-                    groups_line.append("Ungrouped")
+                if len(plot_metaboanalyst[1]) > 0:
+                    for i in df2["File_Name"]:
+                        found = False
+                        for j in plot_metaboanalyst[1]:
+                            if j in i:
+                                found = True
+                                groups_line.append(j)
+                                break
+                        if not found:
+                            groups_line.append("Ungrouped")
+                else:
+                    for i in df2["File_Name"]:
+                        groups_line.append("Ungrouped")
             found_int_std = False
             for i in total_dataframes:
                 if "Internal Standard" in i["Glycan"]:
                     found_int_std = True
                     break
             if found_int_std:
                 with open(save_path+begin_time+"_metaboanalyst_data_normalized.csv", "a") as g:
@@ -2058,15 +2072,16 @@
     except KeyboardInterrupt:
         print("\n\n----------Execution cancelled by user.----------\n", flush=True)
         raise SystemExit(1)
 
 def arrange_raw_data(analyzed_data,
                      samples_names,
                      analyze_ms2,
-                     save_path):
+                     save_path,
+                     from_GUI = False):
     '''Arrange the raw results data into pickled files to be processed by output_filtered_data.
 
     Parameters
     ----------
     analyzed_data : tuple
         Tuple containing multiple informations about the glycans analysis, as outputted by
         analyze_files or analyze_ms2.
@@ -2256,14 +2271,17 @@
         del curve_fitting_dataframes
         f.close()
     with open(temp_path+'raw_data_6', 'wb') as f:
         dill.dump(isotopic_fits_dataframes, f)
         del isotopic_fits_dataframes
         f.close()
     General_Functions.make_gg(temp_path, save_path, begin_time+"_Analysis")
+    if from_GUI:
+        print("File name is "+begin_time+"_Analysis.gg")
+        shutil.rmtree(temp_path)
     print("Done!")
     return begin_time
 
 def print_sep(): ##Complete
     '''Prints a separator consisting of 48 '-' character.
     
     Parameters
@@ -2366,15 +2384,16 @@
                   ret_time_interval,
                   min_isotops,
                   min_ppp,
                   max_charges,
                   custom_noise,
                   close_peaks,
                   multithreaded,
-                  number_cores): ##Complete
+                  number_cores,
+                  from_GUI = False): ##Complete
     '''Integrates all the file-accessing associated functions in this script to go
     through the files data, draw and process eic of hypothetical glycans, does 
     peak-picking and calculates AUC of the peaks.
 
     Parameters
     ----------
     library : dict
@@ -2503,14 +2522,15 @@
     print('Done!')
     print("Pre-processing done in "+str(datetime.datetime.now() - begin_time)+"!")
     print_sep()
     print("Analyzing glycans in samples' MS1 spectra...")
     begin_time = datetime.datetime.now()
     
     results = []
+    temp_results = []
     with concurrent.futures.ProcessPoolExecutor(max_workers = cpu_count) as executor:
         for i_i, i in enumerate(library):
             result = executor.submit(analyze_glycan, 
                                      library,
                                      lib_size,
                                      data,
                                      ms1_index,
@@ -2524,17 +2544,25 @@
                                      close_peaks,
                                      zeroes_arrays,
                                      inf_arrays,
                                      threads_arrays,
                                      rt_array_report,
                                      ms1_id,
                                      i,
-                                     i_i,
-                                     lib_size)
+                                     i_i)
             results.append(result)
+            if from_GUI:
+                temp_results.append(result)
+                if len(temp_results) == cpu_count:
+                    for k_k, k in enumerate(temp_results):
+                        k.result()
+                        del temp_results[k_k]
+                        if len(temp_results) < cpu_count:
+                            break
+                print('Analyzing glycan '+str(i)+': '+str(i_i+1)+'/'+str(lib_size))
     for i in results:
         result_data = i.result()
         analyzed_data[result_data[1]] = result_data[0]
             
     print('Sample MS1 analysis done in '+str(datetime.datetime.now() - begin_time)+'!')
     return analyzed_data, rt_array_report, noise_avg
     
@@ -2552,16 +2580,15 @@
                   close_peaks,
                   zeroes_arrays,
                   inf_arrays,
                   threads_arrays,
                   rt_arrays,
                   ms1_id,
                   i,
-                  i_i,
-                  total_glycans):
+                  i_i):
     '''Analyzes one single glycan. Core function of analyze_files.
     
     Parameters
     ----------
     library : dict
         A glycans library, as generated by Library_Tools.full_glycans_library.
         
@@ -2659,15 +2686,15 @@
     glycan_data : dict
         A modified dictionary entry of the library, including a lot of information of the glycan obtained by the program.
         
     i : string
         The glycan analyzed.
     '''
     try:
-        print('Analyzing glycan '+str(i)+': '+str(i_i+1)+'/'+str(total_glycans))
+        print('Analyzing glycan '+str(i)+': '+str(i_i+1)+'/'+str(lib_size))
         
         glycan_data = library[i]
         glycan_data['Adducts_mz_data'] = {}
         temp_eic = File_Accessing.eic_from_glycan(data,
                                                   i,
                                                   glycan_data,
                                                   ms1_index,
@@ -2752,15 +2779,16 @@
                 permethylated,
                 reduced,
                 lactonized_ethyl_esterified,
                 filter_output,
                 unrestricted_fragments,
                 rt_tolerance,
                 multithreaded,
-                number_cores):
+                number_cores,
+                from_GUI = False):
     '''Analyzes the MS2 data in the sample files, outputting the found matches.
     
     Parameters
     ----------
     ms2_index : dict
         A dictionary containing the ms2 indexes of each sample file.
         
@@ -2900,14 +2928,15 @@
                                   lactonized_ethyl_esterified,
                                   nglycan)
     fragments_data = {}
     print('Scanning MS2 spectra...')
     scan_begin_time = datetime.datetime.now()
     
     results = []
+    temp_results = []
     if multithreaded:
         if number_cores == 'all':
             cpu_count = (os.cpu_count())-2
             if cpu_count <= 0:
                 cpu_count = 1
         else:
             number_cores = int(number_cores)
@@ -2931,14 +2960,23 @@
                                      tolerance,
                                      filter_output,
                                      unrestricted_fragments,
                                      rt_tolerance,
                                      i_i,
                                      i)
             results.append(result)
+            if from_GUI:
+                temp_results.append(result)
+                if len(temp_results) == cpu_count:
+                    for k_k, k in enumerate(temp_results):
+                        k.result()
+                        del temp_results[k_k]
+                        if len(temp_results) < cpu_count:
+                            break
+                print('Analyzing glycan '+str(i)+': '+str(i_i+1)+'/'+str(len(analyzed_data[0])))
             
     for i in results:
         result_data = i.result()
         fragments_data[result_data[1]] = result_data[0]
         
     print('Sample MS2 analysis done in '+str(datetime.datetime.now() - begin_time)+'!')
     return analyzed_data[0], analyzed_data[1], analyzed_data[2], fragments_data
@@ -3042,16 +3080,16 @@
                             
                             found = False
                             for n_n, n in enumerate(fragments):
                                 if 'Monos_Composition' in list(n.keys()):
                                     if lactonized_ethyl_esterified:
                                         if (n['Monos_Composition']['H'] == analyzed_data[0][i]['Monos_Composition']['H']
                                             and n['Monos_Composition']['N'] == analyzed_data[0][i]['Monos_Composition']['N']
-                                            and n['Monos_Composition']['lS'] == analyzed_data[0][i]['Monos_Composition']['lS']
-                                            and n['Monos_Composition']['eS'] == analyzed_data[0][i]['Monos_Composition']['eS']
+                                            and n['Monos_Composition']['Am'] == analyzed_data[0][i]['Monos_Composition']['Am']
+                                            and n['Monos_Composition']['E'] == analyzed_data[0][i]['Monos_Composition']['E']
                                             and n['Monos_Composition']['F'] == analyzed_data[0][i]['Monos_Composition']['F']
                                             and n['Monos_Composition']['G'] == analyzed_data[0][i]['Monos_Composition']['G']):
                                             continue
                                     else:
                                         if (n['Monos_Composition']['H'] == analyzed_data[0][i]['Monos_Composition']['H']
                                             and n['Monos_Composition']['N'] == analyzed_data[0][i]['Monos_Composition']['N']
                                             and n['Monos_Composition']['S'] == analyzed_data[0][i]['Monos_Composition']['S']
@@ -3076,26 +3114,26 @@
                                         viable = []
                                         for o in fragments_comp:
                                             if lactonized_ethyl_esterified:
                                                 if 'H' not in o.keys():
                                                     o['H'] = 0
                                                 if 'N' not in o.keys():
                                                     o['N'] = 0
-                                                if 'lS' not in o.keys():
-                                                    o['lS'] = 0
-                                                if 'eS' not in o.keys():
-                                                    o['eS'] = 0
+                                                if 'Am' not in o.keys():
+                                                    o['Am'] = 0
+                                                if 'E' not in o.keys():
+                                                    o['E'] = 0
                                                 if 'F' not in o.keys():
                                                     o['F'] = 0
                                                 if 'G' not in o.keys():
                                                     o['G'] = 0
                                                 if (o['H'] > analyzed_data[0][i]['Monos_Composition']['H']
                                                     or o['N'] > analyzed_data[0][i]['Monos_Composition']['N']
-                                                    or o['lS'] > analyzed_data[0][i]['Monos_Composition']['lS']
-                                                    or o['eS'] > analyzed_data[0][i]['Monos_Composition']['eS']
+                                                    or o['Am'] > analyzed_data[0][i]['Monos_Composition']['Am']
+                                                    or o['E'] > analyzed_data[0][i]['Monos_Composition']['E']
                                                     or o['F'] > analyzed_data[0][i]['Monos_Composition']['F']
                                                     or o['G'] > analyzed_data[0][i]['Monos_Composition']['G']):
                                                     viable.append(False)
                                                     break
                                                 else:
                                                     viable.append(True)
                                             else:
@@ -3130,15 +3168,15 @@
                                                         count+= 1
                                                 else:
                                                     if o:
                                                         new_formula+= "/"+formula_splitted[o_o]
                                                         count+= 1
                                     elif "/" not in n['Formula'] and not combo:
                                         if lactonized_ethyl_esterified:
-                                            if (n['Monos_Composition']['H'] > analyzed_data[0][i]['Monos_Composition']['H'] or n['Monos_Composition']['N'] > analyzed_data[0][i]['Monos_Composition']['N'] or n['Monos_Composition']['lS'] > analyzed_data[0][i]['Monos_Composition']['lS'] or n['Monos_Composition']['eS'] > analyzed_data[0][i]['Monos_Composition']['eS'] or n['Monos_Composition']['F'] > analyzed_data[0][i]['Monos_Composition']['F'] or n['Monos_Composition']['G'] > analyzed_data[0][i]['Monos_Composition']['G']):
+                                            if (n['Monos_Composition']['H'] > analyzed_data[0][i]['Monos_Composition']['H'] or n['Monos_Composition']['N'] > analyzed_data[0][i]['Monos_Composition']['N'] or n['Monos_Composition']['Am'] > analyzed_data[0][i]['Monos_Composition']['Am'] or n['Monos_Composition']['E'] > analyzed_data[0][i]['Monos_Composition']['E'] or n['Monos_Composition']['F'] > analyzed_data[0][i]['Monos_Composition']['F'] or n['Monos_Composition']['G'] > analyzed_data[0][i]['Monos_Composition']['G']):
                                                 continue
                                         else:
                                             if (n['Monos_Composition']['H'] > analyzed_data[0][i]['Monos_Composition']['H'] or n['Monos_Composition']['N'] > analyzed_data[0][i]['Monos_Composition']['N'] or n['Monos_Composition']['S'] > analyzed_data[0][i]['Monos_Composition']['S'] or n['Monos_Composition']['F'] > analyzed_data[0][i]['Monos_Composition']['F'] or n['Monos_Composition']['G'] > analyzed_data[0][i]['Monos_Composition']['G']):
                                                 continue
                                 for o in n['Adducts_mz']:
                                     if abs(n['Adducts_mz'][o]-m) <= General_Functions.tolerance_calc(tolerance[0], tolerance[1], n['Adducts_mz'][o]): #fragments data outputted in the form of (Glycan, Adduct, Fragment, Fragment mz, intensity, retention time, precursor)
                                         if "_" not in n['Formula']:
```

### Comparing `glycogenius-1.1.7/glycogenius/Modules/File_Accessing.py` & `glycogenius-1.1.8/glycogenius/Modules/File_Accessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,15 @@
         dict with keys for each file id, at which value is a list of lists, with the
         first one being the rt array and the second one the raw int array.
         
     isotopic_fits : dict
         A dictionary containing all the isotopic fitting information for reporting and 
         checking data.
     '''
+    global buffer, buffer_good
     data = {}
     ppm_info = {}
     iso_fitting_quality = {}
     isotopic_fits = {}
     verbose_info = []
     raw_data = {}
     for i in glycan_info['Adducts_mz']:
@@ -245,14 +246,16 @@
             iso_fitting_quality[i][j_j] = copy.deepcopy(zeroes_arrays[j_j])
             data[i][j_j] = [copy.deepcopy(rt_arrays[j_j]), copy.deepcopy(zeroes_arrays[j_j])]
             raw_data[i][j_j] = [copy.deepcopy(rt_arrays[j_j]), copy.deepcopy(zeroes_arrays[j_j])]
             isotopic_fits[i][j_j] = {}
             thread_numbers = threads_arrays[j_j]
             
             #checked possibility of parallelization here, too much overhead (over 10 more time to run, even if using 1 core)
+            buffer = []
+            buffer_good = 0
             for k_k, k in enumerate(thread_numbers):
                 analyze_mz_array(j[k]['m/z array'],
                                  j[k]['intensity array'],
                                  glycan_info,
                                  tolerance,
                                  min_isotops,
                                  noise,
@@ -264,17 +267,17 @@
                                  raw_data,
                                  isotopic_fits,
                                  i,
                                  j_j,
                                  k,
                                  j[k]['retentionTime'],
                                  ms1_id[j_j][k_k],
+                                 ms1_id[-1],
                                  adduct_mass,
                                  adduct_charge)
-                
     return data, ppm_info, iso_fitting_quality, verbose_info, raw_data, isotopic_fits
 
     
 def analyze_mz_array(sliced_mz,
                      sliced_int,
                      glycan_info,
                      tolerance,
@@ -288,14 +291,15 @@
                      raw_data,
                      isotopic_fits,
                      glycan_id,
                      file_id,
                      thread_id,
                      ret_time,
                      ms1_id,
+                     last_ms1_id,
                      adduct_mass,
                      adduct_charge):
     '''The core function of eic_from_glycan. Analyzes a single spectrum and outputs
     relevant information, such as the PPM-error of the monoisotopic peak, isotopic fitting
     information, etc.
     
     Parameters
@@ -396,14 +400,15 @@
         Dot product of two arrays.
         
     Returns
     -------
     nothing
         Edits the target dictionaries/lists directly.
     '''
+    global buffer, buffer_good
     intensity = 0.0 #variable to sum the total deisotopotized intensity
     mono_int = 0.0 #variable to sum the total intensity of the monoisotopic peak
     iso_distro = 1 #starting isotopic distribution peak, always 1
     charge_range = range(1, abs(max_charges)*2)
     target_mz = glycan_info['Adducts_mz'][glycan_id]
     second_peak = (glycan_info['Isotopic_Distribution_Masses'][1]+adduct_mass)/adduct_charge
     sec_peak_rel_int = glycan_info['Isotopic_Distribution'][1]
@@ -434,15 +439,15 @@
             current_iso_peak1 = []
             current_iso_peak2 = []
             current_mz = []
             iso_distro += 1
             iso_found = False
         if not_good: #Here are checks for quick skips
             break
-        if max_int < avg_noise[file_id]*0.5: #if there's no peak with intensity higher than 50% of the average noise of sample, don't even check it
+        if max_int < avg_noise[file_id]: #if there's no peak with intensity higher than the average noise of sample, don't even check it
             break
         if l_l == len(sliced_mz)-1 and not found:
             not_good = True
             break
         if target_mz > sliced_mz[-1]:
             not_good = True
             break
@@ -508,53 +513,82 @@
         if sliced_mz[l_l] > target_mz+General_Functions.tolerance_calc(tolerance[0], tolerance[1], target_mz) or l_l == len(sliced_mz)-1:
             raw_data[glycan_id][file_id][1][ms1_id] = 0.0
             break
         if abs(sliced_mz[l_l] - target_mz) <= General_Functions.tolerance_calc(tolerance[0], tolerance[1], target_mz):
             raw_data[glycan_id][file_id][1][ms1_id] = sliced_int[l_l]
             break
             
-    if len(iso_actual) > 0:
-        dotp = []
-        weights = []
-        number = range(1, len(mz_isos)+1)
-        starting_points = [0, 1]
-        for m_m, m in enumerate(number):
-            intensities = [iso_actual[m_m], iso_target[m_m]]
-            intensity_score = min(intensities)/max(intensities)
-            vector_actual = [m-starting_points[0], iso_actual[m_m]-starting_points[1]]
-            vector_target = [m-starting_points[0], iso_target[m_m]-starting_points[1]]
-            magnitude_target = sqrt(vector_target[0]**2 + vector_target[1]**2)
-            normalized_actual = vector_actual/numpy.linalg.norm(vector_actual)
-            normalized_target = vector_target/numpy.linalg.norm(vector_target)
-            starting_points = [m, iso_target[m_m]]
-            dotproduct = numpy.dot(normalized_actual, normalized_target)
-            dotp.append(numpy.average([(dotproduct+1)/2, intensity_score], weights = [3, 2]))
-            weights.append(1/m)
-        iso_quali = numpy.average(dotp, weights = weights)
-        
-        #reduces score if fewer isotopic peaks are found: punishing for only 2 peaks, normal score from 3 and over
-        if len(iso_actual) == 1:
-            iso_quali = (iso_quali*0.8)
-        
-        mz_isos = [glycan_info['Adducts_mz'][glycan_id]]+mz_isos
-        iso_target = [1]+iso_target
-        iso_actual = [1]+iso_actual
+    if not_good:
+        buffer.append(None)
+            
+    if not not_good:
+        if len(iso_actual) > 0:
+            dotp = []
+            weights = []
+            number = range(1, len(mz_isos)+1)
+            starting_points = [0, 1]
+            for m_m, m in enumerate(number):
+                intensities = [iso_actual[m_m], iso_target[m_m]]
+                intensity_score = min(intensities)/max(intensities)
+                vector_actual = [m-starting_points[0], iso_actual[m_m]-starting_points[1]]
+                vector_target = [m-starting_points[0], iso_target[m_m]-starting_points[1]]
+                magnitude_target = sqrt(vector_target[0]**2 + vector_target[1]**2)
+                normalized_actual = vector_actual/numpy.linalg.norm(vector_actual)
+                normalized_target = vector_target/numpy.linalg.norm(vector_target)
+                starting_points = [m, iso_target[m_m]]
+                dotproduct = numpy.dot(normalized_actual, normalized_target)
+                dotp.append(numpy.average([(dotproduct+1)/2, intensity_score], weights = [3, 2]))
+                weights.append(1/m)
+            iso_quali = numpy.average(dotp, weights = weights)
+            
+            #reduces score if fewer isotopic peaks are found: punishing for only 2 peaks, normal score from 3 and over
+            if len(iso_actual) == 1:
+                iso_quali = (iso_quali*0.8)
+            
+            mz_isos = [glycan_info['Adducts_mz'][glycan_id]]+mz_isos
+            iso_target = [1]+iso_target
+            iso_actual = [1]+iso_actual
+                
+        if len(iso_actual) == 0:
+            iso_quali = 0.0
             
-    if len(iso_actual) == 0:
-        iso_quali = 0.0
+        if len(mono_ppm) > 0:
+            ppm_error = mean(mono_ppm)
+        else:
+            ppm_error = inf
         
-    if len(mono_ppm) > 0:
-        ppm_error = mean(mono_ppm)
-    else:
-        ppm_error = inf
-        
-    ppm_info[glycan_id][file_id][ms1_id] = ppm_error
-    iso_fitting_quality[glycan_id][file_id][ms1_id] = iso_quali
-    data[glycan_id][file_id][1][ms1_id] = intensity
-    isotopic_fits[glycan_id][file_id][ret_time] = [mz_isos, iso_target, iso_actual, iso_quali]
+        buffer.append(([glycan_id, file_id, ms1_id, float("%.2f" % round(ret_time, 2))], [ppm_error, iso_quali, intensity, [mz_isos, iso_target, iso_actual, iso_quali]]))
+        
+    #dinamical clean-up of buffer
+    min_in_a_row = 3
+    buffer_size = 10
+    if len(buffer) >= buffer_size or ms1_id == last_ms1_id: 
+        highest_in_a_row = 0
+        in_a_row = 0
+        for i_i, i in enumerate(buffer):
+            if i != None:
+                in_a_row += 1
+                if in_a_row > highest_in_a_row:
+                    highest_in_a_row = in_a_row
+            else:
+                if in_a_row > 0 and in_a_row < min_in_a_row:
+                    for k_k, k in enumerate(buffer):
+                        if k_k >= i_i:
+                            break
+                        if k_k >= i_i-in_a_row:
+                            buffer[k_k] = None
+                in_a_row = 0
+        if highest_in_a_row >= min_in_a_row: #edit this number to demand a minimum number of points in a row, up to a maximum of the buffer size (10)
+            for i in buffer:
+                if i != None:
+                    ppm_info[i[0][0]][i[0][1]][i[0][2]] = i[1][0]
+                    iso_fitting_quality[i[0][0]][i[0][1]][i[0][2]] = i[1][1]
+                    data[i[0][0]][i[0][1]][1][i[0][2]] = i[1][2]
+                    isotopic_fits[i[0][0]][i[0][1]][i[0][3]] = i[1][3]
+        buffer.pop(0)
     
 def eic_smoothing(y, lmbd = 100, d = 2):
     '''Implementation of the Whittaker smoothing algorithm,
     based on the work by Eilers [1].
 
     [1] P. H. C. Eilers, "A perfect smoother", Anal. Chem. 2003, (75), 3631-3636
     
@@ -786,16 +820,16 @@
     temp_max = 0
     temp_max_id_iu = 0
     temp_min = inf
     temp_min_id_iu = 0
     going_up = False
     going_down = False
     datapoints_per_time = int(0.2/(rt_int[0][rt_int[1].index(max(rt_int[1]))]-rt_int[0][rt_int[1].index(max(rt_int[1]))-1]))
-    slope_threshold = 100*datapoints_per_time
-    threshold = int(datapoints_per_time/3)
+    slope_threshold = 50*datapoints_per_time
+    threshold = int(datapoints_per_time/3) #this is tolerance for stopping a peak
     down_count = 0
     end_count = 0
     for i_i, i in enumerate(rt_int_smoothed[1]):
         if (rt_int[0][i_i] >= rt_interval[1] or rt_int[0][i_i] == rt_int[0][-2]):
             break    
         if rt_int[0][i_i] >= rt_interval[0]:
             slope = (rt_int_smoothed[1][i_i+1]-i)/(rt_int[0][i_i+1]-rt_int[0][i_i])
@@ -810,37 +844,45 @@
                     down_count = 0
                     going_up = False
                     going_down = True
             if (going_down and (slope >= 0 or rt_int_smoothed[1][i_i] == 0.0)):
                 if i < temp_min:
                     temp_min = i
                     temp_min_id_iu = i_i
+                    lowest = rt_int_smoothed[1][temp_start]
+                    new_start = None
+                    for k in range(temp_start, temp_start-(temp_min_id_iu-temp_start)//3, -1):
+                        if rt_int_smoothed[1][k] < lowest:
+                            lowest = rt_int_smoothed[1][k]
+                            new_start = k
+                    if new_start != None:
+                        temp_start = new_start
                 if end_count <= threshold:
                     end_count += 1
                 elif end_count > threshold or rt_int_smoothed[1][i_i] == 0.0:
                     end_count = 0
                     going_down = False
                     found_start = False
                     temp_start_2 = 0
                     for k_k, k in enumerate(rt_int_smoothed[1][temp_start:temp_min_id_iu+1]): #trims leading and/or tailing part of the picked pick
-                        if not found_start and k > temp_max*0.01:
+                        if not found_start and k > temp_max*0.02:
                             temp_start_2 = temp_start+k_k
                             found_start = True
-                        if k_k > temp_max_id_iu-temp_start and k < temp_max*0.01:
+                        if k_k > temp_max_id_iu-temp_start and k < temp_max*0.02:
                             temp_min_id_iu = temp_start+k_k
                             break
                     temp_start = temp_start_2
                     good = False
                     if min_ppp[0]:
                         if temp_min_id_iu-temp_start >= min_ppp[1] or glycan == "Internal Standard":
                             good = True
                     else:
                         if temp_min_id_iu-temp_start >= datapoints_per_time or glycan == "Internal Standard":
                             good = True
-                    if temp_max_id_iu >= temp_min_id_iu: #this avoids slopes as peaks
+                    if temp_max_id_iu >= temp_min_id_iu or rt_int[0][temp_min_id_iu] < rt_interval[0]+0.1: #this avoids slopes as peaks
                         good = False
                     if good:
                         temp_peak_width = (rt_int[0][temp_min_id_iu]-rt_int[0][temp_start])
                         peaks.append({'id': temp_max_id_iu, 'rt': rt_int[0][temp_max_id_iu], 'int': temp_max, 'peak_width': temp_peak_width, 'peak_interval': (rt_int[0][temp_start], rt_int[0][temp_min_id_iu]), 'peak_interval_id': (temp_start, temp_min_id_iu)})
                         # print(peaks[-1])
                         temp_max = 0
                         temp_max_id_iu = 0
```

### Comparing `glycogenius-1.1.7/glycogenius/Modules/General_Functions.py` & `glycogenius-1.1.8/glycogenius/Modules/General_Functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 ##---------------------------------------------------------------------------------------
 ##Hard-coded permanent information
 
 monosaccharides = {
     "H": ("Hexose", "C6O6H12", {"C": 6, "O": 5, "N": 0, "H": 10}),
     "N": ("N-Acetyl Hexosamine", "C8O6NH15", {"C": 8, "O": 5, "N": 1, "H": 13}),
     "S": ("Acetyl Neuraminic Acid", "C11O9NH19", {"C": 11, "O": 8, "N": 1, "H": 17}),
-    "lS": ("Lactonized Acetyl Neuraminic Acid alpha2,3 bound", "C11O8N2H20", {"C": 11, "O": 7, "N": 2, "H": 18}),
-    "eS": ("Ethyl-Esterified Acetyl Neuraminic Acid alpha2,6 bound", "C13O9NH23", {"C": 13, "O": 8, "N": 1, "H": 21}),
+    "Am": ("Lactonized Acetyl Neuraminic Acid alpha2,3 bound", "C11O8N2H20", {"C": 11, "O": 7, "N": 2, "H": 18}),
+    "E": ("Ethyl-Esterified Acetyl Neuraminic Acid alpha2,6 bound", "C13O9NH23", {"C": 13, "O": 8, "N": 1, "H": 21}),
     "F": ("Fucose", "C6O5H12", {"C": 6, "O": 4, "N": 0, "H": 10}),
     "G": ("Glycolyl Neuraminic Acid", "C11O10NH19", {"C": 11, "O": 9, "N": 1, "H": 17})
     }
 '''A hardcoded dictionary containing each single letter code for monosaccharides as key
 and a tuple containing the full monosaccharide name, its full molecular formula and its
 residue composition in dict form as value.
 '''
@@ -535,17 +535,17 @@
     friendly_letters = {}
     current_letter = ""
     for i in string:
         if i != current_letter:
             current_letter = i
             count = string.count(i)
             if i == "L":
-                friendly_letters['lS'] = count
+                friendly_letters['Am'] = count
             if i == "E":
-                friendly_letters['eS'] = count
+                friendly_letters['E'] = count
             elif i != "L" and i != "E":
                 friendly_letters[i] = count
     return friendly_letters
 
 def sum_atoms(*compositions):
     '''Sums the atoms of two compositions.
 
@@ -580,15 +580,15 @@
         summed. ie. {"H": 5, "N": 4, "S": 1, "F": 1, "G": 1}.
 
     Returns
     -------
     summed_comp : dict
         Dictionary containing the sum of each monosaccharides of the compositions.
     '''
-    summed_comp = {"H": 0, "N": 0, "S": 0, "lS": 0, "eS": 0, "F": 0, "G": 0, "T": 0}
+    summed_comp = {"H": 0, "N": 0, "S": 0, "Am": 0, "E": 0, "F": 0, "G": 0, "T": 0}
     for i in compositions:
         for j in i:
             summed_comp[j]+=i[j]
     return summed_comp
 
 def comp_to_formula(composition):
     '''Transforms a composition dictionary into string formula.
@@ -721,16 +721,16 @@
                 else:
                     relative_isotop_mass_low_res.append(i)
                     relative_isotop_pattern_low_res.append(relative_isotop_pattern[i_i])
         return relative_isotop_pattern_low_res, relative_isotop_mass_low_res
     return relative_isotop_pattern, relative_isotop_mass
 
 def gen_adducts_combo(adducts,
-                      exclusions,
-                      max_charge):
+                      exclusions=[],
+                      max_charge=3):
     '''Generates a list of dictionaries with compositions of adducts combinations, based
     on parameters set.
 
     Parameters
     ----------
     adducts : dict
         A dictionary with each key containing a single atom adduct and its value
```

### Comparing `glycogenius-1.1.7/glycogenius/Modules/Library_Tools.py` & `glycogenius-1.1.8/glycogenius/Modules/Library_Tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. It is accessible within the program files
 # or by typing 'license' after running it stand-alone in the terminal
 # by typing 'glycogenius'. If not, see <https://www.gnu.org/licenses/>.
 
-import pathlib
-import importlib
 from . import General_Functions
 from pyteomics import mzxml, mzml, mass, auxiliary
 from itertools import combinations_with_replacement
 from re import split
 from math import inf
+import pathlib
+import importlib
 import sys
 import datetime
 
 ##---------------------------------------------------------------------------------------
 ##Library generating-associated functions (these functions make vast use of the general
 ## functions).
 
@@ -100,47 +100,47 @@
     Returns
     -------
     glycans : list
         A list containing dictionaries of the monosaccharides compositions of all the
         glycans generated.
     '''
     glycans = []
-    def_glycan_comp = {"H": 0, "N": 0, "S": 0, "lS": 0, "eS": 0, "F": 0, "G": 0}
+    def_glycan_comp = {"H": 0, "N": 0, "S": 0, "Am": 0, "E": 0, "F": 0, "G": 0}
     for i in range(min_max_mono[0], min_max_mono[1]+1):
         if lactonized_ethyl_esterified:
             for j in combinations_with_replacement("HNLEFG", i):
                 glycans.append(General_Functions.sum_monos(def_glycan_comp, General_Functions.count_seq_letters("".join(j))))
         else:
             for j in combinations_with_replacement("HNSFG", i):
                 glycans.append(General_Functions.sum_monos(def_glycan_comp, General_Functions.count_seq_letters("".join(j))))
     to_be_removed = []
     for i_i, i in enumerate(glycans):
         if lactonized_ethyl_esterified:
             if ((i['H'] < min_max_hex[0]) or (i['H'] > min_max_hex[1])
                 or (i['N'] < min_max_hexnac[0]) or (i['N'] > min_max_hexnac[1])
-                or (i['lS']+i['eS']+i['G'] < min_max_sialics[0])
-                or (i['lS']+i['eS']+i['G'] > min_max_sialics[1])
+                or (i['Am']+i['E']+i['G'] < min_max_sialics[0])
+                or (i['Am']+i['E']+i['G'] > min_max_sialics[1])
                 or (i['F'] < min_max_fuc[0]) or (i['F'] > min_max_fuc[1])
-                or (i['lS']+i['eS'] < min_max_ac[0]) or (i['lS']+i['eS'] > min_max_ac[1])
+                or (i['Am']+i['E'] < min_max_ac[0]) or (i['Am']+i['E'] > min_max_ac[1])
                 or (i['G'] < min_max_gc[0]) or (i['G'] > min_max_gc[1])):
                 to_be_removed.append(i)
         else:
             if ((i['H'] < min_max_hex[0]) or (i['H'] > min_max_hex[1])
                 or (i['N'] < min_max_hexnac[0]) or (i['N'] > min_max_hexnac[1])
                 or (i['S']+i['G'] < min_max_sialics[0])
                 or (i['S']+i['G'] > min_max_sialics[1])
                 or (i['F'] < min_max_fuc[0]) or (i['F'] > min_max_fuc[1])
                 or (i['S'] < min_max_ac[0]) or (i['S'] > min_max_ac[1])
                 or (i['G'] < min_max_gc[0]) or (i['G'] > min_max_gc[1])):
                 to_be_removed.append(i)
     if n_glycan:
         if lactonized_ethyl_esterified:
             for i_i, i in enumerate(glycans):
-                if ((i['lS']+i['eS']+i['G'] > i['N']-2)
-                    or (i['F'] >= i['N']) or (i['lS']+i['eS']+i['G'] > i['H']-2)
+                if ((i['Am']+i['E']+i['G'] > i['N']-2)
+                    or (i['F'] >= i['N']) or (i['Am']+i['E']+i['G'] > i['H']-2)
                     or (i['H'] < 3) or (i['N'] < 2)):
                     if i not in to_be_removed:
                         to_be_removed.append(i)
         else:
             for i_i, i in enumerate(glycans):
                 if ((i['S']+i['G'] > i['N']-2)
                     or (i['F'] >= i['N']) or (i['S']+i['G'] > i['H']-2)
@@ -250,14 +250,23 @@
     full_library : dict
         A dictionary with each key containing the glycan formula and each key containing
         a dictionary with monosaccharides composition, atoms composition with tag,
         neutral mass, neutral mass with tag, isotopic distribution and the mzs of the
         glycans with the desired adducts combination.
     '''
     full_library = {}
+    
+    try:
+        tag_mass = float(tag_mass)
+    except:
+        if tag_mass.split('-')[0] == 'pep':
+            tag_mass = dict(mass.Composition(sequence = tag_mass.split('-')[-1]))
+            tag_mass['H'] -= 2
+            tag_mass['O'] -= 1
+            
     if tag_mass != 0:
         if type(tag_mass) == float:
             tag = General_Functions.calculate_comp_from_mass(tag_mass)
         elif type(tag_mass) != dict:
             comp_tag = General_Functions.form_to_comp(tag_mass)
             tag = (comp_tag, mass.calculate_mass(comp_tag))
         else:
@@ -333,15 +342,15 @@
                 i_neutral_mass = i_neutral_mass+mass.calculate_mass({'H': 2})
         else:
             i_neutral_mass = i_neutral_mass+tag_mass
         i_iso_dist = [[1.0, 0.9, 0.7, 0.4, 0.1], []]
         for i in range(len(i_iso_dist[0])):
             i_iso_dist[1].append(internal_standard+(i*General_Functions.h_mass))
         full_library[i_formula] = {}
-        full_library[i_formula]['Monos_Composition'] = {"H": 0, "N": 0, "S": 0, "lS": 0, "eS": 0, "F": 0, "G": 0}
+        full_library[i_formula]['Monos_Composition'] = {"H": 0, "N": 0, "S": 0, "Am": 0, "E": 0, "F": 0, "G": 0}
         full_library[i_formula]['Neutral_Mass'] = i_neutral_mass
         full_library[i_formula]['Neutral_Mass+Tag'] = i_neutral_mass
         full_library[i_formula]['Isotopic_Distribution'] = i_iso_dist[0]
         full_library[i_formula]['Isotopic_Distribution_Masses'] = i_iso_dist[1]
         full_library[i_formula]['Adducts_mz'] = {}
         for j in adducts_combo:
             charges = sum(j.values())
@@ -463,32 +472,32 @@
     Returns
     -------
     glycans : list
         A list containing dictionaries with informations about each fragment generated.
     '''
     print("Building fragments library...", end = "", flush = True)
     glycans = []
-    def_glycan_comp = {"H": 0, "N": 0, "S": 0, "lS": 0, "eS": 0, "F": 0, "G": 0, "T" : 0}
+    def_glycan_comp = {"H": 0, "N": 0, "S": 0, "Am": 0, "E": 0, "F": 0, "G": 0, "T" : 0}
     for i in range(1, 18):
         if lactonized_ethyl_esterified:
             for j in combinations_with_replacement("HNLEFG", i):
                 glycans.append(General_Functions.sum_monos(def_glycan_comp, General_Functions.count_seq_letters("".join(j))))
         else:
             for j in combinations_with_replacement("HNSFGT", i):
                 glycans.append(General_Functions.sum_monos(def_glycan_comp, General_Functions.count_seq_letters("".join(j))))
     to_be_removed = []
     for i_i, i in enumerate(glycans):
         if lactonized_ethyl_esterified:
             if ((i['T'] > 1) 
                 or (i['T'] == 1 and i['N'] == 0)
                 or (i['H'] > min_max_hex[1])
                 or (i['N'] > min_max_hexnac[1])
-                or (i['lS']+i['eS']+i['G'] > min_max_sialics[1])
+                or (i['Am']+i['E']+i['G'] > min_max_sialics[1])
                 or (i['F'] > min_max_fuc[1])
-                or (i['lS']+i['eS'] > min_max_ac[1])
+                or (i['Am']+i['E'] > min_max_ac[1])
                 or (i['G'] > min_max_gc[1])):
                 to_be_removed.append(i_i)
         else:
             if ((i['T'] > 1) 
                 or (i['T'] == 1 and i['N'] == 0)
                 or (i['H'] > min_max_hex[1])
                 or (i['N'] > min_max_hexnac[1])
@@ -498,41 +507,52 @@
                 or (i['G'] > min_max_gc[1])):
                 to_be_removed.append(i_i)
         if nglycan and i_i not in to_be_removed: #some rules and hardcoded exceptions for N-Glycans
             if lactonized_ethyl_esterified:
                 if ((i['T'] == 1 and sum(i.values()) < 8 and i['S']+i['G'] > 0)
                     or (sum(i.values()) < 6 and i['S'] >= 1 and i['N'] > 1)
                     or (i['H'] > 0 and i['T'] == 1 and i['N'] < 2)
-                    or (i['H'] == 2 and i['N'] == 1 and i['lS']+i['eS'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
-                    or (i['H'] == 0 and i['N'] == 1 and (i['lS']+i['eS'] == 1 or i['G'] == 1) and i['F'] == 0 and i['T'] == 0)
-                    or (i['H'] == 1 and i['N'] == 3 and i['lS']+i['eS'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
-                    or (i['H'] > 1 and i['N'] == 0 and (i['lS']+i['eS'] == 1 or i['G'] == 1) and i['F'] == 0 and i['T'] == 0)
-                    or (i['H'] == 1 and i['N'] == 1 and i['lS']+i['eS'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
-                    or (i['H'] == 3 and i['N'] == 1 and i['lS']+i['eS'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)):
+                    or (i['H'] == 2 and i['N'] == 1 and i['Am']+i['E'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
+                    or (i['H'] == 0 and i['N'] == 1 and (i['Am']+i['E'] == 1 or i['G'] == 1) and i['F'] == 0 and i['T'] == 0)
+                    or (i['H'] == 1 and i['N'] == 3 and i['Am']+i['E'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
+                    or (i['H'] > 1 and i['N'] == 0 and (i['Am']+i['E'] == 1 or i['G'] == 1) and i['F'] == 0 and i['T'] == 0)
+                    or (i['H'] == 1 and i['N'] == 1 and i['Am']+i['E'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
+                    or (i['H'] == 3 and i['N'] == 1 and i['Am']+i['E'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)):
                     to_be_removed.append(i_i)
             else:
                 if ((i['T'] == 1 and sum(i.values()) < 8 and i['S']+i['G'] > 0)
                     or (sum(i.values()) < 6 and i['S'] >= 1 and i['N'] > 1)
                     or (i['H'] > 0 and i['T'] == 1 and i['N'] < 2)
                     or (i['H'] == 2 and i['N'] == 1 and i['S'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
                     or (i['H'] == 0 and i['N'] == 1 and (i['S'] == 1 or i['G'] == 1) and i['F'] == 0 and i['T'] == 0)
                     or (i['H'] == 1 and i['N'] == 3 and i['S'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
                     or (i['H'] > 1 and i['N'] == 0 and (i['S'] == 1 or i['G'] == 1) and i['F'] == 0 and i['T'] == 0)
                     or (i['H'] == 1 and i['N'] == 1 and i['S'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)
                     or (i['H'] == 3 and i['N'] == 1 and i['S'] == 0 and i['F'] == 0 and i['G'] == 0 and i['T'] == 1)):
                     to_be_removed.append(i_i)
     for i in sorted(to_be_removed, reverse = True):
         del glycans[i]
+    try:
+        tag_mass = float(tag_mass)
+    except:
+        if tag_mass.split('-')[0] == 'pep':
+            tag_mass = dict(mass.Composition(sequence = tag_mass.split('-')[-1]))
+            tag_mass['H'] -= 2
+            tag_mass['O'] -= 1
+            
     if tag_mass != 0:
         if type(tag_mass) == float:
             tag = General_Functions.calculate_comp_from_mass(tag_mass)
-        else:
+        elif type(tag_mass) != dict:
             comp_tag = General_Functions.form_to_comp(tag_mass)
             tag = (comp_tag, mass.calculate_mass(comp_tag))
-            tag_mass = tag[1]
+        else:
+            comp_tag = tag_mass
+            tag = (comp_tag, mass.calculate_mass(comp_tag))
+        tag_mass = tag[1]
     else:
         tag = ({"C": 0, "O": 0, "N": 0, "H": 0}, 0.0)
     adducts_combo = General_Functions.gen_adducts_combo({'H' : 2}, [], max_charges)
     frag_library = []
     combo_frags_lib = []
     adducts_mz = [[], [], []]
     for i_i, i in enumerate(glycans):
```

### Comparing `glycogenius-1.1.7/glycogenius/Modules/core.py` & `glycogenius-1.1.8/glycogenius/Modules/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 from . import CLI
 import time
 import os
 import datetime
 
 #-----------------------------------------------------------------------------
 
-def main():
+def main(args=[]):
     try:
-        if not os.isatty(0):
-            args = Config_Handler.config_handler()
-        else:
-            args = CLI.CLI()
+        if len(args) == 0:
+            if not os.isatty(0):
+                args = Config_Handler.config_handler()
+            else:
+                args = CLI.CLI()
             
         begin_time = datetime.datetime.now()
 
         if args[9]:
             Execution_Functions.output_filtered_data(*args[0])
 
         else:
@@ -65,21 +66,22 @@
                 args[6][1] = data
                 args[6][2] = analyzed_data
                 analyzed_data = Execution_Functions.analyze_ms2(*args[6])
             Execution_Functions.print_sep()
             args[7][0] = analyzed_data
             temp_time = Execution_Functions.arrange_raw_data(*args[7])
             Execution_Functions.print_sep()
-            args[0].append(temp_time)
-            Execution_Functions.output_filtered_data(*args[0])
-                                                     
+            args[0][21] = temp_time
+            if len(args) == 11:
+                Execution_Functions.output_filtered_data(*args[0])
+                   
+        print('Execution complete. Time elapsed: '+str(datetime.datetime.now() - begin_time))
         if os.isatty(0):
-            input('Execution complete. Time elapsed: '+str(datetime.datetime.now() - begin_time)+'\nPress Enter to exit.')
+            input('\nPress Enter to exit.')
         else:
-            print('Execution complete. Time elapsed: '+str(datetime.datetime.now() - begin_time))
             print("Close the window or press CTRL+C to exit.")
             try:
                 while True:
                     time.sleep(3600)
             except KeyboardInterrupt:
                 os._exit(1)
     except KeyboardInterrupt:
```

### Comparing `glycogenius-1.1.7/glycogenius/Parameters_Template.py` & `glycogenius-1.1.8/glycogenius/Parameters_Template.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,483 +154,482 @@
 00000990: 6e67 0d0a 3b09 7468 6520 6c69 7374 2028  ng..;.the list (
 000009a0: 6c69 6e65 206f 7220 636f 6d6d 6120 7365  line or comma se
 000009b0: 7061 7261 7465 6429 2e0d 0a3b 094d 6f6e  parated)...;.Mon
 000009c0: 6f73 6163 6368 6172 6964 6573 2061 6363  osaccharides acc
 000009d0: 6570 7465 643a 2048 6578 6f73 6573 2028  epted: Hexoses (
 000009e0: 4829 2c20 0d0a 3b09 4865 784e 4163 2028  H), ..;.HexNAc (
 000009f0: 4e29 2c20 4163 6574 796c 2053 6961 6c69  N), Acetyl Siali
-00000a00: 6320 4163 6964 2028 5320 6f72 206c 5320  c Acid (S or lS 
-00000a10: 616e 6420 6553 0d0a 3b09 6966 2079 6f75  and eS..;.if you
-00000a20: 2068 6176 6520 6c61 6374 6f6e 697a 6564   have lactonized
-00000a30: 2d65 7468 796c 2073 7465 7269 6669 6564  -ethyl sterified
-00000a40: 2067 6c79 6361 6e73 292c 0d0a 3b09 476c   glycans),..;.Gl
-00000a50: 7963 6f6c 796c 2053 6961 6c69 6320 4163  ycolyl Sialic Ac
-00000a60: 6964 2028 4729 2c20 4465 6f78 7968 6578  id (G), Deoxyhex
-00000a70: 6f73 6520 2846 292e 2043 6173 650d 0a3b  ose (F). Case..;
-00000a80: 0973 656e 7369 7469 7665 2e0d 0a3b 092d  .sensitive...;.-
-00000a90: 3e20 4f6e 6c79 206e 6565 6465 6420 696e  > Only needed in
-00000aa0: 2063 7573 746f 6d5f 6c69 6272 6172 7920   custom_library 
-00000ab0: 6d6f 6465 2e20 0d0a 3b0d 0a74 6f74 616c  mode. ..;..total
-00000ac0: 5f6d 6f6e 6f73 6163 6368 6172 6964 6573  _monosaccharides
-00000ad0: 203d 2035 2c20 3232 0d0a 6865 786f 7365   = 5, 22..hexose
-00000ae0: 7320 3d20 332c 2031 300d 0a68 6578 6e61  s = 3, 10..hexna
-00000af0: 6373 203d 2032 2c20 380d 0a73 6961 6c69  cs = 2, 8..siali
-00000b00: 635f 6163 6964 7320 3d20 302c 2034 0d0a  c_acids = 0, 4..
-00000b10: 6675 636f 7365 7320 3d20 302c 2032 0d0a  fucoses = 0, 2..
-00000b20: 6e65 7535 6163 203d 2030 2c20 340d 0a6e  neu5ac = 0, 4..n
-00000b30: 6575 3567 6320 3d20 302c 2030 0d0a 3b20  eu5gc = 0, 0..; 
-00000b40: 0953 7065 6369 6679 2074 6865 206d 696e  .Specify the min
-00000b50: 696d 756d 2061 6e64 206d 6178 696d 756d  imum and maximum
-00000b60: 206d 6f6e 6f73 6163 6368 6172 6964 6573   monosaccharides
-00000b70: 0d0a 3b09 616d 6f75 6e74 7320 666f 7220  ..;.amounts for 
-00000b80: 6765 6e65 7261 7469 6e67 2061 206c 6962  generating a lib
-00000b90: 7261 7279 2e0d 0a3b 092d 3e20 4f6e 6c79  rary...;.-> Only
-00000ba0: 206e 6565 6465 6420 696e 2067 656e 6572   needed in gener
-00000bb0: 6174 655f 6c69 6272 6172 7920 6d6f 6465  ate_library mode
-00000bc0: 2e0d 0a3b 0d0a 0d0a 5b63 6f6d 6d6f 6e5f  ...;....[common_
-00000bd0: 6c69 6272 6172 795f 6275 696c 6469 6e67  library_building
-00000be0: 5f73 6574 7469 6e67 735d 0d0a 666f 7263  _settings]..forc
-00000bf0: 655f 6e67 6c79 6361 6e20 3d20 7965 730d  e_nglycan = yes.
-00000c00: 0a3b 2009 5573 6564 2074 6f20 666f 7263  .; .Used to forc
-00000c10: 6520 736f 6d65 206d 6f6e 6f73 6163 6368  e some monosacch
-00000c20: 6172 6964 6573 2063 6f6d 706f 7369 7469  arides compositi
-00000c30: 6f6e 730d 0a3b 0961 7373 6f63 6961 7465  ons..;.associate
-00000c40: 6420 7769 7468 204e 2d47 6c79 6361 6e73  d with N-Glycans
-00000c50: 2062 696f 6c6f 6769 6361 6c6c 7920 6b6e   biologically kn
-00000c60: 6f77 6e20 0d0a 3b09 6665 6174 7572 6573  own ..;.features
-00000c70: 2e20 4966 206e 6f74 2075 7365 642c 2067  . If not used, g
-00000c80: 6976 6573 2061 206d 7563 6820 6272 6f61  ives a much broa
-00000c90: 6465 7220 0d0a 3b09 6c69 6272 6172 7920  der ..;.library 
-00000ca0: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
-00000cb0: 2066 6f72 2061 6e61 6c79 7369 7320 6f66   for analysis of
-00000cc0: 200d 0a3b 094f 2d47 6c79 6361 6e73 2c20   ..;.O-Glycans, 
-00000cd0: 666f 7220 6578 616d 706c 652e 0d0a 3b0d  for example...;.
-00000ce0: 0a6d 6178 5f61 6464 7563 7473 203d 2048  .max_adducts = H
-00000cf0: 330d 0a61 6464 7563 7473 5f65 7863 6c75  3..adducts_exclu
-00000d00: 7369 6f6e 203d 200d 0a3b 2009 496e 6469  sion = ..; .Indi
-00000d10: 6361 7465 7320 7468 6520 6465 7369 7265  cates the desire
-00000d20: 6420 6164 6475 6374 7320 616e 6420 7468  d adducts and th
-00000d30: 6569 7220 6d61 7869 6d75 6d0d 0a3b 0961  eir maximum..;.a
-00000d40: 6d6f 756e 742e 2048 334e 6131 206d 6561  mount. H3Na1 mea
-00000d50: 6e73 2061 206d 6178 696d 756d 206f 6620  ns a maximum of 
-00000d60: 3320 4879 6472 6f67 656e 7320 616e 640d  3 Hydrogens and.
-00000d70: 0a3b 0961 206d 6178 696d 756d 206f 6620  .;.a maximum of 
-00000d80: 3120 536f 6469 756d 2070 6572 2061 6464  1 Sodium per add
-00000d90: 7563 7420 636f 6d62 696e 6174 696f 6e2e  uct combination.
-00000da0: 200d 0a3b 0943 6173 6520 7365 6e73 6974   ..;.Case sensit
-00000db0: 6976 652e 2044 6f65 736e 2774 2077 6f72  ive. Doesn't wor
-00000dc0: 6b20 7769 7468 2063 6f6d 706c 6578 2061  k with complex a
-00000dd0: 6464 7563 7473 2c0d 0a3b 0973 7563 6820  dducts,..;.such 
-00000de0: 6173 204e 4834 2e20 5365 7420 6164 6475  as NH4. Set addu
-00000df0: 6374 7320 696e 2027 6164 6475 6374 735f  cts in 'adducts_
-00000e00: 6578 636c 7573 696f 6e27 2074 6f0d 0a3b  exclusion' to..;
-00000e10: 0961 766f 6964 2075 7369 6e67 2073 7065  .avoid using spe
-00000e20: 6369 6669 6320 6164 6475 6374 732e 2043  cific adducts. C
-00000e30: 6f6d 6d61 2073 6570 6172 6174 6564 206c  omma separated l
-00000e40: 6973 742e 0d0a 3b0d 0a6d 6178 5f63 6861  ist...;..max_cha
-00000e50: 7267 6573 203d 2033 0d0a 3b20 094c 696d  rges = 3..; .Lim
-00000e60: 6974 7320 7468 6520 6d61 7869 6d75 6d20  its the maximum 
-00000e70: 616d 6f75 6e74 206f 6620 6361 6c63 756c  amount of calcul
-00000e80: 6174 6564 2063 6861 7267 6573 0d0a 3b09  ated charges..;.
-00000e90: 666f 7220 6561 6368 2067 6c79 6361 6e2e  for each glycan.
-00000ea0: 2053 6574 2074 6f20 6120 6e65 6761 7469   Set to a negati
-00000eb0: 7665 2076 616c 7565 2069 6620 796f 750d  ve value if you.
-00000ec0: 0a3b 0977 616e 7420 746f 2064 6f20 6e65  .;.want to do ne
-00000ed0: 6761 7469 7665 206d 6f64 6520 616e 616c  gative mode anal
-00000ee0: 7973 6973 205b 4558 5045 5249 4d45 4e54  ysis [EXPERIMENT
-00000ef0: 414c 5d2e 0d0a 3b0d 0a72 6564 7563 696e  AL]...;..reducin
-00000f00: 675f 656e 645f 7461 6720 3d20 3133 332e  g_end_tag = 133.
-00000f10: 3036 3434 0d0a 3b20 0949 6620 6120 7265  0644..; .If a re
-00000f20: 6475 6369 6e67 2065 6e64 2074 6167 2069  ducing end tag i
-00000f30: 7320 6164 6465 6420 746f 2074 6865 2067  s added to the g
-00000f40: 6c79 6361 6e73 2c20 0d0a 3b20 0969 6e73  lycans, ..; .ins
-00000f50: 6572 7420 6974 7320 6164 6465 6420 6d61  ert its added ma
-00000f60: 7373 206f 7220 6d6f 6c65 6375 6c61 7220  ss or molecular 
-00000f70: 666f 726d 756c 6120 6865 7265 2e0d 0a3b  formula here...;
-00000f80: 0949 6620 6e6f 2072 6564 7563 696e 6720  .If no reducing 
-00000f90: 656e 6420 7461 6720 6973 2061 6464 6564  end tag is added
-00000fa0: 2074 6f20 7468 6520 676c 7963 616e 732c   to the glycans,
-00000fb0: 200d 0a3b 0973 6574 2074 6869 7320 7661   ..;.set this va
-00000fc0: 6c75 6520 746f 2030 2e20 5072 6f63 6169  lue to 0. Procai
-00000fd0: 6e61 6d69 6465 3a20 3231 392e 3137 3335  namide: 219.1735
-00000fe0: 206f 720d 0a3b 0943 3133 4832 314e 333b   or..;.C13H21N3;
-00000ff0: 2047 6972 6172 6420 5265 6167 656e 7420   Girard Reagent 
-00001000: 503a 2031 3333 2e30 3634 3420 6f72 2043  P: 133.0644 or C
-00001010: 3748 374e 3320 0d0a 3b09 2864 6570 726f  7H7N3 ..;.(depro
-00001020: 746f 6e61 7465 642c 206e 6575 7472 616c  tonated, neutral
-00001030: 292e 2043 616e 2061 6c73 6f20 6265 2075  ). Can also be u
-00001040: 7365 6420 7769 7468 200d 0a3b 0961 2070  sed with ..;.a p
-00001050: 6570 7469 6465 2062 7920 696e 7075 7469  eptide by inputi
-00001060: 6e67 2027 7065 702d 2720 2b20 7468 6520  ng 'pep-' + the 
-00001070: 7065 7469 6465 200d 0a3b 0973 6571 7565  petide ..;.seque
-00001080: 6e63 6520 2869 652e 2027 7065 702d 4e4b  nce (ie. 'pep-NK
-00001090: 2720 666f 7220 7468 6520 7065 7074 6964  ' for the peptid
-000010a0: 6520 4e4b 292e 0d0a 3b0d 0a70 6572 6d65  e NK)...;..perme
-000010b0: 7468 796c 6174 6564 203d 206e 6f0d 0a3b  thylated = no..;
-000010c0: 2009 4966 2074 6865 2073 616d 706c 6520   .If the sample 
-000010d0: 7761 7320 7065 726d 6574 6879 6c61 7465  was permethylate
-000010e0: 642c 2073 6574 2074 6869 7320 0d0a 3b09  d, set this ..;.
-000010f0: 7061 7261 6d65 7465 7220 746f 2022 7965  parameter to "ye
-00001100: 7322 2e20 446f 6573 6e27 7420 7461 6b65  s". Doesn't take
-00001110: 2069 6e74 6f20 6163 636f 756e 7420 0d0a   into account ..
-00001120: 3b09 7061 7274 6961 6c20 7065 726d 6574  ;.partial permet
-00001130: 6879 6c61 7469 6f6e 732e 0d0a 3b0d 0a72  hylations...;..r
-00001140: 6564 7563 6564 203d 206e 6f0d 0a3b 2009  educed = no..; .
-00001150: 4966 2074 6865 2073 616d 706c 6520 646f  If the sample do
-00001160: 6573 6e27 7420 6861 7665 2061 2074 6167  esn't have a tag
-00001170: 2061 6e64 2074 6865 2067 6c79 6361 6e73   and the glycans
-00001180: 0d0a 3b09 6861 6420 7468 6569 7220 7265  ..;.had their re
-00001190: 6475 6369 6e67 2065 6e64 2072 6564 7563  ducing end reduc
-000011a0: 6564 2c20 7365 7420 7468 6973 2074 6f20  ed, set this to 
-000011b0: 2279 6573 222e 0d0a 3b0d 0a6c 6163 746f  "yes"...;..lacto
-000011c0: 6e69 7a65 645f 6574 6879 6c5f 6573 7465  nized_ethyl_este
-000011d0: 7269 6669 6564 203d 206e 6f0d 0a3b 2009  rified = no..; .
-000011e0: 5573 6520 6966 2074 6865 2073 6961 6c69  Use if the siali
-000011f0: 6320 6163 6964 7320 7765 7265 2064 6572  c acids were der
-00001200: 6976 6974 697a 6564 2077 6974 6820 0d0a  ivitized with ..
-00001210: 3b09 6c61 6374 6f6e 697a 6174 696f 6e20  ;.lactonization 
-00001220: 2861 6c70 6861 322c 3329 2061 6e64 2065  (alpha2,3) and e
-00001230: 7468 796c 2065 7374 6572 6966 6963 6174  thyl esterificat
-00001240: 696f 6e20 0d0a 3b09 2861 6c70 6861 322c  ion ..;.(alpha2,
-00001250: 3629 2e20 4c61 6374 6f6e 697a 6564 2041  6). Lactonized A
-00001260: 6365 7479 6c20 5369 616c 6963 2041 6369  cetyl Sialic Aci
-00001270: 6420 7769 6c6c 0d0a 3b09 6265 2069 6465  d will..;.be ide
-00001280: 6e74 6966 6965 6420 6173 2027 6c53 2720  ntified as 'lS' 
-00001290: 616e 6420 4574 6879 6c20 4573 7465 7269  and Ethyl Esteri
-000012a0: 6669 6564 2041 6365 7479 6c0d 0a3b 0953  fied Acetyl..;.S
-000012b0: 6961 6c69 6320 4163 6964 2077 696c 6c20  ialic Acid will 
-000012c0: 6265 2069 6465 6e74 6966 6965 6420 6173  be identified as
-000012d0: 2027 6553 272e 0d0a 3b0d 0a66 6173 745f   'eS'...;..fast_
-000012e0: 6973 6f20 3d20 7965 730d 0a3b 2009 416c  iso = yes..; .Al
-000012f0: 6c6f 7773 2079 6f75 2074 6f20 6361 6c63  lows you to calc
-00001300: 756c 6174 6520 7468 6520 6973 6f74 6f70  ulate the isotop
-00001310: 6963 2064 6973 7472 6962 7574 696f 6e0d  ic distribution.
-00001320: 0a3b 096f 6620 676c 7963 616e 7320 6261  .;.of glycans ba
-00001330: 7365 6420 6f6e 6c79 206f 6e20 6361 7262  sed only on carb
-00001340: 6f6e 2069 736f 746f 7065 7320 2866 6173  on isotopes (fas
-00001350: 742c 200d 0a3b 0969 6e6e 6163 7572 6174  t, ..;.innacurat
-00001360: 6529 2061 6e64 2063 6f72 7265 6374 6564  e) and corrected
-00001370: 2061 7274 6966 6963 6961 6c6c 7920 6f72   artificially or
-00001380: 206f 6e20 616c 6c20 0d0a 3b09 7468 6520   on all ..;.the 
-00001390: 6174 6f6d 7320 6973 6f74 6f70 6573 2028  atoms isotopes (
-000013a0: 5645 5259 2053 4c4f 572c 2076 6572 7920  VERY SLOW, very 
-000013b0: 6163 6375 7261 7465 292e 200d 0a3b 0949  accurate). ..;.I
-000013c0: 6620 6e6f 7420 7573 6564 2c20 6c69 6272  f not used, libr
-000013d0: 6172 7920 6275 696c 6469 6e67 206d 6179  ary building may
-000013e0: 2074 616b 6520 6d61 6e79 2068 6f75 7273   take many hours
-000013f0: 0d0a 3b09 6465 7065 6e64 696e 6720 6f6e  ..;.depending on
-00001400: 2073 697a 652e 0d0a 3b0d 0a68 6967 685f   size...;..high_
-00001410: 7265 736f 6c75 7469 6f6e 5f69 736f 746f  resolution_isoto
-00001420: 7069 635f 6469 7374 203d 206e 6f0d 0a3b  pic_dist = no..;
-00001430: 2009 4966 206e 6f74 2075 7365 642c 2064   .If not used, d
-00001440: 6f65 736e 2774 2063 6c75 6d70 2069 736f  oesn't clump iso
-00001450: 746f 7065 2070 6561 6b73 200d 0a3b 0974  tope peaks ..;.t
-00001460: 6f67 6574 6865 722c 206d 6561 6e69 6e67  ogether, meaning
-00001470: 2074 6861 7420 796f 7527 6c6c 2068 6176   that you'll hav
-00001480: 6520 6d6f 7265 2074 6861 6e20 6f6e 6520  e more than one 
-00001490: 0d0a 3b09 6973 6f74 6f70 6963 2070 6561  ..;.isotopic pea
-000014a0: 6b20 696e 2061 2031 2044 6120 696e 7465  k in a 1 Da inte
-000014b0: 7276 616c 2e20 4f6e 6c79 2075 7365 2074  rval. Only use t
-000014c0: 6869 7320 0d0a 3b09 6966 2079 6f75 2068  his ..;.if you h
-000014d0: 6176 6520 6661 7374 5f69 736f 206f 6666  ave fast_iso off
-000014e0: 2e20 5573 6566 756c 2077 6865 6e20 616e  . Useful when an
-000014f0: 616c 797a 696e 6720 0d0a 3b09 7665 7279  alyzing ..;.very
-00001500: 2068 6967 6820 7265 736f 6c75 7469 6f6e   high resolution
-00001510: 2064 6174 612c 2073 7563 6820 6173 2064   data, such as d
-00001520: 6174 6120 6163 7175 6972 6564 200d 0a3b  ata acquired ..;
-00001530: 096f 6e20 4654 206d 6173 7320 7370 6563  .on FT mass spec
-00001540: 7472 6f6d 6574 6572 732e 0d0a 3b0d 0a69  trometers...;..i
-00001550: 6e74 6572 6e61 6c5f 7374 616e 6461 7264  nternal_standard
-00001560: 5f6d 6173 7320 3d20 302e 300d 0a3b 2009  _mass = 0.0..; .
-00001570: 4966 2075 7369 6e67 2061 6e20 696e 7465  If using an inte
-00001580: 726e 616c 2073 7461 6e64 6172 642c 2069  rnal standard, i
-00001590: 6e73 6572 7420 6974 7320 6d61 7373 200d  nsert its mass .
-000015a0: 0a3b 0968 6572 6520 666f 7220 7468 6520  .;.here for the 
-000015b0: 7363 7269 7074 2074 6f20 6361 6c63 756c  script to calcul
-000015c0: 6174 6520 6974 7320 6172 6561 2e20 5468  ate its area. Th
-000015d0: 6973 200d 0a3b 0961 6c73 6f20 616c 6c6f  is ..;.also allo
-000015e0: 7773 2074 6865 2073 6372 6970 7420 746f  ws the script to
-000015f0: 206f 7574 7075 7420 6120 6e6f 726d 616c   output a normal
-00001600: 697a 6564 200d 0a3b 096d 6574 6162 6f61  ized ..;.metaboa
-00001610: 6e61 6c79 7374 2063 6f6d 7061 7469 626c  nalyst compatibl
-00001620: 6520 6669 6c65 2e0d 0a3b 0d0a 0d0a 5b61  e file...;....[a
-00001630: 6e61 6c79 7369 735f 7061 7261 6d65 7465  nalysis_paramete
-00001640: 7273 5d0d 0a61 6e61 6c79 7a65 5f6d 7332  rs]..analyze_ms2
-00001650: 203d 2079 6573 0d0a 666f 7263 655f 6672   = yes..force_fr
-00001660: 6167 6d65 6e74 735f 746f 5f67 6c79 6361  agments_to_glyca
-00001670: 6e73 203d 2079 6573 0d0a 756e 7265 7374  ns = yes..unrest
-00001680: 7269 6374 6564 5f66 7261 676d 656e 7473  ricted_fragments
-00001690: 203d 206e 6f0d 0a3b 2009 416c 6c6f 7773   = no..; .Allows
-000016a0: 2074 6f20 616e 616c 797a 6520 6d73 3220   to analyze ms2 
-000016b0: 6461 7461 2c20 6173 2077 656c 6c2e 2046  data, as well. F
-000016c0: 7261 676d 656e 7473 200d 0a3b 0969 6465  ragments ..;.ide
-000016d0: 6e74 6966 6965 6420 7769 6c6c 2062 6520  ntified will be 
-000016e0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-000016f0: 6561 6368 2067 6c79 6361 6e2e 200d 0a3b  each glycan. ..;
-00001700: 0959 6f75 2063 616e 2063 686f 6f73 6520  .You can choose 
-00001710: 746f 2066 696c 7465 7220 6964 656e 7469  to filter identi
-00001720: 6669 6564 2066 7261 676d 656e 7473 2062  fied fragments b
-00001730: 7920 0d0a 3b09 6d6f 6e6f 7361 6363 6861  y ..;.monosaccha
-00001740: 7269 6465 7320 636f 6d70 6f73 6974 696f  rides compositio
-00001750: 6e73 2c20 696e 206f 7264 6572 2074 6f20  ns, in order to 
-00001760: 6176 6f69 6420 0d0a 3b09 7265 706f 7274  avoid ..;.report
-00001770: 696e 6720 6672 6167 6d65 6e74 7320 7468  ing fragments th
-00001780: 6174 2061 7265 6e27 7420 636f 6d70 6174  at aren't compat
-00001790: 6962 6c65 2077 6974 6820 0d0a 3b09 6465  ible with ..;.de
-000017a0: 7465 6374 6564 2070 7265 6375 7273 6f72  tected precursor
-000017b0: 2e20 4966 2075 6e72 6573 7472 6963 7465  . If unrestricte
-000017c0: 645f 6672 6167 6d65 6e74 7320 6973 200d  d_fragments is .
-000017d0: 0a3b 0975 7365 642c 2069 7420 7365 6172  .;.used, it sear
-000017e0: 6368 6573 2066 6f72 2067 6c79 6361 6e73  ches for glycans
-000017f0: 2069 6e20 6576 6572 7920 6d73 3220 7363   in every ms2 sc
-00001800: 616e 2c20 0d0a 3b09 7265 6761 7264 6c65  an, ..;.regardle
-00001810: 7373 2069 6620 7468 6520 676c 7963 616e  ss if the glycan
-00001820: 2077 6173 2066 6f75 6e64 2069 6e20 6675   was found in fu
-00001830: 6c6c 2073 6361 6e2e 200d 0a3b 0954 6869  ll scan. ..;.Thi
-00001840: 7320 7769 6c6c 2074 616b 6520 6120 6269  s will take a bi
-00001850: 7420 6c6f 6e67 6572 2e20 0d0a 3b0d 0a61  t longer. ..;..a
-00001860: 6363 7572 6163 795f 756e 6974 203d 2070  ccuracy_unit = p
-00001870: 706d 0d0a 3b20 0944 6574 6572 6d69 6e65  pm..; .Determine
-00001880: 7320 7468 6520 756e 6974 7320 6f66 206d  s the units of m
-00001890: 7a20 746f 6c65 7261 6e63 6520 746f 2062  z tolerance to b
-000018a0: 6520 7573 6564 200d 0a3b 0962 7920 7468  e used ..;.by th
-000018b0: 6520 7363 7269 7074 2e20 4f70 7469 6f6e  e script. Option
-000018c0: 733a 2027 7070 6d27 206f 7220 2770 7727  s: 'ppm' or 'pw'
-000018d0: 2e20 0d0a 3b09 2770 706d 2720 3d20 5061  . ..;.'ppm' = Pa
-000018e0: 7274 6963 6c65 7320 7065 7220 4d69 6c6c  rticles per Mill
-000018f0: 696f 6e2c 2077 6865 7265 2031 3020 7070  ion, where 10 pp
-00001900: 6d20 6973 200d 0a3b 0961 726f 756e 6420  m is ..;.around 
-00001910: 302e 3031 206d 7a20 746f 6c65 7261 6e63  0.01 mz toleranc
-00001920: 6520 6174 206d 7a20 3130 3030 2c20 276d  e at mz 1000, 'm
-00001930: 7a27 203d 2046 6978 6564 200d 0a3b 096d  z' = Fixed ..;.m
-00001940: 7a20 746f 6c65 7261 6e63 6520 6672 6f6d  z tolerance from
-00001950: 2063 656e 7472 6f69 642c 2030 2e30 3120   centroid, 0.01 
-00001960: 6d7a 206d 6561 6e73 2069 7420 0d0a 3b09  mz means it ..;.
-00001970: 746f 6c65 7261 7465 7320 6120 302e 3031  tolerates a 0.01
-00001980: 2076 6172 6961 6e63 6520 696e 206d 7a0d   variance in mz.
-00001990: 0a3b 0d0a 6163 6375 7261 6379 5f76 616c  .;..accuracy_val
-000019a0: 7565 203d 2031 300d 0a3b 2009 5468 6520  ue = 10..; .The 
-000019b0: 7661 6c75 6520 666f 7220 7468 6520 6163  value for the ac
-000019c0: 6375 7261 6379 5f75 6e69 7420 7061 7261  curacy_unit para
-000019d0: 6d65 7465 722e 2059 6f75 200d 0a3b 0963  meter. You ..;.c
-000019e0: 616e 2075 7365 2061 2062 726f 6164 6572  an use a broader
-000019f0: 2061 6363 7572 6163 7920 7661 6c75 6520   accuracy value 
-00001a00: 616e 6420 7468 656e 2066 696c 7465 7220  and then filter 
-00001a10: 0d0a 3b09 7261 7720 6461 7461 2075 7369  ..;.raw data usi
-00001a20: 6e67 206d 6178 5f70 706d 2c20 6275 7420  ng max_ppm, but 
-00001a30: 7468 6973 206d 6179 206c 6561 6420 746f  this may lead to
-00001a40: 200d 0a3b 0966 616c 7365 2070 6f73 6974   ..;.false posit
-00001a50: 6976 6573 2e0d 0a3b 0d0a 7265 745f 7469  ives...;..ret_ti
-00001a60: 6d65 5f69 6e74 6572 7661 6c20 3d20 312c  me_interval = 1,
-00001a70: 2039 3939 0d0a 3b20 0954 6865 206d 696e   999..; .The min
-00001a80: 696d 756d 2061 6e64 206d 6178 696d 756d  imum and maximum
-00001a90: 2072 6574 656e 7469 6f6e 2074 696d 652c   retention time,
-00001aa0: 2069 6e20 4d49 4e55 5445 532c 200d 0a3b   in MINUTES, ..;
-00001ab0: 0975 7365 6420 666f 7220 7661 7269 6f75  .used for variou
-00001ac0: 7320 706f 7274 696f 6e73 206f 6620 7468  s portions of th
-00001ad0: 6520 7363 7269 7074 2e20 4120 7368 6f72  e script. A shor
-00001ae0: 7465 7220 0d0a 3b09 696e 7465 7276 616c  ter ..;.interval
-00001af0: 206f 6620 7265 745f 7469 6d65 206d 616b   of ret_time mak
-00001b00: 6573 2074 6865 2073 6372 6970 7420 7275  es the script ru
-00001b10: 6e20 6661 7374 6572 2c20 0d0a 3b09 736f  n faster, ..;.so
-00001b20: 2074 7279 2074 6f20 7472 696d 2079 6f75   try to trim you
-00001b30: 7220 7361 6d70 6c65 2061 7320 6d75 6368  r sample as much
-00001b40: 2061 7320 706f 7373 6962 6c65 2c20 0d0a   as possible, ..
-00001b50: 3b09 6966 2079 6f75 206b 6e6f 7720 7768  ;.if you know wh
-00001b60: 656e 2079 6f75 7220 616e 616c 7974 6573  en your analytes
-00001b70: 2061 7265 206c 6561 7669 6e67 2074 6865   are leaving the
-00001b80: 200d 0a3b 0963 6f6c 756d 6e2e 0d0a 3b0d   ..;.column...;.
-00001b90: 0a63 7573 746f 6d5f 6d69 6e5f 706f 696e  .custom_min_poin
-00001ba0: 7473 5f70 6572 5f70 6561 6b20 3d20 6e6f  ts_per_peak = no
-00001bb0: 0d0a 6e75 6d62 6572 5f70 6f69 6e74 735f  ..number_points_
-00001bc0: 7065 725f 7065 616b 203d 2035 0d0a 3b20  per_peak = 5..; 
-00001bd0: 0949 6620 7573 6564 2c20 7365 7420 7468  .If used, set th
-00001be0: 6520 6d69 6e69 6d75 6d20 6e75 6d62 6572  e minimum number
-00001bf0: 206f 6620 6461 7461 706f 696e 7473 2074   of datapoints t
-00001c00: 6f20 0d0a 3b09 636f 6e73 6964 6572 2061  o ..;.consider a
-00001c10: 2063 6872 6f6d 6174 6f67 7261 6d20 7065   chromatogram pe
-00001c20: 616b 2070 6172 7420 6f66 2074 6865 2072  ak part of the r
-00001c30: 6177 200d 0a3b 0964 6174 6173 6574 2e20  aw ..;.dataset. 
-00001c40: 4966 206c 6566 7420 6f6e 2046 616c 7365  If left on False
-00001c50: 2069 7420 6361 6c63 756c 6174 6573 200d   it calculates .
-00001c60: 0a3b 0961 7574 6f6d 6174 6963 616c 6c79  .;.automatically
-00001c70: 2e0d 0a3b 0d0a 6c69 6d69 745f 7065 616b  ...;..limit_peak
-00001c80: 735f 7069 636b 6564 203d 2079 6573 0d0a  s_picked = yes..
-00001c90: 6d61 785f 6e75 6d62 6572 5f70 6561 6b73  max_number_peaks
-00001ca0: 203d 2035 0d0a 3b20 0949 6620 7573 6564   = 5..; .If used
-00001cb0: 2c20 7069 636b 7320 6f6e 6c79 2074 6865  , picks only the
-00001cc0: 206d 6f73 7420 696e 7465 6e73 6520 7065   most intense pe
-00001cd0: 616b 206f 6e20 7468 6520 0d0a 3b09 4549  ak on the ..;.EI
-00001ce0: 4320 616e 6420 7570 2074 6f20 5b6d 6178  C and up to [max
-00001cf0: 5f6e 756d 6265 725f 7065 616b 735d 2d31  _number_peaks]-1
-00001d00: 206f 7468 6572 2070 6561 6b73 200d 0a3b   other peaks ..;
-00001d10: 0963 6c6f 7365 7374 2074 6f20 6974 2e20  .closest to it. 
-00001d20: 5761 726e 696e 673a 2054 6869 7320 6d61  Warning: This ma
-00001d30: 7920 7265 6475 6365 2074 6865 2072 616e  y reduce the ran
-00001d40: 6765 200d 0a3b 096f 6620 796f 7572 2072  ge ..;.of your r
-00001d50: 6573 756c 7473 2e0d 0a3b 0d0a 0d0a 5b70  esults...;....[p
-00001d60: 6f73 742d 616e 616c 7973 6973 2f72 6561  ost-analysis/rea
-00001d70: 6e61 6c79 7369 735d 0d0a 6669 6c74 6572  nalysis]..filter
-00001d80: 5f6d 7332 5f62 795f 7265 706f 7274 6572  _ms2_by_reporter
-00001d90: 5f69 6f6e 7320 3d20 4e31 5431 2c20 3336  _ions = N1T1, 36
-00001da0: 362e 3134 0d0a 3b09 5365 7420 7265 706f  6.14..;.Set repo
-00001db0: 7274 6572 2069 6f6e 7320 746f 2068 6964  rter ions to hid
-00001dc0: 6520 4d53 3220 7370 6563 7472 6120 7468  e MS2 spectra th
-00001dd0: 6174 2064 6f6e 2774 0d0a 3b09 636f 6e74  at don't..;.cont
-00001de0: 6169 6e20 7468 656d 2e20 4361 6e20 6265  ain them. Can be
-00001df0: 2062 6173 6564 2077 6974 6820 676c 7963   based with glyc
-00001e00: 616e 7320 666f 726d 756c 6120 0d0a 3b09  ans formula ..;.
-00001e10: 2877 6974 6820 5420 6265 696e 6720 7468  (with T being th
-00001e20: 6520 7265 6475 6369 6e67 2065 6e64 206f  e reducing end o
-00001e30: 6620 7468 6520 676c 7963 616e 2c20 0d0a  f the glycan, ..
-00001e40: 3b09 696e 636c 7564 696e 6720 706f 7373  ;.including poss
-00001e50: 6962 6c79 2074 6865 2074 6167 2c20 6966  ibly the tag, if
-00001e60: 2075 7365 6429 206f 7220 616e 206d 7a2e   used) or an mz.
-00001e70: 0d0a 3b09 0d0a 616c 6967 6e5f 6368 726f  ..;...align_chro
-00001e80: 6d61 746f 6772 616d 7320 3d20 7965 730d  matograms = yes.
-00001e90: 0a3b 2009 4966 2065 6e61 626c 6564 2c20  .; .If enabled, 
-00001ea0: 7769 6c6c 2061 6c69 676e 2074 6865 2061  will align the a
-00001eb0: 7373 6967 6e6d 656e 7473 2061 6e64 2064  ssignments and d
-00001ec0: 7261 776e 200d 0a3b 0970 726f 6365 7373  rawn ..;.process
-00001ed0: 6564 2045 4943 7320 6f66 2074 6865 2064  ed EICs of the d
-00001ee0: 6966 6665 7265 6e74 2073 616d 706c 6573  ifferent samples
-00001ef0: 2e20 5468 6520 0d0a 3b09 616c 6967 6e6d  . The ..;.alignm
-00001f00: 656e 7420 6973 2068 6967 686c 7920 6465  ent is highly de
-00001f10: 7065 6e64 656e 7420 6f6e 2074 6865 2066  pendent on the f
-00001f20: 6561 7475 7265 7320 0d0a 3b09 6964 656e  eatures ..;.iden
-00001f30: 7469 6669 6564 2061 6e64 2074 6865 6972  tified and their
-00001f40: 2069 6e68 6572 656e 7420 7175 616c 6974   inherent qualit
-00001f50: 792c 2073 6f20 7468 696e 6773 200d 0a3b  y, so things ..;
-00001f60: 0977 696c 6c20 6368 616e 6765 2077 6974  .will change wit
-00001f70: 6820 6469 6666 6572 656e 7420 7175 616c  h different qual
-00001f80: 6974 7920 7468 7265 7368 6f6c 6473 2e20  ity thresholds. 
-00001f90: 0d0a 3b0d 0a61 7563 5f70 6572 6365 6e74  ..;..auc_percent
-00001fa0: 6167 655f 7468 7265 7368 6f6c 6420 3d20  age_threshold = 
-00001fb0: 310d 0a3b 2009 416c 6c6f 7773 2079 6f75  1..; .Allows you
-00001fc0: 2074 6f20 7375 7072 6573 7320 6672 6f6d   to supress from
-00001fd0: 2074 6865 2061 6e61 6c79 7369 7320 7065   the analysis pe
-00001fe0: 616b 7320 0d0a 3b09 7468 6174 2061 7265  aks ..;.that are
-00001ff0: 206f 6620 7468 6520 7370 6563 6966 6965   of the specifie
-00002000: 6420 7065 7263 656e 7461 6765 2028 6672  d percentage (fr
-00002010: 6f6d 2030 2520 746f 0d0a 3b09 3130 3025  om 0% to..;.100%
-00002020: 2920 6172 6561 2075 6e64 6572 2063 7572  ) area under cur
-00002030: 7665 2072 656c 6174 6564 2074 6f20 7468  ve related to th
-00002040: 6520 6d6f 7374 2069 6e74 656e 7365 0d0a  e most intense..
-00002050: 3b09 7065 616b 2061 7265 6120 7769 7468  ;.peak area with
-00002060: 696e 2074 6865 2073 616d 6520 6164 6475  in the same addu
-00002070: 6374 2028 6965 2e20 6966 2062 6967 6765  ct (ie. if bigge
-00002080: 7374 200d 0a3b 0970 6561 6b20 6861 7320  st ..;.peak has 
-00002090: 6120 6172 6561 2075 6e64 6572 2063 7572  a area under cur
-000020a0: 7665 206f 6620 3130 3020 616e 6420 0d0a  ve of 100 and ..
-000020b0: 3b09 6175 635f 7065 7263 656e 7461 6765  ;.auc_percentage
-000020c0: 5f74 6872 6573 686f 6c64 2069 7320 7365  _threshold is se
-000020d0: 7420 746f 2031 252c 2065 7665 7279 2070  t to 1%, every p
-000020e0: 6561 6b20 0d0a 3b09 7769 7468 2061 6e20  eak ..;.with an 
-000020f0: 6175 6320 6f66 2031 2061 6e64 2062 656c  auc of 1 and bel
-00002100: 6f77 2077 696c 6c20 6265 2073 7570 7265  ow will be supre
-00002110: 7373 6564 290d 0a3b 0d0a 6d61 785f 7070  ssed)..;..max_pp
-00002120: 6d5f 7468 7265 7368 6f6c 6420 3d20 3130  m_threshold = 10
-00002130: 0d0a 3b20 094d 6178 696d 756d 2050 504d  ..; .Maximum PPM
-00002140: 2065 7272 6f72 2066 6f72 2064 6174 6120   error for data 
-00002150: 6375 7261 7469 6f6e 2e20 4966 2076 616c  curation. If val
-00002160: 7565 2069 7320 0d0a 3b09 6772 6561 7465  ue is ..;.greate
-00002170: 7220 7468 616e 2065 7175 6976 616c 656e  r than equivalen
-00002180: 7420 6163 6375 7261 6379 5f76 616c 7565  t accuracy_value
-00002190: 2c20 6461 7461 2077 6f6e 2774 200d 0a3b  , data won't ..;
-000021a0: 0962 6520 6669 6c74 6572 6564 2062 7920  .be filtered by 
-000021b0: 7468 6973 2063 7269 7465 7269 612c 2061  this criteria, a
-000021c0: 7320 6974 2077 6173 2061 6c72 6561 6479  s it was already
-000021d0: 200d 0a3b 0966 696c 7465 7265 6420 6475   ..;.filtered du
-000021e0: 7269 6e67 2070 726f 6365 7373 696e 6720  ring processing 
-000021f0: 6279 2061 6363 7572 6163 795f 7661 6c75  by accuracy_valu
-00002200: 652e 200d 0a3b 0d0a 6973 6f74 6f70 6963  e. ..;..isotopic
-00002210: 5f66 6974 7469 6e67 5f73 636f 7265 5f74  _fitting_score_t
-00002220: 6872 6573 686f 6c64 203d 2030 2e39 0d0a  hreshold = 0.9..
-00002230: 3b20 094d 696e 696d 756d 2073 636f 7265  ; .Minimum score
-00002240: 206f 6620 7468 6520 6973 6f74 6f70 6963   of the isotopic
-00002250: 2064 6973 7472 6962 7574 696f 6e20 6669   distribution fi
-00002260: 7474 696e 6720 0d0a 3b09 696e 206f 7264  tting ..;.in ord
-00002270: 6572 2074 6f20 636f 6e73 6964 6572 2061  er to consider a
-00002280: 206d 7a20 7065 616b 2076 6961 626c 652e   mz peak viable.
-00002290: 0d0a 3b0d 0a63 7572 7665 5f66 6974 7469  ..;..curve_fitti
-000022a0: 6e67 5f73 636f 7265 5f74 6872 6573 686f  ng_score_thresho
-000022b0: 6c64 203d 2030 2e39 0d0a 3b20 094d 696e  ld = 0.9..; .Min
-000022c0: 696d 756d 2073 636f 7265 2066 6f72 2074  imum score for t
-000022d0: 6865 2063 6872 6f6d 6174 6f67 7261 6d20  he chromatogram 
-000022e0: 7065 616b 2063 7572 7665 200d 0a3b 0966  peak curve ..;.f
-000022f0: 6974 7469 6e67 2074 6f20 6120 6761 7573  itting to a gaus
-00002300: 7369 616e 2074 6f20 636f 6e73 6964 6572  sian to consider
-00002310: 2061 2076 6961 626c 6520 7065 616b 2e20   a viable peak. 
-00002320: 0d0a 3b0d 0a73 6967 6e61 6c5f 746f 5f6e  ..;..signal_to_n
-00002330: 6f69 7365 5f74 6872 6573 686f 6c64 203d  oise_threshold =
-00002340: 2033 0d0a 3b20 094d 696e 696d 756d 2073   3..; .Minimum s
-00002350: 6967 6e61 6c2d 746f 2d6e 6f69 7365 2072  ignal-to-noise r
-00002360: 6174 696f 2074 6f20 636f 6e73 6964 6572  atio to consider
-00002370: 2061 200d 0a3b 0963 6872 6f6d 6174 6f67   a ..;.chromatog
-00002380: 7261 6d20 7065 616b 2076 6961 626c 652e  ram peak viable.
-00002390: 2043 616e 2062 6520 7265 6170 706c 6965   Can be reapplie
-000023a0: 6420 6f6e 200d 0a3b 0972 6177 2064 6174  d on ..;.raw dat
-000023b0: 6120 7265 616e 616c 7973 6973 2e0d 0a3b  a reanalysis...;
-000023c0: 0d0a 6f75 7470 7574 5f63 6f6d 706f 7369  ..output_composi
-000023d0: 7469 6f6e 735f 616e 616c 7973 6973 203d  tions_analysis =
-000023e0: 2079 6573 0d0a 3b20 0949 6620 7573 6564   yes..; .If used
-000023f0: 2c20 616c 736f 2070 6c6f 7473 2064 6174  , also plots dat
-00002400: 6120 7265 6c61 7465 6420 746f 2074 6865  a related to the
-00002410: 2077 686f 6c65 200d 0a3b 0963 6f6d 706f   whole ..;.compo
-00002420: 7369 7469 6f6e 206f 6620 6561 6368 2069  sition of each i
-00002430: 6465 6e74 6966 6965 6420 676c 7963 616e  dentified glycan
-00002440: 2069 6e20 7468 6520 0d0a 3b09 616e 616c   in the ..;.anal
-00002450: 7973 6973 2c20 696e 2061 6464 6974 696f  ysis, in additio
-00002460: 6e20 746f 2074 6865 2070 6561 6b2d 7365  n to the peak-se
-00002470: 7061 7261 7465 6420 6461 7461 2e0d 0a3b  parated data...;
-00002480: 0d0a 6f75 7470 7574 5f6d 6574 6162 6f61  ..output_metaboa
-00002490: 6e61 6c79 7374 5f66 696c 6520 3d20 6e6f  nalyst_file = no
-000024a0: 0d0a 6d65 7461 626f 616e 616c 7973 745f  ..metaboanalyst_
-000024b0: 6772 6f75 7073 203d 2043 4f4e 5452 4f4c  groups = CONTROL
-000024c0: 2c20 5452 4541 5445 440d 0a3b 2009 4865  , TREATED..; .He
-000024d0: 7265 2079 6f75 2073 6574 2075 7020 7768  re you set up wh
-000024e0: 6574 6865 7220 6f72 206e 6f74 2079 6f75  ether or not you
-000024f0: 2077 616e 7420 746f 206f 7574 7075 7420   want to output 
-00002500: 0d0a 3b09 6120 2e63 7376 2066 696c 6520  ..;.a .csv file 
-00002510: 746f 2062 6520 7573 6564 2066 6f72 2070  to be used for p
-00002520: 6c6f 7474 696e 6720 6461 7461 2075 7369  lotting data usi
-00002530: 6e67 200d 0a3b 096d 6574 6162 6f61 6e61  ng ..;.metaboana
-00002540: 6c79 7374 2e20 4966 2079 6f75 2077 616e  lyst. If you wan
-00002550: 7420 7468 6174 2c20 796f 7520 6d75 7374  t that, you must
-00002560: 2073 7065 6369 6679 200d 0a3b 0979 6f75   specify ..;.you
-00002570: 7220 7361 6d70 6c65 2067 726f 7570 732c  r sample groups,
-00002580: 2063 6f6d 6d61 2073 6570 6172 6174 6564   comma separated
-00002590: 2e20 5361 6d70 6c65 200d 0a3b 0967 726f  . Sample ..;.gro
-000025a0: 7570 7320 7370 6563 6966 6965 6420 6d75  ups specified mu
-000025b0: 7374 2062 6520 7072 6573 656e 7420 696e  st be present in
-000025c0: 2073 616d 706c 6520 0d0a 3b09 6669 6c65   sample ..;.file
-000025d0: 6e61 6d65 7320 666f 7220 7072 6f70 6572  names for proper
-000025e0: 2069 6465 6e74 6966 6963 6174 696f 6e2e   identification.
-000025f0: 2049 6620 6e6f 6e65 2069 7320 0d0a 3b09   If none is ..;.
-00002600: 7365 742c 2073 616d 706c 6573 2061 7265  set, samples are
-00002610: 2064 6566 6175 6c74 6564 2074 6f20 2275   defaulted to "u
-00002620: 6e67 726f 7570 6564 222e 2043 6173 6520  ngrouped". Case 
-00002630: 7365 6e73 6974 6976 652e 200d 0a3b 0d0a  sensitive. ..;..
-00002640: 6f75 7470 7574 5f66 6974 7469 6e67 735f  output_fittings_
-00002650: 6461 7461 203d 206e 6f0d 0a3b 2009 416c  data = no..; .Al
-00002660: 6c6f 7773 2074 6f20 6f75 7470 7574 2066  lows to output f
-00002670: 696c 6573 2077 6974 6820 7468 6520 6669  iles with the fi
-00002680: 7474 696e 6773 2064 6174 6120 746f 200d  ttings data to .
-00002690: 0a3b 0963 6865 636b 2073 636f 7269 6e67  .;.check scoring
-000026a0: 2063 7269 7465 7269 6173 2e20 4465 6661   criterias. Defa
-000026b0: 756c 7474 6564 2074 6f20 276e 6f27 2061  ultted to 'no' a
-000026c0: 7320 0d0a 3b09 7468 6573 6520 6669 6c65  s ..;.these file
-000026d0: 7320 7769 6c6c 2062 6520 6269 672e 204f  s will be big. O
-000026e0: 6e6c 7920 7573 6520 6974 2069 6620 796f  nly use it if yo
-000026f0: 7520 7265 616c 6c79 200d 0a3b 096e 6565  u really ..;.nee
-00002700: 642e 0d0a 3b0d 0a6f 7574 7075 745f 706c  d...;..output_pl
-00002710: 6f74 5f64 6174 6120 3d20 6e6f 0d0a 3b20  ot_data = no..; 
-00002720: 0941 6c6c 6f77 7320 746f 206f 7574 7075  .Allows to outpu
-00002730: 7420 6461 7461 2070 6c6f 7474 696e 6720  t data plotting 
-00002740: 6669 6c65 7320 666f 7220 616c 6c20 7468  files for all th
-00002750: 6520 0d0a 3b09 4549 4373 2064 7261 776e  e ..;.EICs drawn
-00002760: 2062 7920 7468 6520 7072 6f67 7261 6d2e   by the program.
-00002770: 2049 6620 7365 7420 746f 2027 6e6f 272c   If set to 'no',
-00002780: 2069 7420 7769 6c6c 200d 0a3b 0973 7469   it will ..;.sti
-00002790: 6c6c 206f 7574 7075 7420 7468 6520 666f  ll output the fo
-000027a0: 756e 6420 676c 7963 616e 7320 4549 432e  und glycans EIC.
-000027b0: 0d0a 3b                                  ..;
+00000a00: 6320 4163 6964 2028 5320 6f72 2041 6d20  c Acid (S or Am 
+00000a10: 616e 6420 450d 0a3b 0969 6620 796f 7520  and E..;.if you 
+00000a20: 6861 7665 206c 6163 746f 6e69 7a65 642d  have lactonized-
+00000a30: 6574 6879 6c20 7374 6572 6966 6965 6420  ethyl sterified 
+00000a40: 676c 7963 616e 7329 2c0d 0a3b 0947 6c79  glycans),..;.Gly
+00000a50: 636f 6c79 6c20 5369 616c 6963 2041 6369  colyl Sialic Aci
+00000a60: 6420 2847 292c 2044 656f 7879 6865 786f  d (G), Deoxyhexo
+00000a70: 7365 2028 4629 2e20 4361 7365 0d0a 3b09  se (F). Case..;.
+00000a80: 7365 6e73 6974 6976 652e 0d0a 3b09 2d3e  sensitive...;.->
+00000a90: 204f 6e6c 7920 6e65 6564 6564 2069 6e20   Only needed in 
+00000aa0: 6375 7374 6f6d 5f6c 6962 7261 7279 206d  custom_library m
+00000ab0: 6f64 652e 200d 0a3b 0d0a 746f 7461 6c5f  ode. ..;..total_
+00000ac0: 6d6f 6e6f 7361 6363 6861 7269 6465 7320  monosaccharides 
+00000ad0: 3d20 352c 2032 320d 0a68 6578 6f73 6573  = 5, 22..hexoses
+00000ae0: 203d 2033 2c20 3130 0d0a 6865 786e 6163   = 3, 10..hexnac
+00000af0: 7320 3d20 322c 2038 0d0a 7369 616c 6963  s = 2, 8..sialic
+00000b00: 5f61 6369 6473 203d 2030 2c20 340d 0a66  _acids = 0, 4..f
+00000b10: 7563 6f73 6573 203d 2030 2c20 320d 0a6e  ucoses = 0, 2..n
+00000b20: 6575 3561 6320 3d20 302c 2034 0d0a 6e65  eu5ac = 0, 4..ne
+00000b30: 7535 6763 203d 2030 2c20 300d 0a3b 2009  u5gc = 0, 0..; .
+00000b40: 5370 6563 6966 7920 7468 6520 6d69 6e69  Specify the mini
+00000b50: 6d75 6d20 616e 6420 6d61 7869 6d75 6d20  mum and maximum 
+00000b60: 6d6f 6e6f 7361 6363 6861 7269 6465 730d  monosaccharides.
+00000b70: 0a3b 0961 6d6f 756e 7473 2066 6f72 2067  .;.amounts for g
+00000b80: 656e 6572 6174 696e 6720 6120 6c69 6272  enerating a libr
+00000b90: 6172 792e 0d0a 3b09 2d3e 204f 6e6c 7920  ary...;.-> Only 
+00000ba0: 6e65 6564 6564 2069 6e20 6765 6e65 7261  needed in genera
+00000bb0: 7465 5f6c 6962 7261 7279 206d 6f64 652e  te_library mode.
+00000bc0: 0d0a 3b0d 0a0d 0a5b 636f 6d6d 6f6e 5f6c  ..;....[common_l
+00000bd0: 6962 7261 7279 5f62 7569 6c64 696e 675f  ibrary_building_
+00000be0: 7365 7474 696e 6773 5d0d 0a66 6f72 6365  settings]..force
+00000bf0: 5f6e 676c 7963 616e 203d 2079 6573 0d0a  _nglycan = yes..
+00000c00: 3b20 0955 7365 6420 746f 2066 6f72 6365  ; .Used to force
+00000c10: 2073 6f6d 6520 6d6f 6e6f 7361 6363 6861   some monosaccha
+00000c20: 7269 6465 7320 636f 6d70 6f73 6974 696f  rides compositio
+00000c30: 6e73 0d0a 3b09 6173 736f 6369 6174 6564  ns..;.associated
+00000c40: 2077 6974 6820 4e2d 476c 7963 616e 7320   with N-Glycans 
+00000c50: 6269 6f6c 6f67 6963 616c 6c79 206b 6e6f  biologically kno
+00000c60: 776e 200d 0a3b 0966 6561 7475 7265 732e  wn ..;.features.
+00000c70: 2049 6620 6e6f 7420 7573 6564 2c20 6769   If not used, gi
+00000c80: 7665 7320 6120 6d75 6368 2062 726f 6164  ves a much broad
+00000c90: 6572 200d 0a3b 096c 6962 7261 7279 2074  er ..;.library t
+00000ca0: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+00000cb0: 666f 7220 616e 616c 7973 6973 206f 6620  for analysis of 
+00000cc0: 0d0a 3b09 4f2d 476c 7963 616e 732c 2066  ..;.O-Glycans, f
+00000cd0: 6f72 2065 7861 6d70 6c65 2e0d 0a3b 0d0a  or example...;..
+00000ce0: 6d61 785f 6164 6475 6374 7320 3d20 4833  max_adducts = H3
+00000cf0: 0d0a 6164 6475 6374 735f 6578 636c 7573  ..adducts_exclus
+00000d00: 696f 6e20 3d20 0d0a 3b20 0949 6e64 6963  ion = ..; .Indic
+00000d10: 6174 6573 2074 6865 2064 6573 6972 6564  ates the desired
+00000d20: 2061 6464 7563 7473 2061 6e64 2074 6865   adducts and the
+00000d30: 6972 206d 6178 696d 756d 0d0a 3b09 616d  ir maximum..;.am
+00000d40: 6f75 6e74 2e20 4833 4e61 3120 6d65 616e  ount. H3Na1 mean
+00000d50: 7320 6120 6d61 7869 6d75 6d20 6f66 2033  s a maximum of 3
+00000d60: 2048 7964 726f 6765 6e73 2061 6e64 0d0a   Hydrogens and..
+00000d70: 3b09 6120 6d61 7869 6d75 6d20 6f66 2031  ;.a maximum of 1
+00000d80: 2053 6f64 6975 6d20 7065 7220 6164 6475   Sodium per addu
+00000d90: 6374 2063 6f6d 6269 6e61 7469 6f6e 2e20  ct combination. 
+00000da0: 0d0a 3b09 4361 7365 2073 656e 7369 7469  ..;.Case sensiti
+00000db0: 7665 2e20 446f 6573 6e27 7420 776f 726b  ve. Doesn't work
+00000dc0: 2077 6974 6820 636f 6d70 6c65 7820 6164   with complex ad
+00000dd0: 6475 6374 732c 0d0a 3b09 7375 6368 2061  ducts,..;.such a
+00000de0: 7320 4e48 342e 2053 6574 2061 6464 7563  s NH4. Set adduc
+00000df0: 7473 2069 6e20 2761 6464 7563 7473 5f65  ts in 'adducts_e
+00000e00: 7863 6c75 7369 6f6e 2720 746f 0d0a 3b09  xclusion' to..;.
+00000e10: 6176 6f69 6420 7573 696e 6720 7370 6563  avoid using spec
+00000e20: 6966 6963 2061 6464 7563 7473 2e20 436f  ific adducts. Co
+00000e30: 6d6d 6120 7365 7061 7261 7465 6420 6c69  mma separated li
+00000e40: 7374 2e0d 0a3b 0d0a 6d61 785f 6368 6172  st...;..max_char
+00000e50: 6765 7320 3d20 330d 0a3b 2009 4c69 6d69  ges = 3..; .Limi
+00000e60: 7473 2074 6865 206d 6178 696d 756d 2061  ts the maximum a
+00000e70: 6d6f 756e 7420 6f66 2063 616c 6375 6c61  mount of calcula
+00000e80: 7465 6420 6368 6172 6765 730d 0a3b 0966  ted charges..;.f
+00000e90: 6f72 2065 6163 6820 676c 7963 616e 2e20  or each glycan. 
+00000ea0: 5365 7420 746f 2061 206e 6567 6174 6976  Set to a negativ
+00000eb0: 6520 7661 6c75 6520 6966 2079 6f75 0d0a  e value if you..
+00000ec0: 3b09 7761 6e74 2074 6f20 646f 206e 6567  ;.want to do neg
+00000ed0: 6174 6976 6520 6d6f 6465 2061 6e61 6c79  ative mode analy
+00000ee0: 7369 7320 5b45 5850 4552 494d 454e 5441  sis [EXPERIMENTA
+00000ef0: 4c5d 2e0d 0a3b 0d0a 7265 6475 6369 6e67  L]...;..reducing
+00000f00: 5f65 6e64 5f74 6167 203d 2031 3333 2e30  _end_tag = 133.0
+00000f10: 3634 340d 0a3b 2009 4966 2061 2072 6564  644..; .If a red
+00000f20: 7563 696e 6720 656e 6420 7461 6720 6973  ucing end tag is
+00000f30: 2061 6464 6564 2074 6f20 7468 6520 676c   added to the gl
+00000f40: 7963 616e 732c 200d 0a3b 2009 696e 7365  ycans, ..; .inse
+00000f50: 7274 2069 7473 2061 6464 6564 206d 6173  rt its added mas
+00000f60: 7320 6f72 206d 6f6c 6563 756c 6172 2066  s or molecular f
+00000f70: 6f72 6d75 6c61 2068 6572 652e 0d0a 3b09  ormula here...;.
+00000f80: 4966 206e 6f20 7265 6475 6369 6e67 2065  If no reducing e
+00000f90: 6e64 2074 6167 2069 7320 6164 6465 6420  nd tag is added 
+00000fa0: 746f 2074 6865 2067 6c79 6361 6e73 2c20  to the glycans, 
+00000fb0: 0d0a 3b09 7365 7420 7468 6973 2076 616c  ..;.set this val
+00000fc0: 7565 2074 6f20 302e 2050 726f 6361 696e  ue to 0. Procain
+00000fd0: 616d 6964 653a 2032 3139 2e31 3733 3520  amide: 219.1735 
+00000fe0: 6f72 0d0a 3b09 4331 3348 3231 4e33 3b20  or..;.C13H21N3; 
+00000ff0: 4769 7261 7264 2052 6561 6765 6e74 2050  Girard Reagent P
+00001000: 3a20 3133 332e 3036 3434 206f 7220 4337  : 133.0644 or C7
+00001010: 4837 4e33 200d 0a3b 0928 6465 7072 6f74  H7N3 ..;.(deprot
+00001020: 6f6e 6174 6564 2c20 6e65 7574 7261 6c29  onated, neutral)
+00001030: 2e20 4361 6e20 616c 736f 2062 6520 7573  . Can also be us
+00001040: 6564 2077 6974 6820 0d0a 3b09 6120 7065  ed with ..;.a pe
+00001050: 7074 6964 6520 6279 2069 6e70 7574 696e  ptide by inputin
+00001060: 6720 2770 6570 2d27 202b 2074 6865 2070  g 'pep-' + the p
+00001070: 6574 6964 6520 0d0a 3b09 7365 7175 656e  etide ..;.sequen
+00001080: 6365 2028 6965 2e20 2770 6570 2d4e 4b27  ce (ie. 'pep-NK'
+00001090: 2066 6f72 2074 6865 2070 6570 7469 6465   for the peptide
+000010a0: 204e 4b29 2e0d 0a3b 0d0a 7065 726d 6574   NK)...;..permet
+000010b0: 6879 6c61 7465 6420 3d20 6e6f 0d0a 3b20  hylated = no..; 
+000010c0: 0949 6620 7468 6520 7361 6d70 6c65 2077  .If the sample w
+000010d0: 6173 2070 6572 6d65 7468 796c 6174 6564  as permethylated
+000010e0: 2c20 7365 7420 7468 6973 200d 0a3b 0970  , set this ..;.p
+000010f0: 6172 616d 6574 6572 2074 6f20 2279 6573  arameter to "yes
+00001100: 222e 2044 6f65 736e 2774 2074 616b 6520  ". Doesn't take 
+00001110: 696e 746f 2061 6363 6f75 6e74 200d 0a3b  into account ..;
+00001120: 0970 6172 7469 616c 2070 6572 6d65 7468  .partial permeth
+00001130: 796c 6174 696f 6e73 2e0d 0a3b 0d0a 7265  ylations...;..re
+00001140: 6475 6365 6420 3d20 6e6f 0d0a 3b20 0949  duced = no..; .I
+00001150: 6620 7468 6520 7361 6d70 6c65 2064 6f65  f the sample doe
+00001160: 736e 2774 2068 6176 6520 6120 7461 6720  sn't have a tag 
+00001170: 616e 6420 7468 6520 676c 7963 616e 730d  and the glycans.
+00001180: 0a3b 0968 6164 2074 6865 6972 2072 6564  .;.had their red
+00001190: 7563 696e 6720 656e 6420 7265 6475 6365  ucing end reduce
+000011a0: 642c 2073 6574 2074 6869 7320 746f 2022  d, set this to "
+000011b0: 7965 7322 2e0d 0a3b 0d0a 616d 696e 6174  yes"...;..aminat
+000011c0: 6564 5f65 7468 796c 5f65 7374 6572 6966  ed_ethyl_esterif
+000011d0: 6965 6420 3d20 6e6f 0d0a 3b20 0955 7365  ied = no..; .Use
+000011e0: 2069 6620 7468 6520 7369 616c 6963 2061   if the sialic a
+000011f0: 6369 6473 2077 6572 6520 6465 7269 7669  cids were derivi
+00001200: 7469 7a65 6420 7769 7468 200d 0a3b 0961  tized with ..;.a
+00001210: 6d69 6e61 7469 6f6e 2028 616c 7068 6132  mination (alpha2
+00001220: 2c33 2920 616e 6420 6574 6879 6c20 6573  ,3) and ethyl es
+00001230: 7465 7269 6669 6361 7469 6f6e 200d 0a3b  terification ..;
+00001240: 0928 616c 7068 6132 2c36 292e 204c 6163  .(alpha2,6). Lac
+00001250: 746f 6e69 7a65 6420 4163 6574 796c 2053  tonized Acetyl S
+00001260: 6961 6c69 6320 4163 6964 2077 696c 6c0d  ialic Acid will.
+00001270: 0a3b 0962 6520 6964 656e 7469 6669 6564  .;.be identified
+00001280: 2061 7320 2741 6d27 2061 6e64 2045 7468   as 'Am' and Eth
+00001290: 796c 2045 7374 6572 6966 6965 6420 4163  yl Esterified Ac
+000012a0: 6574 796c 0d0a 3b09 5369 616c 6963 2041  etyl..;.Sialic A
+000012b0: 6369 6420 7769 6c6c 2062 6520 6964 656e  cid will be iden
+000012c0: 7469 6669 6564 2061 7320 2745 272e 0d0a  tified as 'E'...
+000012d0: 3b0d 0a66 6173 745f 6973 6f20 3d20 7965  ;..fast_iso = ye
+000012e0: 730d 0a3b 2009 416c 6c6f 7773 2079 6f75  s..; .Allows you
+000012f0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+00001300: 6520 6973 6f74 6f70 6963 2064 6973 7472  e isotopic distr
+00001310: 6962 7574 696f 6e0d 0a3b 096f 6620 676c  ibution..;.of gl
+00001320: 7963 616e 7320 6261 7365 6420 6f6e 6c79  ycans based only
+00001330: 206f 6e20 6361 7262 6f6e 2069 736f 746f   on carbon isoto
+00001340: 7065 7320 2866 6173 742c 200d 0a3b 0969  pes (fast, ..;.i
+00001350: 6e6e 6163 7572 6174 6529 2061 6e64 2063  nnacurate) and c
+00001360: 6f72 7265 6374 6564 2061 7274 6966 6963  orrected artific
+00001370: 6961 6c6c 7920 6f72 206f 6e20 616c 6c20  ially or on all 
+00001380: 0d0a 3b09 7468 6520 6174 6f6d 7320 6973  ..;.the atoms is
+00001390: 6f74 6f70 6573 2028 5645 5259 2053 4c4f  otopes (VERY SLO
+000013a0: 572c 2076 6572 7920 6163 6375 7261 7465  W, very accurate
+000013b0: 292e 200d 0a3b 0949 6620 6e6f 7420 7573  ). ..;.If not us
+000013c0: 6564 2c20 6c69 6272 6172 7920 6275 696c  ed, library buil
+000013d0: 6469 6e67 206d 6179 2074 616b 6520 6d61  ding may take ma
+000013e0: 6e79 2068 6f75 7273 0d0a 3b09 6465 7065  ny hours..;.depe
+000013f0: 6e64 696e 6720 6f6e 2073 697a 652e 0d0a  nding on size...
+00001400: 3b0d 0a68 6967 685f 7265 736f 6c75 7469  ;..high_resoluti
+00001410: 6f6e 5f69 736f 746f 7069 635f 6469 7374  on_isotopic_dist
+00001420: 203d 206e 6f0d 0a3b 2009 4966 206e 6f74   = no..; .If not
+00001430: 2075 7365 642c 2064 6f65 736e 2774 2063   used, doesn't c
+00001440: 6c75 6d70 2069 736f 746f 7065 2070 6561  lump isotope pea
+00001450: 6b73 200d 0a3b 0974 6f67 6574 6865 722c  ks ..;.together,
+00001460: 206d 6561 6e69 6e67 2074 6861 7420 796f   meaning that yo
+00001470: 7527 6c6c 2068 6176 6520 6d6f 7265 2074  u'll have more t
+00001480: 6861 6e20 6f6e 6520 0d0a 3b09 6973 6f74  han one ..;.isot
+00001490: 6f70 6963 2070 6561 6b20 696e 2061 2031  opic peak in a 1
+000014a0: 2044 6120 696e 7465 7276 616c 2e20 4f6e   Da interval. On
+000014b0: 6c79 2075 7365 2074 6869 7320 0d0a 3b09  ly use this ..;.
+000014c0: 6966 2079 6f75 2068 6176 6520 6661 7374  if you have fast
+000014d0: 5f69 736f 206f 6666 2e20 5573 6566 756c  _iso off. Useful
+000014e0: 2077 6865 6e20 616e 616c 797a 696e 6720   when analyzing 
+000014f0: 0d0a 3b09 7665 7279 2068 6967 6820 7265  ..;.very high re
+00001500: 736f 6c75 7469 6f6e 2064 6174 612c 2073  solution data, s
+00001510: 7563 6820 6173 2064 6174 6120 6163 7175  uch as data acqu
+00001520: 6972 6564 200d 0a3b 096f 6e20 4654 206d  ired ..;.on FT m
+00001530: 6173 7320 7370 6563 7472 6f6d 6574 6572  ass spectrometer
+00001540: 732e 0d0a 3b0d 0a69 6e74 6572 6e61 6c5f  s...;..internal_
+00001550: 7374 616e 6461 7264 5f6d 6173 7320 3d20  standard_mass = 
+00001560: 302e 300d 0a3b 2009 4966 2075 7369 6e67  0.0..; .If using
+00001570: 2061 6e20 696e 7465 726e 616c 2073 7461   an internal sta
+00001580: 6e64 6172 642c 2069 6e73 6572 7420 6974  ndard, insert it
+00001590: 7320 6d61 7373 200d 0a3b 0968 6572 6520  s mass ..;.here 
+000015a0: 666f 7220 7468 6520 7363 7269 7074 2074  for the script t
+000015b0: 6f20 6361 6c63 756c 6174 6520 6974 7320  o calculate its 
+000015c0: 6172 6561 2e20 5468 6973 200d 0a3b 0961  area. This ..;.a
+000015d0: 6c73 6f20 616c 6c6f 7773 2074 6865 2073  lso allows the s
+000015e0: 6372 6970 7420 746f 206f 7574 7075 7420  cript to output 
+000015f0: 6120 6e6f 726d 616c 697a 6564 200d 0a3b  a normalized ..;
+00001600: 096d 6574 6162 6f61 6e61 6c79 7374 2063  .metaboanalyst c
+00001610: 6f6d 7061 7469 626c 6520 6669 6c65 2e0d  ompatible file..
+00001620: 0a3b 0d0a 0d0a 5b61 6e61 6c79 7369 735f  .;....[analysis_
+00001630: 7061 7261 6d65 7465 7273 5d0d 0a61 6e61  parameters]..ana
+00001640: 6c79 7a65 5f6d 7332 203d 2079 6573 0d0a  lyze_ms2 = yes..
+00001650: 666f 7263 655f 6672 6167 6d65 6e74 735f  force_fragments_
+00001660: 746f 5f67 6c79 6361 6e73 203d 2079 6573  to_glycans = yes
+00001670: 0d0a 756e 7265 7374 7269 6374 6564 5f66  ..unrestricted_f
+00001680: 7261 676d 656e 7473 203d 206e 6f0d 0a3b  ragments = no..;
+00001690: 2009 416c 6c6f 7773 2074 6f20 616e 616c   .Allows to anal
+000016a0: 797a 6520 6d73 3220 6461 7461 2c20 6173  yze ms2 data, as
+000016b0: 2077 656c 6c2e 2046 7261 676d 656e 7473   well. Fragments
+000016c0: 200d 0a3b 0969 6465 6e74 6966 6965 6420   ..;.identified 
+000016d0: 7769 6c6c 2062 6520 6173 736f 6369 6174  will be associat
+000016e0: 6564 2077 6974 6820 6561 6368 2067 6c79  ed with each gly
+000016f0: 6361 6e2e 200d 0a3b 0959 6f75 2063 616e  can. ..;.You can
+00001700: 2063 686f 6f73 6520 746f 2066 696c 7465   choose to filte
+00001710: 7220 6964 656e 7469 6669 6564 2066 7261  r identified fra
+00001720: 676d 656e 7473 2062 7920 0d0a 3b09 6d6f  gments by ..;.mo
+00001730: 6e6f 7361 6363 6861 7269 6465 7320 636f  nosaccharides co
+00001740: 6d70 6f73 6974 696f 6e73 2c20 696e 206f  mpositions, in o
+00001750: 7264 6572 2074 6f20 6176 6f69 6420 0d0a  rder to avoid ..
+00001760: 3b09 7265 706f 7274 696e 6720 6672 6167  ;.reporting frag
+00001770: 6d65 6e74 7320 7468 6174 2061 7265 6e27  ments that aren'
+00001780: 7420 636f 6d70 6174 6962 6c65 2077 6974  t compatible wit
+00001790: 6820 0d0a 3b09 6465 7465 6374 6564 2070  h ..;.detected p
+000017a0: 7265 6375 7273 6f72 2e20 4966 2075 6e72  recursor. If unr
+000017b0: 6573 7472 6963 7465 645f 6672 6167 6d65  estricted_fragme
+000017c0: 6e74 7320 6973 200d 0a3b 0975 7365 642c  nts is ..;.used,
+000017d0: 2069 7420 7365 6172 6368 6573 2066 6f72   it searches for
+000017e0: 2067 6c79 6361 6e73 2069 6e20 6576 6572   glycans in ever
+000017f0: 7920 6d73 3220 7363 616e 2c20 0d0a 3b09  y ms2 scan, ..;.
+00001800: 7265 6761 7264 6c65 7373 2069 6620 7468  regardless if th
+00001810: 6520 676c 7963 616e 2077 6173 2066 6f75  e glycan was fou
+00001820: 6e64 2069 6e20 6675 6c6c 2073 6361 6e2e  nd in full scan.
+00001830: 200d 0a3b 0954 6869 7320 7769 6c6c 2074   ..;.This will t
+00001840: 616b 6520 6120 6269 7420 6c6f 6e67 6572  ake a bit longer
+00001850: 2e20 0d0a 3b0d 0a61 6363 7572 6163 795f  . ..;..accuracy_
+00001860: 756e 6974 203d 2070 706d 0d0a 3b20 0944  unit = ppm..; .D
+00001870: 6574 6572 6d69 6e65 7320 7468 6520 756e  etermines the un
+00001880: 6974 7320 6f66 206d 7a20 746f 6c65 7261  its of mz tolera
+00001890: 6e63 6520 746f 2062 6520 7573 6564 200d  nce to be used .
+000018a0: 0a3b 0962 7920 7468 6520 7363 7269 7074  .;.by the script
+000018b0: 2e20 4f70 7469 6f6e 733a 2027 7070 6d27  . Options: 'ppm'
+000018c0: 206f 7220 2770 7727 2e20 0d0a 3b09 2770   or 'pw'. ..;.'p
+000018d0: 706d 2720 3d20 5061 7274 6963 6c65 7320  pm' = Particles 
+000018e0: 7065 7220 4d69 6c6c 696f 6e2c 2077 6865  per Million, whe
+000018f0: 7265 2031 3020 7070 6d20 6973 200d 0a3b  re 10 ppm is ..;
+00001900: 0961 726f 756e 6420 302e 3031 206d 7a20  .around 0.01 mz 
+00001910: 746f 6c65 7261 6e63 6520 6174 206d 7a20  tolerance at mz 
+00001920: 3130 3030 2c20 276d 7a27 203d 2046 6978  1000, 'mz' = Fix
+00001930: 6564 200d 0a3b 096d 7a20 746f 6c65 7261  ed ..;.mz tolera
+00001940: 6e63 6520 6672 6f6d 2063 656e 7472 6f69  nce from centroi
+00001950: 642c 2030 2e30 3120 6d7a 206d 6561 6e73  d, 0.01 mz means
+00001960: 2069 7420 0d0a 3b09 746f 6c65 7261 7465   it ..;.tolerate
+00001970: 7320 6120 302e 3031 2076 6172 6961 6e63  s a 0.01 varianc
+00001980: 6520 696e 206d 7a0d 0a3b 0d0a 6163 6375  e in mz..;..accu
+00001990: 7261 6379 5f76 616c 7565 203d 2031 300d  racy_value = 10.
+000019a0: 0a3b 2009 5468 6520 7661 6c75 6520 666f  .; .The value fo
+000019b0: 7220 7468 6520 6163 6375 7261 6379 5f75  r the accuracy_u
+000019c0: 6e69 7420 7061 7261 6d65 7465 722e 2059  nit parameter. Y
+000019d0: 6f75 200d 0a3b 0963 616e 2075 7365 2061  ou ..;.can use a
+000019e0: 2062 726f 6164 6572 2061 6363 7572 6163   broader accurac
+000019f0: 7920 7661 6c75 6520 616e 6420 7468 656e  y value and then
+00001a00: 2066 696c 7465 7220 0d0a 3b09 7261 7720   filter ..;.raw 
+00001a10: 6461 7461 2075 7369 6e67 206d 6178 5f70  data using max_p
+00001a20: 706d 2c20 6275 7420 7468 6973 206d 6179  pm, but this may
+00001a30: 206c 6561 6420 746f 200d 0a3b 0966 616c   lead to ..;.fal
+00001a40: 7365 2070 6f73 6974 6976 6573 2e0d 0a3b  se positives...;
+00001a50: 0d0a 7265 745f 7469 6d65 5f69 6e74 6572  ..ret_time_inter
+00001a60: 7661 6c20 3d20 312c 2039 3939 0d0a 3b20  val = 1, 999..; 
+00001a70: 0954 6865 206d 696e 696d 756d 2061 6e64  .The minimum and
+00001a80: 206d 6178 696d 756d 2072 6574 656e 7469   maximum retenti
+00001a90: 6f6e 2074 696d 652c 2069 6e20 4d49 4e55  on time, in MINU
+00001aa0: 5445 532c 200d 0a3b 0975 7365 6420 666f  TES, ..;.used fo
+00001ab0: 7220 7661 7269 6f75 7320 706f 7274 696f  r various portio
+00001ac0: 6e73 206f 6620 7468 6520 7363 7269 7074  ns of the script
+00001ad0: 2e20 4120 7368 6f72 7465 7220 0d0a 3b09  . A shorter ..;.
+00001ae0: 696e 7465 7276 616c 206f 6620 7265 745f  interval of ret_
+00001af0: 7469 6d65 206d 616b 6573 2074 6865 2073  time makes the s
+00001b00: 6372 6970 7420 7275 6e20 6661 7374 6572  cript run faster
+00001b10: 2c20 0d0a 3b09 736f 2074 7279 2074 6f20  , ..;.so try to 
+00001b20: 7472 696d 2079 6f75 7220 7361 6d70 6c65  trim your sample
+00001b30: 2061 7320 6d75 6368 2061 7320 706f 7373   as much as poss
+00001b40: 6962 6c65 2c20 0d0a 3b09 6966 2079 6f75  ible, ..;.if you
+00001b50: 206b 6e6f 7720 7768 656e 2079 6f75 7220   know when your 
+00001b60: 616e 616c 7974 6573 2061 7265 206c 6561  analytes are lea
+00001b70: 7669 6e67 2074 6865 200d 0a3b 0963 6f6c  ving the ..;.col
+00001b80: 756d 6e2e 0d0a 3b0d 0a63 7573 746f 6d5f  umn...;..custom_
+00001b90: 6d69 6e5f 706f 696e 7473 5f70 6572 5f70  min_points_per_p
+00001ba0: 6561 6b20 3d20 6e6f 0d0a 6e75 6d62 6572  eak = no..number
+00001bb0: 5f70 6f69 6e74 735f 7065 725f 7065 616b  _points_per_peak
+00001bc0: 203d 2035 0d0a 3b20 0949 6620 7573 6564   = 5..; .If used
+00001bd0: 2c20 7365 7420 7468 6520 6d69 6e69 6d75  , set the minimu
+00001be0: 6d20 6e75 6d62 6572 206f 6620 6461 7461  m number of data
+00001bf0: 706f 696e 7473 2074 6f20 0d0a 3b09 636f  points to ..;.co
+00001c00: 6e73 6964 6572 2061 2063 6872 6f6d 6174  nsider a chromat
+00001c10: 6f67 7261 6d20 7065 616b 2070 6172 7420  ogram peak part 
+00001c20: 6f66 2074 6865 2072 6177 200d 0a3b 0964  of the raw ..;.d
+00001c30: 6174 6173 6574 2e20 4966 206c 6566 7420  ataset. If left 
+00001c40: 6f6e 2046 616c 7365 2069 7420 6361 6c63  on False it calc
+00001c50: 756c 6174 6573 200d 0a3b 0961 7574 6f6d  ulates ..;.autom
+00001c60: 6174 6963 616c 6c79 2e0d 0a3b 0d0a 6c69  atically...;..li
+00001c70: 6d69 745f 7065 616b 735f 7069 636b 6564  mit_peaks_picked
+00001c80: 203d 2079 6573 0d0a 6d61 785f 6e75 6d62   = yes..max_numb
+00001c90: 6572 5f70 6561 6b73 203d 2035 0d0a 3b20  er_peaks = 5..; 
+00001ca0: 0949 6620 7573 6564 2c20 7069 636b 7320  .If used, picks 
+00001cb0: 6f6e 6c79 2074 6865 206d 6f73 7420 696e  only the most in
+00001cc0: 7465 6e73 6520 7065 616b 206f 6e20 7468  tense peak on th
+00001cd0: 6520 0d0a 3b09 4549 4320 616e 6420 7570  e ..;.EIC and up
+00001ce0: 2074 6f20 5b6d 6178 5f6e 756d 6265 725f   to [max_number_
+00001cf0: 7065 616b 735d 2d31 206f 7468 6572 2070  peaks]-1 other p
+00001d00: 6561 6b73 200d 0a3b 0963 6c6f 7365 7374  eaks ..;.closest
+00001d10: 2074 6f20 6974 2e20 5761 726e 696e 673a   to it. Warning:
+00001d20: 2054 6869 7320 6d61 7920 7265 6475 6365   This may reduce
+00001d30: 2074 6865 2072 616e 6765 200d 0a3b 096f   the range ..;.o
+00001d40: 6620 796f 7572 2072 6573 756c 7473 2e0d  f your results..
+00001d50: 0a3b 0d0a 0d0a 5b70 6f73 742d 616e 616c  .;....[post-anal
+00001d60: 7973 6973 2f72 6561 6e61 6c79 7369 735d  ysis/reanalysis]
+00001d70: 0d0a 6669 6c74 6572 5f6d 7332 5f62 795f  ..filter_ms2_by_
+00001d80: 7265 706f 7274 6572 5f69 6f6e 7320 3d20  reporter_ions = 
+00001d90: 4e31 5431 2c20 3336 362e 3134 0d0a 3b09  N1T1, 366.14..;.
+00001da0: 5365 7420 7265 706f 7274 6572 2069 6f6e  Set reporter ion
+00001db0: 7320 746f 2068 6964 6520 4d53 3220 7370  s to hide MS2 sp
+00001dc0: 6563 7472 6120 7468 6174 2064 6f6e 2774  ectra that don't
+00001dd0: 0d0a 3b09 636f 6e74 6169 6e20 7468 656d  ..;.contain them
+00001de0: 2e20 4361 6e20 6265 2062 6173 6564 2077  . Can be based w
+00001df0: 6974 6820 676c 7963 616e 7320 666f 726d  ith glycans form
+00001e00: 756c 6120 0d0a 3b09 2877 6974 6820 5420  ula ..;.(with T 
+00001e10: 6265 696e 6720 7468 6520 7265 6475 6369  being the reduci
+00001e20: 6e67 2065 6e64 206f 6620 7468 6520 676c  ng end of the gl
+00001e30: 7963 616e 2c20 0d0a 3b09 696e 636c 7564  ycan, ..;.includ
+00001e40: 696e 6720 706f 7373 6962 6c79 2074 6865  ing possibly the
+00001e50: 2074 6167 2c20 6966 2075 7365 6429 206f   tag, if used) o
+00001e60: 7220 616e 206d 7a2e 0d0a 3b09 0d0a 616c  r an mz...;...al
+00001e70: 6967 6e5f 6368 726f 6d61 746f 6772 616d  ign_chromatogram
+00001e80: 7320 3d20 7965 730d 0a3b 2009 4966 2065  s = yes..; .If e
+00001e90: 6e61 626c 6564 2c20 7769 6c6c 2061 6c69  nabled, will ali
+00001ea0: 676e 2074 6865 2061 7373 6967 6e6d 656e  gn the assignmen
+00001eb0: 7473 2061 6e64 2064 7261 776e 200d 0a3b  ts and drawn ..;
+00001ec0: 0970 726f 6365 7373 6564 2045 4943 7320  .processed EICs 
+00001ed0: 6f66 2074 6865 2064 6966 6665 7265 6e74  of the different
+00001ee0: 2073 616d 706c 6573 2e20 5468 6520 0d0a   samples. The ..
+00001ef0: 3b09 616c 6967 6e6d 656e 7420 6973 2068  ;.alignment is h
+00001f00: 6967 686c 7920 6465 7065 6e64 656e 7420  ighly dependent 
+00001f10: 6f6e 2074 6865 2066 6561 7475 7265 7320  on the features 
+00001f20: 0d0a 3b09 6964 656e 7469 6669 6564 2061  ..;.identified a
+00001f30: 6e64 2074 6865 6972 2069 6e68 6572 656e  nd their inheren
+00001f40: 7420 7175 616c 6974 792c 2073 6f20 7468  t quality, so th
+00001f50: 696e 6773 200d 0a3b 0977 696c 6c20 6368  ings ..;.will ch
+00001f60: 616e 6765 2077 6974 6820 6469 6666 6572  ange with differ
+00001f70: 656e 7420 7175 616c 6974 7920 7468 7265  ent quality thre
+00001f80: 7368 6f6c 6473 2e20 0d0a 3b0d 0a61 7563  sholds. ..;..auc
+00001f90: 5f70 6572 6365 6e74 6167 655f 7468 7265  _percentage_thre
+00001fa0: 7368 6f6c 6420 3d20 310d 0a3b 2009 416c  shold = 1..; .Al
+00001fb0: 6c6f 7773 2079 6f75 2074 6f20 7375 7072  lows you to supr
+00001fc0: 6573 7320 6672 6f6d 2074 6865 2061 6e61  ess from the ana
+00001fd0: 6c79 7369 7320 7065 616b 7320 0d0a 3b09  lysis peaks ..;.
+00001fe0: 7468 6174 2061 7265 206f 6620 7468 6520  that are of the 
+00001ff0: 7370 6563 6966 6965 6420 7065 7263 656e  specified percen
+00002000: 7461 6765 2028 6672 6f6d 2030 2520 746f  tage (from 0% to
+00002010: 0d0a 3b09 3130 3025 2920 6172 6561 2075  ..;.100%) area u
+00002020: 6e64 6572 2063 7572 7665 2072 656c 6174  nder curve relat
+00002030: 6564 2074 6f20 7468 6520 6d6f 7374 2069  ed to the most i
+00002040: 6e74 656e 7365 0d0a 3b09 7065 616b 2061  ntense..;.peak a
+00002050: 7265 6120 7769 7468 696e 2074 6865 2073  rea within the s
+00002060: 616d 6520 6164 6475 6374 2028 6965 2e20  ame adduct (ie. 
+00002070: 6966 2062 6967 6765 7374 200d 0a3b 0970  if biggest ..;.p
+00002080: 6561 6b20 6861 7320 6120 6172 6561 2075  eak has a area u
+00002090: 6e64 6572 2063 7572 7665 206f 6620 3130  nder curve of 10
+000020a0: 3020 616e 6420 0d0a 3b09 6175 635f 7065  0 and ..;.auc_pe
+000020b0: 7263 656e 7461 6765 5f74 6872 6573 686f  rcentage_thresho
+000020c0: 6c64 2069 7320 7365 7420 746f 2031 252c  ld is set to 1%,
+000020d0: 2065 7665 7279 2070 6561 6b20 0d0a 3b09   every peak ..;.
+000020e0: 7769 7468 2061 6e20 6175 6320 6f66 2031  with an auc of 1
+000020f0: 2061 6e64 2062 656c 6f77 2077 696c 6c20   and below will 
+00002100: 6265 2073 7570 7265 7373 6564 290d 0a3b  be supressed)..;
+00002110: 0d0a 6d61 785f 7070 6d5f 7468 7265 7368  ..max_ppm_thresh
+00002120: 6f6c 6420 3d20 3130 0d0a 3b20 094d 6178  old = 10..; .Max
+00002130: 696d 756d 2050 504d 2065 7272 6f72 2066  imum PPM error f
+00002140: 6f72 2064 6174 6120 6375 7261 7469 6f6e  or data curation
+00002150: 2e20 4966 2076 616c 7565 2069 7320 0d0a  . If value is ..
+00002160: 3b09 6772 6561 7465 7220 7468 616e 2065  ;.greater than e
+00002170: 7175 6976 616c 656e 7420 6163 6375 7261  quivalent accura
+00002180: 6379 5f76 616c 7565 2c20 6461 7461 2077  cy_value, data w
+00002190: 6f6e 2774 200d 0a3b 0962 6520 6669 6c74  on't ..;.be filt
+000021a0: 6572 6564 2062 7920 7468 6973 2063 7269  ered by this cri
+000021b0: 7465 7269 612c 2061 7320 6974 2077 6173  teria, as it was
+000021c0: 2061 6c72 6561 6479 200d 0a3b 0966 696c   already ..;.fil
+000021d0: 7465 7265 6420 6475 7269 6e67 2070 726f  tered during pro
+000021e0: 6365 7373 696e 6720 6279 2061 6363 7572  cessing by accur
+000021f0: 6163 795f 7661 6c75 652e 200d 0a3b 0d0a  acy_value. ..;..
+00002200: 6973 6f74 6f70 6963 5f66 6974 7469 6e67  isotopic_fitting
+00002210: 5f73 636f 7265 5f74 6872 6573 686f 6c64  _score_threshold
+00002220: 203d 2030 2e39 0d0a 3b20 094d 696e 696d   = 0.9..; .Minim
+00002230: 756d 2073 636f 7265 206f 6620 7468 6520  um score of the 
+00002240: 6973 6f74 6f70 6963 2064 6973 7472 6962  isotopic distrib
+00002250: 7574 696f 6e20 6669 7474 696e 6720 0d0a  ution fitting ..
+00002260: 3b09 696e 206f 7264 6572 2074 6f20 636f  ;.in order to co
+00002270: 6e73 6964 6572 2061 206d 7a20 7065 616b  nsider a mz peak
+00002280: 2076 6961 626c 652e 0d0a 3b0d 0a63 7572   viable...;..cur
+00002290: 7665 5f66 6974 7469 6e67 5f73 636f 7265  ve_fitting_score
+000022a0: 5f74 6872 6573 686f 6c64 203d 2030 2e39  _threshold = 0.9
+000022b0: 0d0a 3b20 094d 696e 696d 756d 2073 636f  ..; .Minimum sco
+000022c0: 7265 2066 6f72 2074 6865 2063 6872 6f6d  re for the chrom
+000022d0: 6174 6f67 7261 6d20 7065 616b 2063 7572  atogram peak cur
+000022e0: 7665 200d 0a3b 0966 6974 7469 6e67 2074  ve ..;.fitting t
+000022f0: 6f20 6120 6761 7573 7369 616e 2074 6f20  o a gaussian to 
+00002300: 636f 6e73 6964 6572 2061 2076 6961 626c  consider a viabl
+00002310: 6520 7065 616b 2e20 0d0a 3b0d 0a73 6967  e peak. ..;..sig
+00002320: 6e61 6c5f 746f 5f6e 6f69 7365 5f74 6872  nal_to_noise_thr
+00002330: 6573 686f 6c64 203d 2033 0d0a 3b20 094d  eshold = 3..; .M
+00002340: 696e 696d 756d 2073 6967 6e61 6c2d 746f  inimum signal-to
+00002350: 2d6e 6f69 7365 2072 6174 696f 2074 6f20  -noise ratio to 
+00002360: 636f 6e73 6964 6572 2061 200d 0a3b 0963  consider a ..;.c
+00002370: 6872 6f6d 6174 6f67 7261 6d20 7065 616b  hromatogram peak
+00002380: 2076 6961 626c 652e 2043 616e 2062 6520   viable. Can be 
+00002390: 7265 6170 706c 6965 6420 6f6e 200d 0a3b  reapplied on ..;
+000023a0: 0972 6177 2064 6174 6120 7265 616e 616c  .raw data reanal
+000023b0: 7973 6973 2e0d 0a3b 0d0a 6f75 7470 7574  ysis...;..output
+000023c0: 5f63 6f6d 706f 7369 7469 6f6e 735f 616e  _compositions_an
+000023d0: 616c 7973 6973 203d 2079 6573 0d0a 3b20  alysis = yes..; 
+000023e0: 0949 6620 7573 6564 2c20 616c 736f 2070  .If used, also p
+000023f0: 6c6f 7473 2064 6174 6120 7265 6c61 7465  lots data relate
+00002400: 6420 746f 2074 6865 2077 686f 6c65 200d  d to the whole .
+00002410: 0a3b 0963 6f6d 706f 7369 7469 6f6e 206f  .;.composition o
+00002420: 6620 6561 6368 2069 6465 6e74 6966 6965  f each identifie
+00002430: 6420 676c 7963 616e 2069 6e20 7468 6520  d glycan in the 
+00002440: 0d0a 3b09 616e 616c 7973 6973 2c20 696e  ..;.analysis, in
+00002450: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
+00002460: 2070 6561 6b2d 7365 7061 7261 7465 6420   peak-separated 
+00002470: 6461 7461 2e0d 0a3b 0d0a 6f75 7470 7574  data...;..output
+00002480: 5f6d 6574 6162 6f61 6e61 6c79 7374 5f66  _metaboanalyst_f
+00002490: 696c 6520 3d20 6e6f 0d0a 6d65 7461 626f  ile = no..metabo
+000024a0: 616e 616c 7973 745f 6772 6f75 7073 203d  analyst_groups =
+000024b0: 2043 4f4e 5452 4f4c 2c20 5452 4541 5445   CONTROL, TREATE
+000024c0: 440d 0a3b 2009 4865 7265 2079 6f75 2073  D..; .Here you s
+000024d0: 6574 2075 7020 7768 6574 6865 7220 6f72  et up whether or
+000024e0: 206e 6f74 2079 6f75 2077 616e 7420 746f   not you want to
+000024f0: 206f 7574 7075 7420 0d0a 3b09 6120 2e63   output ..;.a .c
+00002500: 7376 2066 696c 6520 746f 2062 6520 7573  sv file to be us
+00002510: 6564 2066 6f72 2070 6c6f 7474 696e 6720  ed for plotting 
+00002520: 6461 7461 2075 7369 6e67 200d 0a3b 096d  data using ..;.m
+00002530: 6574 6162 6f61 6e61 6c79 7374 2e20 4966  etaboanalyst. If
+00002540: 2079 6f75 2077 616e 7420 7468 6174 2c20   you want that, 
+00002550: 796f 7520 6d75 7374 2073 7065 6369 6679  you must specify
+00002560: 200d 0a3b 0979 6f75 7220 7361 6d70 6c65   ..;.your sample
+00002570: 2067 726f 7570 732c 2063 6f6d 6d61 2073   groups, comma s
+00002580: 6570 6172 6174 6564 2e20 5361 6d70 6c65  eparated. Sample
+00002590: 200d 0a3b 0967 726f 7570 7320 7370 6563   ..;.groups spec
+000025a0: 6966 6965 6420 6d75 7374 2062 6520 7072  ified must be pr
+000025b0: 6573 656e 7420 696e 2073 616d 706c 6520  esent in sample 
+000025c0: 0d0a 3b09 6669 6c65 6e61 6d65 7320 666f  ..;.filenames fo
+000025d0: 7220 7072 6f70 6572 2069 6465 6e74 6966  r proper identif
+000025e0: 6963 6174 696f 6e2e 2049 6620 6e6f 6e65  ication. If none
+000025f0: 2069 7320 0d0a 3b09 7365 742c 2073 616d   is ..;.set, sam
+00002600: 706c 6573 2061 7265 2064 6566 6175 6c74  ples are default
+00002610: 6564 2074 6f20 2275 6e67 726f 7570 6564  ed to "ungrouped
+00002620: 222e 2043 6173 6520 7365 6e73 6974 6976  ". Case sensitiv
+00002630: 652e 200d 0a3b 0d0a 6f75 7470 7574 5f66  e. ..;..output_f
+00002640: 6974 7469 6e67 735f 6461 7461 203d 206e  ittings_data = n
+00002650: 6f0d 0a3b 2009 416c 6c6f 7773 2074 6f20  o..; .Allows to 
+00002660: 6f75 7470 7574 2066 696c 6573 2077 6974  output files wit
+00002670: 6820 7468 6520 6669 7474 696e 6773 2064  h the fittings d
+00002680: 6174 6120 746f 200d 0a3b 0963 6865 636b  ata to ..;.check
+00002690: 2073 636f 7269 6e67 2063 7269 7465 7269   scoring criteri
+000026a0: 6173 2e20 4465 6661 756c 7474 6564 2074  as. Defaultted t
+000026b0: 6f20 276e 6f27 2061 7320 0d0a 3b09 7468  o 'no' as ..;.th
+000026c0: 6573 6520 6669 6c65 7320 7769 6c6c 2062  ese files will b
+000026d0: 6520 6269 672e 204f 6e6c 7920 7573 6520  e big. Only use 
+000026e0: 6974 2069 6620 796f 7520 7265 616c 6c79  it if you really
+000026f0: 200d 0a3b 096e 6565 642e 0d0a 3b0d 0a6f   ..;.need...;..o
+00002700: 7574 7075 745f 706c 6f74 5f64 6174 6120  utput_plot_data 
+00002710: 3d20 6e6f 0d0a 3b20 0941 6c6c 6f77 7320  = no..; .Allows 
+00002720: 746f 206f 7574 7075 7420 6461 7461 2070  to output data p
+00002730: 6c6f 7474 696e 6720 6669 6c65 7320 666f  lotting files fo
+00002740: 7220 616c 6c20 7468 6520 0d0a 3b09 4549  r all the ..;.EI
+00002750: 4373 2064 7261 776e 2062 7920 7468 6520  Cs drawn by the 
+00002760: 7072 6f67 7261 6d2e 2049 6620 7365 7420  program. If set 
+00002770: 746f 2027 6e6f 272c 2069 7420 7769 6c6c  to 'no', it will
+00002780: 200d 0a3b 0973 7469 6c6c 206f 7574 7075   ..;.still outpu
+00002790: 7420 7468 6520 666f 756e 6420 676c 7963  t the found glyc
+000027a0: 616e 7320 4549 432e 0d0a 3b              ans EIC...;
```

### Comparing `glycogenius-1.1.7/glycogenius.egg-info/PKG-INFO` & `glycogenius-1.1.8/glycogenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glycogenius
-Version: 1.1.7
+Version: 1.1.8
 Summary: GlycoGenius is an all-in-one solution for data analysis of glycomics data.
 Author: Hector Franco Loponte
 Author-email: hectorfloponte@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `glycogenius-1.1.7/glycogenius.egg-info/SOURCES.txt` & `glycogenius-1.1.8/glycogenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.7/setup.py` & `glycogenius-1.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     for lines in f:
         if lines[0] != "!":
             long_description_from_file+= lines
     f.close()
 
 setup(
     name='glycogenius',
-    version='1.1.7',
+    version='1.1.8',
     author='Hector Franco Loponte',
     author_email='hectorfloponte@gmail.com',
     description='GlycoGenius is an all-in-one solution for data analysis of glycomics data.',
     long_description=long_description_from_file,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

