# Comparing `tmp/pycaptcha-guard-0.3.4.tar.gz` & `tmp/pycaptcha-guard-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaptcha-guard-0.3.4.tar", last modified: Wed Mar 27 05:31:59 2024, max compression
+gzip compressed data, was "pycaptcha-guard-0.3.5.tar", last modified: Tue Apr  2 04:33:48 2024, max compression
```

## Comparing `pycaptcha-guard-0.3.4.tar` & `pycaptcha-guard-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.314825 pycaptcha-guard-0.3.4/
--rw-rw-rw-   0        0        0     1090 2024-01-12 05:11:44.000000 pycaptcha-guard-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-03-27 05:31:59.312829 pycaptcha-guard-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-01-12 04:36:58.000000 pycaptcha-guard-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.254505 pycaptcha-guard-0.3.4/pycaptcha_guard/
--rw-rw-rw-   0        0        0        0 2023-12-25 14:14:20.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/__init__.py
--rw-rw-rw-   0        0        0     7408 2024-03-27 05:28:41.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/base_page.py
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.289828 pycaptcha-guard-0.3.4/pycaptcha_guard/capsolver_solution/
--rw-rw-rw-   0        0        0        0 2024-03-20 08:28:41.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/capsolver_solution/__init__.py
--rw-rw-rw-   0        0        0    11849 2024-03-27 05:28:00.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/capsolver_solution/google_recaptcha.py
--rw-rw-rw-   0        0        0     4167 2024-03-27 05:28:11.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/capsolver_solution/textcaptcha.py
--rw-rw-rw-   0        0        0     1791 2024-03-27 05:28:01.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/captcha.py
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.296829 pycaptcha-guard-0.3.4/pycaptcha_guard/captcha_locators/
--rw-rw-rw-   0        0        0        0 2023-12-26 20:12:25.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/captcha_locators/__init__.py
--rw-rw-rw-   0        0        0     1331 2024-03-20 08:05:41.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/captcha_locators/google_recaptcha_locator.py
--rw-rw-rw-   0        0        0      195 2023-12-26 18:43:14.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/captcha_locators/textcaptcha_locator.py
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.300831 pycaptcha-guard-0.3.4/pycaptcha_guard/common_components/
--rw-rw-rw-   0        0        0        0 2023-12-26 20:12:14.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/common_components/__init__.py
--rw-rw-rw-   0        0        0      273 2024-02-15 06:11:34.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/common_components/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.306828 pycaptcha-guard-0.3.4/pycaptcha_guard/nopecha_solution/
--rw-rw-rw-   0        0        0        0 2023-12-26 20:12:00.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/nopecha_solution/__init__.py
--rw-rw-rw-   0        0        0     9820 2024-03-27 05:28:00.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/nopecha_solution/google_recaptcha.py
--rw-rw-rw-   0        0        0     3333 2024-03-27 05:28:00.000000 pycaptcha-guard-0.3.4/pycaptcha_guard/nopecha_solution/textcaptcha.py
-drwxrwxrwx   0        0        0        0 2024-03-27 05:31:59.309830 pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/
--rw-rw-rw-   0        0        0      474 2024-03-27 05:31:59.000000 pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-03-27 05:31:59.000000 pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 05:31:59.000000 pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-03-27 05:31:59.000000 pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-27 05:31:59.000000 pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 05:31:59.315828 pycaptcha-guard-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      591 2024-03-27 05:17:10.000000 pycaptcha-guard-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.222552 pycaptcha-guard-0.3.5/
+-rw-rw-rw-   0        0        0     1090 2024-01-12 05:11:44.000000 pycaptcha-guard-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-02 04:33:48.220561 pycaptcha-guard-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-01-12 04:36:58.000000 pycaptcha-guard-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.171567 pycaptcha-guard-0.3.5/pycaptcha_guard/
+-rw-rw-rw-   0        0        0        0 2023-12-25 14:14:20.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/__init__.py
+-rw-rw-rw-   0        0        0     7588 2024-04-02 04:16:44.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/base_page.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.200554 pycaptcha-guard-0.3.5/pycaptcha_guard/capsolver_solution/
+-rw-rw-rw-   0        0        0        0 2024-03-20 08:28:41.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/capsolver_solution/__init__.py
+-rw-rw-rw-   0        0        0    12045 2024-04-02 04:30:22.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/capsolver_solution/google_recaptcha.py
+-rw-rw-rw-   0        0        0     4167 2024-03-28 05:14:09.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/capsolver_solution/textcaptcha.py
+-rw-rw-rw-   0        0        0     1791 2024-03-27 05:28:01.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/captcha.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.207555 pycaptcha-guard-0.3.5/pycaptcha_guard/captcha_locators/
+-rw-rw-rw-   0        0        0        0 2023-12-26 20:12:25.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/captcha_locators/__init__.py
+-rw-rw-rw-   0        0        0     1331 2024-03-20 08:05:41.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/captcha_locators/google_recaptcha_locator.py
+-rw-rw-rw-   0        0        0      195 2023-12-26 18:43:14.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/captcha_locators/textcaptcha_locator.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.211554 pycaptcha-guard-0.3.5/pycaptcha_guard/common_components/
+-rw-rw-rw-   0        0        0        0 2023-12-26 20:12:14.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/common_components/__init__.py
+-rw-rw-rw-   0        0        0      273 2024-02-15 06:11:34.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/common_components/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.216550 pycaptcha-guard-0.3.5/pycaptcha_guard/nopecha_solution/
+-rw-rw-rw-   0        0        0        0 2023-12-26 20:12:00.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/nopecha_solution/__init__.py
+-rw-rw-rw-   0        0        0    10211 2024-04-01 09:02:24.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/nopecha_solution/google_recaptcha.py
+-rw-rw-rw-   0        0        0     3512 2024-04-01 07:10:46.000000 pycaptcha-guard-0.3.5/pycaptcha_guard/nopecha_solution/textcaptcha.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:33:48.219557 pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-02 04:33:48.000000 pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2024-04-02 04:33:48.000000 pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:33:48.000000 pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-02 04:33:48.000000 pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 04:33:48.000000 pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:33:48.222552 pycaptcha-guard-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      591 2024-04-02 04:33:35.000000 pycaptcha-guard-0.3.5/setup.py
```

### Comparing `pycaptcha-guard-0.3.4/LICENSE` & `pycaptcha-guard-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/base_page.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,19 @@
         
         self.driver.execute_script("window.onfocus")
         element = self.wait_for_element(by_locator)
 
         if element:
             for one in text:
                 element.send_keys(one)
-
-            self.press_enter_on_element(by_locator)
+            try:
+                self.press_enter_on_element(by_locator)
+            except Exception as e:
+                logging.exception(f"Failed to press enter on element {by_locator}: {e}")
+                element.submit()
         time.sleep(2) 
         
         
     def press_enter_on_element(self, locator: Tuple[str, str]):
         """
             Take the element and press enter in that element
```

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/capsolver_solution/google_recaptcha.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/capsolver_solution/google_recaptcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import capsolver
 import requests
 import base64
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.common.exceptions import StaleElementReferenceException
+from selenium.common.exceptions import StaleElementReferenceException, WebDriverException
 
 from pycaptcha_guard.base_page import BasePage
 from pycaptcha_guard.captcha_locators.google_recaptcha_locator import GoogleReCaptchaLocator
 from pycaptcha_guard.common_components import constants
 
 
 class capsolverGoogleReCaptcha(BasePage):
@@ -61,15 +61,17 @@
                 except Exception as e:
                     logging.exception(f"Error while solving captcha {e}")
 
                     
                 logging.info('Going to switch to the default content')
                 self.switch_to_default_content()
             except StaleElementReferenceException:
-                logging.warning("Stale element reference error occured.")
+                logging.warning("Stale element reference error occurred while solving captcha.")
+            except WebDriverException:
+                logging.warning("Webdriver exception occurred while solving captcha Not connected to devtools")
 
             time.sleep(3)
             iframe_popup = self.wait_for_element(GoogleReCaptchaLocator.iframe_popup_recaptcha, constants.WAIT_TIMEOUT, silent=True)
             logging.info('Iframe found Trying again')
             if not iframe_popup:
                 self.captcha = False
```

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/capsolver_solution/textcaptcha.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/capsolver_solution/textcaptcha.py`

 * *Files identical despite different names*

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/captcha.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/captcha.py`

 * *Files identical despite different names*

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/captcha_locators/google_recaptcha_locator.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/captcha_locators/google_recaptcha_locator.py`

 * *Files identical despite different names*

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/nopecha_solution/google_recaptcha.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/nopecha_solution/google_recaptcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import logging
 import nopecha
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.common.exceptions import TimeoutException
+from selenium.common.exceptions import StaleElementReferenceException, WebDriverException
 
 from pycaptcha_guard.base_page import BasePage
 from pycaptcha_guard.captcha_locators.google_recaptcha_locator import GoogleReCaptchaLocator
 from pycaptcha_guard.common_components import constants
 
 
 class nopechaGoogleReCaptcha(BasePage):
@@ -43,28 +43,33 @@
             if round(time.time() - start_time) > constants.CAPTCHA_MAX_TIME:
                 logging.info('Going to click to checkbox again')
                 start_time = time.time()
                 self.click_captcha_checkbox()
             
             tries_count += 1
             
-            iframe_popup = self.wait_for_element(GoogleReCaptchaLocator.iframe_popup_recaptcha)
-            time.sleep(2)
-            iframe_popup_measures = self.get_frame_axis(iframe_popup, GoogleReCaptchaLocator.iframe_popup_recaptcha)
-            self.switch_to_iframe(iframe_popup)
-            try:
-                logging.info("Solving captcha")
-                self.complete_captcha(iframe_popup_measures)                
-              
-            except Exception as e:
-                logging.exception(f"Error while solving captcha {e}")
-
+            try:            
+                iframe_popup = self.wait_for_element(GoogleReCaptchaLocator.iframe_popup_recaptcha)
+                time.sleep(2)
+                iframe_popup_measures = self.get_frame_axis(iframe_popup, GoogleReCaptchaLocator.iframe_popup_recaptcha)
+                self.switch_to_iframe(iframe_popup)
+                try:
+                    logging.info("Solving captcha")
+                    self.complete_captcha(iframe_popup_measures)                
                 
-            logging.info('Going to switch to the default content')
-            self.switch_to_default_content()
+                except Exception as e:
+                    logging.exception(f"Error while solving captcha {e}")
+
+                    
+                logging.info('Going to switch to the default content')
+                self.switch_to_default_content()
+            except StaleElementReferenceException:
+                logging.warning("Stale element reference error occurred while solving captcha.")
+            except WebDriverException:
+                logging.warning("Webdriver exception occurred while solving captcha")
 
             time.sleep(3)
             iframe_popup = self.wait_for_element(GoogleReCaptchaLocator.iframe_popup_recaptcha, constants.WAIT_TIMEOUT, silent=True)
             logging.info('Iframe found Trying again')
             if not iframe_popup:
                 self.captcha = False
```

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard/nopecha_solution/textcaptcha.py` & `pycaptcha-guard-0.3.5/pycaptcha_guard/nopecha_solution/textcaptcha.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,19 @@
                 try:
                     solution = self.get_captcha_solution(captcha_image_src)
                     break
                 except Exception as e:
                     logging.exception(f"Unable to get API response {e}")
                     time.sleep(4)
                     
-            self.captcha = self.fill_input_field(solution)
+            try:       
+                self.captcha = self.fill_input_field(solution)
+            except Exception as e:
+                logging.exception(f"Unable to write the solution in input field {e}")
+            time.sleep(2)
         return self.captcha, tries_count
         
         
     def get_textcaptcha_params(self):
         
         """
             Retrieves the URL of the text captcha image.
```

### Comparing `pycaptcha-guard-0.3.4/pycaptcha_guard.egg-info/SOURCES.txt` & `pycaptcha-guard-0.3.5/pycaptcha_guard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycaptcha-guard-0.3.4/setup.py` & `pycaptcha-guard-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 setuptools.setup(
     name="pycaptcha-guard",
-    version="0.3.4",
+    version="0.3.5",
     author="AleenaMuskan",
     author_email="aleenakhanraees40@gmail.com",
     description="Solve any kind of captcha like human",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=[
         "nopecha==1.0.8",
-        "selenium==4.16.0",
+        "selenium>=4.16.0",
         "pillow==10.1.0",
         "pyautogui==0.9.54",
         "capsolver==1.0.7"
     ],
     python_requires=">=3.9",
 )
```

