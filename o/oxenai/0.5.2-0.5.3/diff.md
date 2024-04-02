# Comparing `tmp/oxenai-0.5.2.tar.gz` & `tmp/oxenai-0.5.3.tar.gz`

## Comparing `oxenai-0.5.2.tar` & `oxenai-0.5.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 oxenai-0.5.2/Cargo.toml
--rw-r--r--   0     1001      127      687 2024-01-23 05:14:59.000000 oxenai-0.5.2/.gitignore
--rw-r--r--   0     1001      127     1255 2024-01-23 05:14:59.000000 oxenai-0.5.2/Develop.md
--rw-r--r--   0     1001      127     1840 2024-01-23 05:14:59.000000 oxenai-0.5.2/README.md
--rw-r--r--   0     1001      127       18 2024-01-23 05:14:59.000000 oxenai-0.5.2/annotations/annotations/labels.txt
--rw-r--r--   0     1001      127       94 2024-01-23 05:14:59.000000 oxenai-0.5.2/annotations/annotations/test.csv
--rw-r--r--   0     1001      127      114 2024-01-23 05:14:59.000000 oxenai-0.5.2/annotations/annotations/train.csv
--rw-r--r--   0     1001      127      717 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/__init__.py
--rw-r--r--   0     1001      127     1387 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/auth.py
--rw-r--r--   0     1001      127     1605 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/clone.py
--rw-r--r--   0     1001      127      746 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/dag.py
--rw-r--r--   0     1001      127     7411 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/dataset.py
--rw-r--r--   0     1001      127     1378 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/features.py
--rw-r--r--   0     1001      127     1500 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/fs.py
--rw-r--r--   0     1001      127      446 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/init.py
--rw-r--r--   0     1001      127      259 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/loaders/__init__.py
--rw-r--r--   0     1001      127     1713 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/loaders/chat.py
--rw-r--r--   0     1001      127     3276 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/loaders/image_classification.py
--rw-r--r--   0     1001      127     1586 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/loaders/regression.py
--rw-r--r--   0     1001      127     6126 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/local_repo.py
--rw-r--r--   0     1001      127     1543 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/op.py
--rw-r--r--   0     1001      127      638 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/__init__.py
--rw-r--r--   0     1001      127      207 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/concat_series.py
--rw-r--r--   0     1001      127      875 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/create_label_map.py
--rw-r--r--   0     1001      127      494 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/encode_labels.py
--rw-r--r--   0     1001      127      440 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/extract_col.py
--rw-r--r--   0     1001      127      214 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/identity.py
--rw-r--r--   0     1001      127      361 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/read_df.py
--rw-r--r--   0     1001      127      792 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/read_image_dir.py
--rw-r--r--   0     1001      127      347 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/read_text.py
--rw-r--r--   0     1001      127     3723 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/resize_images.py
--rw-r--r--   0     1001      127      354 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/ops/str_col_template.py
--rw-r--r--   0     1001      127        0 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/providers/__init__.py
--rw-r--r--   0     1001      127      674 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/providers/dataset_path_provider.py
--rw-r--r--   0     1001      127     2048 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/providers/mock_provider.py
--rw-r--r--   0     1001      127     1593 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/providers/oxen_data_frame_provider.py
--rw-r--r--   0     1001      127    11211 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/remote_repo.py
--rw-r--r--   0     1001      127     7978 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/streaming_dataset.py
--rw-r--r--   0     1001      127     1165 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/user.py
--rw-r--r--   0     1001      127        0 2024-01-23 05:14:59.000000 oxenai-0.5.2/python/oxen/util/__init__.py
--rw-r--r--   0     1001      127      221 2024-01-23 05:14:59.000000 oxenai-0.5.2/requirements.txt
--rw-r--r--   0     1001      127      711 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/auth.rs
--rw-r--r--   0     1001      127      370 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/error.rs
--rw-r--r--   0     1001      127     2768 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/lib.rs
--rw-r--r--   0     1001      127      934 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_branch.rs
--rw-r--r--   0     1001      127     1233 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_commit.rs
--rw-r--r--   0     1001      127      474 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_dataset.rs
--rw-r--r--   0     1001      127      684 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_diff.rs
--rw-r--r--   0     1001      127      953 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_entry.rs
--rw-r--r--   0     1001      127     4927 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_local_repo.rs
--rw-r--r--   0     1001      127     2440 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_paginated_dir_entries.rs
--rw-r--r--   0     1001      127    12670 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_remote_repo.rs
--rw-r--r--   0     1001      127     2432 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_staged_data.rs
--rw-r--r--   0     1001      127      818 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/py_user.rs
--rw-r--r--   0     1001      127     2601 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/remote.rs
--rw-r--r--   0     1001      127      680 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/user.rs
--rw-r--r--   0     1001      127      750 2024-01-23 05:14:59.000000 oxenai-0.5.2/src/util.rs
--rw-r--r--   0     1001      127      345 2024-01-23 05:14:59.000000 oxenai-0.5.2/test.py
--rw-r--r--   0     1001      127        0 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/__init__.py
--rw-r--r--   0     1001      127     3476 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/conftest.py
--rw-r--r--   0     1001      127       18 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/annotations/labels.txt
--rw-r--r--   0     1001      127       94 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/annotations/test.csv
--rw-r--r--   0     1001      127      114 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/annotations/train.csv
--rw-r--r--   0     1001      127    11440 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/1.jpg
--rw-r--r--   0     1001      127     7448 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/2.jpg
--rw-r--r--   0     1001      127     4253 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/3.jpg
--rw-r--r--   0     1001      127    10747 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/4.jpg
--rw-r--r--   0     1001      127     6351 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/5.jpg
--rw-r--r--   0     1001      127     8073 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/6.jpg
--rw-r--r--   0     1001      127     8203 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/7.jpg
--rw-r--r--   0     1001      127     7725 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/8.jpg
--rw-r--r--   0     1001      127     8641 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/CelebA/images/9.jpg
--rw-r--r--   0     1001      127      337 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/ChatBot/examples.tsv
--rw-r--r--   0     1001      127       88 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/ChatBot/prompt.txt
--rw-r--r--   0     1001      127      148 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/data/HousePrices/prices.csv
--rw-r--r--   0     1001      127      516 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_add.py
--rw-r--r--   0     1001      127     1300 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_auth.py
--rw-r--r--   0     1001      127      363 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_chat_loader.py
--rw-r--r--   0     1001      127     1299 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_checkout.py
--rw-r--r--   0     1001      127      711 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_clone.py
--rw-r--r--   0     1001      127      850 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_commit.py
--rw-r--r--   0     1001      127     2444 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_dataloader_pytorch.py
--rw-r--r--   0     1001      127     1558 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_dataset.py
--rw-r--r--   0     1001      127      694 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_download.py
--rw-r--r--   0     1001      127     4872 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_image_classification_loader.py
--rw-r--r--   0     1001      127      338 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_init.py
--rw-r--r--   0     1001      127      441 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_push.py
--rw-r--r--   0     1001      127      912 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_push_pull.py
--rw-r--r--   0     1001      127      537 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_regression_loader.py
--rw-r--r--   0     1001      127      828 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_add.py
--rw-r--r--   0     1001      127      560 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_branch.py
--rw-r--r--   0     1001      127      538 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_checkout.py
--rw-r--r--   0     1001      127      685 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_commit.py
--rw-r--r--   0     1001      127     1473 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_df_add.py
--rw-r--r--   0     1001      127      530 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_list.py
--rw-r--r--   0     1001      127     1439 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_remove.py
--rw-r--r--   0     1001      127      114 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_repo.py
--rw-r--r--   0     1001      127      636 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_remote_status.py
--rw-r--r--   0     1001      127      259 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_status.py
--rw-r--r--   0     1001      127     2060 2024-01-23 05:14:59.000000 oxenai-0.5.2/tests/test_streaming_dataset.py
--rw-r--r--   0     1001      127   135429 2024-01-23 05:14:59.000000 oxenai-0.5.2/Cargo.lock
--rw-r--r--   0     1001      127      663 2024-01-23 05:14:59.000000 oxenai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 oxenai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 oxenai-0.5.3/Cargo.toml
+-rw-r--r--   0     1001      127      687 2024-01-24 00:29:57.000000 oxenai-0.5.3/.gitignore
+-rw-r--r--   0     1001      127     1255 2024-01-24 00:29:57.000000 oxenai-0.5.3/Develop.md
+-rw-r--r--   0     1001      127     1840 2024-01-24 00:29:57.000000 oxenai-0.5.3/README.md
+-rw-r--r--   0     1001      127       18 2024-01-24 00:29:57.000000 oxenai-0.5.3/annotations/annotations/labels.txt
+-rw-r--r--   0     1001      127       94 2024-01-24 00:29:57.000000 oxenai-0.5.3/annotations/annotations/test.csv
+-rw-r--r--   0     1001      127      114 2024-01-24 00:29:57.000000 oxenai-0.5.3/annotations/annotations/train.csv
+-rw-r--r--   0     1001      127      717 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/__init__.py
+-rw-r--r--   0     1001      127     1387 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/auth.py
+-rw-r--r--   0     1001      127     1605 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/clone.py
+-rw-r--r--   0     1001      127      746 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/dag.py
+-rw-r--r--   0     1001      127     7411 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/dataset.py
+-rw-r--r--   0     1001      127     1378 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/features.py
+-rw-r--r--   0     1001      127     1500 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/fs.py
+-rw-r--r--   0     1001      127      446 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/init.py
+-rw-r--r--   0     1001      127      259 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/loaders/__init__.py
+-rw-r--r--   0     1001      127     1713 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/loaders/chat.py
+-rw-r--r--   0     1001      127     3276 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/loaders/image_classification.py
+-rw-r--r--   0     1001      127     1586 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/loaders/regression.py
+-rw-r--r--   0     1001      127     6126 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/local_repo.py
+-rw-r--r--   0     1001      127     1543 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/op.py
+-rw-r--r--   0     1001      127      638 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/__init__.py
+-rw-r--r--   0     1001      127      207 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/concat_series.py
+-rw-r--r--   0     1001      127      875 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/create_label_map.py
+-rw-r--r--   0     1001      127      494 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/encode_labels.py
+-rw-r--r--   0     1001      127      440 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/extract_col.py
+-rw-r--r--   0     1001      127      214 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/identity.py
+-rw-r--r--   0     1001      127      361 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/read_df.py
+-rw-r--r--   0     1001      127      792 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/read_image_dir.py
+-rw-r--r--   0     1001      127      347 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/read_text.py
+-rw-r--r--   0     1001      127     3723 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/resize_images.py
+-rw-r--r--   0     1001      127      354 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/ops/str_col_template.py
+-rw-r--r--   0     1001      127        0 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/providers/__init__.py
+-rw-r--r--   0     1001      127      674 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/providers/dataset_path_provider.py
+-rw-r--r--   0     1001      127     2048 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/providers/mock_provider.py
+-rw-r--r--   0     1001      127     1593 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/providers/oxen_data_frame_provider.py
+-rw-r--r--   0     1001      127    11211 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/remote_repo.py
+-rw-r--r--   0     1001      127     7978 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/streaming_dataset.py
+-rw-r--r--   0     1001      127     1165 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/user.py
+-rw-r--r--   0     1001      127        0 2024-01-24 00:29:57.000000 oxenai-0.5.3/python/oxen/util/__init__.py
+-rw-r--r--   0     1001      127      221 2024-01-24 00:29:57.000000 oxenai-0.5.3/requirements.txt
+-rw-r--r--   0     1001      127      711 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/auth.rs
+-rw-r--r--   0     1001      127      370 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/error.rs
+-rw-r--r--   0     1001      127     2768 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/lib.rs
+-rw-r--r--   0     1001      127      934 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_branch.rs
+-rw-r--r--   0     1001      127     1233 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_commit.rs
+-rw-r--r--   0     1001      127      474 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_dataset.rs
+-rw-r--r--   0     1001      127      684 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_diff.rs
+-rw-r--r--   0     1001      127      953 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_entry.rs
+-rw-r--r--   0     1001      127     4927 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_local_repo.rs
+-rw-r--r--   0     1001      127     2440 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_paginated_dir_entries.rs
+-rw-r--r--   0     1001      127    12671 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_remote_repo.rs
+-rw-r--r--   0     1001      127     2432 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_staged_data.rs
+-rw-r--r--   0     1001      127      818 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/py_user.rs
+-rw-r--r--   0     1001      127     2601 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/remote.rs
+-rw-r--r--   0     1001      127      680 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/user.rs
+-rw-r--r--   0     1001      127      750 2024-01-24 00:29:57.000000 oxenai-0.5.3/src/util.rs
+-rw-r--r--   0     1001      127      345 2024-01-24 00:29:57.000000 oxenai-0.5.3/test.py
+-rw-r--r--   0     1001      127        0 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/__init__.py
+-rw-r--r--   0     1001      127     3476 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/conftest.py
+-rw-r--r--   0     1001      127       18 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/annotations/labels.txt
+-rw-r--r--   0     1001      127       94 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/annotations/test.csv
+-rw-r--r--   0     1001      127      114 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/annotations/train.csv
+-rw-r--r--   0     1001      127    11440 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/1.jpg
+-rw-r--r--   0     1001      127     7448 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/2.jpg
+-rw-r--r--   0     1001      127     4253 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/3.jpg
+-rw-r--r--   0     1001      127    10747 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/4.jpg
+-rw-r--r--   0     1001      127     6351 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/5.jpg
+-rw-r--r--   0     1001      127     8073 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/6.jpg
+-rw-r--r--   0     1001      127     8203 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/7.jpg
+-rw-r--r--   0     1001      127     7725 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/8.jpg
+-rw-r--r--   0     1001      127     8641 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/CelebA/images/9.jpg
+-rw-r--r--   0     1001      127      337 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/ChatBot/examples.tsv
+-rw-r--r--   0     1001      127       88 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/ChatBot/prompt.txt
+-rw-r--r--   0     1001      127      148 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/data/HousePrices/prices.csv
+-rw-r--r--   0     1001      127      516 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_add.py
+-rw-r--r--   0     1001      127     1300 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_auth.py
+-rw-r--r--   0     1001      127      363 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_chat_loader.py
+-rw-r--r--   0     1001      127     1299 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_checkout.py
+-rw-r--r--   0     1001      127      711 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_clone.py
+-rw-r--r--   0     1001      127      850 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_commit.py
+-rw-r--r--   0     1001      127     2444 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_dataloader_pytorch.py
+-rw-r--r--   0     1001      127     1558 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_dataset.py
+-rw-r--r--   0     1001      127      694 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_download.py
+-rw-r--r--   0     1001      127     4872 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_image_classification_loader.py
+-rw-r--r--   0     1001      127      338 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_init.py
+-rw-r--r--   0     1001      127      441 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_push.py
+-rw-r--r--   0     1001      127      912 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_push_pull.py
+-rw-r--r--   0     1001      127      537 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_regression_loader.py
+-rw-r--r--   0     1001      127      828 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_add.py
+-rw-r--r--   0     1001      127      560 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_branch.py
+-rw-r--r--   0     1001      127      538 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_checkout.py
+-rw-r--r--   0     1001      127      685 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_commit.py
+-rw-r--r--   0     1001      127     1473 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_df_add.py
+-rw-r--r--   0     1001      127      530 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_list.py
+-rw-r--r--   0     1001      127     1439 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_remove.py
+-rw-r--r--   0     1001      127      114 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_repo.py
+-rw-r--r--   0     1001      127      636 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_remote_status.py
+-rw-r--r--   0     1001      127      259 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_status.py
+-rw-r--r--   0     1001      127     2060 2024-01-24 00:29:57.000000 oxenai-0.5.3/tests/test_streaming_dataset.py
+-rw-r--r--   0     1001      127   135429 2024-01-24 00:29:57.000000 oxenai-0.5.3/Cargo.lock
+-rw-r--r--   0     1001      127      663 2024-01-24 00:29:57.000000 oxenai-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 oxenai-0.5.3/PKG-INFO
```

### Comparing `oxenai-0.5.2/Cargo.toml` & `oxenai-0.5.3/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "oxen"
-version = "0.5.2"
+version = "0.5.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "oxen"
 crate-type = ["cdylib"]
 
@@ -12,15 +12,15 @@
 pyo3 = "0.20.0"
 pyo3-asyncio = { version = "0.20.0", features = ["attributes", "tokio-runtime"] }
 log = "0.4.17"
 pyo3-log = "0.9.0"
 tokio = { version = "1", features = ["full"] }
 pyo3-polars = "0.9.0"
 serde_json = "1.0.106"
-liboxen = "0.10.7"
+liboxen = "0.10.9"
 # liboxen = { path = "../../rust/Oxen/src/lib" }
 
 [build-dependencies]
 cc = { version = "1.0", features = ["parallel"] }
 bindgen = { version = "0.69.1", default-features = false, features = ["runtime"] }
 glob = "0.3"
 pkg-config = { version = "0.3", optional = true }
```

### Comparing `oxenai-0.5.2/.gitignore` & `oxenai-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/Develop.md` & `oxenai-0.5.3/Develop.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/README.md` & `oxenai-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/__init__.py` & `oxenai-0.5.3/python/oxen/__init__.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/auth.py` & `oxenai-0.5.3/python/oxen/auth.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/clone.py` & `oxenai-0.5.3/python/oxen/clone.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/dag.py` & `oxenai-0.5.3/python/oxen/dag.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/dataset.py` & `oxenai-0.5.3/python/oxen/dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/features.py` & `oxenai-0.5.3/python/oxen/features.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/fs.py` & `oxenai-0.5.3/python/oxen/fs.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/loaders/chat.py` & `oxenai-0.5.3/python/oxen/loaders/chat.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/loaders/image_classification.py` & `oxenai-0.5.3/python/oxen/loaders/image_classification.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/loaders/regression.py` & `oxenai-0.5.3/python/oxen/loaders/regression.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/local_repo.py` & `oxenai-0.5.3/python/oxen/local_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/op.py` & `oxenai-0.5.3/python/oxen/op.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/ops/__init__.py` & `oxenai-0.5.3/python/oxen/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/ops/create_label_map.py` & `oxenai-0.5.3/python/oxen/ops/create_label_map.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/ops/read_image_dir.py` & `oxenai-0.5.3/python/oxen/ops/read_image_dir.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/ops/resize_images.py` & `oxenai-0.5.3/python/oxen/ops/resize_images.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/providers/dataset_path_provider.py` & `oxenai-0.5.3/python/oxen/providers/dataset_path_provider.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/providers/mock_provider.py` & `oxenai-0.5.3/python/oxen/providers/mock_provider.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/providers/oxen_data_frame_provider.py` & `oxenai-0.5.3/python/oxen/providers/oxen_data_frame_provider.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/remote_repo.py` & `oxenai-0.5.3/python/oxen/remote_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/streaming_dataset.py` & `oxenai-0.5.3/python/oxen/streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/python/oxen/user.py` & `oxenai-0.5.3/python/oxen/user.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/auth.rs` & `oxenai-0.5.3/src/auth.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/lib.rs` & `oxenai-0.5.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_branch.rs` & `oxenai-0.5.3/src/py_branch.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_commit.rs` & `oxenai-0.5.3/src/py_commit.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_diff.rs` & `oxenai-0.5.3/src/py_diff.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_entry.rs` & `oxenai-0.5.3/src/py_entry.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_local_repo.rs` & `oxenai-0.5.3/src/py_local_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_paginated_dir_entries.rs` & `oxenai-0.5.3/src/py_paginated_dir_entries.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_remote_repo.rs` & `oxenai-0.5.3/src/py_remote_repo.rs`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,15 @@
         });
 
         match branch {
             Ok(branch) => Ok(PyBranch::from(branch)),
             _ => Err(PyValueError::new_err("Could not get or create branch")),
         }
     }
+
     fn checkout(&mut self, revision: String) -> PyResult<()> {
         let branch = self.get_branch(revision.clone());
         if let Ok(branch) = branch {
             self.set_revision(branch.name().to_string());
             return Ok(());
         }
```

### Comparing `oxenai-0.5.2/src/py_staged_data.rs` & `oxenai-0.5.3/src/py_staged_data.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/py_user.rs` & `oxenai-0.5.3/src/py_user.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/remote.rs` & `oxenai-0.5.3/src/remote.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/user.rs` & `oxenai-0.5.3/src/user.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/src/util.rs` & `oxenai-0.5.3/src/util.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/conftest.py` & `oxenai-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/1.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/1.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/2.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/2.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/3.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/3.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/4.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/4.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/5.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/5.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/6.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/6.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/7.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/7.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/8.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/8.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/data/CelebA/images/9.jpg` & `oxenai-0.5.3/tests/data/CelebA/images/9.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_add.py` & `oxenai-0.5.3/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_auth.py` & `oxenai-0.5.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_checkout.py` & `oxenai-0.5.3/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_clone.py` & `oxenai-0.5.3/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_commit.py` & `oxenai-0.5.3/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_dataloader_pytorch.py` & `oxenai-0.5.3/tests/test_dataloader_pytorch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_dataset.py` & `oxenai-0.5.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_download.py` & `oxenai-0.5.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_image_classification_loader.py` & `oxenai-0.5.3/tests/test_image_classification_loader.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_push_pull.py` & `oxenai-0.5.3/tests/test_push_pull.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_regression_loader.py` & `oxenai-0.5.3/tests/test_regression_loader.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_add.py` & `oxenai-0.5.3/tests/test_remote_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_branch.py` & `oxenai-0.5.3/tests/test_remote_branch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_checkout.py` & `oxenai-0.5.3/tests/test_remote_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_commit.py` & `oxenai-0.5.3/tests/test_remote_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_df_add.py` & `oxenai-0.5.3/tests/test_remote_df_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_list.py` & `oxenai-0.5.3/tests/test_remote_list.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_remove.py` & `oxenai-0.5.3/tests/test_remote_remove.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_remote_status.py` & `oxenai-0.5.3/tests/test_remote_status.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/tests/test_streaming_dataset.py` & `oxenai-0.5.3/tests/test_streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/Cargo.lock` & `oxenai-0.5.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2540,17 +2540,17 @@
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "liboxen"
-version = "0.10.7"
+version = "0.10.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a735fab8cac63199a753f73664d67ff6ae42ea5044c0e3b0f154da4e91da17c"
+checksum = "1026fd0dc5b2211b203667df9e2bbbdc7588ae698d4c4b2e706d80340ed46948"
 dependencies = [
  "actix-files",
  "actix-web",
  "approx",
  "arrow-json",
  "async-compression",
  "async-recursion",
@@ -3094,15 +3094,15 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "oxen"
-version = "0.5.2"
+version = "0.5.3"
 dependencies = [
  "bindgen 0.69.1",
  "cc",
  "glob",
  "liboxen",
  "log",
  "pkg-config",
```

### Comparing `oxenai-0.5.2/pyproject.toml` & `oxenai-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oxenai-0.5.2/PKG-INFO` & `oxenai-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxenai
-Version: 0.5.2
+Version: 0.5.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas ==2.0.1
 Requires-Dist: polars ==0.17.11
 Requires-Dist: pyarrow ==12.0.0
 Requires-Dist: opencv-python-headless ==4.7.0.72
```

