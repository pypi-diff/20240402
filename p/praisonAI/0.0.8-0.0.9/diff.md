# Comparing `tmp/praisonai-0.0.8.tar.gz` & `tmp/praisonai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praisonai-0.0.8.tar", max compression
+gzip compressed data, was "praisonai-0.0.9.tar", max compression
```

## Comparing `praisonai-0.0.8.tar` & `praisonai-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      449 2024-03-25 13:03:47.819949 praisonai-0.0.8/README.md
--rw-r--r--   0        0        0       59 2024-03-25 18:06:26.033522 praisonai-0.0.8/praisonai/__init__.py
--rw-r--r--   0        0        0      144 2024-03-25 20:12:46.307088 praisonai-0.0.8/praisonai/__main__.py
--rw-r--r--   0        0        0     4337 2024-03-25 14:00:46.752020 praisonai-0.0.8/praisonai/auto-old.py
--rw-r--r--   0        0        0     4769 2024-03-25 18:35:58.294230 praisonai-0.0.8/praisonai/auto.py
--rw-r--r--   0        0        0     5352 2024-03-25 14:40:29.875274 praisonai-0.0.8/praisonai/cli-old.py
--rw-r--r--   0        0        0     6922 2024-03-25 20:47:49.212610 praisonai-0.0.8/praisonai/cli.py
--rw-r--r--   0        0        0     3707 2024-03-19 17:31:03.484823 praisonai-0.0.8/praisonai/test.py
--rw-r--r--   0        0        0       21 2024-03-19 17:22:44.218489 praisonai-0.0.8/praisonai/version.py
--rw-r--r--   0        0        0      927 2024-03-25 20:51:57.389444 praisonai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 praisonai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      449 2024-03-25 13:03:47.819949 praisonai-0.0.9/README.md
+-rw-r--r--   0        0        0       59 2024-03-25 18:06:26.033522 praisonai-0.0.9/praisonai/__init__.py
+-rw-r--r--   0        0        0      144 2024-03-25 20:12:46.307088 praisonai-0.0.9/praisonai/__main__.py
+-rw-r--r--   0        0        0     4337 2024-03-25 14:00:46.752020 praisonai-0.0.9/praisonai/auto-old.py
+-rw-r--r--   0        0        0     4717 2024-03-25 21:05:55.097394 praisonai-0.0.9/praisonai/auto.py
+-rw-r--r--   0        0        0     5352 2024-03-25 14:40:29.875274 praisonai-0.0.9/praisonai/cli-old.py
+-rw-r--r--   0        0        0     7599 2024-03-25 21:08:17.051505 praisonai-0.0.9/praisonai/cli.py
+-rw-r--r--   0        0        0     3707 2024-03-19 17:31:03.484823 praisonai-0.0.9/praisonai/test.py
+-rw-r--r--   0        0        0       21 2024-03-19 17:22:44.218489 praisonai-0.0.9/praisonai/version.py
+-rw-r--r--   0        0        0      927 2024-03-25 21:08:46.095214 praisonai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 praisonai-0.0.9/PKG-INFO
```

### Comparing `praisonai-0.0.8/praisonai/auto-old.py` & `praisonai-0.0.9/praisonai/auto-old.py`

 * *Files identical despite different names*

### Comparing `praisonai-0.0.8/praisonai/auto.py` & `praisonai-0.0.9/praisonai/auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,14 @@
 
         yaml_data = {
             "framework": "crewai",
             "topic": self.topic,
             "roles": {},
             "dependencies": []
         }
-        print(self.topic)
-        print(self.framework)
 
         for role_id, role_details in json_data['roles'].items():
             yaml_data['roles'][role_id] = {
                 "backstory": "" + role_details['backstory'],
                 "goal": role_details['goal'],
                 "role": role_details['role'],
                 "tasks": {}
@@ -127,9 +125,9 @@
 }
 }
 }
         """
         return user_content
 
     
-generator = AutoGenerator(framework="crewai", topic="Create a snake game in python")
-print(generator.generate())
+# generator = AutoGenerator(framework="crewai", topic="Create a snake game in python")
+# print(generator.generate())
```

### Comparing `praisonai-0.0.8/praisonai/cli-old.py` & `praisonai-0.0.9/praisonai/cli-old.py`

 * *Files identical despite different names*

### Comparing `praisonai-0.0.8/praisonai/cli.py` & `praisonai-0.0.9/praisonai/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 load_dotenv()
 import autogen
 import gradio as gr
 import argparse
 from .auto import AutoGenerator
 
 class PraisonAI:
-    def __init__(self, agent_file="agents.yaml", framework="crewai", auto=False):
+    def __init__(self, agent_file="agents.yaml", framework="crewai", auto=False, init=False):
         self.config_list = [
             {
                 'model': os.environ.get("OPENAI_MODEL_NAME", "gpt-4-turbo-preview"),
                 'base_url': os.environ.get("OPENAI_API_BASE", "https://api.openai.com/v1"),
             }
         ]
         self.agent_file = agent_file
         self.framework = framework
         self.auto = auto
+        self.init = init
 
     def generate_crew_and_kickoff(self):
         with open(self.agent_file, 'r') as f:
             config = yaml.safe_load(f)
 
         topic = config['topic']  
         framework = self.framework or config.get('framework')
@@ -119,36 +120,45 @@
             else:
                 full_path = os.path.abspath(args.agent_file)
             self.agent_file = full_path
         else:
             full_path = os.path.abspath(self.agent_file)
             self.filename = full_path
         
-        if args.auto:
-            self.topic = ' '.join(args.auto)
-        elif self.auto:  # Use the auto attribute if args.auto is not provided
+        if args.auto or args.init:
+            temp_topic = ' '.join(args.auto) if args.auto else ' '.join(args.init)
+            self.topic = temp_topic
+        elif self.auto or self.init:  # Use the auto attribute if args.auto is not provided
             self.topic = self.auto
             
         if args.auto or self.auto:
+            self.filename = "test.yaml"
             generator = AutoGenerator(topic=self.topic , framework=self.framework)
             self.agent_file = generator.generate()
             result = self.generate_crew_and_kickoff()
             return result
+        elif args.init or self.init:
+            self.filename = "agents.yaml"
+            generator = AutoGenerator(topic=self.topic , framework=self.framework, filename=self.filename)
+            self.agent_file = generator.generate()
+            print("File {} created successfully".format(self.agent_file))
+            return "File {} created successfully".format(self.agent_file)
         
         if ui:
             self.create_gradio_interface()
         else:
             result = self.generate_crew_and_kickoff()
             return result
             
     def parse_args(self):
         parser = argparse.ArgumentParser(prog="praisonai", description="praisonAI command-line interface")
         parser.add_argument("--framework", choices=["crewai", "autogen"], default="crewai", help="Specify the framework")
         parser.add_argument("--ui", action="store_true", help="Enable UI mode")
         parser.add_argument("--auto", nargs=argparse.REMAINDER, help="Enable auto mode and pass arguments for it")
+        parser.add_argument("--init", nargs=argparse.REMAINDER, help="Enable auto mode and pass arguments for it")
         parser.add_argument("agent_file", nargs="?", help="Specify the agent file")
 
         return parser.parse_args()
 
     def create_gradio_interface(self):
         def generate_crew_and_kickoff_interface(agent_file, framework):
             result = self.generate_crew_and_kickoff()
```

### Comparing `praisonai-0.0.8/praisonai/test.py` & `praisonai-0.0.9/praisonai/test.py`

 * *Files identical despite different names*

### Comparing `praisonai-0.0.8/pyproject.toml` & `praisonai-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "praisonAI"
-version = "0.0.8"
+version = "0.0.9"
 description = "praisonAI application combines AutoGen and CrewAI or similar frameworks into a low-code solution for building and managing multi-agent LLM systems, focusing on simplicity, customization, and efficient human-agent collaboration."
 authors = ["Mervin Praison"]
 license = ""
 readme = "README.md"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/mervinpraison/praisonAI"
```

### Comparing `praisonai-0.0.8/PKG-INFO` & `praisonai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praisonAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: praisonAI application combines AutoGen and CrewAI or similar frameworks into a low-code solution for building and managing multi-agent LLM systems, focusing on simplicity, customization, and efficient human-agent collaboration.
 Author: Mervin Praison
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

