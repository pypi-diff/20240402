# Comparing `tmp/llm-api-open-2.1.19.tar.gz` & `tmp/llm-api-open-2.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-api-open-2.1.19.tar", last modified: Tue Apr  2 16:50:28 2024, max compression
+gzip compressed data, was "llm-api-open-2.1.20.tar", last modified: Tue Apr  2 16:59:15 2024, max compression
```

## Comparing `llm-api-open-2.1.19.tar` & `llm-api-open-2.1.20.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.241684 llm-api-open-2.1.19/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15595 2024-04-02 16:50:28.237684 llm-api-open-2.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.233684 llm-api-open-2.1.19/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/configs/chatgpt.json
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/configs/ms_copilot.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:50:28.241684 llm-api-open-2.1.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.233684 llm-api-open-2.1.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.237684 llm-api-open-2.1.19/src/llm_api_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15595 2024-04-02 16:50:28.000000 llm-api-open-2.1.19/src/llm_api_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 16:50:28.000000 llm-api-open-2.1.19/src/llm_api_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:50:28.000000 llm-api-open-2.1.19/src/llm_api_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 16:50:28.000000 llm-api-open-2.1.19/src/llm_api_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 16:50:28.000000 llm-api-open-2.1.19/src/llm_api_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 16:50:28.000000 llm-api-open-2.1.19/src/llm_api_open.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.237684 llm-api-open-2.1.19/src/lmao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.237684 llm-api-open-2.1.19/src/lmao/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/chatgpt/assistantGetLastMessage.js
--rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/chatgpt/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/chatgpt/conversationSearch.js
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/chatgpt/proxy_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/external_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/module_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:50:28.237684 llm-api-open-2.1.19/src/lmao/ms_copilot/
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/ms_copilot/conversationManage.js
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/ms_copilot/conversationParser.js
--rw-r--r--   0 runner    (1001) docker     (127)    43378 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/ms_copilot/ms_copilot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 16:50:22.000000 llm-api-open-2.1.19/src/lmao/ms_copilot/proxy_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.653622 llm-api-open-2.1.20/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/configs/chatgpt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/configs/ms_copilot.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.653622 llm-api-open-2.1.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/src/llm_api_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-02 16:59:15.000000 llm-api-open-2.1.20/src/llm_api_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 16:59:15.000000 llm-api-open-2.1.20/src/llm_api_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:59:15.000000 llm-api-open-2.1.20/src/llm_api_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 16:59:15.000000 llm-api-open-2.1.20/src/llm_api_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 16:59:15.000000 llm-api-open-2.1.20/src/llm_api_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 16:59:15.000000 llm-api-open-2.1.20/src/llm_api_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/src/lmao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/src/lmao/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/chatgpt/assistantGetLastMessage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/chatgpt/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/chatgpt/conversationSearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/chatgpt/proxy_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/external_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/module_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:59:15.657622 llm-api-open-2.1.20/src/lmao/ms_copilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/ms_copilot/conversationManage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/ms_copilot/conversationParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43378 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/ms_copilot/ms_copilot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 16:58:58.000000 llm-api-open-2.1.20/src/lmao/ms_copilot/proxy_extension.py
```

### Comparing `llm-api-open-2.1.19/LICENSE` & `llm-api-open-2.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/PKG-INFO` & `llm-api-open-2.1.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.19
+Version: 2.1.20
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -33,16 +33,16 @@
 Requires-Dist: undetected-chromedriver>=3.5.5
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: markdownify>=0.11.6
 Requires-Dist: Flask>=3.0.2
 
 # 🕊️ LLM-API-Open (LMAO)
 
-| <img src="brandbook/Logo.png" height="auto" width="128" alt="PetalFlow logo"> | <h3>Unofficial open APIs for popular LLMs with self-hosted redirect capability</h3> |
-| ----------------------------------------------------------------------------- | :---------------------------------------------------------------------------------: |
+| <img src="https://github.com/F33RNI/LlM-Api-Open/blob/main/brandbook/Logo.png?raw=true" height="auto" width="128" alt="LLM-API-Open logo"> | <h3>Unofficial open APIs for popular LLMs with self-hosted redirect capability</h3> |
+| ------------------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------: |
 
 ----------
 
 ## ❓ WAT
 
 > 🕊️ LLM-API-Open (LMAO) allows for the free and universal utilization of popular Large Language Models (LLM).
 > This is achieved using browser automation. LLM-API-Open (LMAO) launches a browser in headless mode and controls a website as if a real user were using it.
@@ -81,15 +81,21 @@
 
 ### ⚙️ 1. Download / build / install LLM-API-Open
 
 There is 4 general ways to get LLM-API-Open
 
 #### ⚙️ Install via `pip`
 
-- Install from GitHub directly
+- Install from PyPi
+
+    ```shell
+    pip install llm-api-open
+    ```
+
+- **Or** install from GitHub directly
 
     ```shell
     pip install git+https://github.com/F33RNI/LLM-API-Open.git
     ```
 
 - **Or** clone repo and install
```

### Comparing `llm-api-open-2.1.19/README.md` & `llm-api-open-2.1.20/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 🕊️ LLM-API-Open (LMAO)
 
-| <img src="brandbook/Logo.png" height="auto" width="128" alt="PetalFlow logo"> | <h3>Unofficial open APIs for popular LLMs with self-hosted redirect capability</h3> |
-| ----------------------------------------------------------------------------- | :---------------------------------------------------------------------------------: |
+| <img src="https://github.com/F33RNI/LlM-Api-Open/blob/main/brandbook/Logo.png?raw=true" height="auto" width="128" alt="LLM-API-Open logo"> | <h3>Unofficial open APIs for popular LLMs with self-hosted redirect capability</h3> |
+| ------------------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------: |
 
 ----------
 
 ## ❓ WAT
 
 > 🕊️ LLM-API-Open (LMAO) allows for the free and universal utilization of popular Large Language Models (LLM).
 > This is achieved using browser automation. LLM-API-Open (LMAO) launches a browser in headless mode and controls a website as if a real user were using it.
@@ -44,15 +44,21 @@
 
 ### ⚙️ 1. Download / build / install LLM-API-Open
 
 There is 4 general ways to get LLM-API-Open
 
 #### ⚙️ Install via `pip`
 
-- Install from GitHub directly
+- Install from PyPi
+
+    ```shell
+    pip install llm-api-open
+    ```
+
+- **Or** install from GitHub directly
 
     ```shell
     pip install git+https://github.com/F33RNI/LLM-API-Open.git
     ```
 
 - **Or** clone repo and install
```

### Comparing `llm-api-open-2.1.19/configs/chatgpt.json` & `llm-api-open-2.1.20/configs/chatgpt.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/configs/ms_copilot.json` & `llm-api-open-2.1.20/configs/ms_copilot.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/setup.py` & `llm-api-open-2.1.20/setup.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/llm_api_open.egg-info/PKG-INFO` & `llm-api-open-2.1.20/src/llm_api_open.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.19
+Version: 2.1.20
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -33,16 +33,16 @@
 Requires-Dist: undetected-chromedriver>=3.5.5
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: markdownify>=0.11.6
 Requires-Dist: Flask>=3.0.2
 
 # 🕊️ LLM-API-Open (LMAO)
 
-| <img src="brandbook/Logo.png" height="auto" width="128" alt="PetalFlow logo"> | <h3>Unofficial open APIs for popular LLMs with self-hosted redirect capability</h3> |
-| ----------------------------------------------------------------------------- | :---------------------------------------------------------------------------------: |
+| <img src="https://github.com/F33RNI/LlM-Api-Open/blob/main/brandbook/Logo.png?raw=true" height="auto" width="128" alt="LLM-API-Open logo"> | <h3>Unofficial open APIs for popular LLMs with self-hosted redirect capability</h3> |
+| ------------------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------: |
 
 ----------
 
 ## ❓ WAT
 
 > 🕊️ LLM-API-Open (LMAO) allows for the free and universal utilization of popular Large Language Models (LLM).
 > This is achieved using browser automation. LLM-API-Open (LMAO) launches a browser in headless mode and controls a website as if a real user were using it.
@@ -81,15 +81,21 @@
 
 ### ⚙️ 1. Download / build / install LLM-API-Open
 
 There is 4 general ways to get LLM-API-Open
 
 #### ⚙️ Install via `pip`
 
-- Install from GitHub directly
+- Install from PyPi
+
+    ```shell
+    pip install llm-api-open
+    ```
+
+- **Or** install from GitHub directly
 
     ```shell
     pip install git+https://github.com/F33RNI/LLM-API-Open.git
     ```
 
 - **Or** clone repo and install
```

### Comparing `llm-api-open-2.1.19/src/llm_api_open.egg-info/SOURCES.txt` & `llm-api-open-2.1.20/src/llm_api_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/_version.py` & `llm-api-open-2.1.20/src/lmao/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = "2.1.19"
+__version__ = "2.1.20"
```

### Comparing `llm-api-open-2.1.19/src/lmao/chatgpt/assistantGetLastMessage.js` & `llm-api-open-2.1.20/src/lmao/chatgpt/assistantGetLastMessage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/chatgpt/chatgpt_api.py` & `llm-api-open-2.1.20/src/lmao/chatgpt/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/chatgpt/conversationSearch.js` & `llm-api-open-2.1.20/src/lmao/chatgpt/conversationSearch.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/chatgpt/proxy_extension.py` & `llm-api-open-2.1.20/src/lmao/chatgpt/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/external_api.py` & `llm-api-open-2.1.20/src/lmao/external_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/main.py` & `llm-api-open-2.1.20/src/lmao/main.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/module_wrapper.py` & `llm-api-open-2.1.20/src/lmao/module_wrapper.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/ms_copilot/conversationManage.js` & `llm-api-open-2.1.20/src/lmao/ms_copilot/conversationManage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/ms_copilot/conversationParser.js` & `llm-api-open-2.1.20/src/lmao/ms_copilot/conversationParser.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/ms_copilot/ms_copilot_api.py` & `llm-api-open-2.1.20/src/lmao/ms_copilot/ms_copilot_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.19/src/lmao/ms_copilot/proxy_extension.py` & `llm-api-open-2.1.20/src/lmao/ms_copilot/proxy_extension.py`

 * *Files identical despite different names*

