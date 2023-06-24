# Comparing `tmp/Droplet_Detector-0.1.2.tar.gz` & `tmp/Droplet_Detector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Droplet_Detector-0.1.2.tar", last modified: Sat Jun 24 06:49:32 2023, max compression
+gzip compressed data, was "Droplet_Detector-0.1.3.tar", last modified: Sat Jun 24 06:57:40 2023, max compression
```

## Comparing `Droplet_Detector-0.1.2.tar` & `Droplet_Detector-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:49:32.198257 Droplet_Detector-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:49:32.198257 Droplet_Detector-0.1.2/Droplet_Detector/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/Droplet_Detector/Bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/Droplet_Detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/Droplet_Detector/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/Droplet_Detector/do_xslx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/Droplet_Detector/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/Droplet_Detector/get_contours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:49:32.198257 Droplet_Detector-0.1.2/Droplet_Detector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-24 06:49:32.000000 Droplet_Detector-0.1.2/Droplet_Detector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-24 06:49:32.000000 Droplet_Detector-0.1.2/Droplet_Detector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:49:32.000000 Droplet_Detector-0.1.2/Droplet_Detector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-24 06:49:32.000000 Droplet_Detector-0.1.2/Droplet_Detector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 06:49:32.000000 Droplet_Detector-0.1.2/Droplet_Detector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-24 06:49:32.198257 Droplet_Detector-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:49:32.198257 Droplet_Detector-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-24 06:48:46.000000 Droplet_Detector-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:57:40.950952 Droplet_Detector-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:57:40.946952 Droplet_Detector-0.1.3/Droplet_Detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/Droplet_Detector/Bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/Droplet_Detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/Droplet_Detector/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/Droplet_Detector/do_xslx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/Droplet_Detector/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/Droplet_Detector/get_contours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:57:40.950952 Droplet_Detector-0.1.3/Droplet_Detector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-24 06:57:40.000000 Droplet_Detector-0.1.3/Droplet_Detector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-24 06:57:40.000000 Droplet_Detector-0.1.3/Droplet_Detector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:57:40.000000 Droplet_Detector-0.1.3/Droplet_Detector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-24 06:57:40.000000 Droplet_Detector-0.1.3/Droplet_Detector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 06:57:40.000000 Droplet_Detector-0.1.3/Droplet_Detector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-24 06:57:40.950952 Droplet_Detector-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:57:40.950952 Droplet_Detector-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-24 06:56:43.000000 Droplet_Detector-0.1.3/setup.py
```

### Comparing `Droplet_Detector-0.1.2/Droplet_Detector/Bot.py` & `Droplet_Detector-0.1.3/Droplet_Detector/Bot.py`

 * *Files identical despite different names*

### Comparing `Droplet_Detector-0.1.2/Droplet_Detector/do_xslx.py` & `Droplet_Detector-0.1.3/Droplet_Detector/do_xslx.py`

 * *Files identical despite different names*

### Comparing `Droplet_Detector-0.1.2/Droplet_Detector/draw.py` & `Droplet_Detector-0.1.3/Droplet_Detector/draw.py`

 * *Files identical despite different names*

### Comparing `Droplet_Detector-0.1.2/Droplet_Detector/get_contours.py` & `Droplet_Detector-0.1.3/Droplet_Detector/get_contours.py`

 * *Files identical despite different names*

### Comparing `Droplet_Detector-0.1.2/Droplet_Detector.egg-info/PKG-INFO` & `Droplet_Detector-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,121 @@
 Metadata-Version: 2.1
-Name: Droplet-Detector
-Version: 0.1.2
+Name: Droplet_Detector
+Version: 0.1.3
 Summary: Telegram bot that draws the outlines of drips on a photo !!! Warning!!!  Before running, be sure to create the folders "exel", "new_file" and "save_docs" in the workspace where the python file is located !!!!
 Home-page: https://github.com/kvasik3000/Droplet-Detector
 Author: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 Author-email: superadrenoline3000@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
-Description: # Droplet-Detector
-        
-        ![droplet](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/c1928e58-414d-49ef-97dd-20d10441bfd5)
-        
-        ---
-        
-        ![Build Status](https://github.com/kvasik3000/Droplet-Detector/actions/workflows/python-app.yml/badge.svg?branch=main)
-        <img src = "https://img.shields.io/badge/Code%20Coverage-80%25-success?">
-        <img src = 'https://img.shields.io/github/contributors/kvasik3000/Droplet-Detector?'>  
-        <img src ='https://img.shields.io/github/repo-size/kvasik3000/Droplet-Detector?'>
-        
-        ---
-        
-        ## Введение
-        Перед нашей командой стояла задача создать простой в использовании проект, который будет рисовать контуры капель. Также было необходимо написать код для подсчёта пикселей каждой капли и добавить возможность сохранять данные в виде таблицы. Эта работа позволила нам глубже изучить компьютерное зрение с помощью библиотек **OpenCV2** в Python, научиться работать в команде и дала возможность создать собственного телеграмм-бота.
-        
-        ### Работу выполнили студенты из группы 21932:
-        
-        - [Квас Андрей](https://github.com/kvasik3000)
-        - [Некрасова Анна](https://github.com/NekrasovaAnn)
-        - [Белькова Ксения](https://github.com/didilovu)
-        
-        ## Обнаружение контуров
-        
-        Для корректного обнаружения контуров капель мы использовали **Canny Edge**. Это алгоритм, состоящий из 4 основных шагов:
-        
-        1. Уменьшение шума с помощью гауссовского сглаживания.
-        2. Вычисление градиента изображения с помощью фильтра Собеля.
-        3. Применение Non-Max Suppression для простого подавления локальных минимумов.
-        4. Применения пороговой обработки с Гистерезисом, которая создает 2 пороговых значения T_upper и T_lower, которые используются в функции Canny().
-        
-        Для наглдяности покажем работу алгоритма на следующем изображении капель:
-        
-        ![разг](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/32e768ae-bb56-4cb3-b32c-61f6f3158c25)
-        
-        
-        ## Расчёт площади
-        
-        Для того, чтобы правильно считалась площадь, была необходима отрисовка замкнутых контуров капель. Это и была следующая проблема, с которой мы столкнулись. Для ее решения мы последовательлно применяли несколько функций:
-        
-        1. Уменьшение шума с помощью медианного сглаживания.
-        2. Увелечение резкости изображения с помощью 2D фильтра
-        3. Маска Собеля для выделения контуров.
-        4. Размытие Гаусса для уменьшения шума.
-        5. Обнаружение контуров с помощью Canny.
-        6. Получение массива внешних контуров с помощью findContours.
-        7. Закрашиваниие контуров с помощью fillPoly.
-        8. Повторяем с шага 1 для получившейся маски.
-        9. Сложение двух получившихся масок.
-        10. Отрисовка контуров на картикне.
-        
-        Для подсчета площади капли в пикселях использовалась функция contourArea, которая считает пиксели в замкнутом контуре.
-        
-        В итоге, мы пришли к следующим результатам:
-        
-        ![разг2](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/7904d768-380c-4ff6-be3d-87fbaf159be0)
-        
-        
-        ## Отрисовка контуров на входном изображении
-        
-        В конце программы у нас имеются входное изображение и маска с контурами этого изображения. С помощью функции bitwise_and(img, img, mask=mask) из библиотеки **OpenCV2** мы рисуем маску прямо на входном изображении и выводим это как итог.
-        
-        ## Телеграмм-бот
-        
-        Для взаимодействия пользователя и телеграмм-бота мы использовали библиотеку **Telebot**. Бот запускается с помощью команды /start, после чего он нас приветствует и просит ввести команду Help. Далее мы можем увидеть список команд в определённой последовательности для корректной работы. Наш бот не очень разговорчивый, поэтому если вы попытаетесь поговорить с ним на отдалённые темы, у вас ничего не выйдет.
-        
-        
-        ![Без имени](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/ff7c0fff-05f0-4ddb-8bc3-4225ed99166e)
-        
-        
-        ## DockerHub 
-        - https://hub.docker.com/repository/docker/nekrasovaanna/droplet-detector/general
-        
-        Команда для начала работы проекта
-        ```
-        docker run nekrasovaanna/droplet-detector
-        ```
-        
-        ## Установка с Pypi и запуск
-        Установите библиотеку Droplet_Detector в рабочую область
-        ```
-        pip install Droplet_Detector
-        ```
-        Перед запуском создайте папки в рабочей области "exel", "new_file" and "save_docs"
-        ```
-        mkdir exel,new_file,save_docs
-        ```
-        Импортируйте модуль Bot.py в вашем файле .py
-        ```
-        from Droplet_Detector import Bot
-        ```
-        Запустите бота написав 
-        ```
-        Bot.start()
-        ```
-        Cсылка на бота 
-        ```
-        https://t.me/Droplet_Detector_bot
-        ```
-        ## Источники
-        
-        - https://www.geeksforgeeks.org/python-opencv-canny-function/
-        - https://opencvguide.readthedocs.io/_/downloads/en/latest/pdf/
-        - https://pytba.readthedocs.io/ru/latest/index.html
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Droplet-Detector
+
+![droplet](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/c1928e58-414d-49ef-97dd-20d10441bfd5)
+
+---
+
+![Build Status](https://github.com/kvasik3000/Droplet-Detector/actions/workflows/python-app.yml/badge.svg?branch=main)
+<img src = "https://img.shields.io/badge/Code%20Coverage-80%25-success?">
+<img src = 'https://img.shields.io/github/contributors/kvasik3000/Droplet-Detector?'>  
+<img src ='https://img.shields.io/github/repo-size/kvasik3000/Droplet-Detector?'>
+
+---
+
+## Введение
+Перед нашей командой стояла задача создать простой в использовании проект, который будет рисовать контуры капель. Также было необходимо написать код для подсчёта пикселей каждой капли и добавить возможность сохранять данные в виде таблицы. Эта работа позволила нам глубже изучить компьютерное зрение с помощью библиотек **OpenCV2** в Python, научиться работать в команде и дала возможность создать собственного телеграмм-бота.
+
+### Работу выполнили студенты из группы 21932:
+
+- [Квас Андрей](https://github.com/kvasik3000)
+- [Некрасова Анна](https://github.com/NekrasovaAnn)
+- [Белькова Ксения](https://github.com/didilovu)
+
+## Обнаружение контуров
+
+Для корректного обнаружения контуров капель мы использовали **Canny Edge**. Это алгоритм, состоящий из 4 основных шагов:
+
+1. Уменьшение шума с помощью гауссовского сглаживания.
+2. Вычисление градиента изображения с помощью фильтра Собеля.
+3. Применение Non-Max Suppression для простого подавления локальных минимумов.
+4. Применения пороговой обработки с Гистерезисом, которая создает 2 пороговых значения T_upper и T_lower, которые используются в функции Canny().
+
+Для наглдяности покажем работу алгоритма на следующем изображении капель:
+
+![разг](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/32e768ae-bb56-4cb3-b32c-61f6f3158c25)
+
+
+## Расчёт площади
+
+Для того, чтобы правильно считалась площадь, была необходима отрисовка замкнутых контуров капель. Это и была следующая проблема, с которой мы столкнулись. Для ее решения мы последовательлно применяли несколько функций:
+
+1. Уменьшение шума с помощью медианного сглаживания.
+2. Увелечение резкости изображения с помощью 2D фильтра
+3. Маска Собеля для выделения контуров.
+4. Размытие Гаусса для уменьшения шума.
+5. Обнаружение контуров с помощью Canny.
+6. Получение массива внешних контуров с помощью findContours.
+7. Закрашиваниие контуров с помощью fillPoly.
+8. Повторяем с шага 1 для получившейся маски.
+9. Сложение двух получившихся масок.
+10. Отрисовка контуров на картикне.
+
+Для подсчета площади капли в пикселях использовалась функция contourArea, которая считает пиксели в замкнутом контуре.
+
+В итоге, мы пришли к следующим результатам:
+
+![разг2](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/7904d768-380c-4ff6-be3d-87fbaf159be0)
+
+
+## Отрисовка контуров на входном изображении
+
+В конце программы у нас имеются входное изображение и маска с контурами этого изображения. С помощью функции bitwise_and(img, img, mask=mask) из библиотеки **OpenCV2** мы рисуем маску прямо на входном изображении и выводим это как итог.
+
+## Телеграмм-бот
+
+Для взаимодействия пользователя и телеграмм-бота мы использовали библиотеку **Telebot**. Бот запускается с помощью команды /start, после чего он нас приветствует и просит ввести команду Help. Далее мы можем увидеть список команд в определённой последовательности для корректной работы. Наш бот не очень разговорчивый, поэтому если вы попытаетесь поговорить с ним на отдалённые темы, у вас ничего не выйдет.
+
+
+![Без имени](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/ff7c0fff-05f0-4ddb-8bc3-4225ed99166e)
+
+
+## DockerHub 
+- https://hub.docker.com/repository/docker/nekrasovaanna/droplet-detector/general
+
+Команда для начала работы проекта
+```
+docker run nekrasovaanna/droplet-detector
+```
+
+## Установка с Pypi и запуск
+Установите библиотеку Droplet_Detector в рабочую область
+```
+pip install Droplet_Detector
+```
+Перед запуском создайте папки в рабочей области "exel", "new_file" and "save_docs"
+```
+mkdir exel,new_file,save_docs
+```
+Импортируйте модуль Bot.py в вашем файле .py
+```
+from Droplet_Detector import Bot
+```
+Запустите бота написав 
+```
+Bot.start()
+```
+Cсылка на бота 
+```
+https://t.me/Droplet_Detector_bot
+```
+## Источники
+
+- https://www.geeksforgeeks.org/python-opencv-canny-function/
+- https://opencvguide.readthedocs.io/_/downloads/en/latest/pdf/
+- https://pytba.readthedocs.io/ru/latest/index.html
+
+
```

### Comparing `Droplet_Detector-0.1.2/LICENSE` & `Droplet_Detector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Droplet_Detector-0.1.2/PKG-INFO` & `Droplet_Detector-0.1.3/Droplet_Detector.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,121 @@
 Metadata-Version: 2.1
-Name: Droplet_Detector
-Version: 0.1.2
+Name: Droplet-Detector
+Version: 0.1.3
 Summary: Telegram bot that draws the outlines of drips on a photo !!! Warning!!!  Before running, be sure to create the folders "exel", "new_file" and "save_docs" in the workspace where the python file is located !!!!
 Home-page: https://github.com/kvasik3000/Droplet-Detector
 Author: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 Author-email: superadrenoline3000@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
-Description: # Droplet-Detector
-        
-        ![droplet](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/c1928e58-414d-49ef-97dd-20d10441bfd5)
-        
-        ---
-        
-        ![Build Status](https://github.com/kvasik3000/Droplet-Detector/actions/workflows/python-app.yml/badge.svg?branch=main)
-        <img src = "https://img.shields.io/badge/Code%20Coverage-80%25-success?">
-        <img src = 'https://img.shields.io/github/contributors/kvasik3000/Droplet-Detector?'>  
-        <img src ='https://img.shields.io/github/repo-size/kvasik3000/Droplet-Detector?'>
-        
-        ---
-        
-        ## Введение
-        Перед нашей командой стояла задача создать простой в использовании проект, который будет рисовать контуры капель. Также было необходимо написать код для подсчёта пикселей каждой капли и добавить возможность сохранять данные в виде таблицы. Эта работа позволила нам глубже изучить компьютерное зрение с помощью библиотек **OpenCV2** в Python, научиться работать в команде и дала возможность создать собственного телеграмм-бота.
-        
-        ### Работу выполнили студенты из группы 21932:
-        
-        - [Квас Андрей](https://github.com/kvasik3000)
-        - [Некрасова Анна](https://github.com/NekrasovaAnn)
-        - [Белькова Ксения](https://github.com/didilovu)
-        
-        ## Обнаружение контуров
-        
-        Для корректного обнаружения контуров капель мы использовали **Canny Edge**. Это алгоритм, состоящий из 4 основных шагов:
-        
-        1. Уменьшение шума с помощью гауссовского сглаживания.
-        2. Вычисление градиента изображения с помощью фильтра Собеля.
-        3. Применение Non-Max Suppression для простого подавления локальных минимумов.
-        4. Применения пороговой обработки с Гистерезисом, которая создает 2 пороговых значения T_upper и T_lower, которые используются в функции Canny().
-        
-        Для наглдяности покажем работу алгоритма на следующем изображении капель:
-        
-        ![разг](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/32e768ae-bb56-4cb3-b32c-61f6f3158c25)
-        
-        
-        ## Расчёт площади
-        
-        Для того, чтобы правильно считалась площадь, была необходима отрисовка замкнутых контуров капель. Это и была следующая проблема, с которой мы столкнулись. Для ее решения мы последовательлно применяли несколько функций:
-        
-        1. Уменьшение шума с помощью медианного сглаживания.
-        2. Увелечение резкости изображения с помощью 2D фильтра
-        3. Маска Собеля для выделения контуров.
-        4. Размытие Гаусса для уменьшения шума.
-        5. Обнаружение контуров с помощью Canny.
-        6. Получение массива внешних контуров с помощью findContours.
-        7. Закрашиваниие контуров с помощью fillPoly.
-        8. Повторяем с шага 1 для получившейся маски.
-        9. Сложение двух получившихся масок.
-        10. Отрисовка контуров на картикне.
-        
-        Для подсчета площади капли в пикселях использовалась функция contourArea, которая считает пиксели в замкнутом контуре.
-        
-        В итоге, мы пришли к следующим результатам:
-        
-        ![разг2](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/7904d768-380c-4ff6-be3d-87fbaf159be0)
-        
-        
-        ## Отрисовка контуров на входном изображении
-        
-        В конце программы у нас имеются входное изображение и маска с контурами этого изображения. С помощью функции bitwise_and(img, img, mask=mask) из библиотеки **OpenCV2** мы рисуем маску прямо на входном изображении и выводим это как итог.
-        
-        ## Телеграмм-бот
-        
-        Для взаимодействия пользователя и телеграмм-бота мы использовали библиотеку **Telebot**. Бот запускается с помощью команды /start, после чего он нас приветствует и просит ввести команду Help. Далее мы можем увидеть список команд в определённой последовательности для корректной работы. Наш бот не очень разговорчивый, поэтому если вы попытаетесь поговорить с ним на отдалённые темы, у вас ничего не выйдет.
-        
-        
-        ![Без имени](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/ff7c0fff-05f0-4ddb-8bc3-4225ed99166e)
-        
-        
-        ## DockerHub 
-        - https://hub.docker.com/repository/docker/nekrasovaanna/droplet-detector/general
-        
-        Команда для начала работы проекта
-        ```
-        docker run nekrasovaanna/droplet-detector
-        ```
-        
-        ## Установка с Pypi и запуск
-        Установите библиотеку Droplet_Detector в рабочую область
-        ```
-        pip install Droplet_Detector
-        ```
-        Перед запуском создайте папки в рабочей области "exel", "new_file" and "save_docs"
-        ```
-        mkdir exel,new_file,save_docs
-        ```
-        Импортируйте модуль Bot.py в вашем файле .py
-        ```
-        from Droplet_Detector import Bot
-        ```
-        Запустите бота написав 
-        ```
-        Bot.start()
-        ```
-        Cсылка на бота 
-        ```
-        https://t.me/Droplet_Detector_bot
-        ```
-        ## Источники
-        
-        - https://www.geeksforgeeks.org/python-opencv-canny-function/
-        - https://opencvguide.readthedocs.io/_/downloads/en/latest/pdf/
-        - https://pytba.readthedocs.io/ru/latest/index.html
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Droplet-Detector
+
+![droplet](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/c1928e58-414d-49ef-97dd-20d10441bfd5)
+
+---
+
+![Build Status](https://github.com/kvasik3000/Droplet-Detector/actions/workflows/python-app.yml/badge.svg?branch=main)
+<img src = "https://img.shields.io/badge/Code%20Coverage-80%25-success?">
+<img src = 'https://img.shields.io/github/contributors/kvasik3000/Droplet-Detector?'>  
+<img src ='https://img.shields.io/github/repo-size/kvasik3000/Droplet-Detector?'>
+
+---
+
+## Введение
+Перед нашей командой стояла задача создать простой в использовании проект, который будет рисовать контуры капель. Также было необходимо написать код для подсчёта пикселей каждой капли и добавить возможность сохранять данные в виде таблицы. Эта работа позволила нам глубже изучить компьютерное зрение с помощью библиотек **OpenCV2** в Python, научиться работать в команде и дала возможность создать собственного телеграмм-бота.
+
+### Работу выполнили студенты из группы 21932:
+
+- [Квас Андрей](https://github.com/kvasik3000)
+- [Некрасова Анна](https://github.com/NekrasovaAnn)
+- [Белькова Ксения](https://github.com/didilovu)
+
+## Обнаружение контуров
+
+Для корректного обнаружения контуров капель мы использовали **Canny Edge**. Это алгоритм, состоящий из 4 основных шагов:
+
+1. Уменьшение шума с помощью гауссовского сглаживания.
+2. Вычисление градиента изображения с помощью фильтра Собеля.
+3. Применение Non-Max Suppression для простого подавления локальных минимумов.
+4. Применения пороговой обработки с Гистерезисом, которая создает 2 пороговых значения T_upper и T_lower, которые используются в функции Canny().
+
+Для наглдяности покажем работу алгоритма на следующем изображении капель:
+
+![разг](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/32e768ae-bb56-4cb3-b32c-61f6f3158c25)
+
+
+## Расчёт площади
+
+Для того, чтобы правильно считалась площадь, была необходима отрисовка замкнутых контуров капель. Это и была следующая проблема, с которой мы столкнулись. Для ее решения мы последовательлно применяли несколько функций:
+
+1. Уменьшение шума с помощью медианного сглаживания.
+2. Увелечение резкости изображения с помощью 2D фильтра
+3. Маска Собеля для выделения контуров.
+4. Размытие Гаусса для уменьшения шума.
+5. Обнаружение контуров с помощью Canny.
+6. Получение массива внешних контуров с помощью findContours.
+7. Закрашиваниие контуров с помощью fillPoly.
+8. Повторяем с шага 1 для получившейся маски.
+9. Сложение двух получившихся масок.
+10. Отрисовка контуров на картикне.
+
+Для подсчета площади капли в пикселях использовалась функция contourArea, которая считает пиксели в замкнутом контуре.
+
+В итоге, мы пришли к следующим результатам:
+
+![разг2](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/7904d768-380c-4ff6-be3d-87fbaf159be0)
+
+
+## Отрисовка контуров на входном изображении
+
+В конце программы у нас имеются входное изображение и маска с контурами этого изображения. С помощью функции bitwise_and(img, img, mask=mask) из библиотеки **OpenCV2** мы рисуем маску прямо на входном изображении и выводим это как итог.
+
+## Телеграмм-бот
+
+Для взаимодействия пользователя и телеграмм-бота мы использовали библиотеку **Telebot**. Бот запускается с помощью команды /start, после чего он нас приветствует и просит ввести команду Help. Далее мы можем увидеть список команд в определённой последовательности для корректной работы. Наш бот не очень разговорчивый, поэтому если вы попытаетесь поговорить с ним на отдалённые темы, у вас ничего не выйдет.
+
+
+![Без имени](https://github.com/kvasik3000/Droplet-Detector/assets/124969658/ff7c0fff-05f0-4ddb-8bc3-4225ed99166e)
+
+
+## DockerHub 
+- https://hub.docker.com/repository/docker/nekrasovaanna/droplet-detector/general
+
+Команда для начала работы проекта
+```
+docker run nekrasovaanna/droplet-detector
+```
+
+## Установка с Pypi и запуск
+Установите библиотеку Droplet_Detector в рабочую область
+```
+pip install Droplet_Detector
+```
+Перед запуском создайте папки в рабочей области "exel", "new_file" and "save_docs"
+```
+mkdir exel,new_file,save_docs
+```
+Импортируйте модуль Bot.py в вашем файле .py
+```
+from Droplet_Detector import Bot
+```
+Запустите бота написав 
+```
+Bot.start()
+```
+Cсылка на бота 
+```
+https://t.me/Droplet_Detector_bot
+```
+## Источники
+
+- https://www.geeksforgeeks.org/python-opencv-canny-function/
+- https://opencvguide.readthedocs.io/_/downloads/en/latest/pdf/
+- https://pytba.readthedocs.io/ru/latest/index.html
+
+
```

### Comparing `Droplet_Detector-0.1.2/README.md` & `Droplet_Detector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Droplet_Detector-0.1.2/setup.py` & `Droplet_Detector-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 :authors: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 :license: Apache License, Version 2.0, see LICENSE file
 :copyright: (c) 2023 kvasik3000
 """
 
-version = '0.1.2'
+version = '0.1.3'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 # with open("requirements.txt", "r") as file:
 #     requirements = file.read().splitlines()
```

