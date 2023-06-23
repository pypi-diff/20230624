# Comparing `tmp/reliableGPT-0.2.902.tar.gz` & `tmp/reliableGPT-0.2.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.902.tar", last modified: Fri Jun 23 21:45:47 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.903.tar", last modified: Fri Jun 23 22:46:25 2023, max compression
```

## Comparing `reliableGPT-0.2.902.tar` & `reliableGPT-0.2.903.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 21:45:47.729723 reliableGPT-0.2.902/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.902/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 21:45:47.729633 reliableGPT-0.2.902/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.902/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 21:45:47.729306 reliableGPT-0.2.902/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      244 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 21:45:47.729506 reliableGPT-0.2.902/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.902/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9592 2023-06-23 21:44:38.000000 reliableGPT-0.2.902/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 21:45:47.729756 reliableGPT-0.2.902/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-23 21:44:49.000000 reliableGPT-0.2.902/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 22:46:25.539567 reliableGPT-0.2.903/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.903/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 22:46:25.539477 reliableGPT-0.2.903/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.903/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 22:46:25.538647 reliableGPT-0.2.903/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      270 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 22:46:25.539209 reliableGPT-0.2.903/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.903/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9951 2023-06-23 22:32:41.000000 reliableGPT-0.2.903/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7603 2023-06-23 22:41:56.000000 reliableGPT-0.2.903/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 22:46:25.539598 reliableGPT-0.2.903/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-23 22:46:07.000000 reliableGPT-0.2.903/setup.py
```

### Comparing `reliableGPT-0.2.902/LICENSE` & `reliableGPT-0.2.903/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.902/README.md` & `reliableGPT-0.2.903/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.902/reliablegpt/main.py` & `reliableGPT-0.2.903/reliablegpt/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,34 +24,35 @@
                         subject="reliableGPT: Unhandled Error",
                         html=body)
 
 def make_LLM_request(new_kwargs, self):
     try:
         if "embedding" in str(self.openai_create_function):
             # retry embedding with diff key
+            print(colored(f"ReliableGPT: Retrying Embedding request", "blue"))
             return openai.Embedding.create(**new_kwargs)
         model = new_kwargs['model']
         if "3.5" or "4" in model: # call ChatCompletion
             print(colored(f"ReliableGPT: Retrying request with model CHAT {model}", "blue"))
             return openai.ChatCompletion.create(**new_kwargs)
         else:
             print(colored(f"ReliableGPT: Retrying request with model TEXT {model}", "blue"))
             new_kwargs['prompt'] = " ".join([message["content"] for message in new_kwargs['messages']])
             new_kwargs.pop('messages', None) # remove messages for completion models 
             return openai.Completion.create(**new_kwargs)
     except Exception as e:
         print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
         raise ValueError(e)
 
-def fallback_request(args, kwargs, fallback_strategy):
+def fallback_request(args, kwargs, fallback_strategy, self):
     result = None
     for model in fallback_strategy:
         new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
         new_kwargs['model'] = model  # Update the model
-        result = make_LLM_request(new_kwargs)
+        result = make_LLM_request(new_kwargs, self=self)
         if result != None:
             return result    
     return None
 
 def api_key_handler(args, kwargs, fallback_strategy, user_email, user_token, self=""):
     try:
         url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
@@ -82,23 +83,26 @@
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
     # 4. APIConnectionError - Check your network settings, proxy configuration, SSL certificates, or firewall rules.
     # 5. InvalidRequestError - User input was bad: context_length_exceeded, 
     # 6. AuthenticationError - API key not working, return default hardcoded message
     # 7. ServiceUnavailableError - retry, retry with fallback
+    if openAI_error != None:
+        openAI_error = openAI_error.error # index into the error attribute of the class
+    
     error_type = None # defalt to being None
     if openAI_error != None and 'type' in openAI_error:
         error_type = openAI_error['type']
     if error_type == 'invalid_request_error' or error_type == 'InvalidRequestError':
         # check if this is context window related, try with a 16k model
         if openAI_error.code == 'context_length_exceeded':
             print(colored("ReliableGPT: invalid request error - context_length_exceeded", "red"))
             fallback_strategy = ['gpt-3.5-turbo-16k'] + fallback_strategy
-            result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
+            result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, self=self)
             if result == None:
                 return graceful_string
             else:
                 return result
         if openAI_error.code == "invalid_api_key":
             print(colored("ReliableGPT: invalid request error - invalid_api_key", "red"))
             result = api_key_handler(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, user_email=user_email, user_token=user_token, self=self)
@@ -109,22 +113,23 @@
 
     # todo: alert on user_email that there is now an auth error 
     elif error_type == 'authentication_error' or error_type == 'AuthenticationError':
         print(colored("ReliableGPT: Auth error", "red"))
         return graceful_string
 
     # catch all 
-    result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
+    result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, self=self)
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
 def capture_relevant_info(self, args, kwargs, result=None):
+    #print(f"In capture relevant info {kwargs['metadata']}")
     return
 
 
 class reliableGPT:
     def __init__(
             self, 
             openai_create_function, 
@@ -143,45 +148,46 @@
 
         if self.user_email == "":
             raise ValueError("ReliableGPT Error: Please pass in a user email")
 
     def __call__(self, *args, **kwargs):
         start_time = time.time()
         try:
+            print("in call for normal case")
             capture_relevant_info(self, args, kwargs)
             posthog.capture(self.user_email, 'reliableGPT.request')
             result = self.openai_create_function(*args, **kwargs)
             capture_relevant_info(self, args, kwargs, result)
 
             return result
         except Exception as e:
             result = self.graceful_string # default to graceful string
             try:
                 print(colored(f"ReliableGPT: Error Response from {self.openai_create_function}", 'red'))
                 print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
                 result = handle_openAI_error(
                     args = args,
                     kwargs = kwargs,
-                    openAI_error = e.error,
+                    openAI_error = e,
                     fallback_strategy = self.fallback_strategy,
                     graceful_string = self.graceful_string,
                     user_email = self.user_email,
                     user_token=self.user_token,
                     self=self
                 )
                 print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
                 if result == self.graceful_string:
                     send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Normal Retry"}, self.send_notification)
-                    posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e, 'recovered_response': result})
+                    posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':str(e), 'recovered_response': result})
                     capture_relevant_info(self, args, kwargs, result)
                 else:
-                    posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e, 'recovered_response': result})
+                    posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':str(e), 'recovered_response': result})
                     capture_relevant_info(self, args, kwargs, result)
             except Exception as e2:
-                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error': e, 'error2':e2, 'recovered_response': self.graceful_string})
+                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error':str(e), 'error2':str(e2), 'recovered_response': self.graceful_string})
                 send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
                 capture_relevant_info(self, args, kwargs, result)
                 return result
 
 
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
```

