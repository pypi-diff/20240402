# Comparing `tmp/not1mm-24.4.1.tar.gz` & `tmp/not1mm-24.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-24.4.1.tar", last modified: Mon Apr  1 18:22:06 2024, max compression
+gzip compressed data, was "not1mm-24.4.1.1.tar", last modified: Tue Apr  2 00:11:29 2024, max compression
```

## Comparing `not1mm-24.4.1.tar` & `not1mm-24.4.1.1.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.252732 not1mm-24.4.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26174 2024-04-01 18:22:06.251732 not1mm-24.4.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25130 2024-04-01 18:21:32.000000 not1mm-24.4.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.165731 not1mm-24.4.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   118379 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33404 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/bandmap.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7604 2024-04-01 18:14:52.000000 not1mm-24.4.1/not1mm/checkwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.194731 not1mm-24.4.1/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2912 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/checkwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4783134 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54070 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.226732 not1mm-24.4.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/radio_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/ssbmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2405 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/data/vfo.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/fsutils.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.235732 not1mm-24.4.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1964 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13775 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3196 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      350 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/plugin_common.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/super_check_partial.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-01 18:16:50.000000 not1mm-24.4.1/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    43830 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.249732 not1mm-24.4.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10834 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10840 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10848 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10851 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13643 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_10m.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13688 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13691 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10026 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7974 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13143 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13149 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12438 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_vhf_jan.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11457 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_vhf_jun.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11457 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/arrl_vhf_sep.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11869 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14018 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cq_160_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14061 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cq_160_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12378 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12466 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11083 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11088 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11976 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3369 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11433 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/iaru_hf.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11049 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11051 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11472 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/naqp_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11477 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/naqp_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12278 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/phone_weekly_test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10546 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/stew_perry_topband.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10212 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/plugins/winter_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11530 2024-03-31 16:17:00.000000 not1mm-24.4.1/not1mm/vfo.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-01 18:22:06.250732 not1mm-24.4.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26174 2024-04-01 18:22:06.000000 not1mm-24.4.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4053 2024-04-01 18:22:06.000000 not1mm-24.4.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-01 18:22:06.000000 not1mm-24.4.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-01 18:22:06.000000 not1mm-24.4.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      119 2024-04-01 18:22:06.000000 not1mm-24.4.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-01 18:22:06.000000 not1mm-24.4.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1406 2024-04-01 18:16:50.000000 not1mm-24.4.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-01 18:22:06.252732 not1mm-24.4.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.474084 not1mm-24.4.1.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26390 2024-04-02 00:11:29.473084 not1mm-24.4.1.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25317 2024-04-02 00:07:39.000000 not1mm-24.4.1.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.373083 not1mm-24.4.1.1/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   117984 2024-04-02 00:01:11.000000 not1mm-24.4.1.1/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33404 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/bandmap.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     9657 2024-04-01 22:45:02.000000 not1mm-24.4.1.1/not1mm/checkwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.406083 not1mm-24.4.1.1/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4611 2024-04-01 22:19:43.000000 not1mm-24.4.1.1/not1mm/data/checkwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4783134 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.1.1/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/logwindowx.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54070 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.442084 not1mm-24.4.1.1/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/radio_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/data/ssbmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1413 2024-04-01 22:52:50.000000 not1mm-24.4.1.1/not1mm/data/vfo.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/fsutils.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.456084 not1mm-24.4.1.1/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1964 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13775 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3196 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      350 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/plugin_common.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/super_check_partial.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2024-04-01 21:45:39.000000 not1mm-24.4.1.1/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    43864 2024-04-01 23:58:18.000000 not1mm-24.4.1.1/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.472084 not1mm-24.4.1.1/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10834 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10840 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10848 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10851 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13643 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_10m.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13688 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13691 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10026 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7974 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13143 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13149 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12438 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_vhf_jan.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11457 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_vhf_jun.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11457 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/arrl_vhf_sep.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11869 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14018 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cq_160_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14061 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cq_160_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12378 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12466 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11083 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11088 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11976 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3369 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11433 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/iaru_hf.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11049 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11051 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11472 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/naqp_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11477 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/naqp_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12278 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/phone_weekly_test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10546 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/stew_perry_topband.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10212 2024-03-31 16:17:00.000000 not1mm-24.4.1.1/not1mm/plugins/winter_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11547 2024-04-01 22:45:06.000000 not1mm-24.4.1.1/not1mm/vfo.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-02 00:11:29.472084 not1mm-24.4.1.1/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26390 2024-04-02 00:11:29.000000 not1mm-24.4.1.1/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4079 2024-04-02 00:11:29.000000 not1mm-24.4.1.1/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-02 00:11:29.000000 not1mm-24.4.1.1/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-02 00:11:29.000000 not1mm-24.4.1.1/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-02 00:11:29.000000 not1mm-24.4.1.1/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-02 00:11:29.000000 not1mm-24.4.1.1/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1427 2024-04-01 21:45:39.000000 not1mm-24.4.1.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-02 00:11:29.474084 not1mm-24.4.1.1/setup.cfg
```

### Comparing `not1mm-24.4.1/LICENSE` & `not1mm-24.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/PKG-INFO` & `not1mm-24.4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.1
+Version: 24.4.1.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -24,14 +24,15 @@
 Requires-Dist: pyserial
 Requires-Dist: sounddevice
 Requires-Dist: soundfile
 Requires-Dist: numpy
 Requires-Dist: notctyparser>=23.6.21
 Requires-Dist: rapidfuzz
 Requires-Dist: appdata
+Requires-Dist: Levenshtein
 
 # Not1MM
 
 The worlds #1 unfinished contest logger <sup>*According to my daughter Corinna.<sup>
 
 [![PyPI](https://img.shields.io/pypi/v/not1mm)](https://pypi.org/project/not1mm/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
@@ -172,14 +173,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-1-1] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets.
 - [24-4-1] Removed some un-needed loops and widgets from the check window.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Flatpak
 
 I've tried for a couple days to get not1mm to build as a flatpak. I've failed.
```

### Comparing `not1mm-24.4.1/README.md` & `not1mm-24.4.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-1-1] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets.
 - [24-4-1] Removed some un-needed loops and widgets from the check window.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Flatpak
 
 I've tried for a couple days to get not1mm to build as a flatpak. I've failed.
```

### Comparing `not1mm-24.4.1/not1mm/__main__.py` & `not1mm-24.4.1.1/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3071,4329 +3071,4304 @@
 0000bfe0: 290a 0a20 2020 2064 6566 206c 6175 6e63  )..    def launc
 0000bff0: 685f 6c6f 675f 7769 6e64 6f77 2873 656c  h_log_window(sel
 0000c000: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
 0000c010: 2020 2020 2222 224c 6175 6e63 6820 7468      """Launch th
 0000c020: 6520 6c6f 6720 7769 6e64 6f77 2222 220a  e log window""".
 0000c030: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
 0000c040: 656c 662e 6c6f 675f 7769 6e64 6f77 3a0a  elf.log_window:.
-0000c050: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-0000c060: 7769 6467 6574 203d 204c 6f67 5769 6e64  widget = LogWind
-0000c070: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
-0000c080: 2073 656c 662e 6c6f 675f 7769 6e64 6f77   self.log_window
-0000c090: 203d 2051 446f 636b 5769 6467 6574 286c   = QDockWidget(l
-0000c0a0: 6f67 5f77 6964 6765 742e 7072 6f70 6572  og_widget.proper
-0000c0b0: 7479 2822 7769 6e64 6f77 5469 746c 6522  ty("windowTitle"
-0000c0c0: 292c 2073 656c 6629 0a20 2020 2020 2020  ), self).       
-0000c0d0: 2020 2020 2073 656c 662e 6c6f 675f 7769       self.log_wi
-0000c0e0: 6e64 6f77 2e73 6574 5769 6467 6574 286c  ndow.setWidget(l
-0000c0f0: 6f67 5f77 6964 6765 7429 0a20 2020 2020  og_widget).     
-0000c100: 2020 2020 2020 2073 656c 662e 6164 6444         self.addD
-0000c110: 6f63 6b57 6964 6765 7428 5174 2e42 6f74  ockWidget(Qt.Bot
-0000c120: 746f 6d44 6f63 6b57 6964 6765 7441 7265  tomDockWidgetAre
-0000c130: 612c 2073 656c 662e 6c6f 675f 7769 6e64  a, self.log_wind
-0000c140: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
-0000c150: 2e6c 6f67 5f77 696e 646f 772e 7368 6f77  .log_window.show
-0000c160: 2829 0a0a 2020 2020 6465 6620 6c61 756e  ()..    def laun
-0000c170: 6368 5f62 616e 646d 6170 5f77 696e 646f  ch_bandmap_windo
-0000c180: 7728 7365 6c66 2920 2d3e 204e 6f6e 653a  w(self) -> None:
-0000c190: 0a20 2020 2020 2020 2022 2222 4c61 756e  .        """Laun
-0000c1a0: 6368 2074 6865 2062 616e 646d 6170 2077  ch the bandmap w
-0000c1b0: 696e 646f 7722 2222 0a20 2020 2020 2020  indow""".       
-0000c1c0: 2069 6620 6e6f 7420 7365 6c66 2e62 616e   if not self.ban
-0000c1d0: 646d 6170 5f77 696e 646f 773a 0a20 2020  dmap_window:.   
-0000c1e0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-0000c1f0: 6e64 6d61 705f 7769 6e64 6f77 203d 2042  ndmap_window = B
-0000c200: 616e 644d 6170 5769 6e64 6f77 2829 0a20  andMapWindow(). 
-0000c210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c220: 6164 6444 6f63 6b57 6964 6765 7428 5174  addDockWidget(Qt
-0000c230: 2e52 6967 6874 446f 636b 5769 6467 6574  .RightDockWidget
-0000c240: 4172 6561 2c20 7365 6c66 2e62 616e 646d  Area, self.bandm
-0000c250: 6170 5f77 696e 646f 7729 0a20 2020 2020  ap_window).     
-0000c260: 2020 2073 656c 662e 6261 6e64 6d61 705f     self.bandmap_
-0000c270: 7769 6e64 6f77 2e73 686f 7728 290a 0a20  window.show().. 
-0000c280: 2020 2064 6566 206c 6175 6e63 685f 6368     def launch_ch
-0000c290: 6563 6b5f 7769 6e64 6f77 2873 656c 6629  eck_window(self)
-0000c2a0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000c2b0: 2020 2222 224c 6175 6e63 6820 7468 6520    """Launch the 
-0000c2c0: 6368 6563 6b20 7769 6e64 6f77 2222 220a  check window""".
-0000c2d0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000c2e0: 656c 662e 6368 6563 6b5f 7769 6e64 6f77  elf.check_window
-0000c2f0: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-0000c300: 6563 6b5f 7769 6467 6574 203d 2043 6865  eck_widget = Che
-0000c310: 636b 5769 6e64 6f77 2829 0a20 2020 2020  ckWindow().     
-0000c320: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-0000c330: 6b5f 7769 6e64 6f77 203d 2051 446f 636b  k_window = QDock
-0000c340: 5769 6467 6574 2863 6865 636b 5f77 6964  Widget(check_wid
-0000c350: 6765 742e 7072 6f70 6572 7479 2822 7769  get.property("wi
-0000c360: 6e64 6f77 5469 746c 6522 292c 2073 656c  ndowTitle"), sel
-0000c370: 6629 0a20 2020 2020 2020 2020 2020 2073  f).            s
-0000c380: 656c 662e 6368 6563 6b5f 7769 6e64 6f77  elf.check_window
-0000c390: 2e73 6574 5769 6467 6574 2863 6865 636b  .setWidget(check
-0000c3a0: 5f77 6964 6765 7429 0a20 2020 2020 2020  _widget).       
-0000c3b0: 2020 2020 2073 656c 662e 6164 6444 6f63       self.addDoc
-0000c3c0: 6b57 6964 6765 7428 5174 2e52 6967 6874  kWidget(Qt.Right
-0000c3d0: 446f 636b 5769 6467 6574 4172 6561 2c20  DockWidgetArea, 
-0000c3e0: 7365 6c66 2e63 6865 636b 5f77 696e 646f  self.check_windo
-0000c3f0: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
-0000c400: 6368 6563 6b5f 7769 6e64 6f77 2e73 686f  check_window.sho
-0000c410: 7728 290a 0a20 2020 2064 6566 206c 6175  w()..    def lau
-0000c420: 6e63 685f 7666 6f28 7365 6c66 2920 2d3e  nch_vfo(self) ->
-0000c430: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000c440: 2222 4c61 756e 6368 2074 6865 2056 464f  ""Launch the VFO
-0000c450: 2077 696e 646f 7722 2222 0a20 2020 2020   window""".     
-0000c460: 2020 2069 6620 6e6f 7420 7365 6c66 2e76     if not self.v
-0000c470: 666f 5f77 696e 646f 773a 0a20 2020 2020  fo_window:.     
-0000c480: 2020 2020 2020 2076 666f 5f77 6964 6765         vfo_widge
-0000c490: 7420 3d20 5666 6f57 696e 646f 7728 290a  t = VfoWindow().
-0000c4a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c4b0: 2e76 666f 5f77 696e 646f 7720 3d20 5144  .vfo_window = QD
-0000c4c0: 6f63 6b57 6964 6765 7428 7666 6f5f 7769  ockWidget(vfo_wi
-0000c4d0: 6467 6574 2e70 726f 7065 7274 7928 2277  dget.property("w
-0000c4e0: 696e 646f 7754 6974 6c65 2229 2c20 7365  indowTitle"), se
-0000c4f0: 6c66 290a 2020 2020 2020 2020 2020 2020  lf).            
-0000c500: 7365 6c66 2e76 666f 5f77 696e 646f 772e  self.vfo_window.
-0000c510: 7365 7457 6964 6765 7428 7666 6f5f 7769  setWidget(vfo_wi
-0000c520: 6467 6574 290a 2020 2020 2020 2020 2020  dget).          
-0000c530: 2020 7365 6c66 2e61 6464 446f 636b 5769    self.addDockWi
-0000c540: 6467 6574 2851 742e 5269 6768 7444 6f63  dget(Qt.RightDoc
-0000c550: 6b57 6964 6765 7441 7265 612c 2073 656c  kWidgetArea, sel
-0000c560: 662e 7666 6f5f 7769 6e64 6f77 290a 2020  f.vfo_window).  
-0000c570: 2020 2020 2020 7365 6c66 2e76 666f 5f77        self.vfo_w
-0000c580: 696e 646f 772e 7368 6f77 2829 0a0a 2020  indow.show()..  
-0000c590: 2020 6465 6620 636c 6561 725f 6261 6e64    def clear_band
-0000c5a0: 5f69 6e64 6963 6174 6f72 7328 7365 6c66  _indicators(self
-0000c5b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000c5c0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000c5d0: 6c65 6172 2074 6865 2069 6e64 6963 6174  lear the indicat
-0000c5e0: 6f72 732e 0a0a 2020 2020 2020 2020 5061  ors...        Pa
-0000c5f0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-0000c600: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000c610: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-0000c620: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000c630: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000c640: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-0000c650: 2022 2222 0a20 2020 2020 2020 2066 6f72   """.        for
-0000c660: 205f 2c20 696e 6469 6361 746f 7273 2069   _, indicators i
-0000c670: 6e20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  n self.all_mode_
-0000c680: 696e 6469 6361 746f 7273 2e69 7465 6d73  indicators.items
-0000c690: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000c6a0: 666f 7220 5f2c 2069 6e64 6963 6174 6f72  for _, indicator
-0000c6b0: 2069 6e20 696e 6469 6361 746f 7273 2e69   in indicators.i
-0000c6c0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000c6d0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-0000c6e0: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
-0000c6f0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-0000c700: 2e4e 6f46 7261 6d65 290a 2020 2020 2020  .NoFrame).      
-0000c710: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000c720: 662e 7465 7874 5f63 6f6c 6f72 203d 3d20  f.text_color == 
-0000c730: 5174 2e62 6c61 636b 3a0a 2020 2020 2020  Qt.black:.      
-0000c740: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000c750: 6469 6361 746f 722e 7365 7453 7479 6c65  dicator.setStyle
-0000c760: 5368 6565 7428 0a20 2020 2020 2020 2020  Sheet(.         
-0000c770: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c780: 666f 6e74 2d66 616d 696c 793a 204a 6574  font-family: Jet
-0000c790: 4272 6169 6e73 204d 6f6e 6f3b 2063 6f6c  Brains Mono; col
-0000c7a0: 6f72 3a20 626c 6163 6b3b 220a 2020 2020  or: black;".    
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c7d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000c7e0: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-0000c7f0: 6361 746f 722e 7365 7453 7479 6c65 5368  cator.setStyleSh
-0000c800: 6565 7428 2266 6f6e 742d 6661 6d69 6c79  eet("font-family
-0000c810: 3a20 4a65 7442 7261 696e 7320 4d6f 6e6f  : JetBrains Mono
-0000c820: 3b20 636f 6c6f 723a 2077 6869 7465 2229  ; color: white")
-0000c830: 0a0a 2020 2020 6465 6620 7365 745f 6261  ..    def set_ba
-0000c840: 6e64 5f69 6e64 6963 6174 6f72 2873 656c  nd_indicator(sel
-0000c850: 662c 2062 616e 643a 2073 7472 2920 2d3e  f, band: str) ->
-0000c860: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000c870: 2222 0a20 2020 2020 2020 2053 6574 2074  "".        Set t
-0000c880: 6865 2062 616e 6420 696e 6469 6361 746f  he band indicato
-0000c890: 720a 0a20 2020 2020 2020 2050 6172 616d  r..        Param
-0000c8a0: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
-0000c8b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000c8c0: 2020 6261 6e64 3a20 7374 720a 2020 2020    band: str.    
-0000c8d0: 2020 2020 6261 6e64 2074 6f20 7365 7420      band to set 
-0000c8e0: 696e 6469 6361 746f 7220 666f 720a 0a20  indicator for.. 
-0000c8f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000c900: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000c910: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-0000c920: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000c930: 2020 6966 2062 616e 6420 616e 6420 7365    if band and se
-0000c940: 6c66 2e63 7572 7265 6e74 5f6d 6f64 653a  lf.current_mode:
-0000c950: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c960: 662e 636c 6561 725f 6261 6e64 5f69 6e64  f.clear_band_ind
-0000c970: 6963 6174 6f72 7328 290a 2020 2020 2020  icators().      
-0000c980: 2020 2020 2020 696e 6469 6361 746f 7220        indicator 
-0000c990: 3d20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  = self.all_mode_
-0000c9a0: 696e 6469 6361 746f 7273 5b73 656c 662e  indicators[self.
-0000c9b0: 6375 7272 656e 745f 6d6f 6465 5d2e 6765  current_mode].ge
-0000c9c0: 7428 6261 6e64 2c20 4e6f 6e65 290a 2020  t(band, None).  
-0000c9d0: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
-0000c9e0: 6963 6174 6f72 3a0a 2020 2020 2020 2020  icator:.        
-0000c9f0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-0000ca00: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
-0000ca10: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-0000ca20: 2e42 6f78 290a 2020 2020 2020 2020 2020  .Box).          
-0000ca30: 2020 2020 2020 696e 6469 6361 746f 722e        indicator.
-0000ca40: 7365 7453 7479 6c65 5368 6565 7428 2266  setStyleSheet("f
-0000ca50: 6f6e 742d 6661 6d69 6c79 3a20 4a65 7442  ont-family: JetB
-0000ca60: 7261 696e 7320 4d6f 6e6f 3b20 636f 6c6f  rains Mono; colo
-0000ca70: 723a 2067 7265 656e 3b22 290a 0a20 2020  r: green;")..   
-0000ca80: 2064 6566 2063 6c6f 7365 4576 656e 7428   def closeEvent(
-0000ca90: 7365 6c66 2c20 5f65 7665 6e74 2920 2d3e  self, _event) ->
-0000caa0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000cab0: 2222 0a20 2020 2020 2020 2057 7269 7465  "".        Write
-0000cac0: 2077 696e 646f 7720 7369 7a65 2061 6e64   window size and
-0000cad0: 2070 6f73 6974 696f 6e20 746f 2063 6f6e   position to con
-0000cae0: 6669 6720 6669 6c65 2e0a 0a20 2020 2020  fig file...     
-0000caf0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-0000cb00: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000cb10: 2d0a 2020 2020 2020 2020 5f65 7665 6e74  -.        _event
-0000cb20: 3a20 5143 6c6f 7365 4576 656e 740a 0a20  : QCloseEvent.. 
-0000cb30: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000cb40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000cb50: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-0000cb60: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000cb70: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-0000cb80: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-0000cb90: 2248 414c 5422 0a20 2020 2020 2020 2063  "HALT".        c
-0000cba0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
-0000cbb0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-0000cbc0: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-0000cbd0: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-0000cbe0: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-0000cbf0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-0000cc00: 7072 6566 5b22 7769 6e64 6f77 5f77 6964  pref["window_wid
-0000cc10: 7468 225d 203d 2073 656c 662e 7369 7a65  th"] = self.size
-0000cc20: 2829 2e77 6964 7468 2829 0a20 2020 2020  ().width().     
-0000cc30: 2020 2073 656c 662e 7072 6566 5b22 7769     self.pref["wi
-0000cc40: 6e64 6f77 5f68 6569 6768 7422 5d20 3d20  ndow_height"] = 
-0000cc50: 7365 6c66 2e73 697a 6528 292e 6865 6967  self.size().heig
-0000cc60: 6874 2829 0a20 2020 2020 2020 2073 656c  ht().        sel
-0000cc70: 662e 7072 6566 5b22 7769 6e64 6f77 5f78  f.pref["window_x
-0000cc80: 225d 203d 2073 656c 662e 706f 7328 292e  "] = self.pos().
-0000cc90: 7828 290a 2020 2020 2020 2020 7365 6c66  x().        self
-0000cca0: 2e70 7265 665b 2277 696e 646f 775f 7922  .pref["window_y"
-0000ccb0: 5d20 3d20 7365 6c66 2e70 6f73 2829 2e79  ] = self.pos().y
-0000ccc0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000ccd0: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-0000cce0: 2829 0a0a 2020 2020 6465 6620 6374 795f  ()..    def cty_
-0000ccf0: 6c6f 6f6b 7570 2873 656c 662c 2063 616c  lookup(self, cal
-0000cd00: 6c73 6967 6e3a 2073 7472 2920 2d3e 206c  lsign: str) -> l
-0000cd10: 6973 743a 0a20 2020 2020 2020 2022 2222  ist:.        """
-0000cd20: 4c6f 6f6b 7570 2063 616c 6c73 6967 6e20  Lookup callsign 
-0000cd30: 696e 2063 7479 2e64 6174 2066 696c 652e  in cty.dat file.
-0000cd40: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000cd50: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000cd60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000cd70: 6361 6c6c 7369 676e 203a 2073 7472 0a20  callsign : str. 
-0000cd80: 2020 2020 2020 2063 616c 6c73 6967 6e20         callsign 
-0000cd90: 746f 206c 6f6f 6b75 700a 0a20 2020 2020  to lookup..     
-0000cda0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000cdb0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000cdc0: 2020 2072 6574 7572 6e20 3a20 6c69 7374     return : list
-0000cdd0: 0a20 2020 2020 2020 206c 6973 7420 6f66  .        list of
-0000cde0: 2064 6963 7473 2063 6f6e 7461 696e 696e   dicts containin
-0000cdf0: 6720 7468 6520 6361 6c6c 7369 676e 2061  g the callsign a
-0000ce00: 6e64 2074 6865 2073 7461 7469 6f6e 2e0a  nd the station..
-0000ce10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000ce20: 2020 2020 6361 6c6c 7369 676e 203d 2063      callsign = c
-0000ce30: 616c 6c73 6967 6e2e 7570 7065 7228 290a  allsign.upper().
-0000ce40: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
-0000ce50: 7420 696e 2072 6576 6572 7365 6428 7261  t in reversed(ra
-0000ce60: 6e67 6528 6c65 6e28 6361 6c6c 7369 676e  nge(len(callsign
-0000ce70: 2929 293a 0a20 2020 2020 2020 2020 2020  ))):.           
-0000ce80: 2073 6561 7263 6869 7465 6d20 3d20 6361   searchitem = ca
-0000ce90: 6c6c 7369 676e 5b3a 2063 6f75 6e74 202b  llsign[: count +
-0000cea0: 2031 5d0a 2020 2020 2020 2020 2020 2020   1].            
-0000ceb0: 7265 7375 6c74 203d 207b 6b65 793a 2076  result = {key: v
-0000cec0: 616c 2066 6f72 206b 6579 2c20 7661 6c20  al for key, val 
-0000ced0: 696e 2043 5459 4649 4c45 2e69 7465 6d73  in CTYFILE.items
-0000cee0: 2829 2069 6620 6b65 7920 3d3d 2073 6561  () if key == sea
-0000cef0: 7263 6869 7465 6d7d 0a20 2020 2020 2020  rchitem}.       
-0000cf00: 2020 2020 2069 6620 6e6f 7420 7265 7375       if not resu
-0000cf10: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
-0000cf20: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-0000cf30: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
-0000cf40: 6c74 2e67 6574 2873 6561 7263 6869 7465  lt.get(searchite
-0000cf50: 6d29 2e67 6574 2822 6578 6163 745f 6d61  m).get("exact_ma
-0000cf60: 7463 6822 293a 0a20 2020 2020 2020 2020  tch"):.         
-0000cf70: 2020 2020 2020 2069 6620 7365 6172 6368         if search
-0000cf80: 6974 656d 203d 3d20 6361 6c6c 7369 676e  item == callsign
-0000cf90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cfa0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000cfb0: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
-0000cfc0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-0000cfd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000cfe0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-0000cff0: 6377 7370 6565 645f 7370 696e 626f 785f  cwspeed_spinbox_
-0000d000: 6368 616e 6765 6428 7365 6c66 2920 2d3e  changed(self) ->
-0000d010: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000d020: 2222 0a20 2020 2020 2020 2054 7269 6767  "".        Trigg
-0000d030: 6572 6564 2077 6865 6e20 7661 6c75 6520  ered when value 
-0000d040: 6f66 2043 5720 7370 6565 6420 696e 2074  of CW speed in t
-0000d050: 6865 2073 7069 6e62 6f78 2063 6861 6e67  he spinbox chang
-0000d060: 6573 2e0a 0a20 2020 2020 2020 2050 6172  es...        Par
-0000d070: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-0000d080: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000d090: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
-0000d0a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000d0b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000d0c0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-0000d0d0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-0000d0e0: 656c 662e 6377 2069 7320 4e6f 6e65 3a0a  elf.cw is None:.
-0000d0f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d100: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000d110: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
-0000d120: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-0000d130: 2020 2073 656c 662e 6377 2e73 7065 6564     self.cw.speed
-0000d140: 203d 2073 656c 662e 6377 5f73 7065 6564   = self.cw_speed
-0000d150: 2e76 616c 7565 2829 0a20 2020 2020 2020  .value().       
-0000d160: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
-0000d170: 6463 7728 6622 5c78 3162 327b 7365 6c66  dcw(f"\x1b2{self
-0000d180: 2e63 772e 7370 6565 647d 2229 0a20 2020  .cw.speed}").   
-0000d190: 2020 2020 2069 6620 7365 6c66 2e63 772e       if self.cw.
-0000d1a0: 7365 7276 6572 7479 7065 203d 3d20 323a  servertype == 2:
-0000d1b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d1c0: 662e 6377 2e73 6574 5f77 696e 6b65 7965  f.cw.set_winkeye
-0000d1d0: 725f 7370 6565 6428 7365 6c66 2e63 775f  r_speed(self.cw_
-0000d1e0: 7370 6565 642e 7661 6c75 6528 2929 0a0a  speed.value())..
-0000d1f0: 2020 2020 6465 6620 6b65 7950 7265 7373      def keyPress
-0000d200: 4576 656e 7428 7365 6c66 2c20 6576 656e  Event(self, even
-0000d210: 7429 202d 3e20 4e6f 6e65 3a20 2023 2070  t) -> None:  # p
-0000d220: 796c 696e 743a 2064 6973 6162 6c65 3d69  ylint: disable=i
-0000d230: 6e76 616c 6964 2d6e 616d 650a 2020 2020  nvalid-name.    
-0000d240: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000d250: 5468 6973 206f 7665 7272 6964 6573 2051  This overrides Q
-0000d260: 7420 6b65 7920 6576 656e 742e 0a0a 2020  t key event...  
-0000d270: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000d280: 3a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  :.        ------
-0000d290: 2d2d 2d2d 0a20 2020 2020 2020 2065 7665  ----.        eve
-0000d2a0: 6e74 3a20 514b 6579 4576 656e 740a 2020  nt: QKeyEvent.  
-0000d2b0: 2020 2020 2020 5174 206b 6579 2065 7665        Qt key eve
-0000d2c0: 6e74 0a0a 2020 2020 2020 2020 5265 7475  nt..        Retu
-0000d2d0: 726e 733a 0a20 2020 2020 2020 202d 2d2d  rns:.        ---
-0000d2e0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-0000d2f0: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
-0000d300: 2020 2020 2020 206d 6f64 6966 6965 7220         modifier 
-0000d310: 3d20 6576 656e 742e 6d6f 6469 6669 6572  = event.modifier
-0000d320: 7328 290a 2020 2020 2020 2020 6966 2065  s().        if e
-0000d330: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-0000d340: 2e4b 6579 2e4b 6579 5f4b 3a0a 2020 2020  .Key.Key_K:.    
-0000d350: 2020 2020 2020 2020 7365 6c66 2e74 6f67          self.tog
-0000d360: 676c 655f 6377 5f65 6e74 7279 2829 0a20  gle_cw_entry(). 
-0000d370: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000d380: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
-0000d390: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-0000d3a0: 6579 5f53 2061 6e64 206d 6f64 6966 6965  ey_S and modifie
-0000d3b0: 7220 3d3d 2051 742e 436f 6e74 726f 6c4d  r == Qt.ControlM
-0000d3c0: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-0000d3d0: 2020 2020 2066 7265 7120 3d20 7365 6c66       freq = self
-0000d3e0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000d3f0: 2822 7666 6f61 2229 0a20 2020 2020 2020  ("vfoa").       
-0000d400: 2020 2020 2064 7820 3d20 7365 6c66 2e63       dx = self.c
-0000d410: 616c 6c73 6967 6e2e 7465 7874 2829 0a20  allsign.text(). 
-0000d420: 2020 2020 2020 2020 2020 2069 6620 6672             if fr
-0000d430: 6571 2061 6e64 2064 783a 0a20 2020 2020  eq and dx:.     
-0000d440: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-0000d450: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-0000d460: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
-0000d470: 2022 5350 4f54 4458 220a 2020 2020 2020   "SPOTDX".      
-0000d480: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
-0000d490: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-0000d4a0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-0000d4b0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-0000d4c0: 6478 225d 203d 2064 780a 2020 2020 2020  dx"] = dx.      
-0000d4d0: 2020 2020 2020 2020 2020 636d 645b 2266            cmd["f
-0000d4e0: 7265 7122 5d20 3d20 666c 6f61 7428 696e  req"] = float(in
-0000d4f0: 7428 6672 6571 2920 2f20 3130 3030 290a  t(freq) / 1000).
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-0000d520: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
-0000d530: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
-0000d540: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000d550: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-0000d560: 6579 2829 203d 3d20 5174 2e4b 6579 5f4d  ey() == Qt.Key_M
-0000d570: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
-0000d580: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
-0000d590: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-0000d5a0: 2066 7265 7120 3d20 7365 6c66 2e72 6164   freq = self.rad
-0000d5b0: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-0000d5c0: 6f61 2229 0a20 2020 2020 2020 2020 2020  oa").           
-0000d5d0: 2064 7820 3d20 7365 6c66 2e63 616c 6c73   dx = self.calls
-0000d5e0: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-0000d5f0: 2020 2020 2020 2069 6620 6672 6571 2061         if freq a
-0000d600: 6e64 2064 783a 0a20 2020 2020 2020 2020  nd dx:.         
-0000d610: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 636d 645b 2263 6d64 225d 203d 2022 4d41  cmd["cmd"] = "MA
-0000d640: 524b 4458 220a 2020 2020 2020 2020 2020  RKDX".          
-0000d650: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-0000d660: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-0000d670: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-0000d680: 2020 2020 2020 2063 6d64 5b22 6478 225d         cmd["dx"]
-0000d690: 203d 2064 780a 2020 2020 2020 2020 2020   = dx.          
-0000d6a0: 2020 2020 2020 636d 645b 2266 7265 7122        cmd["freq"
-0000d6b0: 5d20 3d20 666c 6f61 7428 696e 7428 6672  ] = float(int(fr
-0000d6c0: 6571 2920 2f20 3130 3030 290a 2020 2020  eq) / 1000).    
-0000d6d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d6e0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-0000d6f0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-0000d700: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
-0000d710: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000d720: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-0000d730: 203d 3d20 5174 2e4b 6579 5f47 2061 6e64   == Qt.Key_G and
-0000d740: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
-0000d750: 436f 6e74 726f 6c4d 6f64 6966 6965 723a  ControlModifier:
-0000d760: 0a20 2020 2020 2020 2020 2020 2064 7820  .            dx 
-0000d770: 3d20 7365 6c66 2e63 616c 6c73 6967 6e2e  = self.callsign.
-0000d780: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
-0000d790: 2020 2069 6620 6478 3a0a 2020 2020 2020     if dx:.      
-0000d7a0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-0000d7b0: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-0000d7c0: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-0000d7d0: 2246 494e 4444 5822 0a20 2020 2020 2020  "FINDDX".       
-0000d7e0: 2020 2020 2020 2020 2063 6d64 5b22 7374           cmd["st
-0000d7f0: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
-0000d800: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-0000d810: 2020 2020 2020 2020 2020 636d 645b 2264            cmd["d
-0000d820: 7822 5d20 3d20 6478 0a20 2020 2020 2020  x"] = dx.       
-0000d830: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-0000d840: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-0000d850: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-0000d860: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-0000d870: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000d880: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0000d890: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-0000d8a0: 742e 4b65 792e 4b65 795f 4573 6361 7065  t.Key.Key_Escape
-0000d8b0: 2061 6e64 206d 6f64 6966 6965 7220 213d   and modifier !=
-0000d8c0: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
-0000d8d0: 6965 720a 2020 2020 2020 2020 293a 2020  ier.        ):  
-0000d8e0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-0000d8f0: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
-0000d900: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-0000d910: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
-0000d920: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000d930: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-0000d940: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
-0000d950: 6579 5f45 7363 6170 6520 616e 6420 6d6f  ey_Escape and mo
-0000d960: 6469 6669 6572 203d 3d20 5174 2e43 6f6e  difier == Qt.Con
-0000d970: 7472 6f6c 4d6f 6469 6669 6572 3a0a 2020  trolModifier:.  
-0000d980: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000d990: 662e 6377 2069 7320 6e6f 7420 4e6f 6e65  f.cw is not None
-0000d9a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d9b0: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
-0000d9c0: 7665 7274 7970 6520 3d3d 2031 3a0a 2020  vertype == 1:.  
-0000d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9e0: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000d9f0: 2822 5c78 3162 3422 290a 2020 2020 2020  ("\x1b4").      
-0000da00: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000da10: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-0000da20: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-0000da30: 742e 4b65 792e 4b65 795f 5570 3a0a 2020  t.Key.Key_Up:.  
-0000da40: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-0000da50: 7b7d 0a20 2020 2020 2020 2020 2020 2063  {}.            c
-0000da60: 6d64 5b22 636d 6422 5d20 3d20 2250 5245  md["cmd"] = "PRE
-0000da70: 5653 504f 5422 0a20 2020 2020 2020 2020  VSPOT".         
-0000da80: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
-0000da90: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
-0000daa0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000dab0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-0000dac0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
-0000dad0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
-0000dae0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000daf0: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-0000db00: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
-0000db10: 6579 5f44 6f77 6e3a 0a20 2020 2020 2020  ey_Down:.       
-0000db20: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
-0000db30: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
-0000db40: 6d64 225d 203d 2022 4e45 5854 5350 4f54  md"] = "NEXTSPOT
-0000db50: 220a 2020 2020 2020 2020 2020 2020 636d  ".            cm
-0000db60: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
-0000db70: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-0000db80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000db90: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-0000dba0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-0000dbb0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
-0000dbc0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000dbd0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-0000dbe0: 3d3d 2051 742e 4b65 792e 4b65 795f 5061  == Qt.Key.Key_Pa
-0000dbf0: 6765 5570 2061 6e64 206d 6f64 6966 6965  geUp and modifie
-0000dc00: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
-0000dc10: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-0000dc20: 2020 2020 2069 6620 7365 6c66 2e63 7720       if self.cw 
-0000dc30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000dc40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000dc50: 662e 6377 2e73 7065 6564 202b 3d20 310a  f.cw.speed += 1.
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 7365 6c66 2e63 775f 7370 6565 642e 7365  self.cw_speed.se
-0000dc80: 7456 616c 7565 2873 656c 662e 6377 2e73  tValue(self.cw.s
-0000dc90: 7065 6564 290a 2020 2020 2020 2020 2020  peed).          
-0000dca0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-0000dcb0: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
-0000dcc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000dcd0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000dce0: 6e64 6377 2866 225c 7831 6232 7b73 656c  ndcw(f"\x1b2{sel
-0000dcf0: 662e 6377 2e73 7065 6564 7d22 290a 2020  f.cw.speed}").  
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000dd10: 2073 656c 662e 6377 2e73 6572 7665 7274   self.cw.servert
-0000dd20: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000dd40: 6c66 2e63 772e 7365 745f 7769 6e6b 6579  lf.cw.set_winkey
-0000dd50: 6572 5f73 7065 6564 2873 656c 662e 6377  er_speed(self.cw
-0000dd60: 5f73 7065 6564 2e76 616c 7565 2829 290a  _speed.value()).
-0000dd70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dd80: 726e 0a20 2020 2020 2020 2069 6620 6576  rn.        if ev
-0000dd90: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-0000dda0: 4b65 792e 4b65 795f 5061 6765 446f 776e  Key.Key_PageDown
-0000ddb0: 2061 6e64 206d 6f64 6966 6965 7220 213d   and modifier !=
-0000ddc0: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
-0000ddd0: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-0000dde0: 2069 6620 7365 6c66 2e63 7720 6973 206e   if self.cw is n
-0000ddf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000de00: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000de10: 2e73 7065 6564 202d 3d20 310a 2020 2020  .speed -= 1.    
-0000de20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000de30: 2e63 775f 7370 6565 642e 7365 7456 616c  .cw_speed.setVal
-0000de40: 7565 2873 656c 662e 6377 2e73 7065 6564  ue(self.cw.speed
+0000c050: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c060: 2e6c 6f67 5f77 696e 646f 7720 3d20 4c6f  .log_window = Lo
+0000c070: 6757 696e 646f 7728 290a 2020 2020 2020  gWindow().      
+0000c080: 2020 2020 2020 7365 6c66 2e61 6464 446f        self.addDo
+0000c090: 636b 5769 6467 6574 2851 742e 426f 7474  ckWidget(Qt.Bott
+0000c0a0: 6f6d 446f 636b 5769 6467 6574 4172 6561  omDockWidgetArea
+0000c0b0: 2c20 7365 6c66 2e6c 6f67 5f77 696e 646f  , self.log_windo
+0000c0c0: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
+0000c0d0: 6c6f 675f 7769 6e64 6f77 2e73 686f 7728  log_window.show(
+0000c0e0: 290a 0a20 2020 2064 6566 206c 6175 6e63  )..    def launc
+0000c0f0: 685f 6261 6e64 6d61 705f 7769 6e64 6f77  h_bandmap_window
+0000c100: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000c110: 2020 2020 2020 2020 2222 224c 6175 6e63          """Launc
+0000c120: 6820 7468 6520 6261 6e64 6d61 7020 7769  h the bandmap wi
+0000c130: 6e64 6f77 2222 220a 2020 2020 2020 2020  ndow""".        
+0000c140: 6966 206e 6f74 2073 656c 662e 6261 6e64  if not self.band
+0000c150: 6d61 705f 7769 6e64 6f77 3a0a 2020 2020  map_window:.    
+0000c160: 2020 2020 2020 2020 7365 6c66 2e62 616e          self.ban
+0000c170: 646d 6170 5f77 696e 646f 7720 3d20 4261  dmap_window = Ba
+0000c180: 6e64 4d61 7057 696e 646f 7728 290a 2020  ndMapWindow().  
+0000c190: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c1a0: 6464 446f 636b 5769 6467 6574 2851 742e  ddDockWidget(Qt.
+0000c1b0: 5269 6768 7444 6f63 6b57 6964 6765 7441  RightDockWidgetA
+0000c1c0: 7265 612c 2073 656c 662e 6261 6e64 6d61  rea, self.bandma
+0000c1d0: 705f 7769 6e64 6f77 290a 2020 2020 2020  p_window).      
+0000c1e0: 2020 7365 6c66 2e62 616e 646d 6170 5f77    self.bandmap_w
+0000c1f0: 696e 646f 772e 7368 6f77 2829 0a0a 2020  indow.show()..  
+0000c200: 2020 6465 6620 6c61 756e 6368 5f63 6865    def launch_che
+0000c210: 636b 5f77 696e 646f 7728 7365 6c66 2920  ck_window(self) 
+0000c220: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000c230: 2022 2222 4c61 756e 6368 2074 6865 2063   """Launch the c
+0000c240: 6865 636b 2077 696e 646f 7722 2222 0a20  heck window""". 
+0000c250: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c260: 6c66 2e63 6865 636b 5f77 696e 646f 773a  lf.check_window:
+0000c270: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c280: 662e 6368 6563 6b5f 7769 6e64 6f77 203d  f.check_window =
+0000c290: 2043 6865 636b 5769 6e64 6f77 2829 0a20   CheckWindow(). 
+0000c2a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c2b0: 6164 6444 6f63 6b57 6964 6765 7428 5174  addDockWidget(Qt
+0000c2c0: 2e52 6967 6874 446f 636b 5769 6467 6574  .RightDockWidget
+0000c2d0: 4172 6561 2c20 7365 6c66 2e63 6865 636b  Area, self.check
+0000c2e0: 5f77 696e 646f 7729 0a20 2020 2020 2020  _window).       
+0000c2f0: 2073 656c 662e 6368 6563 6b5f 7769 6e64   self.check_wind
+0000c300: 6f77 2e73 686f 7728 290a 0a20 2020 2064  ow.show()..    d
+0000c310: 6566 206c 6175 6e63 685f 7666 6f28 7365  ef launch_vfo(se
+0000c320: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+0000c330: 2020 2020 2022 2222 4c61 756e 6368 2074       """Launch t
+0000c340: 6865 2056 464f 2077 696e 646f 7722 2222  he VFO window"""
+0000c350: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000c360: 7365 6c66 2e76 666f 5f77 696e 646f 773a  self.vfo_window:
+0000c370: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c380: 662e 7666 6f5f 7769 6e64 6f77 203d 2056  f.vfo_window = V
+0000c390: 666f 5769 6e64 6f77 2829 0a20 2020 2020  foWindow().     
+0000c3a0: 2020 2020 2020 2073 656c 662e 6164 6444         self.addD
+0000c3b0: 6f63 6b57 6964 6765 7428 5174 2e52 6967  ockWidget(Qt.Rig
+0000c3c0: 6874 446f 636b 5769 6467 6574 4172 6561  htDockWidgetArea
+0000c3d0: 2c20 7365 6c66 2e76 666f 5f77 696e 646f  , self.vfo_windo
+0000c3e0: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
+0000c3f0: 7666 6f5f 7769 6e64 6f77 2e73 686f 7728  vfo_window.show(
+0000c400: 290a 0a20 2020 2064 6566 2063 6c65 6172  )..    def clear
+0000c410: 5f62 616e 645f 696e 6469 6361 746f 7273  _band_indicators
+0000c420: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000c430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c440: 2020 2020 436c 6561 7220 7468 6520 696e      Clear the in
+0000c450: 6469 6361 746f 7273 2e0a 0a20 2020 2020  dicators...     
+0000c460: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+0000c470: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000c480: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
+0000c490: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000c4a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000c4b0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+0000c4c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c4d0: 2020 666f 7220 5f2c 2069 6e64 6963 6174    for _, indicat
+0000c4e0: 6f72 7320 696e 2073 656c 662e 616c 6c5f  ors in self.all_
+0000c4f0: 6d6f 6465 5f69 6e64 6963 6174 6f72 732e  mode_indicators.
+0000c500: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0000c510: 2020 2020 2066 6f72 205f 2c20 696e 6469       for _, indi
+0000c520: 6361 746f 7220 696e 2069 6e64 6963 6174  cator in indicat
+0000c530: 6f72 732e 6974 656d 7328 293a 0a20 2020  ors.items():.   
+0000c540: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000c550: 6963 6174 6f72 2e73 6574 4672 616d 6553  icator.setFrameS
+0000c560: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
+0000c570: 4672 616d 652e 4e6f 4672 616d 6529 0a20  Frame.NoFrame). 
+0000c580: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c590: 6620 7365 6c66 2e74 6578 745f 636f 6c6f  f self.text_colo
+0000c5a0: 7220 3d3d 2051 742e 626c 6163 6b3a 0a20  r == Qt.black:. 
+0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5c0: 2020 2069 6e64 6963 6174 6f72 2e73 6574     indicator.set
+0000c5d0: 5374 796c 6553 6865 6574 280a 2020 2020  StyleSheet(.    
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2020 2266 6f6e 742d 6661 6d69 6c79      "font-family
+0000c600: 3a20 4a65 7442 7261 696e 7320 4d6f 6e6f  : JetBrains Mono
+0000c610: 3b20 636f 6c6f 723a 2062 6c61 636b 3b22  ; color: black;"
+0000c620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c630: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000c640: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c660: 2069 6e64 6963 6174 6f72 2e73 6574 5374   indicator.setSt
+0000c670: 796c 6553 6865 6574 2822 666f 6e74 2d66  yleSheet("font-f
+0000c680: 616d 696c 793a 204a 6574 4272 6169 6e73  amily: JetBrains
+0000c690: 204d 6f6e 6f3b 2063 6f6c 6f72 3a20 7768   Mono; color: wh
+0000c6a0: 6974 6522 290a 0a20 2020 2064 6566 2073  ite")..    def s
+0000c6b0: 6574 5f62 616e 645f 696e 6469 6361 746f  et_band_indicato
+0000c6c0: 7228 7365 6c66 2c20 6261 6e64 3a20 7374  r(self, band: st
+0000c6d0: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+0000c6e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c6f0: 5365 7420 7468 6520 6261 6e64 2069 6e64  Set the band ind
+0000c700: 6963 6174 6f72 0a0a 2020 2020 2020 2020  icator..        
+0000c710: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+0000c720: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000c730: 2020 2020 2020 2062 616e 643a 2073 7472         band: str
+0000c740: 0a20 2020 2020 2020 2062 616e 6420 746f  .        band to
+0000c750: 2073 6574 2069 6e64 6963 6174 6f72 2066   set indicator f
+0000c760: 6f72 0a0a 2020 2020 2020 2020 5265 7475  or..        Retu
+0000c770: 726e 733a 0a20 2020 2020 2020 202d 2d2d  rns:.        ---
+0000c780: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+0000c790: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
+0000c7a0: 2020 2020 2020 2069 6620 6261 6e64 2061         if band a
+0000c7b0: 6e64 2073 656c 662e 6375 7272 656e 745f  nd self.current_
+0000c7c0: 6d6f 6465 3a0a 2020 2020 2020 2020 2020  mode:.          
+0000c7d0: 2020 7365 6c66 2e63 6c65 6172 5f62 616e    self.clear_ban
+0000c7e0: 645f 696e 6469 6361 746f 7273 2829 0a20  d_indicators(). 
+0000c7f0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+0000c800: 6174 6f72 203d 2073 656c 662e 616c 6c5f  ator = self.all_
+0000c810: 6d6f 6465 5f69 6e64 6963 6174 6f72 735b  mode_indicators[
+0000c820: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
+0000c830: 655d 2e67 6574 2862 616e 642c 204e 6f6e  e].get(band, Non
+0000c840: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+0000c850: 6620 696e 6469 6361 746f 723a 0a20 2020  f indicator:.   
+0000c860: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000c870: 6963 6174 6f72 2e73 6574 4672 616d 6553  icator.setFrameS
+0000c880: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
+0000c890: 4672 616d 652e 426f 7829 0a20 2020 2020  Frame.Box).     
+0000c8a0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+0000c8b0: 6174 6f72 2e73 6574 5374 796c 6553 6865  ator.setStyleShe
+0000c8c0: 6574 2822 666f 6e74 2d66 616d 696c 793a  et("font-family:
+0000c8d0: 204a 6574 4272 6169 6e73 204d 6f6e 6f3b   JetBrains Mono;
+0000c8e0: 2063 6f6c 6f72 3a20 6772 6565 6e3b 2229   color: green;")
+0000c8f0: 0a0a 2020 2020 6465 6620 636c 6f73 6545  ..    def closeE
+0000c900: 7665 6e74 2873 656c 662c 205f 6576 656e  vent(self, _even
+0000c910: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+0000c920: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c930: 5772 6974 6520 7769 6e64 6f77 2073 697a  Write window siz
+0000c940: 6520 616e 6420 706f 7369 7469 6f6e 2074  e and position t
+0000c950: 6f20 636f 6e66 6967 2066 696c 652e 0a0a  o config file...
+0000c960: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000c970: 7273 3a0a 2020 2020 2020 2020 2d2d 2d2d  rs:.        ----
+0000c980: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 205f  ------.        _
+0000c990: 6576 656e 743a 2051 436c 6f73 6545 7665  event: QCloseEve
+0000c9a0: 6e74 0a0a 2020 2020 2020 2020 5265 7475  nt..        Retu
+0000c9b0: 726e 733a 0a20 2020 2020 2020 202d 2d2d  rns:.        ---
+0000c9c0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+0000c9d0: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
+0000c9e0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
+0000c9f0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+0000ca00: 225d 203d 2022 4841 4c54 220a 2020 2020  "] = "HALT".    
+0000ca10: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
+0000ca20: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
+0000ca30: 6465 2829 0a20 2020 2020 2020 2073 656c  de().        sel
+0000ca40: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+0000ca50: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
+0000ca60: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
+0000ca70: 7365 6c66 2e70 7265 665b 2277 696e 646f  self.pref["windo
+0000ca80: 775f 7769 6474 6822 5d20 3d20 7365 6c66  w_width"] = self
+0000ca90: 2e73 697a 6528 292e 7769 6474 6828 290a  .size().width().
+0000caa0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+0000cab0: 665b 2277 696e 646f 775f 6865 6967 6874  f["window_height
+0000cac0: 225d 203d 2073 656c 662e 7369 7a65 2829  "] = self.size()
+0000cad0: 2e68 6569 6768 7428 290a 2020 2020 2020  .height().      
+0000cae0: 2020 7365 6c66 2e70 7265 665b 2277 696e    self.pref["win
+0000caf0: 646f 775f 7822 5d20 3d20 7365 6c66 2e70  dow_x"] = self.p
+0000cb00: 6f73 2829 2e78 2829 0a20 2020 2020 2020  os().x().       
+0000cb10: 2073 656c 662e 7072 6566 5b22 7769 6e64   self.pref["wind
+0000cb20: 6f77 5f79 225d 203d 2073 656c 662e 706f  ow_y"] = self.po
+0000cb30: 7328 292e 7928 290a 2020 2020 2020 2020  s().y().        
+0000cb40: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+0000cb50: 7265 6e63 6528 290a 0a20 2020 2064 6566  rence()..    def
+0000cb60: 2063 7479 5f6c 6f6f 6b75 7028 7365 6c66   cty_lookup(self
+0000cb70: 2c20 6361 6c6c 7369 676e 3a20 7374 7229  , callsign: str)
+0000cb80: 202d 3e20 6c69 7374 3a0a 2020 2020 2020   -> list:.      
+0000cb90: 2020 2222 224c 6f6f 6b75 7020 6361 6c6c    """Lookup call
+0000cba0: 7369 676e 2069 6e20 6374 792e 6461 7420  sign in cty.dat 
+0000cbb0: 6669 6c65 2e0a 0a20 2020 2020 2020 2050  file...        P
+0000cbc0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000cbd0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000cbe0: 2020 2020 2063 616c 6c73 6967 6e20 3a20       callsign : 
+0000cbf0: 7374 720a 2020 2020 2020 2020 6361 6c6c  str.        call
+0000cc00: 7369 676e 2074 6f20 6c6f 6f6b 7570 0a0a  sign to lookup..
+0000cc10: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000cc20: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000cc30: 2020 2020 2020 2020 7265 7475 726e 203a          return :
+0000cc40: 206c 6973 740a 2020 2020 2020 2020 6c69   list.        li
+0000cc50: 7374 206f 6620 6469 6374 7320 636f 6e74  st of dicts cont
+0000cc60: 6169 6e69 6e67 2074 6865 2063 616c 6c73  aining the calls
+0000cc70: 6967 6e20 616e 6420 7468 6520 7374 6174  ign and the stat
+0000cc80: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
+0000cc90: 0a20 2020 2020 2020 2063 616c 6c73 6967  .        callsig
+0000cca0: 6e20 3d20 6361 6c6c 7369 676e 2e75 7070  n = callsign.upp
+0000ccb0: 6572 2829 0a20 2020 2020 2020 2066 6f72  er().        for
+0000ccc0: 2063 6f75 6e74 2069 6e20 7265 7665 7273   count in revers
+0000ccd0: 6564 2872 616e 6765 286c 656e 2863 616c  ed(range(len(cal
+0000cce0: 6c73 6967 6e29 2929 3a0a 2020 2020 2020  lsign))):.      
+0000ccf0: 2020 2020 2020 7365 6172 6368 6974 656d        searchitem
+0000cd00: 203d 2063 616c 6c73 6967 6e5b 3a20 636f   = callsign[: co
+0000cd10: 756e 7420 2b20 315d 0a20 2020 2020 2020  unt + 1].       
+0000cd20: 2020 2020 2072 6573 756c 7420 3d20 7b6b       result = {k
+0000cd30: 6579 3a20 7661 6c20 666f 7220 6b65 792c  ey: val for key,
+0000cd40: 2076 616c 2069 6e20 4354 5946 494c 452e   val in CTYFILE.
+0000cd50: 6974 656d 7328 2920 6966 206b 6579 203d  items() if key =
+0000cd60: 3d20 7365 6172 6368 6974 656d 7d0a 2020  = searchitem}.  
+0000cd70: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000cd80: 2072 6573 756c 743a 0a20 2020 2020 2020   result:.       
+0000cd90: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000cda0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+0000cdb0: 2072 6573 756c 742e 6765 7428 7365 6172   result.get(sear
+0000cdc0: 6368 6974 656d 292e 6765 7428 2265 7861  chitem).get("exa
+0000cdd0: 6374 5f6d 6174 6368 2229 3a0a 2020 2020  ct_match"):.    
+0000cde0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000cdf0: 6561 7263 6869 7465 6d20 3d3d 2063 616c  earchitem == cal
+0000ce00: 6c73 6967 6e3a 0a20 2020 2020 2020 2020  lsign:.         
+0000ce10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ce20: 6e20 7265 7375 6c74 0a20 2020 2020 2020  n result.       
+0000ce30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000ce40: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
+0000ce50: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0000ce60: 2064 6566 2063 7773 7065 6564 5f73 7069   def cwspeed_spi
+0000ce70: 6e62 6f78 5f63 6861 6e67 6564 2873 656c  nbox_changed(sel
+0000ce80: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000ce90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cea0: 5472 6967 6765 7265 6420 7768 656e 2076  Triggered when v
+0000ceb0: 616c 7565 206f 6620 4357 2073 7065 6564  alue of CW speed
+0000cec0: 2069 6e20 7468 6520 7370 696e 626f 7820   in the spinbox 
+0000ced0: 6368 616e 6765 732e 0a0a 2020 2020 2020  changes...      
+0000cee0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+0000cef0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000cf00: 0a20 2020 2020 2020 204e 6f6e 650a 0a20  .        None.. 
+0000cf10: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000cf20: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000cf30: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+0000cf40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cf50: 2069 6620 7365 6c66 2e63 7720 6973 204e   if self.cw is N
+0000cf60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000cf70: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000cf80: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
+0000cf90: 7274 7970 6520 3d3d 2031 3a0a 2020 2020  rtype == 1:.    
+0000cfa0: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000cfb0: 7370 6565 6420 3d20 7365 6c66 2e63 775f  speed = self.cw_
+0000cfc0: 7370 6565 642e 7661 6c75 6528 290a 2020  speed.value().  
+0000cfd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000cfe0: 772e 7365 6e64 6377 2866 225c 7831 6232  w.sendcw(f"\x1b2
+0000cff0: 7b73 656c 662e 6377 2e73 7065 6564 7d22  {self.cw.speed}"
+0000d000: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000d010: 662e 6377 2e73 6572 7665 7274 7970 6520  f.cw.servertype 
+0000d020: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
+0000d030: 2020 7365 6c66 2e63 772e 7365 745f 7769    self.cw.set_wi
+0000d040: 6e6b 6579 6572 5f73 7065 6564 2873 656c  nkeyer_speed(sel
+0000d050: 662e 6377 5f73 7065 6564 2e76 616c 7565  f.cw_speed.value
+0000d060: 2829 290a 0a20 2020 2064 6566 206b 6579  ())..    def key
+0000d070: 5072 6573 7345 7665 6e74 2873 656c 662c  PressEvent(self,
+0000d080: 2065 7665 6e74 2920 2d3e 204e 6f6e 653a   event) -> None:
+0000d090: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+0000d0a0: 626c 653d 696e 7661 6c69 642d 6e61 6d65  ble=invalid-name
+0000d0b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d0c0: 2020 2020 2054 6869 7320 6f76 6572 7269       This overri
+0000d0d0: 6465 7320 5174 206b 6579 2065 7665 6e74  des Qt key event
+0000d0e0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000d0f0: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
+0000d100: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000d110: 2020 6576 656e 743a 2051 4b65 7945 7665    event: QKeyEve
+0000d120: 6e74 0a20 2020 2020 2020 2051 7420 6b65  nt.        Qt ke
+0000d130: 7920 6576 656e 740a 0a20 2020 2020 2020  y event..       
+0000d140: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000d150: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000d160: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+0000d170: 2222 0a0a 2020 2020 2020 2020 6d6f 6469  ""..        modi
+0000d180: 6669 6572 203d 2065 7665 6e74 2e6d 6f64  fier = event.mod
+0000d190: 6966 6965 7273 2829 0a20 2020 2020 2020  ifiers().       
+0000d1a0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+0000d1b0: 3d3d 2051 742e 4b65 792e 4b65 795f 4b3a  == Qt.Key.Key_K:
+0000d1c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d1d0: 662e 746f 6767 6c65 5f63 775f 656e 7472  f.toggle_cw_entr
+0000d1e0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+0000d1f0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+0000d200: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+0000d210: 2051 742e 4b65 795f 5320 616e 6420 6d6f   Qt.Key_S and mo
+0000d220: 6469 6669 6572 203d 3d20 5174 2e43 6f6e  difier == Qt.Con
+0000d230: 7472 6f6c 4d6f 6469 6669 6572 3a0a 2020  trolModifier:.  
+0000d240: 2020 2020 2020 2020 2020 6672 6571 203d            freq =
+0000d250: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000d260: 652e 6765 7428 2276 666f 6122 290a 2020  e.get("vfoa").  
+0000d270: 2020 2020 2020 2020 2020 6478 203d 2073            dx = s
+0000d280: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
+0000d290: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+0000d2a0: 6966 2066 7265 7120 616e 6420 6478 3a0a  if freq and dx:.
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+0000d2d0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+0000d2e0: 6422 5d20 3d20 2253 504f 5444 5822 0a20  d"] = "SPOTDX". 
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d300: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+0000d310: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 636d 645b 2264 7822 5d20 3d20 6478 0a20  cmd["dx"] = dx. 
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d350: 6d64 5b22 6672 6571 225d 203d 2066 6c6f  md["freq"] = flo
+0000d360: 6174 2869 6e74 2866 7265 7129 202f 2031  at(int(freq) / 1
+0000d370: 3030 3029 0a20 2020 2020 2020 2020 2020  000).           
+0000d380: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+0000d390: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+0000d3a0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+0000d3b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d3c0: 726e 0a20 2020 2020 2020 2069 6620 6576  rn.        if ev
+0000d3d0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+0000d3e0: 4b65 795f 4d20 616e 6420 6d6f 6469 6669  Key_M and modifi
+0000d3f0: 6572 203d 3d20 5174 2e43 6f6e 7472 6f6c  er == Qt.Control
+0000d400: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+0000d410: 2020 2020 2020 6672 6571 203d 2073 656c        freq = sel
+0000d420: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0000d430: 7428 2276 666f 6122 290a 2020 2020 2020  t("vfoa").      
+0000d440: 2020 2020 2020 6478 203d 2073 656c 662e        dx = self.
+0000d450: 6361 6c6c 7369 676e 2e74 6578 7428 290a  callsign.text().
+0000d460: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+0000d470: 7265 7120 616e 6420 6478 3a0a 2020 2020  req and dx:.    
+0000d480: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+0000d490: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+0000d4a0: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+0000d4b0: 3d20 224d 4152 4b44 5822 0a20 2020 2020  = "MARKDX".     
+0000d4c0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+0000d4d0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+0000d4e0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+0000d4f0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+0000d500: 2264 7822 5d20 3d20 6478 0a20 2020 2020  "dx"] = dx.     
+0000d510: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+0000d520: 6672 6571 225d 203d 2066 6c6f 6174 2869  freq"] = float(i
+0000d530: 6e74 2866 7265 7129 202f 2031 3030 3029  nt(freq) / 1000)
+0000d540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d550: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+0000d560: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+0000d570: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
+0000d580: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000d590: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+0000d5a0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
+0000d5b0: 4720 616e 6420 6d6f 6469 6669 6572 203d  G and modifier =
+0000d5c0: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
+0000d5d0: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
+0000d5e0: 2020 6478 203d 2073 656c 662e 6361 6c6c    dx = self.call
+0000d5f0: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
+0000d600: 2020 2020 2020 2020 6966 2064 783a 0a20          if dx:. 
+0000d610: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d620: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+0000d630: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+0000d640: 225d 203d 2022 4649 4e44 4458 220a 2020  "] = "FINDDX".  
+0000d650: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+0000d660: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
+0000d670: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d690: 6d64 5b22 6478 225d 203d 2064 780a 2020  md["dx"] = dx.  
+0000d6a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d6b0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+0000d6c0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+0000d6d0: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
+0000d6e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000d6f0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+0000d700: 2020 2020 2065 7665 6e74 2e6b 6579 2829       event.key()
+0000d710: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f45   == Qt.Key.Key_E
+0000d720: 7363 6170 6520 616e 6420 6d6f 6469 6669  scape and modifi
+0000d730: 6572 2021 3d20 5174 2e43 6f6e 7472 6f6c  er != Qt.Control
+0000d740: 4d6f 6469 6669 6572 0a20 2020 2020 2020  Modifier.       
+0000d750: 2029 3a20 2023 2070 796c 696e 743a 2064   ):  # pylint: d
+0000d760: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
+0000d770: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d780: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
+0000d790: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d7a0: 726e 0a20 2020 2020 2020 2069 6620 6576  rn.        if ev
+0000d7b0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+0000d7c0: 4b65 792e 4b65 795f 4573 6361 7065 2061  Key.Key_Escape a
+0000d7d0: 6e64 206d 6f64 6966 6965 7220 3d3d 2051  nd modifier == Q
+0000d7e0: 742e 436f 6e74 726f 6c4d 6f64 6966 6965  t.ControlModifie
+0000d7f0: 723a 0a20 2020 2020 2020 2020 2020 2069  r:.            i
+0000d800: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
+0000d810: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000d820: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000d830: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
+0000d840: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000d850: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+0000d860: 656e 6463 7728 225c 7831 6234 2229 0a20  endcw("\x1b4"). 
+0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d880: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000d890: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+0000d8a0: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f55   == Qt.Key.Key_U
+0000d8b0: 703a 0a20 2020 2020 2020 2020 2020 2063  p:.            c
+0000d8c0: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+0000d8d0: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
+0000d8e0: 2022 5052 4556 5350 4f54 220a 2020 2020   "PREVSPOT".    
+0000d8f0: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
+0000d900: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
+0000d910: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
+0000d920: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+0000d930: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+0000d940: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+0000d950: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d960: 726e 0a20 2020 2020 2020 2069 6620 6576  rn.        if ev
+0000d970: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+0000d980: 4b65 792e 4b65 795f 446f 776e 3a0a 2020  Key.Key_Down:.  
+0000d990: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+0000d9a0: 7b7d 0a20 2020 2020 2020 2020 2020 2063  {}.            c
+0000d9b0: 6d64 5b22 636d 6422 5d20 3d20 224e 4558  md["cmd"] = "NEX
+0000d9c0: 5453 504f 5422 0a20 2020 2020 2020 2020  TSPOT".         
+0000d9d0: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+0000d9e0: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+0000d9f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000da00: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+0000da10: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+0000da20: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+0000da30: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000da40: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+0000da50: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
+0000da60: 6579 5f50 6167 6555 7020 616e 6420 6d6f  ey_PageUp and mo
+0000da70: 6469 6669 6572 2021 3d20 5174 2e43 6f6e  difier != Qt.Con
+0000da80: 7472 6f6c 4d6f 6469 6669 6572 3a0a 2020  trolModifier:.  
+0000da90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000daa0: 662e 6377 2069 7320 6e6f 7420 4e6f 6e65  f.cw is not None
+0000dab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000dac0: 2020 7365 6c66 2e63 772e 7370 6565 6420    self.cw.speed 
+0000dad0: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+0000dae0: 2020 2020 2073 656c 662e 6377 5f73 7065       self.cw_spe
+0000daf0: 6564 2e73 6574 5661 6c75 6528 7365 6c66  ed.setValue(self
+0000db00: 2e63 772e 7370 6565 6429 0a20 2020 2020  .cw.speed).     
+0000db10: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000db20: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
+0000db30: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+0000db40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000db50: 6377 2e73 656e 6463 7728 6622 5c78 3162  cw.sendcw(f"\x1b
+0000db60: 327b 7365 6c66 2e63 772e 7370 6565 647d  2{self.cw.speed}
+0000db70: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000db80: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
+0000db90: 7276 6572 7479 7065 203d 3d20 323a 0a20  rvertype == 2:. 
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2073 656c 662e 6377 2e73 6574 5f77     self.cw.set_w
+0000dbc0: 696e 6b65 7965 725f 7370 6565 6428 7365  inkeyer_speed(se
+0000dbd0: 6c66 2e63 775f 7370 6565 642e 7661 6c75  lf.cw_speed.valu
+0000dbe0: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
+0000dbf0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000dc00: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+0000dc10: 3d20 5174 2e4b 6579 2e4b 6579 5f50 6167  = Qt.Key.Key_Pag
+0000dc20: 6544 6f77 6e20 616e 6420 6d6f 6469 6669  eDown and modifi
+0000dc30: 6572 2021 3d20 5174 2e43 6f6e 7472 6f6c  er != Qt.Control
+0000dc40: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+0000dc50: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+0000dc60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000dc70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dc80: 6c66 2e63 772e 7370 6565 6420 2d3d 2031  lf.cw.speed -= 1
+0000dc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dca0: 2073 656c 662e 6377 5f73 7065 6564 2e73   self.cw_speed.s
+0000dcb0: 6574 5661 6c75 6528 7365 6c66 2e63 772e  etValue(self.cw.
+0000dcc0: 7370 6565 6429 0a20 2020 2020 2020 2020  speed).         
+0000dcd0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000dce0: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
+0000dcf0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000dd00: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+0000dd10: 656e 6463 7728 6622 5c78 3162 327b 7365  endcw(f"\x1b2{se
+0000dd20: 6c66 2e63 772e 7370 6565 647d 2229 0a20  lf.cw.speed}"). 
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000dd40: 6620 7365 6c66 2e63 772e 7365 7276 6572  f self.cw.server
+0000dd50: 7479 7065 203d 3d20 323a 0a20 2020 2020  type == 2:.     
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dd70: 656c 662e 6377 2e73 6574 5f77 696e 6b65  elf.cw.set_winke
+0000dd80: 7965 725f 7370 6565 6428 7365 6c66 2e63  yer_speed(self.c
+0000dd90: 775f 7370 6565 642e 7661 6c75 6528 2929  w_speed.value())
+0000dda0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000ddb0: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
+0000ddc0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+0000ddd0: 2e4b 6579 2e4b 6579 5f54 6162 206f 7220  .Key.Key_Tab or 
+0000dde0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+0000ddf0: 742e 4b65 792e 4b65 795f 4261 636b 7461  t.Key.Key_Backta
+0000de00: 623a 0a20 2020 2020 2020 2020 2020 2069  b:.            i
+0000de10: 6620 7365 6c66 2e73 656e 742e 6861 7346  f self.sent.hasF
+0000de20: 6f63 7573 2829 3a0a 2020 2020 2020 2020  ocus():.        
+0000de30: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000de40: 6562 7567 2822 4672 6f6d 2073 656e 7422  ebug("From sent"
 0000de50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000de60: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
-0000de70: 7665 7274 7970 6520 3d3d 2031 3a0a 2020  vertype == 1:.  
-0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de90: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000dea0: 2866 225c 7831 6232 7b73 656c 662e 6377  (f"\x1b2{self.cw
-0000deb0: 2e73 7065 6564 7d22 290a 2020 2020 2020  .speed}").      
-0000dec0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000ded0: 662e 6377 2e73 6572 7665 7274 7970 6520  f.cw.servertype 
-0000dee0: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
-0000def0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000df00: 772e 7365 745f 7769 6e6b 6579 6572 5f73  w.set_winkeyer_s
-0000df10: 7065 6564 2873 656c 662e 6377 5f73 7065  peed(self.cw_spe
-0000df20: 6564 2e76 616c 7565 2829 290a 2020 2020  ed.value()).    
-0000df30: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000df40: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-0000df50: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
-0000df60: 4b65 795f 5461 6220 6f72 2065 7665 6e74  Key_Tab or event
-0000df70: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-0000df80: 2e4b 6579 5f42 6163 6b74 6162 3a0a 2020  .Key_Backtab:.  
-0000df90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000dfa0: 662e 7365 6e74 2e68 6173 466f 6375 7328  f.sent.hasFocus(
-0000dfb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000dfc0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000dfd0: 2246 726f 6d20 7365 6e74 2229 0a20 2020  "From sent").   
-0000dfe0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000dff0: 6d6f 6469 6669 6572 203d 3d20 5174 2e53  modifier == Qt.S
-0000e000: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
-0000e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e020: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
-0000e030: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
-0000e040: 656c 662e 7365 6e74 290a 2020 2020 2020  elf.sent).      
-0000e050: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000e060: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
-0000e070: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e080: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
-0000e090: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-0000e0a0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000e0b0: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
-0000e0c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e0d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e0e0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-0000e0f0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-0000e100: 6e65 7874 2e67 6574 2873 656c 662e 7365  next.get(self.se
-0000e110: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
-0000e120: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-0000e130: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 6e65 7874 5f74 6162 2e64 6573 656c 6563  next_tab.deselec
-0000e160: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0000e170: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-0000e180: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-0000e190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e1a0: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
-0000e1b0: 6620 7365 6c66 2e72 6563 6569 7665 2e68  f self.receive.h
-0000e1c0: 6173 466f 6375 7328 293a 0a20 2020 2020  asFocus():.     
-0000e1d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000e1e0: 722e 6465 6275 6728 2246 726f 6d20 7265  r.debug("From re
-0000e1f0: 6365 6976 6522 290a 2020 2020 2020 2020  ceive").        
-0000e200: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
-0000e210: 6965 7220 3d3d 2051 742e 5368 6966 744d  ier == Qt.ShiftM
-0000e220: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-0000e230: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0000e240: 765f 7461 6220 3d20 7365 6c66 2e74 6162  v_tab = self.tab
-0000e250: 5f70 7265 762e 6765 7428 7365 6c66 2e72  _prev.get(self.r
-0000e260: 6563 6569 7665 290a 2020 2020 2020 2020  eceive).        
-0000e270: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-0000e280: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
-0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2a0: 2020 2020 7072 6576 5f74 6162 2e64 6573      prev_tab.des
-0000e2b0: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
-0000e2c0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-0000e2d0: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e300: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-0000e310: 6162 203d 2073 656c 662e 7461 625f 6e65  ab = self.tab_ne
-0000e320: 7874 2e67 6574 2873 656c 662e 7265 6365  xt.get(self.rece
-0000e330: 6976 6529 0a20 2020 2020 2020 2020 2020  ive).           
-0000e340: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-0000e350: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e370: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
-0000e380: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-0000e390: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-0000e3a0: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-0000e3b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000e3c0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-0000e3d0: 6966 2073 656c 662e 6f74 6865 725f 312e  if self.other_1.
-0000e3e0: 6861 7346 6f63 7573 2829 3a0a 2020 2020  hasFocus():.    
-0000e3f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000e400: 6572 2e64 6562 7567 2822 4672 6f6d 206f  er.debug("From o
-0000e410: 7468 6572 5f31 2229 0a20 2020 2020 2020  ther_1").       
-0000e420: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
-0000e430: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
-0000e440: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
-0000e450: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000e460: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
-0000e470: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
-0000e480: 6f74 6865 725f 3129 0a20 2020 2020 2020  other_1).       
-0000e490: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0000e4a0: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
-0000e4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e4c0: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
-0000e4d0: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-0000e4e0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0000e4f0: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
-0000e500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e510: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e520: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-0000e530: 7461 6220 3d20 7365 6c66 2e74 6162 5f6e  tab = self.tab_n
-0000e540: 6578 742e 6765 7428 7365 6c66 2e6f 7468  ext.get(self.oth
-0000e550: 6572 5f31 290a 2020 2020 2020 2020 2020  er_1).          
-0000e560: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-0000e570: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
-0000e5a0: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
-0000e5b0: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-0000e5c0: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000e5e0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-0000e5f0: 2069 6620 7365 6c66 2e6f 7468 6572 5f32   if self.other_2
-0000e600: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
-0000e610: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000e620: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
-0000e630: 6f74 6865 725f 3222 290a 2020 2020 2020  other_2").      
-0000e640: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-0000e650: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
-0000e660: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000e680: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
-0000e690: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
-0000e6a0: 2e6f 7468 6572 5f32 290a 2020 2020 2020  .other_2).      
-0000e6b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000e6c0: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+0000de60: 2020 6966 206d 6f64 6966 6965 7220 3d3d    if modifier ==
+0000de70: 2051 742e 5368 6966 744d 6f64 6966 6965   Qt.ShiftModifie
+0000de80: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0000de90: 2020 2020 2020 2070 7265 765f 7461 6220         prev_tab 
+0000dea0: 3d20 7365 6c66 2e74 6162 5f70 7265 762e  = self.tab_prev.
+0000deb0: 6765 7428 7365 6c66 2e73 656e 7429 0a20  get(self.sent). 
+0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ded0: 2020 2070 7265 765f 7461 622e 7365 7446     prev_tab.setF
+0000dee0: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+0000def0: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
+0000df00: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
+0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df20: 2020 2070 7265 765f 7461 622e 656e 6428     prev_tab.end(
+0000df30: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+0000df40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 206e 6578 745f 7461 6220 3d20 7365 6c66   next_tab = self
+0000df70: 2e74 6162 5f6e 6578 742e 6765 7428 7365  .tab_next.get(se
+0000df80: 6c66 2e73 656e 7429 0a20 2020 2020 2020  lf.sent).       
+0000df90: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+0000dfa0: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
+0000dfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dfc0: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
+0000dfd0: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+0000dfe0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+0000dff0: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
+0000e000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e010: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000e020: 2020 2020 6966 2073 656c 662e 7265 6365      if self.rece
+0000e030: 6976 652e 6861 7346 6f63 7573 2829 3a0a  ive.hasFocus():.
+0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e050: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
+0000e060: 6f6d 2072 6563 6569 7665 2229 0a20 2020  om receive").   
+0000e070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e080: 6d6f 6469 6669 6572 203d 3d20 5174 2e53  modifier == Qt.S
+0000e090: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
+0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0b0: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
+0000e0c0: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
+0000e0d0: 656c 662e 7265 6365 6976 6529 0a20 2020  elf.receive).   
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2070 7265 765f 7461 622e 7365 7446 6f63   prev_tab.setFoc
+0000e100: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
+0000e110: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+0000e120: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
+0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e140: 2070 7265 765f 7461 622e 656e 6428 4661   prev_tab.end(Fa
+0000e150: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+0000e160: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000e170: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e180: 6578 745f 7461 6220 3d20 7365 6c66 2e74  ext_tab = self.t
+0000e190: 6162 5f6e 6578 742e 6765 7428 7365 6c66  ab_next.get(self
+0000e1a0: 2e72 6563 6569 7665 290a 2020 2020 2020  .receive).      
+0000e1b0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000e1c0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
+0000e1d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e1e0: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
+0000e1f0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+0000e200: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000e210: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
+0000e220: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e230: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000e240: 2020 2020 2069 6620 7365 6c66 2e6f 7468       if self.oth
+0000e250: 6572 5f31 2e68 6173 466f 6375 7328 293a  er_1.hasFocus():
+0000e260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e270: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000e280: 726f 6d20 6f74 6865 725f 3122 290a 2020  rom other_1").  
+0000e290: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000e2a0: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
+0000e2b0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
+0000e2e0: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
+0000e2f0: 7365 6c66 2e6f 7468 6572 5f31 290a 2020  self.other_1).  
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
+0000e320: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+0000e330: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+0000e340: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e360: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
+0000e370: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+0000e380: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3a0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
+0000e3b0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
+0000e3c0: 662e 6f74 6865 725f 3129 0a20 2020 2020  f.other_1).     
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e3e0: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
+0000e3f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000e400: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+0000e410: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+0000e420: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e430: 6578 745f 7461 622e 656e 6428 4661 6c73  ext_tab.end(Fals
+0000e440: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000e450: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000e460: 2020 2020 2020 6966 2073 656c 662e 6f74        if self.ot
+0000e470: 6865 725f 322e 6861 7346 6f63 7573 2829  her_2.hasFocus()
+0000e480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e490: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000e4a0: 4672 6f6d 206f 7468 6572 5f32 2229 0a20  From other_2"). 
+0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e4c0: 6620 6d6f 6469 6669 6572 203d 3d20 5174  f modifier == Qt
+0000e4d0: 2e53 6869 6674 4d6f 6469 6669 6572 3a0a  .ShiftModifier:.
+0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4f0: 2020 2020 7072 6576 5f74 6162 203d 2073      prev_tab = s
+0000e500: 656c 662e 7461 625f 7072 6576 2e67 6574  elf.tab_prev.get
+0000e510: 2873 656c 662e 6f74 6865 725f 3229 0a20  (self.other_2). 
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2020 2070 7265 765f 7461 622e 7365 7446     prev_tab.setF
+0000e540: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+0000e550: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
+0000e560: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
+0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e580: 2020 2070 7265 765f 7461 622e 656e 6428     prev_tab.end(
+0000e590: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+0000e5a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 206e 6578 745f 7461 6220 3d20 7365 6c66   next_tab = self
+0000e5d0: 2e74 6162 5f6e 6578 742e 6765 7428 7365  .tab_next.get(se
+0000e5e0: 6c66 2e6f 7468 6572 5f32 290a 2020 2020  lf.other_2).    
+0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e600: 6e65 7874 5f74 6162 2e73 6574 466f 6375  next_tab.setFocu
+0000e610: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+0000e620: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+0000e630: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 6e65 7874 5f74 6162 2e65 6e64 2846 616c  next_tab.end(Fal
+0000e660: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+0000e670: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000e680: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000e690: 616c 6c73 6967 6e2e 6861 7346 6f63 7573  allsign.hasFocus
+0000e6a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000e6b0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000e6c0: 2822 4672 6f6d 2063 616c 6c73 6967 6e22  ("From callsign"
 0000e6d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e6e0: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
-0000e6f0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-0000e700: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000e710: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
-0000e720: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e730: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e740: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-0000e750: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-0000e760: 6e65 7874 2e67 6574 2873 656c 662e 6f74  next.get(self.ot
-0000e770: 6865 725f 3229 0a20 2020 2020 2020 2020  her_2).         
-0000e780: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-0000e790: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 2020 206e 6578 745f 7461 622e 6465 7365     next_tab.dese
-0000e7c0: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-0000e7d0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-0000e7e0: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e800: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000e810: 2020 6966 2073 656c 662e 6361 6c6c 7369    if self.callsi
-0000e820: 676e 2e68 6173 466f 6375 7328 293a 0a20  gn.hasFocus():. 
-0000e830: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000e840: 6f67 6765 722e 6465 6275 6728 2246 726f  ogger.debug("Fro
-0000e850: 6d20 6361 6c6c 7369 676e 2229 0a20 2020  m callsign").   
-0000e860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e870: 662e 6368 6563 6b5f 6361 6c6c 7369 676e  f.check_callsign
-0000e880: 2873 656c 662e 6361 6c6c 7369 676e 2e74  (self.callsign.t
-0000e890: 6578 7428 2929 0a20 2020 2020 2020 2020  ext()).         
-0000e8a0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000e8b0: 6865 636b 5f64 7570 6528 7365 6c66 2e63  heck_dupe(self.c
-0000e8c0: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
-0000e8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e8e0: 2020 2020 2073 656c 662e 6475 7065 5f69       self.dupe_i
-0000e8f0: 6e64 6963 6174 6f72 2e73 686f 7728 290a  ndicator.show().
-0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e910: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e920: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000e930: 7570 655f 696e 6469 6361 746f 722e 6869  upe_indicator.hi
-0000e940: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-0000e950: 2020 2020 2069 6620 6d6f 6469 6669 6572       if modifier
-0000e960: 203d 3d20 5174 2e53 6869 6674 4d6f 6469   == Qt.ShiftModi
-0000e970: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-0000e980: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-0000e990: 6162 203d 2073 656c 662e 7461 625f 7072  ab = self.tab_pr
-0000e9a0: 6576 2e67 6574 2873 656c 662e 6361 6c6c  ev.get(self.call
-0000e9b0: 7369 676e 290a 2020 2020 2020 2020 2020  sign).          
-0000e9c0: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-0000e9d0: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 7072 6576 5f74 6162 2e64 6573 656c    prev_tab.desel
-0000ea00: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
-0000ea10: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-0000ea20: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000ea40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000ea50: 2020 2020 2020 2020 7465 7874 203d 2073          text = s
-0000ea60: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-0000ea70: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0000ea80: 2020 2020 2020 2020 7465 7874 203d 2074          text = t
-0000ea90: 6578 742e 7570 7065 7228 290a 2020 2020  ext.upper().    
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 5f74 6865 7468 7265 6164 203d 2074 6872  _thethread = thr
-0000eac0: 6561 6469 6e67 2e54 6872 6561 6428 0a20  eading.Thread(. 
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2020 2020 2020 2074 6172 6765 743d 7365         target=se
-0000eaf0: 6c66 2e63 6865 636b 5f63 616c 6c73 6967  lf.check_callsig
-0000eb00: 6e32 2c0a 2020 2020 2020 2020 2020 2020  n2,.            
-0000eb10: 2020 2020 2020 2020 2020 2020 6172 6773              args
-0000eb20: 3d28 7465 7874 2c29 2c0a 2020 2020 2020  =(text,),.      
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb40: 2020 6461 656d 6f6e 3d54 7275 652c 0a20    daemon=True,. 
-0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb60: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000eb70: 2020 2020 2020 2020 205f 7468 6574 6872           _thethr
-0000eb80: 6561 642e 7374 6172 7428 290a 2020 2020  ead.start().    
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
-0000ebb0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
-0000ebc0: 662e 6361 6c6c 7369 676e 290a 2020 2020  f.callsign).    
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebe0: 6e65 7874 5f74 6162 2e73 6574 466f 6375  next_tab.setFocu
-0000ebf0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000ec00: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-0000ec10: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec30: 6e65 7874 5f74 6162 2e65 6e64 2846 616c  next_tab.end(Fal
-0000ec40: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0000ec50: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000ec60: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-0000ec70: 2920 3d3d 2051 742e 4b65 795f 4631 3a0a  ) == Qt.Key_F1:.
-0000ec80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ec90: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
-0000eca0: 6e5f 6b65 7928 7365 6c66 2e46 3129 0a20  n_key(self.F1). 
-0000ecb0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-0000ecc0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-0000ecd0: 4632 3a0a 2020 2020 2020 2020 2020 2020  F2:.            
-0000ece0: 7365 6c66 2e70 726f 6365 7373 5f66 756e  self.process_fun
-0000ecf0: 6374 696f 6e5f 6b65 7928 7365 6c66 2e46  ction_key(self.F
-0000ed00: 3229 0a20 2020 2020 2020 2069 6620 6576  2).        if ev
-0000ed10: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-0000ed20: 4b65 795f 4633 3a0a 2020 2020 2020 2020  Key_F3:.        
-0000ed30: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
-0000ed40: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
-0000ed50: 6c66 2e46 3329 0a20 2020 2020 2020 2069  lf.F3).        i
-0000ed60: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-0000ed70: 2051 742e 4b65 795f 4634 3a0a 2020 2020   Qt.Key_F4:.    
-0000ed80: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000ed90: 6365 7373 5f66 756e 6374 696f 6e5f 6b65  cess_function_ke
-0000eda0: 7928 7365 6c66 2e46 3429 0a20 2020 2020  y(self.F4).     
-0000edb0: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-0000edc0: 2920 3d3d 2051 742e 4b65 795f 4635 3a0a  ) == Qt.Key_F5:.
-0000edd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ede0: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
-0000edf0: 6e5f 6b65 7928 7365 6c66 2e46 3529 0a20  n_key(self.F5). 
-0000ee00: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-0000ee10: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-0000ee20: 4636 3a0a 2020 2020 2020 2020 2020 2020  F6:.            
-0000ee30: 7365 6c66 2e70 726f 6365 7373 5f66 756e  self.process_fun
-0000ee40: 6374 696f 6e5f 6b65 7928 7365 6c66 2e46  ction_key(self.F
-0000ee50: 3629 0a20 2020 2020 2020 2069 6620 6576  6).        if ev
-0000ee60: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-0000ee70: 4b65 795f 4637 3a0a 2020 2020 2020 2020  Key_F7:.        
-0000ee80: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
-0000ee90: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
-0000eea0: 6c66 2e46 3729 0a20 2020 2020 2020 2069  lf.F7).        i
-0000eeb0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-0000eec0: 2051 742e 4b65 795f 4638 3a0a 2020 2020   Qt.Key_F8:.    
-0000eed0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000eee0: 6365 7373 5f66 756e 6374 696f 6e5f 6b65  cess_function_ke
-0000eef0: 7928 7365 6c66 2e46 3829 0a20 2020 2020  y(self.F8).     
-0000ef00: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-0000ef10: 2920 3d3d 2051 742e 4b65 795f 4639 3a0a  ) == Qt.Key_F9:.
-0000ef20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ef30: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
-0000ef40: 6e5f 6b65 7928 7365 6c66 2e46 3929 0a20  n_key(self.F9). 
-0000ef50: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-0000ef60: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-0000ef70: 4631 303a 0a20 2020 2020 2020 2020 2020  F10:.           
-0000ef80: 2073 656c 662e 7072 6f63 6573 735f 6675   self.process_fu
-0000ef90: 6e63 7469 6f6e 5f6b 6579 2873 656c 662e  nction_key(self.
-0000efa0: 4631 3029 0a20 2020 2020 2020 2069 6620  F10).        if 
-0000efb0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-0000efc0: 742e 4b65 795f 4631 313a 0a20 2020 2020  t.Key_F11:.     
-0000efd0: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
-0000efe0: 6573 735f 6675 6e63 7469 6f6e 5f6b 6579  ess_function_key
-0000eff0: 2873 656c 662e 4631 3129 0a20 2020 2020  (self.F11).     
-0000f000: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-0000f010: 2920 3d3d 2051 742e 4b65 795f 4631 323a  ) == Qt.Key_F12:
-0000f020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f030: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
-0000f040: 6f6e 5f6b 6579 2873 656c 662e 4631 3229  on_key(self.F12)
-0000f050: 0a0a 2020 2020 6465 6620 7365 745f 7769  ..    def set_wi
-0000f060: 6e64 6f77 5f74 6974 6c65 2873 656c 6629  ndow_title(self)
-0000f070: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000f080: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000f090: 7420 7769 6e64 6f77 2074 6974 6c65 2062  t window title b
-0000f0a0: 6173 6564 206f 6e20 6375 7272 656e 7420  ased on current 
-0000f0b0: 7374 6174 652e 0a20 2020 2020 2020 2022  state..        "
-0000f0c0: 2222 0a0a 2020 2020 2020 2020 7666 6f61  ""..        vfoa
-0000f0d0: 203d 2073 656c 662e 7261 6469 6f5f 7374   = self.radio_st
-0000f0e0: 6174 652e 6765 7428 2276 666f 6122 2c20  ate.get("vfoa", 
-0000f0f0: 2222 290a 2020 2020 2020 2020 6966 2076  "").        if v
-0000f100: 666f 613a 0a20 2020 2020 2020 2020 2020  foa:.           
-0000f110: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000f120: 2020 2020 2020 7666 6f61 203d 2069 6e74        vfoa = int
-0000f130: 2876 666f 6129 202f 2031 3030 300a 2020  (vfoa) / 1000.  
-0000f140: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000f150: 2056 616c 7565 4572 726f 723a 0a20 2020   ValueError:.   
-0000f160: 2020 2020 2020 2020 2020 2020 2076 666f               vfo
-0000f170: 6120 3d20 302e 300a 2020 2020 2020 2020  a = 0.0.        
-0000f180: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000f190: 2020 7666 6f61 203d 2030 2e30 0a20 2020    vfoa = 0.0.   
-0000f1a0: 2020 2020 2063 6f6e 7465 7374 5f6e 616d       contest_nam
-0000f1b0: 6520 3d20 2222 0a20 2020 2020 2020 2069  e = "".        i
-0000f1c0: 6620 7365 6c66 2e63 6f6e 7465 7374 3a0a  f self.contest:.
-0000f1d0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000f1e0: 6573 745f 6e61 6d65 203d 2073 656c 662e  est_name = self.
-0000f1f0: 636f 6e74 6573 742e 6e61 6d65 0a20 2020  contest.name.   
-0000f200: 2020 2020 206c 696e 6520 3d20 280a 2020       line = (.  
-0000f210: 2020 2020 2020 2020 2020 6622 7666 6f61            f"vfoa
-0000f220: 3a7b 726f 756e 6428 7666 6f61 2c32 297d  :{round(vfoa,2)}
-0000f230: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
-0000f240: 226d 6f64 653a 7b73 656c 662e 7261 6469  "mode:{self.radi
-0000f250: 6f5f 7374 6174 652e 6765 7428 276d 6f64  o_state.get('mod
-0000f260: 6527 2c20 2727 297d 2022 0a20 2020 2020  e', '')} ".     
-0000f270: 2020 2020 2020 2066 224f 503a 7b73 656c         f"OP:{sel
-0000f280: 662e 6375 7272 656e 745f 6f70 7d20 7b63  f.current_op} {c
-0000f290: 6f6e 7465 7374 5f6e 616d 657d 2022 0a20  ontest_name} ". 
-0000f2a0: 2020 2020 2020 2020 2020 2066 222d 204e             f"- N
-0000f2b0: 6f74 314d 4d20 767b 5f5f 7665 7273 696f  ot1MM v{__versio
-0000f2c0: 6e5f 5f7d 220a 2020 2020 2020 2020 290a  n__}".        ).
-0000f2d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000f2e0: 5769 6e64 6f77 5469 746c 6528 6c69 6e65  WindowTitle(line
-0000f2f0: 290a 0a20 2020 2064 6566 2073 656e 645f  )..    def send_
-0000f300: 776f 726b 6564 5f6c 6973 7428 7365 6c66  worked_list(self
-0000f310: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000f320: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-0000f330: 656e 6420 6d65 7373 6167 6520 636f 6e74  end message cont
-0000f340: 6169 6e69 6e67 2077 6f72 6b65 6420 636f  aining worked co
-0000f350: 6e74 6163 7473 2061 6e64 2062 616e 6473  ntacts and bands
-0000f360: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000f370: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000f380: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000f390: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
-0000f3a0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0000f3b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0000f3c0: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
-0000f3d0: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-0000f3e0: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
-0000f3f0: 6422 5d20 3d20 2257 4f52 4b45 4422 0a20  d"] = "WORKED". 
-0000f400: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-0000f410: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-0000f420: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-0000f430: 636d 645b 2277 6f72 6b65 6422 5d20 3d20  cmd["worked"] = 
-0000f440: 7365 6c66 2e77 6f72 6b65 645f 6c69 7374  self.worked_list
-0000f450: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000f460: 6465 6275 6728 2225 7322 2c20 6622 7b63  debug("%s", f"{c
-0000f470: 6d64 7d22 290a 2020 2020 2020 2020 7365  md}").        se
-0000f480: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-0000f490: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-0000f4a0: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
-0000f4b0: 6620 636c 6561 7269 6e70 7574 7328 7365  f clearinputs(se
-0000f4c0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000f4d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f4e0: 2043 6c65 6172 7320 7468 6520 7465 7874   Clears the text
-0000f4f0: 2069 6e70 7574 2066 6965 6c64 7320 616e   input fields an
-0000f500: 6420 7365 7473 2066 6f63 7573 2074 6f20  d sets focus to 
-0000f510: 6361 6c6c 7369 676e 2066 6965 6c64 2e0a  callsign field..
-0000f520: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000f530: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000f540: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-0000f550: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
-0000f560: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0000f570: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-0000f580: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
-0000f590: 2020 2020 2020 2073 656c 662e 6475 7065         self.dupe
-0000f5a0: 5f69 6e64 6963 6174 6f72 2e68 6964 6528  _indicator.hide(
-0000f5b0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000f5c0: 6f6e 7461 6374 203d 2073 656c 662e 6461  ontact = self.da
-0000f5d0: 7461 6261 7365 2e65 6d70 7479 5f63 6f6e  tabase.empty_con
-0000f5e0: 7461 6374 0a20 2020 2020 2020 2073 656c  tact.        sel
-0000f5f0: 662e 6865 6164 696e 675f 6469 7374 616e  f.heading_distan
-0000f600: 6365 2e73 6574 5465 7874 2822 2229 0a20  ce.setText(""). 
-0000f610: 2020 2020 2020 2073 656c 662e 6478 5f65         self.dx_e
-0000f620: 6e74 6974 792e 7365 7454 6578 7428 2222  ntity.setText(""
-0000f630: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000f640: 662e 636f 6e74 6573 743a 0a20 2020 2020  f.contest:.     
-0000f650: 2020 2020 2020 206d 756c 7473 203d 2073         mults = s
-0000f660: 656c 662e 636f 6e74 6573 742e 7368 6f77  elf.contest.show
-0000f670: 5f6d 756c 7473 2873 656c 6629 0a20 2020  _mults(self).   
-0000f680: 2020 2020 2020 2020 2071 736f 7320 3d20           qsos = 
-0000f690: 7365 6c66 2e63 6f6e 7465 7374 2e73 686f  self.contest.sho
-0000f6a0: 775f 7173 6f28 7365 6c66 290a 2020 2020  w_qso(self).    
-0000f6b0: 2020 2020 2020 2020 6d75 6c74 7374 7269          multstri
-0000f6c0: 6e67 203d 2066 227b 7173 6f73 7d2f 7b6d  ng = f"{qsos}/{m
-0000f6d0: 756c 7473 7d22 0a20 2020 2020 2020 2020  ults}".         
-0000f6e0: 2020 2073 656c 662e 6d75 6c74 732e 7365     self.mults.se
-0000f6f0: 7454 6578 7428 6d75 6c74 7374 7269 6e67  tText(multstring
-0000f700: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
-0000f710: 6f72 6520 3d20 7365 6c66 2e63 6f6e 7465  ore = self.conte
-0000f720: 7374 2e63 616c 635f 7363 6f72 6528 7365  st.calc_score(se
-0000f730: 6c66 290a 2020 2020 2020 2020 2020 2020  lf).            
-0000f740: 7365 6c66 2e73 636f 7265 2e73 6574 5465  self.score.setTe
-0000f750: 7874 2873 7472 2873 636f 7265 2929 0a20  xt(str(score)). 
-0000f760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f770: 636f 6e74 6573 742e 7265 7365 745f 6c61  contest.reset_la
-0000f780: 6265 6c28 7365 6c66 290a 2020 2020 2020  bel(self).      
-0000f790: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
-0000f7a0: 636c 6561 7228 290a 2020 2020 2020 2020  clear().        
-0000f7b0: 6966 2073 656c 662e 6375 7272 656e 745f  if self.current_
-0000f7c0: 6d6f 6465 203d 3d20 2243 5722 3a0a 2020  mode == "CW":.  
-0000f7d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000f7e0: 656e 742e 7365 7454 6578 7428 2235 3939  ent.setText("599
-0000f7f0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-0000f800: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
-0000f810: 6578 7428 2235 3939 2229 0a20 2020 2020  ext("599").     
-0000f820: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f830: 2020 2020 2073 656c 662e 7365 6e74 2e73       self.sent.s
-0000f840: 6574 5465 7874 2822 3539 2229 0a20 2020  etText("59").   
-0000f850: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000f860: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
-0000f870: 3922 290a 2020 2020 2020 2020 7365 6c66  9").        self
-0000f880: 2e6f 7468 6572 5f31 2e63 6c65 6172 2829  .other_1.clear()
-0000f890: 0a20 2020 2020 2020 2073 656c 662e 6f74  .        self.ot
-0000f8a0: 6865 725f 322e 636c 6561 7228 290a 2020  her_2.clear().  
-0000f8b0: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
-0000f8c0: 6967 6e2e 7365 7446 6f63 7573 2829 0a20  ign.setFocus(). 
-0000f8d0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-0000f8e0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-0000f8f0: 225d 203d 2022 4341 4c4c 4348 414e 4745  "] = "CALLCHANGE
-0000f900: 4422 0a20 2020 2020 2020 2063 6d64 5b22  D".        cmd["
-0000f910: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-0000f920: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-0000f930: 2020 2020 636d 645b 2263 616c 6c22 5d20      cmd["call"] 
-0000f940: 3d20 2222 0a20 2020 2020 2020 2073 656c  = "".        sel
-0000f950: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-0000f960: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-0000f970: 6f6e 2863 6d64 290a 0a20 2020 2064 6566  on(cmd)..    def
-0000f980: 2073 6176 655f 636f 6e74 6163 7428 7365   save_contact(se
-0000f990: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000f9a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f9b0: 2053 6176 6520 636f 6e74 6163 7420 746f   Save contact to
-0000f9c0: 2064 6174 6162 6173 652e 0a0a 2020 2020   database...    
-0000f9d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000f9e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000f9f0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
-0000fa00: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000fa10: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000fa20: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-0000fa30: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000fa40: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000fa50: 7361 7669 6e67 2063 6f6e 7461 6374 2229  saving contact")
-0000fa60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000fa70: 2e63 6f6e 7465 7374 2069 7320 4e6f 6e65  .contest is None
-0000fa80: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fa90: 6c66 2e73 686f 775f 6d65 7373 6167 655f  lf.show_message_
-0000faa0: 626f 7828 2259 6f75 2068 6176 6520 6e6f  box("You have no
-0000fab0: 2063 6f6e 7465 7374 2064 6566 696e 6564   contest defined
-0000fac0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0000fad0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000fae0: 6620 6c65 6e28 7365 6c66 2e63 616c 6c73  f len(self.calls
-0000faf0: 6967 6e2e 7465 7874 2829 2920 3c20 333a  ign.text()) < 3:
-0000fb00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000fb10: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
-0000fb20: 6f74 2061 6e79 2863 6861 722e 6973 6469  ot any(char.isdi
-0000fb30: 6769 7428 2920 666f 7220 6368 6172 2069  git() for char i
-0000fb40: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
-0000fb50: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
-0000fb60: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000fb70: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
-0000fb80: 6861 722e 6973 616c 7068 6128 2920 666f  har.isalpha() fo
-0000fb90: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
-0000fba0: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
-0000fbb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000fbc0: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
-0000fbd0: 2e63 6f6e 7461 6374 5b22 5453 225d 203d  .contact["TS"] =
-0000fbe0: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
-0000fbf0: 6d65 2e6e 6f77 2864 6174 6574 696d 652e  me.now(datetime.
-0000fc00: 7469 6d65 7a6f 6e65 2e75 7463 292e 6973  timezone.utc).is
-0000fc10: 6f66 6f72 6d61 7428 0a20 2020 2020 2020  oformat(.       
-0000fc20: 2020 2020 2022 2022 0a20 2020 2020 2020       " ".       
-0000fc30: 2029 5b3a 3139 5d0a 2020 2020 2020 2020   )[:19].        
-0000fc40: 7365 6c66 2e63 6f6e 7461 6374 5b22 4361  self.contact["Ca
-0000fc50: 6c6c 225d 203d 2073 656c 662e 6361 6c6c  ll"] = self.call
-0000fc60: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
-0000fc70: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-0000fc80: 5b22 4672 6571 225d 203d 2072 6f75 6e64  ["Freq"] = round
-0000fc90: 2866 6c6f 6174 2873 656c 662e 7261 6469  (float(self.radi
-0000fca0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
-0000fcb0: 6122 2c20 302e 3029 2920 2f20 3130 3030  a", 0.0)) / 1000
-0000fcc0: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
-0000fcd0: 662e 636f 6e74 6163 745b 2251 5358 4672  f.contact["QSXFr
-0000fce0: 6571 225d 203d 2072 6f75 6e64 280a 2020  eq"] = round(.  
-0000fcf0: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-0000fd00: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000fd10: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
-0000fd20: 2929 202f 2031 3030 302c 2032 0a20 2020  )) / 1000, 2.   
-0000fd30: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0000fd40: 656c 662e 636f 6e74 6163 745b 224d 6f64  elf.contact["Mod
-0000fd50: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
-0000fd60: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0000fd70: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
-0000fd80: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
-0000fd90: 7465 7374 4e61 6d65 225d 203d 2073 656c  testName"] = sel
-0000fda0: 662e 636f 6e74 6573 742e 6361 6272 696c  f.contest.cabril
-0000fdb0: 6c6f 5f6e 616d 650a 2020 2020 2020 2020  lo_name.        
-0000fdc0: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-0000fdd0: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
-0000fde0: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
-0000fdf0: 7374 222c 2022 3022 290a 2020 2020 2020  st", "0").      
-0000fe00: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-0000fe10: 5374 6174 696f 6e50 7265 6669 7822 5d20  StationPrefix"] 
-0000fe20: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
-0000fe30: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
-0000fe40: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0000fe50: 6163 745b 2257 5058 5072 6566 6978 225d  act["WPXPrefix"]
-0000fe60: 203d 2063 616c 6375 6c61 7465 5f77 7078   = calculate_wpx
-0000fe70: 5f70 7265 6669 7828 7365 6c66 2e63 616c  _prefix(self.cal
-0000fe80: 6c73 6967 6e2e 7465 7874 2829 290a 2020  lsign.text()).  
-0000fe90: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-0000fea0: 6374 5b22 4973 5275 6e51 534f 225d 203d  ct["IsRunQSO"] =
-0000feb0: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
-0000fec0: 6e5f 7275 6e2e 6973 4368 6563 6b65 6428  n_run.isChecked(
-0000fed0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000fee0: 6f6e 7461 6374 5b22 4f70 6572 6174 6f72  ontact["Operator
-0000fef0: 225d 203d 2073 656c 662e 6375 7272 656e  "] = self.curren
-0000ff00: 745f 6f70 0a20 2020 2020 2020 2073 656c  t_op.        sel
-0000ff10: 662e 636f 6e74 6163 745b 224e 6574 4269  f.contact["NetBi
-0000ff20: 6f73 4e61 6d65 225d 203d 2073 6f63 6b65  osName"] = socke
-0000ff30: 742e 6765 7468 6f73 746e 616d 6528 290a  t.gethostname().
-0000ff40: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000ff50: 7461 6374 5b22 4973 4f72 6967 696e 616c  tact["IsOriginal
-0000ff60: 225d 203d 2031 0a20 2020 2020 2020 2073  "] = 1.        s
-0000ff70: 656c 662e 636f 6e74 6163 745b 2249 4422  elf.contact["ID"
-0000ff80: 5d20 3d20 7575 6964 2e75 7569 6434 2829  ] = uuid.uuid4()
-0000ff90: 2e68 6578 0a20 2020 2020 2020 2073 656c  .hex.        sel
-0000ffa0: 662e 636f 6e74 6573 742e 7365 745f 636f  f.contest.set_co
-0000ffb0: 6e74 6163 745f 7661 7273 2873 656c 6629  ntact_vars(self)
-0000ffc0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000ffd0: 6e74 6163 745b 2250 6f69 6e74 7322 5d20  ntact["Points"] 
-0000ffe0: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e70  = self.contest.p
-0000fff0: 6f69 6e74 7328 7365 6c66 290a 2020 2020  oints(self).    
-00010000: 2020 2020 6465 6275 675f 6f75 7470 7574      debug_output
-00010010: 203d 2066 227b 7365 6c66 2e63 6f6e 7461   = f"{self.conta
-00010020: 6374 7d22 0a20 2020 2020 2020 206c 6f67  ct}".        log
-00010030: 6765 722e 6465 6275 6728 6465 6275 675f  ger.debug(debug_
-00010040: 6f75 7470 7574 290a 0a20 2020 2020 2020  output)..       
-00010050: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
-00010060: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00010070: 722e 6465 6275 6728 2270 6163 6b65 7473  r.debug("packets
-00010080: 2025 7322 2c20 6622 7b73 656c 662e 6e31   %s", f"{self.n1
-00010090: 6d6d 2e73 656e 645f 636f 6e74 6163 745f  mm.send_contact_
-000100a0: 7061 636b 6574 737d 2229 0a20 2020 2020  packets}").     
-000100b0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000100c0: 316d 6d2e 7365 6e64 5f63 6f6e 7461 6374  1mm.send_contact
-000100d0: 5f70 6163 6b65 7473 3a0a 2020 2020 2020  _packets:.      
-000100e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000100f0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-00010100: 5b22 7469 6d65 7374 616d 7022 5d20 3d20  ["timestamp"] = 
-00010110: 7365 6c66 2e63 6f6e 7461 6374 5b22 5453  self.contact["TS
-00010120: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00010130: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
-00010140: 7461 6374 5f69 6e66 6f5b 226f 6c64 6361  tact_info["oldca
-00010150: 6c6c 225d 203d 2073 656c 662e 6e31 6d6d  ll"] = self.n1mm
-00010160: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2263  .contact_info["c
-00010170: 616c 6c22 5d20 3d20 280a 2020 2020 2020  all"] = (.      
-00010180: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010190: 6c66 2e63 6f6e 7461 6374 5b22 4361 6c6c  lf.contact["Call
-000101a0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-000101b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000101c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-000101d0: 6f6e 7461 6374 5f69 6e66 6f5b 2274 7866  ontact_info["txf
-000101e0: 7265 7122 5d20 3d20 7365 6c66 2e6e 316d  req"] = self.n1m
-000101f0: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-00010200: 7278 6672 6571 225d 203d 2028 0a20 2020  rxfreq"] = (.   
-00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010220: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
-00010230: 5f69 6e66 6f5b 2246 7265 7122 5d0a 2020  _info["Freq"].  
-00010240: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-00010270: 745f 696e 666f 5b22 6d6f 6465 225d 203d  t_info["mode"] =
-00010280: 2073 656c 662e 636f 6e74 6163 745b 224d   self.contact["M
-00010290: 6f64 6522 5d0a 2020 2020 2020 2020 2020  ode"].          
-000102a0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-000102b0: 636f 6e74 6163 745f 696e 666f 5b22 636f  contact_info["co
-000102c0: 6e74 6573 746e 616d 6522 5d20 3d20 7365  ntestname"] = se
-000102d0: 6c66 2e63 6f6e 7461 6374 5b0a 2020 2020  lf.contact[.    
-000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2243 6f6e 7465 7374 4e61 6d65 220a 2020  "ContestName".  
-00010300: 2020 2020 2020 2020 2020 2020 2020 5d2e                ].
-00010310: 7265 706c 6163 6528 222d 222c 2022 2229  replace("-", "")
-00010320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010330: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-00010340: 6374 5f69 6e66 6f5b 2263 6f6e 7465 7374  ct_info["contest
-00010350: 6e72 225d 203d 2073 656c 662e 636f 6e74  nr"] = self.cont
-00010360: 6163 745b 2243 6f6e 7465 7374 4e52 225d  act["ContestNR"]
-00010370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010380: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-00010390: 6374 5f69 6e66 6f5b 2273 7461 7469 6f6e  ct_info["station
-000103a0: 7072 6566 6978 225d 203d 2073 656c 662e  prefix"] = self.
-000103b0: 636f 6e74 6163 745b 2253 7461 7469 6f6e  contact["Station
-000103c0: 5072 6566 6978 225d 0a20 2020 2020 2020  Prefix"].       
-000103d0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-000103e0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-000103f0: 2277 7078 7072 6566 6978 225d 203d 2073  "wpxprefix"] = s
-00010400: 656c 662e 636f 6e74 6163 745b 2257 5058  elf.contact["WPX
-00010410: 5072 6566 6978 225d 0a20 2020 2020 2020  Prefix"].       
-00010420: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-00010430: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-00010440: 2249 7352 756e 5153 4f22 5d20 3d20 7365  "IsRunQSO"] = se
-00010450: 6c66 2e63 6f6e 7461 6374 5b22 4973 5275  lf.contact["IsRu
-00010460: 6e51 534f 225d 0a20 2020 2020 2020 2020  nQSO"].         
-00010470: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00010480: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 226f  .contact_info["o
-00010490: 7065 7261 746f 7222 5d20 3d20 7365 6c66  perator"] = self
-000104a0: 2e63 6f6e 7461 6374 5b22 4f70 6572 6174  .contact["Operat
-000104b0: 6f72 225d 0a20 2020 2020 2020 2020 2020  or"].           
-000104c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-000104d0: 6f6e 7461 6374 5f69 6e66 6f5b 226d 7963  ontact_info["myc
-000104e0: 616c 6c22 5d20 3d20 7365 6c66 2e63 6f6e  all"] = self.con
-000104f0: 7461 6374 5b22 4f70 6572 6174 6f72 225d  tact["Operator"]
-00010500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010510: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-00010520: 6374 5f69 6e66 6f5b 2253 7461 7469 6f6e  ct_info["Station
-00010530: 4e61 6d65 225d 203d 2073 656c 662e 6e31  Name"] = self.n1
-00010540: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-00010550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010560: 2020 2020 2022 4e65 7442 696f 734e 616d       "NetBiosNam
-00010570: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
-00010580: 2020 205d 203d 2073 656c 662e 636f 6e74     ] = self.cont
-00010590: 6163 745b 224e 6574 4269 6f73 4e61 6d65  act["NetBiosName
-000105a0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-000105b0: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
-000105c0: 7461 6374 5f69 6e66 6f5b 2249 734f 7269  tact_info["IsOri
-000105d0: 6769 6e61 6c22 5d20 3d20 7365 6c66 2e63  ginal"] = self.c
-000105e0: 6f6e 7461 6374 5b22 4973 4f72 6967 696e  ontact["IsOrigin
-000105f0: 616c 225d 0a20 2020 2020 2020 2020 2020  al"].           
-00010600: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-00010610: 6f6e 7461 6374 5f69 6e66 6f5b 2249 4422  ontact_info["ID"
-00010620: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
-00010630: 5b22 4944 225d 0a20 2020 2020 2020 2020  ["ID"].         
-00010640: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00010650: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2270  .contact_info["p
-00010660: 6f69 6e74 7322 5d20 3d20 7365 6c66 2e63  oints"] = self.c
-00010670: 6f6e 7461 6374 5b22 506f 696e 7473 225d  ontact["Points"]
-00010680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010690: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-000106a0: 6374 5f69 6e66 6f5b 2273 6e74 225d 203d  ct_info["snt"] =
-000106b0: 2073 656c 662e 636f 6e74 6163 745b 2253   self.contact["S
-000106c0: 4e54 225d 0a20 2020 2020 2020 2020 2020  NT"].           
-000106d0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-000106e0: 6f6e 7461 6374 5f69 6e66 6f5b 2272 6376  ontact_info["rcv
-000106f0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-00010700: 745b 2252 4356 225d 0a20 2020 2020 2020  t["RCV"].       
-00010710: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-00010720: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-00010730: 2273 6e74 6e72 225d 203d 2073 656c 662e  "sntnr"] = self.
-00010740: 636f 6e74 6163 745b 2253 656e 744e 7222  contact["SentNr"
-00010750: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00010760: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-00010770: 6163 745f 696e 666f 5b22 7263 766e 7222  act_info["rcvnr"
-00010780: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
-00010790: 5b22 4e52 225d 0a20 2020 2020 2020 2020  ["NR"].         
-000107a0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-000107b0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2269  .contact_info["i
-000107c0: 736d 756c 7469 706c 6965 7231 225d 203d  smultiplier1"] =
-000107d0: 2073 656c 662e 636f 6e74 6163 742e 6765   self.contact.ge
-000107e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000107f0: 2020 2020 2020 2022 4973 4d75 6c74 6970         "IsMultip
-00010800: 6c69 6572 3122 2c20 300a 2020 2020 2020  lier1", 0.      
-00010810: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010830: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-00010840: 666f 5b22 6973 6d75 6c74 6970 6c69 6572  fo["ismultiplier
-00010850: 3222 5d20 3d20 7365 6c66 2e63 6f6e 7461  2"] = self.conta
-00010860: 6374 2e67 6574 280a 2020 2020 2020 2020  ct.get(.        
-00010870: 2020 2020 2020 2020 2020 2020 2249 734d              "IsM
-00010880: 756c 7469 706c 6965 7232 222c 2030 0a20  ultiplier2", 0. 
-00010890: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000108a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108b0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-000108c0: 6374 5f69 6e66 6f5b 2269 736d 756c 7469  ct_info["ismulti
-000108d0: 706c 6965 7233 225d 203d 2073 656c 662e  plier3"] = self.
-000108e0: 636f 6e74 6163 742e 6765 7428 0a20 2020  contact.get(.   
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2022 4973 4d75 6c74 6970 6c69 6572 3322   "IsMultiplier3"
-00010910: 2c20 300a 2020 2020 2020 2020 2020 2020  , 0.            
-00010920: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010930: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00010940: 636f 6e74 6163 745f 696e 666f 5b22 7365  contact_info["se
-00010950: 6374 696f 6e22 5d20 3d20 7365 6c66 2e63  ction"] = self.c
-00010960: 6f6e 7461 6374 5b22 5365 6374 225d 0a20  ontact["Sect"]. 
-00010970: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010980: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
-00010990: 5f69 6e66 6f5b 2270 7265 6322 5d20 3d20  _info["prec"] = 
-000109a0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5072  self.contact["Pr
-000109b0: 6563 225d 0a20 2020 2020 2020 2020 2020  ec"].           
-000109c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-000109d0: 6f6e 7461 6374 5f69 6e66 6f5b 2263 6b22  ontact_info["ck"
-000109e0: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
-000109f0: 5b22 434b 225d 0a20 2020 2020 2020 2020  ["CK"].         
-00010a00: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00010a10: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 227a  .contact_info["z
-00010a20: 6e22 5d20 3d20 7365 6c66 2e63 6f6e 7461  n"] = self.conta
-00010a30: 6374 5b22 5a4e 225d 0a20 2020 2020 2020  ct["ZN"].       
-00010a40: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-00010a50: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-00010a60: 2270 6f77 6572 225d 203d 2073 656c 662e  "power"] = self.
-00010a70: 636f 6e74 6163 745b 2250 6f77 6572 225d  contact["Power"]
-00010a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010a90: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-00010aa0: 6374 5f69 6e66 6f5b 2262 616e 6422 5d20  ct_info["band"] 
-00010ab0: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
-00010ac0: 4261 6e64 225d 0a20 2020 2020 2020 2020  Band"].         
-00010ad0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00010ae0: 6275 6728 2225 7322 2c20 6622 7b73 656c  bug("%s", f"{sel
-00010af0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-00010b00: 6e66 6f7d 2229 0a20 2020 2020 2020 2020  nfo}").         
-00010b10: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00010b20: 2e73 656e 645f 636f 6e74 6163 745f 696e  .send_contact_in
-00010b30: 666f 2829 0a0a 2020 2020 2020 2020 7365  fo()..        se
-00010b40: 6c66 2e64 6174 6162 6173 652e 6c6f 675f  lf.database.log_
-00010b50: 636f 6e74 6163 7428 7365 6c66 2e63 6f6e  contact(self.con
-00010b60: 7461 6374 290a 2020 2020 2020 2020 7365  tact).        se
-00010b70: 6c66 2e77 6f72 6b65 645f 6c69 7374 203d  lf.worked_list =
-00010b80: 2073 656c 662e 6461 7461 6261 7365 2e67   self.database.g
-00010b90: 6574 5f63 616c 6c73 5f61 6e64 5f62 616e  et_calls_and_ban
-00010ba0: 6473 2829 0a20 2020 2020 2020 2073 656c  ds().        sel
-00010bb0: 662e 7365 6e64 5f77 6f72 6b65 645f 6c69  f.send_worked_li
-00010bc0: 7374 2829 0a20 2020 2020 2020 2073 656c  st().        sel
-00010bd0: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
-00010be0: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
-00010bf0: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
-00010c00: 6d64 225d 203d 2022 5550 4441 5445 4c4f  md"] = "UPDATELO
-00010c10: 4722 0a20 2020 2020 2020 2063 6d64 5b22  G".        cmd["
-00010c20: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00010c30: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00010c40: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00010c50: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
-00010c60: 645f 6173 5f6a 736f 6e28 636d 6429 0a0a  d_as_json(cmd)..
-00010c70: 2020 2020 6465 6620 6e65 775f 636f 6e74      def new_cont
-00010c80: 6573 745f 6469 616c 6f67 2873 656c 6629  est_dialog(self)
-00010c90: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00010ca0: 2020 2222 220a 2020 2020 2020 2020 5368    """.        Sh
-00010cb0: 6f77 206e 6577 2063 6f6e 7465 7374 2064  ow new contest d
-00010cc0: 6961 6c6f 672e 0a0a 2020 2020 2020 2020  ialog...        
-00010cd0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00010ce0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00010cf0: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
-00010d00: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00010d10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00010d20: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00010d30: 2022 2222 0a0a 2020 2020 2020 2020 6c6f   """..        lo
-00010d40: 6767 6572 2e64 6562 7567 2822 4e65 7720  gger.debug("New 
-00010d50: 636f 6e74 6573 7420 4469 616c 6f67 2229  contest Dialog")
-00010d60: 0a0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00010d70: 6f6e 7465 7374 5f64 6961 6c6f 6720 3d20  ontest_dialog = 
-00010d80: 4e65 7743 6f6e 7465 7374 2866 7375 7469  NewContest(fsuti
-00010d90: 6c73 2e41 5050 5f44 4154 415f 5041 5448  ls.APP_DATA_PATH
-00010da0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00010db0: 662e 6375 7272 656e 745f 7061 6c65 7474  f.current_palett
-00010dc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010dd0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00010de0: 6f67 2e73 6574 5061 6c65 7474 6528 7365  og.setPalette(se
-00010df0: 6c66 2e63 7572 7265 6e74 5f70 616c 6574  lf.current_palet
-00010e00: 7465 290a 2020 2020 2020 2020 2020 2020  te).            
-00010e10: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00010e20: 6c6f 672e 6578 6368 616e 6765 2e73 6574  log.exchange.set
-00010e30: 5061 6c65 7474 6528 7365 6c66 2e63 7572  Palette(self.cur
-00010e40: 7265 6e74 5f70 616c 6574 7465 290a 2020  rent_palette).  
-00010e50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00010e60: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
-00010e70: 6572 6174 6f72 732e 7365 7450 616c 6574  erators.setPalet
-00010e80: 7465 2873 656c 662e 6375 7272 656e 745f  te(self.current_
-00010e90: 7061 6c65 7474 6529 0a0a 2020 2020 2020  palette)..      
-00010ea0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00010eb0: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
-00010ec0: 6f6e 6e65 6374 2873 656c 662e 7361 7665  onnect(self.save
-00010ed0: 5f63 6f6e 7465 7374 290a 2020 2020 2020  _contest).      
-00010ee0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00010ef0: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
-00010f00: 6974 2e73 6574 4461 7465 2851 7443 6f72  it.setDate(QtCor
-00010f10: 652e 5144 6174 652e 6375 7272 656e 7444  e.QDate.currentD
-00010f20: 6174 6528 2929 0a20 2020 2020 2020 2073  ate()).        s
-00010f30: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00010f40: 6f67 2e64 6174 6554 696d 6545 6469 742e  og.dateTimeEdit.
-00010f50: 7365 7443 616c 656e 6461 7250 6f70 7570  setCalendarPopup
-00010f60: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
-00010f70: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00010f80: 6f67 2e64 6174 6554 696d 6545 6469 742e  og.dateTimeEdit.
-00010f90: 7365 7454 696d 6528 5174 436f 7265 2e51  setTime(QtCore.Q
-00010fa0: 5469 6d65 2830 2c20 3029 290a 2020 2020  Time(0, 0)).    
-00010fb0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00010fc0: 5f64 6961 6c6f 672e 706f 7765 722e 7365  _dialog.power.se
-00010fd0: 7443 7572 7265 6e74 5465 7874 2822 4c4f  tCurrentText("LO
-00010fe0: 5722 290a 2020 2020 2020 2020 7365 6c66  W").        self
-00010ff0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00011000: 7374 6174 696f 6e2e 7365 7443 7572 7265  station.setCurre
-00011010: 6e74 5465 7874 2822 4649 5845 4422 290a  ntText("FIXED").
-00011020: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00011030: 7465 7374 5f64 6961 6c6f 672e 6f70 656e  test_dialog.open
-00011040: 2829 0a0a 2020 2020 6465 6620 7361 7665  ()..    def save
-00011050: 5f63 6f6e 7465 7374 2873 656c 6629 202d  _contest(self) -
-00011060: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011070: 2222 220a 2020 2020 2020 2020 5361 7665  """.        Save
-00011080: 2043 6f6e 7465 7374 2074 6f20 6461 7461   Contest to data
-00011090: 6261 7365 2e0a 0a20 2020 2020 2020 2050  base...        P
-000110a0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-000110b0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000110c0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-000110d0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-000110e0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-000110f0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-00011100: 2222 220a 0a20 2020 2020 2020 206e 6578  """..        nex
-00011110: 745f 6e75 6d62 6572 203d 2073 656c 662e  t_number = self.
-00011120: 6461 7461 6261 7365 2e67 6574 5f6e 6578  database.get_nex
-00011130: 745f 636f 6e74 6573 745f 6e72 2829 0a20  t_contest_nr(). 
-00011140: 2020 2020 2020 2063 6f6e 7465 7374 203d         contest =
-00011150: 207b 7d0a 2020 2020 2020 2020 636f 6e74   {}.        cont
-00011160: 6573 745b 2243 6f6e 7465 7374 4e61 6d65  est["ContestName
-00011170: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00011180: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00011190: 6469 616c 6f67 2e63 6f6e 7465 7374 2e63  dialog.contest.c
-000111a0: 7572 7265 6e74 5465 7874 2829 2e6c 6f77  urrentText().low
-000111b0: 6572 2829 2e72 6570 6c61 6365 2822 2022  er().replace(" "
-000111c0: 2c20 225f 2229 0a20 2020 2020 2020 2029  , "_").        )
-000111d0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-000111e0: 5b22 5374 6172 7444 6174 6522 5d20 3d20  ["StartDate"] = 
-000111f0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00011200: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
-00011210: 2e64 6174 6554 696d 6528 292e 746f 5374  .dateTime().toSt
-00011220: 7269 6e67 280a 2020 2020 2020 2020 2020  ring(.          
-00011230: 2020 2279 7979 792d 4d4d 2d64 6420 6868    "yyyy-MM-dd hh
-00011240: 3a6d 6d3a 7373 220a 2020 2020 2020 2020  :mm:ss".        
-00011250: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00011260: 745b 224f 7065 7261 746f 7243 6174 6567  t["OperatorCateg
-00011270: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-00011280: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
-00011290: 6174 6f72 5f63 6c61 7373 2e63 7572 7265  ator_class.curre
-000112a0: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-000112b0: 2063 6f6e 7465 7374 5b22 4261 6e64 4361   contest["BandCa
-000112c0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-000112d0: 636f 6e74 6573 745f 6469 616c 6f67 2e62  contest_dialog.b
-000112e0: 616e 642e 6375 7272 656e 7454 6578 7428  and.currentText(
-000112f0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00011300: 745b 2250 6f77 6572 4361 7465 676f 7279  t["PowerCategory
-00011310: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00011320: 745f 6469 616c 6f67 2e70 6f77 6572 2e63  t_dialog.power.c
-00011330: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00011340: 2020 2020 2063 6f6e 7465 7374 5b22 4d6f       contest["Mo
-00011350: 6465 4361 7465 676f 7279 225d 203d 2073  deCategory"] = s
-00011360: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00011370: 6f67 2e6d 6f64 652e 6375 7272 656e 7454  og.mode.currentT
-00011380: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00011390: 6e74 6573 745b 224f 7665 726c 6179 4361  ntest["OverlayCa
-000113a0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-000113b0: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
-000113c0: 7665 726c 6179 2e63 7572 7265 6e74 5465  verlay.currentTe
-000113d0: 7874 2829 0a20 2020 2020 2020 2023 2063  xt().        # c
-000113e0: 6f6e 7465 7374 5b27 436c 6169 6d65 6453  ontest['ClaimedS
-000113f0: 636f 7265 275d 203d 2073 656c 662e 636f  core'] = self.co
-00011400: 6e74 6573 745f 6469 616c 6f67 2e0a 2020  ntest_dialog..  
-00011410: 2020 2020 2020 636f 6e74 6573 745b 224f        contest["O
-00011420: 7065 7261 746f 7273 225d 203d 2073 656c  perators"] = sel
-00011430: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00011440: 2e6f 7065 7261 746f 7273 2e74 6578 7428  .operators.text(
-00011450: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00011460: 745b 2253 6f61 7062 6f78 225d 203d 2073  t["Soapbox"] = s
-00011470: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00011480: 6f67 2e73 6f61 7062 6f78 2e74 6f50 6c61  og.soapbox.toPla
-00011490: 696e 5465 7874 2829 0a20 2020 2020 2020  inText().       
-000114a0: 2063 6f6e 7465 7374 5b22 5365 6e74 4578   contest["SentEx
-000114b0: 6368 616e 6765 225d 203d 2073 656c 662e  change"] = self.
-000114c0: 636f 6e74 6573 745f 6469 616c 6f67 2e65  contest_dialog.e
-000114d0: 7863 6861 6e67 652e 7465 7874 2829 0a20  xchange.text(). 
-000114e0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-000114f0: 436f 6e74 6573 744e 5222 5d20 3d20 6e65  ContestNR"] = ne
-00011500: 7874 5f6e 756d 6265 722e 6765 7428 2263  xt_number.get("c
-00011510: 6f75 6e74 222c 2031 290a 2020 2020 2020  ount", 1).      
-00011520: 2020 7365 6c66 2e70 7265 665b 2263 6f6e    self.pref["con
-00011530: 7465 7374 225d 203d 206e 6578 745f 6e75  test"] = next_nu
-00011540: 6d62 6572 2e67 6574 2822 636f 756e 7422  mber.get("count"
-00011550: 2c20 3129 0a20 2020 2020 2020 2023 2063  , 1).        # c
-00011560: 6f6e 7465 7374 5b27 5375 6254 7970 6527  ontest['SubType'
-00011570: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00011580: 5f64 6961 6c6f 672e 0a20 2020 2020 2020  _dialog..       
-00011590: 2063 6f6e 7465 7374 5b22 5374 6174 696f   contest["Statio
-000115a0: 6e43 6174 6567 6f72 7922 5d20 3d20 7365  nCategory"] = se
-000115b0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000115c0: 672e 7374 6174 696f 6e2e 6375 7272 656e  g.station.curren
-000115d0: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
-000115e0: 636f 6e74 6573 745b 2241 7373 6973 7465  contest["Assiste
-000115f0: 6443 6174 6567 6f72 7922 5d20 3d20 7365  dCategory"] = se
-00011600: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00011610: 672e 6173 7369 7374 6564 2e63 7572 7265  g.assisted.curre
-00011620: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-00011630: 2063 6f6e 7465 7374 5b22 5472 616e 736d   contest["Transm
-00011640: 6974 7465 7243 6174 6567 6f72 7922 5d20  itterCategory"] 
-00011650: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00011660: 6961 6c6f 672e 7472 616e 736d 6974 7465  ialog.transmitte
-00011670: 722e 6375 7272 656e 7454 6578 7428 290a  r.currentText().
-00011680: 2020 2020 2020 2020 2320 636f 6e74 6573          # contes
-00011690: 745b 2754 696d 6543 6174 6567 6f72 7927  t['TimeCategory'
-000116a0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-000116b0: 5f64 6961 6c6f 672e 0a20 2020 2020 2020  _dialog..       
-000116c0: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-000116d0: 7322 2c20 6622 7b63 6f6e 7465 7374 7d22  s", f"{contest}"
-000116e0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
-000116f0: 6174 6162 6173 652e 6164 645f 636f 6e74  atabase.add_cont
-00011700: 6573 7428 636f 6e74 6573 7429 0a20 2020  est(contest).   
-00011710: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-00011720: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
-00011730: 2020 2020 2073 656c 662e 6c6f 6164 5f63       self.load_c
-00011740: 6f6e 7465 7374 2829 0a0a 2020 2020 6465  ontest()..    de
-00011750: 6620 6564 6974 5f73 7461 7469 6f6e 5f73  f edit_station_s
-00011760: 6574 7469 6e67 7328 7365 6c66 2920 2d3e  ettings(self) ->
-00011770: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00011780: 2222 0a20 2020 2020 2020 2053 686f 7720  "".        Show 
-00011790: 7365 7474 696e 6773 2064 6961 6c6f 6720  settings dialog 
-000117a0: 666f 7220 7374 6174 696f 6e2e 0a0a 2020  for station...  
-000117b0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000117c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000117d0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000117e0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000117f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00011800: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-00011810: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00011820: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00011830: 2822 5374 6174 696f 6e20 5365 7474 696e  ("Station Settin
-00011840: 6773 2073 656c 6563 7465 6422 290a 0a20  gs selected").. 
-00011850: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-00011860: 696e 6773 5f64 6961 6c6f 6720 3d20 4564  ings_dialog = Ed
-00011870: 6974 5374 6174 696f 6e28 6673 7574 696c  itStation(fsutil
-00011880: 732e 4150 505f 4441 5441 5f50 4154 4829  s.APP_DATA_PATH)
-00011890: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000118a0: 2e63 7572 7265 6e74 5f70 616c 6574 7465  .current_palette
-000118b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000118c0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-000118d0: 6f67 2e73 6574 5061 6c65 7474 6528 7365  og.setPalette(se
-000118e0: 6c66 2e63 7572 7265 6e74 5f70 616c 6574  lf.current_palet
-000118f0: 7465 290a 0a20 2020 2020 2020 2073 656c  te)..        sel
-00011900: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-00011910: 672e 6163 6365 7074 6564 2e63 6f6e 6e65  g.accepted.conne
-00011920: 6374 2873 656c 662e 7361 7665 5f73 6574  ct(self.save_set
-00011930: 7469 6e67 7329 0a20 2020 2020 2020 2073  tings).        s
-00011940: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00011950: 6c6f 672e 4361 6c6c 2e73 6574 5465 7874  log.Call.setText
-00011960: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-00011970: 7428 2243 616c 6c22 2c20 2222 2929 0a20  t("Call", "")). 
-00011980: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-00011990: 696e 6773 5f64 6961 6c6f 672e 4e61 6d65  ings_dialog.Name
-000119a0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-000119b0: 6174 696f 6e2e 6765 7428 224e 616d 6522  ation.get("Name"
-000119c0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-000119d0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-000119e0: 6c6f 672e 4164 6472 6573 7331 2e73 6574  log.Address1.set
-000119f0: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-00011a00: 6e2e 6765 7428 2253 7472 6565 7431 222c  n.get("Street1",
-00011a10: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
-00011a20: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-00011a30: 6f67 2e41 6464 7265 7373 322e 7365 7454  og.Address2.setT
-00011a40: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-00011a50: 2e67 6574 2822 5374 7265 6574 3222 2c20  .get("Street2", 
-00011a60: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-00011a70: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-00011a80: 672e 4369 7479 2e73 6574 5465 7874 2873  g.City.setText(s
-00011a90: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00011aa0: 2243 6974 7922 2c20 2222 2929 0a20 2020  "City", "")).   
-00011ab0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-00011ac0: 6773 5f64 6961 6c6f 672e 5374 6174 652e  gs_dialog.State.
-00011ad0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-00011ae0: 7469 6f6e 2e67 6574 2822 5374 6174 6522  tion.get("State"
-00011af0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-00011b00: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00011b10: 6c6f 672e 5a69 702e 7365 7454 6578 7428  log.Zip.setText(
-00011b20: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00011b30: 2822 5a69 7022 2c20 2222 2929 0a20 2020  ("Zip", "")).   
-00011b40: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-00011b50: 6773 5f64 6961 6c6f 672e 436f 756e 7472  gs_dialog.Countr
-00011b60: 792e 7365 7454 6578 7428 7365 6c66 2e73  y.setText(self.s
-00011b70: 7461 7469 6f6e 2e67 6574 2822 436f 756e  tation.get("Coun
-00011b80: 7472 7922 2c20 2222 2929 0a20 2020 2020  try", "")).     
-00011b90: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-00011ba0: 5f64 6961 6c6f 672e 4772 6964 5371 7561  _dialog.GridSqua
-00011bb0: 7265 2e73 6574 5465 7874 2873 656c 662e  re.setText(self.
-00011bc0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
-00011bd0: 6453 7175 6172 6522 2c20 2222 2929 0a20  dSquare", "")). 
-00011be0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-00011bf0: 696e 6773 5f64 6961 6c6f 672e 4351 5a6f  ings_dialog.CQZo
-00011c00: 6e65 2e73 6574 5465 7874 2873 7472 2873  ne.setText(str(s
-00011c10: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00011c20: 2243 515a 6f6e 6522 2c20 2222 2929 290a  "CQZone", ""))).
-00011c30: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00011c40: 7469 6e67 735f 6469 616c 6f67 2e49 5455  tings_dialog.ITU
-00011c50: 5a6f 6e65 2e73 6574 5465 7874 2873 7472  Zone.setText(str
-00011c60: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-00011c70: 7428 2249 4152 555a 6f6e 6522 2c20 2222  t("IARUZone", ""
-00011c80: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-00011c90: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00011ca0: 2e4c 6963 656e 7365 2e73 6574 5465 7874  .License.setText
-00011cb0: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-00011cc0: 7428 224c 6963 656e 7365 436c 6173 7322  t("LicenseClass"
-00011cd0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-00011ce0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00011cf0: 6c6f 672e 4c61 7469 7475 6465 2e73 6574  log.Latitude.set
-00011d00: 5465 7874 2873 7472 2873 656c 662e 7374  Text(str(self.st
-00011d10: 6174 696f 6e2e 6765 7428 224c 6174 6974  ation.get("Latit
-00011d20: 7564 6522 2c20 2222 2929 290a 2020 2020  ude", ""))).    
-00011d30: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00011d40: 735f 6469 616c 6f67 2e4c 6f6e 6769 7475  s_dialog.Longitu
-00011d50: 6465 2e73 6574 5465 7874 2873 7472 2873  de.setText(str(s
-00011d60: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00011d70: 224c 6f6e 6769 7475 6465 222c 2022 2229  "Longitude", "")
-00011d80: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00011d90: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-00011da0: 5374 6174 696f 6e54 5852 582e 7365 7454  StationTXRX.setT
-00011db0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-00011dc0: 2e67 6574 2822 7374 6174 696f 6e74 7872  .get("stationtxr
-00011dd0: 7822 2c20 2222 2929 0a20 2020 2020 2020  x", "")).       
-00011de0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-00011df0: 6961 6c6f 672e 506f 7765 722e 7365 7454  ialog.Power.setT
-00011e00: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-00011e10: 2e67 6574 2822 5350 6f77 6522 2c20 2222  .get("SPowe", ""
-00011e20: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00011e30: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-00011e40: 416e 7465 6e6e 612e 7365 7454 6578 7428  Antenna.setText(
-00011e50: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00011e60: 2822 5341 6e74 6522 2c20 2222 2929 0a20  ("SAnte", "")). 
-00011e70: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-00011e80: 696e 6773 5f64 6961 6c6f 672e 416e 7448  ings_dialog.AntH
-00011e90: 6569 6768 742e 7365 7454 6578 7428 7365  eight.setText(se
-00011ea0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-00011eb0: 5341 6e74 4831 222c 2022 2229 290a 2020  SAntH1", "")).  
-00011ec0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-00011ed0: 6e67 735f 6469 616c 6f67 2e41 534c 2e73  ngs_dialog.ASL.s
-00011ee0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-00011ef0: 696f 6e2e 6765 7428 2253 416e 7448 3222  ion.get("SAntH2"
-00011f00: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-00011f10: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00011f20: 6c6f 672e 4152 524c 5365 6374 696f 6e2e  log.ARRLSection.
-00011f30: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-00011f40: 7469 6f6e 2e67 6574 2822 4152 524c 5365  tion.get("ARRLSe
-00011f50: 6374 696f 6e22 2c20 2222 2929 0a20 2020  ction", "")).   
-00011f60: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-00011f70: 6773 5f64 6961 6c6f 672e 526f 7665 7251  gs_dialog.RoverQ
-00011f80: 5448 2e73 6574 5465 7874 2873 656c 662e  TH.setText(self.
-00011f90: 7374 6174 696f 6e2e 6765 7428 2252 6f76  station.get("Rov
-00011fa0: 6572 5154 4822 2c20 2222 2929 0a20 2020  erQTH", "")).   
-00011fb0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-00011fc0: 6773 5f64 6961 6c6f 672e 436c 7562 2e73  gs_dialog.Club.s
-00011fd0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-00011fe0: 696f 6e2e 6765 7428 2243 6c75 6222 2c20  ion.get("Club", 
-00011ff0: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-00012000: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-00012010: 672e 456d 6169 6c2e 7365 7454 6578 7428  g.Email.setText(
-00012020: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00012030: 2822 456d 6169 6c22 2c20 2222 2929 0a20  ("Email", "")). 
-00012040: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-00012050: 696e 6773 5f64 6961 6c6f 672e 6f70 656e  ings_dialog.open
-00012060: 2829 0a0a 2020 2020 6465 6620 7361 7665  ()..    def save
-00012070: 5f73 6574 7469 6e67 7328 7365 6c66 2920  _settings(self) 
-00012080: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00012090: 2022 2222 0a20 2020 2020 2020 2053 6176   """.        Sav
-000120a0: 6520 7365 7474 696e 6773 2074 6f20 6461  e settings to da
-000120b0: 7461 6261 7365 2e0a 0a20 2020 2020 2020  tabase...       
-000120c0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000120d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000120e0: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-000120f0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00012100: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00012110: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-00012120: 2020 2222 220a 0a20 2020 2020 2020 2063    """..        c
-00012130: 7320 3d20 7365 6c66 2e73 6574 7469 6e67  s = self.setting
-00012140: 735f 6469 616c 6f67 2e43 616c 6c2e 7465  s_dialog.Call.te
-00012150: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-00012160: 662e 7374 6174 696f 6e20 3d20 7b7d 0a20  f.station = {}. 
-00012170: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00012180: 696f 6e5b 2243 616c 6c22 5d20 3d20 6373  ion["Call"] = cs
-00012190: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-000121a0: 2073 656c 662e 7374 6174 696f 6e5b 224e   self.station["N
-000121b0: 616d 6522 5d20 3d20 7365 6c66 2e73 6574  ame"] = self.set
-000121c0: 7469 6e67 735f 6469 616c 6f67 2e4e 616d  tings_dialog.Nam
-000121d0: 652e 7465 7874 2829 2e74 6974 6c65 2829  e.text().title()
-000121e0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000121f0: 6174 696f 6e5b 2253 7472 6565 7431 225d  ation["Street1"]
-00012200: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-00012210: 5f64 6961 6c6f 672e 4164 6472 6573 7331  _dialog.Address1
-00012220: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
-00012230: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00012240: 7469 6f6e 5b22 5374 7265 6574 3222 5d20  tion["Street2"] 
-00012250: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-00012260: 6469 616c 6f67 2e41 6464 7265 7373 322e  dialog.Address2.
-00012270: 7465 7874 2829 2e74 6974 6c65 2829 0a20  text().title(). 
-00012280: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00012290: 696f 6e5b 2243 6974 7922 5d20 3d20 7365  ion["City"] = se
-000122a0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-000122b0: 6f67 2e43 6974 792e 7465 7874 2829 2e74  og.City.text().t
-000122c0: 6974 6c65 2829 0a20 2020 2020 2020 2073  itle().        s
-000122d0: 656c 662e 7374 6174 696f 6e5b 2253 7461  elf.station["Sta
-000122e0: 7465 225d 203d 2073 656c 662e 7365 7474  te"] = self.sett
-000122f0: 696e 6773 5f64 6961 6c6f 672e 5374 6174  ings_dialog.Stat
-00012300: 652e 7465 7874 2829 2e75 7070 6572 2829  e.text().upper()
-00012310: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-00012320: 6174 696f 6e5b 225a 6970 225d 203d 2073  ation["Zip"] = s
-00012330: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00012340: 6c6f 672e 5a69 702e 7465 7874 2829 0a20  log.Zip.text(). 
-00012350: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00012360: 696f 6e5b 2243 6f75 6e74 7279 225d 203d  ion["Country"] =
-00012370: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-00012380: 6961 6c6f 672e 436f 756e 7472 792e 7465  ialog.Country.te
-00012390: 7874 2829 2e74 6974 6c65 2829 0a20 2020  xt().title().   
-000123a0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-000123b0: 6e5b 2247 7269 6453 7175 6172 6522 5d20  n["GridSquare"] 
-000123c0: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-000123d0: 6469 616c 6f67 2e47 7269 6453 7175 6172  dialog.GridSquar
-000123e0: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
-000123f0: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
-00012400: 515a 6f6e 6522 5d20 3d20 7365 6c66 2e73  QZone"] = self.s
-00012410: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-00012420: 515a 6f6e 652e 7465 7874 2829 0a20 2020  QZone.text().   
-00012430: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-00012440: 6e5b 2249 4152 555a 6f6e 6522 5d20 3d20  n["IARUZone"] = 
-00012450: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00012460: 616c 6f67 2e49 5455 5a6f 6e65 2e74 6578  alog.ITUZone.tex
-00012470: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00012480: 2e73 7461 7469 6f6e 5b22 4c69 6365 6e73  .station["Licens
-00012490: 6543 6c61 7373 225d 203d 2073 656c 662e  eClass"] = self.
-000124a0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-000124b0: 4c69 6365 6e73 652e 7465 7874 2829 2e74  License.text().t
-000124c0: 6974 6c65 2829 0a20 2020 2020 2020 2073  itle().        s
-000124d0: 656c 662e 7374 6174 696f 6e5b 224c 6174  elf.station["Lat
-000124e0: 6974 7564 6522 5d20 3d20 7365 6c66 2e73  itude"] = self.s
-000124f0: 6574 7469 6e67 735f 6469 616c 6f67 2e4c  ettings_dialog.L
-00012500: 6174 6974 7564 652e 7465 7874 2829 0a20  atitude.text(). 
-00012510: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00012520: 696f 6e5b 224c 6f6e 6769 7475 6465 225d  ion["Longitude"]
-00012530: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-00012540: 5f64 6961 6c6f 672e 4c6f 6e67 6974 7564  _dialog.Longitud
-00012550: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
-00012560: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
-00012570: 5458 6571 225d 203d 2073 656c 662e 7365  TXeq"] = self.se
-00012580: 7474 696e 6773 5f64 6961 6c6f 672e 5374  ttings_dialog.St
-00012590: 6174 696f 6e54 5852 582e 7465 7874 2829  ationTXRX.text()
-000125a0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000125b0: 6174 696f 6e5b 2253 506f 7765 225d 203d  ation["SPowe"] =
-000125c0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-000125d0: 6961 6c6f 672e 506f 7765 722e 7465 7874  ialog.Power.text
-000125e0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000125f0: 7374 6174 696f 6e5b 2253 416e 7465 225d  station["SAnte"]
-00012600: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-00012610: 5f64 6961 6c6f 672e 416e 7465 6e6e 612e  _dialog.Antenna.
-00012620: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-00012630: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
-00012640: 7448 3122 5d20 3d20 7365 6c66 2e73 6574  tH1"] = self.set
-00012650: 7469 6e67 735f 6469 616c 6f67 2e41 6e74  tings_dialog.Ant
-00012660: 4865 6967 6874 2e74 6578 7428 290a 2020  Height.text().  
-00012670: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00012680: 6f6e 5b22 5341 6e74 4832 225d 203d 2073  on["SAntH2"] = s
-00012690: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-000126a0: 6c6f 672e 4153 4c2e 7465 7874 2829 0a20  log.ASL.text(). 
-000126b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000126c0: 696f 6e5b 2241 5252 4c53 6563 7469 6f6e  ion["ARRLSection
-000126d0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-000126e0: 6773 5f64 6961 6c6f 672e 4152 524c 5365  gs_dialog.ARRLSe
-000126f0: 6374 696f 6e2e 7465 7874 2829 2e75 7070  ction.text().upp
-00012700: 6572 2829 0a20 2020 2020 2020 2073 656c  er().        sel
-00012710: 662e 7374 6174 696f 6e5b 2252 6f76 6572  f.station["Rover
-00012720: 5154 4822 5d20 3d20 7365 6c66 2e73 6574  QTH"] = self.set
-00012730: 7469 6e67 735f 6469 616c 6f67 2e52 6f76  tings_dialog.Rov
-00012740: 6572 5154 482e 7465 7874 2829 0a20 2020  erQTH.text().   
-00012750: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-00012760: 6e5b 2243 6c75 6222 5d20 3d20 7365 6c66  n["Club"] = self
-00012770: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00012780: 2e43 6c75 622e 7465 7874 2829 2e74 6974  .Club.text().tit
-00012790: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
-000127a0: 662e 7374 6174 696f 6e5b 2245 6d61 696c  f.station["Email
-000127b0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-000127c0: 6773 5f64 6961 6c6f 672e 456d 6169 6c2e  gs_dialog.Email.
-000127d0: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-000127e0: 656c 662e 6461 7461 6261 7365 2e61 6464  elf.database.add
-000127f0: 5f73 7461 7469 6f6e 2873 656c 662e 7374  _station(self.st
-00012800: 6174 696f 6e29 0a20 2020 2020 2020 2073  ation).        s
-00012810: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00012820: 6c6f 672e 636c 6f73 6528 290a 2020 2020  log.close().    
-00012830: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
-00012840: 656e 745f 6f70 203d 3d20 2222 3a0a 2020  ent_op == "":.  
-00012850: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00012860: 7572 7265 6e74 5f6f 7020 3d20 7365 6c66  urrent_op = self
-00012870: 2e73 7461 7469 6f6e 2e67 6574 2822 4361  .station.get("Ca
-00012880: 6c6c 222c 2022 2229 0a20 2020 2020 2020  ll", "").       
-00012890: 2020 2020 2073 656c 662e 6d61 6b65 5f6f       self.make_o
-000128a0: 705f 6469 7228 290a 2020 2020 2020 2020  p_dir().        
-000128b0: 636f 6e74 6573 745f 636f 756e 7420 3d20  contest_count = 
-000128c0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
-000128d0: 7463 685f 616c 6c5f 636f 6e74 6573 7473  tch_all_contests
-000128e0: 2829 0a20 2020 2020 2020 2069 6620 6c65  ().        if le
-000128f0: 6e28 636f 6e74 6573 745f 636f 756e 7429  n(contest_count)
-00012900: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00012910: 2020 2073 656c 662e 6e65 775f 636f 6e74     self.new_cont
-00012920: 6573 745f 6469 616c 6f67 2829 0a0a 2020  est_dialog()..  
-00012930: 2020 6465 6620 6564 6974 5f6d 6163 726f    def edit_macro
-00012940: 2873 656c 662c 2066 756e 6374 696f 6e5f  (self, function_
-00012950: 6b65 7929 202d 3e20 4e6f 6e65 3a0a 2020  key) -> None:.  
-00012960: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012970: 2020 5368 6f77 2065 6469 7420 6d61 6372    Show edit macr
-00012980: 6f20 6469 616c 6f67 2066 6f72 2066 756e  o dialog for fun
-00012990: 6374 696f 6e20 6b65 792e 0a0a 2020 2020  ction key...    
-000129a0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000129b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000129c0: 2d0a 2020 2020 2020 2020 6675 6e63 7469  -.        functi
-000129d0: 6f6e 5f6b 6579 203a 2073 7472 0a20 2020  on_key : str.   
-000129e0: 2020 2020 2046 756e 6374 696f 6e20 6b65       Function ke
-000129f0: 7920 746f 2065 6469 742e 0a0a 2020 2020  y to edit...    
-00012a00: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00012a10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00012a20: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00012a30: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
-00012a40: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
-00012a50: 616c 6f67 203d 2045 6469 744d 6163 726f  alog = EditMacro
-00012a60: 2866 756e 6374 696f 6e5f 6b65 792c 2066  (function_key, f
-00012a70: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
-00012a80: 5041 5448 290a 0a20 2020 2020 2020 2069  PATH)..        i
-00012a90: 6620 7365 6c66 2e63 7572 7265 6e74 5f70  f self.current_p
-00012aa0: 616c 6574 7465 3a0a 2020 2020 2020 2020  alette:.        
-00012ab0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
-00012ac0: 6372 6f5f 6469 616c 6f67 2e73 6574 5061  cro_dialog.setPa
-00012ad0: 6c65 7474 6528 7365 6c66 2e63 7572 7265  lette(self.curre
-00012ae0: 6e74 5f70 616c 6574 7465 290a 0a20 2020  nt_palette)..   
-00012af0: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-00012b00: 6163 726f 5f64 6961 6c6f 672e 6163 6365  acro_dialog.acce
-00012b10: 7074 6564 2e63 6f6e 6e65 6374 2873 656c  pted.connect(sel
-00012b20: 662e 6564 6974 6564 5f6d 6163 726f 290a  f.edited_macro).
-00012b30: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-00012b40: 745f 6d61 6372 6f5f 6469 616c 6f67 2e6f  t_macro_dialog.o
-00012b50: 7065 6e28 290a 0a20 2020 2064 6566 2065  pen()..    def e
-00012b60: 6469 7465 645f 6d61 6372 6f28 7365 6c66  dited_macro(self
-00012b70: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00012b80: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00012b90: 6176 6520 6564 6974 6564 206d 6163 726f  ave edited macro
-00012ba0: 2074 6f20 6461 7461 6261 7365 2e0a 0a20   to database... 
-00012bb0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00012bc0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00012bd0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00012be0: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
-00012bf0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00012c00: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00012c10: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00012c20: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-00012c30: 6163 726f 5f64 6961 6c6f 672e 6675 6e63  acro_dialog.func
-00012c40: 7469 6f6e 5f6b 6579 2e73 6574 5465 7874  tion_key.setText
-00012c50: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00012c60: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
-00012c70: 616c 6f67 2e6d 6163 726f 5f6c 6162 656c  alog.macro_label
-00012c80: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-00012c90: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
-00012ca0: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
-00012cb0: 2e66 756e 6374 696f 6e5f 6b65 792e 7365  .function_key.se
-00012cc0: 7454 6f6f 6c54 6970 280a 2020 2020 2020  tToolTip(.      
-00012cd0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
-00012ce0: 6d61 6372 6f5f 6469 616c 6f67 2e74 6865  macro_dialog.the
-00012cf0: 5f6d 6163 726f 2e74 6578 7428 290a 2020  _macro.text().  
-00012d00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00012d10: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
-00012d20: 6469 616c 6f67 2e63 6c6f 7365 2829 0a0a  dialog.close()..
-00012d30: 2020 2020 6465 6620 7072 6f63 6573 735f      def process_
-00012d40: 6d61 6372 6f28 7365 6c66 2c20 6d61 6372  macro(self, macr
-00012d50: 6f3a 2073 7472 2920 2d3e 2073 7472 3a0a  o: str) -> str:.
-00012d60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012d70: 2020 2020 5072 6f63 6573 7320 4357 206d      Process CW m
-00012d80: 6163 726f 2073 7562 7374 6974 7574 696f  acro substitutio
-00012d90: 6e73 2066 6f72 2063 6f6e 7465 7374 2e0a  ns for contest..
-00012da0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00012db0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00012dc0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206d  ------.        m
-00012dd0: 6163 726f 203a 2073 7472 0a20 2020 2020  acro : str.     
-00012de0: 2020 204d 6163 726f 2074 6f20 7072 6f63     Macro to proc
-00012df0: 6573 732e 0a0a 2020 2020 2020 2020 5265  ess...        Re
-00012e00: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00012e10: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7374  -----.        st
-00012e20: 720a 2020 2020 2020 2020 5072 6f63 6573  r.        Proces
-00012e30: 7365 6420 6d61 6372 6f2e 0a20 2020 2020  sed macro..     
-00012e40: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00012e50: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
-00012e60: 7461 6261 7365 2e67 6574 5f73 6572 6961  tabase.get_seria
-00012e70: 6c28 290a 2020 2020 2020 2020 6e65 7874  l().        next
-00012e80: 5f73 6572 6961 6c20 3d20 7374 7228 7265  _serial = str(re
-00012e90: 7375 6c74 2e67 6574 2822 7365 7269 616c  sult.get("serial
-00012ea0: 5f6e 7222 2c20 2231 2229 290a 2020 2020  _nr", "1")).    
-00012eb0: 2020 2020 6966 206e 6578 745f 7365 7269      if next_seri
-00012ec0: 616c 203d 3d20 224e 6f6e 6522 3a0a 2020  al == "None":.  
-00012ed0: 2020 2020 2020 2020 2020 6e65 7874 5f73            next_s
-00012ee0: 6572 6961 6c20 3d20 2231 220a 2020 2020  erial = "1".    
-00012ef0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
-00012f00: 6f2e 7570 7065 7228 290a 2020 2020 2020  o.upper().      
-00012f10: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
-00012f20: 7265 706c 6163 6528 2223 222c 206e 6578  replace("#", nex
-00012f30: 745f 7365 7269 616c 290a 2020 2020 2020  t_serial).      
-00012f40: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
-00012f50: 7265 706c 6163 6528 227b 4d59 4341 4c4c  replace("{MYCALL
-00012f60: 7d22 2c20 7365 6c66 2e73 7461 7469 6f6e  }", self.station
-00012f70: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
-00012f80: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
-00012f90: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
-00012fa0: 227b 4849 5343 414c 4c7d 222c 2073 656c  "{HISCALL}", sel
-00012fb0: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
-00012fc0: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
-00012fd0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-00012fe0: 6574 2822 6d6f 6465 2229 203d 3d20 2243  et("mode") == "C
-00012ff0: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
-00013000: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
-00013010: 706c 6163 6528 227b 534e 547d 222c 2073  place("{SNT}", s
-00013020: 656c 662e 7365 6e74 2e74 6578 7428 292e  elf.sent.text().
-00013030: 7265 706c 6163 6528 2239 222c 2022 6e22  replace("9", "n"
-00013040: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
-00013050: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
-00013060: 726f 203d 206d 6163 726f 2e72 6570 6c61  ro = macro.repla
-00013070: 6365 2822 7b53 4e54 7d22 2c20 7365 6c66  ce("{SNT}", self
-00013080: 2e73 656e 742e 7465 7874 2829 290a 2020  .sent.text()).  
-00013090: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-000130a0: 6372 6f2e 7265 706c 6163 6528 227b 5345  cro.replace("{SE
-000130b0: 4e54 4e52 7d22 2c20 7365 6c66 2e6f 7468  NTNR}", self.oth
-000130c0: 6572 5f31 2e74 6578 7428 2929 0a20 2020  er_1.text()).   
-000130d0: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
-000130e0: 726f 2e72 6570 6c61 6365 280a 2020 2020  ro.replace(.    
-000130f0: 2020 2020 2020 2020 227b 4558 4348 7d22          "{EXCH}"
-00013100: 2c20 7365 6c66 2e63 6f6e 7465 7374 5f73  , self.contest_s
-00013110: 6574 7469 6e67 732e 6765 7428 2253 656e  ettings.get("Sen
-00013120: 7445 7863 6861 6e67 6522 2c20 2278 7878  tExchange", "xxx
-00013130: 2229 0a20 2020 2020 2020 2029 0a20 2020  ").        ).   
-00013140: 2020 2020 2072 6574 7572 6e20 6d61 6372       return macr
-00013150: 6f0a 0a20 2020 2064 6566 2076 6f69 6365  o..    def voice
-00013160: 5f73 7472 696e 6728 7365 6c66 2c20 7468  _string(self, th
-00013170: 655f 7374 7269 6e67 3a20 7374 7229 202d  e_string: str) -
-00013180: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00013190: 2222 220a 2020 2020 2020 2020 766f 6963  """.        voic
-000131a0: 6573 2073 7472 696e 6720 7573 696e 6720  es string using 
-000131b0: 6e61 746f 2070 686f 6e65 7469 6373 2e0a  nato phonetics..
-000131c0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000131d0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-000131e0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
-000131f0: 6865 5f73 7472 696e 6720 3a20 7374 720a  he_string : str.
-00013200: 2020 2020 2020 2020 5374 7269 6e67 2074          String t
-00013210: 6f20 766f 6963 6966 792e 0a0a 2020 2020  o voicify...    
-00013220: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00013230: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00013240: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00013250: 2022 2222 0a0a 2020 2020 2020 2020 6c6f   """..        lo
-00013260: 6767 6572 2e64 6562 7567 2822 566f 6963  gger.debug("Voic
-00013270: 696e 673a 2025 7322 2c20 7468 655f 7374  ing: %s", the_st
-00013280: 7269 6e67 290a 2020 2020 2020 2020 6f70  ring).        op
-00013290: 5f70 6174 6820 3d20 6673 7574 696c 732e  _path = fsutils.
-000132a0: 5553 4552 5f44 4154 415f 5041 5448 202f  USER_DATA_PATH /
-000132b0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-000132c0: 0a20 2020 2020 2020 2069 6620 225b 2220  .        if "[" 
-000132d0: 696e 2074 6865 5f73 7472 696e 673a 0a20  in the_string:. 
-000132e0: 2020 2020 2020 2020 2020 2073 7562 5f73             sub_s
-000132f0: 7472 696e 6720 3d20 7468 655f 7374 7269  tring = the_stri
-00013300: 6e67 2e73 7472 6970 2822 5b5d 2229 2e6c  ng.strip("[]").l
-00013310: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
-00013320: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
-00013330: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
-00013340: 7375 625f 7374 7269 6e67 7d2e 7761 7622  sub_string}.wav"
-00013350: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013360: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
-00013370: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
-00013380: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00013390: 2e64 6562 7567 2822 566f 6963 696e 673a  .debug("Voicing:
-000133a0: 2025 7322 2c20 6669 6c65 6e61 6d65 290a   %s", filename).
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 6461 7461 2c20 5f66 7320 3d20 7366 2e72  data, _fs = sf.r
-000133d0: 6561 6428 6669 6c65 6e61 6d65 2c20 6474  ead(filename, dt
-000133e0: 7970 653d 2266 6c6f 6174 3332 2229 0a20  ype="float32"). 
-000133f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013400: 656c 662e 7074 745f 6f6e 2829 0a20 2020  elf.ptt_on().   
-00013410: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00013420: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013430: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-00013440: 2e64 6576 6963 6520 3d20 7365 6c66 2e70  .device = self.p
-00013450: 7265 662e 6765 7428 2273 6f75 6e64 6465  ref.get("soundde
-00013460: 7669 6365 222c 2022 6465 6661 756c 7422  vice", "default"
-00013470: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013480: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-00013490: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
-000134a0: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
-000134b0: 2020 2020 2020 2020 2020 7364 2e70 6c61            sd.pla
-000134c0: 7928 6461 7461 2c20 626c 6f63 6b69 6e67  y(data, blocking
-000134d0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-000134e0: 2020 2020 2020 2020 2020 2020 2320 5f73              # _s
-000134f0: 7461 7475 7320 3d20 7364 2e77 6169 7428  tatus = sd.wait(
-00013500: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013510: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00013520: 736e 796b 2e69 6f2f 6164 7669 736f 722f  snyk.io/advisor/
-00013530: 7079 7468 6f6e 2f73 6f75 6e64 6465 7669  python/sounddevi
-00013540: 6365 2f66 756e 6374 696f 6e73 2f73 6f75  ce/functions/sou
-00013550: 6e64 6465 7669 6365 2e50 6f72 7441 7564  nddevice.PortAud
-00013560: 696f 4572 726f 720a 2020 2020 2020 2020  ioError.        
-00013570: 2020 2020 2020 2020 6578 6365 7074 2073          except s
-00013580: 642e 506f 7274 4175 6469 6f45 7272 6f72  d.PortAudioError
-00013590: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
-000135a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000135b0: 6765 722e 7761 726e 696e 6728 2225 7322  ger.warning("%s"
-000135c0: 2c20 6622 7b65 7272 7d22 290a 0a20 2020  , f"{err}")..   
-000135d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000135e0: 662e 7074 745f 6f66 6628 290a 2020 2020  f.ptt_off().    
-000135f0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00013600: 2020 2020 2020 2073 656c 662e 7074 745f         self.ptt_
-00013610: 6f6e 2829 0a20 2020 2020 2020 2066 6f72  on().        for
-00013620: 206c 6574 7465 7220 696e 2074 6865 5f73   letter in the_s
-00013630: 7472 696e 672e 6c6f 7765 7228 293a 0a20  tring.lower():. 
-00013640: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00013650: 7474 6572 2069 6e20 2261 6263 6465 6667  tter in "abcdefg
-00013660: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
-00013670: 7879 7a20 3132 3334 3536 3738 3930 223a  xyz 1234567890":
-00013680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013690: 2069 6620 6c65 7474 6572 203d 3d20 2220   if letter == " 
-000136a0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000136b0: 2020 2020 2020 206c 6574 7465 7220 3d20         letter = 
-000136c0: 2273 7061 6365 220a 2020 2020 2020 2020  "space".        
-000136d0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-000136e0: 203d 2066 227b 7374 7228 6f70 5f70 6174   = f"{str(op_pat
-000136f0: 6829 7d2f 7b6c 6574 7465 727d 2e77 6176  h)}/{letter}.wav
-00013700: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00013710: 2020 6966 2050 6174 6828 6669 6c65 6e61    if Path(filena
-00013720: 6d65 292e 6973 5f66 696c 6528 293a 0a20  me).is_file():. 
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00013750: 2256 6f69 6369 6e67 3a20 2573 222c 2066  "Voicing: %s", f
-00013760: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
-00013770: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00013780: 612c 205f 6673 203d 2073 662e 7265 6164  a, _fs = sf.read
-00013790: 2866 696c 656e 616d 652c 2064 7479 7065  (filename, dtype
-000137a0: 3d22 666c 6f61 7433 3222 290a 2020 2020  ="float32").    
-000137b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000137d0: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
-000137e0: 6465 6661 756c 742e 6465 7669 6365 203d  default.device =
-000137f0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00013800: 736f 756e 6464 6576 6963 6522 2c20 2264  sounddevice", "d
-00013810: 6566 6175 6c74 2229 0a20 2020 2020 2020  efault").       
-00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013830: 2073 642e 6465 6661 756c 742e 7361 6d70   sd.default.samp
-00013840: 6c65 7261 7465 203d 2034 3431 3030 2e30  lerate = 44100.0
-00013850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013860: 2020 2020 2020 2020 2073 642e 706c 6179           sd.play
-00013870: 2864 6174 612c 2062 6c6f 636b 696e 673d  (data, blocking=
-00013880: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00013890: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000138a0: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
-000138b0: 2c20 6622 7b73 642e 7761 6974 2829 7d22  , f"{sd.wait()}"
-000138c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000138d0: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
-000138e0: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
-000138f0: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
-00013900: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00013910: 6f67 6765 722e 7761 726e 696e 6728 2225  ogger.warning("%
-00013920: 7322 2c20 6622 7b65 7272 7d22 290a 2020  s", f"{err}").  
-00013930: 2020 2020 2020 7365 6c66 2e70 7474 5f6f        self.ptt_o
-00013940: 6666 2829 0a0a 2020 2020 6465 6620 7074  ff()..    def pt
-00013950: 745f 6f6e 2873 656c 6629 202d 3e20 4e6f  t_on(self) -> No
-00013960: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00013970: 2020 2020 2020 2020 5475 726e 206f 6e20          Turn on 
-00013980: 7074 7420 666f 7220 7269 672e 0a0a 2020  ptt for rig...  
-00013990: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000139a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000139b0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000139c0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000139d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000139e0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-000139f0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00013a00: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00013a10: 2822 5054 5420 4f6e 2229 0a20 2020 2020  ("PTT On").     
-00013a20: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-00013a30: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
-00013a40: 2020 2020 7365 6c66 2e6c 6566 7464 6f74      self.leftdot
-00013a50: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
-00013a60: 6772 6565 6e64 6f74 290a 2020 2020 2020  greendot).      
-00013a70: 2020 2020 2020 6170 702e 7072 6f63 6573        app.proces
-00013a80: 7345 7665 6e74 7328 290a 2020 2020 2020  sEvents().      
-00013a90: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-00013aa0: 6f6e 7472 6f6c 2e70 7474 5f6f 6e28 290a  ontrol.ptt_on().
-00013ab0: 0a20 2020 2064 6566 2070 7474 5f6f 6666  .    def ptt_off
-00013ac0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00013ad0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013ae0: 2020 2020 5475 726e 206f 6666 2070 7474      Turn off ptt
-00013af0: 2066 6f72 2072 6967 2e0a 0a20 2020 2020   for rig...     
-00013b00: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00013b10: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00013b20: 0a20 2020 2020 2020 204e 6f6e 650a 0a20  .        None.. 
-00013b30: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00013b40: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00013b50: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
-00013b60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013b70: 6c6f 6767 6572 2e64 6562 7567 2822 5054  logger.debug("PT
-00013b80: 5420 4f66 6622 290a 2020 2020 2020 2020  T Off").        
-00013b90: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00013ba0: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
-00013bb0: 2073 656c 662e 6c65 6674 646f 742e 7365   self.leftdot.se
-00013bc0: 7450 6978 6d61 7028 7365 6c66 2e72 6564  tPixmap(self.red
-00013bd0: 646f 7429 0a20 2020 2020 2020 2020 2020  dot).           
-00013be0: 2061 7070 2e70 726f 6365 7373 4576 656e   app.processEven
-00013bf0: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-00013c00: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-00013c10: 6c2e 7074 745f 6f66 6628 290a 0a20 2020  l.ptt_off()..   
-00013c20: 2064 6566 2070 726f 6365 7373 5f66 756e   def process_fun
-00013c30: 6374 696f 6e5f 6b65 7928 7365 6c66 2c20  ction_key(self, 
-00013c40: 6675 6e63 7469 6f6e 5f6b 6579 2920 2d3e  function_key) ->
-00013c50: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00013c60: 2222 0a20 2020 2020 2020 2043 616c 6c65  "".        Calle
-00013c70: 6420 7768 656e 2061 2066 756e 6374 696f  d when a functio
-00013c80: 6e20 6b65 7920 6973 2063 6c69 636b 6564  n key is clicked
-00013c90: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00013ca0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00013cb0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00013cc0: 2066 756e 6374 696f 6e5f 6b65 7920 3a20   function_key : 
-00013cd0: 5150 7573 6842 7574 746f 6e0a 2020 2020  QPushButton.    
-00013ce0: 2020 2020 4675 6e63 7469 6f6e 206b 6579      Function key
-00013cf0: 2074 6f20 7072 6f63 6573 732e 0a0a 2020   to process...  
-00013d00: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00013d10: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00013d20: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
-00013d30: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00013d40: 6c6f 6767 6572 2e64 6562 7567 2822 4675  logger.debug("Fu
-00013d50: 6e63 7469 6f6e 204b 6579 3a20 2573 222c  nction Key: %s",
-00013d60: 2066 756e 6374 696f 6e5f 6b65 792e 7465   function_key.te
-00013d70: 7874 2829 290a 2020 2020 2020 2020 6966  xt()).        if
-00013d80: 2073 656c 662e 6e31 6d6d 3a0a 2020 2020   self.n1mm:.    
-00013d90: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-00013da0: 6d2e 7261 6469 6f5f 696e 666f 5b22 4675  m.radio_info["Fu
-00013db0: 6e63 7469 6f6e 4b65 7943 6170 7469 6f6e  nctionKeyCaption
-00013dc0: 225d 203d 2066 756e 6374 696f 6e5f 6b65  "] = function_ke
-00013dd0: 792e 7465 7874 2829 0a20 2020 2020 2020  y.text().       
-00013de0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-00013df0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-00013e00: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-00013e10: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-00013e20: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-00013e30: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-00013e40: 6f63 6573 735f 6d61 6372 6f28 6675 6e63  ocess_macro(func
-00013e50: 7469 6f6e 5f6b 6579 2e74 6f6f 6c54 6970  tion_key.toolTip
-00013e60: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
-00013e70: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00013e80: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
-00013e90: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-00013ea0: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
-00013eb0: 6573 735f 6d61 6372 6f28 6675 6e63 7469  ess_macro(functi
-00013ec0: 6f6e 5f6b 6579 2e74 6f6f 6c54 6970 2829  on_key.toolTip()
-00013ed0: 2929 0a0a 2020 2020 6465 6620 7275 6e5f  ))..    def run_
-00013ee0: 7370 5f62 7574 746f 6e73 5f63 6c69 636b  sp_buttons_click
-00013ef0: 6564 2873 656c 6629 202d 3e20 4e6f 6e65  ed(self) -> None
-00013f00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013f10: 2020 2020 2020 4861 6e64 6c65 2052 756e        Handle Run
-00013f20: 2f53 2650 206d 6f64 6520 6368 616e 6765  /S&P mode change
-00013f30: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-00013f40: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00013f50: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00013f60: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
-00013f70: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00013f80: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00013f90: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00013fa0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-00013fb0: 6566 5b22 7275 6e5f 7374 6174 6522 5d20  ef["run_state"] 
-00013fc0: 3d20 7365 6c66 2e72 6164 696f 4275 7474  = self.radioButt
-00013fd0: 6f6e 5f72 756e 2e69 7343 6865 636b 6564  on_run.isChecked
-00013fe0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00013ff0: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-00014000: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00014010: 7265 6164 5f63 775f 6d61 6372 6f73 2829  read_cw_macros()
-00014020: 0a0a 2020 2020 6465 6620 7772 6974 655f  ..    def write_
-00014030: 7072 6566 6572 656e 6365 2873 656c 6629  preference(self)
-00014040: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00014050: 2020 2222 220a 2020 2020 2020 2020 5772    """.        Wr
-00014060: 6974 6520 7072 6566 6572 656e 6365 7320  ite preferences 
-00014070: 746f 2066 696c 652e 0a0a 2020 2020 2020  to file...      
-00014080: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00014090: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000140a0: 2020 2020 2020 2020 4e6f 6e65 0a0a 2020          None..  
-000140b0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-000140c0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-000140d0: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
-000140e0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-000140f0: 6c6f 6767 6572 2e64 6562 7567 2822 7772  logger.debug("wr
-00014100: 6974 6570 7265 6665 7265 6e63 6573 2229  itepreferences")
-00014110: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00014120: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-00014130: 7065 6e28 6673 7574 696c 732e 434f 4e46  pen(fsutils.CONF
-00014140: 4947 5f46 494c 452c 2022 7774 222c 2065  IG_FILE, "wt", e
-00014150: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-00014160: 2061 7320 6669 6c65 5f64 6573 6372 6970   as file_descrip
-00014170: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-00014180: 2020 2020 2066 696c 655f 6465 7363 7269       file_descri
-00014190: 7074 6f72 2e77 7269 7465 2864 756d 7073  ptor.write(dumps
-000141a0: 2873 656c 662e 7072 6566 2c20 696e 6465  (self.pref, inde
-000141b0: 6e74 3d34 2929 0a20 2020 2020 2020 2020  nt=4)).         
-000141c0: 2020 2020 2020 2023 206c 6f67 6765 722e         # logger.
-000141d0: 696e 666f 2822 7772 6974 696e 673a 2025  info("writing: %
-000141e0: 7322 2c20 7365 6c66 2e70 7265 6629 0a20  s", self.pref). 
-000141f0: 2020 2020 2020 2065 7863 6570 7420 494f         except IO
-00014200: 4572 726f 7220 6173 2065 7863 6570 7469  Error as excepti
-00014210: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00014220: 6c6f 6767 6572 2e63 7269 7469 6361 6c28  logger.critical(
-00014230: 2277 7269 7465 7072 6566 6572 656e 6365  "writepreference
-00014240: 733a 2025 7322 2c20 6578 6365 7074 696f  s: %s", exceptio
-00014250: 6e29 0a0a 2020 2020 6465 6620 7265 6164  n)..    def read
-00014260: 7072 6566 6572 656e 6365 7328 7365 6c66  preferences(self
-00014270: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00014280: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00014290: 6573 746f 7265 2070 7265 6665 7265 6e63  estore preferenc
-000142a0: 6573 2069 6620 7468 6579 2065 7869 7374  es if they exist
-000142b0: 2c20 6f74 6865 7277 6973 6520 6372 6561  , otherwise crea
-000142c0: 7465 2073 6f6d 6520 7361 6e65 2064 6566  te some sane def
-000142d0: 6175 6c74 732e 0a0a 2020 2020 2020 2020  aults...        
-000142e0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-000142f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00014300: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
-00014310: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00014320: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00014330: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00014340: 2022 2222 0a0a 2020 2020 2020 2020 6c6f   """..        lo
-00014350: 6767 6572 2e64 6562 7567 2822 7265 6164  gger.debug("read
-00014360: 7072 6566 6572 656e 6365 7322 290a 2020  preferences").  
-00014370: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00014380: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00014390: 682e 6578 6973 7473 2866 7375 7469 6c73  h.exists(fsutils
-000143a0: 2e43 4f4e 4649 475f 4649 4c45 293a 0a20  .CONFIG_FILE):. 
-000143b0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000143c0: 6974 6820 6f70 656e 280a 2020 2020 2020  ith open(.      
-000143d0: 2020 2020 2020 2020 2020 2020 2020 6673                fs
-000143e0: 7574 696c 732e 434f 4e46 4947 5f46 494c  utils.CONFIG_FIL
-000143f0: 452c 2022 7274 222c 2065 6e63 6f64 696e  E, "rt", encodin
-00014400: 673d 2275 7466 2d38 220a 2020 2020 2020  g="utf-8".      
-00014410: 2020 2020 2020 2020 2020 2920 6173 2066            ) as f
-00014420: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
-00014430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014440: 2020 2020 7365 6c66 2e70 7265 6620 3d20      self.pref = 
-00014450: 6c6f 6164 7328 6669 6c65 5f64 6573 6372  loads(file_descr
-00014460: 6970 746f 722e 7265 6164 2829 290a 2020  iptor.read()).  
-00014470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014480: 2020 6c6f 6767 6572 2e69 6e66 6f28 2225    logger.info("%
-00014490: 7322 2c20 7365 6c66 2e70 7265 6629 0a20  s", self.pref). 
-000144a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000144b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000144c0: 206c 6f67 6765 722e 696e 666f 2822 4e6f   logger.info("No
-000144d0: 2070 7265 6665 7265 6e63 6520 6669 6c65   preference file
-000144e0: 2e20 5772 6974 696e 6720 7072 6566 6572  . Writing prefer
-000144f0: 656e 6365 2e22 290a 2020 2020 2020 2020  ence.").        
-00014500: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00014510: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00014520: 2020 2020 2020 2066 7375 7469 6c73 2e43         fsutils.C
-00014530: 4f4e 4649 475f 4649 4c45 2c20 2277 7422  ONFIG_FILE, "wt"
-00014540: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00014550: 3822 0a20 2020 2020 2020 2020 2020 2020  8".             
-00014560: 2020 2029 2061 7320 6669 6c65 5f64 6573     ) as file_des
-00014570: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-00014580: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014590: 662e 7072 6566 203d 2073 656c 662e 7072  f.pref = self.pr
-000145a0: 6566 5f72 6566 2e63 6f70 7928 290a 2020  ef_ref.copy().  
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 2020 6669 6c65 5f64 6573 6372 6970 746f    file_descripto
-000145d0: 722e 7772 6974 6528 6475 6d70 7328 7365  r.write(dumps(se
-000145e0: 6c66 2e70 7265 662c 2069 6e64 656e 743d  lf.pref, indent=
-000145f0: 3429 290a 2020 2020 2020 2020 2020 2020  4)).            
-00014600: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00014610: 6e66 6f28 2225 7322 2c20 7365 6c66 2e70  nfo("%s", self.p
-00014620: 7265 6629 0a20 2020 2020 2020 2065 7863  ref).        exc
-00014630: 6570 7420 494f 4572 726f 7220 6173 2065  ept IOError as e
-00014640: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00014650: 2020 2020 2020 6c6f 6767 6572 2e63 7269        logger.cri
-00014660: 7469 6361 6c28 2245 7272 6f72 3a20 2573  tical("Error: %s
-00014670: 222c 2065 7863 6570 7469 6f6e 290a 0a20  ", exception).. 
-00014680: 2020 2020 2020 2073 656c 662e 6c6f 6f6b         self.look
-00014690: 5f75 7020 3d20 4e6f 6e65 0a20 2020 2020  _up = None.     
-000146a0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-000146b0: 6765 7428 2275 7365 7172 7a22 293a 0a20  get("useqrz"):. 
-000146c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000146d0: 6c6f 6f6b 5f75 7020 3d20 5152 5a6c 6f6f  look_up = QRZloo
-000146e0: 6b75 7028 0a20 2020 2020 2020 2020 2020  kup(.           
-000146f0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-00014700: 6574 2822 6c6f 6f6b 7570 7573 6572 6e61  et("lookupuserna
-00014710: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
-00014720: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-00014730: 6765 7428 226c 6f6f 6b75 7070 6173 7377  get("lookuppassw
-00014740: 6f72 6422 292c 0a20 2020 2020 2020 2020  ord"),.         
-00014750: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-00014760: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00014770: 7573 6568 616d 7174 6822 293a 0a20 2020  usehamqth"):.   
-00014780: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00014790: 6f6b 5f75 7020 3d20 4861 6d51 5448 280a  ok_up = HamQTH(.
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 7365 6c66 2e70 7265 662e 6765 7428 226c  self.pref.get("l
-000147c0: 6f6f 6b75 7075 7365 726e 616d 6522 292c  ookupusername"),
-000147d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000147e0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000147f0: 6c6f 6f6b 7570 7061 7373 776f 7264 2229  lookuppassword")
-00014800: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00014810: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00014820: 2e70 7265 662e 6765 7428 2272 756e 5f73  .pref.get("run_s
-00014830: 7461 7465 2229 3a0a 2020 2020 2020 2020  tate"):.        
-00014840: 2020 2020 7365 6c66 2e72 6164 696f 4275      self.radioBu
-00014850: 7474 6f6e 5f72 756e 2e73 6574 4368 6563  tton_run.setChec
-00014860: 6b65 6428 5472 7565 290a 2020 2020 2020  ked(True).      
-00014870: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014880: 2020 2020 7365 6c66 2e72 6164 696f 4275      self.radioBu
-00014890: 7474 6f6e 5f73 702e 7365 7443 6865 636b  tton_sp.setCheck
-000148a0: 6564 2854 7275 6529 0a0a 2020 2020 2020  ed(True)..      
-000148b0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-000148c0: 6574 2822 636f 6d6d 616e 645f 6275 7474  et("command_butt
-000148d0: 6f6e 7322 293a 0a20 2020 2020 2020 2020  ons"):.         
-000148e0: 2020 2073 656c 662e 6163 7469 6f6e 436f     self.actionCo
-000148f0: 6d6d 616e 645f 4275 7474 6f6e 732e 7365  mmand_Buttons.se
-00014900: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
-00014910: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00014920: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
-00014930: 7469 6f6e 436f 6d6d 616e 645f 4275 7474  tionCommand_Butt
-00014940: 6f6e 732e 7365 7443 6865 636b 6564 2846  ons.setChecked(F
-00014950: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
-00014960: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-00014970: 2263 775f 6d61 6372 6f73 2229 3a0a 2020  "cw_macros"):.  
-00014980: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00014990: 6374 696f 6e43 575f 4d61 6372 6f73 2e73  ctionCW_Macros.s
-000149a0: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
-000149b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000149c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000149d0: 6374 696f 6e43 575f 4d61 6372 6f73 2e73  ctionCW_Macros.s
-000149e0: 6574 4368 6563 6b65 6428 4661 6c73 6529  etChecked(False)
-000149f0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00014a00: 662e 7072 6566 2e67 6574 2822 6261 6e64  f.pref.get("band
-00014a10: 735f 6d6f 6465 7322 293a 0a20 2020 2020  s_modes"):.     
-00014a20: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00014a30: 6f6e 4d6f 6465 5f61 6e64 5f42 616e 6473  onMode_and_Bands
-00014a40: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
-00014a50: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00014a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014a70: 2e61 6374 696f 6e4d 6f64 655f 616e 645f  .actionMode_and_
-00014a80: 4261 6e64 732e 7365 7443 6865 636b 6564  Bands.setChecked
-00014a90: 2846 616c 7365 290a 0a20 2020 2020 2020  (False)..       
-00014aa0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-00014ab0: 696e 7465 7266 6163 6520 3d20 4d75 6c74  interface = Mult
-00014ac0: 6963 6173 7428 0a20 2020 2020 2020 2020  icast(.         
-00014ad0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-00014ae0: 2822 6d75 6c74 6963 6173 745f 6772 6f75  ("multicast_grou
-00014af0: 7022 2c20 2232 3339 2e31 2e31 2e31 2229  p", "239.1.1.1")
-00014b00: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00014b10: 6c66 2e70 7265 662e 6765 7428 226d 756c  lf.pref.get("mul
-00014b20: 7469 6361 7374 5f70 6f72 7422 2c20 3232  ticast_port", 22
-00014b30: 3339 292c 0a20 2020 2020 2020 2020 2020  39),.           
-00014b40: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00014b50: 696e 7465 7266 6163 655f 6970 222c 2022  interface_ip", "
-00014b60: 302e 302e 302e 3022 292c 0a20 2020 2020  0.0.0.0"),.     
-00014b70: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00014b80: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-00014b90: 7266 6163 652e 7265 6164 795f 7265 6164  rface.ready_read
-00014ba0: 5f63 6f6e 6e65 6374 2873 656c 662e 7761  _connect(self.wa
-00014bb0: 7463 685f 7564 7029 0a0a 2020 2020 2020  tch_udp)..      
-00014bc0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-00014bd0: 6574 2822 6461 726b 6d6f 6465 2229 3a0a  et("darkmode"):.
-00014be0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014bf0: 2e61 6374 696f 6e44 6172 6b5f 4d6f 6465  .actionDark_Mode
-00014c00: 5f32 2e73 6574 4368 6563 6b65 6428 5472  _2.setChecked(Tr
-00014c10: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-00014c20: 7365 6c66 2e73 6574 4461 726b 4d6f 6465  self.setDarkMode
-00014c30: 2854 7275 6529 0a20 2020 2020 2020 2065  (True).        e
-00014c40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014c50: 2073 656c 662e 7365 7444 6172 6b4d 6f64   self.setDarkMod
-00014c60: 6528 4661 6c73 6529 0a20 2020 2020 2020  e(False).       
-00014c70: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-00014c80: 4461 726b 5f4d 6f64 655f 322e 7365 7443  Dark_Mode_2.setC
-00014c90: 6865 636b 6564 2846 616c 7365 290a 0a20  hecked(False).. 
-00014ca0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
-00014cb0: 636f 6e74 726f 6c20 3d20 4e6f 6e65 0a0a  control = None..
-00014cc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014cd0: 7072 6566 2e67 6574 2822 7573 6566 6c72  pref.get("useflr
-00014ce0: 6967 222c 2046 616c 7365 293a 0a20 2020  ig", False):.   
-00014cf0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00014d00: 6465 6275 6728 0a20 2020 2020 2020 2020  debug(.         
-00014d10: 2020 2020 2020 2022 5573 696e 6720 666c         "Using fl
-00014d20: 7269 673a 2025 7322 2c0a 2020 2020 2020  rig: %s",.      
-00014d30: 2020 2020 2020 2020 2020 6622 7b73 656c            f"{sel
-00014d40: 662e 7072 6566 2e67 6574 2827 4341 545f  f.pref.get('CAT_
-00014d50: 6970 2729 7d20 7b73 656c 662e 7072 6566  ip')} {self.pref
-00014d60: 2e67 6574 2827 4341 545f 706f 7274 2729  .get('CAT_port')
-00014d70: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-00014d80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00014d90: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 203d  lf.rig_control =
-00014da0: 2043 4154 280a 2020 2020 2020 2020 2020   CAT(.          
-00014db0: 2020 2020 2020 2266 6c72 6967 222c 0a20        "flrig",. 
-00014dc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014dd0: 656c 662e 7072 6566 2e67 6574 2822 4341  elf.pref.get("CA
-00014de0: 545f 6970 222c 2022 3132 372e 302e 302e  T_ip", "127.0.0.
-00014df0: 3122 292c 0a20 2020 2020 2020 2020 2020  1"),.           
-00014e00: 2020 2020 2069 6e74 2873 656c 662e 7072       int(self.pr
-00014e10: 6566 2e67 6574 2822 4341 545f 706f 7274  ef.get("CAT_port
-00014e20: 222c 2031 3233 3435 2929 2c0a 2020 2020  ", 12345)),.    
-00014e30: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00014e40: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-00014e50: 6765 7428 2275 7365 7269 6763 746c 6422  get("userigctld"
-00014e60: 2c20 4661 6c73 6529 3a0a 2020 2020 2020  , False):.      
-00014e70: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00014e80: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
-00014e90: 2020 2020 2255 7369 6e67 2072 6967 6374      "Using rigct
-00014ea0: 6c64 3a20 2573 222c 0a20 2020 2020 2020  ld: %s",.       
-00014eb0: 2020 2020 2020 2020 2066 227b 7365 6c66           f"{self
-00014ec0: 2e70 7265 662e 6765 7428 2743 4154 5f69  .pref.get('CAT_i
-00014ed0: 7027 297d 207b 7365 6c66 2e70 7265 662e  p')} {self.pref.
-00014ee0: 6765 7428 2743 4154 5f70 6f72 7427 297d  get('CAT_port')}
-00014ef0: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00014f00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014f10: 662e 7269 675f 636f 6e74 726f 6c20 3d20  f.rig_control = 
-00014f20: 4341 5428 0a20 2020 2020 2020 2020 2020  CAT(.           
-00014f30: 2020 2020 2022 7269 6763 746c 6422 2c0a       "rigctld",.
-00014f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f50: 7365 6c66 2e70 7265 662e 6765 7428 2243  self.pref.get("C
-00014f60: 4154 5f69 7022 2c20 2231 3237 2e30 2e30  AT_ip", "127.0.0
-00014f70: 2e31 2229 2c0a 2020 2020 2020 2020 2020  .1"),.          
-00014f80: 2020 2020 2020 696e 7428 7365 6c66 2e70        int(self.p
-00014f90: 7265 662e 6765 7428 2243 4154 5f70 6f72  ref.get("CAT_por
-00014fa0: 7422 2c20 3435 3332 2929 2c0a 2020 2020  t", 4532)),.    
-00014fb0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00014fc0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-00014fd0: 6765 7428 2263 7774 7970 6522 2c20 3029  get("cwtype", 0)
-00014fe0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00014ff0: 2020 2073 656c 662e 6377 203d 204e 6f6e     self.cw = Non
-00015000: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-00015010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015020: 2e63 7720 3d20 4357 280a 2020 2020 2020  .cw = CW(.      
-00015030: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
-00015040: 6c66 2e70 7265 662e 6765 7428 2263 7774  lf.pref.get("cwt
-00015050: 7970 6522 2929 2c0a 2020 2020 2020 2020  ype")),.        
-00015060: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-00015070: 662e 6765 7428 2263 7769 7022 292c 0a20  f.get("cwip"),. 
-00015080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015090: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
-000150a0: 2822 6377 706f 7274 222c 2036 3738 3929  ("cwport", 6789)
-000150b0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-000150c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000150d0: 662e 6377 2e73 7065 6564 203d 2032 300a  f.cw.speed = 20.
-000150e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000150f0: 656c 662e 6377 2e73 6572 7665 7274 7970  elf.cw.servertyp
-00015100: 6520 3d3d 2032 3a0a 2020 2020 2020 2020  e == 2:.        
-00015110: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-00015120: 7365 745f 7769 6e6b 6579 6572 5f73 7065  set_winkeyer_spe
-00015130: 6564 2832 3029 0a0a 2020 2020 2020 2020  ed(20)..        
-00015140: 7365 6c66 2e6e 316d 6d20 3d20 4e6f 6e65  self.n1mm = None
-00015150: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00015160: 2e70 7265 662e 6765 7428 2273 656e 645f  .pref.get("send_
-00015170: 6e31 6d6d 5f70 6163 6b65 7473 222c 2046  n1mm_packets", F
-00015180: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
-00015190: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000151a0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-000151b0: 6d20 3d20 4e31 4d4d 280a 2020 2020 2020  m = N1MM(.      
-000151c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000151d0: 6c66 2e70 7265 662e 6765 7428 226e 316d  lf.pref.get("n1m
-000151e0: 6d5f 7261 6469 6f70 6f72 7422 2c20 2231  m_radioport", "1
-000151f0: 3237 2e30 2e30 2e31 3a31 3230 3630 2229  27.0.0.1:12060")
-00015200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015210: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-00015220: 6765 7428 226e 316d 6d5f 636f 6e74 6163  get("n1mm_contac
-00015230: 7470 6f72 7422 2c20 2231 3237 2e30 2e30  tport", "127.0.0
-00015240: 2e31 3a31 3230 3631 2229 2c0a 2020 2020  .1:12061"),.    
-00015250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015260: 7365 6c66 2e70 7265 662e 6765 7428 226e  self.pref.get("n
-00015270: 316d 6d5f 6c6f 6f6b 7570 706f 7274 222c  1mm_lookupport",
-00015280: 2022 3132 372e 302e 302e 313a 3132 3036   "127.0.0.1:1206
-00015290: 3022 292c 0a20 2020 2020 2020 2020 2020  0"),.           
-000152a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000152b0: 6566 2e67 6574 2822 6e31 6d6d 5f73 636f  ef.get("n1mm_sco
-000152c0: 7265 706f 7274 222c 2022 3132 372e 302e  report", "127.0.
-000152d0: 302e 313a 3132 3036 3022 292c 0a20 2020  0.1:12060"),.   
-000152e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000152f0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00015300: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
-00015310: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00015320: 6767 6572 2e77 6172 6e69 6e67 2822 2573  gger.warning("%s
-00015330: 222c 2066 227b 5661 6c75 6545 7272 6f72  ", f"{ValueError
-00015340: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00015350: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f72  self.n1mm.send_r
-00015360: 6164 696f 5f70 6163 6b65 7473 203d 2073  adio_packets = s
-00015370: 656c 662e 7072 6566 2e67 6574 2822 7365  elf.pref.get("se
-00015380: 6e64 5f6e 316d 6d5f 7261 6469 6f22 2c20  nd_n1mm_radio", 
-00015390: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-000153a0: 2020 2073 656c 662e 6e31 6d6d 2e73 656e     self.n1mm.sen
-000153b0: 645f 636f 6e74 6163 745f 7061 636b 6574  d_contact_packet
-000153c0: 7320 3d20 7365 6c66 2e70 7265 662e 6765  s = self.pref.ge
-000153d0: 7428 2273 656e 645f 6e31 6d6d 5f63 6f6e  t("send_n1mm_con
-000153e0: 7461 6374 222c 2046 616c 7365 290a 2020  tact", False).  
-000153f0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015400: 316d 6d2e 7365 6e64 5f6c 6f6f 6b75 705f  1mm.send_lookup_
-00015410: 7061 636b 6574 7320 3d20 7365 6c66 2e70  packets = self.p
-00015420: 7265 662e 6765 7428 2273 656e 645f 6e31  ref.get("send_n1
-00015430: 6d6d 5f6c 6f6f 6b75 7022 2c20 4661 6c73  mm_lookup", Fals
-00015440: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-00015450: 656c 662e 6e31 6d6d 2e73 656e 645f 7363  elf.n1mm.send_sc
-00015460: 6f72 655f 7061 636b 6574 7320 3d20 7365  ore_packets = se
-00015470: 6c66 2e70 7265 662e 6765 7428 2273 656e  lf.pref.get("sen
-00015480: 645f 6e31 6d6d 5f73 636f 7265 222c 2046  d_n1mm_score", F
-00015490: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-000154a0: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
-000154b0: 6f5f 696e 666f 5b22 5374 6174 696f 6e4e  o_info["StationN
-000154c0: 616d 6522 5d20 3d20 7365 6c66 2e70 7265  ame"] = self.pre
-000154d0: 662e 6765 7428 226e 316d 6d5f 7374 6174  f.get("n1mm_stat
-000154e0: 696f 6e5f 6e61 6d65 222c 2022 2229 0a0a  ion_name", "")..
-000154f0: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-00015500: 775f 636f 6d6d 616e 645f 6275 7474 6f6e  w_command_button
-00015510: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
-00015520: 2e73 686f 775f 4357 5f6d 6163 726f 7328  .show_CW_macros(
-00015530: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
-00015540: 6261 6e64 7320 6c69 7374 2069 7320 656d  bands list is em
-00015550: 7074 7920 6669 6c6c 2069 7420 7769 7468  pty fill it with
-00015560: 2048 462e 0a20 2020 2020 2020 2069 6620   HF..        if 
-00015570: 7365 6c66 2e70 7265 662e 6765 7428 2262  self.pref.get("b
-00015580: 616e 6473 222c 205b 5d29 203d 3d20 5b5d  ands", []) == []
-00015590: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000155a0: 6c66 2e70 7265 665b 2262 616e 6473 225d  lf.pref["bands"]
-000155b0: 203d 205b 2231 3630 222c 2022 3830 222c   = ["160", "80",
-000155c0: 2022 3430 222c 2022 3230 222c 2022 3135   "40", "20", "15
-000155d0: 222c 2022 3130 225d 0a0a 2020 2020 2020  ", "10"]..      
-000155e0: 2020 2320 4869 6465 2061 6c6c 2074 6865    # Hide all the
-000155f0: 2062 616e 6473 2061 6e64 2074 6865 6e20   bands and then 
-00015600: 7368 6f77 206f 6e6c 7920 7468 6520 7761  show only the wa
-00015610: 6e74 6564 2062 616e 6473 2e0a 2020 2020  nted bands..    
-00015620: 2020 2020 666f 7220 5f69 6e64 6963 6174      for _indicat
-00015630: 6f72 2069 6e20 5b0a 2020 2020 2020 2020  or in [.        
-00015640: 2020 2020 7365 6c66 2e62 616e 645f 696e      self.band_in
-00015650: 6469 6361 746f 7273 5f63 772c 0a20 2020  dicators_cw,.   
-00015660: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-00015670: 6e64 5f69 6e64 6963 6174 6f72 735f 7373  nd_indicators_ss
-00015680: 622c 0a20 2020 2020 2020 2020 2020 2073  b,.            s
-00015690: 656c 662e 6261 6e64 5f69 6e64 6963 6174  elf.band_indicat
-000156a0: 6f72 735f 7274 7479 2c0a 2020 2020 2020  ors_rtty,.      
-000156b0: 2020 5d3a 0a20 2020 2020 2020 2020 2020    ]:.           
-000156c0: 2066 6f72 205f 6261 6e64 696e 6420 696e   for _bandind in
-000156d0: 205f 696e 6469 6361 746f 722e 7661 6c75   _indicator.valu
-000156e0: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
-000156f0: 2020 2020 2020 5f62 616e 6469 6e64 2e68        _bandind.h
-00015700: 6964 6528 290a 2020 2020 2020 2020 2020  ide().          
-00015710: 2020 666f 7220 6261 6e64 5f74 6f5f 7368    for band_to_sh
-00015720: 6f77 2069 6e20 7365 6c66 2e70 7265 662e  ow in self.pref.
-00015730: 6765 7428 2262 616e 6473 222c 205b 5d29  get("bands", [])
-00015740: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015750: 2020 6966 2062 616e 645f 746f 5f73 686f    if band_to_sho
-00015760: 7720 696e 205f 696e 6469 6361 746f 723a  w in _indicator:
-00015770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015780: 2020 2020 205f 696e 6469 6361 746f 725b       _indicator[
-00015790: 6261 6e64 5f74 6f5f 7368 6f77 5d2e 7368  band_to_show].sh
-000157a0: 6f77 2829 0a20 2020 2020 2020 2023 2073  ow().        # s
-000157b0: 656c 662e 7368 6f77 5f62 616e 645f 6d6f  elf.show_band_mo
-000157c0: 6465 2829 0a0a 2020 2020 6465 6620 7761  de()..    def wa
-000157d0: 7463 685f 7564 7028 7365 6c66 2920 2d3e  tch_udp(self) ->
-000157e0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000157f0: 2222 0a20 2020 2020 2020 2057 6174 6368  "".        Watch
-00015800: 2074 6865 2055 4450 2073 6f63 6b65 7420   the UDP socket 
-00015810: 666f 7220 696e 636f 6d69 6e67 2064 6174  for incoming dat
-00015820: 612e 0a0a 2020 2020 2020 2020 5061 7261  a...        Para
-00015830: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00015840: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00015850: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
-00015860: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00015870: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00015880: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00015890: 0a0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-000158a0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-000158b0: 6e74 6572 6661 6365 2e68 6173 5f70 656e  nterface.has_pen
-000158c0: 6469 6e67 5f64 6174 6167 7261 6d73 2829  ding_datagrams()
-000158d0: 3a0a 2020 2020 2020 2020 2020 2020 6a73  :.            js
-000158e0: 6f6e 5f64 6174 6120 3d20 7365 6c66 2e6d  on_data = self.m
-000158f0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00015900: 6365 2e72 6561 645f 6461 7461 6772 616d  ce.read_datagram
-00015910: 5f61 735f 6a73 6f6e 2829 0a20 2020 2020  _as_json().     
-00015920: 2020 2020 2020 2069 6620 6a73 6f6e 5f64         if json_d
-00015930: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00015940: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00015950: 2020 2020 2020 2020 2020 2020 2020 6a73                js
-00015960: 6f6e 5f64 6174 612e 6765 7428 2263 6d64  on_data.get("cmd
-00015970: 222c 2022 2229 203d 3d20 2247 4554 434f  ", "") == "GETCO
-00015980: 4c55 4d4e 5322 0a20 2020 2020 2020 2020  LUMNS".         
-00015990: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
-000159a0: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
-000159b0: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
-000159c0: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000159e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000159f0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-00015a00: 2873 656c 662e 636f 6e74 6573 742c 2022  (self.contest, "
-00015a10: 636f 6c75 6d6e 7322 293a 0a20 2020 2020  columns"):.     
-00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a30: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
-00015a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a50: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
-00015a60: 2022 5348 4f57 434f 4c55 4d4e 5322 0a20   "SHOWCOLUMNS". 
-00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a80: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00015a90: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00015aa0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+0000e6e0: 2020 7365 6c66 2e63 6865 636b 5f63 616c    self.check_cal
+0000e6f0: 6c73 6967 6e28 7365 6c66 2e63 616c 6c73  lsign(self.calls
+0000e700: 6967 6e2e 7465 7874 2829 290a 2020 2020  ign.text()).    
+0000e710: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000e720: 656c 662e 6368 6563 6b5f 6475 7065 2873  elf.check_dupe(s
+0000e730: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
+0000e740: 7428 2929 3a0a 2020 2020 2020 2020 2020  t()):.          
+0000e750: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000e760: 7570 655f 696e 6469 6361 746f 722e 7368  upe_indicator.sh
+0000e770: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
+0000e780: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000e790: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e7a0: 656c 662e 6475 7065 5f69 6e64 6963 6174  elf.dupe_indicat
+0000e7b0: 6f72 2e68 6964 6528 290a 2020 2020 2020  or.hide().      
+0000e7c0: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+0000e7d0: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
+0000e7e0: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e800: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
+0000e810: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
+0000e820: 2e63 616c 6c73 6967 6e29 0a20 2020 2020  .callsign).     
+0000e830: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e840: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
+0000e850: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000e860: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+0000e870: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+0000e880: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e890: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
+0000e8a0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000e8b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000e8c0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0000e8d0: 7420 3d20 7365 6c66 2e63 616c 6c73 6967  t = self.callsig
+0000e8e0: 6e2e 7465 7874 2829 0a20 2020 2020 2020  n.text().       
+0000e8f0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0000e900: 7420 3d20 7465 7874 2e75 7070 6572 2829  t = text.upper()
+0000e910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e920: 2020 2020 205f 7468 6574 6872 6561 6420       _thethread 
+0000e930: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
+0000e940: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
+0000e950: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+0000e960: 6574 3d73 656c 662e 6368 6563 6b5f 6361  et=self.check_ca
+0000e970: 6c6c 7369 676e 322c 0a20 2020 2020 2020  llsign2,.       
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 2061 7267 733d 2874 6578 742c 292c 0a20   args=(text,),. 
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2020 2064 6165 6d6f 6e3d 5472         daemon=Tr
+0000e9c0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000e9d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 5f74                _t
+0000e9f0: 6865 7468 7265 6164 2e73 7461 7274 2829  hethread.start()
+0000ea00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea10: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
+0000ea20: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
+0000ea30: 7428 7365 6c66 2e63 616c 6c73 6967 6e29  t(self.callsign)
+0000ea40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea50: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
+0000ea60: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
+0000ea70: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+0000ea80: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
+0000ea90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eaa0: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
+0000eab0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
+0000eac0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000ead0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+0000eae0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+0000eaf0: 5f46 313a 0a20 2020 2020 2020 2020 2020  _F1:.           
+0000eb00: 2073 656c 662e 7072 6f63 6573 735f 6675   self.process_fu
+0000eb10: 6e63 7469 6f6e 5f6b 6579 2873 656c 662e  nction_key(self.
+0000eb20: 4631 290a 2020 2020 2020 2020 6966 2065  F1).        if e
+0000eb30: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+0000eb40: 2e4b 6579 5f46 323a 0a20 2020 2020 2020  .Key_F2:.       
+0000eb50: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
+0000eb60: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
+0000eb70: 656c 662e 4632 290a 2020 2020 2020 2020  elf.F2).        
+0000eb80: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+0000eb90: 3d20 5174 2e4b 6579 5f46 333a 0a20 2020  = Qt.Key_F3:.   
+0000eba0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000ebb0: 6f63 6573 735f 6675 6e63 7469 6f6e 5f6b  ocess_function_k
+0000ebc0: 6579 2873 656c 662e 4633 290a 2020 2020  ey(self.F3).    
+0000ebd0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+0000ebe0: 2829 203d 3d20 5174 2e4b 6579 5f46 343a  () == Qt.Key_F4:
+0000ebf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ec00: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
+0000ec10: 6f6e 5f6b 6579 2873 656c 662e 4634 290a  on_key(self.F4).
+0000ec20: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+0000ec30: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+0000ec40: 5f46 353a 0a20 2020 2020 2020 2020 2020  _F5:.           
+0000ec50: 2073 656c 662e 7072 6f63 6573 735f 6675   self.process_fu
+0000ec60: 6e63 7469 6f6e 5f6b 6579 2873 656c 662e  nction_key(self.
+0000ec70: 4635 290a 2020 2020 2020 2020 6966 2065  F5).        if e
+0000ec80: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+0000ec90: 2e4b 6579 5f46 363a 0a20 2020 2020 2020  .Key_F6:.       
+0000eca0: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
+0000ecb0: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
+0000ecc0: 656c 662e 4636 290a 2020 2020 2020 2020  elf.F6).        
+0000ecd0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+0000ece0: 3d20 5174 2e4b 6579 5f46 373a 0a20 2020  = Qt.Key_F7:.   
+0000ecf0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000ed00: 6f63 6573 735f 6675 6e63 7469 6f6e 5f6b  ocess_function_k
+0000ed10: 6579 2873 656c 662e 4637 290a 2020 2020  ey(self.F7).    
+0000ed20: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+0000ed30: 2829 203d 3d20 5174 2e4b 6579 5f46 383a  () == Qt.Key_F8:
+0000ed40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ed50: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
+0000ed60: 6f6e 5f6b 6579 2873 656c 662e 4638 290a  on_key(self.F8).
+0000ed70: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+0000ed80: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+0000ed90: 5f46 393a 0a20 2020 2020 2020 2020 2020  _F9:.           
+0000eda0: 2073 656c 662e 7072 6f63 6573 735f 6675   self.process_fu
+0000edb0: 6e63 7469 6f6e 5f6b 6579 2873 656c 662e  nction_key(self.
+0000edc0: 4639 290a 2020 2020 2020 2020 6966 2065  F9).        if e
+0000edd0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+0000ede0: 2e4b 6579 5f46 3130 3a0a 2020 2020 2020  .Key_F10:.      
+0000edf0: 2020 2020 2020 7365 6c66 2e70 726f 6365        self.proce
+0000ee00: 7373 5f66 756e 6374 696f 6e5f 6b65 7928  ss_function_key(
+0000ee10: 7365 6c66 2e46 3130 290a 2020 2020 2020  self.F10).      
+0000ee20: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+0000ee30: 203d 3d20 5174 2e4b 6579 5f46 3131 3a0a   == Qt.Key_F11:.
+0000ee40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ee50: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
+0000ee60: 6e5f 6b65 7928 7365 6c66 2e46 3131 290a  n_key(self.F11).
+0000ee70: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+0000ee80: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+0000ee90: 5f46 3132 3a0a 2020 2020 2020 2020 2020  _F12:.          
+0000eea0: 2020 7365 6c66 2e70 726f 6365 7373 5f66    self.process_f
+0000eeb0: 756e 6374 696f 6e5f 6b65 7928 7365 6c66  unction_key(self
+0000eec0: 2e46 3132 290a 0a20 2020 2064 6566 2073  .F12)..    def s
+0000eed0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
+0000eee0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000eef0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ef00: 2020 2053 6574 2077 696e 646f 7720 7469     Set window ti
+0000ef10: 746c 6520 6261 7365 6420 6f6e 2063 7572  tle based on cur
+0000ef20: 7265 6e74 2073 7461 7465 2e0a 2020 2020  rent state..    
+0000ef30: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000ef40: 2076 666f 6120 3d20 7365 6c66 2e72 6164   vfoa = self.rad
+0000ef50: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
+0000ef60: 6f61 222c 2022 2229 0a20 2020 2020 2020  oa", "").       
+0000ef70: 2069 6620 7666 6f61 3a0a 2020 2020 2020   if vfoa:.      
+0000ef80: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000ef90: 2020 2020 2020 2020 2020 2076 666f 6120             vfoa 
+0000efa0: 3d20 696e 7428 7666 6f61 2920 2f20 3130  = int(vfoa) / 10
+0000efb0: 3030 0a20 2020 2020 2020 2020 2020 2065  00.            e
+0000efc0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+0000efd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000efe0: 2020 7666 6f61 203d 2030 2e30 0a20 2020    vfoa = 0.0.   
+0000eff0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f000: 2020 2020 2020 2076 666f 6120 3d20 302e         vfoa = 0.
+0000f010: 300a 2020 2020 2020 2020 636f 6e74 6573  0.        contes
+0000f020: 745f 6e61 6d65 203d 2022 220a 2020 2020  t_name = "".    
+0000f030: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+0000f040: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
+0000f050: 2063 6f6e 7465 7374 5f6e 616d 6520 3d20   contest_name = 
+0000f060: 7365 6c66 2e63 6f6e 7465 7374 2e6e 616d  self.contest.nam
+0000f070: 650a 2020 2020 2020 2020 6c69 6e65 203d  e.        line =
+0000f080: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+0000f090: 2276 666f 613a 7b72 6f75 6e64 2876 666f  "vfoa:{round(vfo
+0000f0a0: 612c 3229 7d20 220a 2020 2020 2020 2020  a,2)} ".        
+0000f0b0: 2020 2020 6622 6d6f 6465 3a7b 7365 6c66      f"mode:{self
+0000f0c0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000f0d0: 2827 6d6f 6465 272c 2027 2729 7d20 220a  ('mode', '')} ".
+0000f0e0: 2020 2020 2020 2020 2020 2020 6622 4f50              f"OP
+0000f0f0: 3a7b 7365 6c66 2e63 7572 7265 6e74 5f6f  :{self.current_o
+0000f100: 707d 207b 636f 6e74 6573 745f 6e61 6d65  p} {contest_name
+0000f110: 7d20 220a 2020 2020 2020 2020 2020 2020  } ".            
+0000f120: 6622 2d20 4e6f 7431 4d4d 2076 7b5f 5f76  f"- Not1MM v{__v
+0000f130: 6572 7369 6f6e 5f5f 7d22 0a20 2020 2020  ersion__}".     
+0000f140: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+0000f150: 662e 7365 7457 696e 646f 7754 6974 6c65  f.setWindowTitle
+0000f160: 286c 696e 6529 0a0a 2020 2020 6465 6620  (line)..    def 
+0000f170: 7365 6e64 5f77 6f72 6b65 645f 6c69 7374  send_worked_list
+0000f180: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000f190: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f1a0: 2020 2020 5365 6e64 206d 6573 7361 6765      Send message
+0000f1b0: 2063 6f6e 7461 696e 696e 6720 776f 726b   containing work
+0000f1c0: 6564 2063 6f6e 7461 6374 7320 616e 6420  ed contacts and 
+0000f1d0: 6261 6e64 730a 0a20 2020 2020 2020 2050  bands..        P
+0000f1e0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000f1f0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000f200: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+0000f210: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0000f220: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0000f230: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+0000f240: 2222 220a 0a20 2020 2020 2020 2063 6d64  """..        cmd
+0000f250: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
+0000f260: 645b 2263 6d64 225d 203d 2022 574f 524b  d["cmd"] = "WORK
+0000f270: 4544 220a 2020 2020 2020 2020 636d 645b  ED".        cmd[
+0000f280: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+0000f290: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+0000f2a0: 2020 2020 2063 6d64 5b22 776f 726b 6564       cmd["worked
+0000f2b0: 225d 203d 2073 656c 662e 776f 726b 6564  "] = self.worked
+0000f2c0: 5f6c 6973 740a 2020 2020 2020 2020 6c6f  _list.        lo
+0000f2d0: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+0000f2e0: 2066 227b 636d 647d 2229 0a20 2020 2020   f"{cmd}").     
+0000f2f0: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
+0000f300: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
+0000f310: 5f61 735f 6a73 6f6e 2863 6d64 290a 0a20  _as_json(cmd).. 
+0000f320: 2020 2064 6566 2063 6c65 6172 696e 7075     def clearinpu
+0000f330: 7473 2873 656c 6629 202d 3e20 4e6f 6e65  ts(self) -> None
+0000f340: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f350: 2020 2020 2020 436c 6561 7273 2074 6865        Clears the
+0000f360: 2074 6578 7420 696e 7075 7420 6669 656c   text input fiel
+0000f370: 6473 2061 6e64 2073 6574 7320 666f 6375  ds and sets focu
+0000f380: 7320 746f 2063 616c 6c73 6967 6e20 6669  s to callsign fi
+0000f390: 656c 642e 0a0a 2020 2020 2020 2020 5061  eld...        Pa
+0000f3a0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000f3b0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000f3c0: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
+0000f3d0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000f3e0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000f3f0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+0000f400: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+0000f410: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
+0000f420: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
+0000f430: 656c 662e 636f 6e74 6163 7420 3d20 7365  elf.contact = se
+0000f440: 6c66 2e64 6174 6162 6173 652e 656d 7074  lf.database.empt
+0000f450: 795f 636f 6e74 6163 740a 2020 2020 2020  y_contact.      
+0000f460: 2020 7365 6c66 2e68 6561 6469 6e67 5f64    self.heading_d
+0000f470: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
+0000f480: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+0000f490: 2e64 785f 656e 7469 7479 2e73 6574 5465  .dx_entity.setTe
+0000f4a0: 7874 2822 2229 0a20 2020 2020 2020 2069  xt("").        i
+0000f4b0: 6620 7365 6c66 2e63 6f6e 7465 7374 3a0a  f self.contest:.
+0000f4c0: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
+0000f4d0: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
+0000f4e0: 2e73 686f 775f 6d75 6c74 7328 7365 6c66  .show_mults(self
+0000f4f0: 290a 2020 2020 2020 2020 2020 2020 7173  ).            qs
+0000f500: 6f73 203d 2073 656c 662e 636f 6e74 6573  os = self.contes
+0000f510: 742e 7368 6f77 5f71 736f 2873 656c 6629  t.show_qso(self)
+0000f520: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
+0000f530: 7473 7472 696e 6720 3d20 6622 7b71 736f  tstring = f"{qso
+0000f540: 737d 2f7b 6d75 6c74 737d 220a 2020 2020  s}/{mults}".    
+0000f550: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+0000f560: 7473 2e73 6574 5465 7874 286d 756c 7473  ts.setText(mults
+0000f570: 7472 696e 6729 0a20 2020 2020 2020 2020  tring).         
+0000f580: 2020 2073 636f 7265 203d 2073 656c 662e     score = self.
+0000f590: 636f 6e74 6573 742e 6361 6c63 5f73 636f  contest.calc_sco
+0000f5a0: 7265 2873 656c 6629 0a20 2020 2020 2020  re(self).       
+0000f5b0: 2020 2020 2073 656c 662e 7363 6f72 652e       self.score.
+0000f5c0: 7365 7454 6578 7428 7374 7228 7363 6f72  setText(str(scor
+0000f5d0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+0000f5e0: 7365 6c66 2e63 6f6e 7465 7374 2e72 6573  self.contest.res
+0000f5f0: 6574 5f6c 6162 656c 2873 656c 6629 0a20  et_label(self). 
+0000f600: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+0000f610: 7369 676e 2e63 6c65 6172 2829 0a20 2020  sign.clear().   
+0000f620: 2020 2020 2069 6620 7365 6c66 2e63 7572       if self.cur
+0000f630: 7265 6e74 5f6d 6f64 6520 3d3d 2022 4357  rent_mode == "CW
+0000f640: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+0000f650: 656c 662e 7365 6e74 2e73 6574 5465 7874  elf.sent.setText
+0000f660: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
+0000f670: 2020 2020 7365 6c66 2e72 6563 6569 7665      self.receive
+0000f680: 2e73 6574 5465 7874 2822 3539 3922 290a  .setText("599").
+0000f690: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000f6a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000f6b0: 656e 742e 7365 7454 6578 7428 2235 3922  ent.setText("59"
+0000f6c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000f6d0: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
+0000f6e0: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
+0000f6f0: 2073 656c 662e 6f74 6865 725f 312e 636c   self.other_1.cl
+0000f700: 6561 7228 290a 2020 2020 2020 2020 7365  ear().        se
+0000f710: 6c66 2e6f 7468 6572 5f32 2e63 6c65 6172  lf.other_2.clear
+0000f720: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000f730: 6361 6c6c 7369 676e 2e73 6574 466f 6375  callsign.setFocu
+0000f740: 7328 290a 2020 2020 2020 2020 636d 6420  s().        cmd 
+0000f750: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
+0000f760: 5b22 636d 6422 5d20 3d20 2243 414c 4c43  ["cmd"] = "CALLC
+0000f770: 4841 4e47 4544 220a 2020 2020 2020 2020  HANGED".        
+0000f780: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+0000f790: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+0000f7a0: 0a20 2020 2020 2020 2063 6d64 5b22 6361  .        cmd["ca
+0000f7b0: 6c6c 225d 203d 2022 220a 2020 2020 2020  ll"] = "".      
+0000f7c0: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+0000f7d0: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+0000f7e0: 6173 5f6a 736f 6e28 636d 6429 0a0a 2020  as_json(cmd)..  
+0000f7f0: 2020 6465 6620 7361 7665 5f63 6f6e 7461    def save_conta
+0000f800: 6374 2873 656c 6629 202d 3e20 4e6f 6e65  ct(self) -> None
+0000f810: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f820: 2020 2020 2020 5361 7665 2063 6f6e 7461        Save conta
+0000f830: 6374 2074 6f20 6461 7461 6261 7365 2e0a  ct to database..
+0000f840: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000f850: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000f860: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+0000f870: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
+0000f880: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0000f890: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+0000f8a0: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
+0000f8b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000f8c0: 6275 6728 2273 6176 696e 6720 636f 6e74  bug("saving cont
+0000f8d0: 6163 7422 290a 2020 2020 2020 2020 6966  act").        if
+0000f8e0: 2073 656c 662e 636f 6e74 6573 7420 6973   self.contest is
+0000f8f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000f900: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
+0000f910: 7361 6765 5f62 6f78 2822 596f 7520 6861  sage_box("You ha
+0000f920: 7665 206e 6f20 636f 6e74 6573 7420 6465  ve no contest de
+0000f930: 6669 6e65 642e 2229 0a20 2020 2020 2020  fined.").       
+0000f940: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000f950: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+0000f960: 6361 6c6c 7369 676e 2e74 6578 7428 2929  callsign.text())
+0000f970: 203c 2033 3a0a 2020 2020 2020 2020 2020   < 3:.          
+0000f980: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000f990: 2069 6620 6e6f 7420 616e 7928 6368 6172   if not any(char
+0000f9a0: 2e69 7364 6967 6974 2829 2066 6f72 2063  .isdigit() for c
+0000f9b0: 6861 7220 696e 2073 656c 662e 6361 6c6c  har in self.call
+0000f9c0: 7369 676e 2e74 6578 7428 2929 3a0a 2020  sign.text()):.  
+0000f9d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f9e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000f9f0: 616e 7928 6368 6172 2e69 7361 6c70 6861  any(char.isalpha
+0000fa00: 2829 2066 6f72 2063 6861 7220 696e 2073  () for char in s
+0000fa10: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
+0000fa20: 7428 2929 3a0a 2020 2020 2020 2020 2020  t()):.          
+0000fa30: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000fa40: 2073 656c 662e 636f 6e74 6163 745b 2254   self.contact["T
+0000fa50: 5322 5d20 3d20 6461 7465 7469 6d65 2e64  S"] = datetime.d
+0000fa60: 6174 6574 696d 652e 6e6f 7728 6461 7465  atetime.now(date
+0000fa70: 7469 6d65 2e74 696d 657a 6f6e 652e 7574  time.timezone.ut
+0000fa80: 6329 2e69 736f 666f 726d 6174 280a 2020  c).isoformat(.  
+0000fa90: 2020 2020 2020 2020 2020 2220 220a 2020            " ".  
+0000faa0: 2020 2020 2020 295b 3a31 395d 0a20 2020        )[:19].   
+0000fab0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000fac0: 745b 2243 616c 6c22 5d20 3d20 7365 6c66  t["Call"] = self
+0000fad0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+0000fae0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000faf0: 6e74 6163 745b 2246 7265 7122 5d20 3d20  ntact["Freq"] = 
+0000fb00: 726f 756e 6428 666c 6f61 7428 7365 6c66  round(float(self
+0000fb10: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000fb20: 2822 7666 6f61 222c 2030 2e30 2929 202f  ("vfoa", 0.0)) /
+0000fb30: 2031 3030 302c 2032 290a 2020 2020 2020   1000, 2).      
+0000fb40: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+0000fb50: 5153 5846 7265 7122 5d20 3d20 726f 756e  QSXFreq"] = roun
+0000fb60: 6428 0a20 2020 2020 2020 2020 2020 2066  d(.            f
+0000fb70: 6c6f 6174 2873 656c 662e 7261 6469 6f5f  loat(self.radio_
+0000fb80: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+0000fb90: 2c20 302e 3029 2920 2f20 3130 3030 2c20  , 0.0)) / 1000, 
+0000fba0: 320a 2020 2020 2020 2020 290a 2020 2020  2.        ).    
+0000fbb0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+0000fbc0: 5b22 4d6f 6465 225d 203d 2073 656c 662e  ["Mode"] = self.
+0000fbd0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000fbe0: 226d 6f64 6522 2c20 2222 290a 2020 2020  "mode", "").    
+0000fbf0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+0000fc00: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
+0000fc10: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e63  = self.contest.c
+0000fc20: 6162 7269 6c6c 6f5f 6e61 6d65 0a20 2020  abrillo_name.   
+0000fc30: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000fc40: 745b 2243 6f6e 7465 7374 4e52 225d 203d  t["ContestNR"] =
+0000fc50: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000fc60: 636f 6e74 6573 7422 2c20 2230 2229 0a20  contest", "0"). 
+0000fc70: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0000fc80: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
+0000fc90: 6978 225d 203d 2073 656c 662e 7374 6174  ix"] = self.stat
+0000fca0: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
+0000fcb0: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+0000fcc0: 2e63 6f6e 7461 6374 5b22 5750 5850 7265  .contact["WPXPre
+0000fcd0: 6669 7822 5d20 3d20 6361 6c63 756c 6174  fix"] = calculat
+0000fce0: 655f 7770 785f 7072 6566 6978 2873 656c  e_wpx_prefix(sel
+0000fcf0: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
+0000fd00: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000fd10: 636f 6e74 6163 745b 2249 7352 756e 5153  contact["IsRunQS
+0000fd20: 4f22 5d20 3d20 7365 6c66 2e72 6164 696f  O"] = self.radio
+0000fd30: 4275 7474 6f6e 5f72 756e 2e69 7343 6865  Button_run.isChe
+0000fd40: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
+0000fd50: 656c 662e 636f 6e74 6163 745b 224f 7065  elf.contact["Ope
+0000fd60: 7261 746f 7222 5d20 3d20 7365 6c66 2e63  rator"] = self.c
+0000fd70: 7572 7265 6e74 5f6f 700a 2020 2020 2020  urrent_op.      
+0000fd80: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+0000fd90: 4e65 7442 696f 734e 616d 6522 5d20 3d20  NetBiosName"] = 
+0000fda0: 736f 636b 6574 2e67 6574 686f 7374 6e61  socket.gethostna
+0000fdb0: 6d65 2829 0a20 2020 2020 2020 2073 656c  me().        sel
+0000fdc0: 662e 636f 6e74 6163 745b 2249 734f 7269  f.contact["IsOri
+0000fdd0: 6769 6e61 6c22 5d20 3d20 310a 2020 2020  ginal"] = 1.    
+0000fde0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+0000fdf0: 5b22 4944 225d 203d 2075 7569 642e 7575  ["ID"] = uuid.uu
+0000fe00: 6964 3428 292e 6865 780a 2020 2020 2020  id4().hex.      
+0000fe10: 2020 7365 6c66 2e63 6f6e 7465 7374 2e73    self.contest.s
+0000fe20: 6574 5f63 6f6e 7461 6374 5f76 6172 7328  et_contact_vars(
+0000fe30: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
+0000fe40: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
+0000fe50: 7473 225d 203d 2073 656c 662e 636f 6e74  ts"] = self.cont
+0000fe60: 6573 742e 706f 696e 7473 2873 656c 6629  est.points(self)
+0000fe70: 0a20 2020 2020 2020 2064 6562 7567 5f6f  .        debug_o
+0000fe80: 7574 7075 7420 3d20 6622 7b73 656c 662e  utput = f"{self.
+0000fe90: 636f 6e74 6163 747d 220a 2020 2020 2020  contact}".      
+0000fea0: 2020 6c6f 6767 6572 2e64 6562 7567 2864    logger.debug(d
+0000feb0: 6562 7567 5f6f 7574 7075 7429 0a0a 2020  ebug_output)..  
+0000fec0: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
+0000fed0: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
+0000fee0: 6c6f 6767 6572 2e64 6562 7567 2822 7061  logger.debug("pa
+0000fef0: 636b 6574 7320 2573 222c 2066 227b 7365  ckets %s", f"{se
+0000ff00: 6c66 2e6e 316d 6d2e 7365 6e64 5f63 6f6e  lf.n1mm.send_con
+0000ff10: 7461 6374 5f70 6163 6b65 7473 7d22 290a  tact_packets}").
+0000ff20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000ff30: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
+0000ff40: 6e74 6163 745f 7061 636b 6574 733a 0a20  ntact_packets:. 
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ff60: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000ff70: 5f69 6e66 6f5b 2274 696d 6573 7461 6d70  _info["timestamp
+0000ff80: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000ff90: 745b 2254 5322 5d0a 2020 2020 2020 2020  t["TS"].        
+0000ffa0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000ffb0: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000ffc0: 6f6c 6463 616c 6c22 5d20 3d20 7365 6c66  oldcall"] = self
+0000ffd0: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000ffe0: 666f 5b22 6361 6c6c 225d 203d 2028 0a20  fo["call"] = (. 
+0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010000: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00010010: 2243 616c 6c22 5d0a 2020 2020 2020 2020  "Call"].        
+00010020: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00010030: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00010040: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00010050: 5b22 7478 6672 6571 225d 203d 2073 656c  ["txfreq"] = sel
+00010060: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+00010070: 6e66 6f5b 2272 7866 7265 7122 5d20 3d20  nfo["rxfreq"] = 
+00010080: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010090: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+000100a0: 7261 6469 6f5f 696e 666f 5b22 4672 6571  radio_info["Freq
+000100b0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+000100c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000100d0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+000100e0: 6f6e 7461 6374 5f69 6e66 6f5b 226d 6f64  ontact_info["mod
+000100f0: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7461  e"] = self.conta
+00010100: 6374 5b22 4d6f 6465 225d 0a20 2020 2020  ct["Mode"].     
+00010110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010120: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+00010130: 6f5b 2263 6f6e 7465 7374 6e61 6d65 225d  o["contestname"]
+00010140: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+00010150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010160: 2020 2020 2022 436f 6e74 6573 744e 616d       "ContestNam
+00010170: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+00010180: 2020 205d 2e72 6570 6c61 6365 2822 2d22     ].replace("-"
+00010190: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
+000101a0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+000101b0: 636f 6e74 6163 745f 696e 666f 5b22 636f  contact_info["co
+000101c0: 6e74 6573 746e 7222 5d20 3d20 7365 6c66  ntestnr"] = self
+000101d0: 2e63 6f6e 7461 6374 5b22 436f 6e74 6573  .contact["Contes
+000101e0: 744e 5222 5d0a 2020 2020 2020 2020 2020  tNR"].          
+000101f0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00010200: 636f 6e74 6163 745f 696e 666f 5b22 7374  contact_info["st
+00010210: 6174 696f 6e70 7265 6669 7822 5d20 3d20  ationprefix"] = 
+00010220: 7365 6c66 2e63 6f6e 7461 6374 5b22 5374  self.contact["St
+00010230: 6174 696f 6e50 7265 6669 7822 5d0a 2020  ationPrefix"].  
+00010240: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010250: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+00010260: 696e 666f 5b22 7770 7870 7265 6669 7822  info["wpxprefix"
+00010270: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+00010280: 5b22 5750 5850 7265 6669 7822 5d0a 2020  ["WPXPrefix"].  
+00010290: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000102a0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+000102b0: 696e 666f 5b22 4973 5275 6e51 534f 225d  info["IsRunQSO"]
+000102c0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+000102d0: 2249 7352 756e 5153 4f22 5d0a 2020 2020  "IsRunQSO"].    
+000102e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000102f0: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+00010300: 666f 5b22 6f70 6572 6174 6f72 225d 203d  fo["operator"] =
+00010310: 2073 656c 662e 636f 6e74 6163 745b 224f   self.contact["O
+00010320: 7065 7261 746f 7222 5d0a 2020 2020 2020  perator"].      
+00010330: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00010340: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00010350: 5b22 6d79 6361 6c6c 225d 203d 2073 656c  ["mycall"] = sel
+00010360: 662e 636f 6e74 6163 745b 224f 7065 7261  f.contact["Opera
+00010370: 746f 7222 5d0a 2020 2020 2020 2020 2020  tor"].          
+00010380: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00010390: 636f 6e74 6163 745f 696e 666f 5b22 5374  contact_info["St
+000103a0: 6174 696f 6e4e 616d 6522 5d20 3d20 7365  ationName"] = se
+000103b0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+000103c0: 696e 666f 5b0a 2020 2020 2020 2020 2020  info[.          
+000103d0: 2020 2020 2020 2020 2020 224e 6574 4269            "NetBi
+000103e0: 6f73 4e61 6d65 220a 2020 2020 2020 2020  osName".        
+000103f0: 2020 2020 2020 2020 5d20 3d20 7365 6c66          ] = self
+00010400: 2e63 6f6e 7461 6374 5b22 4e65 7442 696f  .contact["NetBio
+00010410: 734e 616d 6522 5d0a 2020 2020 2020 2020  sName"].        
+00010420: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+00010430: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+00010440: 4973 4f72 6967 696e 616c 225d 203d 2073  IsOriginal"] = s
+00010450: 656c 662e 636f 6e74 6163 745b 2249 734f  elf.contact["IsO
+00010460: 7269 6769 6e61 6c22 5d0a 2020 2020 2020  riginal"].      
+00010470: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00010480: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00010490: 5b22 4944 225d 203d 2073 656c 662e 636f  ["ID"] = self.co
+000104a0: 6e74 6163 745b 2249 4422 5d0a 2020 2020  ntact["ID"].    
+000104b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000104c0: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+000104d0: 666f 5b22 706f 696e 7473 225d 203d 2073  fo["points"] = s
+000104e0: 656c 662e 636f 6e74 6163 745b 2250 6f69  elf.contact["Poi
+000104f0: 6e74 7322 5d0a 2020 2020 2020 2020 2020  nts"].          
+00010500: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00010510: 636f 6e74 6163 745f 696e 666f 5b22 736e  contact_info["sn
+00010520: 7422 5d20 3d20 7365 6c66 2e63 6f6e 7461  t"] = self.conta
+00010530: 6374 5b22 534e 5422 5d0a 2020 2020 2020  ct["SNT"].      
+00010540: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00010550: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00010560: 5b22 7263 7622 5d20 3d20 7365 6c66 2e63  ["rcv"] = self.c
+00010570: 6f6e 7461 6374 5b22 5243 5622 5d0a 2020  ontact["RCV"].  
+00010580: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010590: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+000105a0: 696e 666f 5b22 736e 746e 7222 5d20 3d20  info["sntnr"] = 
+000105b0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5365  self.contact["Se
+000105c0: 6e74 4e72 225d 0a20 2020 2020 2020 2020  ntNr"].         
+000105d0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+000105e0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2272  .contact_info["r
+000105f0: 6376 6e72 225d 203d 2073 656c 662e 636f  cvnr"] = self.co
+00010600: 6e74 6163 745b 224e 5222 5d0a 2020 2020  ntact["NR"].    
+00010610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010620: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+00010630: 666f 5b22 6973 6d75 6c74 6970 6c69 6572  fo["ismultiplier
+00010640: 3122 5d20 3d20 7365 6c66 2e63 6f6e 7461  1"] = self.conta
+00010650: 6374 2e67 6574 280a 2020 2020 2020 2020  ct.get(.        
+00010660: 2020 2020 2020 2020 2020 2020 2249 734d              "IsM
+00010670: 756c 7469 706c 6965 7231 222c 2030 0a20  ultiplier1", 0. 
+00010680: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106a0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+000106b0: 6374 5f69 6e66 6f5b 2269 736d 756c 7469  ct_info["ismulti
+000106c0: 706c 6965 7232 225d 203d 2073 656c 662e  plier2"] = self.
+000106d0: 636f 6e74 6163 742e 6765 7428 0a20 2020  contact.get(.   
+000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106f0: 2022 4973 4d75 6c74 6970 6c69 6572 3222   "IsMultiplier2"
+00010700: 2c20 300a 2020 2020 2020 2020 2020 2020  , 0.            
+00010710: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010720: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00010730: 636f 6e74 6163 745f 696e 666f 5b22 6973  contact_info["is
+00010740: 6d75 6c74 6970 6c69 6572 3322 5d20 3d20  multiplier3"] = 
+00010750: 7365 6c66 2e63 6f6e 7461 6374 2e67 6574  self.contact.get
+00010760: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010770: 2020 2020 2020 2249 734d 756c 7469 706c        "IsMultipl
+00010780: 6965 7233 222c 2030 0a20 2020 2020 2020  ier3", 0.       
+00010790: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000107a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000107b0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+000107c0: 6f5b 2273 6563 7469 6f6e 225d 203d 2073  o["section"] = s
+000107d0: 656c 662e 636f 6e74 6163 745b 2253 6563  elf.contact["Sec
+000107e0: 7422 5d0a 2020 2020 2020 2020 2020 2020  t"].            
+000107f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+00010800: 6e74 6163 745f 696e 666f 5b22 7072 6563  ntact_info["prec
+00010810: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+00010820: 745b 2250 7265 6322 5d0a 2020 2020 2020  t["Prec"].      
+00010830: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00010840: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00010850: 5b22 636b 225d 203d 2073 656c 662e 636f  ["ck"] = self.co
+00010860: 6e74 6163 745b 2243 4b22 5d0a 2020 2020  ntact["CK"].    
+00010870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010880: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+00010890: 666f 5b22 7a6e 225d 203d 2073 656c 662e  fo["zn"] = self.
+000108a0: 636f 6e74 6163 745b 225a 4e22 5d0a 2020  contact["ZN"].  
+000108b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000108c0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+000108d0: 696e 666f 5b22 706f 7765 7222 5d20 3d20  info["power"] = 
+000108e0: 7365 6c66 2e63 6f6e 7461 6374 5b22 506f  self.contact["Po
+000108f0: 7765 7222 5d0a 2020 2020 2020 2020 2020  wer"].          
+00010900: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00010910: 636f 6e74 6163 745f 696e 666f 5b22 6261  contact_info["ba
+00010920: 6e64 225d 203d 2073 656c 662e 636f 6e74  nd"] = self.cont
+00010930: 6163 745b 2242 616e 6422 5d0a 2020 2020  act["Band"].    
+00010940: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00010950: 6572 2e64 6562 7567 2822 2573 222c 2066  er.debug("%s", f
+00010960: 227b 7365 6c66 2e6e 316d 6d2e 636f 6e74  "{self.n1mm.cont
+00010970: 6163 745f 696e 666f 7d22 290a 2020 2020  act_info}").    
+00010980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010990: 2e6e 316d 6d2e 7365 6e64 5f63 6f6e 7461  .n1mm.send_conta
+000109a0: 6374 5f69 6e66 6f28 290a 0a20 2020 2020  ct_info()..     
+000109b0: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+000109c0: 2e6c 6f67 5f63 6f6e 7461 6374 2873 656c  .log_contact(sel
+000109d0: 662e 636f 6e74 6163 7429 0a20 2020 2020  f.contact).     
+000109e0: 2020 2073 656c 662e 776f 726b 6564 5f6c     self.worked_l
+000109f0: 6973 7420 3d20 7365 6c66 2e64 6174 6162  ist = self.datab
+00010a00: 6173 652e 6765 745f 6361 6c6c 735f 616e  ase.get_calls_an
+00010a10: 645f 6261 6e64 7328 290a 2020 2020 2020  d_bands().      
+00010a20: 2020 7365 6c66 2e73 656e 645f 776f 726b    self.send_work
+00010a30: 6564 5f6c 6973 7428 290a 2020 2020 2020  ed_list().      
+00010a40: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+00010a50: 7473 2829 0a0a 2020 2020 2020 2020 636d  ts()..        cm
+00010a60: 6420 3d20 7b7d 0a20 2020 2020 2020 2063  d = {}.        c
+00010a70: 6d64 5b22 636d 6422 5d20 3d20 2255 5044  md["cmd"] = "UPD
+00010a80: 4154 454c 4f47 220a 2020 2020 2020 2020  ATELOG".        
+00010a90: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+00010aa0: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00010ab0: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
+00010ac0: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+00010ad0: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
+00010ae0: 6d64 290a 0a20 2020 2064 6566 206e 6577  md)..    def new
+00010af0: 5f63 6f6e 7465 7374 5f64 6961 6c6f 6728  _contest_dialog(
+00010b00: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00010b10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010b20: 2020 2053 686f 7720 6e65 7720 636f 6e74     Show new cont
+00010b30: 6573 7420 6469 616c 6f67 2e0a 0a20 2020  est dialog...   
+00010b40: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00010b50: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00010b60: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00010b70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00010b80: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00010b90: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+00010ba0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00010bb0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00010bc0: 224e 6577 2063 6f6e 7465 7374 2044 6961  "New contest Dia
+00010bd0: 6c6f 6722 290a 0a20 2020 2020 2020 2073  log")..        s
+00010be0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00010bf0: 6f67 203d 204e 6577 436f 6e74 6573 7428  og = NewContest(
+00010c00: 6673 7574 696c 732e 4150 505f 4441 5441  fsutils.APP_DATA
+00010c10: 5f50 4154 4829 0a20 2020 2020 2020 2069  _PATH).        i
+00010c20: 6620 7365 6c66 2e63 7572 7265 6e74 5f70  f self.current_p
+00010c30: 616c 6574 7465 3a0a 2020 2020 2020 2020  alette:.        
+00010c40: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00010c50: 5f64 6961 6c6f 672e 7365 7450 616c 6574  _dialog.setPalet
+00010c60: 7465 2873 656c 662e 6375 7272 656e 745f  te(self.current_
+00010c70: 7061 6c65 7474 6529 0a20 2020 2020 2020  palette).       
+00010c80: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00010c90: 745f 6469 616c 6f67 2e65 7863 6861 6e67  t_dialog.exchang
+00010ca0: 652e 7365 7450 616c 6574 7465 2873 656c  e.setPalette(sel
+00010cb0: 662e 6375 7272 656e 745f 7061 6c65 7474  f.current_palett
+00010cc0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00010cd0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00010ce0: 6f67 2e6f 7065 7261 746f 7273 2e73 6574  og.operators.set
+00010cf0: 5061 6c65 7474 6528 7365 6c66 2e63 7572  Palette(self.cur
+00010d00: 7265 6e74 5f70 616c 6574 7465 290a 0a20  rent_palette).. 
+00010d10: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00010d20: 6573 745f 6469 616c 6f67 2e61 6363 6570  est_dialog.accep
+00010d30: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
+00010d40: 2e73 6176 655f 636f 6e74 6573 7429 0a20  .save_contest). 
+00010d50: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00010d60: 6573 745f 6469 616c 6f67 2e64 6174 6554  est_dialog.dateT
+00010d70: 696d 6545 6469 742e 7365 7444 6174 6528  imeEdit.setDate(
+00010d80: 5174 436f 7265 2e51 4461 7465 2e63 7572  QtCore.QDate.cur
+00010d90: 7265 6e74 4461 7465 2829 290a 2020 2020  rentDate()).    
+00010da0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00010db0: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+00010dc0: 4564 6974 2e73 6574 4361 6c65 6e64 6172  Edit.setCalendar
+00010dd0: 506f 7075 7028 5472 7565 290a 2020 2020  Popup(True).    
+00010de0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00010df0: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+00010e00: 4564 6974 2e73 6574 5469 6d65 2851 7443  Edit.setTime(QtC
+00010e10: 6f72 652e 5154 696d 6528 302c 2030 2929  ore.QTime(0, 0))
+00010e20: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00010e30: 6e74 6573 745f 6469 616c 6f67 2e70 6f77  ntest_dialog.pow
+00010e40: 6572 2e73 6574 4375 7272 656e 7454 6578  er.setCurrentTex
+00010e50: 7428 224c 4f57 2229 0a20 2020 2020 2020  t("LOW").       
+00010e60: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00010e70: 616c 6f67 2e73 7461 7469 6f6e 2e73 6574  alog.station.set
+00010e80: 4375 7272 656e 7454 6578 7428 2246 4958  CurrentText("FIX
+00010e90: 4544 2229 0a20 2020 2020 2020 2073 656c  ED").        sel
+00010ea0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00010eb0: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
+00010ec0: 2073 6176 655f 636f 6e74 6573 7428 7365   save_contest(se
+00010ed0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00010ee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010ef0: 2053 6176 6520 436f 6e74 6573 7420 746f   Save Contest to
+00010f00: 2064 6174 6162 6173 652e 0a0a 2020 2020   database...    
+00010f10: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00010f20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00010f30: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
+00010f40: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00010f50: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00010f60: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+00010f70: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00010f80: 2020 6e65 7874 5f6e 756d 6265 7220 3d20    next_number = 
+00010f90: 7365 6c66 2e64 6174 6162 6173 652e 6765  self.database.ge
+00010fa0: 745f 6e65 7874 5f63 6f6e 7465 7374 5f6e  t_next_contest_n
+00010fb0: 7228 290a 2020 2020 2020 2020 636f 6e74  r().        cont
+00010fc0: 6573 7420 3d20 7b7d 0a20 2020 2020 2020  est = {}.       
+00010fd0: 2063 6f6e 7465 7374 5b22 436f 6e74 6573   contest["Contes
+00010fe0: 744e 616d 6522 5d20 3d20 280a 2020 2020  tName"] = (.    
+00010ff0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00011000: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
+00011010: 6573 742e 6375 7272 656e 7454 6578 7428  est.currentText(
+00011020: 292e 6c6f 7765 7228 292e 7265 706c 6163  ).lower().replac
+00011030: 6528 2220 222c 2022 5f22 290a 2020 2020  e(" ", "_").    
+00011040: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+00011050: 6e74 6573 745b 2253 7461 7274 4461 7465  ntest["StartDate
+00011060: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+00011070: 745f 6469 616c 6f67 2e64 6174 6554 696d  t_dialog.dateTim
+00011080: 6545 6469 742e 6461 7465 5469 6d65 2829  eEdit.dateTime()
+00011090: 2e74 6f53 7472 696e 6728 0a20 2020 2020  .toString(.     
+000110a0: 2020 2020 2020 2022 7979 7979 2d4d 4d2d         "yyyy-MM-
+000110b0: 6464 2068 683a 6d6d 3a73 7322 0a20 2020  dd hh:mm:ss".   
+000110c0: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+000110d0: 6f6e 7465 7374 5b22 4f70 6572 6174 6f72  ontest["Operator
+000110e0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+000110f0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00011100: 2e6f 7065 7261 746f 725f 636c 6173 732e  .operator_class.
+00011110: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
+00011120: 2020 2020 2020 636f 6e74 6573 745b 2242        contest["B
+00011130: 616e 6443 6174 6567 6f72 7922 5d20 3d20  andCategory"] = 
+00011140: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00011150: 6c6f 672e 6261 6e64 2e63 7572 7265 6e74  log.band.current
+00011160: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+00011170: 6f6e 7465 7374 5b22 506f 7765 7243 6174  ontest["PowerCat
+00011180: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+00011190: 6f6e 7465 7374 5f64 6961 6c6f 672e 706f  ontest_dialog.po
+000111a0: 7765 722e 6375 7272 656e 7454 6578 7428  wer.currentText(
+000111b0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+000111c0: 745b 224d 6f64 6543 6174 6567 6f72 7922  t["ModeCategory"
+000111d0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+000111e0: 5f64 6961 6c6f 672e 6d6f 6465 2e63 7572  _dialog.mode.cur
+000111f0: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
+00011200: 2020 2063 6f6e 7465 7374 5b22 4f76 6572     contest["Over
+00011210: 6c61 7943 6174 6567 6f72 7922 5d20 3d20  layCategory"] = 
+00011220: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00011230: 6c6f 672e 6f76 6572 6c61 792e 6375 7272  log.overlay.curr
+00011240: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
+00011250: 2020 2320 636f 6e74 6573 745b 2743 6c61    # contest['Cla
+00011260: 696d 6564 5363 6f72 6527 5d20 3d20 7365  imedScore'] = se
+00011270: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00011280: 672e 0a20 2020 2020 2020 2063 6f6e 7465  g..        conte
+00011290: 7374 5b22 4f70 6572 6174 6f72 7322 5d20  st["Operators"] 
+000112a0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+000112b0: 6961 6c6f 672e 6f70 6572 6174 6f72 732e  ialog.operators.
+000112c0: 7465 7874 2829 0a20 2020 2020 2020 2063  text().        c
+000112d0: 6f6e 7465 7374 5b22 536f 6170 626f 7822  ontest["Soapbox"
+000112e0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+000112f0: 5f64 6961 6c6f 672e 736f 6170 626f 782e  _dialog.soapbox.
+00011300: 746f 506c 6169 6e54 6578 7428 290a 2020  toPlainText().  
+00011310: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
+00011320: 656e 7445 7863 6861 6e67 6522 5d20 3d20  entExchange"] = 
+00011330: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00011340: 6c6f 672e 6578 6368 616e 6765 2e74 6578  log.exchange.tex
+00011350: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
+00011360: 6573 745b 2243 6f6e 7465 7374 4e52 225d  est["ContestNR"]
+00011370: 203d 206e 6578 745f 6e75 6d62 6572 2e67   = next_number.g
+00011380: 6574 2822 636f 756e 7422 2c20 3129 0a20  et("count", 1). 
+00011390: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+000113a0: 5b22 636f 6e74 6573 7422 5d20 3d20 6e65  ["contest"] = ne
+000113b0: 7874 5f6e 756d 6265 722e 6765 7428 2263  xt_number.get("c
+000113c0: 6f75 6e74 222c 2031 290a 2020 2020 2020  ount", 1).      
+000113d0: 2020 2320 636f 6e74 6573 745b 2753 7562    # contest['Sub
+000113e0: 5479 7065 275d 203d 2073 656c 662e 636f  Type'] = self.co
+000113f0: 6e74 6573 745f 6469 616c 6f67 2e0a 2020  ntest_dialog..  
+00011400: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
+00011410: 7461 7469 6f6e 4361 7465 676f 7279 225d  tationCategory"]
+00011420: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00011430: 6469 616c 6f67 2e73 7461 7469 6f6e 2e63  dialog.station.c
+00011440: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+00011450: 2020 2020 2063 6f6e 7465 7374 5b22 4173       contest["As
+00011460: 7369 7374 6564 4361 7465 676f 7279 225d  sistedCategory"]
+00011470: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00011480: 6469 616c 6f67 2e61 7373 6973 7465 642e  dialog.assisted.
+00011490: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
+000114a0: 2020 2020 2020 636f 6e74 6573 745b 2254        contest["T
+000114b0: 7261 6e73 6d69 7474 6572 4361 7465 676f  ransmitterCatego
+000114c0: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
+000114d0: 6573 745f 6469 616c 6f67 2e74 7261 6e73  est_dialog.trans
+000114e0: 6d69 7474 6572 2e63 7572 7265 6e74 5465  mitter.currentTe
+000114f0: 7874 2829 0a20 2020 2020 2020 2023 2063  xt().        # c
+00011500: 6f6e 7465 7374 5b27 5469 6d65 4361 7465  ontest['TimeCate
+00011510: 676f 7279 275d 203d 2073 656c 662e 636f  gory'] = self.co
+00011520: 6e74 6573 745f 6469 616c 6f67 2e0a 2020  ntest_dialog..  
+00011530: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00011540: 7567 2822 2573 222c 2066 227b 636f 6e74  ug("%s", f"{cont
+00011550: 6573 747d 2229 0a20 2020 2020 2020 2073  est}").        s
+00011560: 656c 662e 6461 7461 6261 7365 2e61 6464  elf.database.add
+00011570: 5f63 6f6e 7465 7374 2863 6f6e 7465 7374  _contest(contest
+00011580: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
+00011590: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+000115a0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000115b0: 6f61 645f 636f 6e74 6573 7428 290a 0a20  oad_contest().. 
+000115c0: 2020 2064 6566 2065 6469 745f 7374 6174     def edit_stat
+000115d0: 696f 6e5f 7365 7474 696e 6773 2873 656c  ion_settings(sel
+000115e0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+000115f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011600: 5368 6f77 2073 6574 7469 6e67 7320 6469  Show settings di
+00011610: 616c 6f67 2066 6f72 2073 7461 7469 6f6e  alog for station
+00011620: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00011630: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00011640: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00011650: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
+00011660: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00011670: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00011680: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+00011690: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+000116a0: 6465 6275 6728 2253 7461 7469 6f6e 2053  debug("Station S
+000116b0: 6574 7469 6e67 7320 7365 6c65 6374 6564  ettings selected
+000116c0: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000116d0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+000116e0: 203d 2045 6469 7453 7461 7469 6f6e 2866   = EditStation(f
+000116f0: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
+00011700: 5041 5448 290a 2020 2020 2020 2020 6966  PATH).        if
+00011710: 2073 656c 662e 6375 7272 656e 745f 7061   self.current_pa
+00011720: 6c65 7474 653a 0a20 2020 2020 2020 2020  lette:.         
+00011730: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+00011740: 5f64 6961 6c6f 672e 7365 7450 616c 6574  _dialog.setPalet
+00011750: 7465 2873 656c 662e 6375 7272 656e 745f  te(self.current_
+00011760: 7061 6c65 7474 6529 0a0a 2020 2020 2020  palette)..      
+00011770: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00011780: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
+00011790: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+000117a0: 655f 7365 7474 696e 6773 290a 2020 2020  e_settings).    
+000117b0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+000117c0: 735f 6469 616c 6f67 2e43 616c 6c2e 7365  s_dialog.Call.se
+000117d0: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+000117e0: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
+000117f0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00011800: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00011810: 2e4e 616d 652e 7365 7454 6578 7428 7365  .Name.setText(se
+00011820: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+00011830: 4e61 6d65 222c 2022 2229 290a 2020 2020  Name", "")).    
+00011840: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+00011850: 735f 6469 616c 6f67 2e41 6464 7265 7373  s_dialog.Address
+00011860: 312e 7365 7454 6578 7428 7365 6c66 2e73  1.setText(self.s
+00011870: 7461 7469 6f6e 2e67 6574 2822 5374 7265  tation.get("Stre
+00011880: 6574 3122 2c20 2222 2929 0a20 2020 2020  et1", "")).     
+00011890: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+000118a0: 5f64 6961 6c6f 672e 4164 6472 6573 7332  _dialog.Address2
+000118b0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+000118c0: 6174 696f 6e2e 6765 7428 2253 7472 6565  ation.get("Stree
+000118d0: 7432 222c 2022 2229 290a 2020 2020 2020  t2", "")).      
+000118e0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+000118f0: 6469 616c 6f67 2e43 6974 792e 7365 7454  dialog.City.setT
+00011900: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+00011910: 2e67 6574 2822 4369 7479 222c 2022 2229  .get("City", "")
+00011920: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00011930: 6574 7469 6e67 735f 6469 616c 6f67 2e53  ettings_dialog.S
+00011940: 7461 7465 2e73 6574 5465 7874 2873 656c  tate.setText(sel
+00011950: 662e 7374 6174 696f 6e2e 6765 7428 2253  f.station.get("S
+00011960: 7461 7465 222c 2022 2229 290a 2020 2020  tate", "")).    
+00011970: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+00011980: 735f 6469 616c 6f67 2e5a 6970 2e73 6574  s_dialog.Zip.set
+00011990: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+000119a0: 6e2e 6765 7428 225a 6970 222c 2022 2229  n.get("Zip", "")
+000119b0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000119c0: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+000119d0: 6f75 6e74 7279 2e73 6574 5465 7874 2873  ountry.setText(s
+000119e0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+000119f0: 2243 6f75 6e74 7279 222c 2022 2229 290a  "Country", "")).
+00011a00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00011a10: 7469 6e67 735f 6469 616c 6f67 2e47 7269  tings_dialog.Gri
+00011a20: 6453 7175 6172 652e 7365 7454 6578 7428  dSquare.setText(
+00011a30: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+00011a40: 2822 4772 6964 5371 7561 7265 222c 2022  ("GridSquare", "
+00011a50: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00011a60: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00011a70: 2e43 515a 6f6e 652e 7365 7454 6578 7428  .CQZone.setText(
+00011a80: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
+00011a90: 2e67 6574 2822 4351 5a6f 6e65 222c 2022  .get("CQZone", "
+00011aa0: 2229 2929 0a20 2020 2020 2020 2073 656c  "))).        sel
+00011ab0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+00011ac0: 672e 4954 555a 6f6e 652e 7365 7454 6578  g.ITUZone.setTex
+00011ad0: 7428 7374 7228 7365 6c66 2e73 7461 7469  t(str(self.stati
+00011ae0: 6f6e 2e67 6574 2822 4941 5255 5a6f 6e65  on.get("IARUZone
+00011af0: 222c 2022 2229 2929 0a20 2020 2020 2020  ", ""))).       
+00011b00: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+00011b10: 6961 6c6f 672e 4c69 6365 6e73 652e 7365  ialog.License.se
+00011b20: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+00011b30: 6f6e 2e67 6574 2822 4c69 6365 6e73 6543  on.get("LicenseC
+00011b40: 6c61 7373 222c 2022 2229 290a 2020 2020  lass", "")).    
+00011b50: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+00011b60: 735f 6469 616c 6f67 2e4c 6174 6974 7564  s_dialog.Latitud
+00011b70: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
+00011b80: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+00011b90: 4c61 7469 7475 6465 222c 2022 2229 2929  Latitude", "")))
+00011ba0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00011bb0: 7474 696e 6773 5f64 6961 6c6f 672e 4c6f  ttings_dialog.Lo
+00011bc0: 6e67 6974 7564 652e 7365 7454 6578 7428  ngitude.setText(
+00011bd0: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
+00011be0: 2e67 6574 2822 4c6f 6e67 6974 7564 6522  .get("Longitude"
+00011bf0: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
+00011c00: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+00011c10: 616c 6f67 2e53 7461 7469 6f6e 5458 5258  alog.StationTXRX
+00011c20: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+00011c30: 6174 696f 6e2e 6765 7428 2273 7461 7469  ation.get("stati
+00011c40: 6f6e 7478 7278 222c 2022 2229 290a 2020  ontxrx", "")).  
+00011c50: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+00011c60: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
+00011c70: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+00011c80: 6174 696f 6e2e 6765 7428 2253 506f 7765  ation.get("SPowe
+00011c90: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+00011ca0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+00011cb0: 616c 6f67 2e41 6e74 656e 6e61 2e73 6574  alog.Antenna.set
+00011cc0: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+00011cd0: 6e2e 6765 7428 2253 416e 7465 222c 2022  n.get("SAnte", "
+00011ce0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00011cf0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00011d00: 2e41 6e74 4865 6967 6874 2e73 6574 5465  .AntHeight.setTe
+00011d10: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+00011d20: 6765 7428 2253 416e 7448 3122 2c20 2222  get("SAntH1", ""
+00011d30: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00011d40: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+00011d50: 4153 4c2e 7365 7454 6578 7428 7365 6c66  ASL.setText(self
+00011d60: 2e73 7461 7469 6f6e 2e67 6574 2822 5341  .station.get("SA
+00011d70: 6e74 4832 222c 2022 2229 290a 2020 2020  ntH2", "")).    
+00011d80: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+00011d90: 735f 6469 616c 6f67 2e41 5252 4c53 6563  s_dialog.ARRLSec
+00011da0: 7469 6f6e 2e73 6574 5465 7874 2873 656c  tion.setText(sel
+00011db0: 662e 7374 6174 696f 6e2e 6765 7428 2241  f.station.get("A
+00011dc0: 5252 4c53 6563 7469 6f6e 222c 2022 2229  RRLSection", "")
+00011dd0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00011de0: 6574 7469 6e67 735f 6469 616c 6f67 2e52  ettings_dialog.R
+00011df0: 6f76 6572 5154 482e 7365 7454 6578 7428  overQTH.setText(
+00011e00: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+00011e10: 2822 526f 7665 7251 5448 222c 2022 2229  ("RoverQTH", "")
+00011e20: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00011e30: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+00011e40: 6c75 622e 7365 7454 6578 7428 7365 6c66  lub.setText(self
+00011e50: 2e73 7461 7469 6f6e 2e67 6574 2822 436c  .station.get("Cl
+00011e60: 7562 222c 2022 2229 290a 2020 2020 2020  ub", "")).      
+00011e70: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00011e80: 6469 616c 6f67 2e45 6d61 696c 2e73 6574  dialog.Email.set
+00011e90: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+00011ea0: 6e2e 6765 7428 2245 6d61 696c 222c 2022  n.get("Email", "
+00011eb0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00011ec0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00011ed0: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
+00011ee0: 2073 6176 655f 7365 7474 696e 6773 2873   save_settings(s
+00011ef0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00011f00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011f10: 2020 5361 7665 2073 6574 7469 6e67 7320    Save settings 
+00011f20: 746f 2064 6174 6162 6173 652e 0a0a 2020  to database...  
+00011f30: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00011f40: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00011f50: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00011f60: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00011f70: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00011f80: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+00011f90: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00011fa0: 2020 2020 6373 203d 2073 656c 662e 7365      cs = self.se
+00011fb0: 7474 696e 6773 5f64 6961 6c6f 672e 4361  ttings_dialog.Ca
+00011fc0: 6c6c 2e74 6578 7428 290a 2020 2020 2020  ll.text().      
+00011fd0: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+00011fe0: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
+00011ff0: 2e73 7461 7469 6f6e 5b22 4361 6c6c 225d  .station["Call"]
+00012000: 203d 2063 732e 7570 7065 7228 290a 2020   = cs.upper().  
+00012010: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+00012020: 6f6e 5b22 4e61 6d65 225d 203d 2073 656c  on["Name"] = sel
+00012030: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+00012040: 672e 4e61 6d65 2e74 6578 7428 292e 7469  g.Name.text().ti
+00012050: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
+00012060: 6c66 2e73 7461 7469 6f6e 5b22 5374 7265  lf.station["Stre
+00012070: 6574 3122 5d20 3d20 7365 6c66 2e73 6574  et1"] = self.set
+00012080: 7469 6e67 735f 6469 616c 6f67 2e41 6464  tings_dialog.Add
+00012090: 7265 7373 312e 7465 7874 2829 2e74 6974  ress1.text().tit
+000120a0: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
+000120b0: 662e 7374 6174 696f 6e5b 2253 7472 6565  f.station["Stree
+000120c0: 7432 225d 203d 2073 656c 662e 7365 7474  t2"] = self.sett
+000120d0: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
+000120e0: 6573 7332 2e74 6578 7428 292e 7469 746c  ess2.text().titl
+000120f0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00012100: 2e73 7461 7469 6f6e 5b22 4369 7479 225d  .station["City"]
+00012110: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+00012120: 5f64 6961 6c6f 672e 4369 7479 2e74 6578  _dialog.City.tex
+00012130: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+00012140: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+00012150: 5b22 5374 6174 6522 5d20 3d20 7365 6c66  ["State"] = self
+00012160: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00012170: 2e53 7461 7465 2e74 6578 7428 292e 7570  .State.text().up
+00012180: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
+00012190: 6c66 2e73 7461 7469 6f6e 5b22 5a69 7022  lf.station["Zip"
+000121a0: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+000121b0: 735f 6469 616c 6f67 2e5a 6970 2e74 6578  s_dialog.Zip.tex
+000121c0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+000121d0: 2e73 7461 7469 6f6e 5b22 436f 756e 7472  .station["Countr
+000121e0: 7922 5d20 3d20 7365 6c66 2e73 6574 7469  y"] = self.setti
+000121f0: 6e67 735f 6469 616c 6f67 2e43 6f75 6e74  ngs_dialog.Count
+00012200: 7279 2e74 6578 7428 292e 7469 746c 6528  ry.text().title(
+00012210: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00012220: 7461 7469 6f6e 5b22 4772 6964 5371 7561  tation["GridSqua
+00012230: 7265 225d 203d 2073 656c 662e 7365 7474  re"] = self.sett
+00012240: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
+00012250: 5371 7561 7265 2e74 6578 7428 290a 2020  Square.text().  
+00012260: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+00012270: 6f6e 5b22 4351 5a6f 6e65 225d 203d 2073  on["CQZone"] = s
+00012280: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+00012290: 6c6f 672e 4351 5a6f 6e65 2e74 6578 7428  log.CQZone.text(
+000122a0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000122b0: 7461 7469 6f6e 5b22 4941 5255 5a6f 6e65  tation["IARUZone
+000122c0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+000122d0: 6773 5f64 6961 6c6f 672e 4954 555a 6f6e  gs_dialog.ITUZon
+000122e0: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
+000122f0: 2073 656c 662e 7374 6174 696f 6e5b 224c   self.station["L
+00012300: 6963 656e 7365 436c 6173 7322 5d20 3d20  icenseClass"] = 
+00012310: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+00012320: 616c 6f67 2e4c 6963 656e 7365 2e74 6578  alog.License.tex
+00012330: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+00012340: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+00012350: 5b22 4c61 7469 7475 6465 225d 203d 2073  ["Latitude"] = s
+00012360: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+00012370: 6c6f 672e 4c61 7469 7475 6465 2e74 6578  log.Latitude.tex
+00012380: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00012390: 2e73 7461 7469 6f6e 5b22 4c6f 6e67 6974  .station["Longit
+000123a0: 7564 6522 5d20 3d20 7365 6c66 2e73 6574  ude"] = self.set
+000123b0: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
+000123c0: 6769 7475 6465 2e74 6578 7428 290a 2020  gitude.text().  
+000123d0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+000123e0: 6f6e 5b22 5354 5865 7122 5d20 3d20 7365  on["STXeq"] = se
+000123f0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+00012400: 6f67 2e53 7461 7469 6f6e 5458 5258 2e74  og.StationTXRX.t
+00012410: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+00012420: 6c66 2e73 7461 7469 6f6e 5b22 5350 6f77  lf.station["SPow
+00012430: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
+00012440: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
+00012450: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00012460: 7365 6c66 2e73 7461 7469 6f6e 5b22 5341  self.station["SA
+00012470: 6e74 6522 5d20 3d20 7365 6c66 2e73 6574  nte"] = self.set
+00012480: 7469 6e67 735f 6469 616c 6f67 2e41 6e74  tings_dialog.Ant
+00012490: 656e 6e61 2e74 6578 7428 290a 2020 2020  enna.text().    
+000124a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+000124b0: 5b22 5341 6e74 4831 225d 203d 2073 656c  ["SAntH1"] = sel
+000124c0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+000124d0: 672e 416e 7448 6569 6768 742e 7465 7874  g.AntHeight.text
+000124e0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000124f0: 7374 6174 696f 6e5b 2253 416e 7448 3222  station["SAntH2"
+00012500: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+00012510: 735f 6469 616c 6f67 2e41 534c 2e74 6578  s_dialog.ASL.tex
+00012520: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00012530: 2e73 7461 7469 6f6e 5b22 4152 524c 5365  .station["ARRLSe
+00012540: 6374 696f 6e22 5d20 3d20 7365 6c66 2e73  ction"] = self.s
+00012550: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+00012560: 5252 4c53 6563 7469 6f6e 2e74 6578 7428  RRLSection.text(
+00012570: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
+00012580: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+00012590: 526f 7665 7251 5448 225d 203d 2073 656c  RoverQTH"] = sel
+000125a0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+000125b0: 672e 526f 7665 7251 5448 2e74 6578 7428  g.RoverQTH.text(
+000125c0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000125d0: 7461 7469 6f6e 5b22 436c 7562 225d 203d  tation["Club"] =
+000125e0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+000125f0: 6961 6c6f 672e 436c 7562 2e74 6578 7428  ialog.Club.text(
+00012600: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+00012610: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+00012620: 456d 6169 6c22 5d20 3d20 7365 6c66 2e73  Email"] = self.s
+00012630: 6574 7469 6e67 735f 6469 616c 6f67 2e45  ettings_dialog.E
+00012640: 6d61 696c 2e74 6578 7428 290a 2020 2020  mail.text().    
+00012650: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+00012660: 652e 6164 645f 7374 6174 696f 6e28 7365  e.add_station(se
+00012670: 6c66 2e73 7461 7469 6f6e 290a 2020 2020  lf.station).    
+00012680: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+00012690: 735f 6469 616c 6f67 2e63 6c6f 7365 2829  s_dialog.close()
+000126a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000126b0: 2e63 7572 7265 6e74 5f6f 7020 3d3d 2022  .current_op == "
+000126c0: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+000126d0: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
+000126e0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+000126f0: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
+00012700: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00012710: 616b 655f 6f70 5f64 6972 2829 0a20 2020  ake_op_dir().   
+00012720: 2020 2020 2063 6f6e 7465 7374 5f63 6f75       contest_cou
+00012730: 6e74 203d 2073 656c 662e 6461 7461 6261  nt = self.databa
+00012740: 7365 2e66 6574 6368 5f61 6c6c 5f63 6f6e  se.fetch_all_con
+00012750: 7465 7374 7328 290a 2020 2020 2020 2020  tests().        
+00012760: 6966 206c 656e 2863 6f6e 7465 7374 5f63  if len(contest_c
+00012770: 6f75 6e74 2920 3d3d 2030 3a0a 2020 2020  ount) == 0:.    
+00012780: 2020 2020 2020 2020 7365 6c66 2e6e 6577          self.new
+00012790: 5f63 6f6e 7465 7374 5f64 6961 6c6f 6728  _contest_dialog(
+000127a0: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+000127b0: 6d61 6372 6f28 7365 6c66 2c20 6675 6e63  macro(self, func
+000127c0: 7469 6f6e 5f6b 6579 2920 2d3e 204e 6f6e  tion_key) -> Non
+000127d0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000127e0: 2020 2020 2020 2053 686f 7720 6564 6974         Show edit
+000127f0: 206d 6163 726f 2064 6961 6c6f 6720 666f   macro dialog fo
+00012800: 7220 6675 6e63 7469 6f6e 206b 6579 2e0a  r function key..
+00012810: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00012820: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00012830: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
+00012840: 756e 6374 696f 6e5f 6b65 7920 3a20 7374  unction_key : st
+00012850: 720a 2020 2020 2020 2020 4675 6e63 7469  r.        Functi
+00012860: 6f6e 206b 6579 2074 6f20 6564 6974 2e0a  on key to edit..
+00012870: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00012880: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00012890: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+000128a0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000128b0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+000128c0: 726f 5f64 6961 6c6f 6720 3d20 4564 6974  ro_dialog = Edit
+000128d0: 4d61 6372 6f28 6675 6e63 7469 6f6e 5f6b  Macro(function_k
+000128e0: 6579 2c20 6673 7574 696c 732e 4150 505f  ey, fsutils.APP_
+000128f0: 4441 5441 5f50 4154 4829 0a0a 2020 2020  DATA_PATH)..    
+00012900: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
+00012910: 656e 745f 7061 6c65 7474 653a 0a20 2020  ent_palette:.   
+00012920: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+00012930: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
+00012940: 7365 7450 616c 6574 7465 2873 656c 662e  setPalette(self.
+00012950: 6375 7272 656e 745f 7061 6c65 7474 6529  current_palette)
+00012960: 0a0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00012970: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+00012980: 2e61 6363 6570 7465 642e 636f 6e6e 6563  .accepted.connec
+00012990: 7428 7365 6c66 2e65 6469 7465 645f 6d61  t(self.edited_ma
+000129a0: 6372 6f29 0a20 2020 2020 2020 2073 656c  cro).        sel
+000129b0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
+000129c0: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
+000129d0: 6465 6620 6564 6974 6564 5f6d 6163 726f  def edited_macro
+000129e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+000129f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012a00: 2020 2020 5361 7665 2065 6469 7465 6420      Save edited 
+00012a10: 6d61 6372 6f20 746f 2064 6174 6162 6173  macro to databas
+00012a20: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
+00012a30: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00012a40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00012a50: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
+00012a60: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00012a70: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00012a80: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+00012a90: 0a0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00012aa0: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+00012ab0: 2e66 756e 6374 696f 6e5f 6b65 792e 7365  .function_key.se
+00012ac0: 7454 6578 7428 0a20 2020 2020 2020 2020  tText(.         
+00012ad0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+00012ae0: 726f 5f64 6961 6c6f 672e 6d61 6372 6f5f  ro_dialog.macro_
+00012af0: 6c61 6265 6c2e 7465 7874 2829 0a20 2020  label.text().   
+00012b00: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00012b10: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
+00012b20: 6961 6c6f 672e 6675 6e63 7469 6f6e 5f6b  ialog.function_k
+00012b30: 6579 2e73 6574 546f 6f6c 5469 7028 0a20  ey.setToolTip(. 
+00012b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012b50: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
+00012b60: 672e 7468 655f 6d61 6372 6f2e 7465 7874  g.the_macro.text
+00012b70: 2829 0a20 2020 2020 2020 2029 0a20 2020  ().        ).   
+00012b80: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+00012b90: 6163 726f 5f64 6961 6c6f 672e 636c 6f73  acro_dialog.clos
+00012ba0: 6528 290a 0a20 2020 2064 6566 2070 726f  e()..    def pro
+00012bb0: 6365 7373 5f6d 6163 726f 2873 656c 662c  cess_macro(self,
+00012bc0: 206d 6163 726f 3a20 7374 7229 202d 3e20   macro: str) -> 
+00012bd0: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
+00012be0: 0a20 2020 2020 2020 2050 726f 6365 7373  .        Process
+00012bf0: 2043 5720 6d61 6372 6f20 7375 6273 7469   CW macro substi
+00012c00: 7475 7469 6f6e 7320 666f 7220 636f 6e74  tutions for cont
+00012c10: 6573 742e 0a0a 2020 2020 2020 2020 5061  est...        Pa
+00012c20: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00012c30: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00012c40: 2020 2020 6d61 6372 6f20 3a20 7374 720a      macro : str.
+00012c50: 2020 2020 2020 2020 4d61 6372 6f20 746f          Macro to
+00012c60: 2070 726f 6365 7373 2e0a 0a20 2020 2020   process...     
+00012c70: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00012c80: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00012c90: 2020 2073 7472 0a20 2020 2020 2020 2050     str.        P
+00012ca0: 726f 6365 7373 6564 206d 6163 726f 2e0a  rocessed macro..
+00012cb0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00012cc0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00012cd0: 6c66 2e64 6174 6162 6173 652e 6765 745f  lf.database.get_
+00012ce0: 7365 7269 616c 2829 0a20 2020 2020 2020  serial().       
+00012cf0: 206e 6578 745f 7365 7269 616c 203d 2073   next_serial = s
+00012d00: 7472 2872 6573 756c 742e 6765 7428 2273  tr(result.get("s
+00012d10: 6572 6961 6c5f 6e72 222c 2022 3122 2929  erial_nr", "1"))
+00012d20: 0a20 2020 2020 2020 2069 6620 6e65 7874  .        if next
+00012d30: 5f73 6572 6961 6c20 3d3d 2022 4e6f 6e65  _serial == "None
+00012d40: 223a 0a20 2020 2020 2020 2020 2020 206e  ":.            n
+00012d50: 6578 745f 7365 7269 616c 203d 2022 3122  ext_serial = "1"
+00012d60: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
+00012d70: 206d 6163 726f 2e75 7070 6572 2829 0a20   macro.upper(). 
+00012d80: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
+00012d90: 6163 726f 2e72 6570 6c61 6365 2822 2322  acro.replace("#"
+00012da0: 2c20 6e65 7874 5f73 6572 6961 6c29 0a20  , next_serial). 
+00012db0: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
+00012dc0: 6163 726f 2e72 6570 6c61 6365 2822 7b4d  acro.replace("{M
+00012dd0: 5943 414c 4c7d 222c 2073 656c 662e 7374  YCALL}", self.st
+00012de0: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
+00012df0: 2c20 2222 2929 0a20 2020 2020 2020 206d  , "")).        m
+00012e00: 6163 726f 203d 206d 6163 726f 2e72 6570  acro = macro.rep
+00012e10: 6c61 6365 2822 7b48 4953 4341 4c4c 7d22  lace("{HISCALL}"
+00012e20: 2c20 7365 6c66 2e63 616c 6c73 6967 6e2e  , self.callsign.
+00012e30: 7465 7874 2829 290a 2020 2020 2020 2020  text()).        
+00012e40: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+00012e50: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
+00012e60: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
+00012e70: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
+00012e80: 726f 2e72 6570 6c61 6365 2822 7b53 4e54  ro.replace("{SNT
+00012e90: 7d22 2c20 7365 6c66 2e73 656e 742e 7465  }", self.sent.te
+00012ea0: 7874 2829 2e72 6570 6c61 6365 2822 3922  xt().replace("9"
+00012eb0: 2c20 226e 2229 290a 2020 2020 2020 2020  , "n")).        
+00012ec0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00012ed0: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
+00012ee0: 7265 706c 6163 6528 227b 534e 547d 222c  replace("{SNT}",
+00012ef0: 2073 656c 662e 7365 6e74 2e74 6578 7428   self.sent.text(
+00012f00: 2929 0a20 2020 2020 2020 206d 6163 726f  )).        macro
+00012f10: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
+00012f20: 2822 7b53 454e 544e 527d 222c 2073 656c  ("{SENTNR}", sel
+00012f30: 662e 6f74 6865 725f 312e 7465 7874 2829  f.other_1.text()
+00012f40: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
+00012f50: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
+00012f60: 0a20 2020 2020 2020 2020 2020 2022 7b45  .            "{E
+00012f70: 5843 487d 222c 2073 656c 662e 636f 6e74  XCH}", self.cont
+00012f80: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00012f90: 2822 5365 6e74 4578 6368 616e 6765 222c  ("SentExchange",
+00012fa0: 2022 7878 7822 290a 2020 2020 2020 2020   "xxx").        
+00012fb0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012fc0: 206d 6163 726f 0a0a 2020 2020 6465 6620   macro..    def 
+00012fd0: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
+00012fe0: 662c 2074 6865 5f73 7472 696e 673a 2073  f, the_string: s
+00012ff0: 7472 2920 2d3e 204e 6f6e 653a 0a20 2020  tr) -> None:.   
+00013000: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013010: 2076 6f69 6365 7320 7374 7269 6e67 2075   voices string u
+00013020: 7369 6e67 206e 6174 6f20 7068 6f6e 6574  sing nato phonet
+00013030: 6963 732e 0a0a 2020 2020 2020 2020 5061  ics...        Pa
+00013040: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00013050: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00013060: 2020 2020 7468 655f 7374 7269 6e67 203a      the_string :
+00013070: 2073 7472 0a20 2020 2020 2020 2053 7472   str.        Str
+00013080: 696e 6720 746f 2076 6f69 6369 6679 2e0a  ing to voicify..
+00013090: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000130a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000130b0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+000130c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000130d0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+000130e0: 2256 6f69 6369 6e67 3a20 2573 222c 2074  "Voicing: %s", t
+000130f0: 6865 5f73 7472 696e 6729 0a20 2020 2020  he_string).     
+00013100: 2020 206f 705f 7061 7468 203d 2066 7375     op_path = fsu
+00013110: 7469 6c73 2e55 5345 525f 4441 5441 5f50  tils.USER_DATA_P
+00013120: 4154 4820 2f20 7365 6c66 2e63 7572 7265  ATH / self.curre
+00013130: 6e74 5f6f 700a 2020 2020 2020 2020 6966  nt_op.        if
+00013140: 2022 5b22 2069 6e20 7468 655f 7374 7269   "[" in the_stri
+00013150: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00013160: 7375 625f 7374 7269 6e67 203d 2074 6865  sub_string = the
+00013170: 5f73 7472 696e 672e 7374 7269 7028 225b  _string.strip("[
+00013180: 5d22 292e 6c6f 7765 7228 290a 2020 2020  ]").lower().    
+00013190: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+000131a0: 203d 2066 227b 7374 7228 6f70 5f70 6174   = f"{str(op_pat
+000131b0: 6829 7d2f 7b73 7562 5f73 7472 696e 677d  h)}/{sub_string}
+000131c0: 2e77 6176 220a 2020 2020 2020 2020 2020  .wav".          
+000131d0: 2020 6966 2050 6174 6828 6669 6c65 6e61    if Path(filena
+000131e0: 6d65 292e 6973 5f66 696c 6528 293a 0a20  me).is_file():. 
+000131f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00013200: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
+00013210: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
+00013220: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00013230: 2020 2020 2064 6174 612c 205f 6673 203d       data, _fs =
+00013240: 2073 662e 7265 6164 2866 696c 656e 616d   sf.read(filenam
+00013250: 652c 2064 7479 7065 3d22 666c 6f61 7433  e, dtype="float3
+00013260: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
+00013270: 2020 2020 7365 6c66 2e70 7474 5f6f 6e28      self.ptt_on(
+00013280: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013290: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000132a0: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
+000132b0: 6661 756c 742e 6465 7669 6365 203d 2073  fault.device = s
+000132c0: 656c 662e 7072 6566 2e67 6574 2822 736f  elf.pref.get("so
+000132d0: 756e 6464 6576 6963 6522 2c20 2264 6566  unddevice", "def
+000132e0: 6175 6c74 2229 0a20 2020 2020 2020 2020  ault").         
+000132f0: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
+00013300: 6661 756c 742e 7361 6d70 6c65 7261 7465  fault.samplerate
+00013310: 203d 2034 3431 3030 2e30 0a20 2020 2020   = 44100.0.     
+00013320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013330: 642e 706c 6179 2864 6174 612c 2062 6c6f  d.play(data, blo
+00013340: 636b 696e 673d 4661 6c73 6529 0a20 2020  cking=False).   
+00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013360: 2023 205f 7374 6174 7573 203d 2073 642e   # _status = sd.
+00013370: 7761 6974 2829 0a20 2020 2020 2020 2020  wait().         
+00013380: 2020 2020 2020 2020 2020 2023 2068 7474             # htt
+00013390: 7073 3a2f 2f73 6e79 6b2e 696f 2f61 6476  ps://snyk.io/adv
+000133a0: 6973 6f72 2f70 7974 686f 6e2f 736f 756e  isor/python/soun
+000133b0: 6464 6576 6963 652f 6675 6e63 7469 6f6e  ddevice/function
+000133c0: 732f 736f 756e 6464 6576 6963 652e 506f  s/sounddevice.Po
+000133d0: 7274 4175 6469 6f45 7272 6f72 0a20 2020  rtAudioError.   
+000133e0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+000133f0: 6570 7420 7364 2e50 6f72 7441 7564 696f  ept sd.PortAudio
+00013400: 4572 726f 7220 6173 2065 7272 3a0a 2020  Error as err:.  
+00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013420: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
+00013430: 2822 2573 222c 2066 227b 6572 727d 2229  ("%s", f"{err}")
+00013440: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013450: 2020 7365 6c66 2e70 7474 5f6f 6666 2829    self.ptt_off()
+00013460: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013470: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
+00013480: 2e70 7474 5f6f 6e28 290a 2020 2020 2020  .ptt_on().      
+00013490: 2020 666f 7220 6c65 7474 6572 2069 6e20    for letter in 
+000134a0: 7468 655f 7374 7269 6e67 2e6c 6f77 6572  the_string.lower
+000134b0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000134c0: 6966 206c 6574 7465 7220 696e 2022 6162  if letter in "ab
+000134d0: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
+000134e0: 7374 7576 7778 797a 2031 3233 3435 3637  stuvwxyz 1234567
+000134f0: 3839 3022 3a0a 2020 2020 2020 2020 2020  890":.          
+00013500: 2020 2020 2020 6966 206c 6574 7465 7220        if letter 
+00013510: 3d3d 2022 2022 3a0a 2020 2020 2020 2020  == " ":.        
+00013520: 2020 2020 2020 2020 2020 2020 6c65 7474              lett
+00013530: 6572 203d 2022 7370 6163 6522 0a20 2020  er = "space".   
+00013540: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00013550: 656e 616d 6520 3d20 6622 7b73 7472 286f  ename = f"{str(o
+00013560: 705f 7061 7468 297d 2f7b 6c65 7474 6572  p_path)}/{letter
+00013570: 7d2e 7761 7622 0a20 2020 2020 2020 2020  }.wav".         
+00013580: 2020 2020 2020 2069 6620 5061 7468 2866         if Path(f
+00013590: 696c 656e 616d 6529 2e69 735f 6669 6c65  ilename).is_file
+000135a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000135b0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000135c0: 6562 7567 2822 566f 6963 696e 673a 2025  ebug("Voicing: %
+000135d0: 7322 2c20 6669 6c65 6e61 6d65 290a 2020  s", filename).  
+000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135f0: 2020 6461 7461 2c20 5f66 7320 3d20 7366    data, _fs = sf
+00013600: 2e72 6561 6428 6669 6c65 6e61 6d65 2c20  .read(filename, 
+00013610: 6474 7970 653d 2266 6c6f 6174 3332 2229  dtype="float32")
+00013620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013630: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00013640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013650: 2020 7364 2e64 6566 6175 6c74 2e64 6576    sd.default.dev
+00013660: 6963 6520 3d20 7365 6c66 2e70 7265 662e  ice = self.pref.
+00013670: 6765 7428 2273 6f75 6e64 6465 7669 6365  get("sounddevice
+00013680: 222c 2022 6465 6661 756c 7422 290a 2020  ", "default").  
+00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136a0: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
+000136b0: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
+000136c0: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
+000136d0: 2020 2020 2020 2020 2020 2020 2020 7364                sd
+000136e0: 2e70 6c61 7928 6461 7461 2c20 626c 6f63  .play(data, bloc
+000136f0: 6b69 6e67 3d46 616c 7365 290a 2020 2020  king=False).    
+00013700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013710: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00013720: 2822 2573 222c 2066 227b 7364 2e77 6169  ("%s", f"{sd.wai
+00013730: 7428 297d 2229 0a20 2020 2020 2020 2020  t()}").         
+00013740: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00013750: 7420 7364 2e50 6f72 7441 7564 696f 4572  t sd.PortAudioEr
+00013760: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
+00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013780: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+00013790: 6e67 2822 2573 222c 2066 227b 6572 727d  ng("%s", f"{err}
+000137a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000137b0: 7074 745f 6f66 6628 290a 0a20 2020 2064  ptt_off()..    d
+000137c0: 6566 2070 7474 5f6f 6e28 7365 6c66 2920  ef ptt_on(self) 
+000137d0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000137e0: 2022 2222 0a20 2020 2020 2020 2054 7572   """.        Tur
+000137f0: 6e20 6f6e 2070 7474 2066 6f72 2072 6967  n on ptt for rig
+00013800: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00013810: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00013820: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00013830: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
+00013840: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00013850: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00013860: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+00013870: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00013880: 6465 6275 6728 2250 5454 204f 6e22 290a  debug("PTT On").
+00013890: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000138a0: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+000138b0: 2020 2020 2020 2020 2073 656c 662e 6c65           self.le
+000138c0: 6674 646f 742e 7365 7450 6978 6d61 7028  ftdot.setPixmap(
+000138d0: 7365 6c66 2e67 7265 656e 646f 7429 0a20  self.greendot). 
+000138e0: 2020 2020 2020 2020 2020 2061 7070 2e70             app.p
+000138f0: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
+00013900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013910: 7269 675f 636f 6e74 726f 6c2e 7074 745f  rig_control.ptt_
+00013920: 6f6e 2829 0a0a 2020 2020 6465 6620 7074  on()..    def pt
+00013930: 745f 6f66 6628 7365 6c66 2920 2d3e 204e  t_off(self) -> N
+00013940: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00013950: 0a20 2020 2020 2020 2054 7572 6e20 6f66  .        Turn of
+00013960: 6620 7074 7420 666f 7220 7269 672e 0a0a  f ptt for rig...
+00013970: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00013980: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00013990: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+000139a0: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
+000139b0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+000139c0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+000139d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000139e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+000139f0: 6728 2250 5454 204f 6666 2229 0a20 2020  g("PTT Off").   
+00013a00: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
+00013a10: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
+00013a20: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
+00013a30: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
+00013a40: 662e 7265 6464 6f74 290a 2020 2020 2020  f.reddot).      
+00013a50: 2020 2020 2020 6170 702e 7072 6f63 6573        app.proces
+00013a60: 7345 7665 6e74 7328 290a 2020 2020 2020  sEvents().      
+00013a70: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
+00013a80: 6f6e 7472 6f6c 2e70 7474 5f6f 6666 2829  ontrol.ptt_off()
+00013a90: 0a0a 2020 2020 6465 6620 7072 6f63 6573  ..    def proces
+00013aa0: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
+00013ab0: 656c 662c 2066 756e 6374 696f 6e5f 6b65  elf, function_ke
+00013ac0: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
+00013ad0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013ae0: 4361 6c6c 6564 2077 6865 6e20 6120 6675  Called when a fu
+00013af0: 6e63 7469 6f6e 206b 6579 2069 7320 636c  nction key is cl
+00013b00: 6963 6b65 642e 0a0a 2020 2020 2020 2020  icked...        
+00013b10: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00013b20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00013b30: 2020 2020 2020 6675 6e63 7469 6f6e 5f6b        function_k
+00013b40: 6579 203a 2051 5075 7368 4275 7474 6f6e  ey : QPushButton
+00013b50: 0a20 2020 2020 2020 2046 756e 6374 696f  .        Functio
+00013b60: 6e20 6b65 7920 746f 2070 726f 6365 7373  n key to process
+00013b70: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00013b80: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00013b90: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00013ba0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00013bb0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00013bc0: 6728 2246 756e 6374 696f 6e20 4b65 793a  g("Function Key:
+00013bd0: 2025 7322 2c20 6675 6e63 7469 6f6e 5f6b   %s", function_k
+00013be0: 6579 2e74 6578 7428 2929 0a20 2020 2020  ey.text()).     
+00013bf0: 2020 2069 6620 7365 6c66 2e6e 316d 6d3a     if self.n1mm:
+00013c00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013c10: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+00013c20: 6f5b 2246 756e 6374 696f 6e4b 6579 4361  o["FunctionKeyCa
+00013c30: 7074 696f 6e22 5d20 3d20 6675 6e63 7469  ption"] = functi
+00013c40: 6f6e 5f6b 6579 2e74 6578 7428 290a 2020  on_key.text().  
+00013c50: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+00013c60: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+00013c70: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
+00013c80: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
+00013c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013ca0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
+00013cb0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+00013cc0: 2866 756e 6374 696f 6e5f 6b65 792e 746f  (function_key.to
+00013cd0: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
+00013ce0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00013cf0: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
+00013d00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013d10: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
+00013d20: 2e70 726f 6365 7373 5f6d 6163 726f 2866  .process_macro(f
+00013d30: 756e 6374 696f 6e5f 6b65 792e 746f 6f6c  unction_key.tool
+00013d40: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
+00013d50: 2072 756e 5f73 705f 6275 7474 6f6e 735f   run_sp_buttons_
+00013d60: 636c 6963 6b65 6428 7365 6c66 2920 2d3e  clicked(self) ->
+00013d70: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00013d80: 2222 0a20 2020 2020 2020 2048 616e 646c  "".        Handl
+00013d90: 6520 5275 6e2f 5326 5020 6d6f 6465 2063  e Run/S&P mode c
+00013da0: 6861 6e67 6573 2e0a 0a20 2020 2020 2020  hanges...       
+00013db0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00013dc0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00013dd0: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
+00013de0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00013df0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00013e00: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
+00013e10: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00013e20: 6c66 2e70 7265 665b 2272 756e 5f73 7461  lf.pref["run_sta
+00013e30: 7465 225d 203d 2073 656c 662e 7261 6469  te"] = self.radi
+00013e40: 6f42 7574 746f 6e5f 7275 6e2e 6973 4368  oButton_run.isCh
+00013e50: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
+00013e60: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+00013e70: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+00013e80: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
+00013e90: 726f 7328 290a 0a20 2020 2064 6566 2077  ros()..    def w
+00013ea0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+00013eb0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00013ec0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013ed0: 2020 2057 7269 7465 2070 7265 6665 7265     Write prefere
+00013ee0: 6e63 6573 2074 6f20 6669 6c65 2e0a 0a20  nces to file... 
+00013ef0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00013f00: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00013f10: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+00013f20: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
+00013f30: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00013f40: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00013f50: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00013f60: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00013f70: 6728 2277 7269 7465 7072 6566 6572 656e  g("writepreferen
+00013f80: 6365 7322 290a 2020 2020 2020 2020 7472  ces").        tr
+00013f90: 793a 0a20 2020 2020 2020 2020 2020 2077  y:.            w
+00013fa0: 6974 6820 6f70 656e 2866 7375 7469 6c73  ith open(fsutils
+00013fb0: 2e43 4f4e 4649 475f 4649 4c45 2c20 2277  .CONFIG_FILE, "w
+00013fc0: 7422 2c20 656e 636f 6469 6e67 3d22 7574  t", encoding="ut
+00013fd0: 662d 3822 2920 6173 2066 696c 655f 6465  f-8") as file_de
+00013fe0: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
+00013ff0: 2020 2020 2020 2020 2020 6669 6c65 5f64            file_d
+00014000: 6573 6372 6970 746f 722e 7772 6974 6528  escriptor.write(
+00014010: 6475 6d70 7328 7365 6c66 2e70 7265 662c  dumps(self.pref,
+00014020: 2069 6e64 656e 743d 3429 290a 2020 2020   indent=4)).    
+00014030: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
+00014040: 6767 6572 2e69 6e66 6f28 2277 7269 7469  gger.info("writi
+00014050: 6e67 3a20 2573 222c 2073 656c 662e 7072  ng: %s", self.pr
+00014060: 6566 290a 2020 2020 2020 2020 6578 6365  ef).        exce
+00014070: 7074 2049 4f45 7272 6f72 2061 7320 6578  pt IOError as ex
+00014080: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+00014090: 2020 2020 206c 6f67 6765 722e 6372 6974       logger.crit
+000140a0: 6963 616c 2822 7772 6974 6570 7265 6665  ical("writeprefe
+000140b0: 7265 6e63 6573 3a20 2573 222c 2065 7863  rences: %s", exc
+000140c0: 6570 7469 6f6e 290a 0a20 2020 2064 6566  eption)..    def
+000140d0: 2072 6561 6470 7265 6665 7265 6e63 6573   readpreferences
+000140e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+000140f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014100: 2020 2020 5265 7374 6f72 6520 7072 6566      Restore pref
+00014110: 6572 656e 6365 7320 6966 2074 6865 7920  erences if they 
+00014120: 6578 6973 742c 206f 7468 6572 7769 7365  exist, otherwise
+00014130: 2063 7265 6174 6520 736f 6d65 2073 616e   create some san
+00014140: 6520 6465 6661 756c 7473 2e0a 0a20 2020  e defaults...   
+00014150: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00014160: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00014170: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00014180: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00014190: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000141a0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+000141b0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000141c0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+000141d0: 2272 6561 6470 7265 6665 7265 6e63 6573  "readpreferences
+000141e0: 2229 0a20 2020 2020 2020 2074 7279 3a0a  ").        try:.
+000141f0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00014200: 732e 7061 7468 2e65 7869 7374 7328 6673  s.path.exists(fs
+00014210: 7574 696c 732e 434f 4e46 4947 5f46 494c  utils.CONFIG_FIL
+00014220: 4529 3a0a 2020 2020 2020 2020 2020 2020  E):.            
+00014230: 2020 2020 7769 7468 206f 7065 6e28 0a20      with open(. 
+00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014250: 2020 2066 7375 7469 6c73 2e43 4f4e 4649     fsutils.CONFI
+00014260: 475f 4649 4c45 2c20 2272 7422 2c20 656e  G_FILE, "rt", en
+00014270: 636f 6469 6e67 3d22 7574 662d 3822 0a20  coding="utf-8". 
+00014280: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00014290: 2061 7320 6669 6c65 5f64 6573 6372 6970   as file_descrip
+000142a0: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+000142b0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000142c0: 6566 203d 206c 6f61 6473 2866 696c 655f  ef = loads(file_
+000142d0: 6465 7363 7269 7074 6f72 2e72 6561 6428  descriptor.read(
+000142e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000142f0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00014300: 666f 2822 2573 222c 2073 656c 662e 7072  fo("%s", self.pr
+00014310: 6566 290a 2020 2020 2020 2020 2020 2020  ef).            
+00014320: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014330: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00014340: 6f28 224e 6f20 7072 6566 6572 656e 6365  o("No preference
+00014350: 2066 696c 652e 2057 7269 7469 6e67 2070   file. Writing p
+00014360: 7265 6665 7265 6e63 652e 2229 0a20 2020  reference.").   
+00014370: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00014380: 6820 6f70 656e 280a 2020 2020 2020 2020  h open(.        
+00014390: 2020 2020 2020 2020 2020 2020 6673 7574              fsut
+000143a0: 696c 732e 434f 4e46 4947 5f46 494c 452c  ils.CONFIG_FILE,
+000143b0: 2022 7774 222c 2065 6e63 6f64 696e 673d   "wt", encoding=
+000143c0: 2275 7466 2d38 220a 2020 2020 2020 2020  "utf-8".        
+000143d0: 2020 2020 2020 2020 2920 6173 2066 696c          ) as fil
+000143e0: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
+000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014400: 2020 7365 6c66 2e70 7265 6620 3d20 7365    self.pref = se
+00014410: 6c66 2e70 7265 665f 7265 662e 636f 7079  lf.pref_ref.copy
+00014420: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00014430: 2020 2020 2020 2066 696c 655f 6465 7363         file_desc
+00014440: 7269 7074 6f72 2e77 7269 7465 2864 756d  riptor.write(dum
+00014450: 7073 2873 656c 662e 7072 6566 2c20 696e  ps(self.pref, in
+00014460: 6465 6e74 3d34 2929 0a20 2020 2020 2020  dent=4)).       
+00014470: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00014480: 6765 722e 696e 666f 2822 2573 222c 2073  ger.info("%s", s
+00014490: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
+000144a0: 2020 6578 6365 7074 2049 4f45 7272 6f72    except IOError
+000144b0: 2061 7320 6578 6365 7074 696f 6e3a 0a20   as exception:. 
+000144c0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000144d0: 722e 6372 6974 6963 616c 2822 4572 726f  r.critical("Erro
+000144e0: 723a 2025 7322 2c20 6578 6365 7074 696f  r: %s", exceptio
+000144f0: 6e29 0a0a 2020 2020 2020 2020 7365 6c66  n)..        self
+00014500: 2e6c 6f6f 6b5f 7570 203d 204e 6f6e 650a  .look_up = None.
+00014510: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00014520: 7072 6566 2e67 6574 2822 7573 6571 727a  pref.get("useqrz
+00014530: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00014540: 7365 6c66 2e6c 6f6f 6b5f 7570 203d 2051  self.look_up = Q
+00014550: 525a 6c6f 6f6b 7570 280a 2020 2020 2020  RZlookup(.      
+00014560: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00014570: 7265 662e 6765 7428 226c 6f6f 6b75 7075  ref.get("lookupu
+00014580: 7365 726e 616d 6522 292c 0a20 2020 2020  sername"),.     
+00014590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000145a0: 7072 6566 2e67 6574 2822 6c6f 6f6b 7570  pref.get("lookup
+000145b0: 7061 7373 776f 7264 2229 2c0a 2020 2020  password"),.    
+000145c0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000145d0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+000145e0: 6765 7428 2275 7365 6861 6d71 7468 2229  get("usehamqth")
+000145f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00014600: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
+00014610: 5154 4828 0a20 2020 2020 2020 2020 2020  QTH(.           
+00014620: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+00014630: 6574 2822 6c6f 6f6b 7570 7573 6572 6e61  et("lookupuserna
+00014640: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
+00014650: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+00014660: 6765 7428 226c 6f6f 6b75 7070 6173 7377  get("lookuppassw
+00014670: 6f72 6422 292c 0a20 2020 2020 2020 2020  ord"),.         
+00014680: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+00014690: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000146a0: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
+000146b0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+000146c0: 6469 6f42 7574 746f 6e5f 7275 6e2e 7365  dioButton_run.se
+000146d0: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
+000146e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000146f0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00014700: 6469 6f42 7574 746f 6e5f 7370 2e73 6574  dioButton_sp.set
+00014710: 4368 6563 6b65 6428 5472 7565 290a 0a20  Checked(True).. 
+00014720: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00014730: 7265 662e 6765 7428 2263 6f6d 6d61 6e64  ref.get("command
+00014740: 5f62 7574 746f 6e73 2229 3a0a 2020 2020  _buttons"):.    
+00014750: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00014760: 696f 6e43 6f6d 6d61 6e64 5f42 7574 746f  ionCommand_Butto
+00014770: 6e73 2e73 6574 4368 6563 6b65 6428 5472  ns.setChecked(Tr
+00014780: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
+00014790: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000147a0: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
+000147b0: 5f42 7574 746f 6e73 2e73 6574 4368 6563  _Buttons.setChec
+000147c0: 6b65 6428 4661 6c73 6529 0a0a 2020 2020  ked(False)..    
+000147d0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+000147e0: 2e67 6574 2822 6377 5f6d 6163 726f 7322  .get("cw_macros"
+000147f0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00014800: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
+00014810: 726f 732e 7365 7443 6865 636b 6564 2854  ros.setChecked(T
+00014820: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
+00014830: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00014840: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
+00014850: 726f 732e 7365 7443 6865 636b 6564 2846  ros.setChecked(F
+00014860: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
+00014870: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00014880: 2262 616e 6473 5f6d 6f64 6573 2229 3a0a  "bands_modes"):.
+00014890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000148a0: 2e61 6374 696f 6e4d 6f64 655f 616e 645f  .actionMode_and_
+000148b0: 4261 6e64 732e 7365 7443 6865 636b 6564  Bands.setChecked
+000148c0: 2854 7275 6529 0a20 2020 2020 2020 2065  (True).        e
+000148d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000148e0: 2073 656c 662e 6163 7469 6f6e 4d6f 6465   self.actionMode
+000148f0: 5f61 6e64 5f42 616e 6473 2e73 6574 4368  _and_Bands.setCh
+00014900: 6563 6b65 6428 4661 6c73 6529 0a0a 2020  ecked(False)..  
+00014910: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00014920: 6361 7374 5f69 6e74 6572 6661 6365 203d  cast_interface =
+00014930: 204d 756c 7469 6361 7374 280a 2020 2020   Multicast(.    
+00014940: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00014950: 662e 6765 7428 226d 756c 7469 6361 7374  f.get("multicast
+00014960: 5f67 726f 7570 222c 2022 3233 392e 312e  _group", "239.1.
+00014970: 312e 3122 292c 0a20 2020 2020 2020 2020  1.1"),.         
+00014980: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+00014990: 2822 6d75 6c74 6963 6173 745f 706f 7274  ("multicast_port
+000149a0: 222c 2032 3233 3929 2c0a 2020 2020 2020  ", 2239),.      
+000149b0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+000149c0: 6765 7428 2269 6e74 6572 6661 6365 5f69  get("interface_i
+000149d0: 7022 2c20 2230 2e30 2e30 2e30 2229 2c0a  p", "0.0.0.0"),.
+000149e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000149f0: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00014a00: 5f69 6e74 6572 6661 6365 2e72 6561 6479  _interface.ready
+00014a10: 5f72 6561 645f 636f 6e6e 6563 7428 7365  _read_connect(se
+00014a20: 6c66 2e77 6174 6368 5f75 6470 290a 0a20  lf.watch_udp).. 
+00014a30: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00014a40: 7265 662e 6765 7428 2264 6172 6b6d 6f64  ref.get("darkmod
+00014a50: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+00014a60: 2073 656c 662e 6163 7469 6f6e 4461 726b   self.actionDark
+00014a70: 5f4d 6f64 655f 322e 7365 7443 6865 636b  _Mode_2.setCheck
+00014a80: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
+00014a90: 2020 2020 2073 656c 662e 7365 7444 6172       self.setDar
+00014aa0: 6b4d 6f64 6528 5472 7565 290a 2020 2020  kMode(True).    
+00014ab0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014ac0: 2020 2020 2020 7365 6c66 2e73 6574 4461        self.setDa
+00014ad0: 726b 4d6f 6465 2846 616c 7365 290a 2020  rkMode(False).  
+00014ae0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00014af0: 6374 696f 6e44 6172 6b5f 4d6f 6465 5f32  ctionDark_Mode_2
+00014b00: 2e73 6574 4368 6563 6b65 6428 4661 6c73  .setChecked(Fals
+00014b10: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00014b20: 2e72 6967 5f63 6f6e 7472 6f6c 203d 204e  .rig_control = N
+00014b30: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
+00014b40: 7365 6c66 2e70 7265 662e 6765 7428 2275  self.pref.get("u
+00014b50: 7365 666c 7269 6722 2c20 4661 6c73 6529  seflrig", False)
+00014b60: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00014b70: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+00014b80: 2020 2020 2020 2020 2020 2020 2255 7369              "Usi
+00014b90: 6e67 2066 6c72 6967 3a20 2573 222c 0a20  ng flrig: %s",. 
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014bb0: 227b 7365 6c66 2e70 7265 662e 6765 7428  "{self.pref.get(
+00014bc0: 2743 4154 5f69 7027 297d 207b 7365 6c66  'CAT_ip')} {self
+00014bd0: 2e70 7265 662e 6765 7428 2743 4154 5f70  .pref.get('CAT_p
+00014be0: 6f72 7427 297d 222c 0a20 2020 2020 2020  ort')}",.       
+00014bf0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014c00: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+00014c10: 726f 6c20 3d20 4341 5428 0a20 2020 2020  rol = CAT(.     
+00014c20: 2020 2020 2020 2020 2020 2022 666c 7269             "flri
+00014c30: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
+00014c40: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+00014c50: 7428 2243 4154 5f69 7022 2c20 2231 3237  t("CAT_ip", "127
+00014c60: 2e30 2e30 2e31 2229 2c0a 2020 2020 2020  .0.0.1"),.      
+00014c70: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
+00014c80: 6c66 2e70 7265 662e 6765 7428 2243 4154  lf.pref.get("CAT
+00014c90: 5f70 6f72 7422 2c20 3132 3334 3529 292c  _port", 12345)),
+00014ca0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00014cb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00014cc0: 7072 6566 2e67 6574 2822 7573 6572 6967  pref.get("userig
+00014cd0: 6374 6c64 222c 2046 616c 7365 293a 0a20  ctld", False):. 
+00014ce0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00014cf0: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
+00014d00: 2020 2020 2020 2020 2022 5573 696e 6720           "Using 
+00014d10: 7269 6763 746c 643a 2025 7322 2c0a 2020  rigctld: %s",.  
+00014d20: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00014d30: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
+00014d40: 4341 545f 6970 2729 7d20 7b73 656c 662e  CAT_ip')} {self.
+00014d50: 7072 6566 2e67 6574 2827 4341 545f 706f  pref.get('CAT_po
+00014d60: 7274 2729 7d22 2c0a 2020 2020 2020 2020  rt')}",.        
+00014d70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00014d80: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
+00014d90: 6f6c 203d 2043 4154 280a 2020 2020 2020  ol = CAT(.      
+00014da0: 2020 2020 2020 2020 2020 2272 6967 6374            "rigct
+00014db0: 6c64 222c 0a20 2020 2020 2020 2020 2020  ld",.           
+00014dc0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+00014dd0: 6574 2822 4341 545f 6970 222c 2022 3132  et("CAT_ip", "12
+00014de0: 372e 302e 302e 3122 292c 0a20 2020 2020  7.0.0.1"),.     
+00014df0: 2020 2020 2020 2020 2020 2069 6e74 2873             int(s
+00014e00: 656c 662e 7072 6566 2e67 6574 2822 4341  elf.pref.get("CA
+00014e10: 545f 706f 7274 222c 2034 3533 3229 292c  T_port", 4532)),
+00014e20: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00014e30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00014e40: 7072 6566 2e67 6574 2822 6377 7479 7065  pref.get("cwtype
+00014e50: 222c 2030 2920 3d3d 2030 3a0a 2020 2020  ", 0) == 0:.    
+00014e60: 2020 2020 2020 2020 7365 6c66 2e63 7720          self.cw 
+00014e70: 3d20 4e6f 6e65 0a20 2020 2020 2020 2065  = None.        e
+00014e80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014e90: 2073 656c 662e 6377 203d 2043 5728 0a20   self.cw = CW(. 
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014eb0: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
+00014ec0: 2822 6377 7479 7065 2229 292c 0a20 2020  ("cwtype")),.   
+00014ed0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014ee0: 662e 7072 6566 2e67 6574 2822 6377 6970  f.pref.get("cwip
+00014ef0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00014f00: 2020 2020 696e 7428 7365 6c66 2e70 7265      int(self.pre
+00014f10: 662e 6765 7428 2263 7770 6f72 7422 2c20  f.get("cwport", 
+00014f20: 3637 3839 2929 2c0a 2020 2020 2020 2020  6789)),.        
+00014f30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00014f40: 2020 7365 6c66 2e63 772e 7370 6565 6420    self.cw.speed 
+00014f50: 3d20 3230 0a20 2020 2020 2020 2020 2020  = 20.           
+00014f60: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
+00014f70: 6572 7479 7065 203d 3d20 323a 0a20 2020  ertype == 2:.   
+00014f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014f90: 662e 6377 2e73 6574 5f77 696e 6b65 7965  f.cw.set_winkeye
+00014fa0: 725f 7370 6565 6428 3230 290a 0a20 2020  r_speed(20)..   
+00014fb0: 2020 2020 2073 656c 662e 6e31 6d6d 203d       self.n1mm =
+00014fc0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00014fd0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+00014fe0: 7365 6e64 5f6e 316d 6d5f 7061 636b 6574  send_n1mm_packet
+00014ff0: 7322 2c20 4661 6c73 6529 3a0a 2020 2020  s", False):.    
+00015000: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00015010: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015020: 662e 6e31 6d6d 203d 204e 314d 4d28 0a20  f.n1mm = N1MM(. 
+00015030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015040: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+00015050: 2822 6e31 6d6d 5f72 6164 696f 706f 7274  ("n1mm_radioport
+00015060: 222c 2022 3132 372e 302e 302e 313a 3132  ", "127.0.0.1:12
+00015070: 3036 3022 292c 0a20 2020 2020 2020 2020  060"),.         
+00015080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015090: 7072 6566 2e67 6574 2822 6e31 6d6d 5f63  pref.get("n1mm_c
+000150a0: 6f6e 7461 6374 706f 7274 222c 2022 3132  ontactport", "12
+000150b0: 372e 302e 302e 313a 3132 3036 3122 292c  7.0.0.1:12061"),
+000150c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150d0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+000150e0: 6574 2822 6e31 6d6d 5f6c 6f6f 6b75 7070  et("n1mm_lookupp
+000150f0: 6f72 7422 2c20 2231 3237 2e30 2e30 2e31  ort", "127.0.0.1
+00015100: 3a31 3230 3630 2229 2c0a 2020 2020 2020  :12060"),.      
+00015110: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015120: 6c66 2e70 7265 662e 6765 7428 226e 316d  lf.pref.get("n1m
+00015130: 6d5f 7363 6f72 6570 6f72 7422 2c20 2231  m_scoreport", "1
+00015140: 3237 2e30 2e30 2e31 3a31 3230 3630 2229  27.0.0.1:12060")
+00015150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015160: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00015170: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00015180: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00015190: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+000151a0: 6728 2225 7322 2c20 6622 7b56 616c 7565  g("%s", f"{Value
+000151b0: 4572 726f 727d 2229 0a20 2020 2020 2020  Error}").       
+000151c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e73       self.n1mm.s
+000151d0: 656e 645f 7261 6469 6f5f 7061 636b 6574  end_radio_packet
+000151e0: 7320 3d20 7365 6c66 2e70 7265 662e 6765  s = self.pref.ge
+000151f0: 7428 2273 656e 645f 6e31 6d6d 5f72 6164  t("send_n1mm_rad
+00015200: 696f 222c 2046 616c 7365 290a 2020 2020  io", False).    
+00015210: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+00015220: 6d2e 7365 6e64 5f63 6f6e 7461 6374 5f70  m.send_contact_p
+00015230: 6163 6b65 7473 203d 2073 656c 662e 7072  ackets = self.pr
+00015240: 6566 2e67 6574 2822 7365 6e64 5f6e 316d  ef.get("send_n1m
+00015250: 6d5f 636f 6e74 6163 7422 2c20 4661 6c73  m_contact", Fals
+00015260: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00015270: 656c 662e 6e31 6d6d 2e73 656e 645f 6c6f  elf.n1mm.send_lo
+00015280: 6f6b 7570 5f70 6163 6b65 7473 203d 2073  okup_packets = s
+00015290: 656c 662e 7072 6566 2e67 6574 2822 7365  elf.pref.get("se
+000152a0: 6e64 5f6e 316d 6d5f 6c6f 6f6b 7570 222c  nd_n1mm_lookup",
+000152b0: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
+000152c0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7365      self.n1mm.se
+000152d0: 6e64 5f73 636f 7265 5f70 6163 6b65 7473  nd_score_packets
+000152e0: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
+000152f0: 2822 7365 6e64 5f6e 316d 6d5f 7363 6f72  ("send_n1mm_scor
+00015300: 6522 2c20 4661 6c73 6529 0a20 2020 2020  e", False).     
+00015310: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00015320: 2e72 6164 696f 5f69 6e66 6f5b 2253 7461  .radio_info["Sta
+00015330: 7469 6f6e 4e61 6d65 225d 203d 2073 656c  tionName"] = sel
+00015340: 662e 7072 6566 2e67 6574 2822 6e31 6d6d  f.pref.get("n1mm
+00015350: 5f73 7461 7469 6f6e 5f6e 616d 6522 2c20  _station_name", 
+00015360: 2222 290a 0a20 2020 2020 2020 2073 656c  "")..        sel
+00015370: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
+00015380: 7574 746f 6e73 2829 0a20 2020 2020 2020  uttons().       
+00015390: 2073 656c 662e 7368 6f77 5f43 575f 6d61   self.show_CW_ma
+000153a0: 6372 6f73 2829 0a0a 2020 2020 2020 2020  cros()..        
+000153b0: 2320 4966 2062 616e 6473 206c 6973 7420  # If bands list 
+000153c0: 6973 2065 6d70 7479 2066 696c 6c20 6974  is empty fill it
+000153d0: 2077 6974 6820 4846 2e0a 2020 2020 2020   with HF..      
+000153e0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+000153f0: 6574 2822 6261 6e64 7322 2c20 5b5d 2920  et("bands", []) 
+00015400: 3d3d 205b 5d3a 0a20 2020 2020 2020 2020  == []:.         
+00015410: 2020 2073 656c 662e 7072 6566 5b22 6261     self.pref["ba
+00015420: 6e64 7322 5d20 3d20 5b22 3136 3022 2c20  nds"] = ["160", 
+00015430: 2238 3022 2c20 2234 3022 2c20 2232 3022  "80", "40", "20"
+00015440: 2c20 2231 3522 2c20 2231 3022 5d0a 0a20  , "15", "10"].. 
+00015450: 2020 2020 2020 2023 2048 6964 6520 616c         # Hide al
+00015460: 6c20 7468 6520 6261 6e64 7320 616e 6420  l the bands and 
+00015470: 7468 656e 2073 686f 7720 6f6e 6c79 2074  then show only t
+00015480: 6865 2077 616e 7465 6420 6261 6e64 732e  he wanted bands.
+00015490: 0a20 2020 2020 2020 2066 6f72 205f 696e  .        for _in
+000154a0: 6469 6361 746f 7220 696e 205b 0a20 2020  dicator in [.   
+000154b0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+000154c0: 6e64 5f69 6e64 6963 6174 6f72 735f 6377  nd_indicators_cw
+000154d0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+000154e0: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
+000154f0: 7273 5f73 7362 2c0a 2020 2020 2020 2020  rs_ssb,.        
+00015500: 2020 2020 7365 6c66 2e62 616e 645f 696e      self.band_in
+00015510: 6469 6361 746f 7273 5f72 7474 792c 0a20  dicators_rtty,. 
+00015520: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
+00015530: 2020 2020 2020 666f 7220 5f62 616e 6469        for _bandi
+00015540: 6e64 2069 6e20 5f69 6e64 6963 6174 6f72  nd in _indicator
+00015550: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
+00015560: 2020 2020 2020 2020 2020 205f 6261 6e64             _band
+00015570: 696e 642e 6869 6465 2829 0a20 2020 2020  ind.hide().     
+00015580: 2020 2020 2020 2066 6f72 2062 616e 645f         for band_
+00015590: 746f 5f73 686f 7720 696e 2073 656c 662e  to_show in self.
+000155a0: 7072 6566 2e67 6574 2822 6261 6e64 7322  pref.get("bands"
+000155b0: 2c20 5b5d 293a 0a20 2020 2020 2020 2020  , []):.         
+000155c0: 2020 2020 2020 2069 6620 6261 6e64 5f74         if band_t
+000155d0: 6f5f 7368 6f77 2069 6e20 5f69 6e64 6963  o_show in _indic
+000155e0: 6174 6f72 3a0a 2020 2020 2020 2020 2020  ator:.          
+000155f0: 2020 2020 2020 2020 2020 5f69 6e64 6963            _indic
+00015600: 6174 6f72 5b62 616e 645f 746f 5f73 686f  ator[band_to_sho
+00015610: 775d 2e73 686f 7728 290a 2020 2020 2020  w].show().      
+00015620: 2020 2320 7365 6c66 2e73 686f 775f 6261    # self.show_ba
+00015630: 6e64 5f6d 6f64 6528 290a 0a20 2020 2064  nd_mode()..    d
+00015640: 6566 2077 6174 6368 5f75 6470 2873 656c  ef watch_udp(sel
+00015650: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00015660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015670: 5761 7463 6820 7468 6520 5544 5020 736f  Watch the UDP so
+00015680: 636b 6574 2066 6f72 2069 6e63 6f6d 696e  cket for incomin
+00015690: 6720 6461 7461 2e0a 0a20 2020 2020 2020  g data...       
+000156a0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000156b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000156c0: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
+000156d0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+000156e0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+000156f0: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
+00015700: 2020 2222 220a 0a20 2020 2020 2020 2077    """..        w
+00015710: 6869 6c65 2073 656c 662e 6d75 6c74 6963  hile self.multic
+00015720: 6173 745f 696e 7465 7266 6163 652e 6861  ast_interface.ha
+00015730: 735f 7065 6e64 696e 675f 6461 7461 6772  s_pending_datagr
+00015740: 616d 7328 293a 0a20 2020 2020 2020 2020  ams():.         
+00015750: 2020 206a 736f 6e5f 6461 7461 203d 2073     json_data = s
+00015760: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00015770: 7465 7266 6163 652e 7265 6164 5f64 6174  terface.read_dat
+00015780: 6167 7261 6d5f 6173 5f6a 736f 6e28 290a  agram_as_json().
+00015790: 2020 2020 2020 2020 2020 2020 6966 206a              if j
+000157a0: 736f 6e5f 6461 7461 3a0a 2020 2020 2020  son_data:.      
+000157b0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157d0: 2020 206a 736f 6e5f 6461 7461 2e67 6574     json_data.get
+000157e0: 2822 636d 6422 2c20 2222 2920 3d3d 2022  ("cmd", "") == "
+000157f0: 4745 5443 4f4c 554d 4e53 220a 2020 2020  GETCOLUMNS".    
+00015800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015810: 616e 6420 6a73 6f6e 5f64 6174 612e 6765  and json_data.ge
+00015820: 7428 2273 7461 7469 6f6e 222c 2022 2229  t("station", "")
+00015830: 203d 3d20 706c 6174 666f 726d 2e6e 6f64   == platform.nod
+00015840: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00015850: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00015860: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00015870: 7361 7474 7228 7365 6c66 2e63 6f6e 7465  sattr(self.conte
+00015880: 7374 2c20 2263 6f6c 756d 6e73 2229 3a0a  st, "columns"):.
+00015890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158a0: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+000158b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158c0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+000158d0: 6422 5d20 3d20 2253 484f 5743 4f4c 554d  d"] = "SHOWCOLUM
+000158e0: 4e53 220a 2020 2020 2020 2020 2020 2020  NS".            
+000158f0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00015900: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+00015910: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+00015920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015930: 2020 2020 2063 6d64 5b22 434f 4c55 4d4e       cmd["COLUMN
+00015940: 5322 5d20 3d20 7365 6c66 2e63 6f6e 7465  S"] = self.conte
+00015950: 7374 2e63 6f6c 756d 6e73 0a20 2020 2020  st.columns.     
+00015960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015970: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
+00015980: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
+00015990: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
+000159a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159b0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+000159c0: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159e0: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
+000159f0: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
+00015a00: 2254 554e 4522 0a20 2020 2020 2020 2020  "TUNE".         
+00015a10: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
+00015a20: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
+00015a30: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
+00015a40: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+00015a50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00015a60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015a70: 2020 2020 2020 2320 6227 7b22 636d 6422        # b'{"cmd"
+00015a80: 3a20 2254 554e 4522 2c20 2266 7265 7122  : "TUNE", "freq"
+00015a90: 3a20 372e 3032 3335 2c20 2273 706f 7422  : 7.0235, "spot"
+00015aa0: 3a20 224d 4d30 4447 4922 7d27 0a20 2020  : "MM0DGI"}'.   
 00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ac0: 636d 645b 2243 4f4c 554d 4e53 225d 203d  cmd["COLUMNS"] =
-00015ad0: 2073 656c 662e 636f 6e74 6573 742e 636f   self.contest.co
-00015ae0: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
-00015af0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015b00: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00015b10: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-00015b20: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
-00015b30: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00015b40: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00015b50: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00015b60: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-00015b70: 736f 6e5f 6461 7461 2e67 6574 2822 636d  son_data.get("cm
-00015b80: 6422 2c20 2222 2920 3d3d 2022 5455 4e45  d", "") == "TUNE
-00015b90: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00015ba0: 2020 2020 2020 616e 6420 6a73 6f6e 5f64        and json_d
-00015bb0: 6174 612e 6765 7428 2273 7461 7469 6f6e  ata.get("station
-00015bc0: 222c 2022 2229 203d 3d20 706c 6174 666f  ", "") == platfo
-00015bd0: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-00015be0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00015bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c00: 2023 2062 277b 2263 6d64 223a 2022 5455   # b'{"cmd": "TU
-00015c10: 4e45 222c 2022 6672 6571 223a 2037 2e30  NE", "freq": 7.0
-00015c20: 3233 352c 2022 7370 6f74 223a 2022 4d4d  235, "spot": "MM
-00015c30: 3044 4749 227d 270a 2020 2020 2020 2020  0DGI"}'.        
-00015c40: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
-00015c50: 3d20 6a73 6f6e 5f64 6174 612e 6765 7428  = json_data.get(
-00015c60: 2266 7265 7122 290a 2020 2020 2020 2020  "freq").        
-00015c70: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
-00015c80: 3d20 666c 6f61 7428 7666 6f29 202a 2031  = float(vfo) * 1
-00015c90: 3030 3030 3030 0a20 2020 2020 2020 2020  000000.         
-00015ca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015cb0: 7261 6469 6f5f 7374 6174 655b 2276 666f  radio_state["vfo
-00015cc0: 6122 5d20 3d20 696e 7428 7666 6f29 0a20  a"] = int(vfo). 
-00015cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ce0: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-00015cf0: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
-00015d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d10: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00015d20: 2e73 6574 5f76 666f 2869 6e74 2876 666f  .set_vfo(int(vfo
-00015d30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00015d40: 2020 2020 2020 2073 706f 7420 3d20 6a73         spot = js
-00015d50: 6f6e 5f64 6174 612e 6765 7428 2273 706f  on_data.get("spo
-00015d60: 7422 2c20 2222 290a 2020 2020 2020 2020  t", "").        
-00015d70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015d80: 2e63 616c 6c73 6967 6e2e 7365 7454 6578  .callsign.setTex
-00015d90: 7428 7370 6f74 290a 2020 2020 2020 2020  t(spot).        
-00015da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015db0: 2e63 616c 6c73 6967 6e5f 6368 616e 6765  .callsign_change
-00015dc0: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-00015dd0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-00015de0: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
-00015df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e00: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
-00015e10: 676e 2e61 6374 6976 6174 6557 696e 646f  gn.activateWindo
-00015e20: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-00015e30: 2020 2020 2020 2020 7769 6e64 6f77 2e72          window.r
-00015e40: 6169 7365 5f28 290a 2020 2020 2020 2020  aise_().        
-00015e50: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00015e60: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-00015e70: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00015e80: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-00015e90: 736f 6e5f 6461 7461 2e67 6574 2822 636d  son_data.get("cm
-00015ea0: 6422 2c20 2222 2920 3d3d 2022 4745 5457  d", "") == "GETW
-00015eb0: 4f52 4b45 444c 4953 5422 0a20 2020 2020  ORKEDLIST".     
-00015ec0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00015ed0: 6e64 206a 736f 6e5f 6461 7461 2e67 6574  nd json_data.get
-00015ee0: 2822 7374 6174 696f 6e22 2c20 2222 2920  ("station", "") 
-00015ef0: 3d3d 2070 6c61 7466 6f72 6d2e 6e6f 6465  == platform.node
-00015f00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00015f10: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00015f20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00015f30: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00015f40: 2e67 6574 5f63 616c 6c73 5f61 6e64 5f62  .get_calls_and_b
-00015f50: 616e 6473 2829 0a20 2020 2020 2020 2020  ands().         
-00015f60: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00015f70: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00015f80: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00015f90: 225d 203d 2022 574f 524b 4544 220a 2020  "] = "WORKED".  
+00015ac0: 2076 666f 203d 206a 736f 6e5f 6461 7461   vfo = json_data
+00015ad0: 2e67 6574 2822 6672 6571 2229 0a20 2020  .get("freq").   
+00015ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015af0: 2076 666f 203d 2066 6c6f 6174 2876 666f   vfo = float(vfo
+00015b00: 2920 2a20 3130 3030 3030 300a 2020 2020  ) * 1000000.    
+00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b20: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+00015b30: 5b22 7666 6f61 225d 203d 2069 6e74 2876  ["vfoa"] = int(v
+00015b40: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
+00015b50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00015b60: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b80: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+00015b90: 6e74 726f 6c2e 7365 745f 7666 6f28 696e  ntrol.set_vfo(in
+00015ba0: 7428 7666 6f29 290a 2020 2020 2020 2020  t(vfo)).        
+00015bb0: 2020 2020 2020 2020 2020 2020 7370 6f74              spot
+00015bc0: 203d 206a 736f 6e5f 6461 7461 2e67 6574   = json_data.get
+00015bd0: 2822 7370 6f74 222c 2022 2229 0a20 2020  ("spot", "").   
+00015be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bf0: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
+00015c00: 6574 5465 7874 2873 706f 7429 0a20 2020  etText(spot).   
+00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c20: 2073 656c 662e 6361 6c6c 7369 676e 5f63   self.callsign_c
+00015c30: 6861 6e67 6564 2829 0a20 2020 2020 2020  hanged().       
+00015c40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015c50: 662e 6361 6c6c 7369 676e 2e73 6574 466f  f.callsign.setFo
+00015c60: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00015c70: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00015c80: 616c 6c73 6967 6e2e 6163 7469 7661 7465  allsign.activate
+00015c90: 5769 6e64 6f77 2829 0a20 2020 2020 2020  Window().       
+00015ca0: 2020 2020 2020 2020 2020 2020 2077 696e               win
+00015cb0: 646f 772e 7261 6973 655f 2829 0a20 2020  dow.raise_().   
+00015cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cd0: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+00015ce0: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00015cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d00: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
+00015d10: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
+00015d20: 2247 4554 574f 524b 4544 4c49 5354 220a  "GETWORKEDLIST".
+00015d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d40: 2020 2020 616e 6420 6a73 6f6e 5f64 6174      and json_dat
+00015d50: 612e 6765 7428 2273 7461 7469 6f6e 222c  a.get("station",
+00015d60: 2022 2229 203d 3d20 706c 6174 666f 726d   "") == platform
+00015d70: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+00015d80: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00015d90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015da0: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
+00015db0: 6162 6173 652e 6765 745f 6361 6c6c 735f  abase.get_calls_
+00015dc0: 616e 645f 6261 6e64 7328 290a 2020 2020  and_bands().    
+00015dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015de0: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00015df0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00015e00: 5b22 636d 6422 5d20 3d20 2257 4f52 4b45  ["cmd"] = "WORKE
+00015e10: 4422 0a20 2020 2020 2020 2020 2020 2020  D".             
+00015e20: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+00015e30: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+00015e40: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+00015e50: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00015e60: 2277 6f72 6b65 6422 5d20 3d20 7265 7375  "worked"] = resu
+00015e70: 6c74 0a20 2020 2020 2020 2020 2020 2020  lt.             
+00015e80: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00015e90: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00015ea0: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+00015eb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015ec0: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ee0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00015ef0: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
+00015f00: 7461 2e67 6574 2822 636d 6422 2c20 2222  ta.get("cmd", ""
+00015f10: 2920 3d3d 2022 4745 5443 4f4e 5445 5354  ) == "GETCONTEST
+00015f20: 5354 4154 5553 220a 2020 2020 2020 2020  STATUS".        
+00015f30: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00015f40: 6a73 6f6e 5f64 6174 612e 6765 7428 2273  json_data.get("s
+00015f50: 7461 7469 6f6e 222c 2022 2229 203d 3d20  tation", "") == 
+00015f60: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00015f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015f90: 2020 2020 2020 2063 6d64 203d 207b 0a20         cmd = {. 
 00015fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fb0: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00015fc0: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00015fd0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00015fe0: 2020 2020 2020 2063 6d64 5b22 776f 726b         cmd["work
-00015ff0: 6564 225d 203d 2072 6573 756c 740a 2020  ed"] = result.  
-00016000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016010: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-00016020: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-00016030: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
+00015fb0: 2020 2020 2020 2022 636d 6422 3a20 2243         "cmd": "C
+00015fc0: 4f4e 5445 5354 5354 4154 5553 222c 0a20  ONTESTSTATUS",. 
+00015fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fe0: 2020 2020 2020 2022 7374 6174 696f 6e22         "station"
+00015ff0: 3a20 706c 6174 666f 726d 2e6e 6f64 6528  : platform.node(
+00016000: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00016010: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
+00016020: 6573 7422 3a20 7365 6c66 2e63 6f6e 7465  est": self.conte
+00016030: 7374 5f73 6574 7469 6e67 732c 0a20 2020  st_settings,.   
 00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016050: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
-00016060: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-00016070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016080: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
-00016090: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
-000160a0: 2247 4554 434f 4e54 4553 5453 5441 5455  "GETCONTESTSTATU
-000160b0: 5322 0a20 2020 2020 2020 2020 2020 2020  S".             
-000160c0: 2020 2020 2020 2061 6e64 206a 736f 6e5f         and json_
-000160d0: 6461 7461 2e67 6574 2822 7374 6174 696f  data.get("statio
-000160e0: 6e22 2c20 2222 2920 3d3d 2070 6c61 7466  n", "") == platf
-000160f0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-00016100: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016120: 2020 636d 6420 3d20 7b0a 2020 2020 2020    cmd = {.      
-00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016140: 2020 2263 6d64 223a 2022 434f 4e54 4553    "cmd": "CONTES
-00016150: 5453 5441 5455 5322 2c0a 2020 2020 2020  TSTATUS",.      
-00016160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016170: 2020 2273 7461 7469 6f6e 223a 2070 6c61    "station": pla
-00016180: 7466 6f72 6d2e 6e6f 6465 2829 2c0a 2020  tform.node(),.  
-00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161a0: 2020 2020 2020 2263 6f6e 7465 7374 223a        "contest":
-000161b0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
-000161c0: 7474 696e 6773 2c0a 2020 2020 2020 2020  ttings,.        
-000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161e0: 226f 7065 7261 746f 7222 3a20 7365 6c66  "operator": self
-000161f0: 2e63 7572 7265 6e74 5f6f 702c 0a20 2020  .current_op,.   
-00016200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016210: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00016220: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-00016230: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00016240: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00016250: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016260: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016280: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00016290: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
-000162a0: 7461 2e67 6574 2822 636d 6422 2c20 2222  ta.get("cmd", ""
-000162b0: 2920 3d3d 2022 4348 414e 4745 4341 4c4c  ) == "CHANGECALL
-000162c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000162d0: 2020 2020 2020 616e 6420 6a73 6f6e 5f64        and json_d
-000162e0: 6174 612e 6765 7428 2273 7461 7469 6f6e  ata.get("station
-000162f0: 222c 2022 2229 203d 3d20 706c 6174 666f  ", "") == platfo
-00016300: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-00016310: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00016320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016330: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
-00016340: 6574 5465 7874 286a 736f 6e5f 6461 7461  etText(json_data
-00016350: 2e67 6574 2822 6361 6c6c 222c 2022 2229  .get("call", "")
-00016360: 290a 0a20 2020 2064 6566 2064 6172 6b5f  )..    def dark_
-00016370: 6d6f 6465 5f73 7461 7465 5f63 6861 6e67  mode_state_chang
-00016380: 6564 2873 656c 6629 202d 3e20 4e6f 6e65  ed(self) -> None
-00016390: 3a0a 2020 2020 2020 2020 2222 2243 616c  :.        """Cal
-000163a0: 6c65 6420 7768 656e 2074 6865 2044 6172  led when the Dar
-000163b0: 6b20 4d6f 6465 206d 656e 7520 7374 6174  k Mode menu stat
-000163c0: 6520 6973 2063 6861 6e67 6564 2e22 2222  e is changed."""
-000163d0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-000163e0: 6566 5b22 6461 726b 6d6f 6465 225d 203d  ef["darkmode"] =
-000163f0: 2073 656c 662e 6163 7469 6f6e 4461 726b   self.actionDark
-00016400: 5f4d 6f64 655f 322e 6973 4368 6563 6b65  _Mode_2.isChecke
-00016410: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
-00016420: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
-00016430: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-00016440: 2e73 6574 4461 726b 4d6f 6465 2873 656c  .setDarkMode(sel
-00016450: 662e 6163 7469 6f6e 4461 726b 5f4d 6f64  f.actionDark_Mod
-00016460: 655f 322e 6973 4368 6563 6b65 6428 2929  e_2.isChecked())
-00016470: 0a0a 2020 2020 6465 6620 6377 5f6d 6163  ..    def cw_mac
-00016480: 726f 735f 7374 6174 655f 6368 616e 6765  ros_state_change
-00016490: 6428 7365 6c66 2920 2d3e 204e 6f6e 653a  d(self) -> None:
-000164a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000164b0: 2020 2020 204d 656e 7520 6974 656d 2074       Menu item t
-000164c0: 6f20 7368 6f77 2f68 6964 6520 6d61 6372  o show/hide macr
-000164d0: 6f20 6275 7474 6f6e 732e 0a0a 2020 2020  o buttons...    
-000164e0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000164f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00016500: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
-00016510: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00016520: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00016530: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-00016540: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00016550: 2020 7365 6c66 2e70 7265 665b 2263 775f    self.pref["cw_
-00016560: 6d61 6372 6f73 225d 203d 2073 656c 662e  macros"] = self.
-00016570: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
-00016580: 6973 4368 6563 6b65 6428 290a 2020 2020  isChecked().    
-00016590: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
-000165a0: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
-000165b0: 2020 2020 7365 6c66 2e73 686f 775f 4357      self.show_CW
-000165c0: 5f6d 6163 726f 7328 290a 0a20 2020 2064  _macros()..    d
-000165d0: 6566 2073 686f 775f 4357 5f6d 6163 726f  ef show_CW_macro
-000165e0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-000165f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016600: 2020 2020 2053 686f 772f 4869 6465 2074       Show/Hide t
-00016610: 6865 206d 6163 726f 2062 7574 746f 6e73  he macro buttons
-00016620: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00016630: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00016640: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00016650: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
-00016660: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00016670: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-00016680: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-00016690: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000166a0: 2e70 7265 662e 6765 7428 2263 775f 6d61  .pref.get("cw_ma
-000166b0: 6372 6f73 2229 3a0a 2020 2020 2020 2020  cros"):.        
-000166c0: 2020 2020 7365 6c66 2e42 7574 746f 6e5f      self.Button_
-000166d0: 526f 7731 2e73 686f 7728 290a 2020 2020  Row1.show().    
-000166e0: 2020 2020 2020 2020 7365 6c66 2e42 7574          self.But
-000166f0: 746f 6e5f 526f 7732 2e73 686f 7728 290a  ton_Row2.show().
-00016700: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016710: 2020 2020 2020 2020 2020 7365 6c66 2e42            self.B
-00016720: 7574 746f 6e5f 526f 7731 2e68 6964 6528  utton_Row1.hide(
-00016730: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00016740: 6c66 2e42 7574 746f 6e5f 526f 7732 2e68  lf.Button_Row2.h
-00016750: 6964 6528 290a 0a20 2020 2064 6566 2063  ide()..    def c
-00016760: 6f6d 6d61 6e64 5f62 7574 746f 6e73 5f73  ommand_buttons_s
-00016770: 7461 7465 5f63 6861 6e67 6528 7365 6c66  tate_change(self
-00016780: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00016790: 2020 2022 2222 0a20 2020 2020 2020 204d     """.        M
-000167a0: 656e 7520 6974 656d 2074 6f20 7368 6f77  enu item to show
-000167b0: 2f68 6964 6520 636f 6d6d 616e 6420 6275  /hide command bu
-000167c0: 7474 6f6e 730a 0a20 2020 2020 2020 2050  ttons..        P
-000167d0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-000167e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000167f0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-00016800: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00016810: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00016820: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-00016830: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
-00016840: 662e 7072 6566 5b22 636f 6d6d 616e 645f  f.pref["command_
-00016850: 6275 7474 6f6e 7322 5d20 3d20 7365 6c66  buttons"] = self
-00016860: 2e61 6374 696f 6e43 6f6d 6d61 6e64 5f42  .actionCommand_B
-00016870: 7574 746f 6e73 2e69 7343 6865 636b 6564  uttons.isChecked
-00016880: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00016890: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-000168a0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000168b0: 7368 6f77 5f63 6f6d 6d61 6e64 5f62 7574  show_command_but
-000168c0: 746f 6e73 2829 0a0a 2020 2020 6465 6620  tons()..    def 
-000168d0: 7368 6f77 5f63 6f6d 6d61 6e64 5f62 7574  show_command_but
-000168e0: 746f 6e73 2873 656c 6629 202d 3e20 4e6f  tons(self) -> No
-000168f0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00016900: 2020 2020 2020 2020 5368 6f77 2f48 6964          Show/Hid
-00016910: 6520 7468 6520 636f 6d6d 616e 6420 6275  e the command bu
-00016920: 7474 6f6e 7320 6465 7065 6e64 696e 6720  ttons depending 
-00016930: 6f6e 2074 6865 2070 7265 6665 7265 6e63  on the preferenc
-00016940: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-00016950: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00016960: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00016970: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
-00016980: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00016990: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020 2020  -------..       
-000169a0: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
-000169b0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000169c0: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
-000169d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000169e0: 656c 662e 436f 6d6d 616e 645f 4275 7474  elf.Command_Butt
-000169f0: 6f6e 732e 7368 6f77 2829 0a20 2020 2020  ons.show().     
-00016a00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00016a10: 2020 2020 2073 656c 662e 436f 6d6d 616e       self.Comman
-00016a20: 645f 4275 7474 6f6e 732e 6869 6465 2829  d_Buttons.hide()
-00016a30: 0a0a 2020 2020 6465 6620 6973 5f66 6c6f  ..    def is_flo
-00016a40: 6174 6162 6c65 2873 656c 662c 2069 7465  atable(self, ite
-00016a50: 6d3a 2073 7472 2920 2d3e 2062 6f6f 6c3a  m: str) -> bool:
-00016a60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016a70: 2020 2020 2043 6865 636b 2074 6f20 7365       Check to se
-00016a80: 6520 6966 2073 7472 696e 6720 6361 6e20  e if string can 
-00016a90: 6265 2061 2066 6c6f 6174 2e0a 0a20 2020  be a float...   
-00016aa0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00016ab0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00016ac0: 2d2d 0a20 2020 2020 2020 2069 7465 6d20  --.        item 
-00016ad0: 3a20 7374 720a 2020 2020 2020 2020 5468  : str.        Th
-00016ae0: 6520 7374 7269 6e67 2074 6f20 7465 7374  e string to test
-00016af0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00016b00: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00016b10: 2d2d 0a20 2020 2020 2020 2062 6f6f 6c0a  --.        bool.
-00016b20: 2020 2020 2020 2020 5472 7565 2069 6620          True if 
-00016b30: 7374 7269 6e67 2063 616e 2062 6520 6120  string can be a 
-00016b40: 666c 6f61 742c 2046 616c 7365 206f 7468  float, False oth
-00016b50: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-00016b60: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
-00016b70: 6974 656d 2e69 736e 756d 6572 6963 2829  item.isnumeric()
-00016b80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00016b90: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00016ba0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00016bb0: 2020 205f 7465 7374 203d 2066 6c6f 6174     _test = float
-00016bc0: 2869 7465 6d29 0a20 2020 2020 2020 2065  (item).        e
-00016bd0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00016be0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00016bf0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00016c00: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00016c10: 2020 2020 6465 6620 6f74 6865 725f 315f      def other_1_
-00016c20: 6368 616e 6765 6428 7365 6c66 2920 2d3e  changed(self) ->
-00016c30: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00016c40: 2222 0a20 2020 2020 2020 2054 6865 2074  "".        The t
-00016c50: 6578 7420 696e 2074 6865 206f 7468 6572  ext in the other
-00016c60: 5f31 2066 6965 6c64 2068 6173 2063 6861  _1 field has cha
-00016c70: 6e67 6564 2e0a 2020 2020 2020 2020 5374  nged..        St
-00016c80: 7269 7020 6f75 7420 616e 7920 7370 6163  rip out any spac
-00016c90: 6573 2061 6e64 2073 6574 2074 6865 2074  es and set the t
-00016ca0: 6578 742e 0a0a 2020 2020 2020 2020 5061  ext...        Pa
-00016cb0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00016cc0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00016cd0: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
-00016ce0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00016cf0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00016d00: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
-00016d10: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
-00016d20: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
-00016d30: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-00016d40: 7474 7228 7365 6c66 2e63 6f6e 7465 7374  ttr(self.contest
-00016d50: 2c20 2261 6476 616e 6365 5f6f 6e5f 7370  , "advance_on_sp
-00016d60: 6163 6522 293a 0a20 2020 2020 2020 2020  ace"):.         
-00016d70: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00016d80: 6f6e 7465 7374 2e61 6476 616e 6365 5f6f  ontest.advance_o
-00016d90: 6e5f 7370 6163 655b 335d 3a0a 2020 2020  n_space[3]:.    
-00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016db0: 7465 7874 203d 2073 656c 662e 6f74 6865  text = self.othe
-00016dc0: 725f 312e 7465 7874 2829 0a20 2020 2020  r_1.text().     
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00016de0: 6578 7420 3d20 7465 7874 2e75 7070 6572  ext = text.upper
+00016050: 2020 2020 2022 6f70 6572 6174 6f72 223a       "operator":
+00016060: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+00016070: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016080: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00016090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000160a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+000160b0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+000160c0: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
+000160d0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+000160e0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+000160f0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00016100: 2020 2020 2020 2020 2020 2020 2020 6a73                js
+00016110: 6f6e 5f64 6174 612e 6765 7428 2263 6d64  on_data.get("cmd
+00016120: 222c 2022 2229 203d 3d20 2243 4841 4e47  ", "") == "CHANG
+00016130: 4543 414c 4c22 0a20 2020 2020 2020 2020  ECALL".         
+00016140: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
+00016150: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
+00016160: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
+00016170: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+00016180: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00016190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000161a0: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
+000161b0: 6967 6e2e 7365 7454 6578 7428 6a73 6f6e  ign.setText(json
+000161c0: 5f64 6174 612e 6765 7428 2263 616c 6c22  _data.get("call"
+000161d0: 2c20 2222 2929 0a0a 2020 2020 6465 6620  , ""))..    def 
+000161e0: 6461 726b 5f6d 6f64 655f 7374 6174 655f  dark_mode_state_
+000161f0: 6368 616e 6765 6428 7365 6c66 2920 2d3e  changed(self) ->
+00016200: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00016210: 2222 4361 6c6c 6564 2077 6865 6e20 7468  ""Called when th
+00016220: 6520 4461 726b 204d 6f64 6520 6d65 6e75  e Dark Mode menu
+00016230: 2073 7461 7465 2069 7320 6368 616e 6765   state is change
+00016240: 642e 2222 220a 2020 2020 2020 2020 7365  d.""".        se
+00016250: 6c66 2e70 7265 665b 2264 6172 6b6d 6f64  lf.pref["darkmod
+00016260: 6522 5d20 3d20 7365 6c66 2e61 6374 696f  e"] = self.actio
+00016270: 6e44 6172 6b5f 4d6f 6465 5f32 2e69 7343  nDark_Mode_2.isC
+00016280: 6865 636b 6564 2829 0a20 2020 2020 2020  hecked().       
+00016290: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
+000162a0: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
+000162b0: 2073 656c 662e 7365 7444 6172 6b4d 6f64   self.setDarkMod
+000162c0: 6528 7365 6c66 2e61 6374 696f 6e44 6172  e(self.actionDar
+000162d0: 6b5f 4d6f 6465 5f32 2e69 7343 6865 636b  k_Mode_2.isCheck
+000162e0: 6564 2829 290a 0a20 2020 2064 6566 2063  ed())..    def c
+000162f0: 775f 6d61 6372 6f73 5f73 7461 7465 5f63  w_macros_state_c
+00016300: 6861 6e67 6564 2873 656c 6629 202d 3e20  hanged(self) -> 
+00016310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00016320: 220a 2020 2020 2020 2020 4d65 6e75 2069  ".        Menu i
+00016330: 7465 6d20 746f 2073 686f 772f 6869 6465  tem to show/hide
+00016340: 206d 6163 726f 2062 7574 746f 6e73 2e0a   macro buttons..
+00016350: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00016360: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00016370: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00016380: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
+00016390: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+000163a0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+000163b0: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
+000163c0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+000163d0: 5b22 6377 5f6d 6163 726f 7322 5d20 3d20  ["cw_macros"] = 
+000163e0: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
+000163f0: 6372 6f73 2e69 7343 6865 636b 6564 2829  cros.isChecked()
+00016400: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
+00016410: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
+00016420: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
+00016430: 6f77 5f43 575f 6d61 6372 6f73 2829 0a0a  ow_CW_macros()..
+00016440: 2020 2020 6465 6620 7368 6f77 5f43 575f      def show_CW_
+00016450: 6d61 6372 6f73 2873 656c 6629 202d 3e20  macros(self) -> 
+00016460: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00016470: 220a 2020 2020 2020 2020 5368 6f77 2f48  ".        Show/H
+00016480: 6964 6520 7468 6520 6d61 6372 6f20 6275  ide the macro bu
+00016490: 7474 6f6e 732e 0a0a 2020 2020 2020 2020  ttons...        
+000164a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000164b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000164c0: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
+000164d0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+000164e0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000164f0: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+00016500: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+00016510: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+00016520: 6377 5f6d 6163 726f 7322 293a 0a20 2020  cw_macros"):.   
+00016530: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
+00016540: 7474 6f6e 5f52 6f77 312e 7368 6f77 2829  tton_Row1.show()
+00016550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016560: 662e 4275 7474 6f6e 5f52 6f77 322e 7368  f.Button_Row2.sh
+00016570: 6f77 2829 0a20 2020 2020 2020 2065 6c73  ow().        els
+00016580: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00016590: 656c 662e 4275 7474 6f6e 5f52 6f77 312e  elf.Button_Row1.
+000165a0: 6869 6465 2829 0a20 2020 2020 2020 2020  hide().         
+000165b0: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
+000165c0: 6f77 322e 6869 6465 2829 0a0a 2020 2020  ow2.hide()..    
+000165d0: 6465 6620 636f 6d6d 616e 645f 6275 7474  def command_butt
+000165e0: 6f6e 735f 7374 6174 655f 6368 616e 6765  ons_state_change
+000165f0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00016600: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00016610: 2020 2020 4d65 6e75 2069 7465 6d20 746f      Menu item to
+00016620: 2073 686f 772f 6869 6465 2063 6f6d 6d61   show/hide comma
+00016630: 6e64 2062 7574 746f 6e73 0a0a 2020 2020  nd buttons..    
+00016640: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00016650: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00016660: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
+00016670: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00016680: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00016690: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+000166a0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000166b0: 2020 7365 6c66 2e70 7265 665b 2263 6f6d    self.pref["com
+000166c0: 6d61 6e64 5f62 7574 746f 6e73 225d 203d  mand_buttons"] =
+000166d0: 2073 656c 662e 6163 7469 6f6e 436f 6d6d   self.actionComm
+000166e0: 616e 645f 4275 7474 6f6e 732e 6973 4368  and_Buttons.isCh
+000166f0: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
+00016700: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+00016710: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+00016720: 7365 6c66 2e73 686f 775f 636f 6d6d 616e  self.show_comman
+00016730: 645f 6275 7474 6f6e 7328 290a 0a20 2020  d_buttons()..   
+00016740: 2064 6566 2073 686f 775f 636f 6d6d 616e   def show_comman
+00016750: 645f 6275 7474 6f6e 7328 7365 6c66 2920  d_buttons(self) 
+00016760: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00016770: 2022 2222 0a20 2020 2020 2020 2053 686f   """.        Sho
+00016780: 772f 4869 6465 2074 6865 2063 6f6d 6d61  w/Hide the comma
+00016790: 6e64 2062 7574 746f 6e73 2064 6570 656e  nd buttons depen
+000167a0: 6469 6e67 206f 6e20 7468 6520 7072 6566  ding on the pref
+000167b0: 6572 656e 6365 2e0a 0a20 2020 2020 2020  erence...       
+000167c0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000167d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000167e0: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
+000167f0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00016800: 2020 2020 202d 2d2d 2d2d 2d2d 0a0a 2020       -------..  
+00016810: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00016820: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+00016830: 6765 7428 2263 6f6d 6d61 6e64 5f62 7574  get("command_but
+00016840: 746f 6e73 2229 3a0a 2020 2020 2020 2020  tons"):.        
+00016850: 2020 2020 7365 6c66 2e43 6f6d 6d61 6e64      self.Command
+00016860: 5f42 7574 746f 6e73 2e73 686f 7728 290a  _Buttons.show().
+00016870: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00016880: 2020 2020 2020 2020 2020 7365 6c66 2e43            self.C
+00016890: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e68  ommand_Buttons.h
+000168a0: 6964 6528 290a 0a20 2020 2064 6566 2069  ide()..    def i
+000168b0: 735f 666c 6f61 7461 626c 6528 7365 6c66  s_floatable(self
+000168c0: 2c20 6974 656d 3a20 7374 7229 202d 3e20  , item: str) -> 
+000168d0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+000168e0: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
+000168f0: 746f 2073 6565 2069 6620 7374 7269 6e67  to see if string
+00016900: 2063 616e 2062 6520 6120 666c 6f61 742e   can be a float.
+00016910: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00016920: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00016930: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00016940: 6974 656d 203a 2073 7472 0a20 2020 2020  item : str.     
+00016950: 2020 2054 6865 2073 7472 696e 6720 746f     The string to
+00016960: 2074 6573 742e 0a0a 2020 2020 2020 2020   test...        
+00016970: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00016980: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00016990: 626f 6f6c 0a20 2020 2020 2020 2054 7275  bool.        Tru
+000169a0: 6520 6966 2073 7472 696e 6720 6361 6e20  e if string can 
+000169b0: 6265 2061 2066 6c6f 6174 2c20 4661 6c73  be a float, Fals
+000169c0: 6520 6f74 6865 7277 6973 652e 0a20 2020  e otherwise..   
+000169d0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000169e0: 2020 6966 2069 7465 6d2e 6973 6e75 6d65    if item.isnume
+000169f0: 7269 6328 293a 0a20 2020 2020 2020 2020  ric():.         
+00016a00: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00016a10: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00016a20: 2020 2020 2020 2020 5f74 6573 7420 3d20          _test = 
+00016a30: 666c 6f61 7428 6974 656d 290a 2020 2020  float(item).    
+00016a40: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+00016a50: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+00016a60: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00016a70: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00016a80: 7275 650a 0a20 2020 2064 6566 206f 7468  rue..    def oth
+00016a90: 6572 5f31 5f63 6861 6e67 6564 2873 656c  er_1_changed(sel
+00016aa0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00016ab0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00016ac0: 5468 6520 7465 7874 2069 6e20 7468 6520  The text in the 
+00016ad0: 6f74 6865 725f 3120 6669 656c 6420 6861  other_1 field ha
+00016ae0: 7320 6368 616e 6765 642e 0a20 2020 2020  s changed..     
+00016af0: 2020 2053 7472 6970 206f 7574 2061 6e79     Strip out any
+00016b00: 2073 7061 6365 7320 616e 6420 7365 7420   spaces and set 
+00016b10: 7468 6520 7465 7874 2e0a 0a20 2020 2020  the text...     
+00016b20: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00016b30: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00016b40: 0a20 2020 2020 2020 204e 6f6e 650a 0a20  .        None.. 
+00016b50: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00016b60: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00016b70: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
+00016b80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00016b90: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+00016ba0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00016bb0: 2068 6173 6174 7472 2873 656c 662e 636f   hasattr(self.co
+00016bc0: 6e74 6573 742c 2022 6164 7661 6e63 655f  ntest, "advance_
+00016bd0: 6f6e 5f73 7061 6365 2229 3a0a 2020 2020  on_space"):.    
+00016be0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00016bf0: 656c 662e 636f 6e74 6573 742e 6164 7661  elf.contest.adva
+00016c00: 6e63 655f 6f6e 5f73 7061 6365 5b33 5d3a  nce_on_space[3]:
+00016c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c20: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
+00016c30: 2e6f 7468 6572 5f31 2e74 6578 7428 290a  .other_1.text().
+00016c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c50: 2020 2020 7465 7874 203d 2074 6578 742e      text = text.
+00016c60: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+00016c70: 2020 2020 2020 2020 2020 2020 2320 706f              # po
+00016c80: 7369 7469 6f6e 203d 2073 656c 662e 6f74  sition = self.ot
+00016c90: 6865 725f 312e 6375 7273 6f72 506f 7369  her_1.cursorPosi
+00016ca0: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
+00016cb0: 2020 2020 2020 2020 2020 2073 7472 6970             strip
+00016cc0: 7065 645f 7465 7874 203d 2074 6578 742e  ped_text = text.
+00016cd0: 7374 7269 7028 292e 7265 706c 6163 6528  strip().replace(
+00016ce0: 2220 222c 2022 2229 0a20 2020 2020 2020  " ", "").       
+00016cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016d00: 662e 6f74 6865 725f 312e 7365 7454 6578  f.other_1.setTex
+00016d10: 7428 7374 7269 7070 6564 5f74 6578 7429  t(stripped_text)
+00016d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d30: 2020 2020 2023 2073 656c 662e 6f74 6865       # self.othe
+00016d40: 725f 312e 7365 7443 7572 736f 7250 6f73  r_1.setCursorPos
+00016d50: 6974 696f 6e28 706f 7369 7469 6f6e 290a  ition(position).
+00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d70: 2020 2020 6966 2022 2022 2069 6e20 7465      if " " in te
+00016d80: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+00016d90: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00016da0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+00016db0: 6e65 7874 2e67 6574 2873 656c 662e 6f74  next.get(self.ot
+00016dc0: 6865 725f 3129 0a20 2020 2020 2020 2020  her_1).         
+00016dd0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016de0: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
 00016df0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00016e00: 2020 2020 2020 2023 2070 6f73 6974 696f         # positio
-00016e10: 6e20 3d20 7365 6c66 2e6f 7468 6572 5f31  n = self.other_1
-00016e20: 2e63 7572 736f 7250 6f73 6974 696f 6e28  .cursorPosition(
-00016e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016e40: 2020 2020 2020 7374 7269 7070 6564 5f74        stripped_t
-00016e50: 6578 7420 3d20 7465 7874 2e73 7472 6970  ext = text.strip
-00016e60: 2829 2e72 6570 6c61 6365 2822 2022 2c20  ().replace(" ", 
-00016e70: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-00016e80: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
-00016e90: 6572 5f31 2e73 6574 5465 7874 2873 7472  er_1.setText(str
-00016ea0: 6970 7065 645f 7465 7874 290a 2020 2020  ipped_text).    
-00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ec0: 2320 7365 6c66 2e6f 7468 6572 5f31 2e73  # self.other_1.s
-00016ed0: 6574 4375 7273 6f72 506f 7369 7469 6f6e  etCursorPosition
-00016ee0: 2870 6f73 6974 696f 6e29 0a20 2020 2020  (position).     
-00016ef0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016f00: 6620 2220 2220 696e 2074 6578 743a 0a20  f " " in text:. 
-00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f20: 2020 2020 2020 206e 6578 745f 7461 6220         next_tab 
-00016f30: 3d20 7365 6c66 2e74 6162 5f6e 6578 742e  = self.tab_next.
-00016f40: 6765 7428 7365 6c66 2e6f 7468 6572 5f31  get(self.other_1
-00016f50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016f60: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00016f70: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
-00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f90: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
-00016fa0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fc0: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
-00016fd0: 616c 7365 290a 0a20 2020 2064 6566 206f  alse)..    def o
-00016fe0: 7468 6572 5f32 5f63 6861 6e67 6564 2873  ther_2_changed(s
-00016ff0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00017000: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00017010: 2020 5465 7874 2069 6e20 6f74 6865 725f    Text in other_
-00017020: 3220 6861 7320 6368 616e 6765 642e 0a20  2 has changed.. 
-00017030: 2020 2020 2020 2053 7472 6970 206f 7574         Strip out
-00017040: 2061 6e79 2073 7061 6365 7320 616e 6420   any spaces and 
-00017050: 7365 7420 7468 6520 7465 7874 2e0a 2020  set the text..  
-00017060: 2020 2020 2020 5061 7273 6520 7468 6520        Parse the 
-00017070: 6578 6368 616e 6765 2069 6620 7468 6520  exchange if the 
-00017080: 636f 6e74 6573 7420 6973 2041 5252 4c20  contest is ARRL 
-00017090: 5377 6565 7073 7461 6b65 732e 0a0a 2020  Sweepstakes...  
-000170a0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000170b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000170c0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000170d0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000170e0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000170f0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-00017100: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00017110: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-00017120: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
-00017130: 2069 6620 2241 5252 4c20 5377 6565 7073   if "ARRL Sweeps
-00017140: 7461 6b65 7322 2069 6e20 7365 6c66 2e63  takes" in self.c
-00017150: 6f6e 7465 7374 2e6e 616d 653a 0a20 2020  ontest.name:.   
-00017160: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017170: 662e 636f 6e74 6573 742e 7061 7273 655f  f.contest.parse_
-00017180: 6578 6368 616e 6765 2873 656c 6629 0a20  exchange(self). 
-00017190: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000171a0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-000171b0: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
-000171c0: 662e 636f 6e74 6573 742c 2022 6164 7661  f.contest, "adva
-000171d0: 6e63 655f 6f6e 5f73 7061 6365 2229 3a0a  nce_on_space"):.
-000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171f0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
-00017200: 6164 7661 6e63 655f 6f6e 5f73 7061 6365  advance_on_space
-00017210: 5b33 5d3a 0a20 2020 2020 2020 2020 2020  [3]:.           
-00017220: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00017230: 7365 6c66 2e6f 7468 6572 5f32 2e74 6578  self.other_2.tex
-00017240: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00017250: 2020 2020 2020 2020 7465 7874 203d 2074          text = t
-00017260: 6578 742e 7570 7065 7228 290a 2020 2020  ext.upper().    
+00016e00: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00016e10: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
+00016e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e30: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+00016e40: 656e 6428 4661 6c73 6529 0a0a 2020 2020  end(False)..    
+00016e50: 6465 6620 6f74 6865 725f 325f 6368 616e  def other_2_chan
+00016e60: 6765 6428 7365 6c66 2920 2d3e 204e 6f6e  ged(self) -> Non
+00016e70: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00016e80: 2020 2020 2020 2054 6578 7420 696e 206f         Text in o
+00016e90: 7468 6572 5f32 2068 6173 2063 6861 6e67  ther_2 has chang
+00016ea0: 6564 2e0a 2020 2020 2020 2020 5374 7269  ed..        Stri
+00016eb0: 7020 6f75 7420 616e 7920 7370 6163 6573  p out any spaces
+00016ec0: 2061 6e64 2073 6574 2074 6865 2074 6578   and set the tex
+00016ed0: 742e 0a20 2020 2020 2020 2050 6172 7365  t..        Parse
+00016ee0: 2074 6865 2065 7863 6861 6e67 6520 6966   the exchange if
+00016ef0: 2074 6865 2063 6f6e 7465 7374 2069 7320   the contest is 
+00016f00: 4152 524c 2053 7765 6570 7374 616b 6573  ARRL Sweepstakes
+00016f10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00016f20: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00016f30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00016f40: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
+00016f50: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00016f60: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00016f70: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+00016f80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00016f90: 2e63 6f6e 7465 7374 3a0a 2020 2020 2020  .contest:.      
+00016fa0: 2020 2020 2020 6966 2022 4152 524c 2053        if "ARRL S
+00016fb0: 7765 6570 7374 616b 6573 2220 696e 2073  weepstakes" in s
+00016fc0: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
+00016fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016fe0: 2020 7365 6c66 2e63 6f6e 7465 7374 2e70    self.contest.p
+00016ff0: 6172 7365 5f65 7863 6861 6e67 6528 7365  arse_exchange(se
+00017000: 6c66 290a 2020 2020 2020 2020 2020 2020  lf).            
+00017010: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00017020: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+00017030: 7228 7365 6c66 2e63 6f6e 7465 7374 2c20  r(self.contest, 
+00017040: 2261 6476 616e 6365 5f6f 6e5f 7370 6163  "advance_on_spac
+00017050: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+00017060: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00017070: 7465 7374 2e61 6476 616e 6365 5f6f 6e5f  test.advance_on_
+00017080: 7370 6163 655b 335d 3a0a 2020 2020 2020  space[3]:.      
+00017090: 2020 2020 2020 2020 2020 2020 2020 7465                te
+000170a0: 7874 203d 2073 656c 662e 6f74 6865 725f  xt = self.other_
+000170b0: 322e 7465 7874 2829 0a20 2020 2020 2020  2.text().       
+000170c0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+000170d0: 7420 3d20 7465 7874 2e75 7070 6572 2829  t = text.upper()
+000170e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000170f0: 2020 2020 2023 2070 6f73 6974 696f 6e20       # position 
+00017100: 3d20 7365 6c66 2e6f 7468 6572 5f32 2e63  = self.other_2.c
+00017110: 7572 736f 7250 6f73 6974 696f 6e28 290a  ursorPosition().
+00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017130: 2020 2020 7374 7269 7070 6564 5f74 6578      stripped_tex
+00017140: 7420 3d20 7465 7874 2e73 7472 6970 2829  t = text.strip()
+00017150: 2e72 6570 6c61 6365 2822 2022 2c20 2222  .replace(" ", ""
+00017160: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017170: 2020 2020 2020 7365 6c66 2e6f 7468 6572        self.other
+00017180: 5f32 2e73 6574 5465 7874 2873 7472 6970  _2.setText(strip
+00017190: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
+000171a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000171b0: 7365 6c66 2e6f 7468 6572 5f32 2e73 6574  self.other_2.set
+000171c0: 4375 7273 6f72 506f 7369 7469 6f6e 2870  CursorPosition(p
+000171d0: 6f73 6974 696f 6e29 0a20 2020 2020 2020  osition).       
+000171e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000171f0: 2220 2220 696e 2074 6578 743a 0a20 2020  " " in text:.   
+00017200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017210: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
+00017220: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
+00017230: 7428 7365 6c66 2e6f 7468 6572 5f32 290a  t(self.other_2).
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+00017260: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
 00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017280: 2320 706f 7369 7469 6f6e 203d 2073 656c  # position = sel
-00017290: 662e 6f74 6865 725f 322e 6375 7273 6f72  f.other_2.cursor
-000172a0: 506f 7369 7469 6f6e 2829 0a20 2020 2020  Position().     
-000172b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000172c0: 7472 6970 7065 645f 7465 7874 203d 2074  tripped_text = t
-000172d0: 6578 742e 7374 7269 7028 292e 7265 706c  ext.strip().repl
-000172e0: 6163 6528 2220 222c 2022 2229 0a20 2020  ace(" ", "").   
-000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017300: 2073 656c 662e 6f74 6865 725f 322e 7365   self.other_2.se
-00017310: 7454 6578 7428 7374 7269 7070 6564 5f74  tText(stripped_t
-00017320: 6578 7429 0a20 2020 2020 2020 2020 2020  ext).           
-00017330: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00017340: 6f74 6865 725f 322e 7365 7443 7572 736f  other_2.setCurso
-00017350: 7250 6f73 6974 696f 6e28 706f 7369 7469  rPosition(positi
-00017360: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-00017370: 2020 2020 2020 2020 6966 2022 2022 2069          if " " i
-00017380: 6e20 7465 7874 3a0a 2020 2020 2020 2020  n text:.        
-00017390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173a0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
-000173b0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
-000173c0: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
-000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173e0: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
-000173f0: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-00017400: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017410: 6578 745f 7461 622e 6465 7365 6c65 6374  ext_tab.deselect
-00017420: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00017430: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00017440: 7461 622e 656e 6428 4661 6c73 6529 0a0a  tab.end(False)..
-00017450: 2020 2020 6465 6620 6361 6c6c 7369 676e      def callsign
-00017460: 5f63 6861 6e67 6564 2873 656c 6629 202d  _changed(self) -
-00017470: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00017480: 2222 220a 2020 2020 2020 2020 4361 6c6c  """.        Call
-00017490: 6564 2077 6865 6e20 7465 7874 2069 6e20  ed when text in 
-000174a0: 7468 6520 6361 6c6c 7369 676e 2066 6965  the callsign fie
-000174b0: 6c64 2068 6173 2063 6861 6e67 6564 2e0a  ld has changed..
-000174c0: 2020 2020 2020 2020 5374 7269 7020 6f75          Strip ou
-000174d0: 7420 616e 7920 7370 6163 6573 2061 6e64  t any spaces and
-000174e0: 2073 6574 2074 6865 2074 6578 742e 0a20   set the text.. 
-000174f0: 2020 2020 2020 2043 6865 636b 2069 6620         Check if 
-00017500: 7468 6520 6669 656c 6420 636f 6e74 6169  the field contai
-00017510: 6e73 2061 2063 6f6d 6d61 6e64 2e0a 0a20  ns a command... 
-00017520: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00017530: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00017540: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00017550: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
-00017560: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00017570: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00017580: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00017590: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
-000175a0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
-000175b0: 0a20 2020 2020 2020 2074 6578 7420 3d20  .        text = 
-000175c0: 7465 7874 2e75 7070 6572 2829 0a20 2020  text.upper().   
-000175d0: 2020 2020 2070 6f73 6974 696f 6e20 3d20       position = 
-000175e0: 7365 6c66 2e63 616c 6c73 6967 6e2e 6375  self.callsign.cu
-000175f0: 7273 6f72 506f 7369 7469 6f6e 2829 0a20  rsorPosition(). 
-00017600: 2020 2020 2020 2073 7472 6970 7065 645f         stripped_
-00017610: 7465 7874 203d 2074 6578 742e 7374 7269  text = text.stri
-00017620: 7028 292e 7265 706c 6163 6528 2220 222c  p().replace(" ",
-00017630: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-00017640: 662e 6361 6c6c 7369 676e 2e73 6574 5465  f.callsign.setTe
-00017650: 7874 2873 7472 6970 7065 645f 7465 7874  xt(stripped_text
-00017660: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00017670: 616c 6c73 6967 6e2e 7365 7443 7572 736f  allsign.setCurso
-00017680: 7250 6f73 6974 696f 6e28 706f 7369 7469  rPosition(positi
-00017690: 6f6e 290a 0a20 2020 2020 2020 2069 6620  on)..        if 
-000176a0: 2220 2220 696e 2074 6578 743a 0a20 2020  " " in text:.   
-000176b0: 2020 2020 2020 2020 2069 6620 7374 7269           if stri
-000176c0: 7070 6564 5f74 6578 7420 3d3d 2022 4357  pped_text == "CW
-000176d0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000176e0: 2020 2073 656c 662e 6368 616e 6765 5f6d     self.change_m
-000176f0: 6f64 6528 7374 7269 7070 6564 5f74 6578  ode(stripped_tex
-00017700: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00017710: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00017720: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
-00017730: 645f 7465 7874 203d 3d20 2252 5454 5922  d_text == "RTTY"
-00017740: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017750: 2020 7365 6c66 2e63 6861 6e67 655f 6d6f    self.change_mo
-00017760: 6465 2873 7472 6970 7065 645f 7465 7874  de(stripped_text
-00017770: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017780: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00017790: 2020 2020 2069 6620 7374 7269 7070 6564       if stripped
-000177a0: 5f74 6578 7420 3d3d 2022 5353 4222 3a0a  _text == "SSB":.
-000177b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177c0: 7365 6c66 2e63 6861 6e67 655f 6d6f 6465  self.change_mode
-000177d0: 2873 7472 6970 7065 645f 7465 7874 290a  (stripped_text).
-000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177f0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00017800: 2020 2069 6620 7374 7269 7070 6564 5f74     if stripped_t
-00017810: 6578 7420 3d3d 2022 4f50 4f4e 223a 0a20  ext == "OPON":. 
-00017820: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017830: 656c 662e 6765 745f 6f70 6f6e 2829 0a20  elf.get_opon(). 
-00017840: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017850: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
-00017860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017870: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00017880: 2020 2020 2069 6620 7374 7269 7070 6564       if stripped
-00017890: 5f74 6578 7420 3d3d 2022 4845 4c50 223a  _text == "HELP":
-000178a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000178b0: 2073 656c 662e 7368 6f77 5f68 656c 705f   self.show_help_
-000178c0: 6469 616c 6f67 2829 0a20 2020 2020 2020  dialog().       
-000178d0: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-000178e0: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-000178f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017900: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
-00017910: 6620 7374 7269 7070 6564 5f74 6578 7420  f stripped_text 
-00017920: 3d3d 2022 5445 5354 223a 0a20 2020 2020  == "TEST":.     
-00017930: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00017940: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
-00017950: 652e 6765 745f 6361 6c6c 735f 616e 645f  e.get_calls_and_
-00017960: 6261 6e64 7328 290a 2020 2020 2020 2020  bands().        
-00017970: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00017980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017990: 2063 6d64 5b22 636d 6422 5d20 3d20 2257   cmd["cmd"] = "W
-000179a0: 4f52 4b45 4422 0a20 2020 2020 2020 2020  ORKED".         
-000179b0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-000179c0: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-000179d0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-000179e0: 2020 2020 2020 2020 636d 645b 2277 6f72          cmd["wor
-000179f0: 6b65 6422 5d20 3d20 7265 7375 6c74 0a20  ked"] = result. 
-00017a00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017a10: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00017a20: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-00017a30: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-00017a40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00017a50: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-00017a60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00017a70: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00017a80: 6966 2073 656c 662e 6973 5f66 6c6f 6174  if self.is_float
-00017a90: 6162 6c65 2873 7472 6970 7065 645f 7465  able(stripped_te
-00017aa0: 7874 293a 0a20 2020 2020 2020 2020 2020  xt):.           
-00017ab0: 2020 2020 2073 656c 662e 6368 616e 6765       self.change
-00017ac0: 5f66 7265 7128 7374 7269 7070 6564 5f74  _freq(stripped_t
-00017ad0: 6578 7429 0a20 2020 2020 2020 2020 2020  ext).           
-00017ae0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00017af0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00017b00: 6563 6b5f 6361 6c6c 7369 676e 2873 7472  eck_callsign(str
-00017b10: 6970 7065 645f 7465 7874 290a 2020 2020  ipped_text).    
-00017b20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00017b30: 6368 6563 6b5f 6475 7065 2873 7472 6970  check_dupe(strip
-00017b40: 7065 645f 7465 7874 293a 0a20 2020 2020  ped_text):.     
-00017b50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017b60: 6475 7065 5f69 6e64 6963 6174 6f72 2e73  dupe_indicator.s
-00017b70: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
-00017b80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00017b90: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
-00017ba0: 655f 696e 6469 6361 746f 722e 6869 6465  e_indicator.hide
-00017bb0: 2829 0a20 2020 2020 2020 2020 2020 205f  ().            _
-00017bc0: 7468 6574 6872 6561 6420 3d20 7468 7265  thethread = thre
-00017bd0: 6164 696e 672e 5468 7265 6164 280a 2020  ading.Thread(.  
-00017be0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00017bf0: 7267 6574 3d73 656c 662e 6368 6563 6b5f  rget=self.check_
-00017c00: 6361 6c6c 7369 676e 322c 0a20 2020 2020  callsign2,.     
-00017c10: 2020 2020 2020 2020 2020 2061 7267 733d             args=
-00017c20: 2874 6578 742c 292c 0a20 2020 2020 2020  (text,),.       
-00017c30: 2020 2020 2020 2020 2064 6165 6d6f 6e3d           daemon=
-00017c40: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00017c50: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00017c60: 5f74 6865 7468 7265 6164 2e73 7461 7274  _thethread.start
-00017c70: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00017c80: 656c 662e 6e65 7874 5f66 6965 6c64 2e73  elf.next_field.s
-00017c90: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-00017ca0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00017cb0: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
-00017cc0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
-00017cd0: 203d 2022 4341 4c4c 4348 414e 4745 4422   = "CALLCHANGED"
-00017ce0: 0a20 2020 2020 2020 2063 6d64 5b22 7374  .        cmd["st
-00017cf0: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
-00017d00: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-00017d10: 2020 636d 645b 2263 616c 6c22 5d20 3d20    cmd["call"] = 
-00017d20: 7374 7269 7070 6564 5f74 6578 740a 2020  stripped_text.  
-00017d30: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00017d40: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00017d50: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-00017d60: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-00017d70: 6563 6b5f 6361 6c6c 7369 676e 2873 7472  eck_callsign(str
-00017d80: 6970 7065 645f 7465 7874 290a 0a20 2020  ipped_text)..   
-00017d90: 2064 6566 2063 6861 6e67 655f 6672 6571   def change_freq
-00017da0: 2873 656c 662c 2073 7472 6970 7065 645f  (self, stripped_
-00017db0: 7465 7874 3a20 7374 7229 202d 3e20 4e6f  text: str) -> No
-00017dc0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00017dd0: 2020 2020 2020 2020 4368 616e 6765 2056          Change V
-00017de0: 464f 2074 6f20 6769 7665 6e20 6672 6571  FO to given freq
-00017df0: 7565 6e63 7920 696e 204b 687a 2061 6e64  uency in Khz and
-00017e00: 2073 6574 2074 6865 2062 616e 6420 696e   set the band in
-00017e10: 6469 6361 746f 722e 0a20 2020 2020 2020  dicator..       
-00017e20: 2053 656e 6420 7468 6520 6e65 7720 6672   Send the new fr
-00017e30: 6571 7565 6e63 7920 746f 2074 6865 2072  equency to the r
-00017e40: 6967 2063 6f6e 7472 6f6c 2e0a 0a20 2020  ig control...   
-00017e50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00017e60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00017e70: 2d2d 0a20 2020 2020 2020 2073 7472 6970  --.        strip
-00017e80: 7065 645f 7465 7874 203a 2073 7472 0a20  ped_text : str. 
-00017e90: 2020 2020 2020 2053 7472 6970 7065 6420         Stripped 
-00017ea0: 6f66 2061 6e79 2073 7061 6365 732e 0a0a  of any spaces...
-00017eb0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00017ec0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00017ed0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-00017ee0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00017ef0: 2020 7666 6f20 3d20 666c 6f61 7428 7374    vfo = float(st
-00017f00: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
-00017f10: 2020 2020 2076 666f 203d 2069 6e74 2876       vfo = int(v
-00017f20: 666f 202a 2031 3030 3029 0a20 2020 2020  fo * 1000).     
-00017f30: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
-00017f40: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
-00017f50: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
-00017f60: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
-00017f70: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00017f80: 6164 696f 5f73 7461 7465 5b22 7666 6f61  adio_state["vfoa
-00017f90: 225d 203d 2076 666f 0a20 2020 2020 2020  "] = vfo.       
-00017fa0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00017fb0: 655b 2262 616e 6422 5d20 3d20 6261 6e64  e["band"] = band
-00017fc0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00017fd0: 6e74 6163 745b 2242 616e 6422 5d20 3d20  ntact["Band"] = 
-00017fe0: 6765 745f 6c6f 6767 6564 5f62 616e 6428  get_logged_band(
-00017ff0: 7374 7228 7666 6f29 290a 2020 2020 2020  str(vfo)).      
-00018000: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
-00018010: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
-00018020: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00018030: 7473 2829 0a20 2020 2020 2020 2069 6620  ts().        if 
-00018040: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00018050: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00018060: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
-00018070: 6574 5f76 666f 2876 666f 290a 2020 2020  et_vfo(vfo).    
-00018080: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00018090: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-000180a0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-000180b0: 225d 203d 2022 5241 4449 4f5f 5354 4154  "] = "RADIO_STAT
-000180c0: 4522 0a20 2020 2020 2020 2063 6d64 5b22  E".        cmd["
-000180d0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-000180e0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-000180f0: 2020 2020 636d 645b 2262 616e 6422 5d20      cmd["band"] 
-00018100: 3d20 6261 6e64 0a20 2020 2020 2020 2063  = band.        c
-00018110: 6d64 5b22 7666 6f61 225d 203d 2076 666f  md["vfoa"] = vfo
-00018120: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
-00018130: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00018140: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00018150: 6d64 290a 0a20 2020 2064 6566 2063 6861  md)..    def cha
-00018160: 6e67 655f 6d6f 6465 2873 656c 662c 206d  nge_mode(self, m
-00018170: 6f64 653a 2073 7472 2920 2d3e 204e 6f6e  ode: str) -> Non
-00018180: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00018190: 2020 2020 2020 2043 6861 6e67 6520 6d6f         Change mo
-000181a0: 6465 2074 6f20 6769 7665 6e20 6d6f 6465  de to given mode
-000181b0: 2e0a 2020 2020 2020 2020 5365 6e64 2074  ..        Send t
-000181c0: 6865 206e 6577 206d 6f64 6520 746f 2074  he new mode to t
-000181d0: 6865 2072 6967 2063 6f6e 7472 6f6c 2e0a  he rig control..
-000181e0: 2020 2020 2020 2020 5365 7420 7468 6520          Set the 
-000181f0: 6261 6e64 2069 6e64 6963 6174 6f72 2e0a  band indicator..
-00018200: 2020 2020 2020 2020 5365 7420 7468 6520          Set the 
-00018210: 7769 6e64 6f77 2074 6974 6c65 2e0a 2020  window title..  
-00018220: 2020 2020 2020 436c 6561 7220 7468 6520        Clear the 
-00018230: 696e 7075 7473 2e0a 2020 2020 2020 2020  inputs..        
-00018240: 5265 6164 2074 6865 2043 5720 6d61 6372  Read the CW macr
-00018250: 6f73 2e0a 0a20 2020 2020 2020 2050 6172  os...        Par
-00018260: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00018270: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00018280: 2020 206d 6f64 6520 3a20 7374 720a 2020     mode : str.  
-00018290: 2020 2020 2020 4d6f 6465 2074 6f20 6368        Mode to ch
-000182a0: 616e 6765 2074 6f2e 0a0a 2020 2020 2020  ange to...      
-000182b0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000182c0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000182d0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
-000182e0: 2222 0a0a 2020 2020 2020 2020 6966 206d  ""..        if m
-000182f0: 6f64 6520 3d3d 2022 4357 223a 0a20 2020  ode == "CW":.   
-00018300: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00018310: 746d 6f64 6528 2243 5722 290a 2020 2020  tmode("CW").    
-00018320: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00018330: 696f 5f73 7461 7465 5b22 6d6f 6465 225d  io_state["mode"]
-00018340: 203d 2022 4357 220a 2020 2020 2020 2020   = "CW".        
-00018350: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
-00018360: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
-00018370: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00018380: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
-00018390: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
-000183a0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-000183b0: 675f 636f 6e74 726f 6c2e 7365 745f 6d6f  g_control.set_mo
-000183c0: 6465 2822 4357 2229 0a20 2020 2020 2020  de("CW").       
-000183d0: 2020 2020 2062 616e 6420 3d20 6765 7462       band = getb
-000183e0: 616e 6428 7374 7228 7365 6c66 2e72 6164  and(str(self.rad
-000183f0: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-00018400: 6f61 222c 2022 302e 3022 2929 290a 2020  oa", "0.0"))).  
-00018410: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00018420: 6574 5f62 616e 645f 696e 6469 6361 746f  et_band_indicato
-00018430: 7228 6261 6e64 290a 2020 2020 2020 2020  r(band).        
-00018440: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
-00018450: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
-00018460: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-00018470: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
-00018480: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
-00018490: 5f63 775f 6d61 6372 6f73 2829 0a20 2020  _cw_macros().   
-000184a0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-000184b0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-000184c0: 3d3d 2022 5254 5459 223a 0a20 2020 2020  == "RTTY":.     
-000184d0: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-000184e0: 6f64 6528 2252 5454 5922 290a 2020 2020  ode("RTTY").    
-000184f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00018500: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-00018510: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018520: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00018530: 2e6f 6e6c 696e 653a 0a20 2020 2020 2020  .online:.       
-00018540: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018550: 662e 7269 675f 636f 6e74 726f 6c2e 7365  f.rig_control.se
-00018560: 745f 6d6f 6465 2822 5254 5459 2229 0a20  t_mode("RTTY"). 
-00018570: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00018580: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00018590: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-000185a0: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
-000185b0: 5d20 3d20 2252 5454 5922 0a20 2020 2020  ] = "RTTY".     
-000185c0: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
-000185d0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
-000185e0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-000185f0: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
-00018600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018610: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
-00018620: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
-00018630: 2020 2020 2020 7365 6c66 2e73 6574 5f77        self.set_w
-00018640: 696e 646f 775f 7469 746c 6528 290a 2020  indow_title().  
-00018650: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00018660: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-00018670: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00018680: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-00018690: 3d3d 2022 5353 4222 3a0a 2020 2020 2020  == "SSB":.      
-000186a0: 2020 2020 2020 7365 6c66 2e73 6574 6d6f        self.setmo
-000186b0: 6465 2822 5353 4222 290a 2020 2020 2020  de("SSB").      
-000186c0: 2020 2020 2020 6966 2069 6e74 2873 656c        if int(sel
-000186d0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-000186e0: 7428 2276 666f 6122 2c20 3029 2920 3e20  t("vfoa", 0)) > 
-000186f0: 3130 3030 3030 3030 3a0a 2020 2020 2020  10000000:.      
+00017280: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
+00017290: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172b0: 6e65 7874 5f74 6162 2e65 6e64 2846 616c  next_tab.end(Fal
+000172c0: 7365 290a 0a20 2020 2064 6566 2063 616c  se)..    def cal
+000172d0: 6c73 6967 6e5f 6368 616e 6765 6428 7365  lsign_changed(se
+000172e0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+000172f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00017300: 2043 616c 6c65 6420 7768 656e 2074 6578   Called when tex
+00017310: 7420 696e 2074 6865 2063 616c 6c73 6967  t in the callsig
+00017320: 6e20 6669 656c 6420 6861 7320 6368 616e  n field has chan
+00017330: 6765 642e 0a20 2020 2020 2020 2053 7472  ged..        Str
+00017340: 6970 206f 7574 2061 6e79 2073 7061 6365  ip out any space
+00017350: 7320 616e 6420 7365 7420 7468 6520 7465  s and set the te
+00017360: 7874 2e0a 2020 2020 2020 2020 4368 6563  xt..        Chec
+00017370: 6b20 6966 2074 6865 2066 6965 6c64 2063  k if the field c
+00017380: 6f6e 7461 696e 7320 6120 636f 6d6d 616e  ontains a comman
+00017390: 642e 0a0a 2020 2020 2020 2020 5061 7261  d...        Para
+000173a0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+000173b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+000173c0: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
+000173d0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000173e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000173f0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+00017400: 0a0a 2020 2020 2020 2020 7465 7874 203d  ..        text =
+00017410: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+00017420: 6578 7428 290a 2020 2020 2020 2020 7465  ext().        te
+00017430: 7874 203d 2074 6578 742e 7570 7065 7228  xt = text.upper(
+00017440: 290a 2020 2020 2020 2020 706f 7369 7469  ).        positi
+00017450: 6f6e 203d 2073 656c 662e 6361 6c6c 7369  on = self.callsi
+00017460: 676e 2e63 7572 736f 7250 6f73 6974 696f  gn.cursorPositio
+00017470: 6e28 290a 2020 2020 2020 2020 7374 7269  n().        stri
+00017480: 7070 6564 5f74 6578 7420 3d20 7465 7874  pped_text = text
+00017490: 2e73 7472 6970 2829 2e72 6570 6c61 6365  .strip().replace
+000174a0: 2822 2022 2c20 2222 290a 2020 2020 2020  (" ", "").      
+000174b0: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
+000174c0: 7365 7454 6578 7428 7374 7269 7070 6564  setText(stripped
+000174d0: 5f74 6578 7429 0a20 2020 2020 2020 2073  _text).        s
+000174e0: 656c 662e 6361 6c6c 7369 676e 2e73 6574  elf.callsign.set
+000174f0: 4375 7273 6f72 506f 7369 7469 6f6e 2870  CursorPosition(p
+00017500: 6f73 6974 696f 6e29 0a0a 2020 2020 2020  osition)..      
+00017510: 2020 6966 2022 2022 2069 6e20 7465 7874    if " " in text
+00017520: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00017530: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
+00017540: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+00017550: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+00017560: 6e67 655f 6d6f 6465 2873 7472 6970 7065  nge_mode(strippe
+00017570: 645f 7465 7874 290a 2020 2020 2020 2020  d_text).        
+00017580: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00017590: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+000175a0: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
+000175b0: 5254 5459 223a 0a20 2020 2020 2020 2020  RTTY":.         
+000175c0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+000175d0: 6765 5f6d 6f64 6528 7374 7269 7070 6564  ge_mode(stripped
+000175e0: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
+000175f0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00017600: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00017610: 6970 7065 645f 7465 7874 203d 3d20 2253  ipped_text == "S
+00017620: 5342 223a 0a20 2020 2020 2020 2020 2020  SB":.           
+00017630: 2020 2020 2073 656c 662e 6368 616e 6765       self.change
+00017640: 5f6d 6f64 6528 7374 7269 7070 6564 5f74  _mode(stripped_t
+00017650: 6578 7429 0a20 2020 2020 2020 2020 2020  ext).           
+00017660: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00017670: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
+00017680: 7065 645f 7465 7874 203d 3d20 224f 504f  ped_text == "OPO
+00017690: 4e22 3a0a 2020 2020 2020 2020 2020 2020  N":.            
+000176a0: 2020 2020 7365 6c66 2e67 6574 5f6f 706f      self.get_opo
+000176b0: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
+000176c0: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
+000176d0: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
+000176e0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000176f0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00017700: 6970 7065 645f 7465 7874 203d 3d20 2248  ipped_text == "H
+00017710: 454c 5022 3a0a 2020 2020 2020 2020 2020  ELP":.          
+00017720: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+00017730: 6865 6c70 5f64 6961 6c6f 6728 290a 2020  help_dialog().  
+00017740: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017750: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+00017760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017770: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00017780: 2020 2020 6966 2073 7472 6970 7065 645f      if stripped_
+00017790: 7465 7874 203d 3d20 2254 4553 5422 3a0a  text == "TEST":.
+000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177b0: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
+000177c0: 7461 6261 7365 2e67 6574 5f63 616c 6c73  tabase.get_calls
+000177d0: 5f61 6e64 5f62 616e 6473 2829 0a20 2020  _and_bands().   
+000177e0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+000177f0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00017800: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+00017810: 203d 2022 574f 524b 4544 220a 2020 2020   = "WORKED".    
+00017820: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00017830: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+00017840: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+00017850: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00017860: 5b22 776f 726b 6564 225d 203d 2072 6573  ["worked"] = res
+00017870: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
+00017880: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
+00017890: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
+000178a0: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
+000178b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000178c0: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
+000178d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000178e0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+000178f0: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+00017900: 666c 6f61 7461 626c 6528 7374 7269 7070  floatable(stripp
+00017910: 6564 5f74 6578 7429 3a0a 2020 2020 2020  ed_text):.      
+00017920: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00017930: 6861 6e67 655f 6672 6571 2873 7472 6970  hange_freq(strip
+00017940: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
+00017950: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017960: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00017970: 6c66 2e63 6865 636b 5f63 616c 6c73 6967  lf.check_callsig
+00017980: 6e28 7374 7269 7070 6564 5f74 6578 7429  n(stripped_text)
+00017990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000179a0: 7365 6c66 2e63 6865 636b 5f64 7570 6528  self.check_dupe(
+000179b0: 7374 7269 7070 6564 5f74 6578 7429 3a0a  stripped_text):.
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179d0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
+000179e0: 746f 722e 7368 6f77 2829 0a20 2020 2020  tor.show().     
+000179f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00017a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017a10: 662e 6475 7065 5f69 6e64 6963 6174 6f72  f.dupe_indicator
+00017a20: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+00017a30: 2020 2020 5f74 6865 7468 7265 6164 203d      _thethread =
+00017a40: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
+00017a50: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00017a60: 2020 2074 6172 6765 743d 7365 6c66 2e63     target=self.c
+00017a70: 6865 636b 5f63 616c 6c73 6967 6e32 2c0a  heck_callsign2,.
+00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a90: 6172 6773 3d28 7465 7874 2c29 2c0a 2020  args=(text,),.  
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00017ab0: 656d 6f6e 3d54 7275 652c 0a20 2020 2020  emon=True,.     
+00017ac0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00017ad0: 2020 2020 205f 7468 6574 6872 6561 642e       _thethread.
+00017ae0: 7374 6172 7428 290a 2020 2020 2020 2020  start().        
+00017af0: 2020 2020 7365 6c66 2e6e 6578 745f 6669      self.next_fi
+00017b00: 656c 642e 7365 7446 6f63 7573 2829 0a20  eld.setFocus(). 
+00017b10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017b20: 6e0a 2020 2020 2020 2020 636d 6420 3d20  n.        cmd = 
+00017b30: 7b7d 0a20 2020 2020 2020 2063 6d64 5b22  {}.        cmd["
+00017b40: 636d 6422 5d20 3d20 2243 414c 4c43 4841  cmd"] = "CALLCHA
+00017b50: 4e47 4544 220a 2020 2020 2020 2020 636d  NGED".        cm
+00017b60: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
+00017b70: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+00017b80: 2020 2020 2020 2063 6d64 5b22 6361 6c6c         cmd["call
+00017b90: 225d 203d 2073 7472 6970 7065 645f 7465  "] = stripped_te
+00017ba0: 7874 0a20 2020 2020 2020 2073 656c 662e  xt.        self.
+00017bb0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00017bc0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00017bd0: 2863 6d64 290a 2020 2020 2020 2020 7365  (cmd).        se
+00017be0: 6c66 2e63 6865 636b 5f63 616c 6c73 6967  lf.check_callsig
+00017bf0: 6e28 7374 7269 7070 6564 5f74 6578 7429  n(stripped_text)
+00017c00: 0a0a 2020 2020 6465 6620 6368 616e 6765  ..    def change
+00017c10: 5f66 7265 7128 7365 6c66 2c20 7374 7269  _freq(self, stri
+00017c20: 7070 6564 5f74 6578 743a 2073 7472 2920  pped_text: str) 
+00017c30: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00017c40: 2022 2222 0a20 2020 2020 2020 2043 6861   """.        Cha
+00017c50: 6e67 6520 5646 4f20 746f 2067 6976 656e  nge VFO to given
+00017c60: 2066 7265 7175 656e 6379 2069 6e20 4b68   frequency in Kh
+00017c70: 7a20 616e 6420 7365 7420 7468 6520 6261  z and set the ba
+00017c80: 6e64 2069 6e64 6963 6174 6f72 2e0a 2020  nd indicator..  
+00017c90: 2020 2020 2020 5365 6e64 2074 6865 206e        Send the n
+00017ca0: 6577 2066 7265 7175 656e 6379 2074 6f20  ew frequency to 
+00017cb0: 7468 6520 7269 6720 636f 6e74 726f 6c2e  the rig control.
+00017cc0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00017cd0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00017ce0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00017cf0: 7374 7269 7070 6564 5f74 6578 7420 3a20  stripped_text : 
+00017d00: 7374 720a 2020 2020 2020 2020 5374 7269  str.        Stri
+00017d10: 7070 6564 206f 6620 616e 7920 7370 6163  pped of any spac
+00017d20: 6573 2e0a 0a20 2020 2020 2020 2052 6574  es...        Ret
+00017d30: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00017d40: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+00017d50: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
+00017d60: 2020 2020 2020 2076 666f 203d 2066 6c6f         vfo = flo
+00017d70: 6174 2873 7472 6970 7065 645f 7465 7874  at(stripped_text
+00017d80: 290a 2020 2020 2020 2020 7666 6f20 3d20  ).        vfo = 
+00017d90: 696e 7428 7666 6f20 2a20 3130 3030 290a  int(vfo * 1000).
+00017da0: 2020 2020 2020 2020 6261 6e64 203d 2067          band = g
+00017db0: 6574 6261 6e64 2873 7472 2876 666f 2929  etband(str(vfo))
+00017dc0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00017dd0: 745f 6261 6e64 5f69 6e64 6963 6174 6f72  t_band_indicator
+00017de0: 2862 616e 6429 0a20 2020 2020 2020 2073  (band).        s
+00017df0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+00017e00: 2276 666f 6122 5d20 3d20 7666 6f0a 2020  "vfoa"] = vfo.  
+00017e10: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+00017e20: 5f73 7461 7465 5b22 6261 6e64 225d 203d  _state["band"] =
+00017e30: 2062 616e 640a 2020 2020 2020 2020 7365   band.        se
+00017e40: 6c66 2e63 6f6e 7461 6374 5b22 4261 6e64  lf.contact["Band
+00017e50: 225d 203d 2067 6574 5f6c 6f67 6765 645f  "] = get_logged_
+00017e60: 6261 6e64 2873 7472 2876 666f 2929 0a20  band(str(vfo)). 
+00017e70: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00017e80: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
+00017e90: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00017ea0: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00017eb0: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00017ec0: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
+00017ed0: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+00017ee0: 726f 6c2e 7365 745f 7666 6f28 7666 6f29  rol.set_vfo(vfo)
+00017ef0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00017f00: 7572 6e0a 2020 2020 2020 2020 636d 6420  urn.        cmd 
+00017f10: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
+00017f20: 5b22 636d 6422 5d20 3d20 2252 4144 494f  ["cmd"] = "RADIO
+00017f30: 5f53 5441 5445 220a 2020 2020 2020 2020  _STATE".        
+00017f40: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+00017f50: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00017f60: 0a20 2020 2020 2020 2063 6d64 5b22 6261  .        cmd["ba
+00017f70: 6e64 225d 203d 2062 616e 640a 2020 2020  nd"] = band.    
+00017f80: 2020 2020 636d 645b 2276 666f 6122 5d20      cmd["vfoa"] 
+00017f90: 3d20 7666 6f0a 2020 2020 2020 2020 7365  = vfo.        se
+00017fa0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+00017fb0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+00017fc0: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
+00017fd0: 6620 6368 616e 6765 5f6d 6f64 6528 7365  f change_mode(se
+00017fe0: 6c66 2c20 6d6f 6465 3a20 7374 7229 202d  lf, mode: str) -
+00017ff0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00018000: 2222 220a 2020 2020 2020 2020 4368 616e  """.        Chan
+00018010: 6765 206d 6f64 6520 746f 2067 6976 656e  ge mode to given
+00018020: 206d 6f64 652e 0a20 2020 2020 2020 2053   mode..        S
+00018030: 656e 6420 7468 6520 6e65 7720 6d6f 6465  end the new mode
+00018040: 2074 6f20 7468 6520 7269 6720 636f 6e74   to the rig cont
+00018050: 726f 6c2e 0a20 2020 2020 2020 2053 6574  rol..        Set
+00018060: 2074 6865 2062 616e 6420 696e 6469 6361   the band indica
+00018070: 746f 722e 0a20 2020 2020 2020 2053 6574  tor..        Set
+00018080: 2074 6865 2077 696e 646f 7720 7469 746c   the window titl
+00018090: 652e 0a20 2020 2020 2020 2043 6c65 6172  e..        Clear
+000180a0: 2074 6865 2069 6e70 7574 732e 0a20 2020   the inputs..   
+000180b0: 2020 2020 2052 6561 6420 7468 6520 4357       Read the CW
+000180c0: 206d 6163 726f 732e 0a0a 2020 2020 2020   macros...      
+000180d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000180e0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000180f0: 2020 2020 2020 2020 6d6f 6465 203a 2073          mode : s
+00018100: 7472 0a20 2020 2020 2020 204d 6f64 6520  tr.        Mode 
+00018110: 746f 2063 6861 6e67 6520 746f 2e0a 0a20  to change to... 
+00018120: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00018130: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00018140: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
+00018150: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00018160: 2069 6620 6d6f 6465 203d 3d20 2243 5722   if mode == "CW"
+00018170: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018180: 6c66 2e73 6574 6d6f 6465 2822 4357 2229  lf.setmode("CW")
+00018190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000181a0: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
+000181b0: 6f64 6522 5d20 3d20 2243 5722 0a20 2020  ode"] = "CW".   
+000181c0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000181d0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
+000181e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000181f0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00018200: 6c2e 6f6e 6c69 6e65 3a0a 2020 2020 2020  l.online:.      
+00018210: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018220: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+00018230: 6574 5f6d 6f64 6528 2243 5722 290a 2020  et_mode("CW").  
+00018240: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
+00018250: 2067 6574 6261 6e64 2873 7472 2873 656c   getband(str(sel
+00018260: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00018270: 7428 2276 666f 6122 2c20 2230 2e30 2229  t("vfoa", "0.0")
+00018280: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+00018290: 656c 662e 7365 745f 6261 6e64 5f69 6e64  elf.set_band_ind
+000182a0: 6963 6174 6f72 2862 616e 6429 0a20 2020  icator(band).   
+000182b0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000182c0: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
+000182d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000182e0: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
+000182f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018300: 2e72 6561 645f 6377 5f6d 6163 726f 7328  .read_cw_macros(
+00018310: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00018320: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00018330: 6d6f 6465 203d 3d20 2252 5454 5922 3a0a  mode == "RTTY":.
+00018340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018350: 2e73 6574 6d6f 6465 2822 5254 5459 2229  .setmode("RTTY")
+00018360: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00018370: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+00018380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018390: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+000183a0: 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a 2020  ntrol.online:.  
+000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183c0: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
+000183d0: 6f6c 2e73 6574 5f6d 6f64 6528 2252 5454  ol.set_mode("RTT
+000183e0: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
+000183f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018400: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018410: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00018420: 6d6f 6465 225d 203d 2022 5254 5459 220a  mode"] = "RTTY".
+00018430: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+00018440: 203d 2067 6574 6261 6e64 2873 7472 2873   = getband(str(s
+00018450: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00018460: 6765 7428 2276 666f 6122 2c20 2230 2e30  get("vfoa", "0.0
+00018470: 2229 2929 0a20 2020 2020 2020 2020 2020  "))).           
+00018480: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
+00018490: 6e64 6963 6174 6f72 2862 616e 6429 0a20  ndicator(band). 
+000184a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000184b0: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
+000184c0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+000184d0: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
+000184e0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000184f0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00018500: 6d6f 6465 203d 3d20 2253 5342 223a 0a20  mode == "SSB":. 
+00018510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018520: 7365 746d 6f64 6528 2253 5342 2229 0a20  setmode("SSB"). 
+00018530: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00018540: 7428 7365 6c66 2e72 6164 696f 5f73 7461  t(self.radio_sta
+00018550: 7465 2e67 6574 2822 7666 6f61 222c 2030  te.get("vfoa", 0
+00018560: 2929 203e 2031 3030 3030 3030 303a 0a20  )) > 10000000:. 
+00018570: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018580: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+00018590: 226d 6f64 6522 5d20 3d20 2255 5342 220a  "mode"] = "USB".
+000185a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000185b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000185c0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+000185d0: 7465 5b22 6d6f 6465 225d 203d 2022 4c53  te["mode"] = "LS
+000185e0: 4222 0a20 2020 2020 2020 2020 2020 2062  B".            b
+000185f0: 616e 6420 3d20 6765 7462 616e 6428 7374  and = getband(st
+00018600: 7228 7365 6c66 2e72 6164 696f 5f73 7461  r(self.radio_sta
+00018610: 7465 2e67 6574 2822 7666 6f61 222c 2022  te.get("vfoa", "
+00018620: 302e 3022 2929 290a 2020 2020 2020 2020  0.0"))).        
+00018630: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
+00018640: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
+00018650: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00018660: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
+00018670: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
+00018680: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00018690: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
+000186a0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+000186b0: 636f 6e74 726f 6c2e 7365 745f 6d6f 6465  control.set_mode
+000186c0: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
+000186d0: 652e 6765 7428 226d 6f64 6522 2929 0a20  e.get("mode")). 
+000186e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000186f0: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
 00018700: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00018710: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-00018720: 225d 203d 2022 5553 4222 0a20 2020 2020  "] = "USB".     
-00018730: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00018740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018750: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
-00018760: 6f64 6522 5d20 3d20 224c 5342 220a 2020  ode"] = "LSB".  
-00018770: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
-00018780: 2067 6574 6261 6e64 2873 7472 2873 656c   getband(str(sel
-00018790: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-000187a0: 7428 2276 666f 6122 2c20 2230 2e30 2229  t("vfoa", "0.0")
-000187b0: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-000187c0: 656c 662e 7365 745f 6261 6e64 5f69 6e64  elf.set_band_ind
-000187d0: 6963 6174 6f72 2862 616e 6429 0a20 2020  icator(band).   
-000187e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000187f0: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
-00018800: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00018810: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00018820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00018830: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-00018840: 6f6c 2e73 6574 5f6d 6f64 6528 7365 6c66  ol.set_mode(self
-00018850: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00018860: 2822 6d6f 6465 2229 290a 2020 2020 2020  ("mode")).      
-00018870: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00018880: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-00018890: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-000188a0: 775f 6d61 6372 6f73 2829 0a0a 2020 2020  w_macros()..    
-000188b0: 6465 6620 6368 6563 6b5f 6361 6c6c 7369  def check_callsi
-000188c0: 676e 2873 656c 662c 2063 616c 6c73 6967  gn(self, callsig
-000188d0: 6e29 202d 3e20 4e6f 6e65 3a0a 2020 2020  n) -> None:.    
-000188e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000188f0: 4368 6563 6b20 6361 6c6c 7369 676e 2061  Check callsign a
-00018900: 7320 6974 2773 2062 6569 6e67 2065 6e74  s it's being ent
-00018910: 6572 6564 2069 6e20 7468 6520 6269 675f  ered in the big_
-00018920: 6374 7920 696e 6465 782e 0a20 2020 2020  cty index..     
-00018930: 2020 2047 6574 2044 5820 656e 7469 7479     Get DX entity
-00018940: 2c20 4351 2c20 4954 5520 616e 6420 636f  , CQ, ITU and co
-00018950: 6e74 696e 656e 742e 0a20 2020 2020 2020  ntinent..       
-00018960: 2047 656f 6772 6170 6869 6320 696e 666f   Geographic info
-00018970: 726d 6174 696f 6e2e 2044 6973 7461 6e63  rmation. Distanc
-00018980: 6520 616e 6420 4865 6164 696e 672e 0a0a  e and Heading...
-00018990: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000189a0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000189b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6361  -----.        ca
-000189c0: 6c6c 7369 676e 203a 2073 7472 0a20 2020  llsign : str.   
-000189d0: 2020 2020 2043 616c 6c73 6967 6e20 746f       Callsign to
-000189e0: 2063 6865 636b 2e0a 0a20 2020 2020 2020   check...       
-000189f0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00018a00: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00018a10: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
-00018a20: 220a 0a20 2020 2020 2020 2072 6573 756c  "..        resul
-00018a30: 7420 3d20 7365 6c66 2e63 7479 5f6c 6f6f  t = self.cty_loo
-00018a40: 6b75 7028 6361 6c6c 7369 676e 290a 2020  kup(callsign).  
-00018a50: 2020 2020 2020 6465 6275 675f 7265 7375        debug_resu
-00018a60: 6c74 203d 2066 227b 7265 7375 6c74 7d22  lt = f"{result}"
-00018a70: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00018a80: 6465 6275 6728 2225 7322 2c20 6465 6275  debug("%s", debu
-00018a90: 675f 7265 7375 6c74 290a 2020 2020 2020  g_result).      
-00018aa0: 2020 6966 2072 6573 756c 743a 0a20 2020    if result:.   
-00018ab0: 2020 2020 2020 2020 2066 6f72 2061 2069           for a i
-00018ac0: 6e20 7265 7375 6c74 2e69 7465 6d73 2829  n result.items()
-00018ad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00018ae0: 2020 656e 7469 7479 203d 2061 5b31 5d2e    entity = a[1].
-00018af0: 6765 7428 2265 6e74 6974 7922 2c20 2222  get("entity", ""
-00018b00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00018b10: 2020 6371 203d 2061 5b31 5d2e 6765 7428    cq = a[1].get(
-00018b20: 2263 7122 2c20 2222 290a 2020 2020 2020  "cq", "").      
-00018b30: 2020 2020 2020 2020 2020 6974 7520 3d20            itu = 
-00018b40: 615b 315d 2e67 6574 2822 6974 7522 2c20  a[1].get("itu", 
-00018b50: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-00018b60: 2020 2020 636f 6e74 696e 656e 7420 3d20      continent = 
-00018b70: 615b 315d 2e67 6574 2822 636f 6e74 696e  a[1].get("contin
-00018b80: 656e 7422 290a 2020 2020 2020 2020 2020  ent").          
-00018b90: 2020 2020 2020 6c61 7420 3d20 666c 6f61        lat = floa
-00018ba0: 7428 615b 315d 2e67 6574 2822 6c61 7422  t(a[1].get("lat"
-00018bb0: 2c20 2230 2e30 2229 290a 2020 2020 2020  , "0.0")).      
-00018bc0: 2020 2020 2020 2020 2020 6c6f 6e20 3d20            lon = 
-00018bd0: 666c 6f61 7428 615b 315d 2e67 6574 2822  float(a[1].get("
-00018be0: 6c6f 6e67 222c 2022 302e 3022 2929 0a20  long", "0.0")). 
-00018bf0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00018c00: 6f6e 203d 206c 6f6e 202a 202d 3120 2023  on = lon * -1  #
-00018c10: 2063 7479 2e64 6174 2066 696c 6520 696e   cty.dat file in
-00018c20: 7665 7274 7320 6c6f 6e67 6974 7564 6573  verts longitudes
-00018c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c40: 2070 7269 6d61 7279 5f70 6678 203d 2061   primary_pfx = a
-00018c50: 5b31 5d2e 6765 7428 2270 7269 6d61 7279  [1].get("primary
-00018c60: 5f70 6678 222c 2022 2229 0a20 2020 2020  _pfx", "").     
-00018c70: 2020 2020 2020 2020 2020 2068 6561 6469             headi
-00018c80: 6e67 203d 2062 6561 7269 6e67 5f77 6974  ng = bearing_wit
-00018c90: 685f 6c61 746c 6f6e 2873 656c 662e 7374  h_latlon(self.st
-00018ca0: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
-00018cb0: 7175 6172 6522 292c 206c 6174 2c20 6c6f  quare"), lat, lo
-00018cc0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00018cd0: 2020 206b 696c 6f6d 6574 6572 7320 3d20     kilometers = 
-00018ce0: 6469 7374 616e 6365 5f77 6974 685f 6c61  distance_with_la
-00018cf0: 746c 6f6e 280a 2020 2020 2020 2020 2020  tlon(.          
-00018d00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00018d10: 7461 7469 6f6e 2e67 6574 2822 4772 6964  tation.get("Grid
-00018d20: 5371 7561 7265 2229 2c20 6c61 742c 206c  Square"), lat, l
-00018d30: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00018d40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00018d50: 2020 2020 2073 656c 662e 6865 6164 696e       self.headin
-00018d60: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
-00018d70: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
-00018d80: 2020 2020 2020 2020 6622 5265 6769 6f6e          f"Region
-00018d90: 616c 2048 6467 207b 6865 6164 696e 677d  al Hdg {heading}
-00018da0: c2b0 204c 5020 7b72 6563 6970 726f 636f  .. LP {reciproco
-00018db0: 6c28 6865 6164 696e 6729 7dc2 b020 2f20  l(heading)}.. / 
-00018dc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018dd0: 2020 2020 2020 6622 6469 7374 616e 6365        f"distance
-00018de0: 207b 696e 7428 6b69 6c6f 6d65 7465 7273   {int(kilometers
-00018df0: 2a30 2e36 3231 3337 3129 7d6d 6920 7b6b  *0.621371)}mi {k
-00018e00: 696c 6f6d 6574 6572 737d 6b6d 220a 2020  ilometers}km".  
-00018e10: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e30: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-00018e40: 756e 7472 7950 7265 6669 7822 5d20 3d20  untryPrefix"] = 
-00018e50: 7072 696d 6172 795f 7066 780a 2020 2020  primary_pfx.    
-00018e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018e70: 2e63 6f6e 7461 6374 5b22 5a4e 225d 203d  .contact["ZN"] =
-00018e80: 2069 6e74 2863 7129 0a20 2020 2020 2020   int(cq).       
-00018e90: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00018ea0: 2e63 6f6e 7465 7374 3a0a 2020 2020 2020  .contest:.      
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018ec0: 2073 656c 662e 636f 6e74 6573 742e 6e61   self.contest.na
-00018ed0: 6d65 203d 3d20 2249 4152 5520 4846 223a  me == "IARU HF":
-00018ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ef0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00018f00: 6e74 6163 745b 225a 4e22 5d20 3d20 696e  ntact["ZN"] = in
-00018f10: 7428 6974 7529 0a20 2020 2020 2020 2020  t(itu).         
-00018f20: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00018f30: 6163 745b 2243 6f6e 7469 6e65 6e74 225d  act["Continent"]
-00018f40: 203d 2063 6f6e 7469 6e65 6e74 0a20 2020   = continent.   
-00018f50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018f60: 662e 6478 5f65 6e74 6974 792e 7365 7454  f.dx_entity.setT
-00018f70: 6578 7428 0a20 2020 2020 2020 2020 2020  ext(.           
-00018f80: 2020 2020 2020 2020 2066 227b 7072 696d           f"{prim
-00018f90: 6172 795f 7066 787d 3a20 7b63 6f6e 7469  ary_pfx}: {conti
-00018fa0: 6e65 6e74 7d2f 7b65 6e74 6974 797d 2063  nent}/{entity} c
-00018fb0: 713a 7b63 717d 2069 7475 3a7b 6974 757d  q:{cq} itu:{itu}
-00018fc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018fd0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00018fe0: 2020 2020 6966 206c 656e 2863 616c 6c73      if len(calls
-00018ff0: 6967 6e29 203e 2032 3a0a 2020 2020 2020  ign) > 2:.      
-00019000: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00019010: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
-00019020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019030: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00019040: 6573 742e 7072 6566 696c 6c28 7365 6c66  est.prefill(self
-00019050: 290a 0a20 2020 2064 6566 2063 6865 636b  )..    def check
-00019060: 5f63 616c 6c73 6967 6e32 2873 656c 662c  _callsign2(self,
-00019070: 2063 616c 6c73 6967 6e29 202d 3e20 4e6f   callsign) -> No
-00019080: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00019090: 2020 2020 2020 2020 4368 6563 6b20 7468          Check th
-000190a0: 6520 6361 6c6c 7369 676e 2061 6674 6572  e callsign after
-000190b0: 2069 7420 6861 7320 6265 656e 2065 6e74   it has been ent
-000190c0: 6572 6564 2e0a 2020 2020 2020 2020 4c6f  ered..        Lo
-000190d0: 6f6b 2075 7020 7468 6520 6361 6c6c 7369  ok up the callsi
-000190e0: 676e 2069 6e20 7468 6520 6361 6c6c 7369  gn in the callsi
-000190f0: 676e 2064 6174 6162 6173 652e 0a20 2020  gn database..   
-00019100: 2020 2020 2047 6574 2074 6865 2067 7269       Get the gri
-00019110: 6420 7371 7561 7265 2061 6e64 2063 616c  d square and cal
-00019120: 6375 6c61 7465 2074 6865 2064 6973 7461  culate the dista
-00019130: 6e63 6520 616e 6420 6865 6164 696e 672e  nce and heading.
-00019140: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00019150: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00019160: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00019170: 6361 6c6c 7369 676e 203a 2073 7472 0a20  callsign : str. 
-00019180: 2020 2020 2020 2043 616c 6c73 6967 6e20         Callsign 
-00019190: 746f 2063 6865 636b 2e0a 0a20 2020 2020  to check...     
-000191a0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-000191b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-000191c0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-000191d0: 2222 220a 0a20 2020 2020 2020 2063 616c  """..        cal
-000191e0: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
-000191f0: 2e73 7472 6970 2829 0a20 2020 2020 2020  .strip().       
-00019200: 2064 6562 7567 5f6c 6f6f 6b75 7020 3d20   debug_lookup = 
-00019210: 6622 7b73 656c 662e 6c6f 6f6b 5f75 707d  f"{self.look_up}
-00019220: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-00019230: 2e64 6562 7567 2822 2573 2c20 2573 222c  .debug("%s, %s",
-00019240: 2063 616c 6c73 6967 6e2c 2064 6562 7567   callsign, debug
-00019250: 5f6c 6f6f 6b75 7029 0a20 2020 2020 2020  _lookup).       
-00019260: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
-00019270: 2e6c 6f6f 6b5f 7570 2c20 2273 6573 7369  .look_up, "sessi
-00019280: 6f6e 2229 3a0a 2020 2020 2020 2020 2020  on"):.          
-00019290: 2020 6966 2073 656c 662e 6c6f 6f6b 5f75    if self.look_u
-000192a0: 702e 7365 7373 696f 6e3a 0a20 2020 2020  p.session:.     
-000192b0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-000192c0: 6e73 6520 3d20 7365 6c66 2e6c 6f6f 6b5f  nse = self.look_
-000192d0: 7570 2e6c 6f6f 6b75 7028 6361 6c6c 7369  up.lookup(callsi
-000192e0: 676e 290a 2020 2020 2020 2020 2020 2020  gn).            
-000192f0: 2020 2020 6465 6275 675f 7265 7370 6f6e      debug_respon
-00019300: 7365 203d 2066 227b 7265 7370 6f6e 7365  se = f"{response
-00019310: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00019320: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00019330: 2254 6865 2052 6573 706f 6e73 653a 2025  "The Response: %
-00019340: 735c 6e22 2c20 6465 6275 675f 7265 7370  s\n", debug_resp
-00019350: 6f6e 7365 290a 2020 2020 2020 2020 2020  onse).          
-00019360: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
-00019370: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00019380: 2020 2020 2020 2074 6865 6972 6772 6964         theirgrid
-00019390: 203d 2072 6573 706f 6e73 652e 6765 7428   = response.get(
-000193a0: 2267 7269 6422 290a 2020 2020 2020 2020  "grid").        
-000193b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000193c0: 2e63 6f6e 7461 6374 5b22 4772 6964 5371  .contact["GridSq
-000193d0: 7561 7265 225d 203d 2074 6865 6972 6772  uare"] = theirgr
-000193e0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-000193f0: 2020 2020 2020 205f 7468 6569 7263 6f75         _theircou
-00019400: 6e74 7279 203d 2072 6573 706f 6e73 652e  ntry = response.
-00019410: 6765 7428 2263 6f75 6e74 7279 2229 0a20  get("country"). 
-00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019430: 2020 2069 6620 7365 6c66 2e73 7461 7469     if self.stati
-00019440: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
-00019450: 7265 222c 2022 2229 3a0a 2020 2020 2020  re", ""):.      
-00019460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019470: 2020 6865 6164 696e 6720 3d20 6265 6172    heading = bear
-00019480: 696e 6728 7365 6c66 2e73 7461 7469 6f6e  ing(self.station
-00019490: 2e67 6574 2822 4772 6964 5371 7561 7265  .get("GridSquare
-000194a0: 222c 2022 2229 2c20 7468 6569 7267 7269  ", ""), theirgri
-000194b0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-000194c0: 2020 2020 2020 2020 2020 206b 696c 6f6d             kilom
-000194d0: 6574 6572 7320 3d20 6469 7374 616e 6365  eters = distance
-000194e0: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-000194f0: 7428 2247 7269 6453 7175 6172 6522 292c  t("GridSquare"),
-00019500: 2074 6865 6972 6772 6964 290a 2020 2020   theirgrid).    
-00019510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019520: 2020 2020 7365 6c66 2e68 6561 6469 6e67      self.heading
-00019530: 5f64 6973 7461 6e63 652e 7365 7454 6578  _distance.setTex
-00019540: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00019550: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019560: 227b 7468 6569 7267 7269 647d 2048 6467  "{theirgrid} Hdg
-00019570: 207b 6865 6164 696e 677d c2b0 204c 5020   {heading}.. LP 
-00019580: 7b72 6563 6970 726f 636f 6c28 6865 6164  {reciprocol(head
-00019590: 696e 6729 7dc2 b020 2f20 220a 2020 2020  ing)}.. / ".    
-000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195b0: 2020 2020 2020 2020 6622 6469 7374 616e          f"distan
-000195c0: 6365 207b 696e 7428 6b69 6c6f 6d65 7465  ce {int(kilomete
-000195d0: 7273 2a30 2e36 3231 3337 3129 7d6d 6920  rs*0.621371)}mi 
-000195e0: 7b6b 696c 6f6d 6574 6572 737d 6b6d 220a  {kilometers}km".
-000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019600: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00019610: 6566 2063 6865 636b 5f64 7570 6528 7365  ef check_dupe(se
-00019620: 6c66 2c20 6361 6c6c 3a20 7374 7229 202d  lf, call: str) -
-00019630: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00019640: 2222 2243 6865 636b 7320 6966 2061 2063  """Checks if a c
-00019650: 616c 6c73 6967 6e20 6973 2061 2064 7570  allsign is a dup
-00019660: 6520 6f6e 2063 7572 7265 6e74 2062 616e  e on current ban
-00019670: 642f 6d6f 6465 2e22 2222 0a20 2020 2020  d/mode.""".     
-00019680: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00019690: 7374 2069 7320 4e6f 6e65 3a0a 2020 2020  st is None:.    
-000196a0: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-000196b0: 775f 6d65 7373 6167 655f 626f 7828 2259  w_message_box("Y
-000196c0: 6f75 2068 6176 6520 6e6f 2063 6f6e 7465  ou have no conte
-000196d0: 7374 206c 6f61 6465 642e 2229 0a20 2020  st loaded.").   
-000196e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000196f0: 4661 6c73 650a 2020 2020 2020 2020 7365  False.        se
-00019700: 6c66 2e63 6f6e 7465 7374 2e70 7265 6475  lf.contest.predu
-00019710: 7065 2873 656c 6629 0a20 2020 2020 2020  pe(self).       
-00019720: 2062 616e 6420 3d20 666c 6f61 7428 6765   band = float(ge
-00019730: 745f 6c6f 6767 6564 5f62 616e 6428 7374  t_logged_band(st
-00019740: 7228 7365 6c66 2e72 6164 696f 5f73 7461  r(self.radio_sta
-00019750: 7465 2e67 6574 2822 7666 6f61 222c 2030  te.get("vfoa", 0
-00019760: 2e30 2929 2929 0a20 2020 2020 2020 206d  .0)))).        m
-00019770: 6f64 6520 3d20 7365 6c66 2e72 6164 696f  ode = self.radio
-00019780: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-00019790: 222c 2022 2229 0a20 2020 2020 2020 2064  ", "").        d
-000197a0: 6562 7567 6c69 6e65 203d 2028 0a20 2020  ebugline = (.   
-000197b0: 2020 2020 2020 2020 2066 2243 616c 6c3a           f"Call:
-000197c0: 207b 6361 6c6c 7d20 4261 6e64 3a20 7b62   {call} Band: {b
-000197d0: 616e 647d 204d 6f64 653a 207b 6d6f 6465  and} Mode: {mode
-000197e0: 7d20 4475 7065 7479 7065 3a20 7b73 656c  } Dupetype: {sel
-000197f0: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
-00019800: 7970 657d 220a 2020 2020 2020 2020 290a  ype}".        ).
-00019810: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00019820: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
-00019830: 6c69 6e65 290a 2020 2020 2020 2020 6966  line).        if
-00019840: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
-00019850: 7065 5f74 7970 6520 3d3d 2031 3a0a 2020  pe_type == 1:.  
-00019860: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00019870: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00019880: 2e63 6865 636b 5f64 7570 6528 6361 6c6c  .check_dupe(call
-00019890: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000198a0: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
-000198b0: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
-000198c0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-000198d0: 656c 662e 6461 7461 6261 7365 2e63 6865  elf.database.che
-000198e0: 636b 5f64 7570 655f 6f6e 5f62 616e 6428  ck_dupe_on_band(
-000198f0: 6361 6c6c 2c20 6261 6e64 290a 2020 2020  call, band).    
-00019900: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-00019910: 6573 742e 6475 7065 5f74 7970 6520 3d3d  est.dupe_type ==
-00019920: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
-00019930: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
-00019940: 7461 6261 7365 2e63 6865 636b 5f64 7570  tabase.check_dup
-00019950: 655f 6f6e 5f62 616e 645f 6d6f 6465 2863  e_on_band_mode(c
-00019960: 616c 6c2c 2062 616e 642c 206d 6f64 6529  all, band, mode)
-00019970: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00019980: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
-00019990: 7065 203d 3d20 343a 0a20 2020 2020 2020  pe == 4:.       
-000199a0: 2020 2020 2072 6573 756c 7420 3d20 7b22       result = {"
-000199b0: 6973 6475 7065 223a 2046 616c 7365 7d0a  isdupe": False}.
-000199c0: 2020 2020 2020 2020 6465 6275 676c 696e          debuglin
-000199d0: 6520 3d20 6622 7b72 6573 756c 747d 220a  e = f"{result}".
-000199e0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-000199f0: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
-00019a00: 6c69 6e65 290a 2020 2020 2020 2020 7265  line).        re
-00019a10: 7475 726e 2072 6573 756c 742e 6765 7428  turn result.get(
-00019a20: 2269 7364 7570 6522 2c20 4661 6c73 6529  "isdupe", False)
-00019a30: 0a0a 2020 2020 6465 6620 7365 746d 6f64  ..    def setmod
-00019a40: 6528 7365 6c66 2c20 6d6f 6465 3a20 7374  e(self, mode: st
-00019a50: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-00019a60: 2020 2020 2222 2243 616c 6c20 7768 656e      """Call when
-00019a70: 2074 6865 206d 6f64 6520 6368 616e 6765   the mode change
-00019a80: 732e 2222 220a 2020 2020 2020 2020 6966  s.""".        if
-00019a90: 206d 6f64 6520 3d3d 2022 4357 223a 0a20   mode == "CW":. 
-00019aa0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00019ab0: 6c66 2e63 7572 7265 6e74 5f6d 6f64 6520  lf.current_mode 
-00019ac0: 213d 2022 4357 223a 0a20 2020 2020 2020  != "CW":.       
-00019ad0: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
-00019ae0: 7272 656e 745f 6d6f 6465 203d 2022 4357  rrent_mode = "CW
-00019af0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00019b00: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
-00019b10: 7454 6578 7428 2243 5722 290a 2020 2020  tText("CW").    
-00019b20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019b30: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
-00019b40: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
-00019b50: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
-00019b60: 652e 7365 7454 6578 7428 2235 3939 2229  e.setText("599")
-00019b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019b80: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-00019b90: 6372 6f73 2829 0a20 2020 2020 2020 2020  cros().         
-00019ba0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00019bb0: 2020 6966 206d 6f64 6520 3d3d 2022 5353    if mode == "SS
-00019bc0: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
-00019bd0: 6966 2073 656c 662e 6375 7272 656e 745f  if self.current_
-00019be0: 6d6f 6465 2021 3d20 2253 5342 223a 0a20  mode != "SSB":. 
-00019bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019c00: 656c 662e 6375 7272 656e 745f 6d6f 6465  elf.current_mode
-00019c10: 203d 2022 5353 4222 0a20 2020 2020 2020   = "SSB".       
-00019c20: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00019c30: 6d6f 6465 2e73 6574 5465 7874 2822 5353  mode.setText("SS
-00019c40: 4222 290a 2020 2020 2020 2020 2020 2020  B").            
-00019c50: 2020 2020 7365 6c66 2e73 656e 742e 7365      self.sent.se
-00019c60: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
-00019c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019c80: 2e72 6563 6569 7665 2e73 6574 5465 7874  .receive.setText
-00019c90: 2822 3539 2229 0a20 2020 2020 2020 2020  ("59").         
-00019ca0: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
-00019cb0: 5f63 775f 6d61 6372 6f73 2829 0a20 2020  _cw_macros().   
-00019cc0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00019cd0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-00019ce0: 3d3d 2022 5254 5459 223a 0a20 2020 2020  == "RTTY":.     
-00019cf0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00019d00: 7572 7265 6e74 5f6d 6f64 6520 213d 2022  urrent_mode != "
-00019d10: 5254 5459 223a 0a20 2020 2020 2020 2020  RTTY":.         
-00019d20: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
-00019d30: 656e 745f 6d6f 6465 203d 2022 5254 5459  ent_mode = "RTTY
-00019d40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00019d50: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
-00019d60: 7454 6578 7428 2252 5454 5922 290a 2020  tText("RTTY").  
-00019d70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019d80: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
-00019d90: 2235 3922 290a 2020 2020 2020 2020 2020  "59").          
-00019da0: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
-00019db0: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
-00019dc0: 0a0a 2020 2020 6465 6620 6765 745f 6f70  ..    def get_op
-00019dd0: 6f6e 2873 656c 6629 202d 3e20 4e6f 6e65  on(self) -> None
-00019de0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00019df0: 2020 2020 2020 4374 726c 2b4f 204f 7065        Ctrl+O Ope
-00019e00: 6e20 7468 6520 4f50 4f4e 2064 6961 6c6f  n the OPON dialo
-00019e10: 672e 0a0a 2020 2020 2020 2020 5061 7261  g...        Para
-00019e20: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00019e30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00019e40: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
-00019e50: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00019e60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00019e70: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00019e80: 0a0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-00019e90: 706f 6e5f 6469 616c 6f67 203d 204f 704f  pon_dialog = OpO
-00019ea0: 6e28 6673 7574 696c 732e 4150 505f 4441  n(fsutils.APP_DA
-00019eb0: 5441 5f50 4154 4829 0a0a 2020 2020 2020  TA_PATH)..      
-00019ec0: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
-00019ed0: 745f 7061 6c65 7474 653a 0a20 2020 2020  t_palette:.     
-00019ee0: 2020 2020 2020 2073 656c 662e 6f70 6f6e         self.opon
-00019ef0: 5f64 6961 6c6f 672e 7365 7450 616c 6574  _dialog.setPalet
-00019f00: 7465 2873 656c 662e 6375 7272 656e 745f  te(self.current_
-00019f10: 7061 6c65 7474 6529 0a0a 2020 2020 2020  palette)..      
-00019f20: 2020 7365 6c66 2e6f 706f 6e5f 6469 616c    self.opon_dial
-00019f30: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
-00019f40: 6563 7428 7365 6c66 2e6e 6577 5f6f 7029  ect(self.new_op)
-00019f50: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-00019f60: 6f6e 5f64 6961 6c6f 672e 6f70 656e 2829  on_dialog.open()
-00019f70: 0a0a 2020 2020 6465 6620 6e65 775f 6f70  ..    def new_op
-00019f80: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00019f90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00019fa0: 2020 2020 4361 6c6c 6564 2077 6865 6e20      Called when 
-00019fb0: 7468 6520 7573 6572 2063 6c69 636b 7320  the user clicks 
-00019fc0: 7468 6520 4f4b 2062 7574 746f 6e20 6f6e  the OK button on
-00019fd0: 2074 6865 204f 504f 4e20 6469 616c 6f67   the OPON dialog
-00019fe0: 2e0a 2020 2020 2020 2020 4372 6561 7465  ..        Create
-00019ff0: 2074 6865 206e 6577 2064 6972 6563 746f   the new directo
-0001a000: 7279 2061 6e64 2063 6f70 7920 7468 6520  ry and copy the 
-0001a010: 7068 6f6e 6574 6963 2066 696c 6573 2e0a  phonetic files..
-0001a020: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0001a030: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0001a040: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-0001a050: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
-0001a060: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0001a070: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-0001a080: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
-0001a090: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
-0001a0a0: 706f 6e5f 6469 616c 6f67 2e4e 6577 4f70  pon_dialog.NewOp
-0001a0b0: 6572 6174 6f72 2e74 6578 7428 293a 0a20  erator.text():. 
-0001a0c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a0d0: 6375 7272 656e 745f 6f70 203d 2073 656c  current_op = sel
-0001a0e0: 662e 6f70 6f6e 5f64 6961 6c6f 672e 4e65  f.opon_dialog.Ne
-0001a0f0: 774f 7065 7261 746f 722e 7465 7874 2829  wOperator.text()
-0001a100: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-0001a110: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
-0001a120: 672e 636c 6f73 6528 290a 2020 2020 2020  g.close().      
-0001a130: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0001a140: 4e65 7720 4f70 3a20 2573 222c 2073 656c  New Op: %s", sel
-0001a150: 662e 6375 7272 656e 745f 6f70 290a 2020  f.current_op).  
-0001a160: 2020 2020 2020 7365 6c66 2e6d 616b 655f        self.make_
-0001a170: 6f70 5f64 6972 2829 0a0a 2020 2020 6465  op_dir()..    de
-0001a180: 6620 6d61 6b65 5f6f 705f 6469 7228 7365  f make_op_dir(se
-0001a190: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0001a1a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001a1b0: 2043 7265 6174 6520 4f50 2064 6972 6563   Create OP direc
-0001a1c0: 746f 7279 2069 6620 6974 2064 6f65 7320  tory if it does 
-0001a1d0: 6e6f 7420 6578 6973 742e 0a20 2020 2020  not exist..     
-0001a1e0: 2020 2043 6f70 7920 7468 6520 7068 6f6e     Copy the phon
-0001a1f0: 6574 6963 2066 696c 6573 2074 6f20 7468  etic files to th
-0001a200: 6520 6e65 7720 6469 7265 6374 6f72 792e  e new directory.
-0001a210: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0001a220: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0001a230: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0001a240: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
-0001a250: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0001a260: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0001a270: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
-0001a280: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001a290: 6375 7272 656e 745f 6f70 3a0a 2020 2020  current_op:.    
-0001a2a0: 2020 2020 2020 2020 6f70 5f70 6174 6820          op_path 
-0001a2b0: 3d20 6673 7574 696c 732e 5553 4552 5f44  = fsutils.USER_D
-0001a2c0: 4154 415f 5041 5448 202f 2073 656c 662e  ATA_PATH / self.
-0001a2d0: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
-0001a2e0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0001a2f0: 6275 6728 226f 705f 7061 7468 3a20 2573  bug("op_path: %s
-0001a300: 222c 2073 7472 286f 705f 7061 7468 2929  ", str(op_path))
-0001a310: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a320: 6f70 5f70 6174 682e 6973 5f64 6972 2829  op_path.is_dir()
-0001a330: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
-0001a340: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0001a350: 722e 6465 6275 6728 2243 7265 6174 696e  r.debug("Creatin
-0001a360: 6720 4f70 2044 6972 6563 746f 7279 3a20  g Op Directory: 
-0001a370: 2573 222c 2073 7472 286f 705f 7061 7468  %s", str(op_path
-0001a380: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001a390: 2020 206f 732e 6d6b 6469 7228 7374 7228     os.mkdir(str(
-0001a3a0: 6f70 5f70 6174 6829 290a 2020 2020 2020  op_path)).      
-0001a3b0: 2020 2020 2020 6966 206f 705f 7061 7468        if op_path
-0001a3c0: 2e69 735f 6469 7228 293a 0a20 2020 2020  .is_dir():.     
-0001a3d0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0001a3e0: 655f 7061 7468 203d 2066 7375 7469 6c73  e_path = fsutils
-0001a3f0: 2e41 5050 5f44 4154 415f 5041 5448 202f  .APP_DATA_PATH /
-0001a400: 2022 7068 6f6e 6574 6963 7322 0a20 2020   "phonetics".   
-0001a410: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0001a420: 6765 722e 6465 6275 6728 2273 6f75 7263  ger.debug("sourc
-0001a430: 655f 7061 7468 3a20 2573 222c 2073 7472  e_path: %s", str
-0001a440: 2873 6f75 7263 655f 7061 7468 2929 0a20  (source_path)). 
-0001a450: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001a460: 6f72 2063 6869 6c64 2069 6e20 736f 7572  or child in sour
-0001a470: 6365 5f70 6174 682e 6974 6572 6469 7228  ce_path.iterdir(
-0001a480: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001a490: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-0001a4a0: 6f6e 5f66 696c 6520 3d20 6f70 5f70 6174  on_file = op_pat
-0001a4b0: 6820 2f20 6368 696c 642e 6e61 6d65 0a20  h / child.name. 
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4d0: 2020 2069 6620 6465 7374 696e 6174 696f     if destinatio
-0001a4e0: 6e5f 6669 6c65 2e69 735f 6669 6c65 2829  n_file.is_file()
-0001a4f0: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
-0001a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a510: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0001a520: 2244 6573 7469 6e61 7469 6f6e 3a20 2573  "Destination: %s
-0001a530: 222c 2073 7472 2864 6573 7469 6e61 7469  ", str(destinati
-0001a540: 6f6e 5f66 696c 6529 290a 2020 2020 2020  on_file)).      
-0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a560: 2020 6465 7374 696e 6174 696f 6e5f 6669    destination_fi
-0001a570: 6c65 2e77 7269 7465 5f62 7974 6573 2863  le.write_bytes(c
-0001a580: 6869 6c64 2e72 6561 645f 6279 7465 7328  hild.read_bytes(
-0001a590: 2929 0a0a 2020 2020 6465 6620 706f 6c6c  ))..    def poll
-0001a5a0: 5f72 6164 696f 2873 656c 6629 202d 3e20  _radio(self) -> 
-0001a5b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0001a5c0: 220a 2020 2020 2020 2020 506f 6c6c 2072  ".        Poll r
-0001a5d0: 6164 696f 2066 6f72 2056 464f 2c20 6d6f  adio for VFO, mo
-0001a5e0: 6465 2c20 6261 6e64 7769 6474 682e 0a20  de, bandwidth.. 
-0001a5f0: 2020 2020 2020 2053 656e 6420 7374 6174         Send stat
-0001a600: 6520 7669 6120 6d75 6c74 6963 6173 742e  e via multicast.
-0001a610: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0001a620: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0001a630: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0001a640: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
-0001a650: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0001a660: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0001a670: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
-0001a680: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0001a690: 5f72 6164 696f 5f69 636f 6e28 3029 0a20  _radio_icon(0). 
-0001a6a0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0001a6b0: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-0001a6c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001a6d0: 7269 675f 636f 6e74 726f 6c2e 6f6e 6c69  rig_control.onli
-0001a6e0: 6e65 2069 7320 4661 6c73 653a 0a20 2020  ne is False:.   
-0001a6f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001a700: 662e 7365 745f 7261 6469 6f5f 6963 6f6e  f.set_radio_icon
-0001a710: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
-0001a720: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-0001a730: 7472 6f6c 2e72 6569 6e69 7428 290a 2020  trol.reinit().  
-0001a740: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0001a750: 662e 7269 675f 636f 6e74 726f 6c2e 6f6e  f.rig_control.on
-0001a760: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
-0001a770: 2020 2020 2020 7365 6c66 2e73 6574 5f72        self.set_r
-0001a780: 6164 696f 5f69 636f 6e28 3229 0a20 2020  adio_icon(2).   
-0001a790: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-0001a7a0: 6f5f 6469 7274 7920 3d20 4661 6c73 650a  o_dirty = False.
-0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7c0: 7666 6f20 3d20 7365 6c66 2e72 6967 5f63  vfo = self.rig_c
-0001a7d0: 6f6e 7472 6f6c 2e67 6574 5f76 666f 2829  ontrol.get_vfo()
-0001a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a7f0: 206d 6f64 6520 3d20 7365 6c66 2e72 6967   mode = self.rig
-0001a800: 5f63 6f6e 7472 6f6c 2e67 6574 5f6d 6f64  _control.get_mod
-0001a810: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0001a820: 2020 2020 6277 203d 2073 656c 662e 7269      bw = self.ri
-0001a830: 675f 636f 6e74 726f 6c2e 6765 745f 6277  g_control.get_bw
-0001a840: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-0001a850: 2020 2020 6966 206d 6f64 6520 3d3d 2022      if mode == "
-0001a860: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
-0001a870: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0001a880: 746d 6f64 6528 6d6f 6465 290a 2020 2020  tmode(mode).    
-0001a890: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-0001a8a0: 6f64 6520 3d3d 2022 4c53 4222 206f 7220  ode == "LSB" or 
-0001a8b0: 6d6f 6465 203d 3d20 2255 5342 223a 0a20  mode == "USB":. 
-0001a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8d0: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
-0001a8e0: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
-0001a8f0: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
-0001a900: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
-0001a910: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001a920: 6c66 2e73 6574 6d6f 6465 2822 5254 5459  lf.setmode("RTTY
-0001a930: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-0001a940: 2020 2020 6966 2076 666f 203d 3d20 2222      if vfo == ""
-0001a950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a960: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0001a970: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a980: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0001a990: 2e67 6574 2822 7666 6f61 2229 2021 3d20  .get("vfoa") != 
-0001a9a0: 7666 6f3a 0a20 2020 2020 2020 2020 2020  vfo:.           
-0001a9b0: 2020 2020 2020 2020 2069 6e66 6f5f 6469           info_di
-0001a9c0: 7274 7920 3d20 5472 7565 0a20 2020 2020  rty = True.     
-0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a9e0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-0001a9f0: 2276 666f 6122 5d20 3d20 7666 6f0a 2020  "vfoa"] = vfo.  
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-0001aa10: 6e64 203d 2067 6574 6261 6e64 2873 7472  nd = getband(str
-0001aa20: 2876 666f 2929 0a20 2020 2020 2020 2020  (vfo)).         
-0001aa30: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0001aa40: 6f5f 7374 6174 655b 2262 616e 6422 5d20  o_state["band"] 
-0001aa50: 3d20 6261 6e64 0a20 2020 2020 2020 2020  = band.         
-0001aa60: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0001aa70: 6163 745b 2242 616e 6422 5d20 3d20 6765  act["Band"] = ge
-0001aa80: 745f 6c6f 6767 6564 5f62 616e 6428 7374  t_logged_band(st
-0001aa90: 7228 7666 6f29 290a 2020 2020 2020 2020  r(vfo)).        
-0001aaa0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0001aab0: 5f62 616e 645f 696e 6469 6361 746f 7228  _band_indicator(
-0001aac0: 6261 6e64 290a 0a20 2020 2020 2020 2020  band)..         
-0001aad0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0001aae0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0001aaf0: 6d6f 6465 2229 2021 3d20 6d6f 6465 3a0a  mode") != mode:.
-0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab10: 2020 2020 696e 666f 5f64 6972 7479 203d      info_dirty =
-0001ab20: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0001ab30: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0001ab40: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-0001ab50: 225d 203d 206d 6f64 650a 0a20 2020 2020  "] = mode..     
-0001ab60: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0001ab70: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0001ab80: 6574 2822 6277 2229 2021 3d20 6277 3a0a  et("bw") != bw:.
-0001ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aba0: 2020 2020 696e 666f 5f64 6972 7479 203d      info_dirty =
-0001abb0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0001abc0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0001abd0: 6164 696f 5f73 7461 7465 5b22 6277 225d  adio_state["bw"]
-0001abe0: 203d 2062 770a 0a20 2020 2020 2020 2020   = bw..         
-0001abf0: 2020 2020 2020 2069 6620 6461 7465 7469         if dateti
-0001ac00: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
-0001ac10: 2920 3e20 676c 6f62 616c 7328 295b 2270  ) > globals()["p
-0001ac20: 6f6c 6c5f 7469 6d65 225d 206f 7220 696e  oll_time"] or in
-0001ac30: 666f 5f64 6972 7479 3a0a 2020 2020 2020  fo_dirty:.      
-0001ac40: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0001ac50: 6767 6572 2e64 6562 7567 2822 5646 4f3a  gger.debug("VFO:
-0001ac60: 2025 7320 204d 4f44 453a 2025 7320 4257   %s  MODE: %s BW
-0001ac70: 3a20 2573 222c 2076 666f 2c20 6d6f 6465  : %s", vfo, mode
-0001ac80: 2c20 6277 290a 2020 2020 2020 2020 2020  , bw).          
-0001ac90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0001aca0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-0001acb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001acc0: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
-0001acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ace0: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-0001acf0: 2252 4144 494f 5f53 5441 5445 220a 2020  "RADIO_STATE".  
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad10: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-0001ad20: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-0001ad30: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0001ad40: 2020 2020 2020 2063 6d64 5b22 6261 6e64         cmd["band
-0001ad50: 225d 203d 2062 616e 640a 2020 2020 2020  "] = band.      
-0001ad60: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0001ad70: 645b 2276 666f 6122 5d20 3d20 7666 6f0a  d["vfoa"] = vfo.
-0001ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad90: 2020 2020 636d 645b 226d 6f64 6522 5d20      cmd["mode"] 
-0001ada0: 3d20 6d6f 6465 0a20 2020 2020 2020 2020  = mode.         
-0001adb0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-0001adc0: 6277 225d 203d 2062 770a 2020 2020 2020  bw"] = bw.      
-0001add0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001ade0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-0001adf0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-0001ae00: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
-0001ae10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001ae20: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
-0001ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae40: 2020 2069 6620 7365 6c66 2e6e 316d 6d2e     if self.n1mm.
-0001ae50: 7365 6e64 5f72 6164 696f 5f70 6163 6b65  send_radio_packe
-0001ae60: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-0001ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae80: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
-0001ae90: 696e 666f 5b22 4672 6571 225d 203d 2076  info["Freq"] = v
-0001aea0: 666f 5b3a 2d31 5d0a 2020 2020 2020 2020  fo[:-1].        
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aec0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0001aed0: 6469 6f5f 696e 666f 5b22 5458 4672 6571  dio_info["TXFreq
-0001aee0: 225d 203d 2076 666f 5b3a 2d31 5d0a 2020  "] = vfo[:-1].  
-0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af00: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001af10: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-0001af20: 4d6f 6465 225d 203d 206d 6f64 650a 2020  Mode"] = mode.  
-0001af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001af50: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-0001af60: 4f70 4361 6c6c 225d 203d 2073 656c 662e  OpCall"] = self.
-0001af70: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
-0001af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af90: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0001afa0: 2e72 6164 696f 5f69 6e66 6f5b 2249 7352  .radio_info["IsR
-0001afb0: 756e 6e69 6e67 225d 203d 2073 7472 280a  unning"] = str(.
-0001afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afe0: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
-0001aff0: 756e 5f73 7461 7465 222c 2046 616c 7365  un_state", False
-0001b000: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001b010: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b030: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001b040: 2e6e 316d 6d2e 7365 6e64 5f72 6164 696f  .n1mm.send_radio
-0001b050: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0001b060: 2020 2020 2020 2067 6c6f 6261 6c73 2829         globals()
-0001b070: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0001b080: 2020 2020 2020 2020 2020 2270 6f6c 6c5f            "poll_
-0001b090: 7469 6d65 220a 2020 2020 2020 2020 2020  time".          
-0001b0a0: 2020 2020 2020 2020 2020 5d20 3d20 6461            ] = da
-0001b0b0: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-0001b0c0: 6e6f 7728 2920 2b20 6461 7465 7469 6d65  now() + datetime
-0001b0d0: 2e74 696d 6564 656c 7461 2873 6563 6f6e  .timedelta(secon
-0001b0e0: 6473 3d31 3029 0a0a 2020 2020 6465 6620  ds=10)..    def 
-0001b0f0: 6564 6974 5f63 775f 6d61 6372 6f73 2873  edit_cw_macros(s
-0001b100: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0001b110: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001b120: 2020 4361 6c6c 7320 7468 6520 6465 6661    Calls the defa
-0001b130: 756c 7420 7465 7874 2065 6469 746f 7220  ult text editor 
-0001b140: 746f 2065 6469 7420 7468 6520 4357 206d  to edit the CW m
-0001b150: 6163 726f 2066 696c 652e 0a0a 2020 2020  acro file...    
-0001b160: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0001b170: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0001b180: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
-0001b190: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0001b1a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0001b1b0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-0001b1c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001b1d0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0001b1e0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0001b1f0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
-0001b200: 2020 2020 2020 6d61 6372 6f5f 6669 6c65        macro_file
-0001b210: 203d 2022 6377 6d61 6372 6f73 2e74 7874   = "cwmacros.txt
-0001b220: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-0001b230: 2020 2020 2020 2020 2020 2020 6d61 6372              macr
-0001b240: 6f5f 6669 6c65 203d 2022 7373 626d 6163  o_file = "ssbmac
-0001b250: 726f 732e 7478 7422 0a20 2020 2020 2020  ros.txt".       
-0001b260: 2069 6620 6e6f 7420 2866 7375 7469 6c73   if not (fsutils
-0001b270: 2e55 5345 525f 4441 5441 5f50 4154 4820  .USER_DATA_PATH 
-0001b280: 2f20 6d61 6372 6f5f 6669 6c65 292e 6578  / macro_file).ex
-0001b290: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
-0001b2a0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0001b2b0: 2822 7265 6164 5f63 775f 6d61 6372 6f73  ("read_cw_macros
-0001b2c0: 3a20 636f 7079 696e 6720 6465 6661 756c  : copying defaul
-0001b2d0: 7420 6d61 6372 6f20 6669 6c65 2e22 290a  t macro file.").
-0001b2e0: 2020 2020 2020 2020 2020 2020 636f 7079              copy
-0001b2f0: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
-0001b300: 2020 2020 2020 6673 7574 696c 732e 4150        fsutils.AP
-0001b310: 505f 4441 5441 5f50 4154 4820 2f20 6d61  P_DATA_PATH / ma
-0001b320: 6372 6f5f 6669 6c65 2c20 6673 7574 696c  cro_file, fsutil
-0001b330: 732e 5553 4552 5f44 4154 415f 5041 5448  s.USER_DATA_PATH
-0001b340: 202f 206d 6163 726f 5f66 696c 650a 2020   / macro_file.  
-0001b350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001b360: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0001b370: 2020 2020 2066 7375 7469 6c73 2e6f 7065       fsutils.ope
-0001b380: 6e46 696c 6557 6974 684f 5328 6673 7574  nFileWithOS(fsut
-0001b390: 696c 732e 5553 4552 5f44 4154 415f 5041  ils.USER_DATA_PA
-0001b3a0: 5448 202f 206d 6163 726f 5f66 696c 6529  TH / macro_file)
-0001b3b0: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-0001b3c0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0001b3d0: 6765 722e 6578 6365 7074 696f 6e28 0a20  ger.exception(. 
-0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001b3f0: 2243 6f75 6c64 206e 6f74 206f 7065 6e20  "Could not open 
-0001b400: 6669 6c65 207b 6673 7574 696c 732e 5553  file {fsutils.US
-0001b410: 4552 5f44 4154 415f 5041 5448 202f 206d  ER_DATA_PATH / m
-0001b420: 6163 726f 5f66 696c 657d 220a 2020 2020  acro_file}".    
-0001b430: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0001b440: 6566 2072 6561 645f 6377 5f6d 6163 726f  ef read_cw_macro
-0001b450: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-0001b460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001b470: 2020 2020 2052 6561 6473 2069 6e20 7468       Reads in th
-0001b480: 6520 4357 206d 6163 726f 732c 2066 6972  e CW macros, fir
-0001b490: 7374 7320 6974 2063 6865 636b 7320 746f  sts it checks to
-0001b4a0: 2073 6565 2069 6620 7468 6520 6669 6c65   see if the file
-0001b4b0: 2065 7869 7374 732e 2049 6620 6974 2064   exists. If it d
-0001b4c0: 6f65 7320 6e6f 742c 0a20 2020 2020 2020  oes not,.       
-0001b4d0: 2061 6e64 2074 6869 7320 6861 7320 6265   and this has be
-0001b4e0: 656e 2070 6163 6b61 6765 6420 7769 7468  en packaged with
-0001b4f0: 2070 7969 6e73 7461 6c6c 6572 2069 7420   pyinstaller it 
-0001b500: 7769 6c6c 2063 6f70 7920 7468 6520 6465  will copy the de
-0001b510: 6661 756c 7420 6669 6c65 2066 726f 6d20  fault file from 
-0001b520: 7468 650a 2020 2020 2020 2020 7465 6d70  the.        temp
-0001b530: 2064 6972 6563 746f 7279 2074 6869 7320   directory this 
-0001b540: 6973 2072 756e 6e69 6e67 2066 726f 6d2e  is running from.
-0001b550: 2e2e 2049 6e20 7468 656f 7279 2e0a 2020  .. In theory..  
-0001b560: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0001b570: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-0001b580: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0001b590: 2229 203d 3d20 2243 5722 3a0a 2020 2020  ") == "CW":.    
-0001b5a0: 2020 2020 2020 2020 6d61 6372 6f5f 6669          macro_fi
-0001b5b0: 6c65 203d 2022 6377 6d61 6372 6f73 2e74  le = "cwmacros.t
-0001b5c0: 7874 220a 2020 2020 2020 2020 656c 7365  xt".        else
-0001b5d0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-0001b5e0: 6372 6f5f 6669 6c65 203d 2022 7373 626d  cro_file = "ssbm
-0001b5f0: 6163 726f 732e 7478 7422 0a0a 2020 2020  acros.txt"..    
-0001b600: 2020 2020 6966 206e 6f74 2028 6673 7574      if not (fsut
-0001b610: 696c 732e 5553 4552 5f44 4154 415f 5041  ils.USER_DATA_PA
-0001b620: 5448 202f 206d 6163 726f 5f66 696c 6529  TH / macro_file)
-0001b630: 2e65 7869 7374 7328 293a 0a20 2020 2020  .exists():.     
-0001b640: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0001b650: 6275 6728 2272 6561 645f 6377 5f6d 6163  bug("read_cw_mac
-0001b660: 726f 733a 2063 6f70 7969 6e67 2064 6566  ros: copying def
-0001b670: 6175 6c74 206d 6163 726f 2066 696c 652e  ault macro file.
-0001b680: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
-0001b690: 6f70 7966 696c 6528 0a20 2020 2020 2020  opyfile(.       
-0001b6a0: 2020 2020 2020 2020 2066 7375 7469 6c73           fsutils
-0001b6b0: 2e41 5050 5f44 4154 415f 5041 5448 202f  .APP_DATA_PATH /
-0001b6c0: 206d 6163 726f 5f66 696c 652c 2066 7375   macro_file, fsu
-0001b6d0: 7469 6c73 2e55 5345 525f 4441 5441 5f50  tils.USER_DATA_P
-0001b6e0: 4154 4820 2f20 6d61 6372 6f5f 6669 6c65  ATH / macro_file
-0001b6f0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001b700: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-0001b710: 280a 2020 2020 2020 2020 2020 2020 6673  (.            fs
-0001b720: 7574 696c 732e 5553 4552 5f44 4154 415f  utils.USER_DATA_
-0001b730: 5041 5448 202f 206d 6163 726f 5f66 696c  PATH / macro_fil
-0001b740: 652c 2022 7222 2c20 656e 636f 6469 6e67  e, "r", encoding
-0001b750: 3d22 7574 662d 3822 0a20 2020 2020 2020  ="utf-8".       
-0001b760: 2029 2061 7320 6669 6c65 5f64 6573 6372   ) as file_descr
-0001b770: 6970 746f 723a 0a20 2020 2020 2020 2020  iptor:.         
-0001b780: 2020 2066 6f72 206c 696e 6520 696e 2066     for line in f
-0001b790: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
-0001b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7b0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0001b7c0: 2020 2020 2020 2020 206d 6f64 652c 2066           mode, f
-0001b7d0: 6b65 792c 2062 7574 746f 6e6e 616d 652c  key, buttonname,
-0001b7e0: 2063 7774 6578 7420 3d20 6c69 6e65 2e73   cwtext = line.s
-0001b7f0: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
-0001b800: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001b810: 206d 6f64 652e 7374 7269 7028 292e 7570   mode.strip().up
-0001b820: 7065 7228 2920 3d3d 2022 5222 2061 6e64  per() == "R" and
-0001b830: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0001b840: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
-0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b860: 2020 2020 2073 656c 662e 666b 6579 735b       self.fkeys[
-0001b870: 666b 6579 2e73 7472 6970 2829 5d20 3d20  fkey.strip()] = 
-0001b880: 2862 7574 746f 6e6e 616d 652e 7374 7269  (buttonname.stri
-0001b890: 7028 292c 2063 7774 6578 742e 7374 7269  p(), cwtext.stri
-0001b8a0: 7028 2929 0a20 2020 2020 2020 2020 2020  p()).           
-0001b8b0: 2020 2020 2020 2020 2069 6620 6d6f 6465           if mode
-0001b8c0: 2e73 7472 6970 2829 2e75 7070 6572 2829  .strip().upper()
-0001b8d0: 2021 3d20 2252 2220 616e 6420 6e6f 7420   != "R" and not 
-0001b8e0: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
-0001b8f0: 756e 5f73 7461 7465 2229 3a0a 2020 2020  un_state"):.    
-0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 7365 6c66 2e66 6b65 7973 5b66      self.fkeys[f
-0001b920: 6b65 792e 7374 7269 7028 295d 203d 2028  key.strip()] = (
-0001b930: 6275 7474 6f6e 6e61 6d65 2e73 7472 6970  buttonname.strip
-0001b940: 2829 2c20 6377 7465 7874 2e73 7472 6970  (), cwtext.strip
-0001b950: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-0001b960: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
-0001b970: 4572 726f 7220 6173 2065 7272 3a0a 2020  Error as err:.  
-0001b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b990: 2020 6c6f 6767 6572 2e69 6e66 6f28 2272    logger.info("r
-0001b9a0: 6561 645f 6377 5f6d 6163 726f 733a 2025  ead_cw_macros: %
-0001b9b0: 7322 2c20 6572 7229 0a20 2020 2020 2020  s", err).       
-0001b9c0: 206b 6579 7320 3d20 7365 6c66 2e66 6b65   keys = self.fke
-0001b9d0: 7973 2e6b 6579 7328 290a 2020 2020 2020  ys.keys().      
-0001b9e0: 2020 6966 2022 4631 2220 696e 206b 6579    if "F1" in key
-0001b9f0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-0001ba00: 656c 662e 4631 2e73 6574 5465 7874 2866  elf.F1.setText(f
-0001ba10: 2246 313a 207b 7365 6c66 2e66 6b65 7973  "F1: {self.fkeys
-0001ba20: 5b27 4631 275d 5b30 5d7d 2229 0a20 2020  ['F1'][0]}").   
-0001ba30: 2020 2020 2020 2020 2073 656c 662e 4631           self.F1
-0001ba40: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-0001ba50: 2e66 6b65 7973 5b22 4631 225d 5b31 5d29  .fkeys["F1"][1])
-0001ba60: 0a20 2020 2020 2020 2069 6620 2246 3222  .        if "F2"
-0001ba70: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
-0001ba80: 2020 2020 2020 7365 6c66 2e46 322e 7365        self.F2.se
-0001ba90: 7454 6578 7428 6622 4632 3a20 7b73 656c  tText(f"F2: {sel
-0001baa0: 662e 666b 6579 735b 2746 3227 5d5b 305d  f.fkeys['F2'][0]
-0001bab0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-0001bac0: 7365 6c66 2e46 322e 7365 7454 6f6f 6c54  self.F2.setToolT
-0001bad0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-0001bae0: 3222 5d5b 315d 290a 2020 2020 2020 2020  2"][1]).        
-0001baf0: 6966 2022 4633 2220 696e 206b 6579 733a  if "F3" in keys:
-0001bb00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001bb10: 662e 4633 2e73 6574 5465 7874 2866 2246  f.F3.setText(f"F
-0001bb20: 333a 207b 7365 6c66 2e66 6b65 7973 5b27  3: {self.fkeys['
-0001bb30: 4633 275d 5b30 5d7d 2229 0a20 2020 2020  F3'][0]}").     
-0001bb40: 2020 2020 2020 2073 656c 662e 4633 2e73         self.F3.s
-0001bb50: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-0001bb60: 6b65 7973 5b22 4633 225d 5b31 5d29 0a20  keys["F3"][1]). 
-0001bb70: 2020 2020 2020 2069 6620 2246 3422 2069         if "F4" i
-0001bb80: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-0001bb90: 2020 2020 7365 6c66 2e46 342e 7365 7454      self.F4.setT
-0001bba0: 6578 7428 6622 4634 3a20 7b73 656c 662e  ext(f"F4: {self.
-0001bbb0: 666b 6579 735b 2746 3427 5d5b 305d 7d22  fkeys['F4'][0]}"
-0001bbc0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0001bbd0: 6c66 2e46 342e 7365 7454 6f6f 6c54 6970  lf.F4.setToolTip
-0001bbe0: 2873 656c 662e 666b 6579 735b 2246 3422  (self.fkeys["F4"
-0001bbf0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-0001bc00: 2022 4635 2220 696e 206b 6579 733a 0a20   "F5" in keys:. 
-0001bc10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001bc20: 4635 2e73 6574 5465 7874 2866 2246 353a  F5.setText(f"F5:
-0001bc30: 207b 7365 6c66 2e66 6b65 7973 5b27 4635   {self.fkeys['F5
-0001bc40: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-0001bc50: 2020 2020 2073 656c 662e 4635 2e73 6574       self.F5.set
-0001bc60: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-0001bc70: 7973 5b22 4635 225d 5b31 5d29 0a20 2020  ys["F5"][1]).   
-0001bc80: 2020 2020 2069 6620 2246 3622 2069 6e20       if "F6" in 
-0001bc90: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-0001bca0: 2020 7365 6c66 2e46 362e 7365 7454 6578    self.F6.setTex
-0001bcb0: 7428 6622 4636 3a20 7b73 656c 662e 666b  t(f"F6: {self.fk
-0001bcc0: 6579 735b 2746 3627 5d5b 305d 7d22 290a  eys['F6'][0]}").
-0001bcd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001bce0: 2e46 362e 7365 7454 6f6f 6c54 6970 2873  .F6.setToolTip(s
-0001bcf0: 656c 662e 666b 6579 735b 2246 3622 5d5b  elf.fkeys["F6"][
-0001bd00: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-0001bd10: 4637 2220 696e 206b 6579 733a 0a20 2020  F7" in keys:.   
-0001bd20: 2020 2020 2020 2020 2073 656c 662e 4637           self.F7
-0001bd30: 2e73 6574 5465 7874 2866 2246 373a 207b  .setText(f"F7: {
-0001bd40: 7365 6c66 2e66 6b65 7973 5b27 4637 275d  self.fkeys['F7']
-0001bd50: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-0001bd60: 2020 2073 656c 662e 4637 2e73 6574 546f     self.F7.setTo
-0001bd70: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-0001bd80: 5b22 4637 225d 5b31 5d29 0a20 2020 2020  ["F7"][1]).     
-0001bd90: 2020 2069 6620 2246 3822 2069 6e20 6b65     if "F8" in ke
-0001bda0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-0001bdb0: 7365 6c66 2e46 382e 7365 7454 6578 7428  self.F8.setText(
-0001bdc0: 6622 4638 3a20 7b73 656c 662e 666b 6579  f"F8: {self.fkey
-0001bdd0: 735b 2746 3827 5d5b 305d 7d22 290a 2020  s['F8'][0]}").  
-0001bde0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-0001bdf0: 382e 7365 7454 6f6f 6c54 6970 2873 656c  8.setToolTip(sel
-0001be00: 662e 666b 6579 735b 2246 3822 5d5b 315d  f.fkeys["F8"][1]
-0001be10: 290a 2020 2020 2020 2020 6966 2022 4639  ).        if "F9
-0001be20: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-0001be30: 2020 2020 2020 2073 656c 662e 4639 2e73         self.F9.s
-0001be40: 6574 5465 7874 2866 2246 393a 207b 7365  etText(f"F9: {se
-0001be50: 6c66 2e66 6b65 7973 5b27 4639 275d 5b30  lf.fkeys['F9'][0
-0001be60: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-0001be70: 2073 656c 662e 4639 2e73 6574 546f 6f6c   self.F9.setTool
-0001be80: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
-0001be90: 4639 225d 5b31 5d29 0a20 2020 2020 2020  F9"][1]).       
-0001bea0: 2069 6620 2246 3130 2220 696e 206b 6579   if "F10" in key
-0001beb0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-0001bec0: 656c 662e 4631 302e 7365 7454 6578 7428  elf.F10.setText(
-0001bed0: 6622 4631 303a 207b 7365 6c66 2e66 6b65  f"F10: {self.fke
-0001bee0: 7973 5b27 4631 3027 5d5b 305d 7d22 290a  ys['F10'][0]}").
-0001bef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001bf00: 2e46 3130 2e73 6574 546f 6f6c 5469 7028  .F10.setToolTip(
-0001bf10: 7365 6c66 2e66 6b65 7973 5b22 4631 3022  self.fkeys["F10"
-0001bf20: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-0001bf30: 2022 4631 3122 2069 6e20 6b65 7973 3a0a   "F11" in keys:.
-0001bf40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001bf50: 2e46 3131 2e73 6574 5465 7874 2866 2246  .F11.setText(f"F
-0001bf60: 3131 3a20 7b73 656c 662e 666b 6579 735b  11: {self.fkeys[
-0001bf70: 2746 3131 275d 5b30 5d7d 2229 0a20 2020  'F11'][0]}").   
-0001bf80: 2020 2020 2020 2020 2073 656c 662e 4631           self.F1
-0001bf90: 312e 7365 7454 6f6f 6c54 6970 2873 656c  1.setToolTip(sel
-0001bfa0: 662e 666b 6579 735b 2246 3131 225d 5b31  f.fkeys["F11"][1
-0001bfb0: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
-0001bfc0: 3132 2220 696e 206b 6579 733a 0a20 2020  12" in keys:.   
-0001bfd0: 2020 2020 2020 2020 2073 656c 662e 4631           self.F1
-0001bfe0: 322e 7365 7454 6578 7428 6622 4631 323a  2.setText(f"F12:
-0001bff0: 207b 7365 6c66 2e66 6b65 7973 5b27 4631   {self.fkeys['F1
-0001c000: 3227 5d5b 305d 7d22 290a 2020 2020 2020  2'][0]}").      
-0001c010: 2020 2020 2020 7365 6c66 2e46 3132 2e73        self.F12.s
-0001c020: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-0001c030: 6b65 7973 5b22 4631 3222 5d5b 315d 290a  keys["F12"][1]).
-0001c040: 0a20 2020 2064 6566 2067 656e 6572 6174  .    def generat
-0001c050: 655f 6164 6966 2873 656c 6629 202d 3e20  e_adif(self) -> 
-0001c060: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0001c070: 220a 2020 2020 2020 2020 4361 6c6c 7320  ".        Calls 
-0001c080: 7468 6520 636f 6e74 6573 7420 4144 4946  the contest ADIF
-0001c090: 2066 696c 6520 6765 6e65 7261 746f 722e   file generator.
-0001c0a0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0001c0b0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0001c0c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0001c0d0: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
-0001c0e0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0001c0f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0001c100: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
-0001c110: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
-0001c120: 2f2f 7777 772e 6164 6966 2e6f 7267 2f33  //www.adif.org/3
-0001c130: 3135 2f41 4449 465f 3331 352e 6874 6d0a  15/ADIF_315.htm.
-0001c140: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0001c150: 6562 7567 2822 2a2a 2a2a 2a2a 4144 4946  ebug("******ADIF
-0001c160: 2a2a 2a2a 2a22 290a 2020 2020 2020 2020  *****").        
-0001c170: 7365 6c66 2e63 6f6e 7465 7374 2e61 6469  self.contest.adi
-0001c180: 6628 7365 6c66 290a 0a20 2020 2064 6566  f(self)..    def
-0001c190: 2067 656e 6572 6174 655f 6361 6272 696c   generate_cabril
-0001c1a0: 6c6f 2873 656c 6629 202d 3e20 4e6f 6e65  lo(self) -> None
-0001c1b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0001c1c0: 2020 2020 2020 4361 6c6c 7320 7468 6520        Calls the 
-0001c1d0: 636f 6e74 6573 7420 4361 6272 696c 6c6f  contest Cabrillo
-0001c1e0: 2066 696c 6520 6765 6e65 7261 746f 722e   file generator.
-0001c1f0: 204d 6179 6265 2e0a 0a20 2020 2020 2020   Maybe...       
-0001c200: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0001c210: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0001c220: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-0001c230: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0001c240: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0001c250: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-0001c260: 2020 2222 220a 0a20 2020 2020 2020 206c    """..        l
-0001c270: 6f67 6765 722e 6465 6275 6728 222a 2a2a  ogger.debug("***
-0001c280: 2a2a 2a43 6162 7269 6c6c 6f2a 2a2a 2a2a  ***Cabrillo*****
-0001c290: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0001c2a0: 636f 6e74 6573 742e 6361 6272 696c 6c6f  contest.cabrillo
-0001c2b0: 2873 656c 6629 0a0a 0a64 6566 206c 6f61  (self)...def loa
-0001c2c0: 645f 666f 6e74 735f 6672 6f6d 5f64 6972  d_fonts_from_dir
-0001c2d0: 2864 6972 6563 746f 7279 3a20 7374 7229  (directory: str)
-0001c2e0: 202d 3e20 7365 743a 0a20 2020 2022 2222   -> set:.    """
-0001c2f0: 0a20 2020 2057 656c 6c20 6974 206c 6f61  .    Well it loa
-0001c300: 6473 2066 6f6e 7473 2066 726f 6d20 6120  ds fonts from a 
-0001c310: 6469 7265 6374 6f72 792e 2e2e 0a0a 2020  directory.....  
-0001c320: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001c330: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001c340: 6469 7265 6374 6f72 7920 3a20 7374 720a  directory : str.
-0001c350: 2020 2020 5468 6520 6469 7265 6374 6f72      The director
-0001c360: 7920 746f 206c 6f61 6420 666f 6e74 7320  y to load fonts 
-0001c370: 6672 6f6d 2e0a 0a20 2020 2052 6574 7572  from...    Retur
-0001c380: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0001c390: 2020 2073 6574 0a20 2020 2041 2073 6574     set.    A set
-0001c3a0: 206f 6620 666f 6e74 2066 616d 696c 6965   of font familie
-0001c3b0: 7320 696e 7374 616c 6c65 6420 696e 2074  s installed in t
-0001c3c0: 6865 2064 6972 6563 746f 7279 2e0a 2020  he directory..  
-0001c3d0: 2020 2222 220a 2020 2020 666f 6e74 5f66    """.    font_f
-0001c3e0: 616d 696c 6965 7320 3d20 7365 7428 290a  amilies = set().
-0001c3f0: 2020 2020 666f 7220 5f66 6920 696e 2051      for _fi in Q
-0001c400: 4469 7228 6469 7265 6374 6f72 7929 2e65  Dir(directory).e
-0001c410: 6e74 7279 496e 666f 4c69 7374 285b 222a  ntryInfoList(["*
-0001c420: 2e74 7466 222c 2022 2a2e 776f 6666 222c  .ttf", "*.woff",
-0001c430: 2022 2a2e 776f 6666 3222 5d29 3a0a 2020   "*.woff2"]):.  
-0001c440: 2020 2020 2020 5f69 6420 3d20 5146 6f6e        _id = QFon
-0001c450: 7444 6174 6162 6173 652e 6164 6441 7070  tDatabase.addApp
-0001c460: 6c69 6361 7469 6f6e 466f 6e74 285f 6669  licationFont(_fi
-0001c470: 2e61 6273 6f6c 7574 6546 696c 6550 6174  .absoluteFilePat
-0001c480: 6828 2929 0a20 2020 2020 2020 2066 6f6e  h()).        fon
-0001c490: 745f 6661 6d69 6c69 6573 207c 3d20 7365  t_families |= se
-0001c4a0: 7428 5146 6f6e 7444 6174 6162 6173 652e  t(QFontDatabase.
-0001c4b0: 6170 706c 6963 6174 696f 6e46 6f6e 7446  applicationFontF
-0001c4c0: 616d 696c 6965 7328 5f69 6429 290a 2020  amilies(_id)).  
-0001c4d0: 2020 7265 7475 726e 2066 6f6e 745f 6661    return font_fa
-0001c4e0: 6d69 6c69 6573 0a0a 0a64 6566 2069 6e73  milies...def ins
-0001c4f0: 7461 6c6c 5f69 636f 6e73 2829 202d 3e20  tall_icons() -> 
-0001c500: 4e6f 6e65 3a0a 2020 2020 2222 2249 6e73  None:.    """Ins
-0001c510: 7461 6c6c 2069 636f 6e73 2222 220a 0a20  tall icons""".. 
-0001c520: 2020 2069 6620 7379 732e 706c 6174 666f     if sys.platfo
-0001c530: 726d 203d 3d20 226c 696e 7578 223a 0a20  rm == "linux":. 
-0001c540: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
-0001c550: 280a 2020 2020 2020 2020 2020 2020 2278  (.            "x
-0001c560: 6467 2d69 636f 6e2d 7265 736f 7572 6365  dg-icon-resource
-0001c570: 2069 6e73 7461 6c6c 202d 2d73 697a 6520   install --size 
-0001c580: 3332 202d 2d63 6f6e 7465 7874 2061 7070  32 --context app
-0001c590: 7320 2d2d 6d6f 6465 2075 7365 7220 220a  s --mode user ".
-0001c5a0: 2020 2020 2020 2020 2020 2020 6622 7b66              f"{f
-0001c5b0: 7375 7469 6c73 2e4d 4f44 554c 455f 5041  sutils.MODULE_PA
-0001c5c0: 5448 7d2f 6461 7461 2f6b 3667 7465 2e6e  TH}/data/k6gte.n
-0001c5d0: 6f74 316d 6d2d 3332 2e70 6e67 206b 3667  ot1mm-32.png k6g
-0001c5e0: 7465 2d6e 6f74 316d 6d22 0a20 2020 2020  te-not1mm".     
-0001c5f0: 2020 2029 0a20 2020 2020 2020 206f 732e     ).        os.
-0001c600: 7379 7374 656d 280a 2020 2020 2020 2020  system(.        
-0001c610: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
-0001c620: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
-0001c630: 2d73 697a 6520 3634 202d 2d63 6f6e 7465  -size 64 --conte
-0001c640: 7874 2061 7070 7320 2d2d 6d6f 6465 2075  xt apps --mode u
-0001c650: 7365 7220 220a 2020 2020 2020 2020 2020  ser ".          
-0001c660: 2020 6622 7b66 7375 7469 6c73 2e4d 4f44    f"{fsutils.MOD
-0001c670: 554c 455f 5041 5448 7d2f 6461 7461 2f6b  ULE_PATH}/data/k
-0001c680: 3667 7465 2e6e 6f74 316d 6d2d 3634 2e70  6gte.not1mm-64.p
-0001c690: 6e67 206b 3667 7465 2d6e 6f74 316d 6d22  ng k6gte-not1mm"
-0001c6a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001c6b0: 2020 206f 732e 7379 7374 656d 280a 2020     os.system(.  
-0001c6c0: 2020 2020 2020 2020 2020 2278 6467 2d69            "xdg-i
-0001c6d0: 636f 6e2d 7265 736f 7572 6365 2069 6e73  con-resource ins
-0001c6e0: 7461 6c6c 202d 2d73 697a 6520 3132 3820  tall --size 128 
-0001c6f0: 2d2d 636f 6e74 6578 7420 6170 7073 202d  --context apps -
-0001c700: 2d6d 6f64 6520 7573 6572 2022 0a20 2020  -mode user ".   
-0001c710: 2020 2020 2020 2020 2066 227b 6673 7574           f"{fsut
-0001c720: 696c 732e 4d4f 4455 4c45 5f50 4154 487d  ils.MODULE_PATH}
-0001c730: 2f64 6174 612f 6b36 6774 652e 6e6f 7431  /data/k6gte.not1
-0001c740: 6d6d 2d31 3238 2e70 6e67 206b 3667 7465  mm-128.png k6gte
-0001c750: 2d6e 6f74 316d 6d22 0a20 2020 2020 2020  -not1mm".       
-0001c760: 2029 0a20 2020 2020 2020 206f 732e 7379   ).        os.sy
-0001c770: 7374 656d 280a 2020 2020 2020 2020 2020  stem(.          
-0001c780: 2020 6622 7864 672d 6465 736b 746f 702d    f"xdg-desktop-
-0001c790: 6d65 6e75 2069 6e73 7461 6c6c 207b 6673  menu install {fs
-0001c7a0: 7574 696c 732e 4d4f 4455 4c45 5f50 4154  utils.MODULE_PAT
-0001c7b0: 487d 2f64 6174 612f 6b36 6774 652d 6e6f  H}/data/k6gte-no
-0001c7c0: 7431 6d6d 2e64 6573 6b74 6f70 220a 2020  t1mm.desktop".  
-0001c7d0: 2020 2020 2020 290a 0a0a 6465 6620 646f        )...def do
-0001c7e0: 696d 7028 6d6f 646e 616d 6529 202d 3e20  imp(modname) -> 
-0001c7f0: 6f62 6a65 6374 3a0a 2020 2020 2222 220a  object:.    """.
-0001c800: 2020 2020 496d 706f 7274 7320 6120 6d6f      Imports a mo
-0001c810: 6475 6c65 2e0a 0a20 2020 2050 6172 616d  dule...    Param
-0001c820: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0001c830: 2d2d 2d2d 0a20 2020 206d 6f64 6e61 6d65  ----.    modname
-0001c840: 203a 2073 7472 0a20 2020 2054 6865 206e   : str.    The n
-0001c850: 616d 6520 6f66 2074 6865 206d 6f64 756c  ame of the modul
-0001c860: 6520 746f 2069 6d70 6f72 742e 0a0a 2020  e to import...  
-0001c870: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-0001c880: 2d2d 2d2d 2d0a 2020 2020 6f62 6a65 6374  -----.    object
-0001c890: 0a20 2020 2054 6865 206d 6f64 756c 6520  .    The module 
-0001c8a0: 6f62 6a65 6374 2e0a 2020 2020 2222 220a  object..    """.
-0001c8b0: 0a20 2020 206c 6f67 6765 722e 6465 6275  .    logger.debu
-0001c8c0: 6728 2264 6f69 6d70 3a20 2573 222c 206d  g("doimp: %s", m
-0001c8d0: 6f64 6e61 6d65 290a 2020 2020 7265 7475  odname).    retu
-0001c8e0: 726e 2069 6d70 6f72 746c 6962 2e69 6d70  rn importlib.imp
-0001c8f0: 6f72 745f 6d6f 6475 6c65 2866 226e 6f74  ort_module(f"not
-0001c900: 316d 6d2e 706c 7567 696e 732e 7b6d 6f64  1mm.plugins.{mod
-0001c910: 6e61 6d65 7d22 290a 0a0a 6465 6620 7275  name}")...def ru
-0001c920: 6e28 2920 2d3e 204e 6f6e 653a 0a20 2020  n() -> None:.   
-0001c930: 2022 2222 0a20 2020 204d 6169 6e20 456e   """.    Main En
-0001c940: 7472 790a 2020 2020 2222 220a 2020 2020  try.    """.    
-0001c950: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
-0001c960: 2020 2020 2020 6622 5265 736f 6c76 6564        f"Resolved
-0001c970: 204f 5320 6669 6c65 2073 7973 7465 6d20   OS file system 
-0001c980: 7061 7468 733a 204d 4f44 554c 455f 5041  paths: MODULE_PA
-0001c990: 5448 207b 6673 7574 696c 732e 4d4f 4455  TH {fsutils.MODU
-0001c9a0: 4c45 5f50 4154 487d 2c20 5553 4552 5f44  LE_PATH}, USER_D
-0001c9b0: 4154 415f 5041 5448 207b 6673 7574 696c  ATA_PATH {fsutil
-0001c9c0: 732e 5553 4552 5f44 4154 415f 5041 5448  s.USER_DATA_PATH
-0001c9d0: 7d2c 2043 4f4e 4649 475f 5041 5448 207b  }, CONFIG_PATH {
-0001c9e0: 6673 7574 696c 732e 434f 4e46 4947 5f50  fsutils.CONFIG_P
-0001c9f0: 4154 487d 220a 2020 2020 290a 2020 2020  ATH}".    ).    
-0001ca00: 696e 7374 616c 6c5f 6963 6f6e 7328 290a  install_icons().
-0001ca10: 2020 2020 7469 6d65 722e 7374 6172 7428      timer.start(
-0001ca20: 3235 3029 0a20 2020 2073 7973 2e65 7869  250).    sys.exi
-0001ca30: 7428 6170 702e 6578 6563 2829 290a 0a0a  t(app.exec())...
-0001ca40: 4445 4255 475f 454e 4142 4c45 4420 3d20  DEBUG_ENABLED = 
-0001ca50: 4661 6c73 650a 6966 2050 6174 6828 222e  False.if Path(".
-0001ca60: 2f64 6562 7567 2229 2e65 7869 7374 7328  /debug").exists(
-0001ca70: 293a 0a20 2020 2044 4542 5547 5f45 4e41  ):.    DEBUG_ENA
-0001ca80: 424c 4544 203d 2054 7275 650a 0a6c 6f67  BLED = True..log
-0001ca90: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-0001caa0: 744c 6f67 6765 7228 225f 5f6d 6169 6e5f  tLogger("__main_
-0001cab0: 5f22 290a 0a6c 6f67 6769 6e67 2e62 6173  _")..logging.bas
-0001cac0: 6963 436f 6e66 6967 280a 2020 2020 6c65  icConfig(.    le
-0001cad0: 7665 6c3d 6c6f 6767 696e 672e 4445 4255  vel=logging.DEBU
-0001cae0: 4720 6966 2044 4542 5547 5f45 4e41 424c  G if DEBUG_ENABL
-0001caf0: 4544 2065 6c73 6520 6c6f 6767 696e 672e  ED else logging.
-0001cb00: 4352 4954 4943 414c 2c0a 2020 2020 666f  CRITICAL,.    fo
-0001cb10: 726d 6174 3d22 5b25 2861 7363 7469 6d65  rmat="[%(asctime
-0001cb20: 2973 5d20 2528 6c65 7665 6c6e 616d 6529  )s] %(levelname)
-0001cb30: 7320 2528 6e61 6d65 2973 202d 2025 2866  s %(name)s - %(f
-0001cb40: 756e 634e 616d 6529 7320 4c69 6e65 2025  uncName)s Line %
-0001cb50: 286c 696e 656e 6f29 643a 2025 286d 6573  (lineno)d: %(mes
-0001cb60: 7361 6765 2973 222c 0a20 2020 2068 616e  sage)s",.    han
-0001cb70: 646c 6572 733d 5b0a 2020 2020 2020 2020  dlers=[.        
-0001cb80: 526f 7461 7469 6e67 4669 6c65 4861 6e64  RotatingFileHand
-0001cb90: 6c65 7228 6673 7574 696c 732e 4c4f 475f  ler(fsutils.LOG_
-0001cba0: 4649 4c45 2c20 6d61 7842 7974 6573 3d31  FILE, maxBytes=1
-0001cbb0: 3034 3930 3030 302c 2062 6163 6b75 7043  0490000, backupC
-0001cbc0: 6f75 6e74 3d32 3029 2c0a 2020 2020 2020  ount=20),.      
-0001cbd0: 2020 6c6f 6767 696e 672e 5374 7265 616d    logging.Stream
-0001cbe0: 4861 6e64 6c65 7228 292c 0a20 2020 205d  Handler(),.    ]
-0001cbf0: 2c0a 290a 6c6f 6767 696e 672e 6765 744c  ,.).logging.getL
-0001cc00: 6f67 6765 7228 2250 7951 7435 2e75 6963  ogger("PyQt5.uic
-0001cc10: 2e75 6970 6172 7365 7222 292e 7365 744c  .uiparser").setL
-0001cc20: 6576 656c 2822 494e 464f 2229 0a6c 6f67  evel("INFO").log
-0001cc30: 6769 6e67 2e67 6574 4c6f 6767 6572 2822  ging.getLogger("
-0001cc40: 5079 5174 352e 7569 632e 7072 6f70 6572  PyQt5.uic.proper
-0001cc50: 7469 6573 2229 2e73 6574 4c65 7665 6c28  ties").setLevel(
-0001cc60: 2249 4e46 4f22 290a 6170 7020 3d20 5174  "INFO").app = Qt
-0001cc70: 5769 6467 6574 732e 5141 7070 6c69 6361  Widgets.QApplica
-0001cc80: 7469 6f6e 2873 7973 2e61 7267 7629 0a66  tion(sys.argv).f
-0001cc90: 616d 696c 6965 7320 3d20 6c6f 6164 5f66  amilies = load_f
-0001cca0: 6f6e 7473 5f66 726f 6d5f 6469 7228 6f73  onts_from_dir(os
-0001ccb0: 2e66 7370 6174 6828 6673 7574 696c 732e  .fspath(fsutils.
-0001ccc0: 4150 505f 4441 5441 5f50 4154 4829 290a  APP_DATA_PATH)).
-0001ccd0: 6c6f 6767 6572 2e69 6e66 6f28 6622 666f  logger.info(f"fo
-0001cce0: 6e74 2066 616d 696c 6965 7320 7b66 616d  nt families {fam
-0001ccf0: 696c 6965 737d 2229 0a77 696e 646f 7720  ilies}").window 
-0001cd00: 3d20 4d61 696e 5769 6e64 6f77 2829 0a68  = MainWindow().h
-0001cd10: 6569 6768 7420 3d20 7769 6e64 6f77 2e70  eight = window.p
-0001cd20: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
-0001cd30: 6865 6967 6874 222c 2033 3030 290a 7769  height", 300).wi
-0001cd40: 6474 6820 3d20 7769 6e64 6f77 2e70 7265  dth = window.pre
-0001cd50: 662e 6765 7428 2277 696e 646f 775f 7769  f.get("window_wi
-0001cd60: 6474 6822 2c20 3730 3029 0a78 203d 2077  dth", 700).x = w
-0001cd70: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
-0001cd80: 7769 6e64 6f77 5f78 222c 202d 3129 0a79  window_x", -1).y
-0001cd90: 203d 2077 696e 646f 772e 7072 6566 2e67   = window.pref.g
-0001cda0: 6574 2822 7769 6e64 6f77 5f79 222c 202d  et("window_y", -
-0001cdb0: 3129 0a77 696e 646f 772e 7365 7447 656f  1).window.setGeo
-0001cdc0: 6d65 7472 7928 782c 2079 2c20 7769 6474  metry(x, y, widt
-0001cdd0: 682c 2068 6569 6768 7429 0a77 696e 646f  h, height).windo
-0001cde0: 772e 6361 6c6c 7369 676e 2e73 6574 466f  w.callsign.setFo
-0001cdf0: 6375 7328 290a 7769 6e64 6f77 2e73 686f  cus().window.sho
-0001ce00: 7728 290a 7469 6d65 7220 3d20 5174 436f  w().timer = QtCo
-0001ce10: 7265 2e51 5469 6d65 7228 290a 7469 6d65  re.QTimer().time
-0001ce20: 722e 7469 6d65 6f75 742e 636f 6e6e 6563  r.timeout.connec
-0001ce30: 7428 7769 6e64 6f77 2e70 6f6c 6c5f 7261  t(window.poll_ra
-0001ce40: 6469 6f29 0a0a 6966 205f 5f6e 616d 655f  dio)..if __name_
-0001ce50: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
-0001ce60: 0a20 2020 2072 756e 2829 0a              .    run().
+00018710: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+00018720: 0a20 2020 2064 6566 2063 6865 636b 5f63  .    def check_c
+00018730: 616c 6c73 6967 6e28 7365 6c66 2c20 6361  allsign(self, ca
+00018740: 6c6c 7369 676e 2920 2d3e 204e 6f6e 653a  llsign) -> None:
+00018750: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00018760: 2020 2020 2043 6865 636b 2063 616c 6c73       Check calls
+00018770: 6967 6e20 6173 2069 7427 7320 6265 696e  ign as it's bein
+00018780: 6720 656e 7465 7265 6420 696e 2074 6865  g entered in the
+00018790: 2062 6967 5f63 7479 2069 6e64 6578 2e0a   big_cty index..
+000187a0: 2020 2020 2020 2020 4765 7420 4458 2065          Get DX e
+000187b0: 6e74 6974 792c 2043 512c 2049 5455 2061  ntity, CQ, ITU a
+000187c0: 6e64 2063 6f6e 7469 6e65 6e74 2e0a 2020  nd continent..  
+000187d0: 2020 2020 2020 4765 6f67 7261 7068 6963        Geographic
+000187e0: 2069 6e66 6f72 6d61 7469 6f6e 2e20 4469   information. Di
+000187f0: 7374 616e 6365 2061 6e64 2048 6561 6469  stance and Headi
+00018800: 6e67 2e0a 0a20 2020 2020 2020 2050 6172  ng...        Par
+00018810: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00018820: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00018830: 2020 2063 616c 6c73 6967 6e20 3a20 7374     callsign : st
+00018840: 720a 2020 2020 2020 2020 4361 6c6c 7369  r.        Callsi
+00018850: 676e 2074 6f20 6368 6563 6b2e 0a0a 2020  gn to check...  
+00018860: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00018870: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00018880: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
+00018890: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+000188a0: 7265 7375 6c74 203d 2073 656c 662e 6374  result = self.ct
+000188b0: 795f 6c6f 6f6b 7570 2863 616c 6c73 6967  y_lookup(callsig
+000188c0: 6e29 0a20 2020 2020 2020 2064 6562 7567  n).        debug
+000188d0: 5f72 6573 756c 7420 3d20 6622 7b72 6573  _result = f"{res
+000188e0: 756c 747d 220a 2020 2020 2020 2020 6c6f  ult}".        lo
+000188f0: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+00018900: 2064 6562 7567 5f72 6573 756c 7429 0a20   debug_result). 
+00018910: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
+00018920: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00018930: 7220 6120 696e 2072 6573 756c 742e 6974  r a in result.it
+00018940: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00018950: 2020 2020 2020 2065 6e74 6974 7920 3d20         entity = 
+00018960: 615b 315d 2e67 6574 2822 656e 7469 7479  a[1].get("entity
+00018970: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
+00018980: 2020 2020 2020 2063 7120 3d20 615b 315d         cq = a[1]
+00018990: 2e67 6574 2822 6371 222c 2022 2229 0a20  .get("cq", ""). 
+000189a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000189b0: 7475 203d 2061 5b31 5d2e 6765 7428 2269  tu = a[1].get("i
+000189c0: 7475 222c 2022 2229 0a20 2020 2020 2020  tu", "").       
+000189d0: 2020 2020 2020 2020 2063 6f6e 7469 6e65           contine
+000189e0: 6e74 203d 2061 5b31 5d2e 6765 7428 2263  nt = a[1].get("c
+000189f0: 6f6e 7469 6e65 6e74 2229 0a20 2020 2020  ontinent").     
+00018a00: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
+00018a10: 2066 6c6f 6174 2861 5b31 5d2e 6765 7428   float(a[1].get(
+00018a20: 226c 6174 222c 2022 302e 3022 2929 0a20  "lat", "0.0")). 
+00018a30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00018a40: 6f6e 203d 2066 6c6f 6174 2861 5b31 5d2e  on = float(a[1].
+00018a50: 6765 7428 226c 6f6e 6722 2c20 2230 2e30  get("long", "0.0
+00018a60: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+00018a70: 2020 2020 6c6f 6e20 3d20 6c6f 6e20 2a20      lon = lon * 
+00018a80: 2d31 2020 2320 6374 792e 6461 7420 6669  -1  # cty.dat fi
+00018a90: 6c65 2069 6e76 6572 7473 206c 6f6e 6769  le inverts longi
+00018aa0: 7475 6465 730a 2020 2020 2020 2020 2020  tudes.          
+00018ab0: 2020 2020 2020 7072 696d 6172 795f 7066        primary_pf
+00018ac0: 7820 3d20 615b 315d 2e67 6574 2822 7072  x = a[1].get("pr
+00018ad0: 696d 6172 795f 7066 7822 2c20 2222 290a  imary_pfx", "").
+00018ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018af0: 6865 6164 696e 6720 3d20 6265 6172 696e  heading = bearin
+00018b00: 675f 7769 7468 5f6c 6174 6c6f 6e28 7365  g_with_latlon(se
+00018b10: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+00018b20: 4772 6964 5371 7561 7265 2229 2c20 6c61  GridSquare"), la
+00018b30: 742c 206c 6f6e 290a 2020 2020 2020 2020  t, lon).        
+00018b40: 2020 2020 2020 2020 6b69 6c6f 6d65 7465          kilomete
+00018b50: 7273 203d 2064 6973 7461 6e63 655f 7769  rs = distance_wi
+00018b60: 7468 5f6c 6174 6c6f 6e28 0a20 2020 2020  th_latlon(.     
+00018b70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018b80: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+00018b90: 2247 7269 6453 7175 6172 6522 292c 206c  "GridSquare"), l
+00018ba0: 6174 2c20 6c6f 6e0a 2020 2020 2020 2020  at, lon.        
+00018bb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00018bc0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00018bd0: 6561 6469 6e67 5f64 6973 7461 6e63 652e  eading_distance.
+00018be0: 7365 7454 6578 7428 0a20 2020 2020 2020  setText(.       
+00018bf0: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
+00018c00: 6567 696f 6e61 6c20 4864 6720 7b68 6561  egional Hdg {hea
+00018c10: 6469 6e67 7dc2 b020 4c50 207b 7265 6369  ding}.. LP {reci
+00018c20: 7072 6f63 6f6c 2868 6561 6469 6e67 297d  procol(heading)}
+00018c30: c2b0 202f 2022 0a20 2020 2020 2020 2020  .. / ".         
+00018c40: 2020 2020 2020 2020 2020 2066 2264 6973             f"dis
+00018c50: 7461 6e63 6520 7b69 6e74 286b 696c 6f6d  tance {int(kilom
+00018c60: 6574 6572 732a 302e 3632 3133 3731 297d  eters*0.621371)}
+00018c70: 6d69 207b 6b69 6c6f 6d65 7465 7273 7d6b  mi {kilometers}k
+00018c80: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
+00018c90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00018ca0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00018cb0: 745b 2243 6f75 6e74 7279 5072 6566 6978  t["CountryPrefix
+00018cc0: 225d 203d 2070 7269 6d61 7279 5f70 6678  "] = primary_pfx
+00018cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018ce0: 2073 656c 662e 636f 6e74 6163 745b 225a   self.contact["Z
+00018cf0: 4e22 5d20 3d20 696e 7428 6371 290a 2020  N"] = int(cq).  
+00018d00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018d10: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d30: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00018d40: 7374 2e6e 616d 6520 3d3d 2022 4941 5255  st.name == "IARU
+00018d50: 2048 4622 3a0a 2020 2020 2020 2020 2020   HF":.          
+00018d60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018d70: 6c66 2e63 6f6e 7461 6374 5b22 5a4e 225d  lf.contact["ZN"]
+00018d80: 203d 2069 6e74 2869 7475 290a 2020 2020   = int(itu).    
+00018d90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018da0: 2e63 6f6e 7461 6374 5b22 436f 6e74 696e  .contact["Contin
+00018db0: 656e 7422 5d20 3d20 636f 6e74 696e 656e  ent"] = continen
+00018dc0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00018dd0: 2020 7365 6c66 2e64 785f 656e 7469 7479    self.dx_entity
+00018de0: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
+00018df0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00018e00: 7b70 7269 6d61 7279 5f70 6678 7d3a 207b  {primary_pfx}: {
+00018e10: 636f 6e74 696e 656e 747d 2f7b 656e 7469  continent}/{enti
+00018e20: 7479 7d20 6371 3a7b 6371 7d20 6974 753a  ty} cq:{cq} itu:
+00018e30: 7b69 7475 7d22 0a20 2020 2020 2020 2020  {itu}".         
+00018e40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018e50: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00018e60: 6361 6c6c 7369 676e 2920 3e20 323a 0a20  callsign) > 2:. 
+00018e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e80: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00018e90: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00018ea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018eb0: 2e63 6f6e 7465 7374 2e70 7265 6669 6c6c  .contest.prefill
+00018ec0: 2873 656c 6629 0a0a 2020 2020 6465 6620  (self)..    def 
+00018ed0: 6368 6563 6b5f 6361 6c6c 7369 676e 3228  check_callsign2(
+00018ee0: 7365 6c66 2c20 6361 6c6c 7369 676e 2920  self, callsign) 
+00018ef0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00018f00: 2022 2222 0a20 2020 2020 2020 2043 6865   """.        Che
+00018f10: 636b 2074 6865 2063 616c 6c73 6967 6e20  ck the callsign 
+00018f20: 6166 7465 7220 6974 2068 6173 2062 6565  after it has bee
+00018f30: 6e20 656e 7465 7265 642e 0a20 2020 2020  n entered..     
+00018f40: 2020 204c 6f6f 6b20 7570 2074 6865 2063     Look up the c
+00018f50: 616c 6c73 6967 6e20 696e 2074 6865 2063  allsign in the c
+00018f60: 616c 6c73 6967 6e20 6461 7461 6261 7365  allsign database
+00018f70: 2e0a 2020 2020 2020 2020 4765 7420 7468  ..        Get th
+00018f80: 6520 6772 6964 2073 7175 6172 6520 616e  e grid square an
+00018f90: 6420 6361 6c63 756c 6174 6520 7468 6520  d calculate the 
+00018fa0: 6469 7374 616e 6365 2061 6e64 2068 6561  distance and hea
+00018fb0: 6469 6e67 2e0a 0a20 2020 2020 2020 2050  ding...        P
+00018fc0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00018fd0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00018fe0: 2020 2020 2063 616c 6c73 6967 6e20 3a20       callsign : 
+00018ff0: 7374 720a 2020 2020 2020 2020 4361 6c6c  str.        Call
+00019000: 7369 676e 2074 6f20 6368 6563 6b2e 0a0a  sign to check...
+00019010: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00019020: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00019030: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+00019040: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00019050: 2020 6361 6c6c 7369 676e 203d 2063 616c    callsign = cal
+00019060: 6c73 6967 6e2e 7374 7269 7028 290a 2020  lsign.strip().  
+00019070: 2020 2020 2020 6465 6275 675f 6c6f 6f6b        debug_look
+00019080: 7570 203d 2066 227b 7365 6c66 2e6c 6f6f  up = f"{self.loo
+00019090: 6b5f 7570 7d22 0a20 2020 2020 2020 206c  k_up}".        l
+000190a0: 6f67 6765 722e 6465 6275 6728 2225 732c  ogger.debug("%s,
+000190b0: 2025 7322 2c20 6361 6c6c 7369 676e 2c20   %s", callsign, 
+000190c0: 6465 6275 675f 6c6f 6f6b 7570 290a 2020  debug_lookup).  
+000190d0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+000190e0: 2873 656c 662e 6c6f 6f6b 5f75 702c 2022  (self.look_up, "
+000190f0: 7365 7373 696f 6e22 293a 0a20 2020 2020  session"):.     
+00019100: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+00019110: 6f6f 6b5f 7570 2e73 6573 7369 6f6e 3a0a  ook_up.session:.
+00019120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019130: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00019140: 6c6f 6f6b 5f75 702e 6c6f 6f6b 7570 2863  look_up.lookup(c
+00019150: 616c 6c73 6967 6e29 0a20 2020 2020 2020  allsign).       
+00019160: 2020 2020 2020 2020 2064 6562 7567 5f72           debug_r
+00019170: 6573 706f 6e73 6520 3d20 6622 7b72 6573  esponse = f"{res
+00019180: 706f 6e73 657d 220a 2020 2020 2020 2020  ponse}".        
+00019190: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000191a0: 6562 7567 2822 5468 6520 5265 7370 6f6e  ebug("The Respon
+000191b0: 7365 3a20 2573 5c6e 222c 2064 6562 7567  se: %s\n", debug
+000191c0: 5f72 6573 706f 6e73 6529 0a20 2020 2020  _response).     
+000191d0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+000191e0: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+000191f0: 2020 2020 2020 2020 2020 2020 7468 6569              thei
+00019200: 7267 7269 6420 3d20 7265 7370 6f6e 7365  rgrid = response
+00019210: 2e67 6574 2822 6772 6964 2229 0a20 2020  .get("grid").   
+00019220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019230: 2073 656c 662e 636f 6e74 6163 745b 2247   self.contact["G
+00019240: 7269 6453 7175 6172 6522 5d20 3d20 7468  ridSquare"] = th
+00019250: 6569 7267 7269 640a 2020 2020 2020 2020  eirgrid.        
+00019260: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
+00019270: 6972 636f 756e 7472 7920 3d20 7265 7370  ircountry = resp
+00019280: 6f6e 7365 2e67 6574 2822 636f 756e 7472  onse.get("countr
+00019290: 7922 290a 2020 2020 2020 2020 2020 2020  y").            
+000192a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000192b0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
+000192c0: 6453 7175 6172 6522 2c20 2222 293a 0a20  dSquare", ""):. 
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 2020 2020 2020 2068 6561 6469 6e67 203d         heading =
+000192f0: 2062 6561 7269 6e67 2873 656c 662e 7374   bearing(self.st
+00019300: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
+00019310: 7175 6172 6522 2c20 2222 292c 2074 6865  quare", ""), the
+00019320: 6972 6772 6964 290a 2020 2020 2020 2020  irgrid).        
+00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019340: 6b69 6c6f 6d65 7465 7273 203d 2064 6973  kilometers = dis
+00019350: 7461 6e63 6528 7365 6c66 2e73 7461 7469  tance(self.stati
+00019360: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
+00019370: 7265 2229 2c20 7468 6569 7267 7269 6429  re"), theirgrid)
+00019380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019390: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000193a0: 6164 696e 675f 6469 7374 616e 6365 2e73  ading_distance.s
+000193b0: 6574 5465 7874 280a 2020 2020 2020 2020  etText(.        
+000193c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193d0: 2020 2020 6622 7b74 6865 6972 6772 6964      f"{theirgrid
+000193e0: 7d20 4864 6720 7b68 6561 6469 6e67 7dc2  } Hdg {heading}.
+000193f0: b020 4c50 207b 7265 6369 7072 6f63 6f6c  . LP {reciprocol
+00019400: 2868 6561 6469 6e67 297d c2b0 202f 2022  (heading)}.. / "
+00019410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019420: 2020 2020 2020 2020 2020 2020 2066 2264               f"d
+00019430: 6973 7461 6e63 6520 7b69 6e74 286b 696c  istance {int(kil
+00019440: 6f6d 6574 6572 732a 302e 3632 3133 3731  ometers*0.621371
+00019450: 297d 6d69 207b 6b69 6c6f 6d65 7465 7273  )}mi {kilometers
+00019460: 7d6b 6d22 0a20 2020 2020 2020 2020 2020  }km".           
+00019470: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00019480: 2020 2020 6465 6620 6368 6563 6b5f 6475      def check_du
+00019490: 7065 2873 656c 662c 2063 616c 6c3a 2073  pe(self, call: s
+000194a0: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
+000194b0: 2020 2020 2022 2222 4368 6563 6b73 2069       """Checks i
+000194c0: 6620 6120 6361 6c6c 7369 676e 2069 7320  f a callsign is 
+000194d0: 6120 6475 7065 206f 6e20 6375 7272 656e  a dupe on curren
+000194e0: 7420 6261 6e64 2f6d 6f64 652e 2222 220a  t band/mode.""".
+000194f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019500: 636f 6e74 6573 7420 6973 204e 6f6e 653a  contest is None:
+00019510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019520: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
+00019530: 6f78 2822 596f 7520 6861 7665 206e 6f20  ox("You have no 
+00019540: 636f 6e74 6573 7420 6c6f 6164 6564 2e22  contest loaded."
+00019550: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00019560: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00019570: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
+00019580: 7072 6564 7570 6528 7365 6c66 290a 2020  predupe(self).  
+00019590: 2020 2020 2020 6261 6e64 203d 2066 6c6f        band = flo
+000195a0: 6174 2867 6574 5f6c 6f67 6765 645f 6261  at(get_logged_ba
+000195b0: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
+000195c0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+000195d0: 6122 2c20 302e 3029 2929 290a 2020 2020  a", 0.0)))).    
+000195e0: 2020 2020 6d6f 6465 203d 2073 656c 662e      mode = self.
+000195f0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00019600: 226d 6f64 6522 2c20 2222 290a 2020 2020  "mode", "").    
+00019610: 2020 2020 6465 6275 676c 696e 6520 3d20      debugline = 
+00019620: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+00019630: 4361 6c6c 3a20 7b63 616c 6c7d 2042 616e  Call: {call} Ban
+00019640: 643a 207b 6261 6e64 7d20 4d6f 6465 3a20  d: {band} Mode: 
+00019650: 7b6d 6f64 657d 2044 7570 6574 7970 653a  {mode} Dupetype:
+00019660: 207b 7365 6c66 2e63 6f6e 7465 7374 2e64   {self.contest.d
+00019670: 7570 655f 7479 7065 7d22 0a20 2020 2020  upe_type}".     
+00019680: 2020 2029 0a20 2020 2020 2020 206c 6f67     ).        log
+00019690: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+000196a0: 6465 6275 676c 696e 6529 0a20 2020 2020  debugline).     
+000196b0: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+000196c0: 7374 2e64 7570 655f 7479 7065 203d 3d20  st.dupe_type == 
+000196d0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+000196e0: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
+000196f0: 6162 6173 652e 6368 6563 6b5f 6475 7065  abase.check_dupe
+00019700: 2863 616c 6c29 0a20 2020 2020 2020 2069  (call).        i
+00019710: 6620 7365 6c66 2e63 6f6e 7465 7374 2e64  f self.contest.d
+00019720: 7570 655f 7479 7065 203d 3d20 323a 0a20  upe_type == 2:. 
+00019730: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00019740: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
+00019750: 652e 6368 6563 6b5f 6475 7065 5f6f 6e5f  e.check_dupe_on_
+00019760: 6261 6e64 2863 616c 6c2c 2062 616e 6429  band(call, band)
+00019770: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00019780: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
+00019790: 7065 203d 3d20 333a 0a20 2020 2020 2020  pe == 3:.       
+000197a0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+000197b0: 6c66 2e64 6174 6162 6173 652e 6368 6563  lf.database.chec
+000197c0: 6b5f 6475 7065 5f6f 6e5f 6261 6e64 5f6d  k_dupe_on_band_m
+000197d0: 6f64 6528 6361 6c6c 2c20 6261 6e64 2c20  ode(call, band, 
+000197e0: 6d6f 6465 290a 2020 2020 2020 2020 6966  mode).        if
+000197f0: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
+00019800: 7065 5f74 7970 6520 3d3d 2034 3a0a 2020  pe_type == 4:.  
+00019810: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00019820: 203d 207b 2269 7364 7570 6522 3a20 4661   = {"isdupe": Fa
+00019830: 6c73 657d 0a20 2020 2020 2020 2064 6562  lse}.        deb
+00019840: 7567 6c69 6e65 203d 2066 227b 7265 7375  ugline = f"{resu
+00019850: 6c74 7d22 0a20 2020 2020 2020 206c 6f67  lt}".        log
+00019860: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+00019870: 6465 6275 676c 696e 6529 0a20 2020 2020  debugline).     
+00019880: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00019890: 2e67 6574 2822 6973 6475 7065 222c 2046  .get("isdupe", F
+000198a0: 616c 7365 290a 0a20 2020 2064 6566 2073  alse)..    def s
+000198b0: 6574 6d6f 6465 2873 656c 662c 206d 6f64  etmode(self, mod
+000198c0: 653a 2073 7472 2920 2d3e 204e 6f6e 653a  e: str) -> None:
+000198d0: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
+000198e0: 2077 6865 6e20 7468 6520 6d6f 6465 2063   when the mode c
+000198f0: 6861 6e67 6573 2e22 2222 0a20 2020 2020  hanges.""".     
+00019900: 2020 2069 6620 6d6f 6465 203d 3d20 2243     if mode == "C
+00019910: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
+00019920: 6966 2073 656c 662e 6375 7272 656e 745f  if self.current_
+00019930: 6d6f 6465 2021 3d20 2243 5722 3a0a 2020  mode != "CW":.  
+00019940: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019950: 6c66 2e63 7572 7265 6e74 5f6d 6f64 6520  lf.current_mode 
+00019960: 3d20 2243 5722 0a20 2020 2020 2020 2020  = "CW".         
+00019970: 2020 2020 2020 2023 2073 656c 662e 6d6f         # self.mo
+00019980: 6465 2e73 6574 5465 7874 2822 4357 2229  de.setText("CW")
+00019990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000199a0: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
+000199b0: 7874 2822 3539 3922 290a 2020 2020 2020  xt("599").      
+000199c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000199d0: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
+000199e0: 3539 3922 290a 2020 2020 2020 2020 2020  599").          
+000199f0: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
+00019a00: 6377 5f6d 6163 726f 7328 290a 2020 2020  cw_macros().    
+00019a10: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00019a20: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
+00019a30: 3d20 2253 5342 223a 0a20 2020 2020 2020  = "SSB":.       
+00019a40: 2020 2020 2069 6620 7365 6c66 2e63 7572       if self.cur
+00019a50: 7265 6e74 5f6d 6f64 6520 213d 2022 5353  rent_mode != "SS
+00019a60: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+00019a70: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
+00019a80: 5f6d 6f64 6520 3d20 2253 5342 220a 2020  _mode = "SSB".  
+00019a90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00019aa0: 7365 6c66 2e6d 6f64 652e 7365 7454 6578  self.mode.setTex
+00019ab0: 7428 2253 5342 2229 0a20 2020 2020 2020  t("SSB").       
+00019ac0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00019ad0: 6e74 2e73 6574 5465 7874 2822 3539 2229  nt.setText("59")
+00019ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019af0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
+00019b00: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
+00019b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019b20: 2e72 6561 645f 6377 5f6d 6163 726f 7328  .read_cw_macros(
+00019b30: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00019b40: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00019b50: 6d6f 6465 203d 3d20 2252 5454 5922 3a0a  mode == "RTTY":.
+00019b60: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00019b70: 656c 662e 6375 7272 656e 745f 6d6f 6465  elf.current_mode
+00019b80: 2021 3d20 2252 5454 5922 3a0a 2020 2020   != "RTTY":.    
+00019b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019ba0: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
+00019bb0: 2252 5454 5922 0a20 2020 2020 2020 2020  "RTTY".         
+00019bc0: 2020 2020 2020 2023 2073 656c 662e 6d6f         # self.mo
+00019bd0: 6465 2e73 6574 5465 7874 2822 5254 5459  de.setText("RTTY
+00019be0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00019bf0: 2020 2073 656c 662e 7365 6e74 2e73 6574     self.sent.set
+00019c00: 5465 7874 2822 3539 2229 0a20 2020 2020  Text("59").     
+00019c10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019c20: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
+00019c30: 2235 3922 290a 0a20 2020 2064 6566 2067  "59")..    def g
+00019c40: 6574 5f6f 706f 6e28 7365 6c66 2920 2d3e  et_opon(self) ->
+00019c50: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00019c60: 2222 0a20 2020 2020 2020 2043 7472 6c2b  "".        Ctrl+
+00019c70: 4f20 4f70 656e 2074 6865 204f 504f 4e20  O Open the OPON 
+00019c80: 6469 616c 6f67 2e0a 0a20 2020 2020 2020  dialog...       
+00019c90: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00019ca0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00019cb0: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
+00019cc0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00019cd0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00019ce0: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
+00019cf0: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+00019d00: 656c 662e 6f70 6f6e 5f64 6961 6c6f 6720  elf.opon_dialog 
+00019d10: 3d20 4f70 4f6e 2866 7375 7469 6c73 2e41  = OpOn(fsutils.A
+00019d20: 5050 5f44 4154 415f 5041 5448 290a 0a20  PP_DATA_PATH).. 
+00019d30: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00019d40: 7572 7265 6e74 5f70 616c 6574 7465 3a0a  urrent_palette:.
+00019d50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019d60: 2e6f 706f 6e5f 6469 616c 6f67 2e73 6574  .opon_dialog.set
+00019d70: 5061 6c65 7474 6528 7365 6c66 2e63 7572  Palette(self.cur
+00019d80: 7265 6e74 5f70 616c 6574 7465 290a 0a20  rent_palette).. 
+00019d90: 2020 2020 2020 2073 656c 662e 6f70 6f6e         self.opon
+00019da0: 5f64 6961 6c6f 672e 6163 6365 7074 6564  _dialog.accepted
+00019db0: 2e63 6f6e 6e65 6374 2873 656c 662e 6e65  .connect(self.ne
+00019dc0: 775f 6f70 290a 2020 2020 2020 2020 7365  w_op).        se
+00019dd0: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e6f  lf.opon_dialog.o
+00019de0: 7065 6e28 290a 0a20 2020 2064 6566 206e  pen()..    def n
+00019df0: 6577 5f6f 7028 7365 6c66 2920 2d3e 204e  ew_op(self) -> N
+00019e00: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00019e10: 0a20 2020 2020 2020 2043 616c 6c65 6420  .        Called 
+00019e20: 7768 656e 2074 6865 2075 7365 7220 636c  when the user cl
+00019e30: 6963 6b73 2074 6865 204f 4b20 6275 7474  icks the OK butt
+00019e40: 6f6e 206f 6e20 7468 6520 4f50 4f4e 2064  on on the OPON d
+00019e50: 6961 6c6f 672e 0a20 2020 2020 2020 2043  ialog..        C
+00019e60: 7265 6174 6520 7468 6520 6e65 7720 6469  reate the new di
+00019e70: 7265 6374 6f72 7920 616e 6420 636f 7079  rectory and copy
+00019e80: 2074 6865 2070 686f 6e65 7469 6320 6669   the phonetic fi
+00019e90: 6c65 732e 0a0a 2020 2020 2020 2020 5061  les...        Pa
+00019ea0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00019eb0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00019ec0: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
+00019ed0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00019ee0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00019ef0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+00019f00: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
+00019f10: 656c 662e 6f70 6f6e 5f64 6961 6c6f 672e  elf.opon_dialog.
+00019f20: 4e65 774f 7065 7261 746f 722e 7465 7874  NewOperator.text
+00019f30: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00019f40: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
+00019f50: 3d20 7365 6c66 2e6f 706f 6e5f 6469 616c  = self.opon_dial
+00019f60: 6f67 2e4e 6577 4f70 6572 6174 6f72 2e74  og.NewOperator.t
+00019f70: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
+00019f80: 2020 2020 2020 7365 6c66 2e6f 706f 6e5f        self.opon_
+00019f90: 6469 616c 6f67 2e63 6c6f 7365 2829 0a20  dialog.close(). 
+00019fa0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00019fb0: 6275 6728 224e 6577 204f 703a 2025 7322  bug("New Op: %s"
+00019fc0: 2c20 7365 6c66 2e63 7572 7265 6e74 5f6f  , self.current_o
+00019fd0: 7029 0a20 2020 2020 2020 2073 656c 662e  p).        self.
+00019fe0: 6d61 6b65 5f6f 705f 6469 7228 290a 0a20  make_op_dir().. 
+00019ff0: 2020 2064 6566 206d 616b 655f 6f70 5f64     def make_op_d
+0001a000: 6972 2873 656c 6629 202d 3e20 4e6f 6e65  ir(self) -> None
+0001a010: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0001a020: 2020 2020 2020 4372 6561 7465 204f 5020        Create OP 
+0001a030: 6469 7265 6374 6f72 7920 6966 2069 7420  directory if it 
+0001a040: 646f 6573 206e 6f74 2065 7869 7374 2e0a  does not exist..
+0001a050: 2020 2020 2020 2020 436f 7079 2074 6865          Copy the
+0001a060: 2070 686f 6e65 7469 6320 6669 6c65 7320   phonetic files 
+0001a070: 746f 2074 6865 206e 6577 2064 6972 6563  to the new direc
+0001a080: 746f 7279 2e0a 0a20 2020 2020 2020 2050  tory...        P
+0001a090: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0001a0a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001a0b0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+0001a0c0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0001a0d0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0001a0e0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+0001a0f0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+0001a100: 7365 6c66 2e63 7572 7265 6e74 5f6f 703a  self.current_op:
+0001a110: 0a20 2020 2020 2020 2020 2020 206f 705f  .            op_
+0001a120: 7061 7468 203d 2066 7375 7469 6c73 2e55  path = fsutils.U
+0001a130: 5345 525f 4441 5441 5f50 4154 4820 2f20  SER_DATA_PATH / 
+0001a140: 7365 6c66 2e63 7572 7265 6e74 5f6f 700a  self.current_op.
+0001a150: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0001a160: 6572 2e64 6562 7567 2822 6f70 5f70 6174  er.debug("op_pat
+0001a170: 683a 2025 7322 2c20 7374 7228 6f70 5f70  h: %s", str(op_p
+0001a180: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
+0001a190: 2020 6966 206f 705f 7061 7468 2e69 735f    if op_path.is_
+0001a1a0: 6469 7228 2920 6973 2046 616c 7365 3a0a  dir() is False:.
+0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1c0: 6c6f 6767 6572 2e64 6562 7567 2822 4372  logger.debug("Cr
+0001a1d0: 6561 7469 6e67 204f 7020 4469 7265 6374  eating Op Direct
+0001a1e0: 6f72 793a 2025 7322 2c20 7374 7228 6f70  ory: %s", str(op
+0001a1f0: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
+0001a200: 2020 2020 2020 2020 6f73 2e6d 6b64 6972          os.mkdir
+0001a210: 2873 7472 286f 705f 7061 7468 2929 0a20  (str(op_path)). 
+0001a220: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
+0001a230: 5f70 6174 682e 6973 5f64 6972 2829 3a0a  _path.is_dir():.
+0001a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a250: 736f 7572 6365 5f70 6174 6820 3d20 6673  source_path = fs
+0001a260: 7574 696c 732e 4150 505f 4441 5441 5f50  utils.APP_DATA_P
+0001a270: 4154 4820 2f20 2270 686f 6e65 7469 6373  ATH / "phonetics
+0001a280: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001a290: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0001a2a0: 736f 7572 6365 5f70 6174 683a 2025 7322  source_path: %s"
+0001a2b0: 2c20 7374 7228 736f 7572 6365 5f70 6174  , str(source_pat
+0001a2c0: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+0001a2d0: 2020 2020 666f 7220 6368 696c 6420 696e      for child in
+0001a2e0: 2073 6f75 7263 655f 7061 7468 2e69 7465   source_path.ite
+0001a2f0: 7264 6972 2829 3a0a 2020 2020 2020 2020  rdir():.        
+0001a300: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+0001a310: 696e 6174 696f 6e5f 6669 6c65 203d 206f  ination_file = o
+0001a320: 705f 7061 7468 202f 2063 6869 6c64 2e6e  p_path / child.n
+0001a330: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0001a340: 2020 2020 2020 2020 6966 2064 6573 7469          if desti
+0001a350: 6e61 7469 6f6e 5f66 696c 652e 6973 5f66  nation_file.is_f
+0001a360: 696c 6528 2920 6973 2046 616c 7365 3a0a  ile() is False:.
+0001a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a380: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0001a390: 6562 7567 2822 4465 7374 696e 6174 696f  ebug("Destinatio
+0001a3a0: 6e3a 2025 7322 2c20 7374 7228 6465 7374  n: %s", str(dest
+0001a3b0: 696e 6174 696f 6e5f 6669 6c65 2929 0a20  ination_file)). 
+0001a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3d0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+0001a3e0: 6f6e 5f66 696c 652e 7772 6974 655f 6279  on_file.write_by
+0001a3f0: 7465 7328 6368 696c 642e 7265 6164 5f62  tes(child.read_b
+0001a400: 7974 6573 2829 290a 0a20 2020 2064 6566  ytes())..    def
+0001a410: 2070 6f6c 6c5f 7261 6469 6f28 7365 6c66   poll_radio(self
+0001a420: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0001a430: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+0001a440: 6f6c 6c20 7261 6469 6f20 666f 7220 5646  oll radio for VF
+0001a450: 4f2c 206d 6f64 652c 2062 616e 6477 6964  O, mode, bandwid
+0001a460: 7468 2e0a 2020 2020 2020 2020 5365 6e64  th..        Send
+0001a470: 2073 7461 7465 2076 6961 206d 756c 7469   state via multi
+0001a480: 6361 7374 2e0a 0a20 2020 2020 2020 2050  cast...        P
+0001a490: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0001a4a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001a4b0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+0001a4c0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0001a4d0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0001a4e0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+0001a4f0: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+0001a500: 662e 7365 745f 7261 6469 6f5f 6963 6f6e  f.set_radio_icon
+0001a510: 2830 290a 2020 2020 2020 2020 6966 2073  (0).        if s
+0001a520: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
+0001a530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a540: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0001a550: 2e6f 6e6c 696e 6520 6973 2046 616c 7365  .online is False
+0001a560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a570: 2020 7365 6c66 2e73 6574 5f72 6164 696f    self.set_radio
+0001a580: 5f69 636f 6e28 3129 0a20 2020 2020 2020  _icon(1).       
+0001a590: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+0001a5a0: 675f 636f 6e74 726f 6c2e 7265 696e 6974  g_control.reinit
+0001a5b0: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+0001a5c0: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+0001a5d0: 6f6c 2e6f 6e6c 696e 653a 0a20 2020 2020  ol.online:.     
+0001a5e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a5f0: 7365 745f 7261 6469 6f5f 6963 6f6e 2832  set_radio_icon(2
+0001a600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001a610: 2020 696e 666f 5f64 6972 7479 203d 2046    info_dirty = F
+0001a620: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+0001a630: 2020 2020 2076 666f 203d 2073 656c 662e       vfo = self.
+0001a640: 7269 675f 636f 6e74 726f 6c2e 6765 745f  rig_control.get_
+0001a650: 7666 6f28 290a 2020 2020 2020 2020 2020  vfo().          
+0001a660: 2020 2020 2020 6d6f 6465 203d 2073 656c        mode = sel
+0001a670: 662e 7269 675f 636f 6e74 726f 6c2e 6765  f.rig_control.ge
+0001a680: 745f 6d6f 6465 2829 0a20 2020 2020 2020  t_mode().       
+0001a690: 2020 2020 2020 2020 2062 7720 3d20 7365           bw = se
+0001a6a0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
+0001a6b0: 6574 5f62 7728 290a 0a20 2020 2020 2020  et_bw()..       
+0001a6c0: 2020 2020 2020 2020 2069 6620 6d6f 6465           if mode
+0001a6d0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a6f0: 6c66 2e73 6574 6d6f 6465 286d 6f64 6529  lf.setmode(mode)
+0001a700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a710: 2069 6620 6d6f 6465 203d 3d20 224c 5342   if mode == "LSB
+0001a720: 2220 6f72 206d 6f64 6520 3d3d 2022 5553  " or mode == "US
+0001a730: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+0001a740: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0001a750: 6d6f 6465 2822 5353 4222 290a 2020 2020  mode("SSB").    
+0001a760: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+0001a770: 6f64 6520 3d3d 2022 5254 5459 223a 0a20  ode == "RTTY":. 
+0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a790: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+0001a7a0: 2252 5454 5922 290a 0a20 2020 2020 2020  "RTTY")..       
+0001a7b0: 2020 2020 2020 2020 2069 6620 7666 6f20           if vfo 
+0001a7c0: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
+0001a7d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001a7e0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0001a7f0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+0001a800: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+0001a810: 2920 213d 2076 666f 3a0a 2020 2020 2020  ) != vfo:.      
+0001a820: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0001a830: 666f 5f64 6972 7479 203d 2054 7275 650a  fo_dirty = True.
+0001a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a850: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+0001a860: 7461 7465 5b22 7666 6f61 225d 203d 2076  tate["vfoa"] = v
+0001a870: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
+0001a880: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
+0001a890: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
+0001a8a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a8b0: 2e72 6164 696f 5f73 7461 7465 5b22 6261  .radio_state["ba
+0001a8c0: 6e64 225d 203d 2062 616e 640a 2020 2020  nd"] = band.    
+0001a8d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a8e0: 2e63 6f6e 7461 6374 5b22 4261 6e64 225d  .contact["Band"]
+0001a8f0: 203d 2067 6574 5f6c 6f67 6765 645f 6261   = get_logged_ba
+0001a900: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
+0001a910: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a920: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
+0001a930: 6174 6f72 2862 616e 6429 0a0a 2020 2020  ator(band)..    
+0001a940: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001a950: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0001a960: 6765 7428 226d 6f64 6522 2920 213d 206d  get("mode") != m
+0001a970: 6f64 653a 0a20 2020 2020 2020 2020 2020  ode:.           
+0001a980: 2020 2020 2020 2020 2069 6e66 6f5f 6469           info_di
+0001a990: 7274 7920 3d20 5472 7565 0a20 2020 2020  rty = True.     
+0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a9b0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+0001a9c0: 226d 6f64 6522 5d20 3d20 6d6f 6465 0a0a  "mode"] = mode..
+0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9e0: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+0001a9f0: 6174 652e 6765 7428 2262 7722 2920 213d  ate.get("bw") !=
+0001aa00: 2062 773a 0a20 2020 2020 2020 2020 2020   bw:.           
+0001aa10: 2020 2020 2020 2020 2069 6e66 6f5f 6469           info_di
+0001aa20: 7274 7920 3d20 5472 7565 0a20 2020 2020  rty = True.     
+0001aa30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001aa40: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+0001aa50: 2262 7722 5d20 3d20 6277 0a0a 2020 2020  "bw"] = bw..    
+0001aa60: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0001aa70: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+0001aa80: 2e6e 6f77 2829 203e 2067 6c6f 6261 6c73  .now() > globals
+0001aa90: 2829 5b22 706f 6c6c 5f74 696d 6522 5d20  ()["poll_time"] 
+0001aaa0: 6f72 2069 6e66 6f5f 6469 7274 793a 0a20  or info_dirty:. 
+0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aac0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0001aad0: 2256 464f 3a20 2573 2020 4d4f 4445 3a20  "VFO: %s  MODE: 
+0001aae0: 2573 2042 573a 2025 7322 2c20 7666 6f2c  %s BW: %s", vfo,
+0001aaf0: 206d 6f64 652c 2062 7729 0a20 2020 2020   mode, bw).     
+0001ab00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001ab10: 656c 662e 7365 745f 7769 6e64 6f77 5f74  elf.set_window_t
+0001ab20: 6974 6c65 2829 0a20 2020 2020 2020 2020  itle().         
+0001ab30: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+0001ab40: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+0001ab50: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+0001ab60: 225d 203d 2022 5241 4449 4f5f 5354 4154  "] = "RADIO_STAT
+0001ab70: 4522 0a20 2020 2020 2020 2020 2020 2020  E".             
+0001ab80: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+0001ab90: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+0001aba0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+0001abb0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+0001abc0: 2262 616e 6422 5d20 3d20 6261 6e64 0a20  "band"] = band. 
+0001abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001abe0: 2020 2063 6d64 5b22 7666 6f61 225d 203d     cmd["vfoa"] =
+0001abf0: 2076 666f 0a20 2020 2020 2020 2020 2020   vfo.           
+0001ac00: 2020 2020 2020 2020 2063 6d64 5b22 6d6f           cmd["mo
+0001ac10: 6465 225d 203d 206d 6f64 650a 2020 2020  de"] = mode.    
+0001ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac30: 636d 645b 2262 7722 5d20 3d20 6277 0a20  cmd["bw"] = bw. 
+0001ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac50: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
+0001ac60: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
+0001ac70: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
+0001ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac90: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
+0001aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001acc0: 6e31 6d6d 2e73 656e 645f 7261 6469 6f5f  n1mm.send_radio_
+0001acd0: 7061 636b 6574 733a 0a20 2020 2020 2020  packets:.       
+0001ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acf0: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
+0001ad00: 6164 696f 5f69 6e66 6f5b 2246 7265 7122  adio_info["Freq"
+0001ad10: 5d20 3d20 7666 6f5b 3a2d 315d 0a20 2020  ] = vfo[:-1].   
+0001ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad30: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0001ad40: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2254  mm.radio_info["T
+0001ad50: 5846 7265 7122 5d20 3d20 7666 6f5b 3a2d  XFreq"] = vfo[:-
+0001ad60: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
+0001ad70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001ad80: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0001ad90: 6e66 6f5b 224d 6f64 6522 5d20 3d20 6d6f  nfo["Mode"] = mo
+0001ada0: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
+0001adb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001adc0: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0001add0: 6e66 6f5b 224f 7043 616c 6c22 5d20 3d20  nfo["OpCall"] = 
+0001ade0: 7365 6c66 2e63 7572 7265 6e74 5f6f 700a  self.current_op.
+0001adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ae10: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+0001ae20: 5b22 4973 5275 6e6e 696e 6722 5d20 3d20  ["IsRunning"] = 
+0001ae30: 7374 7228 0a20 2020 2020 2020 2020 2020  str(.           
+0001ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae50: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+0001ae60: 6574 2822 7275 6e5f 7374 6174 6522 2c20  et("run_state", 
+0001ae70: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aeb0: 2073 656c 662e 6e31 6d6d 2e73 656e 645f   self.n1mm.send_
+0001aec0: 7261 6469 6f28 290a 2020 2020 2020 2020  radio().        
+0001aed0: 2020 2020 2020 2020 2020 2020 676c 6f62              glob
+0001aee0: 616c 7328 295b 0a20 2020 2020 2020 2020  als()[.         
+0001aef0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001af00: 706f 6c6c 5f74 696d 6522 0a20 2020 2020  poll_time".     
+0001af10: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0001af20: 203d 2064 6174 6574 696d 652e 6461 7465   = datetime.date
+0001af30: 7469 6d65 2e6e 6f77 2829 202b 2064 6174  time.now() + dat
+0001af40: 6574 696d 652e 7469 6d65 6465 6c74 6128  etime.timedelta(
+0001af50: 7365 636f 6e64 733d 3130 290a 0a20 2020  seconds=10)..   
+0001af60: 2064 6566 2065 6469 745f 6377 5f6d 6163   def edit_cw_mac
+0001af70: 726f 7328 7365 6c66 2920 2d3e 204e 6f6e  ros(self) -> Non
+0001af80: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0001af90: 2020 2020 2020 2043 616c 6c73 2074 6865         Calls the
+0001afa0: 2064 6566 6175 6c74 2074 6578 7420 6564   default text ed
+0001afb0: 6974 6f72 2074 6f20 6564 6974 2074 6865  itor to edit the
+0001afc0: 2043 5720 6d61 6372 6f20 6669 6c65 2e0a   CW macro file..
+0001afd0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0001afe0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0001aff0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+0001b000: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
+0001b010: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0001b020: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+0001b030: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+0001b040: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+0001b050: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+0001b060: 6f64 6522 2920 3d3d 2022 4357 223a 0a20  ode") == "CW":. 
+0001b070: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+0001b080: 5f66 696c 6520 3d20 2263 776d 6163 726f  _file = "cwmacro
+0001b090: 732e 7478 7422 0a20 2020 2020 2020 2065  s.txt".        e
+0001b0a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001b0b0: 206d 6163 726f 5f66 696c 6520 3d20 2273   macro_file = "s
+0001b0c0: 7362 6d61 6372 6f73 2e74 7874 220a 2020  sbmacros.txt".  
+0001b0d0: 2020 2020 2020 6966 206e 6f74 2028 6673        if not (fs
+0001b0e0: 7574 696c 732e 5553 4552 5f44 4154 415f  utils.USER_DATA_
+0001b0f0: 5041 5448 202f 206d 6163 726f 5f66 696c  PATH / macro_fil
+0001b100: 6529 2e65 7869 7374 7328 293a 0a20 2020  e).exists():.   
+0001b110: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0001b120: 6465 6275 6728 2272 6561 645f 6377 5f6d  debug("read_cw_m
+0001b130: 6163 726f 733a 2063 6f70 7969 6e67 2064  acros: copying d
+0001b140: 6566 6175 6c74 206d 6163 726f 2066 696c  efault macro fil
+0001b150: 652e 2229 0a20 2020 2020 2020 2020 2020  e.").           
+0001b160: 2063 6f70 7966 696c 6528 0a20 2020 2020   copyfile(.     
+0001b170: 2020 2020 2020 2020 2020 2066 7375 7469             fsuti
+0001b180: 6c73 2e41 5050 5f44 4154 415f 5041 5448  ls.APP_DATA_PATH
+0001b190: 202f 206d 6163 726f 5f66 696c 652c 2066   / macro_file, f
+0001b1a0: 7375 7469 6c73 2e55 5345 525f 4441 5441  sutils.USER_DATA
+0001b1b0: 5f50 4154 4820 2f20 6d61 6372 6f5f 6669  _PATH / macro_fi
+0001b1c0: 6c65 0a20 2020 2020 2020 2020 2020 2029  le.            )
+0001b1d0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0001b1e0: 2020 2020 2020 2020 2020 6673 7574 696c            fsutil
+0001b1f0: 732e 6f70 656e 4669 6c65 5769 7468 4f53  s.openFileWithOS
+0001b200: 2866 7375 7469 6c73 2e55 5345 525f 4441  (fsutils.USER_DA
+0001b210: 5441 5f50 4154 4820 2f20 6d61 6372 6f5f  TA_PATH / macro_
+0001b220: 6669 6c65 290a 2020 2020 2020 2020 6578  file).        ex
+0001b230: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0001b240: 2020 6c6f 6767 6572 2e65 7863 6570 7469    logger.excepti
+0001b250: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0001b260: 2020 2020 6622 436f 756c 6420 6e6f 7420      f"Could not 
+0001b270: 6f70 656e 2066 696c 6520 7b66 7375 7469  open file {fsuti
+0001b280: 6c73 2e55 5345 525f 4441 5441 5f50 4154  ls.USER_DATA_PAT
+0001b290: 4820 2f20 6d61 6372 6f5f 6669 6c65 7d22  H / macro_file}"
+0001b2a0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+0001b2b0: 2020 2020 6465 6620 7265 6164 5f63 775f      def read_cw_
+0001b2c0: 6d61 6372 6f73 2873 656c 6629 202d 3e20  macros(self) -> 
+0001b2d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0001b2e0: 220a 2020 2020 2020 2020 5265 6164 7320  ".        Reads 
+0001b2f0: 696e 2074 6865 2043 5720 6d61 6372 6f73  in the CW macros
+0001b300: 2c20 6669 7273 7473 2069 7420 6368 6563  , firsts it chec
+0001b310: 6b73 2074 6f20 7365 6520 6966 2074 6865  ks to see if the
+0001b320: 2066 696c 6520 6578 6973 7473 2e20 4966   file exists. If
+0001b330: 2069 7420 646f 6573 206e 6f74 2c0a 2020   it does not,.  
+0001b340: 2020 2020 2020 616e 6420 7468 6973 2068        and this h
+0001b350: 6173 2062 6565 6e20 7061 636b 6167 6564  as been packaged
+0001b360: 2077 6974 6820 7079 696e 7374 616c 6c65   with pyinstalle
+0001b370: 7220 6974 2077 696c 6c20 636f 7079 2074  r it will copy t
+0001b380: 6865 2064 6566 6175 6c74 2066 696c 6520  he default file 
+0001b390: 6672 6f6d 2074 6865 0a20 2020 2020 2020  from the.       
+0001b3a0: 2074 656d 7020 6469 7265 6374 6f72 7920   temp directory 
+0001b3b0: 7468 6973 2069 7320 7275 6e6e 696e 6720  this is running 
+0001b3c0: 6672 6f6d 2e2e 2e20 496e 2074 6865 6f72  from... In theor
+0001b3d0: 792e 0a20 2020 2020 2020 2022 2222 0a0a  y..        """..
+0001b3e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001b3f0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0001b400: 226d 6f64 6522 2920 3d3d 2022 4357 223a  "mode") == "CW":
+0001b410: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
+0001b420: 726f 5f66 696c 6520 3d20 2263 776d 6163  ro_file = "cwmac
+0001b430: 726f 732e 7478 7422 0a20 2020 2020 2020  ros.txt".       
+0001b440: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001b450: 2020 206d 6163 726f 5f66 696c 6520 3d20     macro_file = 
+0001b460: 2273 7362 6d61 6372 6f73 2e74 7874 220a  "ssbmacros.txt".
+0001b470: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0001b480: 2866 7375 7469 6c73 2e55 5345 525f 4441  (fsutils.USER_DA
+0001b490: 5441 5f50 4154 4820 2f20 6d61 6372 6f5f  TA_PATH / macro_
+0001b4a0: 6669 6c65 292e 6578 6973 7473 2829 3a0a  file).exists():.
+0001b4b0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0001b4c0: 6572 2e64 6562 7567 2822 7265 6164 5f63  er.debug("read_c
+0001b4d0: 775f 6d61 6372 6f73 3a20 636f 7079 696e  w_macros: copyin
+0001b4e0: 6720 6465 6661 756c 7420 6d61 6372 6f20  g default macro 
+0001b4f0: 6669 6c65 2e22 290a 2020 2020 2020 2020  file.").        
+0001b500: 2020 2020 636f 7079 6669 6c65 280a 2020      copyfile(.  
+0001b510: 2020 2020 2020 2020 2020 2020 2020 6673                fs
+0001b520: 7574 696c 732e 4150 505f 4441 5441 5f50  utils.APP_DATA_P
+0001b530: 4154 4820 2f20 6d61 6372 6f5f 6669 6c65  ATH / macro_file
+0001b540: 2c20 6673 7574 696c 732e 5553 4552 5f44  , fsutils.USER_D
+0001b550: 4154 415f 5041 5448 202f 206d 6163 726f  ATA_PATH / macro
+0001b560: 5f66 696c 650a 2020 2020 2020 2020 2020  _file.          
+0001b570: 2020 290a 2020 2020 2020 2020 7769 7468    ).        with
+0001b580: 206f 7065 6e28 0a20 2020 2020 2020 2020   open(.         
+0001b590: 2020 2066 7375 7469 6c73 2e55 5345 525f     fsutils.USER_
+0001b5a0: 4441 5441 5f50 4154 4820 2f20 6d61 6372  DATA_PATH / macr
+0001b5b0: 6f5f 6669 6c65 2c20 2272 222c 2065 6e63  o_file, "r", enc
+0001b5c0: 6f64 696e 673d 2275 7466 2d38 220a 2020  oding="utf-8".  
+0001b5d0: 2020 2020 2020 2920 6173 2066 696c 655f        ) as file_
+0001b5e0: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
+0001b5f0: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+0001b600: 2069 6e20 6669 6c65 5f64 6573 6372 6970   in file_descrip
+0001b610: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+0001b620: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001b630: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+0001b640: 6465 2c20 666b 6579 2c20 6275 7474 6f6e  de, fkey, button
+0001b650: 6e61 6d65 2c20 6377 7465 7874 203d 206c  name, cwtext = l
+0001b660: 696e 652e 7370 6c69 7428 227c 2229 0a20  ine.split("|"). 
+0001b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b680: 2020 2069 6620 6d6f 6465 2e73 7472 6970     if mode.strip
+0001b690: 2829 2e75 7070 6572 2829 203d 3d20 2252  ().upper() == "R
+0001b6a0: 2220 616e 6420 7365 6c66 2e70 7265 662e  " and self.pref.
+0001b6b0: 6765 7428 2272 756e 5f73 7461 7465 2229  get("run_state")
+0001b6c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b6d0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0001b6e0: 6b65 7973 5b66 6b65 792e 7374 7269 7028  keys[fkey.strip(
+0001b6f0: 295d 203d 2028 6275 7474 6f6e 6e61 6d65  )] = (buttonname
+0001b700: 2e73 7472 6970 2829 2c20 6377 7465 7874  .strip(), cwtext
+0001b710: 2e73 7472 6970 2829 290a 2020 2020 2020  .strip()).      
+0001b720: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b730: 206d 6f64 652e 7374 7269 7028 292e 7570   mode.strip().up
+0001b740: 7065 7228 2920 213d 2022 5222 2061 6e64  per() != "R" and
+0001b750: 206e 6f74 2073 656c 662e 7072 6566 2e67   not self.pref.g
+0001b760: 6574 2822 7275 6e5f 7374 6174 6522 293a  et("run_state"):
+0001b770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b780: 2020 2020 2020 2020 2073 656c 662e 666b           self.fk
+0001b790: 6579 735b 666b 6579 2e73 7472 6970 2829  eys[fkey.strip()
+0001b7a0: 5d20 3d20 2862 7574 746f 6e6e 616d 652e  ] = (buttonname.
+0001b7b0: 7374 7269 7028 292c 2063 7774 6578 742e  strip(), cwtext.
+0001b7c0: 7374 7269 7028 2929 0a20 2020 2020 2020  strip()).       
+0001b7d0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0001b7e0: 5661 6c75 6545 7272 6f72 2061 7320 6572  ValueError as er
+0001b7f0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0001b800: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0001b810: 666f 2822 7265 6164 5f63 775f 6d61 6372  fo("read_cw_macr
+0001b820: 6f73 3a20 2573 222c 2065 7272 290a 2020  os: %s", err).  
+0001b830: 2020 2020 2020 6b65 7973 203d 2073 656c        keys = sel
+0001b840: 662e 666b 6579 732e 6b65 7973 2829 0a20  f.fkeys.keys(). 
+0001b850: 2020 2020 2020 2069 6620 2246 3122 2069         if "F1" i
+0001b860: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+0001b870: 2020 2020 7365 6c66 2e46 312e 7365 7454      self.F1.setT
+0001b880: 6578 7428 6622 4631 3a20 7b73 656c 662e  ext(f"F1: {self.
+0001b890: 666b 6579 735b 2746 3127 5d5b 305d 7d22  fkeys['F1'][0]}"
+0001b8a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001b8b0: 6c66 2e46 312e 7365 7454 6f6f 6c54 6970  lf.F1.setToolTip
+0001b8c0: 2873 656c 662e 666b 6579 735b 2246 3122  (self.fkeys["F1"
+0001b8d0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+0001b8e0: 2022 4632 2220 696e 206b 6579 733a 0a20   "F2" in keys:. 
+0001b8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001b900: 4632 2e73 6574 5465 7874 2866 2246 323a  F2.setText(f"F2:
+0001b910: 207b 7365 6c66 2e66 6b65 7973 5b27 4632   {self.fkeys['F2
+0001b920: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+0001b930: 2020 2020 2073 656c 662e 4632 2e73 6574       self.F2.set
+0001b940: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+0001b950: 7973 5b22 4632 225d 5b31 5d29 0a20 2020  ys["F2"][1]).   
+0001b960: 2020 2020 2069 6620 2246 3322 2069 6e20       if "F3" in 
+0001b970: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+0001b980: 2020 7365 6c66 2e46 332e 7365 7454 6578    self.F3.setTex
+0001b990: 7428 6622 4633 3a20 7b73 656c 662e 666b  t(f"F3: {self.fk
+0001b9a0: 6579 735b 2746 3327 5d5b 305d 7d22 290a  eys['F3'][0]}").
+0001b9b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b9c0: 2e46 332e 7365 7454 6f6f 6c54 6970 2873  .F3.setToolTip(s
+0001b9d0: 656c 662e 666b 6579 735b 2246 3322 5d5b  elf.fkeys["F3"][
+0001b9e0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+0001b9f0: 4634 2220 696e 206b 6579 733a 0a20 2020  F4" in keys:.   
+0001ba00: 2020 2020 2020 2020 2073 656c 662e 4634           self.F4
+0001ba10: 2e73 6574 5465 7874 2866 2246 343a 207b  .setText(f"F4: {
+0001ba20: 7365 6c66 2e66 6b65 7973 5b27 4634 275d  self.fkeys['F4']
+0001ba30: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+0001ba40: 2020 2073 656c 662e 4634 2e73 6574 546f     self.F4.setTo
+0001ba50: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+0001ba60: 5b22 4634 225d 5b31 5d29 0a20 2020 2020  ["F4"][1]).     
+0001ba70: 2020 2069 6620 2246 3522 2069 6e20 6b65     if "F5" in ke
+0001ba80: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+0001ba90: 7365 6c66 2e46 352e 7365 7454 6578 7428  self.F5.setText(
+0001baa0: 6622 4635 3a20 7b73 656c 662e 666b 6579  f"F5: {self.fkey
+0001bab0: 735b 2746 3527 5d5b 305d 7d22 290a 2020  s['F5'][0]}").  
+0001bac0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+0001bad0: 352e 7365 7454 6f6f 6c54 6970 2873 656c  5.setToolTip(sel
+0001bae0: 662e 666b 6579 735b 2246 3522 5d5b 315d  f.fkeys["F5"][1]
+0001baf0: 290a 2020 2020 2020 2020 6966 2022 4636  ).        if "F6
+0001bb00: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+0001bb10: 2020 2020 2020 2073 656c 662e 4636 2e73         self.F6.s
+0001bb20: 6574 5465 7874 2866 2246 363a 207b 7365  etText(f"F6: {se
+0001bb30: 6c66 2e66 6b65 7973 5b27 4636 275d 5b30  lf.fkeys['F6'][0
+0001bb40: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+0001bb50: 2073 656c 662e 4636 2e73 6574 546f 6f6c   self.F6.setTool
+0001bb60: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+0001bb70: 4636 225d 5b31 5d29 0a20 2020 2020 2020  F6"][1]).       
+0001bb80: 2069 6620 2246 3722 2069 6e20 6b65 7973   if "F7" in keys
+0001bb90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001bba0: 6c66 2e46 372e 7365 7454 6578 7428 6622  lf.F7.setText(f"
+0001bbb0: 4637 3a20 7b73 656c 662e 666b 6579 735b  F7: {self.fkeys[
+0001bbc0: 2746 3727 5d5b 305d 7d22 290a 2020 2020  'F7'][0]}").    
+0001bbd0: 2020 2020 2020 2020 7365 6c66 2e46 372e          self.F7.
+0001bbe0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+0001bbf0: 666b 6579 735b 2246 3722 5d5b 315d 290a  fkeys["F7"][1]).
+0001bc00: 2020 2020 2020 2020 6966 2022 4638 2220          if "F8" 
+0001bc10: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
+0001bc20: 2020 2020 2073 656c 662e 4638 2e73 6574       self.F8.set
+0001bc30: 5465 7874 2866 2246 383a 207b 7365 6c66  Text(f"F8: {self
+0001bc40: 2e66 6b65 7973 5b27 4638 275d 5b30 5d7d  .fkeys['F8'][0]}
+0001bc50: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+0001bc60: 656c 662e 4638 2e73 6574 546f 6f6c 5469  elf.F8.setToolTi
+0001bc70: 7028 7365 6c66 2e66 6b65 7973 5b22 4638  p(self.fkeys["F8
+0001bc80: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
+0001bc90: 6620 2246 3922 2069 6e20 6b65 7973 3a0a  f "F9" in keys:.
+0001bca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001bcb0: 2e46 392e 7365 7454 6578 7428 6622 4639  .F9.setText(f"F9
+0001bcc0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+0001bcd0: 3927 5d5b 305d 7d22 290a 2020 2020 2020  9'][0]}").      
+0001bce0: 2020 2020 2020 7365 6c66 2e46 392e 7365        self.F9.se
+0001bcf0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+0001bd00: 6579 735b 2246 3922 5d5b 315d 290a 2020  eys["F9"][1]).  
+0001bd10: 2020 2020 2020 6966 2022 4631 3022 2069        if "F10" i
+0001bd20: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+0001bd30: 2020 2020 7365 6c66 2e46 3130 2e73 6574      self.F10.set
+0001bd40: 5465 7874 2866 2246 3130 3a20 7b73 656c  Text(f"F10: {sel
+0001bd50: 662e 666b 6579 735b 2746 3130 275d 5b30  f.fkeys['F10'][0
+0001bd60: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+0001bd70: 2073 656c 662e 4631 302e 7365 7454 6f6f   self.F10.setToo
+0001bd80: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+0001bd90: 2246 3130 225d 5b31 5d29 0a20 2020 2020  "F10"][1]).     
+0001bda0: 2020 2069 6620 2246 3131 2220 696e 206b     if "F11" in k
+0001bdb0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+0001bdc0: 2073 656c 662e 4631 312e 7365 7454 6578   self.F11.setTex
+0001bdd0: 7428 6622 4631 313a 207b 7365 6c66 2e66  t(f"F11: {self.f
+0001bde0: 6b65 7973 5b27 4631 3127 5d5b 305d 7d22  keys['F11'][0]}"
+0001bdf0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001be00: 6c66 2e46 3131 2e73 6574 546f 6f6c 5469  lf.F11.setToolTi
+0001be10: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
+0001be20: 3122 5d5b 315d 290a 2020 2020 2020 2020  1"][1]).        
+0001be30: 6966 2022 4631 3222 2069 6e20 6b65 7973  if "F12" in keys
+0001be40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001be50: 6c66 2e46 3132 2e73 6574 5465 7874 2866  lf.F12.setText(f
+0001be60: 2246 3132 3a20 7b73 656c 662e 666b 6579  "F12: {self.fkey
+0001be70: 735b 2746 3132 275d 5b30 5d7d 2229 0a20  s['F12'][0]}"). 
+0001be80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001be90: 4631 322e 7365 7454 6f6f 6c54 6970 2873  F12.setToolTip(s
+0001bea0: 656c 662e 666b 6579 735b 2246 3132 225d  elf.fkeys["F12"]
+0001beb0: 5b31 5d29 0a0a 2020 2020 6465 6620 6765  [1])..    def ge
+0001bec0: 6e65 7261 7465 5f61 6469 6628 7365 6c66  nerate_adif(self
+0001bed0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0001bee0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0001bef0: 616c 6c73 2074 6865 2063 6f6e 7465 7374  alls the contest
+0001bf00: 2041 4449 4620 6669 6c65 2067 656e 6572   ADIF file gener
+0001bf10: 6174 6f72 2e0a 0a20 2020 2020 2020 2050  ator...        P
+0001bf20: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0001bf30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001bf40: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+0001bf50: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0001bf60: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0001bf70: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+0001bf80: 2222 220a 0a20 2020 2020 2020 2023 2068  """..        # h
+0001bf90: 7474 7073 3a2f 2f77 7777 2e61 6469 662e  ttps://www.adif.
+0001bfa0: 6f72 672f 3331 352f 4144 4946 5f33 3135  org/315/ADIF_315
+0001bfb0: 2e68 746d 0a20 2020 2020 2020 206c 6f67  .htm.        log
+0001bfc0: 6765 722e 6465 6275 6728 222a 2a2a 2a2a  ger.debug("*****
+0001bfd0: 2a41 4449 462a 2a2a 2a2a 2229 0a20 2020  *ADIF*****").   
+0001bfe0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+0001bff0: 742e 6164 6966 2873 656c 6629 0a0a 2020  t.adif(self)..  
+0001c000: 2020 6465 6620 6765 6e65 7261 7465 5f63    def generate_c
+0001c010: 6162 7269 6c6c 6f28 7365 6c66 2920 2d3e  abrillo(self) ->
+0001c020: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0001c030: 2222 0a20 2020 2020 2020 2043 616c 6c73  "".        Calls
+0001c040: 2074 6865 2063 6f6e 7465 7374 2043 6162   the contest Cab
+0001c050: 7269 6c6c 6f20 6669 6c65 2067 656e 6572  rillo file gener
+0001c060: 6174 6f72 2e20 4d61 7962 652e 0a0a 2020  ator. Maybe...  
+0001c070: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0001c080: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0001c090: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+0001c0a0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0001c0b0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001c0c0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+0001c0d0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+0001c0e0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0001c0f0: 2822 2a2a 2a2a 2a2a 4361 6272 696c 6c6f  ("******Cabrillo
+0001c100: 2a2a 2a2a 2a22 290a 2020 2020 2020 2020  *****").        
+0001c110: 7365 6c66 2e63 6f6e 7465 7374 2e63 6162  self.contest.cab
+0001c120: 7269 6c6c 6f28 7365 6c66 290a 0a0a 6465  rillo(self)...de
+0001c130: 6620 6c6f 6164 5f66 6f6e 7473 5f66 726f  f load_fonts_fro
+0001c140: 6d5f 6469 7228 6469 7265 6374 6f72 793a  m_dir(directory:
+0001c150: 2073 7472 2920 2d3e 2073 6574 3a0a 2020   str) -> set:.  
+0001c160: 2020 2222 220a 2020 2020 5765 6c6c 2069    """.    Well i
+0001c170: 7420 6c6f 6164 7320 666f 6e74 7320 6672  t loads fonts fr
+0001c180: 6f6d 2061 2064 6972 6563 746f 7279 2e2e  om a directory..
+0001c190: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+0001c1a0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0001c1b0: 0a20 2020 2064 6972 6563 746f 7279 203a  .    directory :
+0001c1c0: 2073 7472 0a20 2020 2054 6865 2064 6972   str.    The dir
+0001c1d0: 6563 746f 7279 2074 6f20 6c6f 6164 2066  ectory to load f
+0001c1e0: 6f6e 7473 2066 726f 6d2e 0a0a 2020 2020  onts from...    
+0001c1f0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+0001c200: 2d2d 2d0a 2020 2020 7365 740a 2020 2020  ---.    set.    
+0001c210: 4120 7365 7420 6f66 2066 6f6e 7420 6661  A set of font fa
+0001c220: 6d69 6c69 6573 2069 6e73 7461 6c6c 6564  milies installed
+0001c230: 2069 6e20 7468 6520 6469 7265 6374 6f72   in the director
+0001c240: 792e 0a20 2020 2022 2222 0a20 2020 2066  y..    """.    f
+0001c250: 6f6e 745f 6661 6d69 6c69 6573 203d 2073  ont_families = s
+0001c260: 6574 2829 0a20 2020 2066 6f72 205f 6669  et().    for _fi
+0001c270: 2069 6e20 5144 6972 2864 6972 6563 746f   in QDir(directo
+0001c280: 7279 292e 656e 7472 7949 6e66 6f4c 6973  ry).entryInfoLis
+0001c290: 7428 5b22 2a2e 7474 6622 2c20 222a 2e77  t(["*.ttf", "*.w
+0001c2a0: 6f66 6622 2c20 222a 2e77 6f66 6632 225d  off", "*.woff2"]
+0001c2b0: 293a 0a20 2020 2020 2020 205f 6964 203d  ):.        _id =
+0001c2c0: 2051 466f 6e74 4461 7461 6261 7365 2e61   QFontDatabase.a
+0001c2d0: 6464 4170 706c 6963 6174 696f 6e46 6f6e  ddApplicationFon
+0001c2e0: 7428 5f66 692e 6162 736f 6c75 7465 4669  t(_fi.absoluteFi
+0001c2f0: 6c65 5061 7468 2829 290a 2020 2020 2020  lePath()).      
+0001c300: 2020 666f 6e74 5f66 616d 696c 6965 7320    font_families 
+0001c310: 7c3d 2073 6574 2851 466f 6e74 4461 7461  |= set(QFontData
+0001c320: 6261 7365 2e61 7070 6c69 6361 7469 6f6e  base.application
+0001c330: 466f 6e74 4661 6d69 6c69 6573 285f 6964  FontFamilies(_id
+0001c340: 2929 0a20 2020 2072 6574 7572 6e20 666f  )).    return fo
+0001c350: 6e74 5f66 616d 696c 6965 730a 0a0a 6465  nt_families...de
+0001c360: 6620 696e 7374 616c 6c5f 6963 6f6e 7328  f install_icons(
+0001c370: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+0001c380: 2222 496e 7374 616c 6c20 6963 6f6e 7322  ""Install icons"
+0001c390: 2222 0a0a 2020 2020 6966 2073 7973 2e70  ""..    if sys.p
+0001c3a0: 6c61 7466 6f72 6d20 3d3d 2022 6c69 6e75  latform == "linu
+0001c3b0: 7822 3a0a 2020 2020 2020 2020 6f73 2e73  x":.        os.s
+0001c3c0: 7973 7465 6d28 0a20 2020 2020 2020 2020  ystem(.         
+0001c3d0: 2020 2022 7864 672d 6963 6f6e 2d72 6573     "xdg-icon-res
+0001c3e0: 6f75 7263 6520 696e 7374 616c 6c20 2d2d  ource install --
+0001c3f0: 7369 7a65 2033 3220 2d2d 636f 6e74 6578  size 32 --contex
+0001c400: 7420 6170 7073 202d 2d6d 6f64 6520 7573  t apps --mode us
+0001c410: 6572 2022 0a20 2020 2020 2020 2020 2020  er ".           
+0001c420: 2066 227b 6673 7574 696c 732e 4d4f 4455   f"{fsutils.MODU
+0001c430: 4c45 5f50 4154 487d 2f64 6174 612f 6b36  LE_PATH}/data/k6
+0001c440: 6774 652e 6e6f 7431 6d6d 2d33 322e 706e  gte.not1mm-32.pn
+0001c450: 6720 6b36 6774 652d 6e6f 7431 6d6d 220a  g k6gte-not1mm".
+0001c460: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001c470: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
+0001c480: 2020 2020 2020 2020 2022 7864 672d 6963           "xdg-ic
+0001c490: 6f6e 2d72 6573 6f75 7263 6520 696e 7374  on-resource inst
+0001c4a0: 616c 6c20 2d2d 7369 7a65 2036 3420 2d2d  all --size 64 --
+0001c4b0: 636f 6e74 6578 7420 6170 7073 202d 2d6d  context apps --m
+0001c4c0: 6f64 6520 7573 6572 2022 0a20 2020 2020  ode user ".     
+0001c4d0: 2020 2020 2020 2066 227b 6673 7574 696c         f"{fsutil
+0001c4e0: 732e 4d4f 4455 4c45 5f50 4154 487d 2f64  s.MODULE_PATH}/d
+0001c4f0: 6174 612f 6b36 6774 652e 6e6f 7431 6d6d  ata/k6gte.not1mm
+0001c500: 2d36 342e 706e 6720 6b36 6774 652d 6e6f  -64.png k6gte-no
+0001c510: 7431 6d6d 220a 2020 2020 2020 2020 290a  t1mm".        ).
+0001c520: 2020 2020 2020 2020 6f73 2e73 7973 7465          os.syste
+0001c530: 6d28 0a20 2020 2020 2020 2020 2020 2022  m(.            "
+0001c540: 7864 672d 6963 6f6e 2d72 6573 6f75 7263  xdg-icon-resourc
+0001c550: 6520 696e 7374 616c 6c20 2d2d 7369 7a65  e install --size
+0001c560: 2031 3238 202d 2d63 6f6e 7465 7874 2061   128 --context a
+0001c570: 7070 7320 2d2d 6d6f 6465 2075 7365 7220  pps --mode user 
+0001c580: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
+0001c590: 7b66 7375 7469 6c73 2e4d 4f44 554c 455f  {fsutils.MODULE_
+0001c5a0: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+0001c5b0: 2e6e 6f74 316d 6d2d 3132 382e 706e 6720  .not1mm-128.png 
+0001c5c0: 6b36 6774 652d 6e6f 7431 6d6d 220a 2020  k6gte-not1mm".  
+0001c5d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c5e0: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
+0001c5f0: 2020 2020 2020 2066 2278 6467 2d64 6573         f"xdg-des
+0001c600: 6b74 6f70 2d6d 656e 7520 696e 7374 616c  ktop-menu instal
+0001c610: 6c20 7b66 7375 7469 6c73 2e4d 4f44 554c  l {fsutils.MODUL
+0001c620: 455f 5041 5448 7d2f 6461 7461 2f6b 3667  E_PATH}/data/k6g
+0001c630: 7465 2d6e 6f74 316d 6d2e 6465 736b 746f  te-not1mm.deskto
+0001c640: 7022 0a20 2020 2020 2020 2029 0a0a 0a64  p".        )...d
+0001c650: 6566 2064 6f69 6d70 286d 6f64 6e61 6d65  ef doimp(modname
+0001c660: 2920 2d3e 206f 626a 6563 743a 0a20 2020  ) -> object:.   
+0001c670: 2022 2222 0a20 2020 2049 6d70 6f72 7473   """.    Imports
+0001c680: 2061 206d 6f64 756c 652e 0a0a 2020 2020   a module...    
+0001c690: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0001c6a0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6d6f  ---------.    mo
+0001c6b0: 646e 616d 6520 3a20 7374 720a 2020 2020  dname : str.    
+0001c6c0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+0001c6d0: 6d6f 6475 6c65 2074 6f20 696d 706f 7274  module to import
+0001c6e0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0001c6f0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 206f     -------.    o
+0001c700: 626a 6563 740a 2020 2020 5468 6520 6d6f  bject.    The mo
+0001c710: 6475 6c65 206f 626a 6563 742e 0a20 2020  dule object..   
+0001c720: 2022 2222 0a0a 2020 2020 6c6f 6767 6572   """..    logger
+0001c730: 2e64 6562 7567 2822 646f 696d 703a 2025  .debug("doimp: %
+0001c740: 7322 2c20 6d6f 646e 616d 6529 0a20 2020  s", modname).   
+0001c750: 2072 6574 7572 6e20 696d 706f 7274 6c69   return importli
+0001c760: 622e 696d 706f 7274 5f6d 6f64 756c 6528  b.import_module(
+0001c770: 6622 6e6f 7431 6d6d 2e70 6c75 6769 6e73  f"not1mm.plugins
+0001c780: 2e7b 6d6f 646e 616d 657d 2229 0a0a 0a64  .{modname}")...d
+0001c790: 6566 2072 756e 2829 202d 3e20 4e6f 6e65  ef run() -> None
+0001c7a0: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
+0001c7b0: 696e 2045 6e74 7279 0a20 2020 2022 2222  in Entry.    """
+0001c7c0: 0a20 2020 206c 6f67 6765 722e 6465 6275  .    logger.debu
+0001c7d0: 6728 0a20 2020 2020 2020 2066 2252 6573  g(.        f"Res
+0001c7e0: 6f6c 7665 6420 4f53 2066 696c 6520 7379  olved OS file sy
+0001c7f0: 7374 656d 2070 6174 6873 3a20 4d4f 4455  stem paths: MODU
+0001c800: 4c45 5f50 4154 4820 7b66 7375 7469 6c73  LE_PATH {fsutils
+0001c810: 2e4d 4f44 554c 455f 5041 5448 7d2c 2055  .MODULE_PATH}, U
+0001c820: 5345 525f 4441 5441 5f50 4154 4820 7b66  SER_DATA_PATH {f
+0001c830: 7375 7469 6c73 2e55 5345 525f 4441 5441  sutils.USER_DATA
+0001c840: 5f50 4154 487d 2c20 434f 4e46 4947 5f50  _PATH}, CONFIG_P
+0001c850: 4154 4820 7b66 7375 7469 6c73 2e43 4f4e  ATH {fsutils.CON
+0001c860: 4649 475f 5041 5448 7d22 0a20 2020 2029  FIG_PATH}".    )
+0001c870: 0a20 2020 2069 6e73 7461 6c6c 5f69 636f  .    install_ico
+0001c880: 6e73 2829 0a20 2020 2074 696d 6572 2e73  ns().    timer.s
+0001c890: 7461 7274 2832 3530 290a 2020 2020 7379  tart(250).    sy
+0001c8a0: 732e 6578 6974 2861 7070 2e65 7865 6328  s.exit(app.exec(
+0001c8b0: 2929 0a0a 0a44 4542 5547 5f45 4e41 424c  ))...DEBUG_ENABL
+0001c8c0: 4544 203d 2046 616c 7365 0a69 6620 5061  ED = False.if Pa
+0001c8d0: 7468 2822 2e2f 6465 6275 6722 292e 6578  th("./debug").ex
+0001c8e0: 6973 7473 2829 3a0a 2020 2020 4445 4255  ists():.    DEBU
+0001c8f0: 475f 454e 4142 4c45 4420 3d20 5472 7565  G_ENABLED = True
+0001c900: 0a0a 6c6f 6767 6572 203d 206c 6f67 6769  ..logger = loggi
+0001c910: 6e67 2e67 6574 4c6f 6767 6572 2822 5f5f  ng.getLogger("__
+0001c920: 6d61 696e 5f5f 2229 0a0a 6c6f 6767 696e  main__")..loggin
+0001c930: 672e 6261 7369 6343 6f6e 6669 6728 0a20  g.basicConfig(. 
+0001c940: 2020 206c 6576 656c 3d6c 6f67 6769 6e67     level=logging
+0001c950: 2e44 4542 5547 2069 6620 4445 4255 475f  .DEBUG if DEBUG_
+0001c960: 454e 4142 4c45 4420 656c 7365 206c 6f67  ENABLED else log
+0001c970: 6769 6e67 2e43 5249 5449 4341 4c2c 0a20  ging.CRITICAL,. 
+0001c980: 2020 2066 6f72 6d61 743d 225b 2528 6173     format="[%(as
+0001c990: 6374 696d 6529 735d 2025 286c 6576 656c  ctime)s] %(level
+0001c9a0: 6e61 6d65 2973 2025 286e 616d 6529 7320  name)s %(name)s 
+0001c9b0: 2d20 2528 6675 6e63 4e61 6d65 2973 204c  - %(funcName)s L
+0001c9c0: 696e 6520 2528 6c69 6e65 6e6f 2964 3a20  ine %(lineno)d: 
+0001c9d0: 2528 6d65 7373 6167 6529 7322 2c0a 2020  %(message)s",.  
+0001c9e0: 2020 6861 6e64 6c65 7273 3d5b 0a20 2020    handlers=[.   
+0001c9f0: 2020 2020 2052 6f74 6174 696e 6746 696c       RotatingFil
+0001ca00: 6548 616e 646c 6572 2866 7375 7469 6c73  eHandler(fsutils
+0001ca10: 2e4c 4f47 5f46 494c 452c 206d 6178 4279  .LOG_FILE, maxBy
+0001ca20: 7465 733d 3130 3439 3030 3030 2c20 6261  tes=10490000, ba
+0001ca30: 636b 7570 436f 756e 743d 3230 292c 0a20  ckupCount=20),. 
+0001ca40: 2020 2020 2020 206c 6f67 6769 6e67 2e53         logging.S
+0001ca50: 7472 6561 6d48 616e 646c 6572 2829 2c0a  treamHandler(),.
+0001ca60: 2020 2020 5d2c 0a29 0a6c 6f67 6769 6e67      ],.).logging
+0001ca70: 2e67 6574 4c6f 6767 6572 2822 5079 5174  .getLogger("PyQt
+0001ca80: 352e 7569 632e 7569 7061 7273 6572 2229  5.uic.uiparser")
+0001ca90: 2e73 6574 4c65 7665 6c28 2249 4e46 4f22  .setLevel("INFO"
+0001caa0: 290a 6c6f 6767 696e 672e 6765 744c 6f67  ).logging.getLog
+0001cab0: 6765 7228 2250 7951 7435 2e75 6963 2e70  ger("PyQt5.uic.p
+0001cac0: 726f 7065 7274 6965 7322 292e 7365 744c  roperties").setL
+0001cad0: 6576 656c 2822 494e 464f 2229 0a61 7070  evel("INFO").app
+0001cae0: 203d 2051 7457 6964 6765 7473 2e51 4170   = QtWidgets.QAp
+0001caf0: 706c 6963 6174 696f 6e28 7379 732e 6172  plication(sys.ar
+0001cb00: 6776 290a 6661 6d69 6c69 6573 203d 206c  gv).families = l
+0001cb10: 6f61 645f 666f 6e74 735f 6672 6f6d 5f64  oad_fonts_from_d
+0001cb20: 6972 286f 732e 6673 7061 7468 2866 7375  ir(os.fspath(fsu
+0001cb30: 7469 6c73 2e41 5050 5f44 4154 415f 5041  tils.APP_DATA_PA
+0001cb40: 5448 2929 0a6c 6f67 6765 722e 696e 666f  TH)).logger.info
+0001cb50: 2866 2266 6f6e 7420 6661 6d69 6c69 6573  (f"font families
+0001cb60: 207b 6661 6d69 6c69 6573 7d22 290a 7769   {families}").wi
+0001cb70: 6e64 6f77 203d 204d 6169 6e57 696e 646f  ndow = MainWindo
+0001cb80: 7728 290a 6865 6967 6874 203d 2077 696e  w().height = win
+0001cb90: 646f 772e 7072 6566 2e67 6574 2822 7769  dow.pref.get("wi
+0001cba0: 6e64 6f77 5f68 6569 6768 7422 2c20 3330  ndow_height", 30
+0001cbb0: 3029 0a77 6964 7468 203d 2077 696e 646f  0).width = windo
+0001cbc0: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
+0001cbd0: 6f77 5f77 6964 7468 222c 2037 3030 290a  ow_width", 700).
+0001cbe0: 7820 3d20 7769 6e64 6f77 2e70 7265 662e  x = window.pref.
+0001cbf0: 6765 7428 2277 696e 646f 775f 7822 2c20  get("window_x", 
+0001cc00: 2d31 290a 7920 3d20 7769 6e64 6f77 2e70  -1).y = window.p
+0001cc10: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
+0001cc20: 7922 2c20 2d31 290a 7769 6e64 6f77 2e73  y", -1).window.s
+0001cc30: 6574 4765 6f6d 6574 7279 2878 2c20 792c  etGeometry(x, y,
+0001cc40: 2077 6964 7468 2c20 6865 6967 6874 290a   width, height).
+0001cc50: 7769 6e64 6f77 2e63 616c 6c73 6967 6e2e  window.callsign.
+0001cc60: 7365 7446 6f63 7573 2829 0a77 696e 646f  setFocus().windo
+0001cc70: 772e 7368 6f77 2829 0a74 696d 6572 203d  w.show().timer =
+0001cc80: 2051 7443 6f72 652e 5154 696d 6572 2829   QtCore.QTimer()
+0001cc90: 0a74 696d 6572 2e74 696d 656f 7574 2e63  .timer.timeout.c
+0001cca0: 6f6e 6e65 6374 2877 696e 646f 772e 706f  onnect(window.po
+0001ccb0: 6c6c 5f72 6164 696f 290a 0a69 6620 5f5f  ll_radio)..if __
+0001ccc0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
+0001ccd0: 6e5f 5f22 3a0a 2020 2020 7275 6e28 290a  n__":.    run().
```

### Comparing `not1mm-24.4.1/not1mm/bandmap.py` & `not1mm-24.4.1.1/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/checkwindow.py` & `not1mm-24.4.1.1/not1mm/checkwindow.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,54 +6,56 @@
 # pylint: disable=logging-fstring-interpolation, line-too-long
 
 import logging
 import os
 import platform
 import queue
 from json import loads
+import Levenshtein
 
 from PyQt5 import QtGui, uic
 from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QWidget
+from PyQt5.QtWidgets import QLabel, QVBoxLayout, QWidget, QDockWidget
+from PyQt5.QtGui import QMouseEvent
 
 import not1mm.fsutils as fsutils
 from not1mm.lib.database import DataBase
 from not1mm.lib.multicast import Multicast
 from not1mm.lib.super_check_partial import SCP
 
 logger = logging.getLogger(__name__)
 
 
-class CheckWindow(QWidget):
+class CheckWindow(QDockWidget):
     """The check window. Shows list or probable stations."""
 
     multicast_interface = None
     dbname = None
     pref = {}
+    call = None
+    masterLayout: QVBoxLayout = None
+    dxcLayout: QVBoxLayout = None
+    qsoLayout: QVBoxLayout = None
+
+    character_remove_color = "#cc3333"
+    character_add_color = "#3333cc"
+
+    masterScrollWidget: QWidget = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.load_pref()
         self.dbname = fsutils.USER_DATA_PATH / self.pref.get(
             "current_database", "ham.db"
         )
         self.database = DataBase(self.dbname, fsutils.APP_DATA_PATH)
         self.database.current_contest = self.pref.get("contest", 0)
 
         uic.loadUi(fsutils.APP_DATA_PATH / "checkwindow.ui", self)
 
-        self.logList.clear()
-        self.logList.itemClicked.connect(self.item_clicked)
-        self.masterList.clear()
-        self.masterList.itemClicked.connect(self.item_clicked)
-        self.telnetList.clear()
-        self.telnetList.itemClicked.connect(self.item_clicked)
-        self.callhistoryList.clear()
-        self.callhistoryList.hide()
-        self.callhistoryListLabel.hide()
         self.mscp = SCP(fsutils.APP_DATA_PATH)
         self._udpwatch = None
         self.udp_fifo = queue.Queue()
         self.multicast_interface = Multicast(
             self.pref.get("multicast_group", "239.1.1.1"),
             self.pref.get("multicast_port", 2239),
             self.pref.get("interface_ip", "0,0,0,0"),
@@ -62,15 +64,15 @@
 
     def item_clicked(self, item):
         """docstring for item_clicked"""
         if item:
             cmd = {}
             cmd["cmd"] = "CHANGECALL"
             cmd["station"] = platform.node()
-            cmd["call"] = item.text()
+            cmd["call"] = item
             self.multicast_interface.send_as_json(cmd)
 
     def setDarkMode(self, dark: bool):
         """Forces a darkmode palette."""
 
         if dark:
             darkPalette = QtGui.QPalette()
@@ -94,14 +96,15 @@
             darkPalette.setColor(QtGui.QPalette.Highlight, QtGui.QColor(42, 130, 218))
             darkPalette.setColor(QtGui.QPalette.HighlightedText, Qt.black)
             darkPalette.setColor(
                 QtGui.QPalette.Disabled, QtGui.QPalette.HighlightedText, disabledColor
             )
 
             self.setPalette(darkPalette)
+            # self.CheckPartialWindow.setPalette(darkPalette)
         else:
             palette = self.style().standardPalette()
             self.setPalette(palette)
 
     def load_pref(self) -> None:
         """
         Load preference file to get current db filename and sets the initial darkmode state.
@@ -146,19 +149,20 @@
 
             if json_data.get("station", "") != platform.node():
                 continue
             if json_data.get("cmd", "") == "UPDATELOG":
                 self.clear_lists()
             if json_data.get("cmd", "") == "CALLCHANGED":
                 call = json_data.get("call", "")
+                self.call = call
                 self.master_list(call)
                 self.log_list(call)
                 continue
             if json_data.get("cmd", "") == "CHECKSPOTS":
-                self.telnetList.clear()
+                self.populate_layout(self.dxcLayout, [])
                 spots = json_data.get("spots", [])
                 self.telnet_list(spots)
                 continue
             if json_data.get("cmd", "") == "NEWDB":
                 ...
                 # self.load_new_db()
 
@@ -173,71 +177,118 @@
         ----------
         None
 
         Returns
         -------
         None
         """
-        self.logList.clear()
-        self.masterList.clear()
-        self.telnetList.clear()
-        self.callhistoryList.clear()
+        self.populate_layout(self.masterLayout, [])
+        self.populate_layout(self.qsoLayout, [])
+        self.populate_layout(self.dxcLayout, [])
 
     def master_list(self, call: str) -> None:
         """
         Get MASTER.SCP matches to call and display in list.
 
         Parameters
         ----------
         call : str
         Call to get matches for
 
         Returns
         -------
         None
         """
+        self.populate_layout(self.masterLayout, [])
         results = self.mscp.super_check(call)
-        self.masterList.clear()
-        for item in results:
-            if "#" in item:
-                continue
-            self.masterList.addItem(item)
-        self.masterList.show()
+        self.populate_layout(self.masterLayout, filter(lambda x: "#" not in x, results))
 
     def log_list(self, call: str) -> None:
         """
         Get log matches to call and display in list.
 
         Parameters
         ----------
         call : str
         Call to get matches for
 
         Returns
         -------
         None
         """
-        self.logList.clear()
+        self.populate_layout(self.qsoLayout, [])
         if call:
             result = self.database.get_like_calls_and_bands(call)
-            self.logList.addItems(result)
-            self.logList.show()
+            self.populate_layout(self.qsoLayout, result)
 
     def telnet_list(self, spots: list) -> None:
         """
         Get telnet matches to call and display in list.
 
         Parameters
         ----------
         spots : list
         List of spots to get matches for
 
         Returns
         -------
         None
         """
-        self.telnetList.clear()
+        self.populate_layout(self.dxcLayout, [])
         if spots:
-            for calls in spots:
-                call = calls.get("callsign", "")
-                self.telnetList.addItem(call)
-            self.telnetList.show()
+            self.populate_layout(
+                self.dxcLayout,
+                filter(lambda x: x, [x.get("callsign", None) for x in spots]),
+            )
+
+    def populate_layout(self, layout, call_list):
+        for i in reversed(range(layout.count())):
+            if layout.itemAt(i).widget():
+                layout.itemAt(i).widget().setParent(None)
+            else:
+                layout.removeItem(layout.itemAt(i))
+        labels = []
+        for call in call_list:
+            if call:
+                if self.call:
+                    label_text = ""
+                    for tag, i1, i2, j1, j2 in Levenshtein.opcodes(call, self.call):
+                        # logger.debug('{:7}   a[{}:{}] --> b[{}:{}] {!r:>8} --> {!r}'.format(
+                        #    tag, i1, i2, j1, j2, call[i1:i2], self.call[j1:j2]))
+                        if tag == "equal":
+                            label_text += call[i1:i2]
+                            continue
+                        elif tag == "replace":
+                            label_text += f"<span style='background-color: {self.character_remove_color};'>{call[i1:i2]}</span>"
+                        elif tag == "insert" or tag == "delete":
+                            label_text += f"<span style='background-color: {self.character_add_color};'>{call[i1:i2]}</span>"
+                    labels.append(
+                        (
+                            Levenshtein.hamming(call, self.call),
+                            CallLabel(
+                                label_text, call=call, callback=self.item_clicked
+                            ),
+                        )
+                    )
+
+        for _, label in sorted(labels, key=lambda x: x[0]):
+            layout.addWidget(label)
+        # top aligns
+        layout.addStretch(0)
+
+
+class CallLabel(QLabel):
+    call: str = None
+
+    def __init__(
+        self,
+        *args,
+        call=None,
+        callback=None,
+    ):
+        super().__init__(*args)
+        self.call = call
+        self.callback = callback
+
+    def mouseDoubleClickEvent(self, e: QMouseEvent) -> None:
+        if self.call and self.callback:
+            self.callback(self.call)
```

### Comparing `not1mm-24.4.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-24.4.1.1/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/MASTER.SCP` & `not1mm-24.4.1.1/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/about.ui` & `not1mm-24.4.1.1/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/bandmap.ui` & `not1mm-24.4.1.1/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/checkwindow.ui` & `not1mm-24.4.1.1/not1mm/data/vfo.ui`

 * *Files 22% similar despite different names*

#### Comparing `not1mm-24.4.1/not1mm/data/checkwindow.ui` & `not1mm-24.4.1.1/not1mm/data/vfo.ui`

```diff
@@ -1,119 +1,53 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>CheckWindow</class>
-  <widget class="QWidget" name="CheckWindow">
+  <class>DockWidget</class>
+  <widget class="QDockWidget" name="DockWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>310</width>
-        <height>600</height>
+        <width>304</width>
+        <height>132</height>
       </rect>
     </property>
-    <property name="font">
-      <font>
-        <family>JetBrains Mono</family>
-        <pointsize>12</pointsize>
-      </font>
-    </property>
     <property name="windowTitle">
-      <string>Check Partial</string>
+      <string>DockWidget</string>
     </property>
-    <layout class="QGridLayout" name="gridLayout">
-      <property name="leftMargin">
-        <number>2</number>
-      </property>
-      <property name="topMargin">
-        <number>2</number>
-      </property>
-      <property name="rightMargin">
-        <number>2</number>
-      </property>
-      <property name="bottomMargin">
-        <number>2</number>
-      </property>
-      <item row="1" column="1">
-        <widget class="QListWidget" name="masterList">
-          <property name="focusPolicy">
-            <enum>Qt::NoFocus</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="1" column="3">
-        <widget class="QListWidget" name="callhistoryList">
-          <property name="focusPolicy">
-            <enum>Qt::NoFocus</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="1" column="2">
-        <widget class="QListWidget" name="telnetList">
-          <property name="focusPolicy">
-            <enum>Qt::NoFocus</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="1" column="0">
-        <widget class="QListWidget" name="logList">
-          <property name="focusPolicy">
-            <enum>Qt::NoFocus</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="0" column="0">
-        <widget class="QLabel" name="logListLabel">
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>10</pointsize>
-            </font>
-          </property>
-          <property name="text">
-            <string>Log</string>
-          </property>
-        </widget>
-      </item>
-      <item row="0" column="1">
-        <widget class="QLabel" name="masterListLabel">
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>10</pointsize>
-            </font>
-          </property>
-          <property name="text">
-            <string>Master</string>
-          </property>
-        </widget>
-      </item>
-      <item row="0" column="2">
-        <widget class="QLabel" name="telnetListLabel">
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>10</pointsize>
-            </font>
-          </property>
-          <property name="text">
-            <string>Telnet</string>
-          </property>
-        </widget>
-      </item>
-      <item row="0" column="3">
-        <widget class="QLabel" name="callhistoryListLabel">
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>10</pointsize>
-            </font>
-          </property>
-          <property name="text">
-            <string>Call</string>
-          </property>
-        </widget>
-      </item>
-    </layout>
+    <widget class="QWidget" name="dockWidgetContents">
+      <layout class="QGridLayout" name="gridLayout_2">
+        <item row="0" column="0">
+          <widget class="QFrame" name="frame">
+            <property name="frameShape">
+              <enum>QFrame::StyledPanel</enum>
+            </property>
+            <property name="frameShadow">
+              <enum>QFrame::Raised</enum>
+            </property>
+            <layout class="QGridLayout" name="gridLayout">
+              <item row="0" column="0">
+                <widget class="QLCDNumber" name="lcdNumber">
+                  <property name="font">
+                    <font>
+                      <pointsize>25</pointsize>
+                    </font>
+                  </property>
+                  <property name="digitCount">
+                    <number>11</number>
+                  </property>
+                  <property name="segmentStyle">
+                    <enum>QLCDNumber::Flat</enum>
+                  </property>
+                  <property name="intValue" stdset="0">
+                    <number>14032000</number>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
+        </item>
+      </layout>
+    </widget>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `not1mm-24.4.1/not1mm/data/configuration.ui` & `not1mm-24.4.1.1/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/contests.sql` & `not1mm-24.4.1.1/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/cty.json` & `not1mm-24.4.1.1/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/editcontact.ui` & `not1mm-24.4.1.1/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/editmacro.ui` & `not1mm-24.4.1.1/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-24.4.1.1/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-24.4.1.1/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-24.4.1.1/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/logwindow.ui` & `not1mm-24.4.1.1/not1mm/data/logwindowx.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/main.ui` & `not1mm-24.4.1.1/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/new_contest.ui` & `not1mm-24.4.1.1/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/not1mm.html` & `not1mm-24.4.1.1/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/opon.ui` & `not1mm-24.4.1.1/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/0.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/1.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/2.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/3.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/4.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/5.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/6.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/7.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/73.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/8.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/9.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/a.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/again.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/b.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/c.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/contest.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/cq.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/d.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/e.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/f.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/g.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/h.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/i.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/j.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/k.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/l.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/m.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/n.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/nil.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/o.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/p.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/q.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/r.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/roger.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/s.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/space.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/t.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/u.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/v.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/w.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/x.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/y.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/phonetics/z.wav` & `not1mm-24.4.1.1/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/pickcontest.ui` & `not1mm-24.4.1.1/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/radio_green.png` & `not1mm-24.4.1.1/not1mm/data/radio_green.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/radio_grey.png` & `not1mm-24.4.1.1/not1mm/data/radio_grey.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/radio_red.png` & `not1mm-24.4.1.1/not1mm/data/radio_red.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/reddot.png` & `not1mm-24.4.1.1/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/settings.ui` & `not1mm-24.4.1.1/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/data/vfo.ui` & `not1mm-24.4.1.1/not1mm/data/logwindow.ui`

 * *Files 24% similar despite different names*

#### Comparing `not1mm-24.4.1/not1mm/data/vfo.ui` & `not1mm-24.4.1.1/not1mm/data/logwindow.ui`

```diff
@@ -1,84 +1,56 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>VfoWindow</class>
-  <widget class="QWidget" name="VfoWindow">
+  <class>DockWidget</class>
+  <widget class="QDockWidget" name="DockWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>570</width>
-        <height>130</height>
+        <width>818</width>
+        <height>374</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>MainWindow</string>
+      <string>DockWidget</string>
     </property>
-    <layout class="QGridLayout" name="gridLayout_3">
-      <item row="0" column="0">
-        <widget class="QMenuBar" name="menubar"/>
-      </item>
-      <item row="1" column="0">
-        <layout class="QGridLayout" name="gridLayout">
-          <item row="0" column="0">
-            <widget class="QFrame" name="frame">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="frameShape">
-                <enum>QFrame::StyledPanel</enum>
-              </property>
-              <property name="frameShadow">
-                <enum>QFrame::Raised</enum>
-              </property>
-              <layout class="QGridLayout" name="gridLayout_2">
-                <item row="0" column="0">
-                  <widget class="QLCDNumber" name="lcdNumber">
-                    <property name="sizePolicy">
-                      <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
-                        <horstretch>0</horstretch>
-                        <verstretch>0</verstretch>
-                      </sizepolicy>
-                    </property>
-                    <property name="font">
-                      <font>
-                        <pointsize>25</pointsize>
-                      </font>
-                    </property>
-                    <property name="autoFillBackground">
-                      <bool>false</bool>
-                    </property>
-                    <property name="smallDecimalPoint">
-                      <bool>false</bool>
-                    </property>
-                    <property name="digitCount">
-                      <number>11</number>
-                    </property>
-                    <property name="mode">
-                      <enum>QLCDNumber::Dec</enum>
-                    </property>
-                    <property name="segmentStyle">
-                      <enum>QLCDNumber::Flat</enum>
-                    </property>
-                    <property name="intValue" stdset="0">
-                      <number>14032000</number>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
+    <widget class="QWidget" name="dockWidgetContents">
+      <layout class="QVBoxLayout" name="verticalLayout">
+        <item>
+          <widget class="QSplitter" name="splitter">
+            <property name="orientation">
+              <enum>Qt::Vertical</enum>
+            </property>
+            <widget class="QTableWidget" name="generalLog">
+              <property name="font">
+                <font>
+                  <family>JetBrains Mono</family>
+                </font>
+              </property>
+              <property name="focusPolicy">
+                <enum>Qt::NoFocus</enum>
+              </property>
+              <property name="tabKeyNavigation">
+                <bool>false</bool>
+              </property>
+            </widget>
+            <widget class="QTableWidget" name="focusedLog">
+              <property name="font">
+                <font>
+                  <family>JetBrains Mono</family>
+                </font>
+              </property>
+              <property name="focusPolicy">
+                <enum>Qt::NoFocus</enum>
+              </property>
+              <property name="tabKeyNavigation">
+                <bool>false</bool>
+              </property>
             </widget>
-          </item>
-        </layout>
-      </item>
-    </layout>
-    <action name="actionQuit">
-      <property name="text">
-        <string>Quit</string>
-      </property>
-    </action>
+          </widget>
+        </item>
+      </layout>
+    </widget>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `not1mm-24.4.1/not1mm/fsutils.py` & `not1mm-24.4.1.1/not1mm/fsutils.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/cat_interface.py` & `not1mm-24.4.1.1/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/cwinterface.py` & `not1mm-24.4.1.1/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/database.py` & `not1mm-24.4.1.1/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/edit_macro.py` & `not1mm-24.4.1.1/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/edit_station.py` & `not1mm-24.4.1.1/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/ham_utility.py` & `not1mm-24.4.1.1/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/lookup.py` & `not1mm-24.4.1.1/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/multicast.py` & `not1mm-24.4.1.1/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/n1mm.py` & `not1mm-24.4.1.1/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/plugin_common.py` & `not1mm-24.4.1.1/not1mm/lib/plugin_common.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/settings.py` & `not1mm-24.4.1.1/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/super_check_partial.py` & `not1mm-24.4.1.1/not1mm/lib/super_check_partial.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/lib/versiontest.py` & `not1mm-24.4.1.1/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/logwindow.py` & `not1mm-24.4.1.1/not1mm/logwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import platform
 import queue
 from json import loads
 
 import math
 from PyQt5 import QtCore, QtGui, QtWidgets, uic
 from PyQt5.QtCore import Qt, QItemSelectionModel
+from PyQt5.QtWidgets import QDockWidget
 
 import not1mm.fsutils as fsutils
 from not1mm.lib.database import DataBase
 from not1mm.lib.edit_contact import EditContact
 from not1mm.lib.multicast import Multicast
 from not1mm.lib.n1mm import N1MM
 
@@ -47,15 +48,15 @@
         except ValueError:
             return default
         except TypeError:
             return default
     return default
 
 
-class LogWindow(QtWidgets.QWidget):
+class LogWindow(QDockWidget):
     """
     The main window
     """
 
     multicast_interface = None
     dbname = None
     edit_contact_dialog = None
```

### Comparing `not1mm-24.4.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-24.4.1.1/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-24.4.1.1/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_10m.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_10m.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_field_day.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_vhf_jan.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_vhf_jan.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_vhf_jun.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_vhf_jun.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/arrl_vhf_sep.py` & `not1mm-24.4.1.1/not1mm/plugins/arrl_vhf_sep.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/canada_day.py` & `not1mm-24.4.1.1/not1mm/plugins/canada_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cq_160_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/cq_160_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cq_160_ssb.py` & `not1mm-24.4.1.1/not1mm/plugins/cq_160_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-24.4.1.1/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-24.4.1.1/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/cwt.py` & `not1mm-24.4.1.1/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/general_logging.py` & `not1mm-24.4.1.1/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/iaru_hf.py` & `not1mm-24.4.1.1/not1mm/plugins/iaru_hf.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/jidx_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/jidx_ph.py` & `not1mm-24.4.1.1/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/naqp_cw.py` & `not1mm-24.4.1.1/not1mm/plugins/naqp_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/naqp_ssb.py` & `not1mm-24.4.1.1/not1mm/plugins/naqp_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/phone_weekly_test.py` & `not1mm-24.4.1.1/not1mm/plugins/phone_weekly_test.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/stew_perry_topband.py` & `not1mm-24.4.1.1/not1mm/plugins/stew_perry_topband.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/plugins/winter_field_day.py` & `not1mm-24.4.1.1/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.1/not1mm/vfo.py` & `not1mm-24.4.1.1/not1mm/vfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 import os
 import platform
 from json import loads, JSONDecodeError
 
 import serial
 from PyQt5 import QtCore, QtGui, QtWidgets, uic
 from PyQt5.QtCore import Qt, QTimer
-from PyQt5.QtWidgets import QWidget
+from PyQt5.QtWidgets import QWidget, QDockWidget
 
 import not1mm.fsutils as fsutils
 from not1mm.lib.cat_interface import CAT
 from not1mm.lib.multicast import Multicast
 
 logger = logging.getLogger(__name__)
 
 
-class VfoWindow(QWidget):
+class VfoWindow(QDockWidget):
     """The VFO window."""
 
     pref = {}
     old_vfo = ""
     old_pico = ""
     message_shown = False
     multicast_interface = None
```

### Comparing `not1mm-24.4.1/not1mm.egg-info/PKG-INFO` & `not1mm-24.4.1.1/not1mm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.1
+Version: 24.4.1.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -24,14 +24,15 @@
 Requires-Dist: pyserial
 Requires-Dist: sounddevice
 Requires-Dist: soundfile
 Requires-Dist: numpy
 Requires-Dist: notctyparser>=23.6.21
 Requires-Dist: rapidfuzz
 Requires-Dist: appdata
+Requires-Dist: Levenshtein
 
 # Not1MM
 
 The worlds #1 unfinished contest logger <sup>*According to my daughter Corinna.<sup>
 
 [![PyPI](https://img.shields.io/pypi/v/not1mm)](https://pypi.org/project/not1mm/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
@@ -172,14 +173,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-1-1] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets.
 - [24-4-1] Removed some un-needed loops and widgets from the check window.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Flatpak
 
 I've tried for a couple days to get not1mm to build as a flatpak. I've failed.
```

### Comparing `not1mm-24.4.1/not1mm.egg-info/SOURCES.txt` & `not1mm-24.4.1.1/not1mm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 not1mm/data/editmacro.ui
 not1mm/data/greendot.png
 not1mm/data/k6gte-not1mm.desktop
 not1mm/data/k6gte.not1mm-128.png
 not1mm/data/k6gte.not1mm-32.png
 not1mm/data/k6gte.not1mm-64.png
 not1mm/data/logwindow.ui
+not1mm/data/logwindowx.ui
 not1mm/data/main.ui
 not1mm/data/new_contest.ui
 not1mm/data/not1mm.html
 not1mm/data/opon.ui
 not1mm/data/pickcontest.ui
 not1mm/data/radio_green.png
 not1mm/data/radio_grey.png
```

### Comparing `not1mm-24.4.1/pyproject.toml` & `not1mm-24.4.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "24.4.1"
+version = "24.4.1.1"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
@@ -20,14 +20,15 @@
     "pyserial",
     "sounddevice",
     "soundfile",
     "numpy",
     "notctyparser >= 23.6.21",
     "rapidfuzz",
     "appdata",
+    "Levenshtein",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Environment :: X11 Applications :: Qt",
     "Operating System :: POSIX :: Linux",
```

