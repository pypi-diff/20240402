# Comparing `tmp/langchain-decorators-0.5.4.tar.gz` & `tmp/langchain-decorators-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.5.4.tar", last modified: Wed Feb 14 15:21:33 2024, max compression
+gzip compressed data, was "langchain-decorators-0.5.5.tar", last modified: Tue Apr  2 11:00:30 2024, max compression
```

## Comparing `langchain-decorators-0.5.4.tar` & `langchain-decorators-0.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-14 15:21:33.404629 langchain-decorators-0.5.4/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.5.4/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22991 2024-02-14 15:21:33.404336 langchain-decorators-0.5.4/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22584 2023-11-15 22:10:25.000000 langchain-decorators-0.5.4/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.5.4/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-02-14 15:21:33.404675 langchain-decorators-0.5.4/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.5.4/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-14 15:21:33.395960 langchain-decorators-0.5.4/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-14 15:21:33.402364 langchain-decorators-0.5.4/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-02-14 15:21:19.000000 langchain-decorators-0.5.4/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    37071 2024-02-14 08:32:56.000000 langchain-decorators-0.5.4/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain-decorators-0.5.4/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21044 2023-12-18 07:41:39.000000 langchain-decorators-0.5.4/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    24449 2023-12-23 19:44:48.000000 langchain-decorators-0.5.4/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22295 2024-02-12 07:37:20.000000 langchain-decorators-0.5.4/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain-decorators-0.5.4/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain-decorators-0.5.4/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-01-05 14:48:06.000000 langchain-decorators-0.5.4/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain-decorators-0.5.4/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-14 15:21:33.403939 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22991 2024-02-14 15:21:33.000000 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-02-14 15:21:33.000000 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-02-14 15:21:33.000000 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-02-14 15:21:33.000000 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-02-14 15:21:33.000000 langchain-decorators-0.5.4/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.452466 langchain-decorators-0.5.5/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.5.5/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    22991 2024-04-02 11:00:30.452209 langchain-decorators-0.5.5/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    22584 2023-11-15 22:10:25.000000 langchain-decorators-0.5.5/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.5.5/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-04-02 11:00:30.452508 langchain-decorators-0.5.5/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.5.5/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.444472 langchain-decorators-0.5.5/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.449942 langchain-decorators-0.5.5/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-04-02 10:59:59.000000 langchain-decorators-0.5.5/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    37071 2024-02-14 08:32:56.000000 langchain-decorators-0.5.5/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain-decorators-0.5.5/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21044 2023-12-18 07:41:39.000000 langchain-decorators-0.5.5/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain-decorators-0.5.5/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21900 2024-04-02 10:42:42.000000 langchain-decorators-0.5.5/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain-decorators-0.5.5/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain-decorators-0.5.5/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-01-05 14:48:06.000000 langchain-decorators-0.5.5/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain-decorators-0.5.5/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.451899 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    22991 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.5.4/LICENSE` & `langchain-decorators-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/PKG-INFO` & `langchain-decorators-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.4
+Version: 0.5.5
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.5.4/README.md` & `langchain-decorators-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/setup.py` & `langchain-decorators-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/chains.py` & `langchain-decorators-0.5.5/src/langchain_decorators/chains.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/common.py` & `langchain-decorators-0.5.5/src/langchain_decorators/common.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/function_decorator.py` & `langchain-decorators-0.5.5/src/langchain_decorators/function_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.5.5/src/langchain_decorators/output_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,42 +87,50 @@
 
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
         return "Reply only Yes or No.\nUse this format: Final decision: Yes/No"
 
 class JsonOutputParser(BaseOutputParser):
     """Class to parse the output of an LLM call to a Json."""
-    
+
     @property
     def _type(self) -> str:
         return "json"
-    
+
     def find_json_block(self,text, raise_if_not_found=True):
+
+        start_code_block = list(re.finditer(r"(\n|^)```((json)|\n)", text))
+        if start_code_block:
+            i_start = start_code_block[0].span()[1]
+            end_code_block = list(re.finditer(r"\n```($|\n)", text[i_start:]))
+            if end_code_block:
+                i_end = end_code_block[0].span()[0]
+                text = text[i_start : i_start + i_end]
+
         match = re.search(r"[\{|\[].*[\}|\]]", text.strip(),
                               re.MULTILINE | re.IGNORECASE | re.DOTALL)
         if not match and raise_if_not_found:
             raise OutputParserExceptionWithOriginal(message="No JSON found in the response", original_output=text, error_code=ErrorCodes.INVALID_JSON)
         return match
 
     def replace_json_block(self, text: str, replace_func:Callable[[dict],str]) -> str:
         try:
-            
+
             match = self.find_json_block(text)
             json_str = match.group()
             i_start = match.start()
             _i_start = ("\n"+text).rfind("\n```", 0, i_start)
             i_end = match.end()
             _i_end = text.find("\n```\n", i_end)
             i_start=_i_start if _i_start>=0 else i_start
             i_end=_i_end+5 if _i_end>=0 else i_end
 
             json_dict = json.loads(json_str, strict=False)
             replacement = replace_func(json_dict)
             return (text[:i_start] + replacement + text[i_end:]).strip()
-            
 
         except (json.JSONDecodeError) as e:
 
             msg = f"Invalid JSON\n {text}\nGot: {e}"
             raise OutputParserExceptionWithOriginal(msg, text, error_code=ErrorCodes.INVALID_JSON)
 
     def parse(self, text: str) -> dict:
@@ -549,8 +557,8 @@
     return (description if _one_of else f"\" {description} \"")
 
 def describe_field_schema(field_schema:dict):
     if "type" in field_schema:
         res = field_schema.pop("type")
         return res + ", " + ", ".join([f"{k}:{v}" for k,v in field_schema.items()])
     else:
-        return ""
+        return ""
```

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.5.5/src/langchain_decorators/prompt_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import asyncio
 import logging
 import inspect
 
 from functools import wraps
 from types import coroutine
 from typing import Any, Callable, Dict, List, Optional,  Union
@@ -89,53 +88,48 @@
 
         `llm_selector_rule_key` - key of the LLM selector rule to use ... if set, only LLMs with assigned rule with this key will be considered. You can also use llm_selector_rule_key argument when calling the llm_prompt function to override the default rule key. 
 
         `functions_source` - only for bound functions ... name of a field or property on `self` that should be used as a source of functions for the OpenAI functions. If not set, you still can pass in functions as an argument, which will also override this.
 
         `control_kwargs` - kwargs that only controls other the behavior, and shall not be passed as template arguments. These are: `callbacks`, `followup_handle`, `llm_selector_rule_key`, `memory`, `functions`, `function_call`, `capture_stream`, `llm_selector_rule_key`, `stop`
     """
-    
-
 
     if  callable(prompt_type):
         # this is the case when the decorator is called without arguments
         # we initialize params with default values
         func = prompt_type
         prompt_type = PromptTypes.UNDEFINED
     else:
         func = None
-    
+
     if verbose is None:
         verbose = GlobalSettings.get_current_settings().verbose
-    
+
     if verbose:
         if prompt_type:
             prompt_type = prompt_type.as_verbose()
         else:
             prompt_type = PromptTypeSettings(color=LogColors.DARK_GRAY,log_level=100, capture_stream=capture_stream)
-            
-    
-    
+
     def decorator(func):
         name=func.__name__
 
         full_name=f"{func.__module__}.{name}" if func.__module__!="__main__" else name
         is_async = inspect.iscoroutinefunction(func)
-        
-        _llm_selector_rule_key=llm_selector_rule_key
 
+        _llm_selector_rule_key=llm_selector_rule_key
 
         if prompt_type:
             _capture_stream = prompt_type.capture_stream if capture_stream is None else capture_stream
         else:
             _capture_stream = capture_stream
         if _capture_stream and not is_async:
             print_log(f"Warning: capture_stream=True is only supported for async functions. Ignoring capture_stream for {full_name}", logging.WARNING, LogColors.YELLOW)
             _capture_stream=False
-        
+
         @wraps(func)
         def build_chain(*args, **kwargs)->LLMDecoratorChain:
             global_settings = GlobalSettings.get_current_settings()
 
             capture_stream=_capture_stream
 
             if "capture_stream" in kwargs:
@@ -149,85 +143,87 @@
                 capture_stream=False
 
             if "followup_handle" in kwargs:
                 followup_handle=kwargs["followup_handle"]
                 del kwargs["followup_handle"]
             else:
                 followup_handle=None
-            
+
             if not (llm or (prompt_type and prompt_type.llm)):
-                    if llm_selector:
-                        _llm_selector= llm_selector
-                    elif prompt_type and prompt_type.llm_selector:
-                        _llm_selector= prompt_type.llm_selector
-                    else:
-                        _llm_selector=  global_settings.llm_selector 
+                if llm_selector:
+                    _llm_selector= llm_selector
+                elif prompt_type and prompt_type.llm_selector:
+                    _llm_selector= prompt_type.llm_selector
+                else:
+                    _llm_selector=  global_settings.llm_selector 
 
-                    if capture_stream and not _llm_selector:
-                        if not global_settings.default_streaming_llm:
-                            print_log(f"Warning: capture_stream on {name} is on, but the default LLM {llm} doesn't seem to be supporting streaming.", logging.WARNING, LogColors.YELLOW)
-                            
-                        prompt_llm=global_settings.default_streaming_llm or global_settings.default_llm
-                    else:
-                        prompt_llm = global_settings.default_llm
+                if capture_stream and not _llm_selector:
+                    if not global_settings.default_streaming_llm:
+                        print_log(f"Warning: capture_stream on {name} is on, but the default LLM {llm} doesn't seem to be supporting streaming.", logging.WARNING, LogColors.YELLOW)
+
+                    prompt_llm=global_settings.default_streaming_llm or global_settings.default_llm
+                else:
+                    prompt_llm = global_settings.default_llm
+
+                if "llm_selector_rule_key" in kwargs:
+                    llm_selector_rule_key=kwargs["llm_selector_rule_key"]
+                    del kwargs["llm_selector_rule_key"]
+                else:
+                    llm_selector_rule_key=_llm_selector_rule_key
 
-                    if "llm_selector_rule_key" in kwargs:
-                        llm_selector_rule_key=kwargs["llm_selector_rule_key"]
-                        del kwargs["llm_selector_rule_key"]
-                    else:
-                        llm_selector_rule_key=_llm_selector_rule_key
-                
             else:
                 prompt_llm=llm or prompt_type.llm
                 llm_selector_rule_key=None
                 _llm_selector=None # if LLM is explicitly provided, we don't use the selector
                 if capture_stream:
-                    if  hasattr(llm,"streaming"):
-                        if not getattr(llm, "streaming"):
-                            print_log(f"Warning: capture_stream on {name} is on, but the provided LLM {llm} doesn't have streaming on! Stream wont be captured", logging.WARNING, LogColors.YELLOW)
+                    if hasattr(prompt_llm, "streaming"):
+                        if not getattr(prompt_llm, "streaming"):
+                            print_log(
+                                f"Warning: capture_stream on {name} is on, but the provided LLM {prompt_llm} doesn't have streaming on! Stream wont be captured",
+                                logging.WARNING,
+                                LogColors.YELLOW,
+                            )
                     else:
-                        print_log(f"Warning: capture_stream on {name} is on, but the provided LLM {llm} doesn't seem to be supporting streaming.", logging.WARNING, LogColors.YELLOW)
-                   
-                
+                        print_log(
+                            f"Warning: capture_stream on {name} is on, but the provided LLM {prompt_llm} doesn't seem to be supporting streaming.",
+                            logging.WARNING,
+                            LogColors.YELLOW,
+                        )
 
             _self=None
             if len(args)==1 and hasattr(args[0],"__dict__"):
                 # is a proper object
                 _self = args[0]
 
             elif len(args)>1:
                 raise Exception(f"Positional arguments are not supported for prompt functions. Only one positional argument as an object with attributes as a source of inputs is supported. Got: {args}")
-            
-            
+
             prompt_template = PromptDecoratorTemplate.from_func(func, 
                                                             template_format=template_format, 
                                                             output_parser=output_parser, 
                                                             format_instructions_parameter_key=format_instructions_parameter_key,
                                                             template_name=template_name,
                                                             template_version=template_version,
                                                             prompt_type=prompt_type,
                                                             original_kwargs=kwargs
                                                             )
-            
-            
 
             if prompt_template.default_values:
                 kwargs = {**prompt_template.default_values, **kwargs}
 
             if "output_parser" in kwargs:
                 callbacks=kwargs.pop("output_parser")
 
             if "callbacks" in kwargs:
                 callbacks=kwargs.pop("callbacks")
             else:
                 callbacks=[]
-            
+
             if capture_stream:
                 callbacks.append(StreamingContext.StreamingContextCallback())
-            
 
             if "memory" in kwargs:
                 memory = kwargs.pop("memory")
             else:
                 if memory_source:
                     if _self:
                         memory = getattr(_self, memory_source)
@@ -289,52 +285,51 @@
 
             elif isinstance(prompt_template.output_parser, OpenAIFunctionsPydanticOutputParser):
                 function=prompt_template.output_parser.build_llm_function()
                 kwargs["function_call"] = function
                 llmChain = LLMDecoratorChainWithFunctionSupport(**chain_kwargs, functions=[function])
             else:
                 llmChain = LLMDecoratorChain(**chain_kwargs)
-            
+
             reserved_inputs_violations=[key for key in prompt_template.input_variables if key in control_kwargs]
             if reserved_inputs_violations:
                 raise Exception(f"Invalid prompt template: {reserved_inputs_violations} are reserved prompt arguments and cannot be used in prompt template.")
-            
+
             unexpected_inputs = [key for key in kwargs if  key not in prompt_template.input_variables and key not in control_kwargs and key not in func_args ]
             if unexpected_inputs:
                 raise TypeError(f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}\nHint: Make sure that you've used all the inputs in the template")
-            
+
             kwargs = validate_and_enrich_kwargs(kwargs, _self,  memory,prompt_template.input_variables)
-                
-                
+
             if followup_handle:
                 followup_handle.bind_to_chain(llmChain)
                 if callbacks:
                     callbacks.append(followup_handle)
                 else:
                     callbacks=[followup_handle]
-            
+
             if stop_tokens:
                 kwargs["stop"]=stop_tokens
             call_args = {"inputs":kwargs, "return_only_outputs":True, "callbacks":callbacks}
             if llm_kwargs:
                 call_args["llm_kwargs"]=llm_kwargs
             llmChain.default_call_kwargs = call_args
-           
+
             return llmChain
 
         def validate_and_enrich_kwargs(kwargs, input_variables_source, memory, required_args, optional_args=None, additional_input_variables_source=None):
             missing_inputs = [ key for key in required_args if key not in kwargs ]
             if optional_args:
                 missing_inputs.extend([key for key in optional_args if key not in kwargs ])
             if format_instructions_parameter_key in missing_inputs:
                 missing_inputs.remove(format_instructions_parameter_key)
                 kwargs[format_instructions_parameter_key]=None #init the format instructions with None... will be filled later
             if memory and memory.memory_key in missing_inputs:
                 missing_inputs.remove(memory.memory_key)
-            
+
             def get_value_ext(source, key:str, default):
                 # this doesnśt work since native python Formatter doesn't support "." in keys
                 # if "." in key:
                 #     key, subpath = key.split(".",1)
                 # else:
                 subpath=None
 
@@ -343,15 +338,15 @@
                 else:
                     value = getattr(source, key, default)
 
                 if subpath and value and value != default:
                     return get_value_ext(value, subpath, default)
                 else:
                     return value
-                
+
             if missing_inputs:
                 missing_value={}
                 for key in missing_inputs:
                     if input_variables_source or additional_input_variables_source:
                         value= get_value_ext(input_variables_source, key,missing_value)
                         if value is missing_value:
                             value= get_value_ext(additional_input_variables_source, key,missing_value)
@@ -359,82 +354,76 @@
                         value=missing_value
 
                     if value is missing_value:
                         value= get_value_ext(kwargs, key,missing_value)
                         if value is missing_value:
                             if optional_args and key in optional_args:
                                 continue
-                        
+
                             raise TypeError(f"Missing a input for prompt function {full_name}: {key}.")
-                    
+
                     kwargs[key] = value
             return kwargs
-        
-        
+
         def get_preprocessing_args_by_running_func(*args,**kwargs):
             # temporary, we should always declare the args we want to use, but its not backward compatible
             kwargs_keys =  [*inspect.signature(func).parameters.keys()]
-            
+
             _extra_kwargs = [k for k in kwargs if k not in kwargs_keys]
-            
+
             if _extra_kwargs:
                 logging.warning(f"We should always declare all arguments of @llm_prompt if we are planning to use them. {_extra_kwargs} extra kwargs found...")
                 _result = func(*args,**{k:v for k,v in kwargs.items() if k not in _extra_kwargs})
             else:
-                 # use only this in the future
-                 _result = func(*args,**kwargs)
+                # use only this in the future
+                _result = func(*args,**kwargs)
 
             return _result
 
-            
-
         if not is_async:
-            
+
             @wraps(func)
             def wrapper(*args, **kwargs):
                 _kwargs = get_preprocessing_args_by_running_func(*args,**kwargs)
-                
+
                 if _kwargs:
                     if not isinstance(_kwargs,dict):
                         raise Exception(f"Invalid @llm_prompt implementation: the result of the function call must be a dict, to augment the input args. Got: {_kwargs}")
                     kwargs.update(_kwargs)
-            
+
                 llmChain = build_chain(*args, **kwargs)
                 return llmChain.execute()
             wrapper.build_chain=build_chain
-            
+
             if inspect.signature(func).parameters.get("functions"):
                 if not func.__annotations__.get('return') or func.__annotations__.get('return') == OutputWithFunctionCall:
                     wrapper.__annotations__['return']= OutputWithFunctionCall
                 else:
                     wrapper.__annotations__['return']= OutputWithFunctionCall[func.__annotations__.get('return') ]
 
-            
             return wrapper
-        
+
         else:
             @wraps(func)
             async def async_wrapper(*args, **kwargs):
-                
+
                 _kwargs = await get_preprocessing_args_by_running_func(*args,**kwargs)
                 if _kwargs:
                     if not isinstance(_kwargs,dict):
                         raise Exception(f"Invalid @llm_prompt implementation: the result of the function call must be a dict, to augment the input args. Got: {_kwargs}")
                     kwargs.update(_kwargs)
-                
-                
+
                 llmChain = build_chain(*args, **kwargs)
-              
+
                 return await llmChain.aexecute()
-            
+
             async_wrapper.build_chain=build_chain
             if inspect.signature(func).parameters.get("functions"):
                 if not func.__annotations__.get('return') or func.__annotations__.get('return') == OutputWithFunctionCall  or func.__annotations__.get('return') ==  Coroutine[Any,Any,OutputWithFunctionCall]:
                     async_wrapper.__annotations__['return'] = Coroutine[Any,Any,OutputWithFunctionCall]
                 else:
                     async_wrapper.__annotations__['return'] = Coroutine[Any,Any,OutputWithFunctionCall[func.__annotations__.get('return') ]]
             return async_wrapper
     if func:
         return decorator(func)
     else:
         return decorator
-
```

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.5.5/src/langchain_decorators/prompt_template.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/pydantic_helpers.py` & `langchain-decorators-0.5.5/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/schema.py` & `langchain-decorators-0.5.5/src/langchain_decorators/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.5.5/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.5.5/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.4
+Version: 0.5.5
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.5.4/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.5.5/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

