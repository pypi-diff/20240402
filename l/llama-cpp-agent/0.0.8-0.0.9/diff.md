# Comparing `tmp/llama-cpp-agent-0.0.8.tar.gz` & `tmp/llama-cpp-agent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-cpp-agent-0.0.8.tar", last modified: Tue Jan  9 00:17:26 2024, max compression
+gzip compressed data, was "llama-cpp-agent-0.0.9.tar", last modified: Tue Jan  9 00:23:46 2024, max compression
```

## Comparing `llama-cpp-agent-0.0.8.tar` & `llama-cpp-agent-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.057213 llama-cpp-agent-0.0.8/
--rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama-cpp-agent-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    20739 2024-01-09 00:17:26.056206 llama-cpp-agent-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    19866 2024-01-09 00:14:53.000000 llama-cpp-agent-0.0.8/ReadMe.md
--rw-rw-rw-   0        0        0      898 2024-01-09 00:17:12.000000 llama-cpp-agent-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-09 00:17:26.057213 llama-cpp-agent-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.027959 llama-cpp-agent-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.042026 llama-cpp-agent-0.0.8/src/llama_cpp_agent/
--rw-rw-rw-   0        0        0        0 2024-01-04 14:13:41.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.051544 llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/
--rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-12-31 17:45:56.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-rw-rw-   0        0        0     5239 2024-01-06 23:32:35.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-rw-rw-   0        0        0     4285 2024-01-04 13:55:03.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-rw-rw-   0        0        0      985 2023-12-31 16:27:06.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-rw-rw-   0        0        0     5155 2024-01-06 03:18:06.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/function_calling.py
--rw-rw-rw-   0        0        0     7941 2024-01-08 23:56:37.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/function_calling_agent.py
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.052542 llama-cpp-agent-0.0.8/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-rw-rw-   0        0        0    48661 2024-01-08 23:54:53.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-rw-rw-   0        0        0    11797 2024-01-07 06:33:35.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/llm_agent.py
--rw-rw-rw-   0        0        0     3386 2024-01-06 23:32:35.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/llm_prompt_template.py
--rw-rw-rw-   0        0        0     2142 2024-01-07 06:36:32.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/llm_settings.py
--rw-rw-rw-   0        0        0    10575 2024-01-07 06:33:35.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/messages_formatter.py
--rw-rw-rw-   0        0        0     1293 2024-01-06 03:16:07.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/output_parser.py
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.054700 llama-cpp-agent-0.0.8/src/llama_cpp_agent/providers/
--rw-rw-rw-   0        0        0        0 2024-01-08 13:25:58.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/providers/__init__.py
--rw-rw-rw-   0        0        0     2598 2024-01-08 17:08:49.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/providers/llama_cpp_server_provider.py
--rw-rw-rw-   0        0        0     5367 2024-01-07 03:37:58.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent/structured_output_agent.py
-drwxrwxrwx   0        0        0        0 2024-01-09 00:17:26.054700 llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/
--rw-rw-rw-   0        0        0    20739 2024-01-09 00:17:26.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2024-01-09 00:17:26.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-09 00:17:26.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-01-09 00:17:26.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-01-09 00:17:26.000000 llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.885549 llama-cpp-agent-0.0.9/
+-rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama-cpp-agent-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    23095 2024-01-09 00:23:46.884549 llama-cpp-agent-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    22222 2024-01-09 00:21:43.000000 llama-cpp-agent-0.0.9/ReadMe.md
+-rw-rw-rw-   0        0        0      898 2024-01-09 00:22:05.000000 llama-cpp-agent-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-09 00:23:46.885549 llama-cpp-agent-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.858704 llama-cpp-agent-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.869903 llama-cpp-agent-0.0.9/src/llama_cpp_agent/
+-rw-rw-rw-   0        0        0        0 2024-01-04 14:13:41.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.879038 llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/
+-rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-rw-rw-   0        0        0     1903 2023-12-31 17:45:56.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-rw-rw-   0        0        0     5239 2024-01-06 23:32:35.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-rw-rw-   0        0        0     4285 2024-01-04 13:55:03.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-rw-rw-   0        0        0      985 2023-12-31 16:27:06.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-rw-rw-   0        0        0     5155 2024-01-06 03:18:06.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/function_calling.py
+-rw-rw-rw-   0        0        0     7941 2024-01-08 23:56:37.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/function_calling_agent.py
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.880543 llama-cpp-agent-0.0.9/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-rw-rw-   0        0        0    48661 2024-01-08 23:54:53.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-rw-rw-   0        0        0    11797 2024-01-07 06:33:35.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/llm_agent.py
+-rw-rw-rw-   0        0        0     3386 2024-01-06 23:32:35.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/llm_prompt_template.py
+-rw-rw-rw-   0        0        0     2142 2024-01-07 06:36:32.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/llm_settings.py
+-rw-rw-rw-   0        0        0    10575 2024-01-07 06:33:35.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/messages_formatter.py
+-rw-rw-rw-   0        0        0     1293 2024-01-06 03:16:07.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/output_parser.py
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.882549 llama-cpp-agent-0.0.9/src/llama_cpp_agent/providers/
+-rw-rw-rw-   0        0        0        0 2024-01-08 13:25:58.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/providers/__init__.py
+-rw-rw-rw-   0        0        0     2598 2024-01-08 17:08:49.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/providers/llama_cpp_server_provider.py
+-rw-rw-rw-   0        0        0     5367 2024-01-07 03:37:58.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent/structured_output_agent.py
+drwxrwxrwx   0        0        0        0 2024-01-09 00:23:46.883550 llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/
+-rw-rw-rw-   0        0        0    23095 2024-01-09 00:23:46.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2024-01-09 00:23:46.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-09 00:23:46.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-01-09 00:23:46.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-01-09 00:23:46.000000 llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama-cpp-agent-0.0.8/LICENSE` & `llama-cpp-agent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/PKG-INFO` & `llama-cpp-agent-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework for building LLM based AI agents with llama-cpp-python.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -71,28 +71,28 @@
 
 ```
 
 ### Function Calling Agent Example
 This example shows how to use the FunctionCallingAgent for function calling with OpenAI like dictionaries, normal python functions and functions defined as pydantic models like in the "Instructor" library.
 
 ```python
-
 # Example that uses the FunctionCallingAgent class to create a function calling agent.
-
+import json
 from enum import Enum
 from typing import Union, Any
 
 from llama_cpp import Llama
 from pydantic import BaseModel, Field
 
 from llama_cpp_agent.llm_settings import LlamaLLMSettings, LlamaLLMGenerationSettings
 
 from llama_cpp_agent.function_calling_agent import FunctionCallingAgent
 
 
+# llama-cpp-agent supports type hinted function definitions for function calling.
 # Write to file function that can be used by the agent. Docstring will be used in system prompt.
 def write_to_file(chain_of_thought: str, file_path: str, file_content: str):
     """
     Write file to the user filesystem.
     :param chain_of_thought: Your chain of thought while writing the file.
     :param file_path: The file path includes the filename and file ending.
     :param file_content: The actual content to write.
@@ -119,15 +119,15 @@
 # Enum for the calculator tool.
 class MathOperation(Enum):
     ADD = "add"
     SUBTRACT = "subtract"
     MULTIPLY = "multiply"
     DIVIDE = "divide"
 
-
+# llama-cpp-agent also supports "Instructor" library like function definitions as Pydantic models for function calling.
 # Simple pydantic calculator tool for the agent that can add, subtract, multiply, and divide. Docstring and description of fields will be used in system prompt.
 class Calculator(BaseModel):
     """
     Perform a math operation on two numbers.
     """
     number_one: Any = Field(..., description="First number.")
     operation: MathOperation = Field(..., description="Math operation to perform.")
@@ -142,35 +142,79 @@
             return self.number_one * self.number_two
         elif self.operation == MathOperation.DIVIDE:
             return self.number_one / self.number_two
         else:
             raise ValueError("Unknown operation.")
 
 
+# Example function based on an OpenAI example.
+# llama-cpp-agent also supports OpenAI like dictionaries for function definition.
+def get_current_weather(location, unit):
+    """Get the current weather in a given location"""
+    if "London" in location:
+        return json.dumps({"location": "London", "temperature": "42", "unit": unit.value})
+    elif "New York" in location:
+        return json.dumps({"location": "New York", "temperature": "24", "unit": unit.value})
+    elif "North Pole" in location:
+        return json.dumps({"location": "North Pole", "temperature": "-42", "unit": unit.value})
+    else:
+        return json.dumps({"location": location, "temperature": "unknown"})
+# Here is a function definition in OpenAI style
+tools = [
+    {
+        "type": "function",
+        "function": {
+            "name": "get_current_weather",
+            "description": "Get the current weather in a given location",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "location": {
+                        "type": "string",
+                        "description": "The city and state, e.g. San Francisco, CA",
+                    },
+                    "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
+                },
+                "required": ["location"],
+            },
+        },
+    }
+]
+# To make the OpenAI function callable for the function calling agent we need a list with actual function in it:
+tool_functions = [get_current_weather]
+
 # Callback for receiving messages for the user.
 def send_message_to_user_callback(message: str):
     print(message)
 
+
 generation_settings = LlamaLLMGenerationSettings(temperature=0.65, top_p=0.5, tfs_z=0.975)
 
 # Can be saved and loaded like that:
 # generation_settings.save("generation_settings.json")
 # generation_settings = LlamaLLMGenerationSettings.load_from_file("generation_settings.json")
 
-function_call_agent = FunctionCallingAgent(LlamaLLMSettings.load_from_file("openhermes-2.5-mistral-7b.Q8_0.json"),  # Can lama-cpp-python Llama class or LlamaLLMSettings class.
+function_call_agent = FunctionCallingAgent(LlamaLLMSettings.load_from_file("openhermes-2.5-mistral-7b.Q8_0.json"),
+                                           # Can lama-cpp-python Llama class or LlamaLLMSettings class.
                                            llama_generation_settings=generation_settings,
+                                           # A tuple of the OpenAI style function definitions and the actual functions
+                                           open_ai_functions=(tools, tool_functions),
+                                           # Just a list of type hinted functions for normal Python functions
                                            python_functions=[write_to_file, read_file],
+                                           # Just a list of pydantic types
                                            pydantic_functions=[Calculator],
-                                           send_message_to_user_callback=send_message_to_user_callback)
+                                           # Callback for receiving messages for the user.
+                                           send_message_to_user_callback=send_message_to_user_callback, debug_output=True)
 
 while True:
     user_input = input(">")
     function_call_agent.generate_response(user_input)
     function_call_agent.save("function_calling_agent.json")
 
+
 ```
 Example Input 1
 ```text
 What is 42 * 42?
 ```
 Example output 1
 ```json
@@ -189,15 +233,15 @@
     "message": "Function Call Result: 1764"
   }
 }
 Function Call Result: 1764
 ```
 Example Input 2
 ```text
-What is 42 * 42?
+What is the current weather in London celsius?
 ```
 Example output 2
 ```json
 
 {
   "function": "get-current-weather",
   "function-parameters": {
```

### Comparing `llama-cpp-agent-0.0.8/ReadMe.md` & `llama-cpp-agent-0.0.9/ReadMe.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,28 +51,28 @@
 
 ```
 
 ### Function Calling Agent Example
 This example shows how to use the FunctionCallingAgent for function calling with OpenAI like dictionaries, normal python functions and functions defined as pydantic models like in the "Instructor" library.
 
 ```python
-
 # Example that uses the FunctionCallingAgent class to create a function calling agent.
-
+import json
 from enum import Enum
 from typing import Union, Any
 
 from llama_cpp import Llama
 from pydantic import BaseModel, Field
 
 from llama_cpp_agent.llm_settings import LlamaLLMSettings, LlamaLLMGenerationSettings
 
 from llama_cpp_agent.function_calling_agent import FunctionCallingAgent
 
 
+# llama-cpp-agent supports type hinted function definitions for function calling.
 # Write to file function that can be used by the agent. Docstring will be used in system prompt.
 def write_to_file(chain_of_thought: str, file_path: str, file_content: str):
     """
     Write file to the user filesystem.
     :param chain_of_thought: Your chain of thought while writing the file.
     :param file_path: The file path includes the filename and file ending.
     :param file_content: The actual content to write.
@@ -99,15 +99,15 @@
 # Enum for the calculator tool.
 class MathOperation(Enum):
     ADD = "add"
     SUBTRACT = "subtract"
     MULTIPLY = "multiply"
     DIVIDE = "divide"
 
-
+# llama-cpp-agent also supports "Instructor" library like function definitions as Pydantic models for function calling.
 # Simple pydantic calculator tool for the agent that can add, subtract, multiply, and divide. Docstring and description of fields will be used in system prompt.
 class Calculator(BaseModel):
     """
     Perform a math operation on two numbers.
     """
     number_one: Any = Field(..., description="First number.")
     operation: MathOperation = Field(..., description="Math operation to perform.")
@@ -122,35 +122,79 @@
             return self.number_one * self.number_two
         elif self.operation == MathOperation.DIVIDE:
             return self.number_one / self.number_two
         else:
             raise ValueError("Unknown operation.")
 
 
+# Example function based on an OpenAI example.
+# llama-cpp-agent also supports OpenAI like dictionaries for function definition.
+def get_current_weather(location, unit):
+    """Get the current weather in a given location"""
+    if "London" in location:
+        return json.dumps({"location": "London", "temperature": "42", "unit": unit.value})
+    elif "New York" in location:
+        return json.dumps({"location": "New York", "temperature": "24", "unit": unit.value})
+    elif "North Pole" in location:
+        return json.dumps({"location": "North Pole", "temperature": "-42", "unit": unit.value})
+    else:
+        return json.dumps({"location": location, "temperature": "unknown"})
+# Here is a function definition in OpenAI style
+tools = [
+    {
+        "type": "function",
+        "function": {
+            "name": "get_current_weather",
+            "description": "Get the current weather in a given location",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "location": {
+                        "type": "string",
+                        "description": "The city and state, e.g. San Francisco, CA",
+                    },
+                    "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
+                },
+                "required": ["location"],
+            },
+        },
+    }
+]
+# To make the OpenAI function callable for the function calling agent we need a list with actual function in it:
+tool_functions = [get_current_weather]
+
 # Callback for receiving messages for the user.
 def send_message_to_user_callback(message: str):
     print(message)
 
+
 generation_settings = LlamaLLMGenerationSettings(temperature=0.65, top_p=0.5, tfs_z=0.975)
 
 # Can be saved and loaded like that:
 # generation_settings.save("generation_settings.json")
 # generation_settings = LlamaLLMGenerationSettings.load_from_file("generation_settings.json")
 
-function_call_agent = FunctionCallingAgent(LlamaLLMSettings.load_from_file("openhermes-2.5-mistral-7b.Q8_0.json"),  # Can lama-cpp-python Llama class or LlamaLLMSettings class.
+function_call_agent = FunctionCallingAgent(LlamaLLMSettings.load_from_file("openhermes-2.5-mistral-7b.Q8_0.json"),
+                                           # Can lama-cpp-python Llama class or LlamaLLMSettings class.
                                            llama_generation_settings=generation_settings,
+                                           # A tuple of the OpenAI style function definitions and the actual functions
+                                           open_ai_functions=(tools, tool_functions),
+                                           # Just a list of type hinted functions for normal Python functions
                                            python_functions=[write_to_file, read_file],
+                                           # Just a list of pydantic types
                                            pydantic_functions=[Calculator],
-                                           send_message_to_user_callback=send_message_to_user_callback)
+                                           # Callback for receiving messages for the user.
+                                           send_message_to_user_callback=send_message_to_user_callback, debug_output=True)
 
 while True:
     user_input = input(">")
     function_call_agent.generate_response(user_input)
     function_call_agent.save("function_calling_agent.json")
 
+
 ```
 Example Input 1
 ```text
 What is 42 * 42?
 ```
 Example output 1
 ```json
@@ -169,15 +213,15 @@
     "message": "Function Call Result: 1764"
   }
 }
 Function Call Result: 1764
 ```
 Example Input 2
 ```text
-What is 42 * 42?
+What is the current weather in London celsius?
 ```
 Example output 2
 ```json
 
 {
   "function": "get-current-weather",
   "function-parameters": {
```

### Comparing `llama-cpp-agent-0.0.8/pyproject.toml` & `llama-cpp-agent-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.0.8"
+version = "0.0.9"
 description = "A framework for building LLM based AI agents with llama-cpp-python."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.26",
     "pydantic>=2.5.3"
 ]
```

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/function_calling.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/function_calling.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/function_calling_agent.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/function_calling_agent.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/llm_agent.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/llm_agent.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/llm_prompt_template.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/llm_settings.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/llm_settings.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/messages_formatter.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/messages_formatter.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/output_parser.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/providers/llama_cpp_server_provider.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/providers/llama_cpp_server_provider.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent/structured_output_agent.py` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework for building LLM based AI agents with llama-cpp-python.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -71,28 +71,28 @@
 
 ```
 
 ### Function Calling Agent Example
 This example shows how to use the FunctionCallingAgent for function calling with OpenAI like dictionaries, normal python functions and functions defined as pydantic models like in the "Instructor" library.
 
 ```python
-
 # Example that uses the FunctionCallingAgent class to create a function calling agent.
-
+import json
 from enum import Enum
 from typing import Union, Any
 
 from llama_cpp import Llama
 from pydantic import BaseModel, Field
 
 from llama_cpp_agent.llm_settings import LlamaLLMSettings, LlamaLLMGenerationSettings
 
 from llama_cpp_agent.function_calling_agent import FunctionCallingAgent
 
 
+# llama-cpp-agent supports type hinted function definitions for function calling.
 # Write to file function that can be used by the agent. Docstring will be used in system prompt.
 def write_to_file(chain_of_thought: str, file_path: str, file_content: str):
     """
     Write file to the user filesystem.
     :param chain_of_thought: Your chain of thought while writing the file.
     :param file_path: The file path includes the filename and file ending.
     :param file_content: The actual content to write.
@@ -119,15 +119,15 @@
 # Enum for the calculator tool.
 class MathOperation(Enum):
     ADD = "add"
     SUBTRACT = "subtract"
     MULTIPLY = "multiply"
     DIVIDE = "divide"
 
-
+# llama-cpp-agent also supports "Instructor" library like function definitions as Pydantic models for function calling.
 # Simple pydantic calculator tool for the agent that can add, subtract, multiply, and divide. Docstring and description of fields will be used in system prompt.
 class Calculator(BaseModel):
     """
     Perform a math operation on two numbers.
     """
     number_one: Any = Field(..., description="First number.")
     operation: MathOperation = Field(..., description="Math operation to perform.")
@@ -142,35 +142,79 @@
             return self.number_one * self.number_two
         elif self.operation == MathOperation.DIVIDE:
             return self.number_one / self.number_two
         else:
             raise ValueError("Unknown operation.")
 
 
+# Example function based on an OpenAI example.
+# llama-cpp-agent also supports OpenAI like dictionaries for function definition.
+def get_current_weather(location, unit):
+    """Get the current weather in a given location"""
+    if "London" in location:
+        return json.dumps({"location": "London", "temperature": "42", "unit": unit.value})
+    elif "New York" in location:
+        return json.dumps({"location": "New York", "temperature": "24", "unit": unit.value})
+    elif "North Pole" in location:
+        return json.dumps({"location": "North Pole", "temperature": "-42", "unit": unit.value})
+    else:
+        return json.dumps({"location": location, "temperature": "unknown"})
+# Here is a function definition in OpenAI style
+tools = [
+    {
+        "type": "function",
+        "function": {
+            "name": "get_current_weather",
+            "description": "Get the current weather in a given location",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "location": {
+                        "type": "string",
+                        "description": "The city and state, e.g. San Francisco, CA",
+                    },
+                    "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
+                },
+                "required": ["location"],
+            },
+        },
+    }
+]
+# To make the OpenAI function callable for the function calling agent we need a list with actual function in it:
+tool_functions = [get_current_weather]
+
 # Callback for receiving messages for the user.
 def send_message_to_user_callback(message: str):
     print(message)
 
+
 generation_settings = LlamaLLMGenerationSettings(temperature=0.65, top_p=0.5, tfs_z=0.975)
 
 # Can be saved and loaded like that:
 # generation_settings.save("generation_settings.json")
 # generation_settings = LlamaLLMGenerationSettings.load_from_file("generation_settings.json")
 
-function_call_agent = FunctionCallingAgent(LlamaLLMSettings.load_from_file("openhermes-2.5-mistral-7b.Q8_0.json"),  # Can lama-cpp-python Llama class or LlamaLLMSettings class.
+function_call_agent = FunctionCallingAgent(LlamaLLMSettings.load_from_file("openhermes-2.5-mistral-7b.Q8_0.json"),
+                                           # Can lama-cpp-python Llama class or LlamaLLMSettings class.
                                            llama_generation_settings=generation_settings,
+                                           # A tuple of the OpenAI style function definitions and the actual functions
+                                           open_ai_functions=(tools, tool_functions),
+                                           # Just a list of type hinted functions for normal Python functions
                                            python_functions=[write_to_file, read_file],
+                                           # Just a list of pydantic types
                                            pydantic_functions=[Calculator],
-                                           send_message_to_user_callback=send_message_to_user_callback)
+                                           # Callback for receiving messages for the user.
+                                           send_message_to_user_callback=send_message_to_user_callback, debug_output=True)
 
 while True:
     user_input = input(">")
     function_call_agent.generate_response(user_input)
     function_call_agent.save("function_calling_agent.json")
 
+
 ```
 Example Input 1
 ```text
 What is 42 * 42?
 ```
 Example output 1
 ```json
@@ -189,15 +233,15 @@
     "message": "Function Call Result: 1764"
   }
 }
 Function Call Result: 1764
 ```
 Example Input 2
 ```text
-What is 42 * 42?
+What is the current weather in London celsius?
 ```
 Example output 2
 ```json
 
 {
   "function": "get-current-weather",
   "function-parameters": {
```

### Comparing `llama-cpp-agent-0.0.8/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama-cpp-agent-0.0.9/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

