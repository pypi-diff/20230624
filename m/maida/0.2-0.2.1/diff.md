# Comparing `tmp/maida-0.2.tar.gz` & `tmp/maida-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maida-0.2.tar", last modified: Sun Nov 27 04:22:11 2022, max compression
+gzip compressed data, was "maida-0.2.1.tar", last modified: Sat Jun 24 07:39:57 2023, max compression
```

## Comparing `maida-0.2.tar` & `maida-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-27 04:22:11.523749 maida-0.2/
--rw-rw-rw-   0        0        0     1085 2022-02-21 12:40:50.000000 maida-0.2/LICENSE
--rw-rw-rw-   0        0        0     2072 2022-11-27 04:22:11.523749 maida-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1603 2022-11-15 11:42:59.000000 maida-0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-27 04:22:11.476881 maida-0.2/maida/
--rw-rw-rw-   0        0        0       85 2022-11-15 11:42:16.000000 maida-0.2/maida/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-27 04:22:11.523749 maida-0.2/maida/mail/
--rw-rw-rw-   0        0        0     7403 2022-09-14 07:27:19.000000 maida-0.2/maida/mail/__init__.py
--rw-rw-rw-   0        0        0     1493 2022-02-28 03:39:52.000000 maida-0.2/maida/merge_ts_2_mp4.py
-drwxrwxrwx   0        0        0        0 2022-11-27 04:22:11.523749 maida-0.2/maida/ocr/
--rw-rw-rw-   0        0        0     2410 2022-11-27 04:21:52.000000 maida-0.2/maida/ocr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-27 04:22:11.508094 maida-0.2/maida.egg-info/
--rw-rw-rw-   0        0        0     2072 2022-11-27 04:22:11.000000 maida-0.2/maida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-11-27 04:22:11.000000 maida-0.2/maida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-27 04:22:11.000000 maida-0.2/maida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-11-27 04:22:11.000000 maida-0.2/maida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-27 04:22:11.000000 maida-0.2/maida.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-27 04:22:11.523749 maida-0.2/setup.cfg
--rw-rw-rw-   0        0        0      742 2022-11-15 11:32:13.000000 maida-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:39:57.213989 maida-0.2.1/
+-rw-rw-rw-   0        0        0     1085 2022-02-21 12:40:50.000000 maida-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2034 2023-06-24 07:39:57.211990 maida-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-01-18 01:52:38.000000 maida-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 07:39:57.190476 maida-0.2.1/maida/
+-rw-rw-rw-   0        0        0       85 2022-11-15 11:42:16.000000 maida-0.2.1/maida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:39:57.204465 maida-0.2.1/maida/mail/
+-rw-rw-rw-   0        0        0     7940 2023-06-24 06:54:18.000000 maida-0.2.1/maida/mail/__init__.py
+-rw-rw-rw-   0        0        0     1493 2022-02-28 03:39:52.000000 maida-0.2.1/maida/merge_ts_2_mp4.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:39:57.208994 maida-0.2.1/maida/ocr/
+-rw-rw-rw-   0        0        0     2410 2022-11-27 04:21:52.000000 maida-0.2.1/maida/ocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:39:57.202470 maida-0.2.1/maida.egg-info/
+-rw-rw-rw-   0        0        0     2034 2023-06-24 07:39:57.000000 maida-0.2.1/maida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-24 07:39:57.000000 maida-0.2.1/maida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 07:39:57.000000 maida-0.2.1/maida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-24 07:39:57.000000 maida-0.2.1/maida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-24 07:39:57.000000 maida-0.2.1/maida.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 07:39:57.213989 maida-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-24 06:54:18.000000 maida-0.2.1/setup.py
```

### Comparing `maida-0.2/LICENSE` & `maida-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maida-0.2/PKG-INFO` & `maida-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: maida
-Version: 0.2
+Version: 0.2.1
 Summary: No description.
 Home-page: https://github.com/LZC6244/maida
 Author: maida
 Author-email: 624486877@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ocr
 License-File: LICENSE
@@ -22,25 +20,21 @@
 2. 小说图片转文字
 
 ---
 ## 安装
 可以直接 `pip` 安装
 > pip install maida
 
-win 平台安装时若报 `python-levenshtein` 安装失败请根据提示安装相应环境  
-
-或在 https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-levenshtein 使用 whl 安装
-
 ##  mail
 ###  EmailSender
 基于 `smtplib` 的发送邮件脚本  
 ```text
 1. 可以发送文本
 2. 可以发送图片
-3. 可以发送附件（图片、文件等），`附件文件名可以包含中文` 
+3. 可以发送附件（图片、文件等），附件文件名可以包含中文
 4. 可以群发邮件
 5. 可以设置邮件优先级（如标红）
 ```
 
 ### demo
 ```text
 from maida import EmailSender
@@ -54,14 +48,20 @@
 ```
 
 ## ocr【可选】
 
 **安装方式**
 
 > pip install maida[ocr]
+
+win 平台安装时若报 `python-levenshtein` 安装失败请根据提示安装相应环境  
+
+或在 https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-levenshtein 使用 whl 安装
+
+
 ### img_2_cn
 基于 [cnocr](https://github.com/breezedeus/cnocr) 的小说图片转中文文字脚本  
 
 这里提供了一个[来源于网上的小说图片样例](https://github.com/LZC6244/maida/blob/master/test_files/test_img_2_cn.gif)  
 
 可以看出识别效果还是不错的
 
@@ -71,9 +71,7 @@
 
 print(img_2_cn('xxx.gif'))
 ```
 
 ## 版本历程
 详见 [history.md](https://github.com/LZC6244/maida/blob/master/docs/history.md)
 
-
-
```

### Comparing `maida-0.2/README.md` & `maida-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 2. 小说图片转文字
 
 ---
 ## 安装
 可以直接 `pip` 安装
 > pip install maida
 
-win 平台安装时若报 `python-levenshtein` 安装失败请根据提示安装相应环境  
-
-或在 https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-levenshtein 使用 whl 安装
-
 ##  mail
 ###  EmailSender
 基于 `smtplib` 的发送邮件脚本  
 ```text
 1. 可以发送文本
 2. 可以发送图片
-3. 可以发送附件（图片、文件等），`附件文件名可以包含中文` 
+3. 可以发送附件（图片、文件等），附件文件名可以包含中文
 4. 可以群发邮件
 5. 可以设置邮件优先级（如标红）
 ```
 
 ### demo
 ```text
 from maida import EmailSender
@@ -37,14 +33,20 @@
 ```
 
 ## ocr【可选】
 
 **安装方式**
 
 > pip install maida[ocr]
+
+win 平台安装时若报 `python-levenshtein` 安装失败请根据提示安装相应环境  
+
+或在 https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-levenshtein 使用 whl 安装
+
+
 ### img_2_cn
 基于 [cnocr](https://github.com/breezedeus/cnocr) 的小说图片转中文文字脚本  
 
 这里提供了一个[来源于网上的小说图片样例](https://github.com/LZC6244/maida/blob/master/test_files/test_img_2_cn.gif)  
 
 可以看出识别效果还是不错的
```

### Comparing `maida-0.2/maida/mail/__init__.py` & `maida-0.2.1/maida/mail/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,48 +20,78 @@
 
 
 class EmailSender(object):
     from_addr: str
     mail_log: bool
     msg = None
 
-    def __init__(self, email_host, email_port, from_addr, need_auth=True, email_pass=None, mail_log: bool = True):
+    def __init__(self, email_host, email_port, from_addr, need_auth=True, email_pass=None,
+                 mail_ssl=True, mail_tls=True, mail_log: bool = True):
         """
         :param email_host: smtp 服务器地址，如 'smtp.163.com'
         :param email_port: smtp 服务器端口，如 465
         :param from_addr: 发件人
         :param need_auth: 发送邮件是否需要验证，默认为 Ture
         :param email_pass: 发件人授权码
+        :param mail_ssl:是否使用ssl加密连接
+        :param mail_tls:是否使用tls加密连接
         :param mail_log: 是否记录 mail 日志
         """
         self.email_host = email_host
         self.email_port = email_port
         self.from_addr = from_addr
-        self.need_auth = need_auth
         self.email_pass = email_pass
         self.mail_log = mail_log
         self.msg = MIMEMultipart()
         self.from_addr = from_addr
         self.msg['From'] = self.from_addr
 
+        if mail_ssl:
+            # 在创建客户端对象的同时，使用SSL加密连接到邮箱服务器
+            self.cli = smtplib.SMTP_SSL(host=self.email_host, port=self.email_port)
+        else:
+            self.cli = smtplib.SMTP(host=self.email_host, port=self.email_port)
+            if mail_tls:
+                self.cli.starttls()
+        if need_auth:
+            login_result = self.cli.login(self.from_addr, self.email_pass)
+            if login_result and login_result[0] == 235:
+                if self.mail_log:
+                    logger.info(f'[ EmailSender ] Login successful')
+            else:
+                raise UserWarning('[ EmailSender ] Login failed: ', login_result[0], login_result[1])
+        else:
+            logger.info(f'[ EmailSender ] Not need auth')
+
     def clear_attach(self):
         """还原为空白邮件"""
         # self.msg._payload.clear()
         self.msg = MIMEMultipart()
         self.msg['From'] = self.from_addr
 
     def attach_text(self, text=''):
         # 添加邮件正文 （ 纯文本 ）
         msg_text = MIMEText(text, 'plain', 'utf8')
         self.msg.attach(msg_text)
 
     def attach_html(self, text=''):
-        # 添加邮件正文 （ html ）
-        # html 格式不固定，故请将 html 源码全部输入
-        # 此处不通过 MIMEImage 定义图片ID，在 HTML 文本中引用 （ ... ）
+        """
+        添加邮件正文 （ html ）
+        html 格式不固定，故请将 html 源码全部输入
+        此处建议通过 MIMEImage 定义图片 ID ，如果使用 base64 嵌入图片，邮件中仍有几率不显示图片
+        解释：<img>元素引用的不是外部图片，而是邮件内的图片资源附件，故不会被屏蔽。
+        示例如下：
+        from email.mime.image import MIMEImage
+
+        with open('demo.png','rb') as f:
+            img = MIMEImage(f.read())
+            img.add_header('Content-ID','<111>')
+            self.msg.attach(img)
+        mail_body_html='<img src="cid:111">'
+        """
         msg_text = MIMEText(text, 'html', 'utf8')
         self.msg.attach(msg_text)
 
     def attach_file(self, file: Union[str, bytes], file_name=None):
         """
         添加邮件附件
         :param file: 附件路径或者附件二进制，如：
@@ -90,21 +120,19 @@
         else:
             # 文件名不含中文 （ add_header的第一种写法 ）
             att.add_header('content-disposition', 'attachment', filename=file_name)
             # 或者可以这样写
             # att['Content-Disposition'] = 'attachment;filename="%s"' % filename
         self.msg.attach(att)
 
-    def send(self, to_addrs, subject, cc_addrs=None, mail_ssl=True, mail_tls=True, x_priority='3', **kwargs):
+    def send(self, to_addrs, subject, cc_addrs=None, x_priority='3', **kwargs):
         """
         :param to_addrs:收件人（收件人为字符串时，视其为一个仅含该字符串的列表）
         :param subject:邮件标题
         :param cc_addrs:抄送人
-        :param mail_ssl:是否使用ssl加密连接
-        :param mail_tls:是否使用tls加密连接
         :param x_priority:邮件优先级 （ 等同于 email Message 的 X-Priority ）
                 '1'	最高级别（重要性高）
                 '2'	介于中间 （高）
                 '3'	普通级别（不提示重要性）
                 '4'	介于中间 （低）
                 '5'	最低级别（重要性低）
                 '其他' 普通级别（不提示重要性）
@@ -131,43 +159,29 @@
         # 需为用 ';' 连接的字符串
         self.msg['To'] = ','.join(to_addrs)
         self.msg['Subject'] = subject
         self.msg['X-Priority'] = x_priority
         for k, v in kwargs.items():
             self.msg[k] = v
 
-        if mail_ssl:
-            # 在创建客户端对象的同时，使用SSL加密连接到邮箱服务器
-            client = smtplib.SMTP_SSL(host=self.email_host, port=self.email_port)
-        else:
-            client = smtplib.SMTP(host=self.email_host, port=self.email_port)
-            if mail_tls:
-                client.starttls()
-        if self.need_auth:
-            login_result = client.login(self.from_addr, self.email_pass)
-            if login_result and login_result[0] == 235:
-                if self.mail_log:
-                    logger.info(f'[ EmailSender ] Login successful: {subject}')
-            else:
-                raise UserWarning('[ EmailSender ] Login failed: ', login_result[0], login_result[1], f'--- {subject}')
-        else:
-            logger.info(f'[ EmailSender ] Not need auth: {subject}')
-
         from_addr = self.msg['From']
         # 需为一个 list
         to_addrs = self.msg['To'].split(',')
         if self.msg['Cc']:
             cc_addrs = self.msg['Cc'].split(',')
             to_addrs.extend(cc_addrs)
         try:
-            client.sendmail(from_addr, to_addrs, self.msg.as_string())
+            self.cli.sendmail(from_addr, to_addrs, self.msg.as_string())
             if self.mail_log:
                 logger.info(f'[ EmailSender ] Email sent successful: {subject}')
-        finally:
-            client.close()
+        except Exception as e:
+            logger.error(f'[ EmailSender ] Email sent failed: {subject}\n\n{repr(e)}')
+
+    def close(self):
+        self.cli.close()
 
 
 if __name__ == '__main__':
     email_sender = EmailSender(email_host='smtp.qq.com', email_port=465, from_addr='xxx@qq.com', email_pass='xxx')
     content = '这是 maida 发送过来的邮件。请注意查收！'
     email_sender.attach_text(text=content)
     email_sender.attach_file(r'C:\xxx\xx.jpg')
```

### Comparing `maida-0.2/maida/merge_ts_2_mp4.py` & `maida-0.2.1/maida/merge_ts_2_mp4.py`

 * *Files identical despite different names*

### Comparing `maida-0.2/maida/ocr/__init__.py` & `maida-0.2.1/maida/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `maida-0.2/maida.egg-info/PKG-INFO` & `maida-0.2.1/maida.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: maida
-Version: 0.2
+Version: 0.2.1
 Summary: No description.
 Home-page: https://github.com/LZC6244/maida
 Author: maida
 Author-email: 624486877@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ocr
 License-File: LICENSE
@@ -22,25 +20,21 @@
 2. 小说图片转文字
 
 ---
 ## 安装
 可以直接 `pip` 安装
 > pip install maida
 
-win 平台安装时若报 `python-levenshtein` 安装失败请根据提示安装相应环境  
-
-或在 https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-levenshtein 使用 whl 安装
-
 ##  mail
 ###  EmailSender
 基于 `smtplib` 的发送邮件脚本  
 ```text
 1. 可以发送文本
 2. 可以发送图片
-3. 可以发送附件（图片、文件等），`附件文件名可以包含中文` 
+3. 可以发送附件（图片、文件等），附件文件名可以包含中文
 4. 可以群发邮件
 5. 可以设置邮件优先级（如标红）
 ```
 
 ### demo
 ```text
 from maida import EmailSender
@@ -54,14 +48,20 @@
 ```
 
 ## ocr【可选】
 
 **安装方式**
 
 > pip install maida[ocr]
+
+win 平台安装时若报 `python-levenshtein` 安装失败请根据提示安装相应环境  
+
+或在 https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-levenshtein 使用 whl 安装
+
+
 ### img_2_cn
 基于 [cnocr](https://github.com/breezedeus/cnocr) 的小说图片转中文文字脚本  
 
 这里提供了一个[来源于网上的小说图片样例](https://github.com/LZC6244/maida/blob/master/test_files/test_img_2_cn.gif)  
 
 可以看出识别效果还是不错的
 
@@ -71,9 +71,7 @@
 
 print(img_2_cn('xxx.gif'))
 ```
 
 ## 版本历程
 详见 [history.md](https://github.com/LZC6244/maida/blob/master/docs/history.md)
 
-
-
```

### Comparing `maida-0.2/setup.py` & `maida-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="maida",
-    version="0.2",
+    version="0.2.1",
     author="maida",
     author_email="624486877@qq.com",
     description="No description.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LZC6244/maida",
     packages=setuptools.find_packages(),
```

