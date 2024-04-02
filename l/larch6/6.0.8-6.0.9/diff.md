# Comparing `tmp/larch6-6.0.8.tar.gz` & `tmp/larch6-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "larch6-6.0.8.tar", last modified: Thu Jan 18 22:38:06 2024, max compression
+gzip compressed data, was "larch6-6.0.9.tar", last modified: Fri Jan 19 17:39:09 2024, max compression
```

## Comparing `larch6-6.0.8.tar` & `larch6-6.0.9.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.301746 larch6-6.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 22:37:58.000000 larch6-6.0.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.257746 larch6-6.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.265746 larch6-6.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-18 22:37:58.000000 larch6-6.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-18 22:37:58.000000 larch6-6.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-01-18 22:37:58.000000 larch6-6.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.265746 larch6-6.0.8/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.265746 larch6-6.0.8/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/larix.iml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-18 22:37:58.000000 larch6-6.0.8/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-18 22:37:58.000000 larch6-6.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-18 22:37:58.000000 larch6-6.0.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-01-18 22:37:58.000000 larch6-6.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-18 22:38:06.301746 larch6-6.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-01-18 22:37:58.000000 larch6-6.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.265746 larch6-6.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_build.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.265746 larch6-6.0.8/docs/_img/
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_img/larch-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_img/larch_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.265746 larch6-6.0.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_scripts/developer_doc_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_scripts/hide_test_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.269746 larch6-6.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/dataset.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/datatree.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/linear.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/nesting.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/~data.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/api/~models.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.261746 larch6-6.0.8/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.269746 larch6-6.0.8/docs/examples/exampville/
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/200_exampville.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36940 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/201_exville_mode_choice.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/202_exville_mc_logsums.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20053 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/203_exville_dest.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/204_exville_dest_only.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/251_bySpec.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/exampville/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.269746 larch6-6.0.8/docs/examples/mtc/
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/mtc/001_mnl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/mtc/017_mnl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/mtc/022_nl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/mtc/030_mnl_constrain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/mtc/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.273746 larch6-6.0.8/docs/examples/swissmetro/
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/swissmetro/101_swissmetro_mnl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/swissmetro/102-swissmetro-weighted.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/swissmetro/109-swissmetro-nl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/swissmetro/151-swissmetro-panel-latent-class.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.273746 larch6-6.0.8/docs/examples/xlogit-artificial/
--rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/examples/xlogit-artificial/xlogit-test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/switcher.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.273746 larch6-6.0.8/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)    30131 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/choice-models.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23024 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/data-fundamentals.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.273746 larch6-6.0.8/docs/user-guide/example-data/
--rw-r--r--   0 runner    (1001) docker     (127)    24954 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/example-data/exampville_skims.csv
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/example-data/tiny_idca.csv
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/example-data/tiny_idco.csv
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/example-data/tiny_points.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33192 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/larch-demo-xlsx.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-01-18 22:37:58.000000 larch6-6.0.8/docs/user-guide/linear-funcs.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.273746 larch6-6.0.8/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-18 22:37:58.000000 larch6-6.0.8/envs/arboretum.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-18 22:37:58.000000 larch6-6.0.8/envs/colab-like.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-18 22:37:58.000000 larch6-6.0.8/envs/development.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-18 22:37:58.000000 larch6-6.0.8/envs/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-18 22:37:58.000000 larch6-6.0.8/envs/windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-18 22:37:58.000000 larch6-6.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.277746 larch6-6.0.8/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/201_exville_mode_choice.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/MTC-JAX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/Untitled.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/Untitled1.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/accesssor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/latent-class-panel.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18835 2024-01-18 22:37:58.000000 larch6-6.0.8/sandbox/sand.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 22:38:06.301746 larch6-6.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.261746 larch6-6.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.277746 larch6-6.0.8/src/larch/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-18 22:38:06.000000 larch6-6.0.8/src/larch/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/compiled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.281746 larch6-6.0.8/src/larch/data_warehouse/
--rw-r--r--   0 runner    (1001) docker     (127)   375578 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/MTCwork.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   127303 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/artificial_long.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_demographics.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_employment.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   124738 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_households.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   100624 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_persons.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   126202 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_skims.omx
--rw-r--r--   0 runner    (1001) docker     (127)    44886 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_taz.zip
--rw-r--r--   0 runner    (1001) docker     (127)   145928 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/exampville_tours.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   236115 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/itinerary_data.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   117449 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/data_warehouse/swissmetro.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.281746 larch6-6.0.8/src/larch/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/dataset/choice_avail_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/dataset/construct.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/dataset/dim_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    20046 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/dataset/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/dataset/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/datastats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.281746 larch6-6.0.8/src/larch/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.285746 larch6-6.0.8/src/larch/examples/generated/
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_001_mnl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_017_mnl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_022_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_030_mnl_constrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_101_swissmetro_mnl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_102_swissmetro_weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_109_swissmetro_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_151_swissmetro_panel_latent_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_200_exampville.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_201_exville_mode_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_202_exville_mc_logsums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_203_exville_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_204_exville_dest_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_251_bySpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/examples/generated/_xlogit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/folding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.285746 larch6-6.0.8/src/larch/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/logging/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.289746 larch6-6.0.8/src/larch/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56715 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/cascading.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22215 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/draws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/fast_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/from_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/jaxmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    29891 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/latent_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    62678 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/linear_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/mixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/numba_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    23410 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/numba_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    88408 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/numbamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    18905 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/param_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/persist_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/single_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    44493 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/model/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    50334 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/omx.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    81526 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/shorts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.297746 larch6-6.0.8/src/larch/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3100 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.301746 larch6-6.0.8/src/larch/util/activitysim/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/auto_ownership.py
--rw-r--r--   0 runner    (1001) docker     (127)    14544 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/cdap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/data_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/location_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/nonmand_tour_freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/activitysim/tour_mode_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/addict_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/arraytools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/aster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/bitmasking.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/bounded_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/cache_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/colors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3363 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/counting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14265 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/data_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/data_manipulation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15057 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    30771 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    50002 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/figures.py
--rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/histograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/html_table_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)    48092 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/interface_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/multiindex.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/overspec_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/png.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/signal_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/smartread.py
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/temporaryfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/text_manip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/timesize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/touch_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/uid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/visual_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/xhtml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/yaml_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/util/zipdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-18 22:37:58.000000 larch6-6.0.8/src/larch/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.301746 larch6-6.0.8/src/larch6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-18 22:38:06.000000 larch6-6.0.8/src/larch6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-01-18 22:38:06.000000 larch6-6.0.8/src/larch6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 22:38:06.000000 larch6-6.0.8/src/larch6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-18 22:38:06.000000 larch6-6.0.8/src/larch6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-18 22:38:06.000000 larch6-6.0.8/src/larch6.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.301746 larch6-6.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-01-18 22:37:58.000000 larch6-6.0.8/tests/test_exampville.py
--rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-01-18 22:37:58.000000 larch6-6.0.8/tests/test_jax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-18 22:37:58.000000 larch6-6.0.8/tests/test_latent_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-01-18 22:37:58.000000 larch6-6.0.8/tests/test_mtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-01-18 22:37:58.000000 larch6-6.0.8/tests/test_swissmetro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:38:06.301746 larch6-6.0.8/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-01-18 22:37:58.000000 larch6-6.0.8/tools/rip_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.680827 larch6-6.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 17:39:01.000000 larch6-6.0.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.636827 larch6-6.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.640827 larch6-6.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-19 17:39:01.000000 larch6-6.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-19 17:39:01.000000 larch6-6.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-01-19 17:39:01.000000 larch6-6.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.640827 larch6-6.0.9/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.640827 larch6-6.0.9/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/larix.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-19 17:39:01.000000 larch6-6.0.9/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-19 17:39:01.000000 larch6-6.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-01-19 17:39:01.000000 larch6-6.0.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-01-19 17:39:01.000000 larch6-6.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-19 17:39:09.680827 larch6-6.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-01-19 17:39:01.000000 larch6-6.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.644827 larch6-6.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.644827 larch6-6.0.9/docs/_img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_img/larch-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_img/larch_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.644827 larch6-6.0.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_scripts/developer_doc_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_scripts/hide_test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.644827 larch6-6.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/datatree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/linear.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/nesting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/~data.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/api/~models.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.636827 larch6-6.0.9/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.648827 larch6-6.0.9/docs/examples/exampville/
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/200_exampville.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36940 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/201_exville_mode_choice.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/202_exville_mc_logsums.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20053 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/203_exville_dest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26593 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/204_exville_dest_only.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/251_bySpec.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/exampville/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.648827 larch6-6.0.9/docs/examples/mtc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/mtc/001_mnl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/mtc/017_mnl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/mtc/022_nl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/mtc/030_mnl_constrain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/mtc/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.648827 larch6-6.0.9/docs/examples/swissmetro/
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/swissmetro/101_swissmetro_mnl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/swissmetro/102-swissmetro-weighted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/swissmetro/109-swissmetro-nl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/swissmetro/151-swissmetro-panel-latent-class.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.648827 larch6-6.0.9/docs/examples/xlogit-artificial/
+-rw-r--r--   0 runner    (1001) docker     (127)    14646 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/examples/xlogit-artificial/xlogit-test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/switcher.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.648827 larch6-6.0.9/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    30131 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/choice-models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23024 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/data-fundamentals.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.648827 larch6-6.0.9/docs/user-guide/example-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    24954 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/example-data/exampville_skims.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/example-data/tiny_idca.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/example-data/tiny_idco.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/example-data/tiny_points.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33192 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/larch-demo-xlsx.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-01-19 17:39:01.000000 larch6-6.0.9/docs/user-guide/linear-funcs.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.652827 larch6-6.0.9/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-19 17:39:01.000000 larch6-6.0.9/envs/arboretum.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-19 17:39:01.000000 larch6-6.0.9/envs/colab-like.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-19 17:39:01.000000 larch6-6.0.9/envs/development.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-19 17:39:01.000000 larch6-6.0.9/envs/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-19 17:39:01.000000 larch6-6.0.9/envs/windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-19 17:39:01.000000 larch6-6.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.652827 larch6-6.0.9/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/201_exville_mode_choice.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/MTC-JAX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/Untitled.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/Untitled1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/accesssor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/latent-class-panel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18835 2024-01-19 17:39:01.000000 larch6-6.0.9/sandbox/sand.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 17:39:09.680827 larch6-6.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.640827 larch6-6.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.652827 larch6-6.0.9/src/larch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-19 17:39:09.000000 larch6-6.0.9/src/larch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/compiled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.656827 larch6-6.0.9/src/larch/data_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (127)   375578 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/MTCwork.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   127303 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/artificial_long.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_demographics.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_employment.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   124738 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_households.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   100624 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_persons.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   126202 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_skims.omx
+-rw-r--r--   0 runner    (1001) docker     (127)    44886 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_taz.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   145928 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/exampville_tours.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   236115 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/itinerary_data.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   117449 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/data_warehouse/swissmetro.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.660827 larch6-6.0.9/src/larch/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/dataset/choice_avail_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/dataset/construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/dataset/dim_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/dataset/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/dataset/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/datastats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.660827 larch6-6.0.9/src/larch/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.660827 larch6-6.0.9/src/larch/examples/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_001_mnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_017_mnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_022_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_030_mnl_constrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_101_swissmetro_mnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_102_swissmetro_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_109_swissmetro_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_151_swissmetro_panel_latent_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_200_exampville.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_201_exville_mode_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_202_exville_mc_logsums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_203_exville_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_204_exville_dest_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_251_bySpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/examples/generated/_xlogit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/folding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.660827 larch6-6.0.9/src/larch/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/logging/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.668827 larch6-6.0.9/src/larch/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56974 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/cascading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22273 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/draws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/fast_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/from_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38978 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/jaxmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29891 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/latent_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62678 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/linear_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/mixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/numba_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23410 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/numba_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    88408 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/numbamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/param_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/persist_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/single_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44493 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/model/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50334 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/omx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81526 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/shorts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.676827 larch6-6.0.9/src/larch/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3100 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.676827 larch6-6.0.9/src/larch/util/activitysim/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/auto_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14544 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/cdap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/data_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/location_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/nonmand_tour_freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/activitysim/tour_mode_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/addict_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/arraytools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/aster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/bitmasking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/bounded_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/cache_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3363 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/counting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14265 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/data_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/data_manipulation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15057 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30771 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50002 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/figures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/html_table_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48092 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/interface_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/multiindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/overspec_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/png.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/signal_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/smartread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/temporaryfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/text_manip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/timesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/touch_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/visual_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/xhtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/yaml_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/util/zipdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-19 17:39:01.000000 larch6-6.0.9/src/larch/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.680827 larch6-6.0.9/src/larch6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-19 17:39:09.000000 larch6-6.0.9/src/larch6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-01-19 17:39:09.000000 larch6-6.0.9/src/larch6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 17:39:09.000000 larch6-6.0.9/src/larch6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-19 17:39:09.000000 larch6-6.0.9/src/larch6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-19 17:39:09.000000 larch6-6.0.9/src/larch6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.680827 larch6-6.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-01-19 17:39:01.000000 larch6-6.0.9/tests/test_exampville.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-01-19 17:39:01.000000 larch6-6.0.9/tests/test_jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-19 17:39:01.000000 larch6-6.0.9/tests/test_latent_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-01-19 17:39:01.000000 larch6-6.0.9/tests/test_mtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-01-19 17:39:01.000000 larch6-6.0.9/tests/test_swissmetro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 17:39:09.680827 larch6-6.0.9/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-01-19 17:39:01.000000 larch6-6.0.9/tools/rip_examples.py
```

### Comparing `larch6-6.0.8/.github/workflows/ci.yml` & `larch6-6.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/.gitignore` & `larch6-6.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/.idea/inspectionProfiles/Project_Default.xml` & `larch6-6.0.9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/.idea/larix.iml` & `larch6-6.0.9/.idea/larix.iml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/.pre-commit-config.yaml` & `larch6-6.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/Dockerfile` & `larch6-6.0.9/Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     openmatrix \
     zarr \
     geopandas \
     sharrow \
     && \
     micromamba clean --all --yes \
     && \
-    python -m pip install jax jaxlib xlogit --no-cache-dir
+    python -m pip install build jax jaxlib xlogit --no-cache-dir
 
 ENV PYTHONUNBUFFERED=1
 
 # Custom cache invalidation
 ARG CACHEBUST=1
 
 # copy the repo contents into the docker container
 COPY --chown=$MAMBA_USER:$MAMBA_USER . /tmp/larix/larch
 
 # Compile wheel
-RUN python -m pip wheel --wheel-dir=/tmp/wheelhouse --no-deps -v /tmp/larix/larch
+RUN python -m build --outdir=/tmp/wheelhouse /tmp/larix/larch
 
 # Install from wheel
-RUN python -m pip install --no-index --find-links=/tmp/wheelhouse larch
+RUN python -m pip install --no-index --find-links=/tmp/wheelhouse larch6
 
 # Run tests
 RUN python -m pytest -v /tmp/larix/larch --ignore=/tmp/larix/larch/sandbox
```

### Comparing `larch6-6.0.8/LICENSE` & `larch6-6.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/PKG-INFO` & `larch6-6.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: larch6
-Version: 6.0.8
+Version: 6.0.9
 Author-email: Jeff Newman <jeff@driftless.xyz>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.19
 Requires-Dist: pandas>=1.2
 Requires-Dist: pyarrow
 Requires-Dist: xarray
```

### Comparing `larch6-6.0.8/README.md` & `larch6-6.0.9/README.md`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/_config.yml` & `larch6-6.0.9/docs/_config.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Book settings
 # Learn more at https://jupyterbook.org/customize/config.html
 
 title: .
 author: Jeffrey Newman
 logo: _img/larch-logo.png
+copyright: "2024"  # Copyright year to be placed in the footer
 
 # Force re-execution of notebooks on each build.
 # See https://jupyterbook.org/content/execute.html
 execute:
   execute_notebooks: cache
   allow_errors: true
   timeout: 300 # 5 minutes per cell
@@ -19,15 +20,15 @@
 
 # Add a bibtex file so that we can create citations
 bibtex_bibfiles:
 - references.bib
 
 # Information about where the book exists on the web
 repository:
-  url: https://github.com/jpn--/larch  # Online location of your book
+  url: https://github.com/driftlesslabs/larch  # Online location of your book
   path_to_book: doc  # Optional path to your book, relative to the repository root
   branch: master  # Which branch of the repository should be used when creating links (optional)
 
 # Add GitHub buttons to your book
 # See https://jupyterbook.org/customize/config.html#add-a-link-to-your-repository
 html:
   favicon: _img/larch_favicon.png
@@ -82,23 +83,23 @@
     napoleon_use_rtype: false
     rst_epilog: |
       .. |idca| replace:: :ref:`idca <idca>`
       .. |idco| replace:: :ref:`idco <idco>`
     html_theme_options:
       home_page_in_toc: false
       search_bar_text: Search these docs...
-      repository_url: https://github.com/jpn--/larch
+      repository_url: https://github.com/driftlesslabs/larch
       use_repository_button: true
       use_issues_button: true
-      repository_branch: master
+      repository_branch: main
       path_to_docs: docs
-      extra_navbar:
       favicons:
       - rel: icon
         sizes: 32x32
         href: _img/larch_favicon.png
-      switcher:
-        json_url: https://larch.newman.me/switcher.json
-        url_template: https://larch.newman.me/v{version}/
-        version_match: 6.0.0
-      navbar_end:
-      - version-switcher
+#      switcher:
+#        json_url: https://larch.newman.me/switcher.json
+#        url_template: https://larch.newman.me/v{version}/
+#        version_match: 6.0.0
+#      navbar_end:
+#      - version-switcher
+      navigation_with_keys: true
```

### Comparing `larch6-6.0.8/docs/_img/larch-logo.png` & `larch6-6.0.9/docs/_img/larch-logo.png`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/_img/larch_favicon.png` & `larch6-6.0.9/docs/_img/larch_favicon.png`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/_scripts/hide_test_cells.py` & `larch6-6.0.9/docs/_scripts/hide_test_cells.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/_toc.yml` & `larch6-6.0.9/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/api/dataset.rst` & `larch6-6.0.9/docs/api/dataset.rst`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/api/datatree.rst` & `larch6-6.0.9/docs/api/datatree.rst`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/api/linear.rst` & `larch6-6.0.9/docs/api/linear.rst`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/api/model.rst` & `larch6-6.0.9/docs/api/model.rst`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/exampville/200_exampville.ipynb` & `larch6-6.0.9/docs/examples/exampville/200_exampville.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/exampville/201_exville_mode_choice.ipynb` & `larch6-6.0.9/docs/examples/exampville/201_exville_mode_choice.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/exampville/202_exville_mc_logsums.ipynb` & `larch6-6.0.9/docs/examples/exampville/202_exville_mc_logsums.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/exampville/203_exville_dest.ipynb` & `larch6-6.0.9/docs/examples/exampville/203_exville_dest.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/exampville/204_exville_dest_only.ipynb` & `larch6-6.0.9/docs/examples/exampville/204_exville_dest_only.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988486842105263%*

 * *Differences: {"'cells'": "{19: {'metadata': {'tags': ['remove_cell']}}, 24: {'metadata': {'tags': "*

 * *            "['remove_cell']}}, 30: {'metadata': {replace: OrderedDict([('tags', "*

 * *            "['remove_cell'])])}}, 31: {'metadata': {replace: OrderedDict([('tags', "*

 * *            "['remove_cell'])])}}, 51: {'metadata': {'tags': ['remove_cell']}}, 52: {'metadata': "*

 * *            "{'tags': ['remove_cell']}}, 54: {'metadata': {'tags': ['remove_cell']}}, 55: "*

 * *            "{'metadata': {'tags': ['remove_cell']}}, 56: {'metad […]*

```diff
@@ -310,15 +310,17 @@
                 "m.plock(EmpRetail_HighInc=0, EmpRetail_LowInc=0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.availability_any"
             ]
         },
@@ -382,15 +384,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 },
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.d_loglike() == approx([-223.95036, -682.1102, 0.0, 0.0, -7406.393, -34762.906])\n",
                 "assert mj.d_loglike() == approx(\n",
                 "    [-223.81805, -681.7803, 0.0, 0.0, -7406.3945, -34767.668], rel=1e-5\n",
@@ -514,15 +518,19 @@
                 "    rel=1e-2,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "mj.bhhh() == approx(\n",
                 "    np.asarray(\n",
                 "        [\n",
                 "            [\n",
@@ -577,15 +585,19 @@
                 "    )\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.bhhh() == approx(\n",
                 "    np.asarray(\n",
                 "        [\n",
                 "            [\n",
@@ -912,27 +924,31 @@
                 "mg.plock(EmpRetail_HighInc=0, EmpRetail_LowInc=0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert mg.loglike() == approx(-77777.17321427427)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert mg.d_loglike() == approx([-223.95016, -682.1102, 0, 0, -7406.389, -34762.91])"
             ]
         },
@@ -948,15 +964,17 @@
                 "result"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert result.loglike == approx(-70650.07578452416)\n",
                 "assert result.success\n",
                 "assert result.method == \"slsqp\"\n",
@@ -984,28 +1002,32 @@
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert mg.total_weight() == approx(20739.0)\n",
                 "assert mg.n_cases == 79"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert mg.bhhh() == approx(\n",
                 "    np.asarray(\n",
                 "        [\n",
```

### Comparing `larch6-6.0.8/docs/examples/exampville/251_bySpec.ipynb` & `larch6-6.0.9/docs/examples/exampville/251_bySpec.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/mtc/001_mnl.ipynb` & `larch6-6.0.9/docs/examples/mtc/001_mnl.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998204022988506%*

 * *Differences: {"'cells'": "{15: {'metadata': {'tags': ['remove_cell']}}}"}*

```diff
@@ -228,15 +228,17 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e056074c-22a1-469f-be9a-7b2b60a69a12",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "remove_cell"
+                ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "buffer = (\n",
                 "    b\"\\x80\\x05\\x95\\xc9\\x04\\x00\\x00\\x00\\x00\\x00\\x00\\x8c\\x11pandas.core.frame\\x94\\x8c\\tDataFrame\"\n",
                 "    b\"\\x94\\x93\\x94)\\x81\\x94}\\x94(\\x8c\\x04_mgr\\x94\\x8c\\x1epandas.core.internals.managers\\x94\\x8c\\x0c\"\n",
```

### Comparing `larch6-6.0.8/docs/examples/mtc/017_mnl.ipynb` & `larch6-6.0.9/docs/examples/mtc/017_mnl.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/mtc/022_nl.ipynb` & `larch6-6.0.9/docs/examples/mtc/022_nl.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/mtc/030_mnl_constrain.ipynb` & `larch6-6.0.9/docs/examples/mtc/030_mnl_constrain.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/mtc/index.md` & `larch6-6.0.9/docs/examples/mtc/index.md`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/examples/swissmetro/101_swissmetro_mnl.ipynb` & `larch6-6.0.9/docs/examples/swissmetro/101_swissmetro_mnl.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{29: {'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}}"}*

```diff
@@ -336,15 +336,19 @@
                 "m.parameter_summary()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "256df9cd",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.pvals == approx([-0.15475, -0.70178, -0.010842, -0.012776], rel=1e-3)\n",
                 "assert m.pstderr == approx([0.0432357, 0.0548783, 0.000518335, 0.000568829], rel=1e-3)\n",
                 "assert m.parameter_summary().data[\"t Stat\"].values.astype(float) == approx(\n",
                 "    [-3.58, -12.79, -20.92, -22.46], rel=1e-2\n",
```

### Comparing `larch6-6.0.8/docs/examples/swissmetro/102-swissmetro-weighted.ipynb` & `larch6-6.0.9/docs/examples/swissmetro/102-swissmetro-weighted.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991666666666666%*

 * *Differences: {"'cells'": "{22: {'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}, 24: "*

 * *            "{'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}}"}*

```diff
@@ -267,15 +267,19 @@
                 "m.parameter_summary()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d554d49b",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.pvals == approx(\n",
                 "    [-0.114834339145, -0.756969214206, -0.011197899961, -0.013210667574], rel=1e-2\n",
                 ")\n",
                 "assert m.pstderr == approx(\n",
@@ -297,15 +301,19 @@
                 "Looks good!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0674934c",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST numba\n",
                 "m.compute_engine = \"numba\"\n",
                 "m.pvals = 0\n",
                 "m.clear_cache()\n",
                 "assert m.loglike() == approx(-7892.111473285806)\n",
```

### Comparing `larch6-6.0.8/docs/examples/swissmetro/109-swissmetro-nl.ipynb` & `larch6-6.0.9/docs/examples/swissmetro/109-swissmetro-nl.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995471014492754%*

 * *Differences: {"'cells'": "{22: {'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}}"}*

```diff
@@ -272,15 +272,19 @@
                 "m.parameter_summary()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e7024c39",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.pstderr == approx(\n",
                 "    [0.037138242, 0.045185346, 0.00046280216, 0.00056991476, 0.027901005], rel=1e-2\n",
                 ")\n",
                 "assert m.parameter_summary().data[\"t Stat\"].values.astype(float) == approx(\n",
```

### Comparing `larch6-6.0.8/docs/examples/swissmetro/151-swissmetro-panel-latent-class.ipynb` & `larch6-6.0.9/docs/examples/swissmetro/151-swissmetro-panel-latent-class.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'cells'": "{19: {'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}, 20: "*

 * *            "{'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}, 24: {'metadata': "*

 * *            "{replace: OrderedDict([('tags', ['remove_cell'])])}}}"}*

```diff
@@ -233,26 +233,34 @@
                 "b.set_cap(25)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "04125570",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert b.loglike() == approx(-6867.245, rel=1e-4)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "289413f5",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert b.d_loglike() == approx(\n",
                 "    [\n",
                 "        -1.104770e02,\n",
                 "        -1.545916e03,\n",
@@ -296,15 +304,19 @@
                 "b.parameter_summary()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "81c1ee8b",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert result.loglike == approx(-4474.478515625, rel=1e-5)\n",
                 "assert b.pstderr == approx(\n",
                 "    np.array([0.048158, 0.069796, 0.069555, 0.106282, 0.161079, 0.11945, 0.0]), rel=5e-3\n",
                 ")\n",
```

### Comparing `larch6-6.0.8/docs/examples/xlogit-artificial/xlogit-test.ipynb` & `larch6-6.0.9/docs/examples/xlogit-artificial/xlogit-test.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987745098039216%*

 * *Differences: {"'cells'": "{6: {'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}, 7: "*

 * *            "{'metadata': {replace: OrderedDict([('tags', ['remove_cell'])])}}}"}*

```diff
@@ -106,15 +106,19 @@
                 "assert m.loglike() == approx(-4394.45556640625)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dd58ed70",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert m.d_loglike() == approx(\n",
                 "    [\n",
                 "        2.085461e03,\n",
                 "        -1.130608e03,\n",
@@ -134,15 +138,19 @@
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d1b5c104",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "remove_cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "se, hess, ihess = m.jax_param_cov(m.pvals)\n",
                 "assert hess == approx(\n",
                 "    np.array(\n",
                 "        [\n",
```

### Comparing `larch6-6.0.8/docs/user-guide/choice-models.ipynb` & `larch6-6.0.9/docs/user-guide/choice-models.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/user-guide/data-fundamentals.ipynb` & `larch6-6.0.9/docs/user-guide/data-fundamentals.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/user-guide/example-data/exampville_skims.csv` & `larch6-6.0.9/docs/user-guide/example-data/exampville_skims.csv`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/user-guide/larch-demo-xlsx.jpg` & `larch6-6.0.9/docs/user-guide/larch-demo-xlsx.jpg`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/docs/user-guide/linear-funcs.ipynb` & `larch6-6.0.9/docs/user-guide/linear-funcs.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/envs/colab-like.yaml` & `larch6-6.0.9/envs/colab-like.yaml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/envs/development.yaml` & `larch6-6.0.9/envs/development.yaml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/envs/testing.yml` & `larch6-6.0.9/envs/testing.yml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/envs/windows.yaml` & `larch6-6.0.9/envs/windows.yaml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/pyproject.toml` & `larch6-6.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/201_exville_mode_choice.ipynb` & `larch6-6.0.9/sandbox/201_exville_mode_choice.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/MTC-JAX.ipynb` & `larch6-6.0.9/sandbox/MTC-JAX.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/Untitled.ipynb` & `larch6-6.0.9/sandbox/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/Untitled1.ipynb` & `larch6-6.0.9/sandbox/Untitled1.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/accesssor.ipynb` & `larch6-6.0.9/sandbox/accesssor.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/latent-class-panel.ipynb` & `larch6-6.0.9/sandbox/latent-class-panel.ipynb`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/sandbox/sand.py` & `larch6-6.0.9/sandbox/sand.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/__init__.py` & `larch6-6.0.9/src/larch/__init__.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/_optional.py` & `larch6-6.0.9/src/larch/_optional.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 class Nothing:
     def __getattr__(self, name):
         return Nothing()
 
     def __call__(self, *args, **kwargs):
         return Nothing()
 
+    def __bool__(self):
+        return False
+
 
 # optional import: JAX
 try:
     import jax
     import jax.numpy as jnp
     import jax.scipy as js
 except ImportError:
```

### Comparing `larch6-6.0.8/src/larch/compiled.py` & `larch6-6.0.9/src/larch/compiled.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/MTCwork.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/MTCwork.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/artificial_long.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/artificial_long.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/exampville_demographics.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/exampville_demographics.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/exampville_households.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/exampville_households.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/exampville_persons.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/exampville_persons.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/exampville_skims.omx` & `larch6-6.0.9/src/larch/data_warehouse/exampville_skims.omx`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/exampville_taz.zip` & `larch6-6.0.9/src/larch/data_warehouse/exampville_taz.zip`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/exampville_tours.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/exampville_tours.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/itinerary_data.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/itinerary_data.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/data_warehouse/swissmetro.csv.gz` & `larch6-6.0.9/src/larch/data_warehouse/swissmetro.csv.gz`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/dataset/__init__.py` & `larch6-6.0.9/src/larch/dataset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,16 @@
             cache_dir=cache_dir,
             relationships=relationships,
             force_digitization=force_digitization,
             **kwargs,
         )
         dim_order = []
         c = self.root_dataset.dc.CASEID
-        if c is None and len(self.root_dataset.dims) == 1:
-            self.root_dataset.dc.CASEID = list(self.root_dataset.dims.keys())[0]
+        if c is None and len(self.root_dataset.sizes) == 1:
+            self.root_dataset.dc.CASEID = list(self.root_dataset.sizes.keys())[0]
         c = self.root_dataset.dc.CASEID
         if c is not None:
             dim_order.append(c)
         a = self.root_dataset.dc.ALTID
         if a is not None:
             dim_order.append(a)
         self.dim_order = tuple(dim_order)
@@ -231,20 +231,20 @@
         """Str : The _caseptr_ dimension of the root Dataset, if defined."""
         result = self.root_dataset.attrs.get(_CASEPTR, None)
         return result
 
     @property
     def n_cases(self):
         """Int : The size of the _caseid_ dimension of the root Dataset."""
-        return self.root_dataset.dims[self.CASEID]
+        return self.root_dataset.sizes[self.CASEID]
 
     @property
     def n_alts(self):
         """Int : The size of the _altid_ dimension of the root Dataset."""
-        return self.root_dataset.dims[self.ALTID]
+        return self.root_dataset.sizes[self.ALTID]
 
     def query_cases(self, *args, **kwargs):
         """
         Return a new DataTree, with a query filter applied to the root Dataset.
 
         Parameters
         ----------
```

### Comparing `larch6-6.0.8/src/larch/dataset/choice_avail_reporting.py` & `larch6-6.0.9/src/larch/dataset/choice_avail_reporting.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/dataset/construct.py` & `larch6-6.0.9/src/larch/dataset/construct.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 def _initialize_for_larch(obj, caseid=None, alts=None):
     """
     Initialize a Dataset for use with larch.
 
     Parameters
     ----------
     obj : Dataset
-        The dataaset being initialized.
+        The dataset being initialized.
     caseid : str, optional
         The name of a dimension referencing cases.
     alts : Mapping or str or array-like, optional
         If given as a mapping, links alternative codes to names.
         A string names a dimension that defines the alternatives.
         An array or list of integers gives codes for the alternatives,
         which are otherwise unnamed.
 
     Returns
     -------
     Dataset
     """
     if caseid is not None:
-        if caseid not in obj.dims:
+        if caseid not in obj.sizes:
             raise ValueError(f"no dim named '{caseid}' to make into {CASEID}")
         obj.attrs[CASEID] = caseid
     if isinstance(alts, pd.Series):
         alts_dim_name = alts.name or alts.index.name or "_altid_"
         alts_k = xr.DataArray(
             alts.index,
             dims=alts_dim_name,
```

### Comparing `larch6-6.0.8/src/larch/dataset/flow.py` & `larch6-6.0.9/src/larch/dataset/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         -------
         DataTree
         """
         from ..dataset import DataTree
 
         if self.CASEPTR is not None:
             case_index = case_ptr_to_indexes(
-                self._obj.dims[self.CASEALT], self[self.CASEPTR].values
+                self._obj.sizes[self.CASEALT], self[self.CASEPTR].values
             )
             obj = self._obj.assign(
                 {"_case_index_": xr.DataArray(case_index, dims=(self.CASEALT))}
             )
             tree = DataTree(**{label: obj.drop_dims(self.CASEID)})
             ds = obj.keep_dims(self.CASEID)
             ds.attrs.pop("_exclude_dims_", None)
@@ -340,40 +340,42 @@
             return dict(zip(a.values, a.coords["alt_names"].values))
         else:
             return dict(zip(a.values, a.values))
 
     @property
     def n_cases(self):
         try:
-            return self.dims[self.CASEID]
+            return self.sizes[self.CASEID]
         except KeyError:
             try:
-                return self.dims[self.GROUPID] * self.dims[self.INGROUP]
+                return self.sizes[self.GROUPID] * self.sizes[self.INGROUP]
             except KeyError:
                 pass
-            logging.getLogger().error(f"missing {self.CASEID!r} among dims {self.dims}")
+            logging.getLogger().error(
+                f"missing {self.CASEID!r} among dims {self.sizes}"
+            )
             raise
 
     @property
     def n_panels(self):
         try:
-            return self.dims[self.GROUPID]
+            return self.sizes[self.GROUPID]
         except KeyError:
             try:
-                return self.dims[self.CASEID]
+                return self.sizes[self.CASEID]
             except KeyError:
                 pass
             logging.getLogger().error(
-                f"missing {self.GROUPID!r} and {self.CASEID!r} among dims {self.dims}"
+                f"missing {self.GROUPID!r} and {self.CASEID!r} among dims {self.sizes}"
             )
             raise
 
     @property
     def n_in_panel(self):
-        return self.dims[self.INGROUP]
+        return self.sizes[self.INGROUP]
 
     def transfer_dimension_attrs(self, target):
         if not isinstance(target, xr.DataArray | xr.Dataset):
             return target
         updates = {}
         for i in [CASEID, ALTID, GROUPID, INGROUP, CASEALT, CASEPTR]:
             j = self._obj.attrs.get(i, None)
@@ -467,16 +469,16 @@
 
 @xr.register_dataarray_accessor("dc")
 class _DataArrayDC(_GenericFlow):
     _parent_class = xr.DataArray
 
     @property
     def n_alts(self):
-        if self.ALTID in self._obj.dims:
-            return self._obj.shape[self.dims.index(self.ALTID)]
+        if self.ALTID in self._obj.sizes:
+            return self._obj.shape[self.sizes.index(self.ALTID)]
         if "n_alts" in self._obj.attrs:
             return self._obj.attrs["n_alts"]
         raise ValueError("no n_alts set")
 
     def __getitem__(self, name):
         # pass dimension attrs to DataArray
         result = self._obj[name]
@@ -492,16 +494,16 @@
 
 @xr.register_dataset_accessor("dc")
 class _DatasetDC(_GenericFlow):
     _parent_class = xr.Dataset
 
     @property
     def n_alts(self):
-        if self.ALTID in self._obj.dims:
-            return self._obj.dims[self.ALTID]
+        if self.ALTID in self._obj.sizes:
+            return self._obj.sizes[self.ALTID]
         if "n_alts" in self._obj.attrs:
             return self._obj.attrs["n_alts"]
         raise ValueError("no n_alts set")
 
     def __getitem__(self, name):
         # pass dimension attrs to DataArray
         result = self._obj[name]
```

### Comparing `larch6-6.0.8/src/larch/dataset/patch.py` & `larch6-6.0.9/src/larch/dataset/patch.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/datastats.py` & `larch6-6.0.9/src/larch/datastats.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/__init__.py` & `larch6-6.0.9/src/larch/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_017_mnl.py` & `larch6-6.0.9/src/larch/examples/generated/_017_mnl.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_022_nl.py` & `larch6-6.0.9/src/larch/examples/generated/_022_nl.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_030_mnl_constrain.py` & `larch6-6.0.9/src/larch/examples/generated/_030_mnl_constrain.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_101_swissmetro_mnl.py` & `larch6-6.0.9/src/larch/examples/generated/_109_swissmetro_nl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,56 @@
 def example(extract='m', estimate=False):
+    import pandas as pd
+
     import larch as lx
 
-    m = lx.Model()
+    raw_data = pd.read_csv(lx.example_file("swissmetro.csv.gz")).rename_axis(index="CASEID")
+    data = lx.Dataset.construct.from_idco(raw_data, alts={1: "Train", 2: "SM", 3: "Car"})
+    m = lx.Model(data.dc.query_cases("PURPOSE in (1,3) and CHOICE != 0"))
 
-    m.title = "swissmetro example 01 (simple logit)"
+    m.title = "swissmetro example 09 (nested logit)"
 
     m.availability_co_vars = {
         1: "TRAIN_AV * (SP!=0)",
         2: "SM_AV",
         3: "CAR_AV * (SP!=0)",
     }
-
     m.choice_co_code = "CHOICE"
 
     from larch import P, X
 
-    m.utility_co[1] = P("ASC_TRAIN")
-    m.utility_co[2] = 0
-    m.utility_co[3] = P("ASC_CAR")
-    m.utility_co[1] += X("TRAIN_TT") * P("B_TIME")
-    m.utility_co[2] += X("SM_TT") * P("B_TIME")
-    m.utility_co[3] += X("CAR_TT") * P("B_TIME")
-    m.utility_co[1] += X("TRAIN_CO*(GA==0)") * P("B_COST")
-    m.utility_co[2] += X("SM_CO*(GA==0)") * P("B_COST")
-    m.utility_co[3] += X("CAR_CO") * P("B_COST")
+    m.utility_co[1] = P.ASC_TRAIN + P.B_TIME * X.TRAIN_TT + P.B_COST * X("TRAIN_CO*(GA==0)")
+    m.utility_co[2] = P.B_TIME * X.SM_TT + P.B_COST * X("SM_CO*(GA==0)")
+    m.utility_co[3] = P.ASC_CAR + P.B_TIME * X.CAR_TT + P.B_COST * X("CAR_CO")
+
+    m.graph.new_node(parameter="existing", children=[1, 3], name="Existing")
+
+    m.graph
 
     m.ordering = [
         (
             "ASCs",
             "ASC.*",
         ),
         (
             "LOS",
             "B_.*",
         ),
+        ("LogSums", "existing"),
     ]
-
-    import pandas as pd
-
-    raw_data = pd.read_csv(lx.example_file("swissmetro.csv.gz")).rename_axis(index="CASEID")
-    raw_data.head()
-
-    keep = raw_data.eval("PURPOSE in (1,3) and CHOICE != 0")
-    selected_data = raw_data[keep]
-
-    ds = lx.Dataset.construct.from_idco(selected_data, alts={1: "Train", 2: "SM", 3: "Car"})
-
-    ds
-
-    m.datatree = ds
     if not estimate:
         if isinstance(extract, str):
             return locals()[extract]
         else:
             _locals = locals()
             return [_locals.get(i) for i in extract]
     m.set_cap(15)
-    result = m.maximize_loglike(method="SLSQP")
-
-    m.calculate_parameter_covariance();
+    result = m.maximize_loglike()
+    result
 
+    m.calculate_parameter_covariance(robust=True)
     m.parameter_summary()
-
-    # TEST
-    assert m.pvals == approx([-0.15475, -0.70178, -0.010842, -0.012776], rel=1e-3)
-    assert m.pstderr == approx([0.0432357, 0.0548783, 0.000518335, 0.000568829], rel=1e-3)
-    assert m.parameter_summary().data["t Stat"].values.astype(float) == approx(
-        [-3.58, -12.79, -20.92, -22.46], rel=1e-2
-    )
     if isinstance(extract, str):
         return locals()[extract]
     else:
         _locals = locals()
         return [_locals.get(i) for i in extract]
```

### Comparing `larch6-6.0.8/src/larch/examples/generated/_151_swissmetro_panel_latent_class.py` & `larch6-6.0.9/src/larch/examples/generated/_151_swissmetro_panel_latent_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -73,60 +73,23 @@
         datatree=data.dc.set_altids([1, 2, 3]),
         groupid="ID",
     )
 
     b.lock_value(Z_COST=-10000)  # set the lexicographic parameter
 
     b.set_cap(25)
-
-    # TEST
-    assert b.loglike() == approx(-6867.245, rel=1e-4)
-
-    # TEST
-    assert b.d_loglike() == approx(
-        [
-            -1.104770e02,
-            -1.545916e03,
-            -2.188546e01,
-            -9.183448e02,
-            -1.658521e02,
-            8.292606e01,
-            4.470348e-08,
-        ],
-        rel=1e-5,
-    )
     if not estimate:
         if isinstance(extract, str):
             return locals()[extract]
         else:
             _locals = locals()
             return [_locals.get(i) for i in extract]
     result = b.maximize_loglike(method="slsqp")
 
     b.calculate_parameter_covariance();
 
     b.parameter_summary()
-
-    # TEST
-    assert result.loglike == approx(-4474.478515625, rel=1e-5)
-    assert b.pstderr == approx(
-        np.array([0.048158, 0.069796, 0.069555, 0.106282, 0.161079, 0.11945, 0.0]), rel=5e-3
-    )
-    assert b.pvals == approx(
-        np.array(
-            [
-                6.079781e-02,
-                -9.362056e-01,
-                -1.159657e00,
-                -3.095285e00,
-                -7.734768e-01,
-                1.155985e00,
-                -1.000000e04,
-            ]
-        ),
-        rel=5e-3,
-    )
     if isinstance(extract, str):
         return locals()[extract]
     else:
         _locals = locals()
         return [_locals.get(i) for i in extract]
```

### Comparing `larch6-6.0.8/src/larch/examples/generated/_200_exampville.py` & `larch6-6.0.9/src/larch/examples/generated/_200_exampville.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_201_exville_mode_choice.py` & `larch6-6.0.9/src/larch/examples/generated/_201_exville_mode_choice.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_202_exville_mc_logsums.py` & `larch6-6.0.9/src/larch/examples/generated/_202_exville_mc_logsums.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_203_exville_dest.py` & `larch6-6.0.9/src/larch/examples/generated/_203_exville_dest.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/_251_bySpec.py` & `larch6-6.0.9/src/larch/examples/generated/_251_bySpec.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/examples/generated/__init__.py` & `larch6-6.0.9/src/larch/examples/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/folding.py` & `larch6-6.0.9/src/larch/folding.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/logging/__init__.py` & `larch6-6.0.9/src/larch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/basemodel.py` & `larch6-6.0.9/src/larch/model/basemodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import uuid
 import warnings
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
+from .._optional import jax
 from ..dataset import DataTree
 from ..exceptions import MissingDataError
 from .constraints import ParametricConstraintList
 from .linear import DictOfAlts, DictOfLinearFunction, LinearFunction
 from .mixtures import MixtureList
 from .param_core import ParameterBucket
 from .single_parameter import SingleParameter
@@ -198,14 +199,20 @@
         return self._compute_engine
 
     @compute_engine.setter
     def compute_engine(self, engine):
         if engine not in {"numba", "jax", None}:
             raise ValueError("invalid compute engine")
         self._compute_engine = engine
+        if self._compute_engine == "jax" and not jax:
+            warnings.warn(
+                "jax is not installed, falling back to numba",
+                stacklevel=2,
+            )
+            self._compute_engine = "numba"
         if self._compute_engine == "jax" and self.use_streaming:
             warnings.warn(
                 "setting use_streaming to False, jax is not yet compatible",
                 stacklevel=2,
             )
             self.use_streaming = False
```

### Comparing `larch6-6.0.8/src/larch/model/cascading.py` & `larch6-6.0.9/src/larch/model/cascading.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/constraints.py` & `larch6-6.0.9/src/larch/model/constraints.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/dashboard.py` & `larch6-6.0.9/src/larch/model/dashboard.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/data_arrays.py` & `larch6-6.0.9/src/larch/model/data_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,18 +434,18 @@
         if (
             not preserve_vars
             and vars_ca in shared_data_ca.root_dataset
             and not force_flow
         ):
             proposal = shared_data_ca.root_dataset[vars_ca]
             if (
-                shared_data_ca.CASEID in proposal.dims
-                and shared_data_ca.ALTID in proposal.dims
+                shared_data_ca.CASEID in proposal.sizes
+                and shared_data_ca.ALTID in proposal.sizes
             ):
-                proposal = proposal.drop(list(proposal.coords)).rename(tag)
+                proposal = proposal.drop_vars(list(proposal.coords)).rename(tag)
                 return model_dataset.merge(proposal), vars_ca
     if isinstance(vars_ca, str):
         vars_ca = {vars_ca: vars_ca}
     if not isinstance(vars_ca, dict):
         vars_ca = {i: i for i in vars_ca}
     flowname = flownamer(tag, vars_ca, shared_data_ca._hash_features())
     if isinstance(flow, str):
@@ -456,32 +456,32 @@
         shared_data_ca,
         dtype=dtype,
     )
     caseid_dim = shared_data_ca.CASEID
     altid_dim = shared_data_ca.ALTID
     if preserve_vars or len(vars_ca) > 1:
         arr = arr.reshape(
-            model_dataset.dims.get(caseid_dim),
-            model_dataset.dims.get(altid_dim),
+            model_dataset.sizes.get(caseid_dim),
+            model_dataset.sizes.get(altid_dim),
             -1,
         )
         da = DataArray(
             arr,
             dims=[caseid_dim, altid_dim, f"var_{tag}"],
             coords={
                 caseid_dim: model_dataset.coords[caseid_dim],
                 altid_dim: model_dataset.coords[altid_dim],
                 f"var_{tag}": list(vars_ca.keys()),
             },
             name=tag,
         )
     else:
         arr = arr.reshape(
-            model_dataset.dims.get(caseid_dim),
-            model_dataset.dims.get(altid_dim),
+            model_dataset.sizes.get(caseid_dim),
+            model_dataset.sizes.get(altid_dim),
         )
         da = DataArray(
             arr,
             dims=[caseid_dim, altid_dim],
             coords={
                 caseid_dim: model_dataset.coords[caseid_dim],
                 altid_dim: model_dataset.coords[altid_dim],
@@ -505,16 +505,18 @@
 ):
     from ..dataset import DataArray, DataTree
 
     assert isinstance(datatree, DataTree)
     if isinstance(vars_ca, str):
         if not preserve_vars and vars_ca in datatree.root_dataset:
             proposal = datatree.root_dataset[vars_ca]
-            if datatree.CASEALT in proposal.dims:
-                proposal = proposal.drop(list(proposal.coords)).rename(f"{s_tag}_data")
+            if datatree.CASEALT in proposal.sizes:
+                proposal = proposal.drop_vars(list(proposal.coords)).rename(
+                    f"{s_tag}_data"
+                )
                 return model_dataset.merge(proposal), flow
     if isinstance(vars_ca, str):
         vars_ca = {vars_ca: vars_ca}
     if not isinstance(vars_ca, dict):
         vars_ca = {i: i for i in vars_ca}
     flowname = flownamer(s_tag, vars_ca, datatree._hash_features())
     if flow is None or flowname != flow.name:
@@ -522,15 +524,15 @@
     arr = flow.load(
         datatree,
         dtype=dtype,
     )
     casealt_dim = datatree.CASEALT
     if preserve_vars or len(vars_ca) > 1:
         arr = arr.reshape(
-            model_dataset.dims.get(casealt_dim),
+            model_dataset.sizes.get(casealt_dim),
             -1,
         )
         da = DataArray(
             arr,
             dims=[casealt_dim, f"var_{v_tag}"],
             coords={
                 casealt_dim: model_dataset.coords[casealt_dim],
@@ -600,29 +602,29 @@
         dtype=dtype,
     )
     caseid_dim = shared_data_co.CASEID
     if preserve_vars or len(vars_co) > 1:
         if dim_name is None:
             dim_name = f"var_{tag}"
         arr = arr.reshape(
-            model_dataset.dims.get(caseid_dim),
+            model_dataset.sizes.get(caseid_dim),
             -1,
         )
         da = DataArray(
             arr,
             dims=[caseid_dim, dim_name],
             coords={
                 caseid_dim: model_dataset.coords[caseid_dim],
                 dim_name: list(vars_co.keys()),
             },
             name=tag,
         )
     else:
         arr = arr.reshape(
-            model_dataset.dims.get(caseid_dim),
+            model_dataset.sizes.get(caseid_dim),
         )
         da = DataArray(
             arr,
             dims=[caseid_dim],
             coords={
                 caseid_dim: model_dataset.coords[caseid_dim],
             },
```

### Comparing `larch6-6.0.8/src/larch/model/draws.py` & `larch6-6.0.9/src/larch/model/draws.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/fast_mapping.py` & `larch6-6.0.9/src/larch/model/fast_mapping.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/from_spec.py` & `larch6-6.0.9/src/larch/model/from_spec.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/jaxmodel.py` & `larch6-6.0.9/src/larch/model/jaxmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import warnings
 
 import numpy as np
 import pandas as pd
 from xarray import Dataset
 
 from .._optional import jax, jnp
 from ..compiled import compiledmethod, jitmethod, reset_compiled_methods
@@ -82,22 +83,37 @@
         self.prerolled_draws = True
         self.common_draws = False
 
     @property
     def compute_engine(self):
         engine = self._compute_engine
         if engine is None:
-            engine = "jax"
+            if not jax:
+                engine = "numba"
+            else:
+                engine = "jax"
         return engine
 
     @compute_engine.setter
     def compute_engine(self, engine):
         if engine not in {"numba", "jax", None}:
             raise ValueError("invalid compute engine")
         self._compute_engine = engine
+        if self._compute_engine == "jax" and not jax:
+            warnings.warn(
+                "jax is not installed, falling back to numba",
+                stacklevel=2,
+            )
+            self._compute_engine = "numba"
+        if self._compute_engine == "jax" and self.use_streaming:
+            warnings.warn(
+                "setting use_streaming to False, jax is not yet compatible",
+                stacklevel=2,
+            )
+            self.use_streaming = False
 
     prerolled_draws = MangleOnChange(bool)
     common_draws = MangleOnChange(bool)
     n_draws = MangleOnChange(int)
     seed = MangleOnChange()
 
     # @property
```

### Comparing `larch6-6.0.8/src/larch/model/latent_class.py` & `larch6-6.0.9/src/larch/model/latent_class.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/linear.py` & `larch6-6.0.9/src/larch/model/linear.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/linear_math.py` & `larch6-6.0.9/src/larch/model/linear_math.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/mixtures.py` & `larch6-6.0.9/src/larch/model/mixtures.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/numba_optimization.py` & `larch6-6.0.9/src/larch/model/numba_optimization.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/numba_stream.py` & `larch6-6.0.9/src/larch/model/numba_stream.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/numbamodel.py` & `larch6-6.0.9/src/larch/model/numbamodel.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/optimization.py` & `larch6-6.0.9/src/larch/model/optimization.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/param_core.py` & `larch6-6.0.9/src/larch/model/param_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,19 +146,19 @@
             )
         return new_params
 
     def update_parameters(self, other):
         if isinstance(other, ParameterBucket):
             other = other._params
         if isinstance(other, xr.Dataset):
-            if "param_name_2" in other.dims:
+            if "param_name_2" in other.sizes:
                 other = other.drop_dims("param_name_2")  # TODO, keep 2nd dim
-            if len(other.dims) != 1:
+            if len(other.sizes) != 1:
                 raise ValueError("expected parameters to be a 1-d vector")
-            other_dim = iter(other.dims).__next__()
+            other_dim = iter(other.sizes).__next__()
             joint_names = set(self.pnames) | set(other.coords[other_dim].data)
         else:
             joint_names = set(self.pnames) | set(other.pnames)
         should_mangle = False
         new_params = self._params.reindex({self.index_name: sorted(joint_names)})
         filling = [i for i in new_params if i in other]
         try:
@@ -225,15 +225,15 @@
 
     @property
     def parameters(self):
         return self._params
 
     @property
     def n_params(self):
-        return self._params.dims[self.index_name]
+        return self._params.sizes[self.index_name]
 
     @property
     def pvals(self):
         return self._params["value"].to_numpy()
 
     @pvals.setter
     def pvals(self, x):
@@ -549,15 +549,15 @@
         instance.mangle()
 
     def pretty_table(self, name_width=25):
         from rich.table import Table
 
         params = self._params
         rich_table = Table()
-        idx_name, n = next(iter(params.dims.items()))
+        idx_name, n = next(iter(params.sizes.items()))
         for column in params.variables:
             rich_table.add_column(
                 str(column), width=name_width if column == self.index_name else None
             )
         for i in range(n):
             row = [str(params[j].data[i]) for j in params.variables]
             rich_table.add_row(*row)
```

### Comparing `larch6-6.0.8/src/larch/model/saving.py` & `larch6-6.0.9/src/larch/model/saving.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/single_parameter.py` & `larch6-6.0.9/src/larch/model/single_parameter.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/model/tree.py` & `larch6-6.0.9/src/larch/model/tree.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/omx.py` & `larch6-6.0.9/src/larch/omx.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/optimize.py` & `larch6-6.0.9/src/larch/optimize.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/roles.py` & `larch6-6.0.9/src/larch/roles.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/__init__.py` & `larch6-6.0.9/src/larch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/auto_ownership.py` & `larch6-6.0.9/src/larch/util/activitysim/auto_ownership.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/cdap.py` & `larch6-6.0.9/src/larch/util/activitysim/cdap.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/data_maker.py` & `larch6-6.0.9/src/larch/util/activitysim/data_maker.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/general.py` & `larch6-6.0.9/src/larch/util/activitysim/general.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/location_choice.py` & `larch6-6.0.9/src/larch/util/activitysim/location_choice.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/nonmand_tour_freq.py` & `larch6-6.0.9/src/larch/util/activitysim/nonmand_tour_freq.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/activitysim/tour_mode_choice.py` & `larch6-6.0.9/src/larch/util/activitysim/tour_mode_choice.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/addict_yaml.py` & `larch6-6.0.9/src/larch/util/addict_yaml.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/arraytools.py` & `larch6-6.0.9/src/larch/util/arraytools.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/aster.py` & `larch6-6.0.9/src/larch/util/aster.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/bitmasking.py` & `larch6-6.0.9/src/larch/util/bitmasking.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/bounded_kde.py` & `larch6-6.0.9/src/larch/util/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/cache_requests.py` & `larch6-6.0.9/src/larch/util/cache_requests.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/colors.py` & `larch6-6.0.9/src/larch/util/colors.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/common_functions.py` & `larch6-6.0.9/src/larch/util/common_functions.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/counting.py` & `larch6-6.0.9/src/larch/util/counting.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/data_expansion.py` & `larch6-6.0.9/src/larch/util/data_expansion.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/data_manipulation.py` & `larch6-6.0.9/src/larch/util/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/dataframe.py` & `larch6-6.0.9/src/larch/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/display.py` & `larch6-6.0.9/src/larch/util/display.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/excel.py` & `larch6-6.0.9/src/larch/util/excel.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/figures.py` & `larch6-6.0.9/src/larch/util/figures.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/histograms.py` & `larch6-6.0.9/src/larch/util/histograms.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/html_table_to_txt.py` & `larch6-6.0.9/src/larch/util/html_table_to_txt.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/images.py` & `larch6-6.0.9/src/larch/util/images.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/interface_info.py` & `larch6-6.0.9/src/larch/util/interface_info.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/lazy.py` & `larch6-6.0.9/src/larch/util/lazy.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/math.py` & `larch6-6.0.9/src/larch/util/math.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/multiindex.py` & `larch6-6.0.9/src/larch/util/multiindex.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/namespaces.py` & `larch6-6.0.9/src/larch/util/namespaces.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/naming.py` & `larch6-6.0.9/src/larch/util/naming.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/overspec_viewer.py` & `larch6-6.0.9/src/larch/util/overspec_viewer.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/plotting.py` & `larch6-6.0.9/src/larch/util/plotting.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/png.py` & `larch6-6.0.9/src/larch/util/png.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/rate_limiter.py` & `larch6-6.0.9/src/larch/util/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/signal_dict.py` & `larch6-6.0.9/src/larch/util/signal_dict.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/smartread.py` & `larch6-6.0.9/src/larch/util/smartread.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/statistics.py` & `larch6-6.0.9/src/larch/util/statistics.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/styles.py` & `larch6-6.0.9/src/larch/util/styles.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/summary.py` & `larch6-6.0.9/src/larch/util/summary.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/temporaryfile.py` & `larch6-6.0.9/src/larch/util/temporaryfile.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/text_manip.py` & `larch6-6.0.9/src/larch/util/text_manip.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/timesize.py` & `larch6-6.0.9/src/larch/util/timesize.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/touch_notifier.py` & `larch6-6.0.9/src/larch/util/touch_notifier.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/visual_processing.py` & `larch6-6.0.9/src/larch/util/visual_processing.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/xhtml.py` & `larch6-6.0.9/src/larch/util/xhtml.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/yaml_checker.py` & `larch6-6.0.9/src/larch/util/yaml_checker.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch/util/zipdir.py` & `larch6-6.0.9/src/larch/util/zipdir.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/src/larch6.egg-info/PKG-INFO` & `larch6-6.0.9/src/larch6.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: larch6
-Version: 6.0.8
+Version: 6.0.9
 Author-email: Jeff Newman <jeff@driftless.xyz>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.19
 Requires-Dist: pandas>=1.2
 Requires-Dist: pyarrow
 Requires-Dist: xarray
```

### Comparing `larch6-6.0.8/src/larch6.egg-info/SOURCES.txt` & `larch6-6.0.9/src/larch6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/tests/test_exampville.py` & `larch6-6.0.9/tests/test_exampville.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/tests/test_jax.py` & `larch6-6.0.9/tests/test_jax.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/tests/test_latent_class.py` & `larch6-6.0.9/tests/test_latent_class.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/tests/test_mtc.py` & `larch6-6.0.9/tests/test_mtc.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/tests/test_swissmetro.py` & `larch6-6.0.9/tests/test_swissmetro.py`

 * *Files identical despite different names*

### Comparing `larch6-6.0.8/tools/rip_examples.py` & `larch6-6.0.9/tools/rip_examples.py`

 * *Files identical despite different names*

