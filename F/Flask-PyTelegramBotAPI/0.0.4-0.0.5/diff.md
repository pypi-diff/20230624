# Comparing `tmp/Flask-PyTelegramBotAPI-0.0.4.tar.gz` & `tmp/Flask-PyTelegramBotAPI-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-PyTelegramBotAPI-0.0.4.tar", last modified: Wed Jun 14 20:56:12 2023, max compression
+gzip compressed data, was "dist/Flask-PyTelegramBotAPI-0.0.5.tar", last modified: Sat Jun 24 11:01:01 2023, max compression
```

## Comparing `Flask-PyTelegramBotAPI-0.0.4.tar` & `Flask-PyTelegramBotAPI-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:56:12.153559 Flask-PyTelegramBotAPI-0.0.4/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)    18092 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.4/LICENSE
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      224 2023-06-14 20:56:12.153559 Flask-PyTelegramBotAPI-0.0.4/PKG-INFO
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       24 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.4/README.md
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       38 2023-06-14 20:56:12.153559 Flask-PyTelegramBotAPI-0.0.4/setup.cfg
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      456 2023-06-14 20:53:40.000000 Flask-PyTelegramBotAPI-0.0.4/setup.py
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:56:12.149559 Flask-PyTelegramBotAPI-0.0.4/src/
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:56:12.153559 Flask-PyTelegramBotAPI-0.0.4/src/Flask_PyTelegramBotAPI.egg-info/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      224 2023-06-14 20:56:12.000000 Flask-PyTelegramBotAPI-0.0.4/src/Flask_PyTelegramBotAPI.egg-info/PKG-INFO
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      437 2023-06-14 20:56:12.000000 Flask-PyTelegramBotAPI-0.0.4/src/Flask_PyTelegramBotAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)        1 2023-06-14 20:56:12.000000 Flask-PyTelegramBotAPI-0.0.4/src/Flask_PyTelegramBotAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       25 2023-06-14 20:56:12.000000 Flask-PyTelegramBotAPI-0.0.4/src/Flask_PyTelegramBotAPI.egg-info/requires.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       23 2023-06-14 20:56:12.000000 Flask-PyTelegramBotAPI-0.0.4/src/Flask_PyTelegramBotAPI.egg-info/top_level.txt
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 20:56:12.153559 Flask-PyTelegramBotAPI-0.0.4/src/flask_pytelegrambotapi/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      227 2023-06-03 20:00:47.000000 Flask-PyTelegramBotAPI-0.0.4/src/flask_pytelegrambotapi/__init__.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)     3972 2023-06-07 20:26:12.000000 Flask-PyTelegramBotAPI-0.0.4/src/flask_pytelegrambotapi/extension.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       67 2023-05-17 09:35:36.000000 Flask-PyTelegramBotAPI-0.0.4/src/flask_pytelegrambotapi/mixins.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      461 2023-05-16 11:59:07.000000 Flask-PyTelegramBotAPI-0.0.4/src/flask_pytelegrambotapi/utils.py
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-24 11:01:01.667905 Flask-PyTelegramBotAPI-0.0.5/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)    18092 2023-05-15 06:48:50.000000 Flask-PyTelegramBotAPI-0.0.5/LICENSE
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      224 2023-06-24 11:01:01.667905 Flask-PyTelegramBotAPI-0.0.5/PKG-INFO
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       71 2023-06-24 10:13:36.000000 Flask-PyTelegramBotAPI-0.0.5/README.md
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       38 2023-06-24 11:01:01.667905 Flask-PyTelegramBotAPI-0.0.5/setup.cfg
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      456 2023-06-24 10:13:57.000000 Flask-PyTelegramBotAPI-0.0.5/setup.py
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-24 11:01:01.643905 Flask-PyTelegramBotAPI-0.0.5/src/
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-24 11:01:01.659905 Flask-PyTelegramBotAPI-0.0.5/src/Flask_PyTelegramBotAPI.egg-info/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      224 2023-06-24 11:01:01.000000 Flask-PyTelegramBotAPI-0.0.5/src/Flask_PyTelegramBotAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      437 2023-06-24 11:01:01.000000 Flask-PyTelegramBotAPI-0.0.5/src/Flask_PyTelegramBotAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)        1 2023-06-24 11:01:01.000000 Flask-PyTelegramBotAPI-0.0.5/src/Flask_PyTelegramBotAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       25 2023-06-24 11:01:01.000000 Flask-PyTelegramBotAPI-0.0.5/src/Flask_PyTelegramBotAPI.egg-info/requires.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       23 2023-06-24 11:01:01.000000 Flask-PyTelegramBotAPI-0.0.5/src/Flask_PyTelegramBotAPI.egg-info/top_level.txt
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-24 11:01:01.667905 Flask-PyTelegramBotAPI-0.0.5/src/flask_pytelegrambotapi/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      227 2023-06-03 20:00:47.000000 Flask-PyTelegramBotAPI-0.0.5/src/flask_pytelegrambotapi/__init__.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)     3747 2023-06-24 10:08:21.000000 Flask-PyTelegramBotAPI-0.0.5/src/flask_pytelegrambotapi/extension.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       67 2023-05-17 09:35:36.000000 Flask-PyTelegramBotAPI-0.0.5/src/flask_pytelegrambotapi/mixins.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      412 2023-06-24 10:08:21.000000 Flask-PyTelegramBotAPI-0.0.5/src/flask_pytelegrambotapi/utils.py
```

### Comparing `Flask-PyTelegramBotAPI-0.0.4/LICENSE` & `Flask-PyTelegramBotAPI-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-PyTelegramBotAPI-0.0.4/src/flask_pytelegrambotapi/extension.py` & `Flask-PyTelegramBotAPI-0.0.5/src/flask_pytelegrambotapi/extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                  app: Flask | None = None, token: str | None = None, threaded: Optional[bool] = None) -> None:
         token = token or app.config.setdefault('TELEBOT_BOT_TOKEN', None)
 
         if not token:
             raise RuntimeError(
                 "Either 'TELEBOT_BOT_TOKEN' must be set."
             )
-        self.bot = None
+        self.session = None
 
         self._args = {}
         if 'TELEBOT_THREADED' in app.config:
             self._args['threaded'] = app.config['TELEBOT_THREADED']
 
         if threaded:
             self._args['threaded'] = threaded
@@ -53,72 +53,62 @@
 
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app: Flask) -> None:
         state_storage = StatePickleStorage()
 
-        self.bot: telebot.TeleBot = telebot.TeleBot(app.config['TELEBOT_BOT_TOKEN'], state_storage=state_storage,
-                                                    **self._args)
+        self.session: telebot.TeleBot = telebot.TeleBot(app.config['TELEBOT_BOT_TOKEN'], state_storage=state_storage,
+                                                        **self._args)
 
         WEBHOOK_URL_PATH = "/%s/" % (app.config['TELEBOT_BOT_TOKEN'])
 
         @app.route(WEBHOOK_URL_PATH, methods=['POST'])
         def webhook():
             if request.headers.get('content-type') == 'application/json':
                 json_string = request.get_data().decode('utf-8')
                 update = telebot.types.Update.de_json(json_string)
-                self.bot.process_new_updates([update])
+                self.session.process_new_updates([update])
                 return ''
             else:
                 abort(403)
 
         @app.before_request
         def _load_user():
             json_string = request.get_data().decode('utf-8')
 
             contact = None
 
-            from pprint import pprint
             update = telebot.types.Update.de_json(json_string)
-            pprint(update.__dict__)
-
-
-            from pprint import pprint
 
             if update.callback_query:
                 current_app._tg_user = update.callback_query.message.from_user
                 current_app._tg_chat = update.callback_query.message.chat
-                pprint(update.callback_query.__dict__)
             elif update.message:
                 current_app._tg_user = update.message.from_user
                 current_app._tg_chat = update.message.chat
                 contact = update.message.contact
             elif update.edited_message:
                 current_app._tg_user = update.edited_message.from_user
                 current_app._tg_chat = update.edited_message.chat
                 contact = update.edited_message.contact
 
-            if contact:
-                pprint(contact.__dict__)
 
-
-        time.sleep(1)
+        time.sleep(0.5)
         telebot.logger.info('Удаляем старые webhook')
-        self.bot.remove_webhook()
+        self.session.remove_webhook()
 
         time.sleep(0.5)
         telebot.logger.info('Устанавливаем новые webhook')
-        self.bot.set_webhook(url=app.config['TELEBOT_WEBHOOK_URL_BASE'] + WEBHOOK_URL_PATH)
+        self.session.set_webhook(url=app.config['TELEBOT_WEBHOOK_URL_BASE'] + WEBHOOK_URL_PATH)
 
         app.pytelegrambotapi = self
 
     def load_user(self, callback):
-        print(callback)
         self._user_callback = callback
         return callback
 
     def __getattr__(self, item):
-        if item in dir(self.bot):
-            return getattr(self.bot, item)
+        if item in dir(self.session):
+            return getattr(self.session, item)
 
         raise AttributeError("'{}' object has no attribute '{}'".format(type(self).__name__, item))
```

