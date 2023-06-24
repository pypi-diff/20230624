# Comparing `tmp/cdk-extensions-0.0.81.tar.gz` & `tmp/cdk-extensions-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.81.tar", last modified: Wed Jun 21 13:35:11 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.82.tar", last modified: Sat Jun 24 04:06:34 2023, max compression
```

## Comparing `cdk-extensions-0.0.81.tar` & `cdk-extensions-0.0.82.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.314112 cdk-extensions-0.0.81/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.314112 cdk-extensions-0.0.81/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1761984 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/_jsii/cdk-extensions@0.0.81.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/alerting/
--rw-r--r--   0 runner    (1001) docker     (123)   316954 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/alerting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702329 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   278700 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    97141 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507542 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140877 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692580 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.322112 cdk-extensions-0.0.81/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42369 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)    39153 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/resourcegroups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215413 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130474 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58286 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.326112 cdk-extensions-0.0.81/src/cdk_extensions/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-06-21 13:34:59.000000 cdk-extensions-0.0.81/src/cdk_extensions/stepfunctions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:11.318112 cdk-extensions-0.0.81/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-21 13:35:11.000000 cdk-extensions-0.0.81/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-21 13:35:11.000000 cdk-extensions-0.0.81/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:35:11.000000 cdk-extensions-0.0.81/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 13:35:11.000000 cdk-extensions-0.0.81/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 13:35:11.000000 cdk-extensions-0.0.81/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.072998 cdk-extensions-0.0.82/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.076998 cdk-extensions-0.0.82/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.076998 cdk-extensions-0.0.82/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.076998 cdk-extensions-0.0.82/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1776786 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/_jsii/cdk-extensions@0.0.82.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.076998 cdk-extensions-0.0.82/src/cdk_extensions/alerting/
+-rw-r--r--   0 runner    (1001) docker     (123)   342439 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/alerting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.076998 cdk-extensions-0.0.82/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702329 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   278700 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    97141 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507542 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140877 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692580 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.080998 cdk-extensions-0.0.82/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42369 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)    39153 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/resourcegroups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215413 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130474 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58286 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.084998 cdk-extensions-0.0.82/src/cdk_extensions/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-06-24 04:06:20.000000 cdk-extensions-0.0.82/src/cdk_extensions/stepfunctions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:06:34.076998 cdk-extensions-0.0.82/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-24 04:06:34.000000 cdk-extensions-0.0.82/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-24 04:06:34.000000 cdk-extensions-0.0.82/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:06:34.000000 cdk-extensions-0.0.82/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 04:06:34.000000 cdk-extensions-0.0.82/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 04:06:34.000000 cdk-extensions-0.0.82/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.81/LICENSE` & `cdk-extensions-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/PKG-INFO` & `cdk-extensions-0.0.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.81
+Version: 0.0.82
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.81/README.md` & `cdk-extensions-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/setup.py` & `cdk-extensions-0.0.82/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.81",
+    "version": "0.0.82",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -46,15 +46,15 @@
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks",
         "cdk_extensions.stepfunctions"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.81.jsii.tgz"
+            "cdk-extensions@0.0.82.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/alerting/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/alerting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,14 +366,62 @@
 
     def __repr__(self) -> str:
         return "DescriptionBuilderSectionProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="cdk-extensions.alerting.DiscordOverrideOptions",
+    jsii_struct_bases=[],
+    name_mapping={"channel": "channel", "mentions": "mentions"},
+)
+class DiscordOverrideOptions:
+    def __init__(
+        self,
+        *,
+        channel: typing.Optional[builtins.str] = None,
+        mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+    ) -> None:
+        '''
+        :param channel: 
+        :param mentions: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__253bd589f4b779840486be7096aa59433e6c2634024583dedc1e45fa90aefc20)
+            check_type(argname="argument channel", value=channel, expected_type=type_hints["channel"])
+            check_type(argname="argument mentions", value=mentions, expected_type=type_hints["mentions"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if channel is not None:
+            self._values["channel"] = channel
+        if mentions is not None:
+            self._values["mentions"] = mentions
+
+    @builtins.property
+    def channel(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("channel")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def mentions(self) -> typing.Optional[typing.List[builtins.str]]:
+        result = self._values.get("mentions")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DiscordOverrideOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class EcrImageScanSeverity(
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-extensions.alerting.EcrImageScanSeverity",
 ):
     @jsii.member(jsii_name="of")
     @builtins.classmethod
     def of(
@@ -1197,14 +1245,68 @@
 class IssueHander(
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-extensions.alerting.IssueHander",
 ):
     def __init__(self) -> None:
         jsii.create(self.__class__, self, [])
 
+    @jsii.member(jsii_name="discord")
+    @builtins.classmethod
+    def discord(
+        cls,
+        scope: _constructs_77d1e7e8.IConstruct,
+        id: builtins.str,
+        *,
+        channel: builtins.str,
+        token: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+        event_bus: typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus] = None,
+        mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+        name: typing.Optional[builtins.str] = None,
+        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        logging: typing.Optional[typing.Union["StateMachineLogging", typing.Dict[builtins.str, typing.Any]]] = None,
+        account: typing.Optional[builtins.str] = None,
+        environment_from_arn: typing.Optional[builtins.str] = None,
+        physical_name: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+    ) -> "Discord":
+        '''
+        :param scope: -
+        :param id: -
+        :param channel: 
+        :param token: 
+        :param event_bus: 
+        :param mentions: 
+        :param name: 
+        :param timeout: 
+        :param logging: 
+        :param account: The AWS account ID this resource belongs to. Default: - the resource is in the same account as the stack it belongs to
+        :param environment_from_arn: ARN to deduce region and account from. The ARN is parsed and the account and region are taken from the ARN. This should be used for imported resources. Cannot be supplied together with either ``account`` or ``region``. Default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        :param physical_name: The value passed in by users to the physical name prop of the resource. - ``undefined`` implies that a physical name will be allocated by CloudFormation during deployment. - a concrete value implies a specific physical name - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation. Default: - The physical name will be allocated by CloudFormation at deployment time
+        :param region: The AWS region this resource belongs to. Default: - the resource is in the same region as the stack it belongs to
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f869ab3c2616a04b67f30bb9166b3c542397e1994c482091441b40066447005e)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = DiscordProps(
+            channel=channel,
+            token=token,
+            event_bus=event_bus,
+            mentions=mentions,
+            name=name,
+            timeout=timeout,
+            logging=logging,
+            account=account,
+            environment_from_arn=environment_from_arn,
+            physical_name=physical_name,
+            region=region,
+        )
+
+        return typing.cast("Discord", jsii.sinvoke(cls, "discord", [scope, id, props]))
+
     @jsii.member(jsii_name="jiraTicket")
     @builtins.classmethod
     def jira_ticket(
         cls,
         scope: _constructs_77d1e7e8.IConstruct,
         id: builtins.str,
         *,
@@ -4385,14 +4487,371 @@
 
     @builtins.property
     @jsii.member(jsii_name="title")
     def title(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "title"))
 
 
+@jsii.implements(IIssueHandler)
+class Discord(
+    IssuePluginBase,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="cdk-extensions.alerting.Discord",
+):
+    '''A standardized implementation that allows Discord messages to be sent in response to events detected in AWS.
+
+    Intended for use with the ``IssueManager`` state machine which allows
+    arbitrary types of events to be processed into standard values and then
+    output or one of more issue tracking services.
+    '''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.IConstruct,
+        id: builtins.str,
+        *,
+        channel: builtins.str,
+        token: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+        event_bus: typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus] = None,
+        mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+        name: typing.Optional[builtins.str] = None,
+        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        logging: typing.Optional[typing.Union[StateMachineLogging, typing.Dict[builtins.str, typing.Any]]] = None,
+        account: typing.Optional[builtins.str] = None,
+        environment_from_arn: typing.Optional[builtins.str] = None,
+        physical_name: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''Creates a new instance of the JiraTicket class.
+
+        :param scope: A CDK Construct that will serve as this resource's parent in the construct tree.
+        :param id: A name to be associated with the stack and used in resource naming. Must be unique within the context of 'scope'.
+        :param channel: 
+        :param token: 
+        :param event_bus: 
+        :param mentions: 
+        :param name: 
+        :param timeout: 
+        :param logging: 
+        :param account: The AWS account ID this resource belongs to. Default: - the resource is in the same account as the stack it belongs to
+        :param environment_from_arn: ARN to deduce region and account from. The ARN is parsed and the account and region are taken from the ARN. This should be used for imported resources. Cannot be supplied together with either ``account`` or ``region``. Default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        :param physical_name: The value passed in by users to the physical name prop of the resource. - ``undefined`` implies that a physical name will be allocated by CloudFormation during deployment. - a concrete value implies a specific physical name - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation. Default: - The physical name will be allocated by CloudFormation at deployment time
+        :param region: The AWS region this resource belongs to. Default: - the resource is in the same region as the stack it belongs to
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fb4e198a320ebbe55fb811ad6494b480b2e2697eeedb57f725f878668c229625)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = DiscordProps(
+            channel=channel,
+            token=token,
+            event_bus=event_bus,
+            mentions=mentions,
+            name=name,
+            timeout=timeout,
+            logging=logging,
+            account=account,
+            environment_from_arn=environment_from_arn,
+            physical_name=physical_name,
+            region=region,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="buildEventOverrides")
+    def build_event_overrides(
+        self,
+        *,
+        channel: typing.Optional[builtins.str] = None,
+        mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+    ) -> IssueHandlerOverride:
+        '''
+        :param channel: 
+        :param mentions: 
+        '''
+        options = DiscordOverrideOptions(channel=channel, mentions=mentions)
+
+        return typing.cast(IssueHandlerOverride, jsii.invoke(self, "buildEventOverrides", [options]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="DEFAULT_NAME")
+    def DEFAULT_NAME(cls) -> builtins.str:
+        return typing.cast(builtins.str, jsii.sget(cls, "DEFAULT_NAME"))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="MESSAGES_ENDPOINT")
+    def MESSAGES_ENDPOINT(cls) -> builtins.str:
+        return typing.cast(builtins.str, jsii.sget(cls, "MESSAGES_ENDPOINT"))
+
+    @builtins.property
+    @jsii.member(jsii_name="apiDestination")
+    def api_destination(self) -> _aws_cdk_aws_events_ceddda9d.ApiDestination:
+        '''Destination pointing to a Jira instance where tickets are to be created.'''
+        return typing.cast(_aws_cdk_aws_events_ceddda9d.ApiDestination, jsii.get(self, "apiDestination"))
+
+    @builtins.property
+    @jsii.member(jsii_name="channel")
+    def channel(self) -> builtins.str:
+        '''The default Discord channel where messages processed by the handler should be sent if no override is given.
+
+        :group: Inputs
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "channel"))
+
+    @builtins.property
+    @jsii.member(jsii_name="connection")
+    def connection(self) -> _aws_cdk_aws_events_ceddda9d.Connection:
+        '''API connection providing details of how to communicate with the configured Jira instance.'''
+        return typing.cast(_aws_cdk_aws_events_ceddda9d.Connection, jsii.get(self, "connection"))
+
+    @builtins.property
+    @jsii.member(jsii_name="handler")
+    def handler(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.IStateMachine:
+        '''The State Machine that handles creating a Jira ticket for a passed issue.
+
+        Internally this state machine uses the AWS managed ``AWS-CreateJiraIssue``
+        SSM Automation document.
+
+        :group: Resources
+        '''
+        return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.IStateMachine, jsii.get(self, "handler"))
+
+    @builtins.property
+    @jsii.member(jsii_name="mentions")
+    def mentions(self) -> typing.List[builtins.str]:
+        '''Collection of users or roles who should be mentioned by default when sending a message to Discord.'''
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "mentions"))
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        '''The human friendly name that can be used to identify the plugin.
+
+        :group: Inputs
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "name"))
+
+    @builtins.property
+    @jsii.member(jsii_name="token")
+    def token(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
+        '''The token for a Discord bot that has permissions to post in the destination channels.
+
+        The secret should be in JSON format and contain the
+        key:
+
+        token: The token for the bot that has permissions to post in the
+        destination Discord channels.
+
+        :group: Inputs
+        '''
+        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, jsii.get(self, "token"))
+
+    @builtins.property
+    @jsii.member(jsii_name="eventBus")
+    def event_bus(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus]:
+        '''The event bus to use to trigger writes to the Jira instance.
+
+        This integration formats a Jira API response and then sends it to a Jira
+        instance by means of an EventBridge Destination API and a specially
+        crafted event pattern. This is the event bus where the rule to trigger the
+        API will be added and the trigger event will be sent.
+        '''
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus], jsii.get(self, "eventBus"))
+
+    @builtins.property
+    @jsii.member(jsii_name="timeout")
+    def timeout(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''The length of time that the State Machine that handles creation of Jira tickets is allowed to run before timing out.
+
+        :group: Inputs
+        '''
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], jsii.get(self, "timeout"))
+
+
+@jsii.data_type(
+    jsii_type="cdk-extensions.alerting.DiscordProps",
+    jsii_struct_bases=[IssuePluginBaseProps],
+    name_mapping={
+        "account": "account",
+        "environment_from_arn": "environmentFromArn",
+        "physical_name": "physicalName",
+        "region": "region",
+        "logging": "logging",
+        "channel": "channel",
+        "token": "token",
+        "event_bus": "eventBus",
+        "mentions": "mentions",
+        "name": "name",
+        "timeout": "timeout",
+    },
+)
+class DiscordProps(IssuePluginBaseProps):
+    def __init__(
+        self,
+        *,
+        account: typing.Optional[builtins.str] = None,
+        environment_from_arn: typing.Optional[builtins.str] = None,
+        physical_name: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+        logging: typing.Optional[typing.Union[StateMachineLogging, typing.Dict[builtins.str, typing.Any]]] = None,
+        channel: builtins.str,
+        token: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+        event_bus: typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus] = None,
+        mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+        name: typing.Optional[builtins.str] = None,
+        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    ) -> None:
+        '''Configuration controlling how Discord messages should be sent in response to events.
+
+        :param account: The AWS account ID this resource belongs to. Default: - the resource is in the same account as the stack it belongs to
+        :param environment_from_arn: ARN to deduce region and account from. The ARN is parsed and the account and region are taken from the ARN. This should be used for imported resources. Cannot be supplied together with either ``account`` or ``region``. Default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        :param physical_name: The value passed in by users to the physical name prop of the resource. - ``undefined`` implies that a physical name will be allocated by CloudFormation during deployment. - a concrete value implies a specific physical name - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation. Default: - The physical name will be allocated by CloudFormation at deployment time
+        :param region: The AWS region this resource belongs to. Default: - the resource is in the same region as the stack it belongs to
+        :param logging: 
+        :param channel: 
+        :param token: 
+        :param event_bus: 
+        :param mentions: 
+        :param name: 
+        :param timeout: 
+        '''
+        if isinstance(logging, dict):
+            logging = StateMachineLogging(**logging)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__29753140d336d671dafb38ed6d56c41ca40aba29a1c30d7d247039c3e7a19497)
+            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
+            check_type(argname="argument environment_from_arn", value=environment_from_arn, expected_type=type_hints["environment_from_arn"])
+            check_type(argname="argument physical_name", value=physical_name, expected_type=type_hints["physical_name"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
+            check_type(argname="argument channel", value=channel, expected_type=type_hints["channel"])
+            check_type(argname="argument token", value=token, expected_type=type_hints["token"])
+            check_type(argname="argument event_bus", value=event_bus, expected_type=type_hints["event_bus"])
+            check_type(argname="argument mentions", value=mentions, expected_type=type_hints["mentions"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "channel": channel,
+            "token": token,
+        }
+        if account is not None:
+            self._values["account"] = account
+        if environment_from_arn is not None:
+            self._values["environment_from_arn"] = environment_from_arn
+        if physical_name is not None:
+            self._values["physical_name"] = physical_name
+        if region is not None:
+            self._values["region"] = region
+        if logging is not None:
+            self._values["logging"] = logging
+        if event_bus is not None:
+            self._values["event_bus"] = event_bus
+        if mentions is not None:
+            self._values["mentions"] = mentions
+        if name is not None:
+            self._values["name"] = name
+        if timeout is not None:
+            self._values["timeout"] = timeout
+
+    @builtins.property
+    def account(self) -> typing.Optional[builtins.str]:
+        '''The AWS account ID this resource belongs to.
+
+        :default: - the resource is in the same account as the stack it belongs to
+        '''
+        result = self._values.get("account")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def environment_from_arn(self) -> typing.Optional[builtins.str]:
+        '''ARN to deduce region and account from.
+
+        The ARN is parsed and the account and region are taken from the ARN.
+        This should be used for imported resources.
+
+        Cannot be supplied together with either ``account`` or ``region``.
+
+        :default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        '''
+        result = self._values.get("environment_from_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def physical_name(self) -> typing.Optional[builtins.str]:
+        '''The value passed in by users to the physical name prop of the resource.
+
+        - ``undefined`` implies that a physical name will be allocated by
+          CloudFormation during deployment.
+        - a concrete value implies a specific physical name
+        - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated
+          by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation.
+
+        :default: - The physical name will be allocated by CloudFormation at deployment time
+        '''
+        result = self._values.get("physical_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def region(self) -> typing.Optional[builtins.str]:
+        '''The AWS region this resource belongs to.
+
+        :default: - the resource is in the same region as the stack it belongs to
+        '''
+        result = self._values.get("region")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def logging(self) -> typing.Optional[StateMachineLogging]:
+        result = self._values.get("logging")
+        return typing.cast(typing.Optional[StateMachineLogging], result)
+
+    @builtins.property
+    def channel(self) -> builtins.str:
+        result = self._values.get("channel")
+        assert result is not None, "Required property 'channel' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def token(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
+        result = self._values.get("token")
+        assert result is not None, "Required property 'token' is missing"
+        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, result)
+
+    @builtins.property
+    def event_bus(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus]:
+        result = self._values.get("event_bus")
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus], result)
+
+    @builtins.property
+    def mentions(self) -> typing.Optional[typing.List[builtins.str]]:
+        result = self._values.get("mentions")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def name(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def timeout(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        result = self._values.get("timeout")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DiscordProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.implements(IIssueParser)
 class EcrScanFinding(
     IssuePluginBase,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-extensions.alerting.EcrScanFinding",
 ):
     def __init__(
@@ -5932,14 +6391,17 @@
     "ConfigComplianceChangeRuleOptions",
     "DescriptionBuilder",
     "DescriptionBuilderIterator",
     "DescriptionBuilderIteratorProps",
     "DescriptionBuilderProps",
     "DescriptionBuilderSection",
     "DescriptionBuilderSectionProps",
+    "Discord",
+    "DiscordOverrideOptions",
+    "DiscordProps",
     "EcrImageScanSeverity",
     "EcrImageScanSeverityConfiguration",
     "EcrScanFinding",
     "EcrScanFindingEventOptions",
     "EcrScanFindingProps",
     "GuardDutyFinding",
     "GuardDutyFindingProps",
@@ -6036,14 +6498,22 @@
     *,
     title: builtins.str,
     reference_checks: typing.Optional[typing.Sequence[builtins.str]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__253bd589f4b779840486be7096aa59433e6c2634024583dedc1e45fa90aefc20(
+    *,
+    channel: typing.Optional[builtins.str] = None,
+    mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__74d0339c6d2e7f75b5fad2a1cd75c3f1c5bb5fedaae0d185457222fa11329e56(
     name: builtins.str,
     priority: jsii.Number,
     standardized: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -6183,14 +6653,33 @@
 
 def _typecheckingstub__add09d93d064fe5f98082939df59303379ccf56d73870b39e6b320fedfe6964d(
     path: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__f869ab3c2616a04b67f30bb9166b3c542397e1994c482091441b40066447005e(
+    scope: _constructs_77d1e7e8.IConstruct,
+    id: builtins.str,
+    *,
+    channel: builtins.str,
+    token: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    event_bus: typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus] = None,
+    mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+    name: typing.Optional[builtins.str] = None,
+    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    logging: typing.Optional[typing.Union[StateMachineLogging, typing.Dict[builtins.str, typing.Any]]] = None,
+    account: typing.Optional[builtins.str] = None,
+    environment_from_arn: typing.Optional[builtins.str] = None,
+    physical_name: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__bc82eedaec69377fec470cfcf06b82e1b425e2a8c85b604da5b7375421112d61(
     scope: _constructs_77d1e7e8.IConstruct,
     id: builtins.str,
     *,
     credentials: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
     issue_type: builtins.str,
     jira_url: builtins.str,
@@ -6858,14 +7347,50 @@
     prefix: typing.Optional[builtins.str] = None,
     required: typing.Optional[builtins.bool] = None,
     suffix: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__fb4e198a320ebbe55fb811ad6494b480b2e2697eeedb57f725f878668c229625(
+    scope: _constructs_77d1e7e8.IConstruct,
+    id: builtins.str,
+    *,
+    channel: builtins.str,
+    token: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    event_bus: typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus] = None,
+    mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+    name: typing.Optional[builtins.str] = None,
+    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    logging: typing.Optional[typing.Union[StateMachineLogging, typing.Dict[builtins.str, typing.Any]]] = None,
+    account: typing.Optional[builtins.str] = None,
+    environment_from_arn: typing.Optional[builtins.str] = None,
+    physical_name: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__29753140d336d671dafb38ed6d56c41ca40aba29a1c30d7d247039c3e7a19497(
+    *,
+    account: typing.Optional[builtins.str] = None,
+    environment_from_arn: typing.Optional[builtins.str] = None,
+    physical_name: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+    logging: typing.Optional[typing.Union[StateMachineLogging, typing.Dict[builtins.str, typing.Any]]] = None,
+    channel: builtins.str,
+    token: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    event_bus: typing.Optional[_aws_cdk_aws_events_ceddda9d.IEventBus] = None,
+    mentions: typing.Optional[typing.Sequence[builtins.str]] = None,
+    name: typing.Optional[builtins.str] = None,
+    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__73bcbf64ab813f7e2495560494a57d70b4d06ec8af196d2201175402c96def41(
     scope: _constructs_77d1e7e8.IConstruct,
     id: builtins.str,
     *,
     match_type: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
```

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/resourcegroups/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/resourcegroups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions/stepfunctions/__init__.py` & `cdk-extensions-0.0.82/src/cdk_extensions/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.82/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.81
+Version: 0.0.82
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.81/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.82/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.81.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.82.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/alerting/__init__.py
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
```

