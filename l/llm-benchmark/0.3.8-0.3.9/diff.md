# Comparing `tmp/llm_benchmark-0.3.8.tar.gz` & `tmp/llm_benchmark-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_benchmark-0.3.8.tar", max compression
+gzip compressed data, was "llm_benchmark-0.3.9.tar", max compression
```

## Comparing `llm_benchmark-0.3.8.tar` & `llm_benchmark-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1083 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/LICENSE
--rw-r--r--   0        0        0     2124 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/README.md
--rw-r--r--   0        0        0        0 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/__init__.py
--rw-r--r--   0        0        0     1837 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/check_models.py
--rw-r--r--   0        0        0      498 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/check_ollama.py
--rw-r--r--   0        0        0     2064 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/data/benchmark1.yml
--rw-r--r--   0        0        0      216 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/data/benchmark_models_16gb_ram.yml
--rw-r--r--   0        0        0       79 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/data/benchmark_models_4gb_ram.yml
--rw-r--r--   0        0        0      171 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/data/benchmark_models_8gb_ram.yml
--rw-r--r--   0        0        0   596759 2024-03-31 00:36:31.982919 llm_benchmark-0.3.8/llm_benchmark/data/img/sample1.jpg
--rw-r--r--   0        0        0   243536 2024-03-31 00:36:31.986919 llm_benchmark-0.3.8/llm_benchmark/data/img/sample2.jpg
--rw-r--r--   0        0        0   518611 2024-03-31 00:36:31.986919 llm_benchmark-0.3.8/llm_benchmark/data/img/sample3.jpg
--rw-r--r--   0        0        0   236523 2024-03-31 00:36:31.986919 llm_benchmark-0.3.8/llm_benchmark/data/img/sample4.jpg
--rw-r--r--   0        0        0   534025 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/data/img/sample5.jpg
--rw-r--r--   0        0        0     2873 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/main.py
--rw-r--r--   0        0        0     1623 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/query_llm.py
--rw-r--r--   0        0        0     5784 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/run_benchmark.py
--rw-r--r--   0        0        0     2338 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/run_benchmark_one.py
--rw-r--r--   0        0        0        0 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/security_connection/__init__.py
--rw-r--r--   0        0        0      353 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/security_connection/connection.py
--rw-r--r--   0        0        0        0 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/security_connection/security.py
--rw-r--r--   0        0        0        0 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/systeminfo/__init__.py
--rw-r--r--   0        0        0     7068 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/llm_benchmark/systeminfo/sysmain.py
--rw-r--r--   0        0        0      758 2024-03-31 00:36:31.990919 llm_benchmark-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 llm_benchmark-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-03-31 10:30:22.826490 llm_benchmark-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2143 2024-03-31 10:30:22.826490 llm_benchmark-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/__init__.py
+-rw-r--r--   0        0        0     1837 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/check_models.py
+-rw-r--r--   0        0        0      520 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/check_ollama.py
+-rw-r--r--   0        0        0     2064 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/data/benchmark1.yml
+-rw-r--r--   0        0        0      216 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/data/benchmark_models_16gb_ram.yml
+-rw-r--r--   0        0        0       79 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/data/benchmark_models_4gb_ram.yml
+-rw-r--r--   0        0        0      171 2024-03-31 10:30:22.858490 llm_benchmark-0.3.9/llm_benchmark/data/benchmark_models_8gb_ram.yml
+-rw-r--r--   0        0        0   596759 2024-03-31 10:30:22.862490 llm_benchmark-0.3.9/llm_benchmark/data/img/sample1.jpg
+-rw-r--r--   0        0        0   243536 2024-03-31 10:30:22.862490 llm_benchmark-0.3.9/llm_benchmark/data/img/sample2.jpg
+-rw-r--r--   0        0        0   518611 2024-03-31 10:30:22.866490 llm_benchmark-0.3.9/llm_benchmark/data/img/sample3.jpg
+-rw-r--r--   0        0        0   236523 2024-03-31 10:30:22.866490 llm_benchmark-0.3.9/llm_benchmark/data/img/sample4.jpg
+-rw-r--r--   0        0        0   534025 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/data/img/sample5.jpg
+-rw-r--r--   0        0        0     3295 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/main.py
+-rw-r--r--   0        0        0     1623 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/query_llm.py
+-rw-r--r--   0        0        0     5784 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/run_benchmark.py
+-rw-r--r--   0        0        0     2338 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/run_benchmark_one.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/security_connection/__init__.py
+-rw-r--r--   0        0        0      723 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/security_connection/connection.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/security_connection/security.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/systeminfo/__init__.py
+-rw-r--r--   0        0        0     7068 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/llm_benchmark/systeminfo/sysmain.py
+-rw-r--r--   0        0        0      758 2024-03-31 10:30:22.870490 llm_benchmark-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 llm_benchmark-0.3.9/PKG-INFO
```

### Comparing `llm_benchmark-0.3.8/LICENSE` & `llm_benchmark-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/README.md` & `llm_benchmark-0.3.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 
 ## Installation Steps
 
 ```bash
 pip install llm-benchmark
 ```
 
+## Usage for general users directly
+
+```bash
+pip install llm-benchmark
+llm_benchmark hello jason
+llm_benchmark run
+```
+
+## Installation and Usage in Video format
+
+![llm-benchmark](https://github.com/aidatatools/ollama-benchmark/blob/main/llm-benchmark.gif)
+
 It's tested on Python 3.9 and above.
 
 ## ollama installation with the following models installed
 
 7B model can be run on machines with 8GB of RAM
 
 13B model can be run on machines with 16GB of RAM
@@ -44,22 +56,14 @@
 ollama pull mistral:7b
 ollama pull llama2:7b
 ollama pull llama2:13b
 ollama pull llava:7b
 ollama pull llava:13b
 ```
 
-## Usage for general users directly
-
-```bash
-pip install llm-benchmark
-llm_benchmark hello jason
-llm_benchmark run
-```
-
 ## Python Poetry manually(advanced) installation
 
 <https://python-poetry.org/docs/#installing-manually>
 
 ## For developers to develop new features on Windows Powershell or on Ubuntu Linux or macOS
 
 ```bash
@@ -73,24 +77,14 @@
 
 ```bash
 poetry shell
 poetry install
 llm_benchmark hello jason
 ```
 
-### The default sending back the info is
-
-Memory Size: 32GB
-
-CPU: Intel i5-12400
-
-GPU: 3060
-
-OS: Microsoft Windows 11
-
 ### Example #1 send systeminfo and bechmark results to a remote server
 
 ```bash
 llm_benchmark run
 ```
 
 ### Example #2 Do not send systeminfo and bechmark results to a remote server
```

### Comparing `llm_benchmark-0.3.8/llm_benchmark/check_models.py` & `llm_benchmark-0.3.9/llm_benchmark/check_models.py`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/data/benchmark1.yml` & `llm_benchmark-0.3.9/llm_benchmark/data/benchmark1.yml`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/data/img/sample1.jpg` & `llm_benchmark-0.3.9/llm_benchmark/data/img/sample1.jpg`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/data/img/sample2.jpg` & `llm_benchmark-0.3.9/llm_benchmark/data/img/sample2.jpg`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/data/img/sample3.jpg` & `llm_benchmark-0.3.9/llm_benchmark/data/img/sample3.jpg`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/data/img/sample4.jpg` & `llm_benchmark-0.3.9/llm_benchmark/data/img/sample4.jpg`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/data/img/sample5.jpg` & `llm_benchmark-0.3.9/llm_benchmark/data/img/sample5.jpg`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/main.py` & `llm_benchmark-0.3.9/llm_benchmark/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 def run(sendinfo: bool = True):
     sys_info = sysmain.get_extra()
     print(f"Total memory size : {sys_info['memory']:.2f} GB") 
     print(f"cpu_info: {sys_info['cpu']}")
     print(f"gpu_info: {sys_info['gpu']}")
     print(f"os_version: {sys_info['os_version']}")
 
-    check_ollama.check_ollama_version()
+    ollama_version = check_ollama.check_ollama_version()
+    print(f"ollama_version: {ollama_version}")
     print('-'*10)
 
     ft_mem_size = float(f"{sys_info['memory']:.2f}")
     models_file_path = pkg_resources.resource_filename('llm_benchmark','data/benchmark_models_16gb_ram.yml')
     if(ft_mem_size>=4 and ft_mem_size <7):
         models_file_path = pkg_resources.resource_filename('llm_benchmark','data/benchmark_models_4gb_ram.yml')
     elif(ft_mem_size>=7 and ft_mem_size <15):
@@ -37,30 +38,38 @@
 
     check_models.pull_models(models_file_path)
     print('-'*10)
 
     benchmark_file_path = pkg_resources.resource_filename('llm_benchmark','data/benchmark1.yml')
 
     bench_results_info = {}
-    result1 = run_benchmark.run_benchmark(models_file_path,benchmark_file_path, 'instruct')
-    bench_results_info.update(result1)
-    result2 = run_benchmark.run_benchmark(models_file_path,benchmark_file_path, 'question-answer')
-    bench_results_info.update(result2)
-    result3 = run_benchmark.run_benchmark(models_file_path,benchmark_file_path, 'vision-image')
-    bench_results_info.update(result3)
+    is_simulation = True
+    if is_simulation==False :
+        result1 = run_benchmark.run_benchmark(models_file_path,benchmark_file_path, 'instruct')
+        bench_results_info.update(result1)
+        result2 = run_benchmark.run_benchmark(models_file_path,benchmark_file_path, 'question-answer')
+        bench_results_info.update(result2)
+        result3 = run_benchmark.run_benchmark(models_file_path,benchmark_file_path, 'vision-image')
+        bench_results_info.update(result3)
+    else:
+        bench_results_info.update({"llama2:7b":7.65})
+        bench_results_info.update({"gemma2:7b":17.77})
 
     if (sendinfo==True):
         print(f"Sending the following data to a remote server")
         print(f"Your machine UUID : {sysmain.get_uuid()}")
-        print(f"{bench_results_info.items()}")
+        #print(f"{bench_results_info.items()}")
+        x = connection.send_benchmark(sysmain.get_uuid(),ollama_version,bench_results_info)
+        #print(x)
         print('=='*10)
         #print(f"{sys_info.items()}")
-        #sys_info = sysmain.get_extra()
+        sys_info = sysmain.get_extra()
+        sys_info['uuid']=f"{sysmain.get_uuid()}"
         x = connection.send_sysinfo(sys_info)
-        print(x)
+        #print(x)
 
 
 @app.command()
 def goodbye(name: str, formal: bool = False):
     if formal:
         print(f"Goodbye Mr.(Ms.) {name}. Have a good day.")
     else:
```

### Comparing `llm_benchmark-0.3.8/llm_benchmark/query_llm.py` & `llm_benchmark-0.3.9/llm_benchmark/query_llm.py`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/run_benchmark.py` & `llm_benchmark-0.3.9/llm_benchmark/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/run_benchmark_one.py` & `llm_benchmark-0.3.9/llm_benchmark/run_benchmark_one.py`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/llm_benchmark/systeminfo/sysmain.py` & `llm_benchmark-0.3.9/llm_benchmark/systeminfo/sysmain.py`

 * *Files identical despite different names*

### Comparing `llm_benchmark-0.3.8/pyproject.toml` & `llm_benchmark-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_benchmark"
-version = "0.3.8"
+version = "0.3.9"
 description = "LLM Benchmark for Throughputs via Ollama"
 authors = ["Jason Chuang <chuangtcee@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/aidatatools/ollama-benchmark/"
 readme = "README.md"
 keywords = [
     "benchmark",
```

### Comparing `llm_benchmark-0.3.8/PKG-INFO` & `llm_benchmark-0.3.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_benchmark
-Version: 0.3.8
+Version: 0.3.9
 Summary: LLM Benchmark for Throughputs via Ollama
 Home-page: https://github.com/aidatatools/ollama-benchmark/
 License: MIT
 Keywords: benchmark,llama,ollama,llms,local
 Author: Jason Chuang
 Author-email: chuangtcee@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -30,14 +30,26 @@
 
 ## Installation Steps
 
 ```bash
 pip install llm-benchmark
 ```
 
+## Usage for general users directly
+
+```bash
+pip install llm-benchmark
+llm_benchmark hello jason
+llm_benchmark run
+```
+
+## Installation and Usage in Video format
+
+![llm-benchmark](https://github.com/aidatatools/ollama-benchmark/blob/main/llm-benchmark.gif)
+
 It's tested on Python 3.9 and above.
 
 ## ollama installation with the following models installed
 
 7B model can be run on machines with 8GB of RAM
 
 13B model can be run on machines with 16GB of RAM
@@ -70,22 +82,14 @@
 ollama pull mistral:7b
 ollama pull llama2:7b
 ollama pull llama2:13b
 ollama pull llava:7b
 ollama pull llava:13b
 ```
 
-## Usage for general users directly
-
-```bash
-pip install llm-benchmark
-llm_benchmark hello jason
-llm_benchmark run
-```
-
 ## Python Poetry manually(advanced) installation
 
 <https://python-poetry.org/docs/#installing-manually>
 
 ## For developers to develop new features on Windows Powershell or on Ubuntu Linux or macOS
 
 ```bash
@@ -99,24 +103,14 @@
 
 ```bash
 poetry shell
 poetry install
 llm_benchmark hello jason
 ```
 
-### The default sending back the info is
-
-Memory Size: 32GB
-
-CPU: Intel i5-12400
-
-GPU: 3060
-
-OS: Microsoft Windows 11
-
 ### Example #1 send systeminfo and bechmark results to a remote server
 
 ```bash
 llm_benchmark run
 ```
 
 ### Example #2 Do not send systeminfo and bechmark results to a remote server
```

