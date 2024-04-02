# Comparing `tmp/yuag-0.0.57.tar.gz` & `tmp/yuag-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.57.tar", last modified: Mon Apr  1 20:28:18 2024, max compression
+gzip compressed data, was "yuag-0.0.58.tar", last modified: Tue Apr  2 13:45:42 2024, max compression
```

## Comparing `yuag-0.0.57.tar` & `yuag-0.0.58.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:28:18.247694 yuag-0.0.57/
--rw-rw-rw-   0        0        0       52 2024-04-01 20:28:18.244698 yuag-0.0.57/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-01 20:28:18.247694 yuag-0.0.57/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-01 20:28:08.000000 yuag-0.0.57/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:28:18.208681 yuag-0.0.57/yuag/
--rw-rw-rw-   0        0        0     2619 2024-04-01 20:27:54.000000 yuag-0.0.57/yuag/__init__.py
--rw-rw-rw-   0        0        0    30306 2024-04-01 20:27:43.000000 yuag-0.0.57/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:28:18.243691 yuag-0.0.57/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-01 20:28:17.000000 yuag-0.0.57/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-01 20:28:18.000000 yuag-0.0.57/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:28:17.000000 yuag-0.0.57/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-01 20:28:17.000000 yuag-0.0.57/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 13:45:42.705934 yuag-0.0.58/
+-rw-rw-rw-   0        0        0       52 2024-04-02 13:45:42.702935 yuag-0.0.58/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:45:42.706934 yuag-0.0.58/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-02 13:45:35.000000 yuag-0.0.58/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:45:42.670728 yuag-0.0.58/yuag/
+-rw-rw-rw-   0        0        0     2619 2024-04-01 20:27:54.000000 yuag-0.0.58/yuag/__init__.py
+-rw-rw-rw-   0        0        0    30730 2024-04-02 13:45:24.000000 yuag-0.0.58/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:45:42.701381 yuag-0.0.58/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-02 13:45:42.000000 yuag-0.0.58/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-02 13:45:42.000000 yuag-0.0.58/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:45:42.000000 yuag-0.0.58/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 13:45:42.000000 yuag-0.0.58/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.57/yuag/__init__.py` & `yuag-0.0.58/yuag/__init__.py`

 * *Files identical despite different names*

### Comparing `yuag-0.0.57/yuag/yuag.py` & `yuag-0.0.58/yuag/yuag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-import mouse
-import keyboard
-import requests
-from bs4 import BeautifulSoup
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-import time
-import os
-import json
-import re
-import base64
-import shutil
-
-
-
 # استدعاء المكتبات
 def PyPDF2():
     import PyPDF2
     return PyPDF2
 
 def Translator():
     from googletrans import Translator
-    return Translator
-
     from langdetect import detect
 
+    return Translator
+
 def openai():
     import openai
+
     return openai
 
 # global defs
 def wait(wait_time: int = 1):
+    import time
+
     time.sleep(wait_time)
 
 def clear():
+    import os
+
     os.system("cls")
 
 def detect_lang(text: str, detectOrSrc: int = 0):
     from googletrans import Translator
     from langdetect import detect
     
     try:
@@ -56,17 +46,21 @@
             res.append(i)
             i += 1
 
         return res
 
 # file defs
 def filesIn(folder_path: str = "./"):
+    import os
+
     return os.listdir(folder_path)
 
 def rename_file(file_path: str, new_name: str):
+    import os
+
     os.rename(file_path, new_name)
 
 def saveFile(data, file_path: str, encoding: str = "utf-8", save_mode = "w"):
     with open(file_path, save_mode, encoding=encoding) as output_file:
         output_file.write(data)
 
 def readFile(file_path: str, errorAs = 404, errorOnly: int = 0, encoding: str = "utf-8"):
@@ -77,33 +71,39 @@
     except Exception as error:
         if errorOnly == 0:
             return errorAs
         else:
             return error
 
 def readJSON(file_path: str, errorAs = 404, errorOnly: int = 0, encoding: str = "utf-8"):
+    import json
+
     try:
         with open(file_path, 'r', encoding=encoding) as file:
             data = json.load(file)
             return data
     except Exception as error:
         if errorOnly == 0:
             return errorAs
         else:
             return error
 
 def saveJson(data: dict, file_path: str, indent: int = 4, encoding: str = "utf-8", save_mode = "w"):
+    import json
+
     with open(file_path, save_mode, encoding=encoding) as output_file:
         json.dump(data, output_file, indent=indent, ensure_ascii=False)
 
 def savePdf(merger, output_file_path, encoding = "utf-8"):
     with open(output_file_path, "wb", encoding=encoding) as output_file:
         merger.write(output_file)
 
 def copy_file(file_path: str, new_file_path: str = None):
+    import shutil
+
     if new_file_path is None:
         new_file_path = f"{file_path} - Copy"
 
     shutil.copy(file_path, new_file_path)
 
 def move_file(file_path: str, new_folder_path: str = None):
     """
@@ -113,20 +113,26 @@
     ------------
     ```
     file_path = "file.txt"
     new_folder_path = "./folder"
     ```
     """
 
+    import shutil
+
     shutil.move(file_path, new_folder_path)
 
 def delete_file(file_path):
+    import os
+
     os.remove(file_path)
 
 def delete_folder(folder_path):
+    import shutil
+
     shutil.rmtree(folder_path)
 
 # arr defs
 def equalArr(arr: list, dimensions: int = 1): # arr1 = arr2
     '''
     equalArr
     -----------------
@@ -846,14 +852,16 @@
 
     ...\n
     النتيجة:
     ---
     the_link.com
     '''
 
+    import re
+
     if attribute != "":
         check = rf'<{tag} .*?{attribute}="([^"]*)".*?>'
         if endTag == 1: check += rf'.*?</{tag}>'
     else: # inner html
         check = rf'<{tag}.*?>'
         if delete_inner_html == 0:
             check += rf'([^"]*)'
@@ -890,47 +898,63 @@
         else:
             newObj[key] = item
     
     return newObj
 
 # keyboard defs
 def write(text: str, delay: float = 0, restore_state_after: bool = True, exact: bool | None = None):
+    import keyboard
+
     keyboard.write(text, delay, restore_state_after, exact)
 
 def press(hot_key):
+    import keyboard
+
     keyboard.press(hot_key)
 
 def unpress(hot_key):
+    import keyboard
+
     keyboard.release(hot_key)
 
 # mouse defs
 def getMousePosition():
+    import mouse
+
     return [mouse.get_position()[0], mouse.get_position()[1]]
 
 def getMousePositions(saveKey: str ="g", breakKey: str ="0"):
+    import keyboard
+
     all = []
 
     while True:
         if keyboard.is_pressed(saveKey):
             mouse_position = getMousePosition()
             item = input("what is it?\n")
             all.append([ item, mouse_position ])
 
         if keyboard.is_pressed(breakKey):
             break
 
     return all
 
 def click():
+    import mouse
+
     mouse.click()
 
 def right_click():
+    import mouse
+
     mouse.right_click()
 
 def move(x: int, y: int, absolute: bool = True, duration: int = 0):
+    import mouse
+
     mouse.move(x, y, absolute, duration)
 
 # chatGPT
 def chatGPT(user_question: str, api_key: str):
     import openai
 
     openai.api_key = api_key
@@ -946,14 +970,18 @@
     )
 
     answer = response["choices"][0]["message"]["content"]
     return answer
 
 # soup
 def get_soup(link: str, wait: int = 0):
+    from bs4 import BeautifulSoup
+    import requests
+    import time
+
     headers = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'
     }
 
     with requests.Session() as session:
         try:
             result = session.get(link, headers=headers, timeout=10)
@@ -963,14 +991,16 @@
             soup = BeautifulSoup(src, "lxml")
             return soup
         except requests.exceptions.RequestException as e:
             # print(f"Error: {e}")
             return None
 
 def get_redirected_url(link: str): # bit.ly ==> link
+    import requests
+
     # إجراء طلب GET للحصول على الصفحة الأولى
     response = requests.get(link)
 
     # التحقق من وجود عملية تحويل
     if response.history:
         # الحصول على الرابط النهائي بعد التحويل
         final_url = response.url
@@ -982,36 +1012,46 @@
     return item.text
 
 def innerHTML(item):
     return "".join(map(str, item.contents))
 
 # selenium
 def makeFirefoxDriver():
+    from selenium import webdriver
+    from selenium.webdriver.common.by import By
+
     options = webdriver.FirefoxOptions()
     options.add_argument('--headless')
     driver = webdriver.Firefox()
 
     return driver
 
 def driverToSoup(driver):
+    from bs4 import BeautifulSoup
+
     return BeautifulSoup(driver.page_source, "html.parser")
 
 # dataURL
 def imageLink_to_dataurl(image_url, extension = "png", error = 404):
+    import base64
+    import requests
+
     # تنزيل الصورة من الرابط
     response = requests.get(image_url)
     
     # التحقق من أن الاستجابة صحيحة
     if response.status_code == 200:
         data_url = f'data:image/{extension};base64,' + base64.b64encode(response.content).decode('utf-8')
         return data_url
     else:
         return error
 
 def videoFile_to_dataurl(video_path, error = 404):
+    import base64
+
     try:
         # قراءة ملف الفيديو كتسلسل بيانات
         with open(video_path, "rb") as video_file:
             video_data = video_file.read()
 
         # تحويل التسلسل إلى base64
         video_base64 = base64.b64encode(video_data)
```

