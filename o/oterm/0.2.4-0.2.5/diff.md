# Comparing `tmp/oterm-0.2.4.tar.gz` & `tmp/oterm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oterm-0.2.4.tar", max compression
+gzip compressed data, was "oterm-0.2.5.tar", max compression
```

## Comparing `oterm-0.2.4.tar` & `oterm-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1064 2024-03-19 10:20:16.834356 oterm-0.2.4/LICENSE
--rw-r--r--   0        0        0     3303 2024-03-19 10:20:16.834356 oterm-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/__init__.py
--rw-r--r--   0        0        0     7129 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/chat_edit.py
--rw-r--r--   0        0        0     1593 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/chat_export.py
--rw-r--r--   0        0        0      734 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/chat_rename.py
--rw-r--r--   0        0        0     2313 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/image_browser.py
--rw-r--r--   0        0        0     3238 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/oterm.py
--rw-r--r--   0        0        0     3239 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/oterm.tcss
--rw-r--r--   0        0        0     1058 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/prompt_history.py
--rw-r--r--   0        0        0     1947 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/splash.py
--rw-r--r--   0        0        0        0 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/widgets/__init__.py
--rw-r--r--   0        0        0     9680 2024-03-19 10:20:16.834356 oterm-0.2.4/oterm/app/widgets/chat.py
--rw-r--r--   0        0        0     1823 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/app/widgets/image.py
--rw-r--r--   0        0        0     5569 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/app/widgets/prompt.py
--rw-r--r--   0        0        0      879 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/app/widgets/text_area.py
--rw-r--r--   0        0        0        0 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/cli/__init__.py
--rw-r--r--   0        0        0      724 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/cli/oterm.py
--rw-r--r--   0        0        0     3135 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/config.py
--rw-r--r--   0        0        0     1651 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/ollama.py
--rw-r--r--   0        0        0        0 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/__init__.py
--rw-r--r--   0        0        0      892 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/chat.py
--rw-r--r--   0        0        0      572 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/setup.py
--rw-r--r--   0        0        0     5769 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/store.py
--rw-r--r--   0        0        0      359 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/upgrades/__init__.py
--rw-r--r--   0        0        0      574 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/upgrades/v0_1_11.py
--rw-r--r--   0        0        0      514 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/upgrades/v0_1_6.py
--rw-r--r--   0        0        0      522 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/upgrades/v0_2_0.py
--rw-r--r--   0        0        0      533 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/store/upgrades/v0_2_4.py
--rw-r--r--   0        0        0     1408 2024-03-19 10:20:16.838356 oterm-0.2.4/oterm/utils.py
--rw-r--r--   0        0        0     2040 2024-03-19 10:20:16.838356 oterm-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 oterm-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 09:23:57.938553 oterm-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3802 2024-04-02 09:23:57.938553 oterm-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/__init__.py
+-rw-r--r--   0        0        0     7129 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/chat_edit.py
+-rw-r--r--   0        0        0     1593 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/chat_export.py
+-rw-r--r--   0        0        0      734 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/chat_rename.py
+-rw-r--r--   0        0        0     2313 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/image_browser.py
+-rw-r--r--   0        0        0     3238 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/oterm.py
+-rw-r--r--   0        0        0     3239 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/oterm.tcss
+-rw-r--r--   0        0        0     1058 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/prompt_history.py
+-rw-r--r--   0        0        0     1947 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/splash.py
+-rw-r--r--   0        0        0       46 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/__init__.py
+-rw-r--r--   0        0        0     9680 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/chat.py
+-rw-r--r--   0        0        0     1823 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/image.py
+-rw-r--r--   0        0        0      627 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/monkey.py
+-rw-r--r--   0        0        0     5569 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/prompt.py
+-rw-r--r--   0        0        0      879 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/text_area.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/cli/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/cli/oterm.py
+-rw-r--r--   0        0        0     3135 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/config.py
+-rw-r--r--   0        0        0     1651 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/ollama.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/store/__init__.py
+-rw-r--r--   0        0        0      892 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/chat.py
+-rw-r--r--   0        0        0      572 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/setup.py
+-rw-r--r--   0        0        0     5769 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/store.py
+-rw-r--r--   0        0        0      359 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_1_11.py
+-rw-r--r--   0        0        0      514 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_1_6.py
+-rw-r--r--   0        0        0      522 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_2_0.py
+-rw-r--r--   0        0        0      533 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_2_4.py
+-rw-r--r--   0        0        0     1408 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/utils.py
+-rw-r--r--   0        0        0     2040 2024-04-02 09:23:57.942553 oterm-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 oterm-0.2.5/PKG-INFO
```

### Comparing `oterm-0.2.4/LICENSE` & `oterm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/README.md` & `oterm-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,27 @@
 * <kbd>^ Ctrl</kbd>+<kbd>P</kbd> - select an image to include with the next message
 * <kbd>↑</kbd>     - navigate through history of previous prompts
 
 While Ollama is inferring the next message, you can press <kbd>Esc</kbd> to cancel the inference.
 
 Note that some of the shortcuts may not work in a certain context, for example pressing <kbd>↑</kbd> while the prompt is in multi-line mode.
 
+### Copy / Paste
+
+It is difficult to properly support copy/paste in terminal applications. You can copy blocks to your clipboard as such:
+
+* clicking a message will copy it to the clipboard.
+* clicking a code block will only copy the code block to the clipboard.
+
+For most terminals there exists a key modifier you can use to click and drag to manually select text. For example:
+* `iTerm`  <kbd>Option</kbd> key.
+* `Gnome Terminal` <kbd>Shift</kbd> key.
+* `Windows Terminal` <kbd>Shift</kbd> key.
+
+
 ### Customizing models
 
 When creating a new chat, you may not only select the model, but also customize the `template` as well as the `system` instruction to pass to the model. Checking the `JSON output` checkbox will cause the model reply in JSON format. Please note that `oterm` will not (yet) pull models for you, use `ollama` to do that. All the models you have pulled or created will be available to `oterm`.
 
 You can also "edit" the chat to change the template, system prompt or format. Note, that the model cannot be changed once the chat has started. In addition whatever "context" the chat had (an embedding of the previous messages) will be kept.
 
 ### Chat session storage
```

### Comparing `oterm-0.2.4/oterm/app/chat_edit.py` & `oterm-0.2.5/oterm/app/chat_edit.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/chat_export.py` & `oterm-0.2.5/oterm/app/chat_export.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/chat_rename.py` & `oterm-0.2.5/oterm/app/chat_rename.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/image_browser.py` & `oterm-0.2.5/oterm/app/image_browser.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/oterm.py` & `oterm-0.2.5/oterm/app/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/oterm.tcss` & `oterm-0.2.5/oterm/app/oterm.tcss`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/prompt_history.py` & `oterm-0.2.5/oterm/app/prompt_history.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/splash.py` & `oterm-0.2.5/oterm/app/splash.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/widgets/chat.py` & `oterm-0.2.5/oterm/app/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/widgets/image.py` & `oterm-0.2.5/oterm/app/widgets/image.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/widgets/prompt.py` & `oterm-0.2.5/oterm/app/widgets/prompt.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/app/widgets/text_area.py` & `oterm-0.2.5/oterm/app/widgets/text_area.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/cli/oterm.py` & `oterm-0.2.5/oterm/cli/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/config.py` & `oterm-0.2.5/oterm/config.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/ollama.py` & `oterm-0.2.5/oterm/ollama.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/chat.py` & `oterm-0.2.5/oterm/store/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/setup.py` & `oterm-0.2.5/oterm/store/setup.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/store.py` & `oterm-0.2.5/oterm/store/store.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/upgrades/v0_1_11.py` & `oterm-0.2.5/oterm/store/upgrades/v0_1_11.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/upgrades/v0_1_6.py` & `oterm-0.2.5/oterm/store/upgrades/v0_1_6.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/upgrades/v0_2_0.py` & `oterm-0.2.5/oterm/store/upgrades/v0_2_0.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/store/upgrades/v0_2_4.py` & `oterm-0.2.5/oterm/store/upgrades/v0_2_4.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/oterm/utils.py` & `oterm-0.2.5/oterm/utils.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.4/pyproject.toml` & `oterm-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oterm"
-version = "0.2.4"
+version = "0.2.5"
 description = "A text-based terminal client for Ollama."
 authors = ["Yiorgis Gozadinos <ggozadinos@gmail.com>"]
 homepage = "https://github.com/ggozad/oterm"
 repository = "https://github.com/ggozad/oterm"
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `oterm-0.2.4/PKG-INFO` & `oterm-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oterm
-Version: 0.2.4
+Version: 0.2.5
 Summary: A text-based terminal client for Ollama.
 Home-page: https://github.com/ggozad/oterm
 License: MIT
 Author: Yiorgis Gozadinos
 Author-email: ggozadinos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,27 @@
 * <kbd>^ Ctrl</kbd>+<kbd>P</kbd> - select an image to include with the next message
 * <kbd>↑</kbd>     - navigate through history of previous prompts
 
 While Ollama is inferring the next message, you can press <kbd>Esc</kbd> to cancel the inference.
 
 Note that some of the shortcuts may not work in a certain context, for example pressing <kbd>↑</kbd> while the prompt is in multi-line mode.
 
+### Copy / Paste
+
+It is difficult to properly support copy/paste in terminal applications. You can copy blocks to your clipboard as such:
+
+* clicking a message will copy it to the clipboard.
+* clicking a code block will only copy the code block to the clipboard.
+
+For most terminals there exists a key modifier you can use to click and drag to manually select text. For example:
+* `iTerm`  <kbd>Option</kbd> key.
+* `Gnome Terminal` <kbd>Shift</kbd> key.
+* `Windows Terminal` <kbd>Shift</kbd> key.
+
+
 ### Customizing models
 
 When creating a new chat, you may not only select the model, but also customize the `template` as well as the `system` instruction to pass to the model. Checking the `JSON output` checkbox will cause the model reply in JSON format. Please note that `oterm` will not (yet) pull models for you, use `ollama` to do that. All the models you have pulled or created will be available to `oterm`.
 
 You can also "edit" the chat to change the template, system prompt or format. Note, that the model cannot be changed once the chat has started. In addition whatever "context" the chat had (an embedding of the previous messages) will be kept.
 
 ### Chat session storage
```

