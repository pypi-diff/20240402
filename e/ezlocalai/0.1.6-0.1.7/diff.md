# Comparing `tmp/ezlocalai-0.1.6.tar.gz` & `tmp/ezlocalai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezlocalai-0.1.6.tar", last modified: Tue Mar 19 04:08:18 2024, max compression
+gzip compressed data, was "ezlocalai-0.1.7.tar", last modified: Tue Apr  2 03:25:30 2024, max compression
```

## Comparing `ezlocalai-0.1.6.tar` & `ezlocalai-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:08:18.501428 ezlocalai-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/.env
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-19 04:08:18.501428 ezlocalai-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/Pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/cuda-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/cuda.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/cuda118-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/docker-compose-cuda.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/docker-compose-vulkan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:08:18.497428 ezlocalai-0.1.6/ezlocalai/
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai/CTTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai/IMG.py
--rw-r--r--   0 runner    (1001) docker     (127)    13316 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai/LLM.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai/STT.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai/VLM.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/ezlocalai-ngrok.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:08:18.501428 ezlocalai-0.1.6/ezlocalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-19 04:08:18.000000 ezlocalai-0.1.6/ezlocalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-19 04:08:18.000000 ezlocalai-0.1.6/ezlocalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 04:08:18.000000 ezlocalai-0.1.6/ezlocalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-19 04:08:18.000000 ezlocalai-0.1.6/ezlocalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 04:08:18.000000 ezlocalai-0.1.6/ezlocalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 04:08:18.501428 ezlocalai-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-03-19 04:08:13.000000 ezlocalai-0.1.6/start.ps1
--rw-r--r--   0 runner    (1001) docker     (127)  2999694 2024-03-19 04:08:14.000000 ezlocalai-0.1.6/tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-19 04:08:14.000000 ezlocalai-0.1.6/vulkan.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/.env
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/Pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/cuda-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/cuda.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/cuda118-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/deepseek.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/deepseek.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/docker-compose-cuda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/docker-compose-vulkan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/ezlocalai/
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/CTTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/IMG.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13316 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/LLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/STT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/VLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ezlocalai-ngrok.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/ezlocalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 03:25:30.000000 ezlocalai-0.1.7/ezlocalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:25:30.796721 ezlocalai-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/start.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)  2999694 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-02 03:25:26.000000 ezlocalai-0.1.7/vulkan.Dockerfile
```

### Comparing `ezlocalai-0.1.6/Docker.md` & `ezlocalai-0.1.7/Docker.md`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/Dockerfile` & `ezlocalai-0.1.7/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -4,11 +4,16 @@
     apt-get install -y --fix-missing --no-install-recommends git build-essential gcc g++ portaudio19-dev ffmpeg libportaudio2 libasound-dev python3 python3-pip gcc wget && \
     apt-get clean && rm -rf /var/lib/apt/lists/* && \
     python3 -m pip install --upgrade pip --no-cache-dir
 WORKDIR /app
 COPY requirements.txt .
 RUN --mount=type=cache,target=/root/.cache/pip,sharing=locked \
     python3 -m pip install --no-cache-dir -r requirements.txt
+RUN git clone https://github.com/Josh-XT/DeepSeek-VL deepseek && \
+    cd deepseek && \
+    pip install --no-cache-dir -e . && \
+    cd ..
 COPY . .
 ENV HOST 0.0.0.0
 EXPOSE 8091
-ENTRYPOINT ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8091", "--workers", "1", "--proxy-headers"]
+EXPOSE 8502
+CMD streamlit run ui.py & uvicorn app:app --host 0.0.0.0 --port 8091 --workers 1 --proxy-headers
```

### Comparing `ezlocalai-0.1.6/LICENSE` & `ezlocalai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/PKG-INFO` & `ezlocalai-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: ezlocalai
-Version: 0.1.6
+Version: 0.1.7
 Summary: ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
+Requires-Dist: streamlit
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: faster-whisper==1.0.1
 Requires-Dist: pydub==0.25.1
-Requires-Dist: ffmpeg==1.4
+Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: torch==2.2.1
 Requires-Dist: torchaudio==2.2.1
 Requires-Dist: transformers==4.38.2
 Requires-Dist: TTS==0.22.0
 Requires-Dist: sounddevice==0.4.6
 Requires-Dist: pyaudio==0.2.14
 Requires-Dist: webrtcvad==2.0.10
 Requires-Dist: pyngrok==7.1.5
 Requires-Dist: accelerate==0.27.2
 Requires-Dist: python-multipart
 Requires-Dist: llama-cpp-python==0.2.55
+Requires-Dist: openai
 
 # ezlocalai
 
-[![GitHub](https://img.shields.io/badge/GitHub-Local%20LLM-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
+[![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
 
 ezlocalai is an easy set up artificial intelligence server that allows you to easily run multimodal artificial intelligence from your computer. It is designed to be as easy as possible to get started with running local models. It automatically handles downloading the model of your choice and configuring the server based on your CPU, RAM, and GPU specifications. It also includes [OpenAI Style](https://pypi.org/project/openai/) endpoints for easy integration with other applications using ezlocalai as an OpenAI API proxy with any model. Additional functionality is built in for voice cloning text to speech and a voice to text for easy voice communication as well as image generation entirely offline after the initial setup.
 
 ## Prerequisites
 
 - [Git](https://git-scm.com/downloads)
 - [PowerShell 7.X](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)
@@ -94,20 +96,45 @@
 
 Linux:
 
 ```bash
 sudo pwsh start.ps1
 ```
 
+### Deepseek VL Vision Models
+
+- <https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat> (Default)
+- <https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat>
+
+Functionality and endpoint request/response directly mimics the [OpenAI gpt-4-vision API](https://platform.openai.com/docs/guides/vision).
+
+**Only currently available with CUDA GPU.**
+
+Modify `deepseek.yml` if you want to run the 7b model instead of the 1.3b model or want to change any other settings. This also has image generation enabled by default, you can disable it by changing `IMG_ENABLED` to `false` in `deepseek.yml` to reduce video RAM usage. This configuration will fit on a ~16GB GPU.
+
+```bash
+.\deepseek.ps1
+```
+
+Linux:
+
+```bash
+sudo pwsh deepseek.ps1
+```
+
 For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb).
 
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
+## Demo UI
+
+You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
+
 ## Workflow
 
 ```mermaid
 graph TD
    A[app.py] --> B[FASTAPI]
    B --> C[Pipes]
    C --> D[LLM]
```

### Comparing `ezlocalai-0.1.6/Pipes.py` & `ezlocalai-0.1.7/Pipes.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if self.current_vlm != "":
             try:
                 self.vlm = VLM(model=self.current_vlm)
             except Exception as e:
                 logging.error(f"[VLM] Failed to load the model: {e}")
                 self.vlm = None
         if self.vlm is not None:
-            logging.info(f"[ezlocalai] Vision is enabled.")
+            logging.info(f"[ezlocalai] Vision is enabled with {self.current_vlm}.")
         self.img_enabled = os.getenv("IMG_ENABLED", "false").lower() == "true"
         self.img = None
         if self.img_enabled and img_import_success:
             logging.info(f"[IMG] Image generation is enabled.")
             SD_MODEL = os.getenv("SD_MODEL", "stabilityai/sdxl-turbo")
             logging.info(f"[IMG] sdxl-turbo model loading. Please wait...")
             try:
@@ -49,41 +49,44 @@
         logging.info(f"[CTTS] xttsv2_2.0.2 model loaded successfully.")
         self.current_stt = os.getenv("WHISPER_MODEL", "base")
         logging.info(f"[STT] {self.current_stt} model loading. Please wait...")
         self.stt = STT(model=self.current_stt)
         logging.info(f"[STT] {self.current_stt} model loaded successfully.")
         DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "phi-2-dpo")
         self.current_llm = DEFAULT_MODEL if DEFAULT_MODEL else "phi-2-dpo"
-        if self.vlm is not None:
-            self.llm = self.vlm
-        else:
-            logging.info(f"[LLM] {self.current_llm} model loading. Please wait...")
-            self.llm = LLM(model=self.current_llm)
-            if is_vision_model(self.current_llm):
-                if self.vlm is None:
-                    self.vlm = self.llm
-            logging.info(f"[LLM] {self.current_llm} model loaded successfully.")
+        # if self.vlm is not None:
+        #    self.llm = self.vlm
+        # else:
+        logging.info(f"[LLM] {self.current_llm} model loading. Please wait...")
+        self.llm = LLM(model=self.current_llm)
+        if is_vision_model(self.current_llm):
+            if self.vlm is None:
+                self.vlm = self.llm
+        logging.info(f"[LLM] {self.current_llm} model loaded successfully.")
         NGROK_TOKEN = os.environ.get("NGROK_TOKEN", "")
         if NGROK_TOKEN:
             ngrok.set_auth_token(NGROK_TOKEN)
             public_url = ngrok.connect(8091)
             logging.info(f"[ngrok] Public Tunnel: {public_url.public_url}")
             self.local_uri = public_url.public_url
         else:
             self.local_uri = os.environ.get("EZLOCALAI_URL", "http://localhost:8091")
 
     async def get_response(self, data, completion_type="chat"):
         data["local_uri"] = self.local_uri
+        images = []
         if "messages" in data:
             if isinstance(data["messages"][-1]["content"], list):
                 messages = data["messages"][-1]["content"]
                 for message in messages:
                     if "text" in message:
                         prompt = message["text"]
                 for message in messages:
+                    if "image_url" in message:
+                        images.append(message)
                     if "audio_url" in message:
                         audio_url = (
                             message["audio_url"]["url"]
                             if "url" in message["audio_url"]
                             else message["audio_url"]
                         )
                         audio_format = "wav"
@@ -114,14 +117,46 @@
                 base64_audio=base64_audio,
                 audio_format=data["audio_format"],
             )
             if completion_type == "chat":
                 data["messages"][-1]["content"] = prompt
             else:
                 data["prompt"] = prompt
+        user_message = (
+            data["messages"][-1]["content"]
+            if completion_type == "chat"
+            else data["prompt"]
+        )
+        if self.vlm and images:
+            new_messages = [
+                {
+                    "role": "user",
+                    "content": [
+                        {
+                            "type": "text",
+                            "text": "Describe each stage of this image.",
+                        },
+                    ],
+                }
+            ]
+            new_messages[0]["content"].extend(images)
+            image_description = self.vlm.chat(messages=new_messages)
+            print(
+                f"Image Description: {image_description['choices'][0]['message']['content']}"
+            )
+            prompt = (
+                f"\n\nReference the uploaded image description for any questions about the uploaded image. Act as if you can see it. Uploaded Image Description: {image_description['choices'][0]['message']['content']} {data['messages'][-1]['content'][0]['text']}"
+                if completion_type == "chat"
+                else f"\n\nReference the uploaded image description for any questions about the uploaded image. Act as if you can see it. Uploaded Image Description: {image_description['choices'][0]['message']['content']} {data['prompt']}"
+            )
+            print(f"Full Prompt: {prompt}")
+            if completion_type == "chat":
+                data["messages"][-1]["content"] = prompt
+            else:
+                data["prompt"] = prompt
         if completion_type == "chat":
             response = self.llm.chat(**data)
         else:
             response = self.llm.completion(**data)
         generated_image = None
         if "temperature" not in data:
             data["temperature"] = 0.5
@@ -129,36 +164,46 @@
             data["top_p"] = 0.9
         if self.img and img_import_success:
             user_message = (
                 data["messages"][-1]["content"]
                 if completion_type == "chat"
                 else data["prompt"]
             )
+            if isinstance(user_message, list):
+                user_message = prompt
+                for message in messages:
+                    if "image_url" in message:
+                        if "url" in message["image_url"]:
+                            if not message["image_url"]["url"].startswith("data:"):
+                                user_message += (
+                                    "Uploaded Image:"
+                                    + message["image_url"]["url"]
+                                    + "\n"
+                                )
             response_text = (
                 response["choices"][0]["text"]
                 if completion_type != "chat"
                 else response["choices"][0]["message"]["content"]
             )
-            img_gen_prompt = f"Users message: {user_message} \nAssistant response: {response_text} \n\n**The assistant is acting as sentiment analysis expert and only responds with a concise YES or NO answer on if the user would like an image as visual or a picture generated. No other explanation is needed!**\nShould an image be created to accompany the assistant response?\nAssistant: "
+            if "data:" in user_message:
+                user_message = user_message.replace(
+                    user_message.split("data:")[1].split("'")[0], ""
+                )
+            img_gen_prompt = f"Users message: {user_message} \n\n{'The user uploaded an image, one does not need generated unless the user is specifically asking.' if images else ''} **The assistant is acting as sentiment analysis expert and only responds with a concise YES or NO answer on if the user would like an image as visual or a picture generated. No other explanation is needed!**\nWould the user potentially like an image generated based on their message?\nAssistant: "
             logging.info(f"[IMG] Decision maker prompt: {img_gen_prompt}")
             create_img = self.llm.chat(
                 messages=[{"role": "system", "content": img_gen_prompt}],
                 max_tokens=10,
                 temperature=data["temperature"],
                 top_p=data["top_p"],
             )
             create_img = str(create_img["choices"][0]["message"]["content"]).lower()
             logging.info(f"[IMG] Decision maker response: {create_img}")
             if "yes" in create_img or "es," in create_img:
-                prompt = (
-                    data["messages"][-1]["content"]
-                    if completion_type == "chat"
-                    else data["prompt"]
-                )
-                img_prompt = f"**The assistant is acting as a Stable Diffusion Prompt Generator.**\n\nUsers message: {prompt} \nAssistant response: {response} \n\nImportant rules to follow:\n- Describe subjects in detail, specify image type (e.g., digital illustration), art style (e.g., steampunk), and background. Include art inspirations (e.g., Art Station, specific artists). Detail lighting, camera (type, lens, view), and render (resolution, style). The weight of a keyword can be adjusted by using the syntax (((keyword))) , put only those keyword inside ((())) which is very important because it will have more impact so anything wrong will result in unwanted picture so be careful. Realistic prompts: exclude artist, specify lens. Separate with double lines. Max 60 words, avoiding 'real' for fantastical.\n- Based on the message from the user and response of the assistant, you will need to generate one detailed stable diffusion image generation prompt based on the context of the conversation to accompany the assistant response.\n- The prompt can only be up to 60 words long, so try to be concise while using enough descriptive words to make a proper prompt.\n- Following all rules will result in a $2000 tip that you can spend on anything!\n- Must be in markdown code block to be parsed out and only provide prompt in the code block, nothing else.\nStable Diffusion Prompt Generator: "
+                img_prompt = f"**The assistant is acting as a Stable Diffusion Prompt Generator.**\n\nUsers message: {user_message} \nAssistant response: {response_text} \n\nImportant rules to follow:\n- Describe subjects in detail, specify image type (e.g., digital illustration), art style (e.g., steampunk), and background. Include art inspirations (e.g., Art Station, specific artists). Detail lighting, camera (type, lens, view), and render (resolution, style). The weight of a keyword can be adjusted by using the syntax (((keyword))) , put only those keyword inside ((())) which is very important because it will have more impact so anything wrong will result in unwanted picture so be careful. Realistic prompts: exclude artist, specify lens. Separate with double lines. Max 60 words, avoiding 'real' for fantastical.\n- Based on the message from the user and response of the assistant, you will need to generate one detailed stable diffusion image generation prompt based on the context of the conversation to accompany the assistant response.\n- The prompt can only be up to 60 words long, so try to be concise while using enough descriptive words to make a proper prompt.\n- Following all rules will result in a $2000 tip that you can spend on anything!\n- Must be in markdown code block to be parsed out and only provide prompt in the code block, nothing else.\nStable Diffusion Prompt Generator: "
                 image_generation_prompt = self.llm.chat(
                     messages=[{"role": "system", "content": img_prompt}],
                     max_tokens=100,
                     temperature=data["temperature"],
                     top_p=data["top_p"],
                 )
                 image_generation_prompt = str(
```

### Comparing `ezlocalai-0.1.6/README.md` & `ezlocalai-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ezlocalai
 
-[![GitHub](https://img.shields.io/badge/GitHub-Local%20LLM-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
+[![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
 
 ezlocalai is an easy set up artificial intelligence server that allows you to easily run multimodal artificial intelligence from your computer. It is designed to be as easy as possible to get started with running local models. It automatically handles downloading the model of your choice and configuring the server based on your CPU, RAM, and GPU specifications. It also includes [OpenAI Style](https://pypi.org/project/openai/) endpoints for easy integration with other applications using ezlocalai as an OpenAI API proxy with any model. Additional functionality is built in for voice cloning text to speech and a voice to text for easy voice communication as well as image generation entirely offline after the initial setup.
 
 ## Prerequisites
 
 - [Git](https://git-scm.com/downloads)
 - [PowerShell 7.X](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)
@@ -63,20 +63,45 @@
 
 Linux:
 
 ```bash
 sudo pwsh start.ps1
 ```
 
+### Deepseek VL Vision Models
+
+- <https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat> (Default)
+- <https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat>
+
+Functionality and endpoint request/response directly mimics the [OpenAI gpt-4-vision API](https://platform.openai.com/docs/guides/vision).
+
+**Only currently available with CUDA GPU.**
+
+Modify `deepseek.yml` if you want to run the 7b model instead of the 1.3b model or want to change any other settings. This also has image generation enabled by default, you can disable it by changing `IMG_ENABLED` to `false` in `deepseek.yml` to reduce video RAM usage. This configuration will fit on a ~16GB GPU.
+
+```bash
+.\deepseek.ps1
+```
+
+Linux:
+
+```bash
+sudo pwsh deepseek.ps1
+```
+
 For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb).
 
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
+## Demo UI
+
+You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
+
 ## Workflow
 
 ```mermaid
 graph TD
    A[app.py] --> B[FASTAPI]
    B --> C[Pipes]
    C --> D[LLM]
```

### Comparing `ezlocalai-0.1.6/app.py` & `ezlocalai-0.1.7/app.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/docker-compose-cuda.yml` & `ezlocalai-0.1.7/docker-compose-vulkan.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 version: '3.8'
 
 services:
   ezlocalai:
     build: 
       context: .
-      dockerfile: cuda.Dockerfile
+      dockerfile: vulkan.Dockerfile
     environment:
       - EZLOCALAI_URL=${EZLOCALAI_URL-http://localhost:8091}
       - EZLOCALAI_API_KEY=${EZLOCALAI_API_KEY-}
       - GPU_LAYERS=${GPU_LAYERS-0}
       - MAIN_GPU=${MAIN_GPU-0}
       - DEFAULT_MODEL=${DEFAULT_MODEL-phi-2-dpo}
       - LLM_MAX_TOKENS=${LLM_MAX_TOKENS-0}
       - WHISPER_MODEL=${WHISPER_MODEL-base.en}
       - IMG_ENABLED=${IMG_ENABLED-true}
       - SD_MODEL=${SD_MODEL}
+      - VISION_MODEL=${VISION_MODEL}
       - CUDA_DOCKER_ARCH=all
     restart: unless-stopped
     ports:
       - "8091:8091"
+      - "8502:8502"
     volumes:
       - ./models:/app/models
       - ./outputs:/app/outputs
       - ./voices:/app/voices
       - ./whispercpp:/app/whispercpp
       - ./xttsv2_2.0.2:/app/xttsv2_2.0.2
     deploy:
```

### Comparing `ezlocalai-0.1.6/docker-compose-vulkan.yml` & `ezlocalai-0.1.7/docker-compose-cuda.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 version: '3.8'
 
 services:
   ezlocalai:
     build: 
       context: .
-      dockerfile: vulkan.Dockerfile
+      dockerfile: cuda.Dockerfile
     environment:
       - EZLOCALAI_URL=${EZLOCALAI_URL-http://localhost:8091}
       - EZLOCALAI_API_KEY=${EZLOCALAI_API_KEY-}
       - GPU_LAYERS=${GPU_LAYERS-0}
       - MAIN_GPU=${MAIN_GPU-0}
       - DEFAULT_MODEL=${DEFAULT_MODEL-phi-2-dpo}
       - LLM_MAX_TOKENS=${LLM_MAX_TOKENS-0}
       - WHISPER_MODEL=${WHISPER_MODEL-base.en}
       - IMG_ENABLED=${IMG_ENABLED-true}
       - SD_MODEL=${SD_MODEL}
+      - VISION_MODEL=${VISION_MODEL}
       - CUDA_DOCKER_ARCH=all
     restart: unless-stopped
     ports:
       - "8091:8091"
+      - "8502:8502"
     volumes:
       - ./models:/app/models
       - ./outputs:/app/outputs
       - ./voices:/app/voices
       - ./whispercpp:/app/whispercpp
       - ./xttsv2_2.0.2:/app/xttsv2_2.0.2
     deploy:
```

### Comparing `ezlocalai-0.1.6/docker-compose.yml` & `ezlocalai-0.1.7/docker-compose.yml`

 * *Files 21% similar despite different names*

```diff
@@ -6,17 +6,19 @@
     environment:
       - EZLOCALAI_URL=${EZLOCALAI_URL-http://localhost:8091}
       - EZLOCALAI_API_KEY=${EZLOCALAI_API_KEY-}
       - DEFAULT_MODEL=${DEFAULT_MODEL-phi-2-dpo}
       - LLM_MAX_TOKENS=${LLM_MAX_TOKENS-0}
       - WHISPER_MODEL=${WHISPER_MODEL-base.en}
       - IMG_ENABLED=${IMG_ENABLED-false}
+      - VISION_MODEL=${VISION_MODEL}
       - SD_MODEL=${SD_MODEL}
     restart: unless-stopped
     ports:
       - "8091:8091"
+      - "8502:8502"
     volumes:
       - ./models:/app/models
       - ./outputs:/app/outputs
       - ./voices:/app/voices
       - ./whispercpp:/app/whispercpp
       - ./xttsv2_2.0.2:/app/xttsv2_2.0.2
```

### Comparing `ezlocalai-0.1.6/ezlocalai/CTTS.py` & `ezlocalai-0.1.7/ezlocalai/CTTS.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/ezlocalai/IMG.py` & `ezlocalai-0.1.7/ezlocalai/IMG.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/ezlocalai/LLM.py` & `ezlocalai-0.1.7/ezlocalai/LLM.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/ezlocalai/STT.py` & `ezlocalai-0.1.7/ezlocalai/STT.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/ezlocalai/VLM.py` & `ezlocalai-0.1.7/ezlocalai/VLM.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime
 import requests
 import torch
 import PIL.Image
 import uuid
 import tiktoken
 import os
+import base64
 
 
 def get_tokens(text: str) -> int:
     encoding = tiktoken.get_encoding("cl100k_base")
     num_tokens = len(encoding.encode(text))
     return num_tokens
 
@@ -36,66 +37,56 @@
             self.vl_chat_processor = None
             self.tokenizer = None
             self.vl_gpt = None
 
     def chat(self, messages, **kwargs):
         pil_images = []
         images = []
-        conversation = []
+        prompt = ""
         for message in messages:
             if isinstance(message["content"], str):
                 role = message["role"] if "role" in message else "User"
                 if role.lower() == "user":
-                    role = "User"
-                conversation.append(
-                    {
-                        "role": role,
-                        "content": message["content"],
-                    }
-                )
+                    prompt += f"{message['content']}\n\n"
+                if role.lower() == "system":
+                    prompt = f"System: {message['content']}\n\nUser: {prompt}"
             if isinstance(message["content"], list):
                 for msg in message["content"]:
                     if "text" in msg:
                         role = message["role"] if "role" in message else "User"
                         if role.lower() == "user":
-                            role = "User"
-                        conversation.append(
-                            {
-                                "role": role,
-                                "content": "<image_placeholder>" + msg["text"],
-                            }
-                        )
+                            prompt += f"{msg['text']}\n\n"
                     if "image_url" in msg:
                         url = (
                             msg["image_url"]["url"]
                             if "url" in msg["image_url"]
                             else msg["image_url"]
                         )
                         image_path = f"./outputs/{uuid.uuid4().hex}.jpg"
                         if url.startswith("http"):
                             image = requests.get(url).content
-                            with open(image_path, "wb") as f:
-                                f.write(image)
-                            images.append(image_path)
                         else:
-                            with open(image_path, "wb") as f:
-                                f.write(url)
-                            images.append(image_path)
+                            file_type = url.split(",")[0].split("/")[1].split(";")[0]
+                            if file_type == "jpeg":
+                                file_type = "jpg"
+                            image_path = f"./outputs/{uuid.uuid4().hex}.{file_type}"
+                            image = base64.b64decode(url.split(",")[1])
+                        with open(image_path, "wb") as f:
+                            f.write(image)
+                        images.append(image_path)
                         pil_img = PIL.Image.open(image_path)
                         pil_img = pil_img.convert("RGB")
                         pil_images.append(pil_img)
-        if conversation == []:
-            conversation.append(
-                {
-                    "role": "User",
-                    "content": messages[0]["content"],
-                }
-            )
-        conversation[0]["images"] = images
-        conversation.append({"role": "Assistant", "content": ""})
+        if len(images) > 0:
+            for image in images:
+                prompt = f"<image_placeholder> {prompt}"
+        conversation = [
+            {"role": "User", "content": prompt, "images": images},
+            {"role": "Assistant", "content": ""},
+        ]
         prepare_inputs = self.vl_chat_processor(
             conversations=conversation, images=pil_images, force_batchify=True
         ).to(self.vl_gpt.device)
         inputs_embeds = self.vl_gpt.prepare_inputs_embeds(**prepare_inputs)
         outputs = self.vl_gpt.language_model.generate(
             inputs_embeds=inputs_embeds,
             attention_mask=prepare_inputs.attention_mask,
```

### Comparing `ezlocalai-0.1.6/ezlocalai-ngrok.ipynb` & `ezlocalai-0.1.7/ezlocalai-ngrok.ipynb`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/ezlocalai.egg-info/PKG-INFO` & `ezlocalai-0.1.7/ezlocalai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: ezlocalai
-Version: 0.1.6
+Version: 0.1.7
 Summary: ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
+Requires-Dist: streamlit
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: faster-whisper==1.0.1
 Requires-Dist: pydub==0.25.1
-Requires-Dist: ffmpeg==1.4
+Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: torch==2.2.1
 Requires-Dist: torchaudio==2.2.1
 Requires-Dist: transformers==4.38.2
 Requires-Dist: TTS==0.22.0
 Requires-Dist: sounddevice==0.4.6
 Requires-Dist: pyaudio==0.2.14
 Requires-Dist: webrtcvad==2.0.10
 Requires-Dist: pyngrok==7.1.5
 Requires-Dist: accelerate==0.27.2
 Requires-Dist: python-multipart
 Requires-Dist: llama-cpp-python==0.2.55
+Requires-Dist: openai
 
 # ezlocalai
 
-[![GitHub](https://img.shields.io/badge/GitHub-Local%20LLM-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
+[![GitHub](https://img.shields.io/badge/GitHub-ezLocalai-blue?logo=github&style=plastic)](https://github.com/DevXT-LLC/ezlocalai) [![Dockerhub](https://img.shields.io/badge/Docker-ezlocalai-blue?logo=docker&style=plastic)](https://hub.docker.com/r/joshxt/ezlocalai)
 
 ezlocalai is an easy set up artificial intelligence server that allows you to easily run multimodal artificial intelligence from your computer. It is designed to be as easy as possible to get started with running local models. It automatically handles downloading the model of your choice and configuring the server based on your CPU, RAM, and GPU specifications. It also includes [OpenAI Style](https://pypi.org/project/openai/) endpoints for easy integration with other applications using ezlocalai as an OpenAI API proxy with any model. Additional functionality is built in for voice cloning text to speech and a voice to text for easy voice communication as well as image generation entirely offline after the initial setup.
 
 ## Prerequisites
 
 - [Git](https://git-scm.com/downloads)
 - [PowerShell 7.X](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)
@@ -94,20 +96,45 @@
 
 Linux:
 
 ```bash
 sudo pwsh start.ps1
 ```
 
+### Deepseek VL Vision Models
+
+- <https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat> (Default)
+- <https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat>
+
+Functionality and endpoint request/response directly mimics the [OpenAI gpt-4-vision API](https://platform.openai.com/docs/guides/vision).
+
+**Only currently available with CUDA GPU.**
+
+Modify `deepseek.yml` if you want to run the 7b model instead of the 1.3b model or want to change any other settings. This also has image generation enabled by default, you can disable it by changing `IMG_ENABLED` to `false` in `deepseek.yml` to reduce video RAM usage. This configuration will fit on a ~16GB GPU.
+
+```bash
+.\deepseek.ps1
+```
+
+Linux:
+
+```bash
+sudo pwsh deepseek.ps1
+```
+
 For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb).
 
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
+## Demo UI
+
+You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
+
 ## Workflow
 
 ```mermaid
 graph TD
    A[app.py] --> B[FASTAPI]
    B --> C[Pipes]
    C --> D[LLM]
```

### Comparing `ezlocalai-0.1.6/ezlocalai.egg-info/SOURCES.txt` & `ezlocalai-0.1.7/ezlocalai.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 MANIFEST.in
 Pipes.py
 README.md
 app.py
 cuda-requirements.txt
 cuda.Dockerfile
 cuda118-requirements.txt
+deepseek.ps1
+deepseek.yml
 docker-compose-cuda.yml
 docker-compose-vulkan.yml
 docker-compose.yml
 ezlocalai-ngrok.ipynb
 pyproject.toml
 requirements.txt
 setup.py
 start.ps1
 tests.ipynb
+ui.py
 vulkan.Dockerfile
 ezlocalai/CTTS.py
 ezlocalai/IMG.py
 ezlocalai/LLM.py
 ezlocalai/STT.py
 ezlocalai/VLM.py
 ezlocalai/__init__.py
```

### Comparing `ezlocalai-0.1.6/setup.py` & `ezlocalai-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ezlocalai",
-    version="0.1.6",
+    version="0.1.7",
     description="ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

### Comparing `ezlocalai-0.1.6/start.ps1` & `ezlocalai-0.1.7/start.ps1`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/tests.ipynb` & `ezlocalai-0.1.7/tests.ipynb`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.6/vulkan.Dockerfile` & `ezlocalai-0.1.7/vulkan.Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -8,13 +8,18 @@
     mkdir -p /etc/OpenCL/vendors && echo "libnvidia-opencl.so.1" > /etc/OpenCL/vendors/nvidia.icd && \
     apt-get clean && rm -rf /var/lib/apt/lists/* && \
     ln -s /usr/bin/python3 /usr/bin/python
 WORKDIR /app
 ENV HOST=0.0.0.0 \
     CUDA_DOCKER_ARCH=all \
     LLAMA_CUBLAS=1
-COPY . .
 RUN python3 -m pip install --upgrade pip cmake scikit-build setuptools wheel --no-cache-dir && \
     CMAKE_ARGS="-DLLAMA_VULKAN=1" FORCE_CMAKE=1 pip install llama-cpp-python --no-cache-dir && \
     pip install --no-cache-dir -r cuda-requirements.txt
+RUN git clone https://github.com/Josh-XT/DeepSeek-VL deepseek && \
+    cd deepseek && \
+    pip install --no-cache-dir -e . && \
+    cd ..
+COPY . .
 EXPOSE 8091
-ENTRYPOINT ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8091", "--workers", "1", "--proxy-headers"]
+EXPOSE 8502
+CMD streamlit run ui.py & uvicorn app:app --host 0.0.0.0 --port 8091 --workers 1 --proxy-headers
```

