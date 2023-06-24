# Comparing `tmp/EDA_recordk-1.0.2-py3-none-any.whl.zip` & `tmp/EDA_recordk-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5118 bytes, number of entries: 9
+Zip file size: 5124 bytes, number of entries: 9
 -rw-r--r--  2.0 unx     6148 b- defN 23-Jun-24 05:15 .DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA/__init__.py
 -rw-r--r--  2.0 unx     5053 b- defN 23-Jun-23 17:38 EDA/eda.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA_recordk/__init__.py
--rw-r--r--  2.0 unx     5076 b- defN 23-Jun-24 05:23 EDA_recordk/eda.py
--rw-r--r--  2.0 unx      288 b- defN 23-Jun-24 05:24 EDA_recordk-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 05:24 EDA_recordk-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 05:24 EDA_recordk-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 05:24 EDA_recordk-1.0.2.dist-info/RECORD
-9 files, 17336 bytes uncompressed, 3974 bytes compressed:  77.1%
+-rw-r--r--  2.0 unx     5089 b- defN 23-Jun-24 08:09 EDA_recordk/eda.py
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/RECORD
+9 files, 17349 bytes uncompressed, 3980 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: EDA_recordk/__init__.py
 Comment: 
 
 Filename: EDA_recordk/eda.py
 Comment: 
 
-Filename: EDA_recordk-1.0.2.dist-info/METADATA
+Filename: EDA_recordk-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: EDA_recordk-1.0.2.dist-info/WHEEL
+Filename: EDA_recordk-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: EDA_recordk-1.0.2.dist-info/top_level.txt
+Filename: EDA_recordk-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: EDA_recordk-1.0.2.dist-info/RECORD
+Filename: EDA_recordk-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EDA_recordk/eda.py

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy import stats
 
 
 class EDA:
-    def __init__(self, data):
+    def __init__(self, data: pd.DataFrame):
         self.data = data
         self.summary()
         self.missing_values()
         self.unique_values(self.data.columns)
         self.correlation_matrix()
         self.histogram(self.data.columns)
         self.box_plot()
@@ -37,15 +37,15 @@
     # 결측치 확인
     def missing_values(self):
         print('Missing Values:')
         print(self.data.isna().sum())
         print('=' * 25)
 
     def preprocessing(self):
-        missing_columns = self.data.columns[self.data.isnull().any()].tolist()
+        missing_columns = self.data.columns[self.data.isna().any()].tolist()
         sel = '0'
         for i in missing_columns:
             print(f'Missing columns : {i} \n dtype : {self.data[i].dtype} \n cnt:{self.data[i].isna().sum()}')
             print('=' * 25)
             num = ['int64', 'float64']
             if self.data[i].dtype in num:
                 sel = input('1. mode \n 2. mean \n 3. median')
@@ -109,15 +109,15 @@
             for i in nan_col:
                 self.data[i][self.data[i].isin(n)] = np.NaN
         elif change.lower() == 'n':
             pass
         else:
             print('plz press N or Y')
 
-    #heatmap
+    # heatmap
     def correlation_matrix(self):
         corr_matrix = self.data.corr()
         print('Correlation Matrix:')
         plt.figure(figsize=(10, 8))
         sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
         plt.title('Correlation Matrix')
         plt.show()
```

