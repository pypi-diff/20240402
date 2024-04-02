# Comparing `tmp/pyield-0.3.6.tar.gz` & `tmp/pyield-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.3.6.tar", last modified: Wed Mar 27 10:42:57 2024, max compression
+gzip compressed data, was "pyield-0.3.7.tar", last modified: Tue Apr  2 10:45:33 2024, max compression
```

## Comparing `pyield-0.3.6.tar` & `pyield-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.3.6/LICENSE
--rw-r--r--   0        0        0     3908 2024-03-24 20:00:55.060263 pyield-0.3.6/README.md
--rw-r--r--   0        0        0       22 2024-03-24 19:54:43.727885 pyield-0.3.6/pyield/__about__.py
--rw-r--r--   0        0        0      268 2024-03-19 08:17:56.100352 pyield-0.3.6/pyield/__init__.py
--rw-r--r--   0        0        0     7188 2024-03-25 23:08:51.998573 pyield-0.3.6/pyield/anbima.py
--rw-r--r--   0        0        0     7848 2024-03-27 10:35:39.557322 pyield-0.3.6/pyield/br_calendar.py
--rw-r--r--   0        0        0     2192 2024-03-25 10:11:22.647339 pyield-0.3.6/pyield/br_holidays.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.3.6/pyield/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.3.6/pyield/br_holidays_old.txt
--rw-r--r--   0        0        0     4930 2024-03-25 23:59:19.970950 pyield-0.3.6/pyield/di_futures.py
--rw-r--r--   0        0        0     9678 2024-03-26 00:03:11.075285 pyield-0.3.6/pyield/di_web.py
--rw-r--r--   0        0        0     9478 2024-03-27 10:26:00.084342 pyield-0.3.6/pyield/di_xml.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.3.6/pyield/py.typed
--rw-r--r--   0        0        0     1077 2024-03-27 10:42:57.845470 pyield-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0     1138 2024-02-23 08:17:20.287259 pyield-0.3.6/tests/test_br_calendar.py
--rw-r--r--   0        0        0     2434 2024-03-09 15:05:10.956403 pyield-0.3.6/tests/test_di.py
--rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 pyield-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3908 2024-03-24 20:00:55.060263 pyield-0.3.7/README.md
+-rw-r--r--   0        0        0       22 2024-03-28 10:27:28.136217 pyield-0.3.7/pyield/__about__.py
+-rw-r--r--   0        0        0      399 2024-03-28 10:25:48.557918 pyield-0.3.7/pyield/__init__.py
+-rw-r--r--   0        0        0     7564 2024-04-02 10:08:36.904307 pyield-0.3.7/pyield/anbima.py
+-rw-r--r--   0        0        0     9822 2024-04-02 10:43:38.889181 pyield-0.3.7/pyield/br_calendar.py
+-rw-r--r--   0        0        0     2214 2024-04-02 10:06:20.736451 pyield-0.3.7/pyield/br_holidays.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.3.7/pyield/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.3.7/pyield/br_holidays_old.txt
+-rw-r--r--   0        0        0     4975 2024-04-01 11:58:52.601799 pyield-0.3.7/pyield/di_futures.py
+-rw-r--r--   0        0        0     9684 2024-04-02 10:11:24.407591 pyield-0.3.7/pyield/di_web.py
+-rw-r--r--   0        0        0     9546 2024-04-02 10:40:33.557619 pyield-0.3.7/pyield/di_xml.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.3.7/pyield/py.typed
+-rw-r--r--   0        0        0     1077 2024-04-02 10:45:33.588767 pyield-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0     1138 2024-02-23 08:17:20.287259 pyield-0.3.7/tests/test_br_calendar.py
+-rw-r--r--   0        0        0     2434 2024-03-09 15:05:10.956403 pyield-0.3.7/tests/test_di.py
+-rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 pyield-0.3.7/PKG-INFO
```

### Comparing `pyield-0.3.6/LICENSE` & `pyield-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.3.6/README.md` & `pyield-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.3.6/pyield/anbima.py` & `pyield-0.3.7/pyield/anbima.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 import pandas as pd
+from pandas import Timestamp, DataFrame
 from urllib.error import HTTPError
 
 from . import di_futures as di
 from . import br_calendar as cl
 
 # URL Constants
 ANBIMA_NON_MEMBER_URL = "https://www.anbima.com.br/informacoes/merc-sec/arqs/"
 ANBIMA_MEMBER_URL = "http://www.anbima.associados.rtm/merc_sec/arqs/"
 
 # Constant for conversion to basis points
 BP_CONVERSION_FACTOR = 10_000
 
 
-def process_reference_date(
-    reference_date: str | pd.Timestamp | None = None,
-) -> pd.Timestamp:
+def process_reference_date(reference_date: str | Timestamp | None = None) -> Timestamp:
     """
     Process the given reference date, converting it to a pandas Timestamp. If no date is provided,
     use the previous business day based on the Brazilian calendar.
 
     Parameters:
     - reference_date (str | pd.Timestamp | None): The reference date to process.
 
     Returns:
     - pd.Timestamp: The processed reference date.
     """
     if reference_date:  # Force reference_date to be a pd.Timestamp
-        processed_date = pd.Timestamp(reference_date)
+        processed_date = pd.to_datetime(reference_date)
     else:  # If no reference_date is given, use the previous business day
         today = pd.Timestamp.today().normalize()
-        processed_date = cl.offset_bdays(today, -1)
+        processed_date = cl.offset_bdays(today, -1)  # type: ignore
+
+    # Check if the reference date is Timestamp
+    if not isinstance(processed_date, Timestamp):
+        raise ValueError("Reference date must be a pandas Timestamp.")
+
+    # Raise an error if the reference date is in the future
+    if processed_date > pd.Timestamp.today().normalize():
+        raise ValueError("Reference date cannot be in the future.")
 
     return processed_date
 
 
 def get_raw_data(
-    reference_date: str | pd.Timestamp | None = None, is_anbima_member: bool = False
-) -> pd.DataFrame:
+    reference_date: str | Timestamp | None = None, is_anbima_member: bool = False
+) -> DataFrame:
     """
     Fetch indicative rates from ANBIMA for a specific date.
 
     Parameters:
     - reference_date (pd.Timestamp): Date for which to fetch the indicative rates.
     - is_anbima_member (bool): Whether the request is being made by an ANBIMA member.
 
@@ -71,15 +78,15 @@
     except HTTPError:
         error_date = validated_date.strftime("%d-%m-%Y")
         raise ValueError(f"Failed to get ANBIMA rates for {error_date}")
 
     return df
 
 
-def process_raw_data(df: pd.DataFrame) -> pd.DataFrame:
+def process_raw_data(df_raw: DataFrame) -> DataFrame:
     """
     Process raw data from ANBIMA by filtering selected columns, renaming them, and adjusting data formats.
 
     Parameters:
     - df (pd.DataFrame): Raw data DataFrame to process.
 
     Returns:
@@ -100,32 +107,32 @@
         # "Interv. Ind. Inf. (D0)",
         # "Interv. Ind. Sup. (D0)",
         # "Interv. Ind. Inf. (D+1)",
         # "Interv. Ind. Sup. (D+1)",
         # "Criterio": "Criteria",
     }
     select_columns = list(selected_columns_dict.keys())
-    df = df[select_columns].copy()
-    df.rename(columns=selected_columns_dict, inplace=True)
+    df = df_raw[select_columns].copy()
+    df = df.rename(columns=selected_columns_dict)
 
     # Remove percentage from rates
     rate_cols = ["BidRate", "AskRate", "IndicativeRate"]
     df[rate_cols] = df[rate_cols] / 100
 
     df["ReferenceDate"] = pd.to_datetime(df["ReferenceDate"], format="%Y%m%d")
     df["MaturityDate"] = pd.to_datetime(df["MaturityDate"], format="%Y%m%d")
 
     return df.sort_values(["BondType", "MaturityDate"], ignore_index=True)
 
 
 def get_treasury_rates(
-    reference_date: str | pd.Timestamp | None = None,
+    reference_date: str | Timestamp | None = None,
     return_raw=False,
     is_anbima_member=False,
-) -> pd.DataFrame:
+) -> DataFrame:
     """
     Fetch and process indicative rates from ANBIMA for a specific date.
     If no date is provided, the previous business day based on the Brazilian calendar
     is used.
 
      Parameters:
      - reference_date (str | pd.Timestamp | None): Date for which to fetch the indicative rates.
@@ -142,17 +149,17 @@
     if not return_raw:
         df = process_raw_data(df)
 
     return df
 
 
 def calculate_treasury_di_spreads(
-    reference_date: str | pd.Timestamp | None = None,
+    reference_date: str | Timestamp | None = None,
     is_anbima_member=False,
-) -> pd.DataFrame:
+) -> DataFrame:
     """
     Calculate the DI spread for LTN and NTN-F bonds based on ANBIMA's indicative rates.
     If no date is provided, the previous business day based on the Brazilian calendar
     is used.
 
     Parameters:
     - reference_date (str | pd.Timestamp | None): The reference date for querying ANBIMA's indicative rates.
```

### Comparing `pyield-0.3.6/pyield/br_calendar.py` & `pyield-0.3.7/pyield/br_calendar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,41 @@
-from typing import Literal
+from typing import Literal, overload
 
-import pandas as pd
 import numpy as np
+import pandas as pd
+from pandas import Series, Timestamp
 
 from .br_holidays import BrHolidays
 
 # Instância global da classe Holidays
 br_holidays = BrHolidays()
 
 
-def convert_to_numpy_date(
-    dates: pd.Timestamp | pd.Series,
-) -> np.datetime64 | np.ndarray:
+@overload
+def format_input_dates(dates: str | Timestamp | None) -> Timestamp: ...
+
+
+@overload
+def format_input_dates(dates: Series) -> Series: ...
+
+
+# Implementação da função que atende às sobrecargas acima
+def format_input_dates(dates: str | Timestamp | Series | None) -> Timestamp | Series:
+    if dates is None:
+        return pd.Timestamp.today().normalize()
+    result = pd.to_datetime(dates)
+    if isinstance(result, pd.Series):
+        return result
+    elif result is pd.NaT:
+        raise ValueError("Invalid date format.")
+    else:
+        return pd.Timestamp(result).normalize()
+
+
+def convert_to_numpy_date(dates: Timestamp | Series) -> np.datetime64 | np.ndarray:
     """
     Converts the input dates to a numpy datetime64[D] format.
 
     Args:
         dates (str | pd.Timestamp | pd.Series): A single date or a Series of dates.
 
     Returns:
@@ -23,19 +43,35 @@
     """
     if isinstance(dates, pd.Timestamp):
         return np.datetime64(dates, "D")
     else:
         return dates.to_numpy().astype("datetime64[D]")
 
 
+@overload
+def offset_bdays(
+    dates: str | Timestamp | None = None,
+    offset: int = 0,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> Timestamp: ...
+
+
+@overload
+def offset_bdays(
+    dates: Series,
+    offset: int = 0,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> Series: ...
+
+
 def offset_bdays(
-    dates: str | pd.Timestamp | pd.Series,
-    offset: int,
+    dates: str | Timestamp | Series | None = None,
+    offset: int = 0,
     holiday_list: Literal["old", "new", "infer"] = "infer",
-):
+) -> Timestamp | Series:
     """
     Offsets the dates to the next or previous business day. This function is a wrapper
     for `numpy.busday_offset` to be used directly with Pandas data types that infers the
     right list of holidays based on the most recent date in the input.
 
     Args:
         dates (str | pd.Timestamp | pd.Series): A single date or a Series of dates to be offset.
@@ -61,47 +97,77 @@
         >>> yd.offset_bdays(date, 0)
         Timestamp('2023-12-22') # No offset because it's a business day
         >>> yd.offset_bdays(date, 1)
         Timestamp('2023-12-26') # Offset to the next business day
         >>> yd.offset_bdays(date, -1)
         Timestamp('2023-12-21') # Offset to the previous business day
     """
-    # Assure that the input is in pandas datetime64[ns] format
-    dates_pd = pd.to_datetime(dates)
+    formatted_dates = format_input_dates(dates)
 
-    selected_holidays = br_holidays.get_applicable_holidays(dates_pd, holiday_list)
+    selected_holidays = br_holidays.get_applicable_holidays(
+        formatted_dates, holiday_list
+    )
     selected_holidays_np = convert_to_numpy_date(selected_holidays)
 
-    dates_np = convert_to_numpy_date(dates_pd)
+    dates_np = convert_to_numpy_date(formatted_dates)
     offsetted_dates_np = np.busday_offset(
         dates_np, offsets=offset, roll="forward", holidays=selected_holidays_np
     )
+    if isinstance(offsetted_dates_np, np.datetime64):
+        return pd.Timestamp(offsetted_dates_np, unit="ns")
+    else:
+        result = pd.to_datetime(offsetted_dates_np, unit="ns")
+        return pd.Series(result)
+
+
+@overload
+def count_bdays(
+    start: str | Timestamp | None = None,
+    end: str | Timestamp | None = None,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> int: ...
 
-    # Convert the dates back to a pandas datetime64[ns] format
-    return pd.to_datetime(offsetted_dates_np, unit="ns")
 
+@overload
+def count_bdays(
+    start: Series,
+    end: str | Timestamp | Series | None,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> Series: ...
+
+
+@overload
+def count_bdays(
+    start: str | Timestamp | Series | None,
+    end: Series,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> Series: ...
 
-def count_bdays(start, end, holiday_list: Literal["old", "new", "infer"] = "infer"):
+
+def count_bdays(
+    start: str | Timestamp | Series | None = None,
+    end: str | Timestamp | Series | None = None,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> int | Series:
     """
     Counts the number of business days between a `start` (inclusive) and `end`
     (exclusive). If an end date is earlier than the start date, the count will be
     negative. This function is a wrapper for `numpy.busday_count` to be used directly
     with Pandas data types.
 
     Args:
-        start (str | pd.Timestamp, optional): The start date. Defaults to None.
-        end (str | pd.Timestamp optional): The end date. Defaults to None.
+        start (str | Timestamp, optional): The start date. Defaults to None.
+        end (str | Timestamp optional): The end date. Defaults to None.
         holiday_list (str, optional): The list of holidays to use. Defaults to "infer",
             which infers the right list of holidays based on the most recent date in
             the input.
 
     Returns:
-        np.int64 | np.ndarray: The number of business days between the start date and
-        end dates. Returns a single integer if `end` is a single Timestamp, otherwise
-        returns an ndarray of integers.
+        int | pd.Series: The number of business days between the start date and end date.
+        Returns an integer if the result is a single value, otherwise returns a Series.
 
     Notes:
         - For more information on error handling, see numpy.busday_count documentation at
             https://numpy.org/doc/stable/reference/generated/numpy.busday_count.html.
         - The maximum start date is used to determine which list of holidays to use. If the
             maximum start date is earlier than 2023-12-26, the list of holidays is
             `OLD_BR_HOLIDAYS`. Otherwise, the list of holidays is `NEW_BR_HOLIDAYS`.
@@ -111,38 +177,44 @@
         >>> end = '2024-01-01'
         >>> yd.count_bdays(start, end)
         10
 
         >>> start = '2023-01-01'
         >>> end = pd.to_datetime(['2023-01-31', '2023-03-01'])
         >>> yd.count_bdays(start, end)
-        array([22, 40])
+        pd.Series([22, 40], dtype='int64')
     """
-    # Assure that the inputs are in pandas datetime64[ns] format
-    start_pd = pd.to_datetime(start)
-    end_pd = pd.to_datetime(end)
+    formatted_start = format_input_dates(start)
+    formatted_end = format_input_dates(end)
 
     # Determine which list of holidays to use
-    selected_holidays = br_holidays.get_applicable_holidays(start_pd, holiday_list)
+    selected_holidays = br_holidays.get_applicable_holidays(
+        formatted_start, holiday_list
+    )
     selected_holidays_np = convert_to_numpy_date(selected_holidays)
 
     # Convert inputs to numpy datetime64[D] before calling numpy.busday_count
-    start_np = convert_to_numpy_date(start_pd)
-    end_np = convert_to_numpy_date(end_pd)
+    start_np = convert_to_numpy_date(formatted_start)
+    end_np = convert_to_numpy_date(formatted_end)
 
-    return np.busday_count(start_np, end_np, holidays=selected_holidays_np)
+    result_np = np.busday_count(start_np, end_np, holidays=selected_holidays_np)
+    if isinstance(result_np, np.ndarray):
+        # Return pandas Int64 type for type consistency
+        return pd.Series(result_np, dtype="Int64")
+    else:
+        return int(result_np)
 
 
 def generate_bdays(
-    start: str | pd.Timestamp | None = None,
-    end: str | pd.Timestamp | None = None,
-    inclusive="both",
+    start: str | Timestamp | None = None,
+    end: str | Timestamp | None = None,
+    inclusive: Literal["both", "neither", "left", "right"] = "both",
     holiday_list: Literal["old", "new", "infer"] = "infer",
     **kwargs,
-) -> pd.DatetimeIndex:
+) -> Series:
     """
     Generates a Series of business days between a `start` (inclusive) and `end`
     (inclusive) that takes into account the list of brazilian holidays as the default.
     If no start date is provided, the current date is used. If no end date is provided,
     the current date is used.
 
 
@@ -175,28 +247,27 @@
         2023-12-21    2023-12-21
         2023-12-22    2023-12-22
         2023-12-27    2023-12-27
         2023-12-28    2023-12-28
         2023-12-29    2023-12-29
         dtype: object
     """
-    if start:
-        start_pd = pd.to_datetime(start)
-    else:
-        start_pd = pd.Timestamp.today().normalize()
+    formatted_start = format_input_dates(start)
+    formatted_end = format_input_dates(end)
 
-    if end:
-        end_pd = pd.to_datetime(end)
-    else:
-        end_pd = pd.Timestamp.today().normalize()
+    if isinstance(formatted_start, Series) or isinstance(formatted_end, Series):
+        raise ValueError("The start and end dates must be single dates.")
 
-    selected_holidays = br_holidays.get_applicable_holidays(start_pd, holiday_list)
+    selected_holidays = br_holidays.get_applicable_holidays(
+        formatted_start, holiday_list
+    )
     selected_holidays_list = selected_holidays.to_list()
 
-    return pd.bdate_range(
-        start_pd,
-        end_pd,
+    result = pd.bdate_range(
+        formatted_start,
+        formatted_end,
         freq="C",
         inclusive=inclusive,
         holidays=selected_holidays_list,
         **kwargs,
     )
+    return pd.Series(result)
```

### Comparing `pyield-0.3.6/pyield/br_holidays.py` & `pyield-0.3.7/pyield/br_holidays.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 from pathlib import Path
 from typing import Literal
 
 import pandas as pd
+from pandas import Series, Timestamp
 
 
 class BrHolidays:
     # The date (inclusive) when the new holidays list starts to be valid
     TRANSITION_DATE = pd.to_datetime("2023-12-26")
 
     def __init__(self):
         current_dir = Path(__file__).parent
         new_holidays_path = current_dir / "br_holidays_new.txt"
         old_holidays_path = current_dir / "br_holidays_old.txt"
         self.new_holidays = self._load_holidays(new_holidays_path)
         self.old_holidays = self._load_holidays(old_holidays_path)
 
-    def _load_holidays(self, file_path: Path) -> pd.Series:
+    def _load_holidays(self, file_path: Path) -> Series:
         """Loads the list of holidays from a text file and returns it as a pd.Series of pd.Timestamp."""
         df = pd.read_csv(file_path, header=None, names=["date"], comment="#")
         # Convert the dates to a pd.Series of pd.Timestamp
         return pd.to_datetime(df["date"], format="%d/%m/%Y")
 
     def get_applicable_holidays(
         self,
-        dates: pd.Timestamp | pd.Series,
+        dates: Timestamp | Series,
         holiday_list: Literal["old", "new", "infer"] = "infer",
-    ) -> pd.Series:
+    ) -> Series:
         """
         Returns the correct list of holidays to use based on the most recent date in the input.
 
         Args:
             dates (pd.Timestamp | pd.Series): The date(s) to use to infer the holidays.
             holiday_list (str): The holidays list to use. Valid options are 'old', 'new' or
                 'infer'. If 'infer' is used, the list of holidays is selected based on the
                 earliest (minimum) date in the input.
 
         Returns:
             pd.Series: The list of holidays to use.
         """
-        if isinstance(dates, pd.Timestamp):
+        if isinstance(dates, Timestamp):
             earliest_date = dates
         else:
             earliest_date = dates.min()
 
         match holiday_list:
             case "old":
                 return self.old_holidays
```

### Comparing `pyield-0.3.6/pyield/br_holidays_new.txt` & `pyield-0.3.7/pyield/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.3.6/pyield/br_holidays_old.txt` & `pyield-0.3.7/pyield/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.3.6/pyield/di_futures.py` & `pyield-0.3.7/pyield/di_futures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Literal, Optional
+from typing import Literal
 from pathlib import Path
+
 import pandas as pd
-import pandas.api.types
+from pandas import DataFrame, Timestamp
 
 from . import di_web as diw
 from . import di_xml as dix
 from . import br_calendar as brc
 
 
-def get_expiration_date(expiration_code: str) -> Optional[pd.Timestamp]:
+def get_expiration_date(expiration_code: str) -> Timestamp:
     """
     Internal function to convert the expiration code into its expiration date.
 
     Given a expiration code, this function determines its expiration date.
     If the expiration code does not correspond to a valid month or year, or if the input
     is not in the expected format, the function will return a pd.NaT (Not a Timestamp).
     Valid for contract codes from 22-05-2006 (inclusive) onwards.
@@ -59,23 +60,26 @@
 
     try:
         month_code = expiration_code[0]
         month = month_codes[month_code]
         year = int("20" + expiration_code[-2:])
         # The expiration date is always the first business day of the month
         expiration = pd.Timestamp(year, month, 1)
+
         # Adjust to the next business day when expiration date is a weekend or a holiday
-        return brc.offset_bdays(expiration, offset=0)
+        adj_expiration = brc.offset_bdays(expiration, offset=0)
+
+        return adj_expiration
 
     except (KeyError, ValueError):
-        return pd.NaT  # type: ignore
+        raise ValueError("Invalid expiration code.")
 
 
 def get_di(
-    trade_date: str | pd.Timestamp,
+    trade_date: str | Timestamp,
     source_type: Literal["bmf", "b3", "b3s"] = "bmf",
     return_raw: bool = False,
 ) -> pd.DataFrame:
     """
     Gets the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
@@ -117,15 +121,15 @@
         return diw.get_di(trade_date, return_raw)
     elif source_type in ["b3", "b3s"]:
         return dix.get_di(trade_date, source_type, return_raw)
     else:
         raise ValueError("source_type must be either 'bmf', 'b3' or 'b3s'.")
 
 
-def read_di(file_path: Path, return_raw: bool = False) -> pd.DataFrame:
+def read_di(file_path: Path, return_raw: bool = False) -> DataFrame:
     """
     Reads a DI futures data file and returns a DataFrame.
 
     This function reads a DI futures data file and returns a DataFrame with the data.
 
     Args:
         file_path: a Path object indicating the path to the file.
```

### Comparing `pyield-0.3.6/pyield/di_web.py` & `pyield-0.3.7/pyield/di_web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import io
 import warnings
 from typing import Optional
 
 import pandas as pd
+from pandas import Timestamp, Series, DataFrame
 import requests
 
 from . import br_calendar as brc
 from . import di_futures as dif
 
 
 def get_old_expiration_date(
-    ExpirationCode: str, trade_date: pd.Timestamp
-) -> Optional[pd.Timestamp]:
+    ExpirationCode: str, trade_date: Timestamp
+) -> Optional[Timestamp]:
     """
     Internal function to convert an old DI contract code into its ExpirationDate date. Valid for
     contract codes up to 21-05-2006.
 
     Args:
         ExpirationCode (str):
             An old DI ExpirationCode from B3, where the first three letters represent
@@ -67,15 +68,15 @@
         # Must use the old holiday calendar, since this type of contract code was used until 2006
         return brc.offset_bdays(ExpirationDate, offset=0, holiday_list="old")
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
-def get_raw_di(trade_date: pd.Timestamp) -> pd.DataFrame:
+def get_raw_di(trade_date: Timestamp) -> DataFrame:
     """
     Internal function to fetch raw DI futures data from B3 for a specific trade date.
 
     Args:
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
@@ -115,15 +116,15 @@
     except Exception as e:
         warnings.warn(
             f"A {type(e).__name__} occurred while reading the DI futures data for {trade_date.strftime('%d/%m/%Y')}. Returning an empty DataFrame."
         )
         return pd.DataFrame()
 
 
-def convert_prices_to_rates(prices: pd.Series, bd: pd.Series) -> pd.Series:
+def convert_prices_to_rates(prices: Series, bd: Series) -> Series:
     """
     Internal function to convert DI futures prices to rates.
 
     Args:
         prices (pd.Series): A Series containing DI futures prices.
         bd (pd.Series): A Series containing the number of business days to ExpirationDate.
 
@@ -132,15 +133,15 @@
     """
     rates = (100_000 / prices) ** (252 / bd) - 1
 
     # Return rates as percentage
     return 100 * rates
 
 
-def convert_prices_in_older_contracts(df: pd.DataFrame) -> pd.DataFrame:
+def convert_prices_in_older_contracts(df: DataFrame) -> DataFrame:
     # Prior to 01/01/2002, prices were not converted to rates
     convert_cols = [
         "FirstRate",
         "MinRate",
         "MaxRate",
         "AvgRate",
         "LastRate",
@@ -152,15 +153,15 @@
 
     # Invert low and high prices
     df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
 
     return df
 
 
-def process_di(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def process_di(df: DataFrame, trade_date: Timestamp) -> DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
@@ -261,15 +262,15 @@
         "LastAskRate",
         "LastBidRate",
         "SettlementRate",
     ]
     return df[ordered_cols]
 
 
-def get_di(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def get_di(trade_date: Timestamp, return_raw: bool = False) -> DataFrame:
     """
     Gets the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
     trade date. It's the primary external interface for accessing DI data.
 
     Args:
```

### Comparing `pyield-0.3.6/pyield/di_xml.py` & `pyield-0.3.7/pyield/di_xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import io
 import zipfile
 from pathlib import Path
 
 import requests
 import pandas as pd
+from pandas import Timestamp, DataFrame
 from lxml import etree
 
 from . import di_futures as dif
 from . import br_calendar as brc
 
 
-def get_file_from_url(trade_date: pd.Timestamp, source_type: str) -> io.BytesIO:
+def get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
     """
     Types of XML files available:
     Full Price Report (all assets)
         - aprox. 5 MB zipped file;
         - url example: https://www.b3.com.br/pesquisapregao/download?filelist=PR231228.zip
     Simplified Price Report (derivatives)
         - aprox. 50kB zipped file;
@@ -115,24 +116,24 @@
 
         # Adicionar o dicionário à lista
         di_data.append(ticker_data)
 
     return di_data
 
 
-def create_df_from_di_data(di1_data: list) -> pd.DataFrame:
+def create_df_from_di_data(di1_data: list) -> DataFrame:
     # Criar um DataFrame com os dados coletados
     df = pd.DataFrame(di1_data)
 
     # Convert to CSV and then back to pandas to get automatic type conversion
     file = io.StringIO(df.to_csv(index=False))
     return pd.read_csv(file, dtype_backend="numpy_nullable")
 
 
-def filter_and_order_pr_df(df: pd.DataFrame) -> pd.DataFrame:
+def filter_and_order_pr_df(df: DataFrame) -> DataFrame:
     selected_columns = [
         "TradDt",
         "TckrSymb",
         # "MktDataStrmId",
         "OpnIntrst",
         "FinInstrmQty",
         "NtlFinVol",
@@ -160,15 +161,15 @@
         # "VartnPts",
         # "AdjstdValCtrct",
     ]
 
     return df[selected_columns]
 
 
-def filter_and_order_sprd_df(df: pd.DataFrame) -> pd.DataFrame:
+def filter_and_order_sprd_df(df: DataFrame) -> DataFrame:
     cols = [
         "TradDt",
         "TckrSymb",
         "OpnIntrst",
         "AdjstdQt",
         "MinPric",
         "TradAvrgPric",
@@ -182,15 +183,15 @@
         # "PrvsAdjstdQtTax",
         # "PrvsAdjstdQtStin",  # Constant column
     ]
 
     return df[cols]
 
 
-def standardize_column_names(df: pd.DataFrame) -> pd.DataFrame:
+def standardize_column_names(df: DataFrame) -> DataFrame:
     rename_dict = {
         "TradDt": "TradeDate",
         "TckrSymb": "Ticker",
         # "MktDataStrmId"
         # "IntlFinVol",
         "OpnIntrst": "OpenContracts",
         "FinInstrmQty": "TradedQuantity",
@@ -219,15 +220,15 @@
         # "VartnPts",
         # "AdjstdValCtrct",
     }
 
     return df.rename(columns=rename_dict)
 
 
-def process_di_df(df_raw: pd.DataFrame) -> pd.DataFrame:
+def process_di_df(df_raw: DataFrame) -> DataFrame:
     df = df_raw.copy()
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradDt"] = df["TradDt"].astype("datetime64[ns]")
 
     expiration = df["TckrSymb"].str[3:].apply(dif.get_expiration_date)
     df.insert(2, "ExpirationDate", expiration)
 
@@ -239,19 +240,15 @@
 
     # Remove expired contracts
     df.query("BDToExpiration > 0", inplace=True)
 
     return df.sort_values(by=["ExpirationDate"], ignore_index=True)
 
 
-def get_di(
-    trade_date: pd.Timestamp,
-    source_type: str,
-    return_raw: bool,
-) -> pd.DataFrame:
+def get_di(trade_date: Timestamp, source_type: str, return_raw: bool) -> DataFrame:
     zip_file = get_file_from_url(trade_date, source_type)
 
     xml_file = extract_xml_from_zip(zip_file)
 
     di_data = extract_di_data_from_xml(xml_file)
 
     df_raw = create_df_from_di_data(di_data)
@@ -259,25 +256,27 @@
         return df_raw
 
     # Remove unnecessary columns
     if source_type == "b3":
         df_di = filter_and_order_pr_df(df_raw)
     elif source_type == "b3s":
         df_di = filter_and_order_sprd_df(df_raw)
+    else:
+        raise ValueError("Invalid source type. Must be 'b3' or 'b3s'.")
 
     # Process and transform data
     df_di = process_di_df(df_di)
 
     # Standardize column names
     df_di = standardize_column_names(df_di)
 
     return df_di
 
 
-def read_di(file_path: Path, return_raw: bool = False) -> pd.DataFrame:
+def read_di(file_path: Path, return_raw: bool = False) -> DataFrame:
     if file_path:
         if file_path.exists():
             content = file_path.read_bytes()
             zip_file = io.BytesIO(content)
         else:
             raise FileNotFoundError(f"No file found at {file_path}.")
```

### Comparing `pyield-0.3.6/pyproject.toml` & `pyield-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.3.6"
+version = "0.3.7"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.3.6/tests/test_br_calendar.py` & `pyield-0.3.7/tests/test_br_calendar.py`

 * *Files identical despite different names*

### Comparing `pyield-0.3.6/tests/test_di.py` & `pyield-0.3.7/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `pyield-0.3.6/PKG-INFO` & `pyield-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
```

