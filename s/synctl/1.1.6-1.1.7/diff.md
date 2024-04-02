# Comparing `tmp/synctl-1.1.6.tar.gz` & `tmp/synctl-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synctl-1.1.6.tar", last modified: Fri Mar  1 09:18:03 2024, max compression
+gzip compressed data, was "synctl-1.1.7.tar", last modified: Tue Apr  2 06:42:22 2024, max compression
```

## Comparing `synctl-1.1.6.tar` & `synctl-1.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-03-01 09:18:03.890363 synctl-1.1.6/
--rw-r--r--   0 swethalohith   (501) staff       (20)     1064 2023-11-24 04:36:16.000000 synctl-1.1.6/LICENSE
--rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-03-01 09:18:03.890195 synctl-1.1.6/PKG-INFO
--rw-r--r--   0 swethalohith   (501) staff       (20)    34201 2024-03-01 08:01:15.000000 synctl-1.1.6/README.md
--rw-r--r--   0 swethalohith   (501) staff       (20)       81 2023-11-29 08:33:08.000000 synctl-1.1.6/pyproject.toml
--rw-r--r--   0 swethalohith   (501) staff       (20)       38 2024-03-01 09:18:03.890420 synctl-1.1.6/setup.cfg
--rw-r--r--   0 swethalohith   (501) staff       (20)     2143 2023-11-29 08:33:08.000000 synctl-1.1.6/setup.py
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-03-01 09:18:03.887441 synctl-1.1.6/synctl/
--rw-r--r--   0 swethalohith   (501) staff       (20)        0 2023-11-29 08:33:08.000000 synctl-1.1.6/synctl/__init__.py
--rw-r--r--   0 swethalohith   (501) staff       (20)       22 2024-03-01 08:01:32.000000 synctl-1.1.6/synctl/__version__.py
--rwxr-xr-x   0 swethalohith   (501) staff       (20)   201274 2024-03-01 08:01:15.000000 synctl-1.1.6/synctl/cli.py
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-03-01 09:18:03.889470 synctl-1.1.6/synctl.egg-info/
--rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-03-01 09:18:03.000000 synctl-1.1.6/synctl.egg-info/PKG-INFO
--rw-r--r--   0 swethalohith   (501) staff       (20)      328 2024-03-01 09:18:03.000000 synctl-1.1.6/synctl.egg-info/SOURCES.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        1 2024-03-01 09:18:03.000000 synctl-1.1.6/synctl.egg-info/dependency_links.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)       43 2024-03-01 09:18:03.000000 synctl-1.1.6/synctl.egg-info/entry_points.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        1 2023-11-24 05:57:32.000000 synctl-1.1.6/synctl.egg-info/not-zip-safe
--rw-r--r--   0 swethalohith   (501) staff       (20)       17 2024-03-01 09:18:03.000000 synctl-1.1.6/synctl.egg-info/requires.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        7 2024-03-01 09:18:03.000000 synctl-1.1.6/synctl.egg-info/top_level.txt
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-03-01 09:18:03.889651 synctl-1.1.6/tests/
--rw-r--r--   0 swethalohith   (501) staff       (20)    21585 2023-12-18 04:49:58.000000 synctl-1.1.6/tests/test_synctl.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.182553 synctl-1.1.7/
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1064 2023-11-24 04:36:16.000000 synctl-1.1.7/LICENSE
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-02 06:42:22.182362 synctl-1.1.7/PKG-INFO
+-rw-r--r--   0 swethalohith   (501) staff       (20)    34889 2024-04-02 06:39:53.000000 synctl-1.1.7/README.md
+-rw-r--r--   0 swethalohith   (501) staff       (20)       81 2023-11-29 08:33:08.000000 synctl-1.1.7/pyproject.toml
+-rw-r--r--   0 swethalohith   (501) staff       (20)       38 2024-04-02 06:42:22.182617 synctl-1.1.7/setup.cfg
+-rw-r--r--   0 swethalohith   (501) staff       (20)     2143 2023-11-29 08:33:08.000000 synctl-1.1.7/setup.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.178110 synctl-1.1.7/synctl/
+-rw-r--r--   0 swethalohith   (501) staff       (20)        0 2023-11-29 08:33:08.000000 synctl-1.1.7/synctl/__init__.py
+-rw-r--r--   0 swethalohith   (501) staff       (20)       22 2024-04-02 06:39:53.000000 synctl-1.1.7/synctl/__version__.py
+-rwxr-xr-x   0 swethalohith   (501) staff       (20)   219906 2024-04-02 06:39:53.000000 synctl-1.1.7/synctl/cli.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.181460 synctl-1.1.7/synctl.egg-info/
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/PKG-INFO
+-rw-r--r--   0 swethalohith   (501) staff       (20)      328 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/SOURCES.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        1 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/dependency_links.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)       43 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/entry_points.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        1 2023-11-24 05:57:32.000000 synctl-1.1.7/synctl.egg-info/not-zip-safe
+-rw-r--r--   0 swethalohith   (501) staff       (20)       17 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/requires.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        7 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/top_level.txt
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.181679 synctl-1.1.7/tests/
+-rw-r--r--   0 swethalohith   (501) staff       (20)    21585 2023-12-18 04:49:58.000000 synctl-1.1.7/tests/test_synctl.py
```

### Comparing `synctl-1.1.6/LICENSE` & `synctl-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `synctl-1.1.6/PKG-INFO` & `synctl-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctl
-Version: 1.1.6
+Version: 1.1.7
 Summary: Instana Synthetic CLI
 Home-page: https://github.com/instana/synthetic-synctl
 Author: Rong Zhu Shang, Swetha Lohith
 Author-email: shangrz@cn.ibm.com, Swetha.Lohith@ibm.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/instana/synthetic-synctl/issues
 Project-URL: Source, https://github.com/instana/synthetic-synctl
```

### Comparing `synctl-1.1.6/README.md` & `synctl-1.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -806,24 +806,41 @@
 -h, --help             show this help message and exit
 --show-details         output alert details to terminal
 --show-json            output alert json to terminal
 --use-env, -e <name>   use a specified config
 --host <host>          set hostname
 --token <token>        set token
 ```
-### synctl get alert Examples
+# Query Test Results
+`synctl get result` can be used to query Test Results
+
+### synctl get result Syntax
+```
+synctl get result [id] [options]
+```
+### synctl get result Options
 ```
-# Display all alert
-synctl get alert
+-h, --help               show this help message and exit
+--test                   synthetic-test id
+--window-size <window>   set synthetic result window size, support [1,60]m, [1-24]h
+--har                    save HAR to local
+--use-env, -e <name>     use a specified config
+--host <host>            set hostname
+--token <token>          set token
+```
+### synctl get result Examples
+```
+# Display result list  with --window-size, support [1, 60]m, [1-24]h
+synctl get result --test <test-id> --window-size 30m
+
+# show result details with --window-size, support [1, 60]m, [1-24]h
+synctl get result <id> --test <test-id> --window-size 6h
 
-# show alert details
-synctl get alert <id> --show-details
- 
-# show alert payload in json
-synctl get alert <id> --show-json
+# save har to local 
+synctl get result <id> --test <test-id> --har
 ```
 # Create Smart alert
 `synctl create alert` is used to create Smart Alerts.
 
 ### synctl create alert Syntax
 ```
 synctl create alert [options]
```

### Comparing `synctl-1.1.6/setup.py` & `synctl-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `synctl-1.1.6/synctl/cli.py` & `synctl-1.1.7/synctl/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 # from getpass import getpass
 import json
 from pathlib import Path
 import os
 import re
 import signal
 import sys
+
+import tarfile
 import getpass
 # import textwrap
 import time
+from datetime import datetime
 
 import requests
 import urllib3
 
 from synctl.__version__ import __version__
 
 VERSION = __version__
@@ -50,14 +53,15 @@
 SYN_TEST = "test"
 SYN_LOCATION = "location"
 SYN_LO = "lo"  # short for location
 SYN_APPLICATION = "application"
 SYN_APP = "app"  # short for application
 SYN_CRED = "cred"  # short for credentials
 SYN_ALERT = "alert"  # short for smart alerts
+SYN_RESULT = "result"
 
 POSITION_PARAMS = "commands"
 OPTIONS_PARAMS = "options"
 
 NOT_APPLICABLE = "N/A"
 
 NORMAL_CODE, ERROR_CODE = (0, 1)
@@ -112,14 +116,23 @@
 
 def identify_hyphen():
     sys.argv = [
         " " + a if a.startswith('-') and not a.startswith('--') and len(a) > 2 and sys.argv[2] == 'alert' else a
         for a in sys.argv
     ]
 
+def validate_args(args):
+    seen = set()
+    for item in args:
+        if item in seen:
+            print(f"{item} should not be provided multiple times")
+            sys.exit()
+        else:
+            seen.add(item)
+
 COMMAND_CONFIG = 'config'
 COMMAND_CREATE = 'create'
 COMMAND_GET = 'get'
 COMMAND_DELETE = 'delete'
 COMMAND_PATCH = 'patch'
 COMMAND_UPDATE = 'update'
 
@@ -1660,14 +1673,313 @@
             else:
                 self.exit_synctl(ERROR_CODE, f'get test failed, status code: {query_result.status_code}')
         except requests.ConnectTimeout as timeout_error:
             self.exit_synctl(f"Connection to {host} timed out, error is {timeout_error}")
         except requests.ConnectionError as connect_error:
             self.exit_synctl(f"Connection to {host} failed, error is {connect_error}")
 
+    def retrieve_test_results(self, test_id, page=1, page_size=200, window_size=60*60*1000):
+        self.check_host_and_token(self.auth["host"], self.auth["token"])
+        host = self.auth["host"]
+        token = self.auth["token"]
+        if id is None or test_id == "":
+            print("test id should not be empty")
+            return
+        else:
+            retrieve_url = f"{host}/api/synthetics/results/list"
+
+        headers = {
+            'Content-Type': 'application/json',
+            "Authorization": f"apiToken {token}"
+        }
+        summary_config = {"syntheticMetrics":["synthetic.metricsResponseTime","synthetic.metricsResponseSize", "status","synthetic.errors"],
+                          "metrics": [{
+                            "aggregation": "SUM",
+                            "granularity": 600,
+                            "metric": "synthetic.metricsStatus"
+                        }],
+                          "order":{
+                              "by":"synthetic.metricsResponseTime",
+                              "direction":"DESC"
+                          },
+                          "tagFilters":[{
+                              "stringValue": test_id,
+                              "name":"synthetic.testId",
+                              "operator":"EQUALS"
+                          }],
+                          "pagination": {
+                              "page": page,
+                              "pageSize": page_size
+                          },
+                          "timeFrame": {
+                              "to": 0,
+                              "windowSize": window_size
+                          }}
+        try:
+            result = requests.post(retrieve_url,
+                                  headers=headers,
+                                  data=json.dumps(summary_config),
+                                  timeout=60,
+                                  verify=self.insecure)
+            if _status_is_200(result.status_code):
+                data = result.json()
+                return data
+            else:
+                self.exit_synctl(ERROR_CODE,
+                                 f'retrieve test result list failed, status code:: {result.status_code}')
+                return None
+        except requests.ConnectTimeout as timeout_error:
+            self.exit_synctl(f"Connection to {host} timed out, error is {timeout_error}")
+        except requests.ConnectionError as connect_error:
+            self.exit_synctl(f"Connection to {host} failed, error is {connect_error}")
+
+    def __sort_test_result(self, result_list):
+        """sort Synthetic result list by Starttime"""
+        new_list = sorted(
+            result_list, reverse=True, key=lambda result: result["metrics"]["response_time"][0][0] if result is not None else [])
+        return new_list
+
+    def retrieve_test_result_details(self, resultid, testid, HAR):
+        self.check_host_and_token(self.auth["host"], self.auth["token"])
+        host = self.auth["host"]
+        token = self.auth["token"]
+        test = self.retrieve_a_synthetic_test(testid)
+        result = {}
+        result["testid"] = testid
+        result["resultid"] = resultid
+        result["syntheticType"] = test[0]["configuration"]["syntheticType"]
+
+        headers = {
+            'Content-Type': 'application/json',
+            "Authorization": f"apiToken {token}"
+        }
+        try:
+            if id is None or testid == "":
+                print("test id should not be empty")
+                return
+            else:
+                if test[0]["configuration"]["syntheticType"] in [HTTPAction_TYPE, HTTPScript_TYPE]:
+                    retrieve_url_sub = f"{host}/api/synthetics/results/{testid}/{resultid}/detail?type=SUBTRANSACTIONS"
+                    retrieve_url_logs = f"{host}/api/synthetics/results/{testid}/{resultid}/detail?type=LOGS"
+                    result_sub = requests.get(retrieve_url_sub,
+                                              headers=headers,
+                                              timeout=60,
+                                              verify=self.insecure)
+                    result_logs = requests.get(retrieve_url_logs,
+                                               headers=headers,
+                                               timeout=60,
+                                               verify=self.insecure)
+                    if _status_is_200(result_sub.status_code):
+                        result["sub"] = result_sub.json()["subtransactions"]
+                    elif result_sub.status_code != 404:
+                       print(f'get subtransactions for result {resultid} failed, status code: {result_sub.status_code}')
+                    if _status_is_200(result_logs.status_code):
+                        result["logs"] = result_logs.json()["logs"]
+                    elif result_logs.status_code != 404:
+                        print(f'get logs for result {resultid} failed, status code: {result_logs.status_code}')
+
+                elif test[0]["configuration"]["syntheticType"] in  [BrowserScript_TYPE, WebpageScript_TYPE, WebpageAction_TYPE]:
+                    if HAR:
+                        retrieve_url_har = f"{host}/api/synthetics/results/{testid}/{resultid}/detail?type=HAR"
+                        result_har = requests.get(retrieve_url_har,
+                                                  headers=headers,
+                                                  timeout=60,
+                                                  verify=self.insecure)
+                        if _status_is_200(result_har.status_code):
+                            result["har"] = result_har.json()['har']
+                        elif result_har.status_code != 404:
+                            print(f'get har for result {resultid} failed, status code: {result_har.status_code}')
+                    retrieve_url_image = f"{host}/api/synthetics/results/{testid}/{resultid}/file?type=IMAGES"
+                    retrieve_url_videos = f"{host}/api/synthetics/results/{testid}/{resultid}/file?type=VIDEOS"
+                    retrieve_url_logs = f"{host}/api/synthetics/results/{testid}/{resultid}/detail?type=LOGS"
+                    result_logs = requests.get(retrieve_url_logs,
+                                               headers=headers,
+                                               timeout=60,
+                                               verify=self.insecure)
+                    result_image = requests.get(retrieve_url_image,
+                                                headers=headers,
+                                                timeout=60,
+                                                verify=self.insecure)
+                    result_videos = requests.get(retrieve_url_videos,
+                                                 headers=headers,
+                                                 timeout=60,
+                                                 verify=self.insecure)
+                    if _status_is_200(result_logs.status_code):
+                        result["logs"] = result_logs.json()["logFiles"]
+                    elif result_logs.status_code != 404:
+                        print(f"get logs for result {resultid} failed, status code: {result_logs.status_code}")
+                    if _status_is_200(result_image.status_code):
+                        result["image"] = result_image.content
+                    elif result_image.status_code != 404:
+                        print(f'get image for result {resultid} failed, status code: {result_image.status_code}')
+                    if _status_is_200(result_videos.status_code):
+                        result["video"] = result_videos.content
+                    elif result_videos.status_code != 404:
+                        print(f'get videos for result {resultid} failed, status code: {result_videos.status_code}')
+            return result
+        except requests.ConnectTimeout as timeout_error:
+            self.exit_synctl(f"Connection to {host} timed out, error is {timeout_error}")
+        except requests.ConnectionError as connect_error:
+            self.exit_synctl(f"Connection to {host} failed, error is {connect_error}")
+
+    def get_all_test_results(self, test_id, window_size):
+        total_hits = 0
+        result_instance = SyntheticResult()
+        window_size_ms = result_instance.get_window_size(window_size)
+        result_list = self.retrieve_test_results(test_id,window_size=window_size_ms)
+        if result_list is not None:
+            page = result_list["page"] if "page" in result_list else 1
+            page_size = result_list["pageSize"] if "pageSize" in result_list else 200
+            if "totalHits" in result_list:
+                total_hits = result_list["totalHits"]
+
+            if page_size >= total_hits:
+                return result_list
+            else:
+                total_pages = total_hits/page_size
+                if (total_pages - round(total_pages)) > 0:
+                    total_pages += 1
+                for x in range(0, round(total_pages)):
+                    result_list = self.retrieve_test_results(test_id=test_id,
+                                                             page=x+1,
+                                                             page_size=200,
+                                                             window_size=window_size_ms)
+                    return result_list
+        else:
+            return None
+
+    def convert_milliseconds(self, time_ms):
+        if time_ms > 60000:
+            time = f"{time_ms / 60000:.2f}min"
+        elif time_ms > 1000:
+            time = f"{time_ms / 1000:.2f}s"
+        else:
+            time = f"{time_ms}ms"
+        return time
+
+    def change_time_format(self, time):
+        """format time to YYYY-MM-DD, HH:MM:SS"""
+        date_time = datetime.fromtimestamp(time/1000)
+        formatted_date_time = date_time.strftime("%Y-%m-%d, %H:%M:%S")
+
+        return formatted_date_time
+
+    def print_result_details(self, result_details, result_list):
+        for result in result_list:
+            formatted_response_size = "{:.2f} MiB".format(result["metrics"]["response_size"][0][1]/ (1024 * 1024))
+            status = "Successful" if result["metrics"]["status"][0][1] == 1 else "Failed"
+
+            if result["testResultCommonProperties"]["id"] == result_details["resultid"]:
+                print(self.fill_space("Name".upper(), 30), "Value".upper())
+                print(self.fill_space("Result Id", 30), result_details["resultid"])
+                print(self.fill_space("Start Time", 30), self.change_time_format(result["metrics"]["response_time"][0][0]))
+                print(self.fill_space("Status", 30), status)
+                print(self.fill_space("Response Time", 30), str(self.convert_milliseconds(result["metrics"]["response_time"][0][1])))
+                print(self.fill_space("Response Size", 30), str(formatted_response_size))
+                if "har" in result_details:
+                    har_path = os.path.join(result_details["testid"], result_details["resultid"])
+                    os.makedirs(har_path, exist_ok=True)
+                    file_path = os.path.join(har_path, "HAR.json")
+                    with open(file_path, 'w') as f:
+                        json.dump(result_details['har'], f)
+                    print(self.fill_space("HAR", 30), f"HAR has been saved to {file_path}")
+                else:
+                    print(self.fill_space("HAR", 30), "N/A")
+                if "image" in result_details:
+                    with open("images.tar", "wb") as f:
+                        f.write(result_details["image"])
+                    with tarfile.open("images.tar", "r") as tar:
+                        images_path = os.path.join(result_details["testid"], result_details["resultid"], "Screenshots")
+                        tar.extractall(path=images_path)
+                    print(self.fill_space("Screenshots", 30), f"Screenshots has been saved to {images_path}")
+                else:
+                    print(self.fill_space("Screenshots", 30), "N/A")
+                if "video" in result_details:
+                    with open("videos.tar", "wb") as f:
+                        f.write(result_details["video"])
+                    with tarfile.open("videos.tar", "r") as tar:
+                        videos_path = os.path.join(result_details["testid"], result_details["resultid"], "Recordings")
+                        tar.extractall(path=videos_path)
+                    print(self.fill_space("Recordings", 30), f"Recordings has been saved to {videos_path}")
+                else:
+                    print(self.fill_space("Recordings", 30), "N/A")
+                if "sub" in result_details:
+                    print("")
+                    print(self.__fix_length("*", 80))
+                    print("Subtransactions ")
+                    print(self.__fix_length("*", 80))
+                    for x in range(len(result_details["sub"])):
+                        for key, value in result_details["sub"][x]["properties"].items():
+                            if key == 'finishTime' or key == 'startTime':
+                                print(self.fill_space(key, 30), self.format_time(value))
+                            else:
+                                print(self.fill_space(key, 30), value)
+                        for key, value in result_details['sub'][x]["metrics"].items():
+                            print(self.fill_space(key, 30), value)
+                        print(self.__fix_length("*", 80))
+                else:
+                    print(self.fill_space("Subtransactions", 30), "N/A")
+                if "logs" in result_details:
+                    print("")
+                    print("\nConsole logs ")
+                    print(self.__fix_length("*", 80))
+                    if "console.log" in result_details["logs"]:
+                        print(result_details["logs"]["console.log"])
+                    else:
+                        print(result_details["logs"])
+                    print(self.__fix_length("*", 80))
+                    if result_details["syntheticType"] != HTTPScript_TYPE:
+                        if "browser.json" in result_details["logs"]:
+                            print("Browser logs")
+                            print(self.__fix_length("*", 80))
+                            browserlogs = json.loads(result_details["logs"]["browser.json"])
+                            for logs in browserlogs:
+                                print(logs["level"]+ "\n" + self.change_time_format(logs["timestamp"]) + "\n" +  logs["message"])
+                            print("")
+                            print(self.__fix_length("*", 80))
+                        else:
+                            print(self.fill_space("Browser Logs", 30), "N/A")
+                if "errors" in result["testResultCommonProperties"]:
+                    print("Error")
+                    print(self.__fix_length("*", 80))
+                    errors = result["testResultCommonProperties"]["errors"][0].split(",")
+                    for e in errors:
+                        print(e)
+                else:
+                    print(self.fill_space("Error", 30), "N/A")
+                break
+        else:
+            print(f"no result \"{result_details['resultid']}\" found, ensure the window-size is correct.")
+
+    def print_result_list(self, result_list):
+        id_length = 38
+        start_time_length = 30
+        loc_length = 30
+        status_length = 15
+        response_size_length = 8
+        response_time_length = 18
+        sorted_result = self.__sort_test_result(result_list)
+
+        print(self.fill_space("ID".upper(), id_length),
+              self.fill_space("start Time".upper(), start_time_length),
+              self.fill_space("Location".upper(), loc_length),
+              self.fill_space("Status".upper(), status_length),
+              self.fill_space("Response Time".upper(), response_time_length),
+              self.fill_space("Response size".upper(), response_size_length))
+        for result in sorted_result:
+            formatted_response_size = "{:.2f} MiB".format(result["metrics"]["response_size"][0][1]/ (1024 * 1024))
+            status = "Successful" if result["metrics"]["status"][0][1] == 1 else "Failed"
+
+            print(self.fill_space(result["testResultCommonProperties"]["id"], id_length ),
+                  self.fill_space(str(self.change_time_format(result["metrics"]["response_time"][0][0])), start_time_length),
+                  self.fill_space(result["testResultCommonProperties"]["locationDisplayLabel"], loc_length),
+                  self.fill_space(status, status_length),
+                  self.fill_space(str(self.convert_milliseconds(result["metrics"]["response_time"][0][1])), response_time_length),
+                  self.fill_space(str(formatted_response_size), response_size_length))
+
     def retrieve_synthetic_test_by_filter(self, tag_filter, page=1, page_size=200, window_size=60*60*1000):
         host = self.auth["host"]
         token = self.auth["token"]
         self.check_host_and_token(host, token)
 
         if isinstance(tag_filter[0], str) and tag_filter[0].lower() == "locationid":
             summary_config = {
@@ -3702,14 +4014,17 @@
         self.parser_create.add_argument(
             '--name', type=str, metavar="<string>", help='friendly name for smart alert')
 
         self.parser_create.add_argument(
             '--test', type=str, nargs='+', metavar="<id>", help="test id, support multiple test id")
 
         self.parser_create.add_argument(
+            '--window-size', type=str, default="1h", metavar="<window>", help="set Synthetic result window size, support [1,60]m, [1-24]h")
+
+        self.parser_create.add_argument(
             '--alert-channel', type=str, nargs='+', metavar="<id>", help="alert channel id, support multiple alert channel id")
 
         self.parser_create.add_argument(
             '--severity', type=str, metavar="<string>", choices=["warning", "critical"], help="severity of alert")
 
         self.parser_create.add_argument(
             '--violation-count', type=int, metavar="<int>", help="the range is from 1 to 12 failures")
@@ -3724,15 +4039,15 @@
             '--host', type=str, metavar="<host>", help='set hostname')
         self.parser_create.add_argument(
             '--token', type=str, metavar="<token>", help='set token')
 
 
     def get_command_options(self):
         self.parser_get.add_argument(
-            'op_type', choices=['location', 'lo', 'test', 'application', 'app', 'cred', 'alert', 'alert-channel'],
+            'op_type', choices=['location', 'lo', 'test', 'application', 'app', 'cred', 'alert', 'alert-channel', 'result'],
             help="command list")
         # parser_get.add_argument('type_id', type=str,
         #                         required=False, help='test id or location id')
         self.parser_get.add_argument(
             '--type', '-t', type=int, choices=[0, 1, 2, 3, 4], metavar='<int>', help='Synthetic type, 0 HTTPAction, 1 HTTPScript, 2 BrowserScript, 3 WebpageScript, 4 WebpageAction')
         self.parser_get.add_argument(
             'id', type=str, nargs="?", help='Synthetic test id')
@@ -3750,14 +4065,20 @@
         self.parser_get.add_argument(
             "--show-json", action='store_true', help="output test json to terminal")
         self.parser_get.add_argument(
             '--show-result', action='store_true', help="show latency and success rate")
         self.parser_get.add_argument(
             '--filter', nargs='?', default=None, help='filter by location')
 
+        # result list
+        self.parser_get.add_argument(
+            '--test', type=str, nargs='?', metavar="id", help="test id")
+        self.parser_get.add_argument(
+            '--har', action="store_true", help="show har")
+
         # application
         application_group = self.parser_get.add_argument_group()
         application_group.add_argument(
             '--name-filter', type=str, metavar="<app>", help="filter application by name, only applicable for application name")
         # application_group
 
         host_token_group = self.parser_get.add_argument_group()
@@ -3965,14 +4286,15 @@
 
     para_instanace = ParseParameter()
     para_instanace.set_options()
     get_args = para_instanace.get_parser().parse_args()
     update_args = get_args.__dict__.items()
 
     sys_args = sys.argv
+    validate_args(sys_args)
 
     if len(sys_args) <= 1:
         general_helper()
         sys.exit(0)
 
     # show synctl version
     if '-v' in sys_args or '--version' in sys_args:
@@ -4165,14 +4487,31 @@
         elif get_args.op_type == "alert-channel":
             if get_args.id is None:
                 alerting_channel = alert_instance.retrieve_all_alerting_channel()
                 alert_instance.print_alerting_channels(alerting_channel)
             else:
                 single_alert = alert_instance.retrieve_a_single_alerting_channel(get_args.id)
                 alert_instance.print_alerting_channels([single_alert])
+        # show test results
+        elif get_args.op_type == SYN_RESULT:
+            if get_args.test is not None:
+                if get_args.window_size is None:
+                    test_result = syn_instance.get_all_test_results(get_args.test)
+                else:
+                    test_result = syn_instance.get_all_test_results(get_args.test, get_args.window_size)
+                if get_args.id is None:
+                    syn_instance.print_result_list(test_result["items"])
+                else:
+                    if get_args.har is None:
+                        a_result_details = syn_instance.retrieve_test_result_details(get_args.id, get_args.test)
+                    else:
+                        a_result_details = syn_instance.retrieve_test_result_details(get_args.id, get_args.test, get_args.har)
+                    syn_instance.print_result_details(a_result_details, test_result["items"])
+            else:
+                print('testid is required')
     elif COMMAND_CREATE == get_args.sub_command:
         if get_args.syn_type == SYN_CRED:
             cred_payload = CredentialConfiguration()
             if get_args.key is not None:
                 cred_payload.set_credential_name(get_args.key)
             if get_args.value is not None:
                 cred_payload.set_credential_value(get_args.value)
```

### Comparing `synctl-1.1.6/synctl.egg-info/PKG-INFO` & `synctl-1.1.7/synctl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctl
-Version: 1.1.6
+Version: 1.1.7
 Summary: Instana Synthetic CLI
 Home-page: https://github.com/instana/synthetic-synctl
 Author: Rong Zhu Shang, Swetha Lohith
 Author-email: shangrz@cn.ibm.com, Swetha.Lohith@ibm.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/instana/synthetic-synctl/issues
 Project-URL: Source, https://github.com/instana/synthetic-synctl
```

### Comparing `synctl-1.1.6/tests/test_synctl.py` & `synctl-1.1.7/tests/test_synctl.py`

 * *Files identical despite different names*

