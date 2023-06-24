# Comparing `tmp/nselib-0.4.tar.gz` & `tmp/nselib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nselib-0.4.tar", last modified: Tue Jun 20 01:41:41 2023, max compression
+gzip compressed data, was "nselib-0.5.tar", last modified: Sat Jun 24 15:00:36 2023, max compression
```

## Comparing `nselib-0.4.tar` & `nselib-0.5.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.571295 nselib-0.4/
--rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3856 2023-06-20 01:41:41.571295 nselib-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3163 2023-06-20 01:20:48.000000 nselib-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.549257 nselib-0.4/nselib/
--rw-rw-rw-   0        0        0       68 2023-06-20 01:25:54.000000 nselib-0.4/nselib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.561293 nselib-0.4/nselib/capital_market/
--rw-rw-rw-   0        0        0      286 2023-06-20 01:15:48.000000 nselib-0.4/nselib/capital_market/__init__.py
--rw-rw-rw-   0        0        0    16203 2023-06-20 01:25:54.000000 nselib-0.4/nselib/capital_market/capital_market_data.py
--rw-rw-rw-   0        0        0     2133 2023-06-19 17:43:08.000000 nselib-0.4/nselib/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.563257 nselib-0.4/nselib/debt/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.4/nselib/debt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.568257 nselib-0.4/nselib/derivatives/
--rw-rw-rw-   0        0        0      168 2023-06-19 13:36:13.000000 nselib-0.4/nselib/derivatives/__init__.py
--rw-rw-rw-   0        0        0     9032 2023-06-20 01:08:27.000000 nselib-0.4/nselib/derivatives/derivative_data.py
--rw-rw-rw-   0        0        0     4495 2023-06-20 01:00:15.000000 nselib-0.4/nselib/libutil.py
--rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.4/nselib/logger.py
--rw-rw-rw-   0        0        0       15 2023-06-20 01:25:54.000000 nselib-0.4/nselib/version.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.557257 nselib-0.4/nselib.egg-info/
--rw-rw-rw-   0        0        0     3856 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-20 01:41:41.572296 nselib-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-06-20 01:40:52.000000 nselib-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.901224 nselib-0.5/
+-rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4004 2023-06-24 15:00:36.901224 nselib-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3311 2023-06-24 14:56:54.000000 nselib-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.748499 nselib-0.5/nselib/
+-rw-rw-rw-   0        0        0       68 2023-06-24 14:50:51.000000 nselib-0.5/nselib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.792185 nselib-0.5/nselib/capital_market/
+-rw-rw-rw-   0        0        0      330 2023-06-24 13:55:00.000000 nselib-0.5/nselib/capital_market/__init__.py
+-rw-rw-rw-   0        0        0    23344 2023-06-24 14:49:21.000000 nselib-0.5/nselib/capital_market/capital_market_data.py
+-rw-rw-rw-   0        0        0     2556 2023-06-24 10:49:29.000000 nselib-0.5/nselib/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.828662 nselib-0.5/nselib/debt/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.5/nselib/debt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.864619 nselib-0.5/nselib/derivatives/
+-rw-rw-rw-   0        0        0      273 2023-06-24 14:43:31.000000 nselib-0.5/nselib/derivatives/__init__.py
+-rw-rw-rw-   0        0        0    16766 2023-06-24 14:49:21.000000 nselib-0.5/nselib/derivatives/derivative_data.py
+-rw-rw-rw-   0        0        0     4841 2023-06-24 10:07:44.000000 nselib-0.5/nselib/libutil.py
+-rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.5/nselib/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.755435 nselib-0.5/nselib.egg-info/
+-rw-rw-rw-   0        0        0     4004 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-24 15:00:36.902261 nselib-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-06-24 14:50:51.000000 nselib-0.5/setup.py
```

### Comparing `nselib-0.4/LICENSE` & `nselib-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nselib-0.4/PKG-INFO` & `nselib-0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.4
+Version: 0.5
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.4
+# NSElib 0.5
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -57,18 +57,20 @@
 * price_volume_and_deliverable_position_data 
 * price_volume_data
 * deliverable_position_data
 * bulk_deal_data
 * block_deals_data
 * short_selling_data
 * bhav_copy_with_delivery
-* bhav_copy
+* bhav_copy_equities
 * equity_list
 * fno_equity_list
 * nifty50_equity_list
+* india_vix_data
+* index_data
 
 Example : 
 
 from nselib import capital_market 
 
 data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
                                             
@@ -80,14 +82,18 @@
 
 ### Derivative
 * future_price_volume_data
 * option_price_volume_data
 * fno_bhav_copy
 * participant_wise_open_interest
 * participant_wise_trading_volume
+* expiry_dates_future
+* expiry_dates_option_index
+* nse_live_option_chain
+* fii_derivatives_statistics
 
 Example : 
 
 from nselib import derivatives
 
 data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
```

### Comparing `nselib-0.4/README.md` & `nselib-0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NSElib 0.4
+# NSElib 0.5
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -39,18 +39,20 @@
 * price_volume_and_deliverable_position_data 
 * price_volume_data
 * deliverable_position_data
 * bulk_deal_data
 * block_deals_data
 * short_selling_data
 * bhav_copy_with_delivery
-* bhav_copy
+* bhav_copy_equities
 * equity_list
 * fno_equity_list
 * nifty50_equity_list
+* india_vix_data
+* index_data
 
 Example : 
 
 from nselib import capital_market 
 
 data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
                                             
@@ -62,14 +64,18 @@
 
 ### Derivative
 * future_price_volume_data
 * option_price_volume_data
 * fno_bhav_copy
 * participant_wise_open_interest
 * participant_wise_trading_volume
+* expiry_dates_future
+* expiry_dates_option_index
+* nse_live_option_chain
+* fii_derivatives_statistics
 
 Example : 
 
 from nselib import derivatives
 
 data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
```

### Comparing `nselib-0.4/nselib/capital_market/capital_market_data.py` & `nselib-0.5/nselib/capital_market/capital_market_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import datetime as dt
-import time
 import zipfile
 from io import BytesIO, StringIO
 from nselib.libutil import *
 from nselib.constants import *
 
 
 def price_volume_and_deliverable_position_data(symbol: str, from_date: str = None, to_date: str = None,
@@ -16,14 +15,15 @@
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,'1W': for last 7 days data,
                             '1M': from last month same date, '6M': last 6 month data, '1Y': from last year same date)
     :return: pandas.DataFrame
     :raise ValueError if the parameter input is not proper
     """
     validate_date_param(from_date, to_date, period)
+    symbol = cleaning_nse_symbol(symbol=symbol)
     from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
     nse_df = pd.DataFrame(columns=price_volume_and_deliverable_position_data_columns)
     from_date = datetime.strptime(from_date, dd_mm_yyyy)
     to_date = datetime.strptime(to_date, dd_mm_yyyy)
     load_days = (to_date - from_date).days
     while load_days > 0:
         if load_days > 365:
@@ -36,23 +36,24 @@
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
 def get_price_volume_and_deliverable_position_data(symbol: str, from_date: str, to_date: str):
-    # print(from_date, to_date)
-    data_df = pd.DataFrame()
     url = "https://www.nseindia.com/api/historical/securityArchives?"
     payload = f"from={from_date}&to={to_date}&symbol={symbol}&dataType=priceVolumeDeliverable&series=ALL&csv=true"
-    data_text = nse_urlfetch(url + payload).text
-    data_text = data_text.replace('\x82', '').replace('â¹', 'In Rs')
-    with open('file.csv', 'w') as f:
-        f.write(data_text)
-    f.close()
+    try:
+        data_text = nse_urlfetch(url + payload).text
+        data_text = data_text.replace('\x82', '').replace('â¹', 'In Rs')
+        with open('file.csv', 'w') as f:
+            f.write(data_text)
+        f.close()
+    except Exception as e:
+        raise NSEdataNotFound(f" Resource not available MSG: {e}")
     data_df = pd.read_csv('file.csv')
     data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
 def price_volume_data(symbol: str, from_date: str = None, to_date: str = None, period: str = None):
     """
@@ -62,14 +63,15 @@
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,'1W': for last 7 days data,
                             '1M': from last month same date, '6M': last 6 month data, '1Y': from last year same date)
     :return: pandas.DataFrame
     :raise ValueError if the parameter input is not proper
     """
     validate_date_param(from_date, to_date, period)
+    symbol = cleaning_nse_symbol(symbol=symbol)
     from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
     nse_df = pd.DataFrame(columns=price_volume_data_columns)
     from_date = datetime.strptime(from_date, dd_mm_yyyy)
     to_date = datetime.strptime(to_date, dd_mm_yyyy)
     load_days = (to_date - from_date).days
     while load_days > 0:
         if load_days > 365:
@@ -82,21 +84,23 @@
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
 def get_price_volume_data(symbol: str, from_date: str, to_date: str):
-    # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/securityArchives?"
     payload = f"from={from_date}&to={to_date}&symbol={symbol}&dataType=priceVolume&series=ALL&csv=true"
-    data_text = nse_urlfetch(url + payload).text
-    with open('file.csv', 'w') as f:
-        f.write(data_text)
-    f.close()
+    try:
+        data_text = nse_urlfetch(url + payload).text
+        with open('file.csv', 'w') as f:
+            f.write(data_text)
+        f.close()
+    except Exception as e:
+        raise NSEdataNotFound(f" Resource not available MSG: {e}")
     data_df = pd.read_csv('file.csv')
     data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
 def deliverable_position_data(symbol: str, from_date: str = None, to_date: str = None, period: str = None):
     """
@@ -109,14 +113,15 @@
                             '1M': from last month same date,
                             '6M': last 6 month data,
                             '1Y': from last year same date)
     :return: pandas.DataFrame
     :raise ValueError if the parameter input is not proper
     """
     validate_date_param(from_date, to_date, period)
+    symbol = cleaning_nse_symbol(symbol=symbol)
     from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
     nse_df = pd.DataFrame(columns=deliverable_data_columns)
     from_date = datetime.strptime(from_date, dd_mm_yyyy)
     to_date = datetime.strptime(to_date, dd_mm_yyyy)
     load_days = (to_date - from_date).days
     while load_days > 0:
         if load_days > 365:
@@ -129,27 +134,119 @@
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
 def get_deliverable_position_data(symbol: str, from_date: str, to_date: str):
-    # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/securityArchives?"
     payload = f"from={from_date}&to={to_date}&symbol={symbol}&dataType=deliverable&series=ALL&csv=true"
-    data_text = nse_urlfetch(url + payload).text
+    try:
+        data_text = nse_urlfetch(url + payload).text
+    except Exception as e:
+        raise NSEdataNotFound(f" Resource not available MSG: {e}")
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
     data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
+def india_vix_data(from_date: str = None, to_date: str = None, period: str = None):
+    """
+    get india vix spot data  set for the specific time period.
+    :param from_date: '17-03-2022' ('dd-mm-YYYY')
+    :param to_date: '17-06-2023' ('dd-mm-YYYY')
+    :param period: use one {'1D': last day data,'1W': for last 7 days data,
+                            '1M': from last month same date, '6M': last 6 month data, '1Y': from last year same date)
+    :return: pandas.DataFrame
+    :raise ValueError if the parameter input is not proper
+    """
+    validate_date_param(from_date, to_date, period)
+    from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
+    nse_df = pd.DataFrame(columns=india_vix_data_column)
+    from_date = datetime.strptime(from_date, dd_mm_yyyy)
+    to_date = datetime.strptime(to_date, dd_mm_yyyy)
+    load_days = (to_date - from_date).days
+    while load_days > 0:
+        if load_days > 365:
+            end_date = (from_date + dt.timedelta(364)).strftime(dd_mm_yyyy)
+            start_date = from_date.strftime(dd_mm_yyyy)
+        else:
+            end_date = to_date.strftime(dd_mm_yyyy)
+            start_date = from_date.strftime(dd_mm_yyyy)
+        data_df = get_india_vix_data(from_date=start_date, to_date=end_date)
+        from_date = from_date + dt.timedelta(365)
+        load_days = (to_date - from_date).days
+        nse_df = pd.concat([nse_df, data_df], ignore_index=True)
+    return nse_df
+
+
+def get_india_vix_data(from_date: str, to_date: str):
+    url = f"https://www.nseindia.com/api/historical/vixhistory?from={from_date}&to={to_date}&csv=true"
+    try:
+        data_json = nse_urlfetch(url).json()
+        data_df = pd.DataFrame(data_json['data'])
+    except Exception as e:
+        raise NSEdataNotFound(f" Resource not available MSG: {e}")
+    data_df.drop(columns='TIMESTAMP', inplace=True)
+    data_df.columns = cleaning_column_name(data_df.columns)
+    return data_df[india_vix_data_column]
+
+
+def index_data(index:str, from_date: str = None, to_date: str = None, period: str = None):
+    """
+    get historical index data set for the specific time period.
+    apply the index name as per the nse india site
+    :param index: 'NIFTY 50'/'NIFTY BANK'
+    :param from_date: '17-03-2022' ('dd-mm-YYYY')
+    :param to_date: '17-06-2023' ('dd-mm-YYYY')
+    :param period: use one {'1D': last day data,'1W': for last 7 days data,
+                            '1M': from last month same date, '6M': last 6 month data, '1Y': from last year same date)
+    :return: pandas.DataFrame
+    :raise ValueError if the parameter input is not proper
+    """
+    validate_date_param(from_date, to_date, period)
+    from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
+    nse_df = pd.DataFrame(columns=index_data_columns)
+    from_date = datetime.strptime(from_date, dd_mm_yyyy)
+    to_date = datetime.strptime(to_date, dd_mm_yyyy)
+    load_days = (to_date - from_date).days
+    while load_days > 0:
+        if load_days > 365:
+            end_date = (from_date + dt.timedelta(364)).strftime(dd_mm_yyyy)
+            start_date = from_date.strftime(dd_mm_yyyy)
+        else:
+            end_date = to_date.strftime(dd_mm_yyyy)
+            start_date = from_date.strftime(dd_mm_yyyy)
+        data_df = get_index_data(index=index, from_date=start_date, to_date=end_date)
+        from_date = from_date + dt.timedelta(365)
+        load_days = (to_date - from_date).days
+        nse_df = pd.concat([nse_df, data_df], ignore_index=True)
+    return nse_df
+
+
+def get_index_data(index:str, from_date: str, to_date: str):
+    index = index.replace(' ', '%20').upper()
+    url = f"https://www.nseindia.com/api/historical/indicesHistory?indexType={index}&from={from_date}&to={to_date}"
+    try:
+        data_json = nse_urlfetch(url).json()
+        data_close_df = pd.DataFrame(data_json['data']['indexCloseOnlineRecords']).drop(columns=['_id', "EOD_TIMESTAMP"])
+        data_turnover_df = pd.DataFrame(data_json['data']['indexTurnoverRecords']).drop(columns=['_id',
+                                                                                                 'HIT_INDEX_NAME_UPPER'])
+        data_df = pd.merge(data_close_df,data_turnover_df, on='TIMESTAMP', how='inner')
+    except Exception as e:
+        raise NSEdataNotFound(f" Resource not available MSG: {e}")
+    data_df.drop(columns='TIMESTAMP', inplace=True)
+    data_df.columns = cleaning_column_name(data_df.columns)
+    return data_df[index_data_columns]
+
+
 def bulk_deal_data(from_date: str = None, to_date: str = None, period: str = None):
     """
     get bulk deal data set.
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
@@ -274,39 +371,50 @@
 
 
 def get_short_selling_data(from_date: str, to_date: str):
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/short-selling?"
     payload = f"from={from_date}&to={to_date}&csv=true"
     data_text = nse_urlfetch(url + payload).text
+    print((url + payload))
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
     data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
 def bhav_copy_with_delivery(trade_date: str):
+    """
+    get the NSE bhav copy with delivery data as per the traded date
+    :param trade_date: eg:'01-06-2023'
+    :return: pandas data frame
+    """
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     use_date = trade_date.strftime(ddmmyyyy)
     url = f'https://archives.nseindia.com/products/content/sec_bhavdata_full_{use_date}.csv'
     request_bhav = nse_urlfetch(url)
     bhav_df = pd.DataFrame()
     if request_bhav.status_code == 200:
         bhav_df = pd.read_csv(StringIO(request_bhav.text), sep=', ', engine='python')
     elif request_bhav.status_code == 403:
         raise FileNotFoundError(f' Data not found, change the date...')
     return bhav_df[['SYMBOL', 'SERIES', 'OPEN_PRICE', 'HIGH_PRICE', 'LOW_PRICE', 'CLOSE_PRICE',
                     'PREV_CLOSE', 'TTL_TRD_QNTY', 'TURNOVER_LACS', 'NO_OF_TRADES', 'DELIV_QTY',
                     'DELIV_PER', 'DATE1']]
 
 
-def bhav_copy(trade_date: str):
+def bhav_copy_equities(trade_date: str):
+    """
+    get nse bhav copy as per the traded date provided
+    :param trade_date:
+    :return: pandas dataframe
+    """
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     url = 'https://archives.nseindia.com/content/historical/EQUITIES/'
     payload = f"{str(trade_date.strftime('%Y'))}/{str(trade_date.strftime('%b').upper())}/" \
               f"cm{str(trade_date.strftime('%d%b%Y').upper())}bhav.csv.zip"
     request_bhav = nse_urlfetch(url + payload)
     bhav_df = pd.DataFrame()
     if request_bhav.status_code == 200:
@@ -317,33 +425,76 @@
     elif request_bhav.status_code == 403:
         raise FileNotFoundError(f' Data not found, change the date...')
     bhav_df = bhav_df[['SYMBOL', 'SERIES', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'LAST', 'PREVCLOSE', 'TOTTRDQTY',
                        'TOTTRDVAL', 'TIMESTAMP', 'TOTALTRADES']]
     return bhav_df
 
 
+def bhav_copy_indices(trade_date: str):
+    """
+    get nse bhav copy as per the traded date provided
+    :param trade_date: eg:'01-06-2023'
+    :return: pandas dataframe
+    """
+    trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
+    url = f"https://archives.nseindia.com/content/indices/ind_close_all_{str(trade_date.strftime('%d%m%Y').upper())}.csv"
+    try:
+        bhav_df = pd.read_csv(url)
+    except Exception as e:
+        raise FileNotFoundError(f' Bhav copy indices not found for : {trade_date} :: NSE error : {e}')
+    return bhav_df
+
+
 def equity_list():
-    data_df = pd.read_csv("https://archives.nseindia.com/content/equities/EQUITY_L.csv")
+    """
+    get list of all equity available to trade in NSE
+    :return: pandas data frame
+    """
+    try:
+        data_df = pd.read_csv("https://archives.nseindia.com/content/equities/EQUITY_L.csv")
+    except Exception as e:
+        raise FileNotFoundError(f' Equity List not found :: NSE error : {e}')
     data_df = data_df[['SYMBOL', 'NAME OF COMPANY', ' SERIES', ' DATE OF LISTING', ' FACE VALUE']]
     return data_df
 
 
 def fno_equity_list():
-    data_df = pd.read_csv("https://archives.nseindia.com/content/fo/fo_mktlots.csv", skiprows=5)
+    """
+    get a dataframe of all listed derivative list with the recent lot size to trade
+    :return: pandas data frame
+    """
     today = dt.date.today()
     MMM_YY = today.strftime(mmm_yy).upper()
+    try:
+        ind_data_df = pd.read_csv("https://archives.nseindia.com/content/fo/fo_mktlots.csv")
+        data_df = pd.read_csv("https://archives.nseindia.com/content/fo/fo_mktlots.csv", skiprows=5)
+    except Exception as e:
+        raise FileNotFoundError(f' all listed derivative List not found :: NSE error : {e}')
+
+    ind_data_df.columns = [name.replace('    ', '').replace(' ', '') for name in ind_data_df.columns]
+    ind_data_df = ind_data_df[['UNDERLYING', 'SYMBOL', f'{MMM_YY}']].head(4)
+    ind_data_df.columns = ['Company_Name', 'Symbol', f'{MMM_YY}']
     data_df.rename(columns={'Derivatives on Individual Securities': 'Company_Name'}, inplace=True)
     data_df.columns = [name.replace('    ', '').replace(' ', '') for name in data_df.columns]
     data_df = data_df[['Company_Name', 'Symbol', f'{MMM_YY}']]
+    data_df = pd.concat([ind_data_df, data_df], ignore_index=True)
     return data_df
 
 
 def nifty50_equity_list():
-    data_df = pd.read_csv("https://archives.nseindia.com/content/indices/ind_nifty50list.csv")
+    """
+    list of all equities under NIFTY 50 index
+    :return: pandas data frame
+    """
+    try:
+        data_df = pd.read_csv("https://archives.nseindia.com/content/indices/ind_nifty50list.csv")
+    except Exception as e:
+        raise FileNotFoundError(f' equities under NIFTY 50 index not found :: NSE error : {e}')
     data_df = data_df[['Company Name', 'Industry', 'Symbol']]
     return data_df
 
 
 # if __name__ == '__main__':
-#     import nselib
-#     data = nselib.trading_holiday_calendar()
-#     print(data)
+    # import nselib.capital_market as cm
+    # data = index_data(index='NIFTY 50', from_date='23-08-2022', to_date='23-06-2023')
+    # data = fno_equity_list()  #from_date='23-03-2022', to_date='23-06-2023'
+
```

### Comparing `nselib-0.4/nselib/constants.py` & `nselib-0.5/nselib/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 dd_mm_yyyy = '%d-%m-%Y'
 dd_mmm_yyyy = '%d-%b-%Y'
 ddmmyyyy = '%d%m%Y'
 mmm_yy = '%b-%y'
 
 equity_periods = ['1D', '1W', '1M', '3M', '6M', '1Y']
+indices_list = ['NIFTY','FINNIFTY','BANKNIFTY']
+
 
 # ---------- column lists-----------------
 
 price_volume_and_deliverable_position_data_columns = \
     ['Symbol', 'Series', 'Date', 'PrevClose', 'OpenPrice', 'HighPrice',
      'LowPrice', 'LastPrice', 'ClosePrice', 'AveragePrice', 'TotalTradedQuantity',
      'TurnoverInRs', 'No.ofTrades', 'DeliverableQty', '%DlyQttoTradedQty']
@@ -24,18 +26,24 @@
                           'TradePrice/Wght.Avg.Price', 'Remarks']
 
 block_deals_data_columns = ['Date', 'Symbol', 'SecurityName', 'ClientName', 'Buy/Sell', 'QuantityTraded',
                             'TradePrice/Wght.Avg.Price', 'Remarks']
 
 short_selling_data_columns = ['Date', 'Symbol', 'SecurityName', 'Quantity']
 
-bhavcopy_old = ['ISIN', 'TckrSymb', 'SctySrs', 'OpnPric', 'HghPric', 'LwPric', 'ClsPric', 'LastPric',
-                'PrvsClsgPric', 'TtlTradgVol', 'TtlTrfVal', 'TradDt', 'TtlNbOfTxsExctd']
+bhavcopy_old = ['TradDt', 'ISIN', 'TckrSymb', 'SctySrs', 'OpnPric', 'HghPric', 'LwPric', 'ClsPric', 'LastPric',
+                'PrvsClsgPric', 'TtlTradgVol', 'TtlTrfVal', 'TtlNbOfTxsExctd']
 
-bhavcopy_new = ['ISIN', 'SYMBOL', 'SERIES', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'LAST', 'PREVCLOSE', 'TOTTRDQTY',
-                'TOTTRDVAL', 'TIMESTAMP', 'TOTALTRADES']
+bhavcopy_new = ['TIMESTAMP', 'ISIN', 'SYMBOL', 'SERIES', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'LAST', 'PREVCLOSE',
+                'TOTTRDQTY', 'TOTTRDVAL', 'TOTALTRADES']
 
-future_price_volume_data_column = ['INSTRUMENT', 'SYMBOL', 'EXPIRY_DT', 'STRIKE_PRICE', 'OPTION_TYPE', 'MARKET_TYPE',
+future_price_volume_data_column = ['TIMESTAMP', 'INSTRUMENT', 'SYMBOL', 'EXPIRY_DT', 'STRIKE_PRICE', 'OPTION_TYPE', 'MARKET_TYPE',
                                    'OPENING_PRICE', 'TRADE_HIGH_PRICE', 'TRADE_LOW_PRICE', 'CLOSING_PRICE',
                                    'LAST_TRADED_PRICE', 'PREV_CLS', 'SETTLE_PRICE', 'TOT_TRADED_QTY', 'TOT_TRADED_VAL',
-                                   'OPEN_INT', 'CHANGE_IN_OI', 'MARKET_LOT', 'TIMESTAMP', 'UNDERLYING_VALUE']
+                                   'OPEN_INT', 'CHANGE_IN_OI', 'MARKET_LOT', 'UNDERLYING_VALUE']
+
+india_vix_data_column = ['TIMESTAMP', 'INDEX_NAME', 'OPEN_INDEX_VAL', 'CLOSE_INDEX_VAL', 'HIGH_INDEX_VAL',
+                         'LOW_INDEX_VAL', 'PREV_CLOSE', 'VIX_PTS_CHG', 'VIX_PERC_CHG']
+
+index_data_columns = ['TIMESTAMP', 'INDEX_NAME', 'OPEN_INDEX_VAL', 'HIGH_INDEX_VAL', 'CLOSE_INDEX_VAL',
+                      'LOW_INDEX_VAL', 'TRADED_QTY', 'TURN_OVER']
```

### Comparing `nselib-0.4/nselib/libutil.py` & `nselib-0.5/nselib/libutil.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,31 +25,36 @@
 class CalenderNotFound(Exception):
     def __init__(self, message):
 
         # Call the base class constructor with the parameters it needs
         super(CalenderNotFound, self).__init__(message)
 
 
+class NSEdataNotFound(Exception):
+    def __init__(self, message):
+        super(NSEdataNotFound, self).__init__(message)
+
+
 def validate_date_param(from_date:str, to_date:str, period:str):
     if not period and (not from_date or not to_date):
         raise ValueError(' Please provide the valid parameters')
     elif period and period.upper() not in equity_periods:
         raise ValueError(f'period = {period} is not a valid value')
 
     try:
-        from_date = datetime.strptime(from_date, dd_mm_yyyy)
-        to_date = datetime.strptime(to_date, dd_mm_yyyy)
+        if not period:
+            from_date = datetime.strptime(from_date, dd_mm_yyyy)
+            to_date = datetime.strptime(to_date, dd_mm_yyyy)
+            time_delta = (to_date - from_date).days
+            if time_delta < 1:
+                raise ValueError(f'to_date should greater than from_date ')
     except Exception as e:
         print(e)
         raise ValueError(f'either or both from_date = {from_date} || to_date = {to_date} are not valid value')
 
-    time_delta = (to_date-from_date).days
-    if time_delta < 1:
-        raise ValueError(f'to_date should greater than from_date ')
-
 
 def derive_from_and_to_date(from_date:str = None, to_date:str = None, period:str = None):
     if not period:
         return from_date, to_date
     today = date.today()
     conditions = [period.upper()=='1D',
                   period.upper()=='1W',
@@ -66,21 +71,26 @@
     f_date = np.select(conditions,value, default=(today - timedelta(days=1)))
     from_date = pd.to_datetime(str(f_date)).strftime(dd_mm_yyyy)
     today = today.strftime(dd_mm_yyyy)
     return from_date, today
 
 
 def cleaning_column_name(col:list):
-    unwanted_str_list = ['FH_']
+    unwanted_str_list = ['FH_', 'EOD_', 'HIT_']
     new_col=col
     for unwanted in unwanted_str_list:
         new_col = [name.replace(f'{unwanted}', '') for name in new_col]
     return new_col
 
 
+def cleaning_nse_symbol(symbol):
+    symbol = symbol.replace('&','%26')  #URL Parse for Stocks Like M&M Finance
+    return symbol.upper()
+
+
 def nse_urlfetch(url):
     r_session = requests.session()
     nse_live = r_session.get("http://nseindia.com", headers=header)
     return r_session.get(url, headers=header)
 
 
 def get_nselib_path():
```

### Comparing `nselib-0.4/nselib.egg-info/PKG-INFO` & `nselib-0.5/nselib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.4
+Version: 0.5
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.4
+# NSElib 0.5
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -57,18 +57,20 @@
 * price_volume_and_deliverable_position_data 
 * price_volume_data
 * deliverable_position_data
 * bulk_deal_data
 * block_deals_data
 * short_selling_data
 * bhav_copy_with_delivery
-* bhav_copy
+* bhav_copy_equities
 * equity_list
 * fno_equity_list
 * nifty50_equity_list
+* india_vix_data
+* index_data
 
 Example : 
 
 from nselib import capital_market 
 
 data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
                                             
@@ -80,14 +82,18 @@
 
 ### Derivative
 * future_price_volume_data
 * option_price_volume_data
 * fno_bhav_copy
 * participant_wise_open_interest
 * participant_wise_trading_volume
+* expiry_dates_future
+* expiry_dates_option_index
+* nse_live_option_chain
+* fii_derivatives_statistics
 
 Example : 
 
 from nselib import derivatives
 
 data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
```

### Comparing `nselib-0.4/setup.py` & `nselib-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nselib',
     packages=setuptools.find_packages(),
-    version='0.4',
+    version='0.5',
     include_package_data=True,
     description='library to get NSE India data',
     long_description=long_description,
     long_description_content_type="text/markdown", author='RuchiTanmay',
     author_email='ruchitanmay@gmail.com',
     url='https://github.com/RuchiTanmay/nselib',
     install_requires=['requests', 'pandas', 'scipy'],
```

