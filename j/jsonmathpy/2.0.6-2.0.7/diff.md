# Comparing `tmp/jsonmathpy-2.0.6.tar.gz` & `tmp/jsonmathpy-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-2.0.6.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.7.tar", max compression
```

## Comparing `jsonmathpy-2.0.6.tar` & `jsonmathpy-2.0.7.tar`

### file list

```diff
@@ -1,44 +1,42 @@
--rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.6/LICENSE
--rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.6/jsonmathpy/README.md
--rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.6/jsonmathpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.6/jsonmathpy/builders/__init__.py
--rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.6/jsonmathpy/builders/interpreter_builder.py
--rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.6/jsonmathpy/builders/jsonmath_builder.py
--rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.6/jsonmathpy/builders/parser_builder.py
--rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.6/jsonmathpy/core/__init__.py
--rw-r--r--   0        0        0     1287 2023-06-13 19:58:26.356080 jsonmathpy-2.0.6/jsonmathpy/core/interpreter.py
--rw-r--r--   0        0        0      900 2023-06-15 21:00:24.419519 jsonmathpy-2.0.6/jsonmathpy/core/iterator.py
--rw-r--r--   0        0        0     4745 2023-06-15 20:59:55.159008 jsonmathpy-2.0.6/jsonmathpy/core/lexer.py
--rw-r--r--   0        0        0     2759 2023-06-13 19:26:07.972851 jsonmathpy-2.0.6/jsonmathpy/core/nodes.py
--rw-r--r--   0        0        0    11182 2023-06-13 19:31:22.017454 jsonmathpy-2.0.6/jsonmathpy/core/parser.py
--rw-r--r--   0        0        0     4430 2023-06-15 20:53:09.608696 jsonmathpy-2.0.6/jsonmathpy/core/token.py
--rw-r--r--   0        0        0     5686 2023-06-13 19:31:19.329405 jsonmathpy-2.0.6/jsonmathpy/core/types.py
--rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.6/jsonmathpy/interfaces/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.6/jsonmathpy/interfaces/interpreter.py
--rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.6/jsonmathpy/interfaces/interpreter_service.py
--rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.6/jsonmathpy/interfaces/iterator.py
--rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.6/jsonmathpy/interfaces/json_math.py
--rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.6/jsonmathpy/interfaces/lexer.py
--rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.6/jsonmathpy/interfaces/node_provider.py
--rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.6/jsonmathpy/interfaces/parser.py
--rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.6/jsonmathpy/interfaces/parser_service.py
--rw-r--r--   0        0        0      971 2023-06-15 20:53:09.608682 jsonmathpy-2.0.6/jsonmathpy/interfaces/tokens.py
--rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.6/jsonmathpy/main/__init__.py
--rw-r--r--   0        0        0     2410 2023-06-13 19:35:45.765688 jsonmathpy-2.0.6/jsonmathpy/main/base_node.py
--rw-r--r--   0        0        0     1784 2023-06-13 19:35:48.269567 jsonmathpy-2.0.6/jsonmathpy/main/jsonmath.py
--rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.6/jsonmathpy/models/__init__.py
--rw-r--r--   0        0        0      107 2023-06-13 19:26:05.112561 jsonmathpy-2.0.6/jsonmathpy/models/basic_nodes.py
--rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.6/jsonmathpy/models/mapper.py
--rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.6/jsonmathpy/models/node_handler.py
--rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.6/jsonmathpy/models/node_keys.py
--rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.6/jsonmathpy/models/object_configuration.py
--rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.6/jsonmathpy/models/token.py
--rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.6/jsonmathpy/services/__init__.py
--rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.6/jsonmathpy/services/interpreter.py
--rw-r--r--   0        0        0     1414 2023-06-13 18:12:12.541638 jsonmathpy-2.0.6/jsonmathpy/services/parser.py
--rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.6/jsonmathpy/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.6/jsonmathpy/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.6/jsonmathpy/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.6/jsonmathpy/tests/tests_parser.py
--rw-r--r--   0        0        0      408 2023-06-15 22:03:00.770641 jsonmathpy-2.0.6/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.7/jsonmathpy/README.md
+-rw-r--r--   0        0        0       27 2023-06-18 14:17:40.798737 jsonmathpy-2.0.7/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-20 10:52:52.796397 jsonmathpy-2.0.7/jsonmathpy/app.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.7/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0     1370 2023-06-18 14:23:41.762147 jsonmathpy-2.0.7/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      809 2023-06-18 13:59:09.276802 jsonmathpy-2.0.7/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3534 2023-06-18 13:59:09.276723 jsonmathpy-2.0.7/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2762 2023-06-18 13:59:09.276714 jsonmathpy-2.0.7/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    11293 2023-06-18 14:20:43.611071 jsonmathpy-2.0.7/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     4449 2023-06-18 13:59:09.276734 jsonmathpy-2.0.7/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.7/jsonmathpy/interpreter/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-18 14:15:39.247379 jsonmathpy-2.0.7/jsonmathpy/interpreter/interpreter.py
+-rw-r--r--   0        0        0      429 2023-06-18 13:59:09.276671 jsonmathpy-2.0.7/jsonmathpy/interpreter/service_provider.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.7/jsonmathpy/parser/__init__.py
+-rw-r--r--   0        0        0     1540 2023-06-18 14:44:01.487755 jsonmathpy-2.0.7/jsonmathpy/parser/parser.py
+-rw-r--r--   0        0        0     3159 2023-06-20 10:52:44.439227 jsonmathpy-2.0.7/jsonmathpy/parser/service_provider.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:31:29.763895 jsonmathpy-2.0.7/jsonmathpy/shared/__init__.py
+-rw-r--r--   0        0        0     5916 2023-06-18 13:59:09.276760 jsonmathpy-2.0.7/jsonmathpy/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/interpreter.py
+-rw-r--r--   0        0        0      136 2023-06-18 14:15:39.254443 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/parser.py
+-rw-r--r--   0        0        0      196 2023-06-18 14:19:25.879508 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/parser_service.py
+-rw-r--r--   0        0        0      971 2023-06-15 20:53:09.608682 jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/tokens.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.7/jsonmathpy/shared/models/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-13 19:26:05.112561 jsonmathpy-2.0.7/jsonmathpy/shared/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.7/jsonmathpy/shared/models/mapper.py
+-rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.7/jsonmathpy/shared/models/node_handler.py
+-rw-r--r--   0        0        0      564 2023-06-18 14:15:39.260113 jsonmathpy-2.0.7/jsonmathpy/shared/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.7/jsonmathpy/shared/models/object_configuration.py
+-rw-r--r--   0        0        0      164 2023-06-18 14:18:34.051143 jsonmathpy-2.0.7/jsonmathpy/shared/models/token.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.7/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.7/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.7/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.7/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      346 2023-06-24 18:11:20.820004 jsonmathpy-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 jsonmathpy-2.0.7/PKG-INFO
```

### Comparing `jsonmathpy-2.0.6/LICENSE` & `jsonmathpy-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.6/jsonmathpy/core/lexer.py` & `jsonmathpy-2.0.7/jsonmathpy/core/lexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-from jsonmathpy.interfaces.iterator import IIterator
-from jsonmathpy.interfaces.lexer import ILexer
-from jsonmathpy.interfaces.tokens import ITokenProvider
-from jsonmathpy.core.types import TokenSinglets, TokenType
-from enum import Enum
-
-
-class Characters(Enum):
-    """An object containing the set of supported characters, keyd on a set name."""
-    WHITESPACE          = ' \n\t'
-    DIGITS              = '0987654321'
-    LOWERCASECHARACTERS = 'abcdefghijklmnopqrstuvwxyz'
-    UPPERCASECHARACTERS = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-    NONLETTERCHARACTERS = '_{}:^;'
-    OPERATIONS          = '*-+=[](){}^/|&!~><:;.,@%'
-    LETTERS             = LOWERCASECHARACTERS + UPPERCASECHARACTERS
-    CHARACTERS          = LOWERCASECHARACTERS + UPPERCASECHARACTERS + NONLETTERCHARACTERS
-    OBJECTCHARACTERS    = LOWERCASECHARACTERS + UPPERCASECHARACTERS + NONLETTERCHARACTERS + DIGITS
+from jsonmathpy.shared.interfaces.iterator import IIterator
+from jsonmathpy.shared.interfaces.lexer import ILexer
+from jsonmathpy.shared.interfaces.tokens import ITokenProvider
+from jsonmathpy.shared.constants import TokenType
+from jsonmathpy.shared.constants import Characters
 
 
 class Lexer(ILexer):
-    def __init__(self, token_provider: ITokenProvider, characters: IIterator):
+    def __init__(self, token_provider: ITokenProvider):
         self.token_provider = token_provider
+
+    def tokenize(self, characters: IIterator):
         self.characters = characters
         self.characters.advance()
-
-    def tokenize(self):
         # If the token is longer than a single character, we need to defined how to generate it.
         while self.characters.current() != None:
 
             if self.characters.current() in Characters.WHITESPACE.value:
                 self.characters.advance()
 
             elif self.characters.current() in Characters.LETTERS.value:
@@ -70,39 +57,22 @@
                 i += 3
             elif i + 1 < len(ops) and ops[i] in self.token_provider.doubles() and self.token_provider.double_match_exists(ops[i], ops[i+1]):
                 self.token_provider.new_double_operation_token(ops[i], ops[i+1])
                 i += 2
             else:
                 self.token_provider.new_single_operation_token(ops[i])
                 i += 1
-        
-
-
-    def _operationTest(self):
-        ops = []
-        while self.characters.current() != None and self.characters.current() in Characters.OPERATIONS.value:
-            ops.append(self.characters.current())
-            self.characters.advance()
-        if len(ops) == 1:
-            self.token_provider.new_single_operation_token(*ops)
-        elif len(ops) == 2:
-            self.token_provider.new_double_operation_token(*ops)
-        elif len(ops) == 3:
-            self.token_provider.new_tripple_operation_token(*ops)
-        else:
-            for i in ops:
-                self.token_provider.new_single_operation_token(i)
 
     def _object(self):
         obj = ''
         while self.characters.current() != None and self.characters.current() in Characters.OBJECTCHARACTERS.value:
-            if self.characters.current() in Characters.CHARACTERS.value and self.characters.peek() == '(':
+            if self.characters.current() in Characters.CHARACTERS.value and self.characters.peek(1, '') == '(':
                 obj += self.characters.current()
                 self.characters.advance()
-                self.token_provider.new_token(TokenType.FUNCTION, obj)
-            elif self.characters.peek() not in Characters.OBJECTCHARACTERS.value + '(':
+                self.token_provider.new_token(TokenType.FUNCTION, obj)               
+            elif self.characters.peek(1, '') not in Characters.OBJECTCHARACTERS.value + '(':
                 obj += self.characters.current()
                 self.characters.advance()
                 self.token_provider.new_token(TokenType.OBJECT, obj)
             else:
                 obj += self.characters.current()
-                self.characters.advance()
+                self.characters.advance()
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/core/nodes.py` & `jsonmathpy-2.0.7/jsonmathpy/core/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import List
-from jsonmathpy.interfaces.node_provider import INodeProvider
-from jsonmathpy.models.token import Token
-from jsonmathpy.core.types import NodeKeys, NodeType
-from jsonmathpy.models.node_keys import ConfigurationModels
+from jsonmathpy.shared.interfaces.node_provider import INodeProvider
+from jsonmathpy.shared.models.token import Token
+from jsonmathpy.shared.models.node_keys import ConfigurationModels
+from jsonmathpy.shared.constants import NodeKeys, NodeType
 
 class BaseNode:
 
     def __init__(self, node_type: NodeType):
         self.node_type = node_type
 
     def node(self, a, b, c):
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/core/parser.py` & `jsonmathpy-2.0.7/jsonmathpy/core/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-from jsonmathpy.interfaces.iterator import IIterator
-from jsonmathpy.interfaces.node_provider import INodeProvider
-from jsonmathpy.interfaces.parser import IParser
-from jsonmathpy.core.types import NodeType, TokenType
+from jsonmathpy.shared.interfaces.iterator import IIterator
+from jsonmathpy.shared.interfaces.node_provider import INodeProvider
+from jsonmathpy.shared.interfaces.parser import IParser
+from jsonmathpy.shared.constants import NodeType, TokenType
+from jsonmathpy.shared.models.token import Token
+
+
 
 class Parser(IParser):
 
-    def __init__(self, node_provider: INodeProvider, iterating_tokens: IIterator):
+    def __init__(self, node_provider: INodeProvider):
         """
         Constructor for Parser class.
 
         Args:
             tokens: a list of tokens representing the input expression to parse
         """
-        self.iterating_tokens = iterating_tokens
         self.node_provider = node_provider
-        self.iterating_tokens.advance()
 
     def raise_error(self, error_message):
         """
         Helper method to raise exceptions with a custom error message.
 
         Args:
             error_message: a string representing the error message to raise
         """
         raise Exception(error_message)
 
-    def parse(self):
+    def parse(self, iterating_tokens: IIterator):
         """
         Parse the input expression.
 
         Returns:
             The resulting expression tree if the input was valid, None otherwise.
         """
+        self.iterating_tokens = iterating_tokens
+        self.iterating_tokens.advance()
+
         if self.iterating_tokens.current() == None:
             return None
 
         elif len(self.iterating_tokens) >= 3:
             result = self.equation()
 
         elif len(self.iterating_tokens) < 3:
@@ -44,15 +48,15 @@
         elif self.iterating_tokens.current() != None:
             self.raise_error("Syntax Error")
 
         return result
 
     def equation(self):
         current_token = self.iterating_tokens.current()
-        next_token = self.iterating_tokens.peek()
+        next_token = self.iterating_tokens.peek(1, Token(TokenType.NONE, 'NONE'))
         if current_token.type == TokenType.OBJECT and next_token.type == TokenType.EQUAL:
             subject_variable = self.object()
             self.iterating_tokens.advance()
             return self.node_provider.new_node(NodeType.EQUALS, [subject_variable, self.statement()])
         else:
             return self.statement()
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/core/token.py` & `jsonmathpy-2.0.7/jsonmathpy/core/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from jsonmathpy.core.types import TokenType
-from jsonmathpy.interfaces.tokens import ITokenProvider
-from jsonmathpy.models.token import Token
+from jsonmathpy.shared.constants import TokenType
+from jsonmathpy.shared.interfaces.tokens import ITokenProvider
+from jsonmathpy.shared.models.token import Token
 
 
 class TokenProvider(ITokenProvider):
 
     def __init__(self):
         self.tokens = []
 
@@ -19,15 +19,14 @@
         if self.single_match_exists(c1):
             self.tokens.append(self.singles()[c1])
 
     def new_double_operation_token(self, c1, c2) -> None:
         if self.double_match_exists(c1, c2):
             self.tokens.append(self.doubles()[c1][c2])
 
-
     def new_tripple_operation_token(self, c1, c2, c3) -> None:
         if self.tripple_match_exists(c1, c2, c3):
             self.tokens.append(self.tripples()[c1][c2][c3])
 
     def singles(self):
         return {
             '*': Token(TokenType.STAR,          '*'),
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/core/types.py` & `jsonmathpy-2.0.7/jsonmathpy/shared/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     POSITIVE                = 'positive'                # Positive operator '+'
     AND                     = '&'                # Positive operator '+'
     OR                      = '|'                # Positive operator '+'
 
 
 class TokenType(Enum):
     """An enumeration of token types used by a the lexer to genrate tokens."""
+    NONE                    = 'NONE'
 
     # Single Charater Tokens
     PLUS                    = 'PLUS'                      
     MINUS                   = 'MINUS'                      
     STAR                    = 'STAR'                       
     SLASH                   = 'SLASH'                       
     EQUAL                   = 'EQUAL'                                    
@@ -108,18 +109,19 @@
     OBJECT                  = 'OBJECT'                  
     FLOAT                   = 'FLOAT'                   
     INTEGER                 = 'INTEGER'                
     FUNCTION                = 'FUNCTION'               
     ARRAY                   = 'ARRAY'           
 
 
-
 class Characters(Enum):
     """An object containing the set of supported characters, keyd on a set name."""
-    WHITESPACE         = ' \n\t'
-    DIGITS             = '0987654321'
-    LOWERCASES         = 'abcdefghijklmnopqrstuvwxyz'
-    UPPERCASES         = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-    CHARS              = UPPERCASES + LOWERCASES
-    CHARACTERS         = '{}_^=.:'
-    OBJECT_CHARACTERS  = CHARACTERS + UPPERCASES + LOWERCASES + DIGITS
+    WHITESPACE          = ' \n\t'
+    DIGITS              = '0987654321'
+    LOWERCASECHARACTERS = 'abcdefghijklmnopqrstuvwxyz'
+    UPPERCASECHARACTERS = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
+    NONLETTERCHARACTERS = '_{}:^;'
+    OPERATIONS          = '*-+=[](){}^/|&!~><:;.,@%'
+    LETTERS             = LOWERCASECHARACTERS + UPPERCASECHARACTERS
+    CHARACTERS          = LOWERCASECHARACTERS + UPPERCASECHARACTERS + NONLETTERCHARACTERS
+    OBJECTCHARACTERS    = LOWERCASECHARACTERS + UPPERCASECHARACTERS + NONLETTERCHARACTERS + DIGITS
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/interfaces/tokens.py` & `jsonmathpy-2.0.7/jsonmathpy/shared/interfaces/tokens.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.6/jsonmathpy/models/mapper.py` & `jsonmathpy-2.0.7/jsonmathpy/shared/models/mapper.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.6/jsonmathpy/models/node_keys.py` & `jsonmathpy-2.0.7/jsonmathpy/shared/models/node_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
-from typing import Any, Dict, List
-from jsonmathpy.models.basic_nodes import NodeConfigurationModel
-from jsonmathpy.models.node_handler import NodeHandler
-from jsonmathpy.models.object_configuration import ObjectConfigurationModel
+from typing import List
+from jsonmathpy.shared.models.basic_nodes import NodeConfigurationModel
+from jsonmathpy.shared.models.node_handler import NodeHandler
+from jsonmathpy.shared.models.object_configuration import ObjectConfigurationModel
 
 @dataclass
 class ConfigurationModels:
     node_configurations: List[NodeConfigurationModel]
     objs_configurations: List[ObjectConfigurationModel]
 
     def get_node_handlers(self) -> dict[str, NodeHandler]:
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/services/parser.py` & `jsonmathpy-2.0.7/jsonmathpy/parser/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from jsonmathpy.builders.parser_builder import ParserBuilder
+from jsonmathpy.parser.service_provider import ParserServicesProvider
 from jsonmathpy.core.iterator import Iterator
 from jsonmathpy.core.lexer import Lexer
 from jsonmathpy.core.parser import Parser
 from jsonmathpy.core.token import TokenProvider
 from jsonmathpy.core.nodes import NodeProvider
-from jsonmathpy.interfaces.parser_service import IParserService
-from jsonmathpy.models.node_keys import ConfigurationModels
+from jsonmathpy.shared.interfaces.parser_service import IParserService
+from jsonmathpy.shared.models.node_keys import ConfigurationModels
 
 class ParserService(IParserService):
     """
      Implements interface IParserService:
     """
     def __init__(self, node_configuration: ConfigurationModels):
         self.node_configuration = node_configuration
-        self.parser_builder = ParserBuilder(
-                                                        lexer               = Lexer, 
-                                                        parser              = Parser, 
-                                                        token_provider      = TokenProvider,
-                                                        node_provider       = NodeProvider,
-                                                        iterator            = Iterator,
-                                                        configuration_models= self.node_configuration
+        self.parser_serice = ParserServicesProvider(
+                                                        lexer                   = Lexer, 
+                                                        parser                  = Parser, 
+                                                        token_provider          = TokenProvider,
+                                                        node_provider           = NodeProvider,
+                                                        iterator                = Iterator,
+                                                        configuration_models    = self.node_configuration
                                                     )
 
-    def get_ast(self, string: str):
-        self.parser_instance = self.parser_builder.build(string)
-        return self.parser_instance.parse()
+    def parse_string(self, string: str):
+        return self.parser_serice.parse_string_service(string)
+
+    def tokenize_string(self, string: str):
+        return self.parser_serice.tokenize_string_service(string)
```

### Comparing `jsonmathpy-2.0.6/jsonmathpy/tests/tests_e2e.py` & `jsonmathpy-2.0.7/jsonmathpy/tests/tests_e2e.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.6/jsonmathpy/tests/tests_parser.py` & `jsonmathpy-2.0.7/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

