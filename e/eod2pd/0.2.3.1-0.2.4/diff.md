# Comparing `tmp/eod2pd-0.2.3.1.tar.gz` & `tmp/eod2pd-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eod2pd-0.2.3.1.tar", last modified: Thu Mar 28 10:40:05 2024, max compression
+gzip compressed data, was "eod2pd-0.2.4.tar", last modified: Tue Apr  2 18:22:51 2024, max compression
```

## Comparing `eod2pd-0.2.3.1.tar` & `eod2pd-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-28 10:40:05.404625 eod2pd-0.2.3.1/
--rw-r--r--   0 neutro2    (501) staff       (20)     8884 2024-03-28 10:40:05.403723 eod2pd-0.2.3.1/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:52.000000 eod2pd-0.2.3.1/license
--rw-r--r--   0 neutro2    (501) staff       (20)     1044 2024-03-28 10:33:04.000000 eod2pd-0.2.3.1/pyproject.toml
--rw-r--r--   0 neutro2    (501) staff       (20)     6844 2024-03-24 19:07:03.000000 eod2pd-0.2.3.1/readme.md
--rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-03-28 10:40:05.404809 eod2pd-0.2.3.1/setup.cfg
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-28 10:40:05.396496 eod2pd-0.2.3.1/src/
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-28 10:40:05.399784 eod2pd-0.2.3.1/src/eod2pd/
--rw-r--r--   0 neutro2    (501) staff       (20)     1638 2024-03-24 18:23:55.000000 eod2pd-0.2.3.1/src/eod2pd/__init__.py
--rw-r--r--   0 neutro2    (501) staff       (20)     6179 2024-03-24 18:23:05.000000 eod2pd-0.2.3.1/src/eod2pd/downloader.py
--rw-r--r--   0 neutro2    (501) staff       (20)    20705 2024-03-28 10:35:20.000000 eod2pd-0.2.3.1/src/eod2pd/downloaderfunctions.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-28 10:40:05.402554 eod2pd-0.2.3.1/src/eod2pd.egg-info/
--rw-r--r--   0 neutro2    (501) staff       (20)     8884 2024-03-28 10:40:05.000000 eod2pd-0.2.3.1/src/eod2pd.egg-info/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)      301 2024-03-28 10:40:05.000000 eod2pd-0.2.3.1/src/eod2pd.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-03-28 10:40:05.000000 eod2pd-0.2.3.1/src/eod2pd.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2    (501) staff       (20)      114 2024-03-28 10:40:05.000000 eod2pd-0.2.3.1/src/eod2pd.egg-info/requires.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        7 2024-03-28 10:40:05.000000 eod2pd-0.2.3.1/src/eod2pd.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.132999 eod2pd-0.2.4/
+-rw-r--r--   0 neutro2    (501) staff       (20)     8882 2024-04-02 18:22:51.132477 eod2pd-0.2.4/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:52.000000 eod2pd-0.2.4/license
+-rw-r--r--   0 neutro2    (501) staff       (20)     1042 2024-03-29 15:47:09.000000 eod2pd-0.2.4/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     6844 2024-03-24 19:07:03.000000 eod2pd-0.2.4/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-02 18:22:51.133096 eod2pd-0.2.4/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.123624 eod2pd-0.2.4/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.127720 eod2pd-0.2.4/src/eod2pd/
+-rw-r--r--   0 neutro2    (501) staff       (20)     1638 2024-03-24 18:23:55.000000 eod2pd-0.2.4/src/eod2pd/__init__.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     6179 2024-03-24 18:23:05.000000 eod2pd-0.2.4/src/eod2pd/downloader.py
+-rw-r--r--   0 neutro2    (501) staff       (20)    23344 2024-03-29 13:43:53.000000 eod2pd-0.2.4/src/eod2pd/downloaderfunctions.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.131662 eod2pd-0.2.4/src/eod2pd.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     8882 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      301 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)      114 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        7 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/top_level.txt
```

### Comparing `eod2pd-0.2.3.1/PKG-INFO` & `eod2pd-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eod2pd
-Version: 0.2.3.1
+Version: 0.2.4
 Summary: a simple library to quere EODHistoricalData in a multithreaded environment
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: basefunctions>=0.3.3
+Requires-Dist: basefunctions>=0.3.7
 Requires-Dist: requests>=2.31
 Requires-Dist: pandas>=2.1
 Requires-Dist: python-decouple>=3.4
 Requires-Dist: stockstats>=0.6.2
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: pytest>=7.4; extra == "test"
```

### Comparing `eod2pd-0.2.3.1/license` & `eod2pd-0.2.4/license`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.3.1/pyproject.toml` & `eod2pd-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eod2pd"
-version = "0.2.3.1"
+version = "0.2.4"
 
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "a simple library to quere EODHistoricalData in a multithreaded environment"
 
 readme = "readme.md"
 license = { file = "license" }
 requires-python = ">=3.10"
@@ -18,15 +18,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
-  "basefunctions >= 0.3.3",
+  "basefunctions >= 0.3.7",
   "requests >= 2.31",
   "pandas >= 2.1",
   "python-decouple >= 3.4",
   "stockstats >= 0.6.2",
 ]
 
 [project.optional-dependencies]
```

### Comparing `eod2pd-0.2.3.1/readme.md` & `eod2pd-0.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.3.1/src/eod2pd/__init__.py` & `eod2pd-0.2.4/src/eod2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.3.1/src/eod2pd/downloader.py` & `eod2pd-0.2.4/src/eod2pd/downloader.py`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.3.1/src/eod2pd/downloaderfunctions.py` & `eod2pd-0.2.4/src/eod2pd/downloaderfunctions.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,38 +115,44 @@
     # put message into input queue
     send_message(message_content, hook)
 
 
 # -------------------------------------------------------------
 #  get list of exchanges from EODHistoricalData
 # -------------------------------------------------------------
-def get_exchanges() -> pd.DataFrame:
+def get_exchanges(dict_result: bool = True) -> pd.DataFrame:
     """
     Get the list of exchanges from EODHistoricalData.
 
+    Parameters
+    ----------
+    dict_result : bool, optional
+        A flag to indicate if the result should be a dictionary, default: True
+
     Returns
     -------
-    pandas.DataFrame
-        DataFrame containing the list of exchanges.
+    pandas.DataFrame | dict
+        DataFrame containing the list of exchanges or
+        a dictionary containing the list of exchanges.
     """
     # start jobs to get exchanges
     start_jobs_get_exchanges()
-
     # wait until all jobs are done
     basefunctions.default_threadpool.get_input_queue().join()
-
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue()
+    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
+        dict_result=dict_result
+    )
 
 
 # -------------------------------------------------------------
 #  start jobs get list of symbols for a specific exchange from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_exchanges_symbols(
-    exchange: str = "XETRA", params: dict = None, hook: Callable = None
+    exchange: str = None, params: dict = None, hook: Callable = None
 ) -> None:
     """
     Get the list of symbols for a specific exchange from EODHistoricalData.
 
     Parameters
     ----------
     exchangeCode : str, optional
@@ -159,16 +165,20 @@
     Returns
     -------
     pandas.DataFrame
         DataFrame containing the list of symbols for the specified exchange.
     """
     # load api key from environment
     api_key = decouple.config("EOD2PD_API_KEY", default=None)
+    # check if api_key is None
     if api_key is None:
         raise ValueError("##FAILURE## EOD2PD_API_KEY is not set")
+    # check if exchange is None
+    if exchange is None:
+        exchange = "XETRA"
     # build url
     url = (
         f"https://eodhistoricaldata.com/api/exchange-symbol-list/"
         f"{exchange}"
         f"?api_token={api_key}"
         f"&fmt=json"
     )
@@ -185,49 +195,55 @@
 
 
 # -------------------------------------------------------------
 #  get list of symbols for a specific exchange from EODHistoricalData
 # -------------------------------------------------------------
 def get_exchanges_symbols(
     exchanges: List[str] = None,
-) -> dict:
+    dict_result: bool = True,
+) -> pd.DataFrame | dict:
     """
     Get the list of symbols for a specific exchanges from EODHistoricalData.
 
     Parameters
     ----------
     exchanges : list, optional
         A list of exchanges, default: None
+    dict_result : bool, optional
+        A flag to indicate if the result should be a dictionary, default: True
 
     Returns
     -------
-    pandas.DataFrame
-        DataFrame containing the list of symbols for the specified exchange.
+    pandas.DataFrame | dict
+        a DataFrame containing the list of symbols for the specified exchange or
+        a dictionary containing the list of symbols for the specified exchanges
     """
     # check if exchanges is None
     if exchanges is None:
         exchanges = ["XETRA"]
-
+    # check if exchanges is a string
+    if isinstance(exchanges, str):
+        exchanges = [exchanges]
     # loop over all exchanges
     for exchange in exchanges:
         # start jobs to get symbols for exchange
         start_jobs_get_exchanges_symbols(exchange.upper())
-
     # wait until all jobs are done
     basefunctions.default_threadpool.get_input_queue().join()
-
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue()
+    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
+        dict_result=dict_result
+    )
 
 
 # -------------------------------------------------------------
 #  start jobs get symbol prices in a bulk message from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_prices_bulk(
-    exchange: str = "XETRA",
+    exchange: str = None,
     start: str | datetime.date = None,
     end: str | datetime.date = None,
     params: dict = None,
     hook: Callable = None,
 ) -> None:
     """
     Get bulk symbol prices for the given exchange and date.
@@ -249,20 +265,25 @@
 
     Returns
     -------
     pandas.DataFrame
         A DataFrame containing the bulk symbol prices for the given
         exchange and date.
     """
-    # make exchange uppercase
-    exchange = exchange.upper()
     # load api key from environment
     api_key = decouple.config("EOD2PD_API_KEY", default=None)
+    # check if api_key is None
     if api_key is None:
         raise ValueError("##FAILURE## EOD2PD_API_KEY is not set")
+    # check if exchange is None
+    if exchange is None:
+        exchange = "XETRA"
+    # make exchange uppercase
+    exchange = exchange.upper()
+    # check if start and end are None
     if start is None:
         start = datetime.datetime.today()
     if end is None:
         end = datetime.datetime.today()
     if isinstance(start, str):
         start = datetime.datetime.strptime(start, "%Y-%m-%d")
     if isinstance(end, str):
@@ -295,49 +316,57 @@
 # -------------------------------------------------------------
 #  get symbol prices in a bulk message from EODHistoricalData
 # -------------------------------------------------------------
 def get_symbols_prices_bulk(
     exchanges: List[str] = None,
     start: str = None,
     end: str = None,
-) -> dict:
+    dict_result: bool = True,
+) -> pd.DataFrame | dict:
     """
     Get bulk symbol prices for the given exchanges and date.
 
     Parameters
     ----------
     exchanges : str, optional
         A list of exchanges, default: ["XETRA"]
     start : str, optional
         The start date of the prices data, the format is "YY-mm-dd",
         default: None
     end : str, optional
         The end date of the prices data, the format is "YY-mm-dd",
         default: None
+    dict_result : bool, optional
+        A flag to indicate if the result should be a dictionary, default: True
 
     Returns
     -------
-    dict
-        A dictionary containing the bulk symbol prices for the given
-        exchange and date.
+    pandas.DataFrame | dict
+        A DataFrame containing the bulk symbol prices for the given or
+        a dictionary containing the bulk symbol prices for the given
+        exchange and dates.
     """
     # check if exchanges is None
     if exchanges is None:
         exchanges = ["XETRA"]
-
+    # check if exchanges is a string
+    if isinstance(exchanges, str):
+        exchanges = [exchanges]
     # loop over all exchanges
     for exchange in exchanges:
         # start jobs to get symbols bulk prices
         start_jobs_get_symbols_prices_bulk(exchange, start, end)
 
     # wait until all jobs are done
     basefunctions.default_threadpool.get_input_queue().join()
 
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue()
+    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
+        dict_result=dict_result
+    )
 
 
 # -------------------------------------------------------------
 #  start_jobs_get symbol prices from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_prices(
     symbols: List[str] | None,
@@ -349,15 +378,15 @@
 ) -> None:
     """
     Get symbol prices for the given symbols and date.
 
     Parameters
     ----------
     symbols : list, optional
-        The list of symbols to be used, default: None
+        The list of symbols to be used, default: BMW.XETRA
     start : str, optional
         The start date of the prices data, the format is "YY-mm-dd",
         default: "1900-01-01"
     end : str, optional
         The end date of the prices data, the format is "YY-mm-dd",
         default: "2999-12-31"
     freq : str, optional
@@ -370,18 +399,24 @@
     Returns
     -------
     pandas.DataFrame
         A DataFrame containing the symbol prices for the given symbols and date.
     """
     # load api key from environment
     api_key = decouple.config("EOD2PD_API_KEY", default=None)
+    # check if api_key is None
     if api_key is None:
         raise ValueError("##FAILURE## EOD2PD_API_KEY is not set")
+    # check if symbol is None
     if symbols is None:
         symbols = ["BMW.XETRA"]
+    # check if symbols is a string
+    if isinstance(symbols, str):
+        symbols = [symbols]
+    # loop over all symbols
     for symbol in symbols:
         # make symbol uppercase
         symbol = symbol.upper()
         # build the url for the request
         url = (
             f"https://eodhistoricaldata.com/api/eod/{symbol}"
             f"?api_token={api_key}"
@@ -405,46 +440,47 @@
 #  get symbol prices from EODHistoricalData
 # -------------------------------------------------------------
 def get_symbols_prices(
     symbols: List[str] | None,
     start: str = "1900-01-01",
     end: str = "2999-12-31",
     freq: str = "D",
-    combine_dict: bool = False,
+    dict_result: bool = True,
 ) -> dict:
     """
     Get symbol prices for the given symbols and date.
 
     Parameters
     ----------
     symbols : list, optional
-        The list of symbols to be used, default: None
+        The list of symbols to be used, default: "BMW.XETRA"
     start : str, optional
         The start date of the prices data, the format is "YY-mm-dd",
         default: "1900-01-01"
     end : str, optional
         The end date of the prices data, the format is "YY-mm-dd",
         default: "2999-12-31"
     freq : str, optional
         The frequency of the prices data, default: "D"
+    dict_result : bool, optional
+        A flag to indicate if the result should be a dictionary, default: True
 
     Returns
     -------
-    pandas.DataFrame
-        A DataFrame containing the symbol prices for the given symbols and date.
+    pandas.DataFrame | dict
+        A DataFrame containing the symbol prices for the given symbols and date or
+        a dictionary containing the symbols prices for the given symbols and date.
     """
     # start jobs to get symbols prices
     start_jobs_get_symbols_prices(symbols, start, end, freq)
-
     # wait until all jobs are done
     basefunctions.default_threadpool.get_input_queue().join()
-
     # get dataframes from output queue
     return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        combine_dict=combine_dict,
+        dict_result=dict_result
     )
 
 
 # -------------------------------------------------------------
 #  start jobs get symbol dividends from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_dividends(
@@ -474,19 +510,24 @@
     -------
     pandas.DataFrame
         A DataFrame containing the historical symbol dividends for the
         given symbols.
     """
     # load api key from environment
     api_key = decouple.config("EOD2PD_API_KEY", default=None)
+    # check if api_key is None
     if api_key is None:
         raise ValueError("##FAILURE## EOD2PD_API_KEY is not set")
-    # check if symbol is a list
+    # check if symbols is None
     if symbols is None:
         symbols = ["BMW.XETRA"]
+    # check if symbols is a string
+    if isinstance(symbols, str):
+        symbols = [symbols]
+    # loop over all symbols
     for symbol in symbols:
         # make symbol uppercase
         symbol = symbol.upper()
         url = (
             f"https://eodhistoricaldata.com/api/div/{symbol}"
             f"?api_token={api_key}"
             f"&from={start}"
@@ -507,41 +548,44 @@
 # -------------------------------------------------------------
 #  get symbol dividends from EODHistoricalData
 # -------------------------------------------------------------
 def get_symbols_dividends(
     symbols: List[str] | None,
     start: str = "1900-01-01",
     end: str = "2999-12-31",
-) -> dict:
+    dict_result: bool = True,
+) -> pd.DataFrame | dict:
     """
     Get historical symbol dividends for the given symbols.
 
     Parameters
     ----------
     symbols : list of str, optional
         The symbols to retrieve dividends for, default: "BMW.XETRA"
     start : str, optional
         The start date of the dividends data, default: "1900-01-01"
     end : str, optional
         The end date of the dividends, default: "2999-12-31"
+    dict_result : bool, optional
+        A flag to indicate if the result should be a dictionary, default: True
 
     Returns
     -------
-    pandas.DataFrame
-        A DataFrame containing the historical symbol dividends for the
-        given symbols.
+    pandas.DataFrame | dict
+        A DataFrame containing the historical symbol dividends for the given symbols or
+        a dictionary containing the historical symbols dividends for the given symbols.
     """
     # start jobs to get symbols dividends
     start_jobs_get_symbols_dividends(symbols, start, end)
-
     # wait until all jobs are done
     basefunctions.default_threadpool.get_input_queue().join()
-
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue()
+    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
+        dict_result=dict_result
+    )
 
 
 # -------------------------------------------------------------
 #  start jobs get symbol splits from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_splits(
     symbols: List[str] | None,
@@ -570,19 +614,23 @@
     -------
     pandas.DataFrame
         A DataFrame containing the historical symbol dividends for the
         given symbols.
     """
     # load api key from environment
     api_key = decouple.config("EOD2PD_API_KEY", default=None)
+    # check if api_key is None
     if api_key is None:
         raise ValueError("##FAILURE## EOD2PD_API_KEY is not set")
     # check if symbol is a list
     if symbols is None:
         symbols = ["BMW.XETRA"]
+    # check if symbols is a string
+    if isinstance(symbols, str):
+        symbols = [symbols]
     for symbol in symbols:
         # make symbol uppercase
         symbol = symbol.upper()
         url = (
             f"https://eodhistoricaldata.com/api/splits/{symbol}"
             f"?api_token={api_key}"
             f"&from={start}"
@@ -603,56 +651,61 @@
 # -------------------------------------------------------------
 #  get symbol splits from EODHistoricalData
 # -------------------------------------------------------------
 def get_symbols_splits(
     symbols: List[str] | None,
     start: str = "1900-01-01",
     end: str = "2999-12-31",
-) -> dict:
+    dict_result: bool = True,
+) -> pd.DataFrame | dict:
     """
     Get historical symbol splits for the given symbols.
 
     Parameters
     ----------
     symbols : list of str, optional
         The symbols to retrieve splits for, default: "BMW.XETRA"
     start : str, optional
         The start date of the splits data, default: "1900-01-01"
     end : str, optional
         The end date of the splits, default: "2999-12-31"
+    dict_result : bool, optional
+        A flag to indicate if the result should be a dictionary, default: True
 
     Returns
     -------
-    pandas.DataFrame
-        A DataFrame containing the historical symbol dividends for the
-        given symbols.
+    pandas.DataFrame | dict
+        A DataFrame containing the historical symbol dividends for the given symbols or
+        a dictionary containing the historical symbols dividends for the given symbols.
     """
     # start jobs to get symbols splits
     start_jobs_get_symbols_splits(symbols, start, end)
-
     # wait until all jobs are done
     basefunctions.default_threadpool.get_input_queue().join()
-
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue()
+    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
+        dict_result=dict_result
+    )
 
 
 # =========================================================================
 #
 # helper functions
 #
 # =========================================================================
-def send_message(content: EOD2PDMessageContent, hook: Callable = None):
+def send_message(content: EOD2PDMessageContent, hook: Callable = None) -> None:
     """
     Send a message to the EOD2PD message handler.
 
     Parameters
     ----------
-    message_content : EOD2PDMessageContent
+    content : EOD2PDMessageContent
         The content of the message to be sent.
+    hook : Callable, optional
+        A callback function to be executed after sending the message.
     """
     timeout = decouple.config("EOD2PD_TIMEOUT", default=10, cast=int)
     message = basefunctions.threadpool.create_threadpool_message(
         _type=eod2pd.EOD2PDMESSAGEIDENTIFIER,
         content=content,
         timeout=timeout,
         hook=hook,
```

### Comparing `eod2pd-0.2.3.1/src/eod2pd.egg-info/PKG-INFO` & `eod2pd-0.2.4/src/eod2pd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eod2pd
-Version: 0.2.3.1
+Version: 0.2.4
 Summary: a simple library to quere EODHistoricalData in a multithreaded environment
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: basefunctions>=0.3.3
+Requires-Dist: basefunctions>=0.3.7
 Requires-Dist: requests>=2.31
 Requires-Dist: pandas>=2.1
 Requires-Dist: python-decouple>=3.4
 Requires-Dist: stockstats>=0.6.2
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: pytest>=7.4; extra == "test"
```

