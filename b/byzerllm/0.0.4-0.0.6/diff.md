# Comparing `tmp/byzerllm-0.0.4.tar.gz` & `tmp/byzerllm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/byzerllm-0.0.4.tar", last modified: Mon May 15 02:54:46 2023, max compression
+gzip compressed data, was "byzerllm-0.0.6.tar", last modified: Sat Jun 24 13:14:13 2023, max compression
```

## Comparing `byzerllm-0.0.4.tar` & `byzerllm-0.0.6.tar`

### file list

```diff
@@ -1,214 +1,366 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      411 2023-05-15 02:54:46.000000 byzerllm-0.0.4/PKG-INFO
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/test/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4822 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test4.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1769 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test5.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      161 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      788 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test2.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2462 2023-05-12 13:14:31.000000 byzerllm-0.0.4/test/test6.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      541 2023-05-12 13:14:31.000000 byzerllm-0.0.4/test/test7.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      212 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test3.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-05-12 13:13:03.000000 byzerllm-0.0.4/setup.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-05-15 02:54:46.000000 byzerllm-0.0.4/setup.cfg
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/bark/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33373 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/generation.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     9139 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/model.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4243 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/api.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34444 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22660 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18660 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    49004 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33004 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23036 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35300 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26820 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32420 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    50548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    58492 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29540 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    37380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    43564 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21220 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    15516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    53908 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45324 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    44044 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    13436 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42924 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30604 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33860 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    38124 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29324 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    38500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    43084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21916 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35724 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42284 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    41268 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29004 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1943 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/readme.md
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16100 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45748 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21276 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42764 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24260 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33060 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    57852 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20100 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    46604 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45268 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    51668 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18980 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29164 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    52684 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16794 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/announcer.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    37964 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    44148 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34820 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20316 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24796 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    58652 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31724 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    59348 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30284 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5955 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/model_fine.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4110 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/bark_voice.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/moss/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/finetune_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/moss/models/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/configuration_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/quantization.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/custom_autotune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/modeling_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/tokenization_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    17212 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/moss_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-05-12 13:29:36.000000 byzerllm-0.0.4/src/byzerllm/version.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      699 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/utils/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2435 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/utils/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1065 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/utils/text_generator.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      689 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/utils/emb.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/apps/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/apps/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6201 2023-05-15 02:54:13.000000 byzerllm-0.0.4/src/byzerllm/apps/qa.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/config.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      277 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6263 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/other.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16907 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/common.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11082 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1404 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/infer.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3000 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/finetune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/trainer_seq2seq.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/arguments.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/finetune.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/dolly/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/generate.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/consts.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/dolly_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/trainer.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/whisper/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/whisper/whisper_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/whisper/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      411 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8787 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/top_level.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/dependency_links.txt
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.919614 byzerllm-0.0.6/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      314 2023-06-24 13:14:13.919614 byzerllm-0.0.6/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       38 2023-06-24 13:14:13.919614 byzerllm-0.0.6/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-15 03:02:58.000000 byzerllm-0.0.6/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.223565 byzerllm-0.0.6/src/
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.243566 byzerllm-0.0.6/src/byzerllm/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2143 2023-06-24 03:47:49.000000 byzerllm-0.0.6/src/byzerllm/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.299570 byzerllm-0.0.6/src/byzerllm/apps/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      412 2023-06-02 10:27:10.000000 byzerllm-0.0.6/src/byzerllm/apps/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3831 2023-06-15 05:04:13.000000 byzerllm-0.0.6/src/byzerllm/apps/builder.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3045 2023-06-14 04:44:01.000000 byzerllm-0.0.6/src/byzerllm/apps/client.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6389 2023-06-17 12:31:47.000000 byzerllm-0.0.6/src/byzerllm/apps/qa.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1562 2023-06-04 05:15:41.000000 byzerllm-0.0.6/src/byzerllm/apps/vector_db.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.319572 byzerllm-0.0.6/src/byzerllm/baichuan/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2437 2023-06-23 11:59:29.000000 byzerllm-0.0.6/src/byzerllm/baichuan/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.359575 byzerllm-0.0.6/src/byzerllm/bark/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-05-11 02:06:23.000000 byzerllm-0.0.6/src/byzerllm/bark/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4243 2023-05-11 02:06:23.000000 byzerllm-0.0.6/src/byzerllm/bark/api.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.223565 byzerllm-0.0.6/src/byzerllm/bark/assets/
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.427579 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16794 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/announcer.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20316 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31724 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    59348 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33860 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38124 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21220 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15516 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13436 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18980 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34820 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18660 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22660 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30604 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29324 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31460 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44044 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43564 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    53908 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33060 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23036 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26820 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33004 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    46604 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45268 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52684 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42764 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34180 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41268 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44148 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24796 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37964 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50548 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29540 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29004 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30500 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21916 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43084 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42284 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42548 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45324 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32420 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58492 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35300 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49004 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34444 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30284 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58652 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1943 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/readme.md
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    57852 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24260 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51668 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29164 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45748 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42924 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38500 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21276 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35724 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.483583 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39620 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27460 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30660 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34980 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25540 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23300 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45804 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52204 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50764 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49908 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45108 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    55932 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32524 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43244 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25860 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27780 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29804 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51404 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39404 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33804 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30444 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29644 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43724 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42708 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37644 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26716 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25060 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26556 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26340 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19196 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39564 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23140 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27884 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23676 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41428 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38180 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38820 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30980 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27724 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34500 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36844 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26980 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28260 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39884 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44628 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20476 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39084 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22076 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33164 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17220 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25276 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20636 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19836 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17436 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16900 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19300 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16156 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4110 2023-05-11 04:09:04.000000 byzerllm-0.0.6/src/byzerllm/bark/bark_voice.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33373 2023-05-11 02:06:23.000000 byzerllm-0.0.6/src/byzerllm/bark/generation.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     9139 2023-05-11 02:06:23.000000 byzerllm-0.0.6/src/byzerllm/bark/model.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5955 2023-05-11 02:06:23.000000 byzerllm-0.0.6/src/byzerllm/bark/model_fine.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.499585 byzerllm-0.0.6/src/byzerllm/chatglm6b/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-04 03:55:05.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8182 2023-04-04 03:55:05.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/arguments.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21286 2023-05-04 08:53:10.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/finetune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11575 2023-04-04 03:55:05.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/trainer_seq2seq.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.519586 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3000 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/finetune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1404 2023-05-12 05:48:30.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/infer.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.567589 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      277 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16907 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/common.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7620 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/config.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6263 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/other.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11082 2023-05-06 13:50:22.000000 byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.595591 byzerllm-0.0.6/src/byzerllm/dolly/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-25 12:20:22.000000 byzerllm-0.0.6/src/byzerllm/dolly/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-04-25 12:20:22.000000 byzerllm-0.0.6/src/byzerllm/dolly/consts.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1112 2023-04-25 12:45:20.000000 byzerllm-0.0.6/src/byzerllm/dolly/dolly_inference.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10065 2023-04-25 12:44:37.000000 byzerllm-0.0.6/src/byzerllm/dolly/generate.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12156 2023-04-25 12:27:32.000000 byzerllm-0.0.6/src/byzerllm/dolly/trainer.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.599592 byzerllm-0.0.6/src/byzerllm/falcon/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1471 2023-06-22 09:35:02.000000 byzerllm-0.0.6/src/byzerllm/falcon/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.611592 byzerllm-0.0.6/src/byzerllm/llama/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1469 2023-06-08 12:19:01.000000 byzerllm-0.0.6/src/byzerllm/llama/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.623593 byzerllm-0.0.6/src/byzerllm/m3e/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      164 2023-06-14 04:24:41.000000 byzerllm-0.0.6/src/byzerllm/m3e/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.647595 byzerllm-0.0.6/src/byzerllm/moss/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-22 10:54:48.000000 byzerllm-0.0.6/src/byzerllm/moss/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12657 2023-04-23 13:04:50.000000 byzerllm-0.0.6/src/byzerllm/moss/finetune_moss.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.703599 byzerllm-0.0.6/src/byzerllm/moss/models/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-22 10:54:54.000000 byzerllm-0.0.6/src/byzerllm/moss/models/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5097 2023-05-19 09:07:29.000000 byzerllm-0.0.6/src/byzerllm/moss/models/configuration_moss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6735 2023-04-23 12:11:45.000000 byzerllm-0.0.6/src/byzerllm/moss/models/custom_autotune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31351 2023-04-23 12:11:45.000000 byzerllm-0.0.6/src/byzerllm/moss/models/modeling_moss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18866 2023-04-23 12:11:45.000000 byzerllm-0.0.6/src/byzerllm/moss/models/quantization.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15952 2023-04-23 12:11:45.000000 byzerllm-0.0.6/src/byzerllm/moss/models/tokenization_moss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16910 2023-06-05 14:40:24.000000 byzerllm-0.0.6/src/byzerllm/moss/moss_inference.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.703599 byzerllm-0.0.6/src/byzerllm/saas/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-02 02:17:52.000000 byzerllm-0.0.6/src/byzerllm/saas/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.703599 byzerllm-0.0.6/src/byzerllm/saas/chatglm/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2005 2023-06-10 15:08:00.000000 byzerllm-0.0.6/src/byzerllm/saas/chatglm/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.723600 byzerllm-0.0.6/src/byzerllm/saas/sparkdesk/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5014 2023-06-10 15:24:52.000000 byzerllm-0.0.6/src/byzerllm/saas/sparkdesk/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1632 2023-06-24 13:03:15.000000 byzerllm-0.0.6/src/byzerllm/store.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.791605 byzerllm-0.0.6/src/byzerllm/utils/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      143 2023-06-23 08:11:39.000000 byzerllm-0.0.6/src/byzerllm/utils/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3856 2023-06-14 04:24:33.000000 byzerllm-0.0.6/src/byzerllm/utils/emb.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.815607 byzerllm-0.0.6/src/byzerllm/utils/fulltune/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3723 2023-06-22 06:28:25.000000 byzerllm-0.0.6/src/byzerllm/utils/fulltune/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.895613 byzerllm-0.0.6/src/byzerllm/utils/sft/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7639 2023-06-23 14:15:53.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1199 2023-06-21 10:59:26.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/argument.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2019 2023-06-21 10:59:27.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/collator.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2156 2023-06-21 11:05:15.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/dataset.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1614 2023-06-21 10:59:29.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/loss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2620 2023-06-21 10:59:30.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/model.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6746 2023-06-23 02:23:30.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/qlora.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3395 2023-06-21 10:59:30.000000 byzerllm-0.0.6/src/byzerllm/utils/sft/trainer.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3102 2023-06-16 12:42:38.000000 byzerllm-0.0.6/src/byzerllm/utils/text_generator.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       22 2023-06-24 13:07:48.000000 byzerllm-0.0.6/src/byzerllm/version.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.907614 byzerllm-0.0.6/src/byzerllm/whisper/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-11 01:44:23.000000 byzerllm-0.0.6/src/byzerllm/whisper/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-11 07:07:58.000000 byzerllm-0.0.6/src/byzerllm/whisper/whisper_inference.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:14:13.243566 byzerllm-0.0.6/src/byzerllm.egg-info/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      314 2023-06-24 13:14:13.000000 byzerllm-0.0.6/src/byzerllm.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16232 2023-06-24 13:14:13.000000 byzerllm-0.0.6/src/byzerllm.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-06-24 13:14:13.000000 byzerllm-0.0.6/src/byzerllm.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        9 2023-06-24 13:14:13.000000 byzerllm-0.0.6/src/byzerllm.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `byzerllm-0.0.4/setup.py` & `byzerllm-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/generation.py` & `byzerllm-0.0.6/src/byzerllm/bark/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/model.py` & `byzerllm-0.0.6/src/byzerllm/bark/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/api.py` & `byzerllm-0.0.6/src/byzerllm/bark/api.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/readme.md` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/readme.md`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/announcer.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/announcer.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_5.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_4.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_7.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_6.npz` & `byzerllm-0.0.6/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/model_fine.py` & `byzerllm-0.0.6/src/byzerllm/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/bark/bark_voice.py` & `byzerllm-0.0.6/src/byzerllm/bark/bark_voice.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/finetune_moss.py` & `byzerllm-0.0.6/src/byzerllm/moss/finetune_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/models/configuration_moss.py` & `byzerllm-0.0.6/src/byzerllm/moss/models/configuration_moss.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         "num_attention_heads": "n_head",
         "num_hidden_layers": "n_layer",
     }
 
     def __init__(
         self,
         vocab_size=107008,
-        n_positions=2048,
+        n_positions=8096,
         n_ctx=2048,
         n_embd=4096,
         n_layer=28,
         n_head=16,
         rotary_dim=64,
         n_inner=None,
         activation_function="gelu_new",
```

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/models/quantization.py` & `byzerllm-0.0.6/src/byzerllm/moss/models/quantization.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/models/custom_autotune.py` & `byzerllm-0.0.6/src/byzerllm/moss/models/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/models/modeling_moss.py` & `byzerllm-0.0.6/src/byzerllm/moss/models/modeling_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/models/tokenization_moss.py` & `byzerllm-0.0.6/src/byzerllm/moss/models/tokenization_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/moss/moss_inference.py` & `byzerllm-0.0.6/src/byzerllm/moss/moss_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     print(f"Restore model done.")
 
 
 class Inference:
     def __init__(
         self,
         model: Optional[MossForCausalLM] = None,
+        tokenizer: Optional[MossTokenizer] = None,
         model_dir: Optional[str] = None,
         parallelism: bool = True,
         device_map: Optional[Union[str, List[int]]] = None,
     ) -> None:
         """
         Initializes the MossModel with a given model or loads a model from the specified directory.
 
@@ -71,16 +72,19 @@
             self.model = model
         else:
             self.model = (
                 self.Init_Model_Parallelism(raw_model_dir=self.model_dir, device_map=device_map)
                 if parallelism
                 else MossForCausalLM.from_pretrained(self.model_dir).to("cuda")
             )
-
-        self.tokenizer = MossTokenizer.from_pretrained(self.model_dir)
+  
+        if tokenizer:
+            self.tokenizer = tokenizer
+        else:
+            self.tokenizer = MossTokenizer.from_pretrained(self.model_dir)
 
         self.prefix = PREFIX
         self.default_paras = DEFAULT_PARAS
         self.num_layers, self.heads, self.hidden, self.vocab_size = 34, 24, 256, 107008
         
         self.moss_startwords = torch.LongTensor([27, 91, 44, 18420, 91, 31175])
         self.tool_startwords = torch.LongTensor([27, 91, 6935, 1746, 91, 31175])
@@ -335,52 +339,45 @@
 
         Returns:
             Tuple[torch.Tensor, Tuple[torch.Tensor]]: A tuple containing the logits and past key values.
         """
         inputs = {
             "input_ids": input_ids,
             "attention_mask": attention_mask,
-            "past_key_values": past_key_values,
+            "past_key_values": past_key_values            
         }
         with torch.no_grad():
             outputs: BaseModelOutputWithPast = self.model(**inputs)
 
-        return outputs.logits, outputs.past_key_values
+        return outputs.logits, outputs.past_key_values    
 
     def __call__(self, input):
         return self.forward(input)
     
 
-if __name__ == "__main__":
-    import os
-    try:
-        import sys
-        import logging
-        import transformers
-        import datasets
-        logging.basicConfig(
-        format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
-        datefmt="%m/%d/%Y %H:%M:%S",
-        handlers=[logging.StreamHandler(sys.stdout)],)            
-        transformers.utils.logging.set_verbosity_info()            
-        datasets.utils.logging.set_verbosity_info()
-        transformers.utils.logging.enable_default_handler()
-        transformers.utils.logging.enable_explicit_format() 
-    except ImportError:
-        pass 
-    os.environ["CUDA_VISIBLE_DEVICES"] = "0"
-    
-    # Create an Inference instance with the specified model directory.
-    # infer = Inference(model_dir="/home/winubuntu/projects/moss-model/moss-moon-003-sft-plugin-int4",parallelism=False, device_map="auto")
-
-    # If you need to load a quantized model, please instead load the model and then pass it into Inference.__init__.
-    model = MossForCausalLM.from_pretrained("/home/winubuntu/projects/moss-model/moss-moon-003-sft-plugin-int4").half().cuda()
-    infer = Inference(model, device_map="auto")
-
-    # Define a test case string.
-    test_case = "<|Human|>: Hello MOSS<eoh>\n<|MOSS|>:"
-
-    # Generate a response using the Inference instance.
-    res = infer(test_case)
+def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
+        max_length:int=4096, 
+        top_p:float=0.95,
+        temperature:float=0.1):
+    infer = Inference(self,tokenizer)
+    reponses = infer.forward(f'<|Human|>: {ins} <eoh>',{ 
+                "temperature":temperature,
+                "top_k":0,
+                "top_p":top_p, 
+                "length_penalty":1, 
+                "max_time":60, 
+                "repetition_penalty":1.02, 
+                "max_iterations":512, 
+                "regulation_start":512,
+                "prefix_length":len(PREFIX),
+                "max_length":max_length
+                })
+    return [(res,"") for res in reponses]
+
+
+def init_model(model_dir):
+    model = MossForCausalLM.from_pretrained(model_dir).half().cuda()
+    tokenizer = MossTokenizer.from_pretrained(model_dir)
+    import types
+    model.stream_chat = types.MethodType(stream_chat, model)
+    return (model,tokenizer)
 
-    # Print the generated response.
-    print(res)
```

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/config.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/other.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/other.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/common.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/common.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/infer.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/infer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/finetune.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/tunning/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.0.6/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/dolly/generate.py` & `byzerllm-0.0.6/src/byzerllm/dolly/generate.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/dolly/consts.py` & `byzerllm-0.0.6/src/byzerllm/dolly/consts.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/dolly/dolly_inference.py` & `byzerllm-0.0.6/src/byzerllm/dolly/dolly_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/dolly/trainer.py` & `byzerllm-0.0.6/src/byzerllm/dolly/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.4/src/byzerllm/whisper/whisper_inference.py` & `byzerllm-0.0.6/src/byzerllm/whisper/whisper_inference.py`

 * *Files identical despite different names*

