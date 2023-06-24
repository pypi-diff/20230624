# Comparing `tmp/kz_iin_validator-0.6.0.tar.gz` & `tmp/kz_iin_validator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kz_iin_validator-0.6.0.tar", last modified: Tue Apr 11 06:54:52 2023, max compression
+gzip compressed data, was "kz_iin_validator-0.7.0.tar", last modified: Sat Jun 24 12:37:40 2023, max compression
```

## Comparing `kz_iin_validator-0.6.0.tar` & `kz_iin_validator-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 06:54:52.683955 kz_iin_validator-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-04-11 06:54:52.683955 kz_iin_validator-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4439 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 06:54:52.679955 kz_iin_validator-0.6.0/kz_iin_validator/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/iin_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/iin_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 06:54:52.679955 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 06:54:52.683955 kz_iin_validator-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 12:37:40.608109 kz_iin_validator-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-24 12:37:40.608109 kz_iin_validator-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4411 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 12:37:40.608109 kz_iin_validator-0.7.0/kz_iin_validator/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/kz_iin_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/kz_iin_validator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/kz_iin_validator/iin_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/kz_iin_validator/iin_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/kz_iin_validator/iin_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/kz_iin_validator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 12:37:40.608109 kz_iin_validator-0.7.0/kz_iin_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-24 12:37:40.000000 kz_iin_validator-0.7.0/kz_iin_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-24 12:37:40.000000 kz_iin_validator-0.7.0/kz_iin_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-24 12:37:40.000000 kz_iin_validator-0.7.0/kz_iin_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-24 12:37:40.000000 kz_iin_validator-0.7.0/kz_iin_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-24 12:37:40.608109 kz_iin_validator-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-24 12:37:36.000000 kz_iin_validator-0.7.0/setup.py
```

### Comparing `kz_iin_validator-0.6.0/LICENSE.txt` & `kz_iin_validator-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kz_iin_validator-0.6.0/PKG-INFO` & `kz_iin_validator-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: kz_iin_validator
-Version: 0.6.0
-Summary: Kazakhstan IIN parser and validator
-Home-page: https://github.com/ZhymabekRoman/kz-iin-validator
-Author: Zhymabek Roman
-Author-email: robanokssamit@yandex.ru
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # kz-iin-validator
 
 [![MIT License](https://img.shields.io/pypi/l/kz-iin-validator.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://img.shields.io/pypi/v/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![codecov](https://img.shields.io/codecov/c/github/ZhymabekRoman/kz-iin-validator?style=flat-square)](https://app.codecov.io/github/ZhymabekRoman/kz-iin-validator)
 [![tests](https://img.shields.io/github/actions/workflow/status/ZhymabekRoman/kz-iin-validator/pytest.yml?branch=main&style=flat-square)](https://github.com/ZhymabekRoman/kz-iin-validator/actions)
@@ -22,15 +10,14 @@
 
 ## Возможности:
 - Production-ready библиотека
 - 100% code coverage - Библиотека полностью покрыта тестами
 - Zero-depency - Не требует дополнительных зависимостей
 - Базовая валидация данных ИИН, таких как дата, месяц, год
 - Генератор ИИН
-- Два варианта валидации: стандартное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
 - Проверка целостности по хэш сумме ИИН. Алгоритм формирования ИИН регулируется Постановлением правительства РК "Об утверждении Программы перехода на единый номер физического (юридического) лица (индивидуальный идентификационный номер (бизнес-идентификационный номер) в целях создания Национальных реестров идентификационных номеров Республики Казахстан" от 11 июня 2003 года N 565 - [Ссылка на источник приказа](https://adilet.zan.kz/rus/docs/P030000565_)
 
 ## Требования:
 - Python 3.7 и выше * **
 > \* судя по информации утилиты Vermin
 
 > ** я могу адаптировать (забэкпортить) библиотеку для более старых версии Python, но стоит ли оно? Если что дайте мне знать
@@ -84,7 +71,17 @@
 ### Генератор ИИН:
 ```python
 from kz_iin_validator import generate_iin
 
 generated_iin = generate_iin()
 print(generated_iin) # return generated valid IIN as string
 ```
+
+### Извлечь ИИН из текста:
+```python
+from kz_iin_validator import extract_iin
+
+text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit - 251112401047. Aliquam vel diam ac enim consequat rhoncus 700911204362!."
+
+extracted_iin_list = extract_iin(text)
+print(extracted_iin_list)
+```
```

### Comparing `kz_iin_validator-0.6.0/README.md` & `kz_iin_validator-0.7.0/kz_iin_validator.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: kz-iin-validator
+Version: 0.7.0
+Summary: Kazakhstan IIN parser and validator
+Home-page: https://github.com/ZhymabekRoman/kz-iin-validator
+Author: Zhymabek Roman
+Author-email: robanokssamit@yandex.ru
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # kz-iin-validator
 
 [![MIT License](https://img.shields.io/pypi/l/kz-iin-validator.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://img.shields.io/pypi/v/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![codecov](https://img.shields.io/codecov/c/github/ZhymabekRoman/kz-iin-validator?style=flat-square)](https://app.codecov.io/github/ZhymabekRoman/kz-iin-validator)
 [![tests](https://img.shields.io/github/actions/workflow/status/ZhymabekRoman/kz-iin-validator/pytest.yml?branch=main&style=flat-square)](https://github.com/ZhymabekRoman/kz-iin-validator/actions)
@@ -10,15 +22,14 @@
 
 ## Возможности:
 - Production-ready библиотека
 - 100% code coverage - Библиотека полностью покрыта тестами
 - Zero-depency - Не требует дополнительных зависимостей
 - Базовая валидация данных ИИН, таких как дата, месяц, год
 - Генератор ИИН
-- Два варианта валидации: стандартное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
 - Проверка целостности по хэш сумме ИИН. Алгоритм формирования ИИН регулируется Постановлением правительства РК "Об утверждении Программы перехода на единый номер физического (юридического) лица (индивидуальный идентификационный номер (бизнес-идентификационный номер) в целях создания Национальных реестров идентификационных номеров Республики Казахстан" от 11 июня 2003 года N 565 - [Ссылка на источник приказа](https://adilet.zan.kz/rus/docs/P030000565_)
 
 ## Требования:
 - Python 3.7 и выше * **
 > \* судя по информации утилиты Vermin
 
 > ** я могу адаптировать (забэкпортить) библиотеку для более старых версии Python, но стоит ли оно? Если что дайте мне знать
@@ -72,7 +83,17 @@
 ### Генератор ИИН:
 ```python
 from kz_iin_validator import generate_iin
 
 generated_iin = generate_iin()
 print(generated_iin) # return generated valid IIN as string
 ```
+
+### Извлечь ИИН из текста:
+```python
+from kz_iin_validator import extract_iin
+
+text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit - 251112401047. Aliquam vel diam ac enim consequat rhoncus 700911204362!."
+
+extracted_iin_list = extract_iin(text)
+print(extracted_iin_list)
+```
```

### Comparing `kz_iin_validator-0.6.0/kz_iin_validator/iin_generator.py` & `kz_iin_validator-0.7.0/kz_iin_validator/iin_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import random
 
 
 def generate_iin():
+    """
+    Generates a random Individual Identification Number (IIN).
+
+    Returns:
+        str: The randomly generated IIN.
+
+    """
     # year = random.randint(1800, 2099)
     year = random.randint(0, 99)
     month = random.randint(1, 12)
 
     # TODO: manually generate gender instead generating with centry
     # gender = random.choice(list(IINGender))
```

### Comparing `kz_iin_validator-0.6.0/kz_iin_validator/iin_validator.py` & `kz_iin_validator-0.7.0/kz_iin_validator/iin_validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import datetime as dt
-import re
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Union
+from typing import Union, Optional, Tuple
 
 from .exceptions import IINValidateError
 from .utils import is_digit_string
 
-IIN_REGEX_WEAK_FAST = re.compile(r"^[0-9]{12}$")
-IIN_REGEX_WEAK = re.compile(r"^((0[48]|[2468][048]|[13579][26])0230[1-5]|000230[34]|\d\d((0[13578]|1[02])(0[1-9]|[12]\d|3[01])|(0[469]|11)(0[1-9]|[12]\d|30)|02(0[1-9]|[1-2]\d)))[0-6]\d{5}$")
-
 
 @dataclass
 class BornDate:
     day: int
     month: int
     year: int
     datetime: dt.datetime
@@ -32,50 +28,64 @@
     born_date: BornDate
 
 
 class ValidatedIIN(IIN):
     is_validated: bool = True
 
 
-def safe_validate_iin(iin: Union[str, IIN], weak_fast_check: bool = False):
-    # Golang like exception returning logic
+def safe_validate_iin(iin: Union[str, IIN]) -> Tuple[Optional[ValidatedIIN], Exception]:
+    """
+    Golang-like function for Individual Identification Number (IIN) validation.
+
+    Args:
+        iin (Union[str, IIN]): The IIN to be validated. It can be either a string or an IIN object.
+
+    Returns:
+        A tuple of `(ValidatedIIN, Exception)`. The first element is `None` if the IIN is not valid, and the second element is an exception if there was an error validating the IIN.
+
+    """
     try:
-        result = validate_iin(iin, weak_fast_check)
+        result = validate_iin(iin)
     except Exception as ex:
-        exception_msg = f"During validating IIN exception was caught: {str(ex)}"
-        return None, exception_msg
+        return None, ex
     else:
         return result, None
 
 
 # TODO: refactor into separate functions
-def validate_iin(iin: Union[str, IIN], weak_fast_check: bool = False) -> ValidatedIIN:
+def validate_iin(iin: Union[str, IIN]) -> ValidatedIIN:
+    """
+    Validates an Individual Identification Number (IIN).
+
+    Args:
+        iin (Union[str, IIN]): The IIN to be validated. It can be either a string or an IIN object.
+
+    Returns:
+        ValidatedIIN: The validated IIN as a ValidatedIIN object.
+
+    Raises:
+        ValueError: If the provided IIN is invalid.
+
+    """
+
     if isinstance(iin, IIN):
         iin = iin.iin
     elif not isinstance(iin, str):
         raise IINValidateError(f"Parametr 'iin' must be string, not {type(iin).__name__}")
 
-    if weak_fast_check:
-        iin_regex_fast = IIN_REGEX_WEAK_FAST.match(iin)
-        if iin_regex_fast is None:
-            raise IINValidateError("Not valid IIN!")
-
-        iin_regex_weak = IIN_REGEX_WEAK.match(iin)
-        if iin_regex_weak is None:
-            raise IINValidateError("Not correct integers range")
-
     if not is_digit_string(iin):
         raise IINValidateError("IIN must contains only numbers")
 
     if len(iin) != 12:
         raise IINValidateError("IIN must be 12 length")
 
     # iin helper functions
     def iin_int(index):
         return int(iin[index])
+
     def iin_int_range(x, y):
         return int(iin[x:y])
 
     is_person = (iin_int(6) != 0)
     if is_person:
         if iin_int(6) % 2 == 1:
             gender = IINGender.male
```

### Comparing `kz_iin_validator-0.6.0/kz_iin_validator.egg-info/PKG-INFO` & `kz_iin_validator-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kz-iin-validator
-Version: 0.6.0
+Name: kz_iin_validator
+Version: 0.7.0
 Summary: Kazakhstan IIN parser and validator
 Home-page: https://github.com/ZhymabekRoman/kz-iin-validator
 Author: Zhymabek Roman
 Author-email: robanokssamit@yandex.ru
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -22,15 +22,14 @@
 
 ## Возможности:
 - Production-ready библиотека
 - 100% code coverage - Библиотека полностью покрыта тестами
 - Zero-depency - Не требует дополнительных зависимостей
 - Базовая валидация данных ИИН, таких как дата, месяц, год
 - Генератор ИИН
-- Два варианта валидации: стандартное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
 - Проверка целостности по хэш сумме ИИН. Алгоритм формирования ИИН регулируется Постановлением правительства РК "Об утверждении Программы перехода на единый номер физического (юридического) лица (индивидуальный идентификационный номер (бизнес-идентификационный номер) в целях создания Национальных реестров идентификационных номеров Республики Казахстан" от 11 июня 2003 года N 565 - [Ссылка на источник приказа](https://adilet.zan.kz/rus/docs/P030000565_)
 
 ## Требования:
 - Python 3.7 и выше * **
 > \* судя по информации утилиты Vermin
 
 > ** я могу адаптировать (забэкпортить) библиотеку для более старых версии Python, но стоит ли оно? Если что дайте мне знать
@@ -84,7 +83,17 @@
 ### Генератор ИИН:
 ```python
 from kz_iin_validator import generate_iin
 
 generated_iin = generate_iin()
 print(generated_iin) # return generated valid IIN as string
 ```
+
+### Извлечь ИИН из текста:
+```python
+from kz_iin_validator import extract_iin
+
+text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit - 251112401047. Aliquam vel diam ac enim consequat rhoncus 700911204362!."
+
+extracted_iin_list = extract_iin(text)
+print(extracted_iin_list)
+```
```

### Comparing `kz_iin_validator-0.6.0/setup.py` & `kz_iin_validator-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read_requirements(filename):
     with open(filename, "r", encoding="utf-8") as fp:
         return fp.read().strip().splitlines()
 
 
 setup(
     name="kz_iin_validator",
-    version="0.6.0",
+    version="0.7.0",
     python_requires='>=3.7',
     author="Zhymabek Roman",
     author_email="robanokssamit@yandex.ru",
     long_description=readme_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     packages=find_packages(exclude=["tests", "images"]),
```

