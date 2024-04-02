# Comparing `tmp/fluiddyn-0.6.0rc0.tar.gz` & `tmp/fluiddyn-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluiddyn-0.6.0rc0.tar", last modified: Sun Mar  3 15:51:59 2024, max compression
+gzip compressed data, was "fluiddyn-0.6.1.tar", last modified: Tue Apr  2 13:10:35 2024, max compression
```

## Comparing `fluiddyn-0.6.0rc0.tar` & `fluiddyn-0.6.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0      314 2024-01-17 17:19:22.652083 fluiddyn-0.6.0rc0/AUTHORS.md
--rw-r--r--   0        0        0    21394 2023-07-02 17:17:26.226859 fluiddyn-0.6.0rc0/LICENSE.txt
--rw-r--r--   0        0        0     5322 2024-01-17 17:19:22.652083 fluiddyn-0.6.0rc0/README.rst
--rw-r--r--   0        0        0     1136 2023-07-02 17:17:26.270860 fluiddyn-0.6.0rc0/fluiddoc/__init__.py
--rw-r--r--   0        0        0     4408 2024-01-18 13:32:59.118186 fluiddyn-0.6.0rc0/fluiddoc/fluiddocset.py
--rw-r--r--   0        0        0     2344 2023-07-02 17:17:26.274860 fluiddyn-0.6.0rc0/fluiddoc/fluidnbstripout.py
--rw-r--r--   0        0        0     3096 2023-07-13 14:34:07.250117 fluiddyn-0.6.0rc0/fluiddoc/ipynb_maker.py
--rw-r--r--   0        0        0     5174 2023-07-04 21:05:50.968703 fluiddyn-0.6.0rc0/fluiddoc/mathmacro.py
--rw-r--r--   0        0        0     1127 2023-07-13 14:34:07.250117 fluiddyn-0.6.0rc0/fluiddyn/__init__.py
--rw-r--r--   0        0        0      343 2024-02-17 22:55:31.959690 fluiddyn-0.6.0rc0/fluiddyn/_version.py
--rw-r--r--   0        0        0      144 2023-07-02 17:17:26.278860 fluiddyn-0.6.0rc0/fluiddyn/calcul/__init__.py
--rw-r--r--   0        0        0    18805 2023-07-04 21:05:50.972703 fluiddyn-0.6.0rc0/fluiddyn/calcul/easypyfft.py
--rw-r--r--   0        0        0     4223 2024-02-17 22:55:31.963691 fluiddyn-0.6.0rc0/fluiddyn/calcul/setofvariables.py
--rw-r--r--   0        0        0     5250 2024-02-17 22:55:31.963691 fluiddyn-0.6.0rc0/fluiddyn/calcul/signal.py
--rw-r--r--   0        0        0    24798 2024-02-17 22:55:31.963691 fluiddyn-0.6.0rc0/fluiddyn/calcul/sphericalharmo.py
--rw-r--r--   0        0        0        0 2023-07-02 17:17:26.282860 fluiddyn-0.6.0rc0/fluiddyn/calcul/test/__init__.py
--rw-r--r--   0        0        0     5783 2023-07-13 14:34:07.258117 fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_easypyfft.py
--rw-r--r--   0        0        0      330 2023-07-02 17:17:26.286860 fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_setofvariables.py
--rw-r--r--   0        0        0      660 2023-07-02 17:17:26.286860 fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_signal.py
--rw-r--r--   0        0        0      895 2023-07-13 14:34:07.258117 fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_sphericalharmo.py
--rw-r--r--   0        0        0     2887 2023-07-02 17:17:26.290860 fluiddyn-0.6.0rc0/fluiddyn/clusters/__init__.py
--rw-r--r--   0        0        0      875 2023-07-02 17:17:26.290860 fluiddyn-0.6.0rc0/fluiddyn/clusters/azzurra.py
--rw-r--r--   0        0        0      995 2024-02-17 22:55:31.967691 fluiddyn-0.6.0rc0/fluiddyn/clusters/ciment.py
--rw-r--r--   0        0        0     1274 2023-07-13 14:34:07.262117 fluiddyn-0.6.0rc0/fluiddyn/clusters/cines.py
--rw-r--r--   0        0        0      834 2023-07-02 17:17:26.294860 fluiddyn-0.6.0rc0/fluiddyn/clusters/idris.py
--rw-r--r--   0        0        0     1158 2024-02-17 22:55:31.967691 fluiddyn-0.6.0rc0/fluiddyn/clusters/legi.py
--rw-r--r--   0        0        0      716 2023-07-02 17:17:26.294860 fluiddyn-0.6.0rc0/fluiddyn/clusters/licallo.py
--rw-r--r--   0        0        0     8102 2023-07-13 14:34:07.262117 fluiddyn-0.6.0rc0/fluiddyn/clusters/local.py
--rw-r--r--   0        0        0     9408 2024-02-17 22:55:31.971691 fluiddyn-0.6.0rc0/fluiddyn/clusters/oar.py
--rw-r--r--   0        0        0     8351 2023-07-02 17:17:26.298860 fluiddyn-0.6.0rc0/fluiddyn/clusters/pbs.py
--rw-r--r--   0        0        0    16542 2023-07-13 14:34:07.270117 fluiddyn-0.6.0rc0/fluiddyn/clusters/slurm.py
--rw-r--r--   0        0        0     4178 2023-07-02 17:17:26.302860 fluiddyn-0.6.0rc0/fluiddyn/clusters/snic.py
--rw-r--r--   0        0        0        0 2023-07-02 17:17:26.302860 fluiddyn-0.6.0rc0/fluiddyn/clusters/test/__init__.py
--rw-r--r--   0        0        0     1026 2024-02-17 22:55:31.971691 fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_local.py
--rw-r--r--   0        0        0     2720 2024-02-17 22:55:31.971691 fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_oar.py
--rw-r--r--   0        0        0     2797 2024-02-17 22:55:31.975691 fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_pbs.py
--rw-r--r--   0        0        0     3479 2024-02-17 22:55:31.975691 fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_slurm_snic.py
--rw-r--r--   0        0        0     2100 2023-07-02 17:17:26.310860 fluiddyn-0.6.0rc0/fluiddyn/io/__init__.py
--rw-r--r--   0        0        0     5138 2024-02-17 22:55:31.975691 fluiddyn-0.6.0rc0/fluiddyn/io/binary.py
--rw-r--r--   0        0        0     3822 2024-02-17 22:55:31.975691 fluiddyn-0.6.0rc0/fluiddyn/io/dantec.py
--rw-r--r--   0        0        0     3779 2024-01-11 11:14:34.199987 fluiddyn-0.6.0rc0/fluiddyn/io/davis.py
--rw-r--r--   0        0        0    19554 2024-02-17 22:55:31.979691 fluiddyn-0.6.0rc0/fluiddyn/io/digiflow.py
--rw-r--r--   0        0        0     4052 2024-02-17 22:55:31.979691 fluiddyn-0.6.0rc0/fluiddyn/io/dump.py
--rw-r--r--   0        0        0     4758 2024-02-17 22:55:31.983692 fluiddyn-0.6.0rc0/fluiddyn/io/hdf5.py
--rw-r--r--   0        0        0     5683 2023-07-04 21:05:50.988703 fluiddyn-0.6.0rc0/fluiddyn/io/image.py
--rw-r--r--   0        0        0     1378 2023-07-02 17:17:26.318861 fluiddyn-0.6.0rc0/fluiddyn/io/in_py.py
--rw-r--r--   0        0        0    13149 2023-07-13 14:34:07.286118 fluiddyn-0.6.0rc0/fluiddyn/io/multitiff.py
--rw-r--r--   0        0        0     1762 2023-07-02 17:17:26.322861 fluiddyn-0.6.0rc0/fluiddyn/io/mycsv.py
--rw-r--r--   0        0        0    12165 2024-02-17 22:55:31.983692 fluiddyn-0.6.0rc0/fluiddyn/io/ns3d.py
--rw-r--r--   0        0        0     2539 2023-07-02 17:17:26.322861 fluiddyn-0.6.0rc0/fluiddyn/io/query.py
--rw-r--r--   0        0        0     2809 2023-07-04 21:05:50.992703 fluiddyn-0.6.0rc0/fluiddyn/io/rdvision.py
--rw-r--r--   0        0        0     1142 2024-02-17 22:55:31.983692 fluiddyn-0.6.0rc0/fluiddyn/io/redirect_stdout.py
--rw-r--r--   0        0        0      620 2023-07-02 17:17:26.326861 fluiddyn-0.6.0rc0/fluiddyn/io/tee.py
--rw-r--r--   0        0        0        0 2023-07-02 17:17:26.326861 fluiddyn-0.6.0rc0/fluiddyn/io/test/__init__.py
--rw-r--r--   0        0        0     2460 2023-07-02 17:17:26.330861 fluiddyn-0.6.0rc0/fluiddyn/io/test/ns3d_files/PV.t=0000.000
--rw-r--r--   0        0        0      284 2023-07-02 17:17:26.330861 fluiddyn-0.6.0rc0/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28
--rw-r--r--   0        0        0      284 2023-07-02 17:17:26.330861 fluiddyn-0.6.0rc0/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28_little-endian
--rw-r--r--   0        0        0      429 2023-07-02 17:17:26.330861 fluiddyn-0.6.0rc0/fluiddyn/io/test/rdvision_files/Dalsa2.seq
--rw-r--r--   0        0        0       48 2023-07-02 17:17:26.334861 fluiddyn-0.6.0rc0/fluiddyn/io/test/rdvision_files/Dalsa2.sqb
--rw-r--r--   0        0        0     1267 2023-07-02 17:17:26.334861 fluiddyn-0.6.0rc0/fluiddyn/io/test/rdvision_files/Dalsa2.xml
--rw-r--r--   0        0        0     1137 2023-07-02 17:17:26.334861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_binary.py
--rw-r--r--   0        0        0      525 2023-07-02 17:17:26.334861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_dantec.py
--rw-r--r--   0        0        0      660 2023-07-02 17:17:26.338861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_digiflow.py
--rw-r--r--   0        0        0     1456 2023-07-02 17:17:26.338861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_dump.py
--rw-r--r--   0        0        0     2123 2023-07-02 17:17:26.338861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_hdf5.py
--rw-r--r--   0        0        0     2909 2023-07-02 17:17:26.338861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_image.py
--rw-r--r--   0        0        0     1224 2023-07-02 17:17:26.342861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_in_py.py
--rw-r--r--   0        0        0     2411 2023-07-02 17:17:26.342861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_multitiff.py
--rw-r--r--   0        0        0      746 2023-07-02 17:17:26.342861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_mycsv.py
--rw-r--r--   0        0        0     1855 2023-07-02 17:17:26.346861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_ns3d.py
--rw-r--r--   0        0        0     1232 2023-07-13 14:34:07.286118 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_query.py
--rw-r--r--   0        0        0     1027 2023-07-02 17:17:26.346861 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_rdvision.py
--rw-r--r--   0        0        0      739 2023-07-04 21:05:50.996703 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_tee.py
--rw-r--r--   0        0        0     1095 2023-07-04 21:05:50.996703 fluiddyn-0.6.0rc0/fluiddyn/io/test/test_txt.py
--rw-r--r--   0        0        0     3342 2024-02-17 22:55:31.983692 fluiddyn-0.6.0rc0/fluiddyn/io/txt.py
--rw-r--r--   0        0        0      533 2023-07-13 14:34:07.290118 fluiddyn-0.6.0rc0/fluiddyn/output/__init__.py
--rw-r--r--   0        0        0     6098 2023-07-02 17:17:26.350861 fluiddyn-0.6.0rc0/fluiddyn/output/colorchart.py
--rw-r--r--   0        0        0     5323 2024-02-17 22:55:31.987692 fluiddyn-0.6.0rc0/fluiddyn/output/figs.py
--rw-r--r--   0        0        0     1177 2023-07-02 17:17:26.354861 fluiddyn-0.6.0rc0/fluiddyn/output/rcparams.py
--rw-r--r--   0        0        0        0 2023-07-02 17:17:26.354861 fluiddyn-0.6.0rc0/fluiddyn/output/test/__init__.py
--rw-r--r--   0        0        0      307 2023-07-02 17:17:26.354861 fluiddyn-0.6.0rc0/fluiddyn/output/test/test_colorchart.py
--rw-r--r--   0        0        0     1052 2023-07-13 14:34:07.290118 fluiddyn-0.6.0rc0/fluiddyn/output/test/test_figs.py
--rw-r--r--   0        0        0      721 2023-07-02 17:17:26.358861 fluiddyn-0.6.0rc0/fluiddyn/output/util.py
--rw-r--r--   0        0        0     1135 2023-07-13 14:34:07.294118 fluiddyn-0.6.0rc0/fluiddyn/util/__init__.py
--rw-r--r--   0        0        0      133 2023-07-02 17:17:26.358861 fluiddyn-0.6.0rc0/fluiddyn/util/compat.py
--rw-r--r--   0        0        0      304 2023-07-02 17:17:26.362861 fluiddyn-0.6.0rc0/fluiddyn/util/constants.py
--rw-r--r--   0        0        0     1068 2024-02-17 22:55:31.987692 fluiddyn-0.6.0rc0/fluiddyn/util/daemons.py
--rw-r--r--   0        0        0    15219 2024-02-17 22:55:31.987692 fluiddyn-0.6.0rc0/fluiddyn/util/info.py
--rw-r--r--   0        0        0     4282 2023-07-04 21:05:51.000703 fluiddyn-0.6.0rc0/fluiddyn/util/logger.py
--rw-r--r--   0        0        0     3513 2023-07-04 21:05:51.000703 fluiddyn-0.6.0rc0/fluiddyn/util/mail.py
--rw-r--r--   0        0        0     1971 2023-07-13 14:34:07.298118 fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/__init__.py
--rw-r--r--   0        0        0     5860 2024-02-17 22:55:31.991692 fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/cleanmat.py
--rw-r--r--   0        0        0     3238 2024-02-17 22:55:31.991692 fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/mat2wrongpy.py
--rw-r--r--   0        0        0        0 2023-07-02 17:17:26.370862 fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/test/__init__.py
--rw-r--r--   0        0        0      810 2023-07-02 17:17:26.370862 fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/test/courant.m
--rw-r--r--   0        0        0      519 2023-07-02 17:17:26.370862 fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/test/test_matlab2py.py
--rw-r--r--   0        0        0     3780 2023-07-02 17:17:26.374862 fluiddyn-0.6.0rc0/fluiddyn/util/mpi.py
--rw-r--r--   0        0        0    23542 2024-02-17 22:55:31.991692 fluiddyn-0.6.0rc0/fluiddyn/util/numpy_distutils_cpuinfo.py
--rw-r--r--   0        0        0      964 2024-02-17 22:55:31.995692 fluiddyn-0.6.0rc0/fluiddyn/util/opencv.py
--rw-r--r--   0        0        0    23221 2024-01-18 13:32:59.122186 fluiddyn-0.6.0rc0/fluiddyn/util/paramcontainer.py
--rw-r--r--   0        0        0     7281 2024-01-18 13:32:59.122186 fluiddyn-0.6.0rc0/fluiddyn/util/paramcontainer_gui.py
--rw-r--r--   0        0        0    30269 2024-03-03 15:51:07.300395 fluiddyn-0.6.0rc0/fluiddyn/util/serieofarrays.py
--rw-r--r--   0        0        0     4724 2023-07-02 17:17:26.378862 fluiddyn-0.6.0rc0/fluiddyn/util/terminal_colors.py
--rw-r--r--   0        0        0        0 2023-07-02 17:17:26.382862 fluiddyn-0.6.0rc0/fluiddyn/util/test/__init__.py
--rw-r--r--   0        0        0     1814 2023-07-02 17:17:26.382862 fluiddyn-0.6.0rc0/fluiddyn/util/test/file.xml
--rw-r--r--   0        0        0      808 2023-07-02 17:17:26.382862 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_daemons.py
--rw-r--r--   0        0        0      974 2024-02-17 22:55:31.999692 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_info.py
--rw-r--r--   0        0        0      942 2024-01-18 13:32:59.126186 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_logger.py
--rw-r--r--   0        0        0     2194 2023-07-13 14:34:07.306118 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_mpi.py
--rw-r--r--   0        0        0     4725 2023-07-13 14:34:07.306118 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_paramcontainer.py
--rw-r--r--   0        0        0     6484 2024-03-03 15:51:07.304395 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_serieofarrays.py
--rw-r--r--   0        0        0      797 2023-07-02 17:17:26.390862 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_timer.py
--rw-r--r--   0        0        0     2734 2023-07-13 14:34:07.310118 fluiddyn-0.6.0rc0/fluiddyn/util/test/test_util.py
--rw-r--r--   0        0        0     4522 2023-07-04 21:05:51.016703 fluiddyn-0.6.0rc0/fluiddyn/util/timer.py
--rw-r--r--   0        0        0     1200 2023-07-02 17:17:26.394862 fluiddyn-0.6.0rc0/fluiddyn/util/userconfig.py
--rw-r--r--   0        0        0     9277 2024-02-17 22:55:31.999692 fluiddyn-0.6.0rc0/fluiddyn/util/util.py
--rw-r--r--   0        0        0     4443 2023-07-04 21:05:51.016703 fluiddyn-0.6.0rc0/fluiddyn/util/xmltotext.py
--rw-r--r--   0        0        0     4231 2024-03-03 15:51:59.418620 fluiddyn-0.6.0rc0/pyproject.toml
--rw-r--r--   0        0        0     7117 1970-01-01 00:00:00.000000 fluiddyn-0.6.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      314 2024-02-17 22:43:56.129004 fluiddyn-0.6.1/AUTHORS.md
+-rw-r--r--   0        0        0    21394 2024-02-17 22:43:56.129004 fluiddyn-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     5322 2024-02-17 22:43:56.133004 fluiddyn-0.6.1/README.rst
+-rw-r--r--   0        0        0     1136 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/__init__.py
+-rw-r--r--   0        0        0     4408 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/fluiddocset.py
+-rw-r--r--   0        0        0     2344 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/fluidnbstripout.py
+-rw-r--r--   0        0        0     3096 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/ipynb_maker.py
+-rw-r--r--   0        0        0     5174 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/mathmacro.py
+-rw-r--r--   0        0        0     1127 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddyn/__init__.py
+-rw-r--r--   0        0        0      343 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/_version.py
+-rw-r--r--   0        0        0      144 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/__init__.py
+-rw-r--r--   0        0        0    18805 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/easypyfft.py
+-rw-r--r--   0        0        0     4223 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/setofvariables.py
+-rw-r--r--   0        0        0     5250 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/signal.py
+-rw-r--r--   0        0        0    24798 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/sphericalharmo.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/__init__.py
+-rw-r--r--   0        0        0     5783 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_easypyfft.py
+-rw-r--r--   0        0        0      330 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_setofvariables.py
+-rw-r--r--   0        0        0      660 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_signal.py
+-rw-r--r--   0        0        0      895 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_sphericalharmo.py
+-rw-r--r--   0        0        0     2887 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/__init__.py
+-rw-r--r--   0        0        0      875 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/azzurra.py
+-rw-r--r--   0        0        0      995 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/ciment.py
+-rw-r--r--   0        0        0     1274 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/cines.py
+-rw-r--r--   0        0        0      834 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/idris.py
+-rw-r--r--   0        0        0     1045 2024-03-26 14:13:20.514828 fluiddyn-0.6.1/fluiddyn/clusters/legi.py
+-rw-r--r--   0        0        0      716 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/licallo.py
+-rw-r--r--   0        0        0     8102 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/local.py
+-rw-r--r--   0        0        0     9408 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/oar.py
+-rw-r--r--   0        0        0     8351 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/pbs.py
+-rw-r--r--   0        0        0    16542 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/slurm.py
+-rw-r--r--   0        0        0     4178 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/snic.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/test/__init__.py
+-rw-r--r--   0        0        0     1026 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/test/test_local.py
+-rw-r--r--   0        0        0     2865 2024-03-26 14:13:20.514828 fluiddyn-0.6.1/fluiddyn/clusters/test/test_oar.py
+-rw-r--r--   0        0        0     2797 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/clusters/test/test_pbs.py
+-rw-r--r--   0        0        0     3479 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/clusters/test/test_slurm_snic.py
+-rw-r--r--   0        0        0     2115 2024-03-20 15:24:08.394333 fluiddyn-0.6.1/fluiddyn/io/__init__.py
+-rw-r--r--   0        0        0     5138 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/io/binary.py
+-rw-r--r--   0        0        0     3822 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/io/dantec.py
+-rw-r--r--   0        0        0     3779 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/davis.py
+-rw-r--r--   0        0        0    19554 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/digiflow.py
+-rw-r--r--   0        0        0     4052 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/dump.py
+-rw-r--r--   0        0        0     4758 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/hdf5.py
+-rw-r--r--   0        0        0     5683 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/image.py
+-rw-r--r--   0        0        0     1378 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/in_py.py
+-rw-r--r--   0        0        0    13149 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/multitiff.py
+-rw-r--r--   0        0        0     1762 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/mycsv.py
+-rw-r--r--   0        0        0    12165 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/ns3d.py
+-rw-r--r--   0        0        0     2539 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/query.py
+-rw-r--r--   0        0        0     2809 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/rdvision.py
+-rw-r--r--   0        0        0     1142 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/redirect_stdout.py
+-rw-r--r--   0        0        0      620 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/tee.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/test/__init__.py
+-rw-r--r--   0        0        0     2460 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/PV.t=0000.000
+-rw-r--r--   0        0        0      284 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28
+-rw-r--r--   0        0        0      284 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28_little-endian
+-rw-r--r--   0        0        0      429 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.seq
+-rw-r--r--   0        0        0       48 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.sqb
+-rw-r--r--   0        0        0     1267 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.xml
+-rw-r--r--   0        0        0     1137 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/test_binary.py
+-rw-r--r--   0        0        0      525 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_dantec.py
+-rw-r--r--   0        0        0      660 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_digiflow.py
+-rw-r--r--   0        0        0     1456 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_dump.py
+-rw-r--r--   0        0        0     2123 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_hdf5.py
+-rw-r--r--   0        0        0     2909 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_image.py
+-rw-r--r--   0        0        0     1224 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_in_py.py
+-rw-r--r--   0        0        0     2411 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_multitiff.py
+-rw-r--r--   0        0        0      746 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_mycsv.py
+-rw-r--r--   0        0        0     1855 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_ns3d.py
+-rw-r--r--   0        0        0     1232 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_query.py
+-rw-r--r--   0        0        0     1027 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_rdvision.py
+-rw-r--r--   0        0        0      739 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_tee.py
+-rw-r--r--   0        0        0     1095 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/io/test/test_txt.py
+-rw-r--r--   0        0        0     3342 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/io/txt.py
+-rw-r--r--   0        0        0      533 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/output/__init__.py
+-rw-r--r--   0        0        0     6098 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/output/colorchart.py
+-rw-r--r--   0        0        0     5323 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/output/figs.py
+-rw-r--r--   0        0        0     1177 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/rcparams.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/test/__init__.py
+-rw-r--r--   0        0        0      307 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/test/test_colorchart.py
+-rw-r--r--   0        0        0     1052 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/test/test_figs.py
+-rw-r--r--   0        0        0      721 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/util.py
+-rw-r--r--   0        0        0     1135 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/util/__init__.py
+-rw-r--r--   0        0        0      133 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/util/compat.py
+-rw-r--r--   0        0        0      304 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/constants.py
+-rw-r--r--   0        0        0     1068 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/daemons.py
+-rw-r--r--   0        0        0    15219 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/info.py
+-rw-r--r--   0        0        0     4282 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/logger.py
+-rw-r--r--   0        0        0     3513 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/mail.py
+-rw-r--r--   0        0        0     1971 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/__init__.py
+-rw-r--r--   0        0        0     5860 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/cleanmat.py
+-rw-r--r--   0        0        0     3238 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/mat2wrongpy.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/__init__.py
+-rw-r--r--   0        0        0      810 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/courant.m
+-rw-r--r--   0        0        0      519 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/test_matlab2py.py
+-rw-r--r--   0        0        0     3780 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/mpi.py
+-rw-r--r--   0        0        0    23542 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/numpy_distutils_cpuinfo.py
+-rw-r--r--   0        0        0      964 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/opencv.py
+-rw-r--r--   0        0        0    23221 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/paramcontainer.py
+-rw-r--r--   0        0        0     7281 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/paramcontainer_gui.py
+-rw-r--r--   0        0        0    30269 2024-03-03 14:18:58.297248 fluiddyn-0.6.1/fluiddyn/util/serieofarrays.py
+-rw-r--r--   0        0        0     4724 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/terminal_colors.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/test/__init__.py
+-rw-r--r--   0        0        0     1814 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/file.xml
+-rw-r--r--   0        0        0      808 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_daemons.py
+-rw-r--r--   0        0        0      974 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_info.py
+-rw-r--r--   0        0        0      942 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_logger.py
+-rw-r--r--   0        0        0     2194 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_mpi.py
+-rw-r--r--   0        0        0     4725 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/test/test_paramcontainer.py
+-rw-r--r--   0        0        0     6484 2024-03-03 14:18:58.297248 fluiddyn-0.6.1/fluiddyn/util/test/test_serieofarrays.py
+-rw-r--r--   0        0        0      797 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/test/test_timer.py
+-rw-r--r--   0        0        0     2734 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/test/test_util.py
+-rw-r--r--   0        0        0     4522 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/timer.py
+-rw-r--r--   0        0        0     1200 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/userconfig.py
+-rw-r--r--   0        0        0     9277 2024-02-17 22:43:56.245002 fluiddyn-0.6.1/fluiddyn/util/util.py
+-rw-r--r--   0        0        0     4443 2024-02-17 22:43:56.245002 fluiddyn-0.6.1/fluiddyn/util/xmltotext.py
+-rw-r--r--   0        0        0     4238 2024-04-02 13:10:35.881428 fluiddyn-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7114 1970-01-01 00:00:00.000000 fluiddyn-0.6.1/PKG-INFO
```

### Comparing `fluiddyn-0.6.0rc0/LICENSE.txt` & `fluiddyn-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/README.rst` & `fluiddyn-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddoc/__init__.py` & `fluiddyn-0.6.1/fluiddoc/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddoc/fluiddocset.py` & `fluiddyn-0.6.1/fluiddoc/fluiddocset.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddoc/fluidnbstripout.py` & `fluiddyn-0.6.1/fluiddoc/fluidnbstripout.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddoc/ipynb_maker.py` & `fluiddyn-0.6.1/fluiddoc/ipynb_maker.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddoc/mathmacro.py` & `fluiddyn-0.6.1/fluiddoc/mathmacro.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/__init__.py` & `fluiddyn-0.6.1/fluiddyn/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/easypyfft.py` & `fluiddyn-0.6.1/fluiddyn/calcul/easypyfft.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/setofvariables.py` & `fluiddyn-0.6.1/fluiddyn/calcul/setofvariables.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/signal.py` & `fluiddyn-0.6.1/fluiddyn/calcul/signal.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/sphericalharmo.py` & `fluiddyn-0.6.1/fluiddyn/calcul/sphericalharmo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_easypyfft.py` & `fluiddyn-0.6.1/fluiddyn/calcul/test/test_easypyfft.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_signal.py` & `fluiddyn-0.6.1/fluiddyn/calcul/test/test_signal.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/calcul/test/test_sphericalharmo.py` & `fluiddyn-0.6.1/fluiddyn/calcul/test/test_sphericalharmo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/__init__.py` & `fluiddyn-0.6.1/fluiddyn/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/azzurra.py` & `fluiddyn-0.6.1/fluiddyn/clusters/azzurra.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/ciment.py` & `fluiddyn-0.6.1/fluiddyn/clusters/ciment.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/cines.py` & `fluiddyn-0.6.1/fluiddyn/clusters/cines.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/idris.py` & `fluiddyn-0.6.1/fluiddyn/clusters/idris.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/licallo.py` & `fluiddyn-0.6.1/fluiddyn/clusters/licallo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/local.py` & `fluiddyn-0.6.1/fluiddyn/clusters/local.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/oar.py` & `fluiddyn-0.6.1/fluiddyn/clusters/oar.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/pbs.py` & `fluiddyn-0.6.1/fluiddyn/clusters/pbs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/slurm.py` & `fluiddyn-0.6.1/fluiddyn/clusters/slurm.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/snic.py` & `fluiddyn-0.6.1/fluiddyn/clusters/snic.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_local.py` & `fluiddyn-0.6.1/fluiddyn/clusters/test/test_local.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_oar.py` & `fluiddyn-0.6.1/fluiddyn/clusters/test/test_oar.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import subprocess
 import unittest
 from shutil import rmtree
 
 from ...io import stdout_redirected
 from ..ciment import Froggy
-from ..legi import Calcul, Calcul3, Calcul7, Calcul8, Calcul9
+from ..legi import GPU9, Calcul, Calcul2, Calcul6, Calcul7, Calcul8
 from ..oar import ClusterOAR
 
 path_test = "tmp_test"
 
 try:
     subprocess.check_call(["oarsub", "--version"], stdout=subprocess.PIPE)
     oar = True
@@ -30,30 +30,34 @@
         pass
 
 
 class CalculNoCheck(ClusterNoCheck, Calcul):
     pass
 
 
-class Calcul3NoCheck(ClusterNoCheck, Calcul3):
+class Calcul2NoCheck(ClusterNoCheck, Calcul2):
     pass
 
 
-class Calcul9NoCheck(ClusterNoCheck, Calcul9):
+class Calcul6NoCheck(ClusterNoCheck, Calcul6):
     pass
 
 
 class Calcul7NoCheck(ClusterNoCheck, Calcul7):
     pass
 
 
 class Calcul8NoCheck(ClusterNoCheck, Calcul8):
     pass
 
 
+class GPU9NoCheck(ClusterNoCheck, GPU9):
+    pass
+
+
 class FroggyNoCheck(ClusterNoCheck, Froggy):
     pass
 
 
 @unittest.skipUnless(os.name == "posix", "requires POSIX")
 class TestCaseOAR(unittest.TestCase):
     Cluster = ClusterOAR
@@ -94,32 +98,37 @@
 
 
 class TestCaseCalcul(TestCaseOAR):
     Cluster = Calcul
     ClusterNoCheck = CalculNoCheck
 
 
-class TestCaseCalcul3(TestCaseOAR):
-    Cluster = Calcul3
-    ClusterNoCheck = Calcul3NoCheck
-
-
-class TestCaseCalcul9(TestCaseOAR):
-    Cluster = Calcul9
-    ClusterNoCheck = Calcul3NoCheck
-
-
 class TestCaseCalcul7(TestCaseOAR):
     Cluster = Calcul7
-    ClusterNoCheck = Calcul3NoCheck
+    ClusterNoCheck = Calcul7NoCheck
 
 
 class TestCaseCalcul8(TestCaseOAR):
     Cluster = Calcul8
-    ClusterNoCheck = Calcul3NoCheck
+    ClusterNoCheck = Calcul8NoCheck
+
+
+class TestCaseCalcul2(TestCaseOAR):
+    Cluster = Calcul2
+    ClusterNoCheck = Calcul2NoCheck
+
+
+class TestCaseCalcul6(TestCaseOAR):
+    Cluster = Calcul6
+    ClusterNoCheck = Calcul6NoCheck
+
+
+class TestCaseGPU9(TestCaseOAR):
+    Cluster = GPU9
+    ClusterNoCheck = GPU9NoCheck
 
 
 class TestCaseFroggy(TestCaseOAR):
     Cluster = Froggy
     ClusterNoCheck = FroggyNoCheck
```

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_pbs.py` & `fluiddyn-0.6.1/fluiddyn/clusters/test/test_pbs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/clusters/test/test_slurm_snic.py` & `fluiddyn-0.6.1/fluiddyn/clusters/test/test_slurm_snic.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/__init__.py` & `fluiddyn-0.6.1/fluiddyn/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 FLUIDDYN_PATH_WARNING = os.environ.get("FLUIDDYN_PATH_WARNING")
 if FLUIDDYN_PATH_WARNING is None:
     FLUIDDYN_PATH_WARNING = str(HOME_DIR / ".fluiddyn")
 
 
 if not os.path.exists(FLUIDDYN_PATH_WARNING):
-    os.makedirs(FLUIDDYN_PATH_WARNING)
+    os.makedirs(FLUIDDYN_PATH_WARNING, exist_ok=True)
 
 
 def _write_warning(*args, **kargs):
     if "end" in kargs:
         end = kargs["end"]
     else:
         end = "\n"
```

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/binary.py` & `fluiddyn-0.6.1/fluiddyn/io/binary.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/dantec.py` & `fluiddyn-0.6.1/fluiddyn/io/dantec.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/davis.py` & `fluiddyn-0.6.1/fluiddyn/io/davis.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/digiflow.py` & `fluiddyn-0.6.1/fluiddyn/io/digiflow.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/dump.py` & `fluiddyn-0.6.1/fluiddyn/io/dump.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/hdf5.py` & `fluiddyn-0.6.1/fluiddyn/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/image.py` & `fluiddyn-0.6.1/fluiddyn/io/image.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/in_py.py` & `fluiddyn-0.6.1/fluiddyn/io/in_py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/multitiff.py` & `fluiddyn-0.6.1/fluiddyn/io/multitiff.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/mycsv.py` & `fluiddyn-0.6.1/fluiddyn/io/mycsv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/ns3d.py` & `fluiddyn-0.6.1/fluiddyn/io/ns3d.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/query.py` & `fluiddyn-0.6.1/fluiddyn/io/query.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/rdvision.py` & `fluiddyn-0.6.1/fluiddyn/io/rdvision.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/redirect_stdout.py` & `fluiddyn-0.6.1/fluiddyn/io/redirect_stdout.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/tee.py` & `fluiddyn-0.6.1/fluiddyn/io/tee.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/ns3d_files/PV.t=0000.000` & `fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/PV.t=0000.000`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/rdvision_files/Dalsa2.xml` & `fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.xml`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_binary.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_binary.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_dantec.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_dantec.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_digiflow.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_digiflow.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_dump.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_hdf5.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_image.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_image.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_in_py.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_in_py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_multitiff.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_multitiff.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_mycsv.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_mycsv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_ns3d.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_ns3d.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_query.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_query.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_rdvision.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_rdvision.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_tee.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_tee.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/test/test_txt.py` & `fluiddyn-0.6.1/fluiddyn/io/test/test_txt.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/io/txt.py` & `fluiddyn-0.6.1/fluiddyn/io/txt.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/output/__init__.py` & `fluiddyn-0.6.1/fluiddyn/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/output/colorchart.py` & `fluiddyn-0.6.1/fluiddyn/output/colorchart.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/output/figs.py` & `fluiddyn-0.6.1/fluiddyn/output/figs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/output/rcparams.py` & `fluiddyn-0.6.1/fluiddyn/output/rcparams.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/output/test/test_figs.py` & `fluiddyn-0.6.1/fluiddyn/output/test/test_figs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/output/util.py` & `fluiddyn-0.6.1/fluiddyn/output/util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/__init__.py` & `fluiddyn-0.6.1/fluiddyn/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/daemons.py` & `fluiddyn-0.6.1/fluiddyn/util/daemons.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/info.py` & `fluiddyn-0.6.1/fluiddyn/util/info.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/logger.py` & `fluiddyn-0.6.1/fluiddyn/util/logger.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/mail.py` & `fluiddyn-0.6.1/fluiddyn/util/mail.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/__init__.py` & `fluiddyn-0.6.1/fluiddyn/util/matlab2py/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/cleanmat.py` & `fluiddyn-0.6.1/fluiddyn/util/matlab2py/cleanmat.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/mat2wrongpy.py` & `fluiddyn-0.6.1/fluiddyn/util/matlab2py/mat2wrongpy.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/test/courant.m` & `fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/courant.m`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/matlab2py/test/test_matlab2py.py` & `fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/test_matlab2py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/mpi.py` & `fluiddyn-0.6.1/fluiddyn/util/mpi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/numpy_distutils_cpuinfo.py` & `fluiddyn-0.6.1/fluiddyn/util/numpy_distutils_cpuinfo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/opencv.py` & `fluiddyn-0.6.1/fluiddyn/util/opencv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/paramcontainer.py` & `fluiddyn-0.6.1/fluiddyn/util/paramcontainer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/paramcontainer_gui.py` & `fluiddyn-0.6.1/fluiddyn/util/paramcontainer_gui.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/serieofarrays.py` & `fluiddyn-0.6.1/fluiddyn/util/serieofarrays.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/terminal_colors.py` & `fluiddyn-0.6.1/fluiddyn/util/terminal_colors.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/file.xml` & `fluiddyn-0.6.1/fluiddyn/util/test/file.xml`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_daemons.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_daemons.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_info.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_info.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_logger.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_mpi.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_mpi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_paramcontainer.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_paramcontainer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_serieofarrays.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_serieofarrays.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_timer.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_timer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/test/test_util.py` & `fluiddyn-0.6.1/fluiddyn/util/test/test_util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/timer.py` & `fluiddyn-0.6.1/fluiddyn/util/timer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/userconfig.py` & `fluiddyn-0.6.1/fluiddyn/util/userconfig.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/util.py` & `fluiddyn-0.6.1/fluiddyn/util/util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/fluiddyn/util/xmltotext.py` & `fluiddyn-0.6.1/fluiddyn/util/xmltotext.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.0rc0/pyproject.toml` & `fluiddyn-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "fluiddyn"
-version = "0.6.0rc0"
+version = "0.6.1"
 description = "Framework for studying fluid dynamics."
 keywords = [
     "Fluid dynamics",
     "research",
 ]
 authors = [
     { name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr" },
@@ -187,8 +187,8 @@
 ]
 multi_line_output = 3
 skip_glob = [
     ".pixi/*",
 ]
 
 [tool.pytest.ini_options]
-pdbcls = "IPython.terminal.debugger:TerminalPdb"
+addopts = "--pdbcls=IPython.terminal.debugger:TerminalPdb"
```

### Comparing `fluiddyn-0.6.0rc0/PKG-INFO` & `fluiddyn-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluiddyn
-Version: 0.6.0rc0
+Version: 0.6.1
 Summary: Framework for studying fluid dynamics.
 Keywords: Fluid dynamics research
 Home-page: https://foss.heptapod.net/fluiddyn/fluiddyn
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL-B License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

