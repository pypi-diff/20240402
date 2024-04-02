# Comparing `tmp/rocat-0.1.11.tar.gz` & `tmp/rocat-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.1.11.tar", last modified: Mon Apr  1 16:01:09 2024, max compression
+gzip compressed data, was "rocat-0.1.12.tar", last modified: Mon Apr  1 16:32:03 2024, max compression
```

## Comparing `rocat-0.1.11.tar` & `rocat-0.1.12.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.988465 rocat-0.1.11/
--rw-rw-rw-   0        0        0       28 2024-04-01 16:00:53.000000 rocat-0.1.11/MANIFEST.in
--rw-rw-rw-   0        0        0     1332 2024-04-01 16:01:09.987464 rocat-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     1028 2024-04-01 16:00:52.000000 rocat-0.1.11/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.973894 rocat-0.1.11/rocat/
--rw-rw-rw-   0        0        0      133 2024-04-01 16:00:58.000000 rocat-0.1.11/rocat/__init__.py
--rw-rw-rw-   0        0        0      664 2024-04-01 16:00:57.000000 rocat-0.1.11/rocat/chatbot_app.py
--rw-rw-rw-   0        0        0      888 2024-04-01 16:00:56.000000 rocat-0.1.11/rocat/chatbot_modules.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.986465 rocat-0.1.11/rocat.egg-info/
--rw-rw-rw-   0        0        0     1332 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 16:01:09.988465 rocat-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-01 16:00:49.000000 rocat-0.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.985465 rocat-0.1.11/test/
--rw-rw-rw-   0        0        0      286 2024-04-01 15:56:26.000000 rocat-0.1.11/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:03.910059 rocat-0.1.12/
+-rw-rw-rw-   0        0        0     1081 2024-04-01 16:05:34.000000 rocat-0.1.12/LICENSE
+-rw-rw-rw-   0        0        0       28 2024-04-01 16:00:53.000000 rocat-0.1.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     1573 2024-04-01 16:32:03.909060 rocat-0.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2024-04-01 16:25:47.000000 rocat-0.1.12/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:03.893987 rocat-0.1.12/rocat/
+-rw-rw-rw-   0        0        0      133 2024-04-01 16:22:00.000000 rocat-0.1.12/rocat/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-04-01 16:21:57.000000 rocat-0.1.12/rocat/chatbot_app.py
+-rw-rw-rw-   0        0        0      888 2024-04-01 16:21:55.000000 rocat-0.1.12/rocat/chatbot_modules.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:03.908059 rocat-0.1.12/rocat.egg-info/
+-rw-rw-rw-   0        0        0     1573 2024-04-01 16:32:03.000000 rocat-0.1.12/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-01 16:32:03.000000 rocat-0.1.12/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:32:03.000000 rocat-0.1.12/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 16:32:03.000000 rocat-0.1.12/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-01 16:32:03.000000 rocat-0.1.12/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:32:03.910059 rocat-0.1.12/setup.cfg
+-rw-rw-rw-   0        0        0      678 2024-04-01 16:32:01.000000 rocat-0.1.12/setup.py
```

### Comparing `rocat-0.1.11/PKG-INFO` & `rocat-0.1.12/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-Metadata-Version: 2.1
-Name: rocat
-Version: 0.1.11
-Summary: A simple and user-friendly library for AI services
-Home-page: https://github.com/root39293/rocat
-Author: YumetaLab
-Author-email: root@yumeta.kr
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: streamlit
-
 # RoCat: A Simple and User-Friendly Library for AI Services
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects.
 
 ## Installation
 
 You can install RoCat using pip:
 
 ​```
 pip install rocat
 ​```
 
 ## Usage
 
+How to use it
+
+```python
+# main.py
+import rocat as rc
+
+api_key = "your-apikey-here"
+system_prompt = "system-prompt-here"
+app = rc.ChatbotApp(api_key, system_prompt)
+app.create_app()
+```
+
+Running in a streamlit environment
+
+```bash
+streamlit run main.py
+```
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
 
 ## Contributing
 
-Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yourusername/rocat).
+Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/Yumeta-Lab/rocat).
 
 ## Acknowledgements
 
 RoCat is built on top of the following libraries:
 - [OpenAI](https://openai.com/) - API for AI services
 - [Streamlit](https://streamlit.io/) - Framework for building web applications
 
 ## Contact
 
 If you have any questions or inquiries, please contact the author:
 
 - Name: Faith6
-- Email: root@yumeta.kr
-- GitHub: [Yumeta-Lab](https://github.com/Yumeta-Lab)
+- Email: root@yumeta.kr
```

### Comparing `rocat-0.1.11/rocat/chatbot_app.py` & `rocat-0.1.12/rocat/chatbot_app.py`

 * *Files identical despite different names*

### Comparing `rocat-0.1.11/rocat/chatbot_modules.py` & `rocat-0.1.12/rocat/chatbot_modules.py`

 * *Files identical despite different names*

### Comparing `rocat-0.1.11/rocat.egg-info/PKG-INFO` & `rocat-0.1.12/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.11
+Version: 0.1.12
 Summary: A simple and user-friendly library for AI services
-Home-page: https://github.com/root39293/rocat
+Home-page: https://github.com/Yumeta-Lab/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: streamlit
 
 # RoCat: A Simple and User-Friendly Library for AI Services
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects.
 
@@ -19,29 +20,45 @@
 
 ​```
 pip install rocat
 ​```
 
 ## Usage
 
+How to use it
+
+```python
+# main.py
+import rocat as rc
+
+api_key = "your-apikey-here"
+system_prompt = "system-prompt-here"
+app = rc.ChatbotApp(api_key, system_prompt)
+app.create_app()
+```
+
+Running in a streamlit environment
+
+```bash
+streamlit run main.py
+```
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
 
 ## Contributing
 
-Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yourusername/rocat).
+Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/Yumeta-Lab/rocat).
 
 ## Acknowledgements
 
 RoCat is built on top of the following libraries:
 - [OpenAI](https://openai.com/) - API for AI services
 - [Streamlit](https://streamlit.io/) - Framework for building web applications
 
 ## Contact
 
 If you have any questions or inquiries, please contact the author:
 
 - Name: Faith6
 - Email: root@yumeta.kr
-- GitHub: [Yumeta-Lab](https://github.com/Yumeta-Lab)
```

### Comparing `rocat-0.1.11/setup.py` & `rocat-0.1.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.1.11",
+    version="0.1.12",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
-    url="https://github.com/root39293/rocat",
+    url="https://github.com/Yumeta-Lab/rocat",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "openai",
         "streamlit",
     ],
     package_data={
         "": ["*.py"],
```

