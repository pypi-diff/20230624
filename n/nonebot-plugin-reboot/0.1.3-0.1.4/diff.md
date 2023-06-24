# Comparing `tmp/nonebot_plugin_reboot-0.1.3.tar.gz` & `tmp/nonebot_plugin_reboot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_reboot-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_reboot-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_reboot-0.1.3.tar` & `nonebot_plugin_reboot-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1061 2022-06-05 09:17:56.835835 nonebot_plugin_reboot-0.1.3/LICENSE
--rw-r--r--   0        0        0     3255 2022-06-26 09:22:09.557876 nonebot_plugin_reboot-0.1.3/README.md
--rw-r--r--   0        0        0      704 2022-06-26 09:12:35.615369 nonebot_plugin_reboot-0.1.3/nonebot_plugin_reboot/__init__.py
--rw-r--r--   0        0        0      394 2022-06-05 09:17:56.238835 nonebot_plugin_reboot-0.1.3/nonebot_plugin_reboot/command.py
--rw-r--r--   0        0        0      334 2022-06-05 13:18:52.740467 nonebot_plugin_reboot-0.1.3/nonebot_plugin_reboot/config.py
--rw-r--r--   0        0        0     1584 2022-06-18 18:08:47.824279 nonebot_plugin_reboot-0.1.3/nonebot_plugin_reboot/reloader.py
--rw-r--r--   0        0        0      552 2022-06-26 10:30:15.516284 nonebot_plugin_reboot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4031 2022-06-26 10:32:21.030918 nonebot_plugin_reboot-0.1.3/setup.py
--rw-r--r--   0        0        0     3996 2022-06-26 10:32:21.031212 nonebot_plugin_reboot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-02-19 14:04:21.290919 nonebot_plugin_reboot-0.1.4/LICENSE
+-rw-r--r--   0        0        0      842 2023-06-24 10:30:12.896911 nonebot_plugin_reboot-0.1.4/nonebot_plugin_reboot/__init__.py
+-rw-r--r--   0        0        0      410 2023-02-19 14:04:21.322169 nonebot_plugin_reboot-0.1.4/nonebot_plugin_reboot/command.py
+-rw-r--r--   0        0        0      350 2023-02-19 14:04:21.322169 nonebot_plugin_reboot-0.1.4/nonebot_plugin_reboot/config.py
+-rw-r--r--   0        0        0     1646 2023-02-19 14:04:21.322169 nonebot_plugin_reboot-0.1.4/nonebot_plugin_reboot/reloader.py
+-rw-r--r--   0        0        0      573 2023-06-24 10:30:40.514608 nonebot_plugin_reboot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3571 2023-02-19 14:33:51.990234 nonebot_plugin_reboot-0.1.4/README.md
+-rw-r--r--   0        0        0     4276 1970-01-01 00:00:00.000000 nonebot_plugin_reboot-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_reboot-0.1.3/README.md` & `nonebot_plugin_reboot-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# Nonebot-plugin-reboot 
-用命令重启 bot 
-
-[![asciicast](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV.svg)](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV)
-
-## :warning:注意事项
-**不支持** `nb-cli`，即 `nb run` 启动方式。
-需要在 bot 目录下使用 `python bot.py` 启动。
-
-重启时直接对子进程使用 `process.terminate()`，如果你的其他插件启动了子进程，请确保它们能在设定的等待时间内正确关闭子进程，否则子进程会变成孤立进程。  
-:warning: Windows 下因系统 API 的限制进程会直接被杀死， **没有** 等待时间。
-
-<hr>  
-
-插件依赖于 `multiprocessing` `spawn` 生成子进程方式工作，支持由 `nb-cli` 生成的 bot.py，或任何显式加载了 `bot.py` 并在加载插件后调用 `nonebot.run` 的启动方式。  
-
-不支持 `nb run` 启动，因为 `nb run` 使用 `importlib` 在函数内加载 `bot.py`，multiprocessing 生成子进程时不会运行 `bot.py`，即 nonebot 初始化和加载插件的过程，导致启动失败。  
-
-得益于使用 `spawn` 方式启动，每次重启都相当于重新加载了所有代码。只有这个插件本身或者 `bot.py` 有更新时才需要彻底关闭 bot 重启。
-
-
-## 安装
-通过 nb-cli 安装:  
-`nb plugin install nonebot-plugin-reboot`  
-通过 pip 安装:  
-`pip install nonebot-plugin-reboot`  
-
-
-## 使用
-**超级用户**向机器人**私聊**发送**命令** `重启`, `reboot` 或 `restart`  
-> :warning: 注意命令的 `COMMAND_START`.  
-> 例如 /重启 、 /reboot 、 /restart
-
-
-## 配置项 
-`reboot_load_command`: `bool` 
-- 加载内置的 `onebot v11` 重启命令 
-- 可以通过命令 `重启` `reboot` `restart` 触发重启 
-- 默认值: `True` 
-
-`reboot_grace_time_limit`: `int`
-- 收到重启命令后等待进程退出的最长时间，超时会强制杀进程
-- 在 Windows 下没有等待时间，会直接杀进程
-- ~~真寻从ctrl+c到彻底退出居然要六秒~~
-- 默认值: `20`
-
-## `bot.py`
-因为使用了 `spawn` 方式启动子进程，默认的 bot.py 会加载两次插件。  
-
-推荐的写法是将 插件加载部分 和 nonebot启动部分 分开，以避免插件在主进程和子进程都加载一遍
-
-~~真寻启动居然要20秒~~
-
-```python
-#
-# 上面省略
-#
-
-if __name__ == "__mp_main__": # 仅在子进程运行的代码
-    # Please DO NOT modify this file unless you know what you are doing!
-    # As an alternative, you should use command `nb` or modify `pyproject.toml` to load plugins
-    # 加载插件
-    nonebot.load_from_toml("pyproject.toml")
-    nonebot.load_plugins("src/plugins")
-    nonebot.load_plugin("nonebot_plugin_xxxxxx")
-    # ...
-
-if __name__ == "__main__": # 仅在主进程运行的代码
-    # nonebot.logger.warning("Always use `nb run` to start the bot instead of manually running!")
-    # 运行 nonebot
-    nonebot.load_plugin("nonebot_plugin_reboot") # 加载重启插件
-    nonebot.run(app="__mp_main__:app")
-```
-
-
-## API
-```python
-require("nonebot_plugin_reboot")
-from nonebot_plugin_reboot import Reloader
-Reloader.reload(delay=5) # 可选参数 5秒后触发重启
-```
-
-
-## 依赖 
-`nonebot2 >= 2.0.0beta.2`  
-
-启用 `reboot_load_command` 时需要以下依赖  
-`nonebot-adapter-onebot`
+# Nonebot-plugin-reboot 
+![](https://img.shields.io/badge/Development-Inactive-inactive) ![](https://img.shields.io/badge/PullRequests-Welcome-success)
+
+用命令重启 bot 
+
+[![asciicast](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV.svg)](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV)
+
+## :warning:注意事项
+**必须要有** `bot.py`  
+新版 nb-cli 默认不生成 bot.py，需要在 nb 菜单里选择 `生成机器人的入口文件` / `Generate entry file of your bot.` 生成一个，不需要修改。 ~~不要再去群里问bot.py在哪了~~
+
+**不兼容** `fastapi_reload`，见 [#1](https://github.com/18870/nonebot-plugin-reboot/issues/1)、[#2](https://github.com/18870/nonebot-plugin-reboot/issues/2)。  
+不推荐使用 nb-cli 的 `--reload` 参数，这个插件是 `--reload` 在生产环境中的替代品。
+
+重启时直接对子进程使用 `process.terminate()`，如果你的其他插件启动了子进程，请确保它们能在设定的等待时间内正确关闭子进程，否则子进程会变成孤立进程。  
+:warning: Windows 下因系统 API 的限制进程会直接被杀死， **没有** 等待时间。
+
+<hr>  
+
+插件依赖于 `multiprocessing` `spawn` 生成子进程方式工作，支持由 nb-cli 生成的 bot.py，以及其他在加载插件后调用 `nonebot.run()` 的启动方式。  
+
+
+## 安装
+通过 nb-cli 安装:  
+`nb plugin install nonebot-plugin-reboot`  
+
+新版 nb-cli 默认不生成 bot.py，需要在 nb 菜单里选择 `生成机器人的入口文件` / `Generate entry file of your bot.` 生成一个，不需要修改。
+
+
+## 使用
+**超级用户**向机器人**私聊**发送**命令** `重启`, `reboot` 或 `restart`  
+> :warning: 注意命令的 `COMMAND_START`.  
+> 例如 /重启 、 /reboot 、 /restart
+
+
+## 配置项 
+`reboot_load_command`: `bool` 
+- 加载内置的 `onebot v11` 重启命令 
+- 可以通过命令 `重启` `reboot` `restart` 触发重启 
+- 默认值: `True` 
+
+`reboot_grace_time_limit`: `int`
+- 收到重启命令后等待进程退出的最长时间，超时会强制杀进程
+- 在 Windows 下没有等待时间，会直接杀进程
+- ~~真寻从ctrl+c到彻底退出居然要六秒~~
+- 默认值: `20`
+
+
+## `bot.py`
+因为使用了 `spawn` 方式启动子进程，默认情况下会加载两次插件，如果你觉得这不是问题可以忽略这段，也不建议你在不懂的情况下修改 `bot.py`。
+
+推荐的写法是将 插件加载部分 和 启动部分 分开，以避免插件在主进程和子进程都加载一遍
+
+~~真寻启动居然要20秒~~
+
+```python
+#
+# 上面省略
+#
+
+if __name__ == "__mp_main__": # 仅在子进程运行的代码
+    # Please DO NOT modify this file unless you know what you are doing!
+    # As an alternative, you should use command `nb` or modify `pyproject.toml` to load plugins
+    # 加载插件
+    nonebot.load_from_toml("pyproject.toml")
+    # ...
+
+if __name__ == "__main__": # 仅在主进程运行的代码
+    # nonebot.logger.warning("Always use `nb run` to start the bot instead of manually running!")
+    # 运行 nonebot
+    nonebot.load_plugin("nonebot_plugin_reboot") # 加载重启插件
+    nonebot.run(app="__mp_main__:app")
+```
+
+
+## API
+```python
+require("nonebot_plugin_reboot")
+from nonebot_plugin_reboot import Reloader
+Reloader.reload(delay=5) # 可选参数 5秒后触发重启
+```
+
+
+## 依赖 
+- `nonebot2 >= 2.0.0beta.2`  
+
+启用 `reboot_load_command` 时需要以下依赖  
+- `nonebot-adapter-onebot`
```

### Comparing `nonebot_plugin_reboot-0.1.3/nonebot_plugin_reboot/reloader.py` & `nonebot_plugin_reboot-0.1.4/nonebot_plugin_reboot/reloader.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import threading
-from multiprocessing import get_context
-
-import nonebot
-from nonebot import logger
-
-from .config import plugin_config
-
-_nb_run = nonebot.run
-
-
-class Reloader:
-    event: threading.Event = None
-
-    @classmethod
-    def reload(cls, delay: int = 0):
-        if cls.event is None:
-            raise RuntimeError()
-        if delay > 0:
-            threading.Timer(delay, function=cls.event.set).start()
-            return
-        cls.event.set()
-
-
-def _run(ev: threading.Event, *args, **kwargs):
-    Reloader.event = ev
-    _nb_run(*args, **kwargs)
-
-
-def run(*args, **kwargs):
-    should_exit = False
-    ctx = get_context("spawn")
-    while not should_exit:
-        event = ctx.Event()
-        process = ctx.Process(
-            target=_run,
-            args=(
-                event,
-                *args,
-            ),
-            kwargs=kwargs,
-        )
-        process.start()
-        while not should_exit:
-            if event.wait(1):
-                logger.info("Receive reboot event")
-                process.terminate()
-                process.join(plugin_config.reboot_grace_time_limit)
-                if process.is_alive():
-                    logger.warning(
-                        f"Cannot shutdown gracefully in {plugin_config.reboot_grace_time_limit} second, force kill process."
-                    )
-                    process.kill()
-                break
-            elif process.is_alive():
-                continue
-            else:
-                # Process stoped without setting event
-                should_exit = True
-
-
-nonebot.run = run
+import threading
+from multiprocessing import get_context
+
+import nonebot
+from nonebot import logger
+
+from .config import plugin_config
+
+_nb_run = nonebot.run
+
+
+class Reloader:
+    event: threading.Event = None
+
+    @classmethod
+    def reload(cls, delay: int = 0):
+        if cls.event is None:
+            raise RuntimeError()
+        if delay > 0:
+            threading.Timer(delay, function=cls.event.set).start()
+            return
+        cls.event.set()
+
+
+def _run(ev: threading.Event, *args, **kwargs):
+    Reloader.event = ev
+    _nb_run(*args, **kwargs)
+
+
+def run(*args, **kwargs):
+    should_exit = False
+    ctx = get_context("spawn")
+    while not should_exit:
+        event = ctx.Event()
+        process = ctx.Process(
+            target=_run,
+            args=(
+                event,
+                *args,
+            ),
+            kwargs=kwargs,
+        )
+        process.start()
+        while not should_exit:
+            if event.wait(1):
+                logger.info("Receive reboot event")
+                process.terminate()
+                process.join(plugin_config.reboot_grace_time_limit)
+                if process.is_alive():
+                    logger.warning(
+                        f"Cannot shutdown gracefully in {plugin_config.reboot_grace_time_limit} second, force kill process."
+                    )
+                    process.kill()
+                break
+            elif process.is_alive():
+                continue
+            else:
+                # Process stoped without setting event
+                should_exit = True
+
+
+nonebot.run = run
```

### Comparing `nonebot_plugin_reboot-0.1.3/pyproject.toml` & `nonebot_plugin_reboot-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[tool.poetry]
-name = "nonebot_plugin_reboot"
-version = "0.1.3"
-description = "Reboot your bot by using command"
-license = "MIT"
-authors = ["18870 <a20110123@163.com>"]
-readme = "README.md"
-repository = "https://github.com/18870/nonebot-plugin-reboot"
-keywords = ["nonebot"]
-
-[tool.poetry.dependencies]
-python = "^3.7.3"
-nonebot2 = "^2.0.0-beta.2"
-nonebot-adapter-onebot = { version = "^2.1.0", optional = true }
-
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot_plugin_reboot"
+version = "0.1.4"
+description = "Reboot your bot by using command"
+license = "MIT"
+authors = ["18870 <a20110123@163.com>"]
+readme = "README.md"
+repository = "https://github.com/18870/nonebot-plugin-reboot"
+keywords = ["nonebot"]
+
+[tool.poetry.dependencies]
+python = "^3.7.3"
+nonebot2 = "^2.0.0-beta.2"
+nonebot-adapter-onebot = { version = "^2.1.0", optional = true }
+
+[tool.poetry.dev-dependencies]
+pytest = "^5.2"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_reboot-0.1.3/setup.py` & `nonebot_plugin_reboot-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,109 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-reboot
+Version: 0.1.4
+Summary: Reboot your bot by using command
+Home-page: https://github.com/18870/nonebot-plugin-reboot
+License: MIT
+Keywords: nonebot
+Author: 18870
+Author-email: a20110123@163.com
+Requires-Python: >=3.7.3,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0-beta.2,<3.0.0)
+Project-URL: Repository, https://github.com/18870/nonebot-plugin-reboot
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_reboot']
+# Nonebot-plugin-reboot 
+![](https://img.shields.io/badge/Development-Inactive-inactive) ![](https://img.shields.io/badge/PullRequests-Welcome-success)
 
-package_data = \
-{'': ['*']}
+用命令重启 bot 
 
-install_requires = \
-['nonebot2>=2.0.0-beta.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-reboot',
-    'version': '0.1.3',
-    'description': 'Reboot your bot by using command',
-    'long_description': '# Nonebot-plugin-reboot \n用命令重启 bot \n\n[![asciicast](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV.svg)](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV)\n\n## :warning:注意事项\n**不支持** `nb-cli`，即 `nb run` 启动方式。\n需要在 bot 目录下使用 `python bot.py` 启动。\n\n重启时直接对子进程使用 `process.terminate()`，如果你的其他插件启动了子进程，请确保它们能在设定的等待时间内正确关闭子进程，否则子进程会变成孤立进程。  \n:warning: Windows 下因系统 API 的限制进程会直接被杀死， **没有** 等待时间。\n\n<hr>  \n\n插件依赖于 `multiprocessing` `spawn` 生成子进程方式工作，支持由 `nb-cli` 生成的 bot.py，或任何显式加载了 `bot.py` 并在加载插件后调用 `nonebot.run` 的启动方式。  \n\n不支持 `nb run` 启动，因为 `nb run` 使用 `importlib` 在函数内加载 `bot.py`，multiprocessing 生成子进程时不会运行 `bot.py`，即 nonebot 初始化和加载插件的过程，导致启动失败。  \n\n得益于使用 `spawn` 方式启动，每次重启都相当于重新加载了所有代码。只有这个插件本身或者 `bot.py` 有更新时才需要彻底关闭 bot 重启。\n\n\n## 安装\n通过 nb-cli 安装:  \n`nb plugin install nonebot-plugin-reboot`  \n通过 pip 安装:  \n`pip install nonebot-plugin-reboot`  \n\n\n## 使用\n**超级用户**向机器人**私聊**发送**命令** `重启`, `reboot` 或 `restart`  \n> :warning: 注意命令的 `COMMAND_START`.  \n> 例如 /重启 、 /reboot 、 /restart\n\n\n## 配置项 \n`reboot_load_command`: `bool` \n- 加载内置的 `onebot v11` 重启命令 \n- 可以通过命令 `重启` `reboot` `restart` 触发重启 \n- 默认值: `True` \n\n`reboot_grace_time_limit`: `int`\n- 收到重启命令后等待进程退出的最长时间，超时会强制杀进程\n- 在 Windows 下没有等待时间，会直接杀进程\n- ~~真寻从ctrl+c到彻底退出居然要六秒~~\n- 默认值: `20`\n\n## `bot.py`\n因为使用了 `spawn` 方式启动子进程，默认的 bot.py 会加载两次插件。  \n\n推荐的写法是将 插件加载部分 和 nonebot启动部分 分开，以避免插件在主进程和子进程都加载一遍\n\n~~真寻启动居然要20秒~~\n\n```python\n#\n# 上面省略\n#\n\nif __name__ == "__mp_main__": # 仅在子进程运行的代码\n    # Please DO NOT modify this file unless you know what you are doing!\n    # As an alternative, you should use command `nb` or modify `pyproject.toml` to load plugins\n    # 加载插件\n    nonebot.load_from_toml("pyproject.toml")\n    nonebot.load_plugins("src/plugins")\n    nonebot.load_plugin("nonebot_plugin_xxxxxx")\n    # ...\n\nif __name__ == "__main__": # 仅在主进程运行的代码\n    # nonebot.logger.warning("Always use `nb run` to start the bot instead of manually running!")\n    # 运行 nonebot\n    nonebot.load_plugin("nonebot_plugin_reboot") # 加载重启插件\n    nonebot.run(app="__mp_main__:app")\n```\n\n\n## API\n```python\nrequire("nonebot_plugin_reboot")\nfrom nonebot_plugin_reboot import Reloader\nReloader.reload(delay=5) # 可选参数 5秒后触发重启\n```\n\n\n## 依赖 \n`nonebot2 >= 2.0.0beta.2`  \n\n启用 `reboot_load_command` 时需要以下依赖  \n`nonebot-adapter-onebot`',
-    'author': '18870',
-    'author_email': 'a20110123@163.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/18870/nonebot-plugin-reboot',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.3,<4.0.0',
-}
+[![asciicast](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV.svg)](https://asciinema.org/a/z10hzQ7Pgx4s9TVwj0nAv2TsV)
 
+## :warning:注意事项
+**必须要有** `bot.py`  
+新版 nb-cli 默认不生成 bot.py，需要在 nb 菜单里选择 `生成机器人的入口文件` / `Generate entry file of your bot.` 生成一个，不需要修改。 ~~不要再去群里问bot.py在哪了~~
 
-setup(**setup_kwargs)
+**不兼容** `fastapi_reload`，见 [#1](https://github.com/18870/nonebot-plugin-reboot/issues/1)、[#2](https://github.com/18870/nonebot-plugin-reboot/issues/2)。  
+不推荐使用 nb-cli 的 `--reload` 参数，这个插件是 `--reload` 在生产环境中的替代品。
+
+重启时直接对子进程使用 `process.terminate()`，如果你的其他插件启动了子进程，请确保它们能在设定的等待时间内正确关闭子进程，否则子进程会变成孤立进程。  
+:warning: Windows 下因系统 API 的限制进程会直接被杀死， **没有** 等待时间。
+
+<hr>  
+
+插件依赖于 `multiprocessing` `spawn` 生成子进程方式工作，支持由 nb-cli 生成的 bot.py，以及其他在加载插件后调用 `nonebot.run()` 的启动方式。  
+
+
+## 安装
+通过 nb-cli 安装:  
+`nb plugin install nonebot-plugin-reboot`  
+
+新版 nb-cli 默认不生成 bot.py，需要在 nb 菜单里选择 `生成机器人的入口文件` / `Generate entry file of your bot.` 生成一个，不需要修改。
+
+
+## 使用
+**超级用户**向机器人**私聊**发送**命令** `重启`, `reboot` 或 `restart`  
+> :warning: 注意命令的 `COMMAND_START`.  
+> 例如 /重启 、 /reboot 、 /restart
+
+
+## 配置项 
+`reboot_load_command`: `bool` 
+- 加载内置的 `onebot v11` 重启命令 
+- 可以通过命令 `重启` `reboot` `restart` 触发重启 
+- 默认值: `True` 
+
+`reboot_grace_time_limit`: `int`
+- 收到重启命令后等待进程退出的最长时间，超时会强制杀进程
+- 在 Windows 下没有等待时间，会直接杀进程
+- ~~真寻从ctrl+c到彻底退出居然要六秒~~
+- 默认值: `20`
+
+
+## `bot.py`
+因为使用了 `spawn` 方式启动子进程，默认情况下会加载两次插件，如果你觉得这不是问题可以忽略这段，也不建议你在不懂的情况下修改 `bot.py`。
+
+推荐的写法是将 插件加载部分 和 启动部分 分开，以避免插件在主进程和子进程都加载一遍
+
+~~真寻启动居然要20秒~~
+
+```python
+#
+# 上面省略
+#
+
+if __name__ == "__mp_main__": # 仅在子进程运行的代码
+    # Please DO NOT modify this file unless you know what you are doing!
+    # As an alternative, you should use command `nb` or modify `pyproject.toml` to load plugins
+    # 加载插件
+    nonebot.load_from_toml("pyproject.toml")
+    # ...
+
+if __name__ == "__main__": # 仅在主进程运行的代码
+    # nonebot.logger.warning("Always use `nb run` to start the bot instead of manually running!")
+    # 运行 nonebot
+    nonebot.load_plugin("nonebot_plugin_reboot") # 加载重启插件
+    nonebot.run(app="__mp_main__:app")
+```
+
+
+## API
+```python
+require("nonebot_plugin_reboot")
+from nonebot_plugin_reboot import Reloader
+Reloader.reload(delay=5) # 可选参数 5秒后触发重启
+```
+
+
+## 依赖 
+- `nonebot2 >= 2.0.0beta.2`  
+
+启用 `reboot_load_command` 时需要以下依赖  
+- `nonebot-adapter-onebot`
```

