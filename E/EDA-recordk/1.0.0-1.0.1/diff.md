# Comparing `tmp/EDA_recordk-1.0.0-py3-none-any.whl.zip` & `tmp/EDA_recordk-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 4643 bytes, number of entries: 8
+Zip file size: 5138 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jun-24 05:15 .DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA/__init__.py
 -rw-r--r--  2.0 unx     5053 b- defN 23-Jun-23 17:38 EDA/eda.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA_recordk/__init__.py
--rw-r--r--  2.0 unx     5053 b- defN 23-Jun-23 17:38 EDA_recordk/eda.py
--rw-r--r--  2.0 unx      288 b- defN 23-Jun-23 18:32 EDA_recordk-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 18:32 EDA_recordk-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-23 18:32 EDA_recordk-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      601 b- defN 23-Jun-23 18:32 EDA_recordk-1.0.0.dist-info/RECORD
-8 files, 11099 bytes uncompressed, 3593 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx     5073 b- defN 23-Jun-24 05:14 EDA_recordk/eda.py
+-rw-r--r--  2.0 unx      315 b- defN 23-Jun-24 05:15 EDA_recordk-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 05:15 EDA_recordk-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 05:15 EDA_recordk-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 05:15 EDA_recordk-1.0.1.dist-info/RECORD
+9 files, 17360 bytes uncompressed, 3994 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
+Filename: .DS_Store
+Comment: 
+
 Filename: EDA/__init__.py
 Comment: 
 
 Filename: EDA/eda.py
 Comment: 
 
 Filename: EDA_recordk/__init__.py
 Comment: 
 
 Filename: EDA_recordk/eda.py
 Comment: 
 
-Filename: EDA_recordk-1.0.0.dist-info/METADATA
+Filename: EDA_recordk-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: EDA_recordk-1.0.0.dist-info/WHEEL
+Filename: EDA_recordk-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: EDA_recordk-1.0.0.dist-info/top_level.txt
+Filename: EDA_recordk-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: EDA_recordk-1.0.0.dist-info/RECORD
+Filename: EDA_recordk-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EDA_recordk/eda.py

```diff
@@ -9,15 +9,15 @@
     def __init__(self, data):
         self.data = data
         self.summary()
         self.missing_values()
         self.unique_values(self.data.columns)
         self.correlation_matrix()
         self.histogram(self.data.columns)
-        self.box_plot(self.data.columns)
+        self.box_plot()
 
     # 데이터 요약을 보는 함수
     def summary(self):
         print('Data Summary')
         print(self.data.describe())
         print('=' * 25)
         print('Data info:')
@@ -109,14 +109,15 @@
             for i in nan_col:
                 self.data[i][self.data[i].isin(n)] = np.NaN
         elif change.lower() == 'n':
             pass
         else:
             print('plz press N or Y')
 
+    #heatmap
     def correlation_matrix(self):
         corr_matrix = self.data.corr()
         print('Correlation Matrix:')
         plt.figure(figsize=(10, 8))
         sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
         plt.title('Correlation Matrix')
         plt.show()
@@ -135,21 +136,23 @@
     def drop_outlier(self):
         # 변수 타입 확인
         continuous_vars = []
         for column in self.data.columns:
             if self.data[column].dtype in ['int64', 'float64']:
                 continuous_vars.append(column)
 
-            # Z-Score 계산 및 이상치 제거
+            # 이상치 제거
             if len(continuous_vars) > 0:
                 z_scores = np.abs(stats.zscore(self.data[continuous_vars]))
                 threshold = 3
                 filtered_data = self.data.copy()
                 filtered_data[continuous_vars] = filtered_data[continuous_vars][(z_scores < threshold).all(axis=1)]
                 filtered_data.dropna(subset=continuous_vars, inplace=True)
             else:
                 filtered_data = self.data.copy()
+
+            # 이상치 제거한 boxplot
             plt.figure(figsize=(12, 6))
             sns.boxplot(data=filtered_data)
             plt.title('Box Plot')
             plt.show()
             self.data = filtered_data
```

