# Comparing `tmp/freegenius-0.0.8.tar.gz` & `tmp/freegenius-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.8.tar", last modified: Tue Feb 27 11:48:19 2024, max compression
+gzip compressed data, was "freegenius-0.0.9.tar", last modified: Wed Feb 28 14:42:27 2024, max compression
```

## Comparing `freegenius-0.0.8.tar` & `freegenius-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-27 11:48:19.114117 freegenius-0.0.8/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-02-27 11:48:19.114117 freegenius-0.0.8/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-27 11:48:19.114117 freegenius-0.0.8/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      921 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-02-26 10:57:44.000000 freegenius-0.0.8/freegenius/config.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-27 11:48:19.114117 freegenius-0.0.8/freegenius/configs/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10480 2024-02-27 11:46:27.000000 freegenius-0.0.8/freegenius/configs/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3824 2024-02-24 17:48:40.000000 freegenius-0.0.8/freegenius/configs/config_tools.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-27 11:48:19.114117 freegenius-0.0.8/freegenius/core/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   121935 2024-02-27 11:47:12.000000 freegenius-0.0.8/freegenius/core/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    12129 2024-02-26 17:51:52.000000 freegenius-0.0.8/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       16 2024-02-26 10:37:43.000000 freegenius-0.0.8/freegenius/requirements.txt
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-27 11:48:19.114117 freegenius-0.0.8/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17965 2024-02-26 12:14:54.000000 freegenius-0.0.8/freegenius/utils/shortcuts.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-27 11:48:19.114117 freegenius-0.0.8/freegenius.egg-info/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      436 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       53 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       17 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-02-27 11:48:19.000000 freegenius-0.0.8/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-02-27 11:48:19.114117 freegenius-0.0.8/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3147 2024-02-27 11:48:09.000000 freegenius-0.0.8/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-28 14:42:27.925755 freegenius-0.0.9/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2185 2024-02-28 14:42:27.925755 freegenius-0.0.9/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-28 14:42:27.925755 freegenius-0.0.9/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      952 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-02-26 10:57:44.000000 freegenius-0.0.9/freegenius/config.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-28 14:42:27.925755 freegenius-0.0.9/freegenius/configs/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10480 2024-02-27 11:46:27.000000 freegenius-0.0.9/freegenius/configs/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3824 2024-02-24 17:48:40.000000 freegenius-0.0.9/freegenius/configs/config_tools.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-28 14:42:27.925755 freegenius-0.0.9/freegenius/core/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   123019 2024-02-28 14:07:47.000000 freegenius-0.0.9/freegenius/core/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    12129 2024-02-26 17:51:52.000000 freegenius-0.0.9/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       16 2024-02-26 10:37:43.000000 freegenius-0.0.9/freegenius/requirements.txt
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-28 14:42:27.925755 freegenius-0.0.9/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17965 2024-02-26 12:14:54.000000 freegenius-0.0.9/freegenius/utils/shortcuts.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-02-28 14:42:27.925755 freegenius-0.0.9/freegenius.egg-info/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2185 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      436 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       53 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       17 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-02-28 14:42:27.000000 freegenius-0.0.9/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-02-28 14:42:27.925755 freegenius-0.0.9/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3147 2024-02-28 14:42:22.000000 freegenius-0.0.9/setup.py
```

### Comparing `freegenius-0.0.8/PKG-INFO` & `freegenius-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.8
+Version: 0.0.9
 Summary: FreeGenius AI, a FREE, LOCAL, OFFLINE & HIGHLY CUSTOMIZABLE AI suite that supports numerous open-source LLMs, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/freegenius
 Project-URL: Tracker, https://github.com/eliranwong/freegenius/issues
@@ -32,9 +32,12 @@
 
 # Progress
 
 ... in progress ...
 
 * preparing core features: action screening & calling
 
+* testing multi-step actions
+
 not in production yet
 
+
```

### Comparing `freegenius-0.0.8/freegenius/README.md` & `freegenius-0.0.9/freegenius/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,8 +7,10 @@
 
 # Progress
 
 ... in progress ...
 
 * preparing core features: action screening & calling
 
-not in production yet
+* testing multi-step actions
+
+not in production yet
```

### Comparing `freegenius-0.0.8/freegenius/configs/config_essential.py` & `freegenius-0.0.9/freegenius/configs/config_essential.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.8/freegenius/configs/config_tools.py` & `freegenius-0.0.9/freegenius/configs/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.8/freegenius/core/assistant.py` & `freegenius-0.0.9/freegenius/core/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -2053,15 +2053,15 @@
                             self.print("Unable to load internet resources.")
                             SharedUtil.showErrors()
 
                     # openai
                     #completion = self.runCompletion(config.currentMessages, noFunctionCall)
                     # ollama
                     # check for intended actions
-                    action = self.screenActions(fineTunedUserInput)
+                    action = self.getResponseDict(prompt=fineTunedUserInput, system=self.actionScreeningPrompt)["action"]
                     if not action:
                         continue
                     
                     # take action
                     if action in ("python_qa", "other_request") and not action in config.freeGeniusActionMethods:
                         # update message chain
                         config.currentMessages.append({"role": "user", "content": fineTunedUserInput})
@@ -2093,33 +2093,35 @@
                         streamingWordWrapper.keyToStopStreaming(streaming_event)
 
                         # when streaming is done or when user press "ctrl+q"
                         self.streaming_thread.join()
                     else:
                         # action in config.freeGeniusActionMethods
                         if config.developer:
-                            self.print3(f"calling action: {action}")
+                            self.print3(f"Calling action: {action}")
                         parameters = self.extractActionParameters(config.currentMessages, fineTunedUserInput, action)
                         if config.developer:
                             self.print2("Action Parameters:")
                             pprint.pprint(parameters)
                         if parameters:
-                            #response = config.freeGeniusActionMethods[action](parameters)
+                            self.print3(f"Running action: {action}")
+                            # block response for now for testing
                             response = ""
+                            # response = config.freeGeniusActionMethods[action](parameters)
                             if response:
                                 if response == "[INVALID]":
                                     # generate chat content
                                     ...
                                 else:
                                     # update message chain
                                     # further conversation
                                     ...
                             elif config.developer:
                                 # a simple notification without further chat generation
-                                self.print2("Action completed!")
+                                self.print3("Action completed!")
                         else:
                             # generate chat content
                             ...
 
                 # error codes: https://platform.openai.com/docs/guides/error-codes/python-library-error-types
                 except openai.APIError as e:
                     self.stopSpinning()
@@ -2185,46 +2187,51 @@
 {actions}
 
 {examples}
 
 Choose an action and respond with JSON string that contains one single key, "action".
 """
 
-    def screenActions(self, userInput) -> str:
+    def getResponseDict(self, *args, **kwargs) -> dict:
+        """
+        Get structured response in a dictionary
+        """
         completion = ollama.generate(
             model=config.ollamaDefaultModel,
-            prompt=userInput,
-            system=self.actionScreeningPrompt,
             format="json",
             stream=False,
             options=Options(
                 temperature=config.llmTemperature,
             ),
+            *args,
+            **kwargs,
         )
-        # action
-        return json.loads(completion["response"])["action"]
+        return json.loads(completion["response"])
 
     def extractActionParameters(self, ongoingMessages, userInput, action) -> dict:
+        """
+        Extract action parameters
+        """
         def getKeyDescriptions(parameters) -> str:
             descriptions = [f"""* "{parameter}" - {parameters[parameter]["description"]}""" for parameter in parameters]
             return "\n".join(descriptions)
 
         parameters = config.freeGeniusActionParameters[action]
         # create a template
         template = {parameter: "" if parameters[parameter]["type"] == "string" else [] for parameter in parameters} # support string and list/array first, more later
         # prompt
         prompt = f"""Use this template:
 
 {template}
 
-Based on my request, generate a JSON string that contains {len(parameters)} keys: "{'", "'.join(parameters.keys())}"
+Based on my request / query, generate a JSON string that contains {len(parameters)} keys: "{'", "'.join(parameters.keys())}"
 Key descriptions:
 {getKeyDescriptions(parameters)}
 
-Here is my request:
+Here is my request / query:
 
 {userInput}"""
 
         completion = ollama.chat(
             model=config.ollamaDefaultModel,
             messages=[
                 *ongoingMessages,
@@ -2236,15 +2243,34 @@
             format="json",
             stream=False,
             options=Options(
                 temperature=config.llmTemperature,
             ),
         )
         # parameters
-        return json.loads(completion["message"]["content"])
+        output = json.loads(completion["message"]["content"])
+        # final check below
+        if "code" in output and not output["code"]:
+            codeDescription = parameters["code"]["description"]
+            template = {
+                "code": ""
+            }
+            system = f"""Use this template:
+
+{template}
+
+To generate a JSON that contains {len(template)} key, "code", based on my request.
+"code" is the requested python code.
+
+Remember, give me the code only in your response, without extra comment or information."""
+            if config.developer:
+                self.print3(f"""Code generation: {codeDescription}""")
+            codeOutput = self.getResponseDict(prompt=f"""{codeDescription}\n\nHere is my request / query:\n\n{userInput}""", system=system).get("code", "")
+            output["code"] = codeOutput
+        return output
 
     def launchChatbot(self, chatbot, userInput):
         if config.isTermux:
             chatbot = "chatgpt"
         chatbots = {
             "chatgpt": lambda: ChatGPT().run(userInput),
             "geminipro": lambda: GeminiPro(temperature=config.llmTemperature).run(userInput),
```

### Comparing `freegenius-0.0.8/freegenius/main.py` & `freegenius-0.0.9/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.8/freegenius/utils/shortcuts.py` & `freegenius-0.0.9/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.8/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.9/freegenius.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.8
+Version: 0.0.9
 Summary: FreeGenius AI, a FREE, LOCAL, OFFLINE & HIGHLY CUSTOMIZABLE AI suite that supports numerous open-source LLMs, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/freegenius
 Project-URL: Tracker, https://github.com/eliranwong/freegenius/issues
@@ -32,9 +32,12 @@
 
 # Progress
 
 ... in progress ...
 
 * preparing core features: action screening & calling
 
+* testing multi-step actions
+
 not in production yet
 
+
```

### Comparing `freegenius-0.0.8/setup.py` & `freegenius-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         mod = line.strip()
         if mod:
             install_requires.append(mod)
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.08",
+    version="0.0.09",
     python_requires=">=3.8",
     description="FreeGenius AI, a FREE, LOCAL, OFFLINE & HIGHLY CUSTOMIZABLE AI suite that supports numerous open-source LLMs, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     packages=[
         package,
```

