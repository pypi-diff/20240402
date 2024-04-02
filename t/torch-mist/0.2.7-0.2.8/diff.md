# Comparing `tmp/torch_mist-0.2.7.tar.gz` & `tmp/torch_mist-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_mist-0.2.7.tar", max compression
+gzip compressed data, was "torch_mist-0.2.8.tar", max compression
```

## Comparing `torch_mist-0.2.7.tar` & `torch_mist-0.2.8.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rwxr-xr-x   0        0        0     1073 2023-06-20 12:29:18.481563 torch_mist-0.2.7/LICENSE
--rw-r--r--   0        0        0    17949 2024-02-13 12:46:08.072954 torch_mist-0.2.7/README.md
--rw-r--r--   0        0        0     1196 2024-02-19 15:16:25.233035 torch_mist-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-12 12:06:03.239441 torch_mist-0.2.7/scripts/__init__.py
--rw-r--r--   0        0        0     5527 2024-02-15 15:50:38.434954 torch_mist-0.2.7/scripts/compute_mi.py
--rw-r--r--   0        0        0        0 2024-02-12 12:44:27.742128 torch_mist-0.2.7/scripts/config/__init__.py
--rw-r--r--   0        0        0      895 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/config.yaml
--rw-r--r--   0        0        0       58 2024-02-12 14:16:43.288651 torch_mist-0.2.7/scripts/config/data/csv.yaml
--rw-r--r--   0        0        0      456 2024-02-12 13:27:48.435185 torch_mist-0.2.7/scripts/config/data/multimixture.yaml
--rw-r--r--   0        0        0      732 2024-02-13 17:03:28.648580 torch_mist-0.2.7/scripts/config/experiment/eval_distribution_mi.yaml
--rw-r--r--   0        0        0       72 2024-02-13 17:42:27.652998 torch_mist-0.2.7/scripts/config/logger/pandas.yaml
--rw-r--r--   0        0        0       93 2024-01-15 13:21:10.933711 torch_mist-0.2.7/scripts/config/logger/wandb.yaml
--rw-r--r--   0        0        0      144 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/alpha_tuba.yaml
--rw-r--r--   0        0        0      286 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/binned.yaml
--rw-r--r--   0        0        0      156 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/club.yaml
--rw-r--r--   0        0        0      226 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/doe.yaml
--rw-r--r--   0        0        0       89 2024-01-10 16:26:20.693682 torch_mist-0.2.7/scripts/config/mi_estimator/dummy_discriminative.yaml
--rw-r--r--   0        0        0       49 2024-01-10 16:26:03.312125 torch_mist-0.2.7/scripts/config/mi_estimator/dummy_generative.yaml
--rw-r--r--   0        0        0      179 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/flo.yaml
--rw-r--r--   0        0        0      213 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/gm.yaml
--rw-r--r--   0        0        0      293 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/hybrid_pq.yaml
--rw-r--r--   0        0        0      230 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/hybrid_resampled.yaml
--rw-r--r--   0        0        0      231 2024-01-05 17:24:33.473104 torch_mist-0.2.7/scripts/config/mi_estimator/hybrid_reweighed.yaml
--rw-r--r--   0        0        0      129 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/infonce.yaml
--rw-r--r--   0        0        0      159 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/js.yaml
--rw-r--r--   0        0        0      157 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/l1out.yaml
--rw-r--r--   0        0        0      161 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/mine.yaml
--rw-r--r--   0        0        0      160 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/nwj.yaml
--rw-r--r--   0        0        0      224 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/pq.yaml
--rw-r--r--   0        0        0      170 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/smile.yaml
--rw-r--r--   0        0        0      161 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/mi_estimator/tuba.yaml
--rw-r--r--   0        0        0       78 2024-02-14 16:17:36.687348 torch_mist-0.2.7/scripts/config/quantization/kmeans.yaml
--rw-r--r--   0        0        0      242 2024-02-15 15:24:18.875132 torch_mist-0.2.7/scripts/config/quantization/vqvae.yaml
--rw-r--r--   0        0        0      156 2024-02-14 16:06:42.173493 torch_mist-0.2.7/src/torch_mist/__init__.py
--rw-r--r--   0        0        0      193 2023-12-21 08:56:24.079626 torch_mist-0.2.7/src/torch_mist/baseline/__init__.py
--rw-r--r--   0        0        0     3147 2024-01-16 19:21:55.596510 torch_mist-0.2.7/src/torch_mist/baseline/base.py
--rw-r--r--   0        0        0      449 2023-11-29 15:49:05.131105 torch_mist-0.2.7/src/torch_mist/baseline/factories.py
--rw-r--r--   0        0        0      160 2023-11-06 13:11:00.463557 torch_mist-0.2.7/src/torch_mist/critic/__init__.py
--rw-r--r--   0        0        0      619 2024-01-09 14:44:44.324757 torch_mist-0.2.7/src/torch_mist/critic/base.py
--rw-r--r--   0        0        0      362 2024-01-15 13:17:26.283911 torch_mist-0.2.7/src/torch_mist/critic/constant.py
--rw-r--r--   0        0        0     5386 2024-02-13 10:54:32.140685 torch_mist-0.2.7/src/torch_mist/critic/factories.py
--rw-r--r--   0        0        0      723 2024-01-03 12:13:18.036537 torch_mist-0.2.7/src/torch_mist/critic/joint.py
--rw-r--r--   0        0        0     1387 2024-01-17 14:39:26.828546 torch_mist-0.2.7/src/torch_mist/critic/separable.py
--rw-r--r--   0        0        0        0 2023-10-16 12:20:33.634970 torch_mist-0.2.7/src/torch_mist/data/__init__.py
--rw-r--r--   0        0        0     4238 2023-11-10 17:19:40.156950 torch_mist-0.2.7/src/torch_mist/data/multimixture.py
--rw-r--r--   0        0        0     1418 2023-11-10 17:19:39.984949 torch_mist-0.2.7/src/torch_mist/data/multivariate.py
--rw-r--r--   0        0        0      413 2024-01-12 09:01:07.610990 torch_mist-0.2.7/src/torch_mist/data/utils.py
--rw-r--r--   0        0        0       21 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/decomposition/__init__.py
--rw-r--r--   0        0        0     6620 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/decomposition/mid.py
--rw-r--r--   0        0        0      314 2024-01-10 15:45:26.835949 torch_mist-0.2.7/src/torch_mist/distributions/__init__.py
--rw-r--r--   0        0        0     1676 2024-01-17 17:34:12.769234 torch_mist-0.2.7/src/torch_mist/distributions/caching.py
--rw-r--r--   0        0        0     1531 2023-12-21 12:08:11.510517 torch_mist-0.2.7/src/torch_mist/distributions/categorical.py
--rw-r--r--   0        0        0        0 2024-01-10 12:48:21.392238 torch_mist-0.2.7/src/torch_mist/distributions/conditional/__init__.py
--rw-r--r--   0        0        0      677 2024-01-12 09:01:07.630990 torch_mist-0.2.7/src/torch_mist/distributions/conditional/unconditional.py
--rw-r--r--   0        0        0      725 2024-01-17 15:28:15.615508 torch_mist-0.2.7/src/torch_mist/distributions/empirical.py
--rw-r--r--   0        0        0     4250 2024-02-16 10:54:43.825204 torch_mist-0.2.7/src/torch_mist/distributions/factories.py
--rw-r--r--   0        0        0        0 2023-11-02 12:18:32.706923 torch_mist-0.2.7/src/torch_mist/distributions/joint/__init__.py
--rw-r--r--   0        0        0     6984 2024-01-03 14:51:39.747043 torch_mist-0.2.7/src/torch_mist/distributions/joint/base.py
--rw-r--r--   0        0        0     2879 2023-11-10 17:19:40.096950 torch_mist-0.2.7/src/torch_mist/distributions/joint/categorical.py
--rw-r--r--   0        0        0     3346 2023-11-10 17:19:40.124950 torch_mist-0.2.7/src/torch_mist/distributions/joint/wrapper.py
--rw-r--r--   0        0        0     3690 2023-11-10 17:19:40.132950 torch_mist-0.2.7/src/torch_mist/distributions/normal.py
--rw-r--r--   0        0        0      219 2023-06-15 14:06:39.255551 torch_mist-0.2.7/src/torch_mist/distributions/parametrizations/__init__.py
--rw-r--r--   0        0        0     3874 2023-06-26 14:59:12.573939 torch_mist-0.2.7/src/torch_mist/distributions/parametrizations/map.py
--rw-r--r--   0        0        0      253 2024-01-10 09:49:29.316963 torch_mist-0.2.7/src/torch_mist/distributions/transforms/__init__.py
--rw-r--r--   0        0        0     4255 2024-01-17 17:34:12.941232 torch_mist-0.2.7/src/torch_mist/distributions/transforms/base.py
--rw-r--r--   0        0        0     2789 2024-01-12 09:01:07.738990 torch_mist-0.2.7/src/torch_mist/distributions/transforms/factories.py
--rw-r--r--   0        0        0      111 2024-01-10 09:41:25.840192 torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/__init__.py
--rw-r--r--   0        0        0     4143 2024-01-12 09:01:07.842991 torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/linear.py
--rw-r--r--   0        0        0     1150 2024-01-22 15:01:23.369726 torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/normalize.py
--rw-r--r--   0        0        0      971 2024-01-12 09:01:07.666990 torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/permute.py
--rw-r--r--   0        0        0      590 2024-01-10 09:47:49.777166 torch_mist-0.2.7/src/torch_mist/distributions/transforms/utils.py
--rw-r--r--   0        0        0      346 2024-01-03 10:43:13.363492 torch_mist-0.2.7/src/torch_mist/estimators/__init__.py
--rw-r--r--   0        0        0     1726 2024-02-14 19:04:11.574778 torch_mist-0.2.7/src/torch_mist/estimators/base.py
--rw-r--r--   0        0        0      135 2023-11-06 15:39:54.573054 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/__init__.py
--rw-r--r--   0        0        0     7042 2024-01-17 16:23:37.002050 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/base.py
--rw-r--r--   0        0        0     5275 2024-02-13 10:54:32.112686 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/factories.py
--rw-r--r--   0        0        0      245 2024-01-10 11:01:10.141839 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/__init__.py
--rw-r--r--   0        0        0      755 2024-01-05 16:03:19.501289 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/alpha_tuba.py
--rw-r--r--   0        0        0      632 2024-01-12 09:01:07.662990 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/dummy.py
--rw-r--r--   0        0        0     2104 2024-01-17 16:23:36.946051 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/flo.py
--rw-r--r--   0        0        0     1354 2024-01-17 17:34:12.737235 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/infonce.py
--rw-r--r--   0        0        0     1192 2024-01-05 16:03:19.505289 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/js.py
--rw-r--r--   0        0        0     1204 2024-01-16 11:41:31.986678 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/mine.py
--rw-r--r--   0        0        0      474 2023-11-10 17:19:40.128950 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/nwj.py
--rw-r--r--   0        0        0     1482 2024-01-09 14:44:44.408757 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/smile.py
--rw-r--r--   0        0        0      494 2024-01-03 12:29:39.515370 torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/tuba.py
--rw-r--r--   0        0        0      875 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/factories.py
--rw-r--r--   0        0        0      130 2023-11-10 17:19:40.140950 torch_mist-0.2.7/src/torch_mist/estimators/generative/__init__.py
--rw-r--r--   0        0        0     5971 2024-01-17 16:23:36.954051 torch_mist-0.2.7/src/torch_mist/estimators/generative/base.py
--rw-r--r--   0        0        0     6671 2024-01-12 09:01:07.970991 torch_mist-0.2.7/src/torch_mist/estimators/generative/factories.py
--rw-r--r--   0        0        0      153 2024-01-12 09:01:07.674990 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/__init__.py
--rw-r--r--   0        0        0      973 2024-01-09 14:44:44.380757 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/ba.py
--rw-r--r--   0        0        0      825 2023-12-14 12:52:39.911290 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/club.py
--rw-r--r--   0        0        0     1883 2024-01-17 16:23:36.930051 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/doe.py
--rw-r--r--   0        0        0      930 2024-01-12 09:01:07.730990 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/dummy.py
--rw-r--r--   0        0        0     1364 2024-01-16 19:21:55.480514 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/gm.py
--rw-r--r--   0        0        0     2316 2024-01-17 15:28:15.631507 torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/l1out.py
--rw-r--r--   0        0        0       76 2024-01-03 10:43:13.367492 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/__init__.py
--rw-r--r--   0        0        0     3750 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/base.py
--rw-r--r--   0        0        0     1275 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/factories.py
--rw-r--r--   0        0        0      144 2023-12-19 11:21:40.158906 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/__init__.py
--rw-r--r--   0        0        0     3065 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/hybrid_pq.py
--rw-r--r--   0        0        0     1816 2024-01-17 16:23:36.918051 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/resampled.py
--rw-r--r--   0        0        0      812 2024-01-17 16:23:37.018050 torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/reweighted.py
--rw-r--r--   0        0        0     3406 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/multi.py
--rw-r--r--   0        0        0       97 2023-11-06 15:07:50.634288 torch_mist-0.2.7/src/torch_mist/estimators/transformed/__init__.py
--rw-r--r--   0        0        0     4953 2024-01-19 17:06:37.494572 torch_mist-0.2.7/src/torch_mist/estimators/transformed/base.py
--rw-r--r--   0        0        0     1394 2024-02-14 17:41:35.961813 torch_mist-0.2.7/src/torch_mist/estimators/transformed/factories.py
--rw-r--r--   0        0        0       57 2023-11-10 17:19:40.240950 torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/__init__.py
--rw-r--r--   0        0        0     1739 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/binned.py
--rw-r--r--   0        0        0      960 2024-01-03 14:34:25.751166 torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/flip.py
--rw-r--r--   0        0        0     1116 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/pq.py
--rw-r--r--   0        0        0      314 2023-12-20 15:54:31.008800 torch_mist-0.2.7/src/torch_mist/estimators/transformed/utils.py
--rw-r--r--   0        0        0      800 2023-12-01 17:12:24.798153 torch_mist-0.2.7/src/torch_mist/estimators/utils.py
--rw-r--r--   0        0        0     2596 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/nn.py
--rw-r--r--   0        0        0      210 2023-11-09 14:52:43.522135 torch_mist-0.2.7/src/torch_mist/quantization/__init__.py
--rw-r--r--   0        0        0     1427 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/quantization/factories.py
--rw-r--r--   0        0        0     6190 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/quantization/functions.py
--rw-r--r--   0        0        0     4464 2024-02-15 15:35:15.753978 torch_mist-0.2.7/src/torch_mist/quantization/vqvae.py
--rw-r--r--   0        0        0      175 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/utils/__init__.py
--rw-r--r--   0        0        0     3473 2024-01-17 17:34:12.961232 torch_mist-0.2.7/src/torch_mist/utils/caching.py
--rw-r--r--   0        0        0      186 2024-02-12 10:38:24.376568 torch_mist-0.2.7/src/torch_mist/utils/data/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-13 10:54:32.008689 torch_mist-0.2.7/src/torch_mist/utils/data/csv.py
--rw-r--r--   0        0        0     2648 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/utils/data/dataset.py
--rw-r--r--   0        0        0     2392 2024-02-12 10:37:46.980419 torch_mist-0.2.7/src/torch_mist/utils/data/loader.py
--rw-r--r--   0        0        0     4422 2024-01-17 14:31:28.795667 torch_mist-0.2.7/src/torch_mist/utils/data/sampler.py
--rw-r--r--   0        0        0     6516 2024-02-19 15:15:16.531880 torch_mist-0.2.7/src/torch_mist/utils/data/utils.py
--rw-r--r--   0        0        0     6061 2024-02-19 10:48:44.967971 torch_mist-0.2.7/src/torch_mist/utils/estimation.py
--rw-r--r--   0        0        0       66 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/utils/evaluation/__init__.py
--rw-r--r--   0        0        0     1067 2024-02-19 15:16:07.624734 torch_mist-0.2.7/src/torch_mist/utils/evaluation/mi_estimator.py
--rw-r--r--   0        0        0     1684 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/utils/evaluation/model.py
--rw-r--r--   0        0        0      691 2024-01-03 15:40:57.596457 torch_mist-0.2.7/src/torch_mist/utils/freeze.py
--rw-r--r--   0        0        0     1027 2024-01-17 17:34:12.909233 torch_mist-0.2.7/src/torch_mist/utils/indexing.py
--rw-r--r--   0        0        0       41 2023-12-04 17:09:27.481072 torch_mist-0.2.7/src/torch_mist/utils/logging/__init__.py
--rw-r--r--   0        0        0       58 2023-12-04 17:09:27.485072 torch_mist-0.2.7/src/torch_mist/utils/logging/logger/__init__.py
--rw-r--r--   0        0        0     7429 2024-02-19 14:55:44.926483 torch_mist-0.2.7/src/torch_mist/utils/logging/logger/base.py
--rw-r--r--   0        0        0     1490 2024-02-19 14:55:44.954482 torch_mist-0.2.7/src/torch_mist/utils/logging/logger/pandas.py
--rw-r--r--   0        0        0     1953 2024-02-19 14:55:44.942482 torch_mist-0.2.7/src/torch_mist/utils/logging/logger/wandb.py
--rw-r--r--   0        0        0     1064 2024-01-16 12:56:03.949709 torch_mist-0.2.7/src/torch_mist/utils/logging/metrics.py
--rw-r--r--   0        0        0      931 2024-01-17 17:34:12.897233 torch_mist-0.2.7/src/torch_mist/utils/shape.py
--rw-r--r--   0        0        0       76 2023-12-05 14:42:19.504323 torch_mist-0.2.7/src/torch_mist/utils/train/__init__.py
--rw-r--r--   0        0        0     3802 2024-02-15 15:35:00.301944 torch_mist-0.2.7/src/torch_mist/utils/train/mi_estimator.py
--rw-r--r--   0        0        0    11250 2024-02-19 14:44:35.567540 torch_mist-0.2.7/src/torch_mist/utils/train/model.py
--rw-r--r--   0        0        0     3468 2024-02-19 14:50:05.157562 torch_mist-0.2.7/src/torch_mist/utils/train/utils.py
--rw-r--r--   0        0        0    18719 1970-01-01 00:00:00.000000 torch_mist-0.2.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-06-20 12:29:18.481563 torch_mist-0.2.8/LICENSE
+-rw-r--r--   0        0        0    17949 2024-02-13 12:46:08.072954 torch_mist-0.2.8/README.md
+-rw-r--r--   0        0        0     1196 2024-02-22 15:52:23.800974 torch_mist-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-12 12:06:03.239441 torch_mist-0.2.8/scripts/__init__.py
+-rw-r--r--   0        0        0     5527 2024-02-15 15:50:38.434954 torch_mist-0.2.8/scripts/compute_mi.py
+-rw-r--r--   0        0        0        0 2024-02-12 12:44:27.742128 torch_mist-0.2.8/scripts/config/__init__.py
+-rw-r--r--   0        0        0      895 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/config.yaml
+-rw-r--r--   0        0        0       58 2024-02-12 14:16:43.288651 torch_mist-0.2.8/scripts/config/data/csv.yaml
+-rw-r--r--   0        0        0      456 2024-02-12 13:27:48.435185 torch_mist-0.2.8/scripts/config/data/multimixture.yaml
+-rw-r--r--   0        0        0      732 2024-02-13 17:03:28.648580 torch_mist-0.2.8/scripts/config/experiment/eval_distribution_mi.yaml
+-rw-r--r--   0        0        0       72 2024-02-13 17:42:27.652998 torch_mist-0.2.8/scripts/config/logger/pandas.yaml
+-rw-r--r--   0        0        0       93 2024-01-15 13:21:10.933711 torch_mist-0.2.8/scripts/config/logger/wandb.yaml
+-rw-r--r--   0        0        0      144 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/alpha_tuba.yaml
+-rw-r--r--   0        0        0      286 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/binned.yaml
+-rw-r--r--   0        0        0      156 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/club.yaml
+-rw-r--r--   0        0        0      226 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/doe.yaml
+-rw-r--r--   0        0        0       89 2024-01-10 16:26:20.693682 torch_mist-0.2.8/scripts/config/mi_estimator/dummy_discriminative.yaml
+-rw-r--r--   0        0        0       49 2024-01-10 16:26:03.312125 torch_mist-0.2.8/scripts/config/mi_estimator/dummy_generative.yaml
+-rw-r--r--   0        0        0      179 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/flo.yaml
+-rw-r--r--   0        0        0      213 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/gm.yaml
+-rw-r--r--   0        0        0      293 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/hybrid_pq.yaml
+-rw-r--r--   0        0        0      230 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/hybrid_resampled.yaml
+-rw-r--r--   0        0        0      231 2024-01-05 17:24:33.473104 torch_mist-0.2.8/scripts/config/mi_estimator/hybrid_reweighed.yaml
+-rw-r--r--   0        0        0      129 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/infonce.yaml
+-rw-r--r--   0        0        0      159 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/js.yaml
+-rw-r--r--   0        0        0      157 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/l1out.yaml
+-rw-r--r--   0        0        0      161 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/mine.yaml
+-rw-r--r--   0        0        0      160 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/nwj.yaml
+-rw-r--r--   0        0        0      224 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/pq.yaml
+-rw-r--r--   0        0        0      170 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/smile.yaml
+-rw-r--r--   0        0        0      161 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/mi_estimator/tuba.yaml
+-rw-r--r--   0        0        0       78 2024-02-14 16:17:36.687348 torch_mist-0.2.8/scripts/config/quantization/kmeans.yaml
+-rw-r--r--   0        0        0      242 2024-02-15 15:24:18.875132 torch_mist-0.2.8/scripts/config/quantization/vqvae.yaml
+-rw-r--r--   0        0        0      176 2024-02-22 13:00:40.355889 torch_mist-0.2.8/src/torch_mist/__init__.py
+-rw-r--r--   0        0        0      193 2023-12-21 08:56:24.079626 torch_mist-0.2.8/src/torch_mist/baseline/__init__.py
+-rw-r--r--   0        0        0     3147 2024-01-16 19:21:55.596510 torch_mist-0.2.8/src/torch_mist/baseline/base.py
+-rw-r--r--   0        0        0      449 2023-11-29 15:49:05.131105 torch_mist-0.2.8/src/torch_mist/baseline/factories.py
+-rw-r--r--   0        0        0      160 2023-11-06 13:11:00.463557 torch_mist-0.2.8/src/torch_mist/critic/__init__.py
+-rw-r--r--   0        0        0      619 2024-01-09 14:44:44.324757 torch_mist-0.2.8/src/torch_mist/critic/base.py
+-rw-r--r--   0        0        0      362 2024-01-15 13:17:26.283911 torch_mist-0.2.8/src/torch_mist/critic/constant.py
+-rw-r--r--   0        0        0     5386 2024-02-13 10:54:32.140685 torch_mist-0.2.8/src/torch_mist/critic/factories.py
+-rw-r--r--   0        0        0      723 2024-01-03 12:13:18.036537 torch_mist-0.2.8/src/torch_mist/critic/joint.py
+-rw-r--r--   0        0        0     1387 2024-01-17 14:39:26.828546 torch_mist-0.2.8/src/torch_mist/critic/separable.py
+-rw-r--r--   0        0        0        0 2023-10-16 12:20:33.634970 torch_mist-0.2.8/src/torch_mist/data/__init__.py
+-rw-r--r--   0        0        0     4238 2023-11-10 17:19:40.156950 torch_mist-0.2.8/src/torch_mist/data/multimixture.py
+-rw-r--r--   0        0        0     1418 2023-11-10 17:19:39.984949 torch_mist-0.2.8/src/torch_mist/data/multivariate.py
+-rw-r--r--   0        0        0      413 2024-01-12 09:01:07.610990 torch_mist-0.2.8/src/torch_mist/data/utils.py
+-rw-r--r--   0        0        0       21 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/decomposition/__init__.py
+-rw-r--r--   0        0        0     7253 2024-02-22 15:48:41.801250 torch_mist-0.2.8/src/torch_mist/decomposition/mid.py
+-rw-r--r--   0        0        0      314 2024-01-10 15:45:26.835949 torch_mist-0.2.8/src/torch_mist/distributions/__init__.py
+-rw-r--r--   0        0        0     1676 2024-01-17 17:34:12.769234 torch_mist-0.2.8/src/torch_mist/distributions/caching.py
+-rw-r--r--   0        0        0     1531 2023-12-21 12:08:11.510517 torch_mist-0.2.8/src/torch_mist/distributions/categorical.py
+-rw-r--r--   0        0        0        0 2024-01-10 12:48:21.392238 torch_mist-0.2.8/src/torch_mist/distributions/conditional/__init__.py
+-rw-r--r--   0        0        0      677 2024-01-12 09:01:07.630990 torch_mist-0.2.8/src/torch_mist/distributions/conditional/unconditional.py
+-rw-r--r--   0        0        0      725 2024-01-17 15:28:15.615508 torch_mist-0.2.8/src/torch_mist/distributions/empirical.py
+-rw-r--r--   0        0        0     4250 2024-02-16 10:54:43.825204 torch_mist-0.2.8/src/torch_mist/distributions/factories.py
+-rw-r--r--   0        0        0        0 2023-11-02 12:18:32.706923 torch_mist-0.2.8/src/torch_mist/distributions/joint/__init__.py
+-rw-r--r--   0        0        0     6984 2024-01-03 14:51:39.747043 torch_mist-0.2.8/src/torch_mist/distributions/joint/base.py
+-rw-r--r--   0        0        0     2879 2023-11-10 17:19:40.096950 torch_mist-0.2.8/src/torch_mist/distributions/joint/categorical.py
+-rw-r--r--   0        0        0     3346 2023-11-10 17:19:40.124950 torch_mist-0.2.8/src/torch_mist/distributions/joint/wrapper.py
+-rw-r--r--   0        0        0     3690 2023-11-10 17:19:40.132950 torch_mist-0.2.8/src/torch_mist/distributions/normal.py
+-rw-r--r--   0        0        0      219 2023-06-15 14:06:39.255551 torch_mist-0.2.8/src/torch_mist/distributions/parametrizations/__init__.py
+-rw-r--r--   0        0        0     3874 2023-06-26 14:59:12.573939 torch_mist-0.2.8/src/torch_mist/distributions/parametrizations/map.py
+-rw-r--r--   0        0        0      253 2024-01-10 09:49:29.316963 torch_mist-0.2.8/src/torch_mist/distributions/transforms/__init__.py
+-rw-r--r--   0        0        0     4255 2024-01-17 17:34:12.941232 torch_mist-0.2.8/src/torch_mist/distributions/transforms/base.py
+-rw-r--r--   0        0        0     2789 2024-01-12 09:01:07.738990 torch_mist-0.2.8/src/torch_mist/distributions/transforms/factories.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:41:25.840192 torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/__init__.py
+-rw-r--r--   0        0        0     4143 2024-01-12 09:01:07.842991 torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/linear.py
+-rw-r--r--   0        0        0     1150 2024-01-22 15:01:23.369726 torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/normalize.py
+-rw-r--r--   0        0        0      971 2024-01-12 09:01:07.666990 torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/permute.py
+-rw-r--r--   0        0        0      590 2024-01-10 09:47:49.777166 torch_mist-0.2.8/src/torch_mist/distributions/transforms/utils.py
+-rw-r--r--   0        0        0      346 2024-01-03 10:43:13.363492 torch_mist-0.2.8/src/torch_mist/estimators/__init__.py
+-rw-r--r--   0        0        0     1726 2024-02-14 19:04:11.574778 torch_mist-0.2.8/src/torch_mist/estimators/base.py
+-rw-r--r--   0        0        0      135 2023-11-06 15:39:54.573054 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/__init__.py
+-rw-r--r--   0        0        0     7042 2024-01-17 16:23:37.002050 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/base.py
+-rw-r--r--   0        0        0     5275 2024-02-13 10:54:32.112686 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/factories.py
+-rw-r--r--   0        0        0      245 2024-01-10 11:01:10.141839 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/__init__.py
+-rw-r--r--   0        0        0      755 2024-01-05 16:03:19.501289 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/alpha_tuba.py
+-rw-r--r--   0        0        0      632 2024-01-12 09:01:07.662990 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/dummy.py
+-rw-r--r--   0        0        0     2104 2024-01-17 16:23:36.946051 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/flo.py
+-rw-r--r--   0        0        0     1354 2024-01-17 17:34:12.737235 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/infonce.py
+-rw-r--r--   0        0        0     1192 2024-01-05 16:03:19.505289 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/js.py
+-rw-r--r--   0        0        0     1204 2024-01-16 11:41:31.986678 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/mine.py
+-rw-r--r--   0        0        0      474 2023-11-10 17:19:40.128950 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/nwj.py
+-rw-r--r--   0        0        0     1482 2024-01-09 14:44:44.408757 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/smile.py
+-rw-r--r--   0        0        0      494 2024-01-03 12:29:39.515370 torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/tuba.py
+-rw-r--r--   0        0        0      875 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/factories.py
+-rw-r--r--   0        0        0      130 2023-11-10 17:19:40.140950 torch_mist-0.2.8/src/torch_mist/estimators/generative/__init__.py
+-rw-r--r--   0        0        0     5971 2024-01-17 16:23:36.954051 torch_mist-0.2.8/src/torch_mist/estimators/generative/base.py
+-rw-r--r--   0        0        0     6671 2024-01-12 09:01:07.970991 torch_mist-0.2.8/src/torch_mist/estimators/generative/factories.py
+-rw-r--r--   0        0        0      153 2024-01-12 09:01:07.674990 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/__init__.py
+-rw-r--r--   0        0        0      973 2024-01-09 14:44:44.380757 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/ba.py
+-rw-r--r--   0        0        0      825 2023-12-14 12:52:39.911290 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/club.py
+-rw-r--r--   0        0        0     1883 2024-01-17 16:23:36.930051 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/doe.py
+-rw-r--r--   0        0        0      930 2024-01-12 09:01:07.730990 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/dummy.py
+-rw-r--r--   0        0        0     1364 2024-01-16 19:21:55.480514 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/gm.py
+-rw-r--r--   0        0        0     2316 2024-01-17 15:28:15.631507 torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/l1out.py
+-rw-r--r--   0        0        0       76 2024-01-03 10:43:13.367492 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/__init__.py
+-rw-r--r--   0        0        0     3750 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/base.py
+-rw-r--r--   0        0        0     1275 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/factories.py
+-rw-r--r--   0        0        0      144 2023-12-19 11:21:40.158906 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/__init__.py
+-rw-r--r--   0        0        0     3065 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/hybrid_pq.py
+-rw-r--r--   0        0        0     1816 2024-01-17 16:23:36.918051 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/resampled.py
+-rw-r--r--   0        0        0      812 2024-01-17 16:23:37.018050 torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/reweighted.py
+-rw-r--r--   0        0        0     3406 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/multi.py
+-rw-r--r--   0        0        0       97 2023-11-06 15:07:50.634288 torch_mist-0.2.8/src/torch_mist/estimators/transformed/__init__.py
+-rw-r--r--   0        0        0     4953 2024-01-19 17:06:37.494572 torch_mist-0.2.8/src/torch_mist/estimators/transformed/base.py
+-rw-r--r--   0        0        0     1394 2024-02-14 17:41:35.961813 torch_mist-0.2.8/src/torch_mist/estimators/transformed/factories.py
+-rw-r--r--   0        0        0       57 2023-11-10 17:19:40.240950 torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/__init__.py
+-rw-r--r--   0        0        0     1739 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/binned.py
+-rw-r--r--   0        0        0      960 2024-01-03 14:34:25.751166 torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/flip.py
+-rw-r--r--   0        0        0     1116 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/pq.py
+-rw-r--r--   0        0        0      314 2023-12-20 15:54:31.008800 torch_mist-0.2.8/src/torch_mist/estimators/transformed/utils.py
+-rw-r--r--   0        0        0      800 2023-12-01 17:12:24.798153 torch_mist-0.2.8/src/torch_mist/estimators/utils.py
+-rw-r--r--   0        0        0     2596 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/nn.py
+-rw-r--r--   0        0        0      210 2023-11-09 14:52:43.522135 torch_mist-0.2.8/src/torch_mist/quantization/__init__.py
+-rw-r--r--   0        0        0     1427 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/quantization/factories.py
+-rw-r--r--   0        0        0     6190 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/quantization/functions.py
+-rw-r--r--   0        0        0     4464 2024-02-15 15:35:15.753978 torch_mist-0.2.8/src/torch_mist/quantization/vqvae.py
+-rw-r--r--   0        0        0      175 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/utils/__init__.py
+-rw-r--r--   0        0        0     3473 2024-01-17 17:34:12.961232 torch_mist-0.2.8/src/torch_mist/utils/caching.py
+-rw-r--r--   0        0        0      186 2024-02-12 10:38:24.376568 torch_mist-0.2.8/src/torch_mist/utils/data/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-13 10:54:32.008689 torch_mist-0.2.8/src/torch_mist/utils/data/csv.py
+-rw-r--r--   0        0        0     2648 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/utils/data/dataset.py
+-rw-r--r--   0        0        0     2392 2024-02-12 10:37:46.980419 torch_mist-0.2.8/src/torch_mist/utils/data/loader.py
+-rw-r--r--   0        0        0     4422 2024-01-17 14:31:28.795667 torch_mist-0.2.8/src/torch_mist/utils/data/sampler.py
+-rw-r--r--   0        0        0     7992 2024-02-22 12:50:14.329933 torch_mist-0.2.8/src/torch_mist/utils/data/utils.py
+-rw-r--r--   0        0        0    13592 2024-02-22 15:50:29.225090 torch_mist-0.2.8/src/torch_mist/utils/estimation.py
+-rw-r--r--   0        0        0       66 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/utils/evaluation/__init__.py
+-rw-r--r--   0        0        0     1067 2024-02-19 15:16:07.624734 torch_mist-0.2.8/src/torch_mist/utils/evaluation/mi_estimator.py
+-rw-r--r--   0        0        0     1684 2024-02-15 15:35:00.301944 torch_mist-0.2.8/src/torch_mist/utils/evaluation/model.py
+-rw-r--r--   0        0        0      691 2024-01-03 15:40:57.596457 torch_mist-0.2.8/src/torch_mist/utils/freeze.py
+-rw-r--r--   0        0        0     1027 2024-01-17 17:34:12.909233 torch_mist-0.2.8/src/torch_mist/utils/indexing.py
+-rw-r--r--   0        0        0       41 2023-12-04 17:09:27.481072 torch_mist-0.2.8/src/torch_mist/utils/logging/__init__.py
+-rw-r--r--   0        0        0       58 2023-12-04 17:09:27.485072 torch_mist-0.2.8/src/torch_mist/utils/logging/logger/__init__.py
+-rw-r--r--   0        0        0     7481 2024-02-22 12:50:14.345933 torch_mist-0.2.8/src/torch_mist/utils/logging/logger/base.py
+-rw-r--r--   0        0        0     1490 2024-02-19 14:55:44.954482 torch_mist-0.2.8/src/torch_mist/utils/logging/logger/pandas.py
+-rw-r--r--   0        0        0     1953 2024-02-19 14:55:44.942482 torch_mist-0.2.8/src/torch_mist/utils/logging/logger/wandb.py
+-rw-r--r--   0        0        0     1064 2024-01-16 12:56:03.949709 torch_mist-0.2.8/src/torch_mist/utils/logging/metrics.py
+-rw-r--r--   0        0        0      931 2024-01-17 17:34:12.897233 torch_mist-0.2.8/src/torch_mist/utils/shape.py
+-rw-r--r--   0        0        0       76 2023-12-05 14:42:19.504323 torch_mist-0.2.8/src/torch_mist/utils/train/__init__.py
+-rw-r--r--   0        0        0     3813 2024-02-22 15:27:57.406459 torch_mist-0.2.8/src/torch_mist/utils/train/mi_estimator.py
+-rw-r--r--   0        0        0    11818 2024-02-22 15:42:04.842496 torch_mist-0.2.8/src/torch_mist/utils/train/model.py
+-rw-r--r--   0        0        0     3468 2024-02-19 14:50:05.157562 torch_mist-0.2.8/src/torch_mist/utils/train/utils.py
+-rw-r--r--   0        0        0    18719 1970-01-01 00:00:00.000000 torch_mist-0.2.8/PKG-INFO
```

### Comparing `torch_mist-0.2.7/LICENSE` & `torch_mist-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/README.md` & `torch_mist-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/pyproject.toml` & `torch_mist-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch_mist"
-version = "0.2.7"
+version = "0.2.8"
 description = "Mutual Information Estimation toolkit based on pytorch"
 authors = ["Marco Federici"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "torch_mist", from = "src"},
     {include = "scripts"}
```

### Comparing `torch_mist-0.2.7/scripts/compute_mi.py` & `torch_mist-0.2.8/scripts/compute_mi.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/scripts/config/config.yaml` & `torch_mist-0.2.8/scripts/config/config.yaml`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/scripts/config/experiment/eval_distribution_mi.yaml` & `torch_mist-0.2.8/scripts/config/experiment/eval_distribution_mi.yaml`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/baseline/base.py` & `torch_mist-0.2.8/src/torch_mist/baseline/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/critic/base.py` & `torch_mist-0.2.8/src/torch_mist/critic/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/critic/factories.py` & `torch_mist-0.2.8/src/torch_mist/critic/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/critic/joint.py` & `torch_mist-0.2.8/src/torch_mist/critic/joint.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/critic/separable.py` & `torch_mist-0.2.8/src/torch_mist/critic/separable.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/data/multimixture.py` & `torch_mist-0.2.8/src/torch_mist/data/multimixture.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/data/multivariate.py` & `torch_mist-0.2.8/src/torch_mist/data/multivariate.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/decomposition/mid.py` & `torch_mist-0.2.8/src/torch_mist/decomposition/mid.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     instantiate_estimator,
     TransformedMIEstimator,
 )
 from torch_mist.nn import dense_nn
 from torch_mist.utils import train_mi_estimator
 
 
+DEFAULT_MAX_ITERATIONS = 5000
+DEFAULT_BATCH_SIZE = 64
+
 class CenterAndScale(nn.Module):
     def __init__(self, loc: torch.Tensor, scale: torch.Tensor):
         super().__init__()
         self.register_buffer("loc", torch.FloatTensor(loc))
         self.register_buffer("scale", torch.FloatTensor(scale))
 
     def forward(self, data):
@@ -108,31 +111,45 @@
 
         return mi_estimator_params
 
     def _add_default_proj_params(
         self, proj_params: Dict[str, Any]
     ) -> Dict[str, Any]:
         if not ("hidden_dims" in proj_params):
-            proj_params["hidden_dims"] = [64]
+            proj_params["hidden_dims"] = [128]
         if not ("nonlinearity" in proj_params):
             proj_params["nonlinearity"] = nn.ReLU(True)
 
         proj_params["output_dim"] = self.n_dim
         return proj_params
 
     def _add_default_train_params(
         self, train_params: Dict[str, Any]
     ) -> Dict[str, Any]:
         if not ("batch_size" in train_params):
-            train_params["batch_size"] = 64
+            print(
+                "[Info]: batch_size is not specified," +
+                f" using batch_size={DEFAULT_BATCH_SIZE} by default."
+            )
+            train_params["batch_size"] = DEFAULT_BATCH_SIZE
 
         if not ("max_epochs" in train_params) and not (
             "max_iterations" in train_params
         ):
-            train_params["max_epochs"] = 10
+            print(
+                "[Info]: max_epoch and max_iterations are not specified,"+
+                f" using max_iterations={DEFAULT_MAX_ITERATIONS} by default."
+            )
+            train_params["max_iterations"] = DEFAULT_MAX_ITERATIONS
+
+        if not ("early_stopping" in train_params):
+            train_params["early_stopping"] = True
+
+        if not ("verbose" in train_params):
+            train_params["verbose"] = False
 
         return train_params
 
     def _instantiate_proj(self, input_dim: int):
         self.proj_params["input_dim"] = input_dim
         self._proj = dense_nn(**self.proj_params)
```

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/caching.py` & `torch_mist-0.2.8/src/torch_mist/distributions/caching.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/categorical.py` & `torch_mist-0.2.8/src/torch_mist/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/conditional/unconditional.py` & `torch_mist-0.2.8/src/torch_mist/distributions/conditional/unconditional.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/empirical.py` & `torch_mist-0.2.8/src/torch_mist/distributions/empirical.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/factories.py` & `torch_mist-0.2.8/src/torch_mist/distributions/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/joint/base.py` & `torch_mist-0.2.8/src/torch_mist/distributions/joint/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/joint/categorical.py` & `torch_mist-0.2.8/src/torch_mist/distributions/joint/categorical.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/joint/wrapper.py` & `torch_mist-0.2.8/src/torch_mist/distributions/joint/wrapper.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/normal.py` & `torch_mist-0.2.8/src/torch_mist/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/parametrizations/map.py` & `torch_mist-0.2.8/src/torch_mist/distributions/parametrizations/map.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/transforms/base.py` & `torch_mist-0.2.8/src/torch_mist/distributions/transforms/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/transforms/factories.py` & `torch_mist-0.2.8/src/torch_mist/distributions/transforms/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/linear.py` & `torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/linear.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/normalize.py` & `torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/normalize.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/transforms/implementations/permute.py` & `torch_mist-0.2.8/src/torch_mist/distributions/transforms/implementations/permute.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/distributions/transforms/utils.py` & `torch_mist-0.2.8/src/torch_mist/distributions/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/base.py` & `torch_mist-0.2.8/src/torch_mist/estimators/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/base.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/factories.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/alpha_tuba.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/alpha_tuba.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/dummy.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/flo.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/flo.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/infonce.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/infonce.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/js.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/js.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/mine.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/mine.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/discriminative/implementations/smile.py` & `torch_mist-0.2.8/src/torch_mist/estimators/discriminative/implementations/smile.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/factories.py` & `torch_mist-0.2.8/src/torch_mist/estimators/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/base.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/factories.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/ba.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/ba.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/club.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/club.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/doe.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/doe.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/dummy.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/gm.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/gm.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/generative/implementations/l1out.py` & `torch_mist-0.2.8/src/torch_mist/estimators/generative/implementations/l1out.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/hybrid/base.py` & `torch_mist-0.2.8/src/torch_mist/estimators/hybrid/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/hybrid/factories.py` & `torch_mist-0.2.8/src/torch_mist/estimators/hybrid/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/hybrid_pq.py` & `torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/hybrid_pq.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/resampled.py` & `torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/resampled.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/hybrid/implementations/reweighted.py` & `torch_mist-0.2.8/src/torch_mist/estimators/hybrid/implementations/reweighted.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/multi.py` & `torch_mist-0.2.8/src/torch_mist/estimators/multi.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/transformed/base.py` & `torch_mist-0.2.8/src/torch_mist/estimators/transformed/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/transformed/factories.py` & `torch_mist-0.2.8/src/torch_mist/estimators/transformed/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/binned.py` & `torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/binned.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/flip.py` & `torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/flip.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/transformed/implementations/pq.py` & `torch_mist-0.2.8/src/torch_mist/estimators/transformed/implementations/pq.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/estimators/utils.py` & `torch_mist-0.2.8/src/torch_mist/estimators/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/nn.py` & `torch_mist-0.2.8/src/torch_mist/nn.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/quantization/factories.py` & `torch_mist-0.2.8/src/torch_mist/quantization/factories.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/quantization/functions.py` & `torch_mist-0.2.8/src/torch_mist/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/quantization/vqvae.py` & `torch_mist-0.2.8/src/torch_mist/quantization/vqvae.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/caching.py` & `torch_mist-0.2.8/src/torch_mist/utils/caching.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/data/csv.py` & `torch_mist-0.2.8/src/torch_mist/utils/data/csv.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/data/dataset.py` & `torch_mist-0.2.8/src/torch_mist/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/data/loader.py` & `torch_mist-0.2.8/src/torch_mist/utils/data/loader.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/data/sampler.py` & `torch_mist-0.2.8/src/torch_mist/utils/data/sampler.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/data/utils.py` & `torch_mist-0.2.8/src/torch_mist/utils/data/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Union, Tuple, Dict, Callable, List, Any
 
 import numpy as np
 import pandas as pd
 import torch
-from torch.utils.data import DataLoader, random_split, Dataset
+from torch.utils.data import DataLoader, random_split, Dataset, Subset
 
 from torch_mist.estimators import MIEstimator, TransformedMIEstimator
 from torch_mist.estimators.hybrid import PQHybridMIEstimator
 from torch_mist.utils.data import SampleDataset, SameAttributeDataLoader
 from torch_mist.utils.data.dataset import DataFrameDataset
 from torch_mist.utils.data.loader import sample_same_value
 
@@ -58,14 +58,37 @@
     array: Union[torch.Tensor, np.array]
 ) -> torch.FloatTensor:
     if isinstance(array, np.ndarray):
         array = torch.FloatTensor(array)
     return array
 
 
+def is_valid_entry(entry: Union[Dict[str, Any], np.ndarray, torch.Tensor, Tuple[Any, ...]]) -> bool:
+    if isinstance(entry, torch.Tensor):
+        return torch.sum(entry!=entry) == 0
+    elif isinstance(entry, np.ndarray):
+        return np.sum(entry!=entry) == 0
+    elif hasattr(entry, 'values'):
+        is_valid = True
+        for element in entry.values():
+            if not is_valid_entry(element):
+                is_valid = False
+                break
+        return is_valid
+    elif isinstance(entry, tuple):
+        is_valid = True
+        for element in entry:
+            if not is_valid_entry(element):
+                is_valid = False
+                break
+        return is_valid
+    else:
+        return True
+
+
 def make_dataset(data: TensorDictLike) -> Dataset:
     # Validate the input combinations
     if isinstance(data, list) or isinstance(data, tuple):
         if len(data) != 2:
             raise ValueError("data should be a tuple of two elements (x, y).")
         x, y = data[0], data[1]
 
@@ -85,63 +108,90 @@
         dataset = DataFrameDataset(data)
     else:
         dataset = data
 
     return dataset
 
 
+def filter_dataset(dataset: Dataset):
+    # Remove invalid entries
+    valid_ids = []
+    for idx, entry in enumerate(dataset):
+        if is_valid_entry(entry):
+            valid_ids.append(idx)
+    if len(valid_ids)!=len(dataset):
+        print(f"[Warning]: Removing {len(dataset)-len(valid_ids)} entries from the dataset")
+        dataset = Subset(dataset, valid_ids)
+
+    return dataset
+
+
 def is_data_loader(data: TensorDictLike):
     return isinstance(data, DataLoader)
 
+
 def make_default_dataloader(
     data: TensorDictLike,
     batch_size: Optional[int] = None,
     num_workers: int = 0,
-    shuffle: bool = False
+    shuffle: bool = False,
+    filter_invalid_data : bool = True
 ) -> DataLoader:
     if is_data_loader(data):
         dataloader = data
     else:
         if batch_size is None:
             raise ValueError("Please specify a value for batch_size.")
         dataset = make_dataset(data)
+
+        if filter_invalid_data:
+            dataset = filter_dataset(dataset)
+
         dataloader = DataLoader(
             dataset, batch_size=batch_size, num_workers=num_workers, shuffle=shuffle
         )
     return dataloader
 
 def make_default_dataloaders(
     data: TensorDictLike,
     valid_data: Optional[TensorDictLike] = None,
     valid_percentage: float = 0.1,
     batch_size: Optional[int] = None,
+    filter_invalid_data: bool = True,
     num_workers: int = 0,
 ) -> Tuple[DataLoader, Optional[DataLoader]]:
     # Make the datasets if necessary
     if is_data_loader(data):
         train_loader = data
         train_set = data.dataset
         batch_size = data.batch_size
         num_workers = data.num_workers
     else:
         if batch_size is None:
             raise ValueError("Please specify a value for batch_size.")
         train_set = make_dataset(data)
         train_loader = None
 
+    # Filter out NaNs
+    if filter_invalid_data:
+        train_set = filter_dataset(train_set)
+
     if valid_data is None:
         valid_set = None
         valid_loader = None
     elif is_data_loader(valid_data):
         valid_loader = valid_data
         valid_set = None
     else:
         valid_set = make_dataset(valid_data)
         valid_loader = None
 
+    if valid_set and filter_invalid_data:
+        valid_set = filter_dataset(valid_set)
+
     # Create a validation set if specified
     if valid_percentage > 0:
         if valid_set is None and valid_loader is None:
             # Make a random train/valid split
             n_valid = int(len(train_set) * valid_percentage)
             train_set, valid_set = random_split(
                 train_set, [len(train_set) - n_valid, n_valid]
```

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/evaluation/mi_estimator.py` & `torch_mist-0.2.8/src/torch_mist/utils/evaluation/mi_estimator.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/evaluation/model.py` & `torch_mist-0.2.8/src/torch_mist/utils/evaluation/model.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/freeze.py` & `torch_mist-0.2.8/src/torch_mist/utils/freeze.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/indexing.py` & `torch_mist-0.2.8/src/torch_mist/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/logging/logger/base.py` & `torch_mist-0.2.8/src/torch_mist/utils/logging/logger/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,12 +249,12 @@
     @abstractmethod
     def save_model(self, model: nn.Module, name: str):
         filepath = os.path.join(self.log_dir, name)
         torch.save(model, filepath)
 
 
 class DummyLogger(Logger):
-    def _log(self, **kwargs):
+    def _log(self, data: Any, name: str, iteration: int, epoch: int, split: str):
         pass
 
     def _reset_log(self):
         pass
```

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/logging/logger/pandas.py` & `torch_mist-0.2.8/src/torch_mist/utils/logging/logger/pandas.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/logging/logger/wandb.py` & `torch_mist-0.2.8/src/torch_mist/utils/logging/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/logging/metrics.py` & `torch_mist-0.2.8/src/torch_mist/utils/logging/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/shape.py` & `torch_mist-0.2.8/src/torch_mist/utils/shape.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/train/mi_estimator.py` & `torch_mist-0.2.8/src/torch_mist/utils/train/mi_estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     num_workers: int = 0,
     device: Union[torch.device, str] = torch.device("cpu"),
     max_epochs: Optional[int] = None,
     max_iterations: Optional[int] = None,
     optimizer_class: Type[Optimizer] = Adam,
     optimizer_params: Optional[Dict[str, Any]] = None,
     lr_annealing: bool = False,
-    warmup_percentage: float = 0.2,
+    warmup_percentage: float = 0,
     verbose: bool = True,
     logger: Optional[Union[Logger, bool]] = None,
     early_stopping: bool = False,
-    patience: int = 5,
+    patience: Optional[int] = None,
     tolerance: float = 0.001,
     fast_train: bool = False,
     train_logged_methods: Optional[
         List[Union[str, Tuple[str, Callable]]]
     ] = None,
     eval_logged_methods: Optional[
         List[Union[str, Tuple[str, Callable]]]
```

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/train/model.py` & `torch_mist-0.2.8/src/torch_mist/utils/train/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -221,19 +221,19 @@
     num_workers: int = 0,
     device: Union[torch.device, str] = torch.device("cpu"),
     max_epochs: Optional[int] = None,
     max_iterations: Optional[int] = None,
     optimizer_class: Type[Optimizer] = Adam,
     optimizer_params: Optional[Dict[str, Any]] = None,
     lr_annealing: bool = False,
-    warmup_percentage: float = 0.2,
+    warmup_percentage: float = 0,
     verbose: bool = True,
     logger: Optional[Union[Logger, bool]] = None,
     early_stopping: bool = False,
-    patience: int = 5,
+    patience: Optional[int] = None,
     tolerance: float = 0.001,
     fast_train: bool = False,
     train_logged_methods: Optional[
         List[Union[str, Tuple[str, Callable]]]
     ] = None,
     eval_logged_methods: Optional[
         List[Union[str, Tuple[str, Callable]]]
@@ -260,14 +260,23 @@
     max_epochs, max_iterations, warmup_iterations = compute_training_time(
         iterations_per_epoch=len(train_loader),
         max_epochs=max_epochs,
         max_iterations=max_iterations,
         warmup_percentage=warmup_percentage,
     )
 
+    if patience is None:
+        patience = int(max_epochs*0.02)
+        if patience < 1:
+            patience = 1
+
+        print(
+            f"[Info]: patience is not specified, using patience={patience} (~2% of training epochs) by default."
+        )
+
     # Instantiate the optimizer and lr_scheduler
     opt, lr_scheduler = instantiate_optimizer(
         model=model,
         optimizer_class=optimizer_class,
         optimizer_params=optimizer_params,
         lr_annealing=lr_annealing,
         warmup_iterations=warmup_iterations,
@@ -350,14 +359,20 @@
 
         # Determine if the training is over
         if run_manager.should_stop(
             iteration=logger._iteration, score=valid_score, model=model
         ):
             break
 
+    if early_stopping and run_manager.current_patience > 0:
+        print(
+            "[Warning]: The train procedure ended since max_epoch or max_iteration has been reached."+
+            "Consider increasing the training time by specifying larger values of max_epochs or max_iterations."
+        )
+
     # Obtain the training log
     log = logger.get_log()
 
     # Load the state dictionary for the best score.
     # This works only if early_stopping is enabled
     run_manager.load_best_weights(model)
```

### Comparing `torch_mist-0.2.7/src/torch_mist/utils/train/utils.py` & `torch_mist-0.2.8/src/torch_mist/utils/train/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.2.7/PKG-INFO` & `torch_mist-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-mist
-Version: 0.2.7
+Version: 0.2.8
 Summary: Mutual Information Estimation toolkit based on pytorch
 License: MIT
 Author: Marco Federici
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

