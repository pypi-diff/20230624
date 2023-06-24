# Comparing `tmp/inpost-0.1.3.tar.gz` & `tmp/inpost-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.1.3.tar", max compression
+gzip compressed data, was "inpost-0.1.4.tar", max compression
```

## Comparing `inpost-0.1.3.tar` & `inpost-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.3/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.3/inpost/__init__.py
--rw-r--r--   0        0        0    45403 2023-06-08 19:53:36.278873 inpost-0.1.3/inpost/api.py
--rw-r--r--   0        0        0     1173 2023-05-08 21:18:45.284128 inpost-0.1.3/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.3/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2644 2023-05-16 17:58:27.019865 inpost-0.1.3/inpost/static/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.3/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     2541 2023-05-30 13:20:30.662182 inpost-0.1.3/inpost/static/__pycache__/endpoints.cpython-311.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.3/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     5421 2023-05-16 17:58:27.079865 inpost-0.1.3/inpost/static/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.3/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0     3107 2023-05-16 17:58:27.083199 inpost-0.1.3/inpost/static/__pycache__/friends.cpython-311.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.3/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.3/inpost/static/__pycache__/headers.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2023-05-16 17:58:27.086532 inpost-0.1.3/inpost/static/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.3/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0    44670 2023-05-30 14:13:11.007453 inpost-0.1.3/inpost/static/__pycache__/parcels.cpython-311.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.3/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0    11366 2023-05-30 13:20:30.648849 inpost-0.1.3/inpost/static/__pycache__/statuses.cpython-311.pyc
--rw-r--r--   0        0        0     1958 2023-05-17 18:25:42.850624 inpost-0.1.3/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.1.3/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.1.3/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.3/inpost/static/headers.py
--rw-r--r--   0        0        0      670 2023-05-08 21:18:45.284128 inpost-0.1.3/inpost/static/notifications.py
--rw-r--r--   0        0        0    28188 2023-06-08 08:05:09.631212 inpost-0.1.3/inpost/static/parcels.py
--rw-r--r--   0        0        0     7066 2023-05-16 18:03:15.934872 inpost-0.1.3/inpost/static/statuses.py
--rw-r--r--   0        0        0     1072 2023-06-08 11:57:44.626982 inpost-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.3/setup.py
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.4/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.4/inpost/__init__.py
+-rw-r--r--   0        0        0    55209 2023-06-24 11:24:08.133079 inpost-0.1.4/inpost/api.py
+-rw-r--r--   0        0        0     3320 2023-06-24 11:18:00.607432 inpost-0.1.4/inpost/static/__init__.py
+-rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.4/inpost/static/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3534 2023-06-24 11:12:59.058908 inpost-0.1.4/inpost/static/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.4/inpost/static/__pycache__/endpoints.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-06-18 11:17:01.501585 inpost-0.1.4/inpost/static/__pycache__/endpoints.cpython-311.pyc
+-rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.4/inpost/static/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     5477 2023-06-18 11:17:01.504918 inpost-0.1.4/inpost/static/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.4/inpost/static/__pycache__/friends.cpython-310.pyc
+-rw-r--r--   0        0        0     3066 2023-06-18 14:14:33.201671 inpost-0.1.4/inpost/static/__pycache__/friends.cpython-311.pyc
+-rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.4/inpost/static/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.4/inpost/static/__pycache__/headers.cpython-311.pyc
+-rw-r--r--   0        0        0     1658 2023-06-18 11:17:01.534918 inpost-0.1.4/inpost/static/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.4/inpost/static/__pycache__/parcels.cpython-310.pyc
+-rw-r--r--   0        0        0    65008 2023-06-24 11:12:59.105575 inpost-0.1.4/inpost/static/__pycache__/parcels.cpython-311.pyc
+-rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.4/inpost/static/__pycache__/statuses.cpython-310.pyc
+-rw-r--r--   0        0        0    11956 2023-06-24 11:12:59.148909 inpost-0.1.4/inpost/static/__pycache__/statuses.cpython-311.pyc
+-rw-r--r--   0        0        0     2987 2023-06-17 20:11:38.099610 inpost-0.1.4/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2617 2023-06-18 09:47:44.436586 inpost-0.1.4/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     1717 2023-06-18 13:52:29.830316 inpost-0.1.4/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.4/inpost/static/headers.py
+-rw-r--r--   0        0        0      839 2023-06-18 10:28:12.228334 inpost-0.1.4/inpost/static/notifications.py
+-rw-r--r--   0        0        0    44755 2023-06-24 11:18:02.150775 inpost-0.1.4/inpost/static/parcels.py
+-rw-r--r--   0        0        0     8052 2023-06-24 11:18:01.110768 inpost-0.1.4/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1425 2023-06-24 11:43:19.908612 inpost-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.4/setup.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.4/PKG-INFO
```

### Comparing `inpost-0.1.3/README.md` & `inpost-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/__init__.cpython-310.pyc` & `inpost-0.1.4/inpost/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/endpoints.cpython-310.pyc` & `inpost-0.1.4/inpost/static/__pycache__/endpoints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/endpoints.cpython-311.pyc` & `inpost-0.1.4/inpost/static/__pycache__/endpoints.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,192 +1,269 @@
 magic:    0xa70d0d0a
-moddate:  0x261c6564 (Wed May 17 18:25:42 2023 UTC)
-files sz: 1958
+moddate:  0x7a138e64 (Sat Jun 17 20:11:38 2023 UTC)
+files sz: 2987
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700550064005a006501650264013c00000064025a036501650264033c
-      00000064045a046501650264053c00000064005a056501650264063c0000
-      0064075a066501650264083c00000064095a0765016502640a3c00000064
+      00000064045a046501650264053c00000064065a056501650264073c0000
+      0064005a066501650264083c00000064095a0765016502640a3c00000064
       0b5a0865016502640c3c000000640d5a0965016502640e3c000000640f5a
       0a6501650264103c00000064115a0b6501650264123c00000064135a0c65
       01650264143c00000064155a0d6501650264163c00000064175a0e650165
       0264183c00000064195a0f65016502641a3c000000641b5a106501650264
       1c3c000000641d5a1165016502641e3c000000641f5a126501650264203c
       00000064215a136501650264223c00000064235a146501650264243c0000
       0064255a156501650264263c00000064275a166501650264283c00000064
-      295a1765016502642a3c000000642b5300
+      295a1765016502642a3c000000642b5a1865016502642c3c000000642d5a
+      1965016502642e3c000000642f5a1a6501650264303c00000064315a1b65
+      01650264323c00000064335a1c6501650264343c00000064355a1d650165
+      0264363c00000064375a1e6501650264383c00000064395a1f6501650264
+      3a3c000000643b5a2065016502643c3c000000643d5a2165016502643e3c
+      000000643f5300
      0           0 RESUME                   0
    
-     1           2 SETUP_ANNOTATIONS
+     2           2 SETUP_ANNOTATIONS
                  4 LOAD_CONST               0 ('https://api-inmobile-pl.easypack24.net/v1/authenticate')
                  6 STORE_NAME               0 (login)
                  8 LOAD_NAME                1 (str)
                 10 LOAD_NAME                2 (__annotations__)
                 12 LOAD_CONST               1 ('login')
                 14 STORE_SUBSCR
    
-     2          18 LOAD_CONST               2 ('https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/')
+     3          18 LOAD_CONST               2 ('https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/')
                 20 STORE_NAME               3 (send_sms_code)
                 22 LOAD_NAME                1 (str)
                 24 LOAD_NAME                2 (__annotations__)
                 26 LOAD_CONST               3 ('send_sms_code')
                 28 STORE_SUBSCR
    
-     3          32 LOAD_CONST               4 ('https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode')
+     4          32 LOAD_CONST               4 ('https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode')
                 34 STORE_NAME               4 (confirm_sms_code)
                 36 LOAD_NAME                1 (str)
                 38 LOAD_NAME                2 (__annotations__)
                 40 LOAD_CONST               5 ('confirm_sms_code')
                 42 STORE_SUBSCR
    
-     6          46 LOAD_CONST               0 ('https://api-inmobile-pl.easypack24.net/v1/authenticate')
-                48 STORE_NAME               5 (refresh_token)
+     5          46 LOAD_CONST               6 ('https://api-inmobile-pl.easypack24.net/v1/logout')
+                48 STORE_NAME               5 (logout)
                 50 LOAD_NAME                1 (str)
                 52 LOAD_NAME                2 (__annotations__)
-                54 LOAD_CONST               6 ('refresh_token')
+                54 LOAD_CONST               7 ('logout')
                 56 STORE_SUBSCR
    
-     7          60 LOAD_CONST               7 ('https://api-inmobile-pl.easypack24.net/v3/parcels/tracked')
-                62 STORE_NAME               6 (parcels)
+     6          60 LOAD_CONST               0 ('https://api-inmobile-pl.easypack24.net/v1/authenticate')
+                62 STORE_NAME               6 (refresh_token)
                 64 LOAD_NAME                1 (str)
                 66 LOAD_NAME                2 (__annotations__)
-                68 LOAD_CONST               8 ('parcels')
+                68 LOAD_CONST               8 ('refresh_token')
                 70 STORE_SUBSCR
    
-     8          74 LOAD_CONST               9 ('https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/')
-                76 STORE_NAME               7 (parcel)
+     9          74 LOAD_CONST               9 ('https://api-inmobile-pl.easypack24.net/v3/parcels/tracked')
+                76 STORE_NAME               7 (parcels)
                 78 LOAD_NAME                1 (str)
                 80 LOAD_NAME                2 (__annotations__)
-                82 LOAD_CONST              10 ('parcel')
+                82 LOAD_CONST              10 ('parcels')
                 84 STORE_SUBSCR
    
-     9          88 LOAD_CONST              11 ('https://api-inmobile-pl.easypack24.net/v3/parcels/multi/')
-                90 STORE_NAME               8 (multi)
+    10          88 LOAD_CONST              11 ('https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/')
+                90 STORE_NAME               8 (parcel)
                 92 LOAD_NAME                1 (str)
                 94 LOAD_NAME                2 (__annotations__)
-                96 LOAD_CONST              12 ('multi')
+                96 LOAD_CONST              12 ('parcel')
                 98 STORE_SUBSCR
    
-    10         102 LOAD_CONST              13 ('https://api-inmobile-pl.easypack24.net/v1/collect/validate')
-               104 STORE_NAME               9 (collect)
+    11         102 LOAD_CONST              13 ('https://api-inmobile-pl.easypack24.net/v3/parcels/multi/')
+               104 STORE_NAME               9 (multi)
                106 LOAD_NAME                1 (str)
                108 LOAD_NAME                2 (__annotations__)
-               110 LOAD_CONST              14 ('collect')
+               110 LOAD_CONST              14 ('multi')
                112 STORE_SUBSCR
    
-    11         116 LOAD_CONST              15 ('https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen')
-               118 STORE_NAME              10 (reopen)
+    12         116 LOAD_CONST              15 ('https://api-inmobile-pl.easypack24.net/v1/collect/validate')
+               118 STORE_NAME              10 (collect)
                120 LOAD_NAME                1 (str)
                122 LOAD_NAME                2 (__annotations__)
-               124 LOAD_CONST              16 ('reopen')
+               124 LOAD_CONST              16 ('collect')
                126 STORE_SUBSCR
    
-    12         130 LOAD_CONST              17 ('https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open')
-               132 STORE_NAME              11 (compartment_open)
+    13         130 LOAD_CONST              17 ('https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen')
+               132 STORE_NAME              11 (reopen)
                134 LOAD_NAME                1 (str)
                136 LOAD_NAME                2 (__annotations__)
-               138 LOAD_CONST              18 ('compartment_open')
+               138 LOAD_CONST              18 ('reopen')
                140 STORE_SUBSCR
    
-    13         144 LOAD_CONST              19 ('https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status')
-               146 STORE_NAME              12 (compartment_status)
+    14         144 LOAD_CONST              19 ('https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open')
+               146 STORE_NAME              12 (compartment_open)
                148 LOAD_NAME                1 (str)
                150 LOAD_NAME                2 (__annotations__)
-               152 LOAD_CONST              20 ('compartment_status')
+               152 LOAD_CONST              20 ('compartment_open')
                154 STORE_SUBSCR
    
-    14         158 LOAD_CONST              21 ('https://api-inmobile-pl.easypack24.net/v1/collect/terminate')
-               160 STORE_NAME              13 (terminate_collect_session)
+    15         158 LOAD_CONST              21 ('https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status')
+               160 STORE_NAME              13 (compartment_status)
                162 LOAD_NAME                1 (str)
                164 LOAD_NAME                2 (__annotations__)
-               166 LOAD_CONST              22 ('terminate_collect_session')
+               166 LOAD_CONST              22 ('compartment_status')
                168 STORE_SUBSCR
    
-    15         172 LOAD_CONST              23 ('https://api-inmobile-pl.easypack24.net/v1/friends/')
-               174 STORE_NAME              14 (friendship)
+    16         172 LOAD_CONST              23 ('https://api-inmobile-pl.easypack24.net/v1/collect/terminate')
+               174 STORE_NAME              14 (terminate_collect_session)
                176 LOAD_NAME                1 (str)
                178 LOAD_NAME                2 (__annotations__)
-               180 LOAD_CONST              24 ('friendship')
+               180 LOAD_CONST              24 ('terminate_collect_session')
                182 STORE_SUBSCR
    
-    16         186 LOAD_CONST              25 ('https://api-inmobile-pl.easypack24.net/v1/invitations/validate')
-               188 STORE_NAME              15 (validate_friendship)
+    17         186 LOAD_CONST              25 ('https://api-inmobile-pl.easypack24.net/v1/parcels/shared')
+               188 STORE_NAME              15 (shared)
                190 LOAD_NAME                1 (str)
                192 LOAD_NAME                2 (__annotations__)
-               194 LOAD_CONST              26 ('validate_friendship')
+               194 LOAD_CONST              26 ('shared')
                196 STORE_SUBSCR
    
-    17         200 LOAD_CONST              27 ('https://api-inmobile-pl.easypack24.net/v1/invitations/accept')
-               202 STORE_NAME              16 (accept_friendship)
+    20         200 LOAD_CONST              27 ('https://api-inmobile-pl.easypack24.net/v1/parcels')
+               202 STORE_NAME              16 (create)
                204 LOAD_NAME                1 (str)
                206 LOAD_NAME                2 (__annotations__)
-               208 LOAD_CONST              28 ('accept_friendship')
+               208 LOAD_CONST              28 ('create')
                210 STORE_SUBSCR
    
-    18         214 LOAD_CONST              29 ('https://api-inmobile-pl.easypack24.net/v1/parcels/shared')
-               216 STORE_NAME              17 (shared)
+    21         214 LOAD_CONST              29 ('https://api-inmobile-pl.easypack24.net/v3/points')
+               216 STORE_NAME              17 (points)
                218 LOAD_NAME                1 (str)
                220 LOAD_NAME                2 (__annotations__)
-               222 LOAD_CONST              30 ('shared')
+               222 LOAD_CONST              30 ('points')
                224 STORE_SUBSCR
    
-    19         228 LOAD_CONST              31 ('https://api-inmobile-pl.easypack24.net/v3/parcels/sent/')
-               230 STORE_NAME              18 (sent)
+    22         228 LOAD_CONST              31 ('https://api-inmobile-pl.easypack24.net/v1/payments/blik/alias/status')
+               230 STORE_NAME              18 (blik_status)
                232 LOAD_NAME                1 (str)
                234 LOAD_NAME                2 (__annotations__)
-               236 LOAD_CONST              32 ('sent')
+               236 LOAD_CONST              32 ('blik_status')
                238 STORE_SUBSCR
    
-    20         242 LOAD_CONST              33 ('https://api-inmobile-pl.easypack24.net/v1/returns/parcels/')
-               244 STORE_NAME              19 (returns)
+    23         242 LOAD_CONST              33 ('https://api-inmobile-pl.easypack24.net/v1/payments/transactions/create/blik')
+               244 STORE_NAME              19 (create_blik)
                246 LOAD_NAME                1 (str)
                248 LOAD_NAME                2 (__annotations__)
-               250 LOAD_CONST              34 ('returns')
+               250 LOAD_CONST              34 ('create_blik')
                252 STORE_SUBSCR
    
-    21         256 LOAD_CONST              35 ('https://api-inmobile-pl.easypack24.net/v1/prices/parcels')
-               258 STORE_NAME              20 (parcel_prices)
+    27         256 LOAD_CONST              35 ('https://api-inmobile-pl.easypack24.net/v2/parcels/sent/')
+               258 STORE_NAME              20 (sent)
                260 LOAD_NAME                1 (str)
                262 LOAD_NAME                2 (__annotations__)
-               264 LOAD_CONST              36 ('parcel_prices')
+               264 LOAD_CONST              36 ('sent')
                266 STORE_SUBSCR
    
-    22         270 LOAD_CONST              37 ('https://api-inmobile-pl.easypack24.net/v1/returns/tickets')
-               272 STORE_NAME              21 (tickets)
+    28         270 LOAD_CONST              37 ('https://api-inmobile-pl.easypack24.net/v3/points/')
+               272 STORE_NAME              21 (parcel_points)
                274 LOAD_NAME                1 (str)
                276 LOAD_NAME                2 (__annotations__)
-               278 LOAD_CONST              38 ('tickets')
+               278 LOAD_CONST              38 ('parcel_points')
                280 STORE_SUBSCR
    
-    23         284 LOAD_CONST              39 ('https://api-inmobile-pl.easypack24.net/v1/logout')
-               286 STORE_NAME              22 (logout)
+    29         284 LOAD_CONST              39 ('https://api-inmobile-pl.easypack24.net/v1/send/validate/')
+               286 STORE_NAME              22 (validate_sent)
                288 LOAD_NAME                1 (str)
                290 LOAD_NAME                2 (__annotations__)
-               292 LOAD_CONST              40 ('logout')
+               292 LOAD_CONST              40 ('validate_sent')
                294 STORE_SUBSCR
    
-    24         298 LOAD_CONST              41 ('https://api-inmobile-pl.easypack24.net/v2/notifications?type=PUSH%2CNEWS%2CTILE')
-               300 STORE_NAME              23 (parcel_notifications)
+    30         298 LOAD_CONST              41 ('https://api-inmobile-pl.easypack24.net/v1/send/compartment/open')
+               300 STORE_NAME              23 (open_sent)
                302 LOAD_NAME                1 (str)
                304 LOAD_NAME                2 (__annotations__)
-               306 LOAD_CONST              42 ('parcel_notifications')
+               306 LOAD_CONST              42 ('open_sent')
                308 STORE_SUBSCR
-               312 LOAD_CONST              43 (None)
-               314 RETURN_VALUE
+   
+    31         312 LOAD_CONST              43 ('https://api-inmobile-pl.easypack24.net/v1/send/compartment/reopen')
+               314 STORE_NAME              24 (reopen_sent)
+               316 LOAD_NAME                1 (str)
+               318 LOAD_NAME                2 (__annotations__)
+               320 LOAD_CONST              44 ('reopen_sent')
+               322 STORE_SUBSCR
+   
+    32         326 LOAD_CONST              45 ('https://api-inmobile-pl.easypack24.net/v1/send/compartment/status')
+               328 STORE_NAME              25 (status_sent)
+               330 LOAD_NAME                1 (str)
+               332 LOAD_NAME                2 (__annotations__)
+               334 LOAD_CONST              46 ('status_sent')
+               336 STORE_SUBSCR
+   
+    33         340 LOAD_CONST              47 ('https://api-inmobile-pl.easypack24.net/v1/send/confirm')
+               342 STORE_NAME              26 (confirm_sent)
+               344 LOAD_NAME                1 (str)
+               346 LOAD_NAME                2 (__annotations__)
+               348 LOAD_CONST              48 ('confirm_sent')
+               350 STORE_SUBSCR
+   
+    34         354 LOAD_CONST              49 ('https://api-inmobile-pl.easypack24.net/v1/prices/parcels')
+               356 STORE_NAME              27 (parcel_prices)
+               358 LOAD_NAME                1 (str)
+               360 LOAD_NAME                2 (__annotations__)
+               362 LOAD_CONST              50 ('parcel_prices')
+               364 STORE_SUBSCR
+   
+    37         368 LOAD_CONST              51 ('https://api-inmobile-pl.easypack24.net/v1/returns/parcels/')
+               370 STORE_NAME              28 (returns)
+               372 LOAD_NAME                1 (str)
+               374 LOAD_NAME                2 (__annotations__)
+               376 LOAD_CONST              52 ('returns')
+               378 STORE_SUBSCR
+   
+    38         382 LOAD_CONST              53 ('https://api-inmobile-pl.easypack24.net/v1/returns/tickets')
+               384 STORE_NAME              29 (tickets)
+               386 LOAD_NAME                1 (str)
+               388 LOAD_NAME                2 (__annotations__)
+               390 LOAD_CONST              54 ('tickets')
+               392 STORE_SUBSCR
+   
+    39         396 LOAD_CONST              55 ('https://api-inmobile-pl.easypack24.net/v2/notifications?type=PUSH%2CNEWS%2CTILE')
+               398 STORE_NAME              30 (parcel_notifications)
+               400 LOAD_NAME                1 (str)
+               402 LOAD_NAME                2 (__annotations__)
+               404 LOAD_CONST              56 ('parcel_notifications')
+               406 STORE_SUBSCR
+   
+    42         410 LOAD_CONST              57 ('https://api-inmobile-pl.easypack24.net/v1/friends/')
+               412 STORE_NAME              31 (friendship)
+               414 LOAD_NAME                1 (str)
+               416 LOAD_NAME                2 (__annotations__)
+               418 LOAD_CONST              58 ('friendship')
+               420 STORE_SUBSCR
+   
+    43         424 LOAD_CONST              59 ('https://api-inmobile-pl.easypack24.net/v1/invitations/validate')
+               426 STORE_NAME              32 (validate_friendship)
+               428 LOAD_NAME                1 (str)
+               430 LOAD_NAME                2 (__annotations__)
+               432 LOAD_CONST              60 ('validate_friendship')
+               434 STORE_SUBSCR
+   
+    44         438 LOAD_CONST              61 ('https://api-inmobile-pl.easypack24.net/v1/invitations/accept')
+               440 STORE_NAME              33 (accept_friendship)
+               442 LOAD_NAME                1 (str)
+               444 LOAD_NAME                2 (__annotations__)
+               446 LOAD_CONST              62 ('accept_friendship')
+               448 STORE_SUBSCR
+               452 LOAD_CONST              63 (None)
+               454 RETURN_VALUE
    consts
       'https://api-inmobile-pl.easypack24.net/v1/authenticate'
       'login'
       'https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/'
       'send_sms_code'
       'https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode'
       'confirm_sms_code'
+      'https://api-inmobile-pl.easypack24.net/v1/logout'
+      'logout'
       'refresh_token'
       'https://api-inmobile-pl.easypack24.net/v3/parcels/tracked'
       'parcels'
       'https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/'
       'parcel'
       'https://api-inmobile-pl.easypack24.net/v3/parcels/multi/'
       'multi'
@@ -196,38 +273,57 @@
       'reopen'
       'https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open'
       'compartment_open'
       'https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status'
       'compartment_status'
       'https://api-inmobile-pl.easypack24.net/v1/collect/terminate'
       'terminate_collect_session'
-      'https://api-inmobile-pl.easypack24.net/v1/friends/'
-      'friendship'
-      'https://api-inmobile-pl.easypack24.net/v1/invitations/validate'
-      'validate_friendship'
-      'https://api-inmobile-pl.easypack24.net/v1/invitations/accept'
-      'accept_friendship'
       'https://api-inmobile-pl.easypack24.net/v1/parcels/shared'
       'shared'
-      'https://api-inmobile-pl.easypack24.net/v3/parcels/sent/'
+      'https://api-inmobile-pl.easypack24.net/v1/parcels'
+      'create'
+      'https://api-inmobile-pl.easypack24.net/v3/points'
+      'points'
+      'https://api-inmobile-pl.easypack24.net/v1/payments/blik/alias/status'
+      'blik_status'
+      'https://api-inmobile-pl.easypack24.net/v1/payments/transactions/create/blik'
+      'create_blik'
+      'https://api-inmobile-pl.easypack24.net/v2/parcels/sent/'
       'sent'
-      'https://api-inmobile-pl.easypack24.net/v1/returns/parcels/'
-      'returns'
+      'https://api-inmobile-pl.easypack24.net/v3/points/'
+      'parcel_points'
+      'https://api-inmobile-pl.easypack24.net/v1/send/validate/'
+      'validate_sent'
+      'https://api-inmobile-pl.easypack24.net/v1/send/compartment/open'
+      'open_sent'
+      'https://api-inmobile-pl.easypack24.net/v1/send/compartment/reopen'
+      'reopen_sent'
+      'https://api-inmobile-pl.easypack24.net/v1/send/compartment/status'
+      'status_sent'
+      'https://api-inmobile-pl.easypack24.net/v1/send/confirm'
+      'confirm_sent'
       'https://api-inmobile-pl.easypack24.net/v1/prices/parcels'
       'parcel_prices'
+      'https://api-inmobile-pl.easypack24.net/v1/returns/parcels/'
+      'returns'
       'https://api-inmobile-pl.easypack24.net/v1/returns/tickets'
       'tickets'
-      'https://api-inmobile-pl.easypack24.net/v1/logout'
-      'logout'
       'https://api-inmobile-pl.easypack24.net/v2/notifications?type=PUSH%2CNEWS%2CTILE'
       'parcel_notifications'
+      'https://api-inmobile-pl.easypack24.net/v1/friends/'
+      'friendship'
+      'https://api-inmobile-pl.easypack24.net/v1/invitations/validate'
+      'validate_friendship'
+      'https://api-inmobile-pl.easypack24.net/v1/invitations/accept'
+      'accept_friendship'
       None
-   names      ('login', 'str', '__annotations__', 'send_sms_code', 'confirm_sms_code', 'refresh_token', 'parcels', 'parcel', 'multi', 'collect', 'reopen', 'compartment_open', 'compartment_status', 'terminate_collect_session', 'friendship', 'validate_friendship', 'accept_friendship', 'shared', 'sent', 'returns', 'parcel_prices', 'tickets', 'logout', 'parcel_notifications')
+   names      ('login', 'str', '__annotations__', 'send_sms_code', 'confirm_sms_code', 'logout', 'refresh_token', 'parcels', 'parcel', 'multi', 'collect', 'reopen', 'compartment_open', 'compartment_status', 'terminate_collect_session', 'shared', 'create', 'points', 'blik_status', 'create_blik', 'sent', 'parcel_points', 'validate_sent', 'open_sent', 'reopen_sent', 'status_sent', 'confirm_sent', 'parcel_prices', 'returns', 'tickets', 'parcel_notifications', 'friendship', 'validate_friendship', 'accept_friendship')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/loobson/pyprojects/inpost-python/inpost/static/endpoints.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010e010e030e010e010e010e010e010e010e010e010e010e
-      010e010e010e010e010e010e010e010e01
+      0x00ff020210010e010e010e010e030e010e010e010e010e010e010e010e
+      010e030e010e010e010e040e010e010e010e010e010e010e010e030e010e
+      010e030e010e01
```

### Comparing `inpost-0.1.3/inpost/static/__pycache__/exceptions.cpython-310.pyc` & `inpost-0.1.4/inpost/static/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/friends.cpython-310.pyc` & `inpost-0.1.4/inpost/static/__pycache__/friends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/friends.cpython-311.pyc` & `inpost-0.1.4/inpost/static/__pycache__/friends.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7ee8e463 (Thu Feb  9 12:35:10 2023 UTC)
-files sz: 1779
+moddate:  0x1d0c8f64 (Sun Jun 18 13:52:29 2023 UTC)
+files sz: 1717
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a030100020047
@@ -13,20 +13,20 @@
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
      3          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('get', 'Arrow'))
+                12 LOAD_CONST               2 (('Arrow', 'get'))
                 14 IMPORT_NAME              1 (arrow)
-                16 IMPORT_FROM              2 (get)
-                18 STORE_NAME               2 (get)
-                20 IMPORT_FROM              3 (Arrow)
-                22 STORE_NAME               3 (Arrow)
+                16 IMPORT_FROM              2 (Arrow)
+                18 STORE_NAME               2 (Arrow)
+                20 IMPORT_FROM              3 (get)
+                22 STORE_NAME               3 (get)
                 24 POP_TOP
    
      6          26 PUSH_NULL
                 28 LOAD_BUILD_CLASS
                 30 LOAD_CONST               3 (<code object Friend, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 6>)
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               4 ('Friend')
@@ -34,226 +34,219 @@
                 40 CALL                     2
                 50 STORE_NAME               4 (Friend)
                 52 LOAD_CONST               1 (None)
                 54 RETURN_VALUE
    consts
       0
       None
-      ('get', 'Arrow')
+      ('Arrow', 'get')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
-            0x8700970065005a0164005a02640165036a040000000000000000660288
-            0066016402840c5a056506640165036a0400000000000000006602640384
-            04a6000000ab0000000000000000005a07640484005a08880078015a0953
-            00
-                       0 MAKE_CELL                0 (__class__)
+            0x970065005a0164005a02640165036a0400000000000000006602640284
+            045a056506640165036a040000000000000000660264038404a6000000ab
+            0000000000000000005a07640484005a0864055300
+           6           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('Friend')
+                       8 STORE_NAME               2 (__qualname__)
          
-           6           2 RESUME                   0
-                       4 LOAD_NAME                0 (__name__)
-                       6 STORE_NAME               1 (__module__)
-                       8 LOAD_CONST               0 ('Friend')
-                      10 STORE_NAME               2 (__qualname__)
+           7          10 LOAD_CONST               1 ('logger')
+                      12 LOAD_NAME                3 (logging)
+                      14 LOAD_ATTR                4 (Logger)
+                      24 BUILD_TUPLE              2
+                      26 LOAD_CONST               2 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 7>)
+                      28 MAKE_FUNCTION            4 (annotations)
+                      30 STORE_NAME               5 (__init__)
          
-           7          12 LOAD_CONST               1 ('logger')
-                      14 LOAD_NAME                3 (logging)
-                      16 LOAD_ATTR                4 (Logger)
-                      26 BUILD_TUPLE              2
-                      28 LOAD_CLOSURE             0 (__class__)
-                      30 BUILD_TUPLE              1
-                      32 LOAD_CONST               2 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 7>)
-                      34 MAKE_FUNCTION           12 (annotations, closure)
-                      36 STORE_NAME               5 (__init__)
+          21          32 LOAD_NAME                6 (classmethod)
          
-          21          38 LOAD_NAME                6 (classmethod)
+          22          34 LOAD_CONST               1 ('logger')
+                      36 LOAD_NAME                3 (logging)
+                      38 LOAD_ATTR                4 (Logger)
+                      48 BUILD_TUPLE              2
+                      50 LOAD_CONST               3 (<code object from_invitation, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 21>)
+                      52 MAKE_FUNCTION            4 (annotations)
          
-          22          40 LOAD_CONST               1 ('logger')
-                      42 LOAD_NAME                3 (logging)
-                      44 LOAD_ATTR                4 (Logger)
-                      54 BUILD_TUPLE              2
-                      56 LOAD_CONST               3 (<code object from_invitation, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 21>)
-                      58 MAKE_FUNCTION            4 (annotations)
+          21          54 PRECALL                  0
+                      58 CALL                     0
          
-          21          60 PRECALL                  0
-                      64 CALL                     0
+          22          68 STORE_NAME               7 (from_invitation)
          
-          22          74 STORE_NAME               7 (from_invitation)
-         
-          32          76 LOAD_CONST               4 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 32>)
-                      78 MAKE_FUNCTION            0
-                      80 STORE_NAME               8 (__repr__)
-                      82 LOAD_CLOSURE             0 (__class__)
-                      84 COPY                     1
-                      86 STORE_NAME               9 (__classcell__)
-                      88 RETURN_VALUE
+          35          70 LOAD_CONST               4 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 35>)
+                      72 MAKE_FUNCTION            0
+                      74 STORE_NAME               8 (__repr__)
+                      76 LOAD_CONST               5 (None)
+                      78 RETURN_VALUE
          consts
             'Friend'
             'logger'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
-                  0x9501970064017c01760072087c016401190000000000000000006e0164
-                  007c005f0000000000000000007c016402190000000000000000007c005f
-                  0100000000000000007c016403190000000000000000007c005f02000000
-                  00000000007c02a003000000000000000000000000000000000000000089
-                  036a0400000000000000009b0064047c006a0000000000000000009b009d
-                  03a6010000ab0100000000000000007c005f05000000000000000064057c
-                  01760072087c016405190000000000000000006e0164007c005f06000000
-                  000000000064067c0176007215740f000000000000000000007c01640619
-                  000000000000000000a6010000ab0100000000000000006e0164007c005f
-                  08000000000000000064077c0176007215740f000000000000000000007c
-                  01640719000000000000000000a6010000ab0100000000000000006e0164
-                  007c005f0900000000000000007c006a06000000000000000072257c006a
-                  050000000000000000a00a00000000000000000000000000000000000000
-                  0064087c006a0200000000000000009b0064099d03a6010000ab01000000
-                  00000000000100640053007c006a050000000000000000a00a0000000000
-                  00000000000000000000000000000064087c006a0200000000000000009b
-                  009d02a6010000ab010000000000000000010064005300
-                             0 COPY_FREE_VARS           1
-               
-                 7           2 RESUME                   0
-               
-                 8           4 LOAD_CONST               1 ('uuid')
-                             6 LOAD_FAST                1 (friend_data)
-                             8 CONTAINS_OP              0
-                            10 POP_JUMP_FORWARD_IF_FALSE     8 (to 28)
-                            12 LOAD_FAST                1 (friend_data)
-                            14 LOAD_CONST               1 ('uuid')
-                            16 BINARY_SUBSCR
-                            26 JUMP_FORWARD             1 (to 30)
-                       >>   28 LOAD_CONST               0 (None)
-                       >>   30 LOAD_FAST                0 (self)
-                            32 STORE_ATTR               0 (uuid)
-               
-                 9          42 LOAD_FAST                1 (friend_data)
-                            44 LOAD_CONST               2 ('phoneNumber')
-                            46 BINARY_SUBSCR
-                            56 LOAD_FAST                0 (self)
-                            58 STORE_ATTR               1 (phone_number)
-               
-                10          68 LOAD_FAST                1 (friend_data)
-                            70 LOAD_CONST               3 ('name')
-                            72 BINARY_SUBSCR
-                            82 LOAD_FAST                0 (self)
-                            84 STORE_ATTR               2 (name)
-               
-                11          94 LOAD_FAST                2 (logger)
-                            96 LOAD_METHOD              3 (getChild)
-                           118 LOAD_DEREF               3 (__class__)
-                           120 LOAD_ATTR                4 (__name__)
-                           130 FORMAT_VALUE             0
-                           132 LOAD_CONST               4 ('.')
-                           134 LOAD_FAST                0 (self)
-                           136 LOAD_ATTR                0 (uuid)
-                           146 FORMAT_VALUE             0
-                           148 BUILD_STRING             3
-                           150 PRECALL                  1
-                           154 CALL                     1
-                           164 LOAD_FAST                0 (self)
-                           166 STORE_ATTR               5 (_log)
-               
-                12         176 LOAD_CONST               5 ('invitationCode')
-                           178 LOAD_FAST                1 (friend_data)
-                           180 CONTAINS_OP              0
-                           182 POP_JUMP_FORWARD_IF_FALSE     8 (to 200)
-                           184 LOAD_FAST                1 (friend_data)
-                           186 LOAD_CONST               5 ('invitationCode')
-                           188 BINARY_SUBSCR
-                           198 JUMP_FORWARD             1 (to 202)
-                       >>  200 LOAD_CONST               0 (None)
-                       >>  202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               6 (invitaion_code)
-               
-                13         214 LOAD_CONST               6 ('createdDate')
-                           216 LOAD_FAST                1 (friend_data)
-                           218 CONTAINS_OP              0
-                           220 POP_JUMP_FORWARD_IF_FALSE    21 (to 264)
-                           222 LOAD_GLOBAL             15 (NULL + get)
-                           234 LOAD_FAST                1 (friend_data)
-                           236 LOAD_CONST               6 ('createdDate')
-                           238 BINARY_SUBSCR
-                           248 PRECALL                  1
-                           252 CALL                     1
-                           262 JUMP_FORWARD             1 (to 266)
-                       >>  264 LOAD_CONST               0 (None)
-                       >>  266 LOAD_FAST                0 (self)
-                           268 STORE_ATTR               8 (created_date)
-               
-                14         278 LOAD_CONST               7 ('expiryDate')
-                           280 LOAD_FAST                1 (friend_data)
-                           282 CONTAINS_OP              0
-                           284 POP_JUMP_FORWARD_IF_FALSE    21 (to 328)
-                           286 LOAD_GLOBAL             15 (NULL + get)
-                           298 LOAD_FAST                1 (friend_data)
-                           300 LOAD_CONST               7 ('expiryDate')
-                           302 BINARY_SUBSCR
-                           312 PRECALL                  1
-                           316 CALL                     1
-                           326 JUMP_FORWARD             1 (to 330)
-                       >>  328 LOAD_CONST               0 (None)
-                       >>  330 LOAD_FAST                0 (self)
-                           332 STORE_ATTR               9 (expiry_date)
-               
-                16         342 LOAD_FAST                0 (self)
-                           344 LOAD_ATTR                6 (invitaion_code)
-                           354 POP_JUMP_FORWARD_IF_FALSE    37 (to 430)
-               
-                17         356 LOAD_FAST                0 (self)
-                           358 LOAD_ATTR                5 (_log)
-                           368 LOAD_METHOD             10 (debug)
-                           390 LOAD_CONST               8 ('created friendship with ')
-                           392 LOAD_FAST                0 (self)
-                           394 LOAD_ATTR                2 (name)
-                           404 FORMAT_VALUE             0
-                           406 LOAD_CONST               9 (' using from_invitation')
-                           408 BUILD_STRING             3
-                           410 PRECALL                  1
-                           414 CALL                     1
-                           424 POP_TOP
-                           426 LOAD_CONST               0 (None)
-                           428 RETURN_VALUE
-               
-                19     >>  430 LOAD_FAST                0 (self)
-                           432 LOAD_ATTR                5 (_log)
-                           442 LOAD_METHOD             10 (debug)
-                           464 LOAD_CONST               8 ('created friendship with ')
-                           466 LOAD_FAST                0 (self)
-                           468 LOAD_ATTR                2 (name)
-                           478 FORMAT_VALUE             0
-                           480 BUILD_STRING             2
-                           482 PRECALL                  1
-                           486 CALL                     1
-                           496 POP_TOP
-                           498 LOAD_CONST               0 (None)
-                           500 RETURN_VALUE
+                  0x970064017c01760072087c016401190000000000000000006e0164007c
+                  005f0000000000000000007c016402190000000000000000007c005f0100
+                  000000000000007c016403190000000000000000007c005f020000000000
+                  0000007c02a00300000000000000000000000000000000000000007c006a
+                  0400000000000000006a0500000000000000009b0064047c006a00000000
+                  00000000009b009d03a6010000ab0100000000000000007c005f06000000
+                  000000000064057c01760072087c016405190000000000000000006e0164
+                  007c005f07000000000000000064067c0176007215741100000000000000
+                  0000007c01640619000000000000000000a6010000ab0100000000000000
+                  006e0164007c005f09000000000000000064077c01760072157411000000
+                  000000000000007c01640719000000000000000000a6010000ab01000000
+                  00000000006e0164007c005f0a00000000000000007c006a070000000000
+                  00000072257c006a060000000000000000a00b0000000000000000000000
+                  00000000000000000064087c006a0200000000000000009b0064099d03a6
+                  010000ab0100000000000000000100640053007c006a0600000000000000
+                  00a00b000000000000000000000000000000000000000064087c006a0200
+                  000000000000009b009d02a6010000ab0100000000000000000100640053
+                  00
+                 7           0 RESUME                   0
+               
+                 8           2 LOAD_CONST               1 ('uuid')
+                             4 LOAD_FAST                1 (friend_data)
+                             6 CONTAINS_OP              0
+                             8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
+                            10 LOAD_FAST                1 (friend_data)
+                            12 LOAD_CONST               1 ('uuid')
+                            14 BINARY_SUBSCR
+                            24 JUMP_FORWARD             1 (to 28)
+                       >>   26 LOAD_CONST               0 (None)
+                       >>   28 LOAD_FAST                0 (self)
+                            30 STORE_ATTR               0 (uuid)
+               
+                 9          40 LOAD_FAST                1 (friend_data)
+                            42 LOAD_CONST               2 ('phoneNumber')
+                            44 BINARY_SUBSCR
+                            54 LOAD_FAST                0 (self)
+                            56 STORE_ATTR               1 (phone_number)
+               
+                10          66 LOAD_FAST                1 (friend_data)
+                            68 LOAD_CONST               3 ('name')
+                            70 BINARY_SUBSCR
+                            80 LOAD_FAST                0 (self)
+                            82 STORE_ATTR               2 (name)
+               
+                11          92 LOAD_FAST                2 (logger)
+                            94 LOAD_METHOD              3 (getChild)
+                           116 LOAD_FAST                0 (self)
+                           118 LOAD_ATTR                4 (__class__)
+                           128 LOAD_ATTR                5 (__name__)
+                           138 FORMAT_VALUE             0
+                           140 LOAD_CONST               4 ('.')
+                           142 LOAD_FAST                0 (self)
+                           144 LOAD_ATTR                0 (uuid)
+                           154 FORMAT_VALUE             0
+                           156 BUILD_STRING             3
+                           158 PRECALL                  1
+                           162 CALL                     1
+                           172 LOAD_FAST                0 (self)
+                           174 STORE_ATTR               6 (_log)
+               
+                12         184 LOAD_CONST               5 ('invitationCode')
+                           186 LOAD_FAST                1 (friend_data)
+                           188 CONTAINS_OP              0
+                           190 POP_JUMP_FORWARD_IF_FALSE     8 (to 208)
+                           192 LOAD_FAST                1 (friend_data)
+                           194 LOAD_CONST               5 ('invitationCode')
+                           196 BINARY_SUBSCR
+                           206 JUMP_FORWARD             1 (to 210)
+                       >>  208 LOAD_CONST               0 (None)
+                       >>  210 LOAD_FAST                0 (self)
+                           212 STORE_ATTR               7 (invitaion_code)
+               
+                13         222 LOAD_CONST               6 ('createdDate')
+                           224 LOAD_FAST                1 (friend_data)
+                           226 CONTAINS_OP              0
+                           228 POP_JUMP_FORWARD_IF_FALSE    21 (to 272)
+                           230 LOAD_GLOBAL             17 (NULL + get)
+                           242 LOAD_FAST                1 (friend_data)
+                           244 LOAD_CONST               6 ('createdDate')
+                           246 BINARY_SUBSCR
+                           256 PRECALL                  1
+                           260 CALL                     1
+                           270 JUMP_FORWARD             1 (to 274)
+                       >>  272 LOAD_CONST               0 (None)
+                       >>  274 LOAD_FAST                0 (self)
+                           276 STORE_ATTR               9 (created_date)
+               
+                14         286 LOAD_CONST               7 ('expiryDate')
+                           288 LOAD_FAST                1 (friend_data)
+                           290 CONTAINS_OP              0
+                           292 POP_JUMP_FORWARD_IF_FALSE    21 (to 336)
+                           294 LOAD_GLOBAL             17 (NULL + get)
+                           306 LOAD_FAST                1 (friend_data)
+                           308 LOAD_CONST               7 ('expiryDate')
+                           310 BINARY_SUBSCR
+                           320 PRECALL                  1
+                           324 CALL                     1
+                           334 JUMP_FORWARD             1 (to 338)
+                       >>  336 LOAD_CONST               0 (None)
+                       >>  338 LOAD_FAST                0 (self)
+                           340 STORE_ATTR              10 (expiry_date)
+               
+                16         350 LOAD_FAST                0 (self)
+                           352 LOAD_ATTR                7 (invitaion_code)
+                           362 POP_JUMP_FORWARD_IF_FALSE    37 (to 438)
+               
+                17         364 LOAD_FAST                0 (self)
+                           366 LOAD_ATTR                6 (_log)
+                           376 LOAD_METHOD             11 (debug)
+                           398 LOAD_CONST               8 ('created friendship with ')
+                           400 LOAD_FAST                0 (self)
+                           402 LOAD_ATTR                2 (name)
+                           412 FORMAT_VALUE             0
+                           414 LOAD_CONST               9 (' using from_invitation')
+                           416 BUILD_STRING             3
+                           418 PRECALL                  1
+                           422 CALL                     1
+                           432 POP_TOP
+                           434 LOAD_CONST               0 (None)
+                           436 RETURN_VALUE
+               
+                19     >>  438 LOAD_FAST                0 (self)
+                           440 LOAD_ATTR                6 (_log)
+                           450 LOAD_METHOD             11 (debug)
+                           472 LOAD_CONST               8 ('created friendship with ')
+                           474 LOAD_FAST                0 (self)
+                           476 LOAD_ATTR                2 (name)
+                           486 FORMAT_VALUE             0
+                           488 BUILD_STRING             2
+                           490 PRECALL                  1
+                           494 CALL                     1
+                           504 POP_TOP
+                           506 LOAD_CONST               0 (None)
+                           508 RETURN_VALUE
                consts
                   None
                   'uuid'
                   'phoneNumber'
                   'name'
                   '.'
                   'invitationCode'
                   'createdDate'
                   'expiryDate'
                   'created friendship with '
                   ' using from_invitation'
-               names      ('uuid', 'phone_number', 'name', 'getChild', '__name__', '_log', 'invitaion_code', 'get', 'created_date', 'expiry_date', 'debug')
+               names      ('uuid', 'phone_number', 'name', 'getChild', '__class__', '__name__', '_log', 'invitaion_code', 'get', 'created_date', 'expiry_date', 'debug')
                varnames   ('self', 'friend_data', 'logger')
-               freevars   ('__class__',)
+               freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/friends.py'
                name       '__init__'
                firstlineno 7
-               lnotab 0x040126011a011a0152012601400140020e014a02
+               lnotab 0x020126011a011a015c012601400140020e014a02
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 9
                flags     : 3
                code
                   0x970002007c007c01640119000000000000000000640219000000000000
@@ -262,48 +255,49 @@
                   0000000000000000007c016406190000000000000000007c016407190000
                   0000000000000064089c067c02ac09a6020000ab02000000000000000053
                   00
                 21           0 RESUME                   0
                
                 23           2 PUSH_NULL
                              4 LOAD_FAST                0 (cls)
-                             6 LOAD_FAST                1 (invitation_data)
+               
+                25           6 LOAD_FAST                1 (invitation_data)
                              8 LOAD_CONST               1 ('friend')
                             10 BINARY_SUBSCR
                             20 LOAD_CONST               2 ('uuid')
                             22 BINARY_SUBSCR
                
-                24          32 LOAD_FAST                1 (invitation_data)
+                26          32 LOAD_FAST                1 (invitation_data)
                             34 LOAD_CONST               1 ('friend')
                             36 BINARY_SUBSCR
                             46 LOAD_CONST               3 ('phoneNumber')
                             48 BINARY_SUBSCR
                
-                25          58 LOAD_FAST                1 (invitation_data)
+                27          58 LOAD_FAST                1 (invitation_data)
                             60 LOAD_CONST               1 ('friend')
                             62 BINARY_SUBSCR
                             72 LOAD_CONST               4 ('name')
                             74 BINARY_SUBSCR
                
-                26          84 LOAD_FAST                1 (invitation_data)
+                28          84 LOAD_FAST                1 (invitation_data)
                             86 LOAD_CONST               5 ('invitationCode')
                             88 BINARY_SUBSCR
                
-                27          98 LOAD_FAST                1 (invitation_data)
+                29          98 LOAD_FAST                1 (invitation_data)
                            100 LOAD_CONST               6 ('createdDate')
                            102 BINARY_SUBSCR
                
-                28         112 LOAD_FAST                1 (invitation_data)
+                30         112 LOAD_FAST                1 (invitation_data)
                            114 LOAD_CONST               7 ('expiryDate')
                            116 BINARY_SUBSCR
                
-                23         126 LOAD_CONST               8 (('uuid', 'phoneNumber', 'name', 'invitationCode', 'createdDate', 'expiryDate'))
+                24         126 LOAD_CONST               8 (('uuid', 'phoneNumber', 'name', 'invitationCode', 'createdDate', 'expiryDate'))
                            128 BUILD_CONST_KEY_MAP      6
                
-                30         130 LOAD_FAST                2 (logger)
+                32         130 LOAD_FAST                2 (logger)
                
                 23         132 KW_NAMES                 9
                            134 PRECALL                  2
                            138 CALL                     2
                            148 RETURN_VALUE
                consts
                   None
@@ -319,15 +313,15 @@
                names      ()
                varnames   ('cls', 'invitation_data', 'logger')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/friends.py'
                name       'from_invitation'
                firstlineno 21
-               lnotab 0x02021e011a011a010e010e010efb040702f9
+               lnotab 0x020204021a011a011a010e010e010efa040802f7
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
                   0x9700740100000000000000000000640184007c006a0100000000000000
@@ -335,32 +329,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-                32           0 RESUME                   0
+                35           0 RESUME                   0
                
-                33           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 33>)
+                36           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/friends.py", line 36>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-                34          98 LOAD_FAST                0 (self)
+                37          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -382,15 +376,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                      33           0 RETURN_GENERATOR
+                      36           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -416,36 +410,37 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/friends.py'
                      name       '<genexpr>'
-                     firstlineno 33
+                     firstlineno 36
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/friends.py'
                name       '__repr__'
-               firstlineno 32
+               firstlineno 35
                lnotab 0x02016001
-         names      ('__name__', '__module__', '__qualname__', 'logging', 'Logger', '__init__', 'classmethod', 'from_invitation', '__repr__', '__classcell__')
+            None
+         names      ('__name__', '__module__', '__qualname__', 'logging', 'Logger', '__init__', 'classmethod', 'from_invitation', '__repr__')
          varnames   ()
          freevars   ()
-         cellvars   ('__class__',)
+         cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/friends.py'
          name       'Friend'
          firstlineno 6
-         lnotab 0x0c011a0e020114ff0e01020a
+         lnotab 0x0a01160e020114ff0e01020d
       'Friend'
-   names      ('logging', 'arrow', 'get', 'Arrow', 'Friend')
+   names      ('logging', 'arrow', 'Arrow', 'get', 'Friend')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/loobson/pyprojects/inpost-python/inpost/static/friends.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108021003
```

### Comparing `inpost-0.1.3/inpost/static/__pycache__/parcels.cpython-310.pyc` & `inpost-0.1.4/inpost/static/__pycache__/parcels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/statuses.cpython-310.pyc` & `inpost-0.1.4/inpost/static/__pycache__/statuses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.3/inpost/static/__pycache__/statuses.cpython-311.pyc` & `inpost-0.1.4/inpost/static/__pycache__/statuses.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,565 +1,442 @@
 magic:    0xa70d0d0a
-moddate:  0x63c56364 (Tue May 16 18:03:15 2023 UTC)
-files sz: 7066
+moddate:  0xb8cf9664 (Sat Jun 24 11:12:56 2023 UTC)
+files sz: 8052
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a020100640064026c036d045a0401
-      00020047006403840064046502a6030000ab0300000000000000005a0502
-      00470064058400640665016505ac07a6040000ab0400000000000000005a
-      06020047006408840064096506a6030000ab0300000000000000005a0702
-      004700640a8400640b6506a6030000ab0300000000000000005a08020047
-      00640c8400640d6506a6030000ab0300000000000000005a090200470064
-      0e8400640f6506a6030000ab0300000000000000005a0a02004700641084
-      0064116506a6030000ab0300000000000000005a0b020047006412840064
-      136506a6030000ab0300000000000000005a0c0200470064148400641565
-      06a6030000ab0300000000000000005a0d020047006416840064176506a6
-      030000ab0300000000000000005a0e020047006418840064196506a60300
-      00ab0300000000000000005a0f02004700641a8400641b6506a6030000ab
-      0300000000000000005a1002004700641c8400641d6506a6030000ab0300
-      000000000000005a1102004700641e8400641f6506a6030000ab03000000
-      00000000005a1264205300
+      0x9700640064016c006d015a016d025a0201000200470064028400640365
+      02a6030000ab0300000000000000005a0302004700640484006405650165
+      03ac06a6040000ab0400000000000000005a040200470064078400640865
+      04a6030000ab0300000000000000005a050200470064098400640a6504a6
+      030000ab0300000000000000005a0602004700640b8400640c6504a60300
+      00ab0300000000000000005a0702004700640d8400640e6504a6030000ab
+      0300000000000000005a0802004700640f840064106504a6030000ab0300
+      000000000000005a09020047006411840064126504a6030000ab03000000
+      00000000005a0a020047006413840064146504a6030000ab030000000000
+      0000005a0b020047006415840064166504a6030000ab0300000000000000
+      005a0c020047006417840064186504a6030000ab0300000000000000005a
+      0d0200470064198400641a6504a6030000ab0300000000000000005a0e02
+      004700641b8400641c6504a6030000ab0300000000000000005a0f020047
+      00641d8400641e6504a6030000ab0300000000000000005a100200470064
+      1f840064206504a6030000ab0300000000000000005a1102004700642184
+      0064226504a6030000ab0300000000000000005a12020047006423840064
+      246504a6030000ab0300000000000000005a130200470064258400642665
+      04a6030000ab0300000000000000005a14020047006427840064286504a6
+      030000ab0300000000000000005a1564295300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Enum', 'EnumMeta'))
                  6 IMPORT_NAME              0 (enum)
                  8 IMPORT_FROM              1 (Enum)
                 10 STORE_NAME               1 (Enum)
                 12 IMPORT_FROM              2 (EnumMeta)
                 14 STORE_NAME               2 (EnumMeta)
                 16 POP_TOP
    
-     2          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('List',))
-                22 IMPORT_NAME              3 (typing)
-                24 IMPORT_FROM              4 (List)
-                26 STORE_NAME               4 (List)
-                28 POP_TOP
+     4          18 PUSH_NULL
+                20 LOAD_BUILD_CLASS
+                22 LOAD_CONST               2 (<code object Meta, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 4>)
+                24 MAKE_FUNCTION            0
+                26 LOAD_CONST               3 ('Meta')
+                28 LOAD_NAME                2 (EnumMeta)
+                30 PRECALL                  3
+                34 CALL                     3
+                44 STORE_NAME               3 (Meta)
    
-     5          30 PUSH_NULL
-                32 LOAD_BUILD_CLASS
-                34 LOAD_CONST               3 (<code object Meta, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 5>)
-                36 MAKE_FUNCTION            0
-                38 LOAD_CONST               4 ('Meta')
-                40 LOAD_NAME                2 (EnumMeta)
-                42 PRECALL                  3
-                46 CALL                     3
-                56 STORE_NAME               5 (Meta)
+    27          46 PUSH_NULL
+                48 LOAD_BUILD_CLASS
+                50 LOAD_CONST               4 (<code object ParcelBase, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 27>)
+                52 MAKE_FUNCTION            0
+                54 LOAD_CONST               5 ('ParcelBase')
+                56 LOAD_NAME                1 (Enum)
+                58 LOAD_NAME                3 (Meta)
+                60 KW_NAMES                 6
+                62 PRECALL                  4
+                66 CALL                     4
+                76 STORE_NAME               4 (ParcelBase)
    
-    28          58 PUSH_NULL
-                60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object ParcelBase, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 28>)
-                64 MAKE_FUNCTION            0
-                66 LOAD_CONST               6 ('ParcelBase')
-                68 LOAD_NAME                1 (Enum)
-                70 LOAD_NAME                5 (Meta)
-                72 KW_NAMES                 7
-                74 PRECALL                  4
-                78 CALL                     4
-                88 STORE_NAME               6 (ParcelBase)
+    65          78 PUSH_NULL
+                80 LOAD_BUILD_CLASS
+                82 LOAD_CONST               7 (<code object ParcelCarrierSize, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 65>)
+                84 MAKE_FUNCTION            0
+                86 LOAD_CONST               8 ('ParcelCarrierSize')
+                88 LOAD_NAME                4 (ParcelBase)
+                90 PRECALL                  3
+                94 CALL                     3
+               104 STORE_NAME               5 (ParcelCarrierSize)
    
-    66          90 PUSH_NULL
-                92 LOAD_BUILD_CLASS
-                94 LOAD_CONST               8 (<code object ParcelCarrierSize, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 66>)
-                96 MAKE_FUNCTION            0
-                98 LOAD_CONST               9 ('ParcelCarrierSize')
-               100 LOAD_NAME                6 (ParcelBase)
-               102 PRECALL                  3
-               106 CALL                     3
-               116 STORE_NAME               7 (ParcelCarrierSize)
+    76         106 PUSH_NULL
+               108 LOAD_BUILD_CLASS
+               110 LOAD_CONST               9 (<code object ParcelLockerSize, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 76>)
+               112 MAKE_FUNCTION            0
+               114 LOAD_CONST              10 ('ParcelLockerSize')
+               116 LOAD_NAME                4 (ParcelBase)
+               118 PRECALL                  3
+               122 CALL                     3
+               132 STORE_NAME               6 (ParcelLockerSize)
    
-    76         118 PUSH_NULL
-               120 LOAD_BUILD_CLASS
-               122 LOAD_CONST              10 (<code object ParcelLockerSize, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 76>)
-               124 MAKE_FUNCTION            0
-               126 LOAD_CONST              11 ('ParcelLockerSize')
-               128 LOAD_NAME                6 (ParcelBase)
-               130 PRECALL                  3
-               134 CALL                     3
-               144 STORE_NAME               8 (ParcelLockerSize)
+    85         134 PUSH_NULL
+               136 LOAD_BUILD_CLASS
+               138 LOAD_CONST              11 (<code object ParcelDeliveryType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 85>)
+               140 MAKE_FUNCTION            0
+               142 LOAD_CONST              12 ('ParcelDeliveryType')
+               144 LOAD_NAME                4 (ParcelBase)
+               146 PRECALL                  3
+               150 CALL                     3
+               160 STORE_NAME               7 (ParcelDeliveryType)
    
-    84         146 PUSH_NULL
-               148 LOAD_BUILD_CLASS
-               150 LOAD_CONST              12 (<code object ParcelDeliveryType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 84>)
-               152 MAKE_FUNCTION            0
-               154 LOAD_CONST              13 ('ParcelDeliveryType')
-               156 LOAD_NAME                6 (ParcelBase)
-               158 PRECALL                  3
-               162 CALL                     3
-               172 STORE_NAME               9 (ParcelDeliveryType)
+    94         162 PUSH_NULL
+               164 LOAD_BUILD_CLASS
+               166 LOAD_CONST              13 (<code object ParcelShipmentType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 94>)
+               168 MAKE_FUNCTION            0
+               170 LOAD_CONST              14 ('ParcelShipmentType')
+               172 LOAD_NAME                4 (ParcelBase)
+               174 PRECALL                  3
+               178 CALL                     3
+               188 STORE_NAME               8 (ParcelShipmentType)
    
-    92         174 PUSH_NULL
-               176 LOAD_BUILD_CLASS
-               178 LOAD_CONST              14 (<code object ParcelShipmentType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 92>)
-               180 MAKE_FUNCTION            0
-               182 LOAD_CONST              15 ('ParcelShipmentType')
-               184 LOAD_NAME                6 (ParcelBase)
-               186 PRECALL                  3
-               190 CALL                     3
-               200 STORE_NAME              10 (ParcelShipmentType)
+   103         190 PUSH_NULL
+               192 LOAD_BUILD_CLASS
+               194 LOAD_CONST              15 (<code object ParcelAdditionalInsurance, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 103>)
+               196 MAKE_FUNCTION            0
+               198 LOAD_CONST              16 ('ParcelAdditionalInsurance')
+               200 LOAD_NAME                4 (ParcelBase)
+               202 PRECALL                  3
+               206 CALL                     3
+               216 STORE_NAME               9 (ParcelAdditionalInsurance)
    
-   100         202 PUSH_NULL
-               204 LOAD_BUILD_CLASS
-               206 LOAD_CONST              16 (<code object ParcelAdditionalInsurance, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 100>)
-               208 MAKE_FUNCTION            0
-               210 LOAD_CONST              17 ('ParcelAdditionalInsurance')
-               212 LOAD_NAME                6 (ParcelBase)
-               214 PRECALL                  3
-               218 CALL                     3
-               228 STORE_NAME              11 (ParcelAdditionalInsurance)
+   111         218 PUSH_NULL
+               220 LOAD_BUILD_CLASS
+               222 LOAD_CONST              17 (<code object ParcelType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 111>)
+               224 MAKE_FUNCTION            0
+               226 LOAD_CONST              18 ('ParcelType')
+               228 LOAD_NAME                4 (ParcelBase)
+               230 PRECALL                  3
+               234 CALL                     3
+               244 STORE_NAME              10 (ParcelType)
    
-   108         230 PUSH_NULL
-               232 LOAD_BUILD_CLASS
-               234 LOAD_CONST              18 (<code object ParcelType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 108>)
-               236 MAKE_FUNCTION            0
-               238 LOAD_CONST              19 ('ParcelType')
-               240 LOAD_NAME                6 (ParcelBase)
-               242 PRECALL                  3
-               246 CALL                     3
-               256 STORE_NAME              12 (ParcelType)
+   120         246 PUSH_NULL
+               248 LOAD_BUILD_CLASS
+               250 LOAD_CONST              19 (<code object PointType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 120>)
+               252 MAKE_FUNCTION            0
+               254 LOAD_CONST              20 ('PointType')
+               256 LOAD_NAME                4 (ParcelBase)
+               258 PRECALL                  3
+               262 CALL                     3
+               272 STORE_NAME              11 (PointType)
    
-   116         258 PUSH_NULL
-               260 LOAD_BUILD_CLASS
-               262 LOAD_CONST              20 (<code object ParcelStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 116>)
-               264 MAKE_FUNCTION            0
-               266 LOAD_CONST              21 ('ParcelStatus')
-               268 LOAD_NAME                6 (ParcelBase)
-               270 PRECALL                  3
-               274 CALL                     3
-               284 STORE_NAME              13 (ParcelStatus)
+   130         274 PUSH_NULL
+               276 LOAD_BUILD_CLASS
+               278 LOAD_CONST              21 (<code object ParcelPointOperations, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 130>)
+               280 MAKE_FUNCTION            0
+               282 LOAD_CONST              22 ('ParcelPointOperations')
+               284 LOAD_NAME                4 (ParcelBase)
+               286 PRECALL                  3
+               290 CALL                     3
+               300 STORE_NAME              12 (ParcelPointOperations)
    
-   163         286 PUSH_NULL
-               288 LOAD_BUILD_CLASS
-               290 LOAD_CONST              22 (<code object ReturnsStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 163>)
-               292 MAKE_FUNCTION            0
-               294 LOAD_CONST              23 ('ReturnsStatus')
-               296 LOAD_NAME                6 (ParcelBase)
-               298 PRECALL                  3
-               302 CALL                     3
-               312 STORE_NAME              14 (ReturnsStatus)
+   138         302 PUSH_NULL
+               304 LOAD_BUILD_CLASS
+               306 LOAD_CONST              23 (<code object ParcelStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 138>)
+               308 MAKE_FUNCTION            0
+               310 LOAD_CONST              24 ('ParcelStatus')
+               312 LOAD_NAME                4 (ParcelBase)
+               314 PRECALL                  3
+               318 CALL                     3
+               328 STORE_NAME              13 (ParcelStatus)
    
-   170         314 PUSH_NULL
-               316 LOAD_BUILD_CLASS
-               318 LOAD_CONST              24 (<code object ParcelOwnership, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 170>)
-               320 MAKE_FUNCTION            0
-               322 LOAD_CONST              25 ('ParcelOwnership')
-               324 LOAD_NAME                6 (ParcelBase)
-               326 PRECALL                  3
-               330 CALL                     3
-               340 STORE_NAME              15 (ParcelOwnership)
+   188         330 PUSH_NULL
+               332 LOAD_BUILD_CLASS
+               334 LOAD_CONST              25 (<code object DeliveryType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 188>)
+               336 MAKE_FUNCTION            0
+               338 LOAD_CONST              26 ('DeliveryType')
+               340 LOAD_NAME                4 (ParcelBase)
+               342 PRECALL                  3
+               346 CALL                     3
+               356 STORE_NAME              14 (DeliveryType)
    
-   178         342 PUSH_NULL
-               344 LOAD_BUILD_CLASS
-               346 LOAD_CONST              26 (<code object CompartmentExpectedStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 178>)
-               348 MAKE_FUNCTION            0
-               350 LOAD_CONST              27 ('CompartmentExpectedStatus')
-               352 LOAD_NAME                6 (ParcelBase)
-               354 PRECALL                  3
-               358 CALL                     3
-               368 STORE_NAME              16 (CompartmentExpectedStatus)
+   193         358 PUSH_NULL
+               360 LOAD_BUILD_CLASS
+               362 LOAD_CONST              27 (<code object ReturnsStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 193>)
+               364 MAKE_FUNCTION            0
+               366 LOAD_CONST              28 ('ReturnsStatus')
+               368 LOAD_NAME                4 (ParcelBase)
+               370 PRECALL                  3
+               374 CALL                     3
+               384 STORE_NAME              15 (ReturnsStatus)
    
-   185         370 PUSH_NULL
-               372 LOAD_BUILD_CLASS
-               374 LOAD_CONST              28 (<code object CompartmentActualStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 185>)
-               376 MAKE_FUNCTION            0
-               378 LOAD_CONST              29 ('CompartmentActualStatus')
-               380 LOAD_NAME                6 (ParcelBase)
-               382 PRECALL                  3
-               386 CALL                     3
-               396 STORE_NAME              17 (CompartmentActualStatus)
+   200         386 PUSH_NULL
+               388 LOAD_BUILD_CLASS
+               390 LOAD_CONST              29 (<code object ParcelOwnership, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 200>)
+               392 MAKE_FUNCTION            0
+               394 LOAD_CONST              30 ('ParcelOwnership')
+               396 LOAD_NAME                4 (ParcelBase)
+               398 PRECALL                  3
+               402 CALL                     3
+               412 STORE_NAME              16 (ParcelOwnership)
    
-   192         398 PUSH_NULL
-               400 LOAD_BUILD_CLASS
-               402 LOAD_CONST              30 (<code object ParcelServiceName, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 192>)
-               404 MAKE_FUNCTION            0
-               406 LOAD_CONST              31 ('ParcelServiceName')
-               408 LOAD_NAME                6 (ParcelBase)
-               410 PRECALL                  3
-               414 CALL                     3
-               424 STORE_NAME              18 (ParcelServiceName)
-               426 LOAD_CONST              32 (None)
-               428 RETURN_VALUE
+   209         414 PUSH_NULL
+               416 LOAD_BUILD_CLASS
+               418 LOAD_CONST              31 (<code object CompartmentExpectedStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 209>)
+               420 MAKE_FUNCTION            0
+               422 LOAD_CONST              32 ('CompartmentExpectedStatus')
+               424 LOAD_NAME                4 (ParcelBase)
+               426 PRECALL                  3
+               430 CALL                     3
+               440 STORE_NAME              17 (CompartmentExpectedStatus)
+   
+   217         442 PUSH_NULL
+               444 LOAD_BUILD_CLASS
+               446 LOAD_CONST              33 (<code object CompartmentActualStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 217>)
+               448 MAKE_FUNCTION            0
+               450 LOAD_CONST              34 ('CompartmentActualStatus')
+               452 LOAD_NAME                4 (ParcelBase)
+               454 PRECALL                  3
+               458 CALL                     3
+               468 STORE_NAME              18 (CompartmentActualStatus)
+   
+   225         470 PUSH_NULL
+               472 LOAD_BUILD_CLASS
+               474 LOAD_CONST              35 (<code object PaymentType, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 225>)
+               476 MAKE_FUNCTION            0
+               478 LOAD_CONST              36 ('PaymentType')
+               480 LOAD_NAME                4 (ParcelBase)
+               482 PRECALL                  3
+               486 CALL                     3
+               496 STORE_NAME              19 (PaymentType)
+   
+   231         498 PUSH_NULL
+               500 LOAD_BUILD_CLASS
+               502 LOAD_CONST              37 (<code object PaymentStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 231>)
+               504 MAKE_FUNCTION            0
+               506 LOAD_CONST              38 ('PaymentStatus')
+               508 LOAD_NAME                4 (ParcelBase)
+               510 PRECALL                  3
+               514 CALL                     3
+               524 STORE_NAME              20 (PaymentStatus)
+   
+   236         526 PUSH_NULL
+               528 LOAD_BUILD_CLASS
+               530 LOAD_CONST              39 (<code object ParcelServiceName, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 236>)
+               532 MAKE_FUNCTION            0
+               534 LOAD_CONST              40 ('ParcelServiceName')
+               536 LOAD_NAME                4 (ParcelBase)
+               538 PRECALL                  3
+               542 CALL                     3
+               552 STORE_NAME              21 (ParcelServiceName)
+               554 LOAD_CONST              41 (None)
+               556 RETURN_VALUE
    consts
       0
       ('Enum', 'EnumMeta')
-      ('List',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 4
+         stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a0388006601640284
-            085a04640384005a056404640565066405190000000000000000007a0700
-            006602640684045a07880078015a085300
+            085a04880078015a055300
                        0 MAKE_CELL                0 (__class__)
          
-           5           2 RESUME                   0
+           4           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Meta')
                       10 STORE_NAME               2 (__qualname__)
          
-           6          12 LOAD_CLOSURE             0 (__class__)
+           5          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __getitem__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 6>)
+                      16 LOAD_CONST               1 (<code object __getitem__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 5>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__getitem__)
          
-          12          22 LOAD_CLOSURE             0 (__class__)
+          11          22 LOAD_CLOSURE             0 (__class__)
                       24 BUILD_TUPLE              1
-                      26 LOAD_CONST               2 (<code object __getattribute__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 12>)
+                      26 LOAD_CONST               2 (<code object __getattribute__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 11>)
                       28 MAKE_FUNCTION            8 (closure)
                       30 STORE_NAME               4 (__getattribute__)
-         
-          18          32 LOAD_CONST               3 (<code object get_all, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 18>)
-                      34 MAKE_FUNCTION            0
-                      36 STORE_NAME               5 (get_all)
-         
-          21          38 LOAD_CONST               4 ('without')
-                      40 LOAD_CONST               5 ('ParcelBase')
-                      42 LOAD_NAME                6 (List)
-                      44 LOAD_CONST               5 ('ParcelBase')
-                      46 BINARY_SUBSCR
-                      56 BINARY_OP                7 (|)
-                      60 BUILD_TUPLE              2
-                      62 LOAD_CONST               6 (<code object get_without, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 21>)
-                      64 MAKE_FUNCTION            4 (annotations)
-                      66 STORE_NAME               7 (get_without)
-                      68 LOAD_CLOSURE             0 (__class__)
-                      70 COPY                     1
-                      72 STORE_NAME               8 (__classcell__)
-                      74 RETURN_VALUE
+                      32 LOAD_CLOSURE             0 (__class__)
+                      34 COPY                     1
+                      36 STORE_NAME               5 (__classcell__)
+                      38 RETURN_VALUE
          consts
             'Meta'
             code
                argcount  : 2
-               nlocals   : 3
+               nlocals   : 2
                stacksize : 4
                flags     : 3
                code
-                  0x950197000900740100000000000000000000a6000000ab000000000000
-                  000000a00100000000000000000000000000000000000000007c01a60100
-                  00ab01000000000000000053002300740400000000000000000000240072
-                  117d027c006a0300000000000000006302590064007d027e02530064007d
-                  027e0277017700780359007701
+                  0x9501970009007c018121740100000000000000000000a6000000ab0000
+                  00000000000000a00100000000000000000000000000000000000000007c
+                  01a6010000ab0100000000000000006e0164005300230074040000000000
+                  00000000002400720a01007c006a03000000000000000063025900530077
+                  00780359007701
                              0 COPY_FREE_VARS           1
                
-                 6           2 RESUME                   0
+                 5           2 RESUME                   0
                
-                 7           4 NOP
+                 6           4 NOP
                
-                 8           6 LOAD_GLOBAL              1 (NULL + super)
-                            18 PRECALL                  0
-                            22 CALL                     0
-                            32 LOAD_METHOD              1 (__getitem__)
-                            54 LOAD_FAST                1 (item)
-                            56 PRECALL                  1
-                            60 CALL                     1
-                            70 RETURN_VALUE
-                       >>   72 PUSH_EXC_INFO
-               
-                 9          74 LOAD_GLOBAL              4 (KeyError)
-                            86 CHECK_EXC_MATCH
-                            88 POP_JUMP_FORWARD_IF_FALSE    17 (to 124)
-                            90 STORE_FAST               2 (error)
-               
-                10          92 LOAD_FAST                0 (cls)
-                            94 LOAD_ATTR                3 (UNKNOWN)
-                           104 SWAP                     2
-                           106 POP_EXCEPT
-                           108 LOAD_CONST               0 (None)
-                           110 STORE_FAST               2 (error)
-                           112 DELETE_FAST              2 (error)
-                           114 RETURN_VALUE
-                       >>  116 LOAD_CONST               0 (None)
-                           118 STORE_FAST               2 (error)
-                           120 DELETE_FAST              2 (error)
-                           122 RERAISE                  1
-               
-                 9     >>  124 RERAISE                  0
-                       >>  126 COPY                     3
-                           128 POP_EXCEPT
-                           130 RERAISE                  1
+                 7           6 LOAD_FAST                1 (item)
+                             8 POP_JUMP_FORWARD_IF_NONE    33 (to 76)
+                            10 LOAD_GLOBAL              1 (NULL + super)
+                            22 PRECALL                  0
+                            26 CALL                     0
+                            36 LOAD_METHOD              1 (__getitem__)
+                            58 LOAD_FAST                1 (item)
+                            60 PRECALL                  1
+                            64 CALL                     1
+                            74 JUMP_FORWARD             1 (to 78)
+                       >>   76 LOAD_CONST               0 (None)
+                       >>   78 RETURN_VALUE
+                       >>   80 PUSH_EXC_INFO
+               
+                 8          82 LOAD_GLOBAL              4 (KeyError)
+                            94 CHECK_EXC_MATCH
+                            96 POP_JUMP_FORWARD_IF_FALSE    10 (to 118)
+                            98 POP_TOP
+               
+                 9         100 LOAD_FAST                0 (self)
+                           102 LOAD_ATTR                3 (UNKNOWN)
+                           112 SWAP                     2
+                           114 POP_EXCEPT
+                           116 RETURN_VALUE
+               
+                 8     >>  118 RERAISE                  0
+                       >>  120 COPY                     3
+                           122 POP_EXCEPT
+                           124 RERAISE                  1
                ExceptionTable:
-                 6 to 68 -> 72 [0]
-                 72 to 90 -> 126 [1] lasti
-                 92 to 102 -> 116 [1] lasti
-                 104 to 104 -> 126 [1] lasti
-                 116 to 124 -> 126 [1] lasti
+                 6 to 76 -> 80 [0]
+                 80 to 112 -> 120 [1] lasti
+                 118 to 118 -> 120 [1] lasti
                consts
                   None
                names      ('super', '__getitem__', 'KeyError', 'UNKNOWN')
-               varnames   ('cls', 'item', 'error')
+               varnames   ('self', 'item')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__getitem__'
-               firstlineno 6
-               lnotab 0x040102014401120120ff
+               firstlineno 5
+               lnotab 0x040102014c01120112ff
             code
                argcount  : 2
-               nlocals   : 3
+               nlocals   : 2
                stacksize : 4
                flags     : 3
                code
-                  0x950197000900740100000000000000000000a6000000ab000000000000
-                  000000a00100000000000000000000000000000000000000007c01a60100
-                  00ab01000000000000000053002300740400000000000000000000240072
-                  117d027c006a0300000000000000006302590064007d027e02530064007d
-                  027e0277017700780359007701
+                  0x9501970009007c018121740100000000000000000000a6000000ab0000
+                  00000000000000a00100000000000000000000000000000000000000007c
+                  01a6010000ab0100000000000000006e0164005300230074040000000000
+                  00000000002400720a01007c006a03000000000000000063025900530077
+                  00780359007701
                              0 COPY_FREE_VARS           1
                
-                12           2 RESUME                   0
+                11           2 RESUME                   0
                
-                13           4 NOP
+                12           4 NOP
                
-                14           6 LOAD_GLOBAL              1 (NULL + super)
-                            18 PRECALL                  0
-                            22 CALL                     0
-                            32 LOAD_METHOD              1 (__getattribute__)
-                            54 LOAD_FAST                1 (item)
-                            56 PRECALL                  1
-                            60 CALL                     1
-                            70 RETURN_VALUE
-                       >>   72 PUSH_EXC_INFO
-               
-                15          74 LOAD_GLOBAL              4 (KeyError)
-                            86 CHECK_EXC_MATCH
-                            88 POP_JUMP_FORWARD_IF_FALSE    17 (to 124)
-                            90 STORE_FAST               2 (error)
-               
-                16          92 LOAD_FAST                0 (cls)
-                            94 LOAD_ATTR                3 (UNKNOWN)
-                           104 SWAP                     2
-                           106 POP_EXCEPT
-                           108 LOAD_CONST               0 (None)
-                           110 STORE_FAST               2 (error)
-                           112 DELETE_FAST              2 (error)
-                           114 RETURN_VALUE
-                       >>  116 LOAD_CONST               0 (None)
-                           118 STORE_FAST               2 (error)
-                           120 DELETE_FAST              2 (error)
-                           122 RERAISE                  1
-               
-                15     >>  124 RERAISE                  0
-                       >>  126 COPY                     3
-                           128 POP_EXCEPT
-                           130 RERAISE                  1
+                13           6 LOAD_FAST                1 (item)
+                             8 POP_JUMP_FORWARD_IF_NONE    33 (to 76)
+                            10 LOAD_GLOBAL              1 (NULL + super)
+                            22 PRECALL                  0
+                            26 CALL                     0
+                            36 LOAD_METHOD              1 (__getattribute__)
+                            58 LOAD_FAST                1 (item)
+                            60 PRECALL                  1
+                            64 CALL                     1
+                            74 JUMP_FORWARD             1 (to 78)
+                       >>   76 LOAD_CONST               0 (None)
+                       >>   78 RETURN_VALUE
+                       >>   80 PUSH_EXC_INFO
+               
+                14          82 LOAD_GLOBAL              4 (KeyError)
+                            94 CHECK_EXC_MATCH
+                            96 POP_JUMP_FORWARD_IF_FALSE    10 (to 118)
+                            98 POP_TOP
+               
+                15         100 LOAD_FAST                0 (self)
+                           102 LOAD_ATTR                3 (UNKNOWN)
+                           112 SWAP                     2
+                           114 POP_EXCEPT
+                           116 RETURN_VALUE
+               
+                14     >>  118 RERAISE                  0
+                       >>  120 COPY                     3
+                           122 POP_EXCEPT
+                           124 RERAISE                  1
                ExceptionTable:
-                 6 to 68 -> 72 [0]
-                 72 to 90 -> 126 [1] lasti
-                 92 to 102 -> 116 [1] lasti
-                 104 to 104 -> 126 [1] lasti
-                 116 to 124 -> 126 [1] lasti
+                 6 to 76 -> 80 [0]
+                 80 to 112 -> 120 [1] lasti
+                 118 to 118 -> 120 [1] lasti
                consts
                   None
                names      ('super', '__getattribute__', 'KeyError', 'UNKNOWN')
-               varnames   ('cls', 'item', 'error')
+               varnames   ('self', 'item')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__getattribute__'
-               firstlineno 12
-               lnotab 0x040102014401120120ff
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 2
-               flags     : 3
-               code
-                  0x87009700880066016401840889006a0000000000000000004400a60000
-                  00ab0000000000000000005300
-                             0 MAKE_CELL                0 (cls)
-               
-                18           2 RESUME                   0
-               
-                19           4 LOAD_CLOSURE             0 (cls)
-                             6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 19>)
-                            10 MAKE_FUNCTION            8 (closure)
-                            12 LOAD_DEREF               0 (cls)
-                            14 LOAD_ATTR                0 (__members__)
-                            24 GET_ITER
-                            26 PRECALL                  0
-                            30 CALL                     0
-                            40 RETURN_VALUE
-               consts
-                  None
-                  code
-                     argcount  : 1
-                     nlocals   : 2
-                     stacksize : 6
-                     flags     : 19
-                     code
-                        0x9501970067007c005d127d0174010000000000000000000089027c01a6
-                        020000ab02000000000000000091028c135300
-                                   0 COPY_FREE_VARS           1
-                     
-                      19           2 RESUME                   0
-                                   4 BUILD_LIST               0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                18 (to 46)
-                                  10 STORE_FAST               1 (name)
-                                  12 LOAD_GLOBAL              1 (NULL + getattr)
-                                  24 LOAD_DEREF               2 (cls)
-                                  26 LOAD_FAST                1 (name)
-                                  28 PRECALL                  2
-                                  32 CALL                     2
-                                  42 LIST_APPEND              2
-                                  44 JUMP_BACKWARD           19 (to 8)
-                             >>   46 RETURN_VALUE
-                     consts
-                     names      ('getattr',)
-                     varnames   ('.0', 'name')
-                     freevars   ('cls',)
-                     cellvars   ()
-                     filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
-                     name       '<listcomp>'
-                     firstlineno 19
-                     lnotab 0x
-               names      ('__members__',)
-               varnames   ('cls',)
-               freevars   ()
-               cellvars   ('cls',)
-               filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
-               name       'get_all'
-               firstlineno 18
-               lnotab 0x0401
-            'without'
-            'ParcelBase'
-            code
-               argcount  : 2
-               nlocals   : 2
-               stacksize : 4
-               flags     : 3
-               code
-                  0x8701970074010000000000000000000089017402000000000000000000
-                  00a6020000ab0200000000000000007203890167018a0188016601640184
-                  087c00a0020000000000000000000000000000000000000000a6000000ab
-                  0000000000000000004400a6000000ab0000000000000000005300
-                             0 MAKE_CELL                1 (without)
-               
-                21           2 RESUME                   0
-               
-                22           4 LOAD_GLOBAL              1 (NULL + isinstance)
-                            16 LOAD_DEREF               1 (without)
-                            18 LOAD_GLOBAL              2 (ParcelBase)
-                            30 PRECALL                  2
-                            34 CALL                     2
-                            44 POP_JUMP_FORWARD_IF_FALSE     3 (to 52)
-               
-                23          46 LOAD_DEREF               1 (without)
-                            48 BUILD_LIST               1
-                            50 STORE_DEREF              1 (without)
-               
-                25     >>   52 LOAD_CLOSURE             1 (without)
-                            54 BUILD_TUPLE              1
-                            56 LOAD_CONST               1 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 25>)
-                            58 MAKE_FUNCTION            8 (closure)
-                            60 LOAD_FAST                0 (cls)
-                            62 LOAD_METHOD              2 (get_all)
-                            84 PRECALL                  0
-                            88 CALL                     0
-                            98 GET_ITER
-                           100 PRECALL                  0
-                           104 CALL                     0
-                           114 RETURN_VALUE
-               consts
-                  None
-                  code
-                     argcount  : 1
-                     nlocals   : 2
-                     stacksize : 4
-                     flags     : 19
-                     code 0x9501970067007c005d087d017c0189027601af067c0191028c095300
-                                   0 COPY_FREE_VARS           1
-                     
-                      25           2 RESUME                   0
-                                   4 BUILD_LIST               0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                 8 (to 26)
-                                  10 STORE_FAST               1 (element)
-                                  12 LOAD_FAST                1 (element)
-                                  14 LOAD_DEREF               2 (without)
-                                  16 CONTAINS_OP              1
-                                  18 POP_JUMP_BACKWARD_IF_FALSE     6 (to 8)
-                                  20 LOAD_FAST                1 (element)
-                                  22 LIST_APPEND              2
-                                  24 JUMP_BACKWARD            9 (to 8)
-                             >>   26 RETURN_VALUE
-                     consts
-                     names      ()
-                     varnames   ('.0', 'element')
-                     freevars   ('without',)
-                     cellvars   ()
-                     filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
-                     name       '<listcomp>'
-                     firstlineno 25
-                     lnotab 0x
-               names      ('isinstance', 'ParcelBase', 'get_all')
-               varnames   ('cls', 'without')
-               freevars   ()
-               cellvars   ('without',)
-               filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
-               name       'get_without'
-               firstlineno 21
-               lnotab 0x04012a010602
-         names      ('__name__', '__module__', '__qualname__', '__getitem__', '__getattribute__', 'get_all', 'List', 'get_without', '__classcell__')
+               firstlineno 11
+               lnotab 0x040102014c01120112ff
+         names      ('__name__', '__module__', '__qualname__', '__getitem__', '__getattribute__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'Meta'
-         firstlineno 5
-         lnotab 0x0c010a060a060603
+         firstlineno 4
+         lnotab 0x0c010a06
       'Meta'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a03640284005a04640384005a05640484
             005a06640584005a07640684005a08640784005a0964085300
-          28           0 RESUME                   0
+          27           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelBase')
                        8 STORE_NAME               2 (__qualname__)
          
-          29          10 LOAD_CONST               1 ('Base :class:`Enum` class to derive from')
+          28          10 LOAD_CONST               1 ('Base :class:`Enum` class to derive from')
                       12 STORE_NAME               3 (__doc__)
          
-          31          14 LOAD_CONST               2 (<code object __gt__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 31>)
+          30          14 LOAD_CONST               2 (<code object __gt__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 30>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (__gt__)
          
-          37          20 LOAD_CONST               3 (<code object __ge__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 37>)
+          36          20 LOAD_CONST               3 (<code object __ge__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 36>)
                       22 MAKE_FUNCTION            0
                       24 STORE_NAME               5 (__ge__)
          
-          43          26 LOAD_CONST               4 (<code object __le__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 43>)
+          42          26 LOAD_CONST               4 (<code object __le__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 42>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               6 (__le__)
          
-          49          32 LOAD_CONST               5 (<code object __lt__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 49>)
+          48          32 LOAD_CONST               5 (<code object __lt__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 48>)
                       34 MAKE_FUNCTION            0
                       36 STORE_NAME               7 (__lt__)
          
-          55          38 LOAD_CONST               6 (<code object __eq__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 55>)
+          54          38 LOAD_CONST               6 (<code object __eq__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 54>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME               8 (__eq__)
          
-          61          44 LOAD_CONST               7 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 61>)
+          60          44 LOAD_CONST               7 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 60>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               9 (__repr__)
                       50 LOAD_CONST               8 (None)
                       52 RETURN_VALUE
          consts
             'ParcelBase'
             'Base :class:`Enum` class to derive from'
@@ -567,171 +444,171 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab0200000000000000007201090064015300
-                31           0 RESUME                   0
+                30           0 RESUME                   0
                
-                32           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                31           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_GLOBAL              2 (ParcelBase)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE     1 (to 46)
                
-                33          44 NOP
+                32          44 NOP
                
-                35     >>   46 LOAD_CONST               1 (False)
+                34     >>   46 LOAD_CONST               1 (False)
                             48 RETURN_VALUE
                consts
                   None
                   False
                names      ('isinstance', 'ParcelBase')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__gt__'
-               firstlineno 31
+               firstlineno 30
                lnotab 0x02012a010202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab0200000000000000007201090064015300
-                37           0 RESUME                   0
+                36           0 RESUME                   0
                
-                38           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                37           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_GLOBAL              2 (ParcelBase)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE     1 (to 46)
                
-                39          44 NOP
+                38          44 NOP
                
-                41     >>   46 LOAD_CONST               1 (False)
+                40     >>   46 LOAD_CONST               1 (False)
                             48 RETURN_VALUE
                consts
                   None
                   False
                names      ('isinstance', 'ParcelBase')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__ge__'
-               firstlineno 37
+               firstlineno 36
                lnotab 0x02012a010202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab0200000000000000007201090064015300
-                43           0 RESUME                   0
+                42           0 RESUME                   0
                
-                44           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                43           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_GLOBAL              2 (ParcelBase)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE     1 (to 46)
                
-                45          44 NOP
+                44          44 NOP
                
-                47     >>   46 LOAD_CONST               1 (False)
+                46     >>   46 LOAD_CONST               1 (False)
                             48 RETURN_VALUE
                consts
                   None
                   False
                names      ('isinstance', 'ParcelBase')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__le__'
-               firstlineno 43
+               firstlineno 42
                lnotab 0x02012a010202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab0200000000000000007201090064015300
-                49           0 RESUME                   0
+                48           0 RESUME                   0
                
-                50           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                49           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_GLOBAL              2 (ParcelBase)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE     1 (to 46)
                
-                51          44 NOP
+                50          44 NOP
                
-                53     >>   46 LOAD_CONST               1 (False)
+                52     >>   46 LOAD_CONST               1 (False)
                             48 RETURN_VALUE
                consts
                   None
                   False
                names      ('isinstance', 'ParcelBase')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__lt__'
-               firstlineno 49
+               firstlineno 48
                lnotab 0x02012a010202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab02000000000000000072107c006a0200000000000000007c016a
                   0200000000000000006b0200000000530064015300
-                55           0 RESUME                   0
+                54           0 RESUME                   0
                
-                56           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                55           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_GLOBAL              2 (ParcelBase)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE    16 (to 76)
                
-                57          44 LOAD_FAST                0 (self)
+                56          44 LOAD_FAST                0 (self)
                             46 LOAD_ATTR                2 (name)
                             56 LOAD_FAST                1 (other)
                             58 LOAD_ATTR                2 (name)
                             68 COMPARE_OP               2 (==)
                             74 RETURN_VALUE
                
-                59     >>   76 LOAD_CONST               1 (False)
+                58     >>   76 LOAD_CONST               1 (False)
                             78 RETURN_VALUE
                consts
                   None
                   False
                names      ('isinstance', 'ParcelBase', 'name')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__eq__'
-               firstlineno 55
+               firstlineno 54
                lnotab 0x02012a012002
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -740,32 +617,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-                61           0 RESUME                   0
+                60           0 RESUME                   0
                
-                62           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 62>)
+                61           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 61>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-                63          98 LOAD_FAST                0 (self)
+                62          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -787,15 +664,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d0e5c0200007d017d027c019b0064007c029b009d
                         035600970101008c0f64015300
-                      62           0 RETURN_GENERATOR
+                      61           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                14 (to 38)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -816,52 +693,52 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                      name       '<genexpr>'
-                     firstlineno 62
+                     firstlineno 61
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
                name       '__repr__'
-               firstlineno 61
+               firstlineno 60
                lnotab 0x02016001
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__gt__', '__ge__', '__le__', '__lt__', '__eq__', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelBase'
-         firstlineno 28
+         firstlineno 27
          lnotab 0x0a01040206060606060606060606
       'ParcelBase'
       ('metaclass',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065a0864075a0964085300
-          66           0 RESUME                   0
+          65           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelCarrierSize')
                        8 STORE_NAME               2 (__qualname__)
          
-          67          10 LOAD_CONST               1 (':class:`Enum` that holds parcel size for carrier shipment type')
+          66          10 LOAD_CONST               1 (':class:`Enum` that holds parcel size for carrier shipment type')
                       12 STORE_NAME               3 (__doc__)
          
           68          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
           69          18 LOAD_CONST               3 ('8x38x64')
                       20 STORE_NAME               5 (A)
@@ -891,16 +768,16 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'A', 'B', 'C', 'D', 'OTHER')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelCarrierSize'
-         firstlineno 66
-         lnotab 0x0a01040104010401040104010401
+         firstlineno 65
+         lnotab 0x0a01040204010401040104010401
       'ParcelCarrierSize'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
@@ -911,24 +788,24 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelLockerSize')
                        8 STORE_NAME               2 (__qualname__)
          
           77          10 LOAD_CONST               1 (':class:`Enum` that holds parcel size for parcel locker shipment type')
                       12 STORE_NAME               3 (__doc__)
          
-          78          14 LOAD_CONST               2 ('UNKNOWN DATA')
+          79          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-          79          18 LOAD_CONST               3 ('8x38x64')
+          80          18 LOAD_CONST               3 ('8x38x64')
                       20 STORE_NAME               5 (A)
          
-          80          22 LOAD_CONST               4 ('19x38x64')
+          81          22 LOAD_CONST               4 ('19x38x64')
                       24 STORE_NAME               6 (B)
          
-          81          26 LOAD_CONST               5 ('41x38x64')
+          82          26 LOAD_CONST               5 ('41x38x64')
                       28 STORE_NAME               7 (C)
                       30 LOAD_CONST               6 (None)
                       32 RETURN_VALUE
          consts
             'ParcelLockerSize'
             ':class:`Enum` that holds parcel size for parcel locker shipment type'
             'UNKNOWN DATA'
@@ -939,43 +816,43 @@
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'A', 'B', 'C')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelLockerSize'
          firstlineno 76
-         lnotab 0x0a010401040104010401
+         lnotab 0x0a010402040104010401
       'ParcelLockerSize'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065300
-          84           0 RESUME                   0
+          85           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelDeliveryType')
                        8 STORE_NAME               2 (__qualname__)
          
-          85          10 LOAD_CONST               1 (':class:`Enum` that holds parcel delivery types')
+          86          10 LOAD_CONST               1 (':class:`Enum` that holds parcel delivery types')
                       12 STORE_NAME               3 (__doc__)
          
-          86          14 LOAD_CONST               2 ('UNKNOWN DATA')
+          88          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-          87          18 LOAD_CONST               3 ('Paczkomat')
+          89          18 LOAD_CONST               3 ('Paczkomat')
                       20 STORE_NAME               5 (parcel_locker)
          
-          88          22 LOAD_CONST               4 ('Kurier')
+          90          22 LOAD_CONST               4 ('Kurier')
                       24 STORE_NAME               6 (courier)
          
-          89          26 LOAD_CONST               5 ('PaczkoPunkt')
+          91          26 LOAD_CONST               5 ('PaczkoPunkt')
                       28 STORE_NAME               7 (parcel_point)
                       30 LOAD_CONST               6 (None)
                       32 RETURN_VALUE
          consts
             'ParcelDeliveryType'
             ':class:`Enum` that holds parcel delivery types'
             'UNKNOWN DATA'
@@ -985,44 +862,44 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'parcel_locker', 'courier', 'parcel_point')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelDeliveryType'
-         firstlineno 84
-         lnotab 0x0a010401040104010401
+         firstlineno 85
+         lnotab 0x0a010402040104010401
       'ParcelDeliveryType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065300
-          92           0 RESUME                   0
+          94           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelShipmentType')
                        8 STORE_NAME               2 (__qualname__)
          
-          93          10 LOAD_CONST               1 (':class:`Enum` that holds parcel shipment types')
+          95          10 LOAD_CONST               1 (':class:`Enum` that holds parcel shipment types')
                       12 STORE_NAME               3 (__doc__)
          
-          94          14 LOAD_CONST               2 ('UNKNOWN DATA')
+          97          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-          95          18 LOAD_CONST               3 ('Paczkomat')
+          98          18 LOAD_CONST               3 ('Paczkomat')
                       20 STORE_NAME               5 (parcel)
          
-          96          22 LOAD_CONST               4 ('Kurier')
+          99          22 LOAD_CONST               4 ('Kurier')
                       24 STORE_NAME               6 (courier)
          
-          97          26 LOAD_CONST               5 ('PaczkoPunkt')
+         100          26 LOAD_CONST               5 ('PaczkoPunkt')
                       28 STORE_NAME               7 (parcel_point)
                       30 LOAD_CONST               6 (None)
                       32 RETURN_VALUE
          consts
             'ParcelShipmentType'
             ':class:`Enum` that holds parcel shipment types'
             'UNKNOWN DATA'
@@ -1032,44 +909,44 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'parcel', 'courier', 'parcel_point')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelShipmentType'
-         firstlineno 92
-         lnotab 0x0a010401040104010401
+         firstlineno 94
+         lnotab 0x0a010402040104010401
       'ParcelShipmentType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065300
-         100           0 RESUME                   0
+         103           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelAdditionalInsurance')
                        8 STORE_NAME               2 (__qualname__)
          
-         101          10 LOAD_CONST               1 ('UNKNOWN DATA')
+         104          10 LOAD_CONST               1 ('UNKNOWN DATA')
                       12 STORE_NAME               3 (UNKNOWN)
          
-         102          14 LOAD_CONST               2 (1)
+         105          14 LOAD_CONST               2 (1)
                       16 STORE_NAME               4 (UNINSURANCED)
          
-         103          18 LOAD_CONST               3 (2)
+         106          18 LOAD_CONST               3 (2)
                       20 STORE_NAME               5 (ONE)
          
-         104          22 LOAD_CONST               4 (3)
+         107          22 LOAD_CONST               4 (3)
                       24 STORE_NAME               6 (TWO)
          
-         105          26 LOAD_CONST               5 (4)
+         108          26 LOAD_CONST               5 (4)
                       28 STORE_NAME               7 (THREE)
                       30 LOAD_CONST               6 (None)
                       32 RETURN_VALUE
          consts
             'ParcelAdditionalInsurance'
             'UNKNOWN DATA'
             1
@@ -1079,44 +956,44 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'UNKNOWN', 'UNINSURANCED', 'ONE', 'TWO', 'THREE')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelAdditionalInsurance'
-         firstlineno 100
+         firstlineno 103
          lnotab 0x0a010401040104010401
       'ParcelAdditionalInsurance'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065300
-         108           0 RESUME                   0
+         111           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelType')
                        8 STORE_NAME               2 (__qualname__)
          
-         109          10 LOAD_CONST               1 (':class:`Enum` that holds parcel types')
+         112          10 LOAD_CONST               1 (':class:`Enum` that holds parcel types')
                       12 STORE_NAME               3 (__doc__)
          
-         110          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         114          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         111          18 LOAD_CONST               3 ('Przychodzące')
+         115          18 LOAD_CONST               3 ('Przychodzące')
                       20 STORE_NAME               5 (TRACKED)
          
-         112          22 LOAD_CONST               4 ('Wysłane')
+         116          22 LOAD_CONST               4 ('Wysłane')
                       24 STORE_NAME               6 (SENT)
          
-         113          26 LOAD_CONST               5 ('Zwroty')
+         117          26 LOAD_CONST               5 ('Zwroty')
                       28 STORE_NAME               7 (RETURNS)
                       30 LOAD_CONST               6 (None)
                       32 RETURN_VALUE
          consts
             'ParcelType'
             ':class:`Enum` that holds parcel types'
             'UNKNOWN DATA'
@@ -1126,174 +1003,269 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'TRACKED', 'SENT', 'RETURNS')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelType'
-         firstlineno 108
-         lnotab 0x0a010401040104010401
+         firstlineno 111
+         lnotab 0x0a010402040104010401
       'ParcelType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
+            0764065a0864075300
+         120           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('PointType')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         121          10 LOAD_CONST               1 (':class: `Enum` that holds point types')
+                      12 STORE_NAME               3 (__doc__)
+         
+         123          14 LOAD_CONST               2 ('UNNKOWN DATA')
+                      16 STORE_NAME               4 (UNKNOWN)
+         
+         124          18 LOAD_CONST               3 ('Paczkomat')
+                      20 STORE_NAME               5 (PL)
+         
+         125          22 LOAD_CONST               4 ('some paczkomat or pok stuff')
+                      24 STORE_NAME               6 (parcel_locker_superpop)
+         
+         126          26 LOAD_CONST               5 ('Mobilny punkt obsługi klienta')
+                      28 STORE_NAME               7 (POK)
+         
+         127          30 LOAD_CONST               6 ('Punkt odbioru paczki')
+                      32 STORE_NAME               8 (POP)
+                      34 LOAD_CONST               7 (None)
+                      36 RETURN_VALUE
+         consts
+            'PointType'
+            ':class: `Enum` that holds point types'
+            'UNNKOWN DATA'
+            'Paczkomat'
+            'some paczkomat or pok stuff'
+            'Mobilny punkt obsługi klienta'
+            'Punkt odbioru paczki'
+            None
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'PL', 'parcel_locker_superpop', 'POK', 'POP')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
+         name       'PointType'
+         firstlineno 120
+         lnotab 0x0a0104020401040104010401
+      'PointType'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
+         code
+            0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
+            00
+         130           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('ParcelPointOperations')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         131          10 LOAD_CONST               1 (':class: `Enum` that holds parcel operation types')
+                      12 STORE_NAME               3 (__doc__)
+         
+         133          14 LOAD_CONST               2 ('UNNKOWN DATA')
+                      16 STORE_NAME               4 (UNKNOWN)
+         
+         134          18 LOAD_CONST               3 ('c2x-target')
+                      20 STORE_NAME               5 (CREATE)
+         
+         135          22 LOAD_CONST               4 ('remote-send')
+                      24 STORE_NAME               6 (SEND)
+                      26 LOAD_CONST               5 (None)
+                      28 RETURN_VALUE
+         consts
+            'ParcelPointOperations'
+            ':class: `Enum` that holds parcel operation types'
+            'UNNKOWN DATA'
+            'c2x-target'
+            'remote-send'
+            None
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'CREATE', 'SEND')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
+         name       'ParcelPointOperations'
+         firstlineno 130
+         lnotab 0x0a01040204010401
+      'ParcelPointOperations'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
+         code
+            0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
             0d5a0f640e5a10640f5a1164105a1264115a1364125a1464135a1564145a
             1664155a1764165a1864175a1964185a1a64195a1b641a5a1c641b5a1d64
             1c5a1e641d5a1f641e5a2064135a21641f5a2264205a2364215a2464225a
             2564235a2664245a2764255a2864265a2964125a2a64275a2b64285a2c64
             295a2d642a5a2e642b5300
-         116           0 RESUME                   0
+         138           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         117          10 LOAD_CONST               1 (':class:`Enum` that holds parcel statuses')
+         139          10 LOAD_CONST               1 (':class:`Enum` that holds parcel statuses')
                       12 STORE_NAME               3 (__doc__)
          
-         118          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         141          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         119          18 LOAD_CONST               3 ('Utworzona')
+         142          18 LOAD_CONST               3 ('W trakcie przygotowania')
                       20 STORE_NAME               5 (CREATED)
          
-         120          22 LOAD_CONST               4 ('Oferty przygotowane')
+         143          22 LOAD_CONST               4 ('Oferty przygotowane')
                       24 STORE_NAME               6 (OFFERS_PREPARED)
          
-         121          26 LOAD_CONST               5 ('Oferta wybrana')
+         144          26 LOAD_CONST               5 ('Oferta wybrana')
                       28 STORE_NAME               7 (OFFER_SELECTED)
          
-         122          30 LOAD_CONST               6 ('Potwierdzona')
+         145          30 LOAD_CONST               6 ('Potwierdzona')
                       32 STORE_NAME               8 (CONFIRMED)
          
-         123          34 LOAD_CONST               7 ('Gotowa do odbioru w PaczkoPunkcie')
+         146          34 LOAD_CONST               7 ('Gotowa do odbioru w PaczkoPunkcie')
                       36 STORE_NAME               9 (READY_TO_PICKUP_FROM_POK)
          
-         124          38 LOAD_CONST               8 ('Gabaryt')
+         147          38 LOAD_CONST               8 ('Gabaryt')
                       40 STORE_NAME              10 (OVERSIZED)
          
-         125          42 LOAD_CONST               9 ('Nadana w PaczkoPunkcie')
+         148          42 LOAD_CONST               9 ('Nadana w PaczkoPunkcie')
                       44 STORE_NAME              11 (DISPATCHED_BY_SENDER_TO_POK)
          
-         126          46 LOAD_CONST              10 ('Nadana w paczkomacie')
+         149          46 LOAD_CONST              10 ('Nadana w paczkomacie')
                       48 STORE_NAME              12 (DISPATCHED_BY_SENDER)
          
-         127          50 LOAD_CONST              11 ('Odebrana od nadawcy')
+         150          50 LOAD_CONST              11 ('Odebrana od nadawcy')
                       52 STORE_NAME              13 (COLLECTED_FROM_SENDER)
          
-         128          54 LOAD_CONST              12 ('Odebrana przez Kuriera')
+         151          54 LOAD_CONST              12 ('Odebrana przez Kuriera')
                       56 STORE_NAME              14 (TAKEN_BY_COURIER)
          
-         129          58 LOAD_CONST              13 ('Przyjęta w oddziale')
+         152          58 LOAD_CONST              13 ('Przyjęta w oddziale')
                       60 STORE_NAME              15 (ADOPTED_AT_SOURCE_BRANCH)
          
-         130          62 LOAD_CONST              14 ('Wysłana z oddziału')
+         153          62 LOAD_CONST              14 ('Wysłana z oddziału')
                       64 STORE_NAME              16 (SENT_FROM_SOURCE_BRANCH)
          
-         131          66 LOAD_CONST              15 ('Zmiana punktu dostawy')
+         154          66 LOAD_CONST              15 ('Zmiana punktu dostawy')
                       68 STORE_NAME              17 (READDRESSED)
          
-         132          70 LOAD_CONST              16 ('Wydana do doręczenia')
+         155          70 LOAD_CONST              16 ('Wydana do doręczenia')
                       72 STORE_NAME              18 (OUT_FOR_DELIVERY)
          
-         133          74 LOAD_CONST              17 ('Gotowa do odbioru')
+         156          74 LOAD_CONST              17 ('Gotowa do odbioru')
                       76 STORE_NAME              19 (READY_TO_PICKUP)
          
-         134          78 LOAD_CONST              18 ('Wysłano przypomnienie o odbiorze')
+         157          78 LOAD_CONST              18 ('Wysłano przypomnienie o odbiorze')
                       80 STORE_NAME              20 (PICKUP_REMINDER_SENT)
          
-         135          82 LOAD_CONST              19 ('Upłynął czas odbioru')
+         158          82 LOAD_CONST              19 ('Upłynął czas odbioru')
                       84 STORE_NAME              21 (PICKUP_TIME_EXPIRED)
          
-         136          86 LOAD_CONST              20 ('Powrót do oddziału')
+         159          86 LOAD_CONST              20 ('Powrót do oddziału')
                       88 STORE_NAME              22 (AVIZO)
          
-         137          90 LOAD_CONST              21 ('Odebrana z PaczkoPunktu nadawczego')
+         160          90 LOAD_CONST              21 ('Odebrana z PaczkoPunktu nadawczego')
                       92 STORE_NAME              23 (TAKEN_BY_COURIER_FROM_POK)
          
-         138          94 LOAD_CONST              22 ('Odrzucona przez odbiorcę')
+         161          94 LOAD_CONST              22 ('Odrzucona przez odbiorcę')
                       96 STORE_NAME              24 (REJECTED_BY_RECEIVER)
          
-         139          98 LOAD_CONST              23 ('Nie dostarczona')
+         162          98 LOAD_CONST              23 ('Nie dostarczona')
                      100 STORE_NAME              25 (UNDELIVERED)
          
-         140         102 LOAD_CONST              24 ('Opóźnienie w dostarczeniu')
+         163         102 LOAD_CONST              24 ('Opóźnienie w dostarczeniu')
                      104 STORE_NAME              26 (DELAY_IN_DELIVERY)
          
-         141         106 LOAD_CONST              25 ('Zwrócona do nadawcy')
+         164         106 LOAD_CONST              25 ('Zwrócona do nadawcy')
                      108 STORE_NAME              27 (RETURNED_TO_SENDER)
          
-         142         110 LOAD_CONST              26 ('Gotowa do odbioru z oddziału')
+         165         110 LOAD_CONST              26 ('Gotowa do odbioru z oddziału')
                      112 STORE_NAME              28 (READY_TO_PICKUP_FROM_BRANCH)
          
-         143         114 LOAD_CONST              27 ('Doręczona')
+         166         114 LOAD_CONST              27 ('Doręczona')
                      116 STORE_NAME              29 (DELIVERED)
          
-         144         118 LOAD_CONST              28 ('Anulowana')
+         167         118 LOAD_CONST              28 ('Anulowana')
                      120 STORE_NAME              30 (CANCELED)
          
-         145         122 LOAD_CONST              29 ('Zareklamowana')
+         168         122 LOAD_CONST              29 ('Zareklamowana')
                      124 STORE_NAME              31 (CLAIMED)
          
-         146         126 LOAD_CONST              30 ('Przesyłka magazynowana w punkcie obsługi klienta')
+         169         126 LOAD_CONST              30 ('Przesyłka magazynowana w punkcie obsługi klienta')
                      128 STORE_NAME              32 (STACK_IN_CUSTOMER_SERVICE_POINT)
          
-         147         130 LOAD_CONST              19 ('Upłynął czas odbioru')
+         170         130 LOAD_CONST              19 ('Upłynął czas odbioru')
                      132 STORE_NAME              33 (STACK_PARCEL_PICKUP_TIME_EXPIRED)
          
-         148         134 LOAD_CONST              31 ('?')
+         171         134 LOAD_CONST              31 ('?')
                      136 STORE_NAME              34 (UNSTACK_FROM_CUSTOMER_SERVICE_POINT)
          
-         149         138 LOAD_CONST              32 ('Przekazana do punktu obsługi klienta')
+         172         138 LOAD_CONST              32 ('Przekazana do punktu obsługi klienta')
                      140 STORE_NAME              35 (COURIER_AVIZO_IN_CUSTOMER_SERVICE_POINT)
          
-         150         142 LOAD_CONST              33 ('Odebrana przez kuriera z punktu obsługi klienta')
-                     144 STORE_NAME              36 (TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT)
+         174         142 LOAD_CONST              33 ('Odebrana przez kuriera z punktu obsługi klienta')
+         
+         173         144 STORE_NAME              36 (TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT)
          
-         151         146 LOAD_CONST              34 ('Przesyłka magazynowana w paczkomacie tymczasowym')
+         176         146 LOAD_CONST              34 ('Przesyłka magazynowana w paczkomacie tymczasowym')
                      148 STORE_NAME              37 (STACK_IN_BOX_MACHINE)
          
-         152         150 LOAD_CONST              35 ('Upłynął czas odbioru z paczkomatu')
+         177         150 LOAD_CONST              35 ('Upłynął czas odbioru z paczkomatu')
                      152 STORE_NAME              38 (STACK_PARCEL_IN_BOX_MACHINE_PICKUP_TIME_EXPIRED)
          
-         153         154 LOAD_CONST              36 ('Odebrana z paczkomatu')
+         178         154 LOAD_CONST              36 ('Odebrana z paczkomatu')
                      156 STORE_NAME              39 (UNSTACK_FROM_BOX_MACHINE)
          
-         154         158 LOAD_CONST              37 ('Przyjęta w sortowni')
+         179         158 LOAD_CONST              37 ('Przyjęta w sortowni')
                      160 STORE_NAME              40 (ADOPTED_AT_SORTING_CENTER)
          
-         155         162 LOAD_CONST              38 ('Gotowa do doręczenia')
+         180         162 LOAD_CONST              38 ('Gotowa do doręczenia')
                      164 STORE_NAME              41 (OUT_FOR_DELIVERY_TO_ADDRESS)
          
-         156         166 LOAD_CONST              18 ('Wysłano przypomnienie o odbiorze')
+         181         166 LOAD_CONST              18 ('Wysłano przypomnienie o odbiorze')
                      168 STORE_NAME              42 (PICKUP_REMINDER_SENT_ADDRESS)
          
-         157         170 LOAD_CONST              39 ('Nie dostarczono z powodu złego adresu')
+         182         170 LOAD_CONST              39 ('Nie dostarczono z powodu złego adresu')
                      172 STORE_NAME              43 (UNDELIVERED_WRONG_ADDRESS)
          
-         158         174 LOAD_CONST              40 ('Nie dostarczono z powodu nieopłacenia')
+         183         174 LOAD_CONST              40 ('Nie dostarczono z powodu nieopłacenia')
                      176 STORE_NAME              44 (UNDELIVERED_COD_CASH_RECEIVER)
          
-         159         178 LOAD_CONST              41 ('Przekierowana do paczkomatu')
+         184         178 LOAD_CONST              41 ('Przekierowana do paczkomatu')
                      180 STORE_NAME              45 (REDIRECT_TO_BOX)
          
-         160         182 LOAD_CONST              42 ('Anulowano przekierowanie do paczkomatu')
+         185         182 LOAD_CONST              42 ('Anulowano przekierowanie do paczkomatu')
                      184 STORE_NAME              46 (CANCELED_REDIRECT_TO_BOX)
                      186 LOAD_CONST              43 (None)
                      188 RETURN_VALUE
          consts
             'ParcelStatus'
             ':class:`Enum` that holds parcel statuses'
             'UNKNOWN DATA'
-            'Utworzona'
+            'W trakcie przygotowania'
             'Oferty przygotowane'
             'Oferta wybrana'
             'Potwierdzona'
             'Gotowa do odbioru w PaczkoPunkcie'
             'Gabaryt'
             'Nadana w PaczkoPunkcie'
             'Nadana w paczkomacie'
@@ -1332,44 +1304,78 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'CREATED', 'OFFERS_PREPARED', 'OFFER_SELECTED', 'CONFIRMED', 'READY_TO_PICKUP_FROM_POK', 'OVERSIZED', 'DISPATCHED_BY_SENDER_TO_POK', 'DISPATCHED_BY_SENDER', 'COLLECTED_FROM_SENDER', 'TAKEN_BY_COURIER', 'ADOPTED_AT_SOURCE_BRANCH', 'SENT_FROM_SOURCE_BRANCH', 'READDRESSED', 'OUT_FOR_DELIVERY', 'READY_TO_PICKUP', 'PICKUP_REMINDER_SENT', 'PICKUP_TIME_EXPIRED', 'AVIZO', 'TAKEN_BY_COURIER_FROM_POK', 'REJECTED_BY_RECEIVER', 'UNDELIVERED', 'DELAY_IN_DELIVERY', 'RETURNED_TO_SENDER', 'READY_TO_PICKUP_FROM_BRANCH', 'DELIVERED', 'CANCELED', 'CLAIMED', 'STACK_IN_CUSTOMER_SERVICE_POINT', 'STACK_PARCEL_PICKUP_TIME_EXPIRED', 'UNSTACK_FROM_CUSTOMER_SERVICE_POINT', 'COURIER_AVIZO_IN_CUSTOMER_SERVICE_POINT', 'TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT', 'STACK_IN_BOX_MACHINE', 'STACK_PARCEL_IN_BOX_MACHINE_PICKUP_TIME_EXPIRED', 'UNSTACK_FROM_BOX_MACHINE', 'ADOPTED_AT_SORTING_CENTER', 'OUT_FOR_DELIVERY_TO_ADDRESS', 'PICKUP_REMINDER_SENT_ADDRESS', 'UNDELIVERED_WRONG_ADDRESS', 'UNDELIVERED_COD_CASH_RECEIVER', 'REDIRECT_TO_BOX', 'CANCELED_REDIRECT_TO_BOX')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelStatus'
-         firstlineno 116
+         firstlineno 138
          lnotab
-            0x0a01040104010401040104010401040104010401040104010401040104
+            0x0a01040204010401040104010401040104010401040104010401040104
             010401040104010401040104010401040104010401040104010401040104
-            0104010401040104010401040104010401040104010401040104010401
+            01040104010401040202ff02030401040104010401040104010401040104
+            01
       'ParcelStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
+         code 0x970065005a0164005a0264015a0364025a0464035300
+         188           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('DeliveryType')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         189          10 LOAD_CONST               1 ('UNKNOWN DATA')
+                      12 STORE_NAME               3 (UNKNOWN)
+         
+         190          14 LOAD_CONST               2 ('Paczkomat')
+                      16 STORE_NAME               4 (BOX_MACHINE)
+                      18 LOAD_CONST               3 (None)
+                      20 RETURN_VALUE
+         consts
+            'DeliveryType'
+            'UNKNOWN DATA'
+            'Paczkomat'
+            None
+         names      ('__name__', '__module__', '__qualname__', 'UNKNOWN', 'BOX_MACHINE')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
+         name       'DeliveryType'
+         firstlineno 188
+         lnotab 0x0a010401
+      'DeliveryType'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         163           0 RESUME                   0
+         193           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ReturnsStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         164          10 LOAD_CONST               1 ('Zaakceptowano')
+         194          10 LOAD_CONST               1 ('Zaakceptowano')
                       12 STORE_NAME               3 (ACCEPTED)
          
-         165          14 LOAD_CONST               2 ('Nadano')
+         195          14 LOAD_CONST               2 ('Nadano')
                       16 STORE_NAME               4 (USED)
          
-         166          18 LOAD_CONST               3 ('Dostarczono')
+         196          18 LOAD_CONST               3 ('Dostarczono')
                       20 STORE_NAME               5 (DELIVERED)
          
-         167          22 LOAD_CONST               4 ('UNKNOWN DATA')
+         197          22 LOAD_CONST               4 ('UNKNOWN DATA')
                       24 STORE_NAME               6 (UNKNOWN)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'ReturnsStatus'
             'Zaakceptowano'
             'Nadano'
@@ -1378,41 +1384,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'ACCEPTED', 'USED', 'DELIVERED', 'UNKNOWN')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ReturnsStatus'
-         firstlineno 163
+         firstlineno 193
          lnotab 0x0a01040104010401
       'ReturnsStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         170           0 RESUME                   0
+         200           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelOwnership')
                        8 STORE_NAME               2 (__qualname__)
          
-         171          10 LOAD_CONST               1 (':class:`Enum` that holds parcel ownership types')
+         201          10 LOAD_CONST               1 (':class:`Enum` that holds parcel ownership types')
                       12 STORE_NAME               3 (__doc__)
          
-         172          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         203          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         173          18 LOAD_CONST               3 ('Zaprzyjaźniona')
+         204          18 LOAD_CONST               3 ('Zaprzyjaźniona')
                       20 STORE_NAME               5 (FRIEND)
          
-         174          22 LOAD_CONST               4 ('Własna')
+         205          22 LOAD_CONST               4 ('Własna')
                       24 STORE_NAME               6 (OWN)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'ParcelOwnership'
             ':class:`Enum` that holds parcel ownership types'
             'UNKNOWN DATA'
@@ -1421,41 +1427,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'FRIEND', 'OWN')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelOwnership'
-         firstlineno 170
-         lnotab 0x0a01040104010401
+         firstlineno 200
+         lnotab 0x0a01040204010401
       'ParcelOwnership'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         178           0 RESUME                   0
+         209           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CompartmentExpectedStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         179          10 LOAD_CONST               1 (':class:`Enum` that holds compartment expected statuses')
+         210          10 LOAD_CONST               1 (':class:`Enum` that holds compartment expected statuses')
                       12 STORE_NAME               3 (__doc__)
          
-         180          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         212          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         181          18 LOAD_CONST               3 ('Otwarta')
+         213          18 LOAD_CONST               3 ('Otwarta')
                       20 STORE_NAME               5 (OPENED)
          
-         182          22 LOAD_CONST               4 ('Zamknięta')
+         214          22 LOAD_CONST               4 ('Zamknięta')
                       24 STORE_NAME               6 (CLOSED)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'CompartmentExpectedStatus'
             ':class:`Enum` that holds compartment expected statuses'
             'UNKNOWN DATA'
@@ -1464,41 +1470,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'OPENED', 'CLOSED')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'CompartmentExpectedStatus'
-         firstlineno 178
-         lnotab 0x0a01040104010401
+         firstlineno 209
+         lnotab 0x0a01040204010401
       'CompartmentExpectedStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         185           0 RESUME                   0
+         217           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CompartmentActualStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         186          10 LOAD_CONST               1 (':class:`Enum` that holds compartment actual statuses')
+         218          10 LOAD_CONST               1 (':class:`Enum` that holds compartment actual statuses')
                       12 STORE_NAME               3 (__doc__)
          
-         187          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         220          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         188          18 LOAD_CONST               3 ('Otwarta')
+         221          18 LOAD_CONST               3 ('Otwarta')
                       20 STORE_NAME               5 (OPENED)
          
-         189          22 LOAD_CONST               4 ('Zamknięta')
+         222          22 LOAD_CONST               4 ('Zamknięta')
                       24 STORE_NAME               6 (CLOSED)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'CompartmentActualStatus'
             ':class:`Enum` that holds compartment actual statuses'
             'UNKNOWN DATA'
@@ -1507,66 +1513,136 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'OPENED', 'CLOSED')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'CompartmentActualStatus'
-         firstlineno 185
-         lnotab 0x0a01040104010401
+         firstlineno 217
+         lnotab 0x0a01040204010401
       'CompartmentActualStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
+         code 0x970065005a0164005a0264015a0364025a0464035a0564045300
+         225           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('PaymentType')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         226          10 LOAD_CONST               1 ('UNKNOWN DATA')
+                      12 STORE_NAME               3 (UNKNOWN)
+         
+         227          14 LOAD_CONST               2 ('Payments are not supported')
+                      16 STORE_NAME               4 (NOTSUPPORTED)
+         
+         228          18 LOAD_CONST               3 ('Payment by card in the machine')
+                      20 STORE_NAME               5 (BY_CARD_IN_MACHINE)
+                      22 LOAD_CONST               4 (None)
+                      24 RETURN_VALUE
+         consts
+            'PaymentType'
+            'UNKNOWN DATA'
+            'Payments are not supported'
+            'Payment by card in the machine'
+            None
+         names      ('__name__', '__module__', '__qualname__', 'UNKNOWN', 'NOTSUPPORTED', 'BY_CARD_IN_MACHINE')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
+         name       'PaymentType'
+         firstlineno 225
+         lnotab 0x0a0104010401
+      'PaymentType'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
+         code 0x970065005a0164005a0264015a0364025a0464035300
+         231           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('PaymentStatus')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         232          10 LOAD_CONST               1 ('UNKNOWN DATA')
+                      12 STORE_NAME               3 (UNKNOWN)
+         
+         233          14 LOAD_CONST               2 ('Completed')
+                      16 STORE_NAME               4 (C2X_COMPLETED)
+                      18 LOAD_CONST               3 (None)
+                      20 RETURN_VALUE
+         consts
+            'PaymentStatus'
+            'UNKNOWN DATA'
+            'Completed'
+            None
+         names      ('__name__', '__module__', '__qualname__', 'UNKNOWN', 'C2X_COMPLETED')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
+         name       'PaymentStatus'
+         firstlineno 231
+         lnotab 0x0a010401
+      'PaymentStatus'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
             0d5300
-         192           0 RESUME                   0
+         236           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelServiceName')
                        8 STORE_NAME               2 (__qualname__)
          
-         193          10 LOAD_CONST               1 ('UNKNOWN DATA')
+         237          10 LOAD_CONST               1 ('UNKNOWN DATA')
                       12 STORE_NAME               3 (UNKNOWN)
          
-         194          14 LOAD_CONST               2 (1)
+         238          14 LOAD_CONST               2 (1)
                       16 STORE_NAME               4 (ALLEGRO_PARCEL)
          
-         195          18 LOAD_CONST               3 (2)
+         239          18 LOAD_CONST               3 (2)
                       20 STORE_NAME               5 (ALLEGRO_PARCEL_SMART)
          
-         196          22 LOAD_CONST               4 (3)
+         240          22 LOAD_CONST               4 (3)
                       24 STORE_NAME               6 (ALLEGRO_LETTER)
          
-         197          26 LOAD_CONST               5 (4)
+         241          26 LOAD_CONST               5 (4)
                       28 STORE_NAME               7 (ALLEGRO_COURIER)
          
-         198          30 LOAD_CONST               6 (5)
+         242          30 LOAD_CONST               6 (5)
                       32 STORE_NAME               8 (STANDARD)
          
-         199          34 LOAD_CONST               7 (6)
+         243          34 LOAD_CONST               7 (6)
                       36 STORE_NAME               9 (STANDARD_PARCEL_SMART)
          
-         200          38 LOAD_CONST               8 (7)
+         244          38 LOAD_CONST               8 (7)
                       40 STORE_NAME              10 (PASS_THRU)
          
-         201          42 LOAD_CONST               9 (8)
+         245          42 LOAD_CONST               9 (8)
                       44 STORE_NAME              11 (CUSTOMER_SERVICE_POINT)
          
-         202          46 LOAD_CONST              10 (9)
+         246          46 LOAD_CONST              10 (9)
                       48 STORE_NAME              12 (REVERSE)
          
-         203          50 LOAD_CONST              11 (10)
+         247          50 LOAD_CONST              11 (10)
                       52 STORE_NAME              13 (STANDARD_COURIER)
          
-         204          54 LOAD_CONST              12 (11)
+         248          54 LOAD_CONST              12 (11)
                       56 STORE_NAME              14 (REVERSE_RETURN)
                       58 LOAD_CONST              13 (None)
                       60 RETURN_VALUE
          consts
             'ParcelServiceName'
             'UNKNOWN DATA'
             1
@@ -1583,21 +1659,21 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'UNKNOWN', 'ALLEGRO_PARCEL', 'ALLEGRO_PARCEL_SMART', 'ALLEGRO_LETTER', 'ALLEGRO_COURIER', 'STANDARD', 'STANDARD_PARCEL_SMART', 'PASS_THRU', 'CUSTOMER_SERVICE_POINT', 'REVERSE', 'STANDARD_COURIER', 'REVERSE_RETURN')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelServiceName'
-         firstlineno 192
+         firstlineno 236
          lnotab 0x0a0104010401040104010401040104010401040104010401
       'ParcelServiceName'
       None
-   names      ('enum', 'Enum', 'EnumMeta', 'typing', 'List', 'Meta', 'ParcelBase', 'ParcelCarrierSize', 'ParcelLockerSize', 'ParcelDeliveryType', 'ParcelShipmentType', 'ParcelAdditionalInsurance', 'ParcelType', 'ParcelStatus', 'ReturnsStatus', 'ParcelOwnership', 'CompartmentExpectedStatus', 'CompartmentActualStatus', 'ParcelServiceName')
+   names      ('enum', 'Enum', 'EnumMeta', 'Meta', 'ParcelBase', 'ParcelCarrierSize', 'ParcelLockerSize', 'ParcelDeliveryType', 'ParcelShipmentType', 'ParcelAdditionalInsurance', 'ParcelType', 'PointType', 'ParcelPointOperations', 'ParcelStatus', 'DeliveryType', 'ReturnsStatus', 'ParcelOwnership', 'CompartmentExpectedStatus', 'CompartmentActualStatus', 'PaymentType', 'PaymentStatus', 'ParcelServiceName')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c031c1720261c0a1c081c081c081c081c081c2f1c071c
-      081c071c07
+      0x00ff020110031c1720261c0b1c091c091c091c081c091c0a1c081c321c
+      051c071c091c081c081c061c05
```

### Comparing `inpost-0.1.3/inpost/static/exceptions.py` & `inpost-0.1.4/inpost/static/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,118 @@
 from typing import Any
-from .statuses import ParcelType
-from .parcels import Parcel
 
 
 # ------------------ Base ------------------- #
 class BaseInpostError(Exception):
     """Base exception to inherit from
 
     :param reason: reason of BaseInpostError happening
     :type reason: typing.Any"""
 
     def __init__(self, reason):
-        """Constructor method"""
+        """Constructor method
+
+        :param reason: Reason of error
+        :type reason: Any
+        """
         super().__init__(reason)
         self.reason: Any = reason
 
     @property
-    def stacktrace(self):
-        """Gets stacktrace of raised exception"""
+    def stacktrace(self) -> Any:
+        """Gets stacktrace of raised exception
+        :return: reason why exception occured
+        :rtype: Any"""
         return self.reason
 
 
 # ----------------- Parcels ----------------- #
 
+
 class ParcelTypeError(BaseInpostError):
     """Is raised when expected :class:`ParcelType` does not match with actual one"""
+
     pass
 
 
 class NoParcelError(BaseInpostError):
     """Is raised when no parcel is set in :class:`Parcel`"""
+
     pass
 
 
 class UnidentifiedParcelError(BaseInpostError):
     """Is raised when no other :class:`Parcel` error match"""
+
     pass
 
 
 # ----------------- API ----------------- #
 class NotAuthenticatedError(BaseInpostError):
     """Is raised when `Inpost.auth_token` is missing"""
+
     pass
 
 
 class ReAuthenticationError(BaseInpostError):
     """Is raised when `Inpost.auth_token` has expired"""
+
     pass
 
 
 class PhoneNumberError(BaseInpostError):
     """Is raised when `Inpost.phone_number` is invalid or unexpected error connected with phone number occurs"""
+
     pass
 
 
 class SmsCodeError(BaseInpostError):
     """Is raised when `Inpost.sms_code` is invalid or unexpected sms_code occurs"""
+
     pass
 
 
 class RefreshTokenError(BaseInpostError):
     """Is raised when `Inpost.refr_token` is invalid or unexpected error connected with refresh token occurs"""
+
     pass
 
 
 class NotFoundError(BaseInpostError):
     """Is raised when method from :class:`Inpost` returns 404 Not Found HTTP status code"""
+
     pass
 
 
 class UnauthorizedError(BaseInpostError):
     """Is raised when method from :class:`Inpost` returns 401 Unauthorized HTTP status code"""
+
     pass
 
 
 class UnidentifiedAPIError(BaseInpostError):
     """Is raised when no other API error match"""
+
     pass
 
 
 # ----------------- Other ----------------- #
 class UserLocationError(BaseInpostError):
     pass
 
 
 class SingleParamError(BaseInpostError):
     """Is raised when only one param must be filled in but got more"""
+
     pass
 
 
 class MissingParamsError(BaseInpostError):
     """Is raised when none of params are filled"""
+
     pass
 
 
 class UnidentifiedError(BaseInpostError):
     """Is raised when no other error match"""
+
     pass
```

### Comparing `inpost-0.1.3/inpost/static/friends.py` & `inpost-0.1.4/inpost/static/friends.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import logging
 
-from arrow import get, Arrow
+from arrow import Arrow, get
 
 
 class Friend:
     def __init__(self, friend_data, logger: logging.Logger):
-        self.uuid: str = friend_data['uuid'] if 'uuid' in friend_data else None
-        self.phone_number: str = friend_data['phoneNumber']
-        self.name: str = friend_data['name']
-        self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.uuid}')
-        self.invitaion_code: str | None = friend_data['invitationCode'] if 'invitationCode' in friend_data else None
-        self.created_date: Arrow | None = get(friend_data['createdDate']) if 'createdDate' in friend_data else None
-        self.expiry_date: Arrow | None = get(friend_data['expiryDate']) if 'expiryDate' in friend_data else None
+        self.uuid: str = friend_data["uuid"] if "uuid" in friend_data else None
+        self.phone_number: str = friend_data["phoneNumber"]
+        self.name: str = friend_data["name"]
+        self._log: logging.Logger = logger.getChild(f"{self.__class__.__name__}.{self.uuid}")
+        self.invitaion_code: str | None = friend_data["invitationCode"] if "invitationCode" in friend_data else None
+        self.created_date: Arrow | None = get(friend_data["createdDate"]) if "createdDate" in friend_data else None
+        self.expiry_date: Arrow | None = get(friend_data["expiryDate"]) if "expiryDate" in friend_data else None
 
         if self.invitaion_code:
-            self._log.debug(f'created friendship with {self.name} using from_invitation')
+            self._log.debug(f"created friendship with {self.name} using from_invitation")
         else:
-            self._log.debug(f'created friendship with {self.name}')
+            self._log.debug(f"created friendship with {self.name}")
 
     @classmethod
     def from_invitation(cls, invitation_data, logger: logging.Logger):
-        return cls(friend_data={'uuid': invitation_data['friend']['uuid'],
-                                'phoneNumber': invitation_data['friend']['phoneNumber'],
-                                'name': invitation_data['friend']['name'],
-                                'invitationCode': invitation_data['invitationCode'],
-                                'createdDate': invitation_data['createdDate'],
-                                'expiryDate': invitation_data['expiryDate']
-                                },
-                   logger=logger)
+        return cls(
+            friend_data={
+                "uuid": invitation_data["friend"]["uuid"],
+                "phoneNumber": invitation_data["friend"]["phoneNumber"],
+                "name": invitation_data["friend"]["name"],
+                "invitationCode": invitation_data["invitationCode"],
+                "createdDate": invitation_data["createdDate"],
+                "expiryDate": invitation_data["expiryDate"],
+            },
+            logger=logger,
+        )
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
```

### Comparing `inpost-0.1.3/inpost/static/notifications.py` & `inpost-0.1.4/inpost/static/notifications.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from arrow import get, Arrow
+from arrow import Arrow, get
 
 
-class Notification:
-    def __init__(self, notification_data):
-        self.id: str = notification_data['id']
-        self.type: str = notification_data['type']
-        self.action: str = notification_data['action']
-        self.date: Arrow = get(notification_data['date'])
-        self.title: str = notification_data['title']
-        self.content: str = notification_data['content']
-        self.shipment_number: str = notification_data['shipmentNumber']
-        self.read: bool = notification_data['read']
-        self.extra_params: dict = notification_data['extraParams']
-        self.parcel_type: str = notification_data['parcelType']
+class Notification:  # TODO: do docs
+    def __init__(self, notification_data):  # TODO: do docs
+        self.id: str = notification_data.get("id", None)
+        self.type: str = notification_data.get("type", None)
+        self.action: str = notification_data.get("action", None)
+        self.date: Arrow = get(notification_data.get("date")) if "date" in notification_data else None
+        self.title: str = notification_data.get("title", None)
+        self.content: str = notification_data.get("content", None)
+        self.shipment_number: str = notification_data.get("shipmentNumber", None)
+        self.read: bool = notification_data.get("read", None)
+        self.extra_params: dict = notification_data.get("extraParams", None)
+        self.parcel_type: str = notification_data.get("parcelType", None)
```

### Comparing `inpost-0.1.3/inpost/static/parcels.py` & `inpost-0.1.4/inpost/static/parcels.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,102 @@
 import logging
 import random
 from io import BytesIO
 from typing import List, Tuple
 
 import qrcode
-from arrow import get, arrow
+from arrow import arrow, get
 
-from inpost.static.statuses import *
+from inpost.static.statuses import (
+    CompartmentActualStatus,
+    ParcelCarrierSize,
+    ParcelDeliveryType,
+    ParcelLockerSize,
+    ParcelOwnership,
+    ParcelShipmentType,
+    ParcelStatus,
+    PaymentStatus,
+    PaymentType,
+    PointType,
+    ReturnsStatus,
+)
 
 
 class BaseParcel:
     def __init__(self, parcel_data: dict, logger: logging.Logger):
-        self.shipment_number: str = parcel_data.get('shipmentNumber')
-        self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
-        self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
-        self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
-        self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
-        self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
-                                          for event in parcel_data['eventLog']]
+        self.shipment_number = parcel_data.get("shipmentNumber")
+        self._log: logging.Logger = logger.getChild(f"{self.__class__.__name__}.{self.shipment_number}")
+        self.status: ParcelStatus = ParcelStatus[parcel_data.get("status")]
+        self.expiry_date: arrow | None = get(parcel_data["expiryDate"]) if "expiryDate" in parcel_data else None
+        self.operations: Operations = Operations(operations_data=parcel_data["operations"], logger=self._log)
+        self.event_log: List[EventLog] = [
+            EventLog(eventlog_data=event, logger=self._log) for event in parcel_data["eventLog"]
+        ]
 
 
 class Parcel(BaseParcel):
-    """Object representation of :class:`inpost.api.Inpost` compartment properties
+    """Object representation of :class:`inpost.api.Inpost` incoming parcel
 
     :param parcel_data: :class:`dict` containing all parcel data
     :type parcel_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, parcel_data: dict, logger: logging.Logger):
-        """Constructor method"""
+        """Constructor method
+
+        :param parcel_data: dict containing parcel data
+        :type parcel_data: dict
+        :param logger: logger instance
+        :type logger: logging.Logger
+        """
         super().__init__(parcel_data, logger)
-        self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
-        self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data['shipmentType']]
-        self._open_code: str | None = parcel_data.get('openCode', None)
-        self._qr_code: QRCode | None = QRCode(qrcode_data=parcel_data['qrCode'], logger=self._log) \
-            if 'qrCode' in parcel_data else None
-        self.stored_date: arrow | None = get(parcel_data['storedDate']) if 'storedDate' in parcel_data else None
-        self.pickup_date: arrow | None = get(parcel_data['pickUpDate']) if 'pickUpDate' in parcel_data else None
-        self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
-            if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
-        self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log) if 'receiver' in parcel_data else None
-        self.sender: Sender = Sender(sender_data=parcel_data['sender'], logger=self._log) if 'sender' in parcel_data else None
-        self.pickup_point: PickupPoint = PickupPoint(pickuppoint_data=parcel_data['pickUpPoint'], logger=self._log) \
-            if 'pickUpPoint' in parcel_data else None
-        self.multi_compartment: MultiCompartment | None = MultiCompartment(
-            parcel_data['multiCompartment'], logger=self._log) if 'multiCompartment' in parcel_data else None
-        self.is_end_off_week_collection: bool | None = parcel_data.get('endOfWeekCollection', None)
-        self.status: ParcelStatus = ParcelStatus[parcel_data['status']] if 'status' in parcel_data else None
-        self.avizo_transaction_status: str | None = parcel_data.get('avizoTransactionStatus', None)
-        self.shared_to: List[SharedTo] = [SharedTo(sharedto_data=person, logger=self._log)
-                                          for person in parcel_data['sharedTo']] if 'sharedTo' in parcel_data else None
-        self.ownership_status: ParcelOwnership = ParcelOwnership[parcel_data['ownershipStatus']] if 'ownershipStatus' in parcel_data else None
-        self.economy_parcel: bool | None = parcel_data.get('economyParcel', None)
+        self._log: logging.Logger = logger.getChild(f"{self.__class__.__name__}.{self.shipment_number}")
+        self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data.get("shipmentType")]
+        self._open_code: str | None = parcel_data.get("openCode", None)
+        self._qr_code: QRCode | None = (
+            QRCode(qrcode_data=parcel_data["qrCode"], logger=self._log) if "qrCode" in parcel_data else None
+        )
+        self.stored_date: arrow | None = get(parcel_data["storedDate"]) if "storedDate" in parcel_data else None
+        self.pickup_date: arrow | None = get(parcel_data["pickUpDate"]) if "pickUpDate" in parcel_data else None
+        self.parcel_size: ParcelLockerSize | ParcelCarrierSize = (
+            ParcelLockerSize[parcel_data.get("parcelSize")]
+            if self.shipment_type == ParcelShipmentType.parcel
+            else ParcelCarrierSize[parcel_data.get("parcelSize")]
+        )
+        self.receiver: Receiver | None = (
+            Receiver(receiver_data=parcel_data["receiver"], logger=self._log) if "receiver" in parcel_data else None
+        )
+        self.sender: Sender | None = (
+            Sender(sender_data=parcel_data["sender"], logger=self._log) if "sender" in parcel_data else None
+        )
+        self.pickup_point: PickupPoint | None = (
+            PickupPoint(point_data=parcel_data["pickUpPoint"], logger=self._log)
+            if "pickUpPoint" in parcel_data
+            else None
+        )
+        self.multi_compartment: MultiCompartment | None = (
+            MultiCompartment(parcel_data["multiCompartment"], logger=self._log)
+            if "multiCompartment" in parcel_data
+            else None
+        )
+
+        self.is_end_off_week_collection: bool | None = parcel_data.get("endOfWeekCollection", None)
+        self.status: ParcelStatus | None = ParcelStatus[parcel_data.get("status")]
+        self.avizo_transaction_status: str | None = parcel_data.get("avizoTransactionStatus", None)
+        self.shared_to: List[SharedTo] | None = (
+            [SharedTo(sharedto_data=person, logger=self._log) for person in parcel_data["sharedTo"]]
+            if "sharedTo" in parcel_data
+            else None
+        )
+        self.ownership_status: ParcelOwnership | None = ParcelOwnership[parcel_data.get("ownershipStatus")]
+        self.economy_parcel: bool | None = parcel_data.get("economyParcel", None)
         self._compartment_properties: CompartmentProperties | None = None
 
-        self._log.debug(f'created parcel with shipment number {self.shipment_number}')
+        self._log.debug(f"created parcel with shipment number {self.shipment_number}")
 
         # log all unexpected things, so you can make an issue @github
         if self.shipment_type == ParcelShipmentType.UNKNOWN:
             self._log.warning(f'unexpected shipment_type: {parcel_data["shipmentType"]}')
 
         if self.parcel_size == ParcelCarrierSize.UNKNOWN or self.parcel_size == ParcelLockerSize.UNKNOWN:
             self._log.warning(f'unexpected parcel_size: {parcel_data["parcelSize"]}')
@@ -67,561 +104,933 @@
         if self.status == ParcelStatus.UNKNOWN:
             self._log.warning(f'unexpected parcel status: {parcel_data["status"]}')
 
         if self.ownership_status == ParcelOwnership.UNKNOWN:
             self._log.warning(f'unexpected ownership status: {parcel_data["ownershipStatus"]}')
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     def __str__(self):
-        return f"Sender: {str(self.sender)}\n" \
-               f"Shipment number: {self.shipment_number}\n" \
-               f"Status: {self.status}\n" \
-               f"Pickup point: {self.pickup_point}"
+        return (
+            f"Sender: {str(self.sender)}\n"
+            f"Shipment number: {self.shipment_number}\n"
+            f"Status: {self.status}\n"
+            f"Pickup point: {self.pickup_point}"
+        )
 
     @property
     def open_code(self) -> str | None:
         """Returns an open code for :class:`Parcel`
 
         :return: Open code for :class:`Parcel`
         :rtype: str"""
-        self._log.debug('getting open code')
+        self._log.debug("getting open code")
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got open code')
+            self._log.debug("got open code")
             return self._open_code
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def generate_qr_image(self) -> BytesIO | None:
         """Returns a QR image for :class:`Parcel`
 
         :return: QR image for :class:`Parcel`
         :rtype: BytesIO"""
-        self._log.debug('generating qr image')
-        if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got qr image')
+        self._log.debug("generating qr image")
+        if self.shipment_type == ParcelShipmentType.parcel and self._qr_code is not None:
+            self._log.debug("got qr image")
             return self._qr_code.qr_image
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def compartment_properties(self):
         """Returns a compartment properties for :class:`Parcel`
 
         :return: Compartment properties for :class:`Parcel`
         :rtype: CompartmentProperties"""
-        self._log.debug('getting comparment properties')
+        self._log.debug("getting comparment properties")
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got compartment properties')
+            self._log.debug("got compartment properties")
             return self._compartment_properties
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_properties.setter
     def compartment_properties(self, compartmentproperties_data: dict):
         """Set compartment properties for :class:`Parcel`
 
         :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
-        :type compartmentproperties_data: CompartmentProperties"""
-        self._log.debug(f'setting compartment properties with {compartmentproperties_data}')
+        :type compartmentproperties_data: dict"""
+        self._log.debug(f"setting compartment properties with {compartmentproperties_data}")
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('compartment properties set')
-            self._compartment_properties = CompartmentProperties(compartmentproperties_data=compartmentproperties_data,
-                                                                 logger=self._log)
+            self._log.debug("compartment properties set")
+            self._compartment_properties = CompartmentProperties(
+                compartmentproperties_data=compartmentproperties_data, logger=self._log
+            )
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_location(self):
         """Returns a compartment location for :class:`Parcel`
 
         :return: Compartment location for :class:`Parcel`
         :rtype: CompartmentLocation"""
-        self._log.debug('getting compartment location')
+        self._log.debug("getting compartment location")
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got compartment location')
+            self._log.debug("got compartment location")
             return self._compartment_properties.location if self._compartment_properties else None
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_location.setter
     def compartment_location(self, location_data: dict):
         """Set compartment location for :class:`Parcel`
+
         :param location_data: :class:`dict` containing `compartment properties` data for :class:`Parcel`
-        :type location_data: CompartmentProperties"""
-        self._log.debug(f'setting compartment location with {location_data}')
-        if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('compartment location set')
+        :type location_data: dict"""
+        self._log.debug(f"setting compartment location with {location_data}")
+        if self.shipment_type == ParcelShipmentType.parcel and self._compartment_properties is not None:
+            self._log.debug("compartment location set")
             self._compartment_properties.location = location_data
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_status(self) -> CompartmentActualStatus | None:
         """Returns a compartment status for :class:`Parcel`
 
         :return: Compartment status for :class:`Parcel`
         :rtype: CompartmentActualStatus"""
-        self._log.debug('getting compartment status')
+        self._log.debug("getting compartment status")
 
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got compartment status')
+            self._log.debug("got compartment status")
             return self._compartment_properties.status if self._compartment_properties else None
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_status.setter
-    def compartment_status(self, status):
-        self._log.debug(f'setting compartment status with {status}')
+    def compartment_status(self, status) -> None:
+        self._log.debug(f"setting compartment status with {status}")
+        if self._compartment_properties is None:
+            return  # TODO: think out
+
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('compartment status set')
+            self._log.debug("compartment status set")
             self._compartment_properties.status = status
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
-    def compartment_open_data(self):
+    def compartment_open_data(self) -> dict | None:
         """Returns a compartment open data for :class:`Parcel`
 
         :return: dict containing compartment open data for :class:`Parcel`
         :rtype: dict"""
-        self._log.debug('getting compartment open data')
+        self._log.debug("getting compartment open data")
+        if self.receiver is None:
+            return None  # TODO: think out
+
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got compartment open data')
+            self._log.debug("got compartment open data")
             return {
-                'shipmentNumber': self.shipment_number,
-                'openCode': self._open_code,
-                'receiverPhoneNumber': self.receiver.phone_number
+                "shipmentNumber": self.shipment_number,
+                "openCode": self._open_code,
+                "receiverPhoneNumber": self.receiver.phone_number,
             }
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
-    def mocked_location(self):
+    def mocked_location(self) -> dict | None:
         """Returns a mocked location for :class:`Parcel`
 
-        :return: dict containing mocked location for :class:`Parcel`
-        :rtype: dict"""
-        self._log.debug('getting mocked location')
+        :return: dict containing mocked location for :class:`Parcel or None if wrong parcel shipment type`
+        :rtype: dict | None"""
+        self._log.debug("getting mocked location")
+        if self.pickup_point is None:
+            return None  # TODO: think out
         if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug('got mocked location')
+            self._log.debug("got mocked location")
             return {
-                'latitude': round(self.pickup_point.latitude + random.uniform(-0.00005, 0.00005), 6),
-                'longitude': round(self.pickup_point.longitude + random.uniform(-0.00005, 0.00005), 6),
-                'accuracy': round(random.uniform(1, 4), 1)
+                "latitude": round(self.pickup_point.latitude + random.uniform(-0.00005, 0.00005), 6),
+                "longitude": round(self.pickup_point.longitude + random.uniform(-0.00005, 0.00005), 6),
+                "accuracy": round(random.uniform(1, 4), 1),
             }
 
-        self._log.debug(f'wrong ParcelShipmentType: {repr(self.shipment_type)}')
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
-    def is_multicompartment(self):
+    def is_multicompartment(self) -> bool:
         """Specifies if parcel is in multi compartment
+
         :return: True if parcel is in multicompartment
         :rtype: bool"""
         return self.multi_compartment is not None
 
     @property
-    def is_main_multicompartment(self):
+    def is_main_multicompartment(self) -> bool | None:
         """Specifies if parcel is main parcel in multi compartment
         :return: True if parcel is in multicompartment
         :rtype: bool"""
-        if self.is_multicompartment:
+        if self.is_multicompartment and self.multi_compartment is not None:
             return self.multi_compartment.shipment_numbers is not None
 
         return None
 
     @property
-    def has_airsensor(self) -> bool:
-        return self.pickup_point.air_sensor_data is not None
+    def has_airsensor(self) -> bool | None:
+        if self.pickup_point is not None:
+            return self.pickup_point.air_sensor_data is not None
+
+        return None
 
     # @property
     # def get_from_multicompartment(self):
     #     return
 
 
-class ReturnParcel(BaseParcel):
+class ReturnParcel(BaseParcel):  # TODO: see properties and create
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         super().__init__(parcel_data, logger)
-        self.uuid: str = parcel_data['uuid']
-        self.rma: str = parcel_data['rma']
-        self.organization_name: str = parcel_data['organizationName']
-        self.created_date: arrow = parcel_data['createdDate']
-        self.accepted_date: arrow = parcel_data['acceptedDate']
-        self.expiry_date: arrow = parcel_data['expiryDate']
-        self.sent_date: arrow = parcel_data['sentDate']
-        self.delivered_date: arrow = parcel_data['deliveredDate']
-        self.order_number: str = parcel_data['orderNumber']
-        self.form_type: str = parcel_data['formType']
+        self.uuid: str = parcel_data["uuid"]
+        self.rma: str = parcel_data["rma"]
+        self.organization_name: str = parcel_data["organizationName"]
+        self.created_date: arrow = get(parcel_data["createdDate"])
+        self.accepted_date: arrow = get(parcel_data["acceptedDate"])
+        self.expiry_date: arrow = get(parcel_data["expiryDate"])
+        self.sent_date: arrow = get(parcel_data["sentDate"])
+        self.delivered_date: arrow = get(parcel_data["deliveredDate"])
+        self.order_number: str = parcel_data["orderNumber"]
+        self.form_type: str = parcel_data["formType"]
+
+
+class SentParcel(BaseParcel):  # TODO: check properties
+    def __init__(self, parcel_data: dict, logger: logging.Logger):
+        super().__init__(parcel_data, logger)
+        self.origin_system: str = parcel_data.get("originSystem", None)
+        self.quick_send_code: int = parcel_data.get("quickSendCode", None)
+        self._qr_code: QRCode | None = (
+            QRCode(qrcode_data=parcel_data["qrCode"], logger=self._log) if "qrCode" in parcel_data else None
+        )
+        self.confirmation_date: arrow = get(parcel_data.get("confirmationDate", None))
+        self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data["shipmentType"]]
+        self.parcel_size: ParcelLockerSize | ParcelCarrierSize = (
+            ParcelLockerSize[parcel_data.get("parcelSize")]
+            if self.shipment_type == ParcelShipmentType.parcel
+            else ParcelCarrierSize[parcel_data.get("parcelSize")]
+        )
+        self.receiver: Receiver | None = (
+            Receiver(receiver_data=parcel_data["receiver"], logger=self._log) if "receiver" in parcel_data else None
+        )
+        self.sender: Sender | None = (
+            Sender(sender_data=parcel_data["sender"], logger=self._log) if "sender" in parcel_data else None
+        )
+        self.pickup_point: PickupPoint | None = (
+            PickupPoint(point_data=parcel_data["pickUpPoint"], logger=self._log)
+            if "pickUpPoint" in parcel_data
+            else None
+        )
+        self.delivery_point: DeliveryPoint | None = (
+            DeliveryPoint(parcel_data["deliveryPoint"], logger=self._log) if "deliveryPoint" in parcel_data else None
+        )
+        self.drop_off_point: DropOffPoint | None = (
+            DropOffPoint(point_data=parcel_data["dropOffPoint"], logger=self._log)
+            if "dropOffPoint" in parcel_data
+            else None
+        )
+        self.payment: Payment | None = (
+            Payment(payment_details=parcel_data["payment"], logger=self._log) if "payment" in parcel_data else None
+        )
+        self.unlabeled: bool = parcel_data.get("unlabeled", None)
+        self.is_end_off_week_collection: bool | None = parcel_data.get("endOfWeekCollection", None)
+        self.status: ParcelStatus | None = ParcelStatus[parcel_data.get("status")]
+
+    @property
+    def open_code(self) -> int | None:
+        """Returns an open code for :class:`Parcel`
+
+        :return: Open code for :class:`Parcel`
+        :rtype: int"""
+        self._log.debug("getting open code")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("got open code")
+            return self.quick_send_code
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @property
+    def generate_qr_image(self) -> BytesIO | None:
+        """Returns a QR image for :class:`Parcel`
+
+        :return: QR image for :class:`Parcel`
+        :rtype: BytesIO"""
+        self._log.debug("generating qr image")
+        if self.shipment_type == ParcelShipmentType.parcel and self._qr_code is not None:
+            self._log.debug("got qr image")
+            return self._qr_code.qr_image
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @property
+    def compartment_properties(self):
+        """Returns a compartment properties for :class:`Parcel`
+
+        :return: Compartment properties for :class:`Parcel`
+        :rtype: CompartmentProperties"""
+        self._log.debug("getting comparment properties")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("got compartment properties")
+            return self._compartment_properties
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @compartment_properties.setter
+    def compartment_properties(self, compartmentproperties_data: dict):
+        """Set compartment properties for :class:`Parcel`
+
+        :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
+        :type compartmentproperties_data: dict"""
+        self._log.debug(f"setting compartment properties with {compartmentproperties_data}")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("compartment properties set")
+            self._compartment_properties = CompartmentProperties(
+                compartmentproperties_data=compartmentproperties_data, logger=self._log
+            )
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+
+    @property
+    def compartment_location(self):
+        """Returns a compartment location for :class:`Parcel`
+
+        :return: Compartment location for :class:`Parcel`
+        :rtype: CompartmentLocation"""
+        self._log.debug("getting compartment location")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("got compartment location")
+            return self._compartment_properties.location if self._compartment_properties else None
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @compartment_location.setter
+    def compartment_location(self, location_data: dict):
+        """Set compartment location for :class:`Parcel`
+        :param location_data: :class:`dict` containing `compartment properties` data for :class:`Parcel`
+        :type location_data: dict"""
+        self._log.debug(f"setting compartment location with {location_data}")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("compartment location set")
+            self._compartment_properties.location = location_data
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+
+    @property
+    def compartment_status(self) -> CompartmentActualStatus | None:
+        """Returns a compartment status for :class:`Parcel`
+
+        :return: Compartment status for :class:`Parcel`
+        :rtype: CompartmentActualStatus"""
+        self._log.debug("getting compartment status")
+
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("got compartment status")
+            return self._compartment_properties.status if self._compartment_properties else None
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @compartment_status.setter
+    def compartment_status(self, status):
+        self._log.debug(f"setting compartment status with {status}")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("compartment status set")
+            self._compartment_properties.status = status
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+
+    @property
+    def compartment_open_data(self):
+        """Returns a compartment open data for :class:`Parcel`
+
+        :return: dict containing compartment open data for :class:`Parcel`
+        :rtype: dict"""
+        self._log.debug("getting compartment open data")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("got compartment open data")
+            return {
+                "shipmentNumber": self.shipment_number,
+                "openCode": self._open_code,
+                "receiverPhoneNumber": self.receiver.phone_number,
+            }
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @property
+    def mocked_location(self):
+        """Returns a mocked location for :class:`Parcel`
+
+        :return: dict containing mocked location for :class:`Parcel`
+        :rtype: dict"""
+        self._log.debug("getting mocked location")
+        if self.shipment_type == ParcelShipmentType.parcel:
+            self._log.debug("got mocked location")
+            return {
+                "latitude": round(self.pickup_point.latitude + random.uniform(-0.00005, 0.00005), 6),
+                "longitude": round(self.pickup_point.longitude + random.uniform(-0.00005, 0.00005), 6),
+                "accuracy": round(random.uniform(1, 4), 1),
+            }
+
+        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        return None
+
+    @property
+    def has_airsensor(self) -> bool | None:
+        return self.pickup_point.air_sensor_data is not None if self.pickup_point else None
 
 
 class Receiver:
     """Object representation of :class:`Parcel` receiver
 
     :param receiver_data: :class:`dict` containing sender data for :class:`Parcel`
     :type receiver_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, receiver_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.email: str = receiver_data['email']
-        self.phone_number: str = receiver_data['phoneNumber']
-        self.name: str = receiver_data['name']
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
+        """Constructor method
+
+        :param receiver_data: dict containing receiver data
+        :type receiver_data: dict
+        :param logger: logger instance
+        :type logger: logging.Logger"""
+        self.email: str = receiver_data["email"]
+        self.phone_number: str = receiver_data["phoneNumber"]
+        self.name: str = receiver_data["name"]
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
 
-        self._log.debug('created')
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class Sender:
     """Object representation of :class:`Parcel` sender
 
     :param sender_data: :class:`dict` containing sender data for :class:`Parcel`
     :type sender_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, sender_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.sender_name: str = sender_data['name']
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
+        """Constructor method
 
-        self._log.debug('created')
+        :param sender_data: dict containing sender data
+        :type sender_data: dict
+        :param logger: logger instance
+        :type logger: logging.Logger"""
+        self.sender_name: str = sender_data.get("name", None)
+        self.sender_email: str = sender_data.get("email", None)
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     def __str__(self) -> str:
         return self.sender_name
 
 
-class PickupPoint:
-    """Object representation of :class:`Parcel` pickup point
+class Point:
+    """Object representation of :class:`Parcel` point
 
-    :param pickuppoint_data: :class:`dict` containing pickup point data for :class:`Parcel`
-    :type pickuppoint_data: dict
+    :param point_data: :class:`dict` containing point data for :class:`Parcel`
+    :type point_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
-    def __init__(self, pickuppoint_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.name: str = pickuppoint_data['name']
-        self.latitude: float = pickuppoint_data['location']['latitude']
-        self.longitude: float = pickuppoint_data['location']['longitude']
-        self.description: str = pickuppoint_data['locationDescription']
-        self.opening_hours: str = pickuppoint_data['openingHours']
-        self.post_code: str = pickuppoint_data['addressDetails']['postCode']
-        self.city: str = pickuppoint_data['addressDetails']['city']
-        self.province: str = pickuppoint_data['addressDetails']['province']
-        self.street: str = pickuppoint_data['addressDetails']['street']
-        self.building_number: str = pickuppoint_data['addressDetails']['buildingNumber']
-        self.virtual: int = pickuppoint_data['virtual']
-        self.point_type: str = pickuppoint_data['pointType']
-        self.type: List[ParcelDeliveryType] = [ParcelDeliveryType[data] for data in pickuppoint_data['type']]
-        self.location_round_the_clock: bool = pickuppoint_data['location247']
-        self.doubled: bool = pickuppoint_data['doubled']
-        self.image_url: str = pickuppoint_data['imageUrl']
-        self.easy_access_zone: bool = pickuppoint_data['easyAccessZone']
-        self.air_sensor: bool = pickuppoint_data['airSensor']
-        self.air_sensor_data: AirSensorData | None = AirSensorData(pickuppoint_data['airSensorData']) if 'airSensorData' in pickuppoint_data else None
+    def __init__(self, point_data: dict, logger: logging.Logger):
+        """Constructor method
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        :param point_data: :class:`dict` containing point data for :class:`Parcel`
+        :type point_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self.name: str = point_data["name"]
+        self.latitude: float = point_data["location"]["latitude"]
+        self.longitude: float = point_data["location"]["longitude"]
+        self.description: str = point_data["locationDescription"]
+        self.opening_hours: str = point_data["openingHours"]
+        self.post_code: str = point_data["addressDetails"]["postCode"]
+        self.city: str = point_data["addressDetails"]["city"]
+        self.province: str = point_data["addressDetails"]["province"]
+        self.street: str = point_data["addressDetails"]["street"]
+        self.building_number: str = point_data["addressDetails"]["buildingNumber"]
+        self.payment_type: List[PaymentType] | None = (
+            [PaymentType[pt] for pt in point_data["paymentType"]] if "paymentType" in point_data else None
+        )
+        self.virtual: int = point_data["virtual"]
+        self.point_type: PointType | None = PointType[point_data.get("pointType")]
+        self.type: List[ParcelDeliveryType] = (
+            [ParcelDeliveryType[data] for data in point_data["type"]] if "type" in point_data else None
+        )
+        self.location_round_the_clock: bool = point_data["location247"]
+        self.doubled: bool = point_data["doubled"]
+        self.image_url: str = point_data["imageUrl"]
+        self.easy_access_zone: bool = point_data["easyAccessZone"]
+        self.air_sensor: bool = point_data["airSensor"]
+        self.air_sensor_data: AirSensorData | None = (
+            AirSensorData(point_data["airSensorData"], self._log) if "airSensorData" in point_data else None
+        )
+        self.remote_send: bool = point_data.get("remoteSend", None)
+        self.remote_return: bool = point_data.get("remoteReturn", None)
 
+        self._log.debug("created")
         if ParcelDeliveryType.UNKNOWN in self.type:
-            self._log.debug(f'unknown delivery type: {pickuppoint_data["type"]}')
+            self._log.debug(f'unknown delivery type: {point_data["type"]}')
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     def __str__(self) -> str:
         return self.name
 
     @property
     def location(self) -> Tuple[float, float]:
         """Returns a mocked location for :class:`PickupPoint`
 
         :return: tuple containing location for :class:`PickupPoint`
         :rtype: tuple"""
-        self._log.debug('getting location')
+        self._log.debug("getting location")
         return self.latitude, self.longitude
 
 
+class PickupPoint(Point):
+    """Object representation of :class:`Parcel` pick up point
+
+    :param point_data: :class:`dict` containing pickup point data for :class:`Parcel`
+    :type point_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger"""
+
+    def __init__(self, point_data: dict, logger: logging.Logger):
+        super().__init__(point_data, logger)
+
+
+class DropOffPoint(Point):
+    """Object representation of :class:`Parcel` drop off point
+
+    :param point_data: :class:`dict` containing pickup point data for :class:`Parcel`
+    :type point_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger"""
+
+    def __init__(self, point_data: dict, logger: logging.Logger):
+        super().__init__(point_data, logger)
+
+
+class DeliveryPoint:
+    """Object representation of :class: DeliveryPoint
+
+    :param delivery_point: :class:`dict` containing delivery point data for :class:`DeliveryPoint`
+    :type delivery_point: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger"""
+
+    def __init__(self, delivery_point: dict, logger: logging.Logger):
+        self.name = delivery_point.get("name")
+        self.company_name = delivery_point.get("companyName")
+        self.post_code = delivery_point["address"]["postCode"] if "address" in delivery_point else None
+        self.city = delivery_point["address"]["city"] if "address" in delivery_point else None
+        self.street = delivery_point["address"]["street"] if "address" in delivery_point else None
+        self.building_number = delivery_point["address"]["buildingNumber"] if "address" in delivery_point else None
+        self.flat_numer = delivery_point["address"]["flatNumber"] if "address" in delivery_point else None
+
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
+
+    def __repr__(self):
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
+
+
+class Payment:
+    """Object representation of :class: Payment
+    :param payment_details: :class:`dict` containing payment data for :class:`Payment`
+    :type payment_details: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger"""
+
+    def __init__(self, payment_details: dict, logger: logging.Logger):
+        # self.paid: bool = payment_details.get("paid")
+        # self.total_price: float = payment_details.get("totalPrice")
+        # self.insurance_price: float = payment_details.get("insurancePrice")
+        # self.end_of_week_collection_price: float = payment_details.get("endOfWeekCollectionPrice")
+        # self.shipment_discounted: bool = payment_details.get("shipmentDiscounted")
+        # self.transaction_status: str = payment_details.get("transactionStatus")
+
+        self.paid = payment_details.get("paid")
+        self.total_price = payment_details.get("totalPrice")
+        self.insurance_price = payment_details.get("insurancePrice")
+        self.end_of_week_collection_price = payment_details.get("endOfWeekCollectionPrice")
+        self.shipment_discounted = payment_details.get("shipmentDiscounted")
+        self.transaction_status = payment_details.get("transactionStatus")
+
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
+
+    def __repr__(self):
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
+
+
 class MultiCompartment:
     """Object representation of :class:`Parcel` `multicompartment`
 
     :param multicompartment_data: :class:`dict` containing multicompartment data for :class:`Parcel`
     :type multicompartment_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, multicompartment_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.uuid = multicompartment_data['uuid']
-        self.shipment_numbers: List[str] | None = multicompartment_data['shipmentNumbers'] \
-            if 'shipmentNumbers' in multicompartment_data else None
-        self.presentation: bool = multicompartment_data['presentation']
-        self.collected: bool = multicompartment_data['collected']
+        """Constructor method:param multicompartment_data: :class:`dict` containing multicompartment data for :class:`Parcel`
+
+        :type multicompartment_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self.uuid = multicompartment_data["uuid"]
+        self.shipment_numbers: List[str] | None = (
+            multicompartment_data["shipmentNumbers"] if "shipmentNumbers" in multicompartment_data else None
+        )
+        self.presentation: bool = multicompartment_data["presentation"]
+        self.collected: bool = multicompartment_data["collected"]
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class Operations:
     """Object representation of :class:`Parcel` `operations`
 
     :param operations_data: :class:`dict` containing operations data for :class:`Parcel`
     :type operations_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, operations_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.manual_archive: bool = operations_data['manualArchive']
-        self.auto_archivable_since: arrow | None = get(
-            operations_data['autoArchivableSince']) if 'autoArchivableSince' in operations_data else None
-        self.delete: bool = operations_data['delete']
-        self.collect: bool = operations_data['collect']
-        self.expand_avizo: bool = operations_data['expandAvizo']
-        self.highlight: bool = operations_data['highlight']
-        self.refresh_until: arrow = get(operations_data['refreshUntil'])
-        self.request_easy_access_zone: str = operations_data['requestEasyAccessZone']
-        self.is_voicebot: bool = operations_data['voicebot']
-        self.can_share_to_observe: bool = operations_data['canShareToObserve']
-        self.can_share_open_code: bool = operations_data['canShareOpenCode']
-        self.can_share_parcel: bool = operations_data['canShareParcel']
-        self.send: bool | None = operations_data['send'] if 'send' in operations_data else None
+        """Constructor method
+
+        :param operations_data: :class:`dict` containing operations data for :class:`Parcel`
+        :type operations_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self.manual_archive: bool = operations_data["manualArchive"]
+        self.auto_archivable_since: arrow | None = (
+            get(operations_data["autoArchivableSince"]) if "autoArchivableSince" in operations_data else None
+        )
+        self.delete: bool = operations_data.get("delete", None)
+        self.pay_to_send: bool = operations_data.get("payToSend", None)
+        self.collect: bool = operations_data.get("collect", None)
+        self.expand_avizo: bool = operations_data.get("expandAvizo", None)
+        self.highlight: bool = operations_data.get("highlight", None)
+        self.refresh_until: arrow = get(operations_data["refreshUntil"]) if "refreshUntil" in operations_data else None
+        self.request_easy_access_zone: str = operations_data.get("requestEasyAccessZone", None)
+        self.is_voicebot: bool = operations_data.get("voicebot", None)
+        self.can_share_to_observe: bool = operations_data.get("canShareToObserve", None)
+        self.can_share_open_code: bool = operations_data.get("canShareOpenCode", None)
+        self.can_share_parcel: bool = operations_data.get("canShareParcel", None)
+        self.send: bool | None = operations_data.get("send", None)
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class EventLog:
     """Object representation of :class:`Parcel` single eventlog
 
     :param eventlog_data: :class:`dict` containing single eventlog data for :class:`Parcel`
     :type eventlog_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, eventlog_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.type: str = eventlog_data['type']
-        self.name: ParcelStatus | ReturnsStatus = ParcelStatus[
-            eventlog_data['name']] if self.type == 'PARCEL_STATUS' else ReturnsStatus[eventlog_data['name']]
-        self.date: arrow = get(eventlog_data['date'])
+        """Constructor method
+
+        :param eventlog_data: :class:`dict` containing single eventlog data for :class:`Parcel`
+        :type eventlog_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self.type: str = eventlog_data["type"]
+        if self.type == "PARCEL_STATUS":
+            self.name = ParcelStatus[eventlog_data.get("name")]
+        elif self.type == "RETURN_STATUS":
+            self.name = ReturnsStatus[eventlog_data.get("name")]
+        elif self.type == "PAYMENT":
+            self.name = PaymentStatus[eventlog_data.get("name")]
+        else:
+            ...
+        self.date: arrow = get(eventlog_data["date"])
+        self.details: dict | None = eventlog_data.get("details")
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
         if self.name == ParcelStatus.UNKNOWN or self.name == ReturnsStatus.UNKNOWN:
             self._log.debug(f'unknown {self.type}: {eventlog_data["name"]}')
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class SharedTo:
     """Object representation of :class:`Parcel` single shared to
 
     :param sharedto_data: :class:`dict` containing shared to data for :class:`Parcel`
     :type sharedto_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, sharedto_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.uuid: str = sharedto_data['uuid']
-        self.name: str = sharedto_data['name']
-        self.phone_number = sharedto_data['phoneNumber']
+        """Constructor method
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        :param sharedto_data: :class:`dict` containing shared to data for :class:`Parcel`
+        :type sharedto_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self.uuid: str = sharedto_data["uuid"]
+        self.name: str = sharedto_data["name"]
+        self.phone_number = sharedto_data["phoneNumber"]
+
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class QRCode:
     """Object representation of :class:`Parcel` QRCode
 
     :param qrcode_data: :class:`str` containing qrcode data for :class:`Parcel`
     :type qrcode_data: str
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, qrcode_data: str, logger: logging.Logger):
-        """Constructor method"""
+        """Constructor method
+
+        :param qrcode_data: :class:`str` containing qrcode data for :class:`Parcel`
+        :type qrcode_data: str
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
         self._qr_code = qrcode_data
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     @property
     def qr_image(self) -> BytesIO:
         """Returns a generated QR image for :class:`QRCode`
 
         :return: QR Code image
         :rtype: BytesIO"""
-        self._log.debug('generating qr image')
+        self._log.debug("generating qr image")
         qr = qrcode.QRCode(
-            version=3,
-            error_correction=qrcode.constants.ERROR_CORRECT_H,
-            box_size=20,
-            border=4,
-            mask_pattern=5
+            version=3, error_correction=qrcode.constants.ERROR_CORRECT_H, box_size=20, border=4, mask_pattern=5
         )
 
         qr.add_data(self._qr_code)
         qr.make(fit=False)
         img1 = qr.make_image(fill_color="black", back_color="white")
         bio = BytesIO()
-        bio.name = 'qr.png'
-        img1.save(bio, 'PNG')
+        bio.name = "qr.png"
+        img1.save(bio, "PNG")
         bio.seek(0)
-        self._log.debug('generated qr image')
+        self._log.debug("generated qr image")
         return bio
 
 
 class CompartmentLocation:
     """Object representation of :class:`CompartmentProperties` compartment location
 
     :param compartmentlocation_data: :class:`dict` containing compartment location data for :class:`Parcel`
     :type compartmentlocation_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, compartmentlocation_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self.name: str = compartmentlocation_data['compartment']['name']
-        self.side: str = compartmentlocation_data['compartment']['location']['side']
-        self.column: str = compartmentlocation_data['compartment']['location']['column']
-        self.row: str = compartmentlocation_data['compartment']['location']['row']
-        self.open_compartment_waiting_time: int = compartmentlocation_data['openCompartmentWaitingTime']
-        self.action_time: int = compartmentlocation_data['actionTime']
-        self.confirm_action_time: int = compartmentlocation_data['confirmActionTime']
+        """Constructor method
+
+        :param compartmentlocation_data: :class:`dict` containing compartment location data for :class:`Parcel`
+        :type compartmentlocation_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self.name: str = compartmentlocation_data["compartment"]["name"]
+        self.side: str = compartmentlocation_data["compartment"]["location"]["side"]
+        self.column: str = compartmentlocation_data["compartment"]["location"]["column"]
+        self.row: str = compartmentlocation_data["compartment"]["location"]["row"]
+        self.open_compartment_waiting_time: int = compartmentlocation_data["openCompartmentWaitingTime"]
+        self.action_time: int = compartmentlocation_data["actionTime"]
+        self.confirm_action_time: int = compartmentlocation_data["confirmActionTime"]
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class CompartmentProperties:
     """Object representation of :class:`Parcel` compartment properties
 
     :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
     :type compartmentproperties_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, compartmentproperties_data: dict, logger: logging.Logger):
-        """Constructor method"""
-        self._session_uuid: str = compartmentproperties_data['sessionUuid']
-        self._session_expiration_time: int = compartmentproperties_data['sessionExpirationTime']
+        """Constructor method
+
+        :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
+        :type compartmentproperties_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self._session_uuid: str = compartmentproperties_data["sessionUuid"]
+        self._session_expiration_time: int = compartmentproperties_data["sessionExpirationTime"]
         self._location: CompartmentLocation | None = None
         self._status: CompartmentActualStatus | None = None
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
 
     def __repr__(self):
-        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     @property
     def session_uuid(self):
         """Returns a session unique identified for :class:`CompartmentProperties`
 
         :return: string containing session unique identified for :class:`CompartmentProperties`
         :rtype: str"""
-        self._log.debug('getting session uuid')
+        self._log.debug("getting session uuid")
         return self._session_uuid
 
     @property
     def location(self):
         """Returns a compartment location for :class:`CompartmentProperties`
 
         :return: compartment location for :class:`CompartmentProperties`
         :rtype: str"""
-        self._log.debug('getting location')
+        self._log.debug("getting location")
         return self._location
 
     @location.setter
     def location(self, location_data: dict):
         """Set a compartment location for :class:`CompartmentProperties`
 
         :param location_data: dict containing compartment location data for :class:`CompartmentProperties`
         :type location_data: dict"""
-        self._log.debug('setting location')
+        self._log.debug("setting location")
         self._location = CompartmentLocation(location_data, self._log)
 
     @property
     def status(self):
         """Returns a compartment status for :class:`CompartmentProperties`
 
         :return: compartment location for :class:`CompartmentProperties`
         :rtype: CompartmentActualStatus"""
-        self._log.debug('getting status')
+        self._log.debug("getting status")
         return self._status
 
     @status.setter
     def status(self, status_data: str | CompartmentActualStatus):
-        self._log.debug('setting status')
-        self._status = status_data if isinstance(status_data, CompartmentActualStatus) \
-            else CompartmentActualStatus[status_data]
+        self._log.debug("setting status")
+        self._status = (
+            status_data if isinstance(status_data, CompartmentActualStatus) else CompartmentActualStatus[status_data]
+        )
 
         if self._status == CompartmentActualStatus.UNKNOWN and isinstance(status_data, str):
-            self._log.warning(f'unexpected compartment actual status: {status_data}')
+            self._log.warning(f"unexpected compartment actual status: {status_data}")
 
 
 class AirSensorData:
     """Object representation of :class:`Parcel` air sensor data
 
     :param airsensor_data: :class:`dict` containing air sensor data for :class:`Parcel`
     :type airsensor_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
+
     def __init__(self, airsensor_data: dict, logger: logging.Logger):
-        self.updated_until: arrow = airsensor_data['updatedUntil']
-        self.air_quality: str = airsensor_data['airQuality']
-        self.temperature: float = airsensor_data['temperature']
-        self.humidity: float = airsensor_data['humidity']
-        self.pressure: float = airsensor_data['pressure']
-        self.pm25_value: float = airsensor_data['pollutants']['pm25']['value']
-        self.pm25_percent: float = airsensor_data['pollutants']['pm25']['percent']
-        self.pm10_value: float = airsensor_data['pollutants']['pm10']['value']
-        self.pm10_percent: float = airsensor_data['pollutants']['pm10']['percent']
+        """Constructor method
+
+        :param airsensor_data: :class:`dict` containing air sensor data for :class:`Parcel`
+        :type airsensor_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+        self.updated_until: arrow = airsensor_data["updatedUntil"]
+        self.air_quality: str = airsensor_data["airQuality"]
+        self.temperature: float = airsensor_data["temperature"]
+        self.humidity: float = airsensor_data["humidity"]
+        self.pressure: float = airsensor_data["pressure"]
+        self.pm25_value: float = airsensor_data["pollutants"]["pm25"]["value"]
+        self.pm25_percent: float = airsensor_data["pollutants"]["pm25"]["percent"]
+        self.pm10_value: float = airsensor_data["pollutants"]["pm10"]["value"]
+        self.pm10_percent: float = airsensor_data["pollutants"]["pm10"]["percent"]
 
-        self._log: logging.Logger = logger.getChild(__class__.__name__)
-        self._log.debug('created')
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+        self._log.debug("created")
```

### Comparing `inpost-0.1.3/inpost/static/statuses.py` & `inpost-0.1.4/inpost/static/statuses.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from enum import Enum, EnumMeta
-from typing import List
 
 
 class Meta(EnumMeta):  # temporary handler for unexpected keys in enums
-    def __getitem__(cls, item):
+    def __getitem__(self, item):
         try:
-            return super().__getitem__(item)
-        except KeyError as error:
-            return cls.UNKNOWN
+            return super().__getitem__(item) if item is not None else None
+        except KeyError:
+            return self.UNKNOWN
 
-    def __getattribute__(cls, item):
+    def __getattribute__(self, item):
         try:
-            return super().__getattribute__(item)
-        except KeyError as error:
-            return cls.UNKNOWN
-
-    def get_all(cls):
-        return [getattr(cls, name) for name in cls.__members__]
-
-    def get_without(cls, without: 'ParcelBase' | List['ParcelBase']):
-        if isinstance(without, ParcelBase):
-            without = [without]
-
-        return [element for element in cls.get_all() if element not in without]
+            return super().__getattribute__(item) if item is not None else None
+        except KeyError:
+            return self.UNKNOWN
+
+    # def get_all(cls):
+    #     return [getattr(cls, name) for name in cls.__members__]
+    #
+    # def get_without(cls, without: "ParcelBase" | List["ParcelBase"]):
+    #     if isinstance(without, ParcelBase):
+    #         without = [without]
+    #
+    #     return [element for element in cls.get_all() if element not in without]
 
 
 class ParcelBase(Enum, metaclass=Meta):
     """Base :class:`Enum` class to derive from"""
 
     def __gt__(self, other):
         if isinstance(other, ParcelBase):
@@ -56,145 +55,190 @@
         if isinstance(other, ParcelBase):
             return self.name == other.name
 
         return False
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items())
-        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
+        return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class ParcelCarrierSize(ParcelBase):
     """:class:`Enum` that holds parcel size for carrier shipment type"""
-    UNKNOWN = 'UNKNOWN DATA'
-    A = '8x38x64'
-    B = '19x38x64'
-    C = '41x38x64'
-    D = '50x50x80'
-    OTHER = 'UNKNOWN DIMENSIONS'
+
+    UNKNOWN = "UNKNOWN DATA"
+    A = "8x38x64"
+    B = "19x38x64"
+    C = "41x38x64"
+    D = "50x50x80"
+    OTHER = "UNKNOWN DIMENSIONS"
 
 
 class ParcelLockerSize(ParcelBase):
     """:class:`Enum` that holds parcel size for parcel locker shipment type"""
-    UNKNOWN = 'UNKNOWN DATA'
-    A = '8x38x64'
-    B = '19x38x64'
-    C = '41x38x64'
+
+    UNKNOWN = "UNKNOWN DATA"
+    A = "8x38x64"
+    B = "19x38x64"
+    C = "41x38x64"
 
 
 class ParcelDeliveryType(ParcelBase):
     """:class:`Enum` that holds parcel delivery types"""
-    UNKNOWN = 'UNKNOWN DATA'
-    parcel_locker = 'Paczkomat'
-    courier = 'Kurier'
-    parcel_point = 'PaczkoPunkt'
+
+    UNKNOWN = "UNKNOWN DATA"
+    parcel_locker = "Paczkomat"
+    courier = "Kurier"
+    parcel_point = "PaczkoPunkt"
 
 
 class ParcelShipmentType(ParcelBase):
     """:class:`Enum` that holds parcel shipment types"""
-    UNKNOWN = 'UNKNOWN DATA'
-    parcel = 'Paczkomat'
-    courier = 'Kurier'
-    parcel_point = 'PaczkoPunkt'
+
+    UNKNOWN = "UNKNOWN DATA"
+    parcel = "Paczkomat"
+    courier = "Kurier"
+    parcel_point = "PaczkoPunkt"
 
 
 class ParcelAdditionalInsurance(ParcelBase):
-    UNKNOWN = 'UNKNOWN DATA'
+    UNKNOWN = "UNKNOWN DATA"
     UNINSURANCED = 1
     ONE = 2  # UPTO 5000
     TWO = 3  # UPTO 10000
     THREE = 4  # UPTO 20000
 
 
 class ParcelType(ParcelBase):
     """:class:`Enum` that holds parcel types"""
-    UNKNOWN = 'UNKNOWN DATA'
-    TRACKED = 'Przychodzące'
-    SENT = 'Wysłane'
-    RETURNS = 'Zwroty'
+
+    UNKNOWN = "UNKNOWN DATA"
+    TRACKED = "Przychodzące"
+    SENT = "Wysłane"
+    RETURNS = "Zwroty"
+
+
+class PointType(ParcelBase):
+    """:class: `Enum` that holds point types"""
+
+    UNKNOWN = "UNNKOWN DATA"
+    PL = "Paczkomat"
+    parcel_locker_superpop = "some paczkomat or pok stuff"  # TODO: get known what does superpop stand for
+    POK = "Mobilny punkt obsługi klienta"
+    POP = "Punkt odbioru paczki"
+
+
+class ParcelPointOperations(ParcelBase):
+    """:class: `Enum` that holds parcel operation types"""
+
+    UNKNOWN = "UNNKOWN DATA"
+    CREATE = "c2x-target"
+    SEND = "remote-send"
 
 
 class ParcelStatus(ParcelBase):
     """:class:`Enum` that holds parcel statuses"""
-    UNKNOWN = 'UNKNOWN DATA'
-    CREATED = 'Utworzona'  # TODO: translate from app
-    OFFERS_PREPARED = 'Oferty przygotowane'  # TODO: translate from app
-    OFFER_SELECTED = 'Oferta wybrana'  # TODO: translate from app
-    CONFIRMED = 'Potwierdzona'
-    READY_TO_PICKUP_FROM_POK = 'Gotowa do odbioru w PaczkoPunkcie'
-    OVERSIZED = 'Gabaryt'
-    DISPATCHED_BY_SENDER_TO_POK = 'Nadana w PaczkoPunkcie'
-    DISPATCHED_BY_SENDER = 'Nadana w paczkomacie'
-    COLLECTED_FROM_SENDER = 'Odebrana od nadawcy'
-    TAKEN_BY_COURIER = 'Odebrana przez Kuriera'
-    ADOPTED_AT_SOURCE_BRANCH = 'Przyjęta w oddziale'
-    SENT_FROM_SOURCE_BRANCH = 'Wysłana z oddziału'
-    READDRESSED = 'Zmiana punktu dostawy'  # TODO: translate from app
-    OUT_FOR_DELIVERY = 'Wydana do doręczenia'
-    READY_TO_PICKUP = 'Gotowa do odbioru'
-    PICKUP_REMINDER_SENT = 'Wysłano przypomnienie o odbiorze'  # TODO: translate from app
-    PICKUP_TIME_EXPIRED = 'Upłynął czas odbioru'  # TODO: translate from app
-    AVIZO = 'Powrót do oddziału'
-    TAKEN_BY_COURIER_FROM_POK = 'Odebrana z PaczkoPunktu nadawczego'
-    REJECTED_BY_RECEIVER = 'Odrzucona przez odbiorcę'  # TODO: translate from app
-    UNDELIVERED = 'Nie dostarczona'  # TODO: translate from app
-    DELAY_IN_DELIVERY = 'Opóźnienie w dostarczeniu'  # TODO: translate from app
-    RETURNED_TO_SENDER = 'Zwrócona do nadawcy'  # TODO: translate from app
-    READY_TO_PICKUP_FROM_BRANCH = 'Gotowa do odbioru z oddziału'  # TODO: translate from app
-    DELIVERED = 'Doręczona'
-    CANCELED = 'Anulowana'  # TODO: translate from app
-    CLAIMED = 'Zareklamowana'
-    STACK_IN_CUSTOMER_SERVICE_POINT = 'Przesyłka magazynowana w punkcie obsługi klienta'  # TODO: translate from app
-    STACK_PARCEL_PICKUP_TIME_EXPIRED = 'Upłynął czas odbioru'  # TODO: translate from app
-    UNSTACK_FROM_CUSTOMER_SERVICE_POINT = '?'  # TODO: translate from app
-    COURIER_AVIZO_IN_CUSTOMER_SERVICE_POINT = 'Przekazana do punktu obsługi klienta'  # TODO: translate from app
-    TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT = 'Odebrana przez kuriera z punktu obsługi klienta'  # TODO: translate from app
-    STACK_IN_BOX_MACHINE = 'Przesyłka magazynowana w paczkomacie tymczasowym'
-    STACK_PARCEL_IN_BOX_MACHINE_PICKUP_TIME_EXPIRED = 'Upłynął czas odbioru z paczkomatu'  # TODO: translate from app
-    UNSTACK_FROM_BOX_MACHINE = 'Odebrana z paczkomatu'  # TODO: translate from app
-    ADOPTED_AT_SORTING_CENTER = 'Przyjęta w sortowni'
-    OUT_FOR_DELIVERY_TO_ADDRESS = 'Gotowa do doręczenia'
-    PICKUP_REMINDER_SENT_ADDRESS = 'Wysłano przypomnienie o odbiorze'  # TODO: translate from app
-    UNDELIVERED_WRONG_ADDRESS = 'Nie dostarczono z powodu złego adresu'  # TODO: translate from app
-    UNDELIVERED_COD_CASH_RECEIVER = 'Nie dostarczono z powodu nieopłacenia'  # TODO: translate from app
-    REDIRECT_TO_BOX = 'Przekierowana do paczkomatu'  # TODO: translate from app
-    CANCELED_REDIRECT_TO_BOX = 'Anulowano przekierowanie do paczkomatu'  # TODO: translate from app
+
+    UNKNOWN = "UNKNOWN DATA"
+    CREATED = "W trakcie przygotowania"  # TODO: translate from app
+    OFFERS_PREPARED = "Oferty przygotowane"  # TODO: translate from app
+    OFFER_SELECTED = "Oferta wybrana"  # TODO: translate from app
+    CONFIRMED = "Potwierdzona"
+    READY_TO_PICKUP_FROM_POK = "Gotowa do odbioru w PaczkoPunkcie"
+    OVERSIZED = "Gabaryt"
+    DISPATCHED_BY_SENDER_TO_POK = "Nadana w PaczkoPunkcie"
+    DISPATCHED_BY_SENDER = "Nadana w paczkomacie"
+    COLLECTED_FROM_SENDER = "Odebrana od nadawcy"
+    TAKEN_BY_COURIER = "Odebrana przez Kuriera"
+    ADOPTED_AT_SOURCE_BRANCH = "Przyjęta w oddziale"
+    SENT_FROM_SOURCE_BRANCH = "Wysłana z oddziału"
+    READDRESSED = "Zmiana punktu dostawy"  # TODO: translate from app
+    OUT_FOR_DELIVERY = "Wydana do doręczenia"
+    READY_TO_PICKUP = "Gotowa do odbioru"
+    PICKUP_REMINDER_SENT = "Wysłano przypomnienie o odbiorze"  # TODO: translate from app
+    PICKUP_TIME_EXPIRED = "Upłynął czas odbioru"  # TODO: translate from app
+    AVIZO = "Powrót do oddziału"
+    TAKEN_BY_COURIER_FROM_POK = "Odebrana z PaczkoPunktu nadawczego"
+    REJECTED_BY_RECEIVER = "Odrzucona przez odbiorcę"  # TODO: translate from app
+    UNDELIVERED = "Nie dostarczona"  # TODO: translate from app
+    DELAY_IN_DELIVERY = "Opóźnienie w dostarczeniu"  # TODO: translate from app
+    RETURNED_TO_SENDER = "Zwrócona do nadawcy"  # TODO: translate from app
+    READY_TO_PICKUP_FROM_BRANCH = "Gotowa do odbioru z oddziału"  # TODO: translate from app
+    DELIVERED = "Doręczona"
+    CANCELED = "Anulowana"  # TODO: translate from app
+    CLAIMED = "Zareklamowana"
+    STACK_IN_CUSTOMER_SERVICE_POINT = "Przesyłka magazynowana w punkcie obsługi klienta"  # TODO: translate from app
+    STACK_PARCEL_PICKUP_TIME_EXPIRED = "Upłynął czas odbioru"  # TODO: translate from app
+    UNSTACK_FROM_CUSTOMER_SERVICE_POINT = "?"  # TODO: translate from app
+    COURIER_AVIZO_IN_CUSTOMER_SERVICE_POINT = "Przekazana do punktu obsługi klienta"  # TODO: translate from app
+    TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT = (
+        "Odebrana przez kuriera z punktu obsługi klienta"  # TODO: translate from app
+    )
+    STACK_IN_BOX_MACHINE = "Przesyłka magazynowana w paczkomacie tymczasowym"
+    STACK_PARCEL_IN_BOX_MACHINE_PICKUP_TIME_EXPIRED = "Upłynął czas odbioru z paczkomatu"  # TODO: translate from app
+    UNSTACK_FROM_BOX_MACHINE = "Odebrana z paczkomatu"  # TODO: translate from app
+    ADOPTED_AT_SORTING_CENTER = "Przyjęta w sortowni"
+    OUT_FOR_DELIVERY_TO_ADDRESS = "Gotowa do doręczenia"
+    PICKUP_REMINDER_SENT_ADDRESS = "Wysłano przypomnienie o odbiorze"  # TODO: translate from app
+    UNDELIVERED_WRONG_ADDRESS = "Nie dostarczono z powodu złego adresu"  # TODO: translate from app
+    UNDELIVERED_COD_CASH_RECEIVER = "Nie dostarczono z powodu nieopłacenia"  # TODO: translate from app
+    REDIRECT_TO_BOX = "Przekierowana do paczkomatu"  # TODO: translate from app
+    CANCELED_REDIRECT_TO_BOX = "Anulowano przekierowanie do paczkomatu"  # TODO: translate from app
+
+
+class DeliveryType(ParcelBase):  # TODO: look for more types
+    UNKNOWN = "UNKNOWN DATA"
+    BOX_MACHINE = "Paczkomat"
 
 
 class ReturnsStatus(ParcelBase):  # TODO: translate from app and fill missing ones
-    ACCEPTED = 'Zaakceptowano'
-    USED = 'Nadano'
-    DELIVERED = 'Dostarczono'
-    UNKNOWN = 'UNKNOWN DATA'
+    ACCEPTED = "Zaakceptowano"
+    USED = "Nadano"
+    DELIVERED = "Dostarczono"
+    UNKNOWN = "UNKNOWN DATA"
 
 
 class ParcelOwnership(ParcelBase):
     """:class:`Enum` that holds parcel ownership types"""
-    UNKNOWN = 'UNKNOWN DATA'
-    FRIEND = 'Zaprzyjaźniona'
-    OWN = 'Własna'
+
+    UNKNOWN = "UNKNOWN DATA"
+    FRIEND = "Zaprzyjaźniona"
+    OWN = "Własna"
 
 
 # both are the same, only for being clear
 class CompartmentExpectedStatus(ParcelBase):
     """:class:`Enum` that holds compartment expected statuses"""
-    UNKNOWN = 'UNKNOWN DATA'
-    OPENED = 'Otwarta'
-    CLOSED = 'Zamknięta'
+
+    UNKNOWN = "UNKNOWN DATA"
+    OPENED = "Otwarta"
+    CLOSED = "Zamknięta"
 
 
 class CompartmentActualStatus(ParcelBase):
     """:class:`Enum` that holds compartment actual statuses"""
-    UNKNOWN = 'UNKNOWN DATA'
-    OPENED = 'Otwarta'
-    CLOSED = 'Zamknięta'
+
+    UNKNOWN = "UNKNOWN DATA"
+    OPENED = "Otwarta"
+    CLOSED = "Zamknięta"
+
+
+class PaymentType(ParcelBase):
+    UNKNOWN = "UNKNOWN DATA"
+    NOTSUPPORTED = "Payments are not supported"  # klucz 0
+    BY_CARD_IN_MACHINE = "Payment by card in the machine"  # klucz 2
+
+
+class PaymentStatus(ParcelBase):
+    UNKNOWN = "UNKNOWN DATA"
+    C2X_COMPLETED = "Completed"
 
 
 class ParcelServiceName(ParcelBase):
-    UNKNOWN = 'UNKNOWN DATA'
+    UNKNOWN = "UNKNOWN DATA"
     ALLEGRO_PARCEL = 1
     ALLEGRO_PARCEL_SMART = 2
     ALLEGRO_LETTER = 3
     ALLEGRO_COURIER = 4
     STANDARD = 5
     STANDARD_PARCEL_SMART = 6
     PASS_THRU = 7
```

### Comparing `inpost-0.1.3/pyproject.toml` & `inpost-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inpost"
-version = "0.1.3"
+version = "0.1.4"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
@@ -28,7 +28,32 @@
 qrcode = "^7.3.1"
 Pillow = "^9.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+  | tmp
+  | docs
+)/
+'''
+
+[tool.isort]
+line_length = 120
+multi_line_output = 3
+include_trailing_comma = true
+known_third_party = ["aiohttp", "music_service_async_interface", "mutagen"]
```

### Comparing `inpost-0.1.3/setup.py` & `inpost-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.4.0,<10.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'arrow>=1.2.3,<2.0.0',
  'qrcode>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'inpost',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app',
     'long_description': "\n# Inpost Python\n\nFully async Inpost library using Python 3.10.\n\n\n\n\n## Documentation\n\n[Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)\n\n\n## Usage/Examples\n\n\n```python\nfrom inpost.api import Inpost\n\ninp = await Inpost.from_phone_number('555333444')\nawait inp.send_sms_code():\n...\nif await inp.confirm_sms_code(123321):\n   print('Congratulations, you initialized successfully!')\n```\n\n\n## Authors\n\n- [@loboda4450](https://www.github.com/loboda4450)\n- [@mrkazik99](https://www.github.com/mrkazik99)\n\n\n## Used By\n\nThis project is used by the following repos:\n\n[Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)\n\n",
     'author': 'loboda4450',
     'author_email': 'loboda4450@gmail.com',
     'maintainer': 'loboda4450',
     'maintainer_email': 'loboda4450@gmail.com',
     'url': 'https://github.com/IFOSSA/inpost-python',
```

### Comparing `inpost-0.1.3/PKG-INFO` & `inpost-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
```

