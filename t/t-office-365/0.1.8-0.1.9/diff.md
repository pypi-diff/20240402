# Comparing `tmp/t_office_365-0.1.8.tar.gz` & `tmp/t_office_365-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-56facluj/t_office_365-0.1.8.tar", last modified: Fri Mar 22 23:04:42 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-0wbba3z4/t_office_365-0.1.9.tar", last modified: Wed Mar 27 09:33:54 2024, max compression
```

## Comparing `t_office_365-0.1.8.tar` & `t_office_365-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-22 23:04:42.471490 t_office_365-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-22 23:04:21.000000 t_office_365-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2257 2024-03-22 23:04:42.471490 t_office_365-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1473 2024-03-22 23:04:21.000000 t_office_365-0.1.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-22 23:04:21.000000 t_office_365-0.1.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-22 23:04:21.000000 t_office_365-0.1.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-03-22 23:04:42.471490 t_office_365-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1140 2024-03-22 23:04:21.000000 t_office_365-0.1.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-22 23:04:42.467491 t_office_365-0.1.8/t_office_365/
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/core.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/decorators.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-22 23:04:42.471490 t_office_365-0.1.8/t_office_365/drive/
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/drive/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15088 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/drive/drive.py
--rw-rw-rw-   0 root         (0) root         (0)     8241 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/drive/excel.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/drive/onedrive.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/drive/sharepoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-22 23:04:42.471490 t_office_365-0.1.8/t_office_365/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1395 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/endpoints/drive_api.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/endpoints/mail_api.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/endpoints/workbook_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-22 23:04:42.471490 t_office_365-0.1.8/t_office_365/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/exceptions/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/office.py
--rw-rw-rw-   0 root         (0) root         (0)    11408 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/outlook.py
--rw-rw-rw-   0 root         (0) root         (0)     2630 2024-03-22 23:04:21.000000 t_office_365-0.1.8/t_office_365/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-22 23:04:42.471490 t_office_365-0.1.8/t_office_365.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2257 2024-03-22 23:04:42.000000 t_office_365-0.1.8/t_office_365.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-03-22 23:04:42.000000 t_office_365-0.1.8/t_office_365.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-22 23:04:42.000000 t_office_365-0.1.8/t_office_365.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-22 23:04:42.000000 t_office_365-0.1.8/t_office_365.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-22 23:04:42.000000 t_office_365-0.1.8/t_office_365.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-03-22 23:04:42.000000 t_office_365-0.1.8/t_office_365.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-27 09:33:54.932923 t_office_365-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-27 09:33:24.000000 t_office_365-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-03-27 09:33:54.932923 t_office_365-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2024-03-27 09:33:24.000000 t_office_365-0.1.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-27 09:33:24.000000 t_office_365-0.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-27 09:33:24.000000 t_office_365-0.1.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-03-27 09:33:54.932923 t_office_365-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2024-03-27 09:33:24.000000 t_office_365-0.1.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-27 09:33:54.924923 t_office_365-0.1.9/t_office_365/
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/decorators.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-27 09:33:54.928923 t_office_365-0.1.9/t_office_365/drive/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/drive/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15088 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/drive/drive.py
+-rw-rw-rw-   0 root         (0) root         (0)     8241 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/drive/excel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/drive/onedrive.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/drive/sharepoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-27 09:33:54.928923 t_office_365-0.1.9/t_office_365/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/endpoints/drive_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/endpoints/mail_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/endpoints/workbook_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-27 09:33:54.928923 t_office_365-0.1.9/t_office_365/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/office.py
+-rw-rw-rw-   0 root         (0) root         (0)    11669 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/outlook.py
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2024-03-27 09:33:24.000000 t_office_365-0.1.9/t_office_365/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-27 09:33:54.928923 t_office_365-0.1.9/t_office_365.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-03-27 09:33:54.000000 t_office_365-0.1.9/t_office_365.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-03-27 09:33:54.000000 t_office_365-0.1.9/t_office_365.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-27 09:33:54.000000 t_office_365-0.1.9/t_office_365.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-27 09:33:54.000000 t_office_365-0.1.9/t_office_365.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-27 09:33:54.000000 t_office_365-0.1.9/t_office_365.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-03-27 09:33:54.000000 t_office_365-0.1.9/t_office_365.egg-info/top_level.txt
```

### Comparing `t_office_365-0.1.8/PKG-INFO` & `t_office_365-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_office_365
-Version: 0.1.8
+Version: 0.1.9
 Summary: An open-source Python package, t_office_365 providing easy-to-use classes and methods for     interacting with Microsoft Office 365 services, including SharePoint, OneDrive, Outlook, and Excel, with features     such as file management, email handling, and spreadsheet operations.
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_office_365
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_office_365-0.1.8/README.rst` & `t_office_365-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/setup.py` & `t_office_365-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     such as file management, email handling, and spreadsheet operations.",
     long_description=readme,
     keywords="t_office_365",
     name="t_office_365",
     packages=find_packages(include=["t_office_365", "t_office_365.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.1.8",
+    version="0.1.9",
     zip_safe=False,
     install_requires=install_requirements,
 )
```

### Comparing `t_office_365-0.1.8/t_office_365/core.py` & `t_office_365-0.1.9/t_office_365/core.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/drive/drive.py` & `t_office_365-0.1.9/t_office_365/drive/drive.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/drive/excel.py` & `t_office_365-0.1.9/t_office_365/drive/excel.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/drive/onedrive.py` & `t_office_365-0.1.9/t_office_365/drive/onedrive.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/drive/sharepoint.py` & `t_office_365-0.1.9/t_office_365/drive/sharepoint.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/endpoints/drive_api.py` & `t_office_365-0.1.9/t_office_365/endpoints/drive_api.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/endpoints/workbook_api.py` & `t_office_365-0.1.9/t_office_365/endpoints/workbook_api.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/exceptions/exceptions.py` & `t_office_365-0.1.9/t_office_365/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/office.py` & `t_office_365-0.1.9/t_office_365/office.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365/outlook.py` & `t_office_365-0.1.9/t_office_365/outlook.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,32 +83,25 @@
         if pattern_by_subject is not None:
             q_args.append(QueryMap(key="subject", value=pattern_by_subject, method="contains"))
         if from_email:
             q_args.append(QueryMap(key="from", value=from_email, method="equals"))
         if to:
             q_args.append(QueryMap(key="to", value=to, method="equals"))
         if after:
-            q_args.append(
-                QueryMap(key="receivedDateTime", value=after.strftime("%Y-%m-%dT%H:%M:%SZ"), method="greater_equal")
-            )
-            q_args.pop()
+            q_args.append(QueryMap(key="receivedDateTime", value=after, method="greater_equal"))
         if before:
-            q_args.append(
-                QueryMap(key="receivedDateTime", value=before.strftime("%Y-%m-%dT%H:%M:%SZ"), method="less_equal")
-            )
-            q_args.pop()
+            q_args.append(QueryMap(key="receivedDateTime", value=before, method="less_equal"))
 
         mailbox = self.account.mailbox()
-        query = self.__query_map(mailbox.new_query(), q_args)
-
         email_folder = mailbox.get_folder(folder_name=folder_name)
         if not email_folder:
             raise AssetNotFoundError(f'No such folder: "{folder_name}"')
 
-        messages = list(mailbox.get_messages(query=query))
+        query = self.__query_map(email_folder.new_query(), q_args)
+        messages = list(email_folder.get_messages(query=query))
         list(map(lambda m: m.attachments.download_attachments(), messages))
 
         if pattern_by_attachment:
             # Filter messages based on attachment filenames
             filtered_messages = []
             for message in messages:
                 attachments = message.attachments
@@ -142,16 +135,21 @@
 
         :return:
             None
         """
         m = self.account.new_message()
 
         # Add recipients (To and CC)
+        if isinstance(to, str):
+            to = [to]
+        if cc and isinstance(cc, str):
+            cc = [cc]
         list(map(lambda _to: m.to.add(_to), to))
-        list(map(lambda _cc: m.cc.add(_cc), cc))
+        if cc:
+            list(map(lambda _cc: m.cc.add(_cc), cc))
 
         # Set subject and body
         m.subject = subject
         m.body = body
 
         # Save the message
         m.save_message()
@@ -162,29 +160,31 @@
         # Set email body format (HTML or plain text)
         if html:
             m.body_format = "HTML"
 
         # Send the message
         m.send()
 
-    def get_attachment_by_subject(self, subject: str, pattern: re.Pattern, folder_name: str) -> str:
+    def get_attachment_by_subject(
+        self, subject: str, path_to_download_folder: str = "", pattern: re.Pattern = "", folder_name: str = "Inbox"
+    ) -> str:
         """Gets attachment from email by subject.
 
         :param:
             subject (str): Subject of the email to search for.
             pattern (str): Regular expression pattern to match for attachment file name.
             folder_name (str): Name of the folder to retrieve
 
         :return:
             str: File path of the saved attachment.
         """
         mailbox = self.account.mailbox()
         query = self.__query_map(mailbox.new_query(), [QueryMap(key="subject", value=subject, method="equals")])
-        calendar_folder = mailbox.get_folder(folder_name=folder_name)
-        return self.__download_attachments(calendar_folder, query, pattern)
+        folder = mailbox.get_folder(folder_name=folder_name)
+        return self.__download_attachments(folder, query, path_to_download_folder, pattern)
 
     def get_two_factor_code_email(
         self, subject_pattern: re.Pattern, otp_code_pattern: re.Pattern = r"\b\d{6}\b", folder_name: str = "Inbox"
     ) -> str:
         """Retrieve two-factor authentication code from email.
 
         :param:
@@ -208,55 +208,57 @@
                     return match.group(1)
             retry_count += 1
             time.sleep(5)
         else:
             raise ValueError("No email found")
 
     @staticmethod
-    def download_attachment(file: MessageAttachment, download_dir: str = None) -> str:
+    def download_attachment(file: MessageAttachment, download_dir: str = ""):
         """Download an attachment from an email message and save it to the specified directory.
 
         :param:
             file (MessageAttachment): The attachment file object to download.
             download_dir (str): The directory where the attachment will be saved.
 
         :return:
             str: The file path of the downloaded attachment.
         """
         if not download_dir:
-            download_dir = f"{os.getcwd()}/{file.name}"
-        file_path = os.path.join(download_dir)
+            download_dir = os.getcwd()
+        file_path = os.path.join(download_dir, file.name)
         with open(file_path, "wb") as w:
             decoded_content = base64.b64decode(file.content)
             w.write(decoded_content)
         return file_path
 
     @staticmethod
-    def __download_attachments(folder, query, pattern: re.Pattern = ""):
+    def __download_attachments(folder, query, path_to_download_folder: str = "", pattern: re.Pattern = ""):
         """Downloads attachments from messages in a folder that match a specified pattern.
 
         :param:
             folder (Folder): folder from which to retrieve messages.
             query (Query): query object to filter messages.
+            path_to_download_folder (str): path to the folder where the attachment will be saved.
             pattern (str): regular expression pattern to match attachment filenames.
 
         :return:
             str: File path of downloaded attachment.
 
         :raise:
             AttachmentNotFoundError: if no attachment found
         """
         messages = list(folder.get_messages(query=query, download_attachments=True))
         messages = list(filter(lambda x: any(re.match(pattern, f.name) for f in list(x.attachments)), messages))
         messages = sorted(messages, key=lambda x: x.received, reverse=True)
-
+        if not path_to_download_folder:
+            path_to_download_folder = os.getcwd()
         for message in messages:
             for file in message.attachments:
                 if re.match(pattern, file.name):
-                    file_path = os.path.join(os.getcwd(), file.name)
+                    file_path = os.path.join(path_to_download_folder, file.name)
                     with open(file_path, "wb") as w:
                         decoded_content = base64.b64decode(file.content)
                         w.write(decoded_content)
                     return file_path
         else:
             raise AssetNotFoundError("No attachment found")
```

### Comparing `t_office_365-0.1.8/t_office_365/utils.py` & `t_office_365-0.1.9/t_office_365/utils.py`

 * *Files identical despite different names*

### Comparing `t_office_365-0.1.8/t_office_365.egg-info/PKG-INFO` & `t_office_365-0.1.9/t_office_365.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_office_365
-Version: 0.1.8
+Version: 0.1.9
 Summary: An open-source Python package, t_office_365 providing easy-to-use classes and methods for     interacting with Microsoft Office 365 services, including SharePoint, OneDrive, Outlook, and Excel, with features     such as file management, email handling, and spreadsheet operations.
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_office_365
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_office_365-0.1.8/t_office_365.egg-info/SOURCES.txt` & `t_office_365-0.1.9/t_office_365.egg-info/SOURCES.txt`

 * *Files identical despite different names*

