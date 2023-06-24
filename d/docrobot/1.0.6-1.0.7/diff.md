# Comparing `tmp/docrobot-1.0.6.tar.gz` & `tmp/docrobot-1.0.7.tar.gz`

## Comparing `docrobot-1.0.6.tar` & `docrobot-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.6/convert.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.6/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/form.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/form.ui
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.6/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.6/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.7/convert.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.7/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/form.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/form.ui
+-rw-r--r--   0        0        0    21618 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.7/LICENSE
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.0.7/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 docrobot-1.0.7/PKG-INFO
```

### Comparing `docrobot-1.0.6/.github/workflows/python-publish.yml` & `docrobot-1.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.6/src/docrobot/form.py` & `docrobot-1.0.7/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.6/src/docrobot/form.ui` & `docrobot-1.0.7/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.6/src/docrobot/guimain.pyw` & `docrobot-1.0.7/src/docrobot/guimain.pyw`

 * *Files 5% similar despite different names*

```diff
@@ -108,16 +108,15 @@
             # self.textEdit.append(project.p_order + ' 项目开始处理...')
             match = 0  # 已匹配条目数
             doc_name = ''
             try:
                 doc_name = self.workdir + '/RD' + project.p_order + project.p_name + '.docx'
                 document = Document(doc_name)
                 # debug_doc(document)
-                # TODO to be fixed
-                # replace_header(document)
+                match = match + self.replace_comname(document, project)
                 match = match + self.first_table(document, project)
                 match = match + self.start_time(document, project)
                 match = match + self.second_table(document, project)
                 match = match + self.third_table(document, project)
 
                 match = match + self.checkpat2(document, project)
 
@@ -138,44 +137,61 @@
 
     def checkpatent(self, modify=False):
         if modify:
             self.textEdit.setText('')
             self.update_data()
 
         match = 0  # 已匹配条目数
+        unmatch = 0  # 已匹配条目数
         changed = False
         wb = load_workbook(self.file_prj)
         ws = wb.active
         max_row_num = ws.max_row
         range_cell = ws[f'A3:P{max_row_num}']
         i: int = 0
         for r in range_cell:
             if r[11].value is None:
                 break
-            pat_name = str(r[11].value).strip()
 
+            pat_name = str(r[11].value).strip()
+            # 检查专利IP号
             if pat_name == '无':
                 if r[14].value != '无':
-                    self.textEdit.append(str(i + 3) + ' 行: ' + str(r[14].value) + ' ===> ' + '无')
+                    self.textEdit.append(self.arr_prj[i].p_order + ' 项目: ' + str(r[14].value) + ' ===> ' + '无')
                     r[14].value = pat_name
                     changed |= True
+                    unmatch = unmatch + 1
                 else:
                     match = match + 1
             else:
                 lst = pat_name.splitlines()
                 rep = [self.pat_dict[x] if x in self.pat_dict else x for x in lst]
                 for element in rep:
                     if re.search('^\d\d$', element) is None:
                         self.textEdit.append('专利IP错误：' + element)
                 rep = map(lambda e: 'IP' + e, rep)
                 new_ip = ';'.join(rep)
                 if r[14].value != new_ip:
-                    self.textEdit.append(str(i + 3) + ' 行: ' + str(r[14].value) + ' ===> ' + new_ip)
+                    self.textEdit.append(self.arr_prj[i].p_order + ' 项目: ' + str(r[14].value) + ' ===> ' + new_ip)
                     r[14].value = new_ip
                     changed |= True
+                    unmatch = unmatch + 1
+                else:
+                    match = match + 1
+
+            # 检查和替换项目人数
+            rnd_name = str(r[8].value).strip()
+            if not rnd_name.endswith('等'):
+                real_num = len(rnd_name.split('、'))
+                if real_num != int(r[6].value):
+                    self.textEdit.append(self.arr_prj[i].p_order + ' 项目: ' + '研发人员名字数量不匹配:' + rnd_name)
+                    self.textEdit.append('研发人数: ' + str(r[6].value) + ' ===> ' + str(real_num))
+                    r[6].value = real_num
+                    changed |= True
+                    unmatch = unmatch + 1
                 else:
                     match = match + 1
             i = i + 1
         try:
             if changed and modify:
                 wb.save(self.file_prj)
                 xl_app = DispatchEx("Excel.Application")
@@ -187,14 +203,16 @@
                 xl_book = None
                 xl_app.Quit()
                 xl_app = None
         except PermissionError:
             self.textEdit.append('写文件失败，关闭其他占用该文件的程序.' + self.file_prj)
         wb.close()
         self.textEdit.append('项目立项表IP更新完成。 <font color="green"><b>' + str(match) + ' </b></font> 项条目匹配。')
+        if unmatch != 0:
+            self.textEdit.append(' <font color="red"><b>' + str(unmatch) + ' </b></font> 项条目不匹配。')
 
     def checkpat2(self, doc, prj):
         match = 0
         lst = prj.pat_list.splitlines()
         for pat_name in lst:
             if pat_name in self.pat_dict2:
                 pat_num = self.pat_dict2[pat_name]
@@ -327,16 +345,47 @@
             for j, row in enumerate(table.rows):
                 for k, cell in enumerate(row.cells):
                     for l, para in enumerate(cell.paragraphs):
                         self.textEdit.append(f'Table.{i} Row.{j} Cell{k} Para.{l} : ', para.text, sep='')
                         # for j, run in enumerate(para.runs):
                         #     self.textEdit.append(f'Para.{i} Run{j}: ', run.text, sep='')
 
-    def replace_header(self, doc, prj):
-        self.check_replace(doc.sections[0].header.paragraphs, '.*公司', prj.com_name)
+    def replace_comname(self, doc, prj):
+        match = 0
+        para = doc.sections[0].header.paragraphs[0]
+        oldname = para.text.strip()
+
+        if prj.p_comname in para.text:
+            match = match +1
+        else:
+            self.textEdit.append(oldname + ' ===> ' + prj.p_comname)
+            # TODO 这个地方还有个问题， 先用临时凑合一下
+            # found = False
+            # for i, run in enumerate(para.runs):
+            #     if found:
+            #         run.clear()
+            #     if run.text != '':
+            #         run.text = '\t\t' + prj.p_comname
+            #         found = True
+            for i, run in enumerate(para.runs):
+                if run.text == oldname:
+                    run.text = prj.p_comname
+                    self.textEdit.append(oldname + ' ===> ' + prj.p_comname)
+                    match = match + 1
+        match = match + self.check_replace(doc.paragraphs, oldname, prj.p_comname)
+        for table in doc.tables:
+            for row in table.rows:
+                for cell in row.cells:
+                    match = match + self.check_replace(cell.paragraphs, oldname, prj.p_comname)
+
+        # 检查其他可能的未替换的内容，例如去掉深圳，有限公司等
+        # TODO
+
+        return match
+
 
     def first_table(self, doc, prj):
         match = 0
         if doc.tables[0].rows[0].cells[0].paragraphs[0].text == '项目名称：':
             doc.tables[0].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[0].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
@@ -362,26 +411,25 @@
     def second_table(self, doc, prj):
         match = 0
         if doc.tables[1].rows[0].cells[0].paragraphs[0].text == '项目立项名称':
             doc.tables[1].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
 
-        match = match + self.check_replace(doc.tables[1].rows[1].cells[1].paragraphs
-                                           , '项目团队由(.*)人组成，项目实施周期为(.*)个月。'
-                                           ,
+        match = match + self.check_replace(doc.tables[1].rows[1].cells[1].paragraphs,
+                                           '项目团队由(.*)人组成，项目实施周期为(.*)个月。',
                                            '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
-        match = match + self.check_replace(doc.tables[1].rows[6].cells[1].paragraphs
-                                           , '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
+        match = match + self.check_replace(doc.tables[1].rows[6].cells[1].paragraphs,
+                                           '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
                                            prj.p_start + '至' + prj.p_end)
-        match = match + self.check_replace(doc.tables[1].rows[7].cells[1].paragraphs
-                                           , '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
+        match = match + self.check_replace(doc.tables[1].rows[7].cells[1].paragraphs,
+                                           '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
 
-        match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs
-                                           , '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
+        match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs,
+                                           '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
         if prj.p_owner != 'None':
             match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
                                                '项目负责人：' + prj.p_owner)
         if prj.p_rnd != 'None':
             match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*',
                                                '研发成员：' + prj.p_rnd)
         match = match + self.check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
@@ -406,18 +454,18 @@
 
     def third_table(self, doc, prj):
         match = 0
         if doc.tables[2].rows[0].cells[0].paragraphs[0].text == '项目名称':
             doc.tables[2].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[2].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
-        match = match + self.check_replace(doc.tables[2].rows[1].cells[1].paragraphs
-                                           , '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
-        match = match + self.check_replace(doc.tables[2].rows[2].cells[1].paragraphs
-                                           , '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
+        match = match + self.check_replace(doc.tables[2].rows[1].cells[1].paragraphs,
+                                           '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
+        match = match + self.check_replace(doc.tables[2].rows[2].cells[1].paragraphs,
+                                           '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
                                            prj.p_start + '至' + prj.p_end)
 
         if prj.p_owner != 'None':
             doc.tables[2].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_owner
             self.clear_runs(doc.tables[2].rows[3].cells[1].paragraphs[0].runs)
             match = match + 1
         return match
```

### Comparing `docrobot-1.0.6/LICENSE` & `docrobot-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.6/pyproject.toml` & `docrobot-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.6/PKG-INFO` & `docrobot-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.6
+Version: 1.0.7
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,9 +23,9 @@
 安装:  pip install docrobot  
 升级： pip install --upgrade docrobot
 
 然后找到
 
 构建环境准备:
 python -m pip install -U pip setuptools
-pip install pywin32 colorama python-docx openpyxl pyside6 -i https://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com
+pip install pywin32 python-docx openpyxl pyside6 -i https://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com
```

