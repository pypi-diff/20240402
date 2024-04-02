# Comparing `tmp/basecampapi-1.0.0.tar.gz` & `tmp/basecampapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basecampapi-1.0.0.tar", max compression
+gzip compressed data, was "basecampapi-1.1.0.tar", max compression
```

## Comparing `basecampapi-1.0.0.tar` & `basecampapi-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1072 2022-12-22 17:36:14.684065 basecampapi-1.0.0/LICENSE
--rw-r--r--   0        0        0     7690 2023-02-18 14:17:02.624641 basecampapi-1.0.0/README.md
--rw-r--r--   0        0        0      167 2023-02-18 13:33:05.634358 basecampapi-1.0.0/basecampapi/__init__.py
--rw-r--r--   0        0        0     2913 2023-02-18 13:33:05.634598 basecampapi-1.0.0/basecampapi/basecamp.py
--rw-r--r--   0        0        0     1463 2023-02-18 13:33:05.634778 basecampapi-1.0.0/basecampapi/endpoints/attachments.py
--rw-r--r--   0        0        0     2287 2023-02-18 13:33:05.635005 basecampapi-1.0.0/basecampapi/endpoints/camprife.py
--rw-r--r--   0        0        0     6711 2023-02-18 13:33:05.635223 basecampapi-1.0.0/basecampapi/endpoints/messageboard.py
--rw-r--r--   0        0        0      282 2023-02-18 14:18:20.103695 basecampapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8512 1970-01-01 00:00:00.000000 basecampapi-1.0.0/setup.py
--rw-r--r--   0        0        0     8201 1970-01-01 00:00:00.000000 basecampapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-22 17:36:14.684065 basecampapi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7690 2023-02-18 14:17:02.624641 basecampapi-1.1.0/README.md
+-rw-r--r--   0        0        0      167 2023-02-18 19:28:18.325956 basecampapi-1.1.0/basecampapi/__init__.py
+-rw-r--r--   0        0        0     2913 2023-02-18 13:33:05.634598 basecampapi-1.1.0/basecampapi/basecamp.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:16:19.554173 basecampapi-1.1.0/basecampapi/endpoints/__init__.py
+-rw-r--r--   0        0        0     2623 2024-04-02 10:16:19.554612 basecampapi-1.1.0/basecampapi/endpoints/attachments.py
+-rw-r--r--   0        0        0     2287 2023-02-18 13:33:05.635005 basecampapi-1.1.0/basecampapi/endpoints/camprife.py
+-rw-r--r--   0        0        0     6734 2023-02-22 12:52:01.602024 basecampapi-1.1.0/basecampapi/endpoints/messageboard.py
+-rw-r--r--   0        0        0      302 2024-04-02 10:16:19.555271 basecampapi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8538 1970-01-01 00:00:00.000000 basecampapi-1.1.0/setup.py
+-rw-r--r--   0        0        0     8242 1970-01-01 00:00:00.000000 basecampapi-1.1.0/PKG-INFO
```

### Comparing `basecampapi-1.0.0/LICENSE` & `basecampapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basecampapi-1.0.0/README.md` & `basecampapi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `basecampapi-1.0.0/basecampapi/basecamp.py` & `basecampapi-1.1.0/basecampapi/basecamp.py`

 * *Files identical despite different names*

### Comparing `basecampapi-1.0.0/basecampapi/endpoints/camprife.py` & `basecampapi-1.1.0/basecampapi/endpoints/camprife.py`

 * *Files identical despite different names*

### Comparing `basecampapi-1.0.0/basecampapi/endpoints/messageboard.py` & `basecampapi-1.1.0/basecampapi/endpoints/messageboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         Creates a new comment on a message board post. Comments can contain files and rich text.
 
         Parameters:
             message_id (int): The ID of the message on Basecamp to comment on.
             content (str): The body of the comment.
         '''
         create_comment_url = f"{self.__base_url}/buckets/{self.project_id}/recordings/{message_id}/comments.json"
-        response = requests.post(create_comment_url, headers=self.__headers, data='{"content": "'+content+'"}')
+        response = requests.post(create_comment_url, headers=self.__headers, data='{"content": "'+content+'"}') # TODO enable encoding
         if not response.ok:
             raise Exception(f"Status code: {response.status_code}. {response.reason}. Error text: {response.text}.")
         else:
             print("Comment created successfully!")
     
     def update_comment(self, comment_id: int, content: str):
         '''
```

### Comparing `basecampapi-1.0.0/setup.py` & `basecampapi-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['basecampapi', 'basecampapi.endpoints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests']
+['filetype>=1.2.0,<2.0.0', 'requests']
 
 setup_kwargs = {
     'name': 'basecampapi',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': '',
     'long_description': '# Basecamp API\n\nThis package allows simple interaction with [Basecamp API](https://github.com/basecamp/bc3-api) using Python.\n\n## Table of contents\n\n1. [Installation](https://github.com/mare011rs/basecampapi#1-installation)\n2. [Initial authentication: Getting your refresh token](https://github.com/mare011rs/basecampapi#2-initial-authentication-getting-your-refresh-token)\n3. [Authentication with Refresh token](https://github.com/mare011rs/basecampapi#3-authentication-with-refresh-token)\n4. [Attachments](https://github.com/mare011rs/basecampapi#4-attachments)\n5. [Additional information](https://github.com/mare011rs/basecampapi#5-additional-information)\n\n## 1. Installation\nThe package can be installed from your terminal by typing:\n\n    pip install basecampapi\n\nYou need to have python 3.7 or higher installed.\n\n\n## 2. Initial authentication: Getting your refresh token\n\n##### You only need to do this the first time. Once you get your Refresh token you should pass it with your credentials to gain access. \n##### If you already have a Refresh token you should skip this step.\n\nTo be able to interact with Basecamp\'s API, we need to provide an access token upon each API request. Basecamp\'s access tokens are set to expire 2 weeks after being generated, which is why we need to generate a refresh token.\n\nRefresh token allows us to automate the process of generating an access token. We only have to generate the refresh token once and after that we can use it to gain access to Basecamp each time we run our script.\n\nTo gain access you need a developer app on Basecamp. App can be created on https://launchpad.37signals.com/integrations, after which you need to use the generated Client ID, Client Secret and the Redirect URI which you provided for initial authentication. You can read more about the authentication process on [Basecamp API Authentication](https://github.com/basecamp/api/blob/master/sections/authentication.md) page.\n\nTo begin the authentication process, you need to create a dictionary with your app credentials and use it in the `Basecamp` object:\n\n```python\nfrom basecampapi import Basecamp\n\nyour_credentials = {\n\t"account_id": "your-account-id",\n\t"client_id": "your-client-id",\n\t"client_secret": "your-client-secret",\n\t"redirect_uri": "your-redirect-uri"\n}\n\nbc = Basecamp(credentials=your_credentials)\n```\nYour account ID can be found on your Basecamp home page, in the URL address:\n> https:<SPAN></SPAN>//3.basecamp.com/<b>YOUR-ACCOUNT-ID</b>/projects\n\nIf your credentials dictionary does not contain a "refresh_token", an error will be raised which contains a link for the authorization of your app. You need to open that link on the browser where you are logged into your Basecamp account and  click on "Yes, I\'ll allow access":\n\n![Verification page](https://user-images.githubusercontent.com/24939829/209202366-bae05d01-5f8d-4ca6-a0f8-5e1eb9088acd.png  "Verification page")\n\nClicking that button will redirect you to the link you provided as Redirect URI in your credentials, but it will have the verification code in the url address. Save that verification code:\n\n![Verification code](https://user-images.githubusercontent.com/24939829/209202400-d2aa342b-70e1-4fd1-9787-2f3dc1280a57.png  "Verification code")\n\nInitiate the `Basecamp` object again, and provide the code you gathered via the `verification_code` parameter:\n\n```python\n# Verification code variable \nyour_verification_code = "17beb4cd"\n\nbc = Basecamp(credentials=your_credentials, verification_code=your_verification_code)\n```\n\nThis will generate your Refresh token and use that token right away to generate the Access token for your current session. You need to generate your Refresh token only once, but that Refresh token will be used to generate Access token each time you initialize the `Basecamp` object.\n\n\n## 3. Authentication with Refresh token\n\nTo interact with objects on Basecamp you have to initialize the `Basecamo` object. This object will generate your access token and allow you to interact with other Basecamp objects. \n\n```python\nfrom basecampapi import Basecamp\n\nyour_credentials = {\n\t"account_id": "your-account-id",\n\t"client_id": "your-client-id",\n\t"client_secret": "your-client-secret",\n\t"redirect_uri": "your-redirect-uri",\n\t"refresh_token": "your-refresh-token"\n}\n\nbc = Basecamp(credentials=your_credentials)\n```\nThis generates the Access token which is then used in object that interact with Basecamp.\n\n```python\nfrom basecampapi import Campfire\n\n# Initiates a Campfire object using previously created session\nyour_campfire = Campfire(campfire_id=\'your-campfire-id\', project_id=\'your-project-id\')\n\n# Sends a campfire message with desired content\nyour_campfire.write(content="Hello from Python!") \n```\n\n\n## 4. Attachments\n\nWhen attaching images or other files to Basecamp posts we do this by using [Rich text](https://github.com/basecamp/bc3-api/blob/3f71ee57b278be6e71f51488c71197f600395a2b/sections/rich_text.md), which means that we will be sending HTML as content to the Basecamp object we want to interact with. \n\nSending rich text through API is not allowed on all Basecamp objects that have rich text by themselves. Best example are Campfires, when interacting with Basecamp you can upload images and files to a campfire or edit the text style, but Basecamp API does not allow this to be done programatically. Here is a [list](https://github.com/basecamp/bc3-api/blob/3f71ee57b278be6e71f51488c71197f600395a2b/sections/rich_text.md#rich-text-content-attributes) of Basecamp endpoints that can accept rich text.\n\n\nTo upload a file to Basecamp, first we need upload the file to Basecamp\'s server and get its `attachable_sgid`. You can do this by using the `Attachments` object and its `upload_file()` method:\n\n```python\nfrom basecampapi import Attachments\n\nmy_att = Attachments()\nmy_att.upload_file("folder/image.png", filename="my_image")\n```\nAfter this the file will be on Basecamp\'s server and it will have an automatically generated `attachable_sgid` Uploaded files can be accessed through `Attachments.files` dictionary:\n```python\nprint(my_att.files)\n```\nThis returns a dictionary of dictionaries which contain information about the files you uploaded:\n```python\n{\n\t"my_image": {\n\t\t\'filename\': \'my_image\',\n\t\t\'file_size\': \'155291\',\n\t\t\'content-type\': \'image/png\',\n\t\t\'sgid\': \'your-file-sgid\'\n\t\t}\n}\n```\nTo attach a file inside a Basecamp post, comment or any other object where rich text is accessible through API, we need to send an HTML string  as the content parameter of the object we are interacting with, and we need to use the `<bc-attachment>` tag for any file attachments.\n\n```python\n"<bc-attachment sgid=\'your-file-sgid\'></bc-attachment>"\n```\n\nCreating a new Message Board post on Basecamp with our uploaded image will look like this:\n```python\nfrom basecampapi import MessageBoard\n\n# Constructing the content string\ncontent = "Hello world! <br> \\ \n\t<bc-attachment sgid=\'#######\' caption=\'My image\'></bc-attachment> <br> \\\t\n\tThis is an image sent from python."\n\n# Initiating the message board object\nmessage_board = MessageBoard(project_id=123456, message_board_id=123456)\n\n# Creating a message\nmessage_board.create_message(subject="Test message", content=content)\n```\n\n## 5. Additional information\n\nCurrently available endpoints:\n- Campfire - allows reading campfire messages and writing to campfires\n- MessageBoard - allows reading, creating and updating messages, as well as reading, creating and updating comments on messages\n- Attachments - used for uploading files and attaching them to with other Basecamp objects\n\nFuture upgrades:\n- Vaults (Docs & Files)\n- To-dos\n\nRequest new features in [issues](https://github.com/mare011rs/basecampapi/issues).',
     'author': 'mare011rs',
     'author_email': 'mare011rs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `basecampapi-1.0.0/PKG-INFO` & `basecampapi-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: basecampapi
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Author: mare011rs
 Author-email: mare011rs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Basecamp API
 
 This package allows simple interaction with [Basecamp API](https://github.com/basecamp/bc3-api) using Python.
```

