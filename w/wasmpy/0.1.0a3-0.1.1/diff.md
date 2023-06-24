# Comparing `tmp/wasmpy-0.1.0a3.tar.gz` & `tmp/wasmpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wasmpy-0.1.0a3.tar", last modified: Mon Dec 14 17:36:31 2020, max compression
+gzip compressed data, was "wasmpy-0.1.1.tar", last modified: Sat Jun 24 19:03:53 2023, max compression
```

## Comparing `wasmpy-0.1.0a3.tar` & `wasmpy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,158 @@
-drwxrwxrwx   0        0        0        0 2020-12-14 17:36:31.141759 wasmpy-0.1.0a3/
--rw-rw-rw-   0        0        0     1944 2020-12-14 17:36:31.139746 wasmpy-0.1.0a3/PKG-INFO
--rw-rw-rw-   0        0        0      867 2020-11-05 18:16:47.000000 wasmpy-0.1.0a3/README.md
--rw-rw-rw-   0        0        0       42 2020-12-14 17:36:31.142740 wasmpy-0.1.0a3/setup.cfg
--rw-rw-rw-   0        0        0      915 2020-12-14 17:35:25.000000 wasmpy-0.1.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-14 17:36:31.099748 wasmpy-0.1.0a3/wasmpy/
--rw-rw-rw-   0        0        0      107 2020-11-04 21:55:34.000000 wasmpy-0.1.0a3/wasmpy/__init__.py
--rw-rw-rw-   0        0        0     1380 2020-12-13 19:02:16.000000 wasmpy-0.1.0a3/wasmpy/hooks.py
--rw-rw-rw-   0        0        0    13675 2020-12-14 17:27:49.000000 wasmpy-0.1.0a3/wasmpy/instructions.py
--rw-rw-rw-   0        0        0     2239 2020-10-30 18:29:36.000000 wasmpy-0.1.0a3/wasmpy/module.py
--rw-rw-rw-   0        0        0     5316 2020-12-14 17:27:49.000000 wasmpy-0.1.0a3/wasmpy/sections.py
--rw-rw-rw-   0        0        0     2440 2020-12-14 16:55:31.000000 wasmpy-0.1.0a3/wasmpy/types.py
--rw-rw-rw-   0        0        0     2105 2020-12-14 17:27:49.000000 wasmpy-0.1.0a3/wasmpy/values.py
-drwxrwxrwx   0        0        0        0 2020-12-14 17:36:31.136754 wasmpy-0.1.0a3/wasmpy.egg-info/
--rw-rw-rw-   0        0        0     1944 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.903138 wasmpy-0.1.1/
+-rw-rw-rw-   0        0        0     1068 2023-06-15 12:12:24.000000 wasmpy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-06-24 18:22:33.000000 wasmpy-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2445 2023-06-24 19:03:53.903138 wasmpy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1568 2023-06-24 18:50:52.000000 wasmpy-0.1.1/README.md
+-rw-rw-rw-   0        0        0     4922 2023-06-24 09:33:46.000000 wasmpy-0.1.1/opcodes.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:03:53.906562 wasmpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     5270 2023-06-24 19:03:26.000000 wasmpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.761533 wasmpy-0.1.1/wasmpy/
+-rw-rw-rw-   0        0        0      106 2023-06-23 12:23:39.000000 wasmpy-0.1.1/wasmpy/__init__.py
+-rw-rw-rw-   0        0        0     1689 2023-06-23 11:11:55.000000 wasmpy-0.1.1/wasmpy/hooks.py
+-rw-rw-rw-   0        0        0    14893 2023-06-24 07:42:57.000000 wasmpy-0.1.1/wasmpy/instructions.py
+-rw-rw-rw-   0        0        0     3097 2023-06-23 11:13:55.000000 wasmpy-0.1.1/wasmpy/module.py
+-rw-rw-rw-   0        0        0     1085 2023-06-22 15:47:07.000000 wasmpy-0.1.1/wasmpy/native.py
+-rw-rw-rw-   0        0        0     5286 2023-06-23 11:12:14.000000 wasmpy-0.1.1/wasmpy/sections.py
+-rw-rw-rw-   0        0        0     2421 2023-06-21 19:25:53.000000 wasmpy-0.1.1/wasmpy/types.py
+-rw-rw-rw-   0        0        0     2029 2023-06-23 11:12:52.000000 wasmpy-0.1.1/wasmpy/values.py
+-rw-rw-rw-   0        0        0     8283 2023-06-24 08:07:05.000000 wasmpy-0.1.1/wasmpy/win_x86.cpp
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.773825 wasmpy-0.1.1/wasmpy/x86/
+-rw-rw-rw-   0        0        0      217 2023-06-24 06:23:55.000000 wasmpy-0.1.1/wasmpy/x86/helpers.cpp
+-rw-rw-rw-   0        0        0      128 2023-06-24 07:49:47.000000 wasmpy-0.1.1/wasmpy/x86/helpers.h
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.893447 wasmpy-0.1.1/wasmpy/x86/instructions/
+-rw-rw-rw-   0        0        0       16 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/drop
+-rw-rw-rw-   0        0        0       76 2023-06-24 05:34:10.000000 wasmpy-0.1.1/wasmpy/x86/instructions/drop.asm
+-rw-rw-rw-   0        0        0       15 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.const
+-rw-rw-rw-   0        0        0       74 2023-06-24 09:25:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.const.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.eq
+-rw-rw-rw-   0        0        0      182 2023-06-24 06:48:21.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.eq.asm
+-rw-rw-rw-   0        0        0       27 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f64.const
+-rw-rw-rw-   0        0        0      124 2023-06-24 09:31:58.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f64.const.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.add
+-rw-rw-rw-   0        0        0      143 2023-06-24 05:51:43.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.add.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.and
+-rw-rw-rw-   0        0        0      143 2023-06-24 05:54:00.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.and.asm
+-rw-rw-rw-   0        0        0       37 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.clz
+-rw-rw-rw-   0        0        0      178 2023-06-24 05:50:35.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.clz.asm
+-rw-rw-rw-   0        0        0       15 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.const
+-rw-rw-rw-   0        0        0       74 2023-06-24 09:25:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.const.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ctz
+-rw-rw-rw-   0        0        0      154 2023-06-24 05:50:56.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ctz.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_s
+-rw-rw-rw-   0        0        0      177 2023-06-24 05:52:39.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_s.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_u
+-rw-rw-rw-   0        0        0      176 2023-06-24 05:52:55.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_u.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eq
+-rw-rw-rw-   0        0        0      182 2023-06-24 05:38:00.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eq.asm
+-rw-rw-rw-   0        0        0       28 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eqz
+-rw-rw-rw-   0        0        0      143 2023-06-24 05:37:40.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eqz.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_s
+-rw-rw-rw-   0        0        0      183 2023-06-24 05:40:32.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_s.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_u
+-rw-rw-rw-   0        0        0      183 2023-06-24 05:40:50.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_u.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_s
+-rw-rw-rw-   0        0        0      182 2023-06-24 05:39:22.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_s.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_u
+-rw-rw-rw-   0        0        0      182 2023-06-24 05:39:41.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_u.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_s
+-rw-rw-rw-   0        0        0      183 2023-06-24 05:39:57.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_s.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_u
+-rw-rw-rw-   0        0        0      183 2023-06-24 05:40:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_u.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_s
+-rw-rw-rw-   0        0        0      182 2023-06-24 05:38:36.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_s.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_u
+-rw-rw-rw-   0        0        0      182 2023-06-24 05:39:02.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_u.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.mul
+-rw-rw-rw-   0        0        0      144 2023-06-24 05:52:17.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.mul.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ne
+-rw-rw-rw-   0        0        0      184 2023-06-24 05:38:20.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ne.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.or
+-rw-rw-rw-   0        0        0      142 2023-06-24 05:54:14.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.or.asm
+-rw-rw-rw-   0        0        0       21 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.popcnt
+-rw-rw-rw-   0        0        0      100 2023-06-24 05:51:20.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.popcnt.asm
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_s
+-rw-rw-rw-   0        0        0      191 2023-06-24 05:53:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_s.asm
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_u
+-rw-rw-rw-   0        0        0      190 2023-06-24 05:53:43.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_u.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotl
+-rw-rw-rw-   0        0        0      142 2023-06-24 05:55:49.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotl.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotr
+-rw-rw-rw-   0        0        0      142 2023-06-24 05:56:08.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotr.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shl
+-rw-rw-rw-   0        0        0      162 2023-06-24 05:54:48.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shl.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_s
+-rw-rw-rw-   0        0        0      162 2023-06-24 05:55:11.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_s.asm
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_u
+-rw-rw-rw-   0        0        0      162 2023-06-24 05:55:32.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_u.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.sub
+-rw-rw-rw-   0        0        0      143 2023-06-24 05:52:01.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.sub.asm
+-rw-rw-rw-   0        0        0        9 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.wrap_i64
+-rw-rw-rw-   0        0        0       48 2023-06-24 06:35:32.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.wrap_i64.asm
+-rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.xor
+-rw-rw-rw-   0        0        0      143 2023-06-24 05:54:30.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.xor.asm
+-rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.add
+-rw-rw-rw-   0        0        0      246 2023-06-24 06:33:44.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.add.asm
+-rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.and
+-rw-rw-rw-   0        0        0      246 2023-06-24 06:34:24.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.and.asm
+-rw-rw-rw-   0        0        0       69 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.clz
+-rw-rw-rw-   0        0        0      331 2023-06-24 06:32:38.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.clz.asm
+-rw-rw-rw-   0        0        0       27 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.const
+-rw-rw-rw-   0        0        0      124 2023-06-24 09:31:58.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.const.asm
+-rw-rw-rw-   0        0        0       59 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ctz
+-rw-rw-rw-   0        0        0      295 2023-06-24 06:33:00.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ctz.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eq
+-rw-rw-rw-   0        0        0      268 2023-06-24 05:44:08.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eq.asm
+-rw-rw-rw-   0        0        0       39 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eqz
+-rw-rw-rw-   0        0        0      200 2023-06-24 05:43:48.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eqz.asm
+-rw-rw-rw-   0        0        0       33 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_s
+-rw-rw-rw-   0        0        0      169 2023-06-24 06:36:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_s.asm
+-rw-rw-rw-   0        0        0       11 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_u
+-rw-rw-rw-   0        0        0       58 2023-06-24 06:36:41.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_u.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_s
+-rw-rw-rw-   0        0        0      282 2023-06-24 05:47:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_s.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_u
+-rw-rw-rw-   0        0        0      282 2023-06-24 05:47:34.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_u.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_s
+-rw-rw-rw-   0        0        0      281 2023-06-24 05:45:53.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_s.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_u
+-rw-rw-rw-   0        0        0      281 2023-06-24 05:46:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_u.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_s
+-rw-rw-rw-   0        0        0      282 2023-06-24 05:46:31.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_s.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_u
+-rw-rw-rw-   0        0        0      282 2023-06-24 05:46:52.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_u.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_s
+-rw-rw-rw-   0        0        0      281 2023-06-24 05:44:47.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_s.asm
+-rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_u
+-rw-rw-rw-   0        0        0      281 2023-06-24 05:45:20.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_u.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ne
+-rw-rw-rw-   0        0        0      265 2023-06-24 05:44:26.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ne.asm
+-rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.or
+-rw-rw-rw-   0        0        0      244 2023-06-24 06:34:47.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.or.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.popcnt
+-rw-rw-rw-   0        0        0      186 2023-06-24 06:33:26.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.popcnt.asm
+-rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.sub
+-rw-rw-rw-   0        0        0      246 2023-06-24 06:34:02.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.sub.asm
+-rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.xor
+-rw-rw-rw-   0        0        0      246 2023-06-24 06:35:05.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.xor.asm
+-rw-rw-rw-   0        0        0      106 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/select
+-rw-rw-rw-   0        0        0      488 2023-06-24 05:37:04.000000 wasmpy-0.1.1/wasmpy/x86/instructions/select.asm
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.899568 wasmpy-0.1.1/wasmpy/x86/instructions/x64/
+-rw-rw-rw-   0        0        0       87 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.get
+-rw-rw-rw-   0        0        0      398 2023-06-24 08:53:55.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.get.asm
+-rw-rw-rw-   0        0        0      100 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.set
+-rw-rw-rw-   0        0        0      453 2023-06-24 08:54:49.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.set.asm
+-rw-rw-rw-   0        0        0      133 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.tee
+-rw-rw-rw-   0        0        0      614 2023-06-24 08:55:03.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.tee.asm
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.903138 wasmpy-0.1.1/wasmpy/x86/instructions/x86/
+-rw-rw-rw-   0        0        0       81 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.get
+-rw-rw-rw-   0        0        0      398 2023-06-24 09:03:25.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.get.asm
+-rw-rw-rw-   0        0        0       90 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.set
+-rw-rw-rw-   0        0        0      453 2023-06-24 09:03:43.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.set.asm
+-rw-rw-rw-   0        0        0      123 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.tee
+-rw-rw-rw-   0        0        0      614 2023-06-24 09:03:57.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.tee.asm
+-rw-rw-rw-   0        0        0     1193 2023-06-24 07:47:40.000000 wasmpy-0.1.1/wasmpy/x86/opcodes.h
+drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.771318 wasmpy-0.1.1/wasmpy.egg-info/
+-rw-rw-rw-   0        0        0     2445 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4933 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/top_level.txt
```

### Comparing `wasmpy-0.1.0a3/wasmpy/hooks.py` & `wasmpy-0.1.1/wasmpy/hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 from .module import read_module
 import os, sys, types
 
-class WebAssemblyBinaryLoader(object):
+
+def _call(mod):
+    def call(f: str):
+        nonlocal mod
+        for e in mod["exports"]:
+            if e["name"] == f:
+                return e["obj"]
+
+    return call
+
+
+class WebAssemblyBinaryLoader:
     """WebAssembly binary import hook.
     This hook is registered automatically with `import wasmpy`.
     After the initial import a WebAssembly binary format file (.wasm) can
     be loaded with the import statement eg:
     |- mymodule
     |  |- mymodule_2.wasm
     |
@@ -14,14 +25,15 @@
     in example.py:
     ```
     import wasmpy
     import mymodule_1
     from mymodule import mymodule_2
     ``` Will load both binary files.
     """
+
     def find_module(self, fullname, path=None):
         fname = fullname.split(".")[-1] + ".wasm"
         if path is not None and len(path):
             for p in path:
                 if os.path.isfile(os.path.join(p, fname)):
                     self.fname = os.path.join(p, fname)
                     return self
@@ -36,10 +48,13 @@
 
         mod = types.ModuleType(fullname)
         mod.__file__ = self.fname
         mod.__name__ = fullname
         mod.__loader__ = self
         sys.modules[fullname] = mod
         with open(self.fname, "rb") as fp:
-            mod.module = read_module(fp)
+            mod._module = read_module(fp)
+            mod.call = _call(mod._module)
+            if mod._module["start"] is not None:
+                mod.start = mod._module["start"]
 
         return mod
```

### Comparing `wasmpy-0.1.0a3/wasmpy/instructions.py` & `wasmpy-0.1.1/wasmpy/instructions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,619 +1,632 @@
-from .values import get_vec_len, read_sint, read_uint, read_f32, read_f64
-from .types import read_valtype
-
-
-def read_expr(buffer: object) -> tuple:
-    """Read an expression from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#expressions%E2%91%A6
-    in_ = ()
-    instruction = read_instruction(buffer)
-    while instruction != "end":
-        in_ += (instruction,)
-        instruction = read_instruction(buffer)
-
-    return (in_, "end")
-
-
-def read_memarg(buffer: object) -> dict:
-    """Read a memory arg from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#binary-memarg
-    a = read_uint(buffer, 32)
-    o = read_uint(buffer, 32)
-    return {"align": a, "offset": o}
-
-
-def read_instruction(buffer: object) -> "str or tuple":
-    """Read an instruction from buffer."""
-    data = buffer.read(1)
-    # 0x0B (end) and 0x05 (else) explicit instructions
-    if data == b"\x0b":
-        return "end"
-
-    if data == b"\x05":
-        return "else"
-
-    # Control instructions
-    # https://www.w3.org/TR/wasm-core-1/#control-instructions%E2%91%A6
-    if data == b"\0":
-        return "unreachable"
-
-    if data == b"\x01":
-        return "nop"
-
-    if data == b"\x02":
-        try:
-            rt = read_valtype(buffer)
-
-        except TypeError:
-            buffer.seek(-1, 1)
-            if buffer.read(1)[0] != 64:
-                raise TypeError("Invalid blocktype.")
-
-            rt = None
-
-        in_ = []
-        instruction = read_instruction(buffer)
-        while instruction != "end":
-            in_.append(instruction)
-            instruction = read_instruction(buffer)
-
-        return "block", rt, tuple(in_), "end"
-
-    if data == b"\x03":
-        try:
-            rt = read_valtype(buffer)
-
-        except TypeError:
-            buffer.seek(-1, 1)
-            if buffer.read(1)[0] != 64:
-                raise TypeError("Invalid blocktype.")
-
-            rt = None
-
-        in_ = []
-        instruction = read_instruction(buffer)
-        while instruction != "end":
-            in_.append(instruction)
-            instruction = read_instruction(buffer)
-
-        return "loop", rt, tuple(in_), "end"
-
-    if data == b"\x04":
-        try:
-            rt = read_valtype(buffer)
-
-        except TypeError:
-            buffer.seek(-1, 1)
-            if buffer.read(1)[0] != 64:
-                raise TypeError("Invalid blocktype.")
-
-            rt = None
-
-        in1 = []
-        instruction = read_instruction(buffer)
-        while instruction not in ["end", "else"]:
-            in1.append(instruction)
-            instruction = read_instruction(buffer)
-
-        in1 = tuple(in1)
-        if instruction == "end":
-            return "if", rt, in1, "else", (), "end"
-
-        # "else"
-        in2 = []
-        instruction = read_instruction(buffer)
-        while instruction != "end":
-            in2.append(instruction)
-            instruction = read_instruction(buffer)
-
-        return "if", rt, in1, "else", tuple(in2), "end"
-
-    if data == b"\x0c":
-        return "br", read_uint(buffer, 32)
-
-    if data == b"\x0d":
-        return "br_if", read_uint(buffer, 32)
-
-    if data == b"\x0e":
-        l = [read_uint(buffer, 32) for _ in range(get_vec_len(buffer))]
-        return "br_table", l, read_uint(buffer, 32)
-
-    if data == b"\x0f":
-        return "return"
-
-    if data == b"\x10":
-        return "call", read_uint(buffer, 32)
-
-    if data == b"\x11":
-        x = read_uint(buffer, 32)
-        assert buffer.read(1) == b"\0", "Invalid instruction."
-        return "call_indirect", x
-
-    # Parametric instructions
-    # https://www.w3.org/TR/wasm-core-1/#parametric-instructions%E2%91%A6
-    if data == b"\x1a":
-        return "drop"
-
-    if data == b"\x1b":
-        return "select"
-
-    # Variable instructions
-    # https://www.w3.org/TR/wasm-core-1/#variable-instructions%E2%91%A6
-    if data == b"\x20":
-        return "local.get", read_uint(buffer, 32)
-
-    if data == b"\x21":
-        return "local.set", read_uint(buffer, 32)
-
-    if data == b"\x22":
-        return "local.tee", read_uint(buffer, 32)
-
-    if data == b"\x23":
-        return "global.get", read_uint(buffer, 32)
-
-    if data == b"\x24":
-        return "global.set", read_uint(buffer, 32)
-
-    # Memory instructions
-    # https://www.w3.org/TR/wasm-core-1/#memory-instructions%E2%91%A6
-    if data == b"\x28":
-        return "i32.load", read_memarg(buffer)
-
-    if data == b"\x29":
-        return "i64.load", read_memarg(buffer)
-
-    if data == b"\x2a":
-        return "f32.load", read_memarg(buffer)
-
-    if data == b"\x2b":
-        return "f64.load", read_memarg(buffer)
-
-    if data == b"\x2c":
-        return "i32.load8_s", read_memarg(buffer)
-
-    if data == b"\x2d":
-        return "i32.load8_u", read_memarg(buffer)
-
-    if data == b"\x2e":
-        return "i32.load16_s", read_memarg(buffer)
-
-    if data == b"\x2f":
-        return "i32.load16_u", read_memarg(buffer)
-
-    if data == b"\x30":
-        return "i64.load8_s", read_memarg(buffer)
-
-    if data == b"\x31":
-        return "i64.load8_u", read_memarg(buffer)
-
-    if data == b"\x32":
-        return "i64.load16_s", read_memarg(buffer)
-
-    if data == b"\x33":
-        return "i64.load16_u", read_memarg(buffer)
-
-    if data == b"\x34":
-        return "i64.load32_s", read_memarg(buffer)
-
-    if data == b"\x35":
-        return "i64.load32_u", read_memarg(buffer)
-
-    if data == b"\x36":
-        return "i32.store", read_memarg(buffer)
-
-    if data == b"\x37":
-        return "i64.store", read_memarg(buffer)
-
-    if data == b"\x38":
-        return "f32.store", read_memarg(buffer)
-
-    if data == b"\x39":
-        return "f64.store", read_memarg(buffer)
-
-    if data == b"\x3a":
-        return "i32.store8", read_memarg(buffer)
-
-    if data == b"\x3b":
-        return "i32.store16", read_memarg(buffer)
-
-    if data == b"\x3c":
-        return "i64.store8", read_memarg(buffer)
-
-    if data == b"\x3d":
-        return "i64.store16", read_memarg(buffer)
-
-    if data == b"\x3e":
-        return "i64.store32", read_memarg(buffer)
-
-    if data == b"\x3f":
-        assert buffer.read(1) == b"\0"
-        return "memory.size"
-
-    if data == b"\x40":
-        assert buffer.read(1) == b"\0"
-        return "memory.grow"
-
-    # Numeric instructions
-    # https://www.w3.org/TR/wasm-core-1/#numeric-instructions%E2%91%A6
-    if data == b"\x41":
-        return "i32.const", read_sint(buffer, 32)
-
-    if data == b"\x42":
-        return "i64.const", read_sint(buffer, 64)
-
-    if data == b"\x43":
-        return "f32.const", read_f32(buffer)
-
-    if data == b"\x44":
-        return "f64.const", read_f64(buffer)
-
-    if data == b"\x45":
-        return "i32.eqz"
-
-    if data == b"\x46":
-        return "i32.eq"
-
-    if data == b"\x47":
-        return "i32.ne"
-
-    if data == b"\x48":
-        return "i32.lt_s"
-
-    if data == b"\x49":
-        return "i32.lt_u"
-
-    if data == b"\x4a":
-        return "i32.gt_s"
-
-    if data == b"\x4b":
-        return "i32.gt_u"
-
-    if data == b"\x4c":
-        return "i32.le_s"
-
-    if data == b"\x4d":
-        return "i32.le_u"
-
-    if data == b"\x4e":
-        return "i32.ge_s"
-
-    if data == b"\x4f":
-        return "i32.ge_u"
-
-    if data == b"\x50":
-        return "i64.eqz"
-
-    if data == b"\x51":
-        return "i64.eq"
-
-    if data == b"\x52":
-        return "i64.ne"
-
-    if data == b"\x53":
-        return "i64.lt_s"
-
-    if data == b"\x54":
-        return "i64.lt_u"
-
-    if data == b"\x55":
-        return "i64.gt_s"
-
-    if data == b"\x56":
-        return "i64.gt_u"
-
-    if data == b"\x57":
-        return "i64.le_s"
-
-    if data == b"\x58":
-        return "i64.le_u"
-
-    if data == b"\x59":
-        return "i64.ge_s"
-
-    if data == b"\x5a":
-        return "i64.ge_u"
-
-    if data == b"\x5b":
-        return "f32.eq"
-
-    if data == b"\x5c":
-        return "f32.ne"
-
-    if data == b"\x5d":
-        return "f32.lt"
-
-    if data == b"\x5e":
-        return "f32.gt"
-
-    if data == b"\x5f":
-        return "f32.le"
-
-    if data == b"\x60":
-        return "f32.ge"
-
-    if data == b"\x61":
-        return "f64.eq"
-
-    if data == b"\x62":
-        return "f64.ne"
-
-    if data == b"\x63":
-        return "f64.lt"
-
-    if data == b"\x64":
-        return "f64.gt"
-
-    if data == b"\x65":
-        return "f64.le"
-
-    if data == b"\x66":
-        return "f64.ge"
-
-    if data == b"\x67":
-        return "i32.clz"
-
-    if data == b"\x68":
-        return "i32.ctz"
-
-    if data == b"\x69":
-        return "i32.popcnt"
-
-    if data == b"\x6a":
-        return "i32.add"
-
-    if data == b"\x6b":
-        return "i32.sub"
-
-    if data == b"\x6c":
-        return "i32.mul"
-
-    if data == b"\x6d":
-        return "i32.div_s"
-
-    if data == b"\x6e":
-        return "i32.div_u"
-
-    if data == b"\x6f":
-        return "i32.rem_s"
-
-    if data == b"\x70":
-        return "i32.rem_u"
-
-    if data == b"\x71":
-        return "i32.and"
-
-    if data == b"\x72":
-        return "i32.or"
-
-    if data == b"\x73":
-        return "i32.xor"
-
-    if data == b"\x74":
-        return "i32.shl"
-
-    if data == b"\x75":
-        return "i32.shr_s"
-
-    if data == b"\x76":
-        return "i32.shr_u"
-
-    if data == b"\x77":
-        return "i32.rotl"
-
-    if data == b"\x78":
-        return "i32.rotr"
-
-    if data == b"\x79":
-        return "i64.clz"
-
-    if data == b"\x7a":
-        return "i64.ctz"
-
-    if data == b"\x7b":
-        return "i64.popcnt"
-
-    if data == b"\x7c":
-        return "i64.add"
-
-    if data == b"\x7d":
-        return "i64.sub"
-
-    if data == b"\x7e":
-        return "i64.mul"
-
-    if data == b"\x7f":
-        return "i64.div_s"
-
-    if data == b"\x80":
-        return "i64.div_u"
-
-    if data == b"\x81":
-        return "i64.rem_s"
-
-    if data == b"\x82":
-        return "i64.rem_u"
-
-    if data == b"\x83":
-        return "i64.and"
-
-    if data == b"\x84":
-        return "i64.or"
-
-    if data == b"\x85":
-        return "i64.xor"
-
-    if data == b"\x86":
-        return "i64.shl"
-
-    if data == b"\x87":
-        return "i64.shr_s"
-
-    if data == b"\x88":
-        return "i64.shr_u"
-
-    if data == b"\x89":
-        return "i64.rotl"
-
-    if data == b"\x8a":
-        return "i64.rotr"
-
-    if data == b"\x8b":
-        return "f32.abs"
-
-    if data == b"\x8c":
-        return "f32.neg"
-
-    if data == b"\x8d":
-        return "f32.ceil"
-
-    if data == b"\x8e":
-        return "f32.floor"
-
-    if data == b"\x8f":
-        return "f32.trunc"
-
-    if data == b"\x90":
-        return "f32.nearset"
-
-    if data == b"\x91":
-        return "f32.sqrt"
-
-    if data == b"\x92":
-        return "f32.add"
-
-    if data == b"\x93":
-        return "f32.sub"
-
-    if data == b"\x94":
-        return "f32.mul"
-
-    if data == b"\x95":
-        return "f32.div"
-
-    if data == b"\x96":
-        return "f32.min"
-
-    if data == b"\x97":
-        return "f32.max"
-
-    if data == b"\x98":
-        return "f32.copysign"
-
-    if data == b"\x99":
-        return "f64.abs"
-
-    if data == b"\x9a":
-        return "f64.neg"
-
-    if data == b"\x9b":
-        return "f64.ceil"
-
-    if data == b"\x9c":
-        return "f64.floor"
-
-    if data == b"\x9d":
-        return "f64.trunc"
-
-    if data == b"\x9e":
-        return "f64.nearset"
-
-    if data == b"\x9f":
-        return "f64.sqrt"
-
-    if data == b"\xa0":
-        return "f64.add"
-
-    if data == b"\xa1":
-        return "f64.sub"
-
-    if data == b"\xa2":
-        return "f64.mul"
-
-    if data == b"\xa3":
-        return "f64.div"
-
-    if data == b"\xa4":
-        return "f64.min"
-
-    if data == b"\xa5":
-        return "f64.max"
-
-    if data == b"\xa6":
-        return "f64.copysign"
-
-    if data == b"\xa7":
-        return "i32.wrap_i64"
-
-    if data == b"\xa8":
-        return "i32.trunc_f32_s"
-
-    if data == b"\xa9":
-        return "i32.trunc_f32_u"
-
-    if data == b"\xaa":
-        return "i32.trunc_f64_s"
-
-    if data == b"\xab":
-        return "i32.trunc_f64_u"
-
-    if data == b"\xac":
-        return "i64.extend_i32_s"
-
-    if data == b"\xad":
-        return "i64.extend_i32_u"
-
-    if data == b"\xae":
-        return "i64.trunc_f32_s"
-
-    if data == b"\xaf":
-        return "i64.trunc_f32_u"
-
-    if data == b"\xb0":
-        return "i64.trunc_f64_s"
-
-    if data == b"\xb1":
-        return "i64.trunc_f64_u"
-
-    if data == b"\xb2":
-        return "f32.convert_i32_s"
-
-    if data == b"\xb3":
-        return "f32.convert_i32_u"
-
-    if data == b"\xb4":
-        return "f32.convert_i64_s"
-
-    if data == b"\xb5":
-        return "f32.convert_i64_u"
-
-    if data == b"\xb6":
-        return "f32.demote_f64"
-
-    if data == b"\xb7":
-        return "f64.convert_i32_s"
-
-    if data == b"\xb8":
-        return "f64.convert_i32_u"
-
-    if data == b"\xb9":
-        return "f64.convert_i64_s"
-
-    if data == b"\xba":
-        return "f64.convert_i64_u"
-
-    if data == b"\xbb":
-        return "f64.promote_f32"
-
-    if data == b"\xbc":
-        return "i32.reinterpret_f32"
-
-    if data == b"\xbd":
-        return "i64.reinterpret_f64"
-
-    if data == b"\xbe":
-        return "f32.reinterpret_i32"
-
-    if data == b"\xbf":
-        return "f64.reinterpret_i64"
-
-    raise TypeError("Invalid instruction type.")
+from .values import get_vec_len, read_sint, read_uint, read_f32, read_f64
+from .types import read_valtype
+
+
+def expand_bytes(n, bits=32):
+    r = n & 255, (n >> 8) & 255, (n >> 16) & 255, (n >> 24) & 255
+    if bits == 32:
+        return r
+
+    return r + (
+        (n >> 32) & 255,
+        (n >> 40) & 255,
+        (n >> 48) & 255,
+        (n >> 56) & 255,
+    )
+
+
+def read_expr(buffer: object) -> tuple:
+    """Read an expression from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#expressions%E2%91%A6
+    in_ = ()
+    instruction = read_instruction(buffer)
+    while instruction != "end":
+        in_ += (instruction,)
+        instruction = read_instruction(buffer)
+
+    return in_
+
+
+def read_memarg(buffer: object) -> dict:
+    """Read a memory arg from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#binary-memarg
+    a = read_uint(buffer, 32)
+    o = read_uint(buffer, 32)
+    return {"align": a, "offset": o}
+
+
+def read_instruction(buffer: object) -> "str or tuple":
+    """Read an instruction from buffer."""
+    data = buffer.read(1)
+    # 0x0B (end) and 0x05 (else) explicit instructions
+    if data == b"\x0b":
+        return "end"
+
+    if data == b"\x05":
+        return "else"
+
+    # Control instructions
+    # https://www.w3.org/TR/wasm-core-1/#control-instructions%E2%91%A6
+    if data == b"\0":
+        return "unreachable"
+
+    if data == b"\x01":
+        return "nop"
+
+    if data == b"\x02":
+        try:
+            rt = read_valtype(buffer)
+
+        except TypeError:
+            buffer.seek(-1, 1)
+            if buffer.read(1)[0] != 64:
+                raise TypeError("Invalid blocktype.")
+
+            rt = None
+
+        in_ = []
+        instruction = read_instruction(buffer)
+        while instruction != "end":
+            in_.append(instruction)
+            instruction = read_instruction(buffer)
+
+        return "block", rt, tuple(in_), "end"
+
+    if data == b"\x03":
+        try:
+            rt = read_valtype(buffer)
+
+        except TypeError:
+            buffer.seek(-1, 1)
+            if buffer.read(1)[0] != 64:
+                raise TypeError("Invalid blocktype.")
+
+            rt = None
+
+        in_ = []
+        instruction = read_instruction(buffer)
+        while instruction != "end":
+            in_.append(instruction)
+            instruction = read_instruction(buffer)
+
+        return "loop", rt, tuple(in_), "end"
+
+    if data == b"\x04":
+        try:
+            rt = read_valtype(buffer)
+
+        except TypeError:
+            buffer.seek(-1, 1)
+            if buffer.read(1)[0] != 64:
+                raise TypeError("Invalid blocktype.")
+
+            rt = None
+
+        in1 = []
+        instruction = read_instruction(buffer)
+        while instruction not in ["end", "else"]:
+            in1.append(instruction)
+            instruction = read_instruction(buffer)
+
+        in1 = tuple(in1)
+        if instruction == "end":
+            return "if", rt, in1, "else", (), "end"
+
+        # "else"
+        in2 = []
+        instruction = read_instruction(buffer)
+        while instruction != "end":
+            in2.append(instruction)
+            instruction = read_instruction(buffer)
+
+        return "if", rt, in1, "else", tuple(in2), "end"
+
+    if data == b"\x0c":
+        return "br", read_uint(buffer, 32)
+
+    if data == b"\x0d":
+        return "br_if", read_uint(buffer, 32)
+
+    if data == b"\x0e":
+        l = [read_uint(buffer, 32) for _ in range(get_vec_len(buffer))]
+        return "br_table", l, read_uint(buffer, 32)
+
+    if data == b"\x0f":
+        return "return"
+
+    if data == b"\x10":
+        return "call", read_uint(buffer, 32)
+
+    if data == b"\x11":
+        x = read_uint(buffer, 32)
+        assert buffer.read(1) == b"\0", "Invalid instruction."
+        return "call_indirect", x
+
+    # Parametric instructions
+    # https://www.w3.org/TR/wasm-core-1/#parametric-instructions%E2%91%A6
+    if data == b"\x1a":
+        return "drop", data[0]
+
+    if data == b"\x1b":
+        return "select", data[0]
+
+    # Variable instructions
+    # https://www.w3.org/TR/wasm-core-1/#variable-instructions%E2%91%A6
+    if data == b"\x20":
+        return ("local.get", data[0]) + expand_bytes(read_uint(buffer, 32))
+
+    if data == b"\x21":
+        return ("local.set", data[0]) + expand_bytes(read_uint(buffer, 32))
+
+    if data == b"\x22":
+        return ("local.tee", data[0]) + expand_bytes(read_uint(buffer, 32))
+
+    if data == b"\x23":
+        return ("global.get", data[0]) + expand_bytes(read_uint(buffer, 32))
+
+    if data == b"\x24":
+        return ("global.set", data[0]) + expand_bytes(read_uint(buffer, 32))
+
+    # Memory instructions
+    # https://www.w3.org/TR/wasm-core-1/#memory-instructions%E2%91%A6
+    if data == b"\x28":
+        return "i32.load", data[0], read_memarg(buffer)
+
+    if data == b"\x29":
+        return "i64.load", data[0], read_memarg(buffer)
+
+    if data == b"\x2a":
+        return "f32.load", data[0], read_memarg(buffer)
+
+    if data == b"\x2b":
+        return "f64.load", data[0], read_memarg(buffer)
+
+    if data == b"\x2c":
+        return "i32.load8_s", data[0], read_memarg(buffer)
+
+    if data == b"\x2d":
+        return "i32.load8_u", data[0], read_memarg(buffer)
+
+    if data == b"\x2e":
+        return "i32.load16_s", data[0], read_memarg(buffer)
+
+    if data == b"\x2f":
+        return "i32.load16_u", data[0], read_memarg(buffer)
+
+    if data == b"\x30":
+        return "i64.load8_s", data[0], read_memarg(buffer)
+
+    if data == b"\x31":
+        return "i64.load8_u", data[0], read_memarg(buffer)
+
+    if data == b"\x32":
+        return "i64.load16_s", data[0], read_memarg(buffer)
+
+    if data == b"\x33":
+        return "i64.load16_u", data[0], read_memarg(buffer)
+
+    if data == b"\x34":
+        return "i64.load32_s", data[0], read_memarg(buffer)
+
+    if data == b"\x35":
+        return "i64.load32_u", data[0], read_memarg(buffer)
+
+    if data == b"\x36":
+        return "i32.store", data[0], read_memarg(buffer)
+
+    if data == b"\x37":
+        return "i64.store", data[0], read_memarg(buffer)
+
+    if data == b"\x38":
+        return "f32.store", data[0], read_memarg(buffer)
+
+    if data == b"\x39":
+        return "f64.store", data[0], read_memarg(buffer)
+
+    if data == b"\x3a":
+        return "i32.store8", data[0], read_memarg(buffer)
+
+    if data == b"\x3b":
+        return "i32.store16", data[0], read_memarg(buffer)
+
+    if data == b"\x3c":
+        return "i64.store8", data[0], read_memarg(buffer)
+
+    if data == b"\x3d":
+        return "i64.store16", data[0], read_memarg(buffer)
+
+    if data == b"\x3e":
+        return "i64.store32", data[0], read_memarg(buffer)
+
+    if data == b"\x3f":
+        assert buffer.read(1) == b"\0"
+        return "memory.size", data[0]
+
+    if data == b"\x40":
+        assert buffer.read(1) == b"\0"
+        return "memory.grow", data[0]
+
+    # Numeric instructions
+    # https://www.w3.org/TR/wasm-core-1/#numeric-instructions%E2%91%A6
+    if data == b"\x41":
+        return ("i32.const", data[0]) + expand_bytes(read_sint(buffer, 32))
+
+    if data == b"\x42":
+        return ("i64.const", data[0]) + expand_bytes(read_sint(buffer, 64), 64)
+
+    if data == b"\x43":
+        return ("f32.const", data[0]) + expand_bytes(read_f32(buffer))
+
+    if data == b"\x44":
+        return ("f64.const", data[0]) + expand_bytes(read_f64(buffer))
+
+    if data == b"\x45":
+        return "i32.eqz", data[0]
+
+    if data == b"\x46":
+        return "i32.eq", data[0]
+
+    if data == b"\x47":
+        return "i32.ne", data[0]
+
+    if data == b"\x48":
+        return "i32.lt_s", data[0]
+
+    if data == b"\x49":
+        return "i32.lt_u", data[0]
+
+    if data == b"\x4a":
+        return "i32.gt_s", data[0]
+
+    if data == b"\x4b":
+        return "i32.gt_u", data[0]
+
+    if data == b"\x4c":
+        return "i32.le_s", data[0]
+
+    if data == b"\x4d":
+        return "i32.le_u", data[0]
+
+    if data == b"\x4e":
+        return "i32.ge_s", data[0]
+
+    if data == b"\x4f":
+        return "i32.ge_u", data[0]
+
+    if data == b"\x50":
+        return "i64.eqz", data[0]
+
+    if data == b"\x51":
+        return "i64.eq", data[0]
+
+    if data == b"\x52":
+        return "i64.ne", data[0]
+
+    if data == b"\x53":
+        return "i64.lt_s", data[0]
+
+    if data == b"\x54":
+        return "i64.lt_u", data[0]
+
+    if data == b"\x55":
+        return "i64.gt_s", data[0]
+
+    if data == b"\x56":
+        return "i64.gt_u", data[0]
+
+    if data == b"\x57":
+        return "i64.le_s", data[0]
+
+    if data == b"\x58":
+        return "i64.le_u", data[0]
+
+    if data == b"\x59":
+        return "i64.ge_s", data[0]
+
+    if data == b"\x5a":
+        return "i64.ge_u", data[0]
+
+    if data == b"\x5b":
+        return "f32.eq", data[0]
+
+    if data == b"\x5c":
+        return "f32.ne", data[0]
+
+    if data == b"\x5d":
+        return "f32.lt", data[0]
+
+    if data == b"\x5e":
+        return "f32.gt", data[0]
+
+    if data == b"\x5f":
+        return "f32.le", data[0]
+
+    if data == b"\x60":
+        return "f32.ge", data[0]
+
+    if data == b"\x61":
+        return "f64.eq", data[0]
+
+    if data == b"\x62":
+        return "f64.ne", data[0]
+
+    if data == b"\x63":
+        return "f64.lt", data[0]
+
+    if data == b"\x64":
+        return "f64.gt", data[0]
+
+    if data == b"\x65":
+        return "f64.le", data[0]
+
+    if data == b"\x66":
+        return "f64.ge", data[0]
+
+    if data == b"\x67":
+        return "i32.clz", data[0]
+
+    if data == b"\x68":
+        return "i32.ctz", data[0]
+
+    if data == b"\x69":
+        return "i32.popcnt", data[0]
+
+    if data == b"\x6a":
+        return "i32.add", data[0]
+
+    if data == b"\x6b":
+        return "i32.sub", data[0]
+
+    if data == b"\x6c":
+        return "i32.mul", data[0]
+
+    if data == b"\x6d":
+        return "i32.div_s", data[0]
+
+    if data == b"\x6e":
+        return "i32.div_u", data[0]
+
+    if data == b"\x6f":
+        return "i32.rem_s", data[0]
+
+    if data == b"\x70":
+        return "i32.rem_u", data[0]
+
+    if data == b"\x71":
+        return "i32.and", data[0]
+
+    if data == b"\x72":
+        return "i32.or", data[0]
+
+    if data == b"\x73":
+        return "i32.xor", data[0]
+
+    if data == b"\x74":
+        return "i32.shl", data[0]
+
+    if data == b"\x75":
+        return "i32.shr_s", data[0]
+
+    if data == b"\x76":
+        return "i32.shr_u", data[0]
+
+    if data == b"\x77":
+        return "i32.rotl", data[0]
+
+    if data == b"\x78":
+        return "i32.rotr", data[0]
+
+    if data == b"\x79":
+        return "i64.clz", data[0]
+
+    if data == b"\x7a":
+        return "i64.ctz", data[0]
+
+    if data == b"\x7b":
+        return "i64.popcnt", data[0]
+
+    if data == b"\x7c":
+        return "i64.add", data[0]
+
+    if data == b"\x7d":
+        return "i64.sub", data[0]
+
+    if data == b"\x7e":
+        return "i64.mul", data[0]
+
+    if data == b"\x7f":
+        return "i64.div_s", data[0]
+
+    if data == b"\x80":
+        return "i64.div_u", data[0]
+
+    if data == b"\x81":
+        return "i64.rem_s", data[0]
+
+    if data == b"\x82":
+        return "i64.rem_u", data[0]
+
+    if data == b"\x83":
+        return "i64.and", data[0]
+
+    if data == b"\x84":
+        return "i64.or", data[0]
+
+    if data == b"\x85":
+        return "i64.xor", data[0]
+
+    if data == b"\x86":
+        return "i64.shl", data[0]
+
+    if data == b"\x87":
+        return "i64.shr_s", data[0]
+
+    if data == b"\x88":
+        return "i64.shr_u", data[0]
+
+    if data == b"\x89":
+        return "i64.rotl", data[0]
+
+    if data == b"\x8a":
+        return "i64.rotr", data[0]
+
+    if data == b"\x8b":
+        return "f32.abs", data[0]
+
+    if data == b"\x8c":
+        return "f32.neg", data[0]
+
+    if data == b"\x8d":
+        return "f32.ceil", data[0]
+
+    if data == b"\x8e":
+        return "f32.floor", data[0]
+
+    if data == b"\x8f":
+        return "f32.trunc", data[0]
+
+    if data == b"\x90":
+        return "f32.nearset", data[0]
+
+    if data == b"\x91":
+        return "f32.sqrt", data[0]
+
+    if data == b"\x92":
+        return "f32.add", data[0]
+
+    if data == b"\x93":
+        return "f32.sub", data[0]
+
+    if data == b"\x94":
+        return "f32.mul", data[0]
+
+    if data == b"\x95":
+        return "f32.div", data[0]
+
+    if data == b"\x96":
+        return "f32.min", data[0]
+
+    if data == b"\x97":
+        return "f32.max", data[0]
+
+    if data == b"\x98":
+        return "f32.copysign", data[0]
+
+    if data == b"\x99":
+        return "f64.abs", data[0]
+
+    if data == b"\x9a":
+        return "f64.neg", data[0]
+
+    if data == b"\x9b":
+        return "f64.ceil", data[0]
+
+    if data == b"\x9c":
+        return "f64.floor", data[0]
+
+    if data == b"\x9d":
+        return "f64.trunc", data[0]
+
+    if data == b"\x9e":
+        return "f64.nearset", data[0]
+
+    if data == b"\x9f":
+        return "f64.sqrt", data[0]
+
+    if data == b"\xa0":
+        return "f64.add", data[0]
+
+    if data == b"\xa1":
+        return "f64.sub", data[0]
+
+    if data == b"\xa2":
+        return "f64.mul", data[0]
+
+    if data == b"\xa3":
+        return "f64.div", data[0]
+
+    if data == b"\xa4":
+        return "f64.min", data[0]
+
+    if data == b"\xa5":
+        return "f64.max", data[0]
+
+    if data == b"\xa6":
+        return "f64.copysign", data[0]
+
+    if data == b"\xa7":
+        return "i32.wrap_i64", data[0]
+
+    if data == b"\xa8":
+        return "i32.trunc_f32_s", data[0]
+
+    if data == b"\xa9":
+        return "i32.trunc_f32_u", data[0]
+
+    if data == b"\xaa":
+        return "i32.trunc_f64_s", data[0]
+
+    if data == b"\xab":
+        return "i32.trunc_f64_u", data[0]
+
+    if data == b"\xac":
+        return "i64.extend_i32_s", data[0]
+
+    if data == b"\xad":
+        return "i64.extend_i32_u", data[0]
+
+    if data == b"\xae":
+        return "i64.trunc_f32_s", data[0]
+
+    if data == b"\xaf":
+        return "i64.trunc_f32_u", data[0]
+
+    if data == b"\xb0":
+        return "i64.trunc_f64_s", data[0]
+
+    if data == b"\xb1":
+        return "i64.trunc_f64_u", data[0]
+
+    if data == b"\xb2":
+        return "f32.convert_i32_s", data[0]
+
+    if data == b"\xb3":
+        return "f32.convert_i32_u", data[0]
+
+    if data == b"\xb4":
+        return "f32.convert_i64_s", data[0]
+
+    if data == b"\xb5":
+        return "f32.convert_i64_u", data[0]
+
+    if data == b"\xb6":
+        return "f32.demote_f64", data[0]
+
+    if data == b"\xb7":
+        return "f64.convert_i32_s", data[0]
+
+    if data == b"\xb8":
+        return "f64.convert_i32_u", data[0]
+
+    if data == b"\xb9":
+        return "f64.convert_i64_s", data[0]
+
+    if data == b"\xba":
+        return "f64.convert_i64_u", data[0]
+
+    if data == b"\xbb":
+        return "f64.promote_f32", data[0]
+
+    if data == b"\xbc":
+        return "i32.reinterpret_f32", data[0]
+
+    if data == b"\xbd":
+        return "i64.reinterpret_f64", data[0]
+
+    if data == b"\xbe":
+        return "f32.reinterpret_i32", data[0]
+
+    if data == b"\xbf":
+        return "f64.reinterpret_i64", data[0]
+
+    raise TypeError("Invalid instruction type.")
```

### Comparing `wasmpy-0.1.0a3/wasmpy/sections.py` & `wasmpy-0.1.1/wasmpy/sections.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,168 +1,177 @@
-from .types import (
-    read_functype,
-    read_globaltype,
-    read_memtype,
-    read_tabletype,
-    read_valtype,
-)
-from .values import get_vec_len, read_name, read_uint
-from .instructions import read_expr
-
-
-def read_customsec(buffer: object, length: int) -> None:
-    """Read a custom section from buffer."""
-    # Does not return anything as custom sections are dropped.
-    # https://www.w3.org/TR/wasm-core-1/#custom-section%E2%91%A0
-    buffer.read(length)
-
-
-def read_typesec(buffer: object) -> tuple:
-    """Read a type section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#type-section%E2%91%A0
-    return tuple(read_functype(buffer) for _ in range(get_vec_len(buffer)))
-
-
-def read_importsec(buffer: object) -> tuple:
-    """Read an import section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#import-section%E2%91%A0
-    im = ()
-    try:
-        for _ in range(get_vec_len(buffer)):
-            import_ = {"module": read_name(buffer), "name": read_name(buffer)}
-            flag = buffer.read(1)[0]
-            assert flag in range(4)
-            if not flag:
-                import_["desc"] = ("func", read_uint(buffer, 32))
-
-            elif flag == 1:
-                import_["desc"] = ("table", read_tabletype(buffer))
-
-            elif flag == 2:
-                import_["desc"] = ("mem", read_memtype(buffer))
-
-            elif flag == 3:
-                import_["desc"] = ("global", read_globaltype(buffer))
-
-            im += (import_,)
-
-    except (IndexError, AssertionError):
-        raise TypeError("Invalid import section.")
-
-    return im
-
-
-def read_funcsec(buffer: object) -> tuple:
-    """Read a function section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#function-section%E2%91%A0
-    return tuple(read_uint(buffer, 32) for _ in range(get_vec_len(buffer)))
-
-
-def read_tablesec(buffer: object) -> tuple:
-    """Read a table section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#table-section%E2%91%A0
-    return tuple({"type": read_tabletype(buffer)} for _ in range(get_vec_len(buffer)))
-
-
-def read_memsec(buffer: object) -> tuple:
-    """Read a memory section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#memory-section%E2%91%A0
-    return tuple({"type": read_memtype(buffer)} for _ in range(get_vec_len(buffer)))
-
-
-def read_globalsec(buffer: object) -> tuple:
-    """Read a global section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#global-section%E2%91%A0
-    return tuple(
-        {"gt": read_globaltype(buffer), "e": read_expr(buffer)}
-        for _ in range(get_vec_len(buffer))
-    )
-
-
-def read_exportsec(buffer: object) -> tuple:
-    """Read an export section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#export-section%E2%91%A0
-    ex = ()
-    for _ in range(get_vec_len(buffer)):
-        export = {"name": read_name(buffer)}
-        desc = buffer.read(1)[0]
-        assert desc in range(4)
-        if not desc:
-            export["desc"] = "func", read_uint(buffer, 32)
-
-        if desc == 1:
-            export["desc"] = "table", read_uint(buffer, 32)
-
-        if desc == 2:
-            export["desc"] = "mem", read_uint(buffer, 32)
-
-        if desc == 3:
-            export["desc"] = "global", read_uint(buffer, 32)
-
-        ex += (export,)
-
-    return ex
-
-
-def read_startsec(buffer: object) -> dict:
-    """Read a start section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#start-section%E2%91%A0
-    return {"func": read_uint(buffer, 32)}
-
-
-def read_elemsec(buffer: object) -> tuple:
-    """Read an element section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#element-section%E2%91%A0
-    seg = ()
-    for _ in range(get_vec_len(buffer)):
-        seg += (
-            {
-                "table": read_uint(buffer, 32),
-                "offset": read_expr(buffer),
-                "init": tuple(
-                    read_uint(buffer, 32) for _ in range(get_vec_len(buffer))
-                ),
-            },
-        )
-
-    return seg
-
-
-def read_codesec(buffer: object) -> tuple:
-    """Read a code section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#code-section%E2%91%A0
-    code = ()
-    try:
-        for _ in range(get_vec_len(buffer)):
-            size = read_uint(buffer, 32)
-            start = buffer.tell()
-
-            t = ()
-            for _ in range(get_vec_len(buffer)):
-                n = read_uint(buffer, 32)
-                t += ((read_valtype(buffer),),)
-
-            concat_t = ()
-            for locals in t:
-                concat_t += locals
-
-            code += ((concat_t, read_expr(buffer)),)
-            end = buffer.tell()
-            assert size == end - start
-
-    except AssertionError:
-        raise TypeError("Invalid code section.")
-
-    return code
-
-
-def read_datasec(buffer: object) -> tuple:
-    """Read a data section from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#data-section%E2%91%A0
-    return tuple(
-        {
-            "data": read_uint(buffer, 32),
-            "offset": read_expr(buffer),
-            "init": tuple(buffer.read(1)[0] for _ in range(get_vec_len(buffer))),
-        }
-        for _ in range(get_vec_len(buffer))
-    )
+from .types import (
+    read_functype,
+    read_globaltype,
+    read_memtype,
+    read_tabletype,
+    read_valtype,
+)
+from .values import get_vec_len, read_name, read_uint
+from .instructions import read_expr
+
+
+def read_customsec(buffer: object, length: int) -> tuple:
+    """Read a custom section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#custom-section%E2%91%A0
+    start = buffer.tell()
+    name = read_name(buffer)
+    bytes = buffer.read(length - (buffer.tell() - start))
+    return name, bytes
+
+
+def read_typesec(buffer: object) -> tuple:
+    """Read a type section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#type-section%E2%91%A0
+    return tuple(read_functype(buffer) for _ in range(get_vec_len(buffer)))
+
+
+def read_importsec(buffer: object) -> tuple:
+    """Read an import section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#import-section%E2%91%A0
+    im = ()
+    try:
+        for _ in range(get_vec_len(buffer)):
+            import_ = {"module": read_name(buffer), "name": read_name(buffer)}
+            flag = buffer.read(1)[0]
+            assert flag in range(4)
+            if not flag:
+                import_["desc"] = ("func", read_uint(buffer, 32))
+
+            elif flag == 1:
+                import_["desc"] = ("table", read_tabletype(buffer))
+
+            elif flag == 2:
+                import_["desc"] = ("mem", read_memtype(buffer))
+
+            elif flag == 3:
+                import_["desc"] = ("global", read_globaltype(buffer))
+
+            im += (import_,)
+
+    except (IndexError, AssertionError):
+        raise TypeError("Invalid import section.")
+
+    return im
+
+
+def read_funcsec(buffer: object) -> tuple:
+    """Read a function section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#function-section%E2%91%A0
+    return tuple(read_uint(buffer, 32) for _ in range(get_vec_len(buffer)))
+
+
+def read_tablesec(buffer: object) -> tuple:
+    """Read a table section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#table-section%E2%91%A0
+    return tuple(
+        {"type": read_tabletype(buffer)} for _ in range(get_vec_len(buffer))
+    )
+
+
+def read_memsec(buffer: object) -> tuple:
+    """Read a memory section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#memory-section%E2%91%A0
+    return tuple(
+        {"type": read_memtype(buffer)} for _ in range(get_vec_len(buffer))
+    )
+
+
+def read_globalsec(buffer: object) -> tuple:
+    """Read a global section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#global-section%E2%91%A0
+    return tuple(
+        {"gt": read_globaltype(buffer), "e": read_expr(buffer)}
+        for _ in range(get_vec_len(buffer))
+    )
+
+
+def read_exportsec(buffer: object) -> tuple:
+    """Read an export section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#export-section%E2%91%A0
+    ex = ()
+    for _ in range(get_vec_len(buffer)):
+        export = {"name": read_name(buffer)}
+        desc = buffer.read(1)[0]
+        assert desc in range(4)
+        if not desc:
+            export["desc"] = "func", read_uint(buffer, 32)
+
+        if desc == 1:
+            export["desc"] = "table", read_uint(buffer, 32)
+
+        if desc == 2:
+            export["desc"] = "mem", read_uint(buffer, 32)
+
+        if desc == 3:
+            export["desc"] = "global", read_uint(buffer, 32)
+
+        ex += (export,)
+
+    return ex
+
+
+def read_startsec(buffer: object) -> int:
+    """Read a start section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#start-section%E2%91%A0
+    return read_uint(buffer, 32)
+
+
+def read_elemsec(buffer: object) -> tuple:
+    """Read an element section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#element-section%E2%91%A0
+    seg = ()
+    for _ in range(get_vec_len(buffer)):
+        seg += (
+            {
+                "table": read_uint(buffer, 32),
+                "offset": read_expr(buffer),
+                "init": tuple(
+                    read_uint(buffer, 32) for _ in range(get_vec_len(buffer))
+                ),
+            },
+        )
+
+    return seg
+
+
+def read_codesec(buffer: object) -> tuple:
+    """Read a code section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#code-section%E2%91%A0
+    code = ()
+    try:
+        for _ in range(get_vec_len(buffer)):
+            size = read_uint(buffer, 32)
+            start = buffer.tell()
+
+            t = ()
+            for _ in range(get_vec_len(buffer)):
+                n = read_uint(buffer, 32)
+                v = buffer.read(1)[0]
+                t += (tuple(v for _ in range(n)),)
+
+            concat_t = ()
+            for locals in t:
+                concat_t += locals
+
+            code += ((concat_t, read_expr(buffer)),)
+            end = buffer.tell()
+            assert size == end - start
+
+    except AssertionError:
+        raise TypeError("Invalid code section.")
+
+    return code
+
+
+def read_datasec(buffer: object) -> tuple:
+    """Read a data section from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#data-section%E2%91%A0
+    return tuple(
+        {
+            "data": read_uint(buffer, 32),
+            "offset": read_expr(buffer),
+            "init": tuple(
+                buffer.read(1)[0] for _ in range(get_vec_len(buffer))
+            ),
+        }
+        for _ in range(get_vec_len(buffer))
+    )
```

### Comparing `wasmpy-0.1.0a3/wasmpy/values.py` & `wasmpy-0.1.1/wasmpy/values.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import math, struct
-
-f32 = struct.Struct("<f")
-f64 = struct.Struct("<d")
-
-
-def get_vec_len(buffer):
-    """Return the length of a vector consumed from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#vectors%E2%91%A2
-    return read_uint(buffer, 32)
-
-
-def read_uint(buffer, bits):
-    """Read an unsigned integer stored in LEB128 format."""
-    # https://www.w3.org/TR/wasm-core-1/#integers%E2%91%A4
-    consumed_bytes = 0
-    result = 0
-    shift = 0
-
-    try:
-        while True:
-            byte = buffer.read(1)[0]
-            consumed_bytes += 1
-            assert consumed_bytes <= math.ceil(bits / 7)
-            result |= (byte & 127) << shift
-            if not byte >> 7:
-                break
-
-            shift += 7
-
-    except (AssertionError, IndexError):
-        raise TypeError("Invalid integer.")
-
-    return result
-
-
-def read_sint(buffer, bits):
-    """Read a signed integer stored in LEB128 format."""
-    # https://www.w3.org/TR/wasm-core-1/#integers%E2%91%A4
-    try:
-        byte = buffer.read(1)[0]
-        consumed_bytes = 1
-        result = byte & 127
-        shift = 7
-        while byte >> 7:
-            byte = buffer.read(1)[0]
-            consumed_bytes += 1
-            assert consumed_bytes <= math.ceil(bits / 7)
-            result |= (byte & 127) << shift
-            shift += 7
-
-    except (AssertionError, IndexError):
-        raise TypeError("Invalid integer.")
-
-    if result >> consumed_bytes * 7 - 1:
-        result |= ~0 << shift
-
-    return result
-
-
-def read_f32(buffer):
-    """Read a single precision float from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#floating-point%E2%91%A4
-    return f32.unpack(buffer.read(4))
-
-
-def read_f64(buffer):
-    """Read a double precision float from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#floating-point%E2%91%A4
-    return f64.unpack(buffer.read(8))
-
-
-def read_name(buffer):
-    """Read a name from buffer."""
-    # https://www.w3.org/TR/wasm-core-1/#names%E2%91%A2
-    return buffer.read(get_vec_len(buffer)).decode("utf-8")
+import math, struct
+
+f32 = struct.Struct("<f")
+f64 = struct.Struct("<d")
+
+
+def get_vec_len(buffer):
+    """Return the length of a vector consumed from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#vectors%E2%91%A2
+    return read_uint(buffer, 32)
+
+
+def read_uint(buffer, bits):
+    """Read an unsigned integer stored in LEB128 format."""
+    # https://www.w3.org/TR/wasm-core-1/#integers%E2%91%A4
+    consumed_bytes = 0
+    result = 0
+    shift = 0
+
+    try:
+        while True:
+            byte = buffer.read(1)[0]
+            consumed_bytes += 1
+            assert consumed_bytes <= math.ceil(bits / 7)
+            result |= (byte & 127) << shift
+            if not byte >> 7:
+                break
+
+            shift += 7
+
+    except (AssertionError, IndexError):
+        raise TypeError("Invalid integer.")
+
+    return result
+
+
+def read_sint(buffer, bits):
+    """Read a signed integer stored in LEB128 format."""
+    # https://www.w3.org/TR/wasm-core-1/#integers%E2%91%A4
+    try:
+        byte = buffer.read(1)[0]
+        consumed_bytes = 1
+        result = byte & 127
+        shift = 7
+        while byte >> 7:
+            byte = buffer.read(1)[0]
+            consumed_bytes += 1
+            assert consumed_bytes <= math.ceil(bits / 7)
+            result |= (byte & 127) << shift
+            shift += 7
+
+    except (AssertionError, IndexError):
+        raise TypeError("Invalid integer.")
+
+    if result >> consumed_bytes * 7 - 1:
+        result |= ~0 << shift
+
+    return result
+
+
+def read_f32(buffer):
+    """Read a single precision float from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#floating-point%E2%91%A4
+    return f32.unpack(buffer.read(4))
+
+
+def read_f64(buffer):
+    """Read a double precision float from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#floating-point%E2%91%A4
+    return f64.unpack(buffer.read(8))
+
+
+def read_name(buffer):
+    """Read a name from buffer."""
+    # https://www.w3.org/TR/wasm-core-1/#names%E2%91%A2
+    return buffer.read(get_vec_len(buffer)).decode("utf-8")
```

