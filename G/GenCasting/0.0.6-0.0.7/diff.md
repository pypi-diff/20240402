# Comparing `tmp/GenCasting-0.0.6.tar.gz` & `tmp/GenCasting-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenCasting-0.0.6.tar", last modified: Mon Apr  1 21:50:07 2024, max compression
+gzip compressed data, was "GenCasting-0.0.7.tar", last modified: Mon Apr  1 22:41:16 2024, max compression
```

## Comparing `GenCasting-0.0.6.tar` & `GenCasting-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.492378 GenCasting-0.0.6/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.6/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 21:50:07.492013 GenCasting-0.0.6/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.6/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 21:50:07.492510 GenCasting-0.0.6/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1159 2024-04-01 21:38:24.000000 GenCasting-0.0.6/setup.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.489155 GenCasting-0.0.6/src/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.490342 GenCasting-0.0.6/src/GenCasting/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 21:37:16.000000 GenCasting-0.0.6/src/GenCasting/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     6809 2024-04-01 21:27:06.000000 GenCasting-0.0.6/src/GenCasting/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.491677 GenCasting-0.0.6/src/GenCasting.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 21:50:07.490824 GenCasting-0.0.6/src/GenCasting.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-01 21:50:07.491070 GenCasting-0.0.6/src/GenCasting.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 21:50:07.491286 GenCasting-0.0.6/src/GenCasting.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-01 21:50:07.491506 GenCasting-0.0.6/src/GenCasting.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 21:50:07.491732 GenCasting-0.0.6/src/GenCasting.egg-info/top_level.txt
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 22:41:16.548515 GenCasting-0.0.7/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.7/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 22:41:16.548151 GenCasting-0.0.7/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.7/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 22:41:16.548650 GenCasting-0.0.7/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1159 2024-04-01 22:41:12.000000 GenCasting-0.0.7/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 22:41:16.545114 GenCasting-0.0.7/src/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 22:41:16.546336 GenCasting-0.0.7/src/GenCasting/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 21:37:16.000000 GenCasting-0.0.7/src/GenCasting/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     7959 2024-04-01 22:39:58.000000 GenCasting-0.0.7/src/GenCasting/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 22:41:16.547802 GenCasting-0.0.7/src/GenCasting.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 22:41:16.546767 GenCasting-0.0.7/src/GenCasting.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-01 22:41:16.547031 GenCasting-0.0.7/src/GenCasting.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 22:41:16.547367 GenCasting-0.0.7/src/GenCasting.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-01 22:41:16.547634 GenCasting-0.0.7/src/GenCasting.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 22:41:16.547860 GenCasting-0.0.7/src/GenCasting.egg-info/top_level.txt
```

### Comparing `GenCasting-0.0.6/PKG-INFO` & `GenCasting-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GenCasting-0.0.6/setup.py` & `GenCasting-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="GenCasting",
     version=VERSION,
```

### Comparing `GenCasting-0.0.6/src/GenCasting/logit_extraction.py` & `GenCasting-0.0.7/src/GenCasting/logit_extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,16 @@
     def __init__(self,model_name,quantization=None):
         '''
         model_name: str
         
         '''
 
         self.model_name = model_name
-        self.tokens = class_tokens
-        
         self.load_model(quantization)
-        self.token_dict = self.identify_tokens(self.tokens)
-        
+
 
     def load_model(self,quantization=None):
         if quantization == '8bit':
             load_in_8bit = True
             load_in_4bit = False
         elif quantization == '4bit':
             load_in_4bit = True
@@ -60,15 +57,15 @@
         self.model = model
         
         tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         tokenizer.padding_side = "right"
         tokenizer.pad_token = tokenizer.eos_token
         self.tokenizer = tokenizer
 
-    pass
+
     
     def identify_tokens(self,class_tokens = None):
 
         if not hasattr(self,'tokenizer'):
             raise ValueError("Model must be loaded first `load_model`.")
 
         if type(class_tokens) == dict:
@@ -109,21 +106,25 @@
 
         ds = GenerativeDataset(input_text,self.tokenizer)
         collator = DataCollatorWithPadding(self.tokenizer)
         dataloader = DataLoader(ds,batch_size=batch_size,collate_fn=collator)
         
         return dataloader
 
-    def logit_extraction(self,input_data,batch_size=None,gpu=True):
-
+    def logit_extraction(self,input_data,tokens,batch_size=None):
+        self.token_dict = self.identify_tokens(tokens)
+        
         if type(input_data) == list:
             try:
                 input_data = self.get_dataloader(input_data,batch_size=batch_size)
             except:
                 raise ValueError('Batch size must be specified if text list is provided.')
+        
+        elif type(input_data) == str:
+            input_data = self.get_dataloader([input_data],batch_size=batch_size)
 
         if torch.cuda.is_available():
             device = 'cuda'
         else:
             device = 'cpu'
 
         preds = []
@@ -131,24 +132,54 @@
         for batch in tqdm(input_data):
 
             output = self.model(
                 input_ids = batch['input_ids'].to(device),
                 attention_mask = batch['attention_mask'].to(device)
             ).logits.detach().cpu()
 
-            
-            generated = torch.vstack([output[i,batch['length'][i]-1,:] for i in range(len(batch['length']))])
+            # Extract predictions following end of prompt
+            generated = torch.vstack(
+                [output[i,batch['length'][i]-1,:] for i in range(len(batch['length']))]
+            )
             preds.append(
                 softmax(generated[:,list(self.token_dict.values())],dim=-1).numpy()
             )
 
         output_df = pd.DataFrame(np.vstack(preds),columns=list(self.token_dict.keys()))
 
         return output_df
 
+    def text_generation(self,input_data,batch_size=1,max_new_tokens=100):
+        if type(input_data) == list:
+            try:
+                input_data = self.get_dataloader(input_data,batch_size=batch_size)
+            except:
+                raise ValueError('Batch size must be specified if text list is provided.')
+        
+        elif type(input_data) == str:
+            input_data = self.get_dataloader([input_data],batch_size=batch_size)
+
+        if torch.cuda.is_available():
+            device = 'cuda'
+        else:
+            device = 'cpu'
+
+        preds = []
+        self.model.eval()
+        for batch in tqdm(input_data):
+            output = self.model.generate(
+                input_ids = batch['input_ids'].to('cuda'),
+                attention_mask = batch['attention_mask'].to('cuda'),
+                max_new_tokens = max_new_tokens
+            )
+            
+            preds.extend([output[i,batch['length'][i]:] for i in range(len(batch['length']))])
+
+        return preds
+
     def trainer_setup(
         self,
         train_ds,
         response_seq,
         text_field = "prompt",
         lora_alpha = 16,
         lora_rank=32,
```

### Comparing `GenCasting-0.0.6/src/GenCasting.egg-info/PKG-INFO` & `GenCasting-0.0.7/src/GenCasting.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

