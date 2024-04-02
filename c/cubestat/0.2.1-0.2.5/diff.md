# Comparing `tmp/cubestat-0.2.1.tar.gz` & `tmp/cubestat-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.2.1.tar", last modified: Sat Mar 30 00:31:26 2024, max compression
+gzip compressed data, was "cubestat-0.2.5.tar", last modified: Tue Apr  2 16:21:30 2024, max compression
```

## Comparing `cubestat-0.2.1.tar` & `cubestat-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:31:26.423194 cubestat-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-30 00:31:22.000000 cubestat-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-30 00:31:26.423194 cubestat-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-03-30 00:31:22.000000 cubestat-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:31:26.423194 cubestat-0.2.1/cubestat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 00:31:22.000000 cubestat-0.2.1/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20379 2024-03-30 00:31:22.000000 cubestat-0.2.1/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:31:26.423194 cubestat-0.2.1/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-30 00:31:26.000000 cubestat-0.2.1/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-30 00:31:26.000000 cubestat-0.2.1/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 00:31:26.000000 cubestat-0.2.1/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-30 00:31:26.000000 cubestat-0.2.1/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-30 00:31:26.000000 cubestat-0.2.1/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 00:31:26.000000 cubestat-0.2.1/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 00:31:26.423194 cubestat-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-30 00:31:22.000000 cubestat-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.610425 cubestat-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-02 16:21:13.000000 cubestat-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 16:21:30.610425 cubestat-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-02 16:21:13.000000 cubestat-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.606425 cubestat-0.2.5/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14413 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.606425 cubestat-0.2.5/cubestat/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/free_swap_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/linux_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/macos_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/mem_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/nv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/swapusage_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.610425 cubestat-0.2.5/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:21:30.610425 cubestat-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 16:21:13.000000 cubestat-0.2.5/setup.py
```

### Comparing `cubestat-0.2.1/LICENSE` & `cubestat-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.1/README.md` & `cubestat-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # system monitoring horizon charts for terminal
 
 cubestat is a command-line utility to monitor system metrics in horizon chart format. It was originally created for Apple M1/M2 devices, but now works on Linux with nVidia GPU as well, including Google Colab environment.
 
-Let's start with example: running [deep RL loop](https://github.com/okuvshynov/rlscout) on a single MacBook Air M2. We can see model training (on GPU), self-play (done on 4 performance CPU cores) and model evaluation, which runs inference on Neural Engine (ANE):
-![Self-play + training + eval](static/selfplay.png)
+Let's start with an example:
+
+In the clip below we see Mixtral-8x7b inference on MacBook Air with FF layers offloaded to SSD. 
+We can notice somewhat low GPU util (not good), 2Gb/s+ of data read from disk (as we have to fetch the weights), but plenty of free RAM (And we are actually able to serve almost 100Gb model on 24Gb machine with fp16 precision).
+We can also see the disk writes before the inference started - that was model preprocessing which was writing the weights to disk individually.
+
+
+https://github.com/okuvshynov/cubestat/assets/661042/8e1e405e-ca61-4ffb-bedb-e04eb33f8bc2
+
 
 Currently cubestat reports:
 1. CPU utilization - configurable per core ('expanded'), cluster of cores: Efficiency/Performance ('cluster') or both. Is shown as percentage.
 2. GPU utilization per card/chip. Is shown in percentage. Works for Apple's M1/M2 SoC and nVidia GPUs. For nVidia GPU shows memory usage as well.
 3. ANE (Apple's Neural Engine) power consumption. According to `man powermetrics` it is an estimate, but seems working good enough as a proxy to ANE utilization. Is shown as percentage.
-4. Disk and network IO; Is shown in Kb/s.
+4. Disk and network IO; Is shown as rate (Kb/s, Mb/s, Gb/s).
 5. Memory usage in %
+6. Swap usage. Is shown as absolute value (Kb, Mb, Gb)
 
 Despite many monitoring tools available for monitoring system counters, horizon charts have nice information density properties which make it possible to show a history of N measurements for M metrics on a single screen for significantly large N and M. Thus, this tool was created.
 
 ## Installation and Usage:
 
 ```
-pip3 install cubestat
+pip install cubestat
 
 usage: cubestat [-h] [--refresh_ms REFRESH_MS] [--buffer_size BUFFER_SIZE] [--cpu {all,by_cluster,by_core}] [--color {red,green,blue,mixed}] [--percentages {hidden,last}] [--disk] [--network] [--no-disk] [--no-network]
 
 options:
   -h, --help            show this help message and exit
   --refresh_ms REFRESH_MS, -i REFRESH_MS
                         Update frequency, milliseconds
@@ -46,17 +54,17 @@
 * n - show/hide network utilization
 * UP/DOWN - scroll the lines in case there are more cores;
 * LEFT/RIGHT - scroll left/right. Autorefresh is paused when user scrolled to non-latest position. To resume autorefresh either scroll back to the right or press '0';
 * 0 - reset horizontal scroll, continue autorefresh.
 
 Running on Apple devices will require sudo access, as `powermetrics` has this limitation. If you are comfortable doing that, you can update /etc/sudoers to not require password to run powermetrics.
 
-Running on Linux doesn't require it.
+Running on Linux doesn't require sudo.
 
-Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 nVidia GPU instance:
+Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 GPU instance:
 ![multigpu](static/multigpu.png)
 
 ## Apple Neural Engine utilization
 
 A few notes on 'what does this even represent?'. Utilization we report is essentially power consumption reported by powermetrics.
 To convert it to % we divide it by some 'maximum' value observed in experimentation. There are many drawbacks to this:
 * The concept of 'utilization' overall it pretty ambiguous, e.g. for a x86 CPU - when CPU is wasting cycles on a cache miss, is it 'utilized' or not? If CPU is doing scalar instructions on 1 execution port rather than vectorized instructions on several ports, is it 'utilized' or not?
@@ -68,14 +76,15 @@
 
 We can run cubestat on Google Colab instances to monitor GPU/CPU/IO usage.
 
 First cell:
 ```
 !pip install cubestat
 !pip install colab-xterm
+!pip install pynvml
 %load_ext colabxterm
 # export TERM=xterm-256color <---- RUN THIS IN TERMINAL
 # cubestat                   <---- RUN THIS IN TERMINAL
 ```
 
 Start xterm:
 ```
@@ -92,15 +101,15 @@
 
 ![colab cubestat](static/colab_cubestat.png)
 
 
 ## Dependencies
 * Python 3.?+
 * psutil 5.9.5+
-* pynvml for nVidia cards monitoring
+* [optional] pynvml for nVidia cards monitoring
 
 ## TODO
 * Apple Neural Engine correct scale.
 * GPU aggregation
 * CPU by socket/NUMA/SMT
 * status line (why though?)
 * better colors (especially for dark background)
```

### Comparing `cubestat-0.2.1/setup.py` & `cubestat-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.2.1',
+    version='0.2.5',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for system monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE/RAM/swap/IO monitoring for Apple M1/M2/M3, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
```

