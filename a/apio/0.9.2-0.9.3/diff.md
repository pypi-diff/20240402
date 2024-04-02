# Comparing `tmp/apio-0.9.2.tar.gz` & `tmp/apio-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apio-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apio-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apio-0.9.2.tar` & `apio-0.9.3.tar`

### file list

```diff
@@ -1,130 +1,82 @@
--rw-r--r--   0        0        0      938 2024-03-23 11:42:04.315973 apio-0.9.2/.github/workflows/Publish.yml
--rw-r--r--   0        0        0      583 2024-03-23 11:42:04.315973 apio-0.9.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      330 2024-03-23 11:42:04.315973 apio-0.9.2/.gitignore
--rw-r--r--   0        0        0     6159 2024-03-23 11:42:04.315973 apio-0.9.2/.vscode/launch.json
--rw-r--r--   0        0        0    18047 2024-03-23 11:42:04.315973 apio-0.9.2/LICENSE
--rw-r--r--   0        0        0     1092 2024-03-23 11:42:04.315973 apio-0.9.2/Makefile
--rw-r--r--   0        0        0    10110 2024-03-23 11:42:04.315973 apio-0.9.2/README.md
--rw-r--r--   0        0        0      747 2024-03-23 11:42:04.315973 apio-0.9.2/apio/__init__.py
--rw-r--r--   0        0        0     5145 2024-03-23 11:42:04.315973 apio-0.9.2/apio/__main__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/__init__.py
--rw-r--r--   0        0        0     1211 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/boards.py
--rw-r--r--   0        0        0     3160 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/build.py
--rw-r--r--   0        0        0     1400 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/clean.py
--rw-r--r--   0        0        0     1603 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/config.py
--rw-r--r--   0        0        0     1850 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/drivers.py
--rw-r--r--   0        0        0     2277 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/examples.py
--rw-r--r--   0        0        0     1571 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/graph.py
--rw-r--r--   0        0        0     2341 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/init.py
--rw-r--r--   0        0        0     2642 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/install.py
--rw-r--r--   0        0        0     2035 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/lint.py
--rw-r--r--   0        0        0      530 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/raw.py
--rw-r--r--   0        0        0     1003 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/sim.py
--rw-r--r--   0        0        0     1913 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/system.py
--rw-r--r--   0        0        0     1233 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/test.py
--rw-r--r--   0        0        0     2631 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/time.py
--rw-r--r--   0        0        0     2382 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/uninstall.py
--rw-r--r--   0        0        0     1889 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/upgrade.py
--rw-r--r--   0        0        0     3944 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/upload.py
--rw-r--r--   0        0        0     1473 2024-03-23 11:42:04.319973 apio-0.9.2/apio/commands/verify.py
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/__init__.py
--rw-r--r--   0        0        0    12869 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/arguments.py
--rw-r--r--   0        0        0     3000 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/downloader.py
--rw-r--r--   0        0        0    16246 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/drivers.py
--rw-r--r--   0        0        0    10465 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/examples.py
--rw-r--r--   0        0        0    17535 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/installer.py
--rw-r--r--   0        0        0     7344 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/project.py
--rw-r--r--   0        0        0    35402 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/scons.py
--rw-r--r--   0        0        0     9638 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/system.py
--rw-r--r--   0        0        0     3798 2024-03-23 11:42:04.319973 apio-0.9.2/apio/managers/unpacker.py
--rw-r--r--   0        0        0     6051 2024-03-23 11:42:04.319973 apio-0.9.2/apio/profile.py
--rw-r--r--   0        0        0    14985 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources.py
--rw-r--r--   0        0        0     1225 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/80-fpga-ftdi.rules
--rw-r--r--   0        0        0      356 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/80-fpga-serial.rules
--rw-r--r--   0        0        0    15689 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/boards.json
--rw-r--r--   0        0        0      345 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/distribution.json
--rw-r--r--   0        0        0    13388 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/ecp5/SConstruct
--rw-r--r--   0        0        0     7638 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/fpgas.json
--rw-r--r--   0        0        0    13261 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/ice40/SConstruct
--rw-r--r--   0        0        0     1987 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/packages.json
--rw-r--r--   0        0        0     1639 2024-03-23 11:42:04.319973 apio-0.9.2/apio/resources/programmers.json
--rw-r--r--   0        0        0    25124 2024-03-23 11:42:04.319973 apio-0.9.2/apio/util.py
--rwxr-xr-x   0        0        0      517 2024-03-23 11:42:04.319973 apio-0.9.2/apio_run.py
--rw-r--r--   0        0        0     7648 2024-03-23 11:42:04.319973 apio-0.9.2/docs/Makefile
--rw-r--r--   0        0        0     9219 2024-03-23 11:42:04.319973 apio-0.9.2/docs/conf.py
--rw-r--r--   0        0        0      761 2024-03-23 11:42:04.319973 apio-0.9.2/docs/index.rst
--rw-r--r--   0        0        0    13034 2024-03-23 11:42:04.319973 apio-0.9.2/docs/resources/images/FPGA-wars-logo.png
--rw-r--r--   0        0        0     7143 2024-03-23 11:42:04.319973 apio-0.9.2/docs/resources/images/FPGA-wars-logo.svg
--rw-r--r--   0        0        0    15286 2024-03-23 11:42:04.319973 apio-0.9.2/docs/resources/images/Mac OS Drivers flowchart for iceprog.odg
--rw-r--r--   0        0        0    60542 2024-03-23 11:42:04.319973 apio-0.9.2/docs/resources/images/apio-cheat-sheet.png
--rw-r--r--   0        0        0    34579 2024-03-23 11:42:04.319973 apio-0.9.2/docs/resources/images/apio-cheat-sheet.svg
--rw-r--r--   0        0        0   608059 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-icestorm-hello-world.png
--rw-r--r--   0        0        0     5890 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-logo-mini.png
--rw-r--r--   0        0        0    14376 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-logo.png
--rw-r--r--   0        0        0    16777 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-pio-development-min.png
--rw-r--r--   0        0        0    17950 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-pio-development.png
--rw-r--r--   0        0        0    16348 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-pio-min.png
--rw-r--r--   0        0        0    42962 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio-pio.png
--rw-r--r--   0        0        0    27544 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio.jpg
--rw-r--r--   0        0        0    45464 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/apio.svg
--rw-r--r--   0        0        0    37679 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/gtkwave-simulation.png
--rw-r--r--   0        0        0     1435 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/linux.png
--rw-r--r--   0        0        0    97128 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/macos-drivers-flowchart.png
--rw-r--r--   0        0        0      640 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/macosx.png
--rw-r--r--   0        0        0     1868 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/raspbian.png
--rw-r--r--   0        0        0     1603 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/ubuntu.png
--rw-r--r--   0        0        0      498 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/windows.png
--rw-r--r--   0        0        0    31116 2024-03-23 11:42:04.323973 apio-0.9.2/docs/resources/images/yosys-show.png
--rw-r--r--   0        0        0    64757 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/_static/python-installer-add-path.png
--rw-r--r--   0        0        0       91 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/contribute/index.rst
--rw-r--r--   0        0        0     2692 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/contribute/support_new_board.rst
--rw-r--r--   0        0        0     2782 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/installation.rst
--rw-r--r--   0        0        0     3151 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/quick_start.rst
--rw-r--r--   0        0        0     3384 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0     1553 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_build.rst
--rw-r--r--   0        0        0      654 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_clean.rst
--rw-r--r--   0        0        0     1456 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_lint.rst
--rw-r--r--   0        0        0     1328 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_sim.rst
--rw-r--r--   0        0        0     1928 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_time.rst
--rw-r--r--   0        0        0     2168 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_upload.rst
--rw-r--r--   0        0        0      683 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/project_commands/cmd_verify.rst
--rw-r--r--   0        0        0     1689 2024-03-23 11:42:04.323973 apio-0.9.2/docs/source/user_guide/setup_commands/cmd_drivers.rst
--rw-r--r--   0        0        0     1130 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/setup_commands/cmd_init.rst
--rw-r--r--   0        0        0     5369 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/setup_commands/cmd_install.rst
--rw-r--r--   0        0        0     2555 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/setup_commands/cmd_uninstall.rst
--rw-r--r--   0        0        0     4818 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/util_commands/cmd_boards.rst
--rw-r--r--   0        0        0     1584 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/util_commands/cmd_config.rst
--rw-r--r--   0        0        0     1589 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/util_commands/cmd_examples.rst
--rw-r--r--   0        0        0      554 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/util_commands/cmd_raw.rst
--rw-r--r--   0        0        0     1509 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/util_commands/cmd_system.rst
--rw-r--r--   0        0        0      353 2024-03-23 11:42:04.327973 apio-0.9.2/docs/source/user_guide/util_commands/cmd_upgrade.rst
--rw-r--r--   0        0        0     1182 2024-03-23 11:42:04.327973 apio-0.9.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.363973 apio-0.9.2/test/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/__init__.py
--rw-r--r--   0        0        0     9653 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_build.py
--rw-r--r--   0        0        0     1564 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_clean.py
--rw-r--r--   0        0        0      565 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_graph.py
--rw-r--r--   0        0        0      527 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_lint.py
--rw-r--r--   0        0        0      515 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_sim.py
--rw-r--r--   0        0        0      517 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_test.py
--rw-r--r--   0        0        0     1126 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_time.py
--rw-r--r--   0        0        0     3182 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_upload.py
--rw-r--r--   0        0        0      631 2024-03-23 11:42:04.363973 apio-0.9.2/test/code_commands/test_verify.py
--rw-r--r--   0        0        0     2665 2024-03-23 11:42:04.363973 apio-0.9.2/test/conftest.py
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/__init__.py
--rw-r--r--   0        0        0      754 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_boards.py
--rw-r--r--   0        0        0      769 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_config.py
--rw-r--r--   0        0        0      490 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_drivers.py
--rw-r--r--   0        0        0     1116 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_examples.py
--rw-r--r--   0        0        0     3964 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_init.py
--rw-r--r--   0        0        0      843 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_install.py
--rw-r--r--   0        0        0     1266 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_system.py
--rw-r--r--   0        0        0      949 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_uninstall.py
--rw-r--r--   0        0        0      657 2024-03-23 11:42:04.363973 apio-0.9.2/test/env_commands/test_upgrade.py
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.363973 apio-0.9.2/test/packages/__init__.py
--rw-r--r--   0        0        0     8867 2024-03-23 11:42:04.363973 apio-0.9.2/test/packages/test_complete.py
--rw-r--r--   0        0        0     1741 2024-03-23 11:42:04.363973 apio-0.9.2/test/test_apio.py
--rw-r--r--   0        0        0        0 2024-03-23 11:42:04.363973 apio-0.9.2/test2/__init__.py
--rw-r--r--   0        0        0     2666 2024-03-23 11:42:04.363973 apio-0.9.2/test2/test_ledon.py
--rw-r--r--   0        0        0      268 2024-03-23 11:42:04.363973 apio-0.9.2/tox.ini
--rw-r--r--   0        0        0    11254 1970-01-01 00:00:00.000000 apio-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      938 2024-04-02 17:40:48.537737 apio-0.9.3/.github/workflows/Publish.yml
+-rw-r--r--   0        0        0      583 2024-04-02 17:40:48.537737 apio-0.9.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      330 2024-04-02 17:40:48.537737 apio-0.9.3/.gitignore
+-rw-r--r--   0        0        0     6379 2024-04-02 17:40:48.537737 apio-0.9.3/.vscode/launch.json
+-rw-r--r--   0        0        0    18047 2024-04-02 17:40:48.537737 apio-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1092 2024-04-02 17:40:48.537737 apio-0.9.3/Makefile
+-rw-r--r--   0        0        0     4683 2024-04-02 17:40:48.537737 apio-0.9.3/README.md
+-rw-r--r--   0        0        0      747 2024-04-02 17:40:48.537737 apio-0.9.3/apio/__init__.py
+-rw-r--r--   0        0        0     5752 2024-04-02 17:40:48.537737 apio-0.9.3/apio/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/boards.py
+-rw-r--r--   0        0        0     3160 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/build.py
+-rw-r--r--   0        0        0     1400 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/clean.py
+-rw-r--r--   0        0        0     1603 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/config.py
+-rw-r--r--   0        0        0     1850 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/drivers.py
+-rw-r--r--   0        0        0     2277 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/examples.py
+-rw-r--r--   0        0        0     1571 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/graph.py
+-rw-r--r--   0        0        0     2341 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/init.py
+-rw-r--r--   0        0        0     2642 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/install.py
+-rw-r--r--   0        0        0     2035 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/lint.py
+-rw-r--r--   0        0        0      530 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/raw.py
+-rw-r--r--   0        0        0     1003 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/sim.py
+-rw-r--r--   0        0        0     1913 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/system.py
+-rw-r--r--   0        0        0     1233 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/test.py
+-rw-r--r--   0        0        0     2631 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/time.py
+-rw-r--r--   0        0        0     2382 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/uninstall.py
+-rw-r--r--   0        0        0     1889 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/upgrade.py
+-rw-r--r--   0        0        0     3944 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/upload.py
+-rw-r--r--   0        0        0     1473 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/verify.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.537737 apio-0.9.3/apio/managers/__init__.py
+-rw-r--r--   0        0        0    12869 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/arguments.py
+-rw-r--r--   0        0        0     3000 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/downloader.py
+-rw-r--r--   0        0        0    17082 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/drivers.py
+-rw-r--r--   0        0        0    10465 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/examples.py
+-rw-r--r--   0        0        0    17535 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/installer.py
+-rw-r--r--   0        0        0     7344 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/project.py
+-rw-r--r--   0        0        0    35402 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/scons.py
+-rw-r--r--   0        0        0     9638 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/system.py
+-rw-r--r--   0        0        0     3798 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/unpacker.py
+-rw-r--r--   0        0        0     6051 2024-04-02 17:40:48.541737 apio-0.9.3/apio/profile.py
+-rw-r--r--   0        0        0    14985 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources.py
+-rw-r--r--   0        0        0     1225 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/80-fpga-ftdi.rules
+-rw-r--r--   0        0        0      356 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/80-fpga-serial.rules
+-rw-r--r--   0        0        0    15689 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/boards.json
+-rw-r--r--   0        0        0      345 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/distribution.json
+-rw-r--r--   0        0        0    13399 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/ecp5/SConstruct
+-rw-r--r--   0        0        0     7638 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/fpgas.json
+-rw-r--r--   0        0        0    13272 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/ice40/SConstruct
+-rw-r--r--   0        0        0     1987 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/packages.json
+-rw-r--r--   0        0        0     1639 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/programmers.json
+-rw-r--r--   0        0        0    25124 2024-04-02 17:40:48.541737 apio-0.9.3/apio/util.py
+-rwxr-xr-x   0        0        0      517 2024-04-02 17:40:48.541737 apio-0.9.3/apio_run.py
+-rw-r--r--   0        0        0     1182 2024-04-02 17:40:48.541737 apio-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/__init__.py
+-rw-r--r--   0        0        0     9653 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_build.py
+-rw-r--r--   0        0        0     1564 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_clean.py
+-rw-r--r--   0        0        0      565 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_graph.py
+-rw-r--r--   0        0        0      527 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_lint.py
+-rw-r--r--   0        0        0      515 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_sim.py
+-rw-r--r--   0        0        0      517 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_test.py
+-rw-r--r--   0        0        0     1126 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_time.py
+-rw-r--r--   0        0        0     3182 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_upload.py
+-rw-r--r--   0        0        0      631 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_verify.py
+-rw-r--r--   0        0        0     2665 2024-04-02 17:40:48.581738 apio-0.9.3/test/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/__init__.py
+-rw-r--r--   0        0        0      754 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_boards.py
+-rw-r--r--   0        0        0      769 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_config.py
+-rw-r--r--   0        0        0      490 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_drivers.py
+-rw-r--r--   0        0        0     1116 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_examples.py
+-rw-r--r--   0        0        0     3964 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_init.py
+-rw-r--r--   0        0        0      843 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_install.py
+-rw-r--r--   0        0        0     1266 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_system.py
+-rw-r--r--   0        0        0      949 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_uninstall.py
+-rw-r--r--   0        0        0      657 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_upgrade.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/packages/__init__.py
+-rw-r--r--   0        0        0     8867 2024-04-02 17:40:48.581738 apio-0.9.3/test/packages/test_complete.py
+-rw-r--r--   0        0        0     1741 2024-04-02 17:40:48.581738 apio-0.9.3/test/test_apio.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test2/__init__.py
+-rw-r--r--   0        0        0     2666 2024-04-02 17:40:48.581738 apio-0.9.3/test2/test_ledon.py
+-rw-r--r--   0        0        0      268 2024-04-02 17:40:48.581738 apio-0.9.3/tox.ini
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 apio-0.9.3/PKG-INFO
```

### Comparing `apio-0.9.2/.github/workflows/Publish.yml` & `apio-0.9.3/.github/workflows/Publish.yml`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/.github/workflows/build.yml` & `apio-0.9.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/.vscode/launch.json` & `apio-0.9.3/.vscode/launch.json`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 {
     "version": "0.2.0",
     "configurations": [
         {
+            "name": "Apio",
+            "type": "debugpy",
+            "request": "launch",
+            "program": "${file}",
+            "console": "internalConsole",
+            "justMyCode": true
+        },
+        {
             "name": "Apio build",
             "type": "debugpy",
             "request": "launch",
             "program": "${file}",
             "args": ["build","--top-module","caca"],
             "console": "internalConsole",
             "justMyCode": true,
```

### Comparing `apio-0.9.2/LICENSE` & `apio-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/Makefile` & `apio-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/__init__.py` & `apio-0.9.3/apio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -- Licence GPLv2
 
 # --------------------------------------------
 # - Information for the Distribution package
 # --------------------------------------------
 
 # -- Developer: Change this number when releasing a new version
-VERSION = (0, 9, 2)
+VERSION = (0, 9, 3)
 
 # -- Get the version as a string. Ex: "0.10.1"
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "apio"
 __description__ = "Open source ecosystem for open FPGA boards"
 __url__ = "https://github.com/FPGAwars/apio"
```

### Comparing `apio-0.9.2/apio/__main__.py` & `apio-0.9.3/apio/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,21 +133,48 @@
         )
 
         # -- Utility commands
         util_help = find_commands_help(
             _help, ["boards", "config", "examples", "raw", "system", "upgrade"]
         )
 
-        # -- Reformat the Help string
-        _help = "\n".join(_help)
-        _help = _help.replace("Commands:\n", "Project commands:\n")
-        _help += "\n\nSetup commands:\n"
-        _help += "\n".join(setup_help)
-        _help += "\n\nUtility commands:\n"
-        _help += "\n".join(util_help)
-        _help += "\n"
+        # -- Project commands:
+        cmd_help = find_commands_help(
+            _help,
+            [
+                "build",
+                "clean",
+                "sim",
+                "test",
+                "verify",
+                "lint",
+                "time",
+                "upload",
+                "graph",
+            ],
+        )
+
+        # -- Get the Help header
+        index = _help.index("Commands:")
+        header_help = _help[:index]
+
+        # -- Print header
+        click.secho("\n".join(header_help))
+
+        # -- Print project commands:
+        click.secho("Project commands:")
+        click.secho("\n".join(cmd_help))
+        click.secho()
+
+        # -- Print Setup commands:
+        click.secho("Setup commands:")
+        click.secho("\n".join(setup_help))
+        click.secho()
 
-        click.secho(_help)
+        # -- Print utility commands:
+        click.secho("Utility commands:")
+        click.secho("\n".join(util_help))
+        click.secho()
 
     # -- If there is a command, it is executed when this function is finished
     # -- Debug: print the command invoked
     # print(f"{ctx.invoked_subcommand}")
```

### Comparing `apio-0.9.2/apio/commands/boards.py` & `apio-0.9.3/apio/commands/boards.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/build.py` & `apio-0.9.3/apio/commands/build.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/clean.py` & `apio-0.9.3/apio/commands/clean.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/config.py` & `apio-0.9.3/apio/commands/config.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/drivers.py` & `apio-0.9.3/apio/commands/drivers.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/examples.py` & `apio-0.9.3/apio/commands/examples.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/graph.py` & `apio-0.9.3/apio/commands/graph.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/init.py` & `apio-0.9.3/apio/commands/init.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/install.py` & `apio-0.9.3/apio/commands/install.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/lint.py` & `apio-0.9.3/apio/commands/lint.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/raw.py` & `apio-0.9.3/apio/commands/raw.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/sim.py` & `apio-0.9.3/apio/commands/sim.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/system.py` & `apio-0.9.3/apio/commands/system.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/test.py` & `apio-0.9.3/apio/commands/test.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/time.py` & `apio-0.9.3/apio/commands/time.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/uninstall.py` & `apio-0.9.3/apio/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/upgrade.py` & `apio-0.9.3/apio/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/upload.py` & `apio-0.9.3/apio/commands/upload.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/commands/verify.py` & `apio-0.9.3/apio/commands/verify.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/arguments.py` & `apio-0.9.3/apio/managers/arguments.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/downloader.py` & `apio-0.9.3/apio/managers/downloader.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/drivers.py` & `apio-0.9.3/apio/managers/drivers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 # -- This file is part of the Apio project
 # -- (C) 2016-2019 FPGAwars
 # -- Author Jesús Arroyo
 # -- Licence GPLv2
 """Manage board drivers"""
 
 
+import sys
+import shutil
 import subprocess
 from pathlib import Path
-
 import click
-
 from apio import util
 from apio.profile import Profile
 from apio.resources import Resources
 
-
 FTDI_INSTALL_DRIVER_INSTRUCTIONS = """
    FTDI driver installation:
    Usage instructions
 
       1. Connect the FTDI FPGA board
       2. Select (Interface 0)
       3. Replace driver by "libusbK"
@@ -396,50 +395,77 @@
     @staticmethod
     def _check_ftdi_driver_darwin(driver):
         return driver in str(subprocess.check_output(["kextstat"]))
 
     # W0703: Catching too general exception Exception (broad-except)
     # pylint: disable=W0703
     def _ftdi_enable_windows(self):
+
+        # -- Get the drivers apio package base folder
         drivers_base_dir = util.get_package_dir("tools-drivers")
+
+        # -- No folder --> package not installer (or not correctly installed)
+        if not drivers_base_dir:
+            util.show_package_path_error(self.name)
+            util.show_package_install_instructions(self.name)
+            sys.exit(1)
+
+        # -- Build the drivers base bin dir
         drivers_bin_dir = drivers_base_dir / "bin"
-        drivers_share_dir = drivers_base_dir / "share"
-        zadig_ini_path = drivers_share_dir / "zadig.ini"
-        zadig_ini = Path("zadig.ini")
+
+        # -- Check if the driver packages is installed
+        package_ok = util.check_package(
+            self.name, self.version, self.spec_version, drivers_bin_dir
+        )
+
+        # -- Not installed. Exit
+        if not package_ok:
+            sys.exit(1)
+
+        # -- Path to the zadig.ini file
+        # -- It is the zadig config file
+        zadig_ini_src = drivers_base_dir / "share" / "zadig.ini"
+        zadig_ini_dst = Path("zadig.ini")
+
+        # -- copy the zadig.ini file to the current working folder
+        # -- so that zadig open it when executed
+        shutil.copyfile(zadig_ini_src, zadig_ini_dst)
+
+        # -- Show messages for the user
+        click.secho("Launch drivers configuration tool")
+        click.secho(FTDI_INSTALL_DRIVER_INSTRUCTIONS, fg="yellow")
+
+        # -- Zadig exe file with full path:
+        zadig_exe = drivers_base_dir / "bin" / "zadig.exe"
 
         try:
-            if util.check_package(
-                self.name, self.version, self.spec_version, drivers_bin_dir
-            ):
-                click.secho("Launch drivers configuration tool")
-                click.secho(FTDI_INSTALL_DRIVER_INSTRUCTIONS, fg="yellow")
-                # Copy zadig.ini
-                with open(zadig_ini, "w", encoding="utf8") as ini_file:
-                    with open(
-                        zadig_ini_path, "r", encoding="utf8"
-                    ) as local_ini_file:
-                        ini_file.write(local_ini_file.read())
+            # -- Execute zadig!
+            result = util.exec_command(str(zadig_exe))
+            click.secho("FTDI drivers configuration finished", fg="green")
 
-                result = util.exec_command(
-                    str(Path(drivers_bin_dir) / "zadig.exe")
-                )
-                click.secho("FTDI drivers configuration finished", fg="green")
-            else:
-                result = 1
-        except Exception as exc:
+        # -- It was not possible to execute Zadig...
+        except OSError as exc:
             click.secho("Error: " + str(exc), fg="red")
-            result = 1
-        finally:
-            # Remove zadig.ini
-            if zadig_ini.exists():
-                zadig_ini.unlink()
-
-        if not isinstance(result, int):
-            result = result.get("returncode")
-        return result
+            click.secho(
+                "Trying to execute zadig.exe in command line, "
+                "but an error ocurred",
+                fg="red",
+            )
+            click.secho(
+                "Please, execute the command again in the command line with"
+                " administrator privilegdes",
+                fg="red",
+            )
+            sys.exit(1)
+
+        # -- Remove zadig.ini from the current folder. It is no longer needed
+        if zadig_ini_dst.exists():
+            zadig_ini_dst.unlink()
+
+        return result.get("returncode")
 
     @staticmethod
     def _ftdi_disable_windows():
         click.secho("Launch device manager")
         click.secho(FTDI_UNINSTALL_DRIVER_INSTRUCTIONS, fg="yellow")
 
         result = util.exec_command("mmc devmgmt.msc")
```

### Comparing `apio-0.9.2/apio/managers/examples.py` & `apio-0.9.3/apio/managers/examples.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/installer.py` & `apio-0.9.3/apio/managers/installer.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/project.py` & `apio-0.9.3/apio/managers/project.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/scons.py` & `apio-0.9.3/apio/managers/scons.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/system.py` & `apio-0.9.3/apio/managers/system.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/managers/unpacker.py` & `apio-0.9.3/apio/managers/unpacker.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/profile.py` & `apio-0.9.3/apio/profile.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/resources.py` & `apio-0.9.3/apio/resources.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/resources/80-fpga-ftdi.rules` & `apio-0.9.3/apio/resources/80-fpga-ftdi.rules`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/resources/boards.json` & `apio-0.9.3/apio/resources/boards.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/resources/ecp5/SConstruct` & `apio-0.9.3/apio/resources/ecp5/SConstruct`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     generator = iverilog_generator,
     suffix='.out',
     src_suffix='.v',
     source_scanner=list_scanner)
 env.Append(BUILDERS={'IVerilog': iverilog})
 
 dot_builder = Builder(
-    action='yosys -p \"show -format dot -colors 1 -prefix hardware {0}\" {1} $SOURCES'.format(
+    action='yosys -f verilog -p \"show -format dot -colors 1 -prefix hardware {0}\" {1} $SOURCES'.format(
         YOSYS_TOP if YOSYS_TOP else 'unknown_top',
         '' if VERBOSE_ALL else '-q'
     ),
     suffix='.dot',
     src_suffix='.v',
     source_scanner=list_scanner)
 env.Append(BUILDERS={'DOT': dot_builder})
```

### Comparing `apio-0.9.2/apio/resources/fpgas.json` & `apio-0.9.3/apio/resources/fpgas.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/resources/ice40/SConstruct` & `apio-0.9.3/apio/resources/ice40/SConstruct`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     generator = iverilog_generator,
     suffix='.out',
     src_suffix='.v',
     source_scanner=list_scanner)
 env.Append(BUILDERS={'IVerilog': iverilog})
 
 dot_builder = Builder(
-    action='yosys -p \"show -format dot -colors 1 -prefix hardware {0}\" {1} $SOURCES'.format(
+    action='yosys -f verilog -p \"show -format dot -colors 1 -prefix hardware {0}\" {1} $SOURCES'.format(
         YOSYS_TOP if YOSYS_TOP else 'unknown_top',
         '' if VERBOSE_ALL else '-q'
     ),
     suffix='.dot',
     src_suffix='.v',
     source_scanner=list_scanner)
 env.Append(BUILDERS={'DOT': dot_builder})
```

### Comparing `apio-0.9.2/apio/resources/packages.json` & `apio-0.9.3/apio/resources/packages.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/resources/programmers.json` & `apio-0.9.3/apio/resources/programmers.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio/util.py` & `apio-0.9.3/apio/util.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/apio_run.py` & `apio-0.9.3/apio_run.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/pyproject.toml` & `apio-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_build.py` & `apio-0.9.3/test/code_commands/test_build.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_clean.py` & `apio-0.9.3/test/code_commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_graph.py` & `apio-0.9.3/test/code_commands/test_graph.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_lint.py` & `apio-0.9.3/test/code_commands/test_lint.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_sim.py` & `apio-0.9.3/test/code_commands/test_sim.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_test.py` & `apio-0.9.3/test/code_commands/test_test.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_time.py` & `apio-0.9.3/test/code_commands/test_time.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_upload.py` & `apio-0.9.3/test/code_commands/test_upload.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/code_commands/test_verify.py` & `apio-0.9.3/test/code_commands/test_verify.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/conftest.py` & `apio-0.9.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_boards.py` & `apio-0.9.3/test/env_commands/test_boards.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_config.py` & `apio-0.9.3/test/env_commands/test_config.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_examples.py` & `apio-0.9.3/test/env_commands/test_examples.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_init.py` & `apio-0.9.3/test/env_commands/test_init.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_install.py` & `apio-0.9.3/test/env_commands/test_install.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_system.py` & `apio-0.9.3/test/env_commands/test_system.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_uninstall.py` & `apio-0.9.3/test/env_commands/test_uninstall.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/env_commands/test_upgrade.py` & `apio-0.9.3/test/env_commands/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/packages/test_complete.py` & `apio-0.9.3/test/packages/test_complete.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test/test_apio.py` & `apio-0.9.3/test/test_apio.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.2/test2/test_ledon.py` & `apio-0.9.3/test2/test_ledon.py`

 * *Files identical despite different names*

