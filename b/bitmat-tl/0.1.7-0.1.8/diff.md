# Comparing `tmp/bitmat-tl-0.1.7.tar.gz` & `tmp/bitmat-tl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.1.7.tar", last modified: Mon Apr  1 21:47:19 2024, max compression
+gzip compressed data, was "bitmat-tl-0.1.8.tar", last modified: Mon Apr  1 22:02:38 2024, max compression
```

## Comparing `bitmat-tl-0.1.7.tar` & `bitmat-tl-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.7/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     3339 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2727 2024-04-01 21:47:17.000000 bitmat-tl-0.1.7/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-01 21:43:18.000000 bitmat-tl-0.1.7/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1061 2024-04-01 19:33:07.000000 bitmat-tl-0.1.7/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 19:35:36.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.7/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2413 2024-04-01 21:28:16.000000 bitmat-tl-0.1.7/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2987 2024-04-01 21:28:16.000000 bitmat-tl-0.1.7/bitmat/utils/convert_hf_model.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.7/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.7/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     3339 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      502 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-04-01 21:30:16.000000 bitmat-tl-0.1.7/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.8/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     3227 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2615 2024-04-01 21:58:58.000000 bitmat-tl-0.1.8/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      216 2024-04-01 22:00:24.000000 bitmat-tl-0.1.8/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1061 2024-04-01 19:33:07.000000 bitmat-tl-0.1.8/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 19:35:36.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.8/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2413 2024-04-01 21:28:16.000000 bitmat-tl-0.1.8/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2987 2024-04-01 21:28:16.000000 bitmat-tl-0.1.8/bitmat/utils/convert_hf_model.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.8/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.8/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3227 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      502 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-04-01 21:59:16.000000 bitmat-tl-0.1.8/setup.py
```

### Comparing `bitmat-tl-0.1.7/LICENSE` & `bitmat-tl-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/PKG-INFO` & `bitmat-tl-0.1.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,24 @@
-Metadata-Version: 2.1
-Name: bitmat-tl
-Version: 0.1.7
-Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
-Home-page: https://github.com/astramind-ai/BitMat/tree/main
-Author: Marco Lironi
-Author-email: marcolironi@astramind.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: triton
-Requires-Dist: transformers
-Requires-Dist: bitsandbytes
-Requires-Dist: numpy
-
 # BitMat: Improving Matrix Multiplication with Triton
 
-## Introduction
+## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
-## Features
+## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
-Packed int8 Operations: Follows the methodologies from the "1bit-LLM Era" to use packed int8 data, reducing memory usage and increasing throughput.
-Ease of Integration: BitMat is designed to be easily integrated into existing PyTorch workflows, providing a seamless user experience.
-Performance Boost: Significant performance improvements in matrix multiplication, especially beneficial for large-scale deep learning models and high-dimensional data.
-## Installation
+
+Packed int8 Operations: During inference the model uses packed int8 data to reduce memory usage and improve computational efficiency.
+
+Ease of Integration: BitMat is designed to be easily integrated into existing PyTorch/transformers workflows, providing a seamless user experience.
+## 💾 Installation
 ```bash
 pip install bitmat-tl
 ```
 At the moment we only support **Linux** platforms. **Windows** installation is possible but is not tested.
-## Quick Start
+## 🏁 Quick Start
 
 ### High-level API (tranformers-compatible)
 ```python
 from transformers import AutoModelForCausalLM
 from bitmat import convert_hf_model
 
 # Initialize your model
@@ -49,18 +31,18 @@
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
 ```
 
-## Contributing
+## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
-## License
+## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
 
 ## Citation
 If you use BitMat in your research, please cite it using the following Bibtex entry:
 
 ```bibtex
 @article{bitmat2024,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bitmat-tl-0.1.7/README.md` & `bitmat-tl-0.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,43 @@
+Metadata-Version: 2.1
+Name: bitmat-tl
+Version: 0.1.8
+Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
+Home-page: https://github.com/astramind-ai/BitMat/tree/main
+Author: Marco Lironi
+Author-email: marcolironi@astramind.ai
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: triton
+Requires-Dist: transformers
+Requires-Dist: bitsandbytes
+Requires-Dist: numpy
+
 # BitMat: Improving Matrix Multiplication with Triton
 
-## Introduction
+## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
-## Features
+## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
-Packed int8 Operations: Follows the methodologies from the "1bit-LLM Era" to use packed int8 data, reducing memory usage and increasing throughput.
-Ease of Integration: BitMat is designed to be easily integrated into existing PyTorch workflows, providing a seamless user experience.
-Performance Boost: Significant performance improvements in matrix multiplication, especially beneficial for large-scale deep learning models and high-dimensional data.
-## Installation
+
+Packed int8 Operations: During inference the model uses packed int8 data to reduce memory usage and improve computational efficiency.
+
+Ease of Integration: BitMat is designed to be easily integrated into existing PyTorch/transformers workflows, providing a seamless user experience.
+## 💾 Installation
 ```bash
 pip install bitmat-tl
 ```
 At the moment we only support **Linux** platforms. **Windows** installation is possible but is not tested.
-## Quick Start
+## 🏁 Quick Start
 
 ### High-level API (tranformers-compatible)
 ```python
 from transformers import AutoModelForCausalLM
 from bitmat import convert_hf_model
 
 # Initialize your model
@@ -30,18 +50,18 @@
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
 ```
 
-## Contributing
+## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
-## License
+## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
 
 ## Citation
 If you use BitMat in your research, please cite it using the following Bibtex entry:
 
 ```bibtex
 @article{bitmat2024,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bitmat-tl-0.1.7/bitmat/bitlinear.py` & `bitmat-tl-0.1.8/bitmat/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.1.8/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.1.8/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.1.8/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat/utils/bitmat.py` & `bitmat-tl-0.1.8/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.1.8/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat/utils/packing.py` & `bitmat-tl-0.1.8/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.7/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.1.8/bitmat_tl.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.1.7
+Version: 0.1.8
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -15,28 +15,29 @@
 Requires-Dist: triton
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 
 # BitMat: Improving Matrix Multiplication with Triton
 
-## Introduction
+## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
-## Features
+## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
-Packed int8 Operations: Follows the methodologies from the "1bit-LLM Era" to use packed int8 data, reducing memory usage and increasing throughput.
-Ease of Integration: BitMat is designed to be easily integrated into existing PyTorch workflows, providing a seamless user experience.
-Performance Boost: Significant performance improvements in matrix multiplication, especially beneficial for large-scale deep learning models and high-dimensional data.
-## Installation
+
+Packed int8 Operations: During inference the model uses packed int8 data to reduce memory usage and improve computational efficiency.
+
+Ease of Integration: BitMat is designed to be easily integrated into existing PyTorch/transformers workflows, providing a seamless user experience.
+## 💾 Installation
 ```bash
 pip install bitmat-tl
 ```
 At the moment we only support **Linux** platforms. **Windows** installation is possible but is not tested.
-## Quick Start
+## 🏁 Quick Start
 
 ### High-level API (tranformers-compatible)
 ```python
 from transformers import AutoModelForCausalLM
 from bitmat import convert_hf_model
 
 # Initialize your model
@@ -49,18 +50,18 @@
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
 ```
 
-## Contributing
+## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
-## License
+## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
 
 ## Citation
 If you use BitMat in your research, please cite it using the following Bibtex entry:
 
 ```bibtex
 @article{bitmat2024,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bitmat-tl-0.1.7/setup.py` & `bitmat-tl-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.1.7',
+    version='0.1.8',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

