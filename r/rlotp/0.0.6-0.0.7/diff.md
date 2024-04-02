# Comparing `tmp/rlotp-0.0.6.tar.gz` & `tmp/rlotp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlotp-0.0.6.tar", last modified: Sun Mar 31 16:21:48 2024, max compression
+gzip compressed data, was "rlotp-0.0.7.tar", last modified: Tue Apr  2 08:24:22 2024, max compression
```

## Comparing `rlotp-0.0.6.tar` & `rlotp-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-31 16:21:48.685723 rlotp-0.0.6/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1174 2024-03-31 05:37:56.000000 rlotp-0.0.6/LICENSE
--rw-r--r--   0 jahid     (1000) jahid     (1001)       51 2024-03-31 05:27:57.000000 rlotp-0.0.6/MANIFEST.in
--rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-03-31 16:21:48.685723 rlotp-0.0.6/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)     8535 2024-03-31 05:38:54.000000 rlotp-0.0.6/README.rst
--rw-r--r--   0 jahid     (1000) jahid     (1001)      112 2024-03-31 05:27:57.000000 rlotp-0.0.6/pyproject.toml
--rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-03-31 16:21:48.685723 rlotp-0.0.6/setup.cfg
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)     2063 2024-03-31 13:41:58.000000 rlotp-0.0.6/setup.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-31 16:21:48.682390 rlotp-0.0.6/src/
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-31 16:21:48.685723 rlotp-0.0.6/src/rlotp/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     4325 2024-03-31 16:20:49.000000 rlotp-0.0.6/src/rlotp/__init__.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      217 2024-03-31 13:41:58.000000 rlotp-0.0.6/src/rlotp/compat.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1741 2024-03-31 13:41:58.000000 rlotp-0.0.6/src/rlotp/hotp.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     3288 2024-03-31 16:13:55.000000 rlotp-0.0.6/src/rlotp/otp.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)        0 2024-03-31 13:41:58.000000 rlotp-0.0.6/src/rlotp/py.typed
--rw-r--r--   0 jahid     (1000) jahid     (1001)      122 2024-03-31 13:41:58.000000 rlotp-0.0.6/src/rlotp/steam.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     5578 2024-03-31 16:18:48.000000 rlotp-0.0.6/src/rlotp/totp.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     4102 2024-03-31 16:11:32.000000 rlotp-0.0.6/src/rlotp/utils.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-03-31 16:21:03.000000 rlotp-0.0.6/src/rlotp/version.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-31 16:21:48.685723 rlotp-0.0.6/src/rlotp.egg-info/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-03-31 16:21:48.000000 rlotp-0.0.6/src/rlotp.egg-info/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)      399 2024-03-31 16:21:48.000000 rlotp-0.0.6/src/rlotp.egg-info/SOURCES.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-03-31 16:21:48.000000 rlotp-0.0.6/src/rlotp.egg-info/dependency_links.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-03-31 16:21:48.000000 rlotp-0.0.6/src/rlotp.egg-info/not-zip-safe
--rw-r--r--   0 jahid     (1000) jahid     (1001)        6 2024-03-31 16:21:48.000000 rlotp-0.0.6/src/rlotp.egg-info/top_level.txt
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)    20364 2024-03-31 05:36:57.000000 rlotp-0.0.6/test.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.901250 rlotp-0.0.7/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1174 2024-03-31 05:37:56.000000 rlotp-0.0.7/LICENSE
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       51 2024-03-31 05:27:57.000000 rlotp-0.0.7/MANIFEST.in
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-04-02 08:24:22.901250 rlotp-0.0.7/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     8535 2024-03-31 05:38:54.000000 rlotp-0.0.7/README.rst
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      112 2024-03-31 05:27:57.000000 rlotp-0.0.7/pyproject.toml
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-04-02 08:24:22.901250 rlotp-0.0.7/setup.cfg
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)     2063 2024-03-31 13:41:58.000000 rlotp-0.0.7/setup.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.897916 rlotp-0.0.7/src/
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.901250 rlotp-0.0.7/src/rlotp/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     4338 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/__init__.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      217 2024-03-31 13:41:58.000000 rlotp-0.0.7/src/rlotp/compat.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1750 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/hotp.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     3300 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/otp.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        0 2024-03-31 13:41:58.000000 rlotp-0.0.7/src/rlotp/py.typed
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      122 2024-03-31 13:41:58.000000 rlotp-0.0.7/src/rlotp/steam.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     5579 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/totp.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     4114 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/utils.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/version.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.901250 rlotp-0.0.7/src/rlotp.egg-info/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      399 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/SOURCES.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/dependency_links.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/not-zip-safe
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        6 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/top_level.txt
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)    20360 2024-04-02 08:24:13.000000 rlotp-0.0.7/test.py
```

### Comparing `rlotp-0.0.6/LICENSE` & `rlotp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.6/PKG-INFO` & `rlotp-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlotp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Random Length OTP Library in Python
 Home-page: https://github.com/rlotp/rlotp
 Author: Md. Jahidul Hamid & PyOTP contributors
 Author-email: jahidulhamid@yahoo.com
 License: MIT License
 Project-URL: Documentation, https://neurobin.github.io/rlotp
 Project-URL: Source Code, https://github.com/neurobin/rlotp
```

### Comparing `rlotp-0.0.6/README.rst` & `rlotp-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.6/setup.py` & `rlotp-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.6/src/rlotp/__init__.py` & `rlotp-0.0.7/src/rlotp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     :returns: OTP object
     """
 
     # Secret (to be filled in later)
     secret = None
 
     # Implementation (to be filled in later)
-    impl = None
+    encoder = None
 
     # Digits (to be filled in later)
     digits = None
 
     # rdigits (to be filled in later)
     rdigits = None
 
@@ -97,28 +97,28 @@
                 otp_data["digest"] = hashlib.sha1
             elif value == "SHA256":
                 otp_data["digest"] = hashlib.sha256
             elif value == "SHA512":
                 otp_data["digest"] = hashlib.sha512
             else:
                 raise ValueError("Invalid value for algorithm, must be SHA1, SHA256 or SHA512")
-        elif key == "impl":
-            impl = value
-            otp_data["impl"] = impl
+        elif key == "encoder":
+            encoder = value
+            otp_data["encoder"] = encoder
         elif key == "digits":
             digits = int(value)
             otp_data["digits"] = digits
         elif key == "rdigits":
             rdigits = tuple(map(int, value.split("-")))
             otp_data["rdigits"] = rdigits
         elif key == "chargroup":
             chargroup = value
             otp_data["chargroup"] = chargroup
         elif key == "period":
-            otp_data["interval"] = int(value)
+            otp_data["period"] = int(value)
         elif key == "counter":
             otp_data["initial_count"] = int(value)
         elif key != "image":
             raise ValueError("{} is not a valid parameter".format(key))
 
     if not secret:
         raise ValueError("No secret found in URI")
```

### Comparing `rlotp-0.0.6/src/rlotp/hotp.py` & `rlotp-0.0.7/src/rlotp/hotp.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,26 +16,26 @@
         rdigits: Union[Tuple[int, int], None] = None,
         chargroup: str = None,
         digits: int = 6,
         digest: Any = None,
         name: Optional[str] = None,
         issuer: Optional[str] = None,
         initial_count: int = 0,
-        impl: Optional[str] = None,
+        encoder: Optional[str] = None,
     ) -> None:
         """
         :param secret: secret in base32 format
         :param initial_count: starting HMAC counter value, defaults to 0
         :param digits: number of integers in the OTP. Some apps expect this to be 6 digits, others support more.
         :param digest: digest function to use in the HMAC (expected to be SHA1)
         :param name: account name
         :param issuer: issuer
         """
         self.initial_count = initial_count
-        super().__init__(secret, rdigits=rdigits, chargroup=chargroup, digits=digits, digest=digest, name=name, issuer=issuer, impl=impl)
+        super().__init__(secret, rdigits=rdigits, chargroup=chargroup, digits=digits, digest=digest, name=name, issuer=issuer, encoder=encoder)
 
     def at(self, count: int) -> str:
         """
         Generates the OTP for the given count.
 
         :param count: the OTP HMAC counter
         :returns: OTP
```

### Comparing `rlotp-0.0.6/src/rlotp/otp.py` & `rlotp-0.0.7/src/rlotp/otp.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,25 @@
         self,
         secret: str,
         digits: int = 6,
         digest: Any = hashlib.sha1,
         chargroup: Optional[str] = None,
         name: Optional[str] = None,
         issuer: Optional[str] = None,
-        impl: Optional[str] = None,
+        encoder: Optional[str] = None,
     ) -> None:
         if digits > 10:
             raise ValueError("Maximum number of digits is 10")
         self.digits = digits
         self.digest = digest
         self.chargroup = chargroup
         self.secret = secret
         self.name = name or "Secret"
         self.issuer = issuer
-        self.impl = impl
+        self.encoder = encoder
         if self.chargroup and self.chargroup.startswith('alpha'):
             self.chargroup = string.digits + string.ascii_uppercase
         if self.chargroup and  len(self.chargroup) < self.digits:
             raise ValueError("chargroup must be at least the same length as the number of digits")
 
 
     def generate_otp(self, input: int) -> str:
@@ -53,15 +53,15 @@
         code = (
             (hmac_hash[offset] & 0x7F) << 24
             | (hmac_hash[offset + 1] & 0xFF) << 16
             | (hmac_hash[offset + 2] & 0xFF) << 8
             | (hmac_hash[offset + 3] & 0xFF)
         )
         v = ""
-        if self.impl == "steam":
+        if self.encoder == "steam":
             total_chars = len(STEAM_CHARS)
             for _ in range(STEAM_DEFAULT_DIGITS):
                 pos = code % total_chars
                 char = STEAM_CHARS[int(pos)]
                 v += char
                 code //= total_chars
         else:
```

### Comparing `rlotp-0.0.6/src/rlotp/totp.py` & `rlotp-0.0.7/src/rlotp/totp.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,66 +19,66 @@
         secret: str,
         rdigits: Union[Tuple[int, int], None] = None,
         chargroup: str = None,
         digits: int = 6,
         digest: Any = None,
         name: Optional[str] = None,
         issuer: Optional[str] = None,
-        interval: int = 30,
-        impl: Optional[str] = None,
+        period: int = 30,
+        encoder: Optional[str] = None,
     ) -> None:
         """
         :param secret: secret in base32 format
         :param digits: number of integers in the OTP. Some apps expect this to be 6 digits, others support more.
         :param digest: digest function to use in the HMAC (expected to be SHA1)
         :param name: account name
         :param issuer: issuer
-        :param interval: the time interval in seconds for OTP. This defaults to 30.
+        :param period: the time period in seconds for OTP. This defaults to 30.
         """
         self.rdigits = None
         if rdigits:
             if rdigits[0] < 6 or rdigits[1] > 10:
                 raise ValueError("rdigits must be between 6 and 10")
             self.rdigits = (rdigits[0], rdigits[1] + 1)
         if digest is None:
             digest = hashlib.sha1
 
         self.secret = secret
         self.digits = digits
         self.digest = digest
         self.name = name or 'Secret'
         self.issuer = issuer
-        self.interval = interval
+        self.period = period
         self.chargroup = chargroup
-        self.impl = impl
+        self.encoder = encoder
 
     def at(self, for_time: Union[int, datetime.datetime], counter_offset: int = 0) -> str:
         """
         Accepts either a Unix timestamp integer or a datetime object.
 
         To get the time until the next timecode change (seconds until the current OTP expires), use this instead:
 
         .. code:: python
 
             totp = rlotp.TOTP(...)
-            time_remaining = totp.interval - datetime.datetime.now().timestamp() % totp.interval
+            time_remaining = totp.period - datetime.datetime.now().timestamp() % totp.period
 
         :param for_time: the time to generate an OTP for
         :param counter_offset: the amount of ticks to add to the time counter
         :returns: OTP value
         """
         if self.rdigits:
             ns = range(*self.rdigits)
             n = len(str(len(ns)))
             otp1 = OTP(self.secret, digits=n, digest=self.digest, name=self.name, issuer=self.issuer)
             digits = utils.normalize(int(otp1.generate_otp(self.timecode(for_time) + counter_offset) if for_time else counter_offset), ns)
         else:
             digits = self.digits
 
-        otp = OTP(self.secret, digits=digits, digest=self.digest, name=self.name, issuer=self.issuer, chargroup=self.chargroup, impl=self.impl)
+        otp = OTP(self.secret, digits=digits, digest=self.digest, name=self.name, issuer=self.issuer, chargroup=self.chargroup, encoder=self.encoder)
 
         if for_time:
             if not isinstance(for_time, datetime.datetime):
                 for_time = datetime.datetime.fromtimestamp(int(for_time))
             return otp.generate_otp(self.timecode(for_time) + counter_offset)
         # else it's a HOTP, counter_offset is the counter
         return otp.generate_otp(counter_offset)
@@ -133,23 +133,23 @@
             self.secret,
             name if name else self.name,
             issuer=issuer_name if issuer_name else self.issuer,
             algorithm=self.digest().name,
             rdigits=self.rdigits,
             chargroup=self.chargroup,
             digits=self.digits,
-            period=self.interval,
+            period=self.period,
             image=image,
-            impl=self.impl,
+            encoder=self.encoder,
             initial_count=initial_count,
         )
 
     def timecode(self, for_time: datetime.datetime) -> int:
         """
         Accepts either a timezone naive (`for_time.tzinfo is None`) or
         a timezone aware datetime as argument and returns the
         corresponding counter value (timecode).
         """
         if for_time.tzinfo:
-            return int(calendar.timegm(for_time.utctimetuple()) / self.interval)
+            return int(calendar.timegm(for_time.utctimetuple()) / self.period)
         else:
-            return int(time.mktime(for_time.timetuple()) / self.interval)
+            return int(time.mktime(for_time.timetuple()) / self.period)
```

### Comparing `rlotp-0.0.6/src/rlotp/utils.py` & `rlotp-0.0.7/src/rlotp/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     issuer: Optional[str] = None,
     algorithm: Optional[str] = None,
     rdigits: Optional[Tuple[int, int]] = None,
     chargroup: Optional[str] = None,
     digits: Optional[int] = None,
     period: Optional[int] = None,
     image: Optional[str] = None,
-    impl: Optional[str] = None,
+    encoder: Optional[str] = None,
 ) -> str:
     """
     Returns the provisioning URI for the OTP; works for either TOTP or HOTP.
 
     This can then be encoded in a QR Code and used to provision the Google
     Authenticator app.
 
@@ -64,16 +64,16 @@
         url_args["counter"] = initial_count
     if is_algorithm_set:
         url_args["algorithm"] = algorithm.upper()  # type: ignore
     if rdigits:
         url_args["rdigits"] = "-".join(map(str, rdigits))
     if chargroup:
         url_args["chargroup"] = chargroup
-    if impl:
-        url_args["impl"] = impl
+    if encoder:
+        url_args["encoder"] = encoder
     if is_digits_set:
         url_args["digits"] = digits
     if is_period_set:
         url_args["period"] = period
     if image:
         image_uri = urlparse(image)
         if image_uri.scheme != "https" or not image_uri.netloc or not image_uri.path:
```

### Comparing `rlotp-0.0.6/src/rlotp.egg-info/PKG-INFO` & `rlotp-0.0.7/src/rlotp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlotp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Random Length OTP Library in Python
 Home-page: https://github.com/rlotp/rlotp
 Author: Md. Jahidul Hamid & PyOTP contributors
 Author-email: jahidulhamid@yahoo.com
 License: MIT License
 Project-URL: Documentation, https://neurobin.github.io/rlotp
 Project-URL: Source Code, https://github.com/neurobin/rlotp
```

### Comparing `rlotp-0.0.6/test.py` & `rlotp-0.0.7/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         self.assertEqual(url.scheme, "otpauth")
         self.assertEqual(url.netloc, "totp")
         self.assertEqual(url.path, "/FooCorp%21:mark%40percival")
         self.assertEqual(dict(parse_qsl(url.query)), {"secret": "wrn3pqx5uqxqvnqr", "issuer": "FooCorp!"})
         self.assertEqual(totp.provisioning_uri(), rlotp.parse_uri(totp.provisioning_uri()).provisioning_uri())
 
         key = "c7uxuqhgflpw7oruedmglbrk7u6242vb"
-        totp = rlotp.TOTP(key, digits=8, interval=60, digest=hashlib.sha256, name="baco@peperina", issuer="FooCorp")
+        totp = rlotp.TOTP(key, digits=8, period=60, digest=hashlib.sha256, name="baco@peperina", issuer="FooCorp")
         url = urlparse(totp.provisioning_uri())
         self.assertEqual(url.scheme, "otpauth")
         self.assertEqual(url.netloc, "totp")
         self.assertEqual(url.path, "/FooCorp:baco%40peperina")
         self.assertEqual(
             dict(parse_qsl(url.query)),
             {
@@ -219,15 +219,15 @@
                 "digits": "8",
                 "period": "60",
                 "algorithm": "SHA256",
             },
         )
         self.assertEqual(totp.provisioning_uri(), rlotp.parse_uri(totp.provisioning_uri()).provisioning_uri())
 
-        totp = rlotp.TOTP(key, digits=8, interval=60, name="baco@peperina", issuer="FooCorp")
+        totp = rlotp.TOTP(key, digits=8, period=60, name="baco@peperina", issuer="FooCorp")
         url = urlparse(totp.provisioning_uri())
         self.assertEqual(url.scheme, "otpauth")
         self.assertEqual(url.netloc, "totp")
         self.assertEqual(url.path, "/FooCorp:baco%40peperina")
         self.assertEqual(
             dict(parse_qsl(url.query)),
             {"secret": "c7uxuqhgflpw7oruedmglbrk7u6242vb", "issuer": "FooCorp", "digits": "8", "period": "60"},
```

