# Comparing `tmp/EDA_recordk-1.0.4-py3-none-any.whl.zip` & `tmp/EDA_recordk-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5112 bytes, number of entries: 9
+Zip file size: 5110 bytes, number of entries: 9
 -rw-r--r--  2.0 unx     6148 b- defN 23-Jun-24 05:15 .DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA/__init__.py
 -rw-r--r--  2.0 unx     5053 b- defN 23-Jun-23 17:38 EDA/eda.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA_recordk/__init__.py
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-24 09:33 EDA_recordk/eda.py
--rw-r--r--  2.0 unx      288 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/RECORD
-9 files, 17325 bytes uncompressed, 3968 bytes compressed:  77.1%
+-rw-r--r--  2.0 unx     5055 b- defN 23-Jun-24 09:37 EDA_recordk/eda.py
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-24 09:39 EDA_recordk-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 09:39 EDA_recordk-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 09:39 EDA_recordk-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 09:39 EDA_recordk-1.0.5.dist-info/RECORD
+9 files, 17315 bytes uncompressed, 3966 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: EDA_recordk/__init__.py
 Comment: 
 
 Filename: EDA_recordk/eda.py
 Comment: 
 
-Filename: EDA_recordk-1.0.4.dist-info/METADATA
+Filename: EDA_recordk-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: EDA_recordk-1.0.4.dist-info/WHEEL
+Filename: EDA_recordk-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: EDA_recordk-1.0.4.dist-info/top_level.txt
+Filename: EDA_recordk-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: EDA_recordk-1.0.4.dist-info/RECORD
+Filename: EDA_recordk-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EDA_recordk/eda.py

```diff
@@ -132,27 +132,28 @@
         sns.boxplot(data=self.data)
         plt.title('Box Plot')
         plt.show()
 
     def drop_outlier(self):
         # 변수 타입 확인
         continuous_vars = []
+        filtered_data = 0
         for column in self.data.columns:
             if self.data[column].dtype in ['int64', 'float64']:
                 continuous_vars.append(column)
 
-            # 이상치 제거
-            if len(continuous_vars) > 0:
-                z_scores = np.abs(stats.zscore(self.data[continuous_vars]))
-                threshold = 3
-                filtered_data = self.data.copy()
-                filtered_data[continuous_vars] = filtered_data[continuous_vars][(z_scores < threshold).all(axis=1)]
-                filtered_data.dropna(subset=continuous_vars, inplace=True)
-            else:
-                filtered_data = self.data.copy()
+        # 이상치 제거
+        if len(continuous_vars) > 0:
+            z_scores = np.abs(stats.zscore(self.data[continuous_vars]))
+            threshold = 3
+            filtered_data = self.data.copy()
+            filtered_data[continuous_vars] = filtered_data[continuous_vars][(z_scores < threshold).all(axis=1)]
+            filtered_data.dropna(subset=continuous_vars, inplace=True)
+        else:
+            filtered_data = self.data.copy()
 
         # 이상치 제거한 boxplot
         plt.figure(figsize=(12, 6))
         sns.boxplot(data=filtered_data)
         plt.title('Box Plot')
         plt.show()
         self.data = filtered_data
```

## Comparing `EDA_recordk-1.0.4.dist-info/RECORD` & `EDA_recordk-1.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .DS_Store,sha256=C2GgT5T3USlycIoKM2FhFlKjL0dbwj4zlk-fiXD0F84,6148
 EDA/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 EDA/eda.py,sha256=Fr1IKMDbNf2MK-PC5Em4Hv-2wcjHQgv-FAkMdN7nFtQ,5053
 EDA_recordk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-EDA_recordk/eda.py,sha256=96WjLP365DG7r9tFXi0v8zx6uySlm67SCdxehtUgU9w,5065
-EDA_recordk-1.0.4.dist-info/METADATA,sha256=y9zbBf0dOhu8EV04Gc_XwDjcuqMZ_8fFP-REB_Hpc5w,288
-EDA_recordk-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-EDA_recordk-1.0.4.dist-info/top_level.txt,sha256=hVxWHlr1wm64kaBTwhZ66VpzbYJQO_nkGTt4gnTs2qU,12
-EDA_recordk-1.0.4.dist-info/RECORD,,
+EDA_recordk/eda.py,sha256=F9BQh81-mrBqM7rIzQd5UlUaZ8QD_oSNJhLS_cWxFyQ,5055
+EDA_recordk-1.0.5.dist-info/METADATA,sha256=LUuK8xJv0S16Ol_bjbUwuEfN22HrvXWFtCrJsNH1lqc,288
+EDA_recordk-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+EDA_recordk-1.0.5.dist-info/top_level.txt,sha256=hVxWHlr1wm64kaBTwhZ66VpzbYJQO_nkGTt4gnTs2qU,12
+EDA_recordk-1.0.5.dist-info/RECORD,,
```

