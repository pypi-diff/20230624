# Comparing `tmp/technicalmethods-0.2.4-py3-none-any.whl.zip` & `tmp/technicalmethods-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6720 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       31 b- defN 23-Jan-05 13:57 technicalmethods/__init__.py
--rw-rw-rw-  2.0 fat    21990 b- defN 21-Dec-21 16:46 technicalmethods/methods.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jan-05 14:05 technicalmethods-0.2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      414 b- defN 23-Jan-05 14:05 technicalmethods-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-05 14:05 technicalmethods-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jan-05 14:05 technicalmethods-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      598 b- defN 23-Jan-05 14:05 technicalmethods-0.2.4.dist-info/RECORD
-7 files, 24231 bytes uncompressed, 5648 bytes compressed:  76.7%
+Zip file size: 6914 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-24 16:58 technicalmethods/__init__.py
+-rw-rw-rw-  2.0 fat    23747 b- defN 23-Jun-24 17:30 technicalmethods/methods.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-24 17:38 technicalmethods-0.2.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      414 b- defN 23-Jun-24 17:38 technicalmethods-0.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 17:38 technicalmethods-0.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-24 17:38 technicalmethods-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      598 b- defN 23-Jun-24 17:38 technicalmethods-0.2.5.dist-info/RECORD
+7 files, 25988 bytes uncompressed, 5842 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: technicalmethods/__init__.py
 Comment: 
 
 Filename: technicalmethods/methods.py
 Comment: 
 
-Filename: technicalmethods-0.2.4.dist-info/LICENSE
+Filename: technicalmethods-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: technicalmethods-0.2.4.dist-info/METADATA
+Filename: technicalmethods-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: technicalmethods-0.2.4.dist-info/WHEEL
+Filename: technicalmethods-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: technicalmethods-0.2.4.dist-info/top_level.txt
+Filename: technicalmethods-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: technicalmethods-0.2.4.dist-info/RECORD
+Filename: technicalmethods-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## technicalmethods/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
```

## technicalmethods/methods.py

```diff
@@ -13,15 +13,20 @@
 
 class Indicators():
     """
     Calculate various Technical Indicators
 
     """
     @classmethod
-    def MACD(cls, close, fast, slow, signal):
+    def MACD(
+        cls, 
+        close: pd.Series, 
+        fast: int, 
+        slow: int, 
+        signal: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Calculate Moving Average Convergence Divergence
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -52,26 +57,34 @@
 
         # Calculate Price Velocity as the difference between the fast and slow
         # averages
         macd =  ema_fast - ema_slow
 
         # Calculate the Signal line as the exponentially smoothed Price
         # Velocity (using the signal parameter for period)
-        signal = cls.EMA(macd, time_period=signal)
+        signal_line = cls.EMA(macd, time_period=signal)
 
         # Calculate the MACD Histogram as the Price Velocity less the Signal
         # line
-        histogram = macd - signal
+        histogram = macd - signal_line
 
-        return macd, signal, histogram
+        return macd, signal_line, histogram
 
 
     @classmethod
-    def bbands(cls, close, high=None, low=None, time_period=20, sd_up=2,
-               sd_down=2, simple_ma=True, only_close=True):
+    def bbands(
+        cls, 
+        close: pd.Series, 
+        high: pd.Series | None = None, 
+        low: pd.Series | None = None, 
+        time_period: int = 20, 
+        sd_up: int = 2,
+        sd_down: int = 2, 
+        simple_ma: bool = True, 
+        only_close: bool = True) -> tuple[pd.Series, pd.Series, pd.Series]:
         """
         Calculate Bollinger Bands - Upper, Lower and Mid Moving Average
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -108,30 +121,36 @@
             sd = close.rolling(window=time_period).std(ddof=0)
             if simple_ma:
                 ma = close.rolling(window=time_period).mean()
             else:
                 ma = cls.EMA(input_series=close, time_period=time_period)
 
         else:
+            high = pd.Series(high)
+            low = pd.Series(low)
             typical_price = (high + low + close) / 3
             sd = typical_price.rolling(window=time_period).std(ddof=0)
             if simple_ma:
                 ma = typical_price.rolling(window=time_period).mean()
             else:
                 ma = cls.EMA(
                     input_series=typical_price, time_period=time_period)
 
-        upper_band = ma + (sd * sd_up)
-        lower_band = ma - (sd * sd_down)
+        ma = pd.Series(ma)
+        upper_band = pd.Series(ma + (sd * sd_up))
+        lower_band = pd.Series(ma - (sd * sd_down))
 
         return upper_band, ma, lower_band
 
 
     @classmethod
-    def RSI(cls, close, time_period):
+    def RSI(
+        cls, 
+        close: pd.Series, 
+        time_period: int) -> np.ndarray:
         """
         Calculate Relative Strength Index
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -172,15 +191,19 @@
         relative_strength = gain_avg / loss_avg
         rsi = 100 - 100 / (1 + relative_strength)
 
         return rsi
 
 
     @staticmethod
-    def CCI(high, low, close, time_period):
+    def CCI(
+        high: pd.Series, 
+        low: pd.Series, 
+        close: pd.Series, 
+        time_period: int) -> pd.Series:
         """
         Calculate Commodity Channel Index
 
         Parameters
         ----------
         high : Series
             Time series of high prices.
@@ -204,24 +227,32 @@
 
         # 2. Compute a moving average of the n most recent average prices
         moving_average = typical_price.rolling(time_period).mean()
 
         # 3. Compute the mean deviation of the n most recent typical prices
         mean_deviation = np.array([0.0]*len(close))
         for i in range(len(close)):
-            mean_deviation[i] = typical_price[i - time_period+1:i+1].mad()
+            #mean_deviation[i] = typical_price[i - time_period+1:i+1].mad()
+            data = typical_price[i - time_period+1:i+1]
+            mean_deviation[i] = np.abs(data - data.mean(axis=0)).mean(axis=0)
 
         # 4. Compute the Commodity Channel Index
         cci = ((typical_price - moving_average) / (0.015 * mean_deviation))
 
         return cci
 
 
     @classmethod
-    def ADX(cls, high, low, close, time_period, dmi=False):
+    def ADX(
+        cls, 
+        high: pd.Series, 
+        low: pd.Series, 
+        close: pd.Series, 
+        time_period: int, 
+        dmi: bool=False) -> tuple[np.ndarray, np.ndarray, np.ndarray] | np.ndarray:
         """
         Calculate Average Directional Movement Index
 
         Parameters
         ----------
         high : Series
             Time series of high prices.
@@ -277,15 +308,19 @@
             return adx, di_plus_period, di_minus_period
 
         else:
             return adx
 
 
     @classmethod
-    def _directional_movement(cls, high, low, time_period):
+    def _directional_movement(
+        cls, 
+        high: pd.Series, 
+        low: pd.Series, 
+        time_period: int) -> tuple[np.ndarray, np.ndarray]:
         """
         Calculate Directional Movement
 
         Parameters
         ----------
 
         high : Series
@@ -343,15 +378,19 @@
             input_series=dm_minus_1, time_period=time_period,
             wilder=True, average=False)
 
         return dm_plus_period, dm_minus_period
 
 
     @staticmethod
-    def williams_r(high, low, close, time_period):
+    def williams_r(
+        high: pd.Series, 
+        low: pd.Series, 
+        close: pd.Series, 
+        time_period: int) -> pd.Series:
         """
         Calculate Williams %R
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -375,16 +414,22 @@
 
         percent_r = -100 * ((nd_high - close) / (nd_high - nd_low))
 
         return percent_r
 
 
     @staticmethod
-    def stochastic(high, low, close, fast_k_period, slow_k_period=3,
-                   slow_d_period=3, output_type='slow'):
+    def stochastic(
+        high: pd.Series, 
+        low: pd.Series, 
+        close: pd.Series, 
+        fast_k_period: int, 
+        slow_k_period: int = 3,
+        slow_d_period: int = 3, 
+        output_type: str = 'slow') -> tuple[pd.Series, pd.Series]:
         """
         Calculate Stochastic Oscillator
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -430,15 +475,20 @@
         if output_type == 'slow':
             return percent_k_slow, percent_d_slow
 
         return percent_k, percent_d
 
 
     @classmethod
-    def ATR(cls, high, low, close, time_period):
+    def ATR(
+        cls, 
+        high: pd.Series, 
+        low: pd.Series, 
+        close: pd.Series, 
+        time_period: int) -> np.ndarray:
         """
         Calculate Average True Range
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -465,15 +515,18 @@
         atr = cls.EMA(
             input_series=t_range, time_period=time_period, wilder=True)
 
         return atr
 
 
     @staticmethod
-    def breakout(high, low, time_period=20):
+    def breakout(
+        high: pd.Series, 
+        low: pd.Series, 
+        time_period: int = 20) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Calculate n-day breakout
 
         Parameters
         ----------
         high : Series
             Time series of high prices.
@@ -512,15 +565,18 @@
                     flag[row-1] == -1 and high[row] < nd_high[row-1]):
                 flag[row] = -1
 
         return nd_low, nd_high, flag
 
 
     @staticmethod
-    def trend_channel(close, high, low):
+    def trend_channel(
+        close: pd.Series, 
+        high: pd.Series, 
+        low: pd.Series) -> tuple[pd.Series, pd.Series]:
         """
         Calculate Trend lines above and below the price data to form a channel
 
         Parameters
         ----------
         close : Series
             Time series of closing prices.
@@ -573,15 +629,18 @@
 
         low_trend = reg_line[0] * output['counter'] + reg_line[1]
 
         return low_trend, high_trend
 
 
     @staticmethod
-    def true_range(high, low, close):
+    def true_range(
+        high: pd.Series, 
+        low: pd.Series, 
+        close: pd.Series) -> pd.Series:
         """
         Calculates the 1 day True Range given High, Low and Close prices.
 
         Parameters
         ----------
         df : DataFrame
             Input dataframe of High, Low and Close data.
@@ -593,17 +652,17 @@
 
         """
         # Suppress SettingWithCopyWarning caused by slicing DataFrame
         #pd.options.mode.chained_assignment = None
 
         # Calculate the high minus low, absolute value of high minus yesterdays
         # close and the absolute value of the low minus yesterdays close
-        high_low = high - low
-        high_close = np.abs(high - close.shift())
-        close_low = np.abs(low - close.shift())
+        high_low = pd.Series(high - low)
+        high_close = pd.Series(np.abs(high - close.shift()))
+        close_low = pd.Series(np.abs(low - close.shift()))
 
         # Concatenate these 3 series
         ranges = pd.concat([high_low, high_close, close_low], axis=1)
 
         # Calculate the True Range as the maximum of these 3 series
         t_range = ranges.max(skipna=False, axis=1)
 
@@ -633,16 +692,20 @@
         # Create DataFrame from concatenating price columns
         dataframe = pd.concat(fields, axis=1)
 
         return dataframe
 
 
     @staticmethod
-    def EMA(input_series, time_period, wilder=False, average=True,
-            slow_macd=None):
+    def EMA(
+        input_series: pd.Series | np.ndarray, 
+        time_period: int, 
+        wilder: bool = False, 
+        average: bool = True,
+        slow_macd: int | None = None) -> np.ndarray:
         """
         Calculate Exponentially Weighted Moving Average
 
         Parameters
         ----------
         input_series : Series
             Prices to be smoothed.
```

## Comparing `technicalmethods-0.2.4.dist-info/LICENSE` & `technicalmethods-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

