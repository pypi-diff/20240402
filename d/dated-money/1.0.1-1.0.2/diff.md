# Comparing `tmp/dated_money-1.0.1.tar.gz` & `tmp/dated_money-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dated_money-1.0.1.tar", max compression
+gzip compressed data, was "dated_money-1.0.2.tar", max compression
```

## Comparing `dated_money-1.0.1.tar` & `dated_money-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2022-07-17 14:59:24.000000 dated_money-1.0.1/LICENSE
--rw-r--r--   0        0        0     5605 2024-03-30 19:33:35.240000 dated_money-1.0.1/README.md
--rw-r--r--   0        0        0       56 2024-03-29 18:53:32.324975 dated_money-1.0.1/dmon/__init__.py
--rw-r--r--   0        0        0     6339 2024-03-29 18:53:32.325251 dated_money-1.0.1/dmon/currency.py
--rw-r--r--   0        0        0     9361 2024-03-30 18:34:25.714178 dated_money-1.0.1/dmon/money.py
--rw-r--r--   0        0        0    14122 2024-03-30 16:54:09.158573 dated_money-1.0.1/dmon/rates.py
--rw-r--r--   0        0        0      840 2024-03-30 19:34:26.606500 dated_money-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6400 1970-01-01 00:00:00.000000 dated_money-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-07-17 14:59:24.000000 dated_money-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5605 2024-03-30 19:33:35.240000 dated_money-1.0.2/README.md
+-rw-r--r--   0        0        0       56 2024-03-29 18:53:32.324975 dated_money-1.0.2/dmon/__init__.py
+-rw-r--r--   0        0        0     7184 2024-04-01 15:17:42.301219 dated_money-1.0.2/dmon/currency.py
+-rw-r--r--   0        0        0     9361 2024-03-30 18:34:25.714178 dated_money-1.0.2/dmon/money.py
+-rw-r--r--   0        0        0    14122 2024-03-30 16:54:09.158573 dated_money-1.0.2/dmon/rates.py
+-rw-r--r--   0        0        0      840 2024-04-02 10:02:16.563222 dated_money-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6400 1970-01-01 00:00:00.000000 dated_money-1.0.2/PKG-INFO
```

### Comparing `dated_money-1.0.1/LICENSE` & `dated_money-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dated_money-1.0.1/README.md` & `dated_money-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dated_money-1.0.1/dmon/currency.py` & `dated_money-1.0.2/dmon/currency.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,24 @@
     AOA = 'aoa'
     AWG = 'awg'
     AZN = 'azn'
     BAM = 'bam'
     BBD = 'bbd'
     BDT = 'bdt'
     BGN = 'bgn'
+    BHD = 'bhd'
     BIF = 'bif'
     BMD = 'bmd'
     BND = 'bnd'
     BOB = 'bob'
     BRL = 'brl'
     BSD = 'bsd'
+    BTN = 'btn'
     BWP = 'bwp'
+    BYN = 'byn'
     BZD = 'bzd'
     CAD = 'cad'
     CDF = 'cdf'
     CHF = 'chf'
     CLP = 'clp'
     CNY = 'cny'
     COP = 'cop'
@@ -36,58 +39,66 @@
     CZK = 'czk'
     CVE = 'cve'
     DJF = 'djf'
     DKK = 'dkk'
     DOP = 'dop'
     DZD = 'dzd'
     EGP = 'egp'
+    ERN = 'ern'
     ETB = 'etb'
     EUR = 'eur'
     FJD = 'fjd'
     FKP = 'fkp'
     GBP = 'gbp'
     GEL = 'gel'
     GGP = 'ggp'
+    GHS = 'ghs'
     GIP = 'gip'
     GNF = 'gnf'
     GTQ = 'gtq'
     GYD = 'gyd'
     GMD = 'gmd'
     HKD = 'hkd'
     HNL = 'hnl'
     HRK = 'hrk'
     HTG = 'htg'
     HUF = 'huf'
     IDR = 'idr'
     ILS = 'ils'
     IMP = 'imp'
     INR = 'inr'
+    IQD = 'iqd'
     IRR = 'irr'
     ISK = 'isk'
     JEP = 'jep'
     JMD = 'jmd'
+    JOD = 'jod'
     JPY = 'jpy'
     KES = 'kes'
     KGS = 'kgs'
     KHR = 'khr'
     KMF = 'kmf'
+    KPW = 'kpw'
     KRW = 'krw'
+    KWD = 'kwd'
     KYD = 'kyd'
     KZT = 'kzt'
     LAK = 'lak'
     LBP = 'lbp'
     LKR = 'lkr'
     LRD = 'lrd'
     LSL = 'lsl'
+    LYD = 'lyd'
     MAD = 'mad'
     MDL = 'mdl'
     MGA = 'mga'
     MKD = 'mkd'
     MMK = 'mmk'
     MNT = 'mnt'
+    MRU = 'mru'
     MUR = 'mur'
     MXN = 'mxn'
     MYR = 'myr'
     MZN = 'mzn'
     MOP = 'mop'
     MVR = 'mvr'
     MWK = 'mwk'
@@ -109,45 +120,53 @@
     RON = 'ron'
     RSD = 'rsd'
     RUB = 'rub'
     RWF = 'rwf'
     SAR = 'sar'
     SBD = 'sbd'
     SCR = 'scr'
+    SDG = 'sdg'
     SEK = 'sek'
     SGD = 'sgd'
     SHP = 'shp'
+    SLE = 'sle'
     SLL = 'sll'
     SOS = 'sos'
     SRD = 'srd'
+    SSP = 'ssp'
+    STD = 'std'
     SYP = 'syp'
     SZL = 'szl'
     THB = 'thb'
     TJS = 'tjs'
+    TMT = 'tmt'
+    TND = 'tnd'
     TOP = 'top'
     TRY = 'try'
     TTD = 'ttd'
     TVD = 'tvd'
     TWD = 'twd'
     TZS = 'tzs'
     UAH = 'uah'
     UGX = 'ugx'
     USD = 'usd'
     UYU = 'uyu'
     UZS = 'uzs'
     VEF = 'vef'
+    VES = 'ves'
     VND = 'vnd'
     VUV = 'vuv'
     WST = 'wst'
     XAF = 'xaf'
     XCD = 'xcd'
     XOF = 'xof'
     XPF = 'xpf'
     YER = 'yer'
     ZAR = 'zar'
+    ZMW = 'zmw'
 
 
 CurrencySymbols = {
     Currency.AED: 'د.إ',
     Currency.AFN: '؋',
     Currency.ALL: 'Lek ',
     Currency.AMD: '֏',
@@ -157,21 +176,24 @@
     Currency.AOA: 'Kz ',
     Currency.AWG: 'ƒ',
     Currency.AZN: 'ман',
     Currency.BAM: 'KM ',
     Currency.BBD: 'BBD$',
     Currency.BDT: '৳',
     Currency.BGN: 'лв',
+    Currency.BHD: '.د.ب',
     Currency.BIF: 'FBu',
     Currency.BMD: '$',
     Currency.BND: 'B$',
     Currency.BOB: '$b',
     Currency.BRL: 'R$',
     Currency.BSD: 'B$',
+    Currency.BTN: 'Nu.',
     Currency.BWP: 'P ',
+    Currency.BYN: 'Rbl‎',
     Currency.BZD: 'BZ$',
     Currency.CAD: 'C$',
     Currency.CDF: 'FC ',
     Currency.CHF: 'CHF ',
     Currency.CLP: 'CLP',
     Currency.CNY: '¥',
     Currency.COP: 'COP',
@@ -180,58 +202,66 @@
     Currency.CZK: 'Kč',
     Currency.CVE: 'Esc ',
     Currency.DJF: 'Fdj',
     Currency.DKK: 'kr ',
     Currency.DOP: 'RD$',
     Currency.DZD: 'دج',
     Currency.EGP: 'E£',
+    Currency.ERN: 'Nkf‎',
     Currency.ETB: 'ብር',
     Currency.EUR: '€',
     Currency.FJD: 'FJ$',
     Currency.FKP: 'FK£',
     Currency.GBP: '£',
     Currency.GEL: 'ლ',
     Currency.GGP: 'G£',
+    Currency.GHS: 'GH₵',
     Currency.GIP: '£',
     Currency.GNF: 'GFr',
     Currency.GTQ: 'Q ',
     Currency.GYD: 'G$',
     Currency.GMD: 'D ',
     Currency.HKD: 'HK$',
     Currency.HNL: 'L ',
     Currency.HRK: 'kn ',
     Currency.HTG: 'G ',
     Currency.HUF: 'Ft ',
     Currency.IDR: 'Rp ',
     Currency.ILS: '₪',
     Currency.IMP: '£',
     Currency.INR: '₹',
+    Currency.IQD: 'د.ع',
     Currency.IRR: '﷼',
     Currency.ISK: 'kr ',
     Currency.JEP: '£',
     Currency.JMD: 'J$',
+    Currency.JOD: 'د.أ',
     Currency.JPY: 'JP¥',
     Currency.KES: 'Ksh ',
     Currency.KGS: 'лв',
     Currency.KHR: '៛',
     Currency.KMF: 'CF',
+    Currency.KPW: '₩',
     Currency.KRW: '₩',
+    Currency.KWD: 'د.ك',
     Currency.KYD: 'CI$',
     Currency.KZT: 'лв',
     Currency.LAK: '₭',
     Currency.LBP: 'ل.ل.',
     Currency.LKR: '₨',
     Currency.LRD: 'L$',
     Currency.LSL: 'M ',
+    Currency.LYD: 'ل.د',
     Currency.MAD: 'MAD ',
     Currency.MDL: 'L ',
     Currency.MGA: 'Ar ',
     Currency.MKD: 'ден',
     Currency.MMK: 'K',
     Currency.MNT: '₮',
+    Currency.MRU: 'UM‎',
     Currency.MUR: '₨',
     Currency.MXN: 'Mex$',
     Currency.MYR: 'RM ',
     Currency.MZN: 'MT ',
     Currency.MOP: 'MOP$',
     Currency.MVR: 'Rf. ',
     Currency.MWK: 'MK ',
@@ -253,54 +283,62 @@
     Currency.RON: 'lei ',
     Currency.RSD: 'Дин.',
     Currency.RUB: '₽',
     Currency.RWF: 'R₣',
     Currency.SAR: '﷼',
     Currency.SBD: 'SI$',
     Currency.SCR: '₨',
+    Currency.SDG: 'PT',
     Currency.SEK: 'kr ',
     Currency.SGD: 'S$',
     Currency.SHP: '£',
+    Currency.SLE: 'Le ',
     Currency.SLL: 'Le ',
     Currency.SOS: 'S ',
     Currency.SRD: 'Sr$',
+    Currency.SSP: 'SS£',
+    Currency.STD: 'Db',
     Currency.SYP: '£S',
     Currency.SZL: 'L',
     Currency.THB: '฿',
     Currency.TJS: 'SM ',
+    Currency.TMT: 'm',
+    Currency.TND: 'د.ت‎',
     Currency.TOP: 'T$',
     Currency.TRY: '₤',
     Currency.TTD: 'TT$',
     Currency.TVD: '$T',
     Currency.TWD: 'NT$',
     Currency.TZS: 'TSh ',
     Currency.UAH: '₴',
     Currency.UGX: 'USh ',
     Currency.USD: '$',
     Currency.UYU: '$U ',
     Currency.UZS: 'лв',
     Currency.VEF: 'Bs ',
+    Currency.VES: 'Bs. S',
     Currency.VND: '₫',
     Currency.VUV: 'VT ',
     Currency.WST: 'WS$',
     Currency.XAF: 'FCFA ',
     Currency.XCD: 'EC$',
     Currency.XOF: 'CFA ',
     Currency.XPF: '₣',
     Currency.YER: '﷼',
     Currency.ZAR: 'R ',
+    Currency.ZMW: 'ZK',
 }
 
 
-Reverse_symbols = {v: k for k, v in CurrencySymbols.items()}
+ReverseCurrencySymbols = {v: k for k, v in CurrencySymbols.items()}
 
 # These can be used in several currencies, choose one:
-Reverse_symbols['C$'] = Currency.CAD
-Reverse_symbols['A$'] = Currency.AUD
-Reverse_symbols['$'] = Currency.USD
-Reverse_symbols['£'] = Currency.GBP
+ReverseCurrencySymbols['C$'] = Currency.CAD
+ReverseCurrencySymbols['A$'] = Currency.AUD
+ReverseCurrencySymbols['$'] = Currency.USD
+ReverseCurrencySymbols['£'] = Currency.GBP
 
 
 def to_currency_enum(currency: Union[str, Currency]) -> Currency:
     if isinstance(currency, Currency):
         return currency
-    return Currency(Reverse_symbols.get(currency, currency.lower()))
+    return Currency(ReverseCurrencySymbols.get(currency, currency.lower()))
```

### Comparing `dated_money-1.0.1/dmon/money.py` & `dated_money-1.0.2/dmon/money.py`

 * *Files identical despite different names*

### Comparing `dated_money-1.0.1/dmon/rates.py` & `dated_money-1.0.2/dmon/rates.py`

 * *Files identical despite different names*

### Comparing `dated_money-1.0.1/pyproject.toml` & `dated_money-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dated-money"
-version = "1.0.1"
+version = "1.0.2"
 description = "Compute with dated monetary values."
 readme = "README.md"
 authors = ["Juan Reyero <juan@juanreyero.com>"]
 license = "MIT"
 packages = [
     { include = "dmon" }
 ]
```

### Comparing `dated_money-1.0.1/PKG-INFO` & `dated_money-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dated-money
-Version: 1.0.1
+Version: 1.0.2
 Summary: Compute with dated monetary values.
 License: MIT
 Author: Juan Reyero
 Author-email: juan@juanreyero.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

