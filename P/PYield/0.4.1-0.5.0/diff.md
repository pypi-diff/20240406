# Comparing `tmp/pyield-0.4.1.tar.gz` & `tmp/pyield-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.4.1.tar", last modified: Thu Apr  4 06:37:26 2024, max compression
+gzip compressed data, was "pyield-0.5.0.tar", last modified: Sat Apr  6 18:50:20 2024, max compression
```

## Comparing `pyield-0.4.1.tar` & `pyield-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.4.1/LICENSE
--rw-r--r--   0        0        0     3908 2024-03-24 20:00:55.060263 pyield-0.4.1/README.md
--rw-r--r--   0        0        0       22 2024-04-04 06:35:56.778689 pyield-0.4.1/pyield/__about__.py
--rw-r--r--   0        0        0      439 2024-04-03 01:25:29.226587 pyield-0.4.1/pyield/__init__.py
--rw-r--r--   0        0        0     7180 2024-04-04 06:34:56.777051 pyield-0.4.1/pyield/anbima.py
--rw-r--r--   0        0        0    11050 2024-04-03 08:44:15.200333 pyield-0.4.1/pyield/br_calendar.py
--rw-r--r--   0        0        0     2214 2024-04-02 10:06:20.736451 pyield-0.4.1/pyield/br_holidays.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.4.1/pyield/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.4.1/pyield/br_holidays_old.txt
--rw-r--r--   0        0        0     5742 2024-04-03 08:39:31.403271 pyield-0.4.1/pyield/di_futures.py
--rw-r--r--   0        0        0     9684 2024-04-02 10:11:24.407591 pyield-0.4.1/pyield/di_web.py
--rw-r--r--   0        0        0     9546 2024-04-02 10:40:33.557619 pyield-0.4.1/pyield/di_xml.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.4.1/pyield/py.typed
--rw-r--r--   0        0        0     1077 2024-04-04 06:37:26.441092 pyield-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1138 2024-02-23 08:17:20.287259 pyield-0.4.1/tests/test_br_calendar.py
--rw-r--r--   0        0        0     2499 2024-04-03 08:58:18.911442 pyield-0.4.1/tests/test_di.py
--rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 pyield-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3908 2024-03-24 20:00:55.060263 pyield-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-06 18:48:29.912887 pyield-0.5.0/pyield/__about__.py
+-rw-r--r--   0        0        0      428 2024-04-06 05:43:58.958913 pyield-0.5.0/pyield/__init__.py
+-rw-r--r--   0        0        0     7127 2024-04-06 18:37:45.810033 pyield-0.5.0/pyield/anbima.py
+-rw-r--r--   0        0        0    11489 2024-04-06 18:43:46.067542 pyield-0.5.0/pyield/calendar.py
+-rw-r--r--   0        0        0       78 2024-04-06 05:43:41.433643 pyield-0.5.0/pyield/di/__init__.py
+-rw-r--r--   0        0        0     5775 2024-04-06 12:23:44.591710 pyield-0.5.0/pyield/di/core.py
+-rw-r--r--   0        0        0     9680 2024-04-06 12:22:00.239177 pyield-0.5.0/pyield/di/web.py
+-rw-r--r--   0        0        0     9557 2024-04-06 12:23:57.131890 pyield-0.5.0/pyield/di/xml.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.5.0/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.5.0/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.5.0/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2214 2024-04-02 10:06:20.736451 pyield-0.5.0/pyield/holidays/core.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.5.0/pyield/py.typed
+-rw-r--r--   0        0        0     1077 2024-04-06 18:50:20.192255 pyield-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-06 05:41:13.954275 pyield-0.5.0/tests/test_br_calendar.py
+-rw-r--r--   0        0        0     2487 2024-04-06 06:41:17.810251 pyield-0.5.0/tests/test_di.py
+-rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 pyield-0.5.0/PKG-INFO
```

### Comparing `pyield-0.4.1/LICENSE` & `pyield-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.4.1/README.md` & `pyield-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.4.1/pyield/anbima.py` & `pyield-0.5.0/pyield/anbima.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+import io
+
 import pandas as pd
+import requests
+
 from pandas import Timestamp, DataFrame
-from urllib.error import HTTPError
 
-from . import di_futures as di
-from . import br_calendar as cl
+from . import di
+from . import calendar as cl
 
 # URL Constants
 ANBIMA_NON_MEMBER_URL = "https://www.anbima.com.br/informacoes/merc-sec/arqs/"
 ANBIMA_MEMBER_URL = "http://www.anbima.associados.rtm/merc_sec/arqs/"
 
 # Constant for conversion to basis points
-BP_CONVERSION_FACTOR = 10_000
+BPS_CONVERSION_FACTOR = 10_000
 
 
-def normalize_date(reference_date: str | Timestamp | None = None) -> Timestamp:
+def _normalize_date(reference_date: str | Timestamp | None = None) -> Timestamp:
     if isinstance(reference_date, str):
         normalized_date = pd.Timestamp(reference_date).normalize()
     elif isinstance(reference_date, Timestamp):
         normalized_date = reference_date.normalize()
     elif reference_date is None:
         today = pd.Timestamp.today().normalize()
+        # Get last business day before today
         normalized_date = cl.offset_bdays(today, -1)
     else:
         raise ValueError("Invalid date format.")
 
     # Raise an error if the reference date is in the future
     if normalized_date > pd.Timestamp.today().normalize():
         raise ValueError("Reference date cannot be in the future.")
@@ -31,54 +35,59 @@
     # Raise error if the reference date is not a business day
     if not cl.is_business_day(normalized_date):
         raise ValueError("Reference date must be a business day.")
 
     return normalized_date
 
 
-def get_raw_data(
-    reference_date: Timestamp, is_anbima_member: bool = False
-) -> DataFrame:
-    """
-    Fetch indicative rates from ANBIMA for a specific date.
-
-    Parameters:
-    - reference_date (pd.Timestamp): Date for which to fetch the indicative rates.
-    - is_anbima_member (bool): Whether the request is being made by an ANBIMA member.
-
-    Returns:
-    - pd.DataFrame: DataFrame with the indicative rates for the given date.
-    """
-    # Format the date to match the URL format
+def _get_anbima_content(reference_date: Timestamp) -> str:
     url_date = reference_date.strftime("%y%m%d")
+    member_url = f"{ANBIMA_MEMBER_URL}ms{url_date}.txt"
+    non_member_url = f"{ANBIMA_NON_MEMBER_URL}ms{url_date}.txt"
 
-    # Set the base URL according to the member status
-    base_url = ANBIMA_MEMBER_URL if is_anbima_member else ANBIMA_NON_MEMBER_URL
-    # url example: https://www.anbima.com.br/informacoes/merc-sec/arqs/ms231128.txt
-    url = f"{base_url}ms{url_date}.txt"
-
+    # Tries to access the member URL first
     try:
-        df = pd.read_csv(
-            url,
-            sep="@",
-            encoding="latin-1",
-            skiprows=2,
-            decimal=",",
-            thousands=".",
-            na_values=["--"],
-            dtype_backend="numpy_nullable",
-        )
-    except HTTPError:
-        error_date = reference_date.strftime("%d-%m-%Y")
-        raise ValueError(f"Failed to get ANBIMA rates for {error_date}")
+        response = requests.get(member_url)
+        # Checks if the response was successful (status code 200)
+        response.raise_for_status()
+        return response.text
+    except requests.exceptions.RequestException:
+        # Blind attempt to access the member URL
+        pass
 
+    # If the member URL fails, tries to access the non-member URL
+    try:
+        response = requests.get(non_member_url)
+        response.raise_for_status()  # Checks if the second attempt was successful
+        return response.text
+    except requests.exceptions.RequestException:
+        # Both URLs failed
+        return ""
+
+
+def _get_raw_data(reference_date: Timestamp) -> DataFrame:
+    url_content = _get_anbima_content(reference_date)
+    if url_content == "":
+        date_str = reference_date.strftime("%d-%m-%Y")
+        raise ValueError(f"Could not fetch ANBIMA data for {date_str}.")
+
+    df = pd.read_csv(
+        io.StringIO(url_content),
+        sep="@",
+        encoding="latin-1",
+        skiprows=2,
+        decimal=",",
+        thousands=".",
+        na_values=["--"],
+        dtype_backend="numpy_nullable",
+    )
     return df
 
 
-def process_raw_data(df_raw: DataFrame) -> DataFrame:
+def _process_raw_data(df_raw: DataFrame) -> DataFrame:
     """
     Process raw data from ANBIMA by filtering selected columns, renaming them, and adjusting data formats.
 
     Parameters:
     - df (pd.DataFrame): Raw data DataFrame to process.
 
     Returns:
@@ -115,79 +124,75 @@
 
     return df.sort_values(["BondType", "MaturityDate"], ignore_index=True)
 
 
 def get_treasury_rates(
     reference_date: str | Timestamp | None = None,
     return_raw=False,
-    is_anbima_member=False,
 ) -> DataFrame:
     """
     Fetch and process indicative rates from ANBIMA for a specific date.
     If no date is provided, the previous business day based on the Brazilian calendar
     is used.
 
      Parameters:
      - reference_date (str | pd.Timestamp | None): Date for which to fetch the indicative rates.
-        If None, previous business day based on the Brazilian calendar is used.
+        If None, the previous business day based on the Brazilian calendar is used.
      - return_raw (bool): Whether to return raw data without processing.
-     - is_anbima_member (bool): Whether the request is being made by an ANBIMA member.
 
      Returns:
      - pd.DataFrame: DataFrame with the indicative rates for the given date.
     """
 
-    normalized_date = normalize_date(reference_date)
-    df = get_raw_data(normalized_date, is_anbima_member)
+    normalized_date = _normalize_date(reference_date)
+    df = _get_raw_data(normalized_date)
 
     if not return_raw:
-        df = process_raw_data(df)
+        df = _process_raw_data(df)
 
     return df
 
 
 def calculate_treasury_di_spreads(
     reference_date: str | Timestamp | None = None,
-    is_anbima_member=False,
 ) -> DataFrame:
     """
     Calculate the DI spread for LTN and NTN-F bonds based on ANBIMA's indicative rates.
     If no date is provided, the previous business day based on the Brazilian calendar
     is used.
 
     Parameters:
     - reference_date (str | pd.Timestamp | None): The reference date for querying ANBIMA's indicative rates.
         If None, the previous business day based on the Brazilian calendar is used.
-    - is_anbima_member (bool): Specifies whether the request is made by an ANBIMA member.
 
     Returns:
     - pd.DataFrame: A DataFrame containing the bond type, reference date, maturity date, and DI spread in basis points.
     """
     # Validate the reference date, defaulting to the previous business day if not provided
-    normalized_date = normalize_date(reference_date)
+    normalized_date = _normalize_date(reference_date)
 
     # Fetch DI rates and adjust the maturity date format for compatibility
     df_di = di.get_di(normalized_date)[["ExpirationDate", "SettlementRate"]]
 
     # Renaming the columns to match the ANBIMA structure
     df_di.rename(columns={"ExpirationDate": "MaturityDate"}, inplace=True)
 
     # Adjusting maturity date to match bond data format
     df_di["MaturityDate"] = df_di["MaturityDate"].dt.to_period("M").dt.to_timestamp()
 
     # Fetch bond rates, filtering for LTN and NTN-F types
-    df_anbima = get_treasury_rates(normalized_date, False, is_anbima_member)
+    df_anbima = get_treasury_rates(normalized_date, False)
     df_anbima.query("BondType in ['LTN', 'NTN-F']", inplace=True)
 
     # Merge bond and DI rates by maturity date to calculate spreads
     df_final = pd.merge(df_anbima, df_di, how="left", on="MaturityDate")
 
     # Calculating the DI spread as the difference between indicative and settlement rates
     df_final["DISpread"] = df_final["IndicativeRate"] - df_final["SettlementRate"]
 
     # Convert spread to basis points for clarity
-    df_final["DISpread"] = (BP_CONVERSION_FACTOR * df_final["DISpread"]).round(2)
+    df_final["DISpread"] = (BPS_CONVERSION_FACTOR * df_final["DISpread"]).round(2)
 
     # Prepare and return the final sorted DataFrame
     select_columns = ["BondType", "ReferenceDate", "MaturityDate", "DISpread"]
     df_final = df_final[select_columns].copy()
     return df_final.sort_values(["BondType", "MaturityDate"], ignore_index=True)
```

### Comparing `pyield-0.4.1/pyield/br_calendar.py` & `pyield-0.5.0/pyield/calendar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,56 @@
-from typing import Literal, overload
+from typing import Literal, overload, Union
+from datetime import datetime
 
 import numpy as np
 import pandas as pd
-from pandas import Series, Timestamp
 
-from .br_holidays import BrHolidays
 
-# Instância global da classe Holidays
+from .holidays import BrHolidays
+
+SingleDateType = Union[str, np.datetime64, pd.Timestamp, datetime]
+
+SeriesDateType = Union[list, tuple, np.ndarray, pd.Series, pd.Index, pd.DatetimeIndex]
+
+TO_TIMESTAMP_TYPES = (str, np.datetime64, datetime)
+TO_SERIES_TYPES = (list, tuple, np.ndarray, pd.Series, pd.Index, pd.DatetimeIndex)
+
+# Initialize the BrHolidays class
 br_holidays = BrHolidays()
 
 
 @overload
-def normalize_input_dates(dates: str | Timestamp | None) -> Timestamp: ...
+def _normalize_input_dates(
+    dates: SingleDateType | None,
+) -> pd.Timestamp: ...
 
 
 @overload
-def normalize_input_dates(dates: Series) -> Series: ...
+def _normalize_input_dates(
+    dates: SeriesDateType,
+) -> pd.Series: ...
 
 
-def normalize_input_dates(dates: str | Timestamp | Series | None) -> Timestamp | Series:
-    if isinstance(dates, str):
-        return pd.Timestamp(dates).normalize()
-    elif isinstance(dates, Timestamp):
-        return dates.normalize()
-    elif isinstance(dates, Series):
-        return pd.to_datetime(dates)
-    elif dates is None:
+def _normalize_input_dates(
+    dates: SingleDateType | SeriesDateType | None = None,
+) -> pd.Timestamp | pd.Series:
+    if dates is None:
         return pd.Timestamp.today().normalize()
+    elif isinstance(dates, pd.Timestamp):
+        return dates.normalize()
+    elif isinstance(dates, TO_TIMESTAMP_TYPES):
+        return pd.Timestamp(dates).normalize()
+    elif isinstance(dates, TO_SERIES_TYPES):
+        result = pd.to_datetime(dates)
+        return pd.Series(result).dt.normalize()
     else:
         raise ValueError("Invalid date format.")
 
 
-def is_business_day(date: str | Timestamp | None = None) -> bool:
+def is_business_day(date: SingleDateType | None = None) -> bool:
     """
     Checks if the input date is a business day.
 
     Args:
         date (str | Timestamp): The date to check.
 
     Returns:
@@ -43,21 +58,23 @@
 
     Examples:
         >>> yd.is_business_day('2023-12-25') # Christmas
         False
         >>> yd.is_business_day() # Check if today is a business day
         True
     """
-    normalized_date = normalize_input_dates(date)
+    normalized_date = _normalize_input_dates(date)
     # Shift the date if it is not a business day
     adjusted_date = offset_bdays(normalized_date, 0)
     return normalized_date == adjusted_date
 
 
-def convert_to_numpy_date(dates: Timestamp | Series) -> np.datetime64 | np.ndarray:
+def _convert_to_numpy_date(
+    dates: pd.Timestamp | pd.Series,
+) -> np.datetime64 | np.ndarray:
     """
     Converts the input dates to a numpy datetime64[D] format.
 
     Args:
         dates (str | pd.Timestamp | pd.Series): A single date or a Series of dates.
 
     Returns:
@@ -67,36 +84,36 @@
         return np.datetime64(dates, "D")
     else:
         return dates.to_numpy().astype("datetime64[D]")
 
 
 @overload
 def offset_bdays(
-    dates: str | Timestamp | None = None,
+    dates: SingleDateType | None = None,
     offset: int = 0,
     roll: Literal["forward", "backward"] = "forward",
     holiday_list: Literal["old", "new", "infer"] = "infer",
-) -> Timestamp: ...
+) -> pd.Timestamp: ...
 
 
 @overload
 def offset_bdays(
-    dates: Series,
+    dates: SeriesDateType,
     offset: int = 0,
     roll: Literal["forward", "backward"] = "forward",
     holiday_list: Literal["old", "new", "infer"] = "infer",
-) -> Series: ...
+) -> pd.Series: ...
 
 
 def offset_bdays(
-    dates: str | Timestamp | Series | None = None,
+    dates: SingleDateType | SeriesDateType | None = None,
     offset: int = 0,
     roll: Literal["forward", "backward"] = "forward",
     holiday_list: Literal["old", "new", "infer"] = "infer",
-) -> Timestamp | Series:
+) -> pd.Timestamp | pd.Series:
     """
     Offsets the dates to the next or previous business day. This function is a wrapper
     for `numpy.busday_offset` to be used directly with Pandas data types that infers the
     right list of holidays based on the most recent date in the input.
 
     Args:
         dates (str | Timestamp | Series): A single date or a Series of dates to be offset. If
@@ -125,61 +142,69 @@
         >>> yd.offset_bdays(date, 0)
         Timestamp('2023-12-22') # No offset because it's a business day
         >>> yd.offset_bdays(date, 1)
         Timestamp('2023-12-26') # Offset to the next business day
         >>> yd.offset_bdays(date, -1)
         Timestamp('2023-12-21') # Offset to the previous business day
     """
-    normalized_dates = normalize_input_dates(dates)
+    normalized_dates = _normalize_input_dates(dates)
 
     selected_holidays = br_holidays.get_applicable_holidays(
         normalized_dates, holiday_list
     )
-    selected_holidays_np = convert_to_numpy_date(selected_holidays)
+    selected_holidays_np = _convert_to_numpy_date(selected_holidays)
 
-    dates_np = convert_to_numpy_date(normalized_dates)
+    dates_np = _convert_to_numpy_date(normalized_dates)
     offsetted_dates_np = np.busday_offset(
         dates_np, offsets=offset, roll=roll, holidays=selected_holidays_np
     )
     if isinstance(offsetted_dates_np, np.datetime64):
         return pd.Timestamp(offsetted_dates_np, unit="ns")
     else:
         result = pd.to_datetime(offsetted_dates_np, unit="ns")
         return pd.Series(result)
 
 
 @overload
 def count_bdays(
-    start: str | Timestamp | None = None,
-    end: str | Timestamp | None = None,
+    start: SingleDateType | None = None,
+    end: SingleDateType | None = None,
     holiday_list: Literal["old", "new", "infer"] = "infer",
 ) -> int: ...
 
 
 @overload
 def count_bdays(
-    start: Series,
-    end: str | Timestamp | Series | None,
+    start: SeriesDateType,
+    end: SingleDateType | None,
+    holiday_list: Literal["old", "new", "infer"] = "infer",
+) -> pd.Series: ...
+
+
+@overload
+def count_bdays(
+    start: SingleDateType | None,
+    end: SeriesDateType,
     holiday_list: Literal["old", "new", "infer"] = "infer",
-) -> Series: ...
+) -> pd.Series: ...
 
 
 @overload
 def count_bdays(
-    start: str | Timestamp | Series | None,
-    end: Series,
+    start: SeriesDateType,
+    end: SeriesDateType,
     holiday_list: Literal["old", "new", "infer"] = "infer",
-) -> Series: ...
+) -> pd.Series: ...
 
 
 def count_bdays(
-    start: str | Timestamp | Series | None = None,
-    end: str | Timestamp | Series | None = None,
+    start: SingleDateType | SeriesDateType | None = None,
+    end: SingleDateType | SeriesDateType | None = None,
     holiday_list: Literal["old", "new", "infer"] = "infer",
-) -> int | Series:
+) -> int | pd.Series:
     """
     Counts the number of business days between a `start` (inclusive) and `end`
     (exclusive). If an end date is earlier than the start date, the count will be
     negative. This function is a wrapper for `numpy.busday_count` to be used directly
     with Pandas data types.
 
     Args:
@@ -188,15 +213,15 @@
         end (str | Timestamp | Series, optional): The end date. If None, the current date
             is used. Defaults to None.
         holiday_list (str, optional): The list of holidays to use. Defaults to "infer",
             which infers the right list of holidays based on the most recent date in
             the input.
 
     Returns:
-        int | Series: The number of business days between the start date and end date.
+        int | Series | list: The number of business days between the start date and end date.
         Returns an integer if the result is a single value, otherwise returns a Series.
 
     Notes:
         - For more information on error handling, see numpy.busday_count documentation at
             https://numpy.org/doc/stable/reference/generated/numpy.busday_count.html.
         - The maximum start date is used to determine which list of holidays to use. If the
             maximum start date is earlier than 2023-12-26, the list of holidays is
@@ -209,42 +234,41 @@
         10
 
         >>> start = '2023-01-01'
         >>> end = pd.to_datetime(['2023-01-31', '2023-03-01'])
         >>> yd.count_bdays(start, end)
         pd.Series([22, 40], dtype='int64')
     """
-    normalized_start = normalize_input_dates(start)
-    normalized_end = normalize_input_dates(end)
+    normalized_start = _normalize_input_dates(start)
+    normalized_end = _normalize_input_dates(end)
 
     # Determine which list of holidays to use
     selected_holidays = br_holidays.get_applicable_holidays(
         normalized_start, holiday_list
     )
-    selected_holidays_np = convert_to_numpy_date(selected_holidays)
+    selected_holidays_np = _convert_to_numpy_date(selected_holidays)
 
     # Convert inputs to numpy datetime64[D] before calling numpy.busday_count
-    start_np = convert_to_numpy_date(normalized_start)
-    end_np = convert_to_numpy_date(normalized_end)
+    start_np = _convert_to_numpy_date(normalized_start)
+    end_np = _convert_to_numpy_date(normalized_end)
 
     result_np = np.busday_count(start_np, end_np, holidays=selected_holidays_np)
-    if isinstance(result_np, np.ndarray):
-        # Return pandas Int64 type for type consistency
-        return pd.Series(result_np, dtype="Int64")
-    else:
+    if isinstance(result_np, np.int64):
         return int(result_np)
+    else:
+        return pd.Series(result_np, dtype="Int64")
 
 
 def generate_bdays(
-    start: str | Timestamp | None = None,
-    end: str | Timestamp | None = None,
+    start: SingleDateType | None = None,
+    end: SingleDateType | None = None,
     inclusive: Literal["both", "neither", "left", "right"] = "both",
     holiday_list: Literal["old", "new", "infer"] = "infer",
     **kwargs,
-) -> Series:
+) -> pd.Series:
     """
     Generates a Series of business days between a `start` (inclusive) and `end`
     (inclusive) that takes into account the list of brazilian holidays as the default.
     If no start date is provided, the current date is used. If no end date is provided,
     the current date is used.
 
 
@@ -279,19 +303,16 @@
         2023-12-21    2023-12-21
         2023-12-22    2023-12-22
         2023-12-27    2023-12-27
         2023-12-28    2023-12-28
         2023-12-29    2023-12-29
         dtype: object
     """
-    normalized_start = normalize_input_dates(start)
-    normalized_end = normalize_input_dates(end)
-
-    if isinstance(normalized_start, Series) or isinstance(normalized_end, Series):
-        raise ValueError("The start and end dates must be single dates.")
+    normalized_start = _normalize_input_dates(start)
+    normalized_end = _normalize_input_dates(end)
 
     selected_holidays = br_holidays.get_applicable_holidays(
         normalized_start, holiday_list
     )
     selected_holidays_list = selected_holidays.to_list()
 
     result = pd.bdate_range(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyield-0.4.1/pyield/br_holidays.py` & `pyield-0.5.0/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.1/pyield/br_holidays_new.txt` & `pyield-0.5.0/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.4.1/pyield/br_holidays_old.txt` & `pyield-0.5.0/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.4.1/pyield/di_futures.py` & `pyield-0.5.0/pyield/di/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from typing import Literal
 from pathlib import Path
 
 import pandas as pd
 from pandas import DataFrame, Timestamp
 
-from . import di_web as diw
-from . import di_xml as dix
-from . import br_calendar as brc
+from . import web as wb
+from . import xml as dix
+from .. import calendar as cl
 
 
-def normalize_date(trade_date: str | Timestamp | None = None) -> Timestamp:
+def _normalize_date(trade_date: str | Timestamp | None = None) -> Timestamp:
     if isinstance(trade_date, str):
         normalized_date = pd.Timestamp(trade_date).normalize()
     elif isinstance(trade_date, Timestamp):
         normalized_date = trade_date.normalize()
     elif trade_date is None:
         today = pd.Timestamp.today().normalize()
-        normalized_date = brc.offset_bdays(today, -1)
+        # Get last business day before today
+        normalized_date = cl.offset_bdays(today, -1)
     else:
         raise ValueError("Invalid date format.")
 
     # Raise an error if the trade date is in the future
     if normalized_date > pd.Timestamp.today().normalize():
         raise ValueError("Trade date cannot be in the future.")
 
     # Raise error if the reference date is not a business day
-    if not brc.is_business_day(normalized_date):
+    if not cl.is_business_day(normalized_date):
         raise ValueError("Trade date must be a business day.")
 
     return normalized_date
 
 
 def get_expiration_date(expiration_code: str) -> Timestamp:
     """
@@ -84,15 +85,15 @@
         month_code = expiration_code[0]
         month = month_codes[month_code]
         year = int("20" + expiration_code[-2:])
         # The expiration date is always the first business day of the month
         expiration = pd.Timestamp(year, month, 1)
 
         # Adjust to the next business day when expiration date is a weekend or a holiday
-        adj_expiration = brc.offset_bdays(expiration, offset=0)
+        adj_expiration = cl.offset_bdays(expiration, offset=0)
 
         return adj_expiration
 
     except (KeyError, ValueError):
         raise ValueError("Invalid expiration code.")
 
 
@@ -132,18 +133,18 @@
     Notes:
         - The Complete Price Report XML files are approximately 5 MB zipped files.
         - The Simplified Price Report XML files are approximately 50 kB zipped files.
         - File information can be found at: https://www.b3.com.br/data/files/16/70/29/9C/6219D710C8F297D7AC094EA8/Catalogo_precos_v1.3.pdf
 
     """
     # Force trade_date to be a pandas Timestamp
-    normalized_trade_date = normalize_date(trade_date)
+    normalized_trade_date = _normalize_date(trade_date)
 
     if source_type == "bmf":
-        return diw.get_di(normalized_trade_date, return_raw)
+        return wb.get_di(normalized_trade_date, return_raw)
     elif source_type in ["b3", "b3s"]:
         return dix.get_di(normalized_trade_date, source_type, return_raw)
     else:
         raise ValueError("source_type must be either 'bmf', 'b3' or 'b3s'.")
 
 
 def read_di(file_path: Path, return_raw: bool = False) -> DataFrame:
```

### Comparing `pyield-0.4.1/pyield/di_web.py` & `pyield-0.5.0/pyield/di/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import warnings
 from typing import Optional
 
 import pandas as pd
 from pandas import Timestamp, Series, DataFrame
 import requests
 
-from . import br_calendar as brc
-from . import di_futures as dif
+from .. import calendar as cl
+from . import core as cr
 
 
 def get_old_expiration_date(
     ExpirationCode: str, trade_date: Timestamp
 ) -> Optional[Timestamp]:
     """
     Internal function to convert an old DI contract code into its ExpirationDate date. Valid for
@@ -62,21 +62,21 @@
         for year in range(reference_year, reference_year + 10):
             year_codes[str(year)[-1:]] = year
         year = year_codes[ExpirationCode[-1:]]
 
         ExpirationDate = pd.Timestamp(year, month, 1)
         # Adjust to the next business day when ExpirationDate date is a weekend or a holiday
         # Must use the old holiday calendar, since this type of contract code was used until 2006
-        return brc.offset_bdays(ExpirationDate, offset=0, holiday_list="old")
+        return cl.offset_bdays(ExpirationDate, offset=0, holiday_list="old")
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
-def get_raw_di(trade_date: Timestamp) -> DataFrame:
+def _get_raw_di(trade_date: Timestamp) -> DataFrame:
     """
     Internal function to fetch raw DI futures data from B3 for a specific trade date.
 
     Args:
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
@@ -116,15 +116,15 @@
     except Exception as e:
         warnings.warn(
             f"A {type(e).__name__} occurred while reading the DI futures data for {trade_date.strftime('%d/%m/%Y')}. Returning an empty DataFrame."
         )
         return pd.DataFrame()
 
 
-def convert_prices_to_rates(prices: Series, bd: Series) -> Series:
+def _convert_prices_to_rates(prices: Series, bd: Series) -> Series:
     """
     Internal function to convert DI futures prices to rates.
 
     Args:
         prices (pd.Series): A Series containing DI futures prices.
         bd (pd.Series): A Series containing the number of business days to ExpirationDate.
 
@@ -133,35 +133,35 @@
     """
     rates = (100_000 / prices) ** (252 / bd) - 1
 
     # Return rates as percentage
     return 100 * rates
 
 
-def convert_prices_in_older_contracts(df: DataFrame) -> DataFrame:
+def _convert_prices_in_older_contracts(df: DataFrame) -> DataFrame:
     # Prior to 01/01/2002, prices were not converted to rates
     convert_cols = [
         "FirstRate",
         "MinRate",
         "MaxRate",
         "AvgRate",
         "LastRate",
         "LastBidRate",
         "LastAskRate",
     ]
     for col in convert_cols:
-        df[col] = convert_prices_to_rates(df[col], df["BDToExpiration"])
+        df[col] = _convert_prices_to_rates(df[col], df["BDToExpiration"])
 
     # Invert low and high prices
     df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
 
     return df
 
 
-def process_di(df: DataFrame, trade_date: Timestamp) -> DataFrame:
+def _process_di(df: DataFrame, trade_date: Timestamp) -> DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
@@ -201,17 +201,17 @@
 
     # Contract code format was changed in 22/05/2006
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
             get_old_expiration_date, args=(trade_date,)
         )
     else:
-        df["ExpirationDate"] = df["ExpirationCode"].apply(dif.get_expiration_date)
+        df["ExpirationDate"] = df["ExpirationCode"].apply(cr.get_expiration_date)
 
-    df["BDToExpiration"] = brc.count_bdays(trade_date, df["ExpirationDate"])
+    df["BDToExpiration"] = cl.count_bdays(trade_date, df["ExpirationDate"])
     # Convert to nullable integer, since other columns use this data type
     df["BDToExpiration"] = df["BDToExpiration"].astype(pd.Int64Dtype())
     # Remove expired contracts
     df.query("BDToExpiration > 0", inplace=True)
 
     # Columns where 0 means NaN
     cols_with_nan = [
@@ -225,17 +225,17 @@
         "LastAskRate",
     ]
     for col in cols_with_nan:
         df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
 
     # Prior to 17/01/2002 (incluive), prices were not converted to rates
     if trade_date <= pd.Timestamp("2002-01-17"):
-        df = convert_prices_in_older_contracts(df)
+        df = _convert_prices_in_older_contracts(df)
 
-    df["SettlementRate"] = convert_prices_to_rates(
+    df["SettlementRate"] = _convert_prices_to_rates(
         df["SettlementPrice"], df["BDToExpiration"]
     )
 
     # Remove percentage in all rate columns and round to 5 decimal places since it's the precision used by B3
     # Obs: 5 decimal places = 3 decimal places in percentage
     rate_cols = [col for col in df.columns if "Rate" in col]
     for col in rate_cols:
@@ -285,11 +285,11 @@
         >>> get_di("2023-12-28")
 
     Notes:
         - BDToExpiration: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
         - closed_contracts: number of closed contracts at the end of the trading day.
     """
-    df_raw = get_raw_di(trade_date)
+    df_raw = _get_raw_di(trade_date)
     if return_raw:
         return df_raw
-    return process_di(df_raw, trade_date)
+    return _process_di(df_raw, trade_date)
```

### Comparing `pyield-0.4.1/pyield/di_xml.py` & `pyield-0.5.0/pyield/di/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from pathlib import Path
 
 import requests
 import pandas as pd
 from pandas import Timestamp, DataFrame
 from lxml import etree
 
-from . import di_futures as dif
-from . import br_calendar as brc
+from . import core as cr
+from .. import calendar as cd
 
 
-def get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
+def _get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
     """
     Types of XML files available:
     Full Price Report (all assets)
         - aprox. 5 MB zipped file;
         - url example: https://www.b3.com.br/pesquisapregao/download?filelist=PR231228.zip
     Simplified Price Report (derivatives)
         - aprox. 50kB zipped file;
@@ -35,15 +35,15 @@
     if response.status_code != 200 or len(response.content) < 1024:
         formatted_date = trade_date.strftime("%Y-%m-%d")
         raise ValueError(f"There is no data available for {formatted_date}.")
 
     return io.BytesIO(response.content)
 
 
-def extract_xml_from_zip(zip_file: io.BytesIO) -> io.BytesIO:
+def _extract_xml_from_zip(zip_file: io.BytesIO) -> io.BytesIO:
     # First, read the outer file
     with zipfile.ZipFile(zip_file, "r") as outer_zip:
         outer_file_name = outer_zip.namelist()[0]
         outer_file_content = outer_zip.read(outer_file_name)
     outer_file = io.BytesIO(outer_file_content)
 
     # Then, read the inner file
@@ -54,15 +54,15 @@
         xml_filenames.sort()
         # Unzip last file (the most recent as per B3's name convention)
         inner_file_content = inner_zip.read(xml_filenames[-1])
 
     return io.BytesIO(inner_file_content)
 
 
-def extract_di_data_from_xml(xml_file: io.BytesIO) -> list[dict]:
+def _extract_di_data_from_xml(xml_file: io.BytesIO) -> list[dict]:
     parser = etree.XMLParser(
         ns_clean=True, remove_blank_text=True, remove_comments=True, recover=True
     )
     tree = etree.parse(xml_file, parser)
     namespaces = {"ns": "urn:bvmf.217.01.xsd"}
 
     # XPath para encontrar elementos cujo texto começa com "DI1"
@@ -116,24 +116,24 @@
 
         # Adicionar o dicionário à lista
         di_data.append(ticker_data)
 
     return di_data
 
 
-def create_df_from_di_data(di1_data: list) -> DataFrame:
+def _create_df_from_di_data(di1_data: list) -> DataFrame:
     # Criar um DataFrame com os dados coletados
     df = pd.DataFrame(di1_data)
 
     # Convert to CSV and then back to pandas to get automatic type conversion
     file = io.StringIO(df.to_csv(index=False))
     return pd.read_csv(file, dtype_backend="numpy_nullable")
 
 
-def filter_and_order_pr_df(df: DataFrame) -> DataFrame:
+def _filter_and_order_pr_df(df: DataFrame) -> DataFrame:
     selected_columns = [
         "TradDt",
         "TckrSymb",
         # "MktDataStrmId",
         "OpnIntrst",
         "FinInstrmQty",
         "NtlFinVol",
@@ -161,15 +161,15 @@
         # "VartnPts",
         # "AdjstdValCtrct",
     ]
 
     return df[selected_columns]
 
 
-def filter_and_order_sprd_df(df: DataFrame) -> DataFrame:
+def _filter_and_order_sprd_df(df: DataFrame) -> DataFrame:
     cols = [
         "TradDt",
         "TckrSymb",
         "OpnIntrst",
         "AdjstdQt",
         "MinPric",
         "TradAvrgPric",
@@ -183,15 +183,15 @@
         # "PrvsAdjstdQtTax",
         # "PrvsAdjstdQtStin",  # Constant column
     ]
 
     return df[cols]
 
 
-def standardize_column_names(df: DataFrame) -> DataFrame:
+def _standardize_column_names(df: DataFrame) -> DataFrame:
     rename_dict = {
         "TradDt": "TradeDate",
         "TckrSymb": "Ticker",
         # "MktDataStrmId"
         # "IntlFinVol",
         "OpnIntrst": "OpenContracts",
         "FinInstrmQty": "TradedQuantity",
@@ -220,90 +220,90 @@
         # "VartnPts",
         # "AdjstdValCtrct",
     }
 
     return df.rename(columns=rename_dict)
 
 
-def process_di_df(df_raw: DataFrame) -> DataFrame:
+def _process_di_df(df_raw: DataFrame) -> DataFrame:
     df = df_raw.copy()
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradDt"] = df["TradDt"].astype("datetime64[ns]")
 
-    expiration = df["TckrSymb"].str[3:].apply(dif.get_expiration_date)
+    expiration = df["TckrSymb"].str[3:].apply(cr.get_expiration_date)
     df.insert(2, "ExpirationDate", expiration)
 
-    business_days = brc.count_bdays(df["TradDt"], df["ExpirationDate"])
+    business_days = cd.count_bdays(df["TradDt"], df["ExpirationDate"])
     df.insert(3, "BDToExpiration", business_days)
 
     # Convert to nullable integer, since other columns use this data type
     df["BDToExpiration"] = df["BDToExpiration"].astype(pd.Int64Dtype())
 
     # Remove expired contracts
     df.query("BDToExpiration > 0", inplace=True)
 
     return df.sort_values(by=["ExpirationDate"], ignore_index=True)
 
 
 def get_di(trade_date: Timestamp, source_type: str, return_raw: bool) -> DataFrame:
-    zip_file = get_file_from_url(trade_date, source_type)
+    zip_file = _get_file_from_url(trade_date, source_type)
 
-    xml_file = extract_xml_from_zip(zip_file)
+    xml_file = _extract_xml_from_zip(zip_file)
 
-    di_data = extract_di_data_from_xml(xml_file)
+    di_data = _extract_di_data_from_xml(xml_file)
 
-    df_raw = create_df_from_di_data(di_data)
+    df_raw = _create_df_from_di_data(di_data)
     if return_raw:
         return df_raw
 
     # Remove unnecessary columns
     if source_type == "b3":
-        df_di = filter_and_order_pr_df(df_raw)
+        df_di = _filter_and_order_pr_df(df_raw)
     elif source_type == "b3s":
-        df_di = filter_and_order_sprd_df(df_raw)
+        df_di = _filter_and_order_sprd_df(df_raw)
     else:
         raise ValueError("Invalid source type. Must be 'b3' or 'b3s'.")
 
     # Process and transform data
-    df_di = process_di_df(df_di)
+    df_di = _process_di_df(df_di)
 
     # Standardize column names
-    df_di = standardize_column_names(df_di)
+    df_di = _standardize_column_names(df_di)
 
     return df_di
 
 
 def read_di(file_path: Path, return_raw: bool = False) -> DataFrame:
     if file_path:
         if file_path.exists():
             content = file_path.read_bytes()
             zip_file = io.BytesIO(content)
         else:
             raise FileNotFoundError(f"No file found at {file_path}.")
 
-        xml_file = extract_xml_from_zip(zip_file)
+        xml_file = _extract_xml_from_zip(zip_file)
 
-        di_data = extract_di_data_from_xml(xml_file)
+        di_data = _extract_di_data_from_xml(xml_file)
 
-        df_raw = create_df_from_di_data(di_data)
+        df_raw = _create_df_from_di_data(di_data)
         if return_raw:
             return df_raw
 
         # Filename examples: PR231228.zip or SPRD240216.zip
         file_stem = file_path.stem
         if "PR" in file_stem:
-            df_di = filter_and_order_pr_df(df_raw)
+            df_di = _filter_and_order_pr_df(df_raw)
         elif "SPRD" in file_stem:
-            df_di = filter_and_order_sprd_df(df_raw)
+            df_di = _filter_and_order_sprd_df(df_raw)
         else:
             raise ValueError("Filename must start with 'PR' or 'SPRD'.")
 
         # Process and transform data
-        df_di = process_di_df(df_di)
+        df_di = _process_di_df(df_di)
 
         # Standardize column names
-        df_di = standardize_column_names(df_di)
+        df_di = _standardize_column_names(df_di)
 
         return df_di
 
     else:
         raise ValueError("A file path must be provided.")
```

### Comparing `pyield-0.4.1/pyproject.toml` & `pyield-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.4.1"
+version = "0.5.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.4.1/tests/test_br_calendar.py` & `pyield-0.5.0/tests/test_br_calendar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import pandas as pd
 import numpy as np
 
-from pyield import br_calendar as brc
+from pyield import calendar as cl
 
 
 def test_count_bdays_1():
     start = "2023-01-01"
     end = "2023-01-08"
     # 01/01/2023 is a Sunday and a holiday
-    assert brc.count_bdays(start, end) == 5
+    assert cl.count_bdays(start, end) == 5
 
 
 def test_count_bdays_2():
     start = "2023-12-15"
     end = "2024-01-02"
     # 25/12/2023 is a holiday
     # 01/01/2024 is a holiday
-    assert brc.count_bdays(start, end) == 10
+    assert cl.count_bdays(start, end) == 10
 
 
 def test_count_bdays_with_series():
     start = "2023-01-01"
     end = pd.Series(["2023-01-08", "2023-01-22"])
     # Assuming no holidays in these periods
-    assert np.array_equal(brc.count_bdays(start, end), np.array([5, 15]))
+    assert np.array_equal(cl.count_bdays(start, end), np.array([5, 15]))
 
 
 def test_count_bdays_negative_count():
     start = "2023-01-08"
     end = "2023-01-01"
     # Negative count expected
-    assert brc.count_bdays(start, end) == -5
+    assert cl.count_bdays(start, end) == -5
 
 
 def test_count_bdays_new_holiday_list():
     start = "2024-11-20"  # Zumbi Nacional Day
     end = "2024-11-21"
-    assert brc.count_bdays(start, end) == 0
+    assert cl.count_bdays(start, end) == 0
 
 
 def test_count_bdays_old_holiday_list():
     start = "2020-11-20"  # Was not a holiday in 2020
     end = "2020-11-21"
-    assert brc.count_bdays(start, end) == 1
+    assert cl.count_bdays(start, end) == 1
```

### Comparing `pyield-0.4.1/tests/test_di.py` & `pyield-0.5.0/tests/test_di.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import pandas as pd
 import pytest
 
-from pyield import di_futures as dif
-from pyield import di_web as diw
+from pyield.di import core as cr
+from pyield.di import web as wb
 
 
 def test_valid_old_contract_code1():
     expiration_code = "JAN3"  # Valid contract code
     trade_date = pd.Timestamp("2001-05-21")
-    result = diw.get_old_expiration_date(expiration_code, trade_date)
+    result = wb.get_old_expiration_date(expiration_code, trade_date)
     contract_expiration = pd.Timestamp("2003-01-02")
     assert result == contract_expiration
 
 
 def test_valid_old_contract_code2():
     expiration_code = "JAN3"  # Valid contract code
     trade_date = pd.Timestamp("1990-01-01")
-    result = diw.get_old_expiration_date(expiration_code, trade_date)
+    result = wb.get_old_expiration_date(expiration_code, trade_date)
     contract_expiration = pd.Timestamp("1993-01-04")
     assert result == contract_expiration
 
 
 def test_invalid_old_contract_code():
     expiration_code = "J3"  # Invalid contract code
     trade_date = pd.Timestamp("2001-01-02")
     # Must return NaT
-    result = diw.get_old_expiration_date(expiration_code, trade_date)
+    result = wb.get_old_expiration_date(expiration_code, trade_date)
     assert pd.isnull(result)
 
 
 def test_new_contract_code():
     expiration_code = "F23"  # Valid contract code
-    result = dif.get_expiration_date(expiration_code)
+    result = cr.get_expiration_date(expiration_code)
     contract_expiration = pd.Timestamp("2023-01-02")
     assert result == contract_expiration
 
 
 def test_settlement_rate_with_old_holiday_list():
     settlement_rates = {
         "N27": 0.09809,
         "F33": 0.10368,
     }
 
     # 22-12-2023 is before the new holiday calendar
-    df = dif.get_di(trade_date="2023-12-22")
+    df = cr.get_di(trade_date="2023-12-22")
     expiration_codes = list(settlement_rates.keys())  # noqa: F841
     result = df.query("ExpirationCode in @expiration_codes")["SettlementRate"].to_list()
     assert result == list(settlement_rates.values())
 
 
 def test_settlement_rates_with_current_holiday_list():
     settlement_rates = {
@@ -64,19 +64,19 @@
         "F27": 0.09683,
         "N27": 0.09794,
         "F29": 0.10042,
         "F31": 0.10240,
         "F33": 0.10331,
     }
 
-    df = dif.get_di(trade_date="2023-12-26")
+    df = cr.get_di(trade_date="2023-12-26")
     expiration_codes = list(settlement_rates.keys())  # noqa: F841
     results = df.query("ExpirationCode in @expiration_codes")[
         "SettlementRate"
     ].to_list()
     assert results == list(settlement_rates.values())
 
 
 def test_non_business_day():
     non_business_day = "2023-12-24"
     with pytest.raises(ValueError):
-        dif.get_di(trade_date=non_business_day)
+        cr.get_di(trade_date=non_business_day)
```

### Comparing `pyield-0.4.1/PKG-INFO` & `pyield-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
```

