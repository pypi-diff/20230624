# Comparing `tmp/maadstml-3.38.tar.gz` & `tmp/maadstml-3.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.38.tar", last modified: Wed Jun 21 14:24:19 2023, max compression
+gzip compressed data, was "maadstml-3.39.tar", last modified: Sat Jun 24 18:16:47 2023, max compression
```

## Comparing `maadstml-3.38.tar` & `maadstml-3.39.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 14:24:19.130799 maadstml-3.38/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.38/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.38/MANIFEST.in
--rw-rw-rw-   0        0        0   174408 2023-06-21 14:24:19.130799 maadstml-3.38/PKG-INFO
--rw-rw-rw-   0        0        0   173811 2023-06-13 18:28:52.000000 maadstml-3.38/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 14:24:19.113787 maadstml-3.38/maadstml/
--rw-rw-rw-   0        0        0     2387 2023-06-13 18:19:41.000000 maadstml-3.38/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.38/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    82738 2023-06-21 14:23:08.000000 maadstml-3.38/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.38/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:24:19.130799 maadstml-3.38/maadstml.egg-info/
--rw-rw-rw-   0        0        0   174408 2023-06-21 14:24:18.000000 maadstml-3.38/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-21 14:24:19.000000 maadstml-3.38/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 14:24:18.000000 maadstml-3.38/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      223 2023-06-21 14:24:18.000000 maadstml-3.38/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 14:24:18.000000 maadstml-3.38/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      239 2023-06-19 23:47:07.000000 maadstml-3.38/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 14:24:19.130799 maadstml-3.38/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-21 14:13:03.000000 maadstml-3.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:16:47.249958 maadstml-3.39/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.39/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.39/MANIFEST.in
+-rw-rw-rw-   0        0        0   174063 2023-06-24 18:16:47.249958 maadstml-3.39/PKG-INFO
+-rw-rw-rw-   0        0        0   173466 2023-06-24 18:13:52.000000 maadstml-3.39/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:16:47.218073 maadstml-3.39/maadstml/
+-rw-rw-rw-   0        0        0     2260 2023-06-24 18:12:51.000000 maadstml-3.39/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.39/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    81197 2023-06-24 18:12:26.000000 maadstml-3.39/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.39/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:16:47.249958 maadstml-3.39/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   174063 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-24 18:16:47.000000 maadstml-3.39/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstml-3.39/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:16:47.249958 maadstml-3.39/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-24 18:14:31.000000 maadstml-3.39/setup.py
```

### Comparing `maadstml-3.38/LICENSE.txt` & `maadstml-3.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.38/PKG-INFO` & `maadstml-3.39/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: maadstml
-Version: 3.38
-Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
-Home-page: https://github.com/smaurice101/transactionalmachinelearning
-Author: Sebastian Maurice
-Author-email: sebastian.maurice@otics.ca
-License: MIT License
-Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
-Description-Content-Type: text/markdown
-License-File: license.txt
-
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
 *MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
@@ -253,23 +241,14 @@
 
 - **viperexractpdffields**
   - Extracts fields from PDF file
 
 - **viperexractpdffieldbylabel**
   - Extracts fields from PDF file by label name.
 
-- **viperimagetotext**
-  - Extracts text from images like PNG, JPG, etc., which can then be streamed to kafka.
-
-- **viperaudiototext**
-  - Extracts text from audio files like WAV, etc., which can then be streamed to kafka.
-
-- **vipervideototext**
-  - Extracts text from video files like MP4, etc., which can then be streamed to kafka.
-
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
```

### Comparing `maadstml-3.38/README.md` & `maadstml-3.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: maadstml
+Version: 3.39
+Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
+Home-page: https://github.com/smaurice101/transactionalmachinelearning
+Author: Sebastian Maurice
+Author-email: sebastian.maurice@otics.ca
+License: MIT License
+Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
+Description-Content-Type: text/markdown
+License-File: license.txt
+
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
 *MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
@@ -241,23 +253,14 @@
 
 - **viperexractpdffields**
   - Extracts fields from PDF file
 
 - **viperexractpdffieldbylabel**
   - Extracts fields from PDF file by label name.
 
-- **viperimagetotext**
-  - Extracts text from images like PNG, JPG, etc., which can then be streamed to kafka.
-
-- **viperaudiototext**
-  - Extracts text from audio files like WAV, etc., which can then be streamed to kafka.
-
-- **vipervideototext**
-  - Extracts text from video files like MP4, etc., which can then be streamed to kafka.
-
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
```

### Comparing `maadstml-3.38/maadstml/__init__.py` & `maadstml-3.39/maadstml/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,9 @@
 
 from .sendfiles import viperchatgpt
 
 from .sendfiles import viperexractpdffields
 
 from .sendfiles import viperexractpdffieldbylabel
 
-from .sendfiles import viperimagetotext
-
-from .sendfiles import viperaudiototext
-
-from .sendfiles import vipervideototext
 
 name = "maadstml"
```

### Comparing `maadstml-3.38/maadstml/readpdf.py` & `maadstml-3.39/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.38/maadstml/sendfiles.py` & `maadstml-3.39/maadstml/sendfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -4123,1050 +4123,953 @@
 000101a0: 7475 726e 2022 456e 7465 7220 5044 4620  turn "Enter PDF 
 000101b0: 6669 6c65 6e61 6d65 2c20 6c61 6265 6c6e  filename, labeln
 000101c0: 616d 6520 616e 6420 6163 726f 7479 7065  ame and acrotype
 000101d0: 220d 0a20 2020 200d 0a20 2020 2072 6574  "..    ..    ret
 000101e0: 7572 6e20 6c61 6265 6c66 6965 6c64 7328  urn labelfields(
 000101f0: 6669 6c65 6e61 6d65 2c6c 6162 656c 6e61  filename,labelna
 00010200: 6d65 2c61 6372 6f74 7970 6529 0d0a 0d0a  me,acrotype)....
-00010210: 6465 6620 7669 7065 7269 6d61 6765 746f  def viperimageto
-00010220: 7465 7874 2866 696c 656e 616d 6529 3a0d  text(filename):.
-00010230: 0a20 2020 2069 6620 6669 6c65 6e61 6d65  .    if filename
-00010240: 3d3d 2222 3a0d 0a20 2020 2020 2020 2072  =="":..        r
-00010250: 6574 7572 6e20 2245 6e74 6572 2049 4d41  eturn "Enter IMA
-00010260: 4745 2028 706e 672c 206a 7067 2c20 6574  GE (png, jpg, et
-00010270: 632e 2920 6669 6c65 6e61 6d65 220d 0a20  c.) filename".. 
-00010280: 2020 200d 0a20 2020 2072 6574 7572 6e20     ..    return 
-00010290: 646f 6f63 726d 6169 6e28 6669 6c65 6e61  doocrmain(filena
-000102a0: 6d65 290d 0a0d 0a64 6566 2076 6970 6572  me)....def viper
-000102b0: 6175 6469 6f74 6f74 6578 7428 6669 6c65  audiototext(file
-000102c0: 6e61 6d65 293a 0d0a 2020 2020 6966 2066  name):..    if f
-000102d0: 696c 656e 616d 653d 3d22 223a 0d0a 2020  ilename=="":..  
-000102e0: 2020 2020 2020 7265 7475 726e 2022 456e        return "En
-000102f0: 7465 7220 4155 4449 4f20 4669 6c65 2028  ter AUDIO File (
-00010300: 5741 5629 2066 696c 656e 616d 6522 0d0a  WAV) filename"..
-00010310: 2020 2020 0d0a 2020 2020 7265 7475 726e      ..    return
-00010320: 2061 7564 696f 746f 7465 7874 2866 696c   audiototext(fil
-00010330: 656e 616d 6529 0d0a 0d0a 6465 6620 7669  ename)....def vi
-00010340: 7065 7276 6964 656f 746f 7465 7874 2866  pervideototext(f
-00010350: 696c 656e 616d 6529 3a0d 0a20 2020 2069  ilename):..    i
-00010360: 6620 6669 6c65 6e61 6d65 3d3d 2222 3a0d  f filename=="":.
-00010370: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010380: 2245 6e74 6572 2056 4944 454f 2046 696c  "Enter VIDEO Fil
-00010390: 6520 284d 5034 2920 6669 6c65 6e61 6d65  e (MP4) filename
-000103a0: 220d 0a20 2020 200d 0a20 2020 2072 6574  "..    ..    ret
-000103b0: 7572 6e20 636f 6e76 6572 7476 6964 656f  urn convertvideo
-000103c0: 746f 7465 7874 2866 696c 656e 616d 6529  totext(filename)
-000103d0: 0d0a 2020 2020 0d0a 6465 6620 6172 6579  ..    ..def arey
-000103e0: 6f75 6275 7379 2868 6f73 742c 706f 7274  oubusy(host,port
-000103f0: 3d2d 3939 392c 6d69 6372 6f73 6572 7669  =-999,microservi
-00010400: 6365 6964 3d27 2729 3a0d 0a20 2020 2067  ceid=''):..    g
-00010410: 6c6f 6261 6c20 636f 6e6e 6563 7469 6f6e  lobal connection
-00010420: 6572 726f 720d 0a0d 0a20 2020 2069 6620  error....    if 
-00010430: 286c 656e 2868 6f73 7429 3d3d 3020 6f72  (len(host)==0 or
-00010440: 2070 6f72 743d 3d2d 3939 3920 293a 0d0a   port==-999 ):..
-00010450: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00010460: 2250 6c65 6173 6520 656e 7465 7220 686f  "Please enter ho
-00010470: 7374 2c70 6f72 7422 0d0a 2020 2020 7661  st,port"..    va
-00010480: 6c75 653d 2822 6172 6579 6f75 6275 7379  lue=("areyoubusy
-00010490: 2229 0d0a 0d0a 2020 2020 7661 6c3d 6c6f  ")....    val=lo
-000104a0: 6f70 2e72 756e 5f75 6e74 696c 5f63 6f6d  op.run_until_com
-000104b0: 706c 6574 6528 7463 705f 6563 686f 5f63  plete(tcp_echo_c
-000104c0: 6c69 656e 7476 6970 6572 2876 616c 7565  lientviper(value
-000104d0: 2c20 6c6f 6f70 2c68 6f73 742c 706f 7274  , loop,host,port
-000104e0: 2c6d 6963 726f 7365 7276 6963 6569 6429  ,microserviceid)
-000104f0: 290d 0a20 2020 2069 6620 636f 6e6e 6563  )..    if connec
-00010500: 7469 6f6e 6572 726f 723a 0d0a 2020 2020  tionerror:..    
-00010510: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
-00010520: 6563 7469 6f6e 6572 726f 720d 0a0d 0a20  ectionerror.... 
-00010530: 2020 2072 6574 7572 6e20 7661 6c0d 0a0d     return val...
-00010540: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00010550: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010570: 2323 2323 230d 0a69 6d70 6f72 7420 7379  #####..import sy
-00010580: 730d 0a66 726f 6d20 7064 666d 696e 6572  s..from pdfminer
-00010590: 2e70 6466 7061 7273 6572 2069 6d70 6f72  .pdfparser impor
-000105a0: 7420 5044 4650 6172 7365 720d 0a66 726f  t PDFParser..fro
-000105b0: 6d20 7064 666d 696e 6572 2e70 6466 646f  m pdfminer.pdfdo
-000105c0: 6375 6d65 6e74 2069 6d70 6f72 7420 5044  cument import PD
-000105d0: 4644 6f63 756d 656e 740d 0a66 726f 6d20  FDocument..from 
-000105e0: 7064 666d 696e 6572 2e70 6466 7061 6765  pdfminer.pdfpage
-000105f0: 2069 6d70 6f72 7420 5044 4650 6167 650d   import PDFPage.
-00010600: 0a66 726f 6d20 7064 666d 696e 6572 2e70  .from pdfminer.p
-00010610: 6466 7061 6765 2069 6d70 6f72 7420 5044  dfpage import PD
-00010620: 4654 6578 7445 7874 7261 6374 696f 6e4e  FTextExtractionN
-00010630: 6f74 416c 6c6f 7765 640d 0a66 726f 6d20  otAllowed..from 
-00010640: 7064 666d 696e 6572 2e70 6466 696e 7465  pdfminer.pdfinte
-00010650: 7270 2069 6d70 6f72 7420 5044 4652 6573  rp import PDFRes
-00010660: 6f75 7263 654d 616e 6167 6572 0d0a 6672  ourceManager..fr
-00010670: 6f6d 2070 6466 6d69 6e65 722e 7064 6669  om pdfminer.pdfi
-00010680: 6e74 6572 7020 696d 706f 7274 2050 4446  nterp import PDF
-00010690: 5061 6765 496e 7465 7270 7265 7465 720d  PageInterpreter.
-000106a0: 0a23 6672 6f6d 2053 7472 696e 6749 4f20  .#from StringIO 
-000106b0: 696d 706f 7274 2053 7472 696e 6749 4f0d  import StringIO.
-000106c0: 0a66 726f 6d20 696f 2069 6d70 6f72 7420  .from io import 
-000106d0: 5374 7269 6e67 494f 0d0a 696d 706f 7274  StringIO..import
-000106e0: 2075 726c 6c69 622e 7265 7175 6573 7420   urllib.request 
-000106f0: 200d 0a23 696d 706f 7274 2074 6d6c 7465   ..#import tmlte
-00010700: 7874 7375 6d6d 6172 790d 0a69 6d70 6f72  xtsummary..impor
-00010710: 7420 6f73 0d0a 696d 706f 7274 2064 6174  t os..import dat
-00010720: 6574 696d 650d 0a23 696d 706f 7274 2067  etime..#import g
-00010730: 6c6f 620d 0a0d 0a0d 0a66 726f 6d20 7064  lob......from pd
-00010740: 666d 696e 6572 2e6c 6179 6f75 7420 696d  fminer.layout im
-00010750: 706f 7274 204c 4150 6172 616d 730d 0a66  port LAParams..f
-00010760: 726f 6d20 7064 666d 696e 6572 2e63 6f6e  rom pdfminer.con
-00010770: 7665 7274 6572 2069 6d70 6f72 7420 5465  verter import Te
-00010780: 7874 436f 6e76 6572 7465 720d 0a20 0d0a  xtConverter.. ..
-00010790: 636c 6173 7320 4d79 5061 7273 6572 286f  class MyParser(o
-000107a0: 626a 6563 7429 3a0d 0a20 2020 2064 6566  bject):..    def
-000107b0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-000107c0: 7064 6629 3a0d 0a20 2020 2020 2020 2023  pdf):..        #
-000107d0: 2320 536e 6970 7065 6420 6164 6170 7465  # Snipped adapte
-000107e0: 6420 6672 6f6d 2059 7573 756b 6520 5368  d from Yusuke Sh
-000107f0: 696e 7961 6d61 7320 0d0a 2020 2020 2020  inyamas ..      
-00010800: 2020 2350 4446 4d69 6e65 7220 646f 6375    #PDFMiner docu
-00010810: 6d65 6e74 6174 696f 6e0d 0a20 2020 2020  mentation..     
-00010820: 2020 2023 2043 7265 6174 6520 7468 6520     # Create the 
-00010830: 646f 6375 6d65 6e74 206d 6f64 656c 2066  document model f
-00010840: 726f 6d20 7468 6520 6669 6c65 0d0a 2020  rom the file..  
-00010850: 2020 2020 2020 7061 7273 6572 203d 2050        parser = P
-00010860: 4446 5061 7273 6572 286f 7065 6e28 7064  DFParser(open(pd
-00010870: 662c 2027 7262 2729 290d 0a20 2020 2020  f, 'rb'))..     
-00010880: 2020 2064 6f63 756d 656e 7420 3d20 5044     document = PD
-00010890: 4644 6f63 756d 656e 7428 7061 7273 6572  FDocument(parser
-000108a0: 290d 0a20 2020 2020 2020 2023 2054 7279  )..        # Try
-000108b0: 2074 6f20 7061 7273 6520 7468 6520 646f   to parse the do
-000108c0: 6375 6d65 6e74 0d0a 2020 2020 2020 2020  cument..        
-000108d0: 6966 206e 6f74 2064 6f63 756d 656e 742e  if not document.
-000108e0: 6973 5f65 7874 7261 6374 6162 6c65 3a0d  is_extractable:.
-000108f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00010900: 7365 2050 4446 5465 7874 4578 7472 6163  se PDFTextExtrac
-00010910: 7469 6f6e 4e6f 7441 6c6c 6f77 6564 0d0a  tionNotAllowed..
-00010920: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-00010930: 2061 2050 4446 2072 6573 6f75 7263 6520   a PDF resource 
-00010940: 6d61 6e61 6765 7220 6f62 6a65 6374 200d  manager object .
-00010950: 0a20 2020 2020 2020 2023 2074 6861 7420  .        # that 
-00010960: 7374 6f72 6573 2073 6861 7265 6420 7265  stores shared re
-00010970: 736f 7572 6365 732e 0d0a 2020 2020 2020  sources...      
-00010980: 2020 7273 7263 6d67 7220 3d20 5044 4652    rsrcmgr = PDFR
-00010990: 6573 6f75 7263 654d 616e 6167 6572 2829  esourceManager()
-000109a0: 0d0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
-000109b0: 7465 2061 2062 7566 6665 7220 666f 7220  te a buffer for 
-000109c0: 7468 6520 7061 7273 6564 2074 6578 740d  the parsed text.
-000109d0: 0a20 2020 2020 2020 2072 6574 7374 7220  .        retstr 
-000109e0: 3d20 5374 7269 6e67 494f 2829 0d0a 2020  = StringIO()..  
-000109f0: 2020 2020 2020 2320 5370 6163 696e 6720        # Spacing 
-00010a00: 7061 7261 6d65 7465 7273 2066 6f72 2070  parameters for p
-00010a10: 6172 7369 6e67 0d0a 2020 2020 2020 2020  arsing..        
-00010a20: 6c61 7061 7261 6d73 203d 204c 4150 6172  laparams = LAPar
-00010a30: 616d 7328 290d 0a20 2020 2020 2020 2063  ams()..        c
-00010a40: 6f64 6563 203d 2027 7574 662d 3827 0d0a  odec = 'utf-8'..
-00010a50: 200d 0a20 2020 2020 2020 2023 2043 7265   ..        # Cre
-00010a60: 6174 6520 6120 5044 4620 6465 7669 6365  ate a PDF device
-00010a70: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
-00010a80: 2064 6576 6963 6520 3d20 5465 7874 436f   device = TextCo
-00010a90: 6e76 6572 7465 7228 7273 7263 6d67 722c  nverter(rsrcmgr,
-00010aa0: 2072 6574 7374 722c 0d0a 2020 2020 2020   retstr,..      
-00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 2020 2020 2020 206c 6170 6172 616d           laparam
-00010ad0: 7320 3d20 6c61 7061 7261 6d73 290d 0a20  s = laparams).. 
-00010ae0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-00010af0: 6120 5044 4620 696e 7465 7270 7265 7465  a PDF interprete
-00010b00: 7220 6f62 6a65 6374 0d0a 2020 2020 2020  r object..      
-00010b10: 2020 696e 7465 7270 7265 7465 7220 3d20    interpreter = 
-00010b20: 5044 4650 6167 6549 6e74 6572 7072 6574  PDFPageInterpret
-00010b30: 6572 2872 7372 636d 6772 2c20 6465 7669  er(rsrcmgr, devi
-00010b40: 6365 290d 0a20 2020 2020 2020 2023 2050  ce)..        # P
-00010b50: 726f 6365 7373 2065 6163 6820 7061 6765  rocess each page
-00010b60: 2063 6f6e 7461 696e 6564 2069 6e20 7468   contained in th
-00010b70: 6520 646f 6375 6d65 6e74 2e0d 0a20 2020  e document...   
-00010b80: 2020 2020 2066 6f72 2070 6167 6520 696e       for page in
-00010b90: 2050 4446 5061 6765 2e63 7265 6174 655f   PDFPage.create_
-00010ba0: 7061 6765 7328 646f 6375 6d65 6e74 293a  pages(document):
-00010bb0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00010bc0: 7465 7270 7265 7465 722e 7072 6f63 6573  terpreter.proces
-00010bd0: 735f 7061 6765 2870 6167 6529 0d0a 2020  s_page(page)..  
-00010be0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010bf0: 2073 656c 662e 7265 636f 7264 7320 2020   self.records   
-00010c00: 2020 2020 2020 2020 203d 205b 5d0d 0a20           = [].. 
-00010c10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00010c20: 2020 6c69 6e65 7320 3d20 7265 7473 7472    lines = retstr
-00010c30: 2e67 6574 7661 6c75 6528 292e 7370 6c69  .getvalue().spli
-00010c40: 746c 696e 6573 2829 0d0a 2020 2020 2020  tlines()..      
-00010c50: 2020 666f 7220 6c69 6e65 2069 6e20 6c69    for line in li
-00010c60: 6e65 733a 0d0a 2020 2020 2020 2020 2020  nes:..          
-00010c70: 2020 7365 6c66 2e68 616e 646c 655f 6c69    self.handle_li
-00010c80: 6e65 286c 696e 6529 0d0a 2020 2020 200d  ne(line)..     .
-00010c90: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-00010ca0: 6c69 6e65 2873 656c 662c 206c 696e 6529  line(self, line)
-00010cb0: 3a0d 0a20 2020 2020 2020 2023 2043 7573  :..        # Cus
-00010cc0: 746f 6d69 7a65 2079 6f75 7220 6c69 6e65  tomize your line
-00010cd0: 2d62 792d 6c69 6e65 2070 6172 7365 7220  -by-line parser 
-00010ce0: 6865 7265 0d0a 2020 2020 2020 2020 7365  here..        se
-00010cf0: 6c66 2e72 6563 6f72 6473 2e61 7070 656e  lf.records.appen
-00010d00: 6428 6c69 6e65 290d 0a0d 0a64 6566 2073  d(line)....def s
-00010d10: 6372 6170 6570 6466 2874 6865 7572 6c2c  crapepdf(theurl,
-00010d20: 666e 293a 0d0a 2020 2020 7363 7261 7065  fn):..    scrape
-00010d30: 645f 6461 7461 203d 2075 726c 6c69 622e  d_data = urllib.
-00010d40: 7265 7175 6573 742e 7572 6c6f 7065 6e28  request.urlopen(
-00010d50: 7468 6575 726c 2920 200d 0a20 2020 2066  theurl)  ..    f
-00010d60: 696c 6520 3d20 6f70 656e 2866 6e2c 2027  ile = open(fn, '
-00010d70: 7762 2729 0d0a 2020 2020 6669 6c65 2e77  wb')..    file.w
-00010d80: 7269 7465 2873 6372 6170 6564 5f64 6174  rite(scraped_dat
-00010d90: 612e 7265 6164 2829 290d 0a20 2020 2066  a.read())..    f
-00010da0: 696c 652e 636c 6f73 6528 290d 0a20 2020  ile.close()..   
-00010db0: 2023 7265 7475 726e 2061 7274 6963 6c65   #return article
-00010dc0: 5f74 6578 740d 0a0d 0a64 6566 2073 7461  _text....def sta
-00010dd0: 7274 7064 6672 6561 6469 6e67 2866 696c  rtpdfreading(fil
-00010de0: 656e 616d 652c 6676 616c 7565 2c6b 6579  ename,fvalue,key
-00010df0: 636f 756e 7429 3a0d 0a20 2023 6f73 2e70  count):..  #os.p
-00010e00: 6174 682e 6162 7370 6174 6828 6f73 2e67  ath.abspath(os.g
-00010e10: 6574 6377 6428 2929 0d0a 2020 7468 6573  etcwd())..  thes
-00010e20: 697a 653d 726f 756e 6428 6f73 2e70 6174  ize=round(os.pat
-00010e30: 682e 6765 7473 697a 6528 6669 6c65 6e61  h.getsize(filena
-00010e40: 6d65 292f 3130 3030 3030 302c 3229 0d0a  me)/1000000,2)..
-00010e50: 2020 6d5f 7469 6d65 203d 206f 732e 7061    m_time = os.pa
-00010e60: 7468 2e67 6574 6d74 696d 6528 6669 6c65  th.getmtime(file
-00010e70: 6e61 6d65 290d 0a20 2064 745f 6d20 3d20  name)..  dt_m = 
-00010e80: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00010e90: 652e 6672 6f6d 7469 6d65 7374 616d 7028  e.fromtimestamp(
-00010ea0: 6d5f 7469 6d65 290d 0a20 2063 5f74 696d  m_time)..  c_tim
-00010eb0: 6520 3d20 6f73 2e70 6174 682e 6765 7463  e = os.path.getc
-00010ec0: 7469 6d65 2866 696c 656e 616d 6529 0d0a  time(filename)..
-00010ed0: 2020 2320 636f 6e76 6572 7420 6372 6561    # convert crea
-00010ee0: 7469 6f6e 2074 696d 6573 7461 6d70 2069  tion timestamp i
-00010ef0: 6e74 6f20 4461 7465 5469 6d65 206f 626a  nto DateTime obj
-00010f00: 6563 740d 0a20 2064 745f 6320 3d20 6461  ect..  dt_c = da
-00010f10: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-00010f20: 6672 6f6d 7469 6d65 7374 616d 7028 635f  fromtimestamp(c_
-00010f30: 7469 6d65 290d 0a20 2063 6f20 3d20 7374  time)..  co = st
-00010f40: 7228 6474 5f63 2920 5b30 3a31 395d 0d0a  r(dt_c) [0:19]..
-00010f50: 2020 6d6f 203d 2073 7472 2864 745f 6d29    mo = str(dt_m)
-00010f60: 205b 303a 3139 5d0d 0a0d 0a20 2070 203d   [0:19]....  p =
-00010f70: 204d 7950 6172 7365 7228 6669 6c65 6e61   MyParser(filena
-00010f80: 6d65 290d 0a20 2074 6865 7465 7874 3d27  me)..  thetext='
-00010f90: 5c6e 272e 6a6f 696e 2870 2e72 6563 6f72  \n'.join(p.recor
-00010fa0: 6473 290d 0a20 2061 7274 6963 6c65 5f74  ds)..  article_t
-00010fb0: 6578 743d 7468 6574 6578 742e 656e 636f  ext=thetext.enco
-00010fc0: 6465 2827 7574 6638 2729 0d0a 2020 7375  de('utf8')..  su
-00010fd0: 6d6d 6172 697a 6564 3d22 7b5c 2266 696c  mmarized="{\"fil
-00010fe0: 656e 616d 655c 223a 5c22 2220 2b20 6669  ename\":\"" + fi
-00010ff0: 6c65 6e61 6d65 202b 2022 5c22 2c5c 2266  lename + "\",\"f
-00011000: 696c 6573 697a 6528 4d42 295c 223a 222b  ilesize(MB)\":"+
-00011010: 7374 7228 7468 6573 697a 6529 2b22 2c5c  str(thesize)+",\
-00011020: 2266 696c 6563 7265 6174 6564 6f6e 5c22  "filecreatedon\"
-00011030: 3a5c 2222 202b 2063 6f20 2b20 225c 222c  :\"" + co + "\",
-00011040: 5c22 6669 6c65 6d6f 6469 6669 6564 6f6e  \"filemodifiedon
-00011050: 5c22 3a5c 2222 202b 206d 6f20 2b20 225c  \":\"" + mo + "\
-00011060: 222c 5c22 6b65 7977 6f72 6473 5c22 3a22  ",\"keywords\":"
-00011070: 202b 2020 7374 6172 7473 756d 6d61 7279   +  startsummary
-00011080: 2874 6865 7465 7874 2c66 7661 6c75 652c  (thetext,fvalue,
-00011090: 6b65 7963 6f75 6e74 290d 0a20 2320 7072  keycount).. # pr
-000110a0: 696e 7428 7375 6d6d 6172 697a 6564 290d  int(summarized).
-000110b0: 0a20 2072 6574 7572 6e20 7375 6d6d 6172  .  return summar
-000110c0: 697a 6564 0d0a 0d0a 0d0a 2323 2323 2323  ized......######
-000110d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000110e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000110f0: 2323 2323 2323 2323 230d 0a23 2044 6576  #########..# Dev
-00011100: 656c 6f70 6564 2062 7920 4f54 4943 5320  eloped by OTICS 
-00011110: 4164 7661 6e63 6564 2041 6e61 6c79 7469  Advanced Analyti
-00011120: 6373 0d0a 2320 5365 6261 7374 6961 6e20  cs..# Sebastian 
-00011130: 4d61 7572 6963 650d 0a0d 0a69 6d70 6f72  Maurice....impor
-00011140: 7420 6273 3420 6173 2062 7320 200d 0a69  t bs4 as bs  ..i
-00011150: 6d70 6f72 7420 7572 6c6c 6962 2e72 6571  mport urllib.req
-00011160: 7565 7374 2020 0d0a 696d 706f 7274 2072  uest  ..import r
-00011170: 650d 0a69 6d70 6f72 7420 6e6c 746b 0d0a  e..import nltk..
-00011180: 6672 6f6d 206e 6c74 6b2e 746f 6b65 6e69  from nltk.tokeni
-00011190: 7a65 2069 6d70 6f72 7420 5265 6765 7870  ze import Regexp
-000111a0: 546f 6b65 6e69 7a65 720d 0a69 6d70 6f72  Tokenizer..impor
-000111b0: 7420 6865 6170 710d 0a69 6d70 6f72 7420  t heapq..import 
-000111c0: 7379 730d 0a69 6d70 6f72 7420 6f73 0d0a  sys..import os..
-000111d0: 6672 6f6d 2072 616b 655f 6e6c 746b 2069  from rake_nltk i
-000111e0: 6d70 6f72 7420 4d65 7472 6963 2c52 616b  mport Metric,Rak
-000111f0: 650d 0a69 6d70 6f72 7420 6a73 6f6e 0d0a  e..import json..
-00011200: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-00011210: 2070 640d 0a69 6d70 6f72 7420 6e6c 746b   pd..import nltk
-00011220: 2e63 6f72 7075 730d 0a66 726f 6d20 6e6c  .corpus..from nl
-00011230: 746b 2e63 6f72 7075 7320 696d 706f 7274  tk.corpus import
-00011240: 2073 746f 7077 6f72 6473 0d0a 6672 6f6d   stopwords..from
-00011250: 2074 6578 7462 6c6f 6220 696d 706f 7274   textblob import
-00011260: 2054 6578 7442 6c6f 620d 0a66 726f 6d20   TextBlob..from 
-00011270: 7465 7874 626c 6f62 2069 6d70 6f72 7420  textblob import 
-00011280: 576f 7264 0d0a 6672 6f6d 2073 6b6c 6561  Word..from sklea
-00011290: 726e 2e66 6561 7475 7265 5f65 7874 7261  rn.feature_extra
-000112a0: 6374 696f 6e2e 7465 7874 2069 6d70 6f72  ction.text impor
-000112b0: 7420 5466 6964 6654 7261 6e73 666f 726d  t TfidfTransform
-000112c0: 6572 2c54 6669 6466 5665 6374 6f72 697a  er,TfidfVectoriz
-000112d0: 6572 0d0a 6672 6f6d 2073 6b6c 6561 726e  er..from sklearn
-000112e0: 2e66 6561 7475 7265 5f65 7874 7261 6374  .feature_extract
-000112f0: 696f 6e2e 7465 7874 2069 6d70 6f72 7420  ion.text import 
-00011300: 436f 756e 7456 6563 746f 7269 7a65 720d  CountVectorizer.
-00011310: 0a23 6e6c 746b 2e64 6f77 6e6c 6f61 6428  .#nltk.download(
-00011320: 2770 756e 6b74 2729 0d0a 696d 706f 7274  'punkt')..import
-00011330: 2077 6172 6e69 6e67 730d 0a77 6172 6e69   warnings..warni
-00011340: 6e67 732e 6669 6c74 6572 7761 726e 696e  ngs.filterwarnin
-00011350: 6773 2822 6967 6e6f 7265 2229 0d0a 0d0a  gs("ignore")....
-00011360: 236e 6c74 6b2e 646f 776e 6c6f 6164 2827  #nltk.download('
-00011370: 7374 6f70 776f 7264 7327 290d 0a0d 0a64  stopwords')....d
-00011380: 6566 2067 6574 5f73 746f 705f 776f 7264  ef get_stop_word
-00011390: 7328 293a 0d0a 2020 2020 2222 226c 6f61  s():..    """loa
-000113a0: 6420 7374 6f70 2077 6f72 6473 2022 2222  d stop words """
-000113b0: 0d0a 2020 2020 7374 7077 7264 203d 2020  ..    stpwrd =  
-000113c0: 7374 6f70 776f 7264 732e 776f 7264 7328  stopwords.words(
-000113d0: 2765 6e67 6c69 7368 2729 0d0a 2020 2020  'english')..    
-000113e0: 6e65 775f 7374 6f70 776f 7264 7320 3d20  new_stopwords = 
-000113f0: 5b22 6e65 6564 222c 2022 756e 666f 7274  ["need", "unfort
-00011400: 756e 6174 656c 7922 2c20 2274 6f22 2c20  unately", "to", 
-00011410: 226f 6e22 2c20 2264 6169 6c79 222c 2022  "on", "daily", "
-00011420: 7461 6b65 222c 0d0a 2020 2020 2020 2020  take",..        
-00011430: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
-00011440: 6b65 6e22 2c22 6164 6472 6573 7369 6e67  ken","addressing
-00011450: 222c 2273 6f6f 6e65 7222 2c22 7261 7468  ","sooner","rath
-00011460: 6572 222c 226d 616b 6522 2c22 6c61 7465  er","make","late
-00011470: 7222 2c0d 0a20 2020 2020 2020 2020 2020  r",..           
-00011480: 2020 2020 2020 2020 2020 2273 6f6f 6e65            "soone
-00011490: 7222 2c22 7375 6d6d 6172 7922 2c22 6c65  r","summary","le
-000114a0: 6176 6522 2c22 6576 6572 7922 2c22 696e  ave","every","in
-000114b0: 7465 6e64 222c 2266 696e 616c 6c79 222c  tend","finally",
-000114c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000114d0: 2020 2020 2020 2022 656e 7469 7265 6c79         "entirely
-000114e0: 222c 2265 7665 6e22 2c22 656e 7375 7265  ","even","ensure
-000114f0: 222c 2261 6c73 6f22 2c22 6166 6665 6374  ","also","affect
-00011500: 222c 2261 6666 6563 7469 6e67 222c 0d0a  ","affecting",..
-00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011520: 2020 2020 2022 6275 7369 6e65 7373 222c       "business",
-00011530: 2263 6c61 7373 222c 2263 6f6d 7061 6e79  "class","company
-00011540: 222c 2261 6c73 6f22 2c22 7965 6172 222c  ","also","year",
-00011550: 2275 7369 6e67 222c 0d0a 2020 2020 2020  "using",..      
-00011560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011570: 6973 7375 6564 222c 2273 7065 6369 6669  issued","specifi
-00011580: 6322 2c22 7370 6563 6966 6963 616c 6c79  c","specifically
-00011590: 222c 2272 6561 736f 6e22 2c22 7265 616c  ","reason","real
-000115a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000115b0: 2020 2020 2020 2020 2022 7072 6f6a 6563           "projec
-000115c0: 7422 2c22 7061 7274 6963 756c 6172 6c79  t","particularly
-000115d0: 222c 2270 6172 7469 6375 6c61 7222 2c22  ","particular","
-000115e0: 6d61 7474 6572 222c 226d 6169 6e22 2c0d  matter","main",.
-000115f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011600: 2020 2020 2020 226c 6973 7465 6422 2c22        "listed","
-00011610: 636f 6d65 222c 2263 6f6d 7061 6e79 222c  come","company",
-00011620: 2263 6f75 6c64 222c 2263 6f70 7922 2c22  "could","copy","
-00011630: 6669 7273 7422 2c22 6578 616d 706c 6522  first","example"
-00011640: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00011650: 2020 2020 2020 2020 2272 6561 6c22 2c22          "real","
-00011660: 6661 6374 6f72 222c 2277 656c 6c22 2c22  factor","well","
-00011670: 736f 7274 222c 2273 6f63 6961 6c22 2c22  sort","social","
-00011680: 736f 6369 616c 6c79 222c 2274 6872 6f75  socially","throu
-00011690: 6768 6f75 7422 2c0d 0a20 2020 2020 2020  ghout",..       
-000116a0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000116b0: 6561 736f 6e22 2c22 6176 6169 6c61 626c  eason","availabl
-000116c0: 6522 2c22 6170 7072 6f61 6368 222c 2276  e","approach","v
-000116d0: 6172 7922 2c22 7479 7065 222c 2261 6372  ary","type","acr
-000116e0: 6f73 7322 2c0d 0a20 2020 2020 2020 2020  oss",..         
-000116f0: 2020 2020 2020 2020 2020 2020 2261 7661              "ava
-00011700: 696c 6162 6c65 222c 2265 7175 616c 6c79  ilable","equally
-00011710: 222c 226d 616e 6167 6572 222c 2264 6566  ","manager","def
-00011720: 696e 6974 696f 6e22 2c22 7368 6f72 7422  inition","short"
-00011730: 2c22 7265 7370 6f6e 7365 222c 0d0a 2020  ,"response",..  
-00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011750: 2020 2022 7061 6e65 6c22 2c22 7265 7175     "panel","requ
-00011760: 6972 6573 222c 2272 6571 7569 7269 6e67  ires","requiring
-00011770: 222c 2272 6169 7365 222c 2273 686f 7722  ","raise","show"
-00011780: 2c22 646f 6e65 222c 2261 6465 7175 6174  ,"done","adequat
-00011790: 656c 7922 2c0d 0a20 2020 2020 2020 2020  ely",..         
-000117a0: 2020 2020 2020 2020 2020 2020 2267 656e              "gen
-000117b0: 6572 6963 222c 2267 656e 6572 616c 222c  eric","general",
-000117c0: 2263 6f75 7273 6522 2c22 6170 706c 6965  "course","applie
-000117d0: 6422 2c22 7265 6c61 7465 6422 5d0d 0a20  d","related"].. 
-000117e0: 2020 2073 7470 7772 642e 6578 7465 6e64     stpwrd.extend
-000117f0: 286e 6577 5f73 746f 7077 6f72 6473 290d  (new_stopwords).
-00011800: 0a20 2020 2072 6574 7572 6e20 7374 7077  .    return stpw
-00011810: 7264 0d0a 2020 0d0a 0d0a 2020 2020 0d0a  rd..  ....    ..
-00011820: 2323 2020 2020 7769 7468 206f 7065 6e28  ##    with open(
-00011830: 2773 746f 7077 6f72 6473 2e74 7874 272c  'stopwords.txt',
-00011840: 2027 7227 2c20 656e 636f 6469 6e67 3d22   'r', encoding="
-00011850: 7574 662d 3822 2920 6173 2066 3a0d 0a23  utf-8") as f:..#
-00011860: 2320 2020 2020 2020 2073 746f 7077 6f72  #        stopwor
-00011870: 6473 203d 2066 2e72 6561 646c 696e 6573  ds = f.readlines
-00011880: 2829 0d0a 2323 2020 2020 2020 2020 7374  ()..##        st
-00011890: 6f70 5f73 6574 203d 2073 6574 286d 2e73  op_set = set(m.s
-000118a0: 7472 6970 2829 2066 6f72 206d 2069 6e20  trip() for m in 
-000118b0: 7374 6f70 776f 7264 7329 0d0a 2323 2020  stopwords)..##  
-000118c0: 2020 2020 2320 2070 7269 6e74 2866 726f      #  print(fro
-000118d0: 7a65 6e73 6574 2873 746f 705f 7365 7429  zenset(stop_set)
-000118e0: 290d 0a23 2320 2020 2020 2020 2072 6574  )..##        ret
-000118f0: 7572 6e20 6672 6f7a 656e 7365 7428 7374  urn frozenset(st
-00011900: 6f70 5f73 6574 290d 0a0d 0a64 6566 2073  op_set)....def s
-00011910: 6372 6170 6577 6562 2874 6865 7572 6c29  crapeweb(theurl)
-00011920: 3a0d 0a20 2020 2073 6372 6170 6564 5f64  :..    scraped_d
-00011930: 6174 6120 3d20 7572 6c6c 6962 2e72 6571  ata = urllib.req
-00011940: 7565 7374 2e75 726c 6f70 656e 2874 6865  uest.urlopen(the
-00011950: 7572 6c29 2020 0d0a 2020 2020 6172 7469  url)  ..    arti
-00011960: 636c 6520 3d20 7363 7261 7065 645f 6461  cle = scraped_da
-00011970: 7461 2e72 6561 6428 290d 0a0d 0a20 2020  ta.read()....   
-00011980: 2070 6172 7365 645f 6172 7469 636c 6520   parsed_article 
-00011990: 3d20 6273 2e42 6561 7574 6966 756c 536f  = bs.BeautifulSo
-000119a0: 7570 2861 7274 6963 6c65 2c27 6c78 6d6c  up(article,'lxml
-000119b0: 2729 0d0a 0d0a 2020 2020 7061 7261 6772  ')....    paragr
-000119c0: 6170 6873 203d 2070 6172 7365 645f 6172  aphs = parsed_ar
-000119d0: 7469 636c 652e 6669 6e64 5f61 6c6c 2827  ticle.find_all('
-000119e0: 7027 290d 0a0d 0a20 2020 2061 7274 6963  p')....    artic
-000119f0: 6c65 5f74 6578 7420 3d20 2222 0d0a 0d0a  le_text = ""....
-00011a00: 2020 2020 666f 7220 7020 696e 2070 6172      for p in par
-00011a10: 6167 7261 7068 733a 2020 0d0a 2020 2020  agraphs:  ..    
-00011a20: 2020 2020 6172 7469 636c 655f 7465 7874      article_text
-00011a30: 202b 3d20 702e 7465 7874 0d0a 2020 2020   += p.text..    
-00011a40: 7265 7475 726e 2061 7274 6963 6c65 5f74  return article_t
-00011a50: 6578 7420 0d0a 0d0a 6465 6620 636f 6e76  ext ....def conv
-00011a60: 6572 7474 6f6c 6f77 6572 6361 7365 2864  erttolowercase(d
-00011a70: 662c 636f 6c29 3a0d 0a20 2020 2020 2064  f,col):..      d
-00011a80: 665b 636f 6c5d 203d 2064 665b 636f 6c5d  f[col] = df[col]
-00011a90: 2e61 7070 6c79 286c 616d 6264 6120 783a  .apply(lambda x:
-00011aa0: 2022 2022 2e6a 6f69 6e28 782e 6c6f 7765   " ".join(x.lowe
-00011ab0: 7228 2920 666f 7220 7820 696e 2078 2e73  r() for x in x.s
-00011ac0: 706c 6974 2829 2929 0d0a 2020 2020 2020  plit()))..      
-00011ad0: 7265 7475 726e 2064 660d 0a20 2020 200d  return df..    .
-00011ae0: 0a64 6566 2072 656d 6f76 6570 756e 6374  .def removepunct
-00011af0: 7561 7469 6f6e 2864 662c 636f 6c29 3a0d  uation(df,col):.
-00011b00: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
-00011b10: 2064 665b 636f 6c5d 2e73 7472 2e72 6570   df[col].str.rep
-00011b20: 6c61 6365 2827 5b5e 5c77 5c73 5d27 2c27  lace('[^\w\s]','
-00011b30: 2729 0d0a 2020 2020 2020 7265 7475 726e  ')..      return
-00011b40: 2064 660d 0a0d 0a64 6566 2072 656d 6f76   df....def remov
-00011b50: 6573 746f 7077 6f72 6473 2864 662c 636f  estopwords(df,co
-00011b60: 6c29 3a0d 0a20 2020 2020 2073 746f 7020  l):..      stop 
-00011b70: 3d20 7374 6f70 776f 7264 732e 776f 7264  = stopwords.word
-00011b80: 7328 2765 6e67 6c69 7368 2729 0d0a 2020  s('english')..  
-00011b90: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
-00011ba0: 5b63 6f6c 5d2e 6170 706c 7928 6c61 6d62  [col].apply(lamb
-00011bb0: 6461 2078 3a20 2220 222e 6a6f 696e 2878  da x: " ".join(x
-00011bc0: 2066 6f72 2078 2069 6e20 782e 7370 6c69   for x in x.spli
-00011bd0: 7428 2920 6966 2078 206e 6f74 2069 6e20  t() if x not in 
-00011be0: 7374 6f70 2929 0d0a 2020 2020 2020 7265  stop))..      re
-00011bf0: 7475 726e 2064 660d 0a0d 0a64 6566 2072  turn df....def r
-00011c00: 656d 6f76 6563 6f6d 6d6f 6e77 6f72 6473  emovecommonwords
-00011c10: 2864 662c 636f 6c29 3a0d 0a20 2020 2020  (df,col):..     
-00011c20: 2066 7265 7120 3d20 7064 2e53 6572 6965   freq = pd.Serie
-00011c30: 7328 2720 272e 6a6f 696e 2864 665b 636f  s(' '.join(df[co
-00011c40: 6c5d 292e 7370 6c69 7428 2929 2e76 616c  l]).split()).val
-00011c50: 7565 5f63 6f75 6e74 7328 295b 3a31 305d  ue_counts()[:10]
-00011c60: 0d0a 2020 2020 2020 6672 6571 203d 206c  ..      freq = l
-00011c70: 6973 7428 6672 6571 2e69 6e64 6578 290d  ist(freq.index).
-00011c80: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
-00011c90: 2064 665b 636f 6c5d 2e61 7070 6c79 286c   df[col].apply(l
-00011ca0: 616d 6264 6120 783a 2022 2022 2e6a 6f69  ambda x: " ".joi
-00011cb0: 6e28 7820 666f 7220 7820 696e 2078 2e73  n(x for x in x.s
-00011cc0: 706c 6974 2829 2069 6620 7820 6e6f 7420  plit() if x not 
-00011cd0: 696e 2066 7265 7129 290d 0a20 2020 2020  in freq))..     
-00011ce0: 2072 6574 7572 6e20 6466 0d0a 0d0a 6465   return df....de
-00011cf0: 6620 7265 6d6f 7665 7261 7265 776f 7264  f removerareword
-00011d00: 7328 6466 2c63 6f6c 293a 0d0a 2020 2020  s(df,col):..    
-00011d10: 2020 6672 6571 203d 2070 642e 5365 7269    freq = pd.Seri
-00011d20: 6573 2827 2027 2e6a 6f69 6e28 6466 5b63  es(' '.join(df[c
-00011d30: 6f6c 5d29 2e73 706c 6974 2829 292e 7661  ol]).split()).va
-00011d40: 6c75 655f 636f 756e 7473 2829 5b2d 3130  lue_counts()[-10
-00011d50: 3a5d 0d0a 2020 2020 2020 6672 6571 203d  :]..      freq =
-00011d60: 206c 6973 7428 6672 6571 2e69 6e64 6578   list(freq.index
-00011d70: 290d 0a20 2020 2020 2064 665b 636f 6c5d  )..      df[col]
-00011d80: 203d 2064 665b 636f 6c5d 2e61 7070 6c79   = df[col].apply
-00011d90: 286c 616d 6264 6120 783a 2022 2022 2e6a  (lambda x: " ".j
-00011da0: 6f69 6e28 7820 666f 7220 7820 696e 2078  oin(x for x in x
-00011db0: 2e73 706c 6974 2829 2069 6620 7820 6e6f  .split() if x no
-00011dc0: 7420 696e 2066 7265 7129 290d 0a20 2020  t in freq))..   
-00011dd0: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
-00011de0: 6465 6620 636f 7272 6563 7473 7065 6c6c  def correctspell
-00011df0: 696e 6728 6466 2c63 6f6c 293a 0d0a 2020  ing(df,col):..  
-00011e00: 2020 2020 6466 5b63 6f6c 5d5b 3a35 5d2e      df[col][:5].
-00011e10: 6170 706c 7928 6c61 6d62 6461 2078 3a20  apply(lambda x: 
-00011e20: 7374 7228 5465 7874 426c 6f62 2878 292e  str(TextBlob(x).
-00011e30: 636f 7272 6563 7428 2929 290d 0a20 2020  correct()))..   
-00011e40: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
-00011e50: 6465 6620 6c65 6d6d 6174 697a 6174 696f  def lemmatizatio
-00011e60: 6e28 6466 2c63 6f6c 293a 0d0a 2020 2020  n(df,col):..    
-00011e70: 2020 6466 5b63 6f6c 5d20 3d20 6466 5b63    df[col] = df[c
-00011e80: 6f6c 5d2e 6170 706c 7928 6c61 6d62 6461  ol].apply(lambda
-00011e90: 2078 3a20 2220 222e 6a6f 696e 285b 576f   x: " ".join([Wo
-00011ea0: 7264 2877 6f72 6429 2e6c 656d 6d61 7469  rd(word).lemmati
-00011eb0: 7a65 2829 2066 6f72 2077 6f72 6420 696e  ze() for word in
-00011ec0: 2078 2e73 706c 6974 2829 5d29 290d 0a20   x.split()])).. 
-00011ed0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
-00011ee0: 0d0a 6465 6620 7472 6169 6e76 6563 7428  ..def trainvect(
-00011ef0: 6376 2c74 626f 772c 6466 2c63 6f6c 2c6d  cv,tbow,df,col,m
-00011f00: 6178 6b65 7977 6f72 6473 293a 0d0a 2020  axkeywords):..  
-00011f10: 2020 2020 7465 7874 3d64 665b 636f 6c5d      text=df[col]
-00011f20: 2e74 6f6c 6973 7428 290d 0a20 2020 2020  .tolist()..     
-00011f30: 2074 6669 6466 203d 2054 6669 6466 5472   tfidf = TfidfTr
-00011f40: 616e 7366 6f72 6d65 7228 736d 6f6f 7468  ansformer(smooth
-00011f50: 5f69 6466 3d54 7275 652c 7573 655f 6964  _idf=True,use_id
-00011f60: 663d 5472 7565 290d 0a20 2020 2020 2074  f=True)..      t
-00011f70: 6669 6466 2e66 6974 2874 626f 7729 0d0a  fidf.fit(tbow)..
-00011f80: 2020 2020 2020 7466 5f69 6466 5f76 6563        tf_idf_vec
-00011f90: 746f 723d 7466 6964 662e 7472 616e 7366  tor=tfidf.transf
-00011fa0: 6f72 6d28 6376 2e74 7261 6e73 666f 726d  orm(cv.transform
-00011fb0: 2874 6578 7429 290d 0a20 2020 2020 2073  (text))..      s
-00011fc0: 6f72 7465 6469 7465 6d73 3d73 6f72 745f  orteditems=sort_
-00011fd0: 636f 6f28 7466 5f69 6466 5f76 6563 746f  coo(tf_idf_vecto
-00011fe0: 722e 746f 636f 6f28 2929 0d0a 2020 2020  r.tocoo())..    
-00011ff0: 2020 6665 6174 7572 656e 616d 6573 3d63    featurenames=c
-00012000: 762e 6765 745f 6665 6174 7572 655f 6e61  v.get_feature_na
-00012010: 6d65 735f 6f75 7428 290d 0a20 2020 2020  mes_out()..     
-00012020: 206b 6579 776f 7264 733d 6578 7472 6163   keywords=extrac
-00012030: 745f 746f 706e 5f66 726f 6d5f 7665 6374  t_topn_from_vect
-00012040: 6f72 2866 6561 7475 7265 6e61 6d65 732c  or(featurenames,
-00012050: 736f 7274 6564 6974 656d 732c 6d61 786b  sorteditems,maxk
-00012060: 6579 776f 7264 7329 0d0a 2020 2020 2020  eywords)..      
-00012070: 6b65 7977 6f72 6473 3d6a 736f 6e2e 6475  keywords=json.du
-00012080: 6d70 7328 6b65 7977 6f72 6473 290d 0a20  mps(keywords).. 
-00012090: 2020 2020 2320 7072 696e 7428 6b65 7977      # print(keyw
-000120a0: 6f72 6473 290d 0a20 2020 2020 2072 6574  ords)..      ret
-000120b0: 7572 6e20 6b65 7977 6f72 6473 0d0a 0d0a  urn keywords....
-000120c0: 6465 6620 7472 6169 6e62 6f77 2864 662c  def trainbow(df,
-000120d0: 636f 6c29 3a0d 0a20 2020 2020 206d 796c  col):..      myl
-000120e0: 6973 743d 6466 5b63 6f6c 5d2e 746f 6c69  ist=df[col].toli
-000120f0: 7374 2829 0d0a 2020 2020 2020 7374 6f70  st()..      stop
-00012100: 776f 7264 733d 6765 745f 7374 6f70 5f77  words=get_stop_w
-00012110: 6f72 6473 2829 0d0a 2020 2020 2020 6376  ords()..      cv
-00012120: 203d 2043 6f75 6e74 5665 6374 6f72 697a   = CountVectoriz
-00012130: 6572 2873 746f 705f 776f 7264 733d 7374  er(stop_words=st
-00012140: 6f70 776f 7264 7329 0d0a 2020 2020 2020  opwords)..      
-00012150: 7472 6169 6e5f 626f 7720 3d20 6376 2e66  train_bow = cv.f
-00012160: 6974 5f74 7261 6e73 666f 726d 286d 796c  it_transform(myl
-00012170: 6973 7429 0d0a 2020 2020 2020 2370 7269  ist)..      #pri
-00012180: 6e74 286c 6973 7428 6376 2e76 6f63 6162  nt(list(cv.vocab
-00012190: 756c 6172 795f 2e6b 6579 7328 2929 290d  ulary_.keys())).
-000121a0: 0a20 2020 2020 2072 6574 7572 6e20 6376  .      return cv
-000121b0: 2c74 7261 696e 5f62 6f77 0d0a 0d0a 200d  ,train_bow.... .
-000121c0: 0a64 6566 2073 6f72 745f 636f 6f28 636f  .def sort_coo(co
-000121d0: 6f5f 6d61 7472 6978 293a 0d0a 2020 2020  o_matrix):..    
-000121e0: 7475 706c 6573 203d 207a 6970 2863 6f6f  tuples = zip(coo
-000121f0: 5f6d 6174 7269 782e 636f 6c2c 2063 6f6f  _matrix.col, coo
-00012200: 5f6d 6174 7269 782e 6461 7461 290d 0a20  _matrix.data).. 
-00012210: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00012220: 2874 7570 6c65 732c 206b 6579 3d6c 616d  (tuples, key=lam
-00012230: 6264 6120 783a 2028 785b 315d 2c20 785b  bda x: (x[1], x[
-00012240: 305d 292c 2072 6576 6572 7365 3d54 7275  0]), reverse=Tru
-00012250: 6529 0d0a 0d0a 6465 6620 6578 7472 6163  e)....def extrac
-00012260: 745f 746f 706e 5f66 726f 6d5f 7665 6374  t_topn_from_vect
-00012270: 6f72 2866 6561 7475 7265 5f6e 616d 6573  or(feature_names
-00012280: 2c20 736f 7274 6564 5f69 7465 6d73 2c20  , sorted_items, 
-00012290: 746f 706e 3d31 3029 3a0d 0a20 2020 2022  topn=10):..    "
-000122a0: 2222 6765 7420 7468 6520 6665 6174 7572  ""get the featur
-000122b0: 6520 6e61 6d65 7320 616e 6420 7466 2d69  e names and tf-i
-000122c0: 6466 2073 636f 7265 206f 6620 746f 7020  df score of top 
-000122d0: 6e20 6974 656d 7322 2222 0d0a 2020 2020  n items"""..    
-000122e0: 0d0a 2020 2020 2375 7365 206f 6e6c 7920  ..    #use only 
-000122f0: 746f 706e 2069 7465 6d73 2066 726f 6d20  topn items from 
-00012300: 7665 6374 6f72 0d0a 2020 2020 736f 7274  vector..    sort
-00012310: 6564 5f69 7465 6d73 203d 2073 6f72 7465  ed_items = sorte
-00012320: 645f 6974 656d 735b 3a74 6f70 6e5d 0d0a  d_items[:topn]..
-00012330: 0d0a 2020 2020 7363 6f72 655f 7661 6c73  ..    score_vals
-00012340: 203d 205b 5d0d 0a20 2020 2066 6561 7475   = []..    featu
-00012350: 7265 5f76 616c 7320 3d20 5b5d 0d0a 0d0a  re_vals = []....
-00012360: 2020 2020 666f 7220 6964 782c 2073 636f      for idx, sco
-00012370: 7265 2069 6e20 736f 7274 6564 5f69 7465  re in sorted_ite
-00012380: 6d73 3a20 2020 2020 2020 200d 0a20 2020  ms:        ..   
-00012390: 2020 2020 2020 2066 6e61 6d65 203d 2066         fname = f
-000123a0: 6561 7475 7265 5f6e 616d 6573 5b69 6478  eature_names[idx
-000123b0: 5d0d 0a20 2020 2020 2020 2020 2069 6620  ]..          if 
-000123c0: 6c65 6e28 666e 616d 6529 3e33 3a0d 0a20  len(fname)>3:.. 
-000123d0: 2020 2020 2020 2023 6b65 6570 2074 7261         #keep tra
-000123e0: 636b 206f 6620 6665 6174 7572 6520 6e61  ck of feature na
-000123f0: 6d65 2061 6e64 2069 7473 2063 6f72 7265  me and its corre
-00012400: 7370 6f6e 6469 6e67 2073 636f 7265 0d0a  sponding score..
-00012410: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
-00012420: 655f 7661 6c73 2e61 7070 656e 6428 726f  e_vals.append(ro
-00012430: 756e 6428 7363 6f72 652c 2033 2929 0d0a  und(score, 3))..
-00012440: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00012450: 7572 655f 7661 6c73 2e61 7070 656e 6428  ure_vals.append(
-00012460: 6665 6174 7572 655f 6e61 6d65 735b 6964  feature_names[id
-00012470: 785d 290d 0a0d 0a20 2020 2023 6372 6561  x])....    #crea
-00012480: 7465 2061 2074 7570 6c65 7320 6f66 2066  te a tuples of f
-00012490: 6561 7475 7265 2c73 636f 7265 0d0a 2020  eature,score..  
-000124a0: 2020 2372 6573 756c 7473 203d 207a 6970    #results = zip
-000124b0: 2866 6561 7475 7265 5f76 616c 732c 7363  (feature_vals,sc
-000124c0: 6f72 655f 7661 6c73 290d 0a20 2020 2072  ore_vals)..    r
-000124d0: 6573 756c 7473 3d20 7b7d 0d0a 2020 2020  esults= {}..    
-000124e0: 666f 7220 6964 7820 696e 2072 616e 6765  for idx in range
-000124f0: 286c 656e 2866 6561 7475 7265 5f76 616c  (len(feature_val
-00012500: 7329 293a 0d0a 2020 2020 2020 2020 7265  s)):..        re
-00012510: 7375 6c74 735b 6665 6174 7572 655f 7661  sults[feature_va
-00012520: 6c73 5b69 6478 5d5d 3d73 636f 7265 5f76  ls[idx]]=score_v
-00012530: 616c 735b 6964 785d 0d0a 2020 2020 0d0a  als[idx]..    ..
-00012540: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00012550: 7473 0d0a 0d0a 6465 6620 6765 746b 6579  ts....def getkey
-00012560: 776f 7264 7328 6d79 7465 7874 2c6d 6178  words(mytext,max
-00012570: 6b65 7977 6f72 6473 293a 0d0a 2020 2020  keywords):..    
-00012580: 723d 5261 6b65 286d 6178 5f6c 656e 6774  r=Rake(max_lengt
-00012590: 683d 3130 290d 0a20 2020 2072 203d 2052  h=10)..    r = R
-000125a0: 616b 6528 7261 6e6b 696e 675f 6d65 7472  ake(ranking_metr
-000125b0: 6963 3d4d 6574 7269 632e 4445 4752 4545  ic=Metric.DEGREE
-000125c0: 5f54 4f5f 4652 4551 5545 4e43 595f 5241  _TO_FREQUENCY_RA
-000125d0: 5449 4f29 0d0a 2020 2020 2372 203d 2052  TIO)..    #r = R
-000125e0: 616b 6528 7261 6e6b 696e 675f 6d65 7472  ake(ranking_metr
-000125f0: 6963 3d4d 6574 7269 632e 574f 5244 5f44  ic=Metric.WORD_D
-00012600: 4547 5245 4529 0d0a 2020 2020 2372 203d  EGREE)..    #r =
-00012610: 2052 616b 6528 7261 6e6b 696e 675f 6d65   Rake(ranking_me
-00012620: 7472 6963 3d4d 6574 7269 632e 574f 5244  tric=Metric.WORD
-00012630: 5f46 5245 5155 454e 4359 290d 0a20 2020  _FREQUENCY)..   
-00012640: 2064 3d7b 2769 6e70 7574 273a 5b6d 7974   d={'input':[myt
-00012650: 6578 745d 7d0d 0a20 2020 2064 6620 3d20  ext]}..    df = 
-00012660: 7064 2e44 6174 6146 7261 6d65 2864 290d  pd.DataFrame(d).
-00012670: 0a20 2020 2064 663d 636f 6e76 6572 7474  .    df=convertt
-00012680: 6f6c 6f77 6572 6361 7365 2864 662c 2769  olowercase(df,'i
-00012690: 6e70 7574 2729 0d0a 2020 2020 6466 3d72  nput')..    df=r
-000126a0: 656d 6f76 6570 756e 6374 7561 7469 6f6e  emovepunctuation
-000126b0: 2864 662c 2769 6e70 7574 2729 0d0a 2020  (df,'input')..  
-000126c0: 2020 6466 3d72 656d 6f76 6573 746f 7077    df=removestopw
-000126d0: 6f72 6473 2864 662c 2769 6e70 7574 2729  ords(df,'input')
-000126e0: 0d0a 2020 2020 6466 3d72 656d 6f76 6563  ..    df=removec
-000126f0: 6f6d 6d6f 6e77 6f72 6473 2864 662c 2769  ommonwords(df,'i
-00012700: 6e70 7574 2729 0d0a 2020 2020 6466 3d72  nput')..    df=r
-00012710: 656d 6f76 6572 6172 6577 6f72 6473 2864  emoverarewords(d
-00012720: 662c 2769 6e70 7574 2729 0d0a 2020 2020  f,'input')..    
-00012730: 6466 3d63 6f72 7265 6374 7370 656c 6c69  df=correctspelli
-00012740: 6e67 2864 662c 2769 6e70 7574 2729 0d0a  ng(df,'input')..
-00012750: 2020 2020 6466 3d6c 656d 6d61 7469 7a61      df=lemmatiza
-00012760: 7469 6f6e 2864 662c 2769 6e70 7574 2729  tion(df,'input')
-00012770: 0d0a 2020 2020 6d79 7465 7874 3d64 665b  ..    mytext=df[
-00012780: 2769 6e70 7574 275d 5b30 5d0d 0a20 2020  'input'][0]..   
-00012790: 2063 762c 7477 3d74 7261 696e 626f 7728   cv,tw=trainbow(
-000127a0: 6466 2c27 696e 7075 7427 290d 0a20 2020  df,'input')..   
-000127b0: 206b 6579 776f 7264 733d 7472 6169 6e76   keywords=trainv
-000127c0: 6563 7428 6376 2c74 772c 6466 2c27 696e  ect(cv,tw,df,'in
-000127d0: 7075 7427 2c6d 6178 6b65 7977 6f72 6473  put',maxkeywords
-000127e0: 290d 0a0d 0a20 2020 200d 0a20 2020 206b  )....    ..    k
-000127f0: 6579 6275 6620 3d20 2222 0d0a 2020 2020  eybuf = ""..    
-00012800: 6b6a 736f 6e20 3d20 6a73 6f6e 2e6c 6f61  kjson = json.loa
-00012810: 6473 286b 6579 776f 7264 7329 0d0a 2020  ds(keywords)..  
-00012820: 2020 666f 7220 6b65 792c 2076 616c 7565    for key, value
-00012830: 2069 6e20 6b6a 736f 6e2e 6974 656d 7328   in kjson.items(
-00012840: 293a 0d0a 2020 2020 2020 2020 6b65 7962  ):..        keyb
-00012850: 7566 203d 206b 6579 6275 6620 2b20 6b65  uf = keybuf + ke
-00012860: 7920 2b22 2c22 202b 2073 7472 2876 616c  y +"," + str(val
-00012870: 7565 2920 2b20 223a 220d 0a20 2020 206b  ue) + ":"..    k
-00012880: 6579 6275 6620 3d20 6b65 7962 7566 5b3a  eybuf = keybuf[:
-00012890: 2d31 5d0d 0a0d 0a20 2020 2072 6574 7572  -1]....    retur
-000128a0: 6e20 6b65 7962 7566 0d0a 200d 0a64 6566  n keybuf.. ..def
-000128b0: 2064 6f73 756d 6d61 7279 2861 7274 6963   dosummary(artic
-000128c0: 6c65 5f74 6578 742c 6929 3a0d 0a0d 0a0d  le_text,i):.....
-000128d0: 0a20 2020 2061 7274 6963 6c65 5f74 6578  .    article_tex
-000128e0: 7420 3d20 7265 2e73 7562 2872 275c 5b5b  t = re.sub(r'\[[
-000128f0: 302d 395d 2a5c 5d27 2c20 2720 272c 2061  0-9]*\]', ' ', a
-00012900: 7274 6963 6c65 5f74 6578 7429 2020 0d0a  rticle_text)  ..
-00012910: 2020 2020 6172 7469 636c 655f 7465 7874      article_text
-00012920: 203d 2072 652e 7375 6228 7227 5c73 2b27   = re.sub(r'\s+'
-00012930: 2c20 2720 272c 2061 7274 6963 6c65 5f74  , ' ', article_t
-00012940: 6578 7429 0d0a 0d0a 2020 2020 2320 5265  ext)....    # Re
-00012950: 6d6f 7669 6e67 2073 7065 6369 616c 2063  moving special c
-00012960: 6861 7261 6374 6572 7320 616e 6420 6469  haracters and di
-00012970: 6769 7473 0d0a 2020 2020 666f 726d 6174  gits..    format
-00012980: 7465 645f 6172 7469 636c 655f 7465 7874  ted_article_text
-00012990: 203d 2072 652e 7375 6228 275b 5e61 2d7a   = re.sub('[^a-z
-000129a0: 412d 5a5d 272c 2027 2027 2c20 6172 7469  A-Z]', ' ', arti
-000129b0: 636c 655f 7465 7874 2029 2020 0d0a 2020  cle_text )  ..  
-000129c0: 2020 666f 726d 6174 7465 645f 6172 7469    formatted_arti
-000129d0: 636c 655f 7465 7874 203d 2072 652e 7375  cle_text = re.su
-000129e0: 6228 7227 5c73 2b27 2c20 2720 272c 2066  b(r'\s+', ' ', f
-000129f0: 6f72 6d61 7474 6564 5f61 7274 6963 6c65  ormatted_article
-00012a00: 5f74 6578 7429 2020 0d0a 0d0a 2020 2020  _text)  ....    
-00012a10: 7365 6e74 656e 6365 5f6c 6973 7420 3d20  sentence_list = 
-00012a20: 6e6c 746b 2e73 656e 745f 746f 6b65 6e69  nltk.sent_tokeni
-00012a30: 7a65 2861 7274 6963 6c65 5f74 6578 7429  ze(article_text)
-00012a40: 2020 0d0a 2020 2020 2370 7269 6e74 2873    ..    #print(s
-00012a50: 656e 7465 6e63 655f 6c69 7374 290d 0a0d  entence_list)...
-00012a60: 0a20 2020 2073 746f 7077 6f72 6473 203d  .    stopwords =
-00012a70: 206e 6c74 6b2e 636f 7270 7573 2e73 746f   nltk.corpus.sto
-00012a80: 7077 6f72 6473 2e77 6f72 6473 2827 656e  pwords.words('en
-00012a90: 676c 6973 6827 290d 0a0d 0a20 2020 2077  glish')....    w
-00012aa0: 6f72 645f 6672 6571 7565 6e63 6965 7320  ord_frequencies 
-00012ab0: 3d20 7b7d 2020 0d0a 2020 2020 666f 7220  = {}  ..    for 
-00012ac0: 776f 7264 2069 6e20 6e6c 746b 2e77 6f72  word in nltk.wor
-00012ad0: 645f 746f 6b65 6e69 7a65 2866 6f72 6d61  d_tokenize(forma
-00012ae0: 7474 6564 5f61 7274 6963 6c65 5f74 6578  tted_article_tex
-00012af0: 7429 3a20 200d 0a20 2020 2020 2020 2069  t):  ..        i
-00012b00: 6620 776f 7264 206e 6f74 2069 6e20 7374  f word not in st
-00012b10: 6f70 776f 7264 733a 0d0a 2020 2020 2020  opwords:..      
-00012b20: 2020 2020 2020 6966 2077 6f72 6420 6e6f        if word no
-00012b30: 7420 696e 2077 6f72 645f 6672 6571 7565  t in word_freque
-00012b40: 6e63 6965 732e 6b65 7973 2829 3a0d 0a20  ncies.keys():.. 
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00012b60: 6f72 645f 6672 6571 7565 6e63 6965 735b  ord_frequencies[
-00012b70: 776f 7264 5d20 3d20 310d 0a20 2020 2020  word] = 1..     
-00012b80: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00012b90: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-00012ba0: 7264 5f66 7265 7175 656e 6369 6573 5b77  rd_frequencies[w
-00012bb0: 6f72 645d 202b 3d20 310d 0a0d 0a20 2020  ord] += 1....   
-00012bc0: 206d 6178 696d 756d 5f66 7265 7175 6e63   maximum_frequnc
-00012bd0: 7920 3d20 6d61 7828 776f 7264 5f66 7265  y = max(word_fre
-00012be0: 7175 656e 6369 6573 2e76 616c 7565 7328  quencies.values(
-00012bf0: 2929 0d0a 0d0a 2020 2020 666f 7220 776f  ))....    for wo
-00012c00: 7264 2069 6e20 776f 7264 5f66 7265 7175  rd in word_frequ
-00012c10: 656e 6369 6573 2e6b 6579 7328 293a 2020  encies.keys():  
-00012c20: 0d0a 2020 2020 2020 2020 776f 7264 5f66  ..        word_f
-00012c30: 7265 7175 656e 6369 6573 5b77 6f72 645d  requencies[word]
-00012c40: 203d 2028 776f 7264 5f66 7265 7175 656e   = (word_frequen
-00012c50: 6369 6573 5b77 6f72 645d 2f6d 6178 696d  cies[word]/maxim
-00012c60: 756d 5f66 7265 7175 6e63 7929 0d0a 0d0a  um_frequncy)....
-00012c70: 2020 2020 2370 7269 6e74 2877 6f72 645f      #print(word_
-00012c80: 6672 6571 7565 6e63 6965 7329 0d0a 0d0a  frequencies)....
-00012c90: 2020 2020 7365 6e74 656e 6365 5f73 636f      sentence_sco
-00012ca0: 7265 7320 3d20 7b7d 2020 0d0a 2020 2020  res = {}  ..    
-00012cb0: 666f 7220 7365 6e74 2069 6e20 7365 6e74  for sent in sent
-00012cc0: 656e 6365 5f6c 6973 743a 2020 0d0a 2020  ence_list:  ..  
-00012cd0: 2020 2020 2020 666f 7220 776f 7264 2069        for word i
-00012ce0: 6e20 6e6c 746b 2e77 6f72 645f 746f 6b65  n nltk.word_toke
-00012cf0: 6e69 7a65 2873 656e 742e 6c6f 7765 7228  nize(sent.lower(
-00012d00: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00012d10: 2069 6620 776f 7264 2069 6e20 776f 7264   if word in word
-00012d20: 5f66 7265 7175 656e 6369 6573 2e6b 6579  _frequencies.key
-00012d30: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00012d40: 2020 2020 2020 6966 206c 656e 2873 656e        if len(sen
-00012d50: 742e 7370 6c69 7428 2720 2729 2920 3c20  t.split(' ')) < 
-00012d60: 3235 3a0d 0a20 2020 2020 2020 2020 2020  25:..           
-00012d70: 2020 2020 2020 2020 2069 6620 7365 6e74           if sent
-00012d80: 206e 6f74 2069 6e20 7365 6e74 656e 6365   not in sentence
-00012d90: 5f73 636f 7265 732e 6b65 7973 2829 3a0d  _scores.keys():.
-00012da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012db0: 2020 2020 2020 2020 2073 656e 7465 6e63           sentenc
-00012dc0: 655f 7363 6f72 6573 5b73 656e 745d 203d  e_scores[sent] =
-00012dd0: 2077 6f72 645f 6672 6571 7565 6e63 6965   word_frequencie
-00012de0: 735b 776f 7264 5d0d 0a20 2020 2020 2020  s[word]..       
-00012df0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00012e00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00012e10: 2020 2020 2020 2020 2020 2020 7365 6e74              sent
-00012e20: 656e 6365 5f73 636f 7265 735b 7365 6e74  ence_scores[sent
-00012e30: 5d20 2b3d 2077 6f72 645f 6672 6571 7565  ] += word_freque
-00012e40: 6e63 6965 735b 776f 7264 5d0d 0a0d 0a20  ncies[word].... 
-00012e50: 2020 2023 7072 696e 7428 7365 6e74 656e     #print(senten
-00012e60: 6365 5f73 636f 7265 7329 0d0a 0d0a 2020  ce_scores)....  
-00012e70: 2020 7375 6d6d 6172 795f 7365 6e74 656e    summary_senten
-00012e80: 6365 7320 3d20 6865 6170 712e 6e6c 6172  ces = heapq.nlar
-00012e90: 6765 7374 2869 2c20 7365 6e74 656e 6365  gest(i, sentence
-00012ea0: 5f73 636f 7265 732c 206b 6579 3d73 656e  _scores, key=sen
-00012eb0: 7465 6e63 655f 7363 6f72 6573 2e67 6574  tence_scores.get
-00012ec0: 290d 0a20 2020 2023 7072 696e 7428 7375  )..    #print(su
-00012ed0: 6d6d 6172 795f 7365 6e74 656e 6365 7329  mmary_sentences)
-00012ee0: 0d0a 2020 2020 7375 6d6d 6172 7920 3d20  ..    summary = 
-00012ef0: 2720 272e 6a6f 696e 2873 756d 6d61 7279  ' '.join(summary
-00012f00: 5f73 656e 7465 6e63 6573 290d 0a20 2020  _sentences)..   
-00012f10: 2023 7072 696e 7428 2241 4920 5375 6d6d   #print("AI Summ
-00012f20: 6172 7922 290d 0a20 2020 2072 6574 7572  ary")..    retur
-00012f30: 6e20 7375 6d6d 6172 790d 0a0d 0a64 6566  n summary....def
-00012f40: 2073 7461 7274 7375 6d6d 6172 7928 6172   startsummary(ar
-00012f50: 7469 636c 655f 7465 7874 2c66 7661 6c75  ticle_text,fvalu
-00012f60: 652c 6d61 786b 6579 776f 7264 7329 3a0d  e,maxkeywords):.
-00012f70: 0a20 2020 2020 200d 0a20 2320 7472 793a  .      .. # try:
-00012f80: 0d0a 2020 206f 7269 6769 6e61 6c77 6f72  ..   originalwor
-00012f90: 6473 203d 206c 656e 2861 7274 6963 6c65  ds = len(article
-00012fa0: 5f74 6578 742e 7370 6c69 7428 2220 2229  _text.split(" ")
-00012fb0: 290d 0a0d 0a20 2020 666f 7220 6920 696e  )....   for i in
-00012fc0: 2072 616e 6765 2831 2c31 3030 3030 293a   range(1,10000):
-00012fd0: 0d0a 2020 2020 2073 756d 6d61 7279 3d64  ..     summary=d
-00012fe0: 6f73 756d 6d61 7279 2861 7274 6963 6c65  osummary(article
-00012ff0: 5f74 6578 742c 6929 0d0a 2020 2020 2072  _text,i)..     r
-00013000: 6573 203d 206c 656e 2873 756d 6d61 7279  es = len(summary
-00013010: 2e73 706c 6974 2829 290d 0a20 2020 2020  .split())..     
-00013020: 6966 2072 6573 203e 3d20 6676 616c 7565  if res >= fvalue
-00013030: 3a0d 0a20 2020 2020 2020 2020 6272 6561  :..         brea
-00013040: 6b0d 0a0d 0a20 2020 7375 6d6d 6172 7920  k....   summary 
-00013050: 3d20 2072 652e 7375 6228 225c 5c5c 5c78  =  re.sub("\\\\x
-00013060: 5b61 2d66 302d 395d 5b61 2d66 302d 395d  [a-f0-9][a-f0-9]
-00013070: 222c 2022 2022 2c73 756d 6d61 7279 290d  ", " ",summary).
-00013080: 0a20 2020 7375 6d6d 6172 7920 3d20 7265  .   summary = re
-00013090: 2e73 7562 2822 5c5c 7865 325c 5c78 3830  .sub("\\xe2\\x80
-000130a0: 5c5c 7839 3922 2c22 2722 2c20 7375 6d6d  \\x99","'", summ
-000130b0: 6172 7929 0d0a 2020 2073 756d 6d61 7279  ary)..   summary
-000130c0: 3d73 756d 6d61 7279 2e72 6570 6c61 6365  =summary.replace
-000130d0: 2822 5c5c 7865 325c 5c78 3830 5c5c 7839  ("\\xe2\\x80\\x9
-000130e0: 3922 2c22 2722 290d 0a20 2020 7375 6d6d  9","'")..   summ
-000130f0: 6172 793d 7375 6d6d 6172 792e 7265 706c  ary=summary.repl
-00013100: 6163 6528 225c 5c78 6532 5c5c 7838 305c  ace("\\xe2\\x80\
-00013110: 5c78 3930 222c 222d 2229 0d0a 2020 2073  \x90","-")..   s
-00013120: 756d 6d61 7279 3d73 756d 6d61 7279 2e72  ummary=summary.r
-00013130: 6570 6c61 6365 2822 5c5c 7865 325c 5c78  eplace("\\xe2\\x
-00013140: 3830 5c5c 7839 3122 2c22 2d22 290d 0a20  80\\x91","-").. 
-00013150: 2020 7375 6d6d 6172 793d 7375 6d6d 6172    summary=summar
-00013160: 792e 7265 706c 6163 6528 225c 5c78 6532  y.replace("\\xe2
-00013170: 5c5c 7838 305c 5c78 3932 222c 222d 2229  \\x80\\x92","-")
-00013180: 0d0a 2020 2073 756d 6d61 7279 3d73 756d  ..   summary=sum
-00013190: 6d61 7279 2e72 6570 6c61 6365 2822 5c5c  mary.replace("\\
-000131a0: 7865 325c 5c78 3830 5c5c 7839 3322 2c22  xe2\\x80\\x93","
-000131b0: 2d22 290d 0a20 2020 7375 6d6d 6172 793d  -")..   summary=
-000131c0: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
-000131d0: 225c 5c78 6532 5c5c 7838 305c 5c78 3934  "\\xe2\\x80\\x94
-000131e0: 222c 222d 2229 0d0a 2020 2073 756d 6d61  ","-")..   summa
-000131f0: 7279 3d73 756d 6d61 7279 2e72 6570 6c61  ry=summary.repla
-00013200: 6365 2822 5c5c 7865 325c 5c78 3830 5c5c  ce("\\xe2\\x80\\
-00013210: 7839 3522 2c22 2d22 290d 0a20 2020 7375  x95","-")..   su
-00013220: 6d6d 6172 793d 7375 6d6d 6172 792e 7265  mmary=summary.re
-00013230: 706c 6163 6528 225c 5c78 6532 5c5c 7838  place("\\xe2\\x8
-00013240: 305c 5c78 6233 222c 2722 2729 0d0a 2020  0\\xb3",'"')..  
-00013250: 2073 756d 6d61 7279 203d 2073 756d 6d61   summary = summa
-00013260: 7279 2e72 6570 6c61 6365 2827 e280 9c27  ry.replace('...'
-00013270: 2c20 2722 2729 0d0a 2020 2073 756d 6d61  , '"')..   summa
-00013280: 7279 203d 2073 756d 6d61 7279 2e72 6570  ry = summary.rep
-00013290: 6c61 6365 2827 e280 9d27 2c20 2722 2729  lace('...', '"')
-000132a0: 0d0a 2020 2073 756d 6d61 7279 203d 2073  ..   summary = s
-000132b0: 756d 6d61 7279 2e72 6570 6c61 6365 2827  ummary.replace('
-000132c0: e280 9927 2c20 2227 2229 0d0a 2020 2073  ...', "'")..   s
-000132d0: 756d 6d61 7279 203d 2073 756d 6d61 7279  ummary = summary
-000132e0: 2e72 6570 6c61 6365 2827 e280 9827 2c20  .replace('...', 
-000132f0: 2227 2229 0d0a 2020 2073 756d 6d61 7279  "'")..   summary
-00013300: 203d 2073 756d 6d61 7279 2e72 6570 6c61   = summary.repla
-00013310: 6365 2827 e280 9327 2c20 222d 2229 0d0a  ce('...', "-")..
-00013320: 2020 2073 756d 6d61 7279 203d 2073 756d     summary = sum
-00013330: 6d61 7279 2e72 6570 6c61 6365 2827 e280  mary.replace('..
-00013340: a627 2c20 222e 2e2e 2229 0d0a 2020 2073  .', "...")..   s
-00013350: 756d 6d61 7279 203d 2073 756d 6d61 7279  ummary = summary
-00013360: 2e72 6570 6c61 6365 2827 e280 9427 2c20  .replace('...', 
-00013370: 222d 2229 0d0a 2020 2073 756d 6d61 7279  "-")..   summary
-00013380: 203d 2073 756d 6d61 7279 2e72 6570 6c61   = summary.repla
-00013390: 6365 2827 2227 2c20 2222 290d 0a0d 0a20  ce('"', "").... 
-000133a0: 2020 7375 6d6d 6172 7920 3d20 7375 6d6d    summary = summ
-000133b0: 6172 792e 7265 706c 6163 6528 275c 5c75  ary.replace('\\u
-000133c0: 272c 2755 2b27 290d 0a20 2020 7375 6d6d  ','U+')..   summ
-000133d0: 6172 7920 3d20 7265 2e73 7562 2872 273c  ary = re.sub(r'<
-000133e0: 555c 2b28 5b30 2d39 612d 6641 2d46 5d7b  U\+([0-9a-fA-F]{
-000133f0: 342c 367d 293e 272c 206c 616d 6264 6120  4,6})>', lambda 
-00013400: 783a 2063 6872 2869 6e74 2878 2e67 726f  x: chr(int(x.gro
-00013410: 7570 2831 292c 3136 2929 2c20 7375 6d6d  up(1),16)), summ
-00013420: 6172 7929 0d0a 0d0a 2020 206b 6579 776f  ary)....   keywo
-00013430: 7264 733d 6765 746b 6579 776f 7264 7328  rds=getkeywords(
-00013440: 7375 6d6d 6172 792c 6d61 786b 6579 776f  summary,maxkeywo
-00013450: 7264 7329 0d0a 0d0a 2020 2073 756d 6d61  rds)....   summa
-00013460: 7279 776f 7264 7320 3d20 6c65 6e28 7375  rywords = len(su
-00013470: 6d6d 6172 792e 7370 6c69 7428 2220 2229  mmary.split(" ")
-00013480: 290d 0a20 0d0a 2020 206d 6169 6e6f 7574  ).. ..   mainout
-00013490: 3d22 5c22 2220 2b20 6b65 7977 6f72 6473  ="\"" + keywords
-000134a0: 202b 2022 5c22 2c5c 226f 7269 6769 6e61   + "\",\"origina
-000134b0: 6c77 6f72 6463 6f75 6e74 5c22 3a22 202b  lwordcount\":" +
-000134c0: 2073 7472 286f 7269 6769 6e61 6c77 6f72   str(originalwor
-000134d0: 6473 2920 2b20 222c 5c22 7375 6d6d 6172  ds) + ",\"summar
-000134e0: 7977 6f72 6463 6f75 6e74 5c22 3a22 2b20  ywordcount\":"+ 
-000134f0: 7374 7228 7375 6d6d 6172 7977 6f72 6473  str(summarywords
-00013500: 2920 2b22 2c5c 226d 6169 6e73 756d 6d61  ) +",\"mainsumma
-00013510: 7279 5c22 3a7b 5c22 7375 6d6d 6172 795c  ry\":{\"summary\
-00013520: 223a 205c 2222 202b 2073 756d 6d61 7279  ": \"" + summary
-00013530: 202b 2022 5c22 7d7d 220d 0a20 2020 7265   + "\"}}"..   re
-00013540: 7475 726e 206d 6169 6e6f 7574 0d0a 2020  turn mainout..  
-00013550: 200d 0a23 2323 2323 2323 2323 2323 2323   ..#############
-00013560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013570: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013580: 2323 2323 0d0a 0d0a 6672 6f6d 206c 616e  ####....from lan
-00013590: 6763 6861 696e 2e65 6d62 6564 6469 6e67  gchain.embedding
-000135a0: 732e 6f70 656e 6169 2069 6d70 6f72 7420  s.openai import 
-000135b0: 4f70 656e 4149 456d 6265 6464 696e 6773  OpenAIEmbeddings
-000135c0: 0d0a 6672 6f6d 206c 616e 6763 6861 696e  ..from langchain
-000135d0: 2e74 6578 745f 7370 6c69 7474 6572 2069  .text_splitter i
-000135e0: 6d70 6f72 7420 4368 6172 6163 7465 7254  mport CharacterT
-000135f0: 6578 7453 706c 6974 7465 720d 0a66 726f  extSplitter..fro
-00013600: 6d20 6c61 6e67 6368 6169 6e2e 7665 6374  m langchain.vect
-00013610: 6f72 7374 6f72 6573 2e66 6169 7373 2069  orstores.faiss i
-00013620: 6d70 6f72 7420 4641 4953 530d 0a0d 0a66  mport FAISS....f
-00013630: 726f 6d20 6c61 6e67 6368 6169 6e2e 6368  rom langchain.ch
-00013640: 6169 6e73 2e71 7565 7374 696f 6e5f 616e  ains.question_an
-00013650: 7377 6572 696e 6720 696d 706f 7274 206c  swering import l
-00013660: 6f61 645f 7161 5f63 6861 696e 0d0a 6672  oad_qa_chain..fr
-00013670: 6f6d 206c 616e 6763 6861 696e 2e6c 6c6d  om langchain.llm
-00013680: 7320 696d 706f 7274 2050 726f 6d70 744c  s import PromptL
-00013690: 6179 6572 4f70 656e 4149 4368 6174 0d0a  ayerOpenAIChat..
-000136a0: 6672 6f6d 206c 616e 6763 6861 696e 2e63  from langchain.c
-000136b0: 6861 745f 6d6f 6465 6c73 2069 6d70 6f72  hat_models impor
-000136c0: 7420 4368 6174 4f70 656e 4149 0d0a 6672  t ChatOpenAI..fr
-000136d0: 6f6d 206c 616e 6763 6861 696e 2e6c 6c6d  om langchain.llm
-000136e0: 7320 696d 706f 7274 204f 7065 6e41 490d  s import OpenAI.
-000136f0: 0a69 6d70 6f72 7420 6861 7368 6c69 620d  .import hashlib.
-00013700: 0a0d 0a23 2041 6e73 7765 7220 7175 6573  ...# Answer ques
-00013710: 7469 6f6e 7320 6162 6f75 7420 7468 6520  tions about the 
-00013720: 6865 6164 6c69 6e65 730d 0a64 6566 2073  headlines..def s
-00013730: 7461 7274 5f63 6f6e 7665 7273 6174 696f  tart_conversatio
-00013740: 6e28 6f70 656e 6169 6b65 792c 7175 6572  n(openaikey,quer
-00013750: 792c 7465 7874 2c74 656d 7065 7261 7475  y,text,temperatu
-00013760: 7265 2c6d 6f64 656c 293a 0d0a 2020 2020  re,model):..    
-00013770: 2320 4772 6162 2074 6865 2069 6e70 7574  # Grab the input
-00013780: 2066 726f 6d20 7468 6520 4150 490d 0a20   from the API.. 
-00013790: 2020 2020 2020 2023 7175 6572 7920 3d20         #query = 
-000137a0: 696e 7075 7473 5b22 7175 6572 7922 0d0a  inputs["query"..
-000137b0: 0d0a 0d0a 2020 2020 2020 2020 7465 7874  ....        text
-000137c0: 5f73 706c 6974 7465 7220 3d20 4368 6172  _splitter = Char
-000137d0: 6163 7465 7254 6578 7453 706c 6974 7465  acterTextSplitte
-000137e0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-000137f0: 7365 7061 7261 746f 723d 2220 222c 0d0a  separator=" ",..
-00013800: 2020 2020 2020 2020 2020 2020 6368 756e              chun
-00013810: 6b5f 7369 7a65 3d31 3030 302c 0d0a 2020  k_size=1000,..  
-00013820: 2020 2020 2020 2020 2020 6368 756e 6b5f            chunk_
-00013830: 6f76 6572 6c61 703d 3230 302c 0d0a 2020  overlap=200,..  
-00013840: 2020 2020 2020 2020 2020 6c65 6e67 7468            length
-00013850: 5f66 756e 6374 696f 6e3d 6c65 6e2c 0d0a  _function=len,..
-00013860: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00013870: 2020 2020 2074 6578 7473 203d 2074 6578       texts = tex
-00013880: 745f 7370 6c69 7474 6572 2e73 706c 6974  t_splitter.split
-00013890: 5f74 6578 7428 7465 7874 290d 0a20 2020  _text(text)..   
-000138a0: 2020 2020 2065 6d62 6564 6469 6e67 7320       embeddings 
-000138b0: 3d20 4f70 656e 4149 456d 6265 6464 696e  = OpenAIEmbeddin
-000138c0: 6773 2829 0d0a 2020 2020 2020 2020 646f  gs()..        do
-000138d0: 6373 6561 7263 6820 3d20 4641 4953 532e  csearch = FAISS.
-000138e0: 6672 6f6d 5f74 6578 7473 2874 6578 7473  from_texts(texts
-000138f0: 2c20 656d 6265 6464 696e 6773 290d 0a20  , embeddings).. 
-00013900: 2020 2020 2020 2064 6f63 7320 3d20 646f         docs = do
-00013910: 6373 6561 7263 682e 7369 6d69 6c61 7269  csearch.similari
-00013920: 7479 5f73 6561 7263 6828 7175 6572 7929  ty_search(query)
-00013930: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00013940: 2020 2020 6368 6169 6e20 3d20 6c6f 6164      chain = load
-00013950: 5f71 615f 6368 6169 6e28 4f70 656e 4149  _qa_chain(OpenAI
-00013960: 286d 6f64 656c 5f6e 616d 653d 6d6f 6465  (model_name=mode
-00013970: 6c2c 2074 656d 7065 7261 7475 7265 3d74  l, temperature=t
-00013980: 656d 7065 7261 7475 7265 2c6f 7065 6e61  emperature,opena
-00013990: 695f 6170 695f 6b65 793d 6f70 656e 6169  i_api_key=openai
-000139a0: 6b65 7929 2c20 6368 6169 6e5f 7479 7065  key), chain_type
-000139b0: 3d22 7374 7566 6622 290d 0a20 2020 2020  ="stuff")..     
-000139c0: 2020 2072 6573 203d 2063 6861 696e 287b     res = chain({
-000139d0: 2269 6e70 7574 5f64 6f63 756d 656e 7473  "input_documents
-000139e0: 223a 2064 6f63 732c 2022 7175 6573 7469  ": docs, "questi
-000139f0: 6f6e 223a 2071 7565 7279 7d2c 2072 6574  on": query}, ret
-00013a00: 7572 6e5f 6f6e 6c79 5f6f 7574 7075 7473  urn_only_outputs
-00013a10: 3d54 7275 6529 0d0a 0d0a 2020 2020 2020  =True)....      
-00013a20: 2020 2372 6574 7572 6e20 7b22 7072 6564    #return {"pred
-00013a30: 223a 2072 6573 7d0d 0a20 2020 2020 2020  ": res}..       
-00013a40: 2072 6574 7572 6e20 7265 730d 0a0d 0a23   return res....#
-00013a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013a80: 2323 230d 0a66 726f 6d20 7064 6671 7565  ###..from pdfque
-00013a90: 7279 2069 6d70 6f72 7420 5044 4651 7565  ry import PDFQue
-00013aa0: 7279 0d0a 696d 706f 7274 2078 6d6c 746f  ry..import xmlto
-00013ab0: 6469 6374 0d0a 0d0a 0d0a 6465 6620 6c61  dict......def la
-00013ac0: 6265 6c66 6965 6c64 7328 6669 6c65 6e61  belfields(filena
-00013ad0: 6d65 2c6c 6162 656c 6e61 6d65 2c61 6372  me,labelname,acr
-00013ae0: 6f74 7970 6529 3a0d 0a20 2020 2020 7064  otype):..     pd
-00013af0: 6620 3d20 5044 4651 7565 7279 2866 696c  f = PDFQuery(fil
-00013b00: 656e 616d 6529 0d0a 2020 2020 2070 6466  ename)..     pdf
-00013b10: 2e6c 6f61 6428 290d 0a20 2020 2020 234c  .load()..     #L
-00013b20: 5454 6578 744c 696e 6548 6f72 697a 6f6e  TTextLineHorizon
-00013b30: 7461 6c0d 0a20 2020 2020 6c61 6265 6c20  tal..     label 
-00013b40: 3d20 7064 662e 7071 2861 6372 6f74 7970  = pdf.pq(acrotyp
-00013b50: 652b 273a 636f 6e74 6169 6e73 2822 272b  e+':contains("'+
-00013b60: 6c61 6265 6c6e 616d 6520 2b20 2722 2927  labelname + '")'
-00013b70: 290d 0a20 2020 2020 6c65 6674 5f63 6f72  )..     left_cor
-00013b80: 6e65 7220 3d20 666c 6f61 7428 6c61 6265  ner = float(labe
-00013b90: 6c2e 6174 7472 2827 7830 2729 290d 0a20  l.attr('x0')).. 
-00013ba0: 2020 2020 626f 7474 6f6d 5f63 6f72 6e65      bottom_corne
-00013bb0: 7220 3d20 666c 6f61 7428 6c61 6265 6c2e  r = float(label.
-00013bc0: 6174 7472 2827 7930 2729 290d 0a20 2020  attr('y0'))..   
-00013bd0: 2020 6e61 6d65 203d 2070 6466 2e70 7128    name = pdf.pq(
-00013be0: 6163 726f 7479 7065 202b 273a 696e 5f62  acrotype +':in_b
-00013bf0: 626f 7828 2225 732c 2025 732c 2025 732c  box("%s, %s, %s,
-00013c00: 2025 7322 2927 2025 2028 6c65 6674 5f63   %s")' % (left_c
-00013c10: 6f72 6e65 722c 2062 6f74 746f 6d5f 636f  orner, bottom_co
-00013c20: 726e 6572 2d33 302c 206c 6566 745f 636f  rner-30, left_co
-00013c30: 726e 6572 2b31 3530 2c20 626f 7474 6f6d  rner+150, bottom
-00013c40: 5f63 6f72 6e65 7229 292e 7465 7874 2829  _corner)).text()
-00013c50: 0d0a 2020 2020 2072 6574 7572 6e20 6e61  ..     return na
-00013c60: 6d65 0d0a 0d0a 0d0a 6465 6620 6578 7472  me......def extr
-00013c70: 6163 7466 6965 6c64 7328 6669 6c65 6e61  actfields(filena
-00013c80: 6d65 293a 0d0a 2020 2020 2020 2372 6561  me):..      #rea
-00013c90: 6420 7468 6520 5044 460d 0a20 2020 2020  d the PDF..     
-00013ca0: 2070 6466 203d 2050 4446 5175 6572 7928   pdf = PDFQuery(
-00013cb0: 6669 6c65 6e61 6d65 290d 0a20 2020 2020  filename)..     
-00013cc0: 2070 6466 2e6c 6f61 6428 290d 0a0d 0a20   pdf.load().... 
-00013cd0: 2020 2020 2023 6f20 3d20 786d 6c74 6f64       #o = xmltod
-00013ce0: 6963 742e 7061 7273 6528 273c 653e 203c  ict.parse('<e> <
-00013cf0: 613e 7465 7874 3c2f 613e 203c 613e 7465  a>text</a> <a>te
-00013d00: 7874 3c2f 613e 203c 2f65 3e27 290d 0a0d  xt</a> </e>')...
-00013d10: 0a20 2020 2020 2023 636f 6e76 6572 7420  .      #convert 
-00013d20: 7468 6520 7064 6620 746f 2058 4d4c 0d0a  the pdf to XML..
-00013d30: 2020 2020 2020 786d 6c66 696c 653d 2066        xmlfile= f
-00013d40: 696c 656e 616d 6520 2b20 272e 786d 6c27  ilename + '.xml'
-00013d50: 0d0a 2020 2020 2020 7064 662e 7472 6565  ..      pdf.tree
-00013d60: 2e77 7269 7465 2878 6d6c 6669 6c65 2c20  .write(xmlfile, 
-00013d70: 7072 6574 7479 5f70 7269 6e74 203d 2054  pretty_print = T
-00013d80: 7275 6529 0d0a 2020 2020 2020 7769 7468  rue)..      with
-00013d90: 206f 7065 6e28 786d 6c66 696c 6529 2061   open(xmlfile) a
-00013da0: 7320 663a 2073 203d 2066 2e72 6561 6428  s f: s = f.read(
-00013db0: 290d 0a0d 0a20 2020 2020 2023 7072 696e  )....      #prin
-00013dc0: 7428 7329 0d0a 2020 2020 2020 6a73 6f6e  t(s)..      json
-00013dd0: 6275 663d 786d 6c74 6f6a 736f 6e28 732c  buf=xmltojson(s,
-00013de0: 786d 6c66 696c 6529 0d0a 0d0a 2020 2020  xmlfile)....    
-00013df0: 2020 7265 7475 726e 206a 736f 6e62 7566    return jsonbuf
-00013e00: 0d0a 2020 2020 2020 0d0a 0d0a 6465 6620  ..      ....def 
-00013e10: 786d 6c74 6f6a 736f 6e28 786d 6c62 7566  xmltojson(xmlbuf
-00013e20: 6665 722c 786d 6c66 696c 6529 3a0d 0a0d  fer,xmlfile):...
-00013e30: 0a20 2020 2020 206f 203d 2078 6d6c 746f  .      o = xmlto
-00013e40: 6469 6374 2e70 6172 7365 2878 6d6c 6275  dict.parse(xmlbu
-00013e50: 6666 6572 290d 0a20 2020 2020 2078 6d6c  ffer)..      xml
-00013e60: 6a73 6f6e 3d6a 736f 6e2e 6475 6d70 7328  json=json.dumps(
-00013e70: 6f29 0d0a 2020 2020 2020 2370 7269 6e74  o)..      #print
-00013e80: 2878 6d6c 6a73 6f6e 290d 0a20 2020 2020  (xmljson)..     
-00013e90: 2077 6974 6820 6f70 656e 2878 6d6c 6669   with open(xmlfi
-00013ea0: 6c65 202b 2027 2e6a 736f 6e27 2c22 7722  le + '.json',"w"
-00013eb0: 2920 6173 2066 3a0d 0a20 2020 2020 2020  ) as f:..       
-00013ec0: 2066 2e77 7269 7465 2878 6d6c 6a73 6f6e   f.write(xmljson
-00013ed0: 290d 0a0d 0a20 2020 2020 2072 6574 7572  )....      retur
-00013ee0: 6e20 786d 6c6a 736f 6e20 200d 0a0d 0a23  n xmljson  ....#
-00013ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013f10: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00013f20: 696d 706f 7274 2065 6173 796f 6372 0d0a  import easyocr..
-00013f30: 696d 706f 7274 2073 7065 6563 685f 7265  import speech_re
-00013f40: 636f 676e 6974 696f 6e20 6173 2073 720d  cognition as sr.
-00013f50: 0a69 6d70 6f72 7420 6d6f 7669 6570 792e  .import moviepy.
-00013f60: 6564 6974 6f72 2061 7320 6d70 650d 0a0d  editor as mpe...
-00013f70: 0a64 6566 2063 6f6e 7665 7274 7669 6465  .def convertvide
-00013f80: 6f74 6f74 6578 7428 6669 6c65 6e61 6d65  ototext(filename
-00013f90: 293a 0d0a 2020 2020 2020 2020 2363 6f6e  ):..        #con
-00013fa0: 7665 7274 2074 6f20 6175 6469 6f0d 0a20  vert to audio.. 
-00013fb0: 2020 2020 2020 2076 6964 656f 203d 206d         video = m
-00013fc0: 7065 2e56 6964 656f 4669 6c65 436c 6970  pe.VideoFileClip
-00013fd0: 2866 696c 656e 616d 6529 0d0a 2020 2020  (filename)..    
-00013fe0: 2020 2020 6175 6469 6f66 696c 653d 6669      audiofile=fi
-00013ff0: 6c65 6e61 6d65 202b 2022 2e77 6176 220d  lename + ".wav".
-00014000: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00014010: 2020 2076 6964 656f 2e61 7564 696f 2e77     video.audio.w
-00014020: 7269 7465 5f61 7564 696f 6669 6c65 2861  rite_audiofile(a
-00014030: 7564 696f 6669 6c65 290d 0a20 2020 2020  udiofile)..     
-00014040: 2020 2072 6573 756c 7420 3d20 6175 6469     result = audi
-00014050: 6f74 6f74 6578 7428 6175 6469 6f66 696c  ototext(audiofil
-00014060: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
-00014070: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00014080: 756c 740d 0a0d 0a64 6566 2061 7564 696f  ult....def audio
-00014090: 746f 7465 7874 2866 696c 656e 616d 6529  totext(filename)
-000140a0: 3a0d 0a20 2020 2020 2020 2072 203d 2073  :..        r = s
-000140b0: 722e 5265 636f 676e 697a 6572 2829 0d0a  r.Recognizer()..
-000140c0: 2020 2020 2020 2020 6175 6469 6f20 3d20          audio = 
-000140d0: 7372 2e41 7564 696f 4669 6c65 2866 696c  sr.AudioFile(fil
-000140e0: 656e 616d 6529 0d0a 2020 2020 2020 2020  ename)..        
-000140f0: 7769 7468 2061 7564 696f 2061 7320 736f  with audio as so
-00014100: 7572 6365 3a0d 0a20 2020 2020 2020 2020  urce:..         
-00014110: 2061 7564 696f 5f66 696c 6520 3d20 722e   audio_file = r.
-00014120: 7265 636f 7264 2873 6f75 7263 6529 0d0a  record(source)..
-00014130: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00014140: 2072 2e72 6563 6f67 6e69 7a65 5f67 6f6f   r.recognize_goo
-00014150: 676c 6528 6175 6469 6f5f 6669 6c65 290d  gle(audio_file).
-00014160: 0a20 2020 2020 2020 2073 7065 6563 6866  .        speechf
-00014170: 696c 6520 3d20 6669 6c65 6e61 6d65 202b  ile = filename +
-00014180: 2027 2e73 7065 6563 682e 7478 7427 0d0a   '.speech.txt'..
-00014190: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-000141a0: 6e28 6669 6c65 6e61 6d65 202b 2027 2e73  n(filename + '.s
-000141b0: 7065 6563 682e 7478 7427 2c6d 6f64 6520  peech.txt',mode 
-000141c0: 3d27 7727 2920 6173 2066 696c 653a 200d  ='w') as file: .
-000141d0: 0a20 2020 2020 2020 2020 2020 6669 6c65  .           file
-000141e0: 2e77 7269 7465 2872 6573 756c 7429 0d0a  .write(result)..
-000141f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00014200: 2072 6573 756c 7420 2020 0d0a 0d0a 0d0a   result   ......
-00014210: 6465 6620 646f 6f63 726d 6169 6e28 6669  def doocrmain(fi
-00014220: 6c65 6e61 6d65 293a 0d0a 0d0a 2020 2020  lename):....    
-00014230: 7265 6164 6572 203d 2065 6173 796f 6372  reader = easyocr
-00014240: 2e52 6561 6465 7228 5b27 656e 275d 2920  .Reader(['en']) 
-00014250: 2020 0d0a 2020 2020 626f 756e 6420 3d20    ..    bound = 
-00014260: 7265 6164 6572 2e72 6561 6474 6578 7428  reader.readtext(
-00014270: 6669 6c65 6e61 6d65 290d 0a20 2020 2072  filename)..    r
-00014280: 6574 7572 6e20 626f 756e 640d 0a20 2020  eturn bound..   
-00014290: 200d 0a23 6669 6c65 6e61 6d65 3d27 7465   ..#filename='te
-000142a0: 7374 2d74 6178 2e70 6466 2720 2020 2020  st-tax.pdf'     
-000142b0: 0d0a 2370 6466 6a73 6f6e 3d65 7874 7261  ..#pdfjson=extra
-000142c0: 6374 6669 656c 6473 2866 696c 656e 616d  ctfields(filenam
-000142d0: 6529 0d0a 236e 616d 6574 6578 743d 6c61  e)..#nametext=la
-000142e0: 6265 6c66 6965 6c64 7328 6669 6c65 6e61  belfields(filena
-000142f0: 6d65 2c22 4275 7369 6e65 7373 206e 756d  me,"Business num
-00014300: 6265 7222 2c22 4c54 5465 7874 4c69 6e65  ber","LTTextLine
-00014310: 486f 7269 7a6f 6e74 616c 2229 0d0a 2370  Horizontal")..#p
-00014320: 7269 6e74 286e 616d 6574 6578 7429 0d0a  rint(nametext)..
-00014330: 0d0a                                     ..
+00010210: 2020 2020 0d0a 6465 6620 6172 6579 6f75      ..def areyou
+00010220: 6275 7379 2868 6f73 742c 706f 7274 3d2d  busy(host,port=-
+00010230: 3939 392c 6d69 6372 6f73 6572 7669 6365  999,microservice
+00010240: 6964 3d27 2729 3a0d 0a20 2020 2067 6c6f  id=''):..    glo
+00010250: 6261 6c20 636f 6e6e 6563 7469 6f6e 6572  bal connectioner
+00010260: 726f 720d 0a0d 0a20 2020 2069 6620 286c  ror....    if (l
+00010270: 656e 2868 6f73 7429 3d3d 3020 6f72 2070  en(host)==0 or p
+00010280: 6f72 743d 3d2d 3939 3920 293a 0d0a 2020  ort==-999 ):..  
+00010290: 2020 2020 2020 2072 6574 7572 6e20 2250         return "P
+000102a0: 6c65 6173 6520 656e 7465 7220 686f 7374  lease enter host
+000102b0: 2c70 6f72 7422 0d0a 2020 2020 7661 6c75  ,port"..    valu
+000102c0: 653d 2822 6172 6579 6f75 6275 7379 2229  e=("areyoubusy")
+000102d0: 0d0a 0d0a 2020 2020 7661 6c3d 6c6f 6f70  ....    val=loop
+000102e0: 2e72 756e 5f75 6e74 696c 5f63 6f6d 706c  .run_until_compl
+000102f0: 6574 6528 7463 705f 6563 686f 5f63 6c69  ete(tcp_echo_cli
+00010300: 656e 7476 6970 6572 2876 616c 7565 2c20  entviper(value, 
+00010310: 6c6f 6f70 2c68 6f73 742c 706f 7274 2c6d  loop,host,port,m
+00010320: 6963 726f 7365 7276 6963 6569 6429 290d  icroserviceid)).
+00010330: 0a20 2020 2069 6620 636f 6e6e 6563 7469  .    if connecti
+00010340: 6f6e 6572 726f 723a 0d0a 2020 2020 2020  onerror:..      
+00010350: 2020 2072 6574 7572 6e20 636f 6e6e 6563     return connec
+00010360: 7469 6f6e 6572 726f 720d 0a0d 0a20 2020  tionerror....   
+00010370: 2072 6574 7572 6e20 7661 6c0d 0a0d 0a23   return val....#
+00010380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000103a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000103b0: 2323 230d 0a69 6d70 6f72 7420 7379 730d  ###..import sys.
+000103c0: 0a66 726f 6d20 7064 666d 696e 6572 2e70  .from pdfminer.p
+000103d0: 6466 7061 7273 6572 2069 6d70 6f72 7420  dfparser import 
+000103e0: 5044 4650 6172 7365 720d 0a66 726f 6d20  PDFParser..from 
+000103f0: 7064 666d 696e 6572 2e70 6466 646f 6375  pdfminer.pdfdocu
+00010400: 6d65 6e74 2069 6d70 6f72 7420 5044 4644  ment import PDFD
+00010410: 6f63 756d 656e 740d 0a66 726f 6d20 7064  ocument..from pd
+00010420: 666d 696e 6572 2e70 6466 7061 6765 2069  fminer.pdfpage i
+00010430: 6d70 6f72 7420 5044 4650 6167 650d 0a66  mport PDFPage..f
+00010440: 726f 6d20 7064 666d 696e 6572 2e70 6466  rom pdfminer.pdf
+00010450: 7061 6765 2069 6d70 6f72 7420 5044 4654  page import PDFT
+00010460: 6578 7445 7874 7261 6374 696f 6e4e 6f74  extExtractionNot
+00010470: 416c 6c6f 7765 640d 0a66 726f 6d20 7064  Allowed..from pd
+00010480: 666d 696e 6572 2e70 6466 696e 7465 7270  fminer.pdfinterp
+00010490: 2069 6d70 6f72 7420 5044 4652 6573 6f75   import PDFResou
+000104a0: 7263 654d 616e 6167 6572 0d0a 6672 6f6d  rceManager..from
+000104b0: 2070 6466 6d69 6e65 722e 7064 6669 6e74   pdfminer.pdfint
+000104c0: 6572 7020 696d 706f 7274 2050 4446 5061  erp import PDFPa
+000104d0: 6765 496e 7465 7270 7265 7465 720d 0a23  geInterpreter..#
+000104e0: 6672 6f6d 2053 7472 696e 6749 4f20 696d  from StringIO im
+000104f0: 706f 7274 2053 7472 696e 6749 4f0d 0a66  port StringIO..f
+00010500: 726f 6d20 696f 2069 6d70 6f72 7420 5374  rom io import St
+00010510: 7269 6e67 494f 0d0a 696d 706f 7274 2075  ringIO..import u
+00010520: 726c 6c69 622e 7265 7175 6573 7420 200d  rllib.request  .
+00010530: 0a23 696d 706f 7274 2074 6d6c 7465 7874  .#import tmltext
+00010540: 7375 6d6d 6172 790d 0a69 6d70 6f72 7420  summary..import 
+00010550: 6f73 0d0a 696d 706f 7274 2064 6174 6574  os..import datet
+00010560: 696d 650d 0a23 696d 706f 7274 2067 6c6f  ime..#import glo
+00010570: 620d 0a0d 0a0d 0a66 726f 6d20 7064 666d  b......from pdfm
+00010580: 696e 6572 2e6c 6179 6f75 7420 696d 706f  iner.layout impo
+00010590: 7274 204c 4150 6172 616d 730d 0a66 726f  rt LAParams..fro
+000105a0: 6d20 7064 666d 696e 6572 2e63 6f6e 7665  m pdfminer.conve
+000105b0: 7274 6572 2069 6d70 6f72 7420 5465 7874  rter import Text
+000105c0: 436f 6e76 6572 7465 720d 0a20 0d0a 636c  Converter.. ..cl
+000105d0: 6173 7320 4d79 5061 7273 6572 286f 626a  ass MyParser(obj
+000105e0: 6563 7429 3a0d 0a20 2020 2064 6566 205f  ect):..    def _
+000105f0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7064  _init__(self, pd
+00010600: 6629 3a0d 0a20 2020 2020 2020 2023 2320  f):..        ## 
+00010610: 536e 6970 7065 6420 6164 6170 7465 6420  Snipped adapted 
+00010620: 6672 6f6d 2059 7573 756b 6520 5368 696e  from Yusuke Shin
+00010630: 7961 6d61 7320 0d0a 2020 2020 2020 2020  yamas ..        
+00010640: 2350 4446 4d69 6e65 7220 646f 6375 6d65  #PDFMiner docume
+00010650: 6e74 6174 696f 6e0d 0a20 2020 2020 2020  ntation..       
+00010660: 2023 2043 7265 6174 6520 7468 6520 646f   # Create the do
+00010670: 6375 6d65 6e74 206d 6f64 656c 2066 726f  cument model fro
+00010680: 6d20 7468 6520 6669 6c65 0d0a 2020 2020  m the file..    
+00010690: 2020 2020 7061 7273 6572 203d 2050 4446      parser = PDF
+000106a0: 5061 7273 6572 286f 7065 6e28 7064 662c  Parser(open(pdf,
+000106b0: 2027 7262 2729 290d 0a20 2020 2020 2020   'rb'))..       
+000106c0: 2064 6f63 756d 656e 7420 3d20 5044 4644   document = PDFD
+000106d0: 6f63 756d 656e 7428 7061 7273 6572 290d  ocument(parser).
+000106e0: 0a20 2020 2020 2020 2023 2054 7279 2074  .        # Try t
+000106f0: 6f20 7061 7273 6520 7468 6520 646f 6375  o parse the docu
+00010700: 6d65 6e74 0d0a 2020 2020 2020 2020 6966  ment..        if
+00010710: 206e 6f74 2064 6f63 756d 656e 742e 6973   not document.is
+00010720: 5f65 7874 7261 6374 6162 6c65 3a0d 0a20  _extractable:.. 
+00010730: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00010740: 2050 4446 5465 7874 4578 7472 6163 7469   PDFTextExtracti
+00010750: 6f6e 4e6f 7441 6c6c 6f77 6564 0d0a 2020  onNotAllowed..  
+00010760: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
+00010770: 2050 4446 2072 6573 6f75 7263 6520 6d61   PDF resource ma
+00010780: 6e61 6765 7220 6f62 6a65 6374 200d 0a20  nager object .. 
+00010790: 2020 2020 2020 2023 2074 6861 7420 7374         # that st
+000107a0: 6f72 6573 2073 6861 7265 6420 7265 736f  ores shared reso
+000107b0: 7572 6365 732e 0d0a 2020 2020 2020 2020  urces...        
+000107c0: 7273 7263 6d67 7220 3d20 5044 4652 6573  rsrcmgr = PDFRes
+000107d0: 6f75 7263 654d 616e 6167 6572 2829 0d0a  ourceManager()..
+000107e0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+000107f0: 2061 2062 7566 6665 7220 666f 7220 7468   a buffer for th
+00010800: 6520 7061 7273 6564 2074 6578 740d 0a20  e parsed text.. 
+00010810: 2020 2020 2020 2072 6574 7374 7220 3d20         retstr = 
+00010820: 5374 7269 6e67 494f 2829 0d0a 2020 2020  StringIO()..    
+00010830: 2020 2020 2320 5370 6163 696e 6720 7061      # Spacing pa
+00010840: 7261 6d65 7465 7273 2066 6f72 2070 6172  rameters for par
+00010850: 7369 6e67 0d0a 2020 2020 2020 2020 6c61  sing..        la
+00010860: 7061 7261 6d73 203d 204c 4150 6172 616d  params = LAParam
+00010870: 7328 290d 0a20 2020 2020 2020 2063 6f64  s()..        cod
+00010880: 6563 203d 2027 7574 662d 3827 0d0a 200d  ec = 'utf-8'.. .
+00010890: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+000108a0: 6520 6120 5044 4620 6465 7669 6365 206f  e a PDF device o
+000108b0: 626a 6563 740d 0a20 2020 2020 2020 2064  bject..        d
+000108c0: 6576 6963 6520 3d20 5465 7874 436f 6e76  evice = TextConv
+000108d0: 6572 7465 7228 7273 7263 6d67 722c 2072  erter(rsrcmgr, r
+000108e0: 6574 7374 722c 0d0a 2020 2020 2020 2020  etstr,..        
+000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010900: 2020 2020 2020 206c 6170 6172 616d 7320         laparams 
+00010910: 3d20 6c61 7061 7261 6d73 290d 0a20 2020  = laparams)..   
+00010920: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
+00010930: 5044 4620 696e 7465 7270 7265 7465 7220  PDF interpreter 
+00010940: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
+00010950: 696e 7465 7270 7265 7465 7220 3d20 5044  interpreter = PD
+00010960: 4650 6167 6549 6e74 6572 7072 6574 6572  FPageInterpreter
+00010970: 2872 7372 636d 6772 2c20 6465 7669 6365  (rsrcmgr, device
+00010980: 290d 0a20 2020 2020 2020 2023 2050 726f  )..        # Pro
+00010990: 6365 7373 2065 6163 6820 7061 6765 2063  cess each page c
+000109a0: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
+000109b0: 646f 6375 6d65 6e74 2e0d 0a20 2020 2020  document...     
+000109c0: 2020 2066 6f72 2070 6167 6520 696e 2050     for page in P
+000109d0: 4446 5061 6765 2e63 7265 6174 655f 7061  DFPage.create_pa
+000109e0: 6765 7328 646f 6375 6d65 6e74 293a 0d0a  ges(document):..
+000109f0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+00010a00: 7270 7265 7465 722e 7072 6f63 6573 735f  rpreter.process_
+00010a10: 7061 6765 2870 6167 6529 0d0a 2020 2020  page(page)..    
+00010a20: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00010a30: 656c 662e 7265 636f 7264 7320 2020 2020  elf.records     
+00010a40: 2020 2020 2020 203d 205b 5d0d 0a20 2020         = []..   
+00010a50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00010a60: 6c69 6e65 7320 3d20 7265 7473 7472 2e67  lines = retstr.g
+00010a70: 6574 7661 6c75 6528 292e 7370 6c69 746c  etvalue().splitl
+00010a80: 696e 6573 2829 0d0a 2020 2020 2020 2020  ines()..        
+00010a90: 666f 7220 6c69 6e65 2069 6e20 6c69 6e65  for line in line
+00010aa0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010ab0: 7365 6c66 2e68 616e 646c 655f 6c69 6e65  self.handle_line
+00010ac0: 286c 696e 6529 0d0a 2020 2020 200d 0a20  (line)..     .. 
+00010ad0: 2020 2064 6566 2068 616e 646c 655f 6c69     def handle_li
+00010ae0: 6e65 2873 656c 662c 206c 696e 6529 3a0d  ne(self, line):.
+00010af0: 0a20 2020 2020 2020 2023 2043 7573 746f  .        # Custo
+00010b00: 6d69 7a65 2079 6f75 7220 6c69 6e65 2d62  mize your line-b
+00010b10: 792d 6c69 6e65 2070 6172 7365 7220 6865  y-line parser he
+00010b20: 7265 0d0a 2020 2020 2020 2020 7365 6c66  re..        self
+00010b30: 2e72 6563 6f72 6473 2e61 7070 656e 6428  .records.append(
+00010b40: 6c69 6e65 290d 0a0d 0a64 6566 2073 6372  line)....def scr
+00010b50: 6170 6570 6466 2874 6865 7572 6c2c 666e  apepdf(theurl,fn
+00010b60: 293a 0d0a 2020 2020 7363 7261 7065 645f  ):..    scraped_
+00010b70: 6461 7461 203d 2075 726c 6c69 622e 7265  data = urllib.re
+00010b80: 7175 6573 742e 7572 6c6f 7065 6e28 7468  quest.urlopen(th
+00010b90: 6575 726c 2920 200d 0a20 2020 2066 696c  eurl)  ..    fil
+00010ba0: 6520 3d20 6f70 656e 2866 6e2c 2027 7762  e = open(fn, 'wb
+00010bb0: 2729 0d0a 2020 2020 6669 6c65 2e77 7269  ')..    file.wri
+00010bc0: 7465 2873 6372 6170 6564 5f64 6174 612e  te(scraped_data.
+00010bd0: 7265 6164 2829 290d 0a20 2020 2066 696c  read())..    fil
+00010be0: 652e 636c 6f73 6528 290d 0a20 2020 2023  e.close()..    #
+00010bf0: 7265 7475 726e 2061 7274 6963 6c65 5f74  return article_t
+00010c00: 6578 740d 0a0d 0a64 6566 2073 7461 7274  ext....def start
+00010c10: 7064 6672 6561 6469 6e67 2866 696c 656e  pdfreading(filen
+00010c20: 616d 652c 6676 616c 7565 2c6b 6579 636f  ame,fvalue,keyco
+00010c30: 756e 7429 3a0d 0a20 2023 6f73 2e70 6174  unt):..  #os.pat
+00010c40: 682e 6162 7370 6174 6828 6f73 2e67 6574  h.abspath(os.get
+00010c50: 6377 6428 2929 0d0a 2020 7468 6573 697a  cwd())..  thesiz
+00010c60: 653d 726f 756e 6428 6f73 2e70 6174 682e  e=round(os.path.
+00010c70: 6765 7473 697a 6528 6669 6c65 6e61 6d65  getsize(filename
+00010c80: 292f 3130 3030 3030 302c 3229 0d0a 2020  )/1000000,2)..  
+00010c90: 6d5f 7469 6d65 203d 206f 732e 7061 7468  m_time = os.path
+00010ca0: 2e67 6574 6d74 696d 6528 6669 6c65 6e61  .getmtime(filena
+00010cb0: 6d65 290d 0a20 2064 745f 6d20 3d20 6461  me)..  dt_m = da
+00010cc0: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00010cd0: 6672 6f6d 7469 6d65 7374 616d 7028 6d5f  fromtimestamp(m_
+00010ce0: 7469 6d65 290d 0a20 2063 5f74 696d 6520  time)..  c_time 
+00010cf0: 3d20 6f73 2e70 6174 682e 6765 7463 7469  = os.path.getcti
+00010d00: 6d65 2866 696c 656e 616d 6529 0d0a 2020  me(filename)..  
+00010d10: 2320 636f 6e76 6572 7420 6372 6561 7469  # convert creati
+00010d20: 6f6e 2074 696d 6573 7461 6d70 2069 6e74  on timestamp int
+00010d30: 6f20 4461 7465 5469 6d65 206f 626a 6563  o DateTime objec
+00010d40: 740d 0a20 2064 745f 6320 3d20 6461 7465  t..  dt_c = date
+00010d50: 7469 6d65 2e64 6174 6574 696d 652e 6672  time.datetime.fr
+00010d60: 6f6d 7469 6d65 7374 616d 7028 635f 7469  omtimestamp(c_ti
+00010d70: 6d65 290d 0a20 2063 6f20 3d20 7374 7228  me)..  co = str(
+00010d80: 6474 5f63 2920 5b30 3a31 395d 0d0a 2020  dt_c) [0:19]..  
+00010d90: 6d6f 203d 2073 7472 2864 745f 6d29 205b  mo = str(dt_m) [
+00010da0: 303a 3139 5d0d 0a0d 0a20 2070 203d 204d  0:19]....  p = M
+00010db0: 7950 6172 7365 7228 6669 6c65 6e61 6d65  yParser(filename
+00010dc0: 290d 0a20 2074 6865 7465 7874 3d27 5c6e  )..  thetext='\n
+00010dd0: 272e 6a6f 696e 2870 2e72 6563 6f72 6473  '.join(p.records
+00010de0: 290d 0a20 2061 7274 6963 6c65 5f74 6578  )..  article_tex
+00010df0: 743d 7468 6574 6578 742e 656e 636f 6465  t=thetext.encode
+00010e00: 2827 7574 6638 2729 0d0a 2020 7375 6d6d  ('utf8')..  summ
+00010e10: 6172 697a 6564 3d22 7b5c 2266 696c 656e  arized="{\"filen
+00010e20: 616d 655c 223a 5c22 2220 2b20 6669 6c65  ame\":\"" + file
+00010e30: 6e61 6d65 202b 2022 5c22 2c5c 2266 696c  name + "\",\"fil
+00010e40: 6573 697a 6528 4d42 295c 223a 222b 7374  esize(MB)\":"+st
+00010e50: 7228 7468 6573 697a 6529 2b22 2c5c 2266  r(thesize)+",\"f
+00010e60: 696c 6563 7265 6174 6564 6f6e 5c22 3a5c  ilecreatedon\":\
+00010e70: 2222 202b 2063 6f20 2b20 225c 222c 5c22  "" + co + "\",\"
+00010e80: 6669 6c65 6d6f 6469 6669 6564 6f6e 5c22  filemodifiedon\"
+00010e90: 3a5c 2222 202b 206d 6f20 2b20 225c 222c  :\"" + mo + "\",
+00010ea0: 5c22 6b65 7977 6f72 6473 5c22 3a22 202b  \"keywords\":" +
+00010eb0: 2020 7374 6172 7473 756d 6d61 7279 2874    startsummary(t
+00010ec0: 6865 7465 7874 2c66 7661 6c75 652c 6b65  hetext,fvalue,ke
+00010ed0: 7963 6f75 6e74 290d 0a20 2320 7072 696e  ycount).. # prin
+00010ee0: 7428 7375 6d6d 6172 697a 6564 290d 0a20  t(summarized).. 
+00010ef0: 2072 6574 7572 6e20 7375 6d6d 6172 697a   return summariz
+00010f00: 6564 0d0a 0d0a 0d0a 2323 2323 2323 2323  ed......########
+00010f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010f30: 2323 2323 2323 230d 0a23 2044 6576 656c  #######..# Devel
+00010f40: 6f70 6564 2062 7920 4f54 4943 5320 4164  oped by OTICS Ad
+00010f50: 7661 6e63 6564 2041 6e61 6c79 7469 6373  vanced Analytics
+00010f60: 0d0a 2320 5365 6261 7374 6961 6e20 4d61  ..# Sebastian Ma
+00010f70: 7572 6963 650d 0a0d 0a69 6d70 6f72 7420  urice....import 
+00010f80: 6273 3420 6173 2062 7320 200d 0a69 6d70  bs4 as bs  ..imp
+00010f90: 6f72 7420 7572 6c6c 6962 2e72 6571 7565  ort urllib.reque
+00010fa0: 7374 2020 0d0a 696d 706f 7274 2072 650d  st  ..import re.
+00010fb0: 0a69 6d70 6f72 7420 6e6c 746b 0d0a 6672  .import nltk..fr
+00010fc0: 6f6d 206e 6c74 6b2e 746f 6b65 6e69 7a65  om nltk.tokenize
+00010fd0: 2069 6d70 6f72 7420 5265 6765 7870 546f   import RegexpTo
+00010fe0: 6b65 6e69 7a65 720d 0a69 6d70 6f72 7420  kenizer..import 
+00010ff0: 6865 6170 710d 0a69 6d70 6f72 7420 7379  heapq..import sy
+00011000: 730d 0a69 6d70 6f72 7420 6f73 0d0a 6672  s..import os..fr
+00011010: 6f6d 2072 616b 655f 6e6c 746b 2069 6d70  om rake_nltk imp
+00011020: 6f72 7420 4d65 7472 6963 2c52 616b 650d  ort Metric,Rake.
+00011030: 0a69 6d70 6f72 7420 6a73 6f6e 0d0a 696d  .import json..im
+00011040: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+00011050: 640d 0a69 6d70 6f72 7420 6e6c 746b 2e63  d..import nltk.c
+00011060: 6f72 7075 730d 0a66 726f 6d20 6e6c 746b  orpus..from nltk
+00011070: 2e63 6f72 7075 7320 696d 706f 7274 2073  .corpus import s
+00011080: 746f 7077 6f72 6473 0d0a 6672 6f6d 2074  topwords..from t
+00011090: 6578 7462 6c6f 6220 696d 706f 7274 2054  extblob import T
+000110a0: 6578 7442 6c6f 620d 0a66 726f 6d20 7465  extBlob..from te
+000110b0: 7874 626c 6f62 2069 6d70 6f72 7420 576f  xtblob import Wo
+000110c0: 7264 0d0a 6672 6f6d 2073 6b6c 6561 726e  rd..from sklearn
+000110d0: 2e66 6561 7475 7265 5f65 7874 7261 6374  .feature_extract
+000110e0: 696f 6e2e 7465 7874 2069 6d70 6f72 7420  ion.text import 
+000110f0: 5466 6964 6654 7261 6e73 666f 726d 6572  TfidfTransformer
+00011100: 2c54 6669 6466 5665 6374 6f72 697a 6572  ,TfidfVectorizer
+00011110: 0d0a 6672 6f6d 2073 6b6c 6561 726e 2e66  ..from sklearn.f
+00011120: 6561 7475 7265 5f65 7874 7261 6374 696f  eature_extractio
+00011130: 6e2e 7465 7874 2069 6d70 6f72 7420 436f  n.text import Co
+00011140: 756e 7456 6563 746f 7269 7a65 720d 0a23  untVectorizer..#
+00011150: 6e6c 746b 2e64 6f77 6e6c 6f61 6428 2770  nltk.download('p
+00011160: 756e 6b74 2729 0d0a 696d 706f 7274 2077  unkt')..import w
+00011170: 6172 6e69 6e67 730d 0a77 6172 6e69 6e67  arnings..warning
+00011180: 732e 6669 6c74 6572 7761 726e 696e 6773  s.filterwarnings
+00011190: 2822 6967 6e6f 7265 2229 0d0a 0d0a 236e  ("ignore")....#n
+000111a0: 6c74 6b2e 646f 776e 6c6f 6164 2827 7374  ltk.download('st
+000111b0: 6f70 776f 7264 7327 290d 0a0d 0a64 6566  opwords')....def
+000111c0: 2067 6574 5f73 746f 705f 776f 7264 7328   get_stop_words(
+000111d0: 293a 0d0a 2020 2020 2222 226c 6f61 6420  ):..    """load 
+000111e0: 7374 6f70 2077 6f72 6473 2022 2222 0d0a  stop words """..
+000111f0: 2020 2020 7374 7077 7264 203d 2020 7374      stpwrd =  st
+00011200: 6f70 776f 7264 732e 776f 7264 7328 2765  opwords.words('e
+00011210: 6e67 6c69 7368 2729 0d0a 2020 2020 6e65  nglish')..    ne
+00011220: 775f 7374 6f70 776f 7264 7320 3d20 5b22  w_stopwords = ["
+00011230: 6e65 6564 222c 2022 756e 666f 7274 756e  need", "unfortun
+00011240: 6174 656c 7922 2c20 2274 6f22 2c20 226f  ately", "to", "o
+00011250: 6e22 2c20 2264 6169 6c79 222c 2022 7461  n", "daily", "ta
+00011260: 6b65 222c 0d0a 2020 2020 2020 2020 2020  ke",..          
+00011270: 2020 2020 2020 2020 2020 2022 7461 6b65             "take
+00011280: 6e22 2c22 6164 6472 6573 7369 6e67 222c  n","addressing",
+00011290: 2273 6f6f 6e65 7222 2c22 7261 7468 6572  "sooner","rather
+000112a0: 222c 226d 616b 6522 2c22 6c61 7465 7222  ","make","later"
+000112b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000112c0: 2020 2020 2020 2020 2273 6f6f 6e65 7222          "sooner"
+000112d0: 2c22 7375 6d6d 6172 7922 2c22 6c65 6176  ,"summary","leav
+000112e0: 6522 2c22 6576 6572 7922 2c22 696e 7465  e","every","inte
+000112f0: 6e64 222c 2266 696e 616c 6c79 222c 0d0a  nd","finally",..
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2020 2020 2022 656e 7469 7265 6c79 222c       "entirely",
+00011320: 2265 7665 6e22 2c22 656e 7375 7265 222c  "even","ensure",
+00011330: 2261 6c73 6f22 2c22 6166 6665 6374 222c  "also","affect",
+00011340: 2261 6666 6563 7469 6e67 222c 0d0a 2020  "affecting",..  
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2020 2022 6275 7369 6e65 7373 222c 2263     "business","c
+00011370: 6c61 7373 222c 2263 6f6d 7061 6e79 222c  lass","company",
+00011380: 2261 6c73 6f22 2c22 7965 6172 222c 2275  "also","year","u
+00011390: 7369 6e67 222c 0d0a 2020 2020 2020 2020  sing",..        
+000113a0: 2020 2020 2020 2020 2020 2020 2022 6973               "is
+000113b0: 7375 6564 222c 2273 7065 6369 6669 6322  sued","specific"
+000113c0: 2c22 7370 6563 6966 6963 616c 6c79 222c  ,"specifically",
+000113d0: 2272 6561 736f 6e22 2c22 7265 616c 222c  "reason","real",
+000113e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000113f0: 2020 2020 2020 2022 7072 6f6a 6563 7422         "project"
+00011400: 2c22 7061 7274 6963 756c 6172 6c79 222c  ,"particularly",
+00011410: 2270 6172 7469 6375 6c61 7222 2c22 6d61  "particular","ma
+00011420: 7474 6572 222c 226d 6169 6e22 2c0d 0a20  tter","main",.. 
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 226c 6973 7465 6422 2c22 636f      "listed","co
+00011450: 6d65 222c 2263 6f6d 7061 6e79 222c 2263  me","company","c
+00011460: 6f75 6c64 222c 2263 6f70 7922 2c22 6669  ould","copy","fi
+00011470: 7273 7422 2c22 6578 616d 706c 6522 2c0d  rst","example",.
+00011480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011490: 2020 2020 2020 2272 6561 6c22 2c22 6661        "real","fa
+000114a0: 6374 6f72 222c 2277 656c 6c22 2c22 736f  ctor","well","so
+000114b0: 7274 222c 2273 6f63 6961 6c22 2c22 736f  rt","social","so
+000114c0: 6369 616c 6c79 222c 2274 6872 6f75 6768  cially","through
+000114d0: 6f75 7422 2c0d 0a20 2020 2020 2020 2020  out",..         
+000114e0: 2020 2020 2020 2020 2020 2020 2272 6561              "rea
+000114f0: 736f 6e22 2c22 6176 6169 6c61 626c 6522  son","available"
+00011500: 2c22 6170 7072 6f61 6368 222c 2276 6172  ,"approach","var
+00011510: 7922 2c22 7479 7065 222c 2261 6372 6f73  y","type","acros
+00011520: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
+00011530: 2020 2020 2020 2020 2020 2261 7661 696c            "avail
+00011540: 6162 6c65 222c 2265 7175 616c 6c79 222c  able","equally",
+00011550: 226d 616e 6167 6572 222c 2264 6566 696e  "manager","defin
+00011560: 6974 696f 6e22 2c22 7368 6f72 7422 2c22  ition","short","
+00011570: 7265 7370 6f6e 7365 222c 0d0a 2020 2020  response",..    
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2022 7061 6e65 6c22 2c22 7265 7175 6972   "panel","requir
+000115a0: 6573 222c 2272 6571 7569 7269 6e67 222c  es","requiring",
+000115b0: 2272 6169 7365 222c 2273 686f 7722 2c22  "raise","show","
+000115c0: 646f 6e65 222c 2261 6465 7175 6174 656c  done","adequatel
+000115d0: 7922 2c0d 0a20 2020 2020 2020 2020 2020  y",..           
+000115e0: 2020 2020 2020 2020 2020 2267 656e 6572            "gener
+000115f0: 6963 222c 2267 656e 6572 616c 222c 2263  ic","general","c
+00011600: 6f75 7273 6522 2c22 6170 706c 6965 6422  ourse","applied"
+00011610: 2c22 7265 6c61 7465 6422 5d0d 0a20 2020  ,"related"]..   
+00011620: 2073 7470 7772 642e 6578 7465 6e64 286e   stpwrd.extend(n
+00011630: 6577 5f73 746f 7077 6f72 6473 290d 0a20  ew_stopwords).. 
+00011640: 2020 2072 6574 7572 6e20 7374 7077 7264     return stpwrd
+00011650: 0d0a 2020 0d0a 0d0a 2020 2020 0d0a 2323  ..  ....    ..##
+00011660: 2020 2020 7769 7468 206f 7065 6e28 2773      with open('s
+00011670: 746f 7077 6f72 6473 2e74 7874 272c 2027  topwords.txt', '
+00011680: 7227 2c20 656e 636f 6469 6e67 3d22 7574  r', encoding="ut
+00011690: 662d 3822 2920 6173 2066 3a0d 0a23 2320  f-8") as f:..## 
+000116a0: 2020 2020 2020 2073 746f 7077 6f72 6473         stopwords
+000116b0: 203d 2066 2e72 6561 646c 696e 6573 2829   = f.readlines()
+000116c0: 0d0a 2323 2020 2020 2020 2020 7374 6f70  ..##        stop
+000116d0: 5f73 6574 203d 2073 6574 286d 2e73 7472  _set = set(m.str
+000116e0: 6970 2829 2066 6f72 206d 2069 6e20 7374  ip() for m in st
+000116f0: 6f70 776f 7264 7329 0d0a 2323 2020 2020  opwords)..##    
+00011700: 2020 2320 2070 7269 6e74 2866 726f 7a65    #  print(froze
+00011710: 6e73 6574 2873 746f 705f 7365 7429 290d  nset(stop_set)).
+00011720: 0a23 2320 2020 2020 2020 2072 6574 7572  .##        retur
+00011730: 6e20 6672 6f7a 656e 7365 7428 7374 6f70  n frozenset(stop
+00011740: 5f73 6574 290d 0a0d 0a64 6566 2073 6372  _set)....def scr
+00011750: 6170 6577 6562 2874 6865 7572 6c29 3a0d  apeweb(theurl):.
+00011760: 0a20 2020 2073 6372 6170 6564 5f64 6174  .    scraped_dat
+00011770: 6120 3d20 7572 6c6c 6962 2e72 6571 7565  a = urllib.reque
+00011780: 7374 2e75 726c 6f70 656e 2874 6865 7572  st.urlopen(theur
+00011790: 6c29 2020 0d0a 2020 2020 6172 7469 636c  l)  ..    articl
+000117a0: 6520 3d20 7363 7261 7065 645f 6461 7461  e = scraped_data
+000117b0: 2e72 6561 6428 290d 0a0d 0a20 2020 2070  .read()....    p
+000117c0: 6172 7365 645f 6172 7469 636c 6520 3d20  arsed_article = 
+000117d0: 6273 2e42 6561 7574 6966 756c 536f 7570  bs.BeautifulSoup
+000117e0: 2861 7274 6963 6c65 2c27 6c78 6d6c 2729  (article,'lxml')
+000117f0: 0d0a 0d0a 2020 2020 7061 7261 6772 6170  ....    paragrap
+00011800: 6873 203d 2070 6172 7365 645f 6172 7469  hs = parsed_arti
+00011810: 636c 652e 6669 6e64 5f61 6c6c 2827 7027  cle.find_all('p'
+00011820: 290d 0a0d 0a20 2020 2061 7274 6963 6c65  )....    article
+00011830: 5f74 6578 7420 3d20 2222 0d0a 0d0a 2020  _text = ""....  
+00011840: 2020 666f 7220 7020 696e 2070 6172 6167    for p in parag
+00011850: 7261 7068 733a 2020 0d0a 2020 2020 2020  raphs:  ..      
+00011860: 2020 6172 7469 636c 655f 7465 7874 202b    article_text +
+00011870: 3d20 702e 7465 7874 0d0a 2020 2020 7265  = p.text..    re
+00011880: 7475 726e 2061 7274 6963 6c65 5f74 6578  turn article_tex
+00011890: 7420 0d0a 0d0a 6465 6620 636f 6e76 6572  t ....def conver
+000118a0: 7474 6f6c 6f77 6572 6361 7365 2864 662c  ttolowercase(df,
+000118b0: 636f 6c29 3a0d 0a20 2020 2020 2064 665b  col):..      df[
+000118c0: 636f 6c5d 203d 2064 665b 636f 6c5d 2e61  col] = df[col].a
+000118d0: 7070 6c79 286c 616d 6264 6120 783a 2022  pply(lambda x: "
+000118e0: 2022 2e6a 6f69 6e28 782e 6c6f 7765 7228   ".join(x.lower(
+000118f0: 2920 666f 7220 7820 696e 2078 2e73 706c  ) for x in x.spl
+00011900: 6974 2829 2929 0d0a 2020 2020 2020 7265  it()))..      re
+00011910: 7475 726e 2064 660d 0a20 2020 200d 0a64  turn df..    ..d
+00011920: 6566 2072 656d 6f76 6570 756e 6374 7561  ef removepunctua
+00011930: 7469 6f6e 2864 662c 636f 6c29 3a0d 0a20  tion(df,col):.. 
+00011940: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
+00011950: 665b 636f 6c5d 2e73 7472 2e72 6570 6c61  f[col].str.repla
+00011960: 6365 2827 5b5e 5c77 5c73 5d27 2c27 2729  ce('[^\w\s]','')
+00011970: 0d0a 2020 2020 2020 7265 7475 726e 2064  ..      return d
+00011980: 660d 0a0d 0a64 6566 2072 656d 6f76 6573  f....def removes
+00011990: 746f 7077 6f72 6473 2864 662c 636f 6c29  topwords(df,col)
+000119a0: 3a0d 0a20 2020 2020 2073 746f 7020 3d20  :..      stop = 
+000119b0: 7374 6f70 776f 7264 732e 776f 7264 7328  stopwords.words(
+000119c0: 2765 6e67 6c69 7368 2729 0d0a 2020 2020  'english')..    
+000119d0: 2020 6466 5b63 6f6c 5d20 3d20 6466 5b63    df[col] = df[c
+000119e0: 6f6c 5d2e 6170 706c 7928 6c61 6d62 6461  ol].apply(lambda
+000119f0: 2078 3a20 2220 222e 6a6f 696e 2878 2066   x: " ".join(x f
+00011a00: 6f72 2078 2069 6e20 782e 7370 6c69 7428  or x in x.split(
+00011a10: 2920 6966 2078 206e 6f74 2069 6e20 7374  ) if x not in st
+00011a20: 6f70 2929 0d0a 2020 2020 2020 7265 7475  op))..      retu
+00011a30: 726e 2064 660d 0a0d 0a64 6566 2072 656d  rn df....def rem
+00011a40: 6f76 6563 6f6d 6d6f 6e77 6f72 6473 2864  ovecommonwords(d
+00011a50: 662c 636f 6c29 3a0d 0a20 2020 2020 2066  f,col):..      f
+00011a60: 7265 7120 3d20 7064 2e53 6572 6965 7328  req = pd.Series(
+00011a70: 2720 272e 6a6f 696e 2864 665b 636f 6c5d  ' '.join(df[col]
+00011a80: 292e 7370 6c69 7428 2929 2e76 616c 7565  ).split()).value
+00011a90: 5f63 6f75 6e74 7328 295b 3a31 305d 0d0a  _counts()[:10]..
+00011aa0: 2020 2020 2020 6672 6571 203d 206c 6973        freq = lis
+00011ab0: 7428 6672 6571 2e69 6e64 6578 290d 0a20  t(freq.index).. 
+00011ac0: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
+00011ad0: 665b 636f 6c5d 2e61 7070 6c79 286c 616d  f[col].apply(lam
+00011ae0: 6264 6120 783a 2022 2022 2e6a 6f69 6e28  bda x: " ".join(
+00011af0: 7820 666f 7220 7820 696e 2078 2e73 706c  x for x in x.spl
+00011b00: 6974 2829 2069 6620 7820 6e6f 7420 696e  it() if x not in
+00011b10: 2066 7265 7129 290d 0a20 2020 2020 2072   freq))..      r
+00011b20: 6574 7572 6e20 6466 0d0a 0d0a 6465 6620  eturn df....def 
+00011b30: 7265 6d6f 7665 7261 7265 776f 7264 7328  removerarewords(
+00011b40: 6466 2c63 6f6c 293a 0d0a 2020 2020 2020  df,col):..      
+00011b50: 6672 6571 203d 2070 642e 5365 7269 6573  freq = pd.Series
+00011b60: 2827 2027 2e6a 6f69 6e28 6466 5b63 6f6c  (' '.join(df[col
+00011b70: 5d29 2e73 706c 6974 2829 292e 7661 6c75  ]).split()).valu
+00011b80: 655f 636f 756e 7473 2829 5b2d 3130 3a5d  e_counts()[-10:]
+00011b90: 0d0a 2020 2020 2020 6672 6571 203d 206c  ..      freq = l
+00011ba0: 6973 7428 6672 6571 2e69 6e64 6578 290d  ist(freq.index).
+00011bb0: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
+00011bc0: 2064 665b 636f 6c5d 2e61 7070 6c79 286c   df[col].apply(l
+00011bd0: 616d 6264 6120 783a 2022 2022 2e6a 6f69  ambda x: " ".joi
+00011be0: 6e28 7820 666f 7220 7820 696e 2078 2e73  n(x for x in x.s
+00011bf0: 706c 6974 2829 2069 6620 7820 6e6f 7420  plit() if x not 
+00011c00: 696e 2066 7265 7129 290d 0a20 2020 2020  in freq))..     
+00011c10: 2072 6574 7572 6e20 6466 0d0a 0d0a 6465   return df....de
+00011c20: 6620 636f 7272 6563 7473 7065 6c6c 696e  f correctspellin
+00011c30: 6728 6466 2c63 6f6c 293a 0d0a 2020 2020  g(df,col):..    
+00011c40: 2020 6466 5b63 6f6c 5d5b 3a35 5d2e 6170    df[col][:5].ap
+00011c50: 706c 7928 6c61 6d62 6461 2078 3a20 7374  ply(lambda x: st
+00011c60: 7228 5465 7874 426c 6f62 2878 292e 636f  r(TextBlob(x).co
+00011c70: 7272 6563 7428 2929 290d 0a20 2020 2020  rrect()))..     
+00011c80: 2072 6574 7572 6e20 6466 0d0a 0d0a 6465   return df....de
+00011c90: 6620 6c65 6d6d 6174 697a 6174 696f 6e28  f lemmatization(
+00011ca0: 6466 2c63 6f6c 293a 0d0a 2020 2020 2020  df,col):..      
+00011cb0: 6466 5b63 6f6c 5d20 3d20 6466 5b63 6f6c  df[col] = df[col
+00011cc0: 5d2e 6170 706c 7928 6c61 6d62 6461 2078  ].apply(lambda x
+00011cd0: 3a20 2220 222e 6a6f 696e 285b 576f 7264  : " ".join([Word
+00011ce0: 2877 6f72 6429 2e6c 656d 6d61 7469 7a65  (word).lemmatize
+00011cf0: 2829 2066 6f72 2077 6f72 6420 696e 2078  () for word in x
+00011d00: 2e73 706c 6974 2829 5d29 290d 0a20 2020  .split()]))..   
+00011d10: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
+00011d20: 6465 6620 7472 6169 6e76 6563 7428 6376  def trainvect(cv
+00011d30: 2c74 626f 772c 6466 2c63 6f6c 2c6d 6178  ,tbow,df,col,max
+00011d40: 6b65 7977 6f72 6473 293a 0d0a 2020 2020  keywords):..    
+00011d50: 2020 7465 7874 3d64 665b 636f 6c5d 2e74    text=df[col].t
+00011d60: 6f6c 6973 7428 290d 0a20 2020 2020 2074  olist()..      t
+00011d70: 6669 6466 203d 2054 6669 6466 5472 616e  fidf = TfidfTran
+00011d80: 7366 6f72 6d65 7228 736d 6f6f 7468 5f69  sformer(smooth_i
+00011d90: 6466 3d54 7275 652c 7573 655f 6964 663d  df=True,use_idf=
+00011da0: 5472 7565 290d 0a20 2020 2020 2074 6669  True)..      tfi
+00011db0: 6466 2e66 6974 2874 626f 7729 0d0a 2020  df.fit(tbow)..  
+00011dc0: 2020 2020 7466 5f69 6466 5f76 6563 746f      tf_idf_vecto
+00011dd0: 723d 7466 6964 662e 7472 616e 7366 6f72  r=tfidf.transfor
+00011de0: 6d28 6376 2e74 7261 6e73 666f 726d 2874  m(cv.transform(t
+00011df0: 6578 7429 290d 0a20 2020 2020 2073 6f72  ext))..      sor
+00011e00: 7465 6469 7465 6d73 3d73 6f72 745f 636f  teditems=sort_co
+00011e10: 6f28 7466 5f69 6466 5f76 6563 746f 722e  o(tf_idf_vector.
+00011e20: 746f 636f 6f28 2929 0d0a 2020 2020 2020  tocoo())..      
+00011e30: 6665 6174 7572 656e 616d 6573 3d63 762e  featurenames=cv.
+00011e40: 6765 745f 6665 6174 7572 655f 6e61 6d65  get_feature_name
+00011e50: 735f 6f75 7428 290d 0a20 2020 2020 206b  s_out()..      k
+00011e60: 6579 776f 7264 733d 6578 7472 6163 745f  eywords=extract_
+00011e70: 746f 706e 5f66 726f 6d5f 7665 6374 6f72  topn_from_vector
+00011e80: 2866 6561 7475 7265 6e61 6d65 732c 736f  (featurenames,so
+00011e90: 7274 6564 6974 656d 732c 6d61 786b 6579  rteditems,maxkey
+00011ea0: 776f 7264 7329 0d0a 2020 2020 2020 6b65  words)..      ke
+00011eb0: 7977 6f72 6473 3d6a 736f 6e2e 6475 6d70  ywords=json.dump
+00011ec0: 7328 6b65 7977 6f72 6473 290d 0a20 2020  s(keywords)..   
+00011ed0: 2020 2320 7072 696e 7428 6b65 7977 6f72    # print(keywor
+00011ee0: 6473 290d 0a20 2020 2020 2072 6574 7572  ds)..      retur
+00011ef0: 6e20 6b65 7977 6f72 6473 0d0a 0d0a 6465  n keywords....de
+00011f00: 6620 7472 6169 6e62 6f77 2864 662c 636f  f trainbow(df,co
+00011f10: 6c29 3a0d 0a20 2020 2020 206d 796c 6973  l):..      mylis
+00011f20: 743d 6466 5b63 6f6c 5d2e 746f 6c69 7374  t=df[col].tolist
+00011f30: 2829 0d0a 2020 2020 2020 7374 6f70 776f  ()..      stopwo
+00011f40: 7264 733d 6765 745f 7374 6f70 5f77 6f72  rds=get_stop_wor
+00011f50: 6473 2829 0d0a 2020 2020 2020 6376 203d  ds()..      cv =
+00011f60: 2043 6f75 6e74 5665 6374 6f72 697a 6572   CountVectorizer
+00011f70: 2873 746f 705f 776f 7264 733d 7374 6f70  (stop_words=stop
+00011f80: 776f 7264 7329 0d0a 2020 2020 2020 7472  words)..      tr
+00011f90: 6169 6e5f 626f 7720 3d20 6376 2e66 6974  ain_bow = cv.fit
+00011fa0: 5f74 7261 6e73 666f 726d 286d 796c 6973  _transform(mylis
+00011fb0: 7429 0d0a 2020 2020 2020 2370 7269 6e74  t)..      #print
+00011fc0: 286c 6973 7428 6376 2e76 6f63 6162 756c  (list(cv.vocabul
+00011fd0: 6172 795f 2e6b 6579 7328 2929 290d 0a20  ary_.keys())).. 
+00011fe0: 2020 2020 2072 6574 7572 6e20 6376 2c74       return cv,t
+00011ff0: 7261 696e 5f62 6f77 0d0a 0d0a 200d 0a64  rain_bow.... ..d
+00012000: 6566 2073 6f72 745f 636f 6f28 636f 6f5f  ef sort_coo(coo_
+00012010: 6d61 7472 6978 293a 0d0a 2020 2020 7475  matrix):..    tu
+00012020: 706c 6573 203d 207a 6970 2863 6f6f 5f6d  ples = zip(coo_m
+00012030: 6174 7269 782e 636f 6c2c 2063 6f6f 5f6d  atrix.col, coo_m
+00012040: 6174 7269 782e 6461 7461 290d 0a20 2020  atrix.data)..   
+00012050: 2072 6574 7572 6e20 736f 7274 6564 2874   return sorted(t
+00012060: 7570 6c65 732c 206b 6579 3d6c 616d 6264  uples, key=lambd
+00012070: 6120 783a 2028 785b 315d 2c20 785b 305d  a x: (x[1], x[0]
+00012080: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
+00012090: 0d0a 0d0a 6465 6620 6578 7472 6163 745f  ....def extract_
+000120a0: 746f 706e 5f66 726f 6d5f 7665 6374 6f72  topn_from_vector
+000120b0: 2866 6561 7475 7265 5f6e 616d 6573 2c20  (feature_names, 
+000120c0: 736f 7274 6564 5f69 7465 6d73 2c20 746f  sorted_items, to
+000120d0: 706e 3d31 3029 3a0d 0a20 2020 2022 2222  pn=10):..    """
+000120e0: 6765 7420 7468 6520 6665 6174 7572 6520  get the feature 
+000120f0: 6e61 6d65 7320 616e 6420 7466 2d69 6466  names and tf-idf
+00012100: 2073 636f 7265 206f 6620 746f 7020 6e20   score of top n 
+00012110: 6974 656d 7322 2222 0d0a 2020 2020 0d0a  items"""..    ..
+00012120: 2020 2020 2375 7365 206f 6e6c 7920 746f      #use only to
+00012130: 706e 2069 7465 6d73 2066 726f 6d20 7665  pn items from ve
+00012140: 6374 6f72 0d0a 2020 2020 736f 7274 6564  ctor..    sorted
+00012150: 5f69 7465 6d73 203d 2073 6f72 7465 645f  _items = sorted_
+00012160: 6974 656d 735b 3a74 6f70 6e5d 0d0a 0d0a  items[:topn]....
+00012170: 2020 2020 7363 6f72 655f 7661 6c73 203d      score_vals =
+00012180: 205b 5d0d 0a20 2020 2066 6561 7475 7265   []..    feature
+00012190: 5f76 616c 7320 3d20 5b5d 0d0a 0d0a 2020  _vals = []....  
+000121a0: 2020 666f 7220 6964 782c 2073 636f 7265    for idx, score
+000121b0: 2069 6e20 736f 7274 6564 5f69 7465 6d73   in sorted_items
+000121c0: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
+000121d0: 2020 2020 2066 6e61 6d65 203d 2066 6561       fname = fea
+000121e0: 7475 7265 5f6e 616d 6573 5b69 6478 5d0d  ture_names[idx].
+000121f0: 0a20 2020 2020 2020 2020 2069 6620 6c65  .          if le
+00012200: 6e28 666e 616d 6529 3e33 3a0d 0a20 2020  n(fname)>3:..   
+00012210: 2020 2020 2023 6b65 6570 2074 7261 636b       #keep track
+00012220: 206f 6620 6665 6174 7572 6520 6e61 6d65   of feature name
+00012230: 2061 6e64 2069 7473 2063 6f72 7265 7370   and its corresp
+00012240: 6f6e 6469 6e67 2073 636f 7265 0d0a 2020  onding score..  
+00012250: 2020 2020 2020 2020 2020 7363 6f72 655f            score_
+00012260: 7661 6c73 2e61 7070 656e 6428 726f 756e  vals.append(roun
+00012270: 6428 7363 6f72 652c 2033 2929 0d0a 2020  d(score, 3))..  
+00012280: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+00012290: 655f 7661 6c73 2e61 7070 656e 6428 6665  e_vals.append(fe
+000122a0: 6174 7572 655f 6e61 6d65 735b 6964 785d  ature_names[idx]
+000122b0: 290d 0a0d 0a20 2020 2023 6372 6561 7465  )....    #create
+000122c0: 2061 2074 7570 6c65 7320 6f66 2066 6561   a tuples of fea
+000122d0: 7475 7265 2c73 636f 7265 0d0a 2020 2020  ture,score..    
+000122e0: 2372 6573 756c 7473 203d 207a 6970 2866  #results = zip(f
+000122f0: 6561 7475 7265 5f76 616c 732c 7363 6f72  eature_vals,scor
+00012300: 655f 7661 6c73 290d 0a20 2020 2072 6573  e_vals)..    res
+00012310: 756c 7473 3d20 7b7d 0d0a 2020 2020 666f  ults= {}..    fo
+00012320: 7220 6964 7820 696e 2072 616e 6765 286c  r idx in range(l
+00012330: 656e 2866 6561 7475 7265 5f76 616c 7329  en(feature_vals)
+00012340: 293a 0d0a 2020 2020 2020 2020 7265 7375  ):..        resu
+00012350: 6c74 735b 6665 6174 7572 655f 7661 6c73  lts[feature_vals
+00012360: 5b69 6478 5d5d 3d73 636f 7265 5f76 616c  [idx]]=score_val
+00012370: 735b 6964 785d 0d0a 2020 2020 0d0a 2020  s[idx]..    ..  
+00012380: 2020 7265 7475 726e 2072 6573 756c 7473    return results
+00012390: 0d0a 0d0a 6465 6620 6765 746b 6579 776f  ....def getkeywo
+000123a0: 7264 7328 6d79 7465 7874 2c6d 6178 6b65  rds(mytext,maxke
+000123b0: 7977 6f72 6473 293a 0d0a 2020 2020 723d  ywords):..    r=
+000123c0: 5261 6b65 286d 6178 5f6c 656e 6774 683d  Rake(max_length=
+000123d0: 3130 290d 0a20 2020 2072 203d 2052 616b  10)..    r = Rak
+000123e0: 6528 7261 6e6b 696e 675f 6d65 7472 6963  e(ranking_metric
+000123f0: 3d4d 6574 7269 632e 4445 4752 4545 5f54  =Metric.DEGREE_T
+00012400: 4f5f 4652 4551 5545 4e43 595f 5241 5449  O_FREQUENCY_RATI
+00012410: 4f29 0d0a 2020 2020 2372 203d 2052 616b  O)..    #r = Rak
+00012420: 6528 7261 6e6b 696e 675f 6d65 7472 6963  e(ranking_metric
+00012430: 3d4d 6574 7269 632e 574f 5244 5f44 4547  =Metric.WORD_DEG
+00012440: 5245 4529 0d0a 2020 2020 2372 203d 2052  REE)..    #r = R
+00012450: 616b 6528 7261 6e6b 696e 675f 6d65 7472  ake(ranking_metr
+00012460: 6963 3d4d 6574 7269 632e 574f 5244 5f46  ic=Metric.WORD_F
+00012470: 5245 5155 454e 4359 290d 0a20 2020 2064  REQUENCY)..    d
+00012480: 3d7b 2769 6e70 7574 273a 5b6d 7974 6578  ={'input':[mytex
+00012490: 745d 7d0d 0a20 2020 2064 6620 3d20 7064  t]}..    df = pd
+000124a0: 2e44 6174 6146 7261 6d65 2864 290d 0a20  .DataFrame(d).. 
+000124b0: 2020 2064 663d 636f 6e76 6572 7474 6f6c     df=converttol
+000124c0: 6f77 6572 6361 7365 2864 662c 2769 6e70  owercase(df,'inp
+000124d0: 7574 2729 0d0a 2020 2020 6466 3d72 656d  ut')..    df=rem
+000124e0: 6f76 6570 756e 6374 7561 7469 6f6e 2864  ovepunctuation(d
+000124f0: 662c 2769 6e70 7574 2729 0d0a 2020 2020  f,'input')..    
+00012500: 6466 3d72 656d 6f76 6573 746f 7077 6f72  df=removestopwor
+00012510: 6473 2864 662c 2769 6e70 7574 2729 0d0a  ds(df,'input')..
+00012520: 2020 2020 6466 3d72 656d 6f76 6563 6f6d      df=removecom
+00012530: 6d6f 6e77 6f72 6473 2864 662c 2769 6e70  monwords(df,'inp
+00012540: 7574 2729 0d0a 2020 2020 6466 3d72 656d  ut')..    df=rem
+00012550: 6f76 6572 6172 6577 6f72 6473 2864 662c  overarewords(df,
+00012560: 2769 6e70 7574 2729 0d0a 2020 2020 6466  'input')..    df
+00012570: 3d63 6f72 7265 6374 7370 656c 6c69 6e67  =correctspelling
+00012580: 2864 662c 2769 6e70 7574 2729 0d0a 2020  (df,'input')..  
+00012590: 2020 6466 3d6c 656d 6d61 7469 7a61 7469    df=lemmatizati
+000125a0: 6f6e 2864 662c 2769 6e70 7574 2729 0d0a  on(df,'input')..
+000125b0: 2020 2020 6d79 7465 7874 3d64 665b 2769      mytext=df['i
+000125c0: 6e70 7574 275d 5b30 5d0d 0a20 2020 2063  nput'][0]..    c
+000125d0: 762c 7477 3d74 7261 696e 626f 7728 6466  v,tw=trainbow(df
+000125e0: 2c27 696e 7075 7427 290d 0a20 2020 206b  ,'input')..    k
+000125f0: 6579 776f 7264 733d 7472 6169 6e76 6563  eywords=trainvec
+00012600: 7428 6376 2c74 772c 6466 2c27 696e 7075  t(cv,tw,df,'inpu
+00012610: 7427 2c6d 6178 6b65 7977 6f72 6473 290d  t',maxkeywords).
+00012620: 0a0d 0a20 2020 200d 0a20 2020 206b 6579  ...    ..    key
+00012630: 6275 6620 3d20 2222 0d0a 2020 2020 6b6a  buf = ""..    kj
+00012640: 736f 6e20 3d20 6a73 6f6e 2e6c 6f61 6473  son = json.loads
+00012650: 286b 6579 776f 7264 7329 0d0a 2020 2020  (keywords)..    
+00012660: 666f 7220 6b65 792c 2076 616c 7565 2069  for key, value i
+00012670: 6e20 6b6a 736f 6e2e 6974 656d 7328 293a  n kjson.items():
+00012680: 0d0a 2020 2020 2020 2020 6b65 7962 7566  ..        keybuf
+00012690: 203d 206b 6579 6275 6620 2b20 6b65 7920   = keybuf + key 
+000126a0: 2b22 2c22 202b 2073 7472 2876 616c 7565  +"," + str(value
+000126b0: 2920 2b20 223a 220d 0a20 2020 206b 6579  ) + ":"..    key
+000126c0: 6275 6620 3d20 6b65 7962 7566 5b3a 2d31  buf = keybuf[:-1
+000126d0: 5d0d 0a0d 0a20 2020 2072 6574 7572 6e20  ]....    return 
+000126e0: 6b65 7962 7566 0d0a 200d 0a64 6566 2064  keybuf.. ..def d
+000126f0: 6f73 756d 6d61 7279 2861 7274 6963 6c65  osummary(article
+00012700: 5f74 6578 742c 6929 3a0d 0a0d 0a0d 0a20  _text,i):...... 
+00012710: 2020 2061 7274 6963 6c65 5f74 6578 7420     article_text 
+00012720: 3d20 7265 2e73 7562 2872 275c 5b5b 302d  = re.sub(r'\[[0-
+00012730: 395d 2a5c 5d27 2c20 2720 272c 2061 7274  9]*\]', ' ', art
+00012740: 6963 6c65 5f74 6578 7429 2020 0d0a 2020  icle_text)  ..  
+00012750: 2020 6172 7469 636c 655f 7465 7874 203d    article_text =
+00012760: 2072 652e 7375 6228 7227 5c73 2b27 2c20   re.sub(r'\s+', 
+00012770: 2720 272c 2061 7274 6963 6c65 5f74 6578  ' ', article_tex
+00012780: 7429 0d0a 0d0a 2020 2020 2320 5265 6d6f  t)....    # Remo
+00012790: 7669 6e67 2073 7065 6369 616c 2063 6861  ving special cha
+000127a0: 7261 6374 6572 7320 616e 6420 6469 6769  racters and digi
+000127b0: 7473 0d0a 2020 2020 666f 726d 6174 7465  ts..    formatte
+000127c0: 645f 6172 7469 636c 655f 7465 7874 203d  d_article_text =
+000127d0: 2072 652e 7375 6228 275b 5e61 2d7a 412d   re.sub('[^a-zA-
+000127e0: 5a5d 272c 2027 2027 2c20 6172 7469 636c  Z]', ' ', articl
+000127f0: 655f 7465 7874 2029 2020 0d0a 2020 2020  e_text )  ..    
+00012800: 666f 726d 6174 7465 645f 6172 7469 636c  formatted_articl
+00012810: 655f 7465 7874 203d 2072 652e 7375 6228  e_text = re.sub(
+00012820: 7227 5c73 2b27 2c20 2720 272c 2066 6f72  r'\s+', ' ', for
+00012830: 6d61 7474 6564 5f61 7274 6963 6c65 5f74  matted_article_t
+00012840: 6578 7429 2020 0d0a 0d0a 2020 2020 7365  ext)  ....    se
+00012850: 6e74 656e 6365 5f6c 6973 7420 3d20 6e6c  ntence_list = nl
+00012860: 746b 2e73 656e 745f 746f 6b65 6e69 7a65  tk.sent_tokenize
+00012870: 2861 7274 6963 6c65 5f74 6578 7429 2020  (article_text)  
+00012880: 0d0a 2020 2020 2370 7269 6e74 2873 656e  ..    #print(sen
+00012890: 7465 6e63 655f 6c69 7374 290d 0a0d 0a20  tence_list).... 
+000128a0: 2020 2073 746f 7077 6f72 6473 203d 206e     stopwords = n
+000128b0: 6c74 6b2e 636f 7270 7573 2e73 746f 7077  ltk.corpus.stopw
+000128c0: 6f72 6473 2e77 6f72 6473 2827 656e 676c  ords.words('engl
+000128d0: 6973 6827 290d 0a0d 0a20 2020 2077 6f72  ish')....    wor
+000128e0: 645f 6672 6571 7565 6e63 6965 7320 3d20  d_frequencies = 
+000128f0: 7b7d 2020 0d0a 2020 2020 666f 7220 776f  {}  ..    for wo
+00012900: 7264 2069 6e20 6e6c 746b 2e77 6f72 645f  rd in nltk.word_
+00012910: 746f 6b65 6e69 7a65 2866 6f72 6d61 7474  tokenize(formatt
+00012920: 6564 5f61 7274 6963 6c65 5f74 6578 7429  ed_article_text)
+00012930: 3a20 200d 0a20 2020 2020 2020 2069 6620  :  ..        if 
+00012940: 776f 7264 206e 6f74 2069 6e20 7374 6f70  word not in stop
+00012950: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00012960: 2020 2020 6966 2077 6f72 6420 6e6f 7420      if word not 
+00012970: 696e 2077 6f72 645f 6672 6571 7565 6e63  in word_frequenc
+00012980: 6965 732e 6b65 7973 2829 3a0d 0a20 2020  ies.keys():..   
+00012990: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+000129a0: 645f 6672 6571 7565 6e63 6965 735b 776f  d_frequencies[wo
+000129b0: 7264 5d20 3d20 310d 0a20 2020 2020 2020  rd] = 1..       
+000129c0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000129d0: 2020 2020 2020 2020 2020 2020 776f 7264              word
+000129e0: 5f66 7265 7175 656e 6369 6573 5b77 6f72  _frequencies[wor
+000129f0: 645d 202b 3d20 310d 0a0d 0a20 2020 206d  d] += 1....    m
+00012a00: 6178 696d 756d 5f66 7265 7175 6e63 7920  aximum_frequncy 
+00012a10: 3d20 6d61 7828 776f 7264 5f66 7265 7175  = max(word_frequ
+00012a20: 656e 6369 6573 2e76 616c 7565 7328 2929  encies.values())
+00012a30: 0d0a 0d0a 2020 2020 666f 7220 776f 7264  ....    for word
+00012a40: 2069 6e20 776f 7264 5f66 7265 7175 656e   in word_frequen
+00012a50: 6369 6573 2e6b 6579 7328 293a 2020 0d0a  cies.keys():  ..
+00012a60: 2020 2020 2020 2020 776f 7264 5f66 7265          word_fre
+00012a70: 7175 656e 6369 6573 5b77 6f72 645d 203d  quencies[word] =
+00012a80: 2028 776f 7264 5f66 7265 7175 656e 6369   (word_frequenci
+00012a90: 6573 5b77 6f72 645d 2f6d 6178 696d 756d  es[word]/maximum
+00012aa0: 5f66 7265 7175 6e63 7929 0d0a 0d0a 2020  _frequncy)....  
+00012ab0: 2020 2370 7269 6e74 2877 6f72 645f 6672    #print(word_fr
+00012ac0: 6571 7565 6e63 6965 7329 0d0a 0d0a 2020  equencies)....  
+00012ad0: 2020 7365 6e74 656e 6365 5f73 636f 7265    sentence_score
+00012ae0: 7320 3d20 7b7d 2020 0d0a 2020 2020 666f  s = {}  ..    fo
+00012af0: 7220 7365 6e74 2069 6e20 7365 6e74 656e  r sent in senten
+00012b00: 6365 5f6c 6973 743a 2020 0d0a 2020 2020  ce_list:  ..    
+00012b10: 2020 2020 666f 7220 776f 7264 2069 6e20      for word in 
+00012b20: 6e6c 746b 2e77 6f72 645f 746f 6b65 6e69  nltk.word_tokeni
+00012b30: 7a65 2873 656e 742e 6c6f 7765 7228 2929  ze(sent.lower())
+00012b40: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00012b50: 6620 776f 7264 2069 6e20 776f 7264 5f66  f word in word_f
+00012b60: 7265 7175 656e 6369 6573 2e6b 6579 7328  requencies.keys(
+00012b70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00012b80: 2020 2020 6966 206c 656e 2873 656e 742e      if len(sent.
+00012b90: 7370 6c69 7428 2720 2729 2920 3c20 3235  split(' ')) < 25
+00012ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012bb0: 2020 2020 2020 2069 6620 7365 6e74 206e         if sent n
+00012bc0: 6f74 2069 6e20 7365 6e74 656e 6365 5f73  ot in sentence_s
+00012bd0: 636f 7265 732e 6b65 7973 2829 3a0d 0a20  cores.keys():.. 
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 2020 2020 2020 2073 656e 7465 6e63 655f         sentence_
+00012c00: 7363 6f72 6573 5b73 656e 745d 203d 2077  scores[sent] = w
+00012c10: 6f72 645f 6672 6571 7565 6e63 6965 735b  ord_frequencies[
+00012c20: 776f 7264 5d0d 0a20 2020 2020 2020 2020  word]..         
+00012c30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00012c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012c50: 2020 2020 2020 2020 2020 7365 6e74 656e            senten
+00012c60: 6365 5f73 636f 7265 735b 7365 6e74 5d20  ce_scores[sent] 
+00012c70: 2b3d 2077 6f72 645f 6672 6571 7565 6e63  += word_frequenc
+00012c80: 6965 735b 776f 7264 5d0d 0a0d 0a20 2020  ies[word]....   
+00012c90: 2023 7072 696e 7428 7365 6e74 656e 6365   #print(sentence
+00012ca0: 5f73 636f 7265 7329 0d0a 0d0a 2020 2020  _scores)....    
+00012cb0: 7375 6d6d 6172 795f 7365 6e74 656e 6365  summary_sentence
+00012cc0: 7320 3d20 6865 6170 712e 6e6c 6172 6765  s = heapq.nlarge
+00012cd0: 7374 2869 2c20 7365 6e74 656e 6365 5f73  st(i, sentence_s
+00012ce0: 636f 7265 732c 206b 6579 3d73 656e 7465  cores, key=sente
+00012cf0: 6e63 655f 7363 6f72 6573 2e67 6574 290d  nce_scores.get).
+00012d00: 0a20 2020 2023 7072 696e 7428 7375 6d6d  .    #print(summ
+00012d10: 6172 795f 7365 6e74 656e 6365 7329 0d0a  ary_sentences)..
+00012d20: 2020 2020 7375 6d6d 6172 7920 3d20 2720      summary = ' 
+00012d30: 272e 6a6f 696e 2873 756d 6d61 7279 5f73  '.join(summary_s
+00012d40: 656e 7465 6e63 6573 290d 0a20 2020 2023  entences)..    #
+00012d50: 7072 696e 7428 2241 4920 5375 6d6d 6172  print("AI Summar
+00012d60: 7922 290d 0a20 2020 2072 6574 7572 6e20  y")..    return 
+00012d70: 7375 6d6d 6172 790d 0a0d 0a64 6566 2073  summary....def s
+00012d80: 7461 7274 7375 6d6d 6172 7928 6172 7469  tartsummary(arti
+00012d90: 636c 655f 7465 7874 2c66 7661 6c75 652c  cle_text,fvalue,
+00012da0: 6d61 786b 6579 776f 7264 7329 3a0d 0a20  maxkeywords):.. 
+00012db0: 2020 2020 200d 0a20 2320 7472 793a 0d0a       .. # try:..
+00012dc0: 2020 206f 7269 6769 6e61 6c77 6f72 6473     originalwords
+00012dd0: 203d 206c 656e 2861 7274 6963 6c65 5f74   = len(article_t
+00012de0: 6578 742e 7370 6c69 7428 2220 2229 290d  ext.split(" ")).
+00012df0: 0a0d 0a20 2020 666f 7220 6920 696e 2072  ...   for i in r
+00012e00: 616e 6765 2831 2c31 3030 3030 293a 0d0a  ange(1,10000):..
+00012e10: 2020 2020 2073 756d 6d61 7279 3d64 6f73       summary=dos
+00012e20: 756d 6d61 7279 2861 7274 6963 6c65 5f74  ummary(article_t
+00012e30: 6578 742c 6929 0d0a 2020 2020 2072 6573  ext,i)..     res
+00012e40: 203d 206c 656e 2873 756d 6d61 7279 2e73   = len(summary.s
+00012e50: 706c 6974 2829 290d 0a20 2020 2020 6966  plit())..     if
+00012e60: 2072 6573 203e 3d20 6676 616c 7565 3a0d   res >= fvalue:.
+00012e70: 0a20 2020 2020 2020 2020 6272 6561 6b0d  .         break.
+00012e80: 0a0d 0a20 2020 7375 6d6d 6172 7920 3d20  ...   summary = 
+00012e90: 2072 652e 7375 6228 225c 5c5c 5c78 5b61   re.sub("\\\\x[a
+00012ea0: 2d66 302d 395d 5b61 2d66 302d 395d 222c  -f0-9][a-f0-9]",
+00012eb0: 2022 2022 2c73 756d 6d61 7279 290d 0a20   " ",summary).. 
+00012ec0: 2020 7375 6d6d 6172 7920 3d20 7265 2e73    summary = re.s
+00012ed0: 7562 2822 5c5c 7865 325c 5c78 3830 5c5c  ub("\\xe2\\x80\\
+00012ee0: 7839 3922 2c22 2722 2c20 7375 6d6d 6172  x99","'", summar
+00012ef0: 7929 0d0a 2020 2073 756d 6d61 7279 3d73  y)..   summary=s
+00012f00: 756d 6d61 7279 2e72 6570 6c61 6365 2822  ummary.replace("
+00012f10: 5c5c 7865 325c 5c78 3830 5c5c 7839 3922  \\xe2\\x80\\x99"
+00012f20: 2c22 2722 290d 0a20 2020 7375 6d6d 6172  ,"'")..   summar
+00012f30: 793d 7375 6d6d 6172 792e 7265 706c 6163  y=summary.replac
+00012f40: 6528 225c 5c78 6532 5c5c 7838 305c 5c78  e("\\xe2\\x80\\x
+00012f50: 3930 222c 222d 2229 0d0a 2020 2073 756d  90","-")..   sum
+00012f60: 6d61 7279 3d73 756d 6d61 7279 2e72 6570  mary=summary.rep
+00012f70: 6c61 6365 2822 5c5c 7865 325c 5c78 3830  lace("\\xe2\\x80
+00012f80: 5c5c 7839 3122 2c22 2d22 290d 0a20 2020  \\x91","-")..   
+00012f90: 7375 6d6d 6172 793d 7375 6d6d 6172 792e  summary=summary.
+00012fa0: 7265 706c 6163 6528 225c 5c78 6532 5c5c  replace("\\xe2\\
+00012fb0: 7838 305c 5c78 3932 222c 222d 2229 0d0a  x80\\x92","-")..
+00012fc0: 2020 2073 756d 6d61 7279 3d73 756d 6d61     summary=summa
+00012fd0: 7279 2e72 6570 6c61 6365 2822 5c5c 7865  ry.replace("\\xe
+00012fe0: 325c 5c78 3830 5c5c 7839 3322 2c22 2d22  2\\x80\\x93","-"
+00012ff0: 290d 0a20 2020 7375 6d6d 6172 793d 7375  )..   summary=su
+00013000: 6d6d 6172 792e 7265 706c 6163 6528 225c  mmary.replace("\
+00013010: 5c78 6532 5c5c 7838 305c 5c78 3934 222c  \xe2\\x80\\x94",
+00013020: 222d 2229 0d0a 2020 2073 756d 6d61 7279  "-")..   summary
+00013030: 3d73 756d 6d61 7279 2e72 6570 6c61 6365  =summary.replace
+00013040: 2822 5c5c 7865 325c 5c78 3830 5c5c 7839  ("\\xe2\\x80\\x9
+00013050: 3522 2c22 2d22 290d 0a20 2020 7375 6d6d  5","-")..   summ
+00013060: 6172 793d 7375 6d6d 6172 792e 7265 706c  ary=summary.repl
+00013070: 6163 6528 225c 5c78 6532 5c5c 7838 305c  ace("\\xe2\\x80\
+00013080: 5c78 6233 222c 2722 2729 0d0a 2020 2073  \xb3",'"')..   s
+00013090: 756d 6d61 7279 203d 2073 756d 6d61 7279  ummary = summary
+000130a0: 2e72 6570 6c61 6365 2827 e280 9c27 2c20  .replace('...', 
+000130b0: 2722 2729 0d0a 2020 2073 756d 6d61 7279  '"')..   summary
+000130c0: 203d 2073 756d 6d61 7279 2e72 6570 6c61   = summary.repla
+000130d0: 6365 2827 e280 9d27 2c20 2722 2729 0d0a  ce('...', '"')..
+000130e0: 2020 2073 756d 6d61 7279 203d 2073 756d     summary = sum
+000130f0: 6d61 7279 2e72 6570 6c61 6365 2827 e280  mary.replace('..
+00013100: 9927 2c20 2227 2229 0d0a 2020 2073 756d  .', "'")..   sum
+00013110: 6d61 7279 203d 2073 756d 6d61 7279 2e72  mary = summary.r
+00013120: 6570 6c61 6365 2827 e280 9827 2c20 2227  eplace('...', "'
+00013130: 2229 0d0a 2020 2073 756d 6d61 7279 203d  ")..   summary =
+00013140: 2073 756d 6d61 7279 2e72 6570 6c61 6365   summary.replace
+00013150: 2827 e280 9327 2c20 222d 2229 0d0a 2020  ('...', "-")..  
+00013160: 2073 756d 6d61 7279 203d 2073 756d 6d61   summary = summa
+00013170: 7279 2e72 6570 6c61 6365 2827 e280 a627  ry.replace('...'
+00013180: 2c20 222e 2e2e 2229 0d0a 2020 2073 756d  , "...")..   sum
+00013190: 6d61 7279 203d 2073 756d 6d61 7279 2e72  mary = summary.r
+000131a0: 6570 6c61 6365 2827 e280 9427 2c20 222d  eplace('...', "-
+000131b0: 2229 0d0a 2020 2073 756d 6d61 7279 203d  ")..   summary =
+000131c0: 2073 756d 6d61 7279 2e72 6570 6c61 6365   summary.replace
+000131d0: 2827 2227 2c20 2222 290d 0a0d 0a20 2020  ('"', "")....   
+000131e0: 7375 6d6d 6172 7920 3d20 7375 6d6d 6172  summary = summar
+000131f0: 792e 7265 706c 6163 6528 275c 5c75 272c  y.replace('\\u',
+00013200: 2755 2b27 290d 0a20 2020 7375 6d6d 6172  'U+')..   summar
+00013210: 7920 3d20 7265 2e73 7562 2872 273c 555c  y = re.sub(r'<U\
+00013220: 2b28 5b30 2d39 612d 6641 2d46 5d7b 342c  +([0-9a-fA-F]{4,
+00013230: 367d 293e 272c 206c 616d 6264 6120 783a  6})>', lambda x:
+00013240: 2063 6872 2869 6e74 2878 2e67 726f 7570   chr(int(x.group
+00013250: 2831 292c 3136 2929 2c20 7375 6d6d 6172  (1),16)), summar
+00013260: 7929 0d0a 0d0a 2020 206b 6579 776f 7264  y)....   keyword
+00013270: 733d 6765 746b 6579 776f 7264 7328 7375  s=getkeywords(su
+00013280: 6d6d 6172 792c 6d61 786b 6579 776f 7264  mmary,maxkeyword
+00013290: 7329 0d0a 0d0a 2020 2073 756d 6d61 7279  s)....   summary
+000132a0: 776f 7264 7320 3d20 6c65 6e28 7375 6d6d  words = len(summ
+000132b0: 6172 792e 7370 6c69 7428 2220 2229 290d  ary.split(" ")).
+000132c0: 0a20 0d0a 2020 206d 6169 6e6f 7574 3d22  . ..   mainout="
+000132d0: 5c22 2220 2b20 6b65 7977 6f72 6473 202b  \"" + keywords +
+000132e0: 2022 5c22 2c5c 226f 7269 6769 6e61 6c77   "\",\"originalw
+000132f0: 6f72 6463 6f75 6e74 5c22 3a22 202b 2073  ordcount\":" + s
+00013300: 7472 286f 7269 6769 6e61 6c77 6f72 6473  tr(originalwords
+00013310: 2920 2b20 222c 5c22 7375 6d6d 6172 7977  ) + ",\"summaryw
+00013320: 6f72 6463 6f75 6e74 5c22 3a22 2b20 7374  ordcount\":"+ st
+00013330: 7228 7375 6d6d 6172 7977 6f72 6473 2920  r(summarywords) 
+00013340: 2b22 2c5c 226d 6169 6e73 756d 6d61 7279  +",\"mainsummary
+00013350: 5c22 3a7b 5c22 7375 6d6d 6172 795c 223a  \":{\"summary\":
+00013360: 205c 2222 202b 2073 756d 6d61 7279 202b   \"" + summary +
+00013370: 2022 5c22 7d7d 220d 0a20 2020 7265 7475   "\"}}"..   retu
+00013380: 726e 206d 6169 6e6f 7574 0d0a 2020 200d  rn mainout..   .
+00013390: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+000133a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000133b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000133c0: 2323 0d0a 0d0a 6672 6f6d 206c 616e 6763  ##....from langc
+000133d0: 6861 696e 2e65 6d62 6564 6469 6e67 732e  hain.embeddings.
+000133e0: 6f70 656e 6169 2069 6d70 6f72 7420 4f70  openai import Op
+000133f0: 656e 4149 456d 6265 6464 696e 6773 0d0a  enAIEmbeddings..
+00013400: 6672 6f6d 206c 616e 6763 6861 696e 2e74  from langchain.t
+00013410: 6578 745f 7370 6c69 7474 6572 2069 6d70  ext_splitter imp
+00013420: 6f72 7420 4368 6172 6163 7465 7254 6578  ort CharacterTex
+00013430: 7453 706c 6974 7465 720d 0a66 726f 6d20  tSplitter..from 
+00013440: 6c61 6e67 6368 6169 6e2e 7665 6374 6f72  langchain.vector
+00013450: 7374 6f72 6573 2e66 6169 7373 2069 6d70  stores.faiss imp
+00013460: 6f72 7420 4641 4953 530d 0a0d 0a66 726f  ort FAISS....fro
+00013470: 6d20 6c61 6e67 6368 6169 6e2e 6368 6169  m langchain.chai
+00013480: 6e73 2e71 7565 7374 696f 6e5f 616e 7377  ns.question_answ
+00013490: 6572 696e 6720 696d 706f 7274 206c 6f61  ering import loa
+000134a0: 645f 7161 5f63 6861 696e 0d0a 6672 6f6d  d_qa_chain..from
+000134b0: 206c 616e 6763 6861 696e 2e6c 6c6d 7320   langchain.llms 
+000134c0: 696d 706f 7274 2050 726f 6d70 744c 6179  import PromptLay
+000134d0: 6572 4f70 656e 4149 4368 6174 0d0a 6672  erOpenAIChat..fr
+000134e0: 6f6d 206c 616e 6763 6861 696e 2e63 6861  om langchain.cha
+000134f0: 745f 6d6f 6465 6c73 2069 6d70 6f72 7420  t_models import 
+00013500: 4368 6174 4f70 656e 4149 0d0a 6672 6f6d  ChatOpenAI..from
+00013510: 206c 616e 6763 6861 696e 2e6c 6c6d 7320   langchain.llms 
+00013520: 696d 706f 7274 204f 7065 6e41 490d 0a69  import OpenAI..i
+00013530: 6d70 6f72 7420 6861 7368 6c69 620d 0a0d  mport hashlib...
+00013540: 0a23 2041 6e73 7765 7220 7175 6573 7469  .# Answer questi
+00013550: 6f6e 7320 6162 6f75 7420 7468 6520 6865  ons about the he
+00013560: 6164 6c69 6e65 730d 0a64 6566 2073 7461  adlines..def sta
+00013570: 7274 5f63 6f6e 7665 7273 6174 696f 6e28  rt_conversation(
+00013580: 6f70 656e 6169 6b65 792c 7175 6572 792c  openaikey,query,
+00013590: 7465 7874 2c74 656d 7065 7261 7475 7265  text,temperature
+000135a0: 2c6d 6f64 656c 293a 0d0a 2020 2020 2320  ,model):..    # 
+000135b0: 4772 6162 2074 6865 2069 6e70 7574 2066  Grab the input f
+000135c0: 726f 6d20 7468 6520 4150 490d 0a20 2020  rom the API..   
+000135d0: 2020 2020 2023 7175 6572 7920 3d20 696e       #query = in
+000135e0: 7075 7473 5b22 7175 6572 7922 0d0a 0d0a  puts["query"....
+000135f0: 0d0a 2020 2020 2020 2020 7465 7874 5f73  ..        text_s
+00013600: 706c 6974 7465 7220 3d20 4368 6172 6163  plitter = Charac
+00013610: 7465 7254 6578 7453 706c 6974 7465 7228  terTextSplitter(
+00013620: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00013630: 7061 7261 746f 723d 2220 222c 0d0a 2020  parator=" ",..  
+00013640: 2020 2020 2020 2020 2020 6368 756e 6b5f            chunk_
+00013650: 7369 7a65 3d31 3030 302c 0d0a 2020 2020  size=1000,..    
+00013660: 2020 2020 2020 2020 6368 756e 6b5f 6f76          chunk_ov
+00013670: 6572 6c61 703d 3230 302c 0d0a 2020 2020  erlap=200,..    
+00013680: 2020 2020 2020 2020 6c65 6e67 7468 5f66          length_f
+00013690: 756e 6374 696f 6e3d 6c65 6e2c 0d0a 2020  unction=len,..  
+000136a0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+000136b0: 2020 2074 6578 7473 203d 2074 6578 745f     texts = text_
+000136c0: 7370 6c69 7474 6572 2e73 706c 6974 5f74  splitter.split_t
+000136d0: 6578 7428 7465 7874 290d 0a20 2020 2020  ext(text)..     
+000136e0: 2020 2065 6d62 6564 6469 6e67 7320 3d20     embeddings = 
+000136f0: 4f70 656e 4149 456d 6265 6464 696e 6773  OpenAIEmbeddings
+00013700: 2829 0d0a 2020 2020 2020 2020 646f 6373  ()..        docs
+00013710: 6561 7263 6820 3d20 4641 4953 532e 6672  earch = FAISS.fr
+00013720: 6f6d 5f74 6578 7473 2874 6578 7473 2c20  om_texts(texts, 
+00013730: 656d 6265 6464 696e 6773 290d 0a20 2020  embeddings)..   
+00013740: 2020 2020 2064 6f63 7320 3d20 646f 6373       docs = docs
+00013750: 6561 7263 682e 7369 6d69 6c61 7269 7479  earch.similarity
+00013760: 5f73 6561 7263 6828 7175 6572 7929 0d0a  _search(query)..
+00013770: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00013780: 2020 6368 6169 6e20 3d20 6c6f 6164 5f71    chain = load_q
+00013790: 615f 6368 6169 6e28 4f70 656e 4149 286d  a_chain(OpenAI(m
+000137a0: 6f64 656c 5f6e 616d 653d 6d6f 6465 6c2c  odel_name=model,
+000137b0: 2074 656d 7065 7261 7475 7265 3d74 656d   temperature=tem
+000137c0: 7065 7261 7475 7265 2c6f 7065 6e61 695f  perature,openai_
+000137d0: 6170 695f 6b65 793d 6f70 656e 6169 6b65  api_key=openaike
+000137e0: 7929 2c20 6368 6169 6e5f 7479 7065 3d22  y), chain_type="
+000137f0: 7374 7566 6622 290d 0a20 2020 2020 2020  stuff")..       
+00013800: 2072 6573 203d 2063 6861 696e 287b 2269   res = chain({"i
+00013810: 6e70 7574 5f64 6f63 756d 656e 7473 223a  nput_documents":
+00013820: 2064 6f63 732c 2022 7175 6573 7469 6f6e   docs, "question
+00013830: 223a 2071 7565 7279 7d2c 2072 6574 7572  ": query}, retur
+00013840: 6e5f 6f6e 6c79 5f6f 7574 7075 7473 3d54  n_only_outputs=T
+00013850: 7275 6529 0d0a 0d0a 2020 2020 2020 2020  rue)....        
+00013860: 2372 6574 7572 6e20 7b22 7072 6564 223a  #return {"pred":
+00013870: 2072 6573 7d0d 0a20 2020 2020 2020 2072   res}..        r
+00013880: 6574 7572 6e20 7265 730d 0a0d 0a23 2323  eturn res....###
+00013890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000138a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000138b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000138c0: 230d 0a66 726f 6d20 7064 6671 7565 7279  #..from pdfquery
+000138d0: 2069 6d70 6f72 7420 5044 4651 7565 7279   import PDFQuery
+000138e0: 0d0a 696d 706f 7274 2078 6d6c 746f 6469  ..import xmltodi
+000138f0: 6374 0d0a 0d0a 0d0a 6465 6620 6c61 6265  ct......def labe
+00013900: 6c66 6965 6c64 7328 6669 6c65 6e61 6d65  lfields(filename
+00013910: 2c6c 6162 656c 6e61 6d65 2c61 6372 6f74  ,labelname,acrot
+00013920: 7970 6529 3a0d 0a20 2020 2020 7064 6620  ype):..     pdf 
+00013930: 3d20 5044 4651 7565 7279 2866 696c 656e  = PDFQuery(filen
+00013940: 616d 6529 0d0a 2020 2020 2070 6466 2e6c  ame)..     pdf.l
+00013950: 6f61 6428 290d 0a20 2020 2020 234c 5454  oad()..     #LTT
+00013960: 6578 744c 696e 6548 6f72 697a 6f6e 7461  extLineHorizonta
+00013970: 6c0d 0a20 2020 2020 6c61 6265 6c20 3d20  l..     label = 
+00013980: 7064 662e 7071 2861 6372 6f74 7970 652b  pdf.pq(acrotype+
+00013990: 273a 636f 6e74 6169 6e73 2822 272b 6c61  ':contains("'+la
+000139a0: 6265 6c6e 616d 6520 2b20 2722 2927 290d  belname + '")').
+000139b0: 0a20 2020 2020 6c65 6674 5f63 6f72 6e65  .     left_corne
+000139c0: 7220 3d20 666c 6f61 7428 6c61 6265 6c2e  r = float(label.
+000139d0: 6174 7472 2827 7830 2729 290d 0a20 2020  attr('x0'))..   
+000139e0: 2020 626f 7474 6f6d 5f63 6f72 6e65 7220    bottom_corner 
+000139f0: 3d20 666c 6f61 7428 6c61 6265 6c2e 6174  = float(label.at
+00013a00: 7472 2827 7930 2729 290d 0a20 2020 2020  tr('y0'))..     
+00013a10: 6e61 6d65 203d 2070 6466 2e70 7128 6163  name = pdf.pq(ac
+00013a20: 726f 7479 7065 202b 273a 696e 5f62 626f  rotype +':in_bbo
+00013a30: 7828 2225 732c 2025 732c 2025 732c 2025  x("%s, %s, %s, %
+00013a40: 7322 2927 2025 2028 6c65 6674 5f63 6f72  s")' % (left_cor
+00013a50: 6e65 722c 2062 6f74 746f 6d5f 636f 726e  ner, bottom_corn
+00013a60: 6572 2d33 302c 206c 6566 745f 636f 726e  er-30, left_corn
+00013a70: 6572 2b31 3530 2c20 626f 7474 6f6d 5f63  er+150, bottom_c
+00013a80: 6f72 6e65 7229 292e 7465 7874 2829 0d0a  orner)).text()..
+00013a90: 2020 2020 2072 6574 7572 6e20 6e61 6d65       return name
+00013aa0: 0d0a 0d0a 0d0a 6465 6620 6578 7472 6163  ......def extrac
+00013ab0: 7466 6965 6c64 7328 6669 6c65 6e61 6d65  tfields(filename
+00013ac0: 293a 0d0a 2020 2020 2020 2372 6561 6420  ):..      #read 
+00013ad0: 7468 6520 5044 460d 0a20 2020 2020 2070  the PDF..      p
+00013ae0: 6466 203d 2050 4446 5175 6572 7928 6669  df = PDFQuery(fi
+00013af0: 6c65 6e61 6d65 290d 0a20 2020 2020 2070  lename)..      p
+00013b00: 6466 2e6c 6f61 6428 290d 0a0d 0a20 2020  df.load()....   
+00013b10: 2020 2023 6f20 3d20 786d 6c74 6f64 6963     #o = xmltodic
+00013b20: 742e 7061 7273 6528 273c 653e 203c 613e  t.parse('<e> <a>
+00013b30: 7465 7874 3c2f 613e 203c 613e 7465 7874  text</a> <a>text
+00013b40: 3c2f 613e 203c 2f65 3e27 290d 0a0d 0a20  </a> </e>').... 
+00013b50: 2020 2020 2023 636f 6e76 6572 7420 7468       #convert th
+00013b60: 6520 7064 6620 746f 2058 4d4c 0d0a 2020  e pdf to XML..  
+00013b70: 2020 2020 786d 6c66 696c 653d 2066 696c      xmlfile= fil
+00013b80: 656e 616d 6520 2b20 272e 786d 6c27 0d0a  ename + '.xml'..
+00013b90: 2020 2020 2020 7064 662e 7472 6565 2e77        pdf.tree.w
+00013ba0: 7269 7465 2878 6d6c 6669 6c65 2c20 7072  rite(xmlfile, pr
+00013bb0: 6574 7479 5f70 7269 6e74 203d 2054 7275  etty_print = Tru
+00013bc0: 6529 0d0a 2020 2020 2020 7769 7468 206f  e)..      with o
+00013bd0: 7065 6e28 786d 6c66 696c 6529 2061 7320  pen(xmlfile) as 
+00013be0: 663a 2073 203d 2066 2e72 6561 6428 290d  f: s = f.read().
+00013bf0: 0a0d 0a20 2020 2020 2023 7072 696e 7428  ...      #print(
+00013c00: 7329 0d0a 2020 2020 2020 6a73 6f6e 6275  s)..      jsonbu
+00013c10: 663d 786d 6c74 6f6a 736f 6e28 732c 786d  f=xmltojson(s,xm
+00013c20: 6c66 696c 6529 0d0a 0d0a 2020 2020 2020  lfile)....      
+00013c30: 7265 7475 726e 206a 736f 6e62 7566 0d0a  return jsonbuf..
+00013c40: 2020 2020 2020 0d0a 0d0a 6465 6620 786d        ....def xm
+00013c50: 6c74 6f6a 736f 6e28 786d 6c62 7566 6665  ltojson(xmlbuffe
+00013c60: 722c 786d 6c66 696c 6529 3a0d 0a0d 0a20  r,xmlfile):.... 
+00013c70: 2020 2020 206f 203d 2078 6d6c 746f 6469       o = xmltodi
+00013c80: 6374 2e70 6172 7365 2878 6d6c 6275 6666  ct.parse(xmlbuff
+00013c90: 6572 290d 0a20 2020 2020 2078 6d6c 6a73  er)..      xmljs
+00013ca0: 6f6e 3d6a 736f 6e2e 6475 6d70 7328 6f29  on=json.dumps(o)
+00013cb0: 0d0a 2020 2020 2020 2370 7269 6e74 2878  ..      #print(x
+00013cc0: 6d6c 6a73 6f6e 290d 0a20 2020 2020 2077  mljson)..      w
+00013cd0: 6974 6820 6f70 656e 2878 6d6c 6669 6c65  ith open(xmlfile
+00013ce0: 202b 2027 2e6a 736f 6e27 2c22 7722 2920   + '.json',"w") 
+00013cf0: 6173 2066 3a0d 0a20 2020 2020 2020 2066  as f:..        f
+00013d00: 2e77 7269 7465 2878 6d6c 6a73 6f6e 290d  .write(xmljson).
+00013d10: 0a0d 0a20 2020 2020 2072 6574 7572 6e20  ...      return 
+00013d20: 786d 6c6a 736f 6e20 200d 0a0d 0a         xmljson  ....
```

### Comparing `maadstml-3.38/maadstml/tmltextsummary.py` & `maadstml-3.39/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.38/maadstml.egg-info/PKG-INFO` & `maadstml-3.39/maadstml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.38
+Version: 3.39
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -253,23 +253,14 @@
 
 - **viperexractpdffields**
   - Extracts fields from PDF file
 
 - **viperexractpdffieldbylabel**
   - Extracts fields from PDF file by label name.
 
-- **viperimagetotext**
-  - Extracts text from images like PNG, JPG, etc., which can then be streamed to kafka.
-
-- **viperaudiototext**
-  - Extracts text from audio files like WAV, etc., which can then be streamed to kafka.
-
-- **vipervideototext**
-  - Extracts text from video files like MP4, etc., which can then be streamed to kafka.
-
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
```

### Comparing `maadstml-3.38/setup.py` & `maadstml-3.39/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.38',
+    version='3.39',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

