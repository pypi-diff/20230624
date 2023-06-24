# Comparing `tmp/khoj_assistant-0.6.3.dev90.tar.gz` & `tmp/khoj_assistant-0.6.3.dev92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jun 23 22:10:09 2023, max compression
+gzip compressed data, last modified: Sat Jun 24 07:49:57 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev90.tar` & `khoj_assistant-0.6.3.dev92.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3290 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0     9894 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     5981 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     4394 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6565 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    12744 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3410 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1828 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13101 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3866 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3070 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4158 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/LICENSE
--rw-r--r--   0        0        0    22944 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/README.md
--rw-r--r--   0        0        0     2801 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/pyproject.toml
--rw-r--r--   0        0        0    25306 2023-06-23 22:10:09.000000 khoj_assistant-0.6.3.dev90/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3290 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0     9894 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     5981 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     4419 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6647 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    12744 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3492 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1828 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13690 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     3883 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3070 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4158 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/LICENSE
+-rw-r--r--   0        0        0    22944 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/README.md
+-rw-r--r--   0        0        0     2801 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/pyproject.toml
+-rw-r--r--   0        0        0    25306 2023-06-24 07:49:57.000000 khoj_assistant-0.6.3.dev92/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev92/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/main.py` & `khoj_assistant-0.6.3.dev92/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/404.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/content_type_github_input.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 <div class="page">
     <div class="section">
         <h2 class="section-title">
             <img class="card-icon" src="/static/assets/icons/github.svg" alt="Github">
             <span class="card-title-text">Github</span>
         </h2>
         <form>
-            <div id="success" style="display: none;"></div>
             <table>
                 <tr>
                     <td>
                         <label for="pat-token">Personal Access Token</label>
                     </td>
                     <td>
                         <input type="text" id="pat-token" name="pat" value="{{ current_config['pat_token'] }}">
@@ -59,14 +58,15 @@
                     </td>
                     <td>
                         <input type="text" id="embeddings-file" name="embeddings-file" value="{{ current_config['embeddings_file'] }}">
                     </td>
                 </tr>
             </table>
             <div class="section">
+                <div id="success" style="display: none;"></div>
                 <button id="submit" type="submit">Save</button>
             </div>
         </form>
     </div>
 </div>
 <script>
     submit.addEventListener("click", function(event) {
@@ -92,15 +92,15 @@
                 "compressed_jsonl": compressed_jsonl,
                 "embeddings_file": embeddings_file,
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
-                document.getElementById("success").innerHTML = "✅ Successfully updated. Go to <a href='/config'>your settings</a> to regenerate your index.";
+                document.getElementById("success").innerHTML = "✅ Successfully updated. Click Configure on your <a href='/config'>settings page</a> to complete your Khoj setup.";
                 document.getElementById("success").style.display = "block";
             } else {
                 document.getElementById("success").innerHTML = "⚠️ Failed to update settings.";
                 document.getElementById("success").style.display = "block";
             }
         })
     });
```

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/content_type_input.html`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,18 @@
                         <label for="index-heading-entries">Index Heading Entries</label>
                     </td>
                     <td>
                         <input type="text" id="index-heading-entries" name="index-heading-entries" value="{{ current_config['index_heading_entries'] }}">
                     </td>
                 </tr>
             </table>
-            <div id="success" style="display: none;" ></div>
-            <button id="submit" type="submit">Save</button>
+            <div class="section">
+                <div id="success" style="display: none;" ></div>
+                <button id="submit" type="submit">Save</button>
+            </div>
         </form>
     </div>
 </div>
 <script>
     function addButtonEventListener(fieldName) {
         var button = document.getElementById(fieldName + "-button");
         button.addEventListener("click", function(event) {
@@ -141,15 +143,15 @@
                 "embeddings_file": embeddings_file,
                 "index_heading_entries": index_heading_entries
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
-                document.getElementById("success").innerHTML = "✅ Successfully updated. Go to <a href='/config'>your settings</a> to regenerate your index.";
+                document.getElementById("success").innerHTML = "✅ Successfully updated. Click Configure on your <a href='/config'>settings page</a> to complete your Khoj setup.";
                 document.getElementById("success").style.display = "block";
             } else {
                 document.getElementById("success").innerHTML = "⚠️ Failed to update settings.";
                 document.getElementById("success").style.display = "block";
             }
         })
     });
```

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/processor_conversation_input.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 <div class="page">
     <div class="section">
         <h2 class="section-title">
             <img class="card-icon" src="/static/assets/icons/chat.svg" alt="Chat">
             <span class="card-title-text">Chat</span>
         </h2>
         <form id="config-form">
-            <div id="success" style="display: none;" ></div>
             <table>
                 <tr>
                     <td>
                         <label for="openai-api-key">OpenAI API key</label>
                     </td>
                     <td>
                         <input type="text" id="openai-api-key" name="openai-api-key" value="{{ current_config['openai_api_key'] }}">
@@ -43,15 +42,18 @@
                         <label for="chat-model">Chat Model</label>
                     </td>
                     <td>
                         <input type="text" id="chat-model" name="chat-model" value="{{ current_config['chat_model'] }}">
                     </td>
                 </tr>
             </table>
-            <button id="submit" type="submit">Save</button>
+            <div class="section">
+                <div id="success" style="display: none;" ></div>
+                <button id="submit" type="submit">Save</button>
+            </div>
         </form>
     </div>
 </div>
 <script>
     submit.addEventListener("click", function(event) {
         event.preventDefault();
         var openai_api_key = document.getElementById("openai-api-key").value;
@@ -70,15 +72,15 @@
                 "model": model,
                 "chat_model": chat_model
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
-                document.getElementById("success").innerHTML = "✅ Successfully updated. Go to <a href='/config'>your settings</a> to regenerate your index.";
+                document.getElementById("success").innerHTML = "✅ Successfully updated. Click Configure on your <a href='/config'>settings page</a> to complete your Khoj setup.";
                 document.getElementById("success").style.display = "block";
             } else {
                 document.getElementById("success").innerHTML = "⚠️ Failed to update settings.";
                 document.getElementById("success").style.display = "block";
             }
         })
     });
```

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.6.3.dev92/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev92/src/khoj/routers/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # Internal Packages
 from khoj.configure import configure_processor, configure_search
 from khoj.processor.conversation.gpt import converse, extract_questions
 from khoj.processor.conversation.utils import message_to_log, message_to_prompt
 from khoj.search_type import image_search, text_search
 from khoj.utils.helpers import log_telemetry, timer
 from khoj.utils.rawconfig import (
+    ContentConfig,
     FullConfig,
+    ProcessorConfig,
+    SearchConfig,
     SearchResponse,
     TextContentConfig,
     ConversationProcessorConfig,
     GithubContentConfig,
 )
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
@@ -70,35 +73,44 @@
         yaml.dump(yaml.safe_load(state.config.json(by_alias=True)), outfile)
         outfile.close()
     return state.config
 
 
 @api.post("/config/data/content_type/github", status_code=200)
 async def set_content_config_github_data(updated_config: GithubContentConfig):
-    state.config.content_type.github = updated_config
+    if not state.config:
+        state.config = FullConfig()
+        state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+    state.config.content_type = ContentConfig(github=updated_config)
     try:
         save_config_to_file_updated_state()
         return {"status": "ok"}
     except Exception as e:
         return {"status": "error", "message": str(e)}
 
 
 @api.post("/config/data/content_type/{content_type}", status_code=200)
 async def set_content_config_data(content_type: str, updated_config: TextContentConfig):
-    state.config.content_type[content_type] = updated_config
+    if not state.config:
+        state.config = FullConfig()
+        state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+    state.config.content_type = ContentConfig(**{content_type: updated_config})
     try:
         save_config_to_file_updated_state()
         return {"status": "ok"}
     except Exception as e:
         return {"status": "error", "message": str(e)}
 
 
 @api.post("/config/data/processor/conversation", status_code=200)
 async def set_processor_conversation_config_data(updated_config: ConversationProcessorConfig):
-    state.config.processor.conversation = updated_config
+    if not state.config:
+        state.config = FullConfig()
+        state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+    state.config.processor = ProcessorConfig(conversation=updated_config)
     try:
         save_config_to_file_updated_state()
         return {"status": "ok"}
     except Exception as e:
         return {"status": "error", "message": str(e)}
```

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev92/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev92/src/khoj/routers/web_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     default_config = TextContentConfig(
         compressed_jsonl=default_github["compressed-jsonl"],
         embeddings_file=default_github["embeddings-file"],
     )
 
     current_config = (
-        state.config.content_type.github if state.config.content_type.github is not None else default_config
+        state.config.content_type.github if state.config and state.config.content_type.github else default_config
     )
 
     current_config = json.loads(current_config.json())
 
     return templates.TemplateResponse(
         "content_type_github_input.html", context={"request": request, "current_config": current_config}
     )
@@ -61,15 +61,15 @@
 
     default_config = TextContentConfig(
         compressed_jsonl=default_content_type["compressed-jsonl"],
         embeddings_file=default_content_type["embeddings-file"],
     )
     current_config = (
         state.config.content_type[content_type]
-        if state.config.content_type[content_type] is not None
+        if state.config and content_type in state.config.content_type
         else default_config
     )
     current_config = json.loads(current_config.json())
 
     return templates.TemplateResponse(
         "content_type_input.html",
         context={
@@ -89,15 +89,15 @@
         model=default_processor_config["model"],
         conversation_logfile=default_processor_config["conversation-logfile"],
         chat_model=default_processor_config["chat-model"],
     )
 
     current_processor_conversation_config = (
         state.config.processor.conversation
-        if state.config.processor.conversation is not None
+        if state.config and state.config.processor.conversation
         else default_processor_config
     )
     current_processor_conversation_config = json.loads(current_processor_conversation_config.json())
 
     return templates.TemplateResponse(
         "processor_conversation_input.html",
         context={
```

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev92/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev92/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev92/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev92/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev92/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev92/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/.gitignore` & `khoj_assistant-0.6.3.dev92/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/LICENSE` & `khoj_assistant-0.6.3.dev92/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/README.md` & `khoj_assistant-0.6.3.dev92/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/pyproject.toml` & `khoj_assistant-0.6.3.dev92/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev90/PKG-INFO` & `khoj_assistant-0.6.3.dev92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev90
+Version: 0.6.3.dev92
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

