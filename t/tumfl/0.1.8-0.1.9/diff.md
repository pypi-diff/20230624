# Comparing `tmp/tumfl-0.1.8.tar.gz` & `tmp/tumfl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumfl-0.1.8.tar", last modified: Mon May 22 15:03:54 2023, max compression
+gzip compressed data, was "tumfl-0.1.9.tar", last modified: Sat Jun 24 12:20:02 2023, max compression
```

## Comparing `tumfl-0.1.8.tar` & `tumfl-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.422342 tumfl-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 15:03:54.422342 tumfl-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 15:03:41.000000 tumfl-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 15:03:41.000000 tumfl-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 15:03:54.422342 tumfl-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.414342 tumfl-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_dependency_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37003 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.414342 tumfl-0.1.8/tumfl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.418342 tumfl-0.1.8/tumfl/AST/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/ASTNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/BaseFunctionDefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.418342 tumfl-0.1.8/tumfl/AST/Expression/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/BinOp.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/ExpFunctionCall.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/ExpFunctionDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/ExpMethodInvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Index.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/NamedIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Nil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Number.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/String.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/TableField.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/UnOp.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Vararg.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.422342 tumfl-0.1.8/tumfl/AST/Statement/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Assign.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Block.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Break.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/FunctionCall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/FunctionDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Goto.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/If.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/IterativeFor.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/LocalAssign.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/LocalFunctionDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/MethodInvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/NumericFor.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Semicolon.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/While.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/basic_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/dependency_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32804 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.414342 tumfl-0.1.8/tumfl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.343359 tumfl-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-24 12:20:02.343359 tumfl-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-24 12:19:52.000000 tumfl-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 12:19:52.000000 tumfl-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-24 12:20:02.343359 tumfl-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.335359 tumfl-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-24 12:19:52.000000 tumfl-0.1.9/test/test_dependency_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-06-24 12:19:52.000000 tumfl-0.1.9/test/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-06-24 12:19:52.000000 tumfl-0.1.9/test/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37124 2023-06-24 12:19:52.000000 tumfl-0.1.9/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.339359 tumfl-0.1.9/tumfl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.339359 tumfl-0.1.9/tumfl/AST/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/ASTNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/BaseFunctionDefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.339359 tumfl-0.1.9/tumfl/AST/Expression/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/BinOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/ExpFunctionCall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/ExpFunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/ExpMethodInvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/NamedIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Nil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/String.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/TableField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/UnOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Vararg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/Variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.343359 tumfl-0.1.9/tumfl/AST/Statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/FunctionCall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/FunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Goto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/IterativeFor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/LocalAssign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/LocalFunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/MethodInvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/NumericFor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Semicolon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/Statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/While.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/Statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/AST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/basic_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/dependency_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-24 12:19:52.000000 tumfl-0.1.9/tumfl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:20:02.339359 tumfl-0.1.9/tumfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-24 12:20:02.000000 tumfl-0.1.9/tumfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-24 12:20:02.000000 tumfl-0.1.9/tumfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:20:02.000000 tumfl-0.1.9/tumfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-24 12:20:02.000000 tumfl-0.1.9/tumfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 12:20:02.000000 tumfl-0.1.9/tumfl.egg-info/top_level.txt
```

### Comparing `tumfl-0.1.8/PKG-INFO` & `tumfl-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.8
+Version: 0.1.9
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.8/pyproject.toml` & `tumfl-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tumfl"
-version = "0.1.8"
+version = "0.1.9"
 description = "The Ultimate Minimizer For Lua: minimize your lua scripts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["lua", "minimizer", "ast"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `tumfl-0.1.8/test/test_dependency_resolver.py` & `tumfl-0.1.9/test/test_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/test/test_formatter.py` & `tumfl-0.1.9/test/test_formatter.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/test/test_lexer.py` & `tumfl-0.1.9/test/test_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,7 +300,19 @@
         self.assertEqual(lex.get_next_token(), Token(TokenType.ELLIPSIS, "...", 0, 0))
         self.assertEqual(lex.get_next_token(), Token(TokenType.EOF, "eof", 0, 0))
         lex = Lexer("..a...b")
         self.assertEqual(lex.get_next_token(), Token(TokenType.CONCAT, "..", 0, 0))
         self.assertEqual(lex.get_next_token(), Token(TokenType.NAME, "a", 0, 0))
         self.assertEqual(lex.get_next_token(), Token(TokenType.ELLIPSIS, "...", 0, 0))
         self.assertEqual(lex.get_next_token(), Token(TokenType.NAME, "b", 0, 0))
+
+
+class TestShebang(unittest.TestCase):
+    def test_shebang(self):
+        lex = Lexer("#!abc\na")
+        self.assertEqual(lex.get_next_token().type, TokenType.NAME)
+
+
+class EmptyTest(unittest.TestCase):
+    def test_empty(self):
+        lex = Lexer("")
+        self.assertEqual(lex.get_next_token().type, TokenType.EOF)
```

### Comparing `tumfl-0.1.8/test/test_parser.py` & `tumfl-0.1.9/test/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,7 +873,13 @@
                 [],
             )
         )
         repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
+
+
+class EmptyTest(unittest.TestCase):
+    def test_empty(self):
+        parser = Parser("")
+        parser.parse_chunk()
```

### Comparing `tumfl-0.1.8/tumfl/AST/ASTNode.py` & `tumfl-0.1.9/tumfl/AST/ASTNode.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/BaseFunctionDefinition.py` & `tumfl-0.1.9/tumfl/AST/BaseFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/BinOp.py` & `tumfl-0.1.9/tumfl/AST/Expression/BinOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/ExpFunctionDefinition.py` & `tumfl-0.1.9/tumfl/AST/Expression/ExpFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/ExpMethodInvocation.py` & `tumfl-0.1.9/tumfl/AST/Expression/ExpMethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/Name.py` & `tumfl-0.1.9/tumfl/AST/Expression/Name.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/Number.py` & `tumfl-0.1.9/tumfl/AST/Expression/Number.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/String.py` & `tumfl-0.1.9/tumfl/AST/Expression/String.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/TableField.py` & `tumfl-0.1.9/tumfl/AST/Expression/TableField.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/UnOp.py` & `tumfl-0.1.9/tumfl/AST/Expression/UnOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Expression/__init__.py` & `tumfl-0.1.9/tumfl/AST/Expression/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/Assign.py` & `tumfl-0.1.9/tumfl/AST/Statement/Assign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/FunctionCall.py` & `tumfl-0.1.9/tumfl/AST/Statement/FunctionCall.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/FunctionDefinition.py` & `tumfl-0.1.9/tumfl/AST/Statement/FunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/If.py` & `tumfl-0.1.9/tumfl/AST/Statement/If.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/IterativeFor.py` & `tumfl-0.1.9/tumfl/AST/Statement/IterativeFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/LocalAssign.py` & `tumfl-0.1.9/tumfl/AST/Statement/LocalAssign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/LocalFunctionDefinition.py` & `tumfl-0.1.9/tumfl/AST/Statement/LocalFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/MethodInvocation.py` & `tumfl-0.1.9/tumfl/AST/Statement/MethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/NumericFor.py` & `tumfl-0.1.9/tumfl/AST/Statement/NumericFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/AST/Statement/__init__.py` & `tumfl-0.1.9/tumfl/AST/Statement/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/Token.py` & `tumfl-0.1.9/tumfl/Token.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/basic_walker.py` & `tumfl-0.1.9/tumfl/basic_walker.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/dependency_resolver.py` & `tumfl-0.1.9/tumfl/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/error.py` & `tumfl-0.1.9/tumfl/error.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/formatter.py` & `tumfl-0.1.9/tumfl/formatter.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl/lexer.py` & `tumfl-0.1.9/tumfl/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,21 +66,22 @@
 class Lexer:
     def __init__(
         self, text: str, typed: bool = False, ignore_unicode_errors: bool = False
     ) -> None:
         self.text: str = text
         self.text_len: int = len(self.text)
         self.line: int = 0
-        self.column: int = 0
-        self.pos: int = 0
+        self.column: int = -1
+        self.pos: int = -1
         self.newline_warn: int = 0
-        self.current_char: Optional[str] = self.text[self.pos]
+        self.current_char: Optional[str] = None
         self.last_hint: Optional[Tuple[str, int, int]] = None
         self.comments: list[str] = []
         self.unicode_errors: str = "ignore" if ignore_unicode_errors else "strict"
+        self.advance()
         include_typing(typed)
 
     def error(
         self, message: str, line: Optional[int] = None, column: Optional[int] = None
     ) -> NoReturn:
         current_line: int = line if line is not None else self.line
         current_column = column if column is not None else self.column
```

### Comparing `tumfl-0.1.8/tumfl/parser.py` & `tumfl-0.1.9/tumfl/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if self.current_token.type == TokenType.RETURN:
             self._eat_token(TokenType.RETURN)
             if (
                 self.current_token.type
                 not in (TokenType.SEMICOLON,) + self._BLOCK_END_TYPES
             ):
                 block.returns = self._parse_exp_list()
-            if self.current_token.type == TokenType.SEMICOLON:
+            if self.current_token.type == TokenType.SEMICOLON:  # type: ignore
                 self._eat_token()
         if expect_end:
             self._eat_token(TokenType.END)
         return block
 
     def _parse_statement(self) -> Statement:
         """Parse a statement"""
@@ -358,15 +358,15 @@
         funcbody: L_PAREN [namelist [COMMA ELLIPSIS] | ELLIPSIS] R_PAREN block END
         """
         self._switch_hint("parameters")
         self._eat_token(TokenType.L_PAREN)
         parameters: list[Name | Vararg] = []
         if self.current_token.type == TokenType.NAME:
             parameters.extend(self._parse_name_list(leave_vararg=True))
-            if self.current_token.type == TokenType.ELLIPSIS:
+            if self.current_token.type == TokenType.ELLIPSIS:  # type: ignore
                 self._switch_hint("varargs")
                 parameters.append(Vararg.from_token(self.current_token))
                 self._eat_token()
         elif self.current_token.type == TokenType.ELLIPSIS:
             self._switch_hint("varargs")
             parameters.append(Vararg.from_token(self.current_token))
             self._eat_token()
@@ -865,15 +865,15 @@
 
         args: L_PAREN [explist] R_PAREN | tableconstructor | LiteralString
         """
         self._add_hint("function call", "arguments")
         expressions: list[Expression] = []
         if self.current_token.type == TokenType.L_PAREN:
             self._eat_token()
-            if self.current_token.type != TokenType.R_PAREN:
+            if self.current_token.type != TokenType.R_PAREN:  # type: ignore
                 expressions = self._parse_exp_list()
             self._eat_token(TokenType.R_PAREN)
         elif self.current_token.type == TokenType.L_CURL:
             expressions.append(self._parse_table_constructor())
         elif self.current_token.type == TokenType.STRING:
             expressions.append(String.from_token(self.current_token))
             self._eat_token()
```

### Comparing `tumfl-0.1.8/tumfl/utils.py` & `tumfl-0.1.9/tumfl/utils.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.8/tumfl.egg-info/PKG-INFO` & `tumfl-0.1.9/tumfl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.8
+Version: 0.1.9
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.8/tumfl.egg-info/SOURCES.txt` & `tumfl-0.1.9/tumfl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

