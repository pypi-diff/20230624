# Comparing `tmp/EDA_recordk-1.0.3-py3-none-any.whl.zip` & `tmp/EDA_recordk-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5124 bytes, number of entries: 9
+Zip file size: 5112 bytes, number of entries: 9
 -rw-r--r--  2.0 unx     6148 b- defN 23-Jun-24 05:15 .DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA/__init__.py
 -rw-r--r--  2.0 unx     5053 b- defN 23-Jun-23 17:38 EDA/eda.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:23 EDA_recordk/__init__.py
--rw-r--r--  2.0 unx     5089 b- defN 23-Jun-24 08:09 EDA_recordk/eda.py
--rw-r--r--  2.0 unx      288 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 08:09 EDA_recordk-1.0.3.dist-info/RECORD
-9 files, 17349 bytes uncompressed, 3980 bytes compressed:  77.1%
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-24 09:33 EDA_recordk/eda.py
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 23-Jun-24 09:34 EDA_recordk-1.0.4.dist-info/RECORD
+9 files, 17325 bytes uncompressed, 3968 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: EDA_recordk/__init__.py
 Comment: 
 
 Filename: EDA_recordk/eda.py
 Comment: 
 
-Filename: EDA_recordk-1.0.3.dist-info/METADATA
+Filename: EDA_recordk-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: EDA_recordk-1.0.3.dist-info/WHEEL
+Filename: EDA_recordk-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: EDA_recordk-1.0.3.dist-info/top_level.txt
+Filename: EDA_recordk-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: EDA_recordk-1.0.3.dist-info/RECORD
+Filename: EDA_recordk-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EDA_recordk/eda.py

```diff
@@ -146,13 +146,13 @@
                 threshold = 3
                 filtered_data = self.data.copy()
                 filtered_data[continuous_vars] = filtered_data[continuous_vars][(z_scores < threshold).all(axis=1)]
                 filtered_data.dropna(subset=continuous_vars, inplace=True)
             else:
                 filtered_data = self.data.copy()
 
-            # 이상치 제거한 boxplot
-            plt.figure(figsize=(12, 6))
-            sns.boxplot(data=filtered_data)
-            plt.title('Box Plot')
-            plt.show()
-            self.data = filtered_data
+        # 이상치 제거한 boxplot
+        plt.figure(figsize=(12, 6))
+        sns.boxplot(data=filtered_data)
+        plt.title('Box Plot')
+        plt.show()
+        self.data = filtered_data
```

