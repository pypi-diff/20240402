# Comparing `tmp/prosper_nn-0.2.3.tar.gz` & `tmp/prosper_nn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosper_nn-0.2.3.tar", last modified: Tue Jun  6 09:46:02 2023, max compression
+gzip compressed data, was "prosper_nn-0.3.0.tar", last modified: Tue Apr  2 08:04:30 2024, max compression
```

## Comparing `prosper_nn-0.2.3.tar` & `prosper_nn-0.3.0.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/autoencoder/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/autoencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/crcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/crcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17311 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/crcnn/crcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/deep_feed_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/dhcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/dhcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/dhcnn/dhcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/ecnn/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_lstm_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.347272 prosper_nn-0.2.3/prosper_nn/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ensemble/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.347272 prosper_nn-0.2.3/prosper_nn/models/feedforward/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/feedforward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/feedforward/feedforward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.351272 prosper_nn-0.2.3/prosper_nn/models/fuzzy/
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/Data_Intake.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/defuzzification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/frnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzy_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/rule_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.351272 prosper_nn-0.2.3/prosper_nn/models/hcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_lstm_cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.351272 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u.py
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/prosper_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/create_input_ecnn_hcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/generate_time_series_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/neuron_correlation_hidden_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/sensitivity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/visualize_forecasts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.474296 prosper_nn-0.3.0/prosper_nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/autoencoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/autoencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/autoencoder/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/crcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/crcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17413 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/crcnn/crcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/deep_feed_forward/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/deep_feed_forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/deep_feed_forward/deep_feed_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/dhcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/dhcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/dhcnn/dhcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/ecnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/ecnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/ecnn/ecnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/ecnn/ecnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/ecnn/gru_cell_variant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/ensemble/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.478296 prosper_nn-0.3.0/prosper_nn/models/feedforward/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/feedforward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/feedforward/feedforward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/prosper_nn/models/fuzzy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/Data_Intake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/defuzzification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/frnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/fuzzification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/fuzzy_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/membership_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/membership_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/fuzzy/rule_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/prosper_nn/models/hcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11672 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn/hcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn/hcnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn/hcnn_gru_cell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/prosper_nn/models/hcnn_compressed/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn_compressed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn_compressed/hcnn_cell_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn_compressed/hcnn_compressed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/hcnn_known_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/prosper_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/create_input_ecnn_hcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/generate_time_series_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/neuron_correlation_hidden_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12975 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/prosper_nn/utils/visualize_forecasts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:04:30.474296 prosper_nn-0.3.0/prosper_nn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-02 08:04:30.000000 prosper_nn-0.3.0/prosper_nn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 08:04:30.000000 prosper_nn-0.3.0/prosper_nn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:04:30.000000 prosper_nn-0.3.0/prosper_nn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 08:04:30.000000 prosper_nn-0.3.0/prosper_nn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 08:04:30.000000 prosper_nn-0.3.0/prosper_nn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:04:30.482296 prosper_nn-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 08:00:02.000000 prosper_nn-0.3.0/setup.py
```

### Comparing `prosper_nn-0.2.3/LICENSE` & `prosper_nn-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/PKG-INFO` & `prosper_nn-0.3.0/prosper_nn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
-Name: prosper_nn
-Version: 0.2.3
+Name: prosper-nn
+Version: 0.3.0
 Summary: Package contains, in PyTorch implemented, neural networks with problem specific pre-structuring architectures and utils that help building and understanding models.
 Home-page: UNKNOWN
 Author: Nico Beck, Julia Schemm
 Author-email: nico.beck@iis.fraunhofer.de
 License: UNKNOWN
+Description: # Prosper_NN
+        
+        ## Problem-Specific Pre-Structuring of Neural Networks
+        
+        Accurate data-driven forecasts can provide a crucial advantage in many application areas. One of the methods with the most promising results in forecasting time series are neural networks. However, especially in macro-economic applications, it can be difficult and time-consuming to adapt state-of-the-art neural network architectures in a way that leads to satisfying results. For instance, the final prices of materials and stocks result from a highly complex interplay between supply and demand. Additionally, there is often only one (albeit long) historical time series available for training which makes correlations in the data difficult to detect.
+        
+        Under these circumstances, applying state-of-the-art neural networks architectures successfully poses a great challenge. Pre-structuring the models can solve this problem. For this purpose, Zimmermann, Tietz and Grothmann (Neural Networks: Tricks of the Trade, 2012) propose recurrent architectures for various time series problems that help recognize correlations. They recommend Error-Correction Neural Networks (ECNNs), Historical-Consistent Neural Networks (HCNNs) and Causal-Retro-Causal Neural Networks (CRCNNs). One of the main ideas of the pre-structuring is embedding the model in a larger architecture in order to use the past prediction errors for predicting the next time step. The three approaches mentioned use this idea and apply it in different settings. So far, the proposed architectures are not publicly available in common machine learning frameworks. Therefore, we have implemented the models in PyTorch. This way, we can easily test them on diverse datasets.
+        In this package the neural network architectures developed by Hans-Georg Zimmermann are implemented in PyTorch.
+        The full documentation can be found here https://iis-scs-a.pages.fraunhofer.de/prosper/prosper/. There are also tutorials that show how to work with the package.
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Prosper_NN
-
-## Problem-Specific Pre-Structuring of Neural Networks
-
-Accurate data-driven forecasts can provide a crucial advantage in many application areas. One of the methods with the most promising results in forecasting time series are neural networks. However, especially in macro-economic applications, it can be difficult and time-consuming to adapt state-of-the-art neural network architectures in a way that leads to satisfying results. For instance, the final prices of materials and stocks result from a highly complex interplay between supply and demand. Additionally, there is often only one (albeit long) historical time series available for training which makes correlations in the data difficult to detect.
-
-Under these circumstances, applying state-of-the-art neural networks architectures successfully poses a great challenge. Pre-structuring the models can solve this problem. For this purpose, Zimmermann, Tietz and Grothmann (Neural Networks: Tricks of the Trade, 2012) propose recurrent architectures for various time series problems that help recognize correlations. They recommend Error-Correction Neural Networks (ECNNs), Historical-Consistent Neural Networks (HCNNs) and Causal-Retro-Causal Neural Networks (CRCNNs). One of the main ideas of the pre-structuring is embedding the model in a larger architecture in order to use the past prediction errors for predicting the next time step. The three approaches mentioned use this idea and apply it in different settings. So far, the proposed architectures are not publicly available in common machine learning frameworks. Therefore, we have implemented the models in PyTorch. This way, we can easily test them on diverse datasets.
-In this package the neural network architectures developed by Hans-Georg Zimmermann are implemented in PyTorch.
-The full documentation can be found here https://iis-scs-a.pages.fraunhofer.de/prosper/prosper/. There are also tutorials that show how to work with the package.
-
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/autoencoder/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder.py` & `prosper_nn-0.3.0/prosper_nn/models/autoencoder/autoencoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 class Autoencoder(nn.Module):
     """
     An autoencoder that encodes an input into a smaller representation.
     Additionally the model trains a decoder to map the encoded representation back
     to the original dimension.
     """
+
     def __init__(
         self,
         n_inputs: int,
         n_hidden_neurons: int,
         activation: Type[torch.autograd.Function] = torch.tanh,
     ) -> None:
         """
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py` & `prosper_nn-0.3.0/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,25 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from .autoencoder import Autoencoder
-from ..ecnn.ecnn_model import ECNN
+from ..ecnn.ecnn import ECNN
 import torch
 from typing import Tuple
 
 
 class EcnnAutoencoder(torch.nn.Module):
     """
     The module trains an on features encoded with an autoencoder.
     The autoencoder for the encoding can be trained parallel to the ECNN.
     """
+
     def __init__(self, autoencoder: Autoencoder, ecnn: ECNN) -> None:
         """
         Parameters
         ----------
         autoencoder : Autoencoder
             An autoencoder with a encoder and a decoder.
         ecnn : ECNN
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/crcnn/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/crcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/crcnn/crcnn.py` & `prosper_nn-0.3.0/prosper_nn/models/crcnn/crcnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,28 +170,31 @@
             Contains past_error, i.e. the forecasting errors along the past_horizon where Y is known, and forecast, i.e. the forecast along the forecast_horizon, for each pair of causal and retro causal branches.
             If mirroring = True, the forecast contains the fake forecasting errors produced by using the future_bias as a fake future Y. In this case, therefore, the forecast should be used for training and the target should be 0.
             shape=(n_branches-1, past_horizon + forecast_horizon, batchsize, n_features_Y)
         """
 
         self._check_sizes(Y)
 
+        device = self.CRCNNCell_causal.A.weight.device
+
         if self.mirroring:
             future_bias = self.future_bias
         else:
             future_bias = [None] * self.forecast_horizon
 
         # reset saved cell outputs
         past_error = torch.zeros(
-            self.n_branches - 1, self.past_horizon, self.batchsize, self.n_features_Y
+            (self.n_branches - 1, self.past_horizon, self.batchsize, self.n_features_Y), device=device
         )
         forecast = torch.zeros(
-            self.n_branches - 1,
+            (self.n_branches - 1,
             self.forecast_horizon,
             self.batchsize,
-            self.n_features_Y,
+            self.n_features_Y,),
+            device=device
         )
 
         # initialize causal and retro-causal branches
         for i in range(self.n_causal_branches):
             self.state_causal[i][0], _ = self.CRCNNCell_causal(
                 self.init_state_causal.repeat(self.batchsize, 1)
             )
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/deep_feed_forward/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/deep_feed_forward.py` & `prosper_nn-0.3.0/prosper_nn/models/deep_feed_forward/deep_feed_forward.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def __init__(
         self,
         input_dim: int,
         hidden_dim: int,
         output_dim: int,
         deepness: int,
-        activation: Type[torch.autograd.Function] = None,
+        activation: Type[torch.autograd.Function] = torch.tanh,
         dropout_rate: float = 0.0,
     ) -> None:
         """
         Parameters
         ----------
         input_dim : int
             The input dimension of the model.
@@ -77,33 +77,25 @@
         self.deepness = deepness
         self.activation = activation
         self.dropout_rate = dropout_rate
 
         self._check_variables()
 
         # Define Layers
-        for level in range(self.deepness):
-            setattr(
-                self,
-                "hidden_layer%d" % level,
-                nn.Linear(self.input_dim, self.hidden_dim),
-            )
-
-            if level < self.deepness:
-                setattr(
-                    self,
-                    "hidden_layer_connector%d" % level,
-                    nn.Linear(self.hidden_dim, self.hidden_dim),
-                )
-
-            setattr(
-                self,
-                "output_layer%d" % level,
-                nn.Linear(self.hidden_dim, self.output_dim),
-            )
+        self.hidden_layer = [nn.Linear(self.input_dim, self.hidden_dim) for _ in range(self.deepness)]
+        self.hidden_layer = nn.ModuleList(self.hidden_layer)
+
+        self.hidden_layer_connector = [nn.Linear(self.hidden_dim, self.hidden_dim) for _ in range(self.deepness - 1)]
+        self.hidden_layer_connector = nn.ModuleList(self.hidden_layer_connector)
+
+        self.output_layer = [nn.Linear(self.hidden_dim, self.output_dim) for _ in range(self.deepness)]
+        self.output_layer = nn.ModuleList(self.output_layer)
+
+        if self.dropout_rate > 0:
+            self.dropout = nn.Dropout(self.dropout_rate)
 
     def forward(self, x: torch.Tensor) -> torch.tensor:
         """
         Parameters
         ----------
         x : torch.Tensor
             The input tensor given to the Deep-Feed-Forward Neural Network.
@@ -112,52 +104,45 @@
         Returns
         -------
         torch.Tensor
             A output of a level in the model is stored in the tensor with the index that is equal to the level.
             Therefore the first dimension corresponds to the level of deepness in the model.
             The complete output shape is: shape=(deepness, batchsize, output_dim).
         """
-
+        device = self.hidden_layer[0].weight.device
         # Dropout on Input
         if self.dropout_rate > 0:
-            x = nn.Dropout(self.dropout_rate)(x)
+            x = self.dropout(x)
+
         # All Connections to Hidden Layers
-        self.output_hidden_layer = self.deepness * [None]
+        output_hidden_layer = self.deepness * [None]
+
         for level in range(self.deepness):
-            self.horizontal_path = getattr(self, "hidden_layer%d" % level)(x)
+            horizontal_path = self.hidden_layer[level](x)
             if level > 0:
-                self.vertical_path = getattr(
-                    self, "hidden_layer_connector%d" % (level - 1)
-                )(self.output_hidden_layer[level - 1])
-                self.output_hidden_layer[level] = (
-                    self.horizontal_path + self.vertical_path
-                )
+                vertical_path = self.hidden_layer_connector[level - 1](output_hidden_layer[level - 1])
+                output_hidden_layer[level] = (horizontal_path + vertical_path)
             else:
-                self.output_hidden_layer[level] = self.horizontal_path
-            if self.activation is not None:
-                self.output_hidden_layer[level] = self.activation(
-                    self.output_hidden_layer[level]
-                )
+                output_hidden_layer[level] = horizontal_path
+
+            output_hidden_layer[level] = self.activation(output_hidden_layer[level])
 
         # All Connections to Output Layers
-        self.output_output_layer = torch.empty(self.deepness, x.size(0), 1)
+        output_output_layer = torch.empty(((self.deepness,) + x.shape[:-1] + (self.output_dim,)), device=device)
 
         for level in range(self.deepness):
-            self.horizontal_path = getattr(self, "output_layer%d" % level)(
-                self.output_hidden_layer[level]
-            )
+            horizontal_path = self.output_layer[level](output_hidden_layer[level])
+
             if level > 0:
-                self.vertical_path = (self.output_output_layer[level - 1]).detach()
-                self.output_output_layer[level] = (
-                    self.horizontal_path + self.vertical_path
-                )
+                vertical_path = (output_output_layer[level - 1]).detach()
+                output_output_layer[level] = (horizontal_path + vertical_path)
             else:
-                self.output_output_layer[level] = self.horizontal_path
+                output_output_layer[level] = horizontal_path
 
-        return self.output_output_layer
+        return output_output_layer
 
     def _check_variables(self) -> None:
         """
         Checks if self.input_dim, self.hidden_dim, self.output_dim,
         self.deepness, self.dropout_rate have valid inputs.
         Parameters
         ----------
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/dhcnn/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/dhcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/dhcnn/dhcnn.py` & `prosper_nn-0.3.0/prosper_nn/models/dhcnn/dhcnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,23 @@
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch.nn as nn
 import torch
 from typing import Optional
-from ..hcnn import hcnn_cell, hcnn_lstm_cell
+from ..hcnn import hcnn_cell, hcnn_gru_cell
 
 
 class DHCNN(nn.Module):
     """
     The DHCNN class creates a Deep Historical Consistent Neural Network.
     The model uses multiple HCNNs in different levels. The state from the lower
-    level is passed to one upper level. The first level is a HCNN with LSTM implementation.
+    level is passed to one upper level. The first level is a HCNN with the
+    GRU variant 3 implementation.
     """
 
     def __init__(
         self,
         n_state_neurons: int,
         n_features_Y: int,
         past_horizon: int,
@@ -64,15 +65,16 @@
             therefore the amount of teacher forcing.
         forecast_horizon : int
             The forecast horizon gives the amount of time steps into the future,
             where no observation is available.
             It represents the amount of forecast steps the model returns.
         deepness : int
             The number of stacked HCNNs in the Neural Network.
-            A deepness equal to 1 leads to a normal Historical Consistent Neural Network with LSTM.
+            A deepness equal to 1 leads to a normal
+            Historical Consistent Neural Network with GRU variant 3 implementation.
         sparsity : float
             The share of weights that are set to zero in the matrix A.
             These weights are not trainable and therefore always zero.
             For big matrices (dimension > 50) this can be necessary to guarantee
             numerical stability and it increases the long-term memory of the model.
         activation : torch
             The activation function that is applied on the output of the hidden layers.
@@ -120,15 +122,15 @@
                 requires_grad=learn_init_state,
             )
             if init_state is not None:
                 self.init_state.data = init_state
 
         for i in range(deepness):
             if i == 0:
-                HCNNCell = hcnn_lstm_cell.HCNN_LSTM_Cell
+                HCNNCell = hcnn_gru_cell.HCNN_GRU_3_variant
             else:
                 HCNNCell = hcnn_cell.HCNNCell
             setattr(
                 self,
                 "hcnn_cell_level%d" % i,
                 HCNNCell(
                     self.n_state_neurons,
@@ -153,32 +155,25 @@
             Contains for each HCNN level: The past_error, i.e. the forecasting errors along the past_horizon
             where Y is known, and forecast, i.e. the forecast along the
             forecast_horizon. Both can be used for backpropagation.
             shape=(deepness, past_horizon+forecast_horizon, batchsize, n_features_Y)
         """
         self._check_sizes(Y)
         self.batchsize = Y.shape[1]
+        device = self.init_state.device
 
         if self.decrease_teacher_forcing > 0:
             self._adjust_teacher_forcing()
 
         # reset saved cell outputs
         past_error = torch.zeros(
-            self.deepness, self.past_horizon, self.batchsize, self.n_features_Y
+            (self.deepness, self.past_horizon, self.batchsize, self.n_features_Y), device=device
         )
         forecast = torch.zeros(
-            self.deepness, self.forecast_horizon, self.batchsize, self.n_features_Y
-        )
-
-        # LSTM: Keep entries of diagonal matrix between 0 and 1.
-        diag_entries = torch.clamp(
-            self.hcnn_cell_level0.LSTM_regulator.weight.data, 0, 1
-        )
-        self.hcnn_cell_level0.LSTM_regulator.weight.data = torch.nn.Parameter(
-            diag_entries
+            (self.deepness, self.forecast_horizon, self.batchsize, self.n_features_Y), device=device
         )
 
         # past
         for i in range(self.deepness):
             horizontal_stream = self.init_state[i].repeat(self.batchsize, 1)
             for t in range(self.past_horizon):
                 # state is the sum of state from left side and upstream state for higher levels
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/ecnn/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/ecnn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-from .ecnn_model import *
+from .ecnn import *
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_lstm_cell.py` & `prosper_nn-0.3.0/prosper_nn/models/ecnn/ecnn_cell.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-""""""
 """
 Prosper_nn provides implementations for specialized time series forecasting
 neural networks and related utility functions.
 
 Copyright (C) 2022 Nico Beck, Julia Schemm, Henning Frechen, Jacob Fidorra,
     Denni Schmidt, Sai Kiran Srivatsav Gollapalli
 
@@ -20,131 +19,139 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch
 import torch.nn as nn
-from typing import Tuple, Type
+from .gru_cell_variant import GRU_3_variant
+from typing import Tuple, Union, Optional
 
 
-class ECNN_LSTM_Cell(nn.Module):
-
+class ECNNCell(nn.Module):
     """
-    LSTM cell of a Error-Correction Neural Network (ECNN).
-    Compared to the normal ECNN cell, $s_t$ is calculated differently:
+    Cell of a Error-Correction Neural Network (ECNN).
+    It models one time step of an ECNN:
 
     .. math::
-        s_t = (1- LSTMregulator)s_{t-1} + LSTMregulator(tanh(As_{t-1} + Bu_t))
+        s_t = tanh(As_{t-1} + Bu_t + D(\hat{y}_{t-1} - y_{t-1}))
+        \hat{y}_t = Cs_t
 
-    The LSTM regulator is a diagonal matrix with diagonal entries between 0 and 1. At the start of learning, they are
-    all set to one, which means, that the architecture defaults to the regular ECNN architecture. The other extreme
-    would be for the LSTM regulator to only have entries which are 0. Then $s_t=s_{t-1}$ and there is total
-    long-term memory.
     """
 
     def __init__(
         self,
         n_features_U: int,
         n_state_neurons: int,
-        activation: Type[torch.autograd.Function] = torch.tanh,
         n_features_Y: int = 1,
+        recurrent_cell_type: str = "elman",
+        kwargs_recurrent_cell: dict = {},
     ):
         """
-
         Parameters
         ----------
         n_features_U: int
             The number of inputs, i.e. the number of elements of U at each time
             step.
         n_state_neurons: int
             The number of neurons of the hidden layer, i.e. the hidden state state
             at each time step.
-        activation : nn.functional, optional
-            The activation function that is applied on the output of the hidden layers.
-            The same function is used on all hidden layers.
         n_features_Y: int
             The number of outputs, i.e. the number of elements of Y at each time
             step. The default is 1.
-
+        recurrent_cell_type: str
+            Select the cell for the state transition. The cells elman, lstm, gru
+            (all from pytorch) and gru_3_variant (from prosper_nn) are supported.
+        kwargs_recurrent_cell: dict
+            Parameters for the recurrent cell. Activation function can be set here.
 
         Returns
         -------
         None
 
         """
-        super(ECNN_LSTM_Cell, self).__init__()
+        super(ECNNCell, self).__init__()
 
-        self.A = nn.Linear(n_state_neurons, n_state_neurons, bias=False)
-        self.B = nn.Linear(n_features_U, n_state_neurons, bias=False)
         self.C = nn.Linear(n_state_neurons, n_features_Y, bias=False)
-        self.D = nn.Linear(n_features_Y, n_state_neurons, bias=False)
-        self.LSTM_regulator = nn.Linear(1, n_state_neurons, bias=False)
-        nn.init.ones_(self.LSTM_regulator.weight)
 
-        self.act = activation
+        if recurrent_cell_type == "elman":
+            self.recurrent_cell = nn.RNNCell
+        elif recurrent_cell_type == "lstm":
+            self.recurrent_cell = nn.LSTMCell
+        elif recurrent_cell_type == "gru":
+            self.recurrent_cell = nn.GRUCell
+        elif recurrent_cell_type == "gru_3_variant":
+            self.recurrent_cell = GRU_3_variant
+        else:
+            raise ValueError(
+                f"recurrent_cell_type: {recurrent_cell_type} is not known."
+                "Choose from elman, lstm, gru or gru_3_variant."
+            )
+        self.recurrent_cell = self.recurrent_cell(
+            input_size=n_features_U + n_features_Y,
+            hidden_size=n_state_neurons,
+            **kwargs_recurrent_cell,
+        )
 
         self.n_features_Y = n_features_Y
+        self.n_features_U = n_features_U
 
     def forward(
-        self, state: torch.Tensor, U: torch.Tensor = None, Y: torch.Tensor = None
+        self,
+        state: Union[torch.Tensor, Tuple[torch.Tensor]],
+        U: Optional[torch.Tensor] = None,
+        Y: Optional[torch.Tensor] = None,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """
-        Forward pass of the ECNN cell.
+        Calculates one time step with the inputs and returns the prediction and the state
+        of the next time step.
 
         Parameters
         ----------
+        state : torch.Tensor
+            The hidden state of the ECNN at time t-1.
+            state should have shape=(batchsize, n_state_neurons).
         U : torch.Tensor
-            The input for the ECNN at time t.
+            The input for the ECNN at time t (if known).
             U should have shape=(batchsize, n_features_U).
         Y : torch.Tensor
             The output of the ECNN at time t-1.
-            Y should have shape=(batchsize, 1).
-            The Y of the last time step is used to calculate
+            Y should have shape=(batchsize, n_features_Y).
+            The Y of the last time step (if known) is used to calculate
             the error for the error-correction.
-        state : torch.Tensor
-            The hidden state of the ECNN at time t-1.
-            state should have shape=(batchsize, n_state_neurons).
 
         Returns
         -------
         tuple
-            Contains output, which is the error at time t-1 and has the same
-            dimensions as Y, and state, which is the hidden state at time t.
+            Contains output, which is the error or the forecast at time t-1
+            and has the same dimensions as Y,
+            and state, which is the hidden state at time t.
         """
+        if isinstance(state, Tuple):
+            expectation = self.C(state[0])
+        else:
+            expectation = self.C(state)
 
-        expectation = self.C(state)
+        device = expectation.device
+        batchsize = expectation.shape[0]
 
-        self.LSTM_regulator_matrix = torch.diag_embed(
-            torch.reshape(self.LSTM_regulator.weight, (-1,))
-        )
-        if U is not None:
-            if Y is not None:
-                output = expectation - Y
-                state = (
-                    state
-                    + (self.act(self.A(state) + self.B(U) + self.D(output)) - state)
-                    @ self.LSTM_regulator_matrix
-                )
-            else:
-                output = expectation
-                state = (
-                    state
-                    + (self.act(self.A(state) + self.B(U)) - state)
-                    @ self.LSTM_regulator_matrix
-                )
+        if Y is not None:
+            output = expectation - Y
+            error_correction = output
         else:
-            if Y is not None:
-                output = expectation - Y
-                state = (
-                    state
-                    + (self.act(self.A(state) + self.D(output)) - state)
-                    @ self.LSTM_regulator_matrix
-                )
-            else:
-                output = expectation
-                state = (
-                    state
-                    + (self.act(self.A(state)) - state) @ self.LSTM_regulator_matrix
-                )
-
-        return (output, state)
+            output = expectation
+            error_correction = torch.zeros(
+                (batchsize, self.n_features_Y), device=device
+            )
+
+        if U is None:
+            U = torch.zeros((batchsize, self.n_features_U), device=device)
+
+        input = torch.cat((U, error_correction), dim=-1)
+        state = self.recurrent_cell(input, state)
+        return output, state
+
+    def get_batchsize(self, state):
+        if isinstance(state, Tuple):
+            return state[0].shape[0]
+        else:
+            return state.shape[0]
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_model.py` & `prosper_nn-0.3.0/prosper_nn/models/ecnn/ecnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-""""""
 """
 Prosper_nn provides implementations for specialized time series forecasting
 neural networks and related utility functions.
 
 Copyright (C) 2022 Nico Beck, Julia Schemm, Henning Frechen, Jacob Fidorra,
     Denni Schmidt, Sai Kiran Srivatsav Gollapalli
 
@@ -20,16 +19,15 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch
 import torch.nn as nn
-from . import ecnn_cell, ecnn_lstm_cell
-from typing import Tuple, Type
+from . import ecnn_cell
 
 
 class ECNN(torch.nn.Module):
 
     """
     The ECNN class creates a Error Correction Neural Network.
 
@@ -65,19 +63,18 @@
 
     def __init__(
         self,
         n_features_U: int,
         n_state_neurons: int,
         past_horizon: int,
         forecast_horizon: int = 1,
-        lstm: bool = False,
+        recurrent_cell_type: str = "elman",
+        kwargs_recurrent_cell: dict = {},
         approach: str = "backward",
-        init_state: torch.Tensor = None,
         learn_init_state: bool = True,
-        activation: Type[torch.autograd.Function] = torch.tanh,
         n_features_Y: int = 1,
         future_U: bool = False,
     ) -> None:
         """
         Parameters
         ----------
         n_features_U: int
@@ -87,30 +84,26 @@
             The number of neurons of the hidden layer, i.e. the hidden state
             at each time step.
         past_horizon: int
             The length of the sequence of inputs and outputs used for
             prediction.
         forecast_horizon: int
             The forecast horizon.
-        lstm: boolean
-           Include long short-term memory or not. Use either ecnn_cell or ecnn_lstm_cell.
+        recurrent_cell_type: str
+            Possible choices: elman, lstm, gru or gru_3_variant.
+        kwargs_recurrent_cell: dict
+            Parameters for the recurrent cell. Activation function can be set here.
         approach: string
             Either "backward" or "forward".
             A backward approach means that the external features at time t
             have a direct impact on the hidden state at time t.
             A forward approach means that the external features at time t
             only have a direct impact on the hidden state at time t+1.
-        init_state: torch.Tensor
-            The initial hidden state. If none is given, it is generated
-            randomly.
         learn_init_state: boolean
             Learn the initial hidden state or not.
-        activation : nn.functional
-            The activation function that is applied on the output of the hidden layers.
-            The same function is used on all hidden layers.
         n_features_Y: int
             The number of outputs, i.e. the number of elements of Y at each time
             step. The default is 1.
         future_U: boolean
             If false, U is assumed to be only known in the past and thus have
             the length past_horizon.
             If true, U is assumed to be also known in the future, e.g. weekdays,
@@ -124,37 +117,46 @@
         super(ECNN, self).__init__()
 
         self.n_features_U = n_features_U
         self.n_features_Y = n_features_Y
         self.n_state_neurons = n_state_neurons
         self.past_horizon = past_horizon
         self.forecast_horizon = forecast_horizon
-        self.lstm = lstm
         self.approach = approach
         self.future_U = future_U
+        self.learn_init_state = learn_init_state
+        self.recurrent_cell_type = recurrent_cell_type
 
         self._check_variables()
 
-        self.state = [torch.tensor] * (past_horizon + forecast_horizon + 1)
+        if recurrent_cell_type == 'lstm':
+            self.state = ([(torch.tensor, torch.tensor)] * (past_horizon + forecast_horizon + 1))
+        else:
+            self.state = [torch.tensor] * (past_horizon + forecast_horizon + 1)
+
+        self.ECNNCell = ecnn_cell.ECNNCell(
+                n_features_U, n_state_neurons, n_features_Y, recurrent_cell_type, kwargs_recurrent_cell
+            )
 
-        # Choose ECNN cell
-        if lstm:
-            self.ecnn_cell = ecnn_lstm_cell.ECNN_LSTM_Cell
+        self.init_state = self.set_init_state()
+
+
+    def set_init_state(self):
+        if self.recurrent_cell_type == 'lstm':
+            init_state = (nn.Parameter(
+                torch.rand(1, self.n_state_neurons), requires_grad=self.learn_init_state
+            ), nn.Parameter(
+                torch.rand(1, self.n_state_neurons), requires_grad=self.learn_init_state
+            ))
         else:
-            self.ecnn_cell = ecnn_cell.ECNNCell
-        # Init ECNN cell
-        self.ecnn_cell = self.ecnn_cell(
-            n_features_U, n_state_neurons, activation, n_features_Y
-        )
+            init_state = nn.Parameter(
+                torch.rand(1, self.n_state_neurons), requires_grad=self.learn_init_state
+            )
+        return init_state
 
-        self.init_state = nn.Parameter(
-            torch.rand(1, n_state_neurons), requires_grad=learn_init_state
-        )
-        if init_state is not None:
-            self.init_state.data = init_state
 
     def forward(self, U: torch.Tensor, Y: torch.Tensor) -> torch.Tensor:
         """
         Parameters
         ----------
         U: torch.Tensor
             A batch of input features sequences for the ECNN.
@@ -170,90 +172,93 @@
         torch.Tensor
             Contains past_error, the forecasting errors along the past_horizon
             where Y is known, and forecast, the forecast along the
             forecast_horizon. Both can be used for backpropagation.
             shape=(past_horizon+forecast_horizon, batchsize, n_features_Y)
         """
 
-        # LSTM: Keep entries of diagonal matrix between 0 and 1.
-        if self.lstm:
-            diag_entries = torch.clamp(self.ecnn_cell.D.weight.data, 0, 1)
-            self.ecnn_cell.D.weight.data = torch.nn.Parameter(diag_entries)
+        device = self.init_state.device
 
         # Check sizes of input and output
         self.check_sizes(U, Y)
         batchsize = U.shape[1]
 
-        past_error = torch.empty(size=(self.past_horizon, batchsize, self.n_features_Y))
+        past_error = torch.empty(
+            size=(self.past_horizon, batchsize, self.n_features_Y), device=device
+        )
         forecast = torch.empty(
-            size=(self.forecast_horizon, batchsize, self.n_features_Y)
+            size=(self.forecast_horizon, batchsize, self.n_features_Y), device=device
         )
 
         approach = self.approach
 
         if approach == "backward":
             # start
-            _, self.state[0] = self.ecnn_cell(
-                self.init_state.repeat(batchsize, 1), U[0]
-            )
+            _, self.state[0] = self.ECNNCell(self.repeat_init_state(batchsize), U[0])
             # past
             for t in range(1, self.past_horizon):
-                past_error[t - 1], self.state[t] = self.ecnn_cell(
+                past_error[t - 1], self.state[t] = self.ECNNCell(
                     self.state[t - 1], U[t], Y[t - 1]
                 )
             if self.future_U:
-                past_error[t], self.state[t + 1] = self.ecnn_cell(
+                past_error[t], self.state[t + 1] = self.ECNNCell(
                     self.state[t], U=U[t + 1], Y=Y[t]
                 )
                 # future
                 for t in range(
                     self.past_horizon + 1, self.past_horizon + self.forecast_horizon
                 ):
-                    forecast[t - self.past_horizon - 1], self.state[t] = self.ecnn_cell(
+                    forecast[t - self.past_horizon - 1], self.state[t] = self.ECNNCell(
                         self.state[t - 1], U=U[t]
                     )
-                forecast[t - self.past_horizon], self.state[t + 1] = self.ecnn_cell(
+                forecast[t - self.past_horizon], self.state[t + 1] = self.ECNNCell(
                     self.state[t]
                 )
             else:
-                past_error[t], self.state[t + 1] = self.ecnn_cell(self.state[t], Y=Y[t])
+                past_error[t], self.state[t + 1] = self.ECNNCell(self.state[t], Y=Y[t])
                 # future
                 for t in range(
                     self.past_horizon + 1, self.past_horizon + self.forecast_horizon + 1
                 ):
-                    forecast[t - self.past_horizon - 1], self.state[t] = self.ecnn_cell(
+                    forecast[t - self.past_horizon - 1], self.state[t] = self.ECNNCell(
                         self.state[t - 1]
                     )
 
         if approach == "forward":
             # start
-            self.state[0] = self.init_state.repeat(batchsize, 1)
+            self.state[0] = self.self.repeat_init_state(batchsize)
             # past
             for t in range(1, self.past_horizon + 1):
-                past_error[t - 1], self.state[t] = self.ecnn_cell(
+                past_error[t - 1], self.state[t] = self.ECNNCell(
                     self.state[t - 1], U[t - 1], Y[t - 1]
                 )
             # future
             if self.future_U:
                 for t in range(
                     self.past_horizon + 1, self.past_horizon + self.forecast_horizon + 1
                 ):
-                    forecast[t - self.past_horizon - 1], self.state[t] = self.ecnn_cell(
+                    forecast[t - self.past_horizon - 1], self.state[t] = self.ECNNCell(
                         self.state[t - 1], U=U[t - 1]
                     )
             else:
                 for t in range(
                     self.past_horizon + 1, self.past_horizon + self.forecast_horizon + 1
                 ):
-                    forecast[t - self.past_horizon - 1], self.state[t] = self.ecnn_cell(
+                    forecast[t - self.past_horizon - 1], self.state[t] = self.ECNNCell(
                         self.state[t - 1]
                     )
 
         return torch.cat((past_error, forecast), dim=0)
 
+    def repeat_init_state(self, batchsize):
+        if self.recurrent_cell_type == 'lstm':
+            return self.init_state[0].repeat(batchsize, 1), self.init_state[1].repeat(batchsize, 1)
+        else:
+            return self.init_state.repeat(batchsize, 1)
+
     def check_sizes(self, U: torch.Tensor, Y: torch.Tensor) -> None:
         """Checks if U and Y have right shape."""
 
         if self.future_U:
             if (
                 U.size()[0] != self.past_horizon + self.forecast_horizon
                 or U.size()[2] != self.n_features_U
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/ensemble/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/ensemble/ensemble.py` & `prosper_nn-0.3.0/prosper_nn/models/ensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/feedforward/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/feedforward/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/feedforward/feedforward.py` & `prosper_nn-0.3.0/prosper_nn/models/feedforward/feedforward.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/Data_Intake.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/Data_Intake.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/defuzzification.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/defuzzification.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/frnn.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/frnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,25 +98,26 @@
         # each input
         self.rnn = nn.RNN(
             input_size=n_features_input,
             hidden_size=n_features_input,
             num_layers=n_layers,
             batch_first=batch_first,
         )
-        prune_identity = torch.eye(n_features_input)
+        prune_identity = nn.Parameter(torch.eye(n_features_input))
         # Restrict RNN weights so the hidden state and the output resemble the time dependency of
         # the input sequence
         # weights are restricted to a diagonal matrix
         prune.custom_from_mask(self.rnn, "weight_ih_l0", prune_identity)
         prune.custom_from_mask(self.rnn, "weight_hh_l0", prune_identity)
 
         # Fuzzy layer
         self.fuzzy = nn.Sequential(
             Fuzzification(
-                n_features_input=self.n_features_input, membership_fcts=self.membership_fcts
+                n_features_input=self.n_features_input,
+                membership_fcts=self.membership_fcts,
             ),
             FuzzyInference(
                 n_features_input=self.n_features_input,
                 n_membership_fctship_fcts=self.n_membership_fcts,
                 n_rules=self.n_rules,
                 n_output_classes=n_output_classes,
                 rule_matrix=self.rule_matrix,
@@ -139,36 +140,36 @@
         Returns
         -------
         output : torch.Tensor
             Output tensor
         """
         batchsize = inputs.size(0)
         # Initializing hidden_state state for first input using method defined below
-        hidden_state = self.init_hidden(batchsize)
+        hidden_state = self.init_hidden(batchsize, self.rnn.device)
 
         # Passing in the input and hidden_state state into the model and obtaining outputs
         output, hidden_state = self.rnn(inputs, hidden_state)
         # get only output after the last time step
         output = output[:, -1]
         # pass through the fuzzy architecture
         output = self.fuzzy(output)
         return output
 
-    def init_hidden(self, batchsize: int) -> torch.Tensor:
+    def init_hidden(self, batchsize: int, device='cpu') -> torch.Tensor:
         """
         This method generates the first hidden_state state of zeros which is used in the forward pass.
 
         Parameters
         ----------
         batchsize : int
             number of Samples in one batch
 
         Returns
         -------
         hidden_state : torch.Tensor
             newly initialized hidden_state state
 
         """
-        hidden_state = torch.zeros(
-            self.n_layers, batchsize, self.n_features_input
+        hidden_state = torch.zeros((
+            self.n_layers, batchsize, self.n_features_input), device=device
         ).type(torch.DoubleTensor)
         return hidden_state
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzification.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/fuzzification.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzy_inference.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/fuzzy_inference.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_block.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/membership_block.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_functions.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/membership_functions.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/fuzzy/rule_manager.py` & `prosper_nn-0.3.0/prosper_nn/models/fuzzy/rule_manager.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn/hcnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch.nn as nn
 import torch
 from typing import Optional, Type
-from . import hcnn_cell, hcnn_lstm_cell
+from . import hcnn_cell, hcnn_gru_cell
 
 
 class HCNN(nn.Module):
     """
     The HCNN class creates a Historical Consistent Neural Network.
 
     A Historical Consistent Neural Network belongs to the class of Recurrent Neural Networks.
@@ -43,15 +43,15 @@
         self,
         n_state_neurons: int,
         n_features_Y: int,
         past_horizon: int,
         forecast_horizon: int,
         sparsity: float = 0.0,
         activation: Type[torch.autograd.Function] = torch.tanh,
-        lstm: bool = False,
+        cell_type: str = "hcnn_cell",
         init_state: Optional[torch.Tensor] = None,
         learn_init_state: bool = True,
         teacher_forcing: float = 1,
         decrease_teacher_forcing: float = 0,
         backward_full_Y: bool = True,
         ptf_in_backward: bool = True,
     ):
@@ -77,16 +77,17 @@
             These weights are not trainable and therefore always zero.
             For big matrices (dimension > 50) this can be necessary to guarantee
             numerical stability and it increases the long-term memory of the model.
         activation : Type[torch.autograd.Function]
             The activation function that is applied on the output of the hidden layers.
             The same function is used on all hidden layers.
             No function is applied if no function is given.
-        lstm: boolean
-           Include long short-term memory or not.
+        cell_type: str
+            Include a version of the gated recurrent unit.
+            Possible choices: hcnn_cell or hcnn_gru_3_variant.
         init_state : torch.Tensor
             The initial state of the HCNN model.
             Can be given optionally and is chosen randomly if not specified.
         learn_init_state: boolean
             Learn the initial hidden state or not.
         teacher_forcing: float
             The probability that teacher forcing is applied for a single state neuron.
@@ -103,35 +104,36 @@
         super(HCNN, self).__init__()
         self.n_state_neurons = n_state_neurons
         self.n_features_Y = n_features_Y
         self.past_horizon = past_horizon
         self.forecast_horizon = forecast_horizon
         self.sparsity = sparsity
         self.activation = activation
-        self.lstm = lstm
+        self.cell_type = cell_type
         self.teacher_forcing = teacher_forcing
         self.decrease_teacher_forcing = decrease_teacher_forcing
         self.backward_full_Y = backward_full_Y
         self.ptf_in_backward = ptf_in_backward
         self.state = [torch.tensor for _ in range(past_horizon + forecast_horizon + 1)]
 
         self._check_variables()
 
         self.init_state = nn.Parameter(
             torch.randn(1, n_state_neurons), requires_grad=learn_init_state
         )
         if init_state is not None:
             self.init_state.data = init_state
 
-        # choose HCNNCell
-        if lstm:
-            self.HCNNCell = hcnn_lstm_cell.HCNN_LSTM_Cell
-        else:
+        if cell_type == "hcnn_cell":
             self.HCNNCell = hcnn_cell.HCNNCell
-        # init HCNNCELL
+        elif cell_type == "hcnn_gru_3_variant":
+            self.HCNNCell = hcnn_gru_cell.HCNN_GRU_3_variant
+        else:
+            raise ValueError("Cell type is not found")
+
         self.HCNNCell = self.HCNNCell(
             self.n_state_neurons,
             self.n_features_Y,
             self.sparsity,
             self.activation,
             self.teacher_forcing,
             self.backward_full_Y,
@@ -151,28 +153,22 @@
         -------
         torch.Tensor
             Contains past_error, the forecasting errors along the past_horizon
             where Y is known, and forecast, the forecast along the
             forecast_horizon. Both can be used for backpropagation.
             shape=(past_horizon+forecast_horizon, batchsize, n_features_Y)
         """
-
+        device = self.init_state.device
         self.state[0] = self.init_state
-
-        # LSTM: Keep entries of diagonal matrix between 0 and 1.
-        if self.lstm:
-            diag_entries = torch.clamp(self.HCNNCell.LSTM_regulator.weight.data, 0, 1)
-            self.HCNNCell.LSTM_regulator.weight.data = torch.nn.Parameter(diag_entries)
-
         self._check_sizes(Y)
         batchsize = Y.shape[1]
 
         # reset saved cell outputs
-        past_error = torch.zeros(self.past_horizon, batchsize, self.n_features_Y)
-        forecast = torch.zeros(self.forecast_horizon, batchsize, self.n_features_Y)
+        past_error = torch.zeros((self.past_horizon, batchsize, self.n_features_Y), device=device)
+        forecast = torch.zeros((self.forecast_horizon, batchsize, self.n_features_Y), device=device)
 
         # past
         for t in range(self.past_horizon):
             if t == 0:
                 self.state[t + 1], past_error[t] = self.HCNNCell(
                     self.state[t].repeat(batchsize, 1), Y[t]
                 )
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_cell.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn/hcnn_cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 
 class PartialTeacherForcing(nn.Dropout):
     """
     Applies Dropout as partial teacher forcing. Therefore, scaling of the Dropout is reverted,
     so that the partial teacher forcing sets the values to the original observation.
     """
+
     def forward(self, input: Tensor) -> Tensor:
         if not self.training or self.p == 0:
             return input
         else:
             scaled_output = super().forward(input)
             return (1 - self.p) * scaled_output
 
@@ -116,16 +117,16 @@
             self.activation = torch.tanh
 
         self.A = nn.Linear(
             in_features=self.n_state_neurons,
             out_features=self.n_state_neurons,
             bias=False,
         )
-        self.eye = torch.eye(
-            self.n_features_Y, self.n_state_neurons, requires_grad=False
+        self.eye = nn.Parameter(torch.eye(
+            self.n_features_Y, self.n_state_neurons), requires_grad=False
         )
         self.ptf_dropout = PartialTeacherForcing(1 - self.teacher_forcing)
         if self.sparsity > 0:
             prune.random_unstructured(self.A, name="weight", amount=self.sparsity)
         if not self.ptf_in_backward:
             self.ptf_dropout.register_full_backward_hook(no_dropout_backward)
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_lstm_cell.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn/hcnn_gru_cell.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,28 +25,34 @@
 import torch.nn as nn
 import torch
 import torch.nn.utils.prune as prune
 from typing import Optional, Type
 from .hcnn_cell import no_dropout_backward, PartialTeacherForcing
 
 
-class HCNN_LSTM_Cell(nn.Module):
+class HCNN_GRU_3_variant(nn.Module):
     """
-    The HCNN_LSTM_Cell call is implemented to model one forecast step in a HCNN
-    with a simple version of Long-Short-Term Memory.
+    The HCNN_GRU_3_variant call is implemented to model one forecast step in a HCNN
+    with a version similar to the GRU 3 variant in the following paper.
+    One difference is that $$r_t$$ is fixed to a vector with ones in our implementation.
+
+    R. Dey and F. M. Salem, "Gate-variants of Gated Recurrent Unit (GRU) neural networks,"
+    2017 IEEE 60th International Midwest Symposium on Circuits and Systems (MWSCAS),
+    Boston, MA, USA, 2017, pp. 1597-1600, doi: 10.1109/MWSCAS.2017.8053243
+
     By recursively using the cell a HCNN network can be implemented.
     Mathematically the the output of one cell is calculated as following, where
     :math:`s_t^{\\prime}` serves as an interim result:
 
     .. math ::
         s_{t}^\\prime = \\tanh \\left( s_t -[\\mathbb{1}, 0]^T \\cdot ( [\\mathbb{1}, 0] s_t -y_t^d) \\right)
     .. math ::
-        s_{t+1} = (1-D) s_{t}^\\prime + DA \\tanh (s_{t}^\\prime) = s_{t}^\\prime + D(A \\tanh(s_{t}^\\prime)-s_{t}^\\prime)
+        s_{t+1} = (1 - \\sigma(update\_vector)) \\circ s_{t}^\\prime + \\sigma(update\_vector) \circ A \\tanh (s_{t}^\\prime)
     .. math ::
-        y_t = [\\mathbb{1}, 0] \\cdot s_t
+        \\hat{y}_t = [\\mathbb{1}, 0] \\cdot s_t
     """
 
     def __init__(
         self,
         n_state_neurons: int,
         n_features_Y: int,
         sparsity: float = 0.0,
@@ -87,15 +93,15 @@
             If True nothing happens and the Dropout layer is handled as it is in the backward path.
             If False the Dropout layer is skipped in the backward path.
 
         Returns
         -------
         None
         """
-        super(HCNN_LSTM_Cell, self).__init__()
+        super(HCNN_GRU_3_variant, self).__init__()
         self.n_state_neurons = n_state_neurons
         self.n_features_Y = n_features_Y
         self.sparsity = sparsity
         self.activation = activation
         self.teacher_forcing = teacher_forcing
         self.backward_full_Y = backward_full_Y
         self.ptf_in_backward = ptf_in_backward
@@ -104,20 +110,25 @@
             self.activation = torch.tanh
 
         self.A = nn.Linear(
             in_features=self.n_state_neurons,
             out_features=self.n_state_neurons,
             bias=False,
         )
-        self.eye = torch.eye(
-            self.n_features_Y, self.n_state_neurons, requires_grad=False
+        self.eye = nn.Parameter(torch.eye(
+            self.n_features_Y, self.n_state_neurons), requires_grad=False
         )
         self.ptf_dropout = PartialTeacherForcing(1 - self.teacher_forcing)
-        self.LSTM_regulator = nn.Linear(1, n_state_neurons, bias=False)
-        nn.init.ones_(self.LSTM_regulator.weight)
+
+        self.update_vector = nn.Parameter(
+            torch.zeros(n_state_neurons), requires_grad=True
+        )
+        self.ones = nn.Parameter(
+            torch.ones_like(self.update_vector), requires_grad=False
+        )
 
         if self.sparsity > 0:
             prune.random_unstructured(self.A, name="weight", amount=self.sparsity)
         if not self.ptf_in_backward:
             self.ptf_dropout.register_full_backward_hook(no_dropout_backward)
 
     def forward(self, state: torch.Tensor, observation: Optional[torch.Tensor] = None):
@@ -141,34 +152,33 @@
             The updated state of the HCNN.
         output : torch.Tensor
             The output of the HCNN Cell. If an observation is given,
             this output is calculated by the expectation minus the observation.
             If no observation is given, the output is equal to the expectation.
         """
 
-        # Embed LSTM_regulator weights in matrix
-        self.LSTM_regulator_matrix = torch.diag_embed(
-            torch.reshape(self.LSTM_regulator.weight, (-1,))
-        )
         # Cell forward calculations
         expectation = torch.mm(state, self.eye.T)
         if observation is not None:
             if self.backward_full_Y:
                 output = expectation - observation
                 teacher_forcing = torch.mm(self.ptf_dropout(output), self.eye)
             elif not self.backward_full_Y:
                 output = self.ptf_dropout(expectation - observation)
                 teacher_forcing = torch.mm(output, self.eye)
             state = state - teacher_forcing
         else:  # Forecasts
             output = expectation
-        state = (
-            state
-            + (self.A(self.activation(state)) - state) @ self.LSTM_regulator_matrix
-        )
+
+        candidate_activation = self.A(self.activation(state))
+
+        state = (self.ones - torch.sigmoid(self.update_vector)) * state + torch.sigmoid(
+            self.update_vector
+        ) * candidate_activation
+
         return state, output
 
     def set_teacher_forcing(self, teacher_forcing: float) -> None:
         """
         Function to set teacher forcing to a specific value in layer and as self variable.
 
         Parameters
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/__init__.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/hcnn_known_u.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch.nn as nn
 import torch
-from typing import List, Optional, Type
+from typing import Optional, Type
 from prosper_nn.models.hcnn_known_u import hcnn_known_u_cell
 
 
 class HCNN_KNOWN_U(nn.Module):
     # TODO: Include References of HCNN by Zimmermann?
     """
     The HCNN_KNOWN_U class creates a Historical Consistent Neural Network with known features
@@ -157,23 +157,23 @@
         -------
         torch.Tensor
             Contains past_error, the forecasting errors along the past_horizon
             where Y is known, and forecast, the forecast along the
             forecast_horizon. Both can be used for backpropagation.
             shape=(past_horizon+forecast_horizon, batchsize, n_features_Y)
         """
-
+        device = self.init_state.device
         self.state[0] = self.init_state
 
         self._check_sizes(U, Y)
         batchsize = Y.shape[1]
 
         # reset saved cell outputs
-        past_error = torch.zeros(self.past_horizon, batchsize, self.n_features_Y)
-        forecast = torch.zeros(self.forecast_horizon, batchsize, self.n_features_Y)
+        past_error = torch.zeros((self.past_horizon, batchsize, self.n_features_Y), device=device)
+        forecast = torch.zeros((self.forecast_horizon, batchsize, self.n_features_Y), device=device)
 
         # past
         for t in range(self.past_horizon):
             if t == 0:
                 self.state[t + 1], past_error[t] = self.HCNN_K_U_Cell(
                     self.state[t].repeat(batchsize, 1), U[t], Y[t]
                 )
```

### Comparing `prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py` & `prosper_nn-0.3.0/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,39 +103,39 @@
         self.backward_full_Y = backward_full_Y
         self.ptf_in_backward = ptf_in_backward
 
         if type(activation) == str and activation == "torch.tanh":
             self.activation = torch.tanh
 
         # from state to output, used in filtering the hidden neurons.
-        self.eye = torch.eye(
-            self.n_features_Y, self.n_state_neurons, requires_grad=False
+        self.eye = nn.Parameter(torch.eye(
+            self.n_features_Y, self.n_state_neurons), requires_grad=False
         )
 
         # from error with padding for hidden neurons and n_features_U to r state
-        self.eye_err2rstate = torch.eye(
+        self.eye_err2rstate = nn.Parameter(torch.eye(
             self.n_features_Y,
-            self.n_state_neurons + self.n_features_U,
+            self.n_state_neurons + self.n_features_U),
             requires_grad=False,
         )
 
         # from state with padding for n_features_U to r state
-        self.eye_state2rstate = torch.eye(
+        self.eye_state2rstate = nn.Parameter(torch.eye(
             self.n_state_neurons,
-            self.n_state_neurons + self.n_features_U,
+            self.n_state_neurons + self.n_features_U),
             requires_grad=False,
         )
 
         # from n_features_U with padding for n_state_neurons to r state.
         padding = torch.zeros(
             self.n_features_U,
             self.n_state_neurons,
         )
         eye_u = torch.eye(self.n_features_U)
-        self.eye_U2rstate = torch.cat((padding, eye_u), axis=1)
+        self.eye_U2rstate = nn.Parameter(torch.cat((padding, eye_u), axis=1), requires_grad=False)
 
         # from r state to state[t+1]
         self.A = nn.Linear(
             in_features=self.n_state_neurons + self.n_features_U,
             out_features=self.n_state_neurons,
             bias=False,
         )
```

### Comparing `prosper_nn-0.2.3/prosper_nn/utils/create_input_ecnn_hcnn.py` & `prosper_nn-0.3.0/prosper_nn/utils/create_input_ecnn_hcnn.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/utils/generate_time_series_data.py` & `prosper_nn-0.3.0/prosper_nn/utils/generate_time_series_data.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/utils/neuron_correlation_hidden_layers.py` & `prosper_nn-0.3.0/prosper_nn/utils/neuron_correlation_hidden_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,18 @@
 
     abs_max_corr = abs_max_corr.tolist()
     abs_max_corr = round(abs_max_corr, 2)
 
     print_most_corr = "The most correlated neurons are the ones with indices "
     if ind_neurons_neg.nelement() == 0:
         if print_values:
-            print(print_most_corr, ind_neurons.squeeze().tolist(),)
+            print(
+                print_most_corr,
+                ind_neurons.squeeze().tolist(),
+            )
             print("The according Pearson correlation coefficient is", abs_max_corr)
         return (abs_max_corr, ind_neurons)
     elif ind_neurons_pos.nelement() == 0:
         if print_values:
             print(
                 print_most_corr,
                 ind_neurons.squeeze().tolist(),
```

### Comparing `prosper_nn-0.2.3/prosper_nn/utils/sensitivity_analysis.py` & `prosper_nn-0.3.0/prosper_nn/utils/sensitivity_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from typing import Optional, List, Tuple, Union
 
 
 def calculate_sensitivity_analysis(
     model: torch.nn.Module,
     *data: Tuple[torch.Tensor, ...],
     output_neuron: tuple = (0,),
-    batchsize: int = 1
+    batchsize: int = 1,
 ) -> torch.tensor:
     """
     Calculates the sensitivity matrix.
     The function differentiates the target node with respect to the
     input for all observation.
 
     Parameters
@@ -211,14 +211,17 @@
     title : list[str], optional
         Set a title for the plot.
 
     Returns
     -------
     None
     """
+
+    if features is None:
+        features = [f"feature_{i}" for i in range(n_features)]
     if type(data) is torch.Tensor:
         data = (data,)
     # Calculations
     heat = torch.empty((n_task_nodes, n_future_steps, n_features))
     for node in range(0, n_task_nodes):
         for i, time in enumerate(
             range(past_horizon + 1, past_horizon + 1 + n_future_steps)
```

### Comparing `prosper_nn-0.2.3/prosper_nn/utils/visualization.py` & `prosper_nn-0.3.0/prosper_nn/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn/utils/visualize_forecasts.py` & `prosper_nn-0.3.0/prosper_nn/utils/visualize_forecasts.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.3/prosper_nn.egg-info/PKG-INFO` & `prosper_nn-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
-Name: prosper-nn
-Version: 0.2.3
+Name: prosper_nn
+Version: 0.3.0
 Summary: Package contains, in PyTorch implemented, neural networks with problem specific pre-structuring architectures and utils that help building and understanding models.
 Home-page: UNKNOWN
 Author: Nico Beck, Julia Schemm
 Author-email: nico.beck@iis.fraunhofer.de
 License: UNKNOWN
+Description: # Prosper_NN
+        
+        ## Problem-Specific Pre-Structuring of Neural Networks
+        
+        Accurate data-driven forecasts can provide a crucial advantage in many application areas. One of the methods with the most promising results in forecasting time series are neural networks. However, especially in macro-economic applications, it can be difficult and time-consuming to adapt state-of-the-art neural network architectures in a way that leads to satisfying results. For instance, the final prices of materials and stocks result from a highly complex interplay between supply and demand. Additionally, there is often only one (albeit long) historical time series available for training which makes correlations in the data difficult to detect.
+        
+        Under these circumstances, applying state-of-the-art neural networks architectures successfully poses a great challenge. Pre-structuring the models can solve this problem. For this purpose, Zimmermann, Tietz and Grothmann (Neural Networks: Tricks of the Trade, 2012) propose recurrent architectures for various time series problems that help recognize correlations. They recommend Error-Correction Neural Networks (ECNNs), Historical-Consistent Neural Networks (HCNNs) and Causal-Retro-Causal Neural Networks (CRCNNs). One of the main ideas of the pre-structuring is embedding the model in a larger architecture in order to use the past prediction errors for predicting the next time step. The three approaches mentioned use this idea and apply it in different settings. So far, the proposed architectures are not publicly available in common machine learning frameworks. Therefore, we have implemented the models in PyTorch. This way, we can easily test them on diverse datasets.
+        In this package the neural network architectures developed by Hans-Georg Zimmermann are implemented in PyTorch.
+        The full documentation can be found here https://iis-scs-a.pages.fraunhofer.de/prosper/prosper/. There are also tutorials that show how to work with the package.
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Prosper_NN
-
-## Problem-Specific Pre-Structuring of Neural Networks
-
-Accurate data-driven forecasts can provide a crucial advantage in many application areas. One of the methods with the most promising results in forecasting time series are neural networks. However, especially in macro-economic applications, it can be difficult and time-consuming to adapt state-of-the-art neural network architectures in a way that leads to satisfying results. For instance, the final prices of materials and stocks result from a highly complex interplay between supply and demand. Additionally, there is often only one (albeit long) historical time series available for training which makes correlations in the data difficult to detect.
-
-Under these circumstances, applying state-of-the-art neural networks architectures successfully poses a great challenge. Pre-structuring the models can solve this problem. For this purpose, Zimmermann, Tietz and Grothmann (Neural Networks: Tricks of the Trade, 2012) propose recurrent architectures for various time series problems that help recognize correlations. They recommend Error-Correction Neural Networks (ECNNs), Historical-Consistent Neural Networks (HCNNs) and Causal-Retro-Causal Neural Networks (CRCNNs). One of the main ideas of the pre-structuring is embedding the model in a larger architecture in order to use the past prediction errors for predicting the next time step. The three approaches mentioned use this idea and apply it in different settings. So far, the proposed architectures are not publicly available in common machine learning frameworks. Therefore, we have implemented the models in PyTorch. This way, we can easily test them on diverse datasets.
-In this package the neural network architectures developed by Hans-Georg Zimmermann are implemented in PyTorch.
-The full documentation can be found here https://iis-scs-a.pages.fraunhofer.de/prosper/prosper/. There are also tutorials that show how to work with the package.
-
```

### Comparing `prosper_nn-0.2.3/prosper_nn.egg-info/SOURCES.txt` & `prosper_nn-0.3.0/prosper_nn.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 prosper_nn/models/crcnn/__init__.py
 prosper_nn/models/crcnn/crcnn.py
 prosper_nn/models/deep_feed_forward/__init__.py
 prosper_nn/models/deep_feed_forward/deep_feed_forward.py
 prosper_nn/models/dhcnn/__init__.py
 prosper_nn/models/dhcnn/dhcnn.py
 prosper_nn/models/ecnn/__init__.py
+prosper_nn/models/ecnn/ecnn.py
 prosper_nn/models/ecnn/ecnn_cell.py
-prosper_nn/models/ecnn/ecnn_lstm_cell.py
-prosper_nn/models/ecnn/ecnn_model.py
+prosper_nn/models/ecnn/gru_cell_variant.py
 prosper_nn/models/ensemble/__init__.py
 prosper_nn/models/ensemble/ensemble.py
 prosper_nn/models/feedforward/__init__.py
 prosper_nn/models/feedforward/feedforward.py
 prosper_nn/models/fuzzy/Data_Intake.py
 prosper_nn/models/fuzzy/__init__.py
 prosper_nn/models/fuzzy/defuzzification.py
@@ -33,15 +33,18 @@
 prosper_nn/models/fuzzy/fuzzy_inference.py
 prosper_nn/models/fuzzy/membership_block.py
 prosper_nn/models/fuzzy/membership_functions.py
 prosper_nn/models/fuzzy/rule_manager.py
 prosper_nn/models/hcnn/__init__.py
 prosper_nn/models/hcnn/hcnn.py
 prosper_nn/models/hcnn/hcnn_cell.py
-prosper_nn/models/hcnn/hcnn_lstm_cell.py
+prosper_nn/models/hcnn/hcnn_gru_cell.py
+prosper_nn/models/hcnn_compressed/__init__.py
+prosper_nn/models/hcnn_compressed/hcnn_cell_compressed.py
+prosper_nn/models/hcnn_compressed/hcnn_compressed.py
 prosper_nn/models/hcnn_known_u/__init__.py
 prosper_nn/models/hcnn_known_u/hcnn_known_u.py
 prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py
 prosper_nn/utils/__init__.py
 prosper_nn/utils/create_input_ecnn_hcnn.py
 prosper_nn/utils/generate_time_series_data.py
 prosper_nn/utils/neuron_correlation_hidden_layers.py
```

### Comparing `prosper_nn-0.2.3/setup.py` & `prosper_nn-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("requirements.txt", "r", encoding="utf-8") as f:
     packages = f.read().split("\n")
     for pack in packages:
         requirements.append(pack)
 
 setuptools.setup(
     name="prosper_nn",  # Replace with your own username
-    version="0.2.3",
+    version="0.3.0",
     author="Nico Beck, Julia Schemm",
     author_email="nico.beck@iis.fraunhofer.de",
     description="Package contains, in PyTorch implemented, neural networks with problem specific pre-structuring architectures and utils that help building and understanding models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

