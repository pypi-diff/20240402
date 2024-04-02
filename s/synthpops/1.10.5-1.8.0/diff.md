# Comparing `tmp/synthpops-1.10.5.tar.gz` & `tmp/synthpops-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthpops-1.10.5.tar", last modified: Tue Apr  2 20:47:46 2024, max compression
+gzip compressed data, was "synthpops-1.8.0.tar", last modified: Sat May  8 02:52:58 2021, max compression
```

## Comparing `synthpops-1.10.5.tar` & `synthpops-1.8.0.tar`

### file list

```diff
@@ -1,125 +1,100 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:46.002614 synthpops-1.10.5/
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:45.994614 synthpops-1.10.5/.pytest_cache/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)      295 2020-05-23 03:12:40.000000 synthpops-1.10.5/.pytest_cache/README.md
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22767 2024-04-02 20:46:29.000000 synthpops-1.10.5/CHANGELOG.rst
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)    16228 2020-05-18 20:48:39.000000 synthpops-1.10.5/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2021-05-14 23:53:21.000000 synthpops-1.10.5/MANIFEST.in
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6241 2024-04-02 20:47:46.002614 synthpops-1.10.5/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5326 2024-04-02 20:46:29.000000 synthpops-1.10.5/README.md
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:45.994614 synthpops-1.10.5/data/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)      458 2020-12-16 04:07:36.000000 synthpops-1.10.5/data/README.md
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:45.998614 synthpops-1.10.5/docs/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1989 2021-05-08 02:46:59.000000 synthpops-1.10.5/docs/algorithm.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3217 2021-05-08 02:46:59.000000 synthpops-1.10.5/docs/glossary.rst
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     5941 2020-05-18 20:48:40.000000 synthpops-1.10.5/docs/households.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      872 2021-05-08 02:46:59.000000 synthpops-1.10.5/docs/index.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    11988 2024-04-02 20:46:11.000000 synthpops-1.10.5/docs/input_data.rst
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     1594 2020-05-23 06:53:23.000000 synthpops-1.10.5/docs/installation.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      549 2021-05-20 07:25:30.000000 synthpops-1.10.5/docs/modules.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2464 2021-05-08 02:46:59.000000 synthpops-1.10.5/docs/overview.rst
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     5229 2020-05-23 07:07:30.000000 synthpops-1.10.5/docs/schools.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.base.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.config.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      168 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.contact_networks.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      174 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.data_distributions.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.households.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.ltcfs.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.plotting.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.pop.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.sampling.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.schools.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.version.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2021-05-08 02:28:15.000000 synthpops-1.10.5/docs/synthpops.workplaces.rst
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     2989 2020-05-18 20:48:40.000000 synthpops-1.10.5/docs/template_guide.md
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4063 2021-05-08 02:46:59.000000 synthpops-1.10.5/docs/usage.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       30 2021-05-08 02:46:59.000000 synthpops-1.10.5/docs/whatsnew.rst
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     2618 2020-05-18 20:48:40.000000 synthpops-1.10.5/docs/workplaces.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:45.998614 synthpops-1.10.5/examples/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)      211 2020-05-23 06:53:23.000000 synthpops-1.10.5/examples/README.md
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-02 20:47:46.002614 synthpops-1.10.5/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1843 2024-04-02 20:46:29.000000 synthpops-1.10.5/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:45.998614 synthpops-1.10.5/synthpops/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1111 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13445 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6990 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/config.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    32766 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/contact_networks.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:46.002614 synthpops-1.10.5/synthpops/data/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   298323 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/data/MUestimates_all_locations.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   295170 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/data/MUestimates_home.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   295922 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/data/MUestimates_other_locations.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   300497 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/data/MUestimates_school.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   161631 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/data/MUestimates_work.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10570 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/Malawi.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7873 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/Nepal.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14000 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/Senegal-Dakar-Dakar.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9852 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/Senegal-Dakar.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4363 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/Senegal.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6765 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/Zimbabwe.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13735 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/bangladesh-dhaka-dhaka_city.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6511 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Oregon-portland_metro.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5605 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Oregon.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10016 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Washington-Franklin_County.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9971 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Washington-Island_County.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10539 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Washington-Spokane_County.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    11820 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Washington-seattle_metro.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9124 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa-Washington.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4266 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data/usa.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    34104 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    56029 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/data_distributions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2967 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops/defaults.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    31975 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/households.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    17629 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/ltcfs.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:46.002614 synthpops-1.10.5/synthpops/people/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    37451 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/country_age_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8488 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/household_size_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7672 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/loaders.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16231 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/makepop.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    40593 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15676 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/state_age_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4122 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/people/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    90024 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    64147 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/pop.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14004 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/sampling.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    77896 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/schools.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       55 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/version.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18902 2024-04-02 20:46:29.000000 synthpops-1.10.5/synthpops/workplaces.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:45.998614 synthpops-1.10.5/synthpops.egg-info/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     6241 2024-04-02 20:47:45.000000 synthpops-1.10.5/synthpops.egg-info/PKG-INFO
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3109 2024-04-02 20:47:45.000000 synthpops-1.10.5/synthpops.egg-info/SOURCES.txt
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-02 20:47:45.000000 synthpops-1.10.5/synthpops.egg-info/dependency_links.txt
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)      141 2024-04-02 20:47:45.000000 synthpops-1.10.5/synthpops.egg-info/requires.txt
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)       10 2024-04-02 20:47:45.000000 synthpops-1.10.5/synthpops.egg-info/top_level.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:46.002614 synthpops-1.10.5/synthpops_process_raw_data/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    81511 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops_process_raw_data/data_distributions_legacy.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24643 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops_process_raw_data/migrate_legacy_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    36981 2021-05-14 23:53:21.000000 synthpops-1.10.5/synthpops_process_raw_data/process_census.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:46.002614 synthpops-1.10.5/tests/
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-02 20:47:46.002614 synthpops-1.10.5/tests/.pytest_cache/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      295 2021-03-09 23:56:08.000000 synthpops-1.10.5/tests/.pytest_cache/README.md
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1562 2021-05-08 02:46:59.000000 synthpops-1.10.5/tests/test_Dakar.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1967 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_Dakar_full.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1565 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_Malawi.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1644 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_Nepal.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1558 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_Spokane.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1803 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_Zimbabwe.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3087 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_basic_api.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5490 2021-05-14 23:53:21.000000 synthpops-1.10.5/tests/test_config.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    38254 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5323 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_demographics_generated.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10422 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_household_class.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2770 2021-05-08 02:46:59.000000 synthpops-1.10.5/tests/test_household_generation_methods.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2609 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_ltcf_class.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5009 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_ltcfs.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2406 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_oop.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2814 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15317 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4170 2021-05-14 23:53:21.000000 synthpops-1.10.5/tests/test_regression.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8919 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_regression_metapop_summary.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4809 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_school_class.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3279 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_school_inter_grade_mixing.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4971 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_school_mixing_types.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8438 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_school_sizes_by_type.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1881 2021-05-14 23:53:21.000000 synthpops-1.10.5/tests/test_school_with_non_teaching_staff.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10800 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_summary_methods.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4753 2024-04-02 20:46:29.000000 synthpops-1.10.5/tests/test_workplace_class.py
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.176683 synthpops-1.8.0/
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/.pytest_cache/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      295 2020-05-23 03:12:40.000000 synthpops-1.8.0/.pytest_cache/README.md
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    13361 2021-05-08 02:46:59.000000 synthpops-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)    16228 2020-05-18 20:48:39.000000 synthpops-1.8.0/LICENSE
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      173 2021-05-08 02:46:59.000000 synthpops-1.8.0/MANIFEST.in
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     6084 2021-05-08 02:52:58.176683 synthpops-1.8.0/PKG-INFO
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     4536 2021-05-08 02:46:59.000000 synthpops-1.8.0/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      458 2020-12-16 04:07:36.000000 synthpops-1.8.0/data/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/Oregon/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)       74 2020-12-16 04:07:36.000000 synthpops-1.8.0/data/usa/Oregon/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/Washington/
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/Washington/age_distributions/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      236 2020-12-16 04:07:36.000000 synthpops-1.8.0/data/usa/Washington/age_distributions/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/Washington/seattle_metro/
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/Washington/seattle_metro/schools/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      624 2020-12-16 04:07:36.000000 synthpops-1.8.0/data/usa/Washington/seattle_metro/schools/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/Washington/seattle_metro/schools/county_school_enrollment_by_age/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      341 2020-12-16 04:07:36.000000 synthpops-1.8.0/data/usa/Washington/seattle_metro/schools/county_school_enrollment_by_age/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/data/usa/household_living_arrangements/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      356 2020-12-16 04:07:36.000000 synthpops-1.8.0/data/usa/household_living_arrangements/README.md
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.172683 synthpops-1.8.0/docs/
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     1989 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/algorithm.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     3217 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/glossary.rst
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     5941 2020-05-18 20:48:40.000000 synthpops-1.8.0/docs/households.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      872 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/index.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    11988 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/input_data.rst
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     1594 2020-05-23 06:53:23.000000 synthpops-1.8.0/docs/installation.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      473 2021-05-08 02:41:40.000000 synthpops-1.8.0/docs/modules.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     2464 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/overview.rst
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     5229 2020-05-23 07:07:30.000000 synthpops-1.8.0/docs/schools.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      130 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.base.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      136 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.config.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      168 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.contact_networks.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      174 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.data_distributions.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      148 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.households.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      133 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.ltcfs.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      142 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.plotting.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      127 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.pop.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      142 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.sampling.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      139 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.schools.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      139 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.version.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      148 2021-05-08 02:28:15.000000 synthpops-1.8.0/docs/synthpops.workplaces.rst
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     2989 2020-05-18 20:48:40.000000 synthpops-1.8.0/docs/template_guide.md
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     4063 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/usage.rst
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)       30 2021-05-08 02:46:59.000000 synthpops-1.8.0/docs/whatsnew.rst
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     2618 2020-05-18 20:48:40.000000 synthpops-1.8.0/docs/workplaces.rst
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.172683 synthpops-1.8.0/examples/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      211 2020-05-23 06:53:23.000000 synthpops-1.8.0/examples/README.md
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)       38 2021-05-08 02:52:58.176683 synthpops-1.8.0/setup.cfg
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     1855 2021-05-08 02:46:59.000000 synthpops-1.8.0/setup.py
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.172683 synthpops-1.8.0/synthpops/
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      398 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/__init__.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    13148 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/base.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     6990 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/config.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    31428 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/contact_networks.py
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.176683 synthpops-1.8.0/synthpops/data/
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)   298323 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/MUestimates_all_locations.obj
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)   295170 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/MUestimates_home.obj
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)   295922 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/MUestimates_other_locations.obj
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)   300497 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/MUestimates_school.obj
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)   161631 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/MUestimates_work.obj
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     8387 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/Senegal-Dakar-Dakar.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     8418 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/Senegal-Dakar.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     3688 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/Senegal.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     6289 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Oregon-portland_metro.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     6294 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Oregon.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     9886 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Washington-Franklin_County.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     9843 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Washington-Island_County.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    11514 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Washington-Spokane_County.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    11466 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Washington-seattle_metro.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     9146 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa-Washington.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     1740 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data/usa.json
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    33848 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    56029 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/data_distributions.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)     2967 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/defaults.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    21197 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/households.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    29789 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/ltcfs.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    92077 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/plotting.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    63387 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/pop.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    14008 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/sampling.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    73825 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/schools.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)       53 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/version.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    18876 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops/workplaces.py
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.172683 synthpops-1.8.0/synthpops.egg-info/
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     6084 2021-05-08 02:52:58.000000 synthpops-1.8.0/synthpops.egg-info/PKG-INFO
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)     2309 2021-05-08 02:52:58.000000 synthpops-1.8.0/synthpops.egg-info/SOURCES.txt
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)        1 2021-05-08 02:52:58.000000 synthpops-1.8.0/synthpops.egg-info/dependency_links.txt
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)      156 2021-05-08 02:52:58.000000 synthpops-1.8.0/synthpops.egg-info/requires.txt
+-rw-r--r--   0 cliffk    (1001) cliffk    (1001)       10 2021-05-08 02:52:58.000000 synthpops-1.8.0/synthpops.egg-info/top_level.txt
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.176683 synthpops-1.8.0/synthpops_process_raw_data/
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    81511 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops_process_raw_data/data_distributions_legacy.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    24643 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops_process_raw_data/migrate_legacy_data.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    36981 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops_process_raw_data/process_census.py
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)    37351 2021-05-08 02:46:59.000000 synthpops-1.8.0/synthpops_process_raw_data/test_data.py
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.168683 synthpops-1.8.0/tests/
+drwxrwxr-x   0 cliffk    (1001) cliffk    (1001)        0 2021-05-08 02:52:58.176683 synthpops-1.8.0/tests/.pytest_cache/
+-rw-rw-r--   0 cliffk    (1001) cliffk    (1001)      295 2021-03-09 23:56:08.000000 synthpops-1.8.0/tests/.pytest_cache/README.md
```

### Comparing `synthpops-1.10.5/CHANGELOG.rst` & `synthpops-1.8.0/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -18,122 +18,17 @@
 - "Deprecated": a method or feature that has been removed or support will be removed for in the future.
 
 - "Regression Information": a change to the model or update to data resulted in a change to regression results.
 
 - "Github Info": the associated PRs to any changes.
 
 
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Latest versions (1.10.x)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-
-Version 1.10.5 (2022-03-14)
----------------------------
-- Updating the license to Creative Commons Attribution-ShareAlike 4.0 International License.
-
-
-Version 1.10.4 (2021-07-05)
----------------------------
-- Update to README to include the working title of the manuscript. We're doing this so that if people start using the model prior to the manuscript being available, they will still cite the work appropriately instead of using just the website.
-
-
-Version 1.10.3 (2021-05-25)
----------------------------
-- *Fix*: Addressing a bug when schools smaller than expected by the school size distributions are created in the case where there are not enough students left to place in the selected type of school.
-- *Github Info*: PR `505 <https://github.com/amath-idm/synthpops/pull/505>`__
-
-
-Version 1.10.2 (2021-05-22)
----------------------------
-- Adding new json data files plus some example scripts to show users how to make their own json data files from individual raw data files for a given location.
-- *Github Info*: PRs `494 <https://github.com/amath-idm/synthpops/pull/494>`__, `506 <https://github.com/amath-idm/synthpops/pull/506>`__
-
-
-Version 1.10.1 (2021-05-20)
----------------------------
-- *Fix*: Reinstating previous tests on methods within ``sp.data.py`` and updating ``sp.load_location_from_json_str()`` to take an optional parameter to control when checks on data loading are performed.
-- *Github Info*: PR `502 <https://github.com/amath-idm/synthpops/pull/502>`__
-
-
-Version 1.10.0 (2021-05-20)
----------------------------
-- *Feature*: Ports Covasim's ``People`` class to SynthPops, and adds a new method to the ``Pop`` object, ``to_people()``. 
-- While the differences are numerous, the major difference is that the ``People`` class stores data as NumPy arrays rather than as dicts or objects. This leads to performance improvements, at a cost of reduced flexibility. Most notable, ``people.contacts`` is a single edge list per layer, which is very fast to iterate over. Other quantities, such as ``people['age']``, are also flat vectors. 
-- This functionality is not imported into the global SynthPops namespace; you can use it via ``sp.people.People()`` or ``import synthpops.people as spp; spp.People()``.
-- In future, these new classes and functions will be incorporated more tightly into the main SynthPops ``Pop`` class.
-- *Github*: PR `497 <https://github.com/amath-idm/synthpops/pull/497>`__
-
-
-Version 1.9.3 (2021-05-20)
---------------------------
-- *Feature*: Minor feature update - plotting methods will now automatically search for location information to include in the figure titles. In order of `location`, `state_location`, `country_location`, ``sp.plotting.plkwargs.make_title()`` will look for the first available string to prefix the figure title.
-- This update also changes behavior of some logging statements when using plotting methods. Instead of always sending users information about kwargs missing and the value of defaults being used in place, this behavior is now available under the debug mode for SynthPops.
-- *Github Info*: PR `498 <https://github.com/amath-idm/synthpops/pull/498>`__
-
-
-Version 1.9.2 (2021-05-20)
---------------------------
-- *Fix*: Fix to how different layer classes get ages of members in the group or subgroups within. Specifically, this fixes how ages for members of schools and long term care facilities are calculated so that these layer classes can also call on the ages of members with specific roles in the class (i.e., students vs. teachers vs. non-teaching staff, or residents vs. staff). Tests have been added to verify these methods now work as expected.
-- Slight reorganizing of module imports in ``pop.py``
-- *Github Info*: PR `495 <https://github.com/amath-idm/synthpops/pull/495>`__
-
-
-Version 1.9.1 (2021-05-20)
---------------------------
-- *Fix*: Fixing the logic in ``sp.contact_networks.get_contact_counts_by_layer`` so that it no longer returns an empty list in the dictionary counting contacts by layer group id, but rather returns lists populated with actual counts. Test assertions have also been added to catch this in case of future refactor work; see ``test_plotting.py:test_plot_contact_counts_on_pop``.
-- *Github Info*: PR `483 <https://github.com/amath-idm/synthpops/pull/483>`__
-
-
-Version 1.9.0 (2021-05-16)
---------------------------
-- Data folder cleaned up and removed individual csv data files now that synthpops has json data files instead for the collection of data used for each location.
-- Json data objects also updated with documentation on the sources for the original and estimated data. When data have been estimated or inferred, to the best of our ability, we've added a note about this in the notes field.
-- *Github Info*: PR `427 <https://github.com/amath-idm/synthpops/pull/427>`__
-
-
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Versions 1.8.x (1.8.0 – 1.8.4)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-
-Version 1.8.4 (2021-05-14)
---------------------------
-- *Fix*: Catching rare events when schools are created with fewer than the smallest expected school size because there are no more students left to place in a school.
-- *Feature*: Additional functionality to allow for the average classroom size to be different based on school mixing type (random, age_clustered, or age_and_class_clustered). 
-- Warning users when average class size and the average student teacher ratio parameters are incompatible as well as how synthpops handles these situations. 
-- *Fix*: Logic on how average class size and the average student teacher ratio parameters interact to create cohorts of students when the mixing type is age_and_class_clustered. The cohort size is drawn from a poisson on the larger of the two values. Why? Because for schools where students are cohorted into classrooms, there should be at least one teacher per classroom (average student teacher ratio), but there may be more than one (if average class size > average student teacher ratio).
-- *Regression Information*: Refactoring related to schools as described above.
-- *Github*: PR `459 <https://github.com/amath-idm/synthpops/pull/459>`__
-
-
-Version 1.8.3 (2021-05-14)
---------------------------
-- *Fix*: Refactored population generation methods to first determine the ages to be generated or expected to be generated, then have this be an input for methods to generate long term care facility residents' ages, and then methods to generate households and household member ages for the rest of the population residing in that layer. Addresses small n population bug identified with the household_method of 'fixed_ages' (issues `311 <https://github.com/amath-idm/synthpops/issues/311>`__ / `333 <https://github.com/amath-idm/synthpops/issues/333>`__) and allows for arbitrarily small populations (n > 0) to be created, although with smaller n matching the age distribution expected gets harder. 
-- *Fix*: Also fixes zero division errors when calculating pop properties like the enrollment and employment rates by age when there is at least one age with a count of zero people in the population (issue `383 <https://github.com/amath-idm/synthpops/issues/383>`__).
-- Moved all household generation methods to sp.households
-- Method to generate the count of household sizes for a fixed population renamed: ``sp.households.generate_household_sizes_from_fixed_pop_size`` --> ``sp.households.generate_household_size_count_from_fixed_pop_size``
-- ``sp.households.generate_larger_household_sizes`` generalized to all household sizes (now including size 1) in sp.households.generate_household_sizes
-- ``sp.households.generate_larger_household_head_ages`` generalized to all household sizes (now including size 1) in ``sp.households.generate_household_head_ages``
-- New method: ``sp.households.generate_age_count_multinomial``
-- *Deprecated*: ``sp.households.generate_household_head_age_by_size``, ``sp.households.generate_living_alone``, ``sp.households.generate_living_alone_method_2``
-- *Regression Information*: Refactoring population generation methods to first determine the ages to be generated and then place people in residences produces a stochastic change in the regression population. Take a look at how the generated age distributions compare to the expected via pop.plot_ages().
-- *Github Info*: PRs: `384 <https://github.com/amath-idm/synthpops/pull/384>`__
-
-
-Version 1.8.2 (2021-05-12)
---------------------------
-- *Fix*: Fix changes when constraints and other checks are performed in the data loading step. Now all checks should be performed only once after synthpops has checked the location and all of its parent locations for the necessary data to create the networked populations.
-- *Github*: PR `485 <https://github.com/amath-idm/synthpops/pull/485>`__
-
-
-Version 1.8.1 (2021-05-09)
---------------------------
-- *Fix*: Minor fix to how the expected data are called when plotting the head of household age distributions by household size in ``sp.plotting.plot_household_head_ages_by_size()``. Temporarily this method set the location parameter to None when the ability to traverse up parent locations was not yet functional. With that implemented now, we can keep information about all levels of the location and synthpops will look for the first data set available starting from the child location and moving upwards through all parent locations.
-- *Github*: PR `478 <https://github.com/amath-idm/synthpops/pull/478>`__
+~~~~~~~~~~~~~~~~~~~~~~~
+Latest versions (1.8.x)
+~~~~~~~~~~~~~~~~~~~~~~~
 
 
 Version 1.8.0 (2021-05-07)
 --------------------------
 - This is a big one!
 - *Feature*: Class structures implemented for each layer and added to pop objects generated via `pop = sp.Pop()`. For example, now you can do ``pop.get_household(i)`` to get the household with integer ``hhid`` with value ``i`` which will be a ``sp.Household`` object with at minimum the attributes ``hhid``, ``member_uids``, ``reference_uid``, and ``reference_age``.
 - Base class for layer groups available in ``sp.base.py``; see class ``sp.base.LayerGroup()`` for more info. Important to note that this class has a method ``member_ages()`` which takes in a mapping of person ids to age to return the ages of individuals in a layer group. Optional parameter `subgroup_member_uids` allows you to return the ages for a subgroup of individuals.
```

### Comparing `synthpops-1.10.5/LICENSE` & `synthpops-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/README.md` & `synthpops-1.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 # SynthPops
 
-SynthPops is a module designed to generate synthetic populations that are used for COVID-19 (SARS-CoV-2) epidemic analyses. SynthPops can create generic populations with different network characteristics, as well as synthetic populations that interact in different layers of a multilayer contact network. **Note**: SynthPops is currently under active development and most features are fully tested and documented, but not all. We are in the process of expanding to include data and validation on additional regions beyond the original scope of the Seattle-King County region of Washington, USA. At the moment we have data for the following locations (in the synthpops/data folder) :
-
-* Seattle Metro, Washington, USA
-* Spokane County, Washington, USA
-* Franklin County, Washington, USA
-* Island County, Washington, USA
-* Dakar, Dakar Region, Senegal
-* Zimbabwe\*
-* Malawi\*
-* Nepal\*
-
-\* Data for these locations are at the national scale. In the future, we hope to provide data at a more fine grained resolution for these locations.
+SynthPops is a module designed to generate synthetic populations that are used for COVID-19 (SARS-CoV-2) epidemic analyses. SynthPops can create generic populations with different network characteristics, as well as synthetic populations that interact in different layers of a multilayer contact network. **Note**: SynthPops is currently under active development and not all features are fully tested and documented. Currently, synthetic populations are only implemented for one region (Seattle, USA). We are in the process of expanding to include data on additional regions.
 
 
 The code was originally developed to explore the impact of contact tracing and testing in human contact networks in combination with our [Covasim repository](https://github.com/InstituteforDiseaseModeling/covasim). This product uses the Census Bureau Data API but is not endorsed or certified by the Census Bureau.
 
 More extensive installation and usage instructions are in the [SynthPops documentation](https://docs.idmod.org/projects/synthpops/en/latest).
 
-A scientific manuscript describing the model is currently in progress. If you use the model, in the mean time the recommended citation is:
-
-**SynthPops: a generative model of human contact networks**. Mistry D, Kerr CC, Abeysuriya R, Wu M, Fisher M, Thompson A, Skrip L, Cohen JA, Althouse BM, Klein DJ (2021). (in preparation). 
-
-
 ## Installation
 
 Python >=3.7, <3.9 is required. Python 2 is not supported. Virtual environments are strongly recommended but not required.
 
 To install, first clone the GitHub repository:
 
 `git clone https://github.com/InstituteforDiseaseModeling/synthpops.git`
@@ -88,9 +72,9 @@
 ### tests
 
 The `tests` folder contains tests of different functions available in SynthPops.
 
 
 ## Disclaimer
 
-The code in this repository was developed by IDM to support our research in disease transmission and managing epidemics. We’ve made it publicly available under the Creative Commons Attribution-ShareAlike 4.0 International License to provide others with a better understanding of our research and an opportunity to build upon it for their own work. We make no representations that the code works as intended or that we will provide support, address issues that are found, or accept pull requests. You are welcome to create your own fork and modify the code to suit your own modeling needs as contemplated under the Creative Commons Attribution-Noncommercial-ShareAlike 4.0 License.
+The code in this repository was developed by IDM to support our research in disease transmission and managing epidemics. We’ve made it publicly available under the Creative Commons Attribution-Noncommercial-ShareAlike 4.0 License to provide others with a better understanding of our research and an opportunity to build upon it for their own work. We make no representations that the code works as intended or that we will provide support, address issues that are found, or accept pull requests. You are welcome to create your own fork and modify the code to suit your own modeling needs as contemplated under the Creative Commons Attribution-Noncommercial-ShareAlike 4.0 License.
```

### Comparing `synthpops-1.10.5/docs/algorithm.rst` & `synthpops-1.8.0/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/glossary.rst` & `synthpops-1.8.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/households.rst` & `synthpops-1.8.0/docs/households.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/index.rst` & `synthpops-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/input_data.rst` & `synthpops-1.8.0/docs/input_data.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/installation.rst` & `synthpops-1.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/overview.rst` & `synthpops-1.8.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/schools.rst` & `synthpops-1.8.0/docs/schools.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/template_guide.md` & `synthpops-1.8.0/docs/template_guide.md`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/usage.rst` & `synthpops-1.8.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/docs/workplaces.rst` & `synthpops-1.8.0/docs/workplaces.rst`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/setup.py` & `synthpops-1.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,27 +28,28 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
 ]
 
 setup(
     name="synthpops",
     version=version,
-    author="Dina Mistry, Cliff Kerr, Meikang Wu, Mary Fisher, Ace Thompson, and Daniel Klein on behalf of the IDM COVID-19 Response Team",
+    author="Dina Mistry, Cliff Kerr, Meikang Wu, Mary Fisher, and Daniel Klein on behalf of the IDM COVID-19 Response Team",
     author_email="covid@idmod.org",
     description="Synthetic contact network generation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://synthpops.org',
     keywords=["human contact networks", "synthetic population", "age mixing patterns", "census", "demography"],
     platforms=["OS Independent"],
     classifiers=CLASSIFIERS,
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        "sciris>=1.1.1",
+        "sciris>=1.0.0",
+        "covasim>=2.0.0",
         "matplotlib>=3.3.0",
         "numpy",
         "scipy",
         "pandas>=1.2.3",
         "numba",
         "networkx>=2.3",
         "cmocean",
```

### Comparing `synthpops-1.10.5/synthpops/base.py` & `synthpops-1.8.0/synthpops/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,24 +66,15 @@
                     if self[key] is not None:
                         errmsg = f"error: Expected type int or None for {layer_str} key {key}. Instead the type of this value is {type(self[key])}."
                         raise TypeError(errmsg)
 
         return
 
     def member_ages(self, age_by_uid, subgroup_member_uids=None):
-        """
-        Return the ages of members in the layer group given the pop object.
-
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-            subgroup_member_uids (np.ndarray, list) : subgroup of uids to return ages for
-
-        Returns:
-            nd.ndarray : ages of members in group or subgroup
-        """
+        """Return the ages of members in the layer group given the pop object."""
         if len(age_by_uid) == 0:
             print("age_by_uid is empty. Returning an empty array for member_ages.")
             return np.array([])
 
         if subgroup_member_uids is None:
             return np.array(age_by_uid[self['member_uids']])
         else:
@@ -338,16 +329,15 @@
         aggregate_matrix = symmetric_matrix.copy()
         aggregate_matrix = sp.get_aggregate_matrix(aggregate_matrix, age_by_brackets)
 
         asymmetric_matrix = sp.get_asymmetric_matrix(aggregate_matrix, aggregate_age_count)
     """
     M = sc.dcp(symmetric_matrix)
     for a in aggregate_ages:
-        if aggregate_ages[a]:
-            M[a, :] = M[a, :] / float(aggregate_ages[a])
+        M[a, :] = M[a, :] / float(aggregate_ages[a])
 
     return M
 
 
 __all__ += ['get_bin_edges', 'get_bin_labels',
             'count_values', 'count_binned_values', 'binned_values_dist']
```

### Comparing `synthpops-1.10.5/synthpops/config.py` & `synthpops-1.8.0/synthpops/config.py`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/contact_networks.py` & `synthpops-1.8.0/synthpops/contact_networks.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import pandas as pd
 import networkx as nx
 from . import data_distributions as spdata
 from . import schools as spsch
 from .config import logger as log, checkmem
 
 
-def make_contacts(pop,
-                  age_by_uid,
+def make_contacts(age_by_uid,
                   homes_by_uids,
                   students_by_uid_lists=None,
                   teachers_by_uid_lists=None,
                   non_teaching_staff_uid_lists=None,
                   workplace_by_uid_lists=None,
                   facilities_by_uid_lists=None,
                   facilities_staff_uid_lists=None,
@@ -76,55 +75,32 @@
 
         If with_school_types==False, completely random schools will be generated with respect to the average_class_size,
         but other parameters such as average_additional_staff_degree will not be used.
     """
     log.debug('make_contacts_from_microstructure_objects()')
     popdict = {}
 
-    grade_age_mapping = {i: i + 5 for i in range(13)}
-    age_grade_mapping = {i + 5: i for i in range(13)}
+    grade_age_mapping = {i: i+5 for i in range(13)}
+    age_grade_mapping = {i+5: i for i in range(13)}
     age_grade_mapping[3] = 0
     age_grade_mapping[4] = 0
 
     # what are the school types by age
     school_type_by_age = sc.mergedicts(spdata.get_default_school_types_by_age_single(), school_type_by_age)
     school_types = list(set(school_type_by_age.values()))  # get the location specific school types whatever they may be
 
     # check school mixing type
     if isinstance(school_mixing_type, str):
         school_mixing_type_dic = dict.fromkeys(school_types, school_mixing_type)
     elif isinstance(school_mixing_type, dict):
         school_mixing_type_dic = sc.dcp(school_mixing_type)
         school_mixing_type_dic = sc.mergedicts(dict.fromkeys(school_types, 'random'), school_mixing_type_dic)  # if the dictionary given doesn't specify the mixing type for an expected school type, set the mixing type for that school type to random by default
 
-    age_and_class_clustered_flag = False
-    for school_type in school_mixing_type_dic:
-        if school_mixing_type_dic[school_type] == 'age_and_class_clustered':
-            age_and_class_clustered_flag = True
-
-    if not isinstance(average_class_size, dict):
-        average_class_size_by_mixing_type = dict.fromkeys(set(school_mixing_type_dic.values()), average_class_size)
-
-    else:
-        average_class_size_by_mixing_type = sc.dcp(average_class_size)
-        average_class_size_by_mixing_type = sc.mergedicts(dict.fromkeys(set(school_mixing_type_dic.values())), average_class_size_by_mixing_type)
-
-    if age_and_class_clustered_flag:
-        if average_class_size < average_student_teacher_ratio:
-            actual_classroom_size = max(average_class_size, average_student_teacher_ratio)
-            average_class_size_by_mixing_type['age_and_class_clustered'] = actual_classroom_size
-            warning_msg = f"average_class_size: {average_class_size} < average_student_teacher_ratio: {average_student_teacher_ratio}. \n In schools with mixing type 'age_and_class_clustered', synthpops will use the larger of the two to define the classroom sizes."
-            log.warning(warning_msg)
-
-    if len(list(average_class_size_by_mixing_type.keys())) > 1:
-        pop.average_class_size = average_class_size_by_mixing_type
-    else:
-        pop.average_class_size = list(average_class_size_by_mixing_type.values())[0]
-
-    uids = list(age_by_uid.keys())
+    uids = age_by_uid.keys()
+    uids = [uid for uid in uids]
 
     popdict = {}
     # also need to return schools as well and not just school contacts
     schools = {}
 
     # Handle trimming
     do_trim = max_contacts is not None
@@ -139,14 +115,15 @@
         layer_keys = ['H', 'S', 'W', 'C']
 
     log.debug('  starting...' + checkmem())
 
     # TODO: include age-based sex ratios
     sexes = np.random.randint(2, size=len(age_by_uid))
 
+
     for u, uid in enumerate(age_by_uid):
         popdict[uid] = {}
         popdict[uid]['age'] = int(age_by_uid[uid])
         popdict[uid]['sex'] = sexes[u]
         popdict[uid]['loc'] = None
         popdict[uid]['contacts'] = {}
         if use_ltcf:
@@ -226,16 +203,15 @@
             student_ages = [age_by_uid[i] for i in students]
             min_age = min(student_ages)
             this_school_type = school_type_by_age[min_age]
             this_school_mixing_type = school_mixing_type_dic[this_school_type]
             popdict, student_groups, teacher_groups = spsch.add_school_edges(popdict, students, student_ages,
                                                                              teachers, non_teaching_staff, age_by_uid,
                                                                              grade_age_mapping, age_grade_mapping,
-                                                                             average_class_size_by_mixing_type[this_school_mixing_type],
-                                                                             inter_grade_mixing,
+                                                                             average_class_size, inter_grade_mixing,
                                                                              average_student_teacher_ratio,
                                                                              average_teacher_teacher_degree,
                                                                              average_additional_staff_degree,
                                                                              this_school_mixing_type)
 
         else:
             school = students.copy() + teachers.copy() + non_teaching_staff.copy()
@@ -263,45 +239,42 @@
 
         for uid in non_teaching_staff:
             popdict[uid]['scid'] = ns
             popdict[uid]['sc_staff'] = 1
             popdict[uid]['sc_type'] = this_school_type
             popdict[uid]['sc_mixing_type'] = this_school_mixing_type
 
-    pop.schools_in_groups = schools
-
     log.debug('...workplaces ' + checkmem())
     if do_trim and 'W' in trim_keys:
 
         average_degree = max_contacts['W']
         for nw, workplace in enumerate(workplace_by_uid_lists):
             uids = np.array(workplace)
 
             G = random_graph_model(uids, average_degree)  # undirected graph
             for u, uid in enumerate(workplace):
                 v = list(G.neighbors(u))
 
                 popdict[uid]['contacts']['W'] = set(uids[v])
                 popdict[uid]['contacts']['W'].discard(uid)  # this shouldn't be needed
                 popdict[uid]['wpid'] = nw
-                if workplaces_by_industry_codes is not None: # pragma: no cover
+                if workplaces_by_industry_codes is not None:
                     popdict[uid]['wpindcode'] = int(workplaces_by_industry_codes[nw])
 
     else: # pragma: no cover
         for nw, workplace in enumerate(workplace_by_uid_lists):
-
             for uid in workplace:
                 popdict[uid]['contacts']['W'] = set(workplace)
                 popdict[uid]['contacts']['W'].remove(uid)
                 popdict[uid]['wpid'] = nw
                 if workplaces_by_industry_codes is not None:
                     popdict[uid]['wpindcode'] = int(workplaces_by_industry_codes[nw])
 
     log.debug('...done ' + checkmem())
-    return popdict
+    return popdict, schools
 
 
 def create_reduced_contacts_with_group_types(popdict, group_1, group_2, setting, average_degree=20, p_matrix=None, force_cross_edges=True):
     """
     Create contacts between members of group 1 and group 2, fixing the average degree, and the
     probability of an edge between any two groups controlled by p_matrix if provided.
     Forces inter group edge for each individual in group 1 with force_cross_groups equal to True.
@@ -331,15 +304,15 @@
         errormsg = f'This method is likely to create disconnected graphs with average_degree < 2. In order to keep the group connected, use a higher average_degree for nodes across the two groups.'
         raise ValueError(errormsg)
 
     r1 = [int(i) for i in group_1]
     r2 = [int(i) for i in group_2]
 
     n1 = list(np.arange(len(r1)).astype(int))
-    n2 = list(np.arange(len(r1), len(r1) + len(r2)).astype(int))
+    n2 = list(np.arange(len(r1), len(r1)+len(r2)).astype(int))
 
     group = r1 + r2
     sizes = [len(r1), len(r2)]
 
     for i in popdict:
         popdict[i]['contacts'].setdefault(setting, set())
 
@@ -352,23 +325,24 @@
         G = nx.complete_graph(len(group))
         for i in n1:
             group_1_neighbors = [j for j in G.neighbors(i) if j in n1]
 
             # if the person's degree is too high, cut out some contacts
             if len(group_1_neighbors) > average_degree:
                 ncut = len(group_1_neighbors) - average_degree  # rough number to cut
-
+                # ncut = spsamp.pt(ncut)  # sample from poisson that number
+                # ncut = min(len(group_1_neighbors), ncut)  # make sure the number isn't greater than the people available to cut
                 for k in range(ncut):
                     j = np.random.choice(group_1_neighbors)
                     G.remove_edge(i, j)
                     group_1_neighbors.remove(j)
 
     else:
         share_k_matrix = np.ones((2, 2))
-        share_k_matrix *= average_degree / np.sum(sizes)
+        share_k_matrix *= average_degree/np.sum(sizes)
 
         if p_matrix is None:
             p_matrix = share_k_matrix.copy()
 
         # create a graph with edges within each groups and between members of different groups using the probability matrix
         G = nx.stochastic_block_model(sizes, p_matrix)
 
@@ -490,29 +464,29 @@
                 'sc_teacher': len([c for c in person["contacts"]["S"] if popdict[c]['sc_teacher']]),
                 'sc_staff': len([c for c in person["contacts"]["S"] if popdict[c]['sc_staff']]),
                 'ltcf_res': len([c for c in person["contacts"]["LTCF"] if popdict[c]['ltcf_res']]),
                 'ltcf_staff': len([c for c in person["contacts"]["LTCF"] if popdict[c]['ltcf_staff']]),
                 'all_staff': len([c for c in person["contacts"]["S"] if popdict[c]['sc_teacher']]) + len([c for c in person["contacts"]["S"] if popdict[c]['sc_staff']]),
                 'all': len([c for c in person["contacts"][layer]])
             }
-
-            contacts_counter_by_id.setdefault(person[layer_keys[layer]], [])
-            for k1 in people_types:
-                # if this person does not belong to a particular key, we don't need to store the counts under this key
-                if person.get(k1) is not None:
-                    # store sc_teacher, sc_student, sc_staff, all_staff and all below
-                    if layer == "S":
-                        for k2 in people_types:
-                            index_switcher.get(k1)[k2].append(count_switcher.get(k2))
-                        index_switcher.get(k1)["all_staff"].append(
-                            count_switcher.get('sc_teacher') + count_switcher.get('sc_staff'))
-                    # for other types, only all contacts are stored
-                    index_switcher.get(k1)["all"].append(count_switcher.get('all'))
             if with_layer_ids:
-                contacts_counter_by_id[person[layer_keys[layer]]].append(count_switcher.get('all'))
+                contacts_counter_by_id.setdefault(person[layer_keys[layer]], [])
+                for k1 in people_types:
+                    # if this person does not belong to a particular key, we don't need to store the counts under this key
+                    if person.get(k1) is not None:
+                        # store sc_teacher, sc_student, sc_staff, all_staff and all below
+                        if layer == "S":
+                            for k2 in people_types:
+                                index_switcher.get(k1)[k2].append(count_switcher.get(k2))
+                            index_switcher.get(k1)["all_staff"].append(
+                                count_switcher.get('sc_teacher') + count_switcher.get('sc_staff'))
+                        # for other types, only all contacts are stored
+                        index_switcher.get(k1)["all"].append(count_switcher.get('all'))
+
+                    contacts_counter_by_id[person[layer_keys[layer]]].append(count_switcher.get('all'))
     if with_layer_ids:
         return contact_counter, contacts_counter_by_id
     else:
         return contact_counter
 
 
 def filter_people(pop, ages=None, uids=None):
```

### Comparing `synthpops-1.10.5/synthpops/data/MUestimates_all_locations.obj` & `synthpops-1.8.0/synthpops/data/MUestimates_all_locations.obj`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/data/MUestimates_home.obj` & `synthpops-1.8.0/synthpops/data/MUestimates_home.obj`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/data/MUestimates_other_locations.obj` & `synthpops-1.8.0/synthpops/data/MUestimates_other_locations.obj`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/data/MUestimates_school.obj` & `synthpops-1.8.0/synthpops/data/MUestimates_school.obj`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/data/MUestimates_work.obj` & `synthpops-1.8.0/synthpops/data/MUestimates_work.obj`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/data/Nepal.json` & `synthpops-1.8.0/synthpops/data/usa-Oregon-portland_metro.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6586580201387486%*

 * *Differences: {"'citations'": '[]',*

 * * "'employment_rates_by_age'": '{0: {insert: [(1, 0.323)], delete: [1]}, 1: {insert: [(1, 0.323)], '*

 * *                              'delete: [1]}, 2: {insert: [(1, 0.323)], delete: [1]}, 3: {insert: '*

 * *                              '[(1, 0.323)], delete: [1]}, 4: {insert: [(1, 0.731)], delete: [1]}, '*

 * *                              '5: {insert: [(1, 0.731)], delete: [1]}, 6: {insert: [(1, 0.731)], '*

 * *                              'delete: [1]}, 7: {insert: [(1, 0.731)], delete: [1]}, 8: {in […]*

```diff
@@ -1,417 +1,350 @@
 {
-    "citations": [
-        "SMALL AND MEDIUM-SIZED ENTERPRISES IN NEPAL: EXAMINING CONSTRAINTS ON EXPORTING, Paras Kharel and Kshitiz Dahal, 2020",
-        "Report on the Nepal Labour Force Survey 2017/18"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
-            0,
-            0.0
-        ],
-        [
-            1,
-            0.0
-        ],
-        [
-            2,
-            0.0
-        ],
-        [
-            3,
-            0.0
-        ],
-        [
-            4,
-            0.0
-        ],
-        [
-            5,
-            0.0
-        ],
-        [
-            6,
-            0.0
-        ],
-        [
-            7,
-            0.0
-        ],
-        [
-            8,
-            0.0
-        ],
-        [
-            9,
-            0.0
-        ],
-        [
-            10,
-            0.0
-        ],
-        [
-            11,
-            0.0
-        ],
-        [
-            12,
-            0.0
-        ],
-        [
-            13,
-            0.0
-        ],
-        [
-            14,
-            0.0
-        ],
-        [
-            15,
-            0.225
-        ],
-        [
             16,
-            0.225
+            0.323
         ],
         [
             17,
-            0.225
+            0.323
         ],
         [
             18,
-            0.225
+            0.323
         ],
         [
             19,
-            0.225
+            0.323
         ],
         [
             20,
-            0.225
+            0.731
         ],
         [
             21,
-            0.225
+            0.731
         ],
         [
             22,
-            0.225
+            0.731
         ],
         [
             23,
-            0.225
+            0.731
         ],
         [
             24,
-            0.225
+            0.731
         ],
         [
             25,
-            0.461
+            0.815
         ],
         [
             26,
-            0.461
+            0.815
         ],
         [
             27,
-            0.461
+            0.815
         ],
         [
             28,
-            0.461
+            0.815
         ],
         [
             29,
-            0.461
+            0.815
         ],
         [
             30,
-            0.461
+            0.805
         ],
         [
             31,
-            0.461
+            0.805
         ],
         [
             32,
-            0.461
+            0.805
         ],
         [
             33,
-            0.461
+            0.805
         ],
         [
             34,
-            0.461
+            0.805
         ],
         [
             35,
-            0.491
+            0.811
         ],
         [
             36,
-            0.491
+            0.811
         ],
         [
             37,
-            0.491
+            0.811
         ],
         [
             38,
-            0.491
+            0.811
         ],
         [
             39,
-            0.491
+            0.811
         ],
         [
             40,
-            0.491
+            0.811
         ],
         [
             41,
-            0.491
+            0.811
         ],
         [
             42,
-            0.491
+            0.811
         ],
         [
             43,
-            0.491
+            0.811
         ],
         [
             44,
-            0.491
+            0.811
         ],
         [
             45,
-            0.421
+            0.815
         ],
         [
             46,
-            0.421
+            0.815
         ],
         [
             47,
-            0.421
+            0.815
         ],
         [
             48,
-            0.421
+            0.815
         ],
         [
             49,
-            0.421
+            0.815
         ],
         [
             50,
-            0.421
+            0.815
         ],
         [
             51,
-            0.421
+            0.815
         ],
         [
             52,
-            0.421
+            0.815
         ],
         [
             53,
-            0.421
+            0.815
         ],
         [
             54,
-            0.421
+            0.815
         ],
         [
             55,
-            0.272
+            0.738
         ],
         [
             56,
-            0.272
+            0.738
         ],
         [
             57,
-            0.272
+            0.738
         ],
         [
             58,
-            0.272
+            0.738
         ],
         [
             59,
-            0.272
+            0.738
         ],
         [
             60,
-            0.272
+            0.587
         ],
         [
             61,
-            0.272
+            0.587
         ],
         [
             62,
-            0.272
+            0.587
         ],
         [
             63,
-            0.272
+            0.587
         ],
         [
             64,
-            0.272
+            0.587
         ],
         [
             65,
-            0.134
+            0.257
         ],
         [
             66,
-            0.134
+            0.257
         ],
         [
             67,
-            0.134
+            0.257
         ],
         [
             68,
-            0.134
+            0.257
         ],
         [
             69,
-            0.134
+            0.257
         ],
         [
             70,
-            0.134
+            0.257
         ],
         [
             71,
-            0.134
+            0.257
         ],
         [
             72,
-            0.134
+            0.257
         ],
         [
             73,
-            0.134
+            0.257
         ],
         [
             74,
-            0.134
+            0.257
         ],
         [
             75,
-            0.134
+            0.056
         ],
         [
             76,
-            0.0
+            0.056
         ],
         [
             77,
-            0.0
+            0.056
         ],
         [
             78,
-            0.0
+            0.056
         ],
         [
             79,
-            0.0
+            0.056
         ],
         [
             80,
-            0.0
+            0.056
         ],
         [
             81,
-            0.0
+            0.056
         ],
         [
             82,
-            0.0
+            0.056
         ],
         [
             83,
-            0.0
+            0.056
         ],
         [
             84,
-            0.0
+            0.056
         ],
         [
             85,
-            0.0
+            0.056
         ],
         [
             86,
-            0.0
+            0.056
         ],
         [
             87,
-            0.0
+            0.056
         ],
         [
             88,
-            0.0
+            0.056
         ],
         [
             89,
-            0.0
+            0.056
         ],
         [
             90,
-            0.0
+            0.056
         ],
         [
             91,
-            0.0
+            0.056
         ],
         [
             92,
-            0.0
+            0.056
         ],
         [
             93,
-            0.0
+            0.056
         ],
         [
             94,
-            0.0
+            0.056
         ],
         [
             95,
-            0.0
+            0.056
         ],
         [
             96,
-            0.0
+            0.056
         ],
         [
             97,
-            0.0
+            0.056
         ],
         [
             98,
-            0.0
+            0.056
         ],
         [
             99,
-            0.0
+            0.056
         ],
         [
             100,
-            0.0
+            0.056
         ]
     ],
     "enrollment_rates_by_age": [
         [
             0,
             0.0
         ],
@@ -421,203 +354,203 @@
         ],
         [
             2,
             0.0
         ],
         [
             3,
-            0.386
+            0.457
         ],
         [
             4,
-            0.65
+            0.457
         ],
         [
             5,
-            0.974
+            0.946
         ],
         [
             6,
-            0.972
+            0.946
         ],
         [
             7,
-            0.972
+            0.946
         ],
         [
             8,
-            0.972
+            0.946
         ],
         [
             9,
-            0.972
+            0.946
         ],
         [
             10,
-            0.972
+            0.98
         ],
         [
             11,
-            0.972
+            0.98
         ],
         [
             12,
-            0.874
+            0.98
         ],
         [
             13,
-            0.874
+            0.98
         ],
         [
             14,
-            0.874
+            0.98
         ],
         [
             15,
-            0.659
+            0.983
         ],
         [
             16,
-            0.659
+            0.983
         ],
         [
             17,
-            0.22
+            0.983
         ],
         [
             18,
-            0.22
+            0.707
         ],
         [
             19,
-            0.087
+            0.707
         ],
         [
             20,
-            0.087
+            0.343
         ],
         [
             21,
-            0.087
+            0.343
         ],
         [
             22,
-            0.087
+            0.343
         ],
         [
             23,
-            0.087
+            0.343
         ],
         [
             24,
-            0.087
+            0.343
         ],
         [
             25,
-            0.087
+            0.11
         ],
         [
             26,
-            0.0
+            0.11
         ],
         [
             27,
-            0.0
+            0.11
         ],
         [
             28,
-            0.0
+            0.11
         ],
         [
             29,
-            0.0
+            0.11
         ],
         [
             30,
-            0.0
+            0.11
         ],
         [
             31,
-            0.0
+            0.11
         ],
         [
             32,
-            0.0
+            0.11
         ],
         [
             33,
-            0.0
+            0.11
         ],
         [
             34,
-            0.0
+            0.11
         ],
         [
             35,
-            0.0
+            0.026
         ],
         [
             36,
-            0.0
+            0.026
         ],
         [
             37,
-            0.0
+            0.026
         ],
         [
             38,
-            0.0
+            0.026
         ],
         [
             39,
-            0.0
+            0.026
         ],
         [
             40,
-            0.0
+            0.026
         ],
         [
             41,
-            0.0
+            0.026
         ],
         [
             42,
-            0.0
+            0.026
         ],
         [
             43,
-            0.0
+            0.026
         ],
         [
             44,
-            0.0
+            0.026
         ],
         [
             45,
-            0.0
+            0.026
         ],
         [
             46,
-            0.0
+            0.026
         ],
         [
             47,
-            0.0
+            0.026
         ],
         [
             48,
-            0.0
+            0.026
         ],
         [
             49,
-            0.0
+            0.026
         ],
         [
             50,
-            0.0
+            0.026
         ],
         [
             51,
             0.0
         ],
         [
             52,
@@ -812,571 +745,386 @@
             0.0
         ],
         [
             100,
             0.0
         ]
     ],
-    "household_head_age_brackets": [
-        [
-            10,
-            14
-        ],
-        [
-            15,
-            19
-        ],
-        [
-            20,
-            24
-        ],
-        [
-            25,
-            29
-        ],
-        [
-            30,
-            34
-        ],
-        [
-            35,
-            39
-        ],
-        [
-            40,
-            44
-        ],
-        [
-            45,
-            49
-        ],
-        [
-            50,
-            54
-        ],
-        [
-            55,
-            59
-        ],
-        [
-            60,
-            64
-        ],
-        [
-            65,
-            100
-        ]
-    ],
-    "household_head_age_distribution_by_family_size": [
-        [
-            1,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            2,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            3,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            4,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            5,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            6,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            7,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            8,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            9,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ],
-        [
-            10,
-            4,
-            100,
-            365,
-            612,
-            746,
-            851,
-            788,
-            734,
-            625,
-            547,
-            454,
-            775
-        ]
-    ],
+    "household_head_age_brackets": [],
+    "household_head_age_distribution_by_family_size": [],
     "household_size_distribution": [
         [
             1,
-            0.064
+            0.2680756104789062
         ],
         [
             2,
-            0.149
+            0.3602629255864462
         ],
         [
             3,
-            0.191
+            0.1498083139692569
         ],
         [
             4,
-            0.207
+            0.1309842326328058
         ],
         [
             5,
-            0.159
+            0.0551800256977612
         ],
         [
             6,
-            0.102
+            0.0212210730019572
         ],
         [
             7,
-            0.059
-        ],
-        [
-            8,
-            0.03
-        ],
-        [
-            9,
-            0.0195
-        ],
-        [
-            10,
-            0.0195
+            0.0144678186328665
         ]
     ],
-    "location_name": "Nepal",
+    "location_name": "usa-Oregon-portland_metro",
     "ltcf_num_residents_distribution": [],
     "ltcf_num_staff_distribution": [],
     "ltcf_resident_to_staff_ratio_distribution": [],
     "ltcf_use_rate_distribution": [],
-    "notes": [
-        "School size range estimated from average sizes across school types from Education in Figures 2017 (At A Glance) "
-    ],
-    "parent": null,
+    "notes": [],
+    "parent": "usa-Oregon.json",
     "population_age_distributions": [
         {
             "distribution": [
                 [
                     0,
                     4,
-                    0.09459338158296804
+                    0.0569375666600511
                 ],
                 [
                     5,
                     9,
-                    0.09695157915871368
+                    0.0593336979970924
                 ],
                 [
                     10,
                     14,
-                    0.10402858373850708
+                    0.0614059078756077
                 ],
                 [
                     15,
                     19,
-                    0.11289102334344704
+                    0.0587895260823333
                 ],
                 [
                     20,
                     24,
-                    0.11035987147132863
+                    0.0574821419639241
                 ],
                 [
                     25,
                     29,
-                    0.08765000761656047
+                    0.0773071033595859
                 ],
                 [
                     30,
                     34,
-                    0.06802822384816039
+                    0.077707668749768
                 ],
                 [
                     35,
                     39,
-                    0.058799567152861186
+                    0.0753853576205851
                 ],
                 [
                     40,
                     44,
-                    0.05447462615761058
+                    0.0715765576063858
                 ],
                 [
                     45,
                     49,
-                    0.04892757500389567
+                    0.0694051140058314
                 ],
                 [
                     50,
                     54,
-                    0.042625648954371036
+                    0.062004537320754
                 ],
                 [
                     55,
                     59,
-                    0.03495784536138185
+                    0.0634555279637402
                 ],
                 [
                     60,
                     64,
-                    0.02788594412178052
+                    0.0604071164293932
                 ],
                 [
                     65,
                     69,
-                    0.02256749464516301
+                    0.0531376412063593
                 ],
                 [
                     70,
                     74,
-                    0.01621827531289942
+                    0.0388387072831098
                 ],
                 [
                     75,
-                    79,
-                    0.011459165903088129
+                    100,
+                    0.0568258278754786
+                ]
+            ],
+            "num_bins": 16
+        },
+        {
+            "distribution": [
+                [
+                    0,
+                    4,
+                    0.0569375666600511
                 ],
                 [
-                    80,
-                    84,
-                    0.005052027155082888
+                    5,
+                    9,
+                    0.0593336979970924
                 ],
                 [
-                    85,
-                    89,
-                    0.0019225610770200996
+                    10,
+                    14,
+                    0.0614059078756077
                 ],
                 [
-                    90,
-                    94,
-                    0.0005245954082382032
+                    15,
+                    19,
+                    0.0587895260823333
                 ],
                 [
-                    95,
-                    99,
-                    7.878718351338686e-05
+                    20,
+                    24,
+                    0.0574821419639241
                 ],
                 [
+                    25,
+                    29,
+                    0.0773071033595859
+                ],
+                [
+                    30,
+                    34,
+                    0.077707668749768
+                ],
+                [
+                    35,
+                    39,
+                    0.0753853576205851
+                ],
+                [
+                    40,
+                    44,
+                    0.0715765576063858
+                ],
+                [
+                    45,
+                    49,
+                    0.0694051140058314
+                ],
+                [
+                    50,
+                    54,
+                    0.062004537320754
+                ],
+                [
+                    55,
+                    59,
+                    0.0634555279637402
+                ],
+                [
+                    60,
+                    64,
+                    0.0604071164293932
+                ],
+                [
+                    65,
+                    69,
+                    0.0531376412063593
+                ],
+                [
+                    70,
+                    74,
+                    0.0388387072831098
+                ],
+                [
+                    75,
+                    79,
+                    0.0251146028472817
+                ],
+                [
+                    80,
+                    84,
+                    0.0156502874550826
+                ],
+                [
+                    85,
                     100,
-                    100,
-                    3.2158034087096678e-06
+                    0.0160609375731143
                 ]
             ],
-            "num_bins": 21
+            "num_bins": 18
         },
         {
             "distribution": [
                 [
                     0,
                     4,
-                    0.09459338158296804
+                    0.0569375666600511
                 ],
                 [
                     5,
                     9,
-                    0.09695157915871368
+                    0.0593336979970924
                 ],
                 [
                     10,
                     14,
-                    0.10402858373850708
+                    0.0614059078756077
                 ],
                 [
                     15,
                     19,
-                    0.11289102334344704
+                    0.0587895260823333
                 ],
                 [
                     20,
                     24,
-                    0.11035987147132863
+                    0.0574821419639241
                 ],
                 [
                     25,
                     29,
-                    0.08765000761656047
+                    0.0773071033595859
                 ],
                 [
                     30,
                     34,
-                    0.06802822384816039
+                    0.077707668749768
                 ],
                 [
                     35,
                     39,
-                    0.058799567152861186
+                    0.0753853576205851
                 ],
                 [
                     40,
                     44,
-                    0.05447462615761058
+                    0.0715765576063858
                 ],
                 [
                     45,
                     49,
-                    0.04892757500389567
+                    0.0694051140058314
                 ],
                 [
                     50,
                     54,
-                    0.042625648954371036
+                    0.062004537320754
                 ],
                 [
                     55,
                     59,
-                    0.03495784536138185
+                    0.0634555279637402
                 ],
                 [
                     60,
                     64,
-                    0.02788594412178052
+                    0.0604071164293932
                 ],
                 [
                     65,
                     69,
-                    0.02256749464516301
+                    0.0531376412063593
                 ],
                 [
                     70,
                     74,
-                    0.01621827531289942
+                    0.0388387072831098
                 ],
                 [
                     75,
+                    79,
+                    0.0251146028472817
+                ],
+                [
+                    80,
+                    84,
+                    0.0156502874550826
+                ],
+                [
+                    85,
+                    89,
+                    0.0107072917154095
+                ],
+                [
+                    90,
+                    94,
+                    0.0044613715480873
+                ],
+                [
+                    95,
                     100,
-                    0.019040352530351412
+                    0.0008922743096175
                 ]
             ],
-            "num_bins": 16
-        }
-    ],
-    "reference_links": [
-        "https://opendatanepal.com/dataset?res_format=CSV&organization=ministry-of-education",
-        "https://opendatanepal.com/dataset/university-wise-student-enrollment-of-higher-education-by-types-of-campuses/resource/5193053a-b6fe-45e7-a6ba-8aae99ced378",
-        "https://www.unicef.org/nepal/sites/unicef.org.nepal/files/2020-08/Nepal%20ECED%20Costing%20Study.pdf"
-    ],
-    "school_size_brackets": [
-        [
-            80,
-            200
-        ]
-    ],
-    "school_size_distribution": [
-        1.0
-    ],
-    "school_size_distribution_by_type": [
-        {
-            "school_type": "ms",
-            "size_distribution": [
-                1.0
-            ]
-        },
-        {
-            "school_type": "hs",
-            "size_distribution": [
-                1.0
-            ]
-        },
-        {
-            "school_type": "uv",
-            "size_distribution": [
-                1.0
-            ]
-        },
-        {
-            "school_type": "pk",
-            "size_distribution": [
-                1.0
-            ]
-        },
-        {
-            "school_type": "es",
-            "size_distribution": [
-                1.0
-            ]
-        },
-        {
-            "school_type": "ss",
-            "size_distribution": [
-                1.0
-            ]
-        }
-    ],
-    "school_types_by_age": [
-        {
-            "age_range": [
-                3,
-                5
-            ],
-            "school_type": "pk"
-        },
-        {
-            "age_range": [
-                6,
-                11
-            ],
-            "school_type": "es"
-        },
-        {
-            "age_range": [
-                12,
-                14
-            ],
-            "school_type": "ms"
-        },
-        {
-            "age_range": [
-                15,
-                16
-            ],
-            "school_type": "ss"
-        },
-        {
-            "age_range": [
-                17,
-                18
-            ],
-            "school_type": "hs"
-        },
-        {
-            "age_range": [
-                19,
-                100
-            ],
-            "school_type": "uv"
+            "num_bins": 20
         }
     ],
+    "reference_links": [],
+    "school_size_brackets": [],
+    "school_size_distribution": [],
+    "school_size_distribution_by_type": [],
+    "school_types_by_age": [],
     "workplace_size_counts_by_num_personnel": [
         [
+            1,
+            4,
+            38590.0
+        ],
+        [
             5,
+            9,
+            13155.0
+        ],
+        [
+            10,
             19,
-            0.9773
+            9181.0
         ],
         [
             20,
+            49,
+            6476.0
+        ],
+        [
+            50,
             99,
-            0.0157
+            2083.0
         ],
         [
             100,
-            199,
-            0.007
+            249,
+            1106.0
+        ],
+        [
+            250,
+            499,
+            299.0
+        ],
+        [
+            500,
+            999,
+            81.0
+        ],
+        [
+            1000,
+            1999,
+            59.0
         ]
     ]
 }
```

### Comparing `synthpops-1.10.5/synthpops/data/Senegal-Dakar.json` & `synthpops-1.8.0/synthpops/data/usa-Oregon.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.724904227524837%*

 * *Differences: {"'citations'": '[]',*

 * * "'employment_rates_by_age'": '{0: {insert: [(1, 0.323)], delete: [1]}, 1: {insert: [(1, 0.323)], '*

 * *                              'delete: [1]}, 2: {insert: [(1, 0.323)], delete: [1]}, 3: {insert: '*

 * *                              '[(1, 0.323)], delete: [1]}, 4: {insert: [(1, 0.694)], delete: [1]}, '*

 * *                              '5: {insert: [(1, 0.694)], delete: [1]}, 6: {insert: [(1, 0.694)], '*

 * *                              'delete: [1]}, 7: {insert: [(1, 0.694)], delete: [1]}, 8: {in […]*

```diff
@@ -1,421 +1,350 @@
 {
-    "citations": [
-        "Situation des Enfants et des Femmes Dakar Urbain 2015-2016, Agence Nationale de la Statistique et de la Demographie",
-        "Situation Economique et Social du Senegal en 2015, Agence Nationale de la Statistique et de la Demographie (2015)",
-        "Agence Nationale de la Statistique et de la D\u00e9mographie - ANSD/S\u00e9n\u00e9gal, et ICF. 2018. S\u00e9n\u00e9gal : Enqu\u00eate D\u00e9mographique et de Sant\u00e9 Continue - EDS-Continue 2017. Rockville, Maryland, USA : ANSD et ICF.",
-        "Oswald Koussihouede. Three Essays in the Economics of Education. Economics and Finance. Universit\u00e9 Gaston Berger, 2015. English. tel-01150504v2",
-        "Recensement G\u00e9n\u00e9ral des Entreprises (2016)",
-        "Diagnostic de l\u2019\u00c9conomie Informelle au S\u00e9n\u00e9gal"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
-            0,
-            0.0
-        ],
-        [
-            1,
-            0.0
-        ],
-        [
-            2,
-            0.0
-        ],
-        [
-            3,
-            0.0
-        ],
-        [
-            4,
-            0.0
-        ],
-        [
-            5,
-            0.0
-        ],
-        [
-            6,
-            0.0
-        ],
-        [
-            7,
-            0.0
-        ],
-        [
-            8,
-            0.0
-        ],
-        [
-            9,
-            0.0
-        ],
-        [
-            10,
-            0.0
-        ],
-        [
-            11,
-            0.0
-        ],
-        [
-            12,
-            0.0
-        ],
-        [
-            13,
-            0.0
-        ],
-        [
-            14,
-            0.0
-        ],
-        [
-            15,
-            0.273
-        ],
-        [
             16,
-            0.273
+            0.323
         ],
         [
             17,
-            0.273
+            0.323
         ],
         [
             18,
-            0.273
+            0.323
         ],
         [
             19,
-            0.273
+            0.323
         ],
         [
             20,
-            0.359
+            0.694
         ],
         [
             21,
-            0.359
+            0.694
         ],
         [
             22,
-            0.359
+            0.694
         ],
         [
             23,
-            0.359
+            0.694
         ],
         [
             24,
-            0.359
+            0.694
         ],
         [
             25,
-            0.47
+            0.793
         ],
         [
             26,
-            0.47
+            0.793
         ],
         [
             27,
-            0.47
+            0.793
         ],
         [
             28,
-            0.47
+            0.793
         ],
         [
             29,
-            0.47
+            0.793
         ],
         [
             30,
-            0.615
+            0.787
         ],
         [
             31,
-            0.615
+            0.787
         ],
         [
             32,
-            0.615
+            0.787
         ],
         [
             33,
-            0.615
+            0.787
         ],
         [
             34,
-            0.615
+            0.787
         ],
         [
             35,
-            0.645
+            0.799
         ],
         [
             36,
-            0.645
+            0.799
         ],
         [
             37,
-            0.645
+            0.799
         ],
         [
             38,
-            0.645
+            0.799
         ],
         [
             39,
-            0.645
+            0.799
         ],
         [
             40,
-            0.595
+            0.799
         ],
         [
             41,
-            0.595
+            0.799
         ],
         [
             42,
-            0.595
+            0.799
         ],
         [
             43,
-            0.595
+            0.799
         ],
         [
             44,
-            0.595
+            0.799
         ],
         [
             45,
-            0.589
+            0.794
         ],
         [
             46,
-            0.589
+            0.794
         ],
         [
             47,
-            0.589
+            0.794
         ],
         [
             48,
-            0.589
+            0.794
         ],
         [
             49,
-            0.589
+            0.794
         ],
         [
             50,
-            0.589
+            0.794
         ],
         [
             51,
-            0.589
+            0.794
         ],
         [
             52,
-            0.589
+            0.794
         ],
         [
             53,
-            0.589
+            0.794
         ],
         [
             54,
-            0.589
+            0.794
         ],
         [
             55,
-            0.568
+            0.691
         ],
         [
             56,
-            0.568
+            0.691
         ],
         [
             57,
-            0.568
+            0.691
         ],
         [
             58,
-            0.568
+            0.691
         ],
         [
             59,
-            0.568
+            0.691
         ],
         [
             60,
-            0.438
+            0.552
         ],
         [
             61,
-            0.438
+            0.552
         ],
         [
             62,
-            0.438
+            0.552
         ],
         [
             63,
-            0.438
+            0.552
         ],
         [
             64,
-            0.438
+            0.552
         ],
         [
             65,
-            0.331
+            0.233
         ],
         [
             66,
-            0.331
+            0.233
         ],
         [
             67,
-            0.331
+            0.233
         ],
         [
             68,
-            0.331
+            0.233
         ],
         [
             69,
-            0.331
+            0.233
         ],
         [
             70,
-            0.252
+            0.233
         ],
         [
             71,
-            0.252
+            0.233
         ],
         [
             72,
-            0.252
+            0.233
         ],
         [
             73,
-            0.252
+            0.233
         ],
         [
             74,
-            0.252
+            0.233
         ],
         [
             75,
-            0.172
+            0.06
         ],
         [
             76,
-            0.172
+            0.06
         ],
         [
             77,
-            0.172
+            0.06
         ],
         [
             78,
-            0.172
+            0.06
         ],
         [
             79,
-            0.172
+            0.06
         ],
         [
             80,
-            0.071
+            0.06
         ],
         [
             81,
-            0.071
+            0.06
         ],
         [
             82,
-            0.071
+            0.06
         ],
         [
             83,
-            0.071
+            0.06
         ],
         [
             84,
-            0.071
+            0.06
         ],
         [
             85,
-            0.058
+            0.06
         ],
         [
             86,
-            0.058
+            0.06
         ],
         [
             87,
-            0.058
+            0.06
         ],
         [
             88,
-            0.058
+            0.06
         ],
         [
             89,
-            0.058
+            0.06
         ],
         [
             90,
-            0.058
+            0.06
         ],
         [
             91,
-            0.058
+            0.06
         ],
         [
             92,
-            0.058
+            0.06
         ],
         [
             93,
-            0.058
+            0.06
         ],
         [
             94,
-            0.058
+            0.06
         ],
         [
             95,
-            0.058
+            0.06
         ],
         [
             96,
-            0.058
+            0.06
         ],
         [
             97,
-            0.058
+            0.06
         ],
         [
             98,
-            0.058
+            0.06
         ],
         [
             99,
-            0.058
+            0.06
         ],
         [
             100,
-            0.058
+            0.06
         ]
     ],
     "enrollment_rates_by_age": [
         [
             0,
             0.0
         ],
@@ -425,203 +354,203 @@
         ],
         [
             2,
             0.0
         ],
         [
             3,
-            0.0
+            0.439
         ],
         [
             4,
-            0.0
+            0.439
         ],
         [
             5,
-            0.328
+            0.941
         ],
         [
             6,
-            0.416
+            0.941
         ],
         [
             7,
-            0.628
+            0.941
         ],
         [
             8,
-            0.728
+            0.941
         ],
         [
             9,
-            0.833
+            0.941
         ],
         [
             10,
-            0.819
+            0.975
         ],
         [
             11,
-            0.85
+            0.975
         ],
         [
             12,
-            0.827
+            0.975
         ],
         [
             13,
-            0.822
+            0.975
         ],
         [
             14,
-            0.76
+            0.975
         ],
         [
             15,
-            0.681
+            0.97
         ],
         [
             16,
-            0.678
+            0.97
         ],
         [
             17,
-            0.617
+            0.97
         ],
         [
             18,
-            0.574
+            0.71
         ],
         [
             19,
-            0.479
+            0.71
         ],
         [
             20,
-            0.441
+            0.366
         ],
         [
             21,
-            0.404
+            0.366
         ],
         [
             22,
-            0.379
+            0.366
         ],
         [
             23,
-            0.311
+            0.366
         ],
         [
             24,
-            0.365
+            0.366
         ],
         [
             25,
-            0.0
+            0.11
         ],
         [
             26,
-            0.0
+            0.11
         ],
         [
             27,
-            0.0
+            0.11
         ],
         [
             28,
-            0.0
+            0.11
         ],
         [
             29,
-            0.0
+            0.11
         ],
         [
             30,
-            0.0
+            0.11
         ],
         [
             31,
-            0.0
+            0.11
         ],
         [
             32,
-            0.0
+            0.11
         ],
         [
             33,
-            0.0
+            0.11
         ],
         [
             34,
-            0.0
+            0.11
         ],
         [
             35,
-            0.0
+            0.024
         ],
         [
             36,
-            0.0
+            0.024
         ],
         [
             37,
-            0.0
+            0.024
         ],
         [
             38,
-            0.0
+            0.024
         ],
         [
             39,
-            0.0
+            0.024
         ],
         [
             40,
-            0.0
+            0.024
         ],
         [
             41,
-            0.0
+            0.024
         ],
         [
             42,
-            0.0
+            0.024
         ],
         [
             43,
-            0.0
+            0.024
         ],
         [
             44,
-            0.0
+            0.024
         ],
         [
             45,
-            0.0
+            0.024
         ],
         [
             46,
-            0.0
+            0.024
         ],
         [
             47,
-            0.0
+            0.024
         ],
         [
             48,
-            0.0
+            0.024
         ],
         [
             49,
-            0.0
+            0.024
         ],
         [
             50,
-            0.0
+            0.024
         ],
         [
             51,
             0.0
         ],
         [
             52,
@@ -818,15 +747,15 @@
         [
             100,
             0.0
         ]
     ],
     "household_head_age_brackets": [
         [
-            15,
+            18,
             19
         ],
         [
             20,
             24
         ],
         [
@@ -851,366 +780,126 @@
         ],
         [
             50,
             54
         ],
         [
             55,
-            59
-        ],
-        [
-            60,
             64
         ],
         [
             65,
-            69
-        ],
-        [
-            70,
             74
         ],
         [
             75,
-            79
-        ],
-        [
-            80,
-            100
+            99
         ]
     ],
     "household_head_age_distribution_by_family_size": [
         [
             1,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0
         ],
         [
             2,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
+            163.0,
+            999.0,
+            2316.0,
+            2230.0,
+            1880.0,
+            1856.0,
+            2390.0,
+            3118.0,
+            9528.0,
+            9345.0,
+            5584.0
         ],
         [
             3,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
+            115.0,
+            757.0,
+            1545.0,
+            1907.0,
+            2066.0,
+            1811.0,
+            2028.0,
+            2175.0,
+            3311.0,
+            1587.0,
+            588.0
         ],
         [
             4,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
+            135.0,
+            442.0,
+            1029.0,
+            1951.0,
+            2670.0,
+            2547.0,
+            2368.0,
+            1695.0,
+            1763.0,
+            520.0,
+            221.0
         ],
         [
             5,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
+            61.0,
+            172.0,
+            394.0,
+            905.0,
+            1429.0,
+            1232.0,
+            969.0,
+            683.0,
+            623.0,
+            235.0,
+            94.0
         ],
         [
             6,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
+            25.0,
+            81.0,
+            153.0,
+            352.0,
+            511.0,
+            459.0,
+            372.0,
+            280.0,
+            280.0,
+            113.0,
+            49.0
         ],
         [
             7,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
+            24.0,
+            33.0,
+            63.0,
+            144.0,
             279.0,
-            270.0
+            242.0,
+            219.0,
+            115.0,
+            157.0,
+            80.0,
+            16.0
         ],
         [
             8,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            9,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            10,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            11,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            12,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            13,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            14,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            15,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            16,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            17,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            18,
-            19.0,
-            142.0,
-            297.0,
-            614.0,
-            823.0,
-            941.0,
-            933.0,
-            955.0,
-            954.0,
-            944.0,
-            723.0,
-            481.0,
-            279.0,
-            270.0
-        ],
-        [
-            19,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0
-        ],
-        [
-            20,
-            0.0,
-            0.0,
-            0.0,
             0.0,
             0.0,
             0.0,
             0.0,
             0.0,
             0.0,
             0.0,
@@ -1219,387 +908,276 @@
             0.0,
             0.0
         ]
     ],
     "household_size_distribution": [
         [
             1,
-            0.108
+            0.281380808947999
         ],
         [
             2,
-            0.088
+            0.3765260538684283
         ],
         [
             3,
-            0.092
+            0.1437503940941655
         ],
         [
             4,
-            0.085
+            0.1148184256605018
         ],
         [
             5,
-            0.103
+            0.0498735260878212
         ],
         [
             6,
-            0.104
+            0.0195125115803055
         ],
         [
             7,
-            0.076
-        ],
-        [
-            8,
-            0.0559999999999999
-        ],
-        [
-            9,
-            0.05
-        ],
-        [
-            10,
-            0.0264444444444444
-        ],
-        [
-            11,
-            0.0264444444444444
-        ],
-        [
-            12,
-            0.0264444444444444
-        ],
-        [
-            13,
-            0.0264444444444444
-        ],
-        [
-            14,
-            0.0264444444444444
-        ],
-        [
-            15,
-            0.0264444444444444
-        ],
-        [
-            16,
-            0.0264444444444444
-        ],
-        [
-            17,
-            0.0264444444444444
-        ],
-        [
-            18,
-            0.0264444444444444
+            0.0141382797607788
         ]
     ],
-    "location_name": "Senegal-Dakar",
+    "location_name": "usa-Oregon",
     "ltcf_num_residents_distribution": [],
     "ltcf_num_staff_distribution": [],
     "ltcf_resident_to_staff_ratio_distribution": [],
     "ltcf_use_rate_distribution": [],
-    "notes": [
-        "Employment rates are taken from Figure 3.12 of 3-SES-2015_Emploi.pdf",
-        "Enrollment rates for Urban Dakar are taken from the Situation des Enfants at des Femmes Dakar Urbain 2015-2016, Table ED.4 and Table ED.5",
-        "Age of head of household taken from Table 2.12 of Senegal Enquete Demographique et de Sante Continue 2017"
-    ],
-    "parent": "Senegal.json",
+    "notes": [],
+    "parent": "usa.json",
     "population_age_distributions": [
         {
             "distribution": [
                 [
                     0,
                     4,
-                    0.12
+                    0.0529582569989547
+                ],
+                [
+                    5,
+                    9,
+                    0.0558095490543863
+                ],
+                [
+                    10,
+                    14,
+                    0.0604326443303601
+                ],
+                [
+                    15,
+                    19,
+                    0.0592331859478199
+                ],
+                [
+                    20,
+                    24,
+                    0.0631016111246386
+                ],
+                [
+                    25,
+                    29,
+                    0.0702732294593048
+                ],
+                [
+                    30,
+                    34,
+                    0.0706992873192425
+                ],
+                [
+                    35,
+                    39,
+                    0.0721768569258823
+                ],
+                [
+                    40,
+                    44,
+                    0.065064037895203
+                ],
+                [
+                    45,
+                    49,
+                    0.0622025507991608
+                ],
+                [
+                    50,
+                    54,
+                    0.0589574456633972
+                ],
+                [
+                    55,
+                    59,
+                    0.0616100529739052
+                ],
+                [
+                    60,
+                    64,
+                    0.0655126196820712
+                ],
+                [
+                    65,
+                    69,
+                    0.0604741357747057
+                ],
+                [
+                    70,
+                    74,
+                    0.0503101544738328
+                ],
+                [
+                    75,
+                    100,
+                    0.0711843815771348
+                ]
+            ],
+            "num_bins": 16
+        },
+        {
+            "distribution": [
+                [
+                    0,
+                    4,
+                    0.0529582569989547
                 ],
                 [
                     5,
                     9,
-                    0.117
+                    0.0558095490543863
                 ],
                 [
                     10,
                     14,
-                    0.105
+                    0.0604326443303601
                 ],
                 [
                     15,
                     19,
-                    0.098
+                    0.0592331859478199
                 ],
                 [
                     20,
                     24,
-                    0.096
+                    0.0631016111246386
                 ],
                 [
                     25,
                     29,
-                    0.1
+                    0.0702732294593048
                 ],
                 [
                     30,
                     34,
-                    0.083
+                    0.0706992873192425
                 ],
                 [
                     35,
                     39,
-                    0.065
+                    0.0721768569258823
                 ],
                 [
                     40,
                     44,
-                    0.051
+                    0.065064037895203
                 ],
                 [
                     45,
                     49,
-                    0.039
+                    0.0622025507991608
                 ],
                 [
                     50,
                     54,
-                    0.037
+                    0.0589574456633972
                 ],
                 [
                     55,
                     59,
-                    0.029
+                    0.0616100529739052
                 ],
                 [
                     60,
                     64,
-                    0.024
+                    0.0655126196820712
                 ],
                 [
                     65,
                     69,
-                    0.014
+                    0.0604741357747057
                 ],
                 [
                     70,
                     74,
-                    0.009
+                    0.0503101544738328
                 ],
                 [
                     75,
                     79,
-                    0.005
+                    0.0314016734566427
                 ],
                 [
                     80,
                     84,
-                    0.003
+                    0.0194668373110983
                 ],
                 [
                     85,
                     100,
-                    0.002
+                    0.0203158708093938
                 ]
             ],
             "num_bins": 18
         }
     ],
-    "reference_links": [
-        "https://microdata.worldbank.org/index.php/catalog/3485/related-materials",
-        "https://www.ansd.sn/ressources/ses/chapitres/3-SES-2015_Emploi.pdf",
-        "https://dhsprogram.com/publications/publication-fr345-dhs-final-reports.cfm",
-        "https://hal.archives-ouvertes.fr/tel-01150504v2",
-        "https://labordoc.ilo.org/permalink/41ILO_INST/8s7mv9/alma995060592602676"
-    ],
-    "school_size_brackets": [
-        [
-            1,
-            50
-        ],
-        [
-            51,
-            100
-        ],
-        [
-            101,
-            150
-        ],
-        [
-            151,
-            200
-        ],
-        [
-            201,
-            250
-        ],
-        [
-            251,
-            300
-        ],
-        [
-            301,
-            350
-        ],
-        [
-            351,
-            400
-        ],
-        [
-            401,
-            450
-        ],
-        [
-            451,
-            500
-        ],
-        [
-            501,
-            550
-        ],
-        [
-            551,
-            600
-        ],
-        [
-            601,
-            650
-        ],
-        [
-            651,
-            700
-        ],
-        [
-            701,
-            750
-        ],
-        [
-            751,
-            800
-        ],
-        [
-            801,
-            850
-        ],
-        [
-            851,
-            900
-        ],
-        [
-            901,
-            950
-        ],
-        [
-            951,
-            1000
-        ],
-        [
-            1001,
-            1050
-        ],
-        [
-            1051,
-            1100
-        ],
-        [
-            1101,
-            1150
-        ],
-        [
-            1151,
-            1200
-        ],
-        [
-            1201,
-            1250
-        ],
-        [
-            1251,
-            1300
-        ],
-        [
-            1301,
-            1350
-        ],
-        [
-            1351,
-            1400
-        ],
-        [
-            1401,
-            1450
-        ],
-        [
-            1451,
-            1500
-        ]
-    ],
-    "school_size_distribution": [
-        0.0005815478337687009,
-        0.01835940275780583,
-        0.0635747895238934,
-        0.10169149618283796,
-        0.11744784766543039,
-        0.11563180990469378,
-        0.10441112788950066,
-        0.08969433263925763,
-        0.0747934858777752,
-        0.0612579058867474,
-        0.04963768861256398,
-        0.03997831246432716,
-        0.03210122607155025,
-        0.025750590629679243,
-        0.02066431514967983,
-        0.016604773260983325,
-        0.013369132350536621,
-        0.010790015246155117,
-        0.008732051802965215,
-        0.0070870856388488114,
-        0.005769331729045209,
-        0.004711028314792407,
-        0.003858755472712506,
-        0.003170420213112805,
-        0.002612836544499304,
-        0.0021598071042468036,
-        0.0017906140158152027,
-        0.0014888370537154024,
-        0.001241430358247502,
-        0.0010380018048123014
-    ],
+    "reference_links": [],
+    "school_size_brackets": [],
+    "school_size_distribution": [],
     "school_size_distribution_by_type": [],
     "school_types_by_age": [],
     "workplace_size_counts_by_num_personnel": [
         [
             1,
-            1,
-            0.61
-        ],
-        [
-            2,
             4,
-            0.339
+            64238.0
         ],
         [
             5,
             9,
-            0.035
+            22845.0
         ],
         [
             10,
             19,
-            0.008
+            15743.0
         ],
         [
             20,
             49,
-            0.003
+            10413.0
         ],
         [
             50,
             99,
-            0.003
+            3079.0
         ],
         [
             100,
             249,
-            0.002
+            1646.0
+        ],
+        [
+            250,
+            499,
+            426.0
+        ],
+        [
+            500,
+            999,
+            118.0
+        ],
+        [
+            1000,
+            1999,
+            78.0
         ]
     ]
 }
```

### Comparing `synthpops-1.10.5/synthpops/data/Senegal.json` & `synthpops-1.8.0/synthpops/data/Senegal.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'citations'": '[]', "'notes'": '[]', "'reference_links'": '[]'}*

```diff
@@ -1,14 +1,9 @@
 {
-    "citations": [
-        "Situation Economique et Social du Senegal en 2015, Agence Nationale de la Statistique et de la Demographie (2015)",
-        "Oswald Koussihouede. Three Essays in the Economics of Education. Economics and Finance. Universit\u00e9 Gaston Berger, 2015. English. tel-01150504v2",
-        "Recensement G\u00e9n\u00e9ral des Entreprises (2016)",
-        "Diagnostic de l\u2019\u00c9conomie Informelle au S\u00e9n\u00e9gal"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
             0,
             0.0
         ],
         [
@@ -417,24 +412,18 @@
     "household_head_age_distribution_by_family_size": [],
     "household_size_distribution": [],
     "location_name": "Senegal",
     "ltcf_num_residents_distribution": [],
     "ltcf_num_staff_distribution": [],
     "ltcf_resident_to_staff_ratio_distribution": [],
     "ltcf_use_rate_distribution": [],
-    "notes": [
-        "Employment rates are taken from Figure 3.12 of 3-SES-2015_Emploi.pdf"
-    ],
+    "notes": [],
     "parent": "",
     "population_age_distributions": [],
-    "reference_links": [
-        "https://www.ansd.sn/ressources/ses/chapitres/3-SES-2015_Emploi.pdf",
-        "https://hal.archives-ouvertes.fr/tel-01150504v2",
-        "https://labordoc.ilo.org/permalink/41ILO_INST/8s7mv9/alma995060592602676"
-    ],
+    "reference_links": [],
     "school_size_brackets": [
         [
             1,
             50
         ],
         [
             51,
```

### Comparing `synthpops-1.10.5/synthpops/data/usa-Washington-Franklin_County.json` & `synthpops-1.8.0/synthpops/data/usa-Washington-Franklin_County.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9047619047619048%*

 * *Differences: {"'citations'": '[]',*

 * * "'ltcf_use_rate_distribution'": '[[0, 0.0], [1, 0.0], [2, 0.0], [3, 0.0], [4, 0.0], [5, 0.0], [6, '*

 * *                                 '0.0], [7, 0.0], [8, 0.0], [9, 0.0], [10, 0.0], [11, 0.0], [12, '*

 * *                                 '0.0], [13, 0.0], [14, 0.0], [15, 0.0], [16, 0.0], [17, 0.0], '*

 * *                                 '[18, 0.0], [19, 0.0], [20, 0.0], [21, 0.0], [22, 0.0], [23, '*

 * *                                 '0.0], [24, 0.0], [25, 0.0], [26, 0.0], [27, 0.0], [28, 0.0], '*

 * * […]*

```diff
@@ -1,16 +1,9 @@
 {
-    "citations": [
-        "United States Census Bureau",
-        "American Community Survey 2019: Franklin County, WA",
-        "The Older Population: 2010, US Census Bureau",
-        "Look-Up: How Nursing Home Staffing Fluctuates Nationwide, Kaiser Health News, 05-02-2019",
-        "Report Card Enrollment 2019-20 School Year, Washington Office of Superintendent of Public Instruction",
-        "Education Directory, Washington Office of Superintendent of Public Instruction"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
             16,
             0.187
         ],
         [
@@ -844,20 +837,421 @@
         ],
         [
             11.0,
             11.0,
             0.5
         ]
     ],
-    "ltcf_use_rate_distribution": [],
-    "notes": [
-        "Long term care facility resident to care staff ratios are taken from the Kaiser Health News analysis of data from the Centers for Medicare & Medicaid Services based on staffing levels, January-March 2018.",
-        "The age distribution binned to 20 age brackets is estimated for the age groups 85-89 years old, 90-94 years old, 95 years old and over using the relative proportions from the Older Population: 2010 report. These data are available for the national population from the 2010 census and thus represent an estimate of the patterns for different subnational populations within the US currently.",
-        "The supported mapping of student ages to school types is currently a strict 1-1 mapping. This creates a description where different school types are not overlapping in the grades of students taught. However, school types in Washington state are more complex than this and there are some schools covering a different range of grades than presented here (i.e., K-8 or 6-12 vs K-5, 6-8, 9-12, etc.). The data on schools and school types represent a majority (85%+) of the students enrolled in the county for the school year 2019-2020."
+    "ltcf_use_rate_distribution": [
+        [
+            0,
+            0.0
+        ],
+        [
+            1,
+            0.0
+        ],
+        [
+            2,
+            0.0
+        ],
+        [
+            3,
+            0.0
+        ],
+        [
+            4,
+            0.0
+        ],
+        [
+            5,
+            0.0
+        ],
+        [
+            6,
+            0.0
+        ],
+        [
+            7,
+            0.0
+        ],
+        [
+            8,
+            0.0
+        ],
+        [
+            9,
+            0.0
+        ],
+        [
+            10,
+            0.0
+        ],
+        [
+            11,
+            0.0
+        ],
+        [
+            12,
+            0.0
+        ],
+        [
+            13,
+            0.0
+        ],
+        [
+            14,
+            0.0
+        ],
+        [
+            15,
+            0.0
+        ],
+        [
+            16,
+            0.0
+        ],
+        [
+            17,
+            0.0
+        ],
+        [
+            18,
+            0.0
+        ],
+        [
+            19,
+            0.0
+        ],
+        [
+            20,
+            0.0
+        ],
+        [
+            21,
+            0.0
+        ],
+        [
+            22,
+            0.0
+        ],
+        [
+            23,
+            0.0
+        ],
+        [
+            24,
+            0.0
+        ],
+        [
+            25,
+            0.0
+        ],
+        [
+            26,
+            0.0
+        ],
+        [
+            27,
+            0.0
+        ],
+        [
+            28,
+            0.0
+        ],
+        [
+            29,
+            0.0
+        ],
+        [
+            30,
+            0.0
+        ],
+        [
+            31,
+            0.0
+        ],
+        [
+            32,
+            0.0
+        ],
+        [
+            33,
+            0.0
+        ],
+        [
+            34,
+            0.0
+        ],
+        [
+            35,
+            0.0
+        ],
+        [
+            36,
+            0.0
+        ],
+        [
+            37,
+            0.0
+        ],
+        [
+            38,
+            0.0
+        ],
+        [
+            39,
+            0.0
+        ],
+        [
+            40,
+            0.0
+        ],
+        [
+            41,
+            0.0
+        ],
+        [
+            42,
+            0.0
+        ],
+        [
+            43,
+            0.0
+        ],
+        [
+            44,
+            0.0
+        ],
+        [
+            45,
+            0.0
+        ],
+        [
+            46,
+            0.0
+        ],
+        [
+            47,
+            0.0
+        ],
+        [
+            48,
+            0.0
+        ],
+        [
+            49,
+            0.0
+        ],
+        [
+            50,
+            0.0
+        ],
+        [
+            51,
+            0.0
+        ],
+        [
+            52,
+            0.0
+        ],
+        [
+            53,
+            0.0
+        ],
+        [
+            54,
+            0.0
+        ],
+        [
+            55,
+            0.0
+        ],
+        [
+            56,
+            0.0
+        ],
+        [
+            57,
+            0.0
+        ],
+        [
+            58,
+            0.0
+        ],
+        [
+            59,
+            0.0
+        ],
+        [
+            60,
+            0.01014726
+        ],
+        [
+            61,
+            0.01014726
+        ],
+        [
+            62,
+            0.01014726
+        ],
+        [
+            63,
+            0.01014726
+        ],
+        [
+            64,
+            0.01014726
+        ],
+        [
+            65,
+            0.00992606
+        ],
+        [
+            66,
+            0.00992606
+        ],
+        [
+            67,
+            0.00992606
+        ],
+        [
+            68,
+            0.00992606
+        ],
+        [
+            69,
+            0.00992606
+        ],
+        [
+            70,
+            0.00992606
+        ],
+        [
+            71,
+            0.00992606
+        ],
+        [
+            72,
+            0.00992606
+        ],
+        [
+            73,
+            0.00992606
+        ],
+        [
+            74,
+            0.00992606
+        ],
+        [
+            75,
+            0.06078108
+        ],
+        [
+            76,
+            0.06078108
+        ],
+        [
+            77,
+            0.06078108
+        ],
+        [
+            78,
+            0.06078108
+        ],
+        [
+            79,
+            0.06078108
+        ],
+        [
+            80,
+            0.06078108
+        ],
+        [
+            81,
+            0.06078108
+        ],
+        [
+            82,
+            0.06078108
+        ],
+        [
+            83,
+            0.06078108
+        ],
+        [
+            84,
+            0.06078108
+        ],
+        [
+            85,
+            0.18420189
+        ],
+        [
+            86,
+            0.18420189
+        ],
+        [
+            87,
+            0.18420189
+        ],
+        [
+            88,
+            0.18420189
+        ],
+        [
+            89,
+            0.18420189
+        ],
+        [
+            90,
+            0.18420189
+        ],
+        [
+            91,
+            0.18420189
+        ],
+        [
+            92,
+            0.18420189
+        ],
+        [
+            93,
+            0.18420189
+        ],
+        [
+            94,
+            0.18420189
+        ],
+        [
+            95,
+            0.18420189
+        ],
+        [
+            96,
+            0.18420189
+        ],
+        [
+            97,
+            0.18420189
+        ],
+        [
+            98,
+            0.18420189
+        ],
+        [
+            99,
+            0.18420189
+        ],
+        [
+            100,
+            0.18420189
+        ]
     ],
+    "notes": [],
     "parent": "usa-Washington.json",
     "population_age_distributions": [
         {
             "distribution": [
                 [
                     0,
                     4,
@@ -1138,21 +1532,15 @@
                     100,
                     0.0006312733518631
                 ]
             ],
             "num_bins": 20
         }
     ],
-    "reference_links": [
-        "https://data.census.gov/cedsci",
-        "https://khn.org/news/look-up-how-nursing-home-staffing-fluctuates-nationwide/",
-        "https://data.wa.gov/Education/Report-Card-Enrollment-2019-20-School-Year/gtd3-scga",
-        "https://www.census.gov/prod/cen2010/briefs/c2010br-09.pdf",
-        "https://eds.ospi.k12.wa.us/DirectoryEDS.aspx"
-    ],
+    "reference_links": [],
     "school_size_brackets": [
         [
             20,
             50
         ],
         [
             51,
```

### Comparing `synthpops-1.10.5/synthpops/data/usa-Washington-Island_County.json` & `synthpops-1.8.0/synthpops/data/usa-Washington-Island_County.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9047619047619048%*

 * *Differences: {"'citations'": '[]',*

 * * "'ltcf_use_rate_distribution'": '[[0, 0.0], [1, 0.0], [2, 0.0], [3, 0.0], [4, 0.0], [5, 0.0], [6, '*

 * *                                 '0.0], [7, 0.0], [8, 0.0], [9, 0.0], [10, 0.0], [11, 0.0], [12, '*

 * *                                 '0.0], [13, 0.0], [14, 0.0], [15, 0.0], [16, 0.0], [17, 0.0], '*

 * *                                 '[18, 0.0], [19, 0.0], [20, 0.0], [21, 0.0], [22, 0.0], [23, '*

 * *                                 '0.0], [24, 0.0], [25, 0.0], [26, 0.0], [27, 0.0], [28, 0.0], '*

 * * […]*

```diff
@@ -1,16 +1,9 @@
 {
-    "citations": [
-        "United States Census Bureau",
-        "American Community Survey 2019: Island County, WA",
-        "The Older Population: 2010, US Census Bureau",
-        "Look-Up: How Nursing Home Staffing Fluctuates Nationwide, Kaiser Health News, 05-02-2019",
-        "Report Card Enrollment 2019-20 School Year, Washington Office of Superintendent of Public Instruction",
-        "Education Directory, Washington Office of Superintendent of Public Instruction"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
             16,
             0.278
         ],
         [
@@ -849,20 +842,421 @@
         ],
         [
             12.0,
             12.0,
             0.5
         ]
     ],
-    "ltcf_use_rate_distribution": [],
-    "notes": [
-        "Long term care facility resident to care staff ratios are taken from the Kaiser Health News analysis of data from the Centers for Medicare & Medicaid Services based on staffing levels, January-March 2018.",
-        "The age distribution binned to 20 age brackets is estimated for the age groups 85-89 years old, 90-94 years old, 95 years old and over using the relative proportions from the Older Population: 2010 report. These data are available for the national population from the 2010 census and thus represent an estimate of the patterns for different subnational populations within the US currently.",
-        "The supported mapping of student ages to school types is currently a strict 1-1 mapping. This creates a description where different school types are not overlapping in the grades of students taught. However, school types in Washington state are more complex than this and there are some schools covering a different range of grades than presented here (i.e., K-8 or 6-12 vs K-5, 6-8, 9-12, etc.). The data on schools and school types represent a majority (85%+) of the students enrolled in the county for the school year 2019-2020."
+    "ltcf_use_rate_distribution": [
+        [
+            0,
+            0.0
+        ],
+        [
+            1,
+            0.0
+        ],
+        [
+            2,
+            0.0
+        ],
+        [
+            3,
+            0.0
+        ],
+        [
+            4,
+            0.0
+        ],
+        [
+            5,
+            0.0
+        ],
+        [
+            6,
+            0.0
+        ],
+        [
+            7,
+            0.0
+        ],
+        [
+            8,
+            0.0
+        ],
+        [
+            9,
+            0.0
+        ],
+        [
+            10,
+            0.0
+        ],
+        [
+            11,
+            0.0
+        ],
+        [
+            12,
+            0.0
+        ],
+        [
+            13,
+            0.0
+        ],
+        [
+            14,
+            0.0
+        ],
+        [
+            15,
+            0.0
+        ],
+        [
+            16,
+            0.0
+        ],
+        [
+            17,
+            0.0
+        ],
+        [
+            18,
+            0.0
+        ],
+        [
+            19,
+            0.0
+        ],
+        [
+            20,
+            0.0
+        ],
+        [
+            21,
+            0.0
+        ],
+        [
+            22,
+            0.0
+        ],
+        [
+            23,
+            0.0
+        ],
+        [
+            24,
+            0.0
+        ],
+        [
+            25,
+            0.0
+        ],
+        [
+            26,
+            0.0
+        ],
+        [
+            27,
+            0.0
+        ],
+        [
+            28,
+            0.0
+        ],
+        [
+            29,
+            0.0
+        ],
+        [
+            30,
+            0.0
+        ],
+        [
+            31,
+            0.0
+        ],
+        [
+            32,
+            0.0
+        ],
+        [
+            33,
+            0.0
+        ],
+        [
+            34,
+            0.0
+        ],
+        [
+            35,
+            0.0
+        ],
+        [
+            36,
+            0.0
+        ],
+        [
+            37,
+            0.0
+        ],
+        [
+            38,
+            0.0
+        ],
+        [
+            39,
+            0.0
+        ],
+        [
+            40,
+            0.0
+        ],
+        [
+            41,
+            0.0
+        ],
+        [
+            42,
+            0.0
+        ],
+        [
+            43,
+            0.0
+        ],
+        [
+            44,
+            0.0
+        ],
+        [
+            45,
+            0.0
+        ],
+        [
+            46,
+            0.0
+        ],
+        [
+            47,
+            0.0
+        ],
+        [
+            48,
+            0.0
+        ],
+        [
+            49,
+            0.0
+        ],
+        [
+            50,
+            0.0
+        ],
+        [
+            51,
+            0.0
+        ],
+        [
+            52,
+            0.0
+        ],
+        [
+            53,
+            0.0
+        ],
+        [
+            54,
+            0.0
+        ],
+        [
+            55,
+            0.0
+        ],
+        [
+            56,
+            0.0
+        ],
+        [
+            57,
+            0.0
+        ],
+        [
+            58,
+            0.0
+        ],
+        [
+            59,
+            0.0
+        ],
+        [
+            60,
+            0.01014726
+        ],
+        [
+            61,
+            0.01014726
+        ],
+        [
+            62,
+            0.01014726
+        ],
+        [
+            63,
+            0.01014726
+        ],
+        [
+            64,
+            0.01014726
+        ],
+        [
+            65,
+            0.00992606
+        ],
+        [
+            66,
+            0.00992606
+        ],
+        [
+            67,
+            0.00992606
+        ],
+        [
+            68,
+            0.00992606
+        ],
+        [
+            69,
+            0.00992606
+        ],
+        [
+            70,
+            0.00992606
+        ],
+        [
+            71,
+            0.00992606
+        ],
+        [
+            72,
+            0.00992606
+        ],
+        [
+            73,
+            0.00992606
+        ],
+        [
+            74,
+            0.00992606
+        ],
+        [
+            75,
+            0.06078108
+        ],
+        [
+            76,
+            0.06078108
+        ],
+        [
+            77,
+            0.06078108
+        ],
+        [
+            78,
+            0.06078108
+        ],
+        [
+            79,
+            0.06078108
+        ],
+        [
+            80,
+            0.06078108
+        ],
+        [
+            81,
+            0.06078108
+        ],
+        [
+            82,
+            0.06078108
+        ],
+        [
+            83,
+            0.06078108
+        ],
+        [
+            84,
+            0.06078108
+        ],
+        [
+            85,
+            0.18420189
+        ],
+        [
+            86,
+            0.18420189
+        ],
+        [
+            87,
+            0.18420189
+        ],
+        [
+            88,
+            0.18420189
+        ],
+        [
+            89,
+            0.18420189
+        ],
+        [
+            90,
+            0.18420189
+        ],
+        [
+            91,
+            0.18420189
+        ],
+        [
+            92,
+            0.18420189
+        ],
+        [
+            93,
+            0.18420189
+        ],
+        [
+            94,
+            0.18420189
+        ],
+        [
+            95,
+            0.18420189
+        ],
+        [
+            96,
+            0.18420189
+        ],
+        [
+            97,
+            0.18420189
+        ],
+        [
+            98,
+            0.18420189
+        ],
+        [
+            99,
+            0.18420189
+        ],
+        [
+            100,
+            0.18420189
+        ]
     ],
+    "notes": [],
     "parent": "usa-Washington.json",
     "population_age_distributions": [
         {
             "distribution": [
                 [
                     0,
                     4,
@@ -1143,21 +1537,15 @@
                     100,
                     0.0011164486622844
                 ]
             ],
             "num_bins": 20
         }
     ],
-    "reference_links": [
-        "https://data.census.gov/cedsci",
-        "https://khn.org/news/look-up-how-nursing-home-staffing-fluctuates-nationwide/",
-        "https://data.wa.gov/Education/Report-Card-Enrollment-2019-20-School-Year/gtd3-scga",
-        "https://www.census.gov/prod/cen2010/briefs/c2010br-09.pdf",
-        "https://eds.ospi.k12.wa.us/DirectoryEDS.aspx"
-    ],
+    "reference_links": [],
     "school_size_brackets": [
         [
             20,
             50
         ],
         [
             51,
```

### Comparing `synthpops-1.10.5/synthpops/data/usa-Washington-Spokane_County.json` & `synthpops-1.8.0/synthpops/data/usa-Washington-Spokane_County.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8809523809523809%*

 * *Differences: {"'citations'": '[]',*

 * * "'ltcf_num_residents_distribution'": '[[0.0, 19.0, 0.0], [20.0, 39.0, 0.0895522388059701], [40.0, '*

 * *                                      '59.0, 0.1343283582089552], [60.0, 79.0, '*

 * *                                      '0.1343283582089552], [80.0, 99.0, 0.1940298507462686], '*

 * *                                      '[100.0, 119.0, 0.1044776119402985], [120.0, 139.0, '*

 * *                                      '0.1194029850746268], [140.0, 159.0, 0.0597014925373134], '*

 * *                       […]*

```diff
@@ -1,16 +1,9 @@
 {
-    "citations": [
-        "United States Census Bureau",
-        "American Community Survey 2019: Spokane County, WA",
-        "The Older Population: 2010, US Census Bureau",
-        "Look-Up: How Nursing Home Staffing Fluctuates Nationwide, Kaiser Health News, 05-02-2019",
-        "Report Card Enrollment 2019-20 School Year, Washington Office of Superintendent of Public Instruction",
-        "Education Directory, Washington Office of Superintendent of Public Instruction"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
             16,
             0.322
         ],
         [
@@ -785,15 +778,191 @@
         ],
         [
             7,
             0.0157800522380658
         ]
     ],
     "location_name": "usa-Washington-Spokane_County",
-    "ltcf_num_residents_distribution": [],
+    "ltcf_num_residents_distribution": [
+        [
+            0.0,
+            19.0,
+            0.0
+        ],
+        [
+            20.0,
+            39.0,
+            0.0895522388059701
+        ],
+        [
+            40.0,
+            59.0,
+            0.1343283582089552
+        ],
+        [
+            60.0,
+            79.0,
+            0.1343283582089552
+        ],
+        [
+            80.0,
+            99.0,
+            0.1940298507462686
+        ],
+        [
+            100.0,
+            119.0,
+            0.1044776119402985
+        ],
+        [
+            120.0,
+            139.0,
+            0.1194029850746268
+        ],
+        [
+            140.0,
+            159.0,
+            0.0597014925373134
+        ],
+        [
+            160.0,
+            179.0,
+            0.0149253731343283
+        ],
+        [
+            180.0,
+            199.0,
+            0.0
+        ],
+        [
+            200.0,
+            219.0,
+            0.0149253731343283
+        ],
+        [
+            220.0,
+            239.0,
+            0.0149253731343283
+        ],
+        [
+            240.0,
+            259.0,
+            0.0
+        ],
+        [
+            260.0,
+            279.0,
+            0.0298507462686567
+        ],
+        [
+            280.0,
+            299.0,
+            0.0
+        ],
+        [
+            300.0,
+            319.0,
+            0.0298507462686567
+        ],
+        [
+            320.0,
+            339.0,
+            0.0149253731343283
+        ],
+        [
+            340.0,
+            359.0,
+            0.0
+        ],
+        [
+            360.0,
+            379.0,
+            0.0
+        ],
+        [
+            380.0,
+            399.0,
+            0.0
+        ],
+        [
+            400.0,
+            419.0,
+            0.0
+        ],
+        [
+            420.0,
+            439.0,
+            0.0149253731343283
+        ],
+        [
+            440.0,
+            459.0,
+            0.0149253731343283
+        ],
+        [
+            460.0,
+            479.0,
+            0.0
+        ],
+        [
+            480.0,
+            499.0,
+            0.0
+        ],
+        [
+            500.0,
+            519.0,
+            0.0
+        ],
+        [
+            520.0,
+            539.0,
+            0.0149253731343283
+        ],
+        [
+            540.0,
+            559.0,
+            0.0
+        ],
+        [
+            560.0,
+            579.0,
+            0.0
+        ],
+        [
+            580.0,
+            599.0,
+            0.0
+        ],
+        [
+            600.0,
+            619.0,
+            0.0
+        ],
+        [
+            620.0,
+            639.0,
+            0.0
+        ],
+        [
+            640.0,
+            659.0,
+            0.0
+        ],
+        [
+            660.0,
+            679.0,
+            0.0
+        ],
+        [
+            680.0,
+            699.0,
+            0.0
+        ]
+    ],
     "ltcf_num_staff_distribution": [],
     "ltcf_resident_to_staff_ratio_distribution": [
         [
             1.0,
             1.0,
             0.0
         ],
@@ -859,20 +1028,421 @@
         ],
         [
             14.0,
             14.0,
             0.15625
         ]
     ],
-    "ltcf_use_rate_distribution": [],
-    "notes": [
-        "Long term care facility resident to care staff ratios are taken from the Kaiser Health News analysis of data from the Centers for Medicare & Medicaid Services based on staffing levels, January-March 2018.",
-        "The age distribution binned to 20 age brackets is estimated for the age groups 85-89 years old, 90-94 years old, 95 years old and over using the relative proportions from the Older Population: 2010 report. These data are available for the national population from the 2010 census and thus represent an estimate of the patterns for different subnational populations within the US currently.",
-        "The supported mapping of student ages to school types is currently a strict 1-1 mapping. This creates a description where different school types are not overlapping in the grades of students taught. However, school types in Washington state are more complex than this and there are some schools covering a different range of grades than presented here (i.e., K-8 or 6-12 vs K-5, 6-8, 9-12, etc.). The data on schools and school types represent a majority (85%+) of the students enrolled in the county for the school year 2019-2020."
+    "ltcf_use_rate_distribution": [
+        [
+            0,
+            0.0
+        ],
+        [
+            1,
+            0.0
+        ],
+        [
+            2,
+            0.0
+        ],
+        [
+            3,
+            0.0
+        ],
+        [
+            4,
+            0.0
+        ],
+        [
+            5,
+            0.0
+        ],
+        [
+            6,
+            0.0
+        ],
+        [
+            7,
+            0.0
+        ],
+        [
+            8,
+            0.0
+        ],
+        [
+            9,
+            0.0
+        ],
+        [
+            10,
+            0.0
+        ],
+        [
+            11,
+            0.0
+        ],
+        [
+            12,
+            0.0
+        ],
+        [
+            13,
+            0.0
+        ],
+        [
+            14,
+            0.0
+        ],
+        [
+            15,
+            0.0
+        ],
+        [
+            16,
+            0.0
+        ],
+        [
+            17,
+            0.0
+        ],
+        [
+            18,
+            0.0
+        ],
+        [
+            19,
+            0.0
+        ],
+        [
+            20,
+            0.0
+        ],
+        [
+            21,
+            0.0
+        ],
+        [
+            22,
+            0.0
+        ],
+        [
+            23,
+            0.0
+        ],
+        [
+            24,
+            0.0
+        ],
+        [
+            25,
+            0.0
+        ],
+        [
+            26,
+            0.0
+        ],
+        [
+            27,
+            0.0
+        ],
+        [
+            28,
+            0.0
+        ],
+        [
+            29,
+            0.0
+        ],
+        [
+            30,
+            0.0
+        ],
+        [
+            31,
+            0.0
+        ],
+        [
+            32,
+            0.0
+        ],
+        [
+            33,
+            0.0
+        ],
+        [
+            34,
+            0.0
+        ],
+        [
+            35,
+            0.0
+        ],
+        [
+            36,
+            0.0
+        ],
+        [
+            37,
+            0.0
+        ],
+        [
+            38,
+            0.0
+        ],
+        [
+            39,
+            0.0
+        ],
+        [
+            40,
+            0.0
+        ],
+        [
+            41,
+            0.0
+        ],
+        [
+            42,
+            0.0
+        ],
+        [
+            43,
+            0.0
+        ],
+        [
+            44,
+            0.0
+        ],
+        [
+            45,
+            0.0
+        ],
+        [
+            46,
+            0.0
+        ],
+        [
+            47,
+            0.0
+        ],
+        [
+            48,
+            0.0
+        ],
+        [
+            49,
+            0.0
+        ],
+        [
+            50,
+            0.0
+        ],
+        [
+            51,
+            0.0
+        ],
+        [
+            52,
+            0.0
+        ],
+        [
+            53,
+            0.0
+        ],
+        [
+            54,
+            0.0
+        ],
+        [
+            55,
+            0.0
+        ],
+        [
+            56,
+            0.0
+        ],
+        [
+            57,
+            0.0
+        ],
+        [
+            58,
+            0.0
+        ],
+        [
+            59,
+            0.0
+        ],
+        [
+            60,
+            0.01014726
+        ],
+        [
+            61,
+            0.01014726
+        ],
+        [
+            62,
+            0.01014726
+        ],
+        [
+            63,
+            0.01014726
+        ],
+        [
+            64,
+            0.01014726
+        ],
+        [
+            65,
+            0.00992606
+        ],
+        [
+            66,
+            0.00992606
+        ],
+        [
+            67,
+            0.00992606
+        ],
+        [
+            68,
+            0.00992606
+        ],
+        [
+            69,
+            0.00992606
+        ],
+        [
+            70,
+            0.00992606
+        ],
+        [
+            71,
+            0.00992606
+        ],
+        [
+            72,
+            0.00992606
+        ],
+        [
+            73,
+            0.00992606
+        ],
+        [
+            74,
+            0.00992606
+        ],
+        [
+            75,
+            0.06078108
+        ],
+        [
+            76,
+            0.06078108
+        ],
+        [
+            77,
+            0.06078108
+        ],
+        [
+            78,
+            0.06078108
+        ],
+        [
+            79,
+            0.06078108
+        ],
+        [
+            80,
+            0.06078108
+        ],
+        [
+            81,
+            0.06078108
+        ],
+        [
+            82,
+            0.06078108
+        ],
+        [
+            83,
+            0.06078108
+        ],
+        [
+            84,
+            0.06078108
+        ],
+        [
+            85,
+            0.18420189
+        ],
+        [
+            86,
+            0.18420189
+        ],
+        [
+            87,
+            0.18420189
+        ],
+        [
+            88,
+            0.18420189
+        ],
+        [
+            89,
+            0.18420189
+        ],
+        [
+            90,
+            0.18420189
+        ],
+        [
+            91,
+            0.18420189
+        ],
+        [
+            92,
+            0.18420189
+        ],
+        [
+            93,
+            0.18420189
+        ],
+        [
+            94,
+            0.18420189
+        ],
+        [
+            95,
+            0.18420189
+        ],
+        [
+            96,
+            0.18420189
+        ],
+        [
+            97,
+            0.18420189
+        ],
+        [
+            98,
+            0.18420189
+        ],
+        [
+            99,
+            0.18420189
+        ],
+        [
+            100,
+            0.18420189
+        ]
     ],
+    "notes": [],
     "parent": "usa-Washington.json",
     "population_age_distributions": [
         {
             "distribution": [
                 [
                     0,
                     4,
@@ -1153,21 +1723,15 @@
                     100,
                     0.0009741387261959
                 ]
             ],
             "num_bins": 20
         }
     ],
-    "reference_links": [
-        "https://data.census.gov/cedsci",
-        "https://khn.org/news/look-up-how-nursing-home-staffing-fluctuates-nationwide/",
-        "https://data.wa.gov/Education/Report-Card-Enrollment-2019-20-School-Year/gtd3-scga",
-        "https://www.census.gov/prod/cen2010/briefs/c2010br-09.pdf",
-        "https://eds.ospi.k12.wa.us/DirectoryEDS.aspx"
-    ],
+    "reference_links": [],
     "school_size_brackets": [
         [
             20,
             50
         ],
         [
             51,
```

### Comparing `synthpops-1.10.5/synthpops/data/usa-Washington.json` & `synthpops-1.8.0/synthpops/data/usa-Washington.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8809523809523809%*

 * *Differences: {"'citations'": '[]',*

 * * "'household_head_age_brackets'": '[[18, 19], [20, 24], [25, 29], [30, 34], [35, 39], [40, 44], '*

 * *                                  '[45, 49], [50, 54], [55, 64], [65, 74], [75, 99]]',*

 * * "'household_head_age_distribution_by_family_size'": '[[1, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, '*

 * *                                                     '1.0, 1.0, 1.0], [2, 163.0, 999.0, 2316.0, '*

 * *                                                     '2230.0, 1880.0, 1856.0, 2390.0, 3118.0, '*

 * *           […]*

```diff
@@ -1,14 +1,9 @@
 {
-    "citations": [
-        "United States Census Bureau",
-        "American Community Survey 2019: Washington",
-        "The Older Population: 2010, US Census Bureau",
-        "Long-Term Care Providers and Services Users in the United States \u2014 State Estimates Supplement: National Study of Long-Term Care Providers, 2015\u20132016"
-    ],
+    "citations": [],
     "data_provenance_notices": [],
     "employment_rates_by_age": [
         [
             16,
             0.332
         ],
         [
@@ -750,16 +745,174 @@
             0.0
         ],
         [
             100,
             0.0
         ]
     ],
-    "household_head_age_brackets": [],
-    "household_head_age_distribution_by_family_size": [],
+    "household_head_age_brackets": [
+        [
+            18,
+            19
+        ],
+        [
+            20,
+            24
+        ],
+        [
+            25,
+            29
+        ],
+        [
+            30,
+            34
+        ],
+        [
+            35,
+            39
+        ],
+        [
+            40,
+            44
+        ],
+        [
+            45,
+            49
+        ],
+        [
+            50,
+            54
+        ],
+        [
+            55,
+            64
+        ],
+        [
+            65,
+            74
+        ],
+        [
+            75,
+            99
+        ]
+    ],
+    "household_head_age_distribution_by_family_size": [
+        [
+            1,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0
+        ],
+        [
+            2,
+            163.0,
+            999.0,
+            2316.0,
+            2230.0,
+            1880.0,
+            1856.0,
+            2390.0,
+            3118.0,
+            9528.0,
+            9345.0,
+            5584.0
+        ],
+        [
+            3,
+            115.0,
+            757.0,
+            1545.0,
+            1907.0,
+            2066.0,
+            1811.0,
+            2028.0,
+            2175.0,
+            3311.0,
+            1587.0,
+            588.0
+        ],
+        [
+            4,
+            135.0,
+            442.0,
+            1029.0,
+            1951.0,
+            2670.0,
+            2547.0,
+            2368.0,
+            1695.0,
+            1763.0,
+            520.0,
+            221.0
+        ],
+        [
+            5,
+            61.0,
+            172.0,
+            394.0,
+            905.0,
+            1429.0,
+            1232.0,
+            969.0,
+            683.0,
+            623.0,
+            235.0,
+            94.0
+        ],
+        [
+            6,
+            25.0,
+            81.0,
+            153.0,
+            352.0,
+            511.0,
+            459.0,
+            372.0,
+            280.0,
+            280.0,
+            113.0,
+            49.0
+        ],
+        [
+            7,
+            24.0,
+            33.0,
+            63.0,
+            144.0,
+            279.0,
+            242.0,
+            219.0,
+            115.0,
+            157.0,
+            80.0,
+            16.0
+        ],
+        [
+            8,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0
+        ]
+    ],
     "household_size_distribution": [
         [
             1,
             0.2619887241739551
         ],
         [
             2,
@@ -1192,17 +1345,15 @@
             0.18420189
         ],
         [
             100,
             0.18420189
         ]
     ],
-    "notes": [
-        "The age distribution binned to 20 age brackets is estimated for the age groups 85-89 years old, 90-94 years old, 95 years old and over using the relative proportions from the Older Population: 2010 report. These data are available for the national population from the 2010 census and thus represent an estimate of the patterns for different subnational populations within the US currently."
-    ],
+    "notes": [],
     "parent": "usa.json",
     "population_age_distributions": [
         {
             "distribution": [
                 [
                     0,
                     4,
@@ -1483,18 +1634,15 @@
                     100,
                     0.0009530811675372
                 ]
             ],
             "num_bins": 20
         }
     ],
-    "reference_links": [
-        "https://data.census.gov/cedsci",
-        "https://www.cdc.gov/nchs/npals/webtables.htm"
-    ],
+    "reference_links": [],
     "school_size_brackets": [
         [
             20,
             50
         ],
         [
             51,
```

### Comparing `synthpops-1.10.5/synthpops/data.py` & `synthpops-1.8.0/synthpops/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,19 @@
     Returns:
         json: The location json object with necessary data fields filled from
         the parent location.
     """
     # DM: parameter name of location should change to better reflect what this parameter actually is: the location data object
     logger.debug(f"Loading parent location from filepath [{parent_file_path}]")
     try:
-        parent_obj = load_location_from_filepath(parent_file_path, check_constraints=False)
+        parent_obj = load_location_from_filepath(parent_file_path)
         location = populate_parent_data_from_json_obj(location, parent_obj)
     except:
-        logger.warning(f"You may have an invalid data configuration: couldn't load parent "
+        logger.debug(f"You may have an invalid data configuration: couldn't load parent"
+        # logger.warning(f"You may have an invalid data configuration: couldn't load parent "
                     f"from filepath [{parent_file_path}] for location [{location.location_name}]")
     return location
 
 
 def populate_parent_data_from_json_obj(location, parent):
     """
     Loading a location json object with necessary data fields filled from the
@@ -234,51 +235,45 @@
     if type(parent) is JsonDict:
         parent_location = Location(parent)
         return populate_parent_data_from_json_obj(location, parent_location)
 
     raise RuntimeError(f'Invalid type for parent field: [{type(parent)}]')
 
 
-def load_location_from_json(json_obj, check_constraints=None):
+def load_location_from_json(json_obj):
     """
     Load location data from json object with some checks made.
 
     Args:
         json_obj (json): json object containing location data
 
     Returns:
         json: The json object with location data.
     """
-    if check_constraints is None:
-        check_constraints = True
-
     location = Location(json_obj)
+    check_location_constraints_satisfied(location)
+    check_all_probability_distribution_sums(location)
+    check_all_probability_distribution_nonnegative(location)
 
     populate_parent_data(location)
-
-    if check_constraints:
-        check_location_constraints_satisfied(location)
-        check_all_probability_distribution_sums(location)
-        check_all_probability_distribution_nonnegative(location)
-
     return location
 
 
-def load_location_from_json_str(json_str, check_constraints=None):
+def load_location_from_json_str(json_str):
     """
     Load location data from json str with some checks made.
 
     Args:
         json_str (str): string version of the json object
 
     Returns:
         json: The json object with location data.
     """
     json_obj = json.loads(json_str)
-    return load_location_from_json(json_obj, check_constraints=check_constraints)
+    return load_location_from_json(json_obj)
 
 
 def get_relative_path(datadir):
     """
     Get the relative path for the data folder.
 
     Args:
@@ -311,33 +306,30 @@
     """
     if property_name in location.keys():
         return getattr(location, property_name)
     else:
         return [False, None]
 
 
-def load_location_from_filepath(rel_filepath, check_constraints=None):
+def load_location_from_filepath(rel_filepath):
     """
     Loads location data object from provided relative filepath where the file path is
     relative to defaults.settings.datadir.
 
     Args:
         rel_filepath (str): relative file path for the location data
 
     Returns:
         json: The json object with location data.
     """
-    if check_constraints is None:
-        check_constraints = True
-
     filepath = os.path.join(get_relative_path(defaults.settings.datadir), rel_filepath)
     logger.debug(f"Opening location from filepath [{filepath}]")
     f = open(filepath, 'r')
     json_obj = json.load(f)
-    return load_location_from_json(json_obj, check_constraints=check_constraints)
+    return load_location_from_json(json_obj)
 
 
 def save_location_to_filepath(location, abs_filepath):
     """
     Saves json object with location data to provided absolute filepath.
 
     Args:
```

### Comparing `synthpops-1.10.5/synthpops/data_distributions.py` & `synthpops-1.8.0/synthpops/data_distributions.py`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/defaults.py` & `synthpops-1.8.0/synthpops/defaults.py`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops/households.py` & `synthpops-1.8.0/synthpops/households.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sciris as sc
 import numpy as np
 import pandas as pd
 from collections import Counter
 from .config import logger as log, checkmem
 from . import base as spb
 from . import sampling as spsamp
-from . import ltcfs as spltcf
 from . import data_distributions as spdata
 
 
 class Household(spb.LayerGroup):
     """
     A class for individual households and methods to operate on each.
 
@@ -148,34 +147,34 @@
         pop.households[household['hhid']] = sc.dcp(household)
 
     pop.populate = True
 
     return
 
 
-def generate_household_size_count_from_fixed_pop_size(N, hh_size_distr):
+def generate_household_sizes_from_fixed_pop_size(N, hh_size_distr):
     """
     Given a number of people and a household size distribution, generate the number of homes of each size needed to place everyone in a household.
 
     Args:
         N      (int)         : The number of people in the population.
         hh_size_distr (dict) : The distribution of household sizes.
 
     Returns:
         An array with the count of households of size s at index s-1.
     """
-    log.debug('generate_household_size_count_from_fixed_pop_size()')
+
     # Quickly produce number of expected households for a population of size N
     ss = np.sum([hh_size_distr[s] * s for s in hh_size_distr])
     f = N / np.round(ss, 1)
     hh_sizes = np.zeros(len(hh_size_distr))
 
     for s in hh_size_distr:
-        hh_sizes[s - 1] = int(hh_size_distr[s] * f)
-    N_gen = np.sum([hh_sizes[s - 1] * s for s in hh_size_distr], dtype=int)
+        hh_sizes[s-1] = int(hh_size_distr[s] * f)
+    N_gen = np.sum([hh_sizes[s-1] * s for s in hh_size_distr], dtype=int)
 
     # Check what population size was created from the drawn count of household sizes
     people_to_add_or_remove = N_gen - N
 
     # did not create household sizes to match or exceed the population size so add count for households needed
     hh_size_keys = [k for k in hh_size_distr]
     hh_size_distr_array = [hh_size_distr[k] for k in hh_size_keys]
@@ -185,46 +184,89 @@
         while people_to_add > 0:
             new_household_size = np.random.choice(hh_size_keys, p=hh_size_distr_array)
 
             if new_household_size > people_to_add:
                 new_household_size = people_to_add
             people_to_add -= new_household_size
 
-            hh_sizes[new_household_size - 1] += 1
+            hh_sizes[new_household_size-1] += 1
 
     # created households that result in too many people
     elif people_to_add_or_remove > 0:
         people_to_remove = people_to_add_or_remove
         while people_to_remove > 0:
 
             new_household_size_to_remove = np.random.choice(hh_size_keys, p=hh_size_distr_array)
             if new_household_size_to_remove > people_to_remove:
                 new_household_size_to_remove = people_to_remove
 
             people_to_remove -= new_household_size_to_remove
-            hh_sizes[new_household_size_to_remove - 1] -= 1
+            hh_sizes[new_household_size_to_remove-1] -= 1
 
     hh_sizes = hh_sizes.astype(int)
     return hh_sizes
 
 
+def generate_household_head_age_by_size(hha_by_size_counts, hha_brackets, hh_size, single_year_age_distr):
+    """
+    Generate the age of the head of the household, also known as the reference person of the household,
+    conditional on the size of the household.
+
+    Args:
+        hha_by_size_counts (matrix)  : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
+        hha_brackets (dict)          : The age brackets for the heads of household.
+        hh_size (int)                : The household size.
+        single_year_age_distr (dict) : The age distribution.
+
+    Returns:
+        Age of the head of the household or reference person.
+    """
+    distr = hha_by_size_counts[hh_size-1, :]
+    b = spsamp.sample_single_arr(distr)
+    hha = spsamp.sample_from_range(single_year_age_distr, hha_brackets[b][0], hha_brackets[b][-1])
+
+    return hha
+
+
+def generate_living_alone(hh_sizes, hha_by_size_counts, hha_brackets, single_year_age_distr):
+    """
+    Generate the ages of those living alone.
+
+    Args:
+        hh_sizes (array)             : The count of household size s at index s-1.
+        hha_by_size_counts (matrix)  : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
+        hha_brackets (dict)          : The age brackets for the heads of household.
+        single_year_age_distr (dict) : The age distribution.
+
+    Returns:
+        An array of households of size 1 where each household is a row and the value in the row is the age of the household member.
+    """
+
+    size = 1
+    homes = np.zeros((hh_sizes[size-1], 1), dtype=int)
+
+    for h in range(hh_sizes[size-1]):
+        hha = generate_household_head_age_by_size(hha_by_size_counts, hha_brackets, size, single_year_age_distr)
+        homes[h][0] = int(hha)
+
+    return homes
+
+
 def assign_uids_by_homes(homes, id_len=16, use_int=True):
     """
     Assign IDs to everyone in order by their households.
 
     Args:
         homes (array)  : The generated synthetic ages of household members.
         id_len (int)   : The length of the UID.
         use_int (bool) : If True, use ints for the uids of individuals; otherwise use strings of length 'id_len'.
 
     Returns:
         A copy of the generated households with IDs in place of ages, and a dictionary mapping ID to age.
     """
-    log.debug('assign_uids_by_homes()')
-
     age_by_uid = dict()
     homes_by_uids = []
 
     for h, home in enumerate(homes):
 
         home_ids = []
         for a in home:
@@ -249,111 +291,116 @@
         n (int)                        : number of people to generate
         age_distr (list or np.ndarray) : single year age distribution
 
     Returns:
         dict: A dictionary with the count of people to generate for each age
         given an age distribution and the number of people to generate.
     """
-    log.debug('generate_age_count()')
     age_range = np.arange(0, len(age_distr))
     chosen = np.random.choice(age_range, size=n, p=age_distr)
     age_count = Counter(chosen)
     age_count = sc.mergedicts(dict.fromkeys(age_range, 0), age_count)
     return age_count
 
 
-def generate_age_count_multinomial(n, age_distr):
+def generate_living_alone_method_2(hh_sizes, hha_by_size, hha_brackets, age_count):
     """
-    Generate a stochastic count of people for each age given the age
-    distribution (age_distr) and number of people to generate (n).
+    Generate the ages of those living alone.
 
     Args:
-        n (int)                        : number of people to generate
-        age_distr (list or np.ndarray) : single year age distribution
+        hh_sizes (array)     : The count of household size s at index s-1.
+        hha_by_size (matrix) : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
+        hha_brackets (dict)  : The age brackets for the heads of household.
+        age_distr (dict)     : The age distribution.
 
     Returns:
-        dict: A dictionary with the count of people to generate for each age
-        given an age distribution and the number of people to generate.
+        An array of households of size 1 where each household is a row and the
+        value in the row is the age of the household member.
     """
-    log.debug('generate_age_count_multinomial()')
-    age_count = np.random.multinomial(n, age_distr)
-    return dict(zip(range(len(age_distr)), age_count))
+    distr = hha_by_size[0, :]
+    distr = distr / np.sum(distr)
+
+    h1_count = hh_sizes[0]
+    hha_b = np.random.choice(range(len(distr)), size=h1_count, p=distr)
 
+    hha_b_count = Counter(hha_b)
+    hha_living_alone = []
+    for hha_bi in hha_brackets:
+        possible_hha_bi_ages = []
+        for a in hha_brackets[hha_bi]:
+            possible_hha_bi_ages.extend([a] * age_count[a])
+        np.random.shuffle(possible_hha_bi_ages)
+        chosen_hha = possible_hha_bi_ages[0:hha_b_count[hha_bi]]
+        hha_living_alone.extend(chosen_hha)
+    np.random.shuffle(hha_living_alone)
 
-def generate_household_head_ages(household_sizes, hha_by_size, hha_brackets, ages_left_to_assign):
+    homes = np.array(hha_living_alone).astype(int).reshape((len(hha_living_alone), 1))
+    return homes
+
+
+def generate_larger_household_sizes(hh_sizes):
     """
-    Generate the head of household ages conditional on household size and the
-    expected ages of people in the population.
+    Create a list of the households larger than 1 in random order so that as
+    individuals are placed by age into homes running out of specific ages is not
+    systemically an issue for any given household size unless certain sizes
+    greatly outnumber households of other sizes.
 
     Args:
-        household_sizes (np.array) : Array of household sizes to be generated
-        hha_by_size (matrix)       : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
-        hha_brackets (dict)        : The age brackets for the heads of household.
-        ages_left_to_assign (dic)  : The counter of ages for the generated population left to place in a residence
+        hh_sizes (array) : The count of household size s at index s-1.
 
     Returns:
-        An array of head of household ages, updated counter of the ages in the
-        population left to place in a residence.
+        Np.array: An array of household sizes to be generated and place people
+        into households.
     """
-    household_head_ages = []
+    larger_hh_size_array = []
+    for hs in range(2, len(hh_sizes) + 1):
+        larger_hh_size_array.extend([hs] * hh_sizes[hs - 1])
+    larger_hh_size_array = np.array(larger_hh_size_array)
+    np.random.shuffle(larger_hh_size_array)
+    return larger_hh_size_array
+
 
-    for nh, hs in enumerate(household_sizes):
+def generate_larger_households_head_ages(larger_hh_size_array, hha_by_size, hha_brackets, ages_left_to_assign):
+    """
+    Generate the ages of the heads of households for households larger than 2.
+    """
+    larger_hha_chosen = []
+
+    # go through every household and choose the head age
+    for nh, hs in enumerate(larger_hh_size_array):
         hs_distr = hha_by_size[hs - 1, :]
         hbi = spsamp.fast_choice(hs_distr)
         hbi_distr = np.array([ages_left_to_assign[a] for a in hha_brackets[hbi]])
 
         while sum(hbi_distr) == 0: # pragma: no cover
             hbi = spsamp.fast_choice(hs_distr)
             hbi_distr = np.array([ages_left_to_assign[a] for a in hha_brackets[hbi]])
 
         hha = hha_brackets[hbi][spsamp.fast_choice(hbi_distr)]
         ages_left_to_assign[hha] -= 1
 
-        household_head_ages.append(hha)
-    household_head_ages = np.array(household_head_ages).astype(int)
+        larger_hha_chosen.append(hha)
 
-    return household_head_ages, ages_left_to_assign
+    return larger_hha_chosen, ages_left_to_assign
 
 
-def generate_household_sizes(hh_sizes):
-    """
-    Create a list of the household sizes in random order so that as individuals
-    are placed by age into homes running out of specific ages is not
-    systemically an issue for any given household size unless certain sizes
-    greatly outnumber households of other sizes.
-
-    Args:
-        hh_sizes (array) : The count of household size s at index s-1.
-
-    Returns:
-        Np.array: An array of household sizes to be generated and place people
-        into households.
-    """
-    household_sizes = []
-    for hs in range(1, len(hh_sizes) + 1):
-        household_sizes.extend([hs] * hh_sizes[hs - 1])
-    household_sizes = np.array(household_sizes)
-    np.random.shuffle(household_sizes)
-    return household_sizes
-
-
-def generate_larger_households_fixed_ages(larger_hh_size_array, larger_hha_chosen, hha_brackets, cm_age_brackets, cm_age_by_brackets, household_matrix, ages_left_to_assign, homes_dic):
+def generate_larger_households_method_2(larger_hh_size_array, larger_hha_chosen, hha_brackets, cm_age_brackets, cm_age_by_brackets, household_matrix, ages_left_to_assign, homes_dic):
     """
     Assign people to households larger than one person (excluding special
     residences like long term care facilities or agricultural workers living in
-    shared residential quarters).
+    shared residential quarters.
 
     Args:
         hh_sizes (array)              : The count of household size s at index s-1.
         hha_by_size (matrix)          : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
         hha_brackets (dict)           : The age brackets for the heads of household.
         cm_age_brackets (dict)        : The age brackets for the contact matrix.
         cm_age_by_brackets (dict)     : A dictionary mapping age to the age bracket range it falls within.
         household_matrix (dict)       : The age-specific contact matrix for the household ontact setting.
-        ages_left_to_assign (dict)    : Age count of people left to place in households larger than one person.
+        larger_homes_age_count (dict) : Age count of people left to place in households larger than one person.
 
     Returns:
         dict: A dictionary of households by age indexed by household size.
     """
 
     # go through every household and assign the ages of the other household members from those left to place
     for nh, hs in enumerate(larger_hh_size_array):
@@ -394,225 +441,18 @@
 
             home[nj] = aj
         homes_dic[hs].append(home)
 
     for hs in homes_dic:
         homes_dic[hs] = np.array(homes_dic[hs]).astype(int)
 
-    # at this point everyone should have been placed into a home
-    sum_remaining = sum(ages_left_to_assign.values())
-    assert sum_remaining == 0, f"Check failed: generating larger households 'fixed_ages' method. {sum_remaining} and {ages_left_to_assign}."
+    assert sum(ages_left_to_assign.values()) == 0, 'Check failed: generating larger households method 2.'  # at this point everyone should have been placed into a home
     return homes_dic, ages_left_to_assign
 
 
-def generate_all_households_fixed_ages(n_remaining, hh_sizes, hha_by_size, hha_brackets, cm_age_brackets, cm_age_by_brackets, contact_matrices, ages_left_to_assign):
-    """
-    Generate the ages of those living in households together. First create
-    households of people living alone, then larger households. For households
-    larger than 1, a reference individual's age is sampled conditional on the
-    household size, while all other household members have their ages sampled
-    conditional on the reference person's age and the age mixing contact matrix
-    in households for the population under study. Fix the count of ages in the
-    population before placing individuals in households so that the age
-    distribution of the generated population is fixed to closely match the age
-    distribution from data on the population.
-
-    Args:
-        n_remaining (int)             : The number of people in the population left to place in a residence.
-        hh_sizes (array)              : The count of household size s at index s-1.
-        hha_by_size_counts (matrix)   : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
-        hha_brackets (dict)           : The age brackets for the heads of household.
-        cm_age_brackets (dict)        : The dictionary mapping age bracket keys to age bracket range matching the household contact matrix.
-        cm_age_by_brackets (dict) : The dictionary mapping age to the age bracket range it falls within matching the household contact matrix.
-        contact_matrices (dict)     : The dictionary of the age-specific contact matrix for different physical contact settings.
-        ages_left_to_assign (dict)    : Age count of people left to place in households larger than one person.
-
-    Returns:
-        An array of all households where each household is a row and the values
-        in the row are the ages of the household members. The first age in the
-        row is the age of the reference individual. Households are randomly
-        shuffled by size.
-    """
-    log.debug('generate_all_households_fixed_ages()')
-    household_sizes = generate_household_sizes(hh_sizes)
-
-    # generate the ages for heads of households or reference persons conditional on the household size and the age distribution
-    household_head_ages, ages_left_to_assign = generate_household_head_ages(household_sizes, hha_by_size, hha_brackets, ages_left_to_assign)
-
-    homes_dic = dict()
-
-    # find all of the people living alone and their ages
-    living_alone = list(household_head_ages[household_sizes == 1])
-    homes_dic[1] = np.array(living_alone).astype(int).reshape((len(living_alone), 1))  # make an array of each individual home
-
-    # arrays of the larger household sizes and the ages of the heads or reference persons for each (reference person ages generated conditional on household size and age distribution)
-    larger_household_sizes = household_sizes[household_sizes > 1]
-    heads_of_larger_households = household_head_ages[household_sizes > 1]
-
-    for size in range(2, len(hh_sizes) + 1):
-        homes_dic[size] = []
-
-    # work off a copy of the household mixing matrix
-    household_matrix = sc.dcp(contact_matrices['H'])
-
-    homes_dic, ages_left_to_assign = generate_larger_households_fixed_ages(larger_household_sizes, heads_of_larger_households, hha_brackets, cm_age_brackets, cm_age_by_brackets, household_matrix, ages_left_to_assign, homes_dic)
-    homes = get_all_households(homes_dic)
-
-    return homes_dic, homes
-
-
-def generate_larger_households_infer_ages(size, larger_household_sizes, heads_of_larger_households, hha_brackets, cm_age_brackets, cm_age_by_brackets, household_matrix, adjusted_age_dist, p=0.15):
-    """
-    Generate ages of those living in households of greater than one individual.
-    Reference individual is sampled conditional on the household size. All other
-    household members have their ages sampled conditional on the reference
-    person's age and the age mixing contact matrix in households for the
-    population under study.
-
-    Args:
-        size (int)                   : The household size.
-        hh_sizes (array)             : The count of household size s at index s-1.
-        hha_by_size_counts (matrix)  : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
-        hha_brackets (dict)          : The age brackets for the heads of household.
-        cm_age_brackets (dict)       : The dictionary mapping age bracket keys to age bracket range matching the household contact matrix.
-        cm_age_by_brackets (dict)    : The dictionary mapping age to the age bracket range it falls within matching the household contact matrix.
-        household_matrix (dict)      : Age-specific contact matrix for contacts in the household setting.
-        single_year_age_distr (dict) : The age distribution.
-
-    Returns:
-        An array of households for size ``size`` where each household is a row
-        and the values in the row are the ages of the household members. The
-        first age in the row is the age of the reference individual.
-    """
-    log.debug('generate_larger_households_infer_ages()')
-    # calibrated to work for Seattle metro - use fixed_ages method for other populations
-    # p = 0.15  # This is a placeholder value. Users will need to change this to fit whatever population they are working with if using this method
-
-    household_size_mask = larger_household_sizes == size
-    households_of_this_size = larger_household_sizes[household_size_mask]
-    heads_of_this_size = heads_of_larger_households[household_size_mask]
-
-    homes = np.zeros((len(households_of_this_size), size), dtype=int)
-
-    for nh in range(len(households_of_this_size)):
-
-        hha = heads_of_this_size[nh]
-
-        homes[nh][0] = hha
-
-        b = cm_age_by_brackets[hha]
-        b = min(b, household_matrix.shape[0] - 1)  # Ensure it doesn't go past the end of the array - likely not needed
-        b_prob = household_matrix[b, :]
-
-        for n in range(1, size):
-            bi = spsamp.sample_single_arr(b_prob)
-            ai = spsamp.sample_from_range(adjusted_age_dist, cm_age_brackets[bi][0], cm_age_brackets[bi][-1])  # sample from a range, defining the probabilities of the distribution and the minimum and maximum of the range
-
-            if ai > 5 and ai <= 20:  # This is a placeholder range. Users will need to change this to fit their whatever population they are working with if using this method
-                if np.random.binomial(1, p):
-                    ai = spsamp.sample_from_range(adjusted_age_dist, 25, 32)
-
-            ai = spltcf.ltcf_resample_age(adjusted_age_dist, ai)
-
-            homes[nh][n] = ai
-
-    return homes
-
-
-def generate_all_households_infer_ages(n, n_remaining, hh_sizes, hha_by_size, hha_brackets, cm_age_brackets, cm_age_by_brackets, contact_matrices, adjusted_age_dist, ages_left_to_assign):
-    """
-    Generate the ages of those living in households together. First create
-    households of people living alone, then larger households. For households
-    larger than 1, a reference individual's age is sampled conditional on the
-    household size, while all other household members have their ages sampled
-    conditional on the reference person's age and the age mixing contact matrix
-    in households for the population under study.
-
-    Args:
-        n (int)                     : The number of people in the population.
-        n_remaining (int)           : The number of people in the population left to place in a residence.
-        hh_sizes (array)            : The count of household size s at index s-1.
-        hha_by_size_counts (matrix) : A matrix in which each row contains the age distribution of the reference person for household size s at index s-1.
-        hha_brackets (dict)         : The age brackets for the heads of household.
-        cm_age_brackets (dict)      : The dictionary mapping age bracket keys to age bracket range matching the household contact matrix.
-        cm_age_by_brackets (dict)   : The dictionary mapping age to the age bracket range it falls within matching the household contact matrix.
-        contact_matrices (dict)     : The dictionary of the age-specific contact matrix for different physical contact settings.
-        ages_left_to_assign (dict)  : Age count of people left to place in households larger than one person.
-
-    Returns:
-        An array of all households where each household is a row and the values
-        in the row are the ages of the household members. The first age in the
-        row is the age of the reference individual. Households are randomly
-        shuffled by size.
-
-    Note:
-        This method is not guaranteed to model the population age distribution
-        well automatically. The method called inside,
-        generate_larger_households_infer_ages uses the method ltcf_resample_age to
-        fit Seattle, Washington populations with long term care facilities
-        generated. For a method that matches the age distribution well for
-        populations in general, please use generate_all_households_fixed_ages.
-
-        The following contains an example of how you may resample from an age
-        range that is over produced and instead sample ages from an age range
-        that is under produced in your population. This kind of customization
-        may be necessary when your age mixing matrix and the population you are
-        interested in modeling differ in important but subtle ways. For example,
-        generally household age mixing matrices reflect mixing patterns for
-        households composed of families. This means household age mixing
-        matrices do not generally cover college or university aged individuals
-        living together. Without this customization, this algorithm tends to
-        under produce young adults. This method also has a tendency to
-        underproduce the elderly, and does not explicitly model the elderly
-        living in nursing homes. Customizations like this should be considered
-        in context of the specific population and culture you are trying to
-        model. In some cultures, it is common to live in non-family households,
-        while in others family households are the most common and include
-        multi-generational family households. If you are unsure of how to
-        proceed with customizations please take a look at the references listed
-        in the overview documentation for more information.
-    """
-    log.debug('generate_all_households_infer_ages()')
-    household_sizes = generate_household_sizes(hh_sizes)
-
-    # generate the ages for heads of households or reference persons conditional on the household size and the age distribution
-    household_head_ages, ages_left_to_assign = generate_household_head_ages(household_sizes, hha_by_size, hha_brackets, ages_left_to_assign)
-
-    homes_dic = dict()
-
-    # find all of the people living alone and their ages
-    living_alone = list(household_head_ages[household_sizes == 1])
-    homes_dic[1] = np.array(living_alone).astype(int).reshape((len(living_alone), 1))  # make an array of each individual home
-
-    # arrays of the larger household sizes and the ages of the heads or reference persons for each (reference person ages generated conditional on household size and age distribution)
-    larger_household_sizes = household_sizes[household_sizes > 1]
-    heads_of_larger_households = household_head_ages[household_sizes > 1]
-
-    for size in range(2, len(hh_sizes) + 1):
-        homes_dic[size] = []
-
-    # work off a copy of the household mixing matrix
-    household_matrix = sc.dcp(contact_matrices['H'])
-
-    # remove the ages of household heads or reference persons already places
-    for hha in household_head_ages:
-        adjusted_age_dist[hha] -= 1 / n
-    for a in adjusted_age_dist:
-        adjusted_age_dist[a] = max(adjusted_age_dist[a], 0)
-    adjusted_age_dist_values = np.array([adjusted_age_dist[a] for a in adjusted_age_dist])
-
-    # generate the large households and ages of those people
-    for size in range(2, len(hh_sizes) + 1):
-        homes_dic[size] = generate_larger_households_infer_ages(size, larger_household_sizes, heads_of_larger_households, hha_brackets, cm_age_brackets, cm_age_by_brackets, household_matrix, adjusted_age_dist_values)
-
-    homes = get_all_households(homes_dic)
-
-    return homes_dic, homes
-
-
 def get_all_households(homes_dic):
     """
     Get all households in a list, randomly assorted.
 
     Args:
         homes_dic (dict): A dictionary of households by age indexed by household size
 
@@ -685,29 +525,28 @@
 
     Returns:
         np.ndarray: An array with rows as household size and columns as
         household head age brackets.
     """
     popdict = pop.popdict
     loc_pars = sc.dcp(pop.loc_pars)
-    # loc_pars.location = None
+    loc_pars.location = None
     hha_brackets = spdata.get_head_age_brackets(**loc_pars)  # temporarily location should be None until data json work will automatically search up when data are not available
 
     # hha_index use age as key and bracket index as value
     hha_index = spb.get_index_by_brackets(hha_brackets)
     uids = get_household_heads(popdict=popdict)
     d = {}
     # construct tables for each houldhold head
     for uid in uids.values():
         d[popdict[uid]['hhid']] = {'hhid': popdict[uid]['hhid'],
                                    'age': popdict[uid]['age'],
                                    'family_size': len(popdict[uid]['contacts']['H']) + 1,
                                    'hh_age_bracket': hha_index[popdict[uid]['age']]}
     df_household_age = pd.DataFrame.from_dict(d, orient="index")
-
     # aggregate by age_bracket (column) and family_size (row)
     df_household_age = df_household_age.groupby(['hh_age_bracket', 'family_size'], as_index=False).count()\
         .pivot(index='family_size', columns='hh_age_bracket', values='hhid').fillna(0)
     return np.array(df_household_age.values)
 
 
 def get_generated_household_size_distribution(household_sizes):
```

### Comparing `synthpops-1.10.5/synthpops/plotting.py` & `synthpops-1.8.0/synthpops/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
 This module provides plotting methods including methods to plot the age-specific contact matrix in different contact layers.
 """
-
 import itertools
 import os
 import sciris as sc
 import numpy as np
+import covasim as cv
+import pandas as pd
 import matplotlib as mplt
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from collections import Counter
-import cmasher as cmr # Uses implicit import
-import cmocean as cmo # Uses implicit import
+import cmasher as cmr
+import cmocean as cmo
 import seaborn as sns
 
 from . import config as cfg
 from . import base as spb
 from . import defaults as spd
 from . import data_distributions as spdata
 from . import ltcfs as spltcf
 from . import households as sphh
 from . import schools as spsch
 from . import workplaces as spw
 from . import contact_networks as spcnx
 from . import pop as sppop
-from . import people as spp
 
 
 __all__ = ['plotting_kwargs', 'calculate_contact_matrix', 'plot_contacts',
            'plot_array', 'plot_ages',
            'plot_household_sizes',
            # 'plot_household_head_ages',
            # 'plot_household_head_ages_by_household_size',
-           'plot_ltcf_resident_sizes',
+           'plot_ltcf_resident_sizes', 
            # 'plot_ltcf_resident_staff_ratios',
            'plot_enrollment_rates_by_age', 'plot_employment_rates_by_age',
            'plot_school_sizes', 'plot_workplace_sizes',
            'plot_household_head_ages_by_size',
            'plot_contact_counts']  # defines what will be * imported from synthpops, eveything else will need to be imported as synthpops.plotting.method_a, etc.
 
 
@@ -146,60 +146,31 @@
         # if loc_pars exists, then update the default_pop_pars with that information
         if 'loc_pars' in self:
             default_pop_pars.update(self['loc_pars'])
 
         # sometimes when not working with a pop object you might be missing location information directly as kwargs and need to use defaults or set the information
         for k in default_pop_pars:
             if k not in self:
-                cfg.logger.debug(f"kwargs is missing key: {k}. Using the default value: {default_pop_pars[k]}.")
+                cfg.logger.info(f"kwargs is missing key: {k}. Using the default value: {default_pop_pars[k]}.")
                 self[k] = default_pop_pars[k]
 
         for k in default_age_pars:
             if k not in self:
-                cfg.logger.debug(f"kwargs is missing key: {k}. Using the default value: {default_age_pars[k]}.")
+                cfg.logger.info(f"kwargs is missing key: {k}. Using the default value: {default_age_pars[k]}.")
                 self[k] = default_age_pars[k]
 
         # loc_pars not in self yet
         if 'loc_pars' not in self:
             self['loc_pars'] = sc.objdict({k: self[k] for k in default_pop_pars})
 
         if not self.smooth_ages:
             self.window_length = 1
 
         return
 
-    def make_title(self, suffix=None, override=False):
-        """
-        Create the title for the figure depending on the location information
-        and if there already exists a preset title_prefix.
-
-        Args:
-            suffix (str) : title suffix
-            override (bool): If True, override the title_prefix already stored in self and create a new one.
-
-        Returns:
-            None.
-        """
-        if suffix is None:
-            suffix = ""
-
-        location_text = [self[k] for k in ['location', 'state_location', 'country_location'] if self[k] is not None]
-        if len(location_text):
-            location_text = location_text[0]
-        else:
-            location_text = ""
-        if override is False:
-            if 'title_prefix' not in self or self.title_prefix is None:
-                self.title_prefix = f"{location_text}_{suffix}"
-        else:
-            self.title_prefix = f"{location_text}_{suffix}"
-
-        self.title_prefix = self.title_prefix.replace('_', ' ').title()
-        return
-
     def restore_defaults(self):
         """Reset matplotlib defaults."""
         mplt.rcParams.update(mplt.rcParamsDefault)
         return
 
     def update_defaults(self, method_defaults, kwargs):
         """Update defaults with method defaults and kwargs."""
@@ -330,15 +301,15 @@
     for aggregated age brackets.
 
     Args:
         matrix (np.array)                  : symmetric contact matrix, element ij is the contact for an average individual in age group i with all of their contacts in age group j
         age_count (dict)                   : dictionary with the count of individuals in the population for each age
         aggregate_age_count (dict)         : dictionary with the count of individuals in the population in each age bracket
         age_brackets (dict)                : dictionary mapping age bracket keys to age bracket range
-        age_by_brackets (dict)             : dictionary mapping age to the age bracket range it falls in
+        age_by_brackets (dict)         : dictionary mapping age to the age bracket range it falls in
         **layer (str)                      : name of the physial contact layer: H for households, S for schools, W for workplaces, C for community, etc.
         **density_or_frequency (str)       : Default value is 'density', see notes for more details.
         **logcolors_flag (bool)            : If True, plot heatmap in logscale
         **aggregate_flag (bool)            : If True, plot the contact matrix for aggregate age brackets, else single year age contact matrix.
         **cmap(str or Matplotlib colormap) : colormap
         **fontsize (int)                   : base font size
         **rotation (int)                   : rotation for x axis labels
@@ -663,15 +634,15 @@
 
 
 def plot_ages(pop, **kwargs):
     """
     Plot a comparison of the expected and generated age distribution.
 
     Args:
-        pop (pop object)    : population, either synthpops.pop.Pop, sp.people.People, or dict
+        pop (pop object)    : population, either synthpops.pop.Pop, covasim.people.People, or dict
         **left (float)      : Matplotlib.figure.subplot.left
         **right (float)     : Matplotlib.figure.subplot.right
         **top (float)       : Matplotlib.figure.subplot.top
         **bottom (float)    : Matplotlib.figure.subplot.bottom
         **color_1 (str)     : color for expected data
         **color_2 (str)     : color for data from generated population
         **fontsize (float)  : Matplotlib.figure.fontsize
@@ -680,15 +651,15 @@
         **do_show (bool)    : If True, show the plot
         **do_save (bool)    : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
-        If using pop with type sp.people.Pop or dict, args must be supplied
+        If using pop with type covasim.people.Pop or dict, args must be supplied
         for the location parameters to get the expected distribution.
 
     **Example**::
 
         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_age_distribution_comparison()
@@ -708,37 +679,38 @@
 
     # define after plkwargs gets updated
     if isinstance(pop, sppop.Pop):
         plkwargs.loc_pars = pop.loc_pars
         plkwargs.smooth_ages = pop.smooth_ages
         plkwargs.window_length = pop.window_length
 
-    elif not isinstance(pop, (dict, spp.People)):
+    elif not isinstance(pop, (dict, cv.people.People)):
         raise NotImplementedError(f"This method does not support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
 
     # now check for missing plkwargs and use default values if not found
     plkwargs.set_default_pop_pars()
-    plkwargs.make_title("age distribution")
+    if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+        plkwargs.title_prefix = f"{plkwargs.location}_age_distribution"
 
     # get the expected age distribution
-    expected_age_dist = spdata.get_smoothed_single_year_age_distr(**sc.mergedicts(plkwargs.loc_pars, dict(window_length=plkwargs.window_length)))
+    expected_age_dist = spdata.get_smoothed_single_year_age_distr(**sc.mergedicts(plkwargs.loc_pars, dict(window_length= plkwargs.window_length)))
     expected_age_dist_values = [expected_age_dist[k] * 100 for k in sorted(expected_age_dist.keys())]
 
     if plkwargs.comparison:
         generated_age_count = dict.fromkeys(expected_age_dist.keys(), 0)  # sets ordering of keys consistently
 
         # get the generated age distribution
         if isinstance(pop, sppop.Pop):
             generated_age_count = pop.information.age_count
 
         elif isinstance(pop, dict):
             generated_age_count = spb.count_ages(pop)
 
-        elif isinstance(pop, spp.People):
-            generated_age_count = sc.mergedicts(generated_age_count, Counter(pop.age))  # with smaller populations, pop.age might not have all ages
+        elif isinstance(pop, cv.people.People):
+            generated_age_count = Counter(pop.age)
 
         generated_age_dist = spb.norm_dic(generated_age_count)
         generated_age_dist_values = [generated_age_dist[k] * 100 for k in sorted(generated_age_dist.keys())]
         max_y = np.ceil(max(0, max(expected_age_dist_values), max(generated_age_dist_values)))
 
     else:
         generated_age_dist_values = None
@@ -781,15 +753,15 @@
         **do_save (bool)    : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
         If using pop with type dict, args must be supplied for the location
-        parameter to get the expected rates. sp.people.People pop type
+        parameter to get the expected rates. Covasim.people.People pop type
         not yet supported.
 
     **Example**::
 
         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_household_sizes()
@@ -811,15 +783,16 @@
     if isinstance(pop, sppop.Pop):
         plkwargs.loc_pars = pop.loc_pars
     elif not isinstance(pop, dict):
         raise NotImplementedError(f"This method does not yet support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
 
     # now check for the missing plkwargs and use default values if not found
     plkwargs.set_default_pop_pars()
-    plkwargs.make_title("household sizes")
+    if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+        plkwargs.title_prefix = f"{plkwargs.location}_household_sizes"
 
     # get the expected household size distribution
     expected_household_size_dist = spdata.get_household_size_distr(**plkwargs.loc_pars)
     expected_household_size_dist_values = [expected_household_size_dist[k] * 100 for k in sorted(expected_household_size_dist.keys())]
 
     if plkwargs.comparison:
         generated_household_size_count = dict.fromkeys(expected_household_size_dist.keys(), 0)
@@ -854,14 +827,80 @@
     ax.tick_params(labelsize=plkwargs.fontsize)
 
     fig = finalize_figure(fig, plkwargs)
 
     return fig, ax
 
 
+# # TBC: placeholder for now
+# def plot_household_head_ages(pop, **kwargs):
+#     """
+#     Plot a comparison of the expected and generated head of household ages.
+
+#     Args:
+#         pop (pop object)    : population, either synthpops.pop.Pop or dict
+#         **left (float)      : Matplotlib.figure.subplot.left
+#         **right (float)     : Matplotlib.figure.subplot.right
+#         **top (float)       : Matplotlib.figure.subplot.top
+#         **bottom (float)    : Matplotlib.figure.subplot.bottom
+#         **color_1 (str)     : color for expected data
+#         **color_2 (str)     : color for data from generated population
+#         **fontsize (float)  : Matplotlib.figure.fontsize
+#         **figname (str)     : name to save figure to disk
+#         **comparison (bool) : If True, plot comparison to the generated population
+#         **do_show (bool)    : If True, show the plot
+#         **do_save (bool)    : If True, save the plot to disk
+
+#     Returns:
+#         Matplotlib figure and axes.
+
+#     Note:
+#         If using pop with type dict, args must be supplied for the location
+#         parameter to get the expected rates. Covasim.people.People pop type
+#         not yet supported.
+
+#     **Example**::
+
+#         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
+#         pop = sp.Pop(**pars)
+#         fig, ax = pop.plot_household_head_ages()
+
+#         popdict = pop.to_dict()
+#         kwargs = pars.copy()
+#         kwargs['datadir'] = sp.datadir
+#         fig, ax = sp.plot_household_head_ages(popdict, **kwargs)
+#     """
+#     plkwargs = get_plkwargs(pop)
+#     cmap = plt.get_cmap('rocket')
+
+#     # method specific plotting defaults
+#     method_defaults = dict(left=0.10, right=0.95, top=0.90, bottom=0.10, color_1=cmap(0.63), color_2=cmap(0.45),
+#                            fontsize=12, figname='enrollment_rates_by_age', comparison=True, binned=True)
+
+#     plkwargs.update_defaults(method_defaults, kwargs)
+
+#     # define after plkwargs gets updated
+#     if isinstance(pop, sppop.Pop):
+#         plkwargs.loc_pars = pop.loc_pars
+#     elif not isinstance(pop, dict):
+#         raise ValueError(f"This method does not yet support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
+
+#     # now check for the missing plkwargs and use default values if not found
+#     plkwargs.set_default_pop_pars()
+#     if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+#         plkwargs.title_prefix = f"{plkwargs.location}_household_head_ages_by_household_size"
+
+#     fig, ax = plt.subplots(1, 1, figsize=(plkwargs.width, plkwargs.height), dpi=plkwargs.display_dpi)
+#     fig.subplots_adjust(**plkwargs.axis)
+
+#     fig = finalize_figure(fig, plkwargs)
+
+#     return fig, ax
+
+
 def plot_ltcf_resident_sizes(pop, **kwargs):
     """
     Plot a comparison of the expected and generated ltcf resident sizes.
 
     Args:
         pop (pop object)    : population, either synthpops.pop.Pop or dict
         **left (float)      : Matplotlib.figure.subplot.left
@@ -877,15 +916,15 @@
         **do_save (bool)    : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
         If using pop with type dict, args must be supplied for the location
-        parameter to get the expected rates. sp.people.People pop type
+        parameter to get the expected rates. Covasim.people.People pop type
         not yet supported.
 
     **Example**::
 
         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_ltcf_resident_sizes()
@@ -908,15 +947,16 @@
     if isinstance(pop, sppop.Pop):
         plkwargs.loc_pars = pop.loc_pars
     elif not isinstance(pop, dict):
         raise NotImplementedError(f"This method does not yet support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
 
     # now check for the missing plkwargs and use default values if not found
     plkwargs.set_default_pop_pars()
-    plkwargs.make_title("long term care facility resident sizes")
+    if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+        plkwargs.title_prefix = f"{plkwargs.location}_ltcf_resident_sizes"
 
     # get the expected ltcf resident sizes
     expected_ltcf_resident_sizes_binned = spdata.get_long_term_care_facility_residents_distr(**plkwargs.loc_pars)
     expected_ltcf_resident_sizes_binned_values = [expected_ltcf_resident_sizes_binned[k] * 100 for k in sorted(expected_ltcf_resident_sizes_binned.keys())]
     ltcf_resident_size_brackets = spdata.get_long_term_care_facility_residents_distr_brackets(**plkwargs.loc_pars)
     bins = spb.get_bin_edges(ltcf_resident_size_brackets)
     bin_labels = spb.get_bin_labels(ltcf_resident_size_brackets)
@@ -975,15 +1015,15 @@
 #         **do_save (bool)    : If True, save the plot to disk
 
 #     Returns:
 #         Matplotlib figure and axes.
 
 #     Note:
 #         If using pop with type dict, args must be supplied for the location
-#         parameter to get the expected rates. sp.people.People pop type
+#         parameter to get the expected rates. Covasim.people.People pop type
 #         not yet supported.
 
 #     **Example**::
 
 #         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
 #         pop = sp.Pop(**pars)
 #         fig, ax = pop.plot_ltcf_resident_staff_ratios()
@@ -1024,15 +1064,15 @@
         **do_save (bool)    : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
         If using pop with type dict, args must be supplied for the location
-        parameter to get the expected rates. sp.people.People pop type
+        parameter to get the expected rates. Covasim.people.People pop type
         not yet supported.
 
     **Example**::
 
         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_enrollment_rates_by_age()
@@ -1054,15 +1094,16 @@
     if isinstance(pop, sppop.Pop):
         plkwargs.loc_pars = pop.loc_pars
     elif not isinstance(pop, dict):
         raise NotImplementedError(f"This method does not yet support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
 
     # now check for the missing plkwargs and use default values if not found
     plkwargs.set_default_pop_pars()
-    plkwargs.make_title("enrollment rates by age")
+    if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+        plkwargs.title_prefix = f"{plkwargs.location}_enrollment_rates_by_age"
 
     # get the expected enrollment rates
     expected_enrollment_rates_by_age = spdata.get_school_enrollment_rates(**plkwargs.loc_pars)
     expected_enrollment_rates_by_age_values = [expected_enrollment_rates_by_age[a] * 100 for a in sorted(expected_enrollment_rates_by_age.keys())]
 
     if plkwargs.comparison:
         generated_enrollment_rates_by_age = dict.fromkeys(expected_enrollment_rates_by_age.keys(), 0)
@@ -1116,15 +1157,15 @@
         **do_save (bool)    : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
         If using pop with type dict, args must be supplied for the location
-        parameter to get the expected rates. sp.people.People pop type
+        parameter to get the expected rates. Covasim.people.People pop type
         not yet supported.
 
     **Example**::
 
         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_employment_rates_by_age()
@@ -1146,15 +1187,16 @@
     if isinstance(pop, sppop.Pop):
         plkwargs.loc_pars = pop.loc_pars
     elif not isinstance(pop, dict):
         raise NotImplementedError(f"This method does not support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
 
     # now check for the missing plkwargs and use default values if not found
     plkwargs.set_default_pop_pars()
-    plkwargs.make_title("employment rates by age")
+    if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+        plkwargs.title_prefix = f"{plkwargs.location}_employment_rates_by_age"
 
     # get the expected employment rates
     expected_employment_rates_by_age = dict.fromkeys(np.arange(spd.settings.max_age), 0)
     expected_employment_rates_by_age = sc.mergedicts(expected_employment_rates_by_age, spdata.get_employment_rates(**plkwargs.loc_pars))
     expected_employment_rates_by_age_values = [expected_employment_rates_by_age[a] * 100 for a in sorted(expected_employment_rates_by_age.keys())]
 
     if plkwargs.comparison:
@@ -1216,15 +1258,15 @@
         **do_show (bool)                : If True, show the plot
         **do_save (bool)                : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
-        If using pop with type sp.people.Pop or dict, args must be supplied
+        If using pop with type covasim.people.Pop or dict, args must be supplied
         for the location parameters to get the expected distribution.
 
     **Example**::
 
         pars = {'n': 10e3, 'location'='seattle_metro', 'state_location'='Washington', 'country_location'='usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_school_sizes_by_type()
@@ -1286,16 +1328,19 @@
         expected_school_size_dist.pop(school_type, None)
         plkwargs.school_type_labels.pop(school_type, None)
 
     sorted_school_types = sorted(expected_school_size_dist.keys())
     n_school_types = len(sorted_school_types)
     plkwargs.nrows = n_school_types
 
-    plkwargs.make_title()  # make title_prefix with just location information
-    location_text = plkwargs.title_prefix
+    # location text
+    if plkwargs.location is not None:
+        location_text = f"{plkwargs.location.replace('_', ' ').title()}"
+    else:
+        location_text = f"{spd.settings.location.replace('_', ' ').title()}"
 
     # create fig, ax, set cmap
     fig, ax = plt.subplots(n_school_types, 1, figsize=(plkwargs.display_width, plkwargs.display_height), dpi=plkwargs.display_dpi)
     cmap = mplt.cm.get_cmap(plkwargs.cmap)
 
     # readjust figure parameters
     if plkwargs.nrows == 1:
@@ -1377,15 +1422,15 @@
         **do_save (bool)    : If True, save the plot to disk
 
     Returns:
         Matplotlib figure and axes.
 
     Note:
         If using pop with type dict, args must be supplied for the location
-        parameter to get the expected rates. sp.people.People pop type
+        parameter to get the expected rates. Covasim.people.People pop type
         not yet supported.
 
     **Example**::
 
         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
         pop = sp.Pop(**pars)
         fig, ax = pop.plot_workplace_sizes()
@@ -1408,15 +1453,16 @@
     if isinstance(pop, sppop.Pop):
         plkwargs.loc_pars = pop.loc_pars
     elif not isinstance(pop, dict):
         raise NotImplementedError(f"This method does not yet support pop objects with the type {type(pop)}. Please look at the notes and try another supported pop type.")
 
     # now check for the missing plkwargs and use default values if not found
     plkwargs.set_default_pop_pars()
-    plkwargs.make_title("workplace sizes")
+    if 'title_prefix' not in plkwargs or plkwargs.title_prefix is None:
+        plkwargs.title_prefix = f"{plkwargs.location}_workplace_sizes"
 
     # get the expected workplace sizes
     temp_loc_pars = sc.dcp(plkwargs.loc_pars)  # to be removed once data for location is merged
     temp_loc_pars.location = None
     expected_work_sizes_binned = spb.norm_dic(spdata.get_workplace_size_distr_by_brackets(**temp_loc_pars))
     expected_work_sizes_binned_values = [expected_work_sizes_binned[k] * 100 for k in sorted(expected_work_sizes_binned.keys())]
     work_size_brackets = spdata.get_workplace_size_brackets(**temp_loc_pars)
@@ -1498,47 +1544,49 @@
                                  fontsize=14,
                                  cmap="rocket_r",
                                  figname="household_head_age_family_size",
                                  height=8, width=17, rotation=45,
                                  )
     plkwargs.update_defaults(method_defaults, kwargs)
 
+    pop.loc_pars.location = None
+
     # get the labels of the head of household age brackets
     hha_brackets = spdata.get_head_age_brackets(**pop.loc_pars)
     xticklabels = [f"{hha_brackets[b][0]}-{hha_brackets[b][-1]}" for b in hha_brackets.keys()]
 
     expected_hh_ages = spdata.get_head_age_by_size_distr(**pop.loc_pars)
 
     # we will ignore the first row (family_size = 1) for plotting
     # flip to make each row an age bin for calculation then flip back
-    expected_hh_ages = expected_hh_ages[0:len(expected_hh_ages), :]  # include all household sizes, including 1
+    expected_hh_ages = expected_hh_ages[1:len(expected_hh_ages), :]
 
     expected_hh_ages_percentage = expected_hh_ages / np.sum(expected_hh_ages, axis=1)[:, np.newaxis]
     expected_hh_ages_percentage[np.isnan(expected_hh_ages_percentage)] = 0
 
     expected_hh_ages_percentage *= 100
 
     actual_hh_ages = sphh.get_household_head_ages_by_size(pop)
-    actual_hh_ages = actual_hh_ages[0:len(expected_hh_ages), :]  # include all household sizes, including 1
+    actual_hh_ages = actual_hh_ages[1:len(expected_hh_ages), :]
 
     actual_hh_ages_percentage = actual_hh_ages / np.sum(actual_hh_ages, axis=1)[:, np.newaxis]
     actual_hh_ages_percentage[np.isnan(actual_hh_ages_percentage)] = 0
 
     actual_hh_ages_percentage *= 100
 
     # spdata.get_head_age_by_size_distr returns an extra row so we need to match number of rows
     householdsize_rows = min(len(actual_hh_ages_percentage), len(expected_hh_ages_percentage))
-    household_sizes = [i + 1 for i in range(0, len(expected_hh_ages_percentage) - 1)]
+    household_sizes = [i + 2 for i in range(0, len(expected_hh_ages_percentage) - 1)]
     yticklabels = household_sizes
 
     interval = 5
 
     data_range_min = 0
     data_range_max = max(np.max(expected_hh_ages_percentage), np.max(actual_hh_ages_percentage))
-    data_range_max = int(np.ceil(data_range_max / interval)) * interval
+    data_range_max = int(np.ceil(data_range_max/interval)) * interval
     data_range = [data_range_min, data_range_max]
 
     return plot_heatmap(expected=expected_hh_ages_percentage[0:householdsize_rows, :],
                         actual=actual_hh_ages_percentage[0:householdsize_rows, :],
                         xticklabels=xticklabels, yticklabels=yticklabels,
                         xlabel='Head of Household Age', ylabel='Household Size',
                         cbar_ylabel='%',
@@ -1609,15 +1657,15 @@
     axs[1].set_title('Generated', fontsize=plkwargs.fontsize + 1)
     fig.suptitle(plkwargs.title_prefix, fontsize=plkwargs.fontsize + 1)
 
     divider = make_axes_locatable(axs[1])
     cax = divider.new_horizontal(size=plkwargs.divider_size, pad=plkwargs.divider_pad)
     fig.add_axes(cax)
     cbar = fig.colorbar(im[1], cax=cax)
-    cbar.ax.tick_params(axis='y', labelsize=plkwargs.fontsize - 2)
+    cbar.ax.tick_params(axis='y', labelsize=plkwargs.fontsize-2)
     cbar.ax.set_ylabel(cbar_ylabel)
 
     finalize_figure(fig, plkwargs)
 
     return fig, ax
 
 
@@ -1656,22 +1704,22 @@
 
     if max(len(people_types), len(contact_types)) > 1:
         fig.tight_layout()
         for ax, counter in zip(axes.flatten(), list(itertools.product(people_types, contact_types))):
             ax.hist(contact_counter[counter[0]][counter[1]], color=plkwargs.color_1, edgecolor=plkwargs.color_2, rwidth=0.8)
             ax.set_title(f'{counter[0]} to {counter[1]}', fontsize=plkwargs.fontsize)
             ax.tick_params(which='major', labelsize=plkwargs.fontsize)
-            ax.set_xlabel('No. of contacts', fontsize=plkwargs.fontsize - 1)
+            ax.set_xlabel('No. of contacts', fontsize=plkwargs.fontsize-1)
     else:
         from_index = list(people_types)[0]
         to_index = list(contact_types)[0]
         axes.hist(contact_counter.get(from_index).get(to_index), color=plkwargs.color_1, edgecolor=plkwargs.color_2, rwidth=0.8)
         axes.set_title(f'{from_index} to {to_index}', fontsize=plkwargs.fontsize)
         axes.tick_params(which='major', labelsize=plkwargs.fontsize)
-        axes.set_xlabel('No. of contacts', fontsize=plkwargs.fontsize - 1)
+        axes.set_xlabel('No. of contacts', fontsize=plkwargs.fontsize-1)
 
     finalize_figure(fig, plkwargs)
     plt.close()
     return fig, axes
 
 
 # dev / analysis tool
@@ -1699,20 +1747,18 @@
         degree_df = spcnx.count_layer_degree(pop, layer, ages, uids, uids_included)
 
     plkwargs = plotting_kwargs()
     # default_cmap = sns.cubehelix_palette(light=1, as_cmap=True)
     default_cmap = mplt.cm.get_cmap("rocket")
     method_defaults = sc.objdict(cmap=default_cmap, alpha=0.99, thresh=0.0001, cbar=True,
                                  shade=True, xlim=[0, 101], height=5, ratio=5,
-                                 # title_prefix=f"Degree by Age for Layer: {layer}",
+                                 title_prefix=f"Degree by Age for Layer: {layer}",
                                  fontsize=10, save_dpi=400,
                                  )
     plkwargs.update_defaults(method_defaults, kwargs)
-    plkwargs.set_default_pop_pars()
-    plkwargs.make_title(f"Degree by Age for Layer: {layer}")
 
     interval = 5
     max_y = int(np.ceil(max(degree_df['degree'].values) / interval) * interval)
     min_y = min(degree_df['degree'].values)
     max_b = max(max_y, plkwargs.xlim[-1])
 
     if kind == 'kde':
@@ -1742,15 +1788,15 @@
                           ratio=plkwargs.ratio, height=plkwargs.height, space=0,
                           bins=max_b,
                           marginal_kws=dict(bins=np.arange(0, max_b)),
                           )
 
     g.plot_marginals(sns.kdeplot, color=plkwargs.cmap(0.5), shade=plkwargs.shade, alpha=plkwargs.alpha * 0.8, legend=False)
 
-    g.fig.suptitle(plkwargs.title_prefix, fontsize=plkwargs.fontsize + 1.5)
+    g.fig.suptitle(plkwargs.title_prefix, fontsize=plkwargs.fontsize+1.5, horizontalalignment='left')
     g.ax_joint.set_xlabel('Age', fontsize=plkwargs.fontsize)
     g.ax_joint.set_ylabel('Degree', fontsize=plkwargs.fontsize)
     g.ax_joint.tick_params(labelsize=plkwargs.fontsize)
 
     finalize_figure(g.fig, plkwargs)
     return g
 
@@ -1777,25 +1823,23 @@
     if degree_df is None:
         degree_df = spcnx.count_layer_degree(pop, layer, ages, uids, uids_included)
 
     plkwargs = plotting_kwargs()
     cmap = sns.cubehelix_palette(light=1, as_cmap=True)
     method_defaults = sc.objdict(cmap=cmap, alpha=0.99, thresh=0.001, cbar=True,
                                  shade=True, xlim=[0, 101], height=7,
+                                 title_prefix=f"Degree by Age for Layer: {layer}",
                                  fontsize=10, save_dpi=400,
                                  )
     plkwargs.update_defaults(method_defaults, kwargs)
-    plkwargs.set_default_pop_pars()
-    plkwargs.make_title(f"Degree by Age for Layer: {layer}")
-
     fig, ax = plt.subplots(1, 1, figsize=(plkwargs.height, plkwargs.height))
     ax = sns.boxplot(x='age', y='degree', data=degree_df, palette=[plkwargs.cmap(0.5)], ax=ax)
     ax.set_xticks(np.arange(plkwargs.xlim[0], plkwargs.xlim[1], 10))
     ax.set_xlim(plkwargs.xlim)
-    ax.set_title(plkwargs.title_prefix, fontsize=plkwargs.fontsize + 2)
+    ax.set_title('Workplace Degree Distribution', fontsize=plkwargs.fontsize+2)
     ax.set_xlabel('Age', fontsize=plkwargs.fontsize)
     ax.set_ylabel('Degree', fontsize=plkwargs.fontsize)
     finalize_figure(fig, plkwargs)
 
     return fig, ax
 
 
@@ -1820,29 +1864,27 @@
     Returns:
         Matplotlib figure and axes.
     """
     plkwargs = plotting_kwargs()
     method_defaults = sc.objdict(alpha=0.99, thresh=0.001, cbar=True, shade=True, xlim=[0, 101],
                                  subplot_height=3, subplot_width=3.1, left=0.06, right=0.97, bottom=0.10)
     plkwargs.update_defaults(method_defaults, kwargs)
-    plkwargs.set_default_pop_pars()
-
     plkwargs.height = np.ceil(len(pop_list) / 3) * plkwargs.subplot_height
     plkwargs.width = (len(pop_list) % 3 + 3) * plkwargs.subplot_width
 
     ncols = min(3, len(pop_list))
     nrows, ncols = sc.get_rows_cols(len(pop_list), ncols=ncols)
     fig, axes = plt.subplots(nrows=nrows, ncols=ncols, figsize=(plkwargs.width, plkwargs.height), dpi=plkwargs.display_dpi)
 
     fig.subplots_adjust(**plkwargs.axis)
 
     interval = 5
 
     for ni, pop in enumerate(pop_list):
-        cmap = sns.cubehelix_palette(light=1, as_cmap=True, rot=(ni + 1) * 0.1)
+        cmap = sns.cubehelix_palette(light=1, as_cmap=True, rot=(ni+1) * 0.1)
         degree_dfi = spcnx.count_layer_degree(pop, layer=layer, ages=ages)
         max_y = int(np.ceil(max(degree_dfi['degree'].values) / interval) * interval)
         min_y = int(np.floor(min(degree_dfi['degree'].values) / interval) * interval)
         max_b = max(max_y, plkwargs.xlim[-1])
 
         if len(pop_list) > 3:
             nr = int(ni // 3)
@@ -1861,16 +1903,15 @@
         elif kind == 'hist':
             sns.histplot(x='age', y='degree', data=degree_dfi, cmap=cmap,
                          alpha=plkwargs.alpha, stat='density',
                          cbar=plkwargs.cbar, ax=axi)
 
         axi.set_xlim(plkwargs.xlim)
         axi.set_ylim(min_y, max_y)
-        plkwargs.make_title(f"Pop: {ni} Layer: {layer}", override=True)
-        axi.set_title(plkwargs.title_prefix, fontsize=plkwargs.fontsize)
+        axi.set_title(f'Pop: {ni}  Layer: {layer}', fontsize=plkwargs.fontsize)
 
     finalize_figure(fig, plkwargs)
 
     return fig, axes
 
 
 # dev / analysis tool
@@ -1893,15 +1934,14 @@
         Matplotlib figure and axes.
     """
     plkwargs = plotting_kwargs()
     method_defaults = sc.objdict(alpha=0.8, thresh=0.001, cbar=True, shade=True, xlim=[0, 101],
                                  subplot_height=2.2, subplot_width=6, left=0.06, right=0.97,
                                  bottom=0.08, top=0.92, hspace=0.5, )
     plkwargs.update_defaults(method_defaults, kwargs)
-    plkwargs.set_default_pop_pars()
 
     nrows = len(pop.layers)
 
     plkwargs.height = nrows * plkwargs.subplot_height
     plkwargs.width = plkwargs.subplot_width
 
     fig, axs = plt.subplots(nrows, 1, figsize=(plkwargs.width, plkwargs.height), dpi=plkwargs.display_dpi)
@@ -1922,13 +1962,12 @@
         color = cmap(0.3 + 0.15 * nl)
 
         axs[nl].fill_between(x, ylo, yhi, color=color, alpha=plkwargs.alpha * 0.6, lw=0)
         axs[nl].fill_between(x, y25, y75, color=color, alpha=plkwargs.alpha * 0.8, lw=0)
         axs[nl].plot(x, y, color=color, lw=1.5)
 
         axs[nl].set_xlim(plkwargs.xlim)
-        plkwargs.make_title(pop.layer_mappings[layer], override=True)
-        axs[nl].set_title(plkwargs.title_prefix, fontsize=plkwargs.fontsize)
+        axs[nl].set_title(pop.layer_mappings[layer], fontsize=plkwargs.fontsize)
 
     finalize_figure(fig, plkwargs)
 
     return fig, axs
```

### Comparing `synthpops-1.10.5/synthpops/pop.py` & `synthpops-1.8.0/synthpops/pop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
-This module provides the main class for interacting with SynthPops, the Pop class.
+This module provides the layer for communicating with the agent-based model Covasim.
 """
 
 import numpy as np
 import sciris as sc
 from .config import logger as log
 from . import version as spv
-from . import defaults
-from . import base as spb
 from . import config as cfg
 from . import sampling as spsamp
+from . import base as spb
 from . import data_distributions as spdata
+from . import contact_networks as spcnx
 from . import ltcfs as spltcf
 from . import households as sphh
 from . import schools as spsch
 from . import workplaces as spw
-from . import contact_networks as spcnx
 from . import plotting as sppl
-from . import people as spp
+from . import defaults
 
 
 __all__ = ['Pop', 'make_population', 'generate_synthetic_population']
 
 
 class Pop(sc.prettyobj):
 
@@ -112,27 +111,26 @@
             do_make (bool)                          : whether to make the population
 
         Returns:
             network (dict): A dictionary of the full population with ages, connections, and other attributes.
         '''
         log.debug('Pop()')
 
+        # Assign all the variables
+        self.loc_pars           = sc.objdict()
+        self.school_pars        = sc.objdict()
+        self.ltcf_pars          = sc.objdict()
+
         # General parameters
         if n is None:
             log.warning(f"Pop size n not given, generating a population with a default size of {defaults.default_pop_size} people.")
             n = defaults.default_pop_size
-
         elif n < defaults.default_pop_size:
             log.warning(f"Pop size n: {n} is too small for synthpops to make contact networks that statistically represent real world populations. Resultant networks may not look realistic.")
 
-        # Assign all the variables
-        self.loc_pars           = sc.objdict()
-        self.school_pars        = sc.objdict()
-        self.ltcf_pars          = sc.objdict()
-
         self.n                  = int(n)
         self.max_contacts       = sc.mergedicts({'W': 20}, max_contacts)
         self.with_industry_code = with_industry_code
         self.rand_seed          = rand_seed
         self.country_location   = country_location
         self.state_location     = state_location
         self.location           = location
@@ -276,83 +274,67 @@
         teacher_age_max                 = self.school_pars.teacher_age_max
         with_non_teaching_staff         = self.school_pars.with_non_teaching_staff
         average_student_all_staff_ratio = self.school_pars.average_student_all_staff_ratio
         average_additional_staff_degree = self.school_pars.average_additional_staff_degree
         staff_age_min                   = self.school_pars.staff_age_min
         staff_age_max                   = self.school_pars.staff_age_max
 
-        # Load and store the expected age distribution of the population
-        age_bracket_dist = spdata.read_age_bracket_distr(**loc_pars)  # age distribution defined by bins or age brackets
-        expected_age_dist = spdata.get_smoothed_single_year_age_distr(**loc_pars, window_length=self.window_length)
-        self.expected_age_dist = expected_age_dist
-        expected_age_dist_values = [expected_age_dist[a] for a in expected_age_dist]
-        self.expected_age_dist_values = expected_age_dist_values
-
-        # Load and store the age brackets
-        age_brackets = spdata.get_census_age_brackets(**loc_pars)
-        self.age_brackets = age_brackets
-        # mapping
-        age_by_brackets = spb.get_age_by_brackets(age_brackets)
-        self.age_by_brackets = age_by_brackets
-
         # Load the contact matrix
         contact_matrices = spdata.get_contact_matrices(datadir, sheet_name=sheet_name)
         # Store expected contact matrices
         self.contact_matrices = contact_matrices
 
         # Load age brackets, and mapping dictionary that matches contact matrices
         contact_matrix_shape = contact_matrices[list(contact_matrices.keys())[0]].shape
         contact_matrix_row = contact_matrix_shape[0]
 
         cm_age_brackets = spdata.get_census_age_brackets(**loc_pars, nbrackets=contact_matrix_row)
-        self.cm_age_brackets = cm_age_brackets
         cm_age_by_brackets = spb.get_age_by_brackets(cm_age_brackets)
-        self.cm_age_by_brackets = cm_age_by_brackets
 
-        # Generate an age count for the population --- this will get passed around to methods generating the different layers where people live: long term care facilities, households, agricultural living quarters, other group living arrangements
-        age_count = sphh.generate_age_count_multinomial(n, expected_age_dist_values)
+        # Generate LTCFs
+        n_nonltcf, age_brackets, age_by_brackets, ltcf_adjusted_age_distr, facilities = spltcf.generate_ltcfs(n, with_facilities, datadir, country_location, state_location, location, use_default, smooth_ages, window_length)
 
-        # Ages left to assign to a residence
-        ages_left_to_assign = sc.dcp(age_count)
-
-        # Generate LTCFs and remove some people from the age count of people left to place in a resident by age
-        n_nonltcf, ltcf_adjusted_age_dist, ltcf_adjusted_age_dist_values, ages_left_to_assign, facilities = spltcf.generate_ltcfs(n, with_facilities, loc_pars, expected_age_dist, ages_left_to_assign)
+        # Store expected age data
+        self.age_brackets = age_brackets
+        self.age_by_brackets = age_by_brackets
 
         # Generate households
-        household_size_dist = spdata.get_household_size_distr(**loc_pars)
-        hh_sizes = sphh.generate_household_size_count_from_fixed_pop_size(n_nonltcf, household_size_dist)
+        household_size_distr = spdata.get_household_size_distr(**loc_pars)
+        hh_sizes = sphh.generate_household_sizes_from_fixed_pop_size(n_nonltcf, household_size_distr)
+
         hha_brackets = spdata.get_head_age_brackets(**loc_pars)
         hha_by_size = spdata.get_head_age_by_size_distr(**loc_pars)
 
         if household_method == 'fixed_ages':
 
-            homes_dic, homes = sphh.generate_all_households_fixed_ages(n_nonltcf, hh_sizes, hha_by_size, hha_brackets, cm_age_brackets, cm_age_by_brackets, contact_matrices, ages_left_to_assign)
+            homes_dic, homes = spltcf.generate_all_households_method_2(n_nonltcf, hh_sizes, hha_by_size, hha_brackets, cm_age_brackets, cm_age_by_brackets, contact_matrices, ltcf_adjusted_age_distr)
 
         else:
-            log.debug("defaulting to 'infer_ages' household generation method. See method notes for description.")
-            homes_dic, homes = sphh.generate_all_households_infer_ages(n, n_nonltcf, hh_sizes, hha_by_size, hha_brackets, cm_age_brackets, cm_age_by_brackets, contact_matrices, ltcf_adjusted_age_dist, ages_left_to_assign)
+            log.debug("defaulting to 'infer_ages' household generation method. See class notes for description.")
+            homes_dic, homes = spltcf.generate_all_households_method_1(n_nonltcf, hh_sizes, hha_by_size, hha_brackets, cm_age_brackets, cm_age_by_brackets, contact_matrices, ltcf_adjusted_age_distr)
 
         # Handle homes and facilities
         homes = facilities + homes
         homes_by_uids, age_by_uid = sphh.assign_uids_by_homes(homes)  # include facilities to assign ids
         age_by_uid_arr = np.array([age_by_uid[i] for i in range(self.n)], dtype=int)
         self.age_by_uid = age_by_uid_arr
 
         facilities_by_uid_lists = homes_by_uids[0:len(facilities)]
 
         # Generate school sizes
-        school_sizes_dist_by_brackets = spdata.get_school_size_distr_by_brackets(**loc_pars)  # without school type
-        school_size_brackets = spdata.get_school_size_brackets(**loc_pars)  # for right now the size distribution for all school types will use the same brackets or bins
+        school_sizes_count_by_brackets = spdata.get_school_size_distr_by_brackets(**loc_pars)
+        school_size_brackets = spdata.get_school_size_brackets(**loc_pars)
 
         # Figure out who's going to school as a student with enrollment rates (gets called inside sp.get_uids_in_school)
         uids_in_school, uids_in_school_by_age, ages_in_school_count = spsch.get_uids_in_school(datadir, n_nonltcf, location, state_location, country_location, age_by_uid, homes_by_uids, use_default=use_default)  # this will call in school enrollment rates
 
         if with_school_types:
             school_size_distr_by_type = spdata.get_school_size_distr_by_type(**loc_pars)
 
+            school_size_brackets = spdata.get_school_size_brackets(**loc_pars)  # for right now the size distribution for all school types will use the same brackets or bins
             school_type_age_ranges = spdata.get_school_type_age_ranges(**loc_pars)
 
             school_types_distr_by_age = spsch.get_school_types_distr_by_age(school_type_age_ranges)
             school_type_by_age = spsch.get_school_types_by_age_single(school_types_distr_by_age)
 
             student_age_lists, student_uid_lists, school_types = spsch.send_students_to_school_with_school_types(school_size_distr_by_type,
                                                                                                                  school_size_brackets,
@@ -360,16 +342,15 @@
                                                                                                                  uids_in_school_by_age,
                                                                                                                  ages_in_school_count,
                                                                                                                  school_types_distr_by_age,
                                                                                                                  school_type_age_ranges)
 
         else:
             # Get school sizes
-            school_sizes = spsch.generate_school_sizes(school_sizes_dist_by_brackets, school_size_brackets, uids_in_school)
-
+            school_sizes = spsch.generate_school_sizes(school_sizes_count_by_brackets, school_size_brackets, uids_in_school)
             # Assign students to school using contact matrix method - generic schools
             student_age_lists, student_uid_lists, school_types = spsch.send_students_to_school(school_sizes,
                                                                                                uids_in_school,
                                                                                                uids_in_school_by_age,
                                                                                                ages_in_school_count,
                                                                                                cm_age_brackets,
                                                                                                cm_age_by_brackets,
@@ -450,61 +431,56 @@
                                                                                                                                                                    cm_age_by_brackets,
                                                                                                                                                                    contact_matrices)
 
         # remove facilities from homes --- have already assigned each person a uid
         homes_by_uids = homes_by_uids[len(facilities_by_uid_lists):]
         homes = homes[len(facilities_by_uid_lists):]
 
-        population = spcnx.make_contacts(self,
-                                         age_by_uid=age_by_uid,
-                                         homes_by_uids=homes_by_uids,
-                                         students_by_uid_lists=student_uid_lists,
-                                         teachers_by_uid_lists=teacher_uid_lists,
-                                         non_teaching_staff_uid_lists=non_teaching_staff_uid_lists,
-                                         workplace_by_uid_lists=workplace_uid_lists,
-                                         facilities_by_uid_lists=facilities_by_uid_lists,
-                                         facilities_staff_uid_lists=facilities_staff_uid_lists,
-                                         use_two_group_reduction=use_two_group_reduction,
-                                         average_LTCF_degree=average_LTCF_degree,
-                                         with_school_types=with_school_types,
-                                         school_mixing_type=school_mixing_type,
-                                         average_class_size=average_class_size,
-                                         inter_grade_mixing=inter_grade_mixing,
-                                         average_student_teacher_ratio=average_student_teacher_ratio,
-                                         average_teacher_teacher_degree=average_teacher_teacher_degree,
-                                         average_student_all_staff_ratio=average_student_all_staff_ratio,
-                                         average_additional_staff_degree=average_additional_staff_degree,
-                                         school_type_by_age=school_type_by_age,
-                                         max_contacts=max_contacts)
+        # population, schools_in_groups = spcnx.make_contacts_from_microstructure_objects(age_by_uid=age_by_uid,
+        population, schools_in_groups = spcnx.make_contacts(age_by_uid=age_by_uid,
+                                                            homes_by_uids=homes_by_uids,
+                                                            students_by_uid_lists=student_uid_lists,
+                                                            teachers_by_uid_lists=teacher_uid_lists,
+                                                            non_teaching_staff_uid_lists=non_teaching_staff_uid_lists,
+                                                            workplace_by_uid_lists=workplace_uid_lists,
+                                                            facilities_by_uid_lists=facilities_by_uid_lists,
+                                                            facilities_staff_uid_lists=facilities_staff_uid_lists,
+                                                            use_two_group_reduction=use_two_group_reduction,
+                                                            average_LTCF_degree=average_LTCF_degree,
+                                                            with_school_types=with_school_types,
+                                                            school_mixing_type=school_mixing_type,
+                                                            average_class_size=average_class_size,
+                                                            inter_grade_mixing=inter_grade_mixing,
+                                                            average_student_teacher_ratio=average_student_teacher_ratio,
+                                                            average_teacher_teacher_degree=average_teacher_teacher_degree,
+                                                            average_student_all_staff_ratio=average_student_all_staff_ratio,
+                                                            average_additional_staff_degree=average_additional_staff_degree,
+                                                            school_type_by_age=school_type_by_age,
+                                                            max_contacts=max_contacts)
 
         # Change types
         for key, person in population.items():
             for layerkey in population[key]['contacts'].keys():
                 population[key]['contacts'][layerkey] = list(population[key]['contacts'][layerkey])
 
-        school_mixing_types = [self.schools_in_groups[ns]['school_mixing_type'] for ns in range(len(self.schools_in_groups))]
+        school_mixing_types = [schools_in_groups[ns]['school_mixing_type'] for ns in range(len(schools_in_groups))]
 
         # temporarily store some information
         self.homes_by_uids = homes_by_uids
         self.workplace_uid_lists = workplace_uid_lists
         self.student_uid_lists = student_uid_lists
         self.teacher_uid_lists = teacher_uid_lists
         self.non_teaching_staff_uid_lists = non_teaching_staff_uid_lists
         self.school_types = school_types
         self.school_mixing_types = school_mixing_types
+        self.schools_in_groups = schools_in_groups
         if self.ltcf_pars.with_facilities:
             self.facilities_by_uid_lists = facilities_by_uid_lists
             self.facilities_staff_uid_lists = facilities_staff_uid_lists
 
-            sum_ltcf_res = sum([len(f) for f in self.facilities_by_uid_lists])
-            if sum_ltcf_res == 0:
-                log.warning(f"Heads up: Population size and long term care facility use rates were too low, no facilities were created for this population. If you wish to include people living in this type of layer, consider using a larger population size or checking your data on long term care facility use rates. Changing pop.with_facilities to False.")
-                self.layers.remove('LTCF')
-                self.ltcf_pars.with_facilities = False
-
         self.set_layer_classes()
         self.clean_up_layer_info()
 
         return population
 
     def set_layer_classes(self):
         """Add layer classes."""
@@ -1085,22 +1061,25 @@
         Returns:
             dict: Dictionary of the count of contacts in the layer for the
             different people types in the layer. See
             sp.contact_networks.get_contact_counts_by_layer() for method details.
         """
         return spcnx.get_contact_counts_by_layer(self.popdict, layer, **kwargs)
 
-    def to_people(self):
-        ''' Convert to the alternative People representation of a population '''
-        ppl = spp.make_people(popdict=self.popdict, rand_seed=self.rand_seed)  # Create the corresponding population
-        return ppl
-
     def plot_people(self, *args, **kwargs):
         """Placeholder example of plotting the people in a population."""
-        ppl = self.to_people()
+        import covasim as cv  # Optional import
+
+        pars = dict(
+            pop_size   = self.n,
+            pop_type   = 'synthpops',
+            beta_layer = {k: 1 for k in 'hscwl'},
+        )
+        sim = cv.Sim(pars, popfile=self.popdict)
+        ppl = cv.make_people(sim)  # Create the corresponding population
         fig = ppl.plot(*args, **kwargs)
         return fig
 
     def plot_contacts(self, *args, **kwargs):
         """Plot matrices of the contacts for a given layer or layers."""
         fig = sppl.plot_contacts(self.popdict, *args, **kwargs)
         return fig
@@ -1151,14 +1130,28 @@
             pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
             pop = sp.Pop(**pars)
             fig, ax = pop.plot_household_sizes()
         """
         fig, ax = sppl.plot_household_sizes(self, **kwargs)
         return fig, ax
 
+    # # TBC: placeholder for now
+    # def plot_household_head_ages(self, **kwargs):
+    #     """
+    #     Plot a comparison of the expected and generated head of household ages.
+
+    #     **Examples**::
+
+    #         pars = {'n': 10e3, 'location':'seattle_metro', 'state_location':'Washington', 'country_location':'usa'}
+    #         pop = sp.Pop(**pars)
+    #         fig, ax = pop.plot_household_head_ages()
+    #     """
+    #     fig, ax = sppl.plot_household_head_ages(self, **kwargs)
+    #     return fig, ax
+
     def plot_household_head_ages_by_size(self, **kwargs):
         """
         Plot a comparison of the expected and generated age distribution of the
         household heads by the household size.
 
         **Examples**::
```

### Comparing `synthpops-1.10.5/synthpops/sampling.py` & `synthpops-1.8.0/synthpops/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     expect_quin = truedist.ppf(quintiles)
 
     # If null hypothesis is rejected, print a warning or error
     if not null:
         msg = f''''
 Variable{label} with n={n_samples} samples is out of range using the distribution:
     {dist}({args}) →
-    p={pvalue} < α={alpha}
+    p={pvalue} < α={alpha}hehe
 Expected quintiles are: {expect_quin}
 Observed quintiles are: {obvs_quin}
 Observed median is in quantile: {quantile}'''
         if die:
             raise ValueError(msg)
         elif verbose:
             warnings.warn(msg)
```

### Comparing `synthpops-1.10.5/synthpops/schools.py` & `synthpops-1.8.0/synthpops/schools.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import logging
 
 from . import data_distributions as spdata
 from . import defaults
 
 from . import base as spb
 from . import sampling as spsamp
-from . import contact_networks as spcnx
 from .config import logger as log
 
 
 __all__ = ['get_school_type_labels', 'count_enrollment_by_school_type',
            'get_generated_school_size_distributions', 'count_enrollment_by_age',
            'get_enrollment_rates_by_age',
            'School',
@@ -104,59 +103,29 @@
         """
         return np.concatenate((self['student_uids'], self['teacher_uids'], self['non_teaching_staff_uids']))
 
     def member_ages(self, age_by_uid):
         """
         Return ages of all school members: students, teachers, and non teaching staff.
 
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
         Returns:
             np.ndarray: school member ages
         """
-        return np.concatenate((self.student_ages(age_by_uid),
-                               self.teacher_ages(age_by_uid),
-                               self.non_teaching_staff_ages(age_by_uid)))
+        return np.concatenate((self.member_ages(age_by_uid, self['student_uids']),
+                               self.member_ages(age_by_uid, self['teacher_uids']),
+                               self.member_ages(age_by_uid, self['non_teaching_staff_uids'])))
 
     def student_ages(self, age_by_uid):
-        """
-        Return student ages in the school.
-
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
-        Returns:
-            np.ndarray : student ages in school
-        """
-        return super().member_ages(age_by_uid, self['student_uids'])
+        return self.member_ages(age_by_uid, self['student_uids'])
 
     def teacher_ages(self, age_by_uid):
-        """
-        Return teacher ages in the school.
-
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
-        Returns:
-            np.ndarray : teacher ages in school
-        """
-        return super().member_ages(age_by_uid, self['teacher_uids'])
+        return self.member_ages(age_by_uid, self['teacher_uids'])
 
     def non_teaching_staff_ages(self, age_by_uid):
-        """
-        Return non-teaching staff ages in the school.
-
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
-        Returns:
-            np.ndarray : non-teaching staff ages in school
-        """
-        return super().member_ages(age_by_uid, self['non_teaching_staff_uids'])
+        return self.member_ages(age_by_uid, self['non_teaching_staff_uids'])
 
     def __len__(self):
         """Return the length as the number of members in the school."""
         return len(self.member_uids)
 
     def get_classroom(self, clid):
         """
@@ -233,46 +202,25 @@
         """
         return np.concatenate((self['student_uids'], self['teacher_uids']))
 
     def member_ages(self, age_by_uid):
         """
         Return ages of all classroom members: students and teachers.
 
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
         Returns:
             np.ndarray : classroom member ages
         """
-        return np.concatenate((self.student_ages(age_by_uid),
-                               self.teacher_ages(age_by_uid)))
+        return np.concatenate((self.member_ages(age_by_uid, self['student_uids']),
+                               self.member_ages(age_by_uid, self['teacher_uids'])))
 
     def student_ages(self, age_by_uid):
-        """
-        Return student ages in the classroom.
-
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
-        Returns:
-            np.ndarray : student ages in classroom
-        """
-        return super().member_ages(age_by_uid, self['student_uids'])
+        return self.member_ages(age_by_uid, self['student_uids'])
 
     def teacher_ages(self, age_by_uid):
-        """
-        Return teacher ages in the classroom.
-
-        Args:
-            age_by_uid (np.ndarray) : mapping of age to uid
-
-        Returns:
-            np.ndarray : teacher ages in classroom
-        """
-        return super().member_ages(age_by_uid, self['teacher_uids'])
+        return self.member_ages(age_by_uid, self['teacher_uids'])
 
     def __len__(self):
         """Return the length as the number of members in the classroom."""
         return len(self.member_uids)
 
 
 def get_school(pop, scid):
@@ -586,71 +534,36 @@
         potential_student_ages = []
         for a in school_type_age_range:
             potential_student_ages.extend([a] * ages_in_school_count[a])
 
         if size >= len(potential_student_ages):
             size = len(potential_student_ages)
             school_age_count = {a: ages_in_school_count[a] for a in school_type_age_range}
-            other_schools = [ns for ns in range(len(student_uid_lists)) if school_types[ns] == school_type]
-            log.debug(f"other schools to merge with {other_schools} {school_type} {size} {school_size_brackets[0][0]}")
-
-            # school is too small, try to merge it without another school of the same type
-            if (size < school_size_brackets[0][0]) & (len(other_schools) > 0):
-                log.debug(f'School size ({size + 1}) smaller than minimum school size {school_size_brackets[0][0]}. Will try now to merge with another school of the same type already made.')
-
-                # another random school of the same type
-                rns = other_schools[spsamp.fast_choice(np.ones(len(other_schools)))]
-
-                for n, a in enumerate(school_type_age_range):
-                    count = len(uids_in_school_by_age[a])
-                    school_uids_in_age = uids_in_school_by_age[a]
-                    new_student_ages.extend([a for i in range(count)])
-                    new_student_uids.extend(school_uids_in_age)
-                    ages_in_school_count[a] -= count
-
-                # add to a previously generated school, add their ages and their uids, school type was already determined
-                student_age_lists[rns].extend(new_student_ages)
-                student_uid_lists[rns].extend(new_student_uids)
-
-            else:
-                log.debug(f'School size ({size + 1}) smaller than minimum school size {school_size_brackets[0][0]} but there are no other schools of the same type to merge with, so creating this one with however many students are available.')
-                for n, a in enumerate(school_type_age_range):
-                    count = len(uids_in_school_by_age[a])
-                    school_uids_in_age = uids_in_school_by_age[a]
-                    new_student_ages.extend([a for i in range(count)])
-                    new_student_uids.extend(school_uids_in_age)
-                    ages_in_school_count[a] -= count
-
-                # add new school to lists although smaller than expected from school size distribution data
-                student_age_lists.append(new_student_ages)
-                student_uid_lists.append(new_student_uids)
-                school_types.append(school_type)
 
         else:
             chosen = np.random.choice(potential_student_ages, size=size, replace=False)
             school_age_count = Counter(chosen)
 
-            for n, a in enumerate(school_type_age_range):
-                count = school_age_count[a]
-                school_uids_in_age = uids_in_school_by_age[a][:count]
-                uids_in_school_by_age[a] = uids_in_school_by_age[a][count:]
-                new_student_ages += [a for i in range(count)]
-                new_student_uids += school_uids_in_age
-                ages_in_school_count[a] -= count
-
-            # have created a new school and now adding the school with students to the lists for each data type (age, uid, and school type)
-            student_age_lists.append(new_student_ages)
-            student_uid_lists.append(new_student_uids)
-            school_types.append(school_type)
+        for n, a in enumerate(school_type_age_range):
+            count = school_age_count[a]
+
+            school_uids_in_age = uids_in_school_by_age[a][:count]  # assign students to the school
+            uids_in_school_by_age[a] = uids_in_school_by_age[a][count:]
+            new_student_ages += [a for i in range(count)]
+            new_student_uids += school_uids_in_age
+            ages_in_school_count[a] -= count
 
-        # having placed the students in the appropriate school, either a new one or an old one when sizes are too small, remove these students from those available to place in future schools
         for uid in new_student_uids:
             uids_in_school.pop(uid, None)
         ages_in_school_distr = spb.norm_dic(ages_in_school_count)
 
+        student_age_lists.append(new_student_ages)
+        student_uid_lists.append(new_student_uids)
+        school_types.append(school_type)
+
     return student_age_lists, student_uid_lists, school_types
 
 
 # adding edges to the popdict, either from an edgelist or groups (groups are better when you have fully connected graphs - no need to enumerate for n*(n-1)/2 edges!)
 def add_contacts_from_edgelist(popdict, edgelist, setting):
     """
     Add contacts to popdict from edges in an edgelist. Note that this simply
@@ -766,30 +679,31 @@
 
     # create a graph of contacts in the school
     G = nx.Graph()
 
     for a in uids_in_school_by_age:
 
         # for Erdos Renyi graph of N nodes and average degree k, p is essentially the density of all possible edges --> p = # edges / # all possible edges. With average degree k, # of edges is roughly N * k / 2 and # of all possible edges is N * (N-1) / 2, which leads us to k = (N - 1) * p or, in Stirling's Approx. k = N * p, that is p = k / N
-        Ga = spcnx.random_graph_model(uids_in_school_by_age[a], average_class_size)
+        p = float(average_class_size) / len(uids_in_school_by_age[a])  # density of contacts within each grade
+
+        Ga = nx.erdos_renyi_graph(len(uids_in_school_by_age[a]), p)  # creates a well mixed graph across the grade/age
         for e in Ga.edges():
             i, j = e
 
             # add each edge to the overall school graph
             G.add_edge(uids_in_school_by_age[a][i], uids_in_school_by_age[a][j])
 
-    # make sure all students are in the graph by adding those without an edge yet
-    missing_uids = set(student_uids) - set(G.nodes())
-    G.add_nodes_from(missing_uids)
-
-    # flag was turned on to indicate that the average degree is too low. How can we add more edges? do the following: create a second random graph across the entire school. Loop over everyone and grab edges as necessary. Loop again to remove edges if it's too many.
+    # flag was turned on to indicate that the average degree is too low. How can we add more edges? Maybe do the following: create a second random graph across the entire school. Loop over everyone and grab edges as necessary? Loop again to remove edges if it's too many.
     if age_groups_smaller_than_degree:
 
+        # add some extra edges
         G = add_random_contacts_from_graph(G, average_class_size)
 
+    # log.debug(f"clustering within age/grade clustered school: {nx.transitivity(G)}")
+
     # rewire some edges between people within the same grade/age to now being edges across grades/ages
     E = list(G.edges())
     np.random.shuffle(E)
 
     nE = int(len(E) / 2.)  # we'll loop over edges in pairs so only need to loop over half the length
     missed_rewiring = 0
 
@@ -819,15 +733,15 @@
                 missed_rewiring += 1
                 continue
 
             G.remove_edges_from([ei, ej])
             G.add_edges_from([new_ei, new_ej])
 
     # calculate school age mixing and print some debugging statements
-    if logging.getLevelName(log.level) == 'DEBUG': # pragma: no cover
+    if logging.getLevelName(log.level) == 'DEBUG':
         print(f"clustering within age/grade clustered school: {nx.transitivity(G)}")
         print(f"missed rewiring {missed_rewiring} edge pairs out of {nE} possible pairs.")
         ecount = np.zeros((len(age_keys), len(age_keys)))
         for e in G.edges():
             i, j = e
 
             age_i = age_by_uid[i]
@@ -845,16 +759,14 @@
 
 def generate_clustered_classes_by_grade_in_school(student_uids, student_ages, age_by_uid, grade_age_mapping, age_grade_mapping, average_class_size=20, return_edges=False):
     """
     Generate edges for contacts mostly within the same age/grade. Edges are
     randomly distributed so that clustering is roughly average_class_size/size
     of the grade.
 
-    The last classroom created may be much smaller than the average_class_size.
-
     Args:
         student_uids (list)        : list of uids of students in the school
         student_ages (list)        : list of the ages of the students in the school
         age_by_uid (dict)          : dict mapping uid to age
         grade_age_mapping (dict)   : dict mapping grade to an age
         age_grade_mapping (dict)   : dict mapping age to a grade
         average_class_size (float) : average class size
@@ -887,60 +799,54 @@
         nodes = sc.dcp(uids_in_school_by_age[a])
         np.random.shuffle(nodes)
 
         while len(nodes) > 0:
             cluster_size = np.random.poisson(average_class_size)
 
             if cluster_size > len(nodes):
-                # gather the last group of nodes into a pool to choose from afterwards
                 nodes_left += list(nodes)
                 break
 
             group = nodes[:cluster_size]
             if cluster_size > 0:
                 groups.append(group)
             nodes = nodes[cluster_size:]
 
-    # shuffle the students left over to place into classrooms
     np.random.shuffle(nodes_left)
 
+    if len(groups) == 0:
+        groups.append(nodes_left)
+        nodes_left = []
+
     while len(nodes_left) > 0:
         cluster_size = np.random.poisson(average_class_size)
 
         if cluster_size > len(nodes_left):
-            cluster_size = len(nodes_left)
             break
 
         group = nodes_left[:cluster_size]
         if cluster_size > 0:
             groups.append(group)
         nodes_left = nodes_left[cluster_size:]
 
-    # with some school sizes and parameter values you may not have made any classrooms yet
-    if len(groups) == 0:
-        groups.append(nodes_left[:cluster_size])
-        nodes_left = nodes_left[cluster_size:]
-
-    else:
-        for i in nodes_left:
-            ng = spsamp.fast_choice(np.ones(len(groups)))  # choose one of the other classes to add to
-            groups[ng].append(i)
+    for i in nodes_left:
+        ng = np.random.choice(a=np.arange(len(groups)))  # choose one of the other classes to add to
+        groups[ng].append(i)
 
-    if return_edges: # pragma: no cover
+    if return_edges:
         for ng in range(len(groups)):
             group = groups[ng]
             Gn = nx.complete_graph(len(group))
             for e in Gn.edges():
                 i, j = e
                 node_i = group[i]
                 node_j = group[j]
                 G.add_edge(node_i, node_j)
 
-    if logging.getLevelName(log.level) == 'DEBUG': # pragma: no cover
-
+    if logging.getLevelName(log.level) == 'DEBUG':
         if return_edges:
             ecount = np.zeros((len(age_keys), len(age_keys)))
             for e in G.edges():
                 i, j = e
 
                 age_i = age_by_uid[i]
                 index_i = age_keys_indices[age_i]
@@ -974,22 +880,22 @@
     """
     edges = []
     if average_teacher_teacher_degree > len(teacher_uids):
         eiter = combinations(teacher_uids, 2)
         edges = [e for e in eiter]
 
     else:
-        G = spcnx.random_graph_model(teacher_uids, average_teacher_teacher_degree)
+        p = average_teacher_teacher_degree / len(teacher_uids)
+        G = nx.erdos_renyi_graph(len(teacher_uids), p)
         for e in G.edges():
             i, j = e
             teacher_i = teacher_uids[i]
             teacher_j = teacher_uids[j]
             e = (teacher_i, teacher_j)
             edges.append(e)
-
     return edges
 
 
 def generate_edges_for_teachers_in_random_classes(student_uids, student_ages, teacher_uids, age_by_uid, average_student_teacher_ratio=20, average_teacher_teacher_degree=4):
     """
     Generate edges for teachers, including to both students and other teachers
     at the same school. Well mixed contacts within the same age/grade, some
@@ -1079,32 +985,34 @@
     for t in teachers_assigned:
         log.debug(f"teacher {t}, age: {age_by_uid[t]}, has {G.degree(t)} contacts with students")
 
     # not returning student-student contacts
     return edges
 
 
-def generate_edges_for_teachers_in_clustered_classes(groups, teacher_uids, average_teacher_teacher_degree=4, return_edges=False):
+def generate_edges_for_teachers_in_clustered_classes(groups, teacher_uids, average_student_teacher_ratio=20, average_teacher_teacher_degree=4, return_edges=False): 
     """
     Generate edges for teachers, including to both students and other teachers
     at the same school. Students and teachers are clustered into disjoint
     classes.
 
     Args:
         groups (list)                          : list of lists of students, clustered into groups mostly by grade
         teacher_uids (list)                    : list of teachers in the school
+        average_student_teacher_ratio (float)  : average number of students per teacher
         average_teacher_teacher_degree (float) : average number of contacts with other teachers
         return_edges (bool)                    : If True, return edges, else return two groups of contacts - students and teachers for each class
 
     Return:
         List of edges connected to teachers.
 
     """
     edges = []
     teacher_groups = []
+
     np.random.shuffle(groups)  # shuffle the clustered groups of students / classes so that the classes aren't ordered from youngest to oldest
 
     available_teachers = sc.dcp(teacher_uids)
 
     # have exactly as many teachers as needed
     if len(groups) == len(available_teachers):
         for ng, t in enumerate(available_teachers):
@@ -1166,21 +1074,25 @@
 
     Args:
         all_school_uids (list)   : list of uids of individuals in the school
         average_class_size (int) : average class size or number of contacts in school
 
     Returns:
         List of edges between individuals in school.
+
     """
     edges = []
-    G = spcnx.random_graph_model(all_school_uids, average_class_size)  # undirected graph
-    for u, uid in enumerate(all_school_uids):
-        es = [(uid, all_school_uids[v]) for v in G.neighbors(u)]
-        edges.extend(es)
-
+    p = average_class_size / len(all_school_uids)
+    G = nx.erdos_renyi_graph(len(all_school_uids), p)  # replace with nx's fast ER implementation
+    for n, e in enumerate(G.edges()):
+        i, j = e
+        node_i = all_school_uids[i]
+        node_j = all_school_uids[j]
+        e = (node_i, node_j)
+        edges.append(e)
     return edges
 
 
 def add_school_edges(popdict, student_uids, student_ages, teacher_uids, non_teaching_staff_uids, age_by_uid, grade_age_mapping, age_grade_mapping, average_class_size=20, inter_grade_mixing=0.1, average_student_teacher_ratio=20, average_teacher_teacher_degree=3, average_additional_staff_degree=20, school_mixing_type='random'):
     """
     Generate edges for teachers, including to both students and other teachers
     at the same school. When school_mixing_type is 'age_clustered' then
@@ -1209,15 +1121,14 @@
         Updated popdict with edges generated in schools.
 
     Notes:
         average_teacher_teacher_degree will not be used in school_mixing_type == 'random' scenario.
     """
     # completely random contacts across the school, no guarantee of contact with a teacher, much like universities
     available_school_mixing_types = ['random', 'age_clustered', 'age_and_class_clustered']
-
     if school_mixing_type not in available_school_mixing_types:
         print(f"school_mixing_type: {school_mixing_type} 'does not exist. Please change this to one of: {available_school_mixing_types}")
 
     if school_mixing_type == 'random':
         school_uids = []
         school_uids.extend(student_uids)
         school_uids.extend(teacher_uids)
@@ -1225,44 +1136,42 @@
         add_contacts_from_edgelist(popdict, edges, 'S')
         student_groups = [student_uids]
         teacher_groups = [teacher_uids]
 
     # random contacts across a grade in the school, most edges will across the same age group, much like middle schools or high schools, the inter_grade_mixing parameter is a tuning parameter, students get at least one teacher as a contact
     elif school_mixing_type == 'age_clustered':
         edges = generate_random_classes_by_grade_in_school(student_uids, student_ages, age_by_uid, grade_age_mapping, age_grade_mapping, average_class_size, inter_grade_mixing)
-
         teacher_edges = generate_edges_for_teachers_in_random_classes(student_uids, student_ages, teacher_uids, age_by_uid, average_student_teacher_ratio, average_teacher_teacher_degree)
         edges += teacher_edges
-
         add_contacts_from_edgelist(popdict, edges, 'S')
         student_groups = [student_uids]
         teacher_groups = [teacher_uids]
 
     # completely clustered into classes by age, one teacher per class at least
     elif school_mixing_type == 'age_and_class_clustered':
 
-        student_groups = generate_clustered_classes_by_grade_in_school(student_uids, student_ages, age_by_uid, grade_age_mapping, age_grade_mapping, average_class_size=average_class_size, return_edges=False)
-        student_groups_2 = sc.dcp(student_groups)
-        student_groups, teacher_groups = generate_edges_for_teachers_in_clustered_classes(student_groups, teacher_uids, average_teacher_teacher_degree=average_teacher_teacher_degree)
-
-        sum_diff = sum([len(group) for group in student_groups]) - sum([len(group) for group in student_groups_2])
-        assert sum_diff == 0, f'Check failed. sum of the differences between student groups is not zero. Total school enrollment changed between the step of creating student groups and assigning teachers to each group. sum is {sum_diff}'
+        student_groups = generate_clustered_classes_by_grade_in_school(student_uids, student_ages, age_by_uid, grade_age_mapping, age_grade_mapping, average_class_size, return_edges=False)
+        student_groups, teacher_groups = generate_edges_for_teachers_in_clustered_classes(student_groups, teacher_uids, average_student_teacher_ratio, average_teacher_teacher_degree)
 
+        n_expected_edges = 0
+        n_expected_edges_list = []
         for ng in range(len(student_groups)):
             student_group = student_groups[ng]
             teacher_group = teacher_groups[ng]
             group = student_group
             group += teacher_group
-
+            n_expected_edges += len(group) * (len(group) - 1) / 2
+            n_expected_edges_list.append(len(group) * (len(group) - 1) / 2)
             add_contacts_from_group(popdict, group, 'S')
 
-        log.debug(f"average_class_size, {average_class_size}, 'class_group sizes', {[len(group) for group in student_groups]}")
-
         # additional edges between teachers in different classes - makes distinct clusters connected - this may add edges again between teachers in the same class
         teacher_edges = generate_edges_between_teachers(teacher_uids, average_teacher_teacher_degree)
+        n_expected_edges += len(teacher_edges)
+        # log.debug(f"n_expected_edges_list: {n_expected_edges_list}")
+
         add_contacts_from_edgelist(popdict, teacher_edges, 'S')
 
     all_school_uids = []
     all_school_uids.extend(student_uids)
     all_school_uids.extend(teacher_uids)
     additional_staff_edges = generate_random_contacts_for_additional_school_members(all_school_uids, non_teaching_staff_uids, average_additional_staff_degree)
     add_contacts_from_edgelist(popdict, additional_staff_edges, 'S')
@@ -1274,14 +1183,15 @@
     """
     Return probabilities of school type for each age. For now assuming no
     overlapping of grades between school types.
 
     Return:
         A dictionary of default probabilities for the school type likely for
         each age.
+
     """
     school_types_distr_by_age = {}
     for a in range(101):
         school_types_distr_by_age[a] = dict.fromkeys(list(school_type_age_ranges.keys()), 0.)
 
     for k in school_type_age_ranges.keys():
         for a in school_type_age_ranges[k]:
@@ -1458,18 +1368,18 @@
 
     else:
         n_all_staff_list = [max(1, int(i/average_student_all_staff_ratio)) for i in n_students_list]  # need at least one staff member
     n_non_teaching_staff_list = [n_all_staff_list[i] - n_teachers_list[i] for i in range(len(n_students_list))]
 
     min_n_non_teaching_staff = min(n_non_teaching_staff_list)
 
-    # log.debug(f"list of number of students per school: {n_students_list}")
-    # log.debug(f"list of number of teachers per school: {n_teachers_list}")
-    # log.debug(f"list of number of all staff expected per school: {n_all_staff_list}")
-    # log.debug(f"list of number of non teaching staff expected per school: {n_non_teaching_staff_list}")
+    log.debug(f"list of number of students per school: {n_students_list}")
+    log.debug(f"list of number of teachers per school: {n_teachers_list}")
+    log.debug(f"list of number of all staff expected per school: {n_all_staff_list}")
+    log.debug(f"list of number of non teaching staff expected per school: {n_non_teaching_staff_list}")
     if min_n_non_teaching_staff <= 0:
         errormsg = f"At least one school expects only 1 non teaching staff member. Either check the average_student_teacher_ratio ({average_student_teacher_ratio}) and the average_student_all_staff_ratio ({average_student_all_staff_ratio}) if you do not expect this to be the case, or some of the generated schools may have too few staff members."
         log.debug(errormsg)
 
     n_non_teaching_staff_list = [i if i > 0 else 1 for i in n_non_teaching_staff_list]  # force one extra staff member beyond teachers
 
     non_teaching_staff_uid_lists = []
@@ -1489,38 +1399,38 @@
             non_teaching_staff_uids_in_this_school.append(uid)
 
         non_teaching_staff_uid_lists.append(non_teaching_staff_uids_in_this_school)
 
     return non_teaching_staff_uid_lists, potential_worker_uids, potential_worker_uids_by_age, workers_by_age_to_assign_count
 
 
-def add_random_contacts_from_graph(G, average_degree):
+def add_random_contacts_from_graph(G, expected_average_degree):
     """
     Add additional edges at random to achieve the expected or desired average
     degree.
 
     Args:
-        G (networkx Graph)   : networkx Graph object
-        average_degree (int) : expected or desired average degree
+        G (networkx Graph)            : networkx Graph object
+        expected_average_degree (int) : expected or desired average degree
 
     Returns:
         Updated networkx Graph object with additional edges added at random.
 
     """
     nodes = G.nodes()
 
     ordered_node_ids = {node: node_id for node_id, node in enumerate(nodes)}
     ids_to_ordered_nodes = {node_id: node for node_id, node in enumerate(nodes)}
 
     if len(nodes) == 0:
         return G
 
-    p = average_degree / len(nodes)
+    p = expected_average_degree / len(nodes)
 
-    G2 = spcnx.random_graph_model(nodes, average_degree)
+    G2 = nx.erdos_renyi_graph(len(nodes), p)  # will return a graph with nodes relabeled from 0 through len(nodes)-1
 
     for node in nodes:
         ordered_node_id = ordered_node_ids[node]
 
         extra_neighbors = list(G2.neighbors(ordered_node_id))
         extra_edges_needed = len(extra_neighbors) - G.degree(node)
 
@@ -1727,15 +1637,15 @@
     Args:
         enrollment_count_by_age (dict) : dictionary of the count of enrolled students
         age_count (dict)               : dictionary of the age count
 
     Returns:
         dict: Dictionary of the enrollment rates by age.
     """
-    return {a: enrollment_count_by_age[a] / age_count[a] if age_count[a] > 0 else 0 for a in sorted(age_count.keys())}
+    return {a: enrollment_count_by_age[a] / age_count[a] for a in sorted(age_count.keys())}
 
 
 def count_enrollment_by_school_type(popdict, **kwargs):
     """
     Get enrollment sizes by school types in popdict.
 
     Args:
```

### Comparing `synthpops-1.10.5/synthpops/workplaces.py` & `synthpops-1.8.0/synthpops/workplaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         employment_rates (dict)                 : A dictionary of employment rates by age.
         potential_worker_ages_left_count (dict) : A dictionary of the count of workers to assign by age.
         uids_by_age (dict)                      : A dictionary mapping age to the list of ids with that age.
 
     Returns:
         A dictionary with a count of workers to assign to a workplace.
     """
-    log.debug('get_workers_by_age_to_assign()')
+
     workers_by_age_to_assign_count = dict.fromkeys(np.arange(101), 0)
     for a in potential_worker_ages_left_count:
         if a in employment_rates:
             try:
                 c = int(employment_rates[a] * len(uids_by_age[a]))
             except:
                 c = 0
@@ -372,15 +372,15 @@
         popdict (dict) : population dictionary
 
     Returns:
         dict: Dictionary of the count of employed people by age in popdict.
     """
     employment_count_by_age = dict.fromkeys(np.arange(0, defaults.settings.max_age), 0)
     for i, person in popdict.items():
-        if person['ltcf_staff'] or person['sc_teacher'] or person['sc_staff'] or person['wpid']:
+        if person['ltcf_staff'] is not None or person['sc_teacher'] is not None or person['sc_staff'] is not None or person['wpid'] is not None:
             employment_count_by_age[person['age']] += 1
 
     return employment_count_by_age
 
 
 def get_employment_rates_by_age(employment_count_by_age, age_count):
     """
@@ -389,15 +389,15 @@
     Args:
         employment_count_by_age (dict) : dictionary of the count of employed people
         age_count (dict)               : dictionary of the age count
 
     Returns:
         dict: Dictionary of the employment rates by age.
     """
-    return {a: employment_count_by_age[a] / age_count[a] if age_count[a] > 0 else 0 for a in sorted(age_count.keys())}
+    return {a: employment_count_by_age[a] / age_count[a] for a in sorted(age_count.keys())}
 
 
 def get_workplace_sizes(popdict):
     """
     Get workplace sizes of regular workplaces in popdict. This only includes
     workplaces that are not long term care facilities (LTCF) or schools (S).
```

### Comparing `synthpops-1.10.5/synthpops_process_raw_data/data_distributions_legacy.py` & `synthpops-1.8.0/synthpops_process_raw_data/data_distributions_legacy.py`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops_process_raw_data/migrate_legacy_data.py` & `synthpops-1.8.0/synthpops_process_raw_data/migrate_legacy_data.py`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/synthpops_process_raw_data/process_census.py` & `synthpops-1.8.0/synthpops_process_raw_data/process_census.py`

 * *Files identical despite different names*

### Comparing `synthpops-1.10.5/tests/test_data.py` & `synthpops-1.8.0/synthpops_process_raw_data/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 
 import numpy as np
 import pandas as pd
 import sciris as sc
 import synthpops as sp
 import os
 import unittest
-import pathlib
 
-datadir = pathlib.Path(__file__).parent.parent.joinpath("synthpops/data").absolute()
+sp.settings.datadir = sc.thisdir(__file__, 'unittests')
+
+# for Testconvert_df_to_json_array()
+pars = sc.objdict(
+            location_name = 'usa-Washington',  # name of the location
+            property_name = 'population_age_distributions',  # name of the property to compare to
+            filepath      = os.path.join(sp.settings.datadir,
+                                         'Washington_age_bracket_distr_16.dat'),  # path to the file to convert to array
+            cols_ind      = [],  # list of column indices to include in array in conversion
+            int_cols_ind  = [],  # list of column induces to convert to ints
+            )
 
 
 class TestLocation(unittest.TestCase):
     """
     These tests need to be run from the root synthpops/tests folder, because some of the tests involve relative
     filepath assumptions based on that.
     """
 
-    @classmethod
-    def setUpClass(cls) -> None:
-        sp.settings.datadir = sc.thisdir(__file__, 'testdata')
-
-    @classmethod
-    def tearDownClass(cls) -> None:
-        sp.settings.datadir = datadir
-
     def minimal_test_str(self):
         test_str = """{
           "location_name": "test_location",
           "data_provenance_notices": ["notice1","notice2"],
           "reference_links": ["reference1","reference2"],
           "citations": ["citation1","citation2"],
           "parent": {},
@@ -187,15 +188,15 @@
           ]
         }"""
         return test_str
 
     def minimal_location_with_parent_filepath_test_str(self):
         test_str = """{
           "location_name": "test_location_child",
-          "parent": "test_location_A.json",
+          "parent": "unittests/test_location_A.json",
           "employment_rates_by_age": [
             [19,0.300],
             [20,0.693]
           ],
           "school_size_distribution": [
             0.45,
             0.55
@@ -213,24 +214,24 @@
     def test_load_empty_object_test_str(self):
         """
         Make sure that an empty json object populates all lists as empty.
         Because parts of the code rely on this assumption.
         location_name is a required field so it must be present.
         """
         test_str = """{"location_name": "test_location"}"""
-        location = sp.load_location_from_json_str(test_str, check_constraints=False)
+        location = sp.load_location_from_json_str(test_str)
         self.assertEqual(location.location_name, "test_location",
                          "location_name incorrect")
         for list_property in location.get_list_properties():
             att = getattr(location, list_property)
             self.assertTrue(att is not None and len(att) == 0)
 
     def test_load_minimal_location(self):
         test_str = self.minimal_test_str()
-        location = sp.load_location_from_json_str(test_str, check_constraints=False)
+        location = sp.load_location_from_json_str(test_str)
 
         self.assertEqual(location.location_name, "test_location",
                          "location_name incorrect")
 
         self.assertEqual(len(location.data_provenance_notices), 2,
                          "Array length incorrect")
 
@@ -522,35 +523,34 @@
     def test_load_minimal_location_with_parent(self):
         test_str = self.minimal_location_with_parent_test_str()
         location = sp.load_location_from_json_str(test_str)
         self.check_minimal_location_with_parent(location)
 
     def test_load_minimal_location_with_parent_filepath(self):
         test_str = self.minimal_location_with_parent_filepath_test_str()
-        location = sp.load_location_from_json_str(test_str, check_constraints=False)
+        location = sp.load_location_from_json_str(test_str)
         self.check_minimal_location_with_parent(location)
 
     def test_load_minimal_location_with_parent_filepath_from_filepath(self):
-        child_filepath = "test_location_child.json"
-        location = sp.load_location_from_filepath(child_filepath, check_constraints=False)
+        child_filepath = os.path.join("unittests", "test_location_child.json")
+        location = sp.load_location_from_filepath(child_filepath)
         self.check_minimal_location_with_parent(location)
 
     def check_minimal_location_with_parent(self, location):
         # All but the three specified lists are existing and empty...
         for list_property in location.get_list_properties():
             att = getattr(location, list_property)
             # what fields are we planning to test...
             if str(list_property) in ["employment_rates_by_age",
                                       "population_age_distributions",
                                       "school_size_distribution_by_type",
                                       "school_size_distribution",
                                       "school_size_brackets",
                                       "reference_links",
                                       "citations",
-                                      "notes",
                                       ]:
                 continue
             self.assertTrue(att is not None and len(att) == 0)  # everything else should be empty
 
         self.assertEqual(location.location_name, "test_location_child",
                          "location_name incorrect")
 
@@ -628,29 +628,21 @@
         self.assertEqual(len(location.school_size_distribution), 2,
                          "Array length incorrect")
         self.assertEqual(location.school_size_distribution[0], 0.45,
                          "Array entry incorrect")
         self.assertEqual(location.school_size_distribution[1], 0.55,
                          "Array entry  incorrect")
 
-    @unittest.skip("constraint check not working properly, need investigation.")
-    def test_constraint_check(self):
-        location = sp.load_location_from_filepath("test_location_grand_child.json", check_constraints=True)
-        self.assertEqual(location['school_size_distribution'], [0.5, 0.5])
-
-        with self.assertWarns(Warning) as wn:
-            sp.load_location_from_filepath("test_location_bad.json", check_constraints=True)
-            self.assertTrue('has some negative values' in str(wn), 'Check failed: expect to get negative distribution check messages')
-
 
 class TestChecks(unittest.TestCase):
     """
     Test checks can be run on probability distributions. Checks made: sum of
     probability distributions is close to 1, distribution has no negative values.
     """
+
     def test_check_probability_distribution_sums(self, location_name='usa-Washington-seattle_metro', property_list=None, tolerance=1e-2):
         """
         Run all checks for fields in property_list representing probability distributions. Each
         should have a sum that equals 1 within the tolerance level.
 
         Args:
             location_name(str)   : name of the location json to test
@@ -707,24 +699,14 @@
                 print(f'{property_name} check passed.')
 
 
 class Testconvert_df_to_json_array(unittest.TestCase):
     """
     Test different aspects of the sp.data.convert_df_to_json_array() method.
     """
-    pars = sc.objdict(
-        location_name='usa-Washington',  # name of the location
-        property_name='population_age_distributions',  # name of the property to compare to
-        cols_ind=[],  # list of column indices to include in array in conversion
-        int_cols_ind=[],  # list of column induces to convert to ints
-    )
-    @classmethod
-    def setUpClass(cls) -> None:
-        # for Testconvert_df_to_json_array()
-        cls.pars['filepath'] = os.path.join(sc.thisdir(__file__, 'testdata'), 'Washington_age_bracket_distr_16.dat')
 
     def setup_convert_df_to_json_array(self, pars):
         """
         Set up objects to compare.
 
         Args:
             pars (dict): dictionary to get the data array and json array for comparison.
@@ -763,28 +745,28 @@
         """
         Test that the sp.convert_df_to_json_entry() converts the desired data from
         a dataframe to an array of arrays like those that can be uploaded to the
         json data objects synthpops uses.
         """
         sp.logger.info("Testing method to convert pandas dataframe to json arrays.")
 
-        arr, json_array = self.setup_convert_df_to_json_array(self.pars)
+        arr, json_array = self.setup_convert_df_to_json_array(pars)
         assert arr == json_array, "Arrays don't match"
 
         if verbose:
             print(f"The pandas table converted to an array matches the corresponding json array for {pars.property_name} in location: {pars.location_name}")
 
     def test_convert_df_to_json_entry_int_values(self):
         """
         Test that when converting a df to arrays, some of the columns specified are
         made into ints, like when we have columns specifying the age bracket min or
         max values.
         """
         sp.logger.info("Test that specified columns are converted to ints when data from a df is converted to a json array.")
-        test_pars = sc.dcp(self.pars)
+        test_pars = sc.dcp(pars)
         test_pars.int_cols_ind = [0, 1]  # want to convert values from columns 0 and 1 to integers
 
         arr, json_array = self.setup_convert_df_to_json_array(test_pars)
 
         for i in range(len(arr)):
             for j in test_pars.int_cols_ind:
                 assert isinstance(arr[i][j], int), f"Value at ({i},{j}): {arr[i][j]} is not an integer as expected."
```

