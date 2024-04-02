# Comparing `tmp/chiasmodon-0.2.8.tar.gz` & `tmp/chiasmodon-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-0.2.8.tar", last modified: Sat Mar 23 21:45:17 2024, max compression
+gzip compressed data, was "chiasmodon-0.2.9.tar", last modified: Sat Mar 23 21:45:53 2024, max compression
```

## Comparing `chiasmodon-0.2.8.tar` & `chiasmodon-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-03-23 21:45:17.778672 chiasmodon-0.2.8/
--rwxrwxrwx   0 user      (1000) user      (1000)     1053 2024-03-23 04:53:05.000000 chiasmodon-0.2.8/LICENSE.txt
--rwxrwxrwx   0 user      (1000) user      (1000)     8104 2024-03-23 21:45:17.776617 chiasmodon-0.2.8/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     7329 2024-03-23 21:44:41.000000 chiasmodon-0.2.8/README.md
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-03-23 21:45:17.756803 chiasmodon-0.2.8/chiasmodon.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)     8104 2024-03-23 21:45:17.000000 chiasmodon-0.2.8/chiasmodon.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)      237 2024-03-23 21:45:17.000000 chiasmodon-0.2.8/chiasmodon.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2024-03-23 21:45:17.000000 chiasmodon-0.2.8/chiasmodon.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       16 2024-03-23 21:45:17.000000 chiasmodon-0.2.8/chiasmodon.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2024-03-23 21:45:17.000000 chiasmodon-0.2.8/chiasmodon.egg-info/top_level.txt
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-03-23 21:45:17.766806 chiasmodon-0.2.8/cli/
--rwxrwxrwx   0 user      (1000) user      (1000)    11816 2024-03-23 21:02:02.000000 chiasmodon-0.2.8/cli/chiasmodon_cli.py
--rwxrwxrwx   0 user      (1000) user      (1000)    10381 2024-03-23 21:45:13.000000 chiasmodon-0.2.8/pychiasmodon.py
--rwxrwxrwx   0 user      (1000) user      (1000)       38 2024-03-23 21:45:17.779742 chiasmodon-0.2.8/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)     1322 2024-03-23 21:44:49.000000 chiasmodon-0.2.8/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-03-23 21:45:53.976700 chiasmodon-0.2.9/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1053 2024-03-23 04:53:05.000000 chiasmodon-0.2.9/LICENSE.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)     8101 2024-03-23 21:45:53.974698 chiasmodon-0.2.9/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     7326 2024-03-23 21:45:36.000000 chiasmodon-0.2.9/README.md
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-03-23 21:45:53.956942 chiasmodon-0.2.9/chiasmodon.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     8101 2024-03-23 21:45:53.000000 chiasmodon-0.2.9/chiasmodon.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      237 2024-03-23 21:45:53.000000 chiasmodon-0.2.9/chiasmodon.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2024-03-23 21:45:53.000000 chiasmodon-0.2.9/chiasmodon.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       16 2024-03-23 21:45:53.000000 chiasmodon-0.2.9/chiasmodon.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2024-03-23 21:45:53.000000 chiasmodon-0.2.9/chiasmodon.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-03-23 21:45:53.964889 chiasmodon-0.2.9/cli/
+-rwxrwxrwx   0 user      (1000) user      (1000)    11816 2024-03-23 21:02:02.000000 chiasmodon-0.2.9/cli/chiasmodon_cli.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    10381 2024-03-23 21:45:50.000000 chiasmodon-0.2.9/pychiasmodon.py
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2024-03-23 21:45:53.976700 chiasmodon-0.2.9/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)     1322 2024-03-23 21:45:47.000000 chiasmodon-0.2.9/setup.py
```

### Comparing `chiasmodon-0.2.8/LICENSE.txt` & `chiasmodon-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-0.2.8/PKG-INFO` & `chiasmodon-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/0xchiasmodon/pychiasmodon
 Author: 0xchiasmodon
 License: UNKNOWN
 Keywords: Chiasmodon OSINT tool Open Source Intelligence Domain search Domain emails Domain credentials User Passwords CIDRs ASNs Subdomains Reconnaissance Security assessment Digital footprint Network infrastructure Attack surface Information gathering Target domain Email search Credential search Network reconnaissance
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -24,19 +24,19 @@
 - [x] **✉️Email, 👤Username, 🔒Password**: Conduct searches based on email, username, or password to identify potential security risks or compromised credentials.
 - [x] **📋Output Customization**: Choose the desired output format (text, JSON, or CSV) and specify the filename to save the search results.
 - [x] **⚙️Additional Options**: The tool offers various additional options, such as viewing different result types (credentials, URLs, subdomains, emails, passwords, usernames, or applications), setting API tokens, specifying timeouts, limiting results, and more.
 
 
 ## 🚀Comping soon
 
-- [ ] **📱Phone**: Get ready to uncover even more valuable data by searching for information associated with phone numbers. Whether you're investigating a particular individual or looking for connections between phone numbers and other entities, this new feature will provide you with valuable insights.
+- [] **📱Phone**: Get ready to uncover even more valuable data by searching for information associated with phone numbers. Whether you're investigating a particular individual or looking for connections between phone numbers and other entities, this new feature will provide you with valuable insights.
 
-- [ ] **🏢Company Name**: We understand the importance of comprehensive company research. In our upcoming release, you'll be able to search by company name and access a wide range of documents associated with that company. This feature will provide you with a convenient and efficient way to gather crucial information, such as legal documents, financial reports, and other relevant records.
+- [] **🏢Company Name**: We understand the importance of comprehensive company research. In our upcoming release, you'll be able to search by company name and access a wide range of documents associated with that company. This feature will provide you with a convenient and efficient way to gather crucial information, such as legal documents, financial reports, and other relevant records.
 
-- [ ] **👤Face (Photo)**: Visual data is a powerful tool, and we are excited to introduce our advanced facial recognition feature. With "Search by Face (Photo)," you can upload an image containing a face and leverage cutting-edge technology to identify and match individuals across various data sources. This will allow you to gather valuable information, such as social media profiles, online presence, and potential connections, all through the power of facial recognition.
+- [] **👤Face (Photo)**: Visual data is a powerful tool, and we are excited to introduce our advanced facial recognition feature. With "Search by Face (Photo)," you can upload an image containing a face and leverage cutting-edge technology to identify and match individuals across various data sources. This will allow you to gather valuable information, such as social media profiles, online presence, and potential connections, all through the power of facial recognition.
 
 ## 🔑 Subscription
 Join us today and unlock the potential of our cutting-edge OSINT tool. Contact https://t.me/Chiasmod0n on Telegram to subscribe and start harnessing the power of Chiasmodon for your domain investigations.
 
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
```

### Comparing `chiasmodon-0.2.8/README.md` & `chiasmodon-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 - [x] **✉️Email, 👤Username, 🔒Password**: Conduct searches based on email, username, or password to identify potential security risks or compromised credentials.
 - [x] **📋Output Customization**: Choose the desired output format (text, JSON, or CSV) and specify the filename to save the search results.
 - [x] **⚙️Additional Options**: The tool offers various additional options, such as viewing different result types (credentials, URLs, subdomains, emails, passwords, usernames, or applications), setting API tokens, specifying timeouts, limiting results, and more.
 
 
 ## 🚀Comping soon
 
-- [ ] **📱Phone**: Get ready to uncover even more valuable data by searching for information associated with phone numbers. Whether you're investigating a particular individual or looking for connections between phone numbers and other entities, this new feature will provide you with valuable insights.
+- [] **📱Phone**: Get ready to uncover even more valuable data by searching for information associated with phone numbers. Whether you're investigating a particular individual or looking for connections between phone numbers and other entities, this new feature will provide you with valuable insights.
 
-- [ ] **🏢Company Name**: We understand the importance of comprehensive company research. In our upcoming release, you'll be able to search by company name and access a wide range of documents associated with that company. This feature will provide you with a convenient and efficient way to gather crucial information, such as legal documents, financial reports, and other relevant records.
+- [] **🏢Company Name**: We understand the importance of comprehensive company research. In our upcoming release, you'll be able to search by company name and access a wide range of documents associated with that company. This feature will provide you with a convenient and efficient way to gather crucial information, such as legal documents, financial reports, and other relevant records.
 
-- [ ] **👤Face (Photo)**: Visual data is a powerful tool, and we are excited to introduce our advanced facial recognition feature. With "Search by Face (Photo)," you can upload an image containing a face and leverage cutting-edge technology to identify and match individuals across various data sources. This will allow you to gather valuable information, such as social media profiles, online presence, and potential connections, all through the power of facial recognition.
+- [] **👤Face (Photo)**: Visual data is a powerful tool, and we are excited to introduce our advanced facial recognition feature. With "Search by Face (Photo)," you can upload an image containing a face and leverage cutting-edge technology to identify and match individuals across various data sources. This will allow you to gather valuable information, such as social media profiles, online presence, and potential connections, all through the power of facial recognition.
 
 ## 🔑 Subscription
 Join us today and unlock the potential of our cutting-edge OSINT tool. Contact https://t.me/Chiasmod0n on Telegram to subscribe and start harnessing the power of Chiasmodon for your domain investigations.
 
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
```

### Comparing `chiasmodon-0.2.8/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-0.2.9/chiasmodon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/0xchiasmodon/pychiasmodon
 Author: 0xchiasmodon
 License: UNKNOWN
 Keywords: Chiasmodon OSINT tool Open Source Intelligence Domain search Domain emails Domain credentials User Passwords CIDRs ASNs Subdomains Reconnaissance Security assessment Digital footprint Network infrastructure Attack surface Information gathering Target domain Email search Credential search Network reconnaissance
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -24,19 +24,19 @@
 - [x] **✉️Email, 👤Username, 🔒Password**: Conduct searches based on email, username, or password to identify potential security risks or compromised credentials.
 - [x] **📋Output Customization**: Choose the desired output format (text, JSON, or CSV) and specify the filename to save the search results.
 - [x] **⚙️Additional Options**: The tool offers various additional options, such as viewing different result types (credentials, URLs, subdomains, emails, passwords, usernames, or applications), setting API tokens, specifying timeouts, limiting results, and more.
 
 
 ## 🚀Comping soon
 
-- [ ] **📱Phone**: Get ready to uncover even more valuable data by searching for information associated with phone numbers. Whether you're investigating a particular individual or looking for connections between phone numbers and other entities, this new feature will provide you with valuable insights.
+- [] **📱Phone**: Get ready to uncover even more valuable data by searching for information associated with phone numbers. Whether you're investigating a particular individual or looking for connections between phone numbers and other entities, this new feature will provide you with valuable insights.
 
-- [ ] **🏢Company Name**: We understand the importance of comprehensive company research. In our upcoming release, you'll be able to search by company name and access a wide range of documents associated with that company. This feature will provide you with a convenient and efficient way to gather crucial information, such as legal documents, financial reports, and other relevant records.
+- [] **🏢Company Name**: We understand the importance of comprehensive company research. In our upcoming release, you'll be able to search by company name and access a wide range of documents associated with that company. This feature will provide you with a convenient and efficient way to gather crucial information, such as legal documents, financial reports, and other relevant records.
 
-- [ ] **👤Face (Photo)**: Visual data is a powerful tool, and we are excited to introduce our advanced facial recognition feature. With "Search by Face (Photo)," you can upload an image containing a face and leverage cutting-edge technology to identify and match individuals across various data sources. This will allow you to gather valuable information, such as social media profiles, online presence, and potential connections, all through the power of facial recognition.
+- [] **👤Face (Photo)**: Visual data is a powerful tool, and we are excited to introduce our advanced facial recognition feature. With "Search by Face (Photo)," you can upload an image containing a face and leverage cutting-edge technology to identify and match individuals across various data sources. This will allow you to gather valuable information, such as social media profiles, online presence, and potential connections, all through the power of facial recognition.
 
 ## 🔑 Subscription
 Join us today and unlock the potential of our cutting-edge OSINT tool. Contact https://t.me/Chiasmod0n on Telegram to subscribe and start harnessing the power of Chiasmodon for your domain investigations.
 
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
```

### Comparing `chiasmodon-0.2.8/cli/chiasmodon_cli.py` & `chiasmodon-0.2.9/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-0.2.8/pychiasmodon.py` & `chiasmodon-0.2.9/pychiasmodon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import sys
 import time
 import requests
 from yaspin import Spinner
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 class Chiasmodon:
     API_URL         = 'https://chiasmodon.club/v2/api/beta'
     API_HEADERS     = {'user-agent':'cli/python'}
     VIEW_TYPE = {
         'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password'],
         'url':['domain', 'email', 'cidr', 'asn', 'username','password'],
```

### Comparing `chiasmodon-0.2.8/setup.py` & `chiasmodon-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='0.2.8',
+      version='0.2.9',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='0xchiasmodon',
       keywords='Chiasmodon OSINT tool Open Source Intelligence Domain search Domain emails Domain credentials User Passwords CIDRs ASNs Subdomains Reconnaissance Security assessment Digital footprint Network infrastructure Attack surface Information gathering Target domain Email search Credential search Network reconnaissance',
       url='https://github.com/0xchiasmodon/pychiasmodon',
       packages=['.'],
```

