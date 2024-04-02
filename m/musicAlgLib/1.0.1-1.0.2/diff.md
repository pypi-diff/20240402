# Comparing `tmp/musicAlgLib-1.0.1.tar.gz` & `tmp/musicAlgLib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.0.1.tar", last modified: Tue Apr  2 06:17:37 2024, max compression
+gzip compressed data, was "musicAlgLib-1.0.2.tar", last modified: Tue Apr  2 06:22:49 2024, max compression
```

## Comparing `musicAlgLib-1.0.1.tar` & `musicAlgLib-1.0.2.tar`

### file list

```diff
@@ -1,79 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.250917 musicAlgLib-1.0.1/
--rw-rw-rw-   0        0        0     7736 2024-04-02 06:17:37.250917 musicAlgLib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.226117 musicAlgLib-1.0.1/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.230084 musicAlgLib-1.0.1/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.231077 musicAlgLib-1.0.1/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.231572 musicAlgLib-1.0.1/musicAlgLib/DLLs/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/DLLs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.231572 musicAlgLib-1.0.1/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.1/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.232565 musicAlgLib-1.0.1/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19032 2024-04-01 09:34:54.000000 musicAlgLib-1.0.1/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.233060 musicAlgLib-1.0.1/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.1/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.235540 musicAlgLib-1.0.1/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.236532 musicAlgLib-1.0.1/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.237524 musicAlgLib-1.0.1/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.238021 musicAlgLib-1.0.1/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.238516 musicAlgLib-1.0.1/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.1/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.240996 musicAlgLib-1.0.1/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.242484 musicAlgLib-1.0.1/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.243972 musicAlgLib-1.0.1/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.244964 musicAlgLib-1.0.1/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.1/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.1/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.245461 musicAlgLib-1.0.1/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.1/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4832 2024-04-02 06:12:21.000000 musicAlgLib-1.0.1/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    14684 2024-01-25 06:27:05.000000 musicAlgLib-1.0.1/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.246453 musicAlgLib-1.0.1/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0     9675 2024-04-02 06:12:21.000000 musicAlgLib-1.0.1/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.247940 musicAlgLib-1.0.1/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.248453 musicAlgLib-1.0.1/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.249429 musicAlgLib-1.0.1/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.1/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.250420 musicAlgLib-1.0.1/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.1/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8411 2024-01-25 08:01:25.000000 musicAlgLib-1.0.1/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:17:37.229093 musicAlgLib-1.0.1/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     7736 2024-04-02 06:17:37.000000 musicAlgLib-1.0.1/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1769 2024-04-02 06:17:37.000000 musicAlgLib-1.0.1/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:17:37.000000 musicAlgLib-1.0.1/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-02 06:17:37.000000 musicAlgLib-1.0.1/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 06:17:37.000000 musicAlgLib-1.0.1/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 06:17:37.251413 musicAlgLib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     9712 2024-04-02 06:17:28.000000 musicAlgLib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.215248 musicAlgLib-1.0.2/
+-rw-rw-rw-   0        0        0     4676 2024-04-02 06:22:49.214753 musicAlgLib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.177552 musicAlgLib-1.0.2/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.181520 musicAlgLib-1.0.2/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.182016 musicAlgLib-1.0.2/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.197392 musicAlgLib-1.0.2/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.197392 musicAlgLib-1.0.2/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.2/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.198384 musicAlgLib-1.0.2/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19032 2024-04-01 09:34:54.000000 musicAlgLib-1.0.2/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.198880 musicAlgLib-1.0.2/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.2/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.199376 musicAlgLib-1.0.2/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.200864 musicAlgLib-1.0.2/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.201360 musicAlgLib-1.0.2/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.202352 musicAlgLib-1.0.2/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.202848 musicAlgLib-1.0.2/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.2/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.204832 musicAlgLib-1.0.2/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.207313 musicAlgLib-1.0.2/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.208800 musicAlgLib-1.0.2/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.209296 musicAlgLib-1.0.2/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.2/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.2/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.209792 musicAlgLib-1.0.2/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.2/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4832 2024-04-02 06:12:21.000000 musicAlgLib-1.0.2/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    14684 2024-01-25 06:27:05.000000 musicAlgLib-1.0.2/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.210784 musicAlgLib-1.0.2/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0     9675 2024-04-02 06:12:21.000000 musicAlgLib-1.0.2/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.211280 musicAlgLib-1.0.2/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.212272 musicAlgLib-1.0.2/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.213264 musicAlgLib-1.0.2/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.2/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.213760 musicAlgLib-1.0.2/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.2/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8411 2024-01-25 08:01:25.000000 musicAlgLib-1.0.2/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:22:49.180528 musicAlgLib-1.0.2/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-02 06:22:49.000000 musicAlgLib-1.0.2/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-02 06:22:49.000000 musicAlgLib-1.0.2/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 06:22:49.000000 musicAlgLib-1.0.2/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-02 06:22:49.000000 musicAlgLib-1.0.2/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 06:22:49.000000 musicAlgLib-1.0.2/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 06:22:49.215248 musicAlgLib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     5840 2024-04-02 06:22:41.000000 musicAlgLib-1.0.2/setup.py
```

### Comparing `musicAlgLib-1.0.1/PKG-INFO` & `musicAlgLib-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -49,71 +49,40 @@
     src = "a.pcm"
     test = "b.pcm"
     cle = "c.pcm"
     tnlr,nplr,snri,dsn  = compute_audio_quality("G160",testFile=test,refFile=src,cleFile=cle,samplerate=48000)
     #p563 example
     test = "a.wav"
     Mos,SpeechLevel,Snr,NoiseLevel = compute_audio_quality('P563',testFile=test)
-    :param metrics: G160/P563/POLQA/PESQ/STOI/STI/PEAQ/SDR/SII/LOUDNESS/MUSIC/MATCH/
-                    TRANSIENT/GAINTABLE/ATTACKRELEASE/MUSICSTA/AGCDELAY/MATCHAEC/
-                    ERLE/SLIENCE/FORMAT/AECMOS/AIMOS/TRMS/ARMS/PRMS/SRMS/LRATE/NOISE/CLIP/DELAY/ECHO/SPEC/PITCH/EQ，必选项
-    # G160 无采样率限制；  WAV/PCM输入 ；三端输入: clean、ref、test；无时间长度要求；
-    # P563 8000hz(其他采样率会强制转换到8khz)；  WAV/PCM输入 ；单端输入: test；时长 < 20s；
+    :param metrics: /POLQA/PEAQ/LOUDNESS/MUSIC/MATCH/
+                    /MUSICSTA/
+                    /SLIENCE/FORMAT/TRMS/ARMS/PRMS/SRMS/CLIP/DELAY/ECHO/SPEC/PITCH/EQ，必选项
     # POLQA 窄带模式  8k  超宽带模式 48k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
-    # PESQ 窄带模式  8k   宽带模式 16k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
-    # STOI 无采样率限制; 双端输入：ref、test；无时间长度要求；
-    # STI >8k(实际会计算8khz的频谱)； WAV/PCM输入 ；双端输入：ref、test；时长 > 20s
     # PEAQ 无采样率限制；WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
-    # SDR 无采样率限制; WAV/PCM输入 ; 双端输入：ref、test；无时间长度要求；
     # MATCH 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     # MUSIC 无采样率限制;WAV/PCM输入;双端输入：ref、test；无时间长度要求；
-    # TRANSIENT 无采样率限制,WAV/PCM输入;三端输入：cle、noise、test； 无时间长度要求；
-    # GAINTABLE 无采样率限制,WAV/PCM输入;双端输入：ref、test；固定信号输入；
-    # ATTACKRELEASE 无采样率限制,WAV/PCM输入;双端输入：ref、test；固定信号输入；
     # MUSICSTA 无采样率限制,WAV/PCM输入;双端输入：ref、test；无时间长度要求；
-    # AGCDELAY 无采样率限制,WAV/PCM输入;双端输入：ref、test；无时间长度要求；
-    # MATCHAEC 无采样率限制 WAV/PCM输入;三端输入：ref、mic,test，；无时间长度要求；
-    # ELRE 无采样率限制 WAV/PCM输入;三端输入：mic,ref、test；无时间长度要求；
     # SLIENCE 无采样率限制 WAV/PCM/MP4输入;单端输入：test；无时间长度要求；
     # FORMAT 无采样率限制 WAV/MP4输入;单端输入：test；无时间长度要求；
-    # AECMOS 无采样率限制 WAV/PCM输入 ；三端输入：mic,ref、test；无时间长度要求；
-    # AIMOS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # TRMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # ARMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # PRMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # SRMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
-    # LRATE 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
-    # NOISE 无采样率限制 WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
     # CLIP 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # DELAY 无采样率限制; WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
-    # ECHO 无采样率限制; WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
     # SPEC 无采样率限制; WAV/PCM输入;单端输入：test； 无时间长度要求；
     # PITCH 无采样率限制；WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
     # EQ 无采样率限制；WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
     # MATCH2 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     # MATCH3 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     不同指标输入有不同的采样率要求，如果传入的文件不符合该指标的要求，会自动变采样到合法的区间
     :param testFile: 被测文件，必选项
     :param refFile:  参考文件，可选项，全参考指标必选，比如POLQA/PESQ/PEAQ
-    :param micFile:  micIN，可选项，回声指标必选，MATCHAEC/ELRE/AECMOS
-    :param cleFile:  干净语音文件，可选项，G160,TRANSIENT需要
-    :param noiseFile 噪声文件，可选项，突发噪声信噪比计算需要
-    :param aecCaliFile 用于做AEC对齐的校准文件  MATCHAEC专用
     :param outFile 输出文件，可选项，对齐文件可选
-    :param samplerate: 采样率，可选项，pcm文件需要 default = 16000
-    :param bitwidth: 比特位宽度，可选项，pcm文件需要 default = 2
-    :param channel: 通道数，可选项，pcm文件需要 default = 1
-    :param refOffset: ref文件的样点偏移，可选项，指标G160需要
-    :param testOffset: test文件的样点偏移，可选项，指标G160需要
-    :param maxComNLevel: 测试G160文件的最大舒适噪声
-    :param speechPauseLevel 测试G160文件的语音间歇段的噪声
     :param audioType  输入音频的模式 0：语音 1：音乐 MATCH/GAINTABLE需要
-    :param aecStartPoint  计算AECMOS，选择从第几秒开始计算
-    :param aecTargetType  0:Chiness 1:English 2:Single Digit 3:Music  计算MATCHAEC/ELRE
-    :param aecScenario 计算aec mos专用     0:'doubletalk_with_movement', 1:'doubletalk', 2:'farend_singletalk_with_movement', 3:'farend_singletalk', 4:'nearend_singletalk'
     :param rmsCalsection 计算rms的区间 TRMS和ARMS需要，时间单位s，比如：[1,20]
     :param polqaMode 计算polqa的模式 0:默认模式  1: 理想模式：排除小声音的影响，把声音校准到理想点平 -26db
     :param pitchLogMode 计算pitch的模式 0：线性模式，用于SetLocalVoicePitch接口; 1：对数模式,用于SetAudioMixingPitch接口；默认为1
     :param fineDelaySection 精准计算延时(MTACH3)，需要手动标出语音块的位置，比如有三段：speech_section=[[2.423,4.846],[5.577,7.411],[8,10.303]]
     :return:
```

### Comparing `musicAlgLib-1.0.1/README.md` & `musicAlgLib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.0.2/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.0.2/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.0.2/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.0.2/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.0.2/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.0.2/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.0.2/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.0.2/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.0.2/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.0.2/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.0.2/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.0.2/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.0.2/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.0.2/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/STI/sti.py` & `musicAlgLib-1.0.2/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.0.2/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/__init__.py` & `musicAlgLib-1.0.2/musicAlgLib/__init__.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/commFunction.py` & `musicAlgLib-1.0.2/musicAlgLib/commFunction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.0.2/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.0.2/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/main.py` & `musicAlgLib-1.0.2/musicAlgLib/main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.0.2/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.0.2/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.0.2/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.1/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.0.2/musicAlgLib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -49,71 +49,40 @@
     src = "a.pcm"
     test = "b.pcm"
     cle = "c.pcm"
     tnlr,nplr,snri,dsn  = compute_audio_quality("G160",testFile=test,refFile=src,cleFile=cle,samplerate=48000)
     #p563 example
     test = "a.wav"
     Mos,SpeechLevel,Snr,NoiseLevel = compute_audio_quality('P563',testFile=test)
-    :param metrics: G160/P563/POLQA/PESQ/STOI/STI/PEAQ/SDR/SII/LOUDNESS/MUSIC/MATCH/
-                    TRANSIENT/GAINTABLE/ATTACKRELEASE/MUSICSTA/AGCDELAY/MATCHAEC/
-                    ERLE/SLIENCE/FORMAT/AECMOS/AIMOS/TRMS/ARMS/PRMS/SRMS/LRATE/NOISE/CLIP/DELAY/ECHO/SPEC/PITCH/EQ，必选项
-    # G160 无采样率限制；  WAV/PCM输入 ；三端输入: clean、ref、test；无时间长度要求；
-    # P563 8000hz(其他采样率会强制转换到8khz)；  WAV/PCM输入 ；单端输入: test；时长 < 20s；
+    :param metrics: /POLQA/PEAQ/LOUDNESS/MUSIC/MATCH/
+                    /MUSICSTA/
+                    /SLIENCE/FORMAT/TRMS/ARMS/PRMS/SRMS/CLIP/DELAY/ECHO/SPEC/PITCH/EQ，必选项
     # POLQA 窄带模式  8k  超宽带模式 48k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
-    # PESQ 窄带模式  8k   宽带模式 16k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
-    # STOI 无采样率限制; 双端输入：ref、test；无时间长度要求；
-    # STI >8k(实际会计算8khz的频谱)； WAV/PCM输入 ；双端输入：ref、test；时长 > 20s
     # PEAQ 无采样率限制；WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
-    # SDR 无采样率限制; WAV/PCM输入 ; 双端输入：ref、test；无时间长度要求；
     # MATCH 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     # MUSIC 无采样率限制;WAV/PCM输入;双端输入：ref、test；无时间长度要求；
-    # TRANSIENT 无采样率限制,WAV/PCM输入;三端输入：cle、noise、test； 无时间长度要求；
-    # GAINTABLE 无采样率限制,WAV/PCM输入;双端输入：ref、test；固定信号输入；
-    # ATTACKRELEASE 无采样率限制,WAV/PCM输入;双端输入：ref、test；固定信号输入；
     # MUSICSTA 无采样率限制,WAV/PCM输入;双端输入：ref、test；无时间长度要求；
-    # AGCDELAY 无采样率限制,WAV/PCM输入;双端输入：ref、test；无时间长度要求；
-    # MATCHAEC 无采样率限制 WAV/PCM输入;三端输入：ref、mic,test，；无时间长度要求；
-    # ELRE 无采样率限制 WAV/PCM输入;三端输入：mic,ref、test；无时间长度要求；
     # SLIENCE 无采样率限制 WAV/PCM/MP4输入;单端输入：test；无时间长度要求；
     # FORMAT 无采样率限制 WAV/MP4输入;单端输入：test；无时间长度要求；
-    # AECMOS 无采样率限制 WAV/PCM输入 ；三端输入：mic,ref、test；无时间长度要求；
-    # AIMOS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # TRMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # ARMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # PRMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # SRMS 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
-    # LRATE 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
-    # NOISE 无采样率限制 WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
     # CLIP 无采样率限制 WAV/PCM输入 ；单端输入：test；无时间长度要求；
     # DELAY 无采样率限制; WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
-    # ECHO 无采样率限制; WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
     # SPEC 无采样率限制; WAV/PCM输入;单端输入：test； 无时间长度要求；
     # PITCH 无采样率限制；WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
     # EQ 无采样率限制；WAV/PCM输入;双端输入：ref、test； 无时间长度要求；
     # MATCH2 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     # MATCH3 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     不同指标输入有不同的采样率要求，如果传入的文件不符合该指标的要求，会自动变采样到合法的区间
     :param testFile: 被测文件，必选项
     :param refFile:  参考文件，可选项，全参考指标必选，比如POLQA/PESQ/PEAQ
-    :param micFile:  micIN，可选项，回声指标必选，MATCHAEC/ELRE/AECMOS
-    :param cleFile:  干净语音文件，可选项，G160,TRANSIENT需要
-    :param noiseFile 噪声文件，可选项，突发噪声信噪比计算需要
-    :param aecCaliFile 用于做AEC对齐的校准文件  MATCHAEC专用
     :param outFile 输出文件，可选项，对齐文件可选
-    :param samplerate: 采样率，可选项，pcm文件需要 default = 16000
-    :param bitwidth: 比特位宽度，可选项，pcm文件需要 default = 2
-    :param channel: 通道数，可选项，pcm文件需要 default = 1
-    :param refOffset: ref文件的样点偏移，可选项，指标G160需要
-    :param testOffset: test文件的样点偏移，可选项，指标G160需要
-    :param maxComNLevel: 测试G160文件的最大舒适噪声
-    :param speechPauseLevel 测试G160文件的语音间歇段的噪声
     :param audioType  输入音频的模式 0：语音 1：音乐 MATCH/GAINTABLE需要
-    :param aecStartPoint  计算AECMOS，选择从第几秒开始计算
-    :param aecTargetType  0:Chiness 1:English 2:Single Digit 3:Music  计算MATCHAEC/ELRE
-    :param aecScenario 计算aec mos专用     0:'doubletalk_with_movement', 1:'doubletalk', 2:'farend_singletalk_with_movement', 3:'farend_singletalk', 4:'nearend_singletalk'
     :param rmsCalsection 计算rms的区间 TRMS和ARMS需要，时间单位s，比如：[1,20]
     :param polqaMode 计算polqa的模式 0:默认模式  1: 理想模式：排除小声音的影响，把声音校准到理想点平 -26db
     :param pitchLogMode 计算pitch的模式 0：线性模式，用于SetLocalVoicePitch接口; 1：对数模式,用于SetAudioMixingPitch接口；默认为1
     :param fineDelaySection 精准计算延时(MTACH3)，需要手动标出语音块的位置，比如有三段：speech_section=[[2.423,4.846],[5.577,7.411],[8,10.303]]
     :return:
```

