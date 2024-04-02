# Comparing `tmp/spchat-0.1.2.tar.gz` & `tmp/spchat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spchat-0.1.2.tar", last modified: Wed Mar 13 04:23:14 2024, max compression
+gzip compressed data, was "spchat-0.2.0.tar", last modified: Tue Apr  2 01:32:00 2024, max compression
```

## Comparing `spchat-0.1.2.tar` & `spchat-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,33 @@
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-13 04:23:14.225859 spchat-0.1.2/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      831 2024-03-13 04:23:14.225859 spchat-0.1.2/PKG-INFO
--rwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)      182 2024-03-13 04:10:49.000000 spchat-0.1.2/README.md
--rwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)      848 2024-03-13 04:23:06.000000 spchat-0.1.2/pyproject.toml
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       38 2024-03-13 04:23:14.225859 spchat-0.1.2/setup.cfg
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-13 04:23:14.221860 spchat-0.1.2/spchat/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      361 2024-03-12 14:00:05.000000 spchat-0.1.2/spchat/__init__.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)    22420 2024-03-13 00:06:54.000000 spchat-0.1.2/spchat/core.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-10 03:21:51.000000 spchat-0.1.2/spchat/filters.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     7470 2024-03-12 23:59:30.000000 spchat-0.1.2/spchat/prompts.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     4288 2024-03-12 14:00:05.000000 spchat-0.1.2/spchat/retrievers.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     6077 2024-03-12 14:00:05.000000 spchat-0.1.2/spchat/utils.py
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-13 04:23:14.221860 spchat-0.1.2/spchat.egg-info/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      831 2024-03-13 04:23:14.000000 spchat-0.1.2/spchat.egg-info/PKG-INFO
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      299 2024-03-13 04:23:14.000000 spchat-0.1.2/spchat.egg-info/SOURCES.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        1 2024-03-13 04:23:14.000000 spchat-0.1.2/spchat.egg-info/dependency_links.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       97 2024-03-13 04:23:14.000000 spchat-0.1.2/spchat.egg-info/requires.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       12 2024-03-13 04:23:14.000000 spchat-0.1.2/spchat.egg-info/top_level.txt
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-13 04:23:14.221860 spchat-0.1.2/tests/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     1491 2024-03-12 14:00:05.000000 spchat-0.1.2/tests/test_chat.py
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.636650 spchat-0.2.0/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     3635 2024-04-02 01:32:00.636650 spchat-0.2.0/PKG-INFO
+-rwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)     3140 2024-03-26 12:06:45.000000 spchat-0.2.0/README.md
+-rwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)      679 2024-04-02 01:31:36.000000 spchat-0.2.0/pyproject.toml
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       38 2024-04-02 01:32:00.636650 spchat-0.2.0/setup.cfg
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.624650 spchat-0.2.0/spchat/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      469 2024-03-26 05:42:13.000000 spchat-0.2.0/spchat/__init__.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)    13914 2024-04-01 08:19:08.000000 spchat-0.2.0/spchat/avatars.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)    24099 2024-03-27 04:27:25.000000 spchat-0.2.0/spchat/chat.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-10 03:21:51.000000 spchat-0.2.0/spchat/filters.py
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.628650 spchat-0.2.0/spchat/gradio/
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.628650 spchat-0.2.0/spchat/gradio/common/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)    10045 2024-03-23 10:11:01.000000 spchat-0.2.0/spchat/gradio/common/anonymous.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)    13327 2024-03-26 05:49:17.000000 spchat-0.2.0/spchat/gradio/components.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     3265 2024-03-26 05:49:16.000000 spchat-0.2.0/spchat/gradio/models.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     7296 2024-03-13 12:47:23.000000 spchat-0.2.0/spchat/prompts.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     4284 2024-03-25 03:13:01.000000 spchat-0.2.0/spchat/retrievers.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     7158 2024-04-01 11:46:40.000000 spchat-0.2.0/spchat/session.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        0 2024-03-29 04:08:38.000000 spchat-0.2.0/spchat/stage.py
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.632650 spchat-0.2.0/spchat/templates/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     1381 2024-03-26 05:49:16.000000 spchat-0.2.0/spchat/templates/__init__.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      464 2024-03-19 10:12:58.000000 spchat-0.2.0/spchat/templates/ca.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)    15324 2024-03-19 09:54:45.000000 spchat-0.2.0/spchat/templates/stability.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     2794 2024-03-19 09:55:31.000000 spchat-0.2.0/spchat/templates/unique.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     6206 2024-03-21 04:54:36.000000 spchat-0.2.0/spchat/utils.py
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.632650 spchat-0.2.0/spchat.egg-info/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     3635 2024-04-02 01:32:00.000000 spchat-0.2.0/spchat.egg-info/PKG-INFO
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      546 2024-04-02 01:32:00.000000 spchat-0.2.0/spchat.egg-info/SOURCES.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        1 2024-04-02 01:32:00.000000 spchat-0.2.0/spchat.egg-info/dependency_links.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       67 2024-04-02 01:32:00.000000 spchat-0.2.0/spchat.egg-info/requires.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        7 2024-04-02 01:32:00.000000 spchat-0.2.0/spchat.egg-info/top_level.txt
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:32:00.632650 spchat-0.2.0/tests/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     1491 2024-03-14 02:05:35.000000 spchat-0.2.0/tests/test_chat.py
```

### Comparing `spchat-0.1.2/pyproject.toml` & `spchat-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,39 +13,30 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "chromadb",
     "loguru",
     "openai",
-    "pandas"
+    "pandas",
 ]
-version = "0.1.2"
+version = "0.2.0"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
-    "flake8",
-    "mypy",
-    "black",
-    "isort",
-    "jupyterlab",
+    "ruff",
 ]
 
 gpu = [
     "flash-attn",
 ]
 
 [tool.setuptools.packages.find]
-exclude = ["tests", "expriments", "train_model", "playground", "lm-evaluation-harness"]
+exclude = ["tests", "dist"]
 
-[tool.black]
+[tool.ruff]
 line-length = 88
+indent-width = 4
 
-[tool.isort]
-profile = "black"
-
-[tool.flake8]
-max-line-length = 88
-
-[tool.mypy]
-ignore_missing_imports = true
+[tool.ruff.format]
+quote-style = "double"
```

### Comparing `spchat-0.1.2/spchat/core.py` & `spchat-0.2.0/spchat/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 
 from spchat.prompts import ChatTemplate, get_template
 
 SPEAKERS = ["assistant", "user"]
 
 
 @dataclass
+class Speaker:
+    name: str
+    id: str
+
+    def __eq__(self, other):
+        return self.id == other.id
+
+
+@dataclass
 class Utterance:
     speaker: str
     content: str
 
     def __post_init__(self):
         self._timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self._id = uuid.uuid4()
@@ -38,15 +47,15 @@
     def add(
         self,
         utterance: "Utterance",
         linebreak_op=Literal[None, "add", "remove"],
         whitespace_op=Literal[None, "add", "remove"],
     ):
         assert self.speaker == utterance.speaker, "Speakers must be the same"
-        if linebreak_op == "remove" and not whitespace_op:
+        if linebreak_op == "remove" and whitespace_op is None:
             logger.warning(
                 "'remove_line_breaks=True' and 'add_whitespace=False' can only work on the languages that don't use whitespace to separate words such as Chinese, Japanese, and Korean."
             )
         if whitespace_op == "add":
             self.content += " " + utterance.content
         elif whitespace_op == "remove":
             if self.content.endswith(" "):
@@ -66,23 +75,26 @@
         if self.speaker == "assistant":
             return template.format_assistant(self.content)
         elif self.speaker == "user":
             return template.format_user(self.content)
         else:
             return template.format_speaker(speaker=self.speaker, content=self.content)
 
+    def rename(self, new_speaker):
+        self.speaker = new_speaker
+
     def remove_line_breaks(self, no_whitespace=False):
         if no_whitespace:
             self.content = self.content.replace("\n", "")
         else:
             self.content = self.content.replace("\n", " ")
 
     @staticmethod
     def from_dict(
-        message,
+        message: dict,
         speaker_column: str = "role",
         content_column: str = "content",
         target_speaker: str | list[str] | None = None,
     ):
         if isinstance(target_speaker, list):
             if message[speaker_column] in target_speaker:
                 return Utterance(content=message[content_column], speaker="assistant")
@@ -91,32 +103,35 @@
         elif isinstance(target_speaker, str):
             if message[speaker_column] == target_speaker:
                 return Utterance(content=message[content_column], speaker="assistant")
             else:
                 return Utterance(content=message[content_column], speaker="user")
         else:
             return Utterance(
-                content=message["content"], speaker=message[speaker_column]
+                content=message[content_column], speaker=message[speaker_column]
             )
 
-    def to_dict(self):
-        return asdict(self)
+    def to_dict(self, speaker_column="speaker", content_column="content"):
+        return {speaker_column: self.speaker, content_column: self.content}
 
     def to_dialog_data_format(self):
         return {"content": self.content, "role": self.speaker}
 
     def to_mt_dialog_data_format(self):
         return {"content": self.content, "speaker": self.speaker}
 
 
 class Memory:
-    def __init__(self, history: list[Utterance] = [], id: str | None = None):
-        if history:
+    def __init__(self, history: list[Utterance] | None = None, id: str | None = None):
+        if history is None:
+            self._history = []
+        elif isinstance(history, list):
             self._history = history
-        if not id:
+
+        if id is None:
             self._id = str(uuid.uuid4())
         else:
             self._id = id
 
     def __getitem__(self, idx):
         return self._history[idx]
 
@@ -126,37 +141,46 @@
     def __repr__(self):
         return f"Memory(history={self._history}, id={self._id})"
 
     def __iter__(self):
         return iter(self._history)
 
     def add(
-        self, utterance: Utterance | str, speaker=str | None, index: int | None = None
+        self, utterance: Utterance | str, speaker: str | None, index: int | None = None
     ):
         if isinstance(utterance, str):
-            if not speaker:
+            if speaker is None:
                 raise ValueError("speaker must be provided when utterance is a string")
             utterance = Utterance(content=utterance, speaker=speaker)
         elif not isinstance(utterance, Utterance):
             raise ValueError(
                 "utterance must be a string or an Utterance instance, not "
                 + str(type(utterance))
             )
+        else:
+            if not utterance.speaker or not utterance.content:
+                logger.warning(
+                    "Utterance must have both speaker and content. Skipping adding utterance."
+                )
+                return
 
         if index is not None:
             self._history.insert(index, utterance)
         else:
             self._history.append(utterance)
 
     def pop(self, idx, inplace=True) -> Utterance | list[Utterance] | None:
         if inplace:
             return self._history.pop(idx)
         else:
             return self._history[:idx] + self._history[idx + 1 :]
 
+    def forget(self, idx_exp: int | str):
+        self._history = eval(f"self._history[{idx_exp}]")
+
     def clear(self):
         self._history = []
 
     def show(self):
         for u in self._history:
             print(f"{u.speaker}: {u.content}")
 
@@ -168,15 +192,15 @@
         self,
         inplace=True,
         whitespace_op=Literal[None, "add", "remove"],
         linebreak_op=Literal[None, "add", "remove"],
     ) -> "Memory":
         uttrs: list[Utterance] = []
         for u in self._history:
-            if not uttrs:
+            if len(uttrs) == 0:
                 uttrs.append(u)
             elif u.speaker == uttrs[-1].speaker:
                 uttrs[-1].add(
                     u,
                     whitespace_op=whitespace_op,
                     linebreak_op=linebreak_op,
                 )
@@ -237,19 +261,22 @@
                     last_uttr = self.pop(self._history.index(u))
                     return (last_uttr, self)
             raise ValueError("No user utterance found in history")
 
         else:
             return (None, self)
 
-    def to_dict(self):
-        return {
-            "id": self.id,
-            "history": [u.to_dict() for u in self.history],
-        }
+    def to_dict(self, include_id=False, history_column="messages"):
+        d = {}
+        if include_id:
+            d["id"] = self.id
+        d[history_column] = [u.to_dict() for u in self._history]
+        d["speakers"] = self.unique_speakers
+
+        return d
 
     def to_gr_history(self):
         self.consolidate()
         gr_history = []
         for u in self.history:
             if u.speaker == "assistant":
                 gr_history.append([None, u.content])
@@ -286,31 +313,39 @@
         else:
             return None
 
     @property
     def size(self) -> int:
         return len(self._history)
 
+    @property
+    def unique_speakers(self) -> list[str]:
+        return sorted(list(set([u.speaker for u in self._history])))
+
 
 class Dialog:
     def __init__(
         self,
         template: ChatTemplate | str,
         template_registry: dict[str, ChatTemplate] | None = None,
-        memory: Memory | list[Utterance] = [],
+        memory: Memory | list[Utterance] | None = None,
         **kwargs,
     ):
         self.set_template(template, template_registry, **kwargs)
 
         if isinstance(memory, list):
             self._memory = Memory(history=memory)
-        elif not isinstance(memory, Memory):
-            raise ValueError("`memory` must be one of [Memory | list[Utterance]]")
-        else:
+        elif isinstance(memory, Memory):
             self._memory = memory
+        elif memory is None:
+            self._memory = Memory()
+        else:
+            raise ValueError(
+                f"memory must be a list of Utterance instances or a Memory instance, not {type(memory)}"
+            )
 
         assert isinstance(self._memory, Memory), "memory must be a Memory instance"
 
     def __repr__(self):
         return f"Dialog(template={self.template}, memory={self.memory})"
 
     def __str__(self):
@@ -335,14 +370,19 @@
 
     def clear(self):
         self._memory.clear()
 
     def show(self):
         self._memory.show()
 
+    def rename_speaker(self, speaker: str, new_speaker: str):
+        for u in self._memory:
+            if u.speaker == speaker:
+                u.speaker = new_speaker
+
     def get_query_and_history(self):
         return self._memory.query, self.history_text_without_query
 
     def format(self, **kwargs):
         """Format the chat history to be used in a prompt template"""
 
         if "user_utterance" in self.template.input_variables:
@@ -373,18 +413,18 @@
             history = history[:-1]
         return history
 
     @classmethod
     def format_with_template(
         cls,
         memory: Memory | list[Utterance],
-        template,
-        template_registry,
-        template_kwargs={},
-        format_kwargs={},
+        template: ChatTemplate | str,
+        template_registry: dict[str, ChatTemplate] | None = None,
+        template_kwargs: dict = {},
+        format_kwargs: dict = {},
     ) -> str:
         instance = cls(
             template=template,
             template_registry=template_registry,
             memory=memory,
             **template_kwargs,
         )
@@ -393,43 +433,51 @@
 
     def consolidate(self, **kwargs):
         self.memory.consolidate(inplace=True, **kwargs)
 
     def set_template(
         self,
         template: ChatTemplate | str,
-        template_registry: dict[str, ChatTemplate] = {},
+        template_registry: dict[str, ChatTemplate] | None = None,
         **kwargs,
     ):
         self.template = get_template(template, template_registry, **kwargs)
 
     def from_list(
         self,
         messages: dict | list[list[str]],
         speaker_column: str = "role",
-        target_speaker: str | list[str] | None = None,
+        target_speaker: str | list[str] | int | None = None,
     ):
         for message in messages:
             if isinstance(message, dict):
-                self.add(
-                    Utterance.from_dict(
-                        message,
-                        speaker_column=speaker_column,
-                        target_speaker=target_speaker,
+                if not isinstance(target_speaker, int):
+                    self.add(
+                        Utterance.from_dict(
+                            message,
+                            speaker_column=speaker_column,
+                            target_speaker=target_speaker,
+                        )
                     )
-                )
+                # else:
+                #     self.add(
+                #         Utterance.from_dict(
+                #             message,
+                #         )
+                #     )
             elif isinstance(message, list):
                 self.add(
                     Utterance(
                         content=message[1],
                         speaker=(
                             "assistant" if message[0] in ["AI", "assistant"] else "user"
                         ),
                     )
                 )
+
         return self
 
     def to_dict(self):
         return self._memory.to_dict()
 
     def to_dialog_data_format(self):
         return [u.to_dialog_data_format() for u in self.history]
@@ -466,14 +514,18 @@
     def id(self):
         return self._memory.id
 
     @property
     def memory(self):
         return self._memory
 
+    @property
+    def unique_speakers(self) -> list[str]:
+        return self._memory.unique_speakers
+
 
 @dataclass
 class DialogDataFormat:
     assistant_id: str
     messages: list[dict] | Dialog
     num_assistant_utters: int
     num_user_utters: int
@@ -506,21 +558,19 @@
         if isinstance(self.messages, Dialog):
             self.messages = self.messages.to_dialog_data_format()
         if isinstance(self.query, Utterance):
             self.query = self.query.to_dialog_data_format()
         return asdict(self)
 
     @classmethod
-    def from_dict(cls, data, template_style: str, template_kwargs: dict = {}):
+    def from_dict(cls, data, template_style: str, **kwargs):
         kwargs = {}
         for k, v in data.items():
             if k == "messages" and isinstance(v, list):
-                kwargs[k] = Dialog(
-                    template_style=template_style, **template_kwargs
-                ).from_list(v)
+                kwargs[k] = Dialog(template_style=template_style, **kwargs).from_list(v)
             elif k == "query" and v:
                 kwargs[k] = Utterance.from_dict(v)
 
             elif k in DialogDataFormat.__annotations__:
                 kwargs[k] = v
             else:
                 logger.warning(f"Key {k} not found in DialogDataFormat annotations")
@@ -529,69 +579,76 @@
     @property
     def text(self) -> str:
         return self.messages.text
 
 
 @dataclass
 class MultiTurnDialogDataFormat:
-    messages: list[dict] | list[Dialog]
+    messages: list[dict] | Dialog
     speakers: list[str]
     num_messages: int
     min: int
     max: int
     note: str | None = None
     target_speaker: str | list[str] | None = None
     template: ChatTemplate | str | None = None
+    template_registry: dict[str, ChatTemplate] | None = None
     template_kwargs: dict = field(default_factory=dict)
     do_split: bool = False
 
     def __repr__(self):
         return f"MultiTurnDialogDataFormat(messages={self.messages}, speakers={self.speakers}, num_messages={self.num_messages}, min={self.min}, max={self.max}, note={self.note})"
 
     def __post_init__(self):
         if isinstance(self.messages, list):
             if self.do_split:
                 self.response = self.messages.pop(-1)
             self.messages = [
                 Dialog(
                     template=self.template,
+                    template_registry=self.template_registry,
                     **self.template_kwargs,
                 ).from_list(
                     m, speaker_column="speaker", target_speaker=self.target_speaker
                 )
                 for m in self.messages
             ]
         else:
             if self.do_split:
                 self.response = self.messages.pop(-1)
 
     def to_dict(self):
         if isinstance(self.messages, list):
-            self.messages = [m.to_mt_dialog_data_format() for m in self.messages]
+            self.messages = [m.to_dict() for m in self.messages]
         return asdict(self)
 
     @classmethod
     def from_dict(
         cls,
         data,
-        template_style: str,
+        template: ChatTemplate | str,
+        template_registry: dict[str, ChatTemplate] | None = None,
         template_kwargs: dict = {},
         target_speaker: str | list[str] | None = None,
         do_split: bool = False,
     ):
         kwargs = {}
         for k, v in data.items():
+
             if k == "messages" and isinstance(v, list):
                 kwargs[k] = Dialog(
-                    template_style=template_style, **template_kwargs
+                    template=template,
+                    template_registry=template_registry,
+                    **template_kwargs,
                 ).from_list(
                     v,
                     speaker_column="speaker",
                     target_speaker=target_speaker,
                 )
+
             elif k in MultiTurnDialogDataFormat.__annotations__:
                 kwargs[k] = v
             else:
                 logger.warning(
                     f"Key {k} not found in MultiTurnDialogDataFormat annotations"
                 )
         kwargs["do_split"] = do_split
@@ -676,18 +733,7 @@
                 user_min = min(int(user_min), len(u.content))
                 user_max = max(user_max, len(u.content))
 
         assert assistant_min != 1e5, "No assistant messages found"
         assert user_min != 1e5, "No user messages found"
 
         return assistant_min, assistant_max, user_min, user_max
-
-
-if __name__ == "__main__":
-    from datasets import load_dataset
-
-    ds = load_dataset("Spiral-AI/gpt-chat-mt", split="eval")
-    data = ds[0]
-    data = MultiTurnDialogDataFormat.from_dict(
-        data, template_style="ca_default", target_speaker="aoi____dayo"
-    )
-    print(data)
```

### Comparing `spchat-0.1.2/spchat/prompts.py` & `spchat-0.2.0/spchat/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,34 +73,30 @@
 
     def format(self, *args, **kwargs):
         return self.template.format(*args, **kwargs)
 
 
 def get_template(
     template: ChatTemplate | str,
-    template_registry: dict[str, ChatTemplate] = {},
+    template_registry: dict[str, ChatTemplate] | None = None,
     **kwargs,
 ) -> ChatTemplate:
     if isinstance(template, str):
-        if not template_registry:
+        if template_registry is None:
             raise ValueError(
                 "template_registry must be provided when template is a string"
             )
         elif template not in template_registry:
             raise ValueError(
                 f"Template {template} not found in 'template_registry'. 'template_registry' contains {list(template_registry.keys())}"
             )
         return template_registry[template](**kwargs)
-    elif isinstance(template, ChatTemplate):
-        return template
+
     else:
-        raise ValueError(
-            "template must be a string or a ChatTemplate instance, not "
-            + str(type(template))
-        )
+        return template
 
 
 class HistoryMixin(ABC):
     @abstractmethod
     def format_user(self, content: str) -> str:
         pass
```

### Comparing `spchat-0.1.2/spchat/retrievers.py` & `spchat-0.2.0/spchat/retrievers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from pathlib import Path
 
 import chromadb
 import tqdm
 from datasets import load_dataset
 from loguru import logger
-from spiralllm.utils import get_single_openai_api_key
+from spllm.utils import get_single_openai_api_key
 
 
 class FactRetriever:
     VIOLATED_NAMING_CONVENTION = "violated_chromadb_naming_convention"
 
     def __init__(
         self,
```

### Comparing `spchat-0.1.2/spchat/utils.py` & `spchat-0.2.0/spchat/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 
 import pandas as pd
 from datasets import Dataset, load_dataset
 from loguru import logger
 from tqdm import tqdm
 
-from .core import DialogDataFormat, MultiTurnDialogDataFormat
+from .chat import DialogDataFormat, MultiTurnDialogDataFormat
+from .prompts import ChatTemplate
 
 
 def get_hereafter(prompt, query, include_query=False):
     index = prompt.find(query)
 
     if index != -1:
         result_text = prompt[index:]
@@ -168,22 +169,24 @@
     prompter = template(**kwargs)
     prompt, response = prompter.format_from_dialog_data(data)
     return {"prompt": prompt + response.content}
 
 
 def to_mt_prompt(
     data,
-    template_style: str,
+    template: ChatTemplate | str,
+    template_registry: dict[str, ChatTemplate] = {},
     target_speaker: str | list[str] | None = None,
     do_split: bool = False,
     **kwargs,
 ):
     data = MultiTurnDialogDataFormat.from_dict(
         data,
-        template_style=template_style,
+        template=template,
+        template_registry=template_registry,
         target_speaker=target_speaker,
         template_kwargs=kwargs,
         do_split=do_split,
     )  # FIXME: implement format_from_mt_dialog_data
     if do_split:
         prompt, response = data.to_prompt_and_response()
         return {"prompt": prompt + response}
```

### Comparing `spchat-0.1.2/tests/test_chat.py` & `spchat-0.2.0/tests/test_chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 import pytest
 
-from spchat.core import Utterance
+from spchat.chat import Utterance
 
 
 def test_utterance_post_init():
     utterance = Utterance(content="Hello", speaker="user")
     assert isinstance(utterance.id, str)
     assert len(utterance.id) > 0  # UUIDが生成されていることを確認
     assert utterance.timestamp == datetime.now().strftime("%Y-%m-%d %H:%M:%S")
```

