# Comparing `tmp/malet-0.1.7.tar.gz` & `tmp/malet-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malet-0.1.7.tar", last modified: Thu Mar  7 03:40:38 2024, max compression
+gzip compressed data, was "malet-0.1.8.tar", last modified: Tue Apr  2 13:52:29 2024, max compression
```

## Comparing `malet-0.1.7.tar` & `malet-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 03:40:38.674205 malet-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-07 03:40:30.000000 malet-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-03-07 03:40:38.674205 malet-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22931 2024-03-07 03:40:30.000000 malet-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-07 03:40:30.000000 malet-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 03:40:38.674205 malet-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 03:40:38.670205 malet-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 03:40:38.670205 malet-0.1.7/src/malet/
--rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/get_slurm_run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 03:40:38.674205 malet-0.1.7/src/malet/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/plot_utils/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/plot_utils/plot_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/plot_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-07 03:40:30.000000 malet-0.1.7/src/malet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 03:40:38.674205 malet-0.1.7/src/malet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-03-07 03:40:38.000000 malet-0.1.7/src/malet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-07 03:40:38.000000 malet-0.1.7/src/malet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 03:40:38.000000 malet-0.1.7/src/malet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 03:40:38.000000 malet-0.1.7/src/malet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-07 03:40:38.000000 malet-0.1.7/src/malet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 03:40:38.000000 malet-0.1.7/src/malet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.183107 malet-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 13:52:21.000000 malet-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-04-02 13:52:29.183107 malet-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22931 2024-04-02 13:52:21.000000 malet-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-02 13:52:21.000000 malet-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:52:29.183107 malet-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.179108 malet-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.179108 malet-0.1.8/src/malet/
+-rw-r--r--   0 runner    (1001) docker     (127)    24765 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/get_slurm_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.183107 malet-0.1.8/src/malet/plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot_utils/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot_utils/plot_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.183107 malet-0.1.8/src/malet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/top_level.txt
```

### Comparing `malet-0.1.7/LICENSE` & `malet-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/PKG-INFO` & `malet-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malet
-Version: 0.1.7
+Version: 0.1.8
 Summary: Malet: a tool for machine learning experiment
 Author-email: Dongyeop Lee <dylee23@postech.ac.kr>
 License: Copyright (c) 2023 Dongyeop Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `malet-0.1.7/README.md` & `malet-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/pyproject.toml` & `malet-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 packages = ["malet", "malet.plot_utils"]
 package-dir = {""="src"}
 
 [project]
 name = "malet"
-version = "0.1.7"
+version = "0.1.8"
 description = "Malet: a tool for machine learning experiment"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["machine learning", "experiment", "plot"]
 authors = [
   {name = "Dongyeop Lee", email = "dylee23@postech.ac.kr"},
```

### Comparing `malet-0.1.7/src/malet/experiment.py` & `malet-0.1.8/src/malet/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,37 +151,34 @@
   
 
 @dataclass
 class ExperimentLog:
   static_configs: dict
   grid_fields: list
   logs_file: str
-  info_fields: list
   
   metric_fields: Optional[list] = None
   df: Optional[pd.DataFrame]=None
   auto_update_tsv: bool = False
   
   __sep: ClassVar[str] = '-'*45 + '\n'
   
   def __post_init__(self):
     if self.df is None:
       assert self.metric_fields is not None, 'Specify the metric fields of the experiment.'
       assert not (f:=set(self.grid_fields) & set(self.metric_fields)), f'Overlapping field names {f} in grid_fields and metric_fields. Remove one of them.'
-      columns = self.grid_fields + self.info_fields + self.metric_fields
-      self.df = pd.DataFrame(columns=columns).set_index(self.grid_fields)
+      self.df = pd.DataFrame(columns=self.grid_fields+self.metric_fields).set_index(self.grid_fields)
     else:
-      self.metric_fields = [i for i in list(self.df) if i not in self.info_fields]
-    self.field_order = self.info_fields + self.metric_fields
+      self.metric_fields = list(self.df)
   
   # Constructors.
   # -----------------------------------------------------------------------------  
   @classmethod
-  def from_exp_config(cls, exp_config, logs_file: str, info_fields: list, metric_fields: Optional[list]=None, auto_update_tsv: bool=False):
-    return cls(*(exp_config[k] for k in ['static_configs', 'grid_fields']), logs_file=logs_file, info_fields=info_fields,
+  def from_exp_config(cls, exp_config, logs_file: str, metric_fields: Optional[list]=None, auto_update_tsv: bool=False):
+    return cls(*(exp_config[k] for k in ['static_configs', 'grid_fields']), logs_file=logs_file,
                metric_fields=metric_fields, auto_update_tsv = auto_update_tsv)
 
   @classmethod
   def from_tsv(cls, logs_file: str, parse_str=True, auto_update_tsv: bool=False):
     '''open tsv with yaml header'''
     return cls(**cls.parse_tsv(logs_file, parse_str=parse_str), logs_file=logs_file, auto_update_tsv=auto_update_tsv)
   
@@ -214,27 +211,23 @@
       idx = csv_idx.strip().split('\t')
       csv_head = '\t'.join(idx+col)
       csv_str = '\n'.join([csv_head, *csv_body])
       
       df = pd.read_csv(io.StringIO(csv_str), sep='\t')
       df = df.drop(['id'], axis=1)
       
-      # make str(list) to list
-      if not df.empty:
-        list_filt = lambda f: isinstance(v:=df[f].iloc[0], str) and ('[' in v or '(' in v)
-        list_fields = [*filter(list_filt, list(df))]
-        if parse_str:
-          df[list_fields] = df[list_fields].applymap(str2value)
+      if parse_str:
+          df = df.applymap(str2value)
       
       # set grid_fields to multiindex
       df = df.set_index(idx[1:])
       
     return {'static_configs': static_configs,
             'grid_fields': idx[1:],
-            'info_fields': list(df),
+            'metric_fields': list(df),
             'df': df}
   
 
   def load_tsv(self, logs_file, parse_str=True):
     '''load tsv with yaml header'''
     if logs_file is not None:
       self.logs_file=logs_file
@@ -282,26 +275,41 @@
     return wrapped
 
   
   # Add results.
   # -----------------------------------------------------------------------------
   
   @partial(update_tsv, mode='r')
-  def add_result(self, configs, metrics=dict(), **infos):
+  def add_result(self, configs, **metrics):
     '''Add experiment run result to dataframe'''
+    if configs in self:
+      cur_gridval = list2tuple([configs[k] for k in self.grid_fields])
+      self.df = self.df.drop(cur_gridval)
+    
+    configs = {k:list2tuple(configs[k]) for k in self.grid_fields}
+    metrics = {k:metrics.get(k) for k in self.metric_fields}
+    result_dict = {k:[v] for k, v in {**configs, **metrics}.items()}
+    result_df = pd.DataFrame(result_dict).set_index(self.grid_fields)
+    self.df = pd.concat([self.df, result_df])[self.metric_fields]
+    
+    # Dataframe.loc based code
+    # problem: pandas unable to distinguish between 
+    #              ``.loc[(col_idx, row_idx)]`` and ``.loc[(multi_idx_1, multi_idx_2)]``
+    #          for 2-level multiindex dataframe
+    """
     cur_gridval = list2tuple([configs[k] for k in self.grid_fields])
     
-    row_dict = {**infos, **metrics}
-    df_row = [row_dict.get(k) for k in self.field_order]
+    df_row = [metrics.get(k) for k in self.field_order]
       
     # Write over metric results if there is a config saved
     if configs in self:
       self.df = self.df.drop(cur_gridval)
     
     self.df.loc[cur_gridval] = df_row
+    """
     
   @staticmethod
   def __add_column(df, new_column_name, fn, *fn_arg_fields):
     '''Add new column field computed from existing fields in self.df'''
     def mapper(*args):
       if all(isinstance(i, (int, float, str, tuple, list)) for i in args):
         return fn(*args)
@@ -364,19 +372,18 @@
       self.df[sf] = [list2tuple(self.static_configs.get(sf, np.nan))]*len(self)
 
     for sf in new_to_othr_sf:
       other.df[sf] = [list2tuple(other.static_configs.get(sf, np.nan))]*len(other)
 
     self.static_configs = new_sttc
     self.grid_fields += new_to_self_sf
-    self.field_order = self.info_fields + self.metric_fields
     
     self.df, other.df = (obj.df.reset_index() for obj in (self, other))
-    self.df = pd.concat([self.df, other.df])[self.grid_fields+self.field_order] \
-                .set_index(self.grid_fields)
+    self.df = pd.concat([self.df, other.df]) \
+                .set_index(self.grid_fields)[self.metric_fields]
     return self
 
   def merge(self, *others, same=True):
     '''Merge multiple logs into self'''
     for other in others:
       self.__merge_one(other, same=same)
 
@@ -407,28 +414,27 @@
   
   
   @partial(update_tsv, mode='r')
   def isin(self, config):
     '''Check if specific experiment config was already executed in log.'''
     if self.df.empty: return False
 
-    cfg_same_with = lambda dct: [config[d]==dct[d] for d in dct.keys()]
+    cfg_same_in_static = all([config[k]==v for k, v in self.static_configs.items() if k in config])
     cfg_matched_df = self.__cfg_match_row(config)
     
-    return all(cfg_same_with(self.static_configs)) and not cfg_matched_df.empty
+    return cfg_same_in_static and not cfg_matched_df.empty
 
 
-  def get_metric_and_info(self, config):
+  def get_metric(self, config):
     '''Search matching log with given config dict and return metric_dict, info_dict'''
     assert config in self, 'config should be in self when using get_metric_dict.'
     
     cfg_matched_df = self.__cfg_match_row(config)
     metric_dict = {k:(v.iloc[0] if not (v:=cfg_matched_df[k]).empty else None) for k in self.metric_fields}
-    info_dict = {k:(v.iloc[0] if not (v:=cfg_matched_df[k]).empty else None) for k in self.info_fields}
-    return metric_dict, info_dict
+    return metric_dict
 
   def is_same_exp(self, other):
     '''Check if both logs have same config fields.'''
     fields = lambda log: set(log.static_configs.keys()) | set(log.grid_fields)
     return fields(self)==fields(other)
     
     
@@ -454,16 +460,16 @@
     
     df['metric_value'] = df.apply(lambda df: df['metric_value'][df.step-1] if isinstance(df['metric_value'], list) else df['metric_value'], axis=1) # list[epoch] for all fields
     
     df = mov_to_index('step', 'total_steps')
     
     # delete string and NaN valued rows
     df = df[pd.to_numeric(df['metric_value'], errors='coerce').notnull()]\
-           .dropna()\
-           .astype('float')
+              .dropna()\
+              .astype('float')
     
     return df
 
     
   def __contains__(self, config):
     return self.isin(config)
 
@@ -488,16 +494,14 @@
   
   Following is supported
   - Provides 2 methods parallel friedly experiments scheduling (can choose with bash arguments).
     - (plan splitting) Splits experiment plans evenly.
     - (current run checking) Save configs of currently running experiments to tsv so other running code can know.
   - Saves experiment logs, automatically resumes experiment using saved log.
   '''
-  info_field: ClassVar[list] = ['datetime', 'status']
-  
   __RUNNING: ClassVar[str] = 'R'
   __FAILED: ClassVar[str] = 'F'
   __COMPLETED: ClassVar[str] = 'C'
   
   def __init__(self, 
                exp_folder_path: str,
                exp_function: ExpFunc,
@@ -553,30 +557,30 @@
     # Configure experiment log
     if os.path.exists(logs_file): # Check if there already is a file
       log = ExperimentLog.from_tsv(logs_file, auto_update_tsv=auto_update_tsv) # resumes automatically
     else: # Create new log
       logs_path, _ = os.path.split(logs_file)
       if not os.path.exists(logs_path):
         os.makedirs(logs_path)
-      log = ExperimentLog.from_exp_config(self.configs.__dict__, logs_file, self.info_field, 
+      log = ExperimentLog.from_exp_config(self.configs.__dict__, logs_file,
                                           metric_fields=metric_fields, auto_update_tsv=auto_update_tsv)
       log.to_tsv()
     return log
   
   
   @staticmethod
   def get_paths(exp_folder):
     cfg_file = os.path.join(exp_folder, 'exp_config.yaml')
     tsv_file = os.path.join(exp_folder, 'log.tsv')
     fig_dir = os.path.join(exp_folder, 'figure')
     return cfg_file, tsv_file, fig_dir
   
   def get_log_checkpoint(self, config, empty_metric):
-    metric_dict, info_dict = self.log.get_metric_and_info(config)
-    if info_dict['status'] == self.__FAILED:
+    metric_dict = self.log.get_metric(config)
+    if metric_dict['status'] == self.__FAILED:
       return metric_dict
     return empty_metric
     
   def update_log(self, metric_dict, config):
     self.log.add_result(metric_dict, configs=config, 
                         datetime=str(datetime.now()), status=self.__RUNNING)
     self.log.to_tsv()
@@ -589,16 +593,16 @@
     elif isinstance(self.exp_bs, str):
       logging.info(f'Experiment : {self.configs.name} (split : {self.exp_bi}/{self.configs.grid_dict[self.exp_bs]})')
     
     # run experiment plans 
     for i, config in enumerate(self.configs):
 
       if config in self.log:
-        metric_dict, info_dict = self.log.get_metric_and_info(config)
-        if info_dict.get('status') != self.__FAILED:
+        metric_dict = self.log.get_metric(config)
+        if metric_dict.get('status') != self.__FAILED:
           continue # skip already executed runs
       
       # if config not in self.log or status==self.__FAILED
       if self.configs_save:
         self.log.add_result(config, status=self.__RUNNING)
         self.log.to_tsv()
 
@@ -614,16 +618,17 @@
           metric_dict = self.exp_func(config)
       except:
         self.log.add_result(config, status=self.__FAILED)
         self.log.to_tsv()
         raise
       
       # Open log file and add result
-      self.log.add_result(config, metrics=metric_dict,
-                          datetime=str(datetime.now()), status=self.__COMPLETED)
+      self.log.add_result(config, **metric_dict,
+                          datetime=str(datetime.now()), 
+                          status=self.__COMPLETED)
       self.log.to_tsv()
       
       logging.info("Saved experiment data to log")
       
       
   @staticmethod
   def resplit_logs(exp_folder_path: str, target_split: int=1, save_backup: bool=True):
@@ -655,20 +660,19 @@
       # get configs
       configs = ConfigIter(cfg_file)
       
       for n in range(target_split):
         # empty log
         lgs = ExperimentLog.from_exp_config(configs.__dict__, 
                                             os.path.join(logs_folder, f'split_{n}.tsv',),
-                                            base.info_fields,
                                             base.metric_fields)
         
         # resplitting nth split
         cfgs_temp = copy.deepcopy(configs)
         cfgs_temp.filter_iter(lambda i, _: i%target_split==n)
         for cfg in track(cfgs_temp, description=f'split: {n}/{target_split}'):
           if cfg in base:
-            metric_dict, info_dict = base.get_metric_and_info(cfg)
-            lgs.add_result(cfg, metric_dict, **info_dict)
+            metric_dict = base.get_metric(cfg)
+            lgs.add_result(cfg, **metric_dict)
           
         lgs.to_tsv()
```

### Comparing `malet-0.1.7/src/malet/get_slurm_run_status.py` & `malet-0.1.8/src/malet/get_slurm_run_status.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/src/malet/plot.py` & `malet-0.1.8/src/malet/plot.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/src/malet/plot_utils/data_processor.py` & `malet-0.1.8/src/malet/plot_utils/data_processor.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/src/malet/plot_utils/plot_drawer.py` & `malet-0.1.8/src/malet/plot_utils/plot_drawer.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/src/malet/plot_utils/utils.py` & `malet-0.1.8/src/malet/plot_utils/utils.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.7/src/malet/utils.py` & `malet-0.1.8/src/malet/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,8 +34,13 @@
   if isinstance(l, dict):
     return {k: list2tuple(v) for k, v in l.items()}
   return l
     
 
 def str2value(value_str):
     """Casts string back to standard python types"""
-    return literal_eval(value_str) if isinstance(value_str, str) else value_str
+    if not isinstance(value_str, str): return value_str
+    value_str = value_str.replace('inf', '2e+308')
+    try:
+      return literal_eval(value_str)
+    except:
+      return value_str
```

### Comparing `malet-0.1.7/src/malet.egg-info/PKG-INFO` & `malet-0.1.8/src/malet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malet
-Version: 0.1.7
+Version: 0.1.8
 Summary: Malet: a tool for machine learning experiment
 Author-email: Dongyeop Lee <dylee23@postech.ac.kr>
 License: Copyright (c) 2023 Dongyeop Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

