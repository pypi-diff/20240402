# Comparing `tmp/musicAlgLib-1.0.3.tar.gz` & `tmp/musicAlgLib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.0.3.tar", last modified: Tue Apr  2 06:37:14 2024, max compression
+gzip compressed data, was "musicAlgLib-1.0.5.tar", last modified: Tue Apr  2 11:47:02 2024, max compression
```

## Comparing `musicAlgLib-1.0.3.tar` & `musicAlgLib-1.0.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.887330 musicAlgLib-1.0.3/
--rw-rw-rw-   0        0        0     4676 2024-04-02 06:37:14.886834 musicAlgLib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.854098 musicAlgLib-1.0.3/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.858066 musicAlgLib-1.0.3/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.858562 musicAlgLib-1.0.3/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.869474 musicAlgLib-1.0.3/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.869970 musicAlgLib-1.0.3/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.3/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.870962 musicAlgLib-1.0.3/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19032 2024-04-01 09:34:54.000000 musicAlgLib-1.0.3/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.871459 musicAlgLib-1.0.3/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.3/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.872451 musicAlgLib-1.0.3/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.873443 musicAlgLib-1.0.3/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.873938 musicAlgLib-1.0.3/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.875426 musicAlgLib-1.0.3/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.875426 musicAlgLib-1.0.3/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.3/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.877906 musicAlgLib-1.0.3/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.879395 musicAlgLib-1.0.3/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.880386 musicAlgLib-1.0.3/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.881379 musicAlgLib-1.0.3/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.3/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.3/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.881874 musicAlgLib-1.0.3/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.3/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4832 2024-04-02 06:12:21.000000 musicAlgLib-1.0.3/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    14684 2024-01-25 06:27:05.000000 musicAlgLib-1.0.3/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.882370 musicAlgLib-1.0.3/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0     9497 2024-04-02 06:37:02.000000 musicAlgLib-1.0.3/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.883859 musicAlgLib-1.0.3/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.884850 musicAlgLib-1.0.3/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.885842 musicAlgLib-1.0.3/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.3/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.886338 musicAlgLib-1.0.3/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.3/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8411 2024-01-25 08:01:25.000000 musicAlgLib-1.0.3/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:37:14.857074 musicAlgLib-1.0.3/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-02 06:37:14.000000 musicAlgLib-1.0.3/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-02 06:37:14.000000 musicAlgLib-1.0.3/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:37:14.000000 musicAlgLib-1.0.3/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-02 06:37:14.000000 musicAlgLib-1.0.3/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 06:37:14.000000 musicAlgLib-1.0.3/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 06:37:14.887330 musicAlgLib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     5840 2024-04-02 06:37:02.000000 musicAlgLib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.519126 musicAlgLib-1.0.5/
+-rw-rw-rw-   0        0        0     4676 2024-04-02 11:47:02.518630 musicAlgLib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.487878 musicAlgLib-1.0.5/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.491350 musicAlgLib-1.0.5/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.492342 musicAlgLib-1.0.5/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.503254 musicAlgLib-1.0.5/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.503750 musicAlgLib-1.0.5/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.5/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.504246 musicAlgLib-1.0.5/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19032 2024-04-01 09:34:54.000000 musicAlgLib-1.0.5/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.504742 musicAlgLib-1.0.5/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.5/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.505238 musicAlgLib-1.0.5/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.506230 musicAlgLib-1.0.5/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.506726 musicAlgLib-1.0.5/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.507222 musicAlgLib-1.0.5/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.507718 musicAlgLib-1.0.5/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.5/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.510198 musicAlgLib-1.0.5/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.511686 musicAlgLib-1.0.5/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.0.5/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.512678 musicAlgLib-1.0.5/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.513174 musicAlgLib-1.0.5/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.5/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.5/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.513670 musicAlgLib-1.0.5/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.5/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4832 2024-04-02 06:12:21.000000 musicAlgLib-1.0.5/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    14684 2024-01-25 06:27:05.000000 musicAlgLib-1.0.5/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.514166 musicAlgLib-1.0.5/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0     9497 2024-04-02 06:37:02.000000 musicAlgLib-1.0.5/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.515158 musicAlgLib-1.0.5/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.515654 musicAlgLib-1.0.5/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.516646 musicAlgLib-1.0.5/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.5/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.518134 musicAlgLib-1.0.5/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.5/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8411 2024-04-02 11:46:20.000000 musicAlgLib-1.0.5/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:02.490854 musicAlgLib-1.0.5/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-02 11:47:02.000000 musicAlgLib-1.0.5/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-02 11:47:02.000000 musicAlgLib-1.0.5/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:47:02.000000 musicAlgLib-1.0.5/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-02 11:47:02.000000 musicAlgLib-1.0.5/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 11:47:02.000000 musicAlgLib-1.0.5/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:47:02.519126 musicAlgLib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     5840 2024-04-02 11:46:56.000000 musicAlgLib-1.0.5/setup.py
```

### Comparing `musicAlgLib-1.0.3/PKG-INFO` & `musicAlgLib-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.3
+Version: 1.0.5
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.3/README.md` & `musicAlgLib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.0.5/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.0.5/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.0.5/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.0.5/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.0.5/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.0.5/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.0.5/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.0.5/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.0.5/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.0.5/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.0.5/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.0.5/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.0.5/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #                 fs, double type, emxArray_real_T *sig_out, double *delay, double
 #                 *err)
 
 # void matchsig_2(const emxArray_real_T *ref, const emxArray_real_T *sig, double
 #                 fs, double type, emxArray_real_T *sig_out, double *delay, double
 #                 *err)
 
-def match_sig(refFile=None,testFile=None,outFile=None,audioType=0):
+def match_sig(refFile=None,testFile=None,outFile=None,audioType=1):
     """
     Parameters
     ----------
     refFile
     testFile
     outFile
     audioType  0:speech,1:music
```

### Comparing `musicAlgLib-1.0.3/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.0.5/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.0.5/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/STI/sti.py` & `musicAlgLib-1.0.5/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.0.5/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/__init__.py` & `musicAlgLib-1.0.5/musicAlgLib/__init__.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/commFunction.py` & `musicAlgLib-1.0.5/musicAlgLib/commFunction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.0.5/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.0.5/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/main.py` & `musicAlgLib-1.0.5/musicAlgLib/main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.0.5/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.0.5/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.0.5/musicAlgLib/timeAligment/time_align.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         assert  caltimes > 0
         cc_list = []
         for times in range(caltimes):
             start = int(startpoint + times * frameshift * targetfs)
             srcblock = refdata[start:start + int(single_frame_size*targetfs)]
             limit = min(maxsearchlen,int(start+(single_frame_size+delaysearchRange)*targetfs))
             dstbloack = testdata[start:limit]
-            maxCoin, startPoint = get_max_cc_by_dll(srcblock, dstbloack, get_my_dll(), 3)
+            maxCoin, startPoint = get_max_cc_by_dll(srcblock, dstbloack, get_my_dll(), 1)
 
             if maxCoin > delayThreshhold:
                 cc_list.append(round((startPoint / targetfs), 8))
         if len(cc_list) == 0:
             curDealy = None
         else:
             curDealy = sum(cc_list)/len(cc_list)
@@ -221,15 +221,15 @@
     caltimes = int(caltimes)
     assert  caltimes > 0
     cc_list = []
     for times in range(caltimes):
         start = int(times * single_frame_size * targetfs)
         srcblock = refdata[start:start + single_frame_size*targetfs]
         dstbloack = testdata[start:start + (single_frame_size+delaysearchRange)*targetfs]
-        maxCoin, startPoint = get_max_cc_by_dll(srcblock, dstbloack, get_my_dll(), 3)
+        maxCoin, startPoint = get_max_cc_by_dll(srcblock, dstbloack, get_my_dll(), 1)
         print(maxCoin,startPoint)
         if maxCoin > delayThreshhold:
             cc_list.append(round((startPoint / targetfs), 8))
     print(cc_list)
     if len(cc_list) == 0:
         return  None
     else:
```

### Comparing `musicAlgLib-1.0.3/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.0.5/musicAlgLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.3
+Version: 1.0.5
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.3/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.0.5/musicAlgLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.3/setup.py` & `musicAlgLib-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.0.03',
+    version='1.0.05',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
```

