# Comparing `tmp/petrosa-0.0.55-py3-none-any.whl.zip` & `tmp/petrosa-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,11 @@
-Zip file size: 3218339 bytes, number of entries: 22
--rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/__init__.py
--rw-r--r--  2.0 unx     1811 b- defN 20-Feb-02 00:00 petrosa/binance/binance.py
--rw-r--r--  2.0 unx     1473 b- defN 20-Feb-02 00:00 petrosa/checkers/consistency.py
--rw-r--r--  2.0 unx        9 b- defN 20-Feb-02 00:00 petrosa/converters/.gitignore
+Zip file size: 5384 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/converters/__init__.py
--rw-r--r--  2.0 unx     2778 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
--rw-r--r--  2.0 unx     1502 b- defN 20-Feb-02 00:00 petrosa/converters/data.pickle
--rw-r--r--  2.0 unx      173 b- defN 20-Feb-02 00:00 petrosa/converters/myparams.pickle
--rw-r--r--  2.0 unx        5 b- defN 20-Feb-02 00:00 petrosa/converters/params.pickle
--rw-r--r--  2.0 unx 12175544 b- defN 20-Feb-02 00:00 petrosa/converters/stats.pickle
--rw-r--r--  2.0 unx     3688 b- defN 20-Feb-02 00:00 petrosa/database/mongo.py
--rw-r--r--  2.0 unx     1820 b- defN 20-Feb-02 00:00 petrosa/database/sql.py
--rw-r--r--  2.0 unx      462 b- defN 20-Feb-02 00:00 petrosa/messaging/kafkaproducer.py
--rw-r--r--  2.0 unx      547 b- defN 20-Feb-02 00:00 petrosa/messaging/kafkareceiver.py
--rw-r--r--  2.0 unx      198 b- defN 20-Feb-02 00:00 petrosa/observability/opentel.py
+-rw-r--r--  2.0 unx     2257 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/ta/__init__.py
--rw-r--r--  2.0 unx    25122 b- defN 20-Feb-02 00:00 petrosa/ta/strategies.py
--rw-r--r--  2.0 unx      970 b- defN 20-Feb-02 00:00 petrosa/ta/utils.py
-?rw-r--r--  2.0 unx      867 b- defN 20-Feb-02 00:00 petrosa-0.0.55.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.55.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.55.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1823 b- defN 20-Feb-02 00:00 petrosa-0.0.55.dist-info/RECORD
-22 files, 12219942 bytes uncompressed, 3215363 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx    22023 b- defN 20-Feb-02 00:00 petrosa/ta/strategies.py
+-rw-r--r--  2.0 unx      822 b- defN 20-Feb-02 00:00 petrosa/ta/utils.py
+?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/RECORD
+9 files, 27675 bytes uncompressed, 4164 bytes compressed:  85.0%
```

## zipnote {}

```diff
@@ -1,67 +1,28 @@
-Filename: petrosa/__init__.py
-Comment: 
-
-Filename: petrosa/binance/binance.py
-Comment: 
-
-Filename: petrosa/checkers/consistency.py
-Comment: 
-
-Filename: petrosa/converters/.gitignore
-Comment: 
-
 Filename: petrosa/converters/__init__.py
 Comment: 
 
 Filename: petrosa/converters/backtests.py
 Comment: 
 
-Filename: petrosa/converters/data.pickle
-Comment: 
-
-Filename: petrosa/converters/myparams.pickle
-Comment: 
-
-Filename: petrosa/converters/params.pickle
-Comment: 
-
-Filename: petrosa/converters/stats.pickle
-Comment: 
-
-Filename: petrosa/database/mongo.py
-Comment: 
-
-Filename: petrosa/database/sql.py
-Comment: 
-
-Filename: petrosa/messaging/kafkaproducer.py
-Comment: 
-
-Filename: petrosa/messaging/kafkareceiver.py
-Comment: 
-
-Filename: petrosa/observability/opentel.py
-Comment: 
-
 Filename: petrosa/ta/__init__.py
 Comment: 
 
 Filename: petrosa/ta/strategies.py
 Comment: 
 
 Filename: petrosa/ta/utils.py
 Comment: 
 
-Filename: petrosa-0.0.55.dist-info/METADATA
+Filename: petrosa-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: petrosa-0.0.55.dist-info/WHEEL
+Filename: petrosa-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: petrosa-0.0.55.dist-info/licenses/LICENSE
+Filename: petrosa-0.0.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: petrosa-0.0.55.dist-info/RECORD
+Filename: petrosa-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## petrosa/converters/backtests.py

```diff
@@ -1,17 +1,9 @@
-import copy
 import datetime
-
 import pandas as pd
-import pkg_resources
-import logging
-
-ver = pkg_resources.get_distribution('petrosa').version
-logging.info("petrosa-utils version: " + ver)
-
 
 def remove_weird_chars(results):
     # results_json = json.loads(json.dumps(results.to_dict(), default=str))
     results_json = results
 
     new_res = {}
 
@@ -31,65 +23,55 @@
         new_key = new_key.lower()
 
         new_res[new_key] = results_json[old_key]
 
     return new_res
 
 def dict_time_convert(stats):
+    from datetime import timedelta
     ret_res = {}
     
     for key in stats.keys():
         if isinstance(stats[key], pd.Timedelta):
             ret_res[key] = stats[key].total_seconds()
         elif isinstance(stats[key], pd.Timestamp):
             ret_res[key] = stats[key].to_pydatetime()
         else:
             ret_res[key] = stats[key]
 
     return ret_res
 
-def result_maker(bt_stats, bt_params, bt_test_params, test_type):
-    bt_stats = copy.deepcopy(bt_stats)
-    bt_params = copy.deepcopy(bt_params)
-    bt_test_params = copy.deepcopy(bt_test_params)
-    test_type = copy.deepcopy(test_type)
-                
-    if '_trades' in bt_stats:
-        del(bt_stats['_trades'])
-    if '_strategy' in bt_stats:
-        del(bt_stats['_strategy'])
-    if '_equity_curve' in bt_stats:
-        del(bt_stats['_equity_curve'])
+def result_maker(stats, params, test_params, test_type):
+    if '_trades' in stats:
+        del(stats['_trades'])
+    if '_strategy' in stats:
+        del(stats['_strategy'])
+    if '_equity_curve' in stats:
+        del(stats['_equity_curve'])
         
-    if '_id' in bt_test_params:
-        del(bt_test_params["_id"])
+    if '_id' in test_params:
+        del(test_params["_id"])
 
-    bt_stats = remove_weird_chars(bt_stats)
-    bt_params = remove_weird_chars(bt_params)
+    stats = remove_weird_chars(stats)
+    params = remove_weird_chars(params)
 
-    bt_stats = dict_time_convert(bt_stats)
+    stats = dict_time_convert(stats)
     
-    ret = {**bt_test_params, **bt_stats, **bt_params}
+    ret = {**test_params, **stats, **params}
     ret['test_type'] = test_type
     ret['insert_timestamp'] = datetime.datetime.now()
         
     return ret
 
 
 def list_maker(stats, test_params):
     list_doc = {}
     list_doc['insert_timestamp'] = datetime.datetime.now()
     list_doc['n_trades'] = stats['# Trades']
     list_doc['strategy'] = test_params['strategy']
     list_doc['period'] = test_params['period']
     list_doc['symbol'] = test_params['symbol']
     list_doc['trades_list'] = stats._trades.to_dict('records')
-    
-    td_list = []
-    
-    for item in list_doc['trades_list']:
-        td_list.append(dict_time_convert(item))
 
-    list_doc['trades_list'] = td_list
     ret = {**list_doc, **test_params}
     
     return ret
```

## petrosa/ta/strategies.py

```diff
@@ -1,46 +1,19 @@
 import logging
 
 from ..ta import utils
-import pkg_resources
-import logging
-
-ver = pkg_resources.get_distribution('petrosa').version
-logging.info("petrosa-utils version: " + ver)
-
-
-strategy_list = ['inside_bar_buy',
-                 'inside_bar_sell',
-                 'continuous_stitch_buy',
-                 'continuous_stitch_sell',
-                 'setup_91_buy',
-                 'setup_91_sell',
-                 'setup_92_buy',
-                 'setup_92_sell',
-                 'setup_93_buy',
-                 'setup_93_sell',
-                 'setup_94_buy',
-                 'setup_94_sell',
-                 'fox_trap_buy',
-                 'fox_trap_sell',
-                 'bear_trap_buy',
-                 'bear_trap_sell',
-                 'bbss_sell',
-                 'bbss_buy',
-                 ]
 
 def inside_bar_buy(candles, timeframe, periods=126):
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     low = float(list(dat['Low'])[-1])
     high = float(list(dat['High'])[-1])
 
     ema8 = dat["Close"].ewm(span=8, adjust=True, min_periods=7).mean()
     ema80 = dat["Close"].ewm(span=80, adjust=True, min_periods=79).mean()
@@ -77,15 +50,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     low = float(list(dat['Low'])[-1])
     high = float(list(dat['High'])[-1])
 
     ema8 = dat["Close"].ewm(span=8, adjust=True, min_periods=7).mean()
     ema80 = dat["Close"].ewm(span=80, adjust=True, min_periods=79).mean()
@@ -116,15 +88,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     last_close = float(list(dat['Close'])[-2])
     low = float(list(dat['Low'])[-1])
     high = float(list(dat['High'])[-1])
     high2 = float(list(dat['High'])[-2])
     high3 = float(list(dat['High'])[-3])
@@ -162,15 +133,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     low = float(list(dat['Low'])[-1])
     low2 = float(list(dat['Low'])[-2])
     low3 = float(list(dat['Low'])[-3])
     high = float(list(dat['High'])[-1])
     high1 = float(list(dat['High'])[-2])
     last_close = float(list(dat['Close'])[-2])
@@ -211,15 +181,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(dat['Close'].iloc[-1])
     low = float(dat['Low'].iloc[-1])
     high = float(dat['High'].iloc[-1])
 
     ema9 = dat["Close"].ewm(span=9, min_periods=8, adjust=True).mean()
     ema9_last = ema9.iloc[-1]
@@ -250,15 +219,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(dat['Close'].iloc[-1])
     low = float(dat['Low'].iloc[-1])
     high = float(dat['High'].iloc[-1])
 
     ema9 = dat["Close"].ewm(span=9, min_periods=8, adjust=True).mean()
     ema9_last = ema9.iloc[-1]
@@ -289,15 +257,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     low = float(dat['Low'].iloc[-1])
     high = float(dat['High'].iloc[-1])
 
     close = float(dat['Close'].iloc[-1])
     last_low = float(dat['Low'].iloc[-2])
 
@@ -328,15 +295,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     low = float(dat['Low'].iloc[-1])
     high = float(dat['High'].iloc[-1])
 
     close = float(dat['Close'].iloc[-1])
     last_high = float(dat['High'].iloc[-2])
 
@@ -367,15 +333,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     ema9 = dat["Close"].ewm(span=9, min_periods=8, adjust=True).mean()
     inclination = ema9.diff()
 
     buy_cond_1 = False in list(dat['Low'][-3:].astype(float) > ema9[-3:])
     buy_cond_2 = False in list(inclination[-5:] > 0)
 
@@ -407,15 +372,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     ema9 = dat["Close"].ewm(span=9, min_periods=8, adjust=True).mean()
     inclination = ema9.diff()
 
     sell_cond_1 = False in list(dat['High'][-3:].astype(float) < ema9[-3:])
     sell_cond_2 = False in list(inclination[-5:] < 0)
 
@@ -447,15 +411,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     ema9 = dat["Close"].ewm(span=9, min_periods=8, adjust=True).mean()
     dat['ema'] = ema9
     inc_ema9 = ema9.diff()
 
     buy_cond_1 = False in list(dat['Low'][-7:-2].astype(float) > ema9[-7:-2])
 
@@ -485,15 +448,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     ema9 = dat["Close"].ewm(span=9, min_periods=8, adjust=True).mean()
     dat['ema'] = ema9
     inc_ema9 = ema9.diff()
 
     sell_cond_1 = False in list(dat['High'][-7:-2].astype(float) < ema9[-7:-2])
 
@@ -527,15 +489,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     low = float(list(dat['Low'])[-1])
     high = float(dat['High'].iloc[-1])
     high2 = float(dat['High'].iloc[-2])
     high3 = float(dat['High'].iloc[-3])
 
@@ -574,15 +535,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     high = float(list(dat['High'])[-1])
     low = float(list(dat['Low'])[-1])
     low2 = float(list(dat['Low'])[-2])
     low3 = float(list(dat['Low'])[-3])
 
@@ -619,15 +579,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     last_close = float(list(dat['Close'])[-2])
     low = float(list(dat['Low'])[-1])
     high = float(list(dat['High'])[-1])
     high2 = float(list(dat['High'])[-2])
     high3 = float(list(dat['High'])[-3])
@@ -664,15 +623,14 @@
 
     dat = candles
 
     dat = dat.sort_index(ascending=True)
 
     if len(dat) < periods:
         logging.info('Error: insufficient data')
-        return {}
 
     close = float(list(dat['Close'])[-1])
     last_close = float(list(dat['Close'])[-2])
     low = float(list(dat['Low'])[-1])
     low2 = float(list(dat['Low'])[-2])
     low3 = float(list(dat['Low'])[-3])
     high = float(list(dat['High'])[-1])
@@ -700,66 +658,7 @@
                                         disruption_value=low,
                                         stop_loss=high,
                                         take_profit=low -
                                         ((high - low) * 2),
                                         direction='LOWER')
     else:
         return {}
-
-
-def bbss_sell(candles, timeframe, periods=30):
-
-    dat = candles
-
-    dat = dat.sort_index(ascending=True)
-
-    if len(dat) < periods:
-        logging.info('Error: insufficient data')
-        return {}
-
-    low = float(list(dat['Low'])[-1])
-    high = float(list(dat['High'])[-1])
-    close = float(list(dat['Close'])[-1])
-
-
-
-    if not (False in list(dat.Close.iloc[-9:].values > dat.Close.iloc[-13:-4].values)) and dat.Close.iloc[-10] < dat.Close.iloc[-14]:
-
-        return utils.strategy_output(ticker=dat.ticker.iloc[-1],
-                                        timeframe=timeframe,
-                                        pet_datetime=dat.index[-1],
-                                        entry_value=low,
-                                        disruption_value=low,
-                                        stop_loss=high,
-                                        take_profit=low -
-                                        ((high - low) * 2),
-                                        direction='LOWER')
-    else:
-        return {}
-
-
-def bbss_buy(candles, timeframe, periods=30):
-
-    dat = candles
-
-    dat = dat.sort_index(ascending=True)
-
-    if len(dat) < periods:
-        logging.info('Error: insufficient data')
-        return {}
-
-    low = float(list(dat['Low'])[-1])
-    high = float(list(dat['High'])[-1])
-
-    if not (False in list(dat.Close.iloc[-9:].values < dat.Close.iloc[-13:-4].values)) and dat.Close.iloc[-10] > dat.Close.iloc[-14]:
-
-        return utils.strategy_output(ticker=dat.ticker.iloc[-1],
-                                        timeframe=timeframe,
-                                        pet_datetime=dat.index[-1],
-                                        entry_value=high,
-                                        disruption_value=high,
-                                        stop_loss=low,
-                                        take_profit=high +
-                                        ((high - low) * 2),
-                                        direction='UPPER')
-    else:
-        return {}
```

## petrosa/ta/utils.py

```diff
@@ -1,26 +1,20 @@
 import datetime
-import pkg_resources
-import logging
-
-ver = pkg_resources.get_distribution('petrosa').version
-logging.info("petrosa-utils version: " + ver)
-
 
 
 def strategy_output(
     ticker,
     timeframe,
     pet_datetime,
     entry_value,
     disruption_value,
     stop_loss,
     take_profit,
     direction
-) -> dict:
+):
 
     if (timeframe == 'm15'):
         minutes = 15
     elif (timeframe == 'm30'):
         minutes = 30
     elif (timeframe == 'h1'):
         minutes = 60
```

## Comparing `petrosa-0.0.55.dist-info/licenses/LICENSE` & `petrosa-0.0.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

