# Comparing `tmp/clubscore-0.2.2.tar.gz` & `tmp/clubscore-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clubscore-0.2.2.tar", last modified: Fri Jun  9 18:10:05 2023, max compression
+gzip compressed data, was "clubscore-0.2.3.tar", last modified: Sat Jun 24 15:34:53 2023, max compression
```

## Comparing `clubscore-0.2.2.tar` & `clubscore-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 18:10:05.190611 clubscore-0.2.2/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.2.2/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-09 18:10:05.190225 clubscore-0.2.2/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.2.2/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 18:10:05.180339 clubscore-0.2.2/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.2.2/clubscore/API.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.2/clubscore/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     4453 2023-06-09 18:06:40.000000 clubscore-0.2.2/clubscore/bot.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 18:10:05.187892 clubscore-0.2.2/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.2.2/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.2.2/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.2.2/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     3966 2023-05-16 22:26:38.000000 clubscore-0.2.2/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.2/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     4237 2023-06-09 15:50:58.000000 clubscore-0.2.2/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 18:10:05.183991 clubscore-0.2.2/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-09 18:10:05.000000 clubscore-0.2.2/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      452 2023-06-09 18:10:05.000000 clubscore-0.2.2/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-06-09 18:10:05.000000 clubscore-0.2.2/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-06-09 18:10:05.000000 clubscore-0.2.2/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-06-09 18:10:05.000000 clubscore-0.2.2/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-06-09 18:10:05.190767 clubscore-0.2.2/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-06-09 18:06:57.000000 clubscore-0.2.2/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 18:10:05.189196 clubscore-0.2.2/tests/
--rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.2.2/tests/test_templates.py
--rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.275006 clubscore-0.2.3/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.2.3/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-24 15:34:53.274412 clubscore-0.2.3/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.2.3/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.261828 clubscore-0.2.3/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)     1206 2023-06-24 15:29:38.000000 clubscore-0.2.3/clubscore/API.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.3/clubscore/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     5159 2023-06-24 13:56:51.000000 clubscore-0.2.3/clubscore/bot.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.272076 clubscore-0.2.3/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     5435 2023-06-24 11:41:29.000000 clubscore-0.2.3/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     3171 2023-06-24 14:23:56.000000 clubscore-0.2.3/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1161 2023-06-24 10:52:02.000000 clubscore-0.2.3/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     4241 2023-06-24 13:03:31.000000 clubscore-0.2.3/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.3/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     6333 2023-06-24 14:44:16.000000 clubscore-0.2.3/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.266713 clubscore-0.2.3/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      452 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-06-24 15:34:53.275134 clubscore-0.2.3/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-06-24 15:19:52.000000 clubscore-0.2.3/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.273607 clubscore-0.2.3/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1966 2023-06-24 14:08:30.000000 clubscore-0.2.3/tests/test_templates.py
+-rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.2.3/tests/test_utils.py
```

### Comparing `clubscore-0.2.2/LICENSE` & `clubscore-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.2/PKG-INFO` & `clubscore-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.2.2/clubscore/bot.py` & `clubscore-0.2.3/clubscore/bot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import telebot
 from clubscore.objects.CONTAINER import *
-from clubscore.API import getRoundRobinStandings
+import importlib
 import xml.etree.ElementTree as ET
 from io import BytesIO
 import clubscore.utils as u
 import json
 import traceback
 import requests
 
@@ -47,30 +47,52 @@
 
     def update_status(message):
         d[message.from_user.id] = message.text.replace('/', '')
 
     @bot.message_handler(commands=['start'])
     def start(message):
         update_status(message)
-        bot.send_message(message.chat.id, "TESTBOTMANAGER")
+        bot.send_message(message.chat.id, f"Welcome in {BOT}! A Clubscore product!")
+        help(message)
+
+    @bot.message_handler(commands=['teams'])
+    def teams(message):
+        bot.send_message(message.chat.id, u.print_file_tree("teams"))
+
+    @bot.message_handler(commands=['help'])
+    def help(message):
+        s = "You have the following commands:\n\n"
+        for e in sorted(comandi_elite):
+            s += "/" + e + "\n"
+        for e in sorted(singleapi):
+            s += "/" + e + "\n"
+        bot.send_message(message.chat.id, s)
+
 
     @bot.message_handler(commands=[k for k in comandi_elite])
     def risultati(message):
         m = message.text.replace('/', '')
         template = comandi_elite[m]
         print(template)
         update_status(message)
         bot.send_message(message.chat.id, u.getTemplateGuide(template))
 
     @bot.message_handler(commands=[k for k in singleapi])
     def risultati(message):
         m = message.text.replace('/', '')
         template = singleapi[m]
-        print(template,m)
-        lista = getRoundRobinStandings("l6jdjhakox")
+
+        function_name = u.getTemplateText(template, "API").strip()
+        params = u.getTemplateText(template, "PARAMETERS").strip().split("\n")
+
+        module_name = "clubscore.API"
+        module = importlib.import_module(module_name)
+        function = getattr(module, function_name)
+
+        lista = function(*params)
 
         root = ET.parse(template).getroot()
         width = int(root.attrib["width"])
         height = int(root.attrib["height"])
 
         image = Image.new('RGB', (width, height), color=(255, 255, 255))
         CONTAINER.interpretaTemplate(image, template, lista)
```

### Comparing `clubscore-0.2.2/clubscore/objects/CONTAINER.py` & `clubscore-0.2.3/clubscore/objects/CONTAINER.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 
 
     """
     costruttore a partire da dizionario XML dell'oggetto
     """
 
     @staticmethod
-    def initiate(image, root, dict, lines):
+    def initiate(image, root, dict, lines, template):
+
+        if dict["ref"][0] == ".":
+            dict["ref"] = u.fix_path(dict["ref"],template)
 
         if "requires_line" in dict:
             info_container = lines.pop(0).strip().split(",")
 
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
@@ -49,15 +52,15 @@
         elements = CONTAINER.interpretaTemplate(image, dict["ref"], info_container)
 
         return CONTAINER(image, x + int(dict["x"]), y + int(dict["y"]), width, height, elements)
 
 
 
     @staticmethod
-    def initiateMultiple(image, root, el, lines):
+    def initiateMultiple(image, root, el, lines, template):
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
         dict = el.attrib
 
         width = 0 if "width" not in dict else int(dict["width"])
         height = 0 if "height" not in dict else int(dict["height"])
@@ -117,28 +120,29 @@
         height = 0 if "height" not in root.attrib else int(root.attrib["height"])
 
         elements = []
 
         for el in children:
 
             if el.tag == "IMG":
-                elements.append(IMG.initiate(image, root, el.attrib, lines))
+                elements.append(IMG.initiate(image, root, el.attrib, lines, template))
             elif el.tag == "TEXT":
-                elements.append(TEXT.initiate(image, root, el.attrib,lines))
+                elements.append(TEXT.initiate(image, root, el.attrib,lines, template))
             elif el.tag == "RECTANGLE":
-                elements.append(RECTANGLE.initiate(image, root, el.attrib))
+                elements.append(RECTANGLE.initiate(image, root, el.attrib, template))
             elif el.tag == "CONTAINER":
-                elements.append(CONTAINER.initiate(image, root, el.attrib,lines))
+                elements.append(CONTAINER.initiate(image, root, el.attrib,lines, template))
             elif el.tag == "MULTIPLE":
-                elements.append(CONTAINER.initiateMultiple(image, root, el,lines))
+                elements.append(CONTAINER.initiateMultiple(image, root, el,lines, template))
             elif el.tag == "COMBO":
                 #lista di appoggio per combo
                 info = lines.pop(0).strip().split(",") * len(list(el))
+                #print(info)
                 for k in list(el):
-                    elements.append(getattr(sys.modules[__name__], k.tag).initiate(image, root, k.attrib, info))
+                    elements.append(getattr(sys.modules[__name__], k.tag).initiate(image, root, k.attrib, info,template))
                 #elements.append(CONTAINER.initiateMultiple(image, root, el,lines))
 
 
 
         main_container = CONTAINER(image, x, y, width, height, elements)
 
         if root.tag == "MAIN_CONTAINER":
```

### Comparing `clubscore-0.2.2/clubscore/objects/IMG.py` & `clubscore-0.2.3/clubscore/objects/IMG.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 
     """
     image: immagine di background di riferimento
     foto: nome del file da recuperare (eventuale)
     x,y : coordinate
     width: larghezza immagine
     """
-    def __init__(self, image, foto, x, y, width, centerX=True, centerY=True):
+    def __init__(self, image, foto, x, y, width, centerX=True, centerY=True, rgb = None):
         self.image = image
         self.foto = foto
         self.x = x
         self.y = y
         self.width = width
         self.centerX = centerX
         self.centerY = centerY
+        self.rgb = rgb
 
     """
     inserisce la foto dentro l'image di riferimento, prima imposta la dimensione
     Restituisce l'altezza della foto
     """
     def inserisci(self, relative_x = 0, relative_y = 0):
 
@@ -31,14 +32,17 @@
             foto = Image.open(self.foto)
         else:
             foto = Image.open(BytesIO(self.foto)).convert("RGBA")
 
 
         png, w, h = u.diagonal_resize(foto, self.width)
 
+        if self.rgb is not None:
+            png = u.coloraPNG(png, self.rgb[0], self.rgb[1], self.rgb[2])
+
         if self.centerX:
             w = int(w/2)
         else:
             w = 0
 
         if self.centerY:
             h = int(h/2)
@@ -49,44 +53,58 @@
 
         return h
 
     """
     costruttore a partire da dizionario XML dell'oggetto
     """
     @staticmethod
-    def initiate(image, root, dict, lines):
+    def initiate(image, root, dict, lines, template):
+
+        rgb = None
+
+        #sostituzione del punto "locale" con il path assoluto
+        if dict["foto"][0] == ".":
+            dict["foto"] = u.fix_path(dict["foto"],template)
+
 
         if "+" in dict["foto"]:
             dict["foto"] = lines.pop(0).strip()
 
         else:
 
             if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
                 dict["foto"] = "../" + dict["foto"]
 
             if "*" in dict["foto"]:
                 testo = lines.pop(0).strip()
+                print(testo)
 
+                if "!" in testo:
+                    rgb = (255, 255, 255)
+                    testo.replace("!","")
+
+                elif "?" in testo:
+                    rgb = (0, 0, 0)
+                    testo.replace("?", "")
+
+
+                if dict["foto"] != "../*":
+                    #dovrebbe succedere sempre, tranne quando lancio il test di trasparenza
+                    path = dict["foto"].split("/*")[0]
+                    testo = u.matchWord(testo, u.getTeams(path))
+                    dict["foto"] = f"{path}/{testo}.png"
+                else:
+                    dict["foto"] = testo
 
-                path = dict["foto"].split("/*")[0]
-
-
-
-                testo = u.matchWord(testo, u.getTeams(path))
-
-                #dict["foto"] = dict["foto"].replace("*", testo)
-                dict["foto"] = f"{path}/{testo}.png"
-
-
+                print()
 
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
 
 
-
         centerX = True if "centerX" not in dict or dict["centerX"] is "True" else False
         centerY = True if "centerY" not in dict or dict["centerY"] is "True" else False
 
         width = int(root.attrib["width"]) if "width" not in dict else int(dict["width"])
 
-        return IMG(image, dict["foto"], x + int(dict["x"]), y + int(dict["y"]), width, centerX, centerY)
+        return IMG(image, dict["foto"], x + int(dict["x"]), y + int(dict["y"]), width, centerX, centerY, rgb)
```

### Comparing `clubscore-0.2.2/clubscore/objects/RECTANGLE.py` & `clubscore-0.2.3/clubscore/objects/RECTANGLE.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         draw = ImageDraw.Draw(self.image)
         draw.rectangle([(self.x + relative_x, self.y + relative_y), (self.x + self.width + relative_x, self.y + self.height + relative_y)], fill=self.color)
 
     """
         costruttore a partire da dizionario XML dell'oggetto
     """
     @staticmethod
-    def initiate(image, root, dict):
+    def initiate(image, root, dict, template):
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
 
         return RECTANGLE(image, x + int(dict["x"]), y + int(dict["y"]), int(dict["width"]), int(dict["height"]),dict["color"])
```

### Comparing `clubscore-0.2.2/clubscore/objects/TEXT.py` & `clubscore-0.2.3/clubscore/objects/TEXT.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,37 +9,41 @@
     test: testo da scrivere
     font_path: font di riferimento  da utilizzare (fornire path)
     x,y : coordinate
     size: size di partenza o size da applicare nel font
     color: colore da utilizzare nel testo
     """
 
-    def __init__(self, image, testo, font_path, x, y, size, color, centerX=True, centerY=True, perimeter_fill = -1):
+    def __init__(self, image, testo, font_path, x, y, size, color, centerX=True, centerY=True, perimeter_fill = -1, justify=None):
         self.image = image
         self.testo = testo
         self.font_path = font_path
         self.x = x
         self.y = y
         self.size = size
         self.color = color
         self.centerX = centerX
         self.centerY = centerY
         self.perimeter_fill = perimeter_fill
+        self.justify = justify
 
     """
     inserisce il testo in maniera agnostica, non sa nulla se non le coordinate, e la dimensione del font
     """
 
     def inserisci(self, relative_x = 0, relative_y = 0):
         if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
             self.font_path = "../" + self.font_path
 
         font = ImageFont.truetype(self.font_path, self.size)
         draw = ImageDraw.Draw(self.image)
 
+        if self.justify == "right":
+            self.x -= int(draw.textlength(self.testo, font))
+
         if self.centerX:
             w = int(draw.textlength(self.testo, font)/2)
         else:
             w = 0
 
         if self.centerY:
             h = int(font.getbbox(self.testo)[3]/2)
@@ -47,38 +51,40 @@
             h = 0
 
         if self.perimeter_fill == -1:
             draw.text((int(self.x + relative_x-w), int(self.y + relative_y-h)), self.testo, font=font, fill=self.color)
 
         else:
 
-
             total_text_width, total_text_height = draw.textsize(self.testo, font=font)
             width_difference = self.perimeter_fill - total_text_width
             gap_width = int(width_difference / (len(self.testo) - 1))
             xpos = self.x
             ypos = self.y
             for letter in self.testo:
                 draw.text((xpos, ypos), letter, self.color, font=font)
                 letter_width, letter_height = draw.textsize(letter, font=font)
                 xpos += letter_width + gap_width
 
     """
     costruttore a partire da dizionario XML dell'oggetto
     """
     @staticmethod
-    def initiate(image, root, dict, lines):
+    def initiate(image, root, dict, lines, template):
 
         if "testo" in dict:
             if "*" in dict["testo"]:
 
                 testo = lines.pop(0).strip()
 
                 if "match_word" in dict:
-                    print(dict["match_word"])
+
+                    if dict["match_word"][0] == ".":
+                        dict["match_word"] = u.fix_path(dict["match_word"], template)
+
                     testo = u.matchWord(testo, u.getTeamsFromTXT(dict["match_word"]))
 
                 if "upper" in dict and "True" in dict["upper"]:
                     testo = testo.upper()
 
                 dict["testo"] = dict["testo"].replace("*", testo)
 
@@ -88,15 +94,15 @@
 
             for i in range(len(lines)):
                 repl = "{%s}" % str(i)
                 if repl in dict["concatenation"]:
                     testo = lines[i].strip()
 
                     if "match_word" in dict:
-                        print(dict["match_word"])
+
                         testo = u.matchWord(testo, u.getTeamsFromTXT(dict["match_word"]))
 
                     if "upper" in dict and "True" in dict["upper"]:
                         testo = testo.upper()
 
                     dict["concatenation"] = dict["concatenation"].replace(repl, testo)
 
@@ -111,9 +117,10 @@
 
 
         perimeter_fill = -1 if "perimeter_fill" not in dict else int(dict["perimeter_fill"])
 
 
         centerX = True if "centerX" not in dict or dict["centerX"] is "True" else False
         centerY = True if "centerY" not in dict or dict["centerY"] is "True" else False
+        justify = None if "justify" not in dict else dict["justify"]
 
-        return TEXT(image, final_text, dict["font"], x + int(dict["x"]), y + int(dict["y"]), int(dict["size"]),dict["color"], centerX, centerY,perimeter_fill)
+        return TEXT(image, final_text, dict["font"], x + int(dict["x"]), y + int(dict["y"]), int(dict["size"]),dict["color"], centerX, centerY,perimeter_fill,justify)
```

### Comparing `clubscore-0.2.2/clubscore/utils.py` & `clubscore-0.2.3/clubscore/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import xml.etree.ElementTree as ET
 import difflib
 import os
 import requests
 import logging
 import os
 from bs4 import BeautifulSoup
-
+import glob
 
 # set the logging level (e.g. DEBUG, INFO, WARNING, ERROR)
 logging.basicConfig(level=logging.INFO)
 
 """
 Prende un file in formato PNG e lo colora completamente di
 un colore specifico in rgb.
@@ -57,15 +57,80 @@
 
     return font
 
 
 """
 
 """
+#sostituisce il . locale di un template con quello assoluto
+def fix_path(current_path, template_path):
+    if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
+        current_path = os.path.dirname(template_path)[3:] + current_path[1:]
+    else:
+        current_path = os.path.dirname(template_path) + current_path[1:]
+
+    return current_path
+
+
+def print_file_tree(folder_path, indent=''):
+    all_files = glob.glob(folder_path + "/**/*", recursive=True)
+
+    # Create a dictionary to store files grouped by folder_name
+    file_tree = {}
+
+    for file_path in all_files:
+        if os.path.isfile(file_path):
+            folder_name = os.path.basename(os.path.dirname(file_path))
+            file_name = os.path.basename(file_path)
+
+            # Group files by folder_name in the file_tree dictionary
+            if folder_name not in file_tree:
+                file_tree[folder_name] = []
+            file_tree[folder_name].append(file_name.replace(".png",""))
+
+    s = ""
+    # Recursively print the file tree structure
+    for folder_name, files in file_tree.items():
+        s += indent + folder_name + '/' +'\n'
+        print(indent + folder_name + '/')
+        for file_name in sorted(files):
+            print(indent + '  ' + file_name)
+            s += indent + '  ' + file_name + '\n'
+
+        s += "\n"
+
+    return s
+
+
+def get_all_teams(folder_path):
+    # Utilizza glob in modo ricorsivo per trovare tutti i file nella cartella e nelle sottocartelle
+    all_files = glob.glob(folder_path + "/**/*.png", recursive=True)
+
+    return(all_files)
+
+def fix_transparency_issue(png):
+    image = Image.open(png)
+    print(png, image.mode)
+    image = image.convert("RGBA")
+
+    pixel_data = image.getdata()
+    new_pixel_data = []
+
+    for pixel in pixel_data:
+        r, g, b, a = pixel
+
+        if a == 0 and (r != 0 or g != 0 or b != 0):
+            new_pixel_data.append((r, g, b, 255))
+        else:
+            new_pixel_data.append(pixel)
+
+    new_image = Image.new("RGBA", image.size)
+    new_image.putdata(new_pixel_data)
 
+    new_image.save(png)
 
 """
 presa una foto fa il resize rispettando il vincolo di larghezza
 """
 
 
 def diagonal_resize(foto, new_width, new_height=0):
@@ -101,15 +166,15 @@
 
 """
 Recupera la lista delle squadre di cui si hanno le grafiche
 """
 
 
 def getTeams(path):
-    return list(map(lambda elem: elem.replace('.png', ''), os.listdir(path)))
+    return [os.path.basename(elem).replace('.png', '') for elem in glob.glob(path + '/*.png')]
 
 def getTeamsFromTXT(path):
     if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
         path = "../" + path
 
     print(path)
```

### Comparing `clubscore-0.2.2/clubscore.egg-info/PKG-INFO` & `clubscore-0.2.3/clubscore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.2.2/setup.py` & `clubscore-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.2.2',
+    version='0.2.3',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

### Comparing `clubscore-0.2.2/tests/test_templates.py` & `clubscore-0.2.3/tests/test_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import json
 import importlib
 
 
 class TestImageTransparency(unittest.TestCase):
 
-    @parameterized.expand([(team) for team in u.getTeams("../teams")])
+    @parameterized.expand([(team) for team in u.get_all_teams("../teams")])
     def test_transparency_mask__(self, team):
         os.environ['ENV'] = 'testing'
 
         template = "templates/test/main.xml"
 
         image = CONTAINER.CONTAINER.create_image_from_template(template, [team])
```

### Comparing `clubscore-0.2.2/tests/test_utils.py` & `clubscore-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

