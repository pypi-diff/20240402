# Comparing `tmp/quickfin-1.6.0.tar.gz` & `tmp/quickfin-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfin-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quickfin-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quickfin-1.6.0.tar` & `quickfin-1.7.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.6.0/README.md
--rw-r--r--   0        0        0      729 2024-04-01 14:20:04.529503 quickfin-1.6.0/pyproject.toml
--rw-r--r--   0        0        0    28708 2024-04-01 14:19:53.389110 quickfin-1.6.0/quickfin.py
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 quickfin-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.7.0/README.md
+-rw-r--r--   0        0        0      730 2024-04-02 09:40:45.743229 quickfin-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0    26853 2024-04-02 09:40:19.685593 quickfin-1.7.0/quickfin.py
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 quickfin-1.7.0/PKG-INFO
```

### Comparing `quickfin-1.6.0/pyproject.toml` & `quickfin-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickfin"
-version = "1.6.0"
+version = "1.7.0"
 authors = [{name = "Derek Evans"}]
 description = "A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "plotly"
```

### Comparing `quickfin-1.6.0/quickfin.py` & `quickfin-1.7.0/quickfin.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A Python module providing instant access to live
 and historical stock market price data, automated
 Plotly data visualization generators and a metadata
 catalog for referencing equities, stock symbols, sectors,
 and industry information.
 """
 
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 __author__ = "Derek Evans <https://github.com/REPNOT>"
 __date__ = "28 March 2024"
 
 import json
 from pprint import pprint
 import requests
 import datetime
@@ -24,15 +24,15 @@
 
 class FinInfo():
 
     """
     A class for accessing a metadata catalog for referencing. 
     equities, stock symbols, sectors, and industry information.
 
-    THE FOLLOWING APPLIES TO ALL FinInfo FUNCTIONS:
+    THE FOLLOWING APPLIES TO ALL FinInfo METHOD:
 
     If the value is set to `False`
     for the `payload` parameter, this method
     will `pretty print` the requested data omitting
     a return value.  Otherwise, the value assigned to the
     `payload` parameter is set to `True` by default, and
     the method will return a data payload.
@@ -361,15 +361,14 @@
         for the stock symbol passed to the `symbol`
         parameter.  Method will return live market
         price quotes during trading hours.
 
         PAYLOAD CONTENTS:
 
         Object
-
         """
 
         self.symbol = symbol
         info = FinInfo()
         self.info = info.equity(symbol)
 
         try:
@@ -470,54 +469,14 @@
         except:
             return '===  SYMBOL DATA TYPE ERROR OR SYMBOL UNAVAILABLE  ==='
 
 
     def history(self, symbol, days=None, date=None, date_start=None, date_end=None):
 
         """
-        Return data payload containing a list
-        of all stock symbols belonging to the
-        industry passed to the `industry` parameter
-        available in the metadata catalog. 
-
-        PAYLOAD CONTENTS:
-
-        An array of strings.
-
-        By default, the return value will include an 
-        object containing all industries and associated 
-        symbols.
-
-        Return data payload containing a list
-        of all stock symbols belonging to the
-        sector passed to the `sector` parameter
-        available in the metadata catalog. 
-
-        PAYLOAD CONTENTS:
-
-        An array of strings.
-
-        By default, the return value will include an 
-        object containing all sectors and associated 
-        symbols.
-
-        A class providing instant access to live 
-        and historical stock market price data and
-        automated Plotly data visualization generators.
-
-        Return data payload containing the
-        most recent stock price data available
-        for the stock symbol passed to the `symbol`
-        parameter.  Method will return live market
-        price quotes during trading hours.
-
-        PAYLOAD CONTENTS:
-
-        Object
-
         Return data payload containing all historical
         stock price data available for the stock symbol 
         passed to the `symbol` parameter.
         
         Passing a positive integer value to the `days` 
         parameter will filter the historical data to include
         records for the number of most recent days 
@@ -541,27 +500,18 @@
         PAYLOAD CONTENTS:
 
         Object containing equity metadata,
         current price data, and an array
         of objects consisting of daily price
         data for all available dates.
 
-
         """
 
         self.symbol = symbol
 
-        if date_start == None and date_end == None:
-            pass
-        elif (date_start != None and date_end == None) or (date_start == None and date_end != None):
-            return '===  ERROR: BOTH date_start & date_end MUST BE POSITIVE INTEGER VALUES FOR DATE RANGES  ==='
-        elif date_start != None and date_end != None and type(date_start) is not int or type(date_end) is not int or date_start <= 0 or date_start <= 0:
-            return '===  ERROR: BOTH date_start & date_end MUST BE POSITIVE INTEGER VALUES FOR DATE RANGES  ==='
-        else:
-            pass
 
         try:
             url = self.base_url + self.symbol + self.tail_url
             self.rawData = urlopen(Request(url)).readlines()
         except:
             return '===  ERROR: GET REQUEST FAILED  ==='
 
@@ -655,15 +605,15 @@
                 if self.row_data['Day Range'] < 0:
                     self.row_data['Day Range'] = self.row_data['Day Range'] * -1
                 else:
                     pass
 
             except:
 
-                self.data['Day Range'] = ''
+                self.row_data['Day Range'] = ''
 
             self.data["history"].append(self.row_data)
 
         if days == None and date == None and date_start == None and date_end == None:
 
             return self.data
 
@@ -716,15 +666,15 @@
 
         PAYLOAD CONTENTS:
 
         Plotly Visualization
 
         """
 
-        if type(days) is not int or days >= 0:
+        if type(days) is not int or days < 1:
             return f'===  DATA TYPE ERROR - DAYS MUST BE INTEGER VALUE GREATER THAN OR EQUAL TO 1  ==='
         else:
             pass
 
         self.symbol = symbol
         self.days = days
         self.data = self.history(symbol, self.days)
@@ -748,15 +698,14 @@
                 increasing_line_color= 'green', 
                 decreasing_line_color= 'red'
             )]
         )
 
         fig.update_layout(xaxis_rangeslider_visible=False)
         fig.update_xaxes(type="category", tickangle=60, automargin="height+width", autorange="reversed")
-        fig.show()
 
         try:
             fig.show()
             return self.history
         except:
             return f'===  SYMBOL DATA TYPE ERROR OR INVALID SYMBOL  ==='
 
@@ -823,15 +772,14 @@
         quote_data = [row[self.param] for row in self.history]
         dates = [f'{str(row["Date"]).split("-")[1]}-{str(row["Date"]).split("-")[-1]}-{str(row["Date"]).split("-")[0][2:]}' for row in self.history]
 
         fig = go.Figure([go.Scatter(x=dates, y=quote_data)])
 
         fig.update_layout(xaxis_rangeslider_visible=False)
         fig.update_xaxes(type="category", tickangle=60, automargin="height+width", autorange="reversed")
-        fig.show()
 
         try:
             fig.show()
             return self.history
         except:
             return f'===  SYMBOL DATA TYPE ERROR OR INVALID SYMBOL  ==='
 
@@ -903,13 +851,12 @@
                     line_color='darkslategray',
                     fill_color='lightcyan',
                     align='left'
                 )
             )
         ])
 
-
         try:
             fig.show()
             return self.history
         except:
             return f'===  SYMBOL DATA TYPE ERROR OR INVALID SYMBOL  ==='
```

### Comparing `quickfin-1.6.0/PKG-INFO` & `quickfin-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quickfin
-Version: 1.6.0
+Version: 1.7.0
 Summary: A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information.
 Author: Derek Evans
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: plotly
 Project-URL: Home, https://quickfin.techbyderek.com/
```

