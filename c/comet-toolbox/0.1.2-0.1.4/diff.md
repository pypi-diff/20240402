# Comparing `tmp/comet_toolbox-0.1.2.tar.gz` & `tmp/comet_toolbox-0.1.4.tar.gz`

## Comparing `comet_toolbox-0.1.2.tar` & `comet_toolbox-0.1.4.tar`

### file list

```diff
@@ -1,223 +1,225 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/.gitattributes
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/__init__.py
--rwxr-xr-x   0        0        0     3969 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/data.py
--rw-r--r--   0        0        0    24483 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/graph.py
--rwxr-xr-x   0        0        0    61580 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/gui.py
--rwxr-xr-x   0        0        0    44939 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/methods.py
--rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/multiverse.py
--rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/simulation.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/simulation.txt
--rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/single_state.txt
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/img/badge.svg
--rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/img/content.drawio
--rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/img/content.png
--rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/img/gui.png
--rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/src/comet/resources/img/logo.png
--rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_analysis.ipynb
--rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_dfc.ipynb
--rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_graph.ipynb
--rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_multiverse.ipynb
--rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_data/abide_50008.txt
--rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_data/aomic_multi.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_data/simulation.txt
--rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/example_data/xcpd.tsv
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_1.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_10.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_11.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_12.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_13.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_14.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_15.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_16.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_17.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_18.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_19.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_2.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_20.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_21.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_22.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_23.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_24.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_25.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_26.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_27.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_28.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_29.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_3.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_30.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_31.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_32.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_33.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_34.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_35.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_36.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_37.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_38.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_39.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_4.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_40.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_41.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_42.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_43.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_44.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_45.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_46.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_47.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_48.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_49.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_5.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_50.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_51.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_52.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_53.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_54.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_55.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_56.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_57.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_58.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_59.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_6.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_60.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_61.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_62.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_63.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_64.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_65.py
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_66.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_67.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_68.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_69.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_7.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_70.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_71.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_72.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_73.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_74.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_75.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_76.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_77.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_78.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_79.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_8.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_80.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_81.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_82.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_83.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_84.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_85.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_86.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_87.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_88.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_89.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_9.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_90.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_91.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_92.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_93.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_94.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_95.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/universe_96.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/pipelines.csv
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_1.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_10.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_11.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_12.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_13.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_14.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_15.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_16.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_17.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_18.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_19.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_2.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_20.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_21.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_22.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_23.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_24.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_25.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_26.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_27.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_28.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_29.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_3.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_30.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_31.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_32.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_33.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_34.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_35.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_36.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_37.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_38.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_39.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_4.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_40.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_41.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_42.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_43.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_44.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_45.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_46.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_47.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_48.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_49.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_5.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_50.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_51.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_52.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_53.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_54.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_55.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_56.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_57.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_58.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_59.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_6.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_60.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_61.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_62.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_63.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_64.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_65.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_66.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_67.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_68.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_69.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_7.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_70.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_71.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_72.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_73.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_74.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_75.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_76.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_77.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_78.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_79.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_8.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_80.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_81.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_82.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_83.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_84.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_85.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_86.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_87.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_88.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_89.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_9.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_90.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_91.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_92.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_93.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_94.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_95.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/tutorials/multiverse/results/universe_96.pkl
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/LICENSE
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/README.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 comet_toolbox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/.gitattributes
+-rw-r--r--   0        0        0  1662983 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/amir.mat
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/simulation.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/__init__.py
+-rwxr-xr-x   0        0        0     3969 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/data.py
+-rw-r--r--   0        0        0    24483 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/graph.py
+-rw-r--r--   0        0        0    64136 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/gui.py
+-rwxr-xr-x   0        0        0    44939 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/methods.py
+-rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/multiverse.py
+-rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/simulation.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/simulation.txt
+-rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/single_state.txt
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/img/badge.svg
+-rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/img/content.drawio
+-rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/img/content.png
+-rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/img/gui.png
+-rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/src/comet/resources/img/logo.png
+-rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_analysis.ipynb
+-rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_dfc.ipynb
+-rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_graph.ipynb
+-rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_multiverse.ipynb
+-rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_data/abide_50008.txt
+-rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_data/aomic_multi.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_data/simulation.txt
+-rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/example_data/xcpd.tsv
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_1.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_10.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_11.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_12.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_13.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_14.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_15.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_16.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_17.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_18.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_19.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_2.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_20.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_21.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_22.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_23.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_24.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_25.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_26.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_27.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_28.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_29.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_3.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_30.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_31.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_32.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_33.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_34.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_35.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_36.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_37.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_38.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_39.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_4.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_40.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_41.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_42.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_43.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_44.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_45.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_46.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_47.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_48.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_49.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_5.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_50.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_51.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_52.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_53.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_54.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_55.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_56.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_57.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_58.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_59.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_6.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_60.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_61.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_62.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_63.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_64.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_65.py
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_66.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_67.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_68.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_69.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_7.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_70.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_71.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_72.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_73.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_74.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_75.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_76.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_77.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_78.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_79.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_8.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_80.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_81.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_82.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_83.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_84.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_85.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_86.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_87.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_88.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_89.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_9.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_90.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_91.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_92.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_93.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_94.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_95.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/universe_96.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/pipelines.csv
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_1.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_10.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_11.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_12.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_13.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_14.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_15.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_16.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_17.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_18.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_19.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_2.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_20.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_21.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_22.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_23.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_24.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_25.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_26.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_27.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_28.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_29.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_3.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_30.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_31.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_32.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_33.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_34.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_35.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_36.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_37.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_38.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_39.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_4.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_40.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_41.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_42.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_43.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_44.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_45.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_46.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_47.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_48.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_49.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_5.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_50.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_51.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_52.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_53.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_54.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_55.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_56.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_57.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_58.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_59.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_6.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_60.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_61.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_62.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_63.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_64.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_65.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_66.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_67.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_68.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_69.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_7.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_70.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_71.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_72.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_73.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_74.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_75.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_76.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_77.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_78.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_79.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_8.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_80.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_81.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_82.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_83.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_84.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_85.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_86.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_87.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_88.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_89.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_9.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_90.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_91.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_92.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_93.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_94.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_95.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/tutorials/multiverse/results/universe_96.pkl
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/README.md
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 comet_toolbox-0.1.4/PKG-INFO
```

### Comparing `comet_toolbox-0.1.2/src/comet/data.py` & `comet_toolbox-0.1.4/src/comet/data.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/graph.py` & `comet_toolbox-0.1.4/src/comet/graph.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/gui.py` & `comet_toolbox-0.1.4/src/comet/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import sys
+import copy
 import pickle
 import inspect
 import numpy as np
 import pandas as pd
+from typing import Any, Dict
 from scipy.io import loadmat, savemat
+from dataclasses import dataclass, field
 from importlib import resources as pkg_resources
 
-import qdarkstyle
-from PyQt6.QtCore import Qt, QPoint, QThread, pyqtSignal, QObject
-from PyQt6.QtGui import QEnterEvent, QFontMetrics
-from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton, QVBoxLayout, QHBoxLayout, \
-    QSlider, QToolTip, QWidget, QLabel, QFileDialog, QComboBox, QLineEdit, QSizePolicy, \
-    QSpacerItem, QCheckBox, QTabWidget, QMessageBox, QSpinBox, QDoubleSpinBox
-
+# Plotting imports
 from matplotlib.image import imread
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.figure import Figure
 from matplotlib.ticker import FuncFormatter
 import matplotlib.gridspec as gridspec
 
+# Qt imports
+import qdarkstyle
+from PyQt6.QtCore import Qt, QPoint, QThread, pyqtSignal, QObject
+from PyQt6.QtGui import QEnterEvent, QFontMetrics
+from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton, QVBoxLayout, QHBoxLayout, \
+    QSlider, QToolTip, QWidget, QLabel, QFileDialog, QComboBox, QLineEdit, QSizePolicy, \
+    QSpacerItem, QCheckBox, QTabWidget, QMessageBox, QSpinBox, QDoubleSpinBox
+
+# DFC methods
 from . import methods
 import pydfc
 
-# Worker class for dFC calculations, which run in a separate thread
 class Worker(QObject):
+    # Worker class for dFC calculation (runs in a separate thread)
     finished = pyqtSignal()
     error = pyqtSignal(str)
     result = pyqtSignal(object)
 
     def __init__(self, calculationFunc, parameters):
         super().__init__()
         self.calculationFunc = calculationFunc
@@ -39,44 +45,103 @@
             result = self.calculationFunc(self.parameters)
             self.result.emit(result)  # Emit results
         except Exception as e:
             self.error.emit(str(e))  # Emit errors
         finally:
             self.finished.emit()  # Notify completion
 
-# Info button class
 class InfoButton(QPushButton):
+    # Info button class
     def __init__(self, info_text, parent=None):
         super().__init__("i", parent)
         self.info_text = info_text
         self.setStyleSheet("QPushButton { border: 1px solid black;}")
         self.setFixedSize(20, 20)
 
     def enterEvent(self, event: QEnterEvent):
         tooltip_pos = self.mapToGlobal(QPoint(self.width(), 0)) # Tooltip position can be adjusted here
         QToolTip.showText(tooltip_pos, self.info_text)
         super().enterEvent(event)
 
+@dataclass
+class Data:
+    # Data class to hold currently relevant data
+    file_name:    str        = field(default=None)         # data file name
+    file_data:    np.ndarray = field(default=None)         # input time series data
+    roi_names:    np.ndarray = field(default=None)         # input roi data     
+
+    dfc_instance: Any        = field(default=None)         # instance of the dFC class
+    dfc_name:     str        = field(default=None)         # method class name
+    dfc_params:   Dict       = field(default_factory=dict) # input parameters
+    dfc_data:     np.ndarray = field(default=None)         # dfc data
+    dfc_states:   Dict       = field(default_factory=dict) # dfc states
+    dfc_state_tc: np.ndarray = field(default=None)         # dfc state time course
+    dfc_edge_ts:  np.ndarray = field(default=None)         # dfc edge time series
+
+    def clear_dfc_data(self):
+        self.dfc_instance = None
+        self.dfc_name     = None
+        self.dfc_params   = {}
+        self.dfc_data     = None
+        self.dfc_states   = {}
+        self.dfc_state_tc = None
+        self.dfc_edge_ts  = None
+
+class DataStorage:
+    # Database class for storing calculated data
+    def __init__(self):
+        self.storage = {}
+
+    def generate_hash(self, data_obj):
+        # Generate a hash based on method_name, file_name, and sorted params
+        # This hash will be used to check if identical data exists
+        hashable_params = {k: v for k, v in data_obj.dfc_params.items() if not isinstance(v, np.ndarray)}
+        params_tuple = tuple(sorted(hashable_params.items()))
+        return hash((data_obj.file_name, data_obj.dfc_name, params_tuple))
+
+    def add_data(self, data_obj):
+        self.delete_data(data_obj) # Delete existing data for the same method
+
+        data_hash = self.generate_hash(data_obj)
+        if data_hash not in self.storage:
+            self.storage[data_hash] = copy.deepcopy(data_obj) # IMPORTANT: deep copy for a completely new data object
+            return True
+        return False
+    
+    def delete_data(self, data_obj):
+        # Identify and delete existing entries with the same dfc_name as data_obj
+        keys_to_delete = [key for key, value in self.storage.items() if value.dfc_name == data_obj.dfc_name]
+        for key in keys_to_delete:
+            del self.storage[key]
+    
+    def check_for_identical_data(self, data_obj):
+        # Get data and parameters for previously calculated identical data
+        data_hash = self.generate_hash(data_obj)
+        data = self.storage.get(data_hash, None)   
+        return copy.deepcopy(data) # IMPORTANT: deep copy
+    
+    def check_previous_data(self, methodName):
+        # Get data for the last calculation with a given method
+        for data_obj in reversed(list(self.storage.values())):
+            if data_obj.dfc_name == methodName and data_obj.dfc_data is not None:
+                return copy.deepcopy(data_obj) # IMPORTANT: deep copy
+        return None
+
 class App(QMainWindow):
     def __init__(self, init_data=None, init_method=None):
         super().__init__()
         self.title = 'Comet Dynamic Functional Connectivity Toolbox'
-        self.ts_data = None
-        self.roi_data = None
-        self.dfc_data = {}
-        self.state_tc = None
-        self.dfc_states = None
-        self.edge_ts = None
-        self.abortFlag = False
-        self.init_method = init_method
-        self.dfc_data_dict = {}
-        self.selected_class_name = None
+        self.init_flag = True
+
+        self.data = Data()
+        self.data_storage = DataStorage()
+
         self.currentSliderValue = 0
         self.currentTabIndex = 0
-        self.file_name = ""
+
         self.param_names = {
             "self":                 "self", 
             "time_series":          "Time series",
             "windowsize":           "Window size",
             "shape":                "Window shape",
             "std":                  "Window sigma",
             "diagonal":             "Main diagonal",
@@ -115,21 +180,21 @@
             "iterations":            "Iterations",
             "sw_method":            "Sliding window",
             "dhmm_obs_state_ratio": "State ratio",
             "vlim":                 "Color axis limit"
 
         }
         self.reverse_param_names = {v: k for k, v in self.param_names.items()}
-
-        self.initUI()
         
-        self.dfc_data['data'] = init_data
-        self.dfc_data['parameters'] = None # TODO pass parameters
+        self.initUI()
 
-        if self.dfc_data['data'] is not None:
+        if init_data is not None:
+            self.data.dfc_data = init_data
+            self.data.dfc_instance = init_method
+            self.data.file_data = "loaded from script"
             self.init_from_calculated_data()
 
     def initUI(self):
         self.setWindowTitle(self.title)
         mainLayout = QHBoxLayout()
 
         ###############################
@@ -176,33 +241,29 @@
         self.staticCheckBox.stateChanged.connect(self.updateMethodComboBox)
         
         self.methodComboBox = QComboBox()
         self.leftLayout.addWidget(self.methodLabel)
         self.leftLayout.addLayout(checkboxLayout)
         self.leftLayout.addWidget(self.methodComboBox)
 
-        # Retrieve class names and their human-readable names
-        self.class_info = {
-            obj.name: name  # Map human-readable name to class name
-            for name, obj in inspect.getmembers(methods)
-            if inspect.isclass(obj) and obj.__module__ == methods.__name__ and name != "ConnectivityMethod"
-        }
+        # Get all the dFC methods and names
+        self.class_info = self.get_dfc_methods()
 
         # Create a layout for dynamic textboxes
         self.parameterLayout = QVBoxLayout()
 
         # Create a container widget for the parameter layout
         self.parameterContainer = QWidget()  # Use an instance attribute to access it later
         self.parameterContainer.setLayout(self.parameterLayout)
         self.parameterContainer.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Expanding)
 
         # Add the container widget to the left layout directly below the combobox
         self.leftLayout.addWidget(self.parameterContainer)
         
-        # Initial population of the combobox
+        # Initial population of the combobox, this does the entire initialization
         self.updateMethodComboBox()
 
         # Add parameter textbox for time_series
         self.time_series_textbox = QLineEdit()
         self.time_series_textbox.setReadOnly(True) # read only as based on the loaded file
 
         # Add a stretch after the parameter layout container
@@ -323,17 +384,14 @@
         self.backButton.clicked.connect(self.moveBack)
         self.forwardButton.clicked.connect(self.moveForward)
         self.forwardLargeButton.clicked.connect(self.moveForwardLarge)
 
         navButtonLayout.addStretch(1)  # Spacer to the right of the buttons
         rightLayout.addLayout(navButtonLayout)
 
-        # Initialize parameters for the default method (from left layout but has to be done after figure creation)
-        self.onMethodChanged()
-
         # UI elements for dFC time series plotting
         self.rowSelector = QSpinBox()
         self.rowSelector.setMaximum(0)
         self.rowSelector.valueChanged.connect(self.plotTimeSeries)
 
         self.colSelector = QSpinBox()
         self.colSelector.setMaximum(0)
@@ -359,27 +417,36 @@
         self.setCentralWidget(centralWidget)
 
         # Set checkboxes to default values
         self.continuousCheckBox.setChecked(True)
         self.stateBasedCheckBox.setChecked(True)
         self.staticCheckBox.setChecked(True)
 
+    def get_dfc_methods(self):
+        # Retrieve class names and their human-readable names
+        # Keys: human-readable names, Values: class names
+        dfc_methods = {
+            obj.name: name  # Map human-readable name to class name
+            for name, obj in inspect.getmembers(methods)
+            if inspect.isclass(obj) and obj.__module__ == methods.__name__ and name != "ConnectivityMethod"
+        }
+
+        return dfc_methods
+
     def init_from_calculated_data(self):
         # Make sure both the dFC data and the method object are provided
-        assert self.init_method is not None, "Please provide the method object corresponding to your dFC data as the second argument to the GUI."
-
+        assert self.data.dfc_instance is not None, "Please provide the method object corresponding to your dFC data as the second argument to the GUI."
         # Get parameters
-        self.selected_class_name = self.class_info.get(self.init_method.name)
+        #self.data.dfc_name = self.class_info.get(self.init_method.name)
         self.getParameters() # TODO: Something goes wrong here for SW (maybe because of strings in the parameters)
-        self.dfc_data['parameters'] = self.parameters
-        self.dfc_data_dict[self.selected_class_name] = {'data': self.dfc_data['data'], 'parameters': self.dfc_data['parameters']}
+        self.data_storage.add_data(self.data) # Add to data storage
 
         # Set the slider elements
-        total_length = self.dfc_data['data'].shape[2] if len(self.dfc_data['data'].shape) == 3 else 0
-        position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.dfc_data['data'].shape) == 3 else " static "
+        total_length = self.data.dfc_data.shape[2] if len(self.data.dfc_data.shape) == 3 else 0
+        position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.data.dfc_data.shape) == 3 else " static "
         self.positionLabel.setText(position_text)
         self.slider.setValue(self.slider.value())
 
         # Disable the GUI elements
         self.methodComboBox.setEnabled(False)
         self.calculateButton.setEnabled(False)
         self.clearMemoryButton.setEnabled(False)
@@ -396,39 +463,44 @@
 
         self.rowSelector.setValue(1)
         self.plotTimeSeries()
 
     def onMethodChanged(self, methodName=None):
         # Clear old variables and data
         self.clearLayout(self.parameterLayout)
-        self.dfc_data['data'] = None
-        self.dfc_data['parameters'] = None
 
         if methodName == None or methodName == "Use checkboxes to get available methods":
             return
         
         # Get selected connectivity method
-        self.selected_class_name = self.class_info.get(methodName)
-        selected_class = getattr(methods, self.selected_class_name, None)
-        if self.init_method is not None:
-            selected_class = self.init_method
-
-        # If connectivity for this method already exists we load and plot it
-        if self.selected_class_name in self.dfc_data_dict:
-            self.dfc_data = self.dfc_data_dict[self.selected_class_name]
+        self.data.dfc_instance = getattr(methods, self.class_info.get(methodName), None) # the actual class
+        self.data.dfc_name = self.class_info.get(methodName) # class name
+
+        # Create and get new parameter layout
+        #self.data.dfc_data = None
+        self.data.dfc_params = {}
+        self.setup_class_parameters(self.data.dfc_instance)
+        self.parameterLayout.addStretch(1) # Stretch to fill empty space
+        self.getParameters()
+
+        # See if some data has previously been calculated, we change the paramters to this
+        previous_data = self.data_storage.check_previous_data(self.data.dfc_name)
+        if previous_data is not None:
+            self.data = previous_data
+            self.setParameters()
             self.plot_dfc()
             self.updateDistribution()
             self.plotTimeSeries()
             self.slider.show()
-            self.calculatingLabel.setText(f"Loaded {self.selected_class_name} with shape {self.dfc_data['data'].shape}")
-            print(f"Loaded {self.selected_class_name} from memory")
+            self.calculatingLabel.setText(f"Loaded {self.data.dfc_name} with shape {self.data.dfc_data.shape}")
+            print(f"Loaded {self.data.dfc_name} from memory")
 
             # Update the slider
-            total_length = self.dfc_data['data'].shape[2] if len(self.dfc_data['data'].shape) == 3 else 0
-            position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.dfc_data['data'].shape) == 3 else " static "
+            total_length = self.data.dfc_data.shape[2] if len(self.data.dfc_data.shape) == 3 else 0
+            position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.data.dfc_data.shape) == 3 else " static "
             self.positionLabel.setText(position_text)
             self.slider.setValue(self.slider.value())
         
         # If connectivity data does not exist we reset the figure and slider to prepare for a new calculation
         # This also indicates to the user that this data was not yet calculated/saved
         else:
             self.figure.clear()
@@ -440,45 +512,37 @@
             self.timeSeriesCanvas.draw()
 
             position_text = f"no data available"
             self.positionLabel.setText(position_text)
             self.slider.setValue(self.slider.value())
             self.slider.hide()
 
-        # This dynamically creates the parameter labels and input boxes
-        self.setup_class_parameters(selected_class)
-
-        self.parameterLayout.addStretch(1) # Stretch to fill empty space
         self.update() # Update UI
 
-    def setup_class_parameters(self, selected_class):
+    def setup_class_parameters(self, class_instance):
         # Now the parameter labels and boxes are set up    
         labels = []
 
         # Calculate the maximum label width (just a visual thing)
         max_label_width = 0
-        init_signature = inspect.signature(selected_class.__init__)
+        init_signature = inspect.signature(class_instance.__init__)
         font_metrics = QFontMetrics(self.font())
         for param in init_signature.parameters.values():
             label_width = font_metrics.boundingRect(f"{self.param_names[param.name]}:").width()
             max_label_width = max(max_label_width, label_width)
 
         # Special case for 'time_series' parameter as this is created from the loaded file
         # Add label for time_series
         time_series_label = QLabel("Time series:")
         time_series_label.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Preferred)
         time_series_label.setMinimumSize(time_series_label.sizeHint())
         labels.append(time_series_label)
         
-        if self.init_method is None:
-            self.time_series_textbox.setText(self.file_name)
-            self.time_series_textbox.setEnabled(True)
-        else:
-            self.time_series_textbox.setText("from script")
-            self.time_series_textbox.setEnabled(False)
+        self.time_series_textbox.setText(self.data.file_name)
+        self.time_series_textbox.setEnabled(True)
 
         # Create info button for time_series
         time_series_info_text = "2D time series loaded from file. Time has to be the first dimension."
         time_series_info_button = InfoButton(time_series_info_text)
 
         time_series_layout = QHBoxLayout()
         time_series_layout.addWidget(time_series_label)
@@ -486,16 +550,14 @@
         time_series_layout.addWidget(time_series_info_button)
         self.parameterLayout.addLayout(time_series_layout)
 
         # Adjust max width for aesthetics
         max_label_width += 10
         time_series_label.setFixedWidth(max_label_width)
 
-        existing_params = vars(selected_class)
-
         for param in init_signature.parameters.values():
             if param.name not in ['self', 'time_series', 'tril', 'standardize', 'params']:
                 # Create label for parameter
                 param_label = QLabel(f"{self.param_names[param.name]}:")
                 param_label.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Preferred)
                 param_label.setMinimumSize(param_label.sizeHint())
                 param_label.setFixedWidth(max_label_width)
@@ -503,69 +565,56 @@
 
                 # Determine the widget type based on the parameter
                 # Dropdown for boolean parameters
                 if type(param.default) == bool:
                     param_input_widget = QComboBox()
                     param_input_widget.addItems(["True", "False"])
                     
-                    if self.init_method is None:
-                        default_index = param_input_widget.findText(str(param.default))
-                        param_input_widget.setCurrentIndex(default_index)
-                        param_input_widget.setEnabled(True)
-                    else:
-                        default_index = param_input_widget.findText(str(existing_params[param.name]))
-                        param_input_widget.setCurrentIndex(default_index)
-                        param_input_widget.setEnabled(False)
+                    default_index = param_input_widget.findText(str(param.default))
+                    param_input_widget.setCurrentIndex(default_index)
+                    param_input_widget.setEnabled(True)
+
                 # Dropdown for parameters with predefined options
-                elif param.name in selected_class.options:
+                elif param.name in class_instance.options:
                     param_input_widget = QComboBox()
-                    param_input_widget.addItems(selected_class.options[param.name])
-                    if param.default in selected_class.options[param.name]:
-                        if self.init_method is None:
-                            default_index = param_input_widget.findText(param.default)
-                            param_input_widget.setCurrentIndex(default_index)
-                            param_input_widget.setEnabled(True)
-                        else:
-                            param_input_widget.setCurrentIndex(str(existing_params[param.name]))
-                            param_input_widget.setEnabled(False)    
+                    param_input_widget.addItems(class_instance.options[param.name])
+                    
+                    if param.default in class_instance.options[param.name]:
+                        default_index = param_input_widget.findText(param.default)
+                        param_input_widget.setCurrentIndex(default_index)
+                        param_input_widget.setEnabled(True)
+
                 # Spinbox for integer parameterss
                 elif type(param.default) == int:
                     param_input_widget = QSpinBox()
                     param_input_widget.setMaximum(10000)
                     param_input_widget.setMinimum(-10000)
                     param_input_widget.setSingleStep(1)
-                    if self.init_method is None:
-                        param_input_widget.setValue(int(param.default) if param.default != inspect.Parameter.empty else 0)
-                        param_input_widget.setEnabled(True)
-                    else:
-                        param_input_widget.setValue(int(existing_params[param.name]))
-                        param_input_widget.setEnabled(False)
+
+                    param_input_widget.setValue(int(param.default) if param.default != inspect.Parameter.empty else 0)
+                    param_input_widget.setEnabled(True)
+
                 # Spinbox for float parameters
                 elif type(param.default) == float:
                     param_input_widget = QDoubleSpinBox()
                     param_input_widget.setMaximum(10000.0)
                     param_input_widget.setMinimum(-10000.0)
                     param_input_widget.setSingleStep(0.1)
-                    if self.init_method is None:
-                        param_input_widget.setValue(float(param.default) if param.default != inspect.Parameter.empty else 0.0)
-                        param_input_widget.setEnabled(True)
-                    else: 
-                        param_input_widget.setValue(float(existing_params[param.name]))
-                        param_input_widget.setEnabled(False)
+
+                    param_input_widget.setValue(float(param.default) if param.default != inspect.Parameter.empty else 0.0)
+                    param_input_widget.setEnabled(True)
+
                 # Text field for other types of parameters
                 else:
-                    if self.init_method is None:
-                        param_input_widget = QLineEdit(str(param.default) if param.default != inspect.Parameter.empty else "")
-                        param_input_widget.setEnabled(True)
-                    else:
-                        param_input_widget.setValue(str(existing_params[param.name]))
-                        param_input_widget.setEnabled(False)
+                    param_input_widget = QLineEdit(str(param.default) if param.default != inspect.Parameter.empty else "")
+                    param_input_widget.setEnabled(True)
+   
 
                 # Create info button with tooltip
-                info_text = self.getInfoText(param.name, self.selected_class_name)
+                info_text = self.getInfoText(param.name, self.data.dfc_name)
                 info_button = InfoButton(info_text)
 
                 # Create layout for label, widget, and info button
                 param_layout = QHBoxLayout()
                 param_layout.addWidget(param_label)
                 param_layout.addWidget(param_input_widget)
                 param_layout.addWidget(info_button) 
@@ -641,15 +690,15 @@
     def onTabChanged(self):
         self.currentTabIndex = self.tabWidget.currentIndex()
         # index 0: Connectivity plot
         # index 1: Time series plot
         # index 2: Distribution plot
         # index 3: Graph analysis
 
-        if self.dfc_data['data'] is None:
+        if self.data.dfc_data is None:
             self.plot_logo()
             self.canvas.draw()
             self.distributionFigure.clear()
             self.distributionCanvas.draw()
             self.timeSeriesFigure.clear()
             self.timeSeriesCanvas.draw()
             self.backLargeButton.hide()
@@ -664,30 +713,30 @@
             self.slider.show()
             self.slider.setValue(self.currentSliderValue)
             self.backLargeButton.show()
             self.backButton.show()
             self.forwardButton.show()
             self.forwardLargeButton.show()
 
-            if self.dfc_data['data'] is not None:
-                total_length = self.dfc_data['data'].shape[2] if len(self.dfc_data['data'].shape) == 3 else 0
-                position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.dfc_data['data'].shape) == 3 else " static "
+            if self.data.dfc_data is not None:
+                total_length = self.data.dfc_data.shape[2] if len(self.data.dfc_data.shape) == 3 else 0
+                position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.data.dfc_data.shape) == 3 else " static "
             else:
                 position_text = "no data available"
 
             self.positionLabel.setText(position_text)
 
         elif self.currentTabIndex == 1:
             self.backLargeButton.hide()
             self.backButton.hide()
             self.forwardButton.hide()
             self.forwardLargeButton.hide()
             
             # If we have nothing to scroll though, hide some GUI elements
-            if len(self.dfc_data['data'].shape) == 2 or self.edge_ts is not None or self.state_tc is not None:
+            if len(self.data.dfc_data.shape) == 2 or self.data.dfc_edge_ts is not None or self.data.dfc_state_tc is not None:
                 position_text = ""
                 self.slider.hide()
                 
                 # Disable brain area selector widgets
                 for i in range(self.timeSeriesSelectorLayout.count()):    
                     widget = self.timeSeriesSelectorLayout.itemAt(i).widget()
                     if widget is not None:
@@ -701,15 +750,15 @@
                 # Enable brain area selector widgets
                 for i in range(self.timeSeriesSelectorLayout.count()):    
                     widget = self.timeSeriesSelectorLayout.itemAt(i).widget()
                     if widget is not None:
                         widget.setVisible(True)
 
             # We have a static measure
-            if len(self.dfc_data['data'].shape) == 2 and self.edge_ts is None and self.state_tc is None:
+            if len(self.data.dfc_data.shape) == 2 and self.data.dfc_edge_ts is None and self.data.dfc_state_tc is None:
                 self.timeSeriesFigure.clear()
                 self.timeSeriesCanvas.draw()
 
                 # Disable brain area selector widgets
                 for i in range(self.timeSeriesSelectorLayout.count()):    
                     widget = self.timeSeriesSelectorLayout.itemAt(i).widget()
                     if widget is not None:
@@ -818,196 +867,233 @@
             elif item.spacerItem():  # If the item is a spacer
                 # No need to delete spacer items; they are automatically handled by Qt
                 pass
     
     def loadFile(self):
         fileFilter = "All Supported Files (*.mat *.txt *.npy *pkl *tsv);;MAT Files (*.mat);;Text Files (*.txt);;NumPy Files (*.npy);;Pickle Files (*.pkl);;TSV Files (*.tsv))"
         file_path, _ = QFileDialog.getOpenFileName(self, "Load File", "", fileFilter)
-        self.file_name = file_path.split('/')[-1]
+        file_name = file_path.split('/')[-1]
+        self.data.file_name = file_name
+        self.getParameters() # Get current UI parameters
 
         if not file_path:
             return  # Early exit if no file is selected
 
-        try:
-            if file_path.endswith('.mat'):
-                self.ts_data = loadmat(file_path)  # Assuming you'll adjust how to extract the array
-            elif file_path.endswith('.txt'):
-                self.ts_data = np.loadtxt(file_path)
-            elif file_path.endswith('.npy'):
-                self.ts_data = np.load(file_path)
-            elif file_path.endswith('.pkl'):
-                with open(file_path, 'rb') as f:
-                    self.ts_data = pickle.load(f)
-            elif file_path.endswith(".tsv"):
-                data = pd.read_csv(file_path, sep='\t', header=None, na_values='n/a')
+        if file_path.endswith('.mat'):
+            data_dict = loadmat(file_path)
+            self.data.file_data = data_dict[list(data_dict.keys())[-1]] # always get data for the last key
+        elif file_path.endswith('.txt'):
+            self.data.file_data = np.loadtxt(file_path)
+        elif file_path.endswith('.npy'):
+            self.data.file_data = np.load(file_path)
+        elif file_path.endswith('.pkl'):
+            with open(file_path, 'rb') as f:
+                self.data.file_data = pickle.load(f)
+        elif file_path.endswith(".tsv"):
+            data = pd.read_csv(file_path, sep='\t', header=None, na_values='n/a')
 
-                if data.iloc[0].apply(lambda x: np.isscalar(x) and np.isreal(x)).all():
-                    rois = None  # No rois found, the first row is part of the data
-                else:
-                    rois = data.iloc[0]  # The first row is rois
-                    data = data.iloc[1:]  # Remove the header row from the data
+            if data.iloc[0].apply(lambda x: np.isscalar(x) and np.isreal(x)).all():
+                rois = None  # No rois found, the first row is part of the data
+            else:
+                rois = data.iloc[0]  # The first row is rois
+                data = data.iloc[1:]  # Remove the header row from the data
 
-                # Convert all data to numeric, making sure 'n/a' and other non-numeric are treated as NaN
-                data = data.apply(pd.to_numeric, errors='coerce')
+            # Convert all data to numeric, making sure 'n/a' and other non-numeric are treated as NaN
+            data = data.apply(pd.to_numeric, errors='coerce')
 
-                # Identify entirely empty columns
-                empty_columns = data.columns[data.isna().all()]
-                
-                # Remove corresponding rois if rois exist
-                if rois is not None:
-                    removed_rois = rois[empty_columns].to_list()
-                    print("The following regions were empty and thus removed:", removed_rois)
-                    rois = rois.drop(empty_columns)
+            # Identify entirely empty columns
+            empty_columns = data.columns[data.isna().all()]
+            
+            # Remove corresponding rois if rois exist
+            if rois is not None:
+                removed_rois = rois[empty_columns].to_list()
+                print("The following regions were empty and thus removed:", removed_rois)
+                rois = rois.drop(empty_columns)
 
-                # Remove entirely empty columns and rows
-                data = data.dropna(axis=1, how='all').dropna(axis=0, how='all')
+            # Remove entirely empty columns and rows
+            data = data.dropna(axis=1, how='all').dropna(axis=0, how='all')
 
-                # Convert the cleaned data back to numpy array
-                self.ts_data = data.to_numpy()
+            # Convert the cleaned data back to numpy array
+            self.data.file_data = data.to_numpy()
 
-                # Update header_list if rois exist
-                self.roi_data = np.array(rois, dtype=object)
+            # Update header_list if rois exist
+            self.data.roi_names = np.array(rois, dtype=object)
 
-            else:
-                self.ts_data = None
-                self.time_series_textbox.setText("Unsupported file format")
+        else:
+            self.data.file_data = None
+            self.time_series_textbox.setText("Unsupported file format")
 
-            # New data, reset slider and plot
-            self.currentSliderValue = 0
-            self.slider.setValue(0)
-            self.figure.clear()
-            self.canvas.draw()
+        # New data, reset slider and plot
+        self.currentSliderValue = 0
+        self.slider.setValue(0)
+        self.figure.clear()
+        self.canvas.draw()
 
-            # Set filenames depending on file type
-            if file_path.endswith('.pkl'):
-                self.fileNameLabel.setText(f"Loaded TIME_SERIES object")
-                self.time_series_textbox.setText(self.file_name)
-
-                self.continuousCheckBox.setEnabled(False)
-                self.continuousCheckBox.setChecked(False)
-
-                self.stateBasedCheckBox.setEnabled(True)
-                self.stateBasedCheckBox.setChecked(True)
-
-                self.staticCheckBox.setEnabled(False)
-                self.staticCheckBox.setChecked(False)
-
-                self.reshapeCheckbox.setEnabled(False)
-            else: 
-                self.fileNameLabel.setText(f"Loaded {self.file_name} with shape {self.ts_data.shape}")
-                self.time_series_textbox.setText(self.file_name)
-
-                self.continuousCheckBox.setEnabled(True)
-                self.continuousCheckBox.setChecked(True)
-
-                self.stateBasedCheckBox.setEnabled(False)
-                self.stateBasedCheckBox.setChecked(False)
-
-                self.staticCheckBox.setEnabled(True)
-                self.staticCheckBox.setChecked(True)
-      
-                self.reshapeCheckbox.setEnabled(True)
-
-            # Show transpose textbox
-            self.reshapeCheckbox.show()
-
-            # Reset and enable the GUI elements
-            self.methodComboBox.setEnabled(True)
-            #self.methodComboBox.setCurrentText("Sliding Window")
-            self.init_method = None
-            #self.onMethodChanged()
-
-            self.methodComboBox.setEnabled(True)
-            self.calculateButton.setEnabled(True)
-            self.clearMemoryButton.setEnabled(True)
-            self.keepInMemoryCheckbox.setEnabled(True)
+        # Set filenames depending on file type
+        if file_path.endswith('.pkl'):
+            self.fileNameLabel.setText(f"Loaded TIME_SERIES object")
+            self.time_series_textbox.setText(file_name)
 
-        except Exception as e:
-            print(f"Error loading data: {e}")
-            self.fileNameLabel.setText(f"Error. No time series data has been loaded.")
+            self.continuousCheckBox.setEnabled(False)
+            self.continuousCheckBox.setChecked(False)
+
+            self.stateBasedCheckBox.setEnabled(True)
+            self.stateBasedCheckBox.setChecked(True)
+
+            self.staticCheckBox.setEnabled(False)
+            self.staticCheckBox.setChecked(False)
+
+            self.reshapeCheckbox.setEnabled(False)
+        else:
+            self.fileNameLabel.setText(f"Loaded {self.data.file_name} with shape {self.data.file_data.shape}")
+            self.time_series_textbox.setText(file_name)
+
+            self.continuousCheckBox.setEnabled(True)
+            self.continuousCheckBox.setChecked(True)
+
+            self.stateBasedCheckBox.setEnabled(False)
+            self.stateBasedCheckBox.setChecked(False)
+
+            self.staticCheckBox.setEnabled(True)
+            self.staticCheckBox.setChecked(True)
+    
+            self.reshapeCheckbox.setEnabled(True)
+
+        # Show transpose textbox
+        self.reshapeCheckbox.show()
+
+        # Reset and enable the GUI elements
+        self.methodComboBox.setEnabled(True)
+        self.methodComboBox.setEnabled(True)
+        self.calculateButton.setEnabled(True)
+        self.clearMemoryButton.setEnabled(True)
+        self.keepInMemoryCheckbox.setEnabled(True)
 
     def saveFile(self):
-        if not hasattr(self, 'dfc_data'):
+        if self.data.dfc_data is None:
             print("No dFC data available to save.")
             return
 
         # Open a file dialog to specify where to save the file
         filePath, _ = QFileDialog.getSaveFileName(self, "Save File", "", "MAT Files (*.mat)")
         
         if filePath:
             # Ensure the file has the correct extension
             if not filePath.endswith('.mat'):
                 filePath += '.mat'
             
             # Save the data
             try:
-                savemat(filePath, {'dfc_data': self.dfc_data['data'], 'roi_data': self.roi_data})
+                datadict = self.dataclass_to_dict(self.data)
+                savemat(filePath, datadict)
             except Exception as e:
                 print(f"Error saving data: {e}")
 
+    def compare_param_dicts(self, dict1, dict2):
+        # Check if both inputs are dictionaries
+        if not isinstance(dict1, dict) or not isinstance(dict2, dict):
+            return False
+        
+        # Check if the keys match
+        if sorted(dict1.keys()) != sorted(dict2.keys()):
+            return False
+        
+        # Recursively compare values
+        for key in dict1.keys():
+            value1 = dict1[key]
+            value2 = dict2[key]
+            
+            if isinstance(value1, dict) and isinstance(value2, dict):
+                # Recursively compare nested dictionaries
+                if not self.compare_param_dicts(value1, value2):
+                    return False
+            elif isinstance(value1, np.ndarray) and isinstance(value2, np.ndarray):
+                # Compare NumPy arrays
+                if not np.array_equal(value1, value2):
+                    return False
+            elif value1 != value2:
+                # Compare other types
+                return False
+        
+        # All checks passed, dictionaries are equivalent
+        return True
+
+    def dataclass_to_dict(self, data_instance):
+        data_dict = {}
+        for field in data_instance.__dataclass_fields__:
+            value = getattr(data_instance, field)
+            if isinstance(value, np.ndarray):
+                data_dict[field] = value
+            elif isinstance(value, dict):
+                # Assume dictionaries contain simple types or numpy arrays
+                data_dict[field] = {k: (v.tolist() if isinstance(v, np.ndarray) else v) for k, v in value.items()}
+            elif value is None:
+                # Handle None values appropriately
+                data_dict[field] = np.array([])
+            elif field == 'dfc_instance':
+                # For the dfc_instance only its type is stored
+                data_dict[field] = str(type(value))
+            else:
+                data_dict[field] = value
+        return data_dict
+
     def onReshapeCheckboxChanged(self, state):
-        if self.ts_data is None:
+        if self.data.file_data is None:
             return  # No data loaded, so do nothing
 
         if state == Qt.CheckState.Checked:
             # Transpose the data
-            self.ts_data = self.ts_data.transpose()
+            self.data.file_data = self.data.file_data.transpose()
         else:
             # Transpose it back to original
-            self.ts_data = self.ts_data.transpose()
+            self.data.file_data = self.data.file_data.transpose()
 
         # Update the labels
-        self.fileNameLabel.setText(f"Loaded {self.time_series_textbox.text()} with shape: {self.ts_data.shape}")
-        self.time_series_textbox.setText(self.file_name)
+        self.fileNameLabel.setText(f"Loaded {self.time_series_textbox.text()} with shape: {self.data.file_data.shape}")
+        self.time_series_textbox.setText(self.data.file_name)
 
     def handleResult(self, result):
-        # Handles the result of the worker thread
-        self.dfc_data = result
-
-        #if self.abortFlag:
-        #    print("Calculation was aborted, no results will be shown.")
-        #    self.abortFlag = False
-        #    return
-
         # Update the sliders and text
-        if self.dfc_data['data'] is not None:
-            self.calculatingLabel.setText(f"Calculated {self.selected_class_name} with shape {self.dfc_data['data'].shape}")
+        if self.data.dfc_data is not None:
+            self.calculatingLabel.setText(f"Calculated {self.data.dfc_name} with shape {self.data.dfc_data.shape}")
             
-            if len(self.dfc_data['data'].shape) == 3:
+            if len(self.data.dfc_data.shape) == 3:
                 self.slider.show()
-                self.rowSelector.setMaximum(self.dfc_data['data'].shape[0] - 1)
-                self.colSelector.setMaximum(self.dfc_data['data'].shape[1] - 1)
+                self.rowSelector.setMaximum(self.data.dfc_data.shape[0] - 1)
+                self.colSelector.setMaximum(self.data.dfc_data.shape[1] - 1)
                 self.rowSelector.setValue(1)
 
             # Update time label
-            total_length = self.dfc_data['data'].shape[2] if len(self.dfc_data['data'].shape) == 3 else 0
+            total_length = self.data.dfc_data.shape[2] if len(self.data.dfc_data.shape) == 3 else 0
             
             if self.currentTabIndex == 0 or self.currentTabIndex == 2:
-                position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.dfc_data['data'].shape) == 3 else " static "
+                position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.data.dfc_data.shape) == 3 else " static "
             else:
                 position_text = ""
 
             self.positionLabel.setText(position_text)
             self.slider.setValue(self.slider.value())
             
         # Plot
         self.plot_dfc()
         self.updateDistribution()
         self.plotTimeSeries()
         self.calculateButton.setEnabled(True)
         self.onTabChanged()
+        self.update()
 
     def handleError(self, error):
         # Handles errors in the worker thread
         print(f"Error occurred: {error}")
 
     def getParameters(self):
         # Get the time series and parameters (from the UI) for the selected connectivity method and store them in a dictionary
-        self.parameters = {}
-        self.parameters['time_series'] = self.ts_data
+        
+        # Time series data
+        self.data.dfc_params['time_series'] = self.data.file_data
 
         # Converts string to boolean, float, or retains as string if conversion is not applicable
         def convert_value(value):
             if value.lower() in ['true', 'false']:
                 return value.lower() == 'true'
             try:
                 return float(value)
@@ -1033,210 +1119,219 @@
 
                 widget = layout.itemAt(1).widget()
                 value = get_widget_value(widget)
 
                 if value is not None:  # Ensure there is a value before attempting to convert and store
                     param_key = self.reverse_param_names.get(label)
                     if param_key:  # Ensure the key exists in the reverse_param_names dictionary
-                        self.parameters[param_key] = convert_value(value) if isinstance(value, str) else value
+                        self.data.dfc_params[param_key] = convert_value(value) if isinstance(value, str) else value
                     else:
                         self.calculatingLabel.setText(f"Error: Unrecognized parameter '{label}'")
                 else:
                     # Value could not be retrieved from the widget
                     self.calculatingLabel.setText(f"Error: No value entered for parameter '{label}'")
 
+    def setParameters(self):
+        # Converts value to string
+        def convert_value_to_string(value):
+            if isinstance(value, bool):
+                return 'true' if value else 'false'
+            elif isinstance(value, (int, float)):
+                return str(value)
+            else:
+                return value
+
+        # Sets the value of the widget based on its type
+        def set_widget_value(widget, value):
+            if isinstance(widget, QLineEdit):
+                widget.setText(value)
+            elif isinstance(widget, QComboBox):
+                index = widget.findText(value)
+                if index >= 0:
+                    widget.setCurrentIndex(index)
+            elif isinstance(widget, (QSpinBox, QDoubleSpinBox)):
+                widget.setValue(int(value))
+
+        # No parameters yet, return
+        if not self.data.dfc_params:
+            self.getParameters()
+            return
+
+        # Time series data has to be in the params as we run the dFC method with just these params
+        self.data.dfc_params['time_series'] = self.data.file_data
+
+        # Set the parameters in the UI based on the stored dictionary
+        for i in range(self.parameterLayout.count()):
+            layout = self.parameterLayout.itemAt(i).layout()
+            if layout:
+                label = layout.itemAt(0).widget().text().rstrip(':')
+                if label == 'Time series':
+                    continue  # Skip 'time_series' as it's already set
+
+                param_key = self.reverse_param_names.get(label)
+                if param_key:  # Ensure the key exists in the reverse_param_names dictionary
+                    value = self.data.dfc_params.get(param_key)
+                    if value is not None:  # Ensure there is a value before attempting to convert and set
+                        widget = layout.itemAt(1).widget()
+                        set_widget_value(widget, convert_value_to_string(value))
+                    else:
+                        # Value could not be retrieved from the dictionary
+                        self.calculatingLabel.setText(f"Error: No value entered for parameter '{label}'")
+                else:
+                    self.calculatingLabel.setText(f"Error: Unrecognized parameter '{label}'")
+
     def onCalculateConnectivity(self):
         # Check if ts_data is available
-        if self.ts_data is None:
+        if self.data.file_data is None:
             self.calculatingLabel.setText(f"Error. No time series data has been loaded.")
             return
-    
-        # Check if method is available
-        selected_class = getattr(methods, self.selected_class_name, None)
-        if not selected_class:
-            print("Selected class not found in connectivity module")
-            return
         
+        # Get the current parameters from the UI for the upcoming calculation
+        self.getParameters()
+    
         # Process all pending events
         QApplication.processEvents() 
-
-        # Gets the parameters and stores them in self.parameters
-        self.getParameters()
         
         # Start worker thread for dFC calculations and submit for calculation
         self.workerThread = QThread()
-        self.worker = Worker(self.calculateDFC, self.parameters)
+        self.worker = Worker(self.calculateDFC, self.data.dfc_params)
         self.worker.moveToThread(self.workerThread)
         
         self.worker.finished.connect(self.workerThread.quit)
         self.worker.result.connect(self.handleResult)
         self.worker.error.connect(self.handleError)
 
         self.workerThread.started.connect(self.worker.run)
         self.workerThread.start()
         self.calculatingLabel.setText(f"Calculating {self.methodComboBox.currentText()}, please wait...")
         self.calculateButton.setEnabled(False)
     
-    def check_data_dict_equality(self, dict1, dict2):
-        if dict1.keys() != dict2.keys():
-            return False  # The dictionaries have different sets of keys
-        
-        for key in dict1:
-            val1, val2 = dict1[key], dict2[key]
-            
-            # If both values are numpy arrays, use numpy.array_equal
-            if isinstance(val1, np.ndarray) and isinstance(val2, np.ndarray):
-                if not np.array_equal(val1, val2):
-                    return False
-            # If values are dictionaries, recursively compare
-            elif isinstance(val1, dict) and isinstance(val2, dict):
-                if not self.check_data_dict_equality(val1, val2):
-                    return False
-            # For other types, use standard equality check
-            else:
-                if val1 != val2:
-                    return False
-
-        return True  # All keys and values are equal
-
     def calculateDFC(self, parameters):
         keep_in_memory = self.keepInMemoryCheckbox.isChecked()
         
-        # Try to calculate dFC, throw an exception if  it fails
-        try:
-            # Check if data for the selected class name exists with the same parameters
-            existing_data = self.dfc_data_dict.get(self.selected_class_name) # returns None if key does not exist (avoid KeyError)
-            #if existing_data is not None and existing_data.get('data') is not None and existing_data.get('data').size > 0 and self.check_data_dict_equality(existing_data.get('parameters'), parameters):
-            if existing_data is not None and existing_data.get('data') is not None and self.check_data_dict_equality(existing_data.get('parameters'), parameters):
-                print(f"Using stored data for {self.selected_class_name} with given parameters")
-                return {"data": existing_data['data'], "parameters": parameters}
-
-            # If parameters have changed or data doesn't exist, proceed to calculate new data
-            selected_class = getattr(methods, self.selected_class_name, None)
-            if not selected_class:
-                print("Selected class not found in connectivity module")
-                return None
-
-            connectivity_calculator = selected_class(**parameters)
-            result = connectivity_calculator.connectivity()
-            
-            # In case the method returns multiple values. The first one is always the NxNxT dfc matrix
-            if isinstance(result, tuple):
-                self.dfc_data['data'], _ = result
-                self.dfc_data['parameters'] = parameters
-                self.state_tc = None
-                self.edge_ts = result[1][0] if isinstance(result[1], tuple) else None
-
-            # Result is DFC object (pydfc methods)
-            elif isinstance(result, pydfc.dfc.DFC):
-                self.dfc_data['data'] = np.transpose(result.get_dFC_mat(), (1, 2, 0))
-                self.dfc_data['parameters'] = parameters
-                self.dfc_states = result.FCSs
-                self.state_tc = result.state_TC()
-                self.edge_ts = None
-            
-            # Only a single matrix is returned (most cases)
-            else:
-                self.dfc_data['data'] = result
-                self.dfc_data['parameters'] = parameters
-                self.state_tc = None
-                self.edge_ts = None
-
-            # Store in memory if checkbox is checked
-            if keep_in_memory:
-                # Update the dictionary entry for the selected_class_name with the new data and parameters
-                self.dfc_data_dict[self.selected_class_name] = {'data': self.dfc_data['data'], 'parameters': parameters}
-                print(f"Updated {self.selected_class_name} data with new parameters in memory")
+        # Try to calculate dFC, throw an exception if it fails
+        # TODO: Add try except block again
 
-            return self.dfc_data
-
-        except Exception as e:
-            print(f"Exception when calculating dFC: {e}")
-            self.calculatingLabel.setText(f"Error calculating connectivity, check parameters.")
-            return None
+        # Check if data already exists
+        existing_data = self.data_storage.check_for_identical_data(self.data)
+        if existing_data is not None:
+            return existing_data
+        
+        # Data does not exist, perform calculation
+        connectivity_calculator = self.data.dfc_instance(**parameters)
+        result = connectivity_calculator.connectivity()
+        self.init_flag = False
+
+        # In case the method returns multiple values. The first one is always the NxNxT dfc matrix
+        if isinstance(result, tuple):
+            self.data.dfc_data = result[0]
+            self.data.dfc_params = parameters
+            self.data.dfc_state_tc = None
+            self.data.dfc_edge_ts = result[1][0] if isinstance(result[1], tuple) else None
+
+        # Result is DFC object (pydfc methods)
+        elif isinstance(result, pydfc.dfc.DFC):
+            self.data.dfc_data = np.transpose(result.get_dFC_mat(), (1, 2, 0))
+            self.data.dfc_params = parameters
+            self.data.dfc_states = result.FCSs_
+            self.data.dfc_state_tc = result.state_TC()
+            self.data.dfc_edge_ts = None
+        
+        # Only a single matrix is returned (most cases)
+        else:
+            self.data.dfc_data = result
+            self.data.dfc_params = parameters
+            self.data.dfc_state_tc = None
+            self.data.dfc_edge_ts = None
+
+        # Store in memory if checkbox is checked
+        if keep_in_memory:
+            # Update the dictionary entry for the selected_class_name with the new data and parameters
+            self.data_storage.add_data(self.data)
+            #print(f"Added {self.data.dfc_name} data to memory")
 
-    def saveDataToDict(self, parameters):
-        self.dfc_data_dict[self.selected_class_name] = {'data': self.dfc_data['data'], 'parameters': parameters}
-        return
+        print("Finished calculation.")    
+        return self.data
 
     def onKeepInMemoryChanged(self, state):
-        if state == 2 and self.dfc_data['data'] is not None:
-            self.saveDataToDict(self.parameters)
-            print(f"Saved {self.selected_class_name} data to memory")
+        if state == 2 and self.data.dfc_data is not None:
+            self.data_storage.add_data(self.data)
+            #print(f"Saved {self.data.dfc_name} data to memory")
                 
     def onClearMemory(self):
-        self.dfc_data_dict = {}
+        self.data_storage = DataStorage()
         
         self.figure.clear()
         self.canvas.draw()
         self.distributionFigure.clear()
         self.distributionCanvas.draw()
 
         self.calculatingLabel.setText(f"Cleared memory")
         print("Cleared memory")
-
         return
 
     def plot_dfc(self):
-        if not hasattr(self, 'dfc_data'):
+        current_data = self.data.dfc_data
+        
+        if current_data is None:
             print("No calculated data available for plotting")
             return
 
         self.figure.clear()
         ax = self.figure.add_subplot(111)
 
-        if self.dfc_data['data'] is not None:
-            current_data = self.dfc_data['data']
-            try:
-                current_slice = current_data[:, :, self.currentSliderValue] if len(current_data.shape) == 3 else current_data
-                vmax = np.max(np.abs(current_slice))
-                self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
-            except:
-                current_slice = current_data[:, :, 0] if len(current_data.shape) == 3 else current_data
-                vmax = np.max(np.abs(current_slice))
-                self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
-
-            # Create the colorbar
-            divider = make_axes_locatable(ax)
-            cax = divider.append_axes("right", size="5%", pad=0.15)
-            cbar = self.figure.colorbar(self.im, cax=cax)
-            cbar.ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
+        try:
+            current_slice = current_data[:, :, self.currentSliderValue] if len(current_data.shape) == 3 else current_data
+            vmax = np.max(np.abs(current_slice))
+            self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
+        except:
+            current_slice = current_data[:, :, 0] if len(current_data.shape) == 3 else current_data
+            vmax = np.max(np.abs(current_slice))
+            self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
+
+        # Create the colorbar
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.15)
+        cbar = self.figure.colorbar(self.im, cax=cax)
+        cbar.ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
 
-            self.slider.setMaximum(current_data.shape[2] - 1 if len(current_data.shape) == 3 else 0)
-        
+        self.slider.setMaximum(current_data.shape[2] - 1 if len(current_data.shape) == 3 else 0)
+    
         self.figure.set_facecolor('#E0E0E0')
         self.figure.tight_layout()
         self.canvas.draw()
 
     def plotTimeSeries(self):
-        current_data = self.dfc_data['data']
+        current_data = self.data.dfc_data
+
         # Get dimensions of the data
         if current_data is not None and current_data.ndim == 3:
             self.rowSelector.setMaximum(current_data.shape[0] - 1)
             self.colSelector.setMaximum(current_data.shape[1] - 1)
 
         row = self.rowSelector.value()
         col = self.colSelector.value()
         self.rowSelector.show()
         self.colSelector.show()
 
-        if current_data is not None and row < current_data.shape[0] and col < current_data.shape[1] and self.edge_ts is None and self.state_tc is None:    
+        if current_data is not None and row < current_data.shape[0] and col < current_data.shape[1] and self.data.dfc_edge_ts is None and self.data.dfc_state_tc is None:    
             self.timeSeriesFigure.clear()
             ax = self.timeSeriesFigure.add_subplot(111)
             time_series = current_data[row, col, :] if len(current_data.shape) == 3 else current_data[row, col]
             ax.set_title(f"dFC time course between region {row} and {col}.")
             
             ax.plot(time_series)
             self.timeSeriesCanvas.draw()
 
-        elif self.state_tc is not None:
+        elif self.data.dfc_state_tc is not None:
             self.timeSeriesFigure.clear()
 
-            time_series = self.state_tc
-            num_states = len(self.dfc_states)
+            time_series = self.data.dfc_state_tc
+            num_states = len(self.data.dfc_states)
+
             # Setup the gridspec layout
             gs = gridspec.GridSpec(3, num_states, self.timeSeriesFigure, height_ratios=[1, 0.5, 1])
 
             # Hite selectors
             self.rowSelector.hide()
             self.colSelector.hide()
 
@@ -1244,37 +1339,37 @@
             ax_time_series = self.timeSeriesFigure.add_subplot(gs[0, :])
             ax_time_series.plot(time_series)
             ax_time_series.set_ylabel("State")
             ax_time_series.set_title("State time course")
             ax_time_series.set_xlabel("Time (TRs)")
 
             # Plot the individual states
-            for col, (state, matrix) in enumerate(self.dfc_states.items()):
+            for col, (state, matrix) in enumerate(self.data.dfc_states.items()):
                 ax_state = self.timeSeriesFigure.add_subplot(gs[2, col])
                 ax_state.imshow(matrix, cmap='coolwarm', aspect=1)
                 ax_state.set_title(f"State {col+1}")
                 ax_state.set_xticks([])
                 ax_state.set_yticks([]) 
 
             self.timeSeriesFigure.canvas.draw()
 
-        elif self.edge_ts is not None:
+        elif self.data.dfc_edge_ts is not None:
             self.timeSeriesFigure.clear()
             gs = gridspec.GridSpec(3, 1, self.timeSeriesFigure, height_ratios=[2, 0.5, 1]) # GridSpec with 3 rows and 1 column
 
             # The first subplot occupies the 1st row
             ax1 = self.timeSeriesFigure.add_subplot(gs[:1, 0])
-            ax1.imshow(self.edge_ts.T, cmap='coolwarm', aspect='auto', vmin=-1*self.parameters["vlim"], vmax=self.parameters["vlim"])
+            ax1.imshow(self.data.dfc_edge_ts.T, cmap='coolwarm', aspect='auto', vmin=-1*self.data.dfc_params["vlim"], vmax=self.data.dfc_params["vlim"])
             ax1.set_title("Edge time series")
             ax1.set_xlabel("Time (TRs)")
             ax1.set_ylabel("Edges")
 
             # The second subplot occupies the 3rd row
             ax2 = self.timeSeriesFigure.add_subplot(gs[2, 0])
-            mean_edge_values = np.mean(self.edge_ts.T, axis=0)
+            mean_edge_values = np.mean(self.data.dfc_edge_ts.T, axis=0)
             ax2.plot(mean_edge_values)
             ax2.set_xlim(0, len(mean_edge_values) - 1)
             ax2.set_title("Mean time series")
             ax2.set_xlabel("Time (TRs)")
             ax2.set_ylabel("Mean Edge Value")
             
             self.timeSeriesFigure.canvas.draw()
@@ -1294,15 +1389,15 @@
         self.im = ax.imshow(logo)
 
         self.figure.set_facecolor('#f4f1f6')
         self.figure.tight_layout()
         self.canvas.draw()
 
     def updateDistribution(self):
-        current_data = self.dfc_data['data']
+        current_data = self.data.dfc_data
 
         if current_data is None or not hasattr(self, 'distributionFigure'):
             self.distributionFigure.clear()
             return
 
         # Clear the current distribution plot
         self.distributionFigure.clear()
@@ -1312,32 +1407,32 @@
         ax = self.distributionFigure.add_subplot(111)
         ax.hist(current_slice.flatten(), bins=50)  # number of bins
 
         self.distributionCanvas.draw()
 
     def onSliderValueChanged(self, value):
         # Ensure there is data to work with
-        if self.dfc_data['data'] is None or self.im is None:
+        if self.data.dfc_data is None or self.im is None:
             return
         
         if self.currentTabIndex == 0 or self.currentTabIndex == 2:
             # Get and update the data of the imshow object
             self.currentSliderValue = value
-            data = self.dfc_data['data']
+            data = self.data.dfc_data
             self.im.set_data(data[:, :, value]) if len(data.shape) == 3 else self.im.set_data(data)
 
             vlim = np.max(np.abs(data[:, :, value])) if len(data.shape) == 3 else np.max(np.abs(data))
             self.im.set_clim(-vlim, vlim)
 
             # Redraw the canvas
             self.canvas.draw()
             self.updateDistribution()
 
-            total_length = self.dfc_data['data'].shape[2] if len(self.dfc_data['data'].shape) == 3 else 0
-            position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.dfc_data['data'].shape) == 3 else " static "
+            total_length = self.data.dfc_data.shape[2] if len(self.data.dfc_data.shape) == 3 else 0
+            position_text = f"t = {self.currentSliderValue} / {total_length-1}" if len(self.data.dfc_data.shape) == 3 else " static "
             self.positionLabel.setText(position_text)
 
     
         elif self.currentTabIndex == 1:
             self.updateTimeSeriesPlot(value)
 
     def moveBack(self):
@@ -1361,18 +1456,18 @@
         self.currentSliderValue = max(0, min(self.slider.value() + delta, self.slider.maximum()))
         self.slider.setValue(self.currentSliderValue)
 
         self.plot_dfc()
         self.updateDistribution()
 
     def updateTimeSeriesPlot(self, center):
-        if self.dfc_data['data'] is None:
+        if self.data.dfc_data is None:
             return
 
-        max_index = self.dfc_data['data'].shape[2] - 1 if len(self.dfc_data['data'].shape) == 3 else 0
+        max_index = self.data.dfc_data.shape[2] - 1 if len(self.data.dfc_data.shape) == 3 else 0
         width = 101
 
         # Determine if we should show the entire series or a window
         if center == 0 or center == max_index:
             start = 0
             end = max_index
         else:
@@ -1382,15 +1477,14 @@
         row = self.rowSelector.value()
         col = self.colSelector.value()
         time_series_slice = self.dfc_data['data'][row, col, start:end]
 
         self.timeSeriesFigure.clear()
         ax = self.timeSeriesFigure.add_subplot(111)
         ax.plot(range(start, end), time_series_slice)
-        #ax.set_title(f"dFC time series ({row}, {col})")
         self.timeSeriesCanvas.draw()
 
 def run(dfc_data=None, method=None):
     app = QApplication(sys.argv)
 
     # Set global stylesheet for tooltips
     QApplication.instance().setStyleSheet("""
```

### Comparing `comet_toolbox-0.1.2/src/comet/methods.py` & `comet_toolbox-0.1.4/src/comet/methods.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/multiverse.py` & `comet_toolbox-0.1.4/src/comet/multiverse.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/simulation.pkl` & `comet_toolbox-0.1.4/src/comet/resources/simulation.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/simulation.txt` & `comet_toolbox-0.1.4/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/single_state.txt` & `comet_toolbox-0.1.4/src/comet/resources/single_state.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/img/badge.svg` & `comet_toolbox-0.1.4/src/comet/resources/img/badge.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/img/content.drawio` & `comet_toolbox-0.1.4/src/comet/resources/img/content.drawio`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/img/content.png` & `comet_toolbox-0.1.4/src/comet/resources/img/content.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/img/gui.png` & `comet_toolbox-0.1.4/src/comet/resources/img/gui.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/src/comet/resources/img/logo.png` & `comet_toolbox-0.1.4/src/comet/resources/img/logo.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_analysis.ipynb` & `comet_toolbox-0.1.4/tutorials/example_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_dfc.ipynb` & `comet_toolbox-0.1.4/tutorials/example_dfc.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_graph.ipynb` & `comet_toolbox-0.1.4/tutorials/example_graph.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_multiverse.ipynb` & `comet_toolbox-0.1.4/tutorials/example_multiverse.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_data/abide_50008.txt` & `comet_toolbox-0.1.4/tutorials/example_data/abide_50008.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_data/aomic_multi.pkl` & `comet_toolbox-0.1.4/tutorials/example_data/aomic_multi.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_data/simulation.txt` & `comet_toolbox-0.1.4/src/comet/resources/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/example_data/xcpd.tsv` & `comet_toolbox-0.1.4/tutorials/example_data/xcpd.tsv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_1.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_1.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_10.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_10.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_11.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_11.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_12.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_12.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_13.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_13.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_14.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_14.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_15.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_15.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_16.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_16.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_17.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_17.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_18.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_18.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_19.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_19.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_2.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_2.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_20.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_20.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_21.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_21.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_22.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_22.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_23.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_23.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_24.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_24.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_25.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_25.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_26.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_26.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_27.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_27.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_28.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_28.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_29.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_29.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_3.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_3.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_30.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_30.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_31.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_31.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_32.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_32.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_33.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_33.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_34.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_34.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_35.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_35.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_36.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_36.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_37.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_37.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_38.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_38.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_39.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_39.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_4.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_4.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_40.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_40.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_41.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_41.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_42.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_42.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_43.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_43.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_44.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_44.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_45.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_45.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_46.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_46.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_47.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_47.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_48.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_48.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_49.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_49.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_5.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_5.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_50.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_50.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_51.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_51.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_52.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_52.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_53.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_53.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_54.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_54.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_55.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_55.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_56.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_56.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_57.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_57.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_58.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_58.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_59.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_59.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_6.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_6.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_60.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_60.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_61.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_61.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_62.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_62.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_63.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_63.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_64.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_64.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_65.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_65.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_66.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_66.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_67.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_67.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_68.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_68.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_69.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_69.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_7.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_7.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_70.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_70.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_71.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_71.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_72.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_72.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_73.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_73.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_74.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_74.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_75.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_75.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_76.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_76.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_77.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_77.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_78.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_78.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_79.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_79.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_8.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_8.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_80.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_80.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_81.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_81.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_82.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_82.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_83.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_83.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_84.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_84.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_85.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_85.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_86.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_86.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_87.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_87.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_88.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_88.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_89.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_89.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_9.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_9.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_90.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_90.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_91.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_91.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_92.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_92.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_93.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_93.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_94.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_94.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_95.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_95.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/universe_96.py` & `comet_toolbox-0.1.4/tutorials/multiverse/universe_96.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/results/forking_paths.pkl` & `comet_toolbox-0.1.4/tutorials/multiverse/results/forking_paths.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.1.4/tutorials/multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/tutorials/multiverse/results/pipelines.csv` & `comet_toolbox-0.1.4/tutorials/multiverse/results/pipelines.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/.gitignore` & `comet_toolbox-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/LICENSE` & `comet_toolbox-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/README.md` & `comet_toolbox-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.1.2/pyproject.toml` & `comet_toolbox-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comet-toolbox"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   {name="Micha Burkhardt", email="micha.burkhardt@uol.de"},
 ]
 description = "Dynamic functional connectivity toolbox for multiverse analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `comet_toolbox-0.1.2/PKG-INFO` & `comet_toolbox-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: comet-toolbox
-Version: 0.1.2
+Version: 0.1.4
 Summary: Dynamic functional connectivity toolbox for multiverse analysis
 Project-URL: Homepage, https://github.com/mibur1/dfc-multiverse
 Project-URL: Issues, https://github.com/mibur1/dfc-multiverse/issues
 Author-email: Micha Burkhardt <micha.burkhardt@uol.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

