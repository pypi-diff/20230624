# Comparing `tmp/aicodebot-0.4.0.tar.gz` & `tmp/aicodebot-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.4.0.tar", last modified: Thu Jun 22 18:02:37 2023, max compression
+gzip compressed data, was "aicodebot-0.4.1.tar", last modified: Sat Jun 24 21:38:04 2023, max compression
```

## Comparing `aicodebot-0.4.0.tar` & `aicodebot-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.891184 aicodebot-0.4.0/
--rw-r--r--   0 nick       (501) staff       (20)    34523 2023-06-22 18:00:57.000000 aicodebot-0.4.0/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     6655 2023-06-22 18:02:37.891071 aicodebot-0.4.0/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     6020 2023-06-22 18:00:57.000000 aicodebot-0.4.0/README.md
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.889372 aicodebot-0.4.0/aicodebot/
--rw-r--r--   0 nick       (501) staff       (20)       97 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/.aicodebot.template
--rw-r--r--   0 nick       (501) staff       (20)       18 2023-06-22 18:01:18.000000 aicodebot-0.4.0/aicodebot/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     7834 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/cli.py
--rw-r--r--   0 nick       (501) staff       (20)      366 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/helpers.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.890744 aicodebot-0.4.0/aicodebot/prompts/
--rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      838 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 nick       (501) staff       (20)     1018 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 nick       (501) staff       (20)      287 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/debug.yaml
--rw-r--r--   0 nick       (501) staff       (20)      212 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/fun_fact.yaml
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.890157 aicodebot-0.4.0/aicodebot.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     6655 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      511 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       48 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 nick       (501) staff       (20)       42 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)       10 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 nick       (501) staff       (20)     2789 2023-06-22 18:00:57.000000 aicodebot-0.4.0/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)       38 2023-06-22 18:02:37.891216 aicodebot-0.4.0/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     1526 2023-06-22 18:00:57.000000 aicodebot-0.4.0/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.890884 aicodebot-0.4.0/tests/
--rw-r--r--   0 nick       (501) staff       (20)      535 2023-06-22 18:00:57.000000 aicodebot-0.4.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.231264 aicodebot-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-24 21:37:41.000000 aicodebot-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-24 21:38:04.231264 aicodebot-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-24 21:37:41.000000 aicodebot-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.227265 aicodebot-0.4.1/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.231264 aicodebot-0.4.1/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/fun_fact.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.227265 aicodebot-0.4.1/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-24 21:37:41.000000 aicodebot-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:38:04.231264 aicodebot-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-24 21:37:41.000000 aicodebot-0.4.1/setup.py
```

### Comparing `aicodebot-0.4.0/LICENSE` & `aicodebot-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.4.0/aicodebot/cli.py` & `aicodebot-0.4.1/aicodebot/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,43 +71,50 @@
 
     # Set up the language model
     llm = OpenAI(temperature=1, max_tokens=DEFAULT_MAX_TOKENS)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
-    name = exec_and_get_output(["git", "config", "--get", "user.name"])
-
     with console.status("Thinking", spinner="point"):
-        response = chain.run(name)
+        response = chain.run({})
         console.print(response, style=bot_style)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--max-tokens", type=int, default=250)
 @click.option("-y", "--yes", is_flag=True, default=False, help="Don't ask for confirmation before committing.")
-def commit(verbose, max_tokens, yes):
+@click.option("--skip-pre-commit", is_flag=True, help="Skip running pre-commit (otherwise run it if it is found).")
+def commit(verbose, max_tokens, yes, skip_pre_commit):
     """Generate a git commit message and commit changes after you approve."""
     setup_environment()
 
+    # Check if pre-commit is installed and .pre-commit-config.yaml exists
+    if not skip_pre_commit and Path(".pre-commit-config.yaml").exists():
+        console.print("Running pre-commit checks...")
+        result = subprocess.run(["pre-commit", "run", "--all-files"])
+        if result.returncode != 0:
+            console.print("Pre-commit checks failed. Please fix the issues and try again.")
+            return
+
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "commit_message.yaml")
 
     # Set up the language model
     llm = OpenAI(temperature=0.1, max_tokens=max_tokens)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     # Get the changes from git
     staged_files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     base_git_diff = ["git", "diff", "-U10"]  # Tell diff to provide 10 lines of context
     if not staged_files:
-        # If no files are staged, stage all changed files
+        # If no files are staged, Assume they want to commit all changed files
         exec_and_get_output(["git", "add", "-A"])
         # Get the diff for all changes since the last commit
         diff = exec_and_get_output(base_git_diff + ["HEAD"])
         # Get the list of files to be committed
         files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     else:
         # If some files are staged, get the diff for those files
@@ -166,24 +173,25 @@
 
     # Print the output of the command
     output = f"Standard Output:\n{process.stdout}\nStandard Error:\n{process.stderr}"
     console.print(f"Output:\n{output}")
 
     # Print a message about the exit status
     if process.returncode == 0:
-        console.print("The command completed successfully.")
+        console.print("✅ The command completed successfully.")
     else:
         console.print(f"The command exited with status {process.returncode}.")
 
     # If the command failed, send its output to ChatGPT for analysis
     if process.returncode != 0:
         error_output = process.stderr
         with console.status("Thinking", spinner="point"):
             response = chat_chain.run(error_output)
             console.print(response, style=bot_style)
+        sys.exit(process.returncode)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 def fun_fact(verbose):
     """Tell me something interesting about programming or AI."""
     setup_environment()
```

### Comparing `aicodebot-0.4.0/aicodebot/prompts/alignment.yaml` & `aicodebot-0.4.1/aicodebot/prompts/alignment.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 _type: prompt
 template_format: f-string
-input_variables: ["name"]
+input_variables: []
 template: |
     You're an advocate for aligned AI.
     You don't subscribe to the idea that AI is a black box.
     You believe that AI should be explainable, transparent, and fair.
-    You're a champion for AI ethics and you're not afraid to speak up when you see something that's not right.
-    You love to teach about how we can bring empathy, heart, and ethics into AI.
-
-    The name of the person you are talking to is {name}
+    You're a champion for AI ethics and you're not afraid to speak up when
+    you see something that's not right.
+    You love to teach about how we can bring empathy and heart into AI.
 
     Give us an inspirational message for the healthy alignment of AI and humanity.
 
-    Be verbose, about 2-3 paragraphs, and give specifics for things software engineers can do to make AI more
-    aligned with humanity.
+    Be verbose, about 2-3 paragraphs, and give specifics for things software
+    engineers can do to make AI more aligned with humanity.
 
     Include some humor, but don't be too silly.
 
     Contextually appropriate emojis are encouraged, but not required.
```

### Comparing `aicodebot-0.4.0/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.4.1/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.4.0/pyproject.toml` & `aicodebot-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     "RET507",  # Allow for return values to be set after continue
     "RET508",  # Allow for return values to be set after break
     "S101",    # assert
     "S105",    # possible hardcoded password
     "S308",    # Trust us with mark_safe
     "S311",    # Trust us with random
     "S324",    # Trust us with hashlib
+    "S603",    # Trust us with subprocess
+    "S607",    # Trust us with subprocess with partial commands
     "SIM108",  # Don't force ternary operators
     "TRY003",  # long messages in exceptions are ok
 ]
 # https://beta.ruff.rs/docs/rules/#ruff-specific-rules-ruf
 line-length = 120
 select = [
     # Note, don't use isort through ruff, it's not as configurable as the standalone tool
```

### Comparing `aicodebot-0.4.0/setup.py` & `aicodebot-0.4.1/setup.py`

 * *Files identical despite different names*

