# Comparing `tmp/falcon_challenge-0.2.1.tar.gz` & `tmp/falcon_challenge-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.2.1.tar", last modified: Tue Mar 26 23:38:26 2024, max compression
+gzip compressed data, was "falcon_challenge-0.2.3.tar", last modified: Tue Apr  2 20:50:19 2024, max compression
```

## Comparing `falcon_challenge-0.2.1.tar` & `falcon_challenge-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:38:26.349853 falcon_challenge-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-26 23:38:26.349853 falcon_challenge-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:38:26.345853 falcon_challenge-0.2.1/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/ndt2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:38:26.349853 falcon_challenge-0.2.1/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:38:26.349853 falcon_challenge-0.2.1/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-26 23:38:26.000000 falcon_challenge-0.2.1/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-26 23:38:26.000000 falcon_challenge-0.2.1/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 23:38:26.000000 falcon_challenge-0.2.1/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-26 23:38:26.000000 falcon_challenge-0.2.1/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 23:38:26.000000 falcon_challenge-0.2.1/falcon_challenge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 23:38:26.349853 falcon_challenge-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-26 23:38:21.000000 falcon_challenge-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:19.715232 falcon_challenge-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-02 20:50:19.711232 falcon_challenge-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:19.711232 falcon_challenge-0.2.3/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/ndt2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:19.711232 falcon_challenge-0.2.3/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:19.711232 falcon_challenge-0.2.3/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-02 20:50:19.000000 falcon_challenge-0.2.3/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-02 20:50:19.000000 falcon_challenge-0.2.3/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:50:19.000000 falcon_challenge-0.2.3/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 20:50:19.000000 falcon_challenge-0.2.3/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 20:50:19.000000 falcon_challenge-0.2.3/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:19.711232 falcon_challenge-0.2.3/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:50:19.715232 falcon_challenge-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 20:50:15.000000 falcon_challenge-0.2.3/setup.py
```

### Comparing `falcon_challenge-0.2.1/LICENSE` & `falcon_challenge-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/README.md` & `falcon_challenge-0.2.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     - `minival` (Copy dandiset minival folder into this folder)
     - `eval` (Copy the ground truth held in and held out data into this folder)
 
 H1 should unfold correctly just from unzipping the provided directory. M1 should work by renaming the provided dandiset to `m1` and `minival` folder inside, and then copying the provided eval data into this folder. Each of the lowest level dirs holds the NWB files.
 
 ### Code
 This codebase contains starter code for implementing your own method for the FALCON challenge. 
-- The `falcon_challenge` folder contains the logic for the evaluator. Submitted solutions must confirm to the interface specified in `falcon_challenge.interface`.
+- The `falcon_challenge` folder contains the logic for the evaluator. Submitted solutions must conform to the interface specified in `falcon_challenge.interface`.
 - In `data_demos`, we provide notebooks that survey each dataset released as part of this challenge.
 - In `decoder_demos`, we provide sample decoders and baselines that are formatted to be ready for submission to the challenge. To use them, see the comments in the header of each file ending in `_sample.py`. Your solutions should look similar once implemented!
 
 For example, you can prepare and evaluate a linear decoder by running:
 ```bash
 python decoder_demos/sklearn_decoder.py --training_dir data/h1/held_in_calib/ --calibration_dir data/h1/held_out_calib/ --mode all --task h1
 python sklearn_sample.py --evaluation local --phase minival --split h1
@@ -51,12 +51,23 @@
 ```bash
 # Build
 sudo docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
 sudo docker run -v PATH_TO_YOUR_DATA_DIR:/dataset/evaluation_data -it sk_smoke
 ## If your solution needs GPUs, append a --gpus all flag to `docker run`
 ```
 
-## EvalAI Submission (under construction)
-To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the EvalAI submission tab. It should look something like:
+## EvalAI Submission
+Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands, or run `test_docker_local.sh --docker-name mysubmission`. This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
+
+To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). It should look something like:
 `
 evalai push decoder_container:latest --phase <phase-name>
 `
+
+### Troubleshooting
+Docker:
+- If this is your first time with docker, note that `sudo` access is needed, or your user needs to be in the `docker` group. `docker info` should run without error.
+- While `sudo` is sufficient for local development, the EvalAI submission step will ultimately require your user to be able to run `docker` commands without `sudo`.
+- To do this, [add yourself to the `docker` group](https://docs.docker.com/engine/install/linux-postinstall/). Note you may [need vigr](https://askubuntu.com/questions/964040/usermod-says-account-doesnt-exist-but-adduser-says-it-does) to add your own user.
+
+EvalAI:
+- `pip install evalai` may fail on python 3.11, see: https://github.com/aio-libs/aiohttp/issues/6600. We recommend creating a separate env for submission in this case.
```

### Comparing `falcon_challenge-0.2.1/decoder_demos/decoding_utils.py` & `falcon_challenge-0.2.3/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/decoder_demos/filtering.py` & `falcon_challenge-0.2.3/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/decoder_demos/ndt2_decoder.py` & `falcon_challenge-0.2.3/decoder_demos/ndt2_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 r"""
-    Load an sklearn decoder.
-    To train, for example:
-    `python decoder_demos/sklearn_decoder.py --training_dir data/h1/train --calibration_dir data/h1/test --mode all`
-    To evaluate, for example:
-    `python decode_submit.py --evaluation remote/local`
+    NDT2 wrapper. Not for running.
 """
 from typing import List
 from pathlib import Path
 import numpy as np
 import torch
 import pytorch_lightning as pl
 from einops import rearrange
 
 from hydra import compose, initialize_config_module
 
-from falcon_challenge.config import FalconConfig, FalconTask
+from falcon_challenge.config import FalconConfig
 from falcon_challenge.interface import BCIDecoder
 
 from context_general_bci.utils import suppress_default_registry
 suppress_default_registry()
 from context_general_bci.config import RootConfig, propagate_config, DataKey, MetaKey
 from context_general_bci.dataset import DataAttrs, ContextAttrs
 from context_general_bci.subjects import SubjectName
@@ -30,16 +26,14 @@
 def format_array_name(subject: str):
     return f'FALCON{subject}-M1'
 
 class NDT2Decoder(BCIDecoder):
     r"""
         Load an NDT2 decoder, prepared in:
         https://github.com/joel99/context_general_bci
-
-        # TODO KV cache - difficult without rotary embeddings
     """
 
     def __init__(
             self,
             task_config: FalconConfig,
             model_ckpt_path: str,
             model_cfg_stem: str,
@@ -79,37 +73,36 @@
         pl.seed_everything(seed=cfg.seed)
 
         self.subject = getattr(SubjectName, f'falcon_{task_config.task.name}')
         context_idx = {
             MetaKey.array.name: [format_array_name(self.subject)],
             MetaKey.subject.name: [self.subject],
             MetaKey.session.name: sorted([
-                self.format_dataset_tag(handle) for handle in task_config.dataset_handles
+                self._task_config.hash_dataset(handle) for handle in task_config.dataset_handles
             ]),
             MetaKey.task.name: [self.exp_task],
         }
         data_attrs = DataAttrs.from_config(cfg.dataset, context=ContextAttrs(**context_idx))
         cfg.model.task.decode_normalizer = zscore_path
         model = load_from_checkpoint(model_ckpt_path, cfg=cfg.model, data_attrs=data_attrs)
         model = transfer_model(model, cfg.model, data_attrs)
         self.model = model.to('cuda:0')
         self.model.eval()
 
         assert task_config.bin_size_ms == cfg.dataset.bin_size_ms, "Bin size mismatch, transform not implemented."
         self.observation_buffer = torch.zeros((cfg.dataset.max_length_ms // task_config.bin_size_ms, task_config.n_channels), dtype=torch.uint8, device='cuda:0')
 
-    def format_dataset_tag(self, dataset_stem: str):
-        return FalconContextInfo.get_id(self.subject, self.exp_task, FalconContextInfo.get_alias(self.exp_task, self.subject, dataset_stem))
-
     def reset(self, dataset: Path = ""):
         dataset_tag = dataset.stem
-        # dataset_tag =  self.get_file_tag(dataset) # e.g. stem including _set_N suffix
         self.set_steps = 0
         self.observation_buffer.zero_()
-        self.meta_key = torch.tensor([self.model.data_attrs.context.session.index(self.format_dataset_tag(dataset_tag))], device='cuda:0')
+        self.meta_key = torch.tensor([
+            self.model.data_attrs.context.session.index(
+                self._task_config.hash_dataset(dataset_tag)
+            )], device='cuda:0')
 
     def predict(self, neural_observations: np.ndarray):
         r"""
             neural_observations: array of shape (n_channels), binned spike counts
         """
         self.observe(neural_observations)
         decoder_in = rearrange(self.observation_buffer[-self.set_steps:], 't c -> 1 t c 1')
```

### Comparing `falcon_challenge-0.2.1/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.2.3/decoder_demos/ndt2_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 r"""
     Sample NDT2 decoder for the Falcon Challenge.
 
-    H1: https://wandb.ai/joelye9/context_general_bci/runs/rasu7u1w
+    H1: https://wandb.ai/joelye9/context_general_bci/runs/edf4h5ym
+    M1: https://wandb.ai/joelye9/context_general_bci/runs/93snpffp
 """
 
 import argparse
 
 from falcon_challenge.config import FalconConfig, FalconTask
 from falcon_challenge.evaluator import FalconEvaluator
 
@@ -16,15 +17,15 @@
     parser.add_argument(
         "--evaluation", type=str, required=True, choices=["local", "remote"]
     )
     parser.add_argument(
         "--model-path", type=str, default='./local_data/ndt2_h1_sample.pth'
     )
     parser.add_argument(
-        "--config-stem", type=str, default='falcon/h1/h1_scale_data',
+        "--config-stem", type=str, default='falcon/h1/h1',
         help="Name in context-general-bci codebase for config. \
             Currently, directly referencing e.g. a local yaml is not implemented unclear how to get Hydra to find it in search path."
     )
     parser.add_argument(
         "--zscore-path", type=str, default='./local_data/ndt2_zscore_h1.pt'
     )
     parser.add_argument(
```

### Comparing `falcon_challenge-0.2.1/decoder_demos/random_decoder.py` & `falcon_challenge-0.2.3/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.2.3/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.2.3/decoder_demos/sklearn_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 )
 from decoder_demos.decoding_utils import (
     TRAIN_TEST,
     generate_lagged_matrix,
     fit_and_eval_decoder,
 )
 
-HISTORY = 0
-
 def prepare_train_test(
         binned_spikes: np.ndarray,
         targets: np.ndarray,
         blacklist: Optional[np.ndarray]=None,
         history: int=0,
         ):
     signal = apply_exponential_filter(binned_spikes)
@@ -153,15 +151,15 @@
         train_y,
         test_x,
         test_y,
         x_mean,
         x_std,
         y_mean,
         y_std
-    ) = prepare_train_test(all_neural_data, all_covariates, ~all_eval_mask, history=HISTORY)
+    ) = prepare_train_test(all_neural_data, all_covariates, ~all_eval_mask, history=history)
     score, decoder = fit_and_eval_decoder(train_x, train_y, test_x, test_y)
     print(f"CV Fit score: {score:.2f}")
     (
         cal_neural_data,
         _,
         _,
         _,
@@ -197,27 +195,29 @@
         save_path
     )
 
 def fit_last_session(
     datafiles: List[Path],
     calibration_datafiles: List[Path],
     task_config: FalconConfig,
-    save_path: Path
+    save_path: Path,
+    history = 0,
 ):
     day_unique = set([f.stem.split('_')[0] for f in datafiles])
     last_day = sorted(day_unique)[-1]
     fit_datafiles = [d for d in datafiles if last_day in d.stem]
     return fit_sklearn_decoder(
         fit_datafiles,
         calibration_datafiles,
         task_config,
-        save_path
+        save_path,
+        history = history
     )
 
-def main(task, training_dir, calibration_dir, mode):
+def main(task, training_dir, calibration_dir, history, mode):
     # Your main function logic here
     if mode == 'all':
         fit_fn = fit_sklearn_decoder
     elif mode == 'last':
         fit_fn = fit_last_session
     else:
         raise ValueError(f"Unknown mode: {mode}")
@@ -225,21 +225,22 @@
     calibration_dir = Path(calibration_dir)
     task_config = FalconConfig(
         task=FalconTask.__dict__[task],
     )
     save_path = Path(f'local_data/sklearn_{task_config.task}.pkl')
     datafiles = list(training_dir.glob('*calib*.nwb'))
     calibration_datafiles = list(calibration_dir.glob('*calib*.nwb'))
-    fit_fn(datafiles, calibration_datafiles, task_config, save_path)
+    fit_fn(datafiles, calibration_datafiles, task_config, save_path, history=history)
     print(f"Saved to {save_path}")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='Train sklearn decoder')
 
     parser.add_argument('--task', type=str, choices=['h1', 'm1', 'm2'], help='Task for training')
     parser.add_argument('--training_dir', '-t', type=str, help='Root directory for training files')
     parser.add_argument('--calibration_dir', '-c', type=str, help='Root directory for calibration files')
     parser.add_argument('--mode', '-m', type=str, choices=['all', 'last'], help='Mode for training')
+    parser.add_argument('--history', type=int, default=0, help='History for decoder')
 
     args = parser.parse_args()
 
-    main(args.task, args.training_dir, args.calibration_dir, args.mode)
+    main(args.task, args.training_dir, args.calibration_dir, args.history, args.mode)
```

### Comparing `falcon_challenge-0.2.1/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.2.3/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/falcon_challenge/config.py` & `falcon_challenge-0.2.3/falcon_challenge/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     bin_size_ms: int = 20
     dataset_handles: list[str] = field(default_factory=lambda: []) # Compute with evaluator.get_eval_handles
 
     @property
     def n_channels(self):
         if self.task == FalconTask.h1:
             return 176
+        elif self.task == FalconTask.h2:
+            return 192
         elif self.task == FalconTask.m1:
             return 96
         elif self.task == FalconTask.m2:
             return 96
         raise NotImplementedError(f"Task {self.task} not implemented.")
 
     @property
@@ -43,30 +45,35 @@
             return 7
         elif self.task == FalconTask.h2:
             return 28
         elif self.task == FalconTask.m1:
             return 16
         elif self.task == FalconTask.m2:
             return 2
+        raise NotImplementedError(f"Task {self.task} not implemented.")
         
     def hash_dataset(self, handle: str):
         r"""
             handle - path.stem of a datafile.
             Convenience function to help identify what "session" a datafile belongs to.
         """
         if self.task == FalconTask.h1:
-            # dandi-like atm but not quite determined; e.g. S608_set_1_calib
+            handle = handle.replace('-', '_')
+            # dandi-like atm but not quite determined; e.g. S0_set_1_calib
+            # remove split and set information
             pieces = handle.split('_')
-            if pieces[-1] in ['minival', 'calib', 'calibration', 'eval', 'full']:
-                return '_'.join(pieces[:-1])
-            return handle
+            for piece in pieces:
+                if piece[0] == 'S':
+                    return piece
+            raise ValueError(f"Could not find session in {handle}.")
         elif self.task == FalconTask.h2:
-            return NotImplementedError("H2 not implemented.")
+            return handle.split('_')[-1].split('-')[-1]
         elif self.task == FalconTask.m1: # return date
             # sub-MonkeyL-held-in-minival_ses-20120924_behavior+ecephys.nwb
+            # or L_20120924_held_in_eval.nwb
             if 'behavior+ecephys' in handle:
                 return handle.split('_')[-2].split('-')[-1]
             return handle.split('_')[1]
         elif self.task == FalconTask.m2:
             raise NotImplementedError("M2 not implemented.")
 
 cs = ConfigStore.instance()
```

### Comparing `falcon_challenge-0.2.1/falcon_challenge/evaluator.py` & `falcon_challenge-0.2.3/falcon_challenge/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 from falcon_challenge.interface import BCIDecoder
 from falcon_challenge.dataloaders import load_nwb
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 HELD_IN_KEYS = {
-    FalconTask.h1: ['S608', 'S610', 'S613', 'S615', 'S619', 'S625'],
+    FalconTask.h1: ['S0_', 'S1_', 'S2_', 'S3_', 'S4_', 'S5_'],
     FalconTask.m1: ['L_20120924', 'L_20120926', 'L_20120927', 'L_20120928'],
 }
 
 HELD_OUT_KEYS = {
-    FalconTask.h1: ['S627', 'S631', 'S633', 'S636', 'S639', 'S641', 'S644'],
+    FalconTask.h1: ['S6_', 'S7_', 'S8_', 'S9_', 'S10_', 'S11_', 'S12_'],
     FalconTask.m1: ['L_20121004', 'L_20121017', 'L_20121022', 'L_20121024'],
 }
 
 # Development time flag. False allows direct evaluation without payload writing, only usable for local minival.
 # Should be set to true for remote evaluation.
 # USE_PKLS = False
 USE_PKLS = True
@@ -44,15 +44,18 @@
         Evaluate payloads with potentially multiple splits worth of data
         - Low pri: can I provide all results or just one split's worth entry? Currently providing 1, examples just provide 1, but in general would be nice to provide all. User shouldn't be able to submit more than 1, though.
     """
     # ! Want: Locally, test_annotation should be somewhere safe (tmp)
     # ! Remotely, it shoudl be /submission/submission.csv exactly.
     # Ignore explicit annotations provided and directly search for concatenated answers
     test_annotation_file = os.environ.get("GT_PATH", './local_gt.pkl')
+    logger.info(f"Evaluation: Docker side")
     logger.info(f"Loading GT from {test_annotation_file}")
+    logger.info(f"Loading submission from {user_submission_file}")
+    logger.info(f"Phase: {phase_codename}")
 
     result = []
     # Load pickles
     with open(test_annotation_file, 'rb') as test_annotation_file, open(user_submission_file, 'rb') as user_submission_file:
         test_annotations = pickle.load(test_annotation_file)
         user_submission = pickle.load(user_submission_file)
     for datasplit in user_submission: # datasplit e.g. h1, m1
@@ -159,15 +162,15 @@
         gt_path = os.environ.get("GT_PATH", './local_gt.pkl')
         if not gt_path:
             raise ValueError("GT_PATH not set in remote env which expects it. Cannot forward to separate evaluate runscript.")
             
         if phase == 'test':
             eval_files_held_in = [f for f in eval_files if any(k in f.name for k in HELD_IN_KEYS[self.dataset])]
             eval_files_held_out = [f for f in eval_files if any(k in f.name for k in HELD_OUT_KEYS[self.dataset])]
-            assert len(eval_files) == len(eval_files_held_in) + len(eval_files_held_out), "Mismatch in extracted eval files: Eval file state is not consistent with benchmark creation settings."
+            assert len(eval_files) == len(eval_files_held_in) + len(eval_files_held_out), f"Mismatch in extracted eval #: Eval file state is not consistent with benchmark creation settings. Found {len(eval_files)} files, {len(eval_files_held_in)} held in, {len(eval_files_held_out)} held out."
             all_preds_held_in, all_targets_held_in, all_eval_mask_held_in = self.predict_files(decoder, eval_files_held_in)
             all_preds_held_out, all_targets_held_out, all_eval_mask_held_out = self.predict_files(decoder, eval_files_held_out)
 
             # Indirect remote setup to satisfy EvalAI interface. Save metrics / comparison to file.
             if USE_PKLS:
                 pred_payload = {self.dataset.name: {
                     'held_in_pred': all_preds_held_in,
@@ -204,21 +207,25 @@
                     metrics[f'{HELDIN_OR_OUT_MAP["held_in"]} {k}'] = v
         
         if USE_PKLS:
             with open(prediction_path, 'wb') as f:
                 pickle.dump(pred_payload, f)
             with open(gt_path, 'wb') as f:
                 pickle.dump(truth_payload, f)
+            import time
+            # Sleep so it's definitely available
 
             # TODO - this subsequent line of logic needs to be owned by challenge worker - currently in here for Beta testing.
             print(evaluate(
                 test_annotation_file=gt_path,
                 user_submission_file=prediction_path,
                 phase_codename=phase
             ))
+            print("Sleeping for remote eval - feel free to interrupt for local eval.")
+            time.sleep(300) # Gunjan, EvalAI contact says that current static code eval has an issue where the submission dump is only polled by the EvalAI worker comparison script every 5 minutes
         else:
             for k, v in metrics.items():
                 logger.info("{}: {}".format(k, v))
         
 
     @staticmethod
     def compute_metrics_regression(preds, targets, eval_mask):
@@ -228,16 +235,16 @@
             "R2": r2_score(targets, preds, multioutput='variance_weighted'),
             "R2 Std.": 0, # TODO Clay
         }
 
     @staticmethod
     def compute_metrics_classification(preds, targets, eval_mask):
         return {
-            "WER": 1-(preds == targets)[eval_mask].mean(),
-            "WER Std.": 0, # TODO Clay
+            "CER": 1-(preds == targets)[eval_mask].mean(),
+            "CER Std.": 0, # TODO Clay
         }
 
     def compute_metrics(self, all_preds, all_targets, all_eval_mask=None):
         r"""
             all_preds: array of shape (n_timesteps, k_dim)
             all_targets: array of shape (n_timesteps, k_dim)
             all_eval_mask: array of shape (n_timesteps, k_dim). True if we should evaluate this timestep.
```

### Comparing `falcon_challenge-0.2.1/falcon_challenge/interface.py` & `falcon_challenge-0.2.3/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.1/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.2.3/falcon_challenge.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,8 +17,19 @@
 falcon_challenge/dataloaders.py
 falcon_challenge/evaluator.py
 falcon_challenge/interface.py
 falcon_challenge.egg-info/PKG-INFO
 falcon_challenge.egg-info/SOURCES.txt
 falcon_challenge.egg-info/dependency_links.txt
 falcon_challenge.egg-info/requires.txt
-falcon_challenge.egg-info/top_level.txt
+falcon_challenge.egg-info/top_level.txt
+preproc/__init__.py
+preproc/assemble_data.py
+preproc/filtering.py
+preproc/h2_preproc.py
+preproc/m1_fewshot_trial_counts.py
+preproc/m1_reachgrasp_preprocv2.py
+preproc/m2_fewshot_trial_counts.py
+preproc/m2_preproc.py
+preproc/nwb_create_utils.py
+preproc/wrapper_convert_batch.py
+preproc/zip_data.py
```

### Comparing `falcon_challenge-0.2.1/setup.py` & `falcon_challenge-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.2.1',
+    version='0.2.3',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

