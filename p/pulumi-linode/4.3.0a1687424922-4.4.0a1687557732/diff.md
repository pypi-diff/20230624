# Comparing `tmp/pulumi_linode-4.3.0a1687424922.tar.gz` & `tmp/pulumi_linode-4.4.0a1687557732.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_linode-4.3.0a1687424922.tar", last modified: Thu Jun 22 09:14:54 2023, max compression
+gzip compressed data, was "pulumi_linode-4.4.0a1687557732.tar", last modified: Fri Jun 23 22:07:50 2023, max compression
```

## Comparing `pulumi_linode-4.3.0a1687424922.tar` & `pulumi_linode-4.4.0a1687557732.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.986074 pulumi_linode-4.3.0a1687424922/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/pulumi_linode/
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134820 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/account_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/pulumi_linode/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/database_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_zonefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_linode_object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_networking_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_vlans.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/image.py
--rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_shared_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_object.py
--rw-r--r--   0 runner    (1001) docker     (123)   257564 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/rdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:14:53.986074 pulumi_linode-4.3.0a1687424922/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:07:50.859901 pulumi_linode-4.4.0a1687557732/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-23 22:07:50.859901 pulumi_linode-4.4.0a1687557732/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:07:50.855901 pulumi_linode-4.4.0a1687557732/pulumi_linode/
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178907 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/account_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:07:50.855901 pulumi_linode-4.4.0a1687557732/pulumi_linode/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/database_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/firewall_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_mysql_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_domain_zonefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_linode_object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_lke_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_networking_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_stack_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/instance_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/instance_shared_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/object_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/object_storage_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)   258855 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:07:50.855901 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:07:50.859901 pulumi_linode-4.4.0a1687557732/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-23 22:07:50.000000 pulumi_linode-4.4.0a1687557732/setup.py
```

### Comparing `pulumi_linode-4.3.0a1687424922/PKG-INFO` & `pulumi_linode-4.4.0a1687557732/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_linode
-Version: 4.3.0a1687424922
+Version: 4.4.0a1687557732
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.3.0a1687424922/README.md` & `pulumi_linode-4.4.0a1687557732/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/__init__.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/_inputs.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/_inputs.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,34 +51,49 @@
     'UserImageGrantArgs',
     'UserLinodeGrantArgs',
     'UserLongviewGrantArgs',
     'UserNodebalancerGrantArgs',
     'UserStackscriptGrantArgs',
     'UserVolumeGrantArgs',
     'GetAccountLoginsFilterArgs',
+    'GetAccountLoginsLoginArgs',
+    'GetDatabaseBackupsBackupArgs',
     'GetDatabaseBackupsFilterArgs',
+    'GetDatabaseEnginesEngineArgs',
     'GetDatabaseEnginesFilterArgs',
     'GetDatabaseMysqlBackupsFilterArgs',
+    'GetDatabasesDatabaseArgs',
     'GetDatabasesFilterArgs',
     'GetImagesFilterArgs',
+    'GetImagesImageArgs',
     'GetInstanceTypesFilterArgs',
+    'GetInstanceTypesTypeArgs',
+    'GetInstanceTypesTypeAddonArgs',
+    'GetInstanceTypesTypeAddonBackupArgs',
+    'GetInstanceTypesTypeAddonBackupPriceArgs',
+    'GetInstanceTypesTypePriceArgs',
     'GetInstancesFilterArgs',
+    'GetRegionResolverArgs',
     'GetRegionsFilterArgs',
     'GetRegionsRegionArgs',
     'GetRegionsRegionResolverArgs',
     'GetStackScriptsFilterArgs',
+    'GetStackScriptsStackscriptArgs',
+    'GetStackScriptsStackscriptUserDefinedFieldArgs',
+    'GetUserDatabaseGrantArgs',
     'GetUserDomainGrantArgs',
     'GetUserFirewallGrantArgs',
     'GetUserImageGrantArgs',
     'GetUserLinodeGrantArgs',
     'GetUserLongviewGrantArgs',
     'GetUserNodebalancerGrantArgs',
     'GetUserStackscriptGrantArgs',
     'GetUserVolumeGrantArgs',
     'GetVlansFilterArgs',
+    'GetVlansVlanArgs',
 ]
 
 @pulumi.input_type
 class DatabaseMysqlUpdatesArgs:
     def __init__(__self__, *,
                  day_of_week: pulumi.Input[str],
                  duration: pulumi.Input[int],
@@ -2847,14 +2862,174 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetAccountLoginsLoginArgs:
+    def __init__(__self__, *,
+                 datetime: str,
+                 id: int,
+                 ip: str,
+                 restricted: bool,
+                 status: str,
+                 username: str):
+        """
+        :param str datetime: When the login was initiated.
+        :param int id: The unique ID of this login object.
+        :param str ip: The remote IP address that requested the login.
+        :param bool restricted: True if the User that was logged into was a restricted User, false otherwise.
+        :param str username: The username of the User that was logged into.
+        """
+        pulumi.set(__self__, "datetime", datetime)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "ip", ip)
+        pulumi.set(__self__, "restricted", restricted)
+        pulumi.set(__self__, "status", status)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def datetime(self) -> str:
+        """
+        When the login was initiated.
+        """
+        return pulumi.get(self, "datetime")
+
+    @datetime.setter
+    def datetime(self, value: str):
+        pulumi.set(self, "datetime", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        """
+        The unique ID of this login object.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: int):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def ip(self) -> str:
+        """
+        The remote IP address that requested the login.
+        """
+        return pulumi.get(self, "ip")
+
+    @ip.setter
+    def ip(self, value: str):
+        pulumi.set(self, "ip", value)
+
+    @property
+    @pulumi.getter
+    def restricted(self) -> bool:
+        """
+        True if the User that was logged into was a restricted User, false otherwise.
+        """
+        return pulumi.get(self, "restricted")
+
+    @restricted.setter
+    def restricted(self, value: bool):
+        pulumi.set(self, "restricted", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: str):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        The username of the User that was logged into.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: str):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class GetDatabaseBackupsBackupArgs:
+    def __init__(__self__, *,
+                 created: str,
+                 id: int,
+                 label: str,
+                 type: str):
+        """
+        :param str created: A time value given in a combined date and time format that represents when the database backup was created.
+        :param int id: The ID of the database backup object.
+        :param str label: The database backup’s label, for display purposes only.
+        :param str type: The type of database backup, determined by how the backup was created.
+        """
+        pulumi.set(__self__, "created", created)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def created(self) -> str:
+        """
+        A time value given in a combined date and time format that represents when the database backup was created.
+        """
+        return pulumi.get(self, "created")
+
+    @created.setter
+    def created(self, value: str):
+        pulumi.set(self, "created", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        """
+        The ID of the database backup object.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: int):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        The database backup’s label, for display purposes only.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The type of database backup, determined by how the backup was created.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: str):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
 class GetDatabaseBackupsFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by.
@@ -2900,14 +3075,66 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetDatabaseEnginesEngineArgs:
+    def __init__(__self__, *,
+                 engine: str,
+                 id: str,
+                 version: str):
+        """
+        :param str engine: The Managed Database engine type.
+        :param str id: The Managed Database engine ID in engine/version format.
+        :param str version: The Managed Database engine version.
+        """
+        pulumi.set(__self__, "engine", engine)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def engine(self) -> str:
+        """
+        The Managed Database engine type.
+        """
+        return pulumi.get(self, "engine")
+
+    @engine.setter
+    def engine(self, value: str):
+        pulumi.set(self, "engine", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The Managed Database engine ID in engine/version format.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: str):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        """
+        The Managed Database engine version.
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: str):
+        pulumi.set(self, "version", value)
+
+
+@pulumi.input_type
 class GetDatabaseEnginesFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by.
@@ -3006,14 +3233,272 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetDatabasesDatabaseArgs:
+    def __init__(__self__, *,
+                 allow_lists: Sequence[str],
+                 cluster_size: int,
+                 created: str,
+                 encrypted: bool,
+                 engine: str,
+                 host_primary: str,
+                 host_secondary: str,
+                 id: int,
+                 instance_uri: str,
+                 label: str,
+                 region: str,
+                 replication_type: str,
+                 ssl_connection: bool,
+                 status: str,
+                 type: str,
+                 updated: str,
+                 version: str):
+        """
+        :param Sequence[str] allow_lists: A list of IP addresses that can access the Managed Database.
+        :param int cluster_size: The number of Linode Instance nodes deployed to the Managed Database.
+        :param str created: When this Managed Database was created.
+        :param bool encrypted: Whether the Managed Databases is encrypted.
+        :param str engine: The Managed Database engine.
+        :param str host_primary: The primary host for the Managed Database.
+        :param str host_secondary: The secondary/private network host for the Managed Database.
+        :param int id: The ID of the Managed Database.
+        :param str label: A unique, user-defined string referring to the Managed Database.
+        :param str region: The region to use for the Managed Database.
+        :param str replication_type: The replication method used for the Managed Database.
+        :param bool ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database.
+        :param str status: The operating status of the Managed Database.
+        :param str type: The Linode Instance type used for the nodes of the  Managed Database instance.
+        :param str updated: When this Managed Database was last updated.
+        :param str version: The Managed Database engine version.
+        """
+        pulumi.set(__self__, "allow_lists", allow_lists)
+        pulumi.set(__self__, "cluster_size", cluster_size)
+        pulumi.set(__self__, "created", created)
+        pulumi.set(__self__, "encrypted", encrypted)
+        pulumi.set(__self__, "engine", engine)
+        pulumi.set(__self__, "host_primary", host_primary)
+        pulumi.set(__self__, "host_secondary", host_secondary)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "instance_uri", instance_uri)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "replication_type", replication_type)
+        pulumi.set(__self__, "ssl_connection", ssl_connection)
+        pulumi.set(__self__, "status", status)
+        pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "updated", updated)
+        pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter(name="allowLists")
+    def allow_lists(self) -> Sequence[str]:
+        """
+        A list of IP addresses that can access the Managed Database.
+        """
+        return pulumi.get(self, "allow_lists")
+
+    @allow_lists.setter
+    def allow_lists(self, value: Sequence[str]):
+        pulumi.set(self, "allow_lists", value)
+
+    @property
+    @pulumi.getter(name="clusterSize")
+    def cluster_size(self) -> int:
+        """
+        The number of Linode Instance nodes deployed to the Managed Database.
+        """
+        return pulumi.get(self, "cluster_size")
+
+    @cluster_size.setter
+    def cluster_size(self, value: int):
+        pulumi.set(self, "cluster_size", value)
+
+    @property
+    @pulumi.getter
+    def created(self) -> str:
+        """
+        When this Managed Database was created.
+        """
+        return pulumi.get(self, "created")
+
+    @created.setter
+    def created(self, value: str):
+        pulumi.set(self, "created", value)
+
+    @property
+    @pulumi.getter
+    def encrypted(self) -> bool:
+        """
+        Whether the Managed Databases is encrypted.
+        """
+        return pulumi.get(self, "encrypted")
+
+    @encrypted.setter
+    def encrypted(self, value: bool):
+        pulumi.set(self, "encrypted", value)
+
+    @property
+    @pulumi.getter
+    def engine(self) -> str:
+        """
+        The Managed Database engine.
+        """
+        return pulumi.get(self, "engine")
+
+    @engine.setter
+    def engine(self, value: str):
+        pulumi.set(self, "engine", value)
+
+    @property
+    @pulumi.getter(name="hostPrimary")
+    def host_primary(self) -> str:
+        """
+        The primary host for the Managed Database.
+        """
+        return pulumi.get(self, "host_primary")
+
+    @host_primary.setter
+    def host_primary(self, value: str):
+        pulumi.set(self, "host_primary", value)
+
+    @property
+    @pulumi.getter(name="hostSecondary")
+    def host_secondary(self) -> str:
+        """
+        The secondary/private network host for the Managed Database.
+        """
+        return pulumi.get(self, "host_secondary")
+
+    @host_secondary.setter
+    def host_secondary(self, value: str):
+        pulumi.set(self, "host_secondary", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        """
+        The ID of the Managed Database.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: int):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter(name="instanceUri")
+    def instance_uri(self) -> str:
+        return pulumi.get(self, "instance_uri")
+
+    @instance_uri.setter
+    def instance_uri(self, value: str):
+        pulumi.set(self, "instance_uri", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        A unique, user-defined string referring to the Managed Database.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        """
+        The region to use for the Managed Database.
+        """
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: str):
+        pulumi.set(self, "region", value)
+
+    @property
+    @pulumi.getter(name="replicationType")
+    def replication_type(self) -> str:
+        """
+        The replication method used for the Managed Database.
+        """
+        return pulumi.get(self, "replication_type")
+
+    @replication_type.setter
+    def replication_type(self, value: str):
+        pulumi.set(self, "replication_type", value)
+
+    @property
+    @pulumi.getter(name="sslConnection")
+    def ssl_connection(self) -> bool:
+        """
+        Whether to require SSL credentials to establish a connection to the Managed Database.
+        """
+        return pulumi.get(self, "ssl_connection")
+
+    @ssl_connection.setter
+    def ssl_connection(self, value: bool):
+        pulumi.set(self, "ssl_connection", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        """
+        The operating status of the Managed Database.
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: str):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The Linode Instance type used for the nodes of the  Managed Database instance.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: str):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter
+    def updated(self) -> str:
+        """
+        When this Managed Database was last updated.
+        """
+        return pulumi.get(self, "updated")
+
+    @updated.setter
+    def updated(self, value: str):
+        pulumi.set(self, "updated", value)
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        """
+        The Managed Database engine version.
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: str):
+        pulumi.set(self, "version", value)
+
+
+@pulumi.input_type
 class GetDatabasesFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by.
@@ -3112,14 +3597,197 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetImagesImageArgs:
+    def __init__(__self__, *,
+                 created: str,
+                 created_by: str,
+                 deprecated: bool,
+                 description: str,
+                 expiry: str,
+                 id: str,
+                 is_public: bool,
+                 label: str,
+                 size: int,
+                 status: str,
+                 type: str,
+                 vendor: str):
+        """
+        :param str created: When this Image was created.
+        :param str created_by: The name of the User who created this Image, or "linode" for official Images.
+        :param bool deprecated: Whether or not this Image is deprecated. Will only be true for deprecated public Images.
+        :param str description: A detailed description of this Image.
+        :param str id: The unique ID of this Image.  The ID of private images begin with `private/` followed by the numeric identifier of the private image, for example `private/12345`.
+        :param bool is_public: True if the Image is public.
+        :param str label: A short description of the Image.
+        :param int size: The minimum size this Image needs to deploy. Size is in MB. example: 2500
+        :param str status: The current status of this image. (`creating`, `pending_upload`, `available`)
+        :param str type: How the Image was created. Manual Images can be created at any time. "Automatic" Images are created automatically from a deleted Linode. (`manual`, `automatic`)
+        :param str vendor: The upstream distribution vendor. `None` for private Images.
+        """
+        pulumi.set(__self__, "created", created)
+        pulumi.set(__self__, "created_by", created_by)
+        pulumi.set(__self__, "deprecated", deprecated)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "expiry", expiry)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "is_public", is_public)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "size", size)
+        pulumi.set(__self__, "status", status)
+        pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "vendor", vendor)
+
+    @property
+    @pulumi.getter
+    def created(self) -> str:
+        """
+        When this Image was created.
+        """
+        return pulumi.get(self, "created")
+
+    @created.setter
+    def created(self, value: str):
+        pulumi.set(self, "created", value)
+
+    @property
+    @pulumi.getter(name="createdBy")
+    def created_by(self) -> str:
+        """
+        The name of the User who created this Image, or "linode" for official Images.
+        """
+        return pulumi.get(self, "created_by")
+
+    @created_by.setter
+    def created_by(self, value: str):
+        pulumi.set(self, "created_by", value)
+
+    @property
+    @pulumi.getter
+    def deprecated(self) -> bool:
+        """
+        Whether or not this Image is deprecated. Will only be true for deprecated public Images.
+        """
+        return pulumi.get(self, "deprecated")
+
+    @deprecated.setter
+    def deprecated(self, value: bool):
+        pulumi.set(self, "deprecated", value)
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        A detailed description of this Image.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: str):
+        pulumi.set(self, "description", value)
+
+    @property
+    @pulumi.getter
+    def expiry(self) -> str:
+        return pulumi.get(self, "expiry")
+
+    @expiry.setter
+    def expiry(self, value: str):
+        pulumi.set(self, "expiry", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The unique ID of this Image.  The ID of private images begin with `private/` followed by the numeric identifier of the private image, for example `private/12345`.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: str):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter(name="isPublic")
+    def is_public(self) -> bool:
+        """
+        True if the Image is public.
+        """
+        return pulumi.get(self, "is_public")
+
+    @is_public.setter
+    def is_public(self, value: bool):
+        pulumi.set(self, "is_public", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        A short description of the Image.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def size(self) -> int:
+        """
+        The minimum size this Image needs to deploy. Size is in MB. example: 2500
+        """
+        return pulumi.get(self, "size")
+
+    @size.setter
+    def size(self, value: int):
+        pulumi.set(self, "size", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        """
+        The current status of this image. (`creating`, `pending_upload`, `available`)
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: str):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        How the Image was created. Manual Images can be created at any time. "Automatic" Images are created automatically from a deleted Linode. (`manual`, `automatic`)
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: str):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter
+    def vendor(self) -> str:
+        """
+        The upstream distribution vendor. `None` for private Images.
+        """
+        return pulumi.get(self, "vendor")
+
+    @vendor.setter
+    def vendor(self, value: str):
+        pulumi.set(self, "vendor", value)
+
+
+@pulumi.input_type
 class GetInstanceTypesFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by. See the Filterable Fields section for a complete list of filterable fields.
@@ -3165,14 +3833,249 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetInstanceTypesTypeArgs:
+    def __init__(__self__, *,
+                 addons: Sequence['GetInstanceTypesTypeAddonArgs'],
+                 class_: str,
+                 disk: int,
+                 id: str,
+                 label: str,
+                 memory: int,
+                 network_out: int,
+                 prices: Sequence['GetInstanceTypesTypePriceArgs'],
+                 transfer: int,
+                 vcpus: int):
+        """
+        :param str class_: The class of the Linode Type. See all classes [here](https://www.linode.com/docs/api/linode-types/#type-view__responses).
+        :param int disk: The Disk size, in MB, of the Linode Type.
+        :param str id: The ID representing the Linode Type.
+        :param str label: The Linode Type's label is for display purposes only.
+        :param int memory: The amount of RAM included in this Linode Type.
+        :param int network_out: The Mbits outbound bandwidth allocation.
+        :param int transfer: The monthly outbound transfer amount, in MB.
+        :param int vcpus: The number of VCPU cores this Linode Type offers.
+        """
+        pulumi.set(__self__, "addons", addons)
+        pulumi.set(__self__, "class_", class_)
+        pulumi.set(__self__, "disk", disk)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "memory", memory)
+        pulumi.set(__self__, "network_out", network_out)
+        pulumi.set(__self__, "prices", prices)
+        pulumi.set(__self__, "transfer", transfer)
+        pulumi.set(__self__, "vcpus", vcpus)
+
+    @property
+    @pulumi.getter
+    def addons(self) -> Sequence['GetInstanceTypesTypeAddonArgs']:
+        return pulumi.get(self, "addons")
+
+    @addons.setter
+    def addons(self, value: Sequence['GetInstanceTypesTypeAddonArgs']):
+        pulumi.set(self, "addons", value)
+
+    @property
+    @pulumi.getter(name="class")
+    def class_(self) -> str:
+        """
+        The class of the Linode Type. See all classes [here](https://www.linode.com/docs/api/linode-types/#type-view__responses).
+        """
+        return pulumi.get(self, "class_")
+
+    @class_.setter
+    def class_(self, value: str):
+        pulumi.set(self, "class_", value)
+
+    @property
+    @pulumi.getter
+    def disk(self) -> int:
+        """
+        The Disk size, in MB, of the Linode Type.
+        """
+        return pulumi.get(self, "disk")
+
+    @disk.setter
+    def disk(self, value: int):
+        pulumi.set(self, "disk", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The ID representing the Linode Type.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: str):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        The Linode Type's label is for display purposes only.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def memory(self) -> int:
+        """
+        The amount of RAM included in this Linode Type.
+        """
+        return pulumi.get(self, "memory")
+
+    @memory.setter
+    def memory(self, value: int):
+        pulumi.set(self, "memory", value)
+
+    @property
+    @pulumi.getter(name="networkOut")
+    def network_out(self) -> int:
+        """
+        The Mbits outbound bandwidth allocation.
+        """
+        return pulumi.get(self, "network_out")
+
+    @network_out.setter
+    def network_out(self, value: int):
+        pulumi.set(self, "network_out", value)
+
+    @property
+    @pulumi.getter
+    def prices(self) -> Sequence['GetInstanceTypesTypePriceArgs']:
+        return pulumi.get(self, "prices")
+
+    @prices.setter
+    def prices(self, value: Sequence['GetInstanceTypesTypePriceArgs']):
+        pulumi.set(self, "prices", value)
+
+    @property
+    @pulumi.getter
+    def transfer(self) -> int:
+        """
+        The monthly outbound transfer amount, in MB.
+        """
+        return pulumi.get(self, "transfer")
+
+    @transfer.setter
+    def transfer(self, value: int):
+        pulumi.set(self, "transfer", value)
+
+    @property
+    @pulumi.getter
+    def vcpus(self) -> int:
+        """
+        The number of VCPU cores this Linode Type offers.
+        """
+        return pulumi.get(self, "vcpus")
+
+    @vcpus.setter
+    def vcpus(self, value: int):
+        pulumi.set(self, "vcpus", value)
+
+
+@pulumi.input_type
+class GetInstanceTypesTypeAddonArgs:
+    def __init__(__self__, *,
+                 backups: Sequence['GetInstanceTypesTypeAddonBackupArgs']):
+        pulumi.set(__self__, "backups", backups)
+
+    @property
+    @pulumi.getter
+    def backups(self) -> Sequence['GetInstanceTypesTypeAddonBackupArgs']:
+        return pulumi.get(self, "backups")
+
+    @backups.setter
+    def backups(self, value: Sequence['GetInstanceTypesTypeAddonBackupArgs']):
+        pulumi.set(self, "backups", value)
+
+
+@pulumi.input_type
+class GetInstanceTypesTypeAddonBackupArgs:
+    def __init__(__self__, *,
+                 prices: Sequence['GetInstanceTypesTypeAddonBackupPriceArgs']):
+        pulumi.set(__self__, "prices", prices)
+
+    @property
+    @pulumi.getter
+    def prices(self) -> Sequence['GetInstanceTypesTypeAddonBackupPriceArgs']:
+        return pulumi.get(self, "prices")
+
+    @prices.setter
+    def prices(self, value: Sequence['GetInstanceTypesTypeAddonBackupPriceArgs']):
+        pulumi.set(self, "prices", value)
+
+
+@pulumi.input_type
+class GetInstanceTypesTypeAddonBackupPriceArgs:
+    def __init__(__self__, *,
+                 hourly: float,
+                 monthly: float):
+        pulumi.set(__self__, "hourly", hourly)
+        pulumi.set(__self__, "monthly", monthly)
+
+    @property
+    @pulumi.getter
+    def hourly(self) -> float:
+        return pulumi.get(self, "hourly")
+
+    @hourly.setter
+    def hourly(self, value: float):
+        pulumi.set(self, "hourly", value)
+
+    @property
+    @pulumi.getter
+    def monthly(self) -> float:
+        return pulumi.get(self, "monthly")
+
+    @monthly.setter
+    def monthly(self, value: float):
+        pulumi.set(self, "monthly", value)
+
+
+@pulumi.input_type
+class GetInstanceTypesTypePriceArgs:
+    def __init__(__self__, *,
+                 hourly: float,
+                 monthly: float):
+        pulumi.set(__self__, "hourly", hourly)
+        pulumi.set(__self__, "monthly", monthly)
+
+    @property
+    @pulumi.getter
+    def hourly(self) -> float:
+        return pulumi.get(self, "hourly")
+
+    @hourly.setter
+    def hourly(self, value: float):
+        pulumi.set(self, "hourly", value)
+
+    @property
+    @pulumi.getter
+    def monthly(self) -> float:
+        return pulumi.get(self, "monthly")
+
+    @monthly.setter
+    def monthly(self, value: float):
+        pulumi.set(self, "monthly", value)
+
+
+@pulumi.input_type
 class GetInstancesFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by. See the Filterable Fields section for a list of filterable fields.
@@ -3218,14 +4121,51 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetRegionResolverArgs:
+    def __init__(__self__, *,
+                 ipv4: str,
+                 ipv6: str):
+        """
+        :param str ipv4: The IPv4 addresses for this region’s DNS resolvers, separated by commas.
+        :param str ipv6: The IPv6 addresses for this region’s DNS resolvers, separated by commas.
+        """
+        pulumi.set(__self__, "ipv4", ipv4)
+        pulumi.set(__self__, "ipv6", ipv6)
+
+    @property
+    @pulumi.getter
+    def ipv4(self) -> str:
+        """
+        The IPv4 addresses for this region’s DNS resolvers, separated by commas.
+        """
+        return pulumi.get(self, "ipv4")
+
+    @ipv4.setter
+    def ipv4(self, value: str):
+        pulumi.set(self, "ipv4", value)
+
+    @property
+    @pulumi.getter
+    def ipv6(self) -> str:
+        """
+        The IPv6 addresses for this region’s DNS resolvers, separated by commas.
+        """
+        return pulumi.get(self, "ipv6")
+
+    @ipv6.setter
+    def ipv6(self, value: str):
+        pulumi.set(self, "ipv6", value)
+
+
+@pulumi.input_type
 class GetRegionsFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by. See the Filterable Fields section for a complete list of filterable fields.
@@ -3451,221 +4391,661 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetStackScriptsStackscriptArgs:
+    def __init__(__self__, *,
+                 created: str,
+                 deployments_active: int,
+                 deployments_total: int,
+                 description: str,
+                 id: str,
+                 images: Sequence[str],
+                 is_public: bool,
+                 label: str,
+                 rev_note: str,
+                 script: str,
+                 updated: str,
+                 user_defined_fields: Sequence['GetStackScriptsStackscriptUserDefinedFieldArgs'],
+                 user_gravatar_id: str,
+                 username: str):
+        """
+        :param str created: The date this StackScript was created.
+        :param int deployments_active: Count of currently active, deployed Linodes created from this StackScript.
+        :param int deployments_total: The total number of times this StackScript has been deployed.
+        :param str description: A description for the StackScript.
+        :param str id: The unique ID of the StackScript.
+        :param Sequence[str] images: An array of Image IDs representing the Images that this StackScript is compatible for deploying with.
+        :param bool is_public: This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private.
+        :param str label: A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
+        :param str rev_note: This field allows you to add notes for the set of revisions made to this StackScript.
+        :param str script: The script to execute when provisioning a new Linode with this StackScript.
+        :param str updated: The date this StackScript was updated.
+        :param Sequence['GetStackScriptsStackscriptUserDefinedFieldArgs'] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
+        :param str user_gravatar_id: The Gravatar ID for the User who created the StackScript.
+        :param str username: The User who created the StackScript.
+        """
+        pulumi.set(__self__, "created", created)
+        pulumi.set(__self__, "deployments_active", deployments_active)
+        pulumi.set(__self__, "deployments_total", deployments_total)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "images", images)
+        pulumi.set(__self__, "is_public", is_public)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "rev_note", rev_note)
+        pulumi.set(__self__, "script", script)
+        pulumi.set(__self__, "updated", updated)
+        pulumi.set(__self__, "user_defined_fields", user_defined_fields)
+        pulumi.set(__self__, "user_gravatar_id", user_gravatar_id)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def created(self) -> str:
+        """
+        The date this StackScript was created.
+        """
+        return pulumi.get(self, "created")
+
+    @created.setter
+    def created(self, value: str):
+        pulumi.set(self, "created", value)
+
+    @property
+    @pulumi.getter(name="deploymentsActive")
+    def deployments_active(self) -> int:
+        """
+        Count of currently active, deployed Linodes created from this StackScript.
+        """
+        return pulumi.get(self, "deployments_active")
+
+    @deployments_active.setter
+    def deployments_active(self, value: int):
+        pulumi.set(self, "deployments_active", value)
+
+    @property
+    @pulumi.getter(name="deploymentsTotal")
+    def deployments_total(self) -> int:
+        """
+        The total number of times this StackScript has been deployed.
+        """
+        return pulumi.get(self, "deployments_total")
+
+    @deployments_total.setter
+    def deployments_total(self, value: int):
+        pulumi.set(self, "deployments_total", value)
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        A description for the StackScript.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: str):
+        pulumi.set(self, "description", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The unique ID of the StackScript.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: str):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def images(self) -> Sequence[str]:
+        """
+        An array of Image IDs representing the Images that this StackScript is compatible for deploying with.
+        """
+        return pulumi.get(self, "images")
+
+    @images.setter
+    def images(self, value: Sequence[str]):
+        pulumi.set(self, "images", value)
+
+    @property
+    @pulumi.getter(name="isPublic")
+    def is_public(self) -> bool:
+        """
+        This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private.
+        """
+        return pulumi.get(self, "is_public")
+
+    @is_public.setter
+    def is_public(self, value: bool):
+        pulumi.set(self, "is_public", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter(name="revNote")
+    def rev_note(self) -> str:
+        """
+        This field allows you to add notes for the set of revisions made to this StackScript.
+        """
+        return pulumi.get(self, "rev_note")
+
+    @rev_note.setter
+    def rev_note(self, value: str):
+        pulumi.set(self, "rev_note", value)
+
+    @property
+    @pulumi.getter
+    def script(self) -> str:
+        """
+        The script to execute when provisioning a new Linode with this StackScript.
+        """
+        return pulumi.get(self, "script")
+
+    @script.setter
+    def script(self, value: str):
+        pulumi.set(self, "script", value)
+
+    @property
+    @pulumi.getter
+    def updated(self) -> str:
+        """
+        The date this StackScript was updated.
+        """
+        return pulumi.get(self, "updated")
+
+    @updated.setter
+    def updated(self, value: str):
+        pulumi.set(self, "updated", value)
+
+    @property
+    @pulumi.getter(name="userDefinedFields")
+    def user_defined_fields(self) -> Sequence['GetStackScriptsStackscriptUserDefinedFieldArgs']:
+        """
+        This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
+        """
+        return pulumi.get(self, "user_defined_fields")
+
+    @user_defined_fields.setter
+    def user_defined_fields(self, value: Sequence['GetStackScriptsStackscriptUserDefinedFieldArgs']):
+        pulumi.set(self, "user_defined_fields", value)
+
+    @property
+    @pulumi.getter(name="userGravatarId")
+    def user_gravatar_id(self) -> str:
+        """
+        The Gravatar ID for the User who created the StackScript.
+        """
+        return pulumi.get(self, "user_gravatar_id")
+
+    @user_gravatar_id.setter
+    def user_gravatar_id(self, value: str):
+        pulumi.set(self, "user_gravatar_id", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        The User who created the StackScript.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: str):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class GetStackScriptsStackscriptUserDefinedFieldArgs:
+    def __init__(__self__, *,
+                 default: str,
+                 example: str,
+                 label: str,
+                 many_of: str,
+                 name: str,
+                 one_of: str):
+        """
+        :param str default: The default value. If not specified, this value will be used.
+        :param str example: An example value for the field.
+        :param str label: A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
+        :param str many_of: A list of acceptable values for the field in any quantity, combination or order.
+        :param str name: The name of the field to filter by. See the Filterable Fields section for a complete list of filterable fields.
+        :param str one_of: A list of acceptable single values for the field.
+        """
+        pulumi.set(__self__, "default", default)
+        pulumi.set(__self__, "example", example)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "many_of", many_of)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "one_of", one_of)
+
+    @property
+    @pulumi.getter
+    def default(self) -> str:
+        """
+        The default value. If not specified, this value will be used.
+        """
+        return pulumi.get(self, "default")
+
+    @default.setter
+    def default(self, value: str):
+        pulumi.set(self, "default", value)
+
+    @property
+    @pulumi.getter
+    def example(self) -> str:
+        """
+        An example value for the field.
+        """
+        return pulumi.get(self, "example")
+
+    @example.setter
+    def example(self, value: str):
+        pulumi.set(self, "example", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter(name="manyOf")
+    def many_of(self) -> str:
+        """
+        A list of acceptable values for the field in any quantity, combination or order.
+        """
+        return pulumi.get(self, "many_of")
+
+    @many_of.setter
+    def many_of(self, value: str):
+        pulumi.set(self, "many_of", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the field to filter by. See the Filterable Fields section for a complete list of filterable fields.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: str):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="oneOf")
+    def one_of(self) -> str:
+        """
+        A list of acceptable single values for the field.
+        """
+        return pulumi.get(self, "one_of")
+
+    @one_of.setter
+    def one_of(self, value: str):
+        pulumi.set(self, "one_of", value)
+
+
+@pulumi.input_type
+class GetUserDatabaseGrantArgs:
+    def __init__(__self__, *,
+                 id: int,
+                 label: str,
+                 permissions: str):
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "permissions", permissions)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: int):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def permissions(self) -> str:
+        return pulumi.get(self, "permissions")
+
+    @permissions.setter
+    def permissions(self, value: str):
+        pulumi.set(self, "permissions", value)
+
+
+@pulumi.input_type
 class GetUserDomainGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserFirewallGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserImageGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserLinodeGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserLongviewGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserNodebalancerGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserStackscriptGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class GetUserVolumeGrantArgs:
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: int):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: str):
         pulumi.set(self, "permissions", value)
 
@@ -3719,7 +5099,74 @@
         return pulumi.get(self, "match_by")
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
+@pulumi.input_type
+class GetVlansVlanArgs:
+    def __init__(__self__, *,
+                 created: str,
+                 label: str,
+                 linodes: Sequence[int],
+                 region: str):
+        """
+        :param str created: When the VLAN was created.
+        :param str label: The unique label of the VLAN.
+        :param Sequence[int] linodes: The running Linodes currently attached to the VLAN.
+        :param str region: The region the VLAN is located in. See all regions [here](https://api.linode.com/v4/regions).
+        """
+        pulumi.set(__self__, "created", created)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "linodes", linodes)
+        pulumi.set(__self__, "region", region)
+
+    @property
+    @pulumi.getter
+    def created(self) -> str:
+        """
+        When the VLAN was created.
+        """
+        return pulumi.get(self, "created")
+
+    @created.setter
+    def created(self, value: str):
+        pulumi.set(self, "created", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        The unique label of the VLAN.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def linodes(self) -> Sequence[int]:
+        """
+        The running Linodes currently attached to the VLAN.
+        """
+        return pulumi.get(self, "linodes")
+
+    @linodes.setter
+    def linodes(self, value: Sequence[int]):
+        pulumi.set(self, "linodes", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        """
+        The region the VLAN is located in. See all regions [here](https://api.linode.com/v4/regions).
+        """
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: str):
+        pulumi.set(self, "region", value)
+
+
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/_utilities.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/account_settings.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/config/vars.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/database_access_controls.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/database_access_controls.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/database_mysql.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/database_postgresql.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/domain.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/domain_record.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall_device.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/firewall_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_login.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_logins.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account_logins.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,21 +39,21 @@
     def filters(self) -> Optional[Sequence['outputs.GetAccountLoginsFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The unique ID of this login object.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def logins(self) -> Sequence['outputs.GetAccountLoginsLoginResult']:
+    def logins(self) -> Optional[Sequence['outputs.GetAccountLoginsLoginResult']]:
         return pulumi.get(self, "logins")
 
 
 class AwaitableGetAccountLoginsResult(GetAccountLoginsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -61,14 +61,15 @@
         return GetAccountLoginsResult(
             filters=self.filters,
             id=self.id,
             logins=self.logins)
 
 
 def get_account_logins(filters: Optional[Sequence[pulumi.InputType['GetAccountLoginsFilterArgs']]] = None,
+                       logins: Optional[Sequence[pulumi.InputType['GetAccountLoginsLoginArgs']]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAccountLoginsResult:
     """
     Provides information about Linode account logins that match a set of filters.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode account login.
@@ -95,25 +96,27 @@
 
     * `restricted`
 
     * `username`
     """
     __args__ = dict()
     __args__['filters'] = filters
+    __args__['logins'] = logins
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getAccountLogins:getAccountLogins', __args__, opts=opts, typ=GetAccountLoginsResult).value
 
     return AwaitableGetAccountLoginsResult(
         filters=__ret__.filters,
         id=__ret__.id,
         logins=__ret__.logins)
 
 
 @_utilities.lift_output_func(get_account_logins)
 def get_account_logins_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetAccountLoginsFilterArgs']]]]] = None,
+                              logins: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetAccountLoginsLoginArgs']]]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccountLoginsResult]:
     """
     Provides information about Linode account logins that match a set of filters.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode account login.
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_settings.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_account_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,14 @@
         Account-wide backups default.
         """
         return pulumi.get(self, "backups_enabled")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="longviewSubscription")
     def longview_subscription(self) -> str:
         """
         The Longview Pro tier you are currently subscribed to.
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_backups.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,30 +32,30 @@
         pulumi.set(__self__, "database_id", database_id)
         if database_type and not isinstance(database_type, str):
             raise TypeError("Expected argument 'database_type' to be a str")
         pulumi.set(__self__, "database_type", database_type)
         if filters and not isinstance(filters, list):
             raise TypeError("Expected argument 'filters' to be a list")
         pulumi.set(__self__, "filters", filters)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
+        if id and not isinstance(id, int):
+            raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if latest and not isinstance(latest, bool):
             raise TypeError("Expected argument 'latest' to be a bool")
         pulumi.set(__self__, "latest", latest)
         if order and not isinstance(order, str):
             raise TypeError("Expected argument 'order' to be a str")
         pulumi.set(__self__, "order", order)
         if order_by and not isinstance(order_by, str):
             raise TypeError("Expected argument 'order_by' to be a str")
         pulumi.set(__self__, "order_by", order_by)
 
     @property
     @pulumi.getter
-    def backups(self) -> Sequence['outputs.GetDatabaseBackupsBackupResult']:
+    def backups(self) -> Optional[Sequence['outputs.GetDatabaseBackupsBackupResult']]:
         return pulumi.get(self, "backups")
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> int:
         return pulumi.get(self, "database_id")
 
@@ -67,17 +67,17 @@
     @property
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.GetDatabaseBackupsFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def id(self) -> int:
         """
-        The provider-assigned unique ID for this managed resource.
+        The ID of the database backup object.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def latest(self) -> Optional[bool]:
         return pulumi.get(self, "latest")
@@ -105,15 +105,16 @@
             filters=self.filters,
             id=self.id,
             latest=self.latest,
             order=self.order,
             order_by=self.order_by)
 
 
-def get_database_backups(database_id: Optional[int] = None,
+def get_database_backups(backups: Optional[Sequence[pulumi.InputType['GetDatabaseBackupsBackupArgs']]] = None,
+                         database_id: Optional[int] = None,
                          database_type: Optional[str] = None,
                          filters: Optional[Sequence[pulumi.InputType['GetDatabaseBackupsFilterArgs']]] = None,
                          latest: Optional[bool] = None,
                          order: Optional[str] = None,
                          order_by: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseBackupsResult:
     """
@@ -151,14 +152,15 @@
     :param bool latest: If true, only the latest backup will be returned.
            
            * `filter` - (Optional) A set of filters used to select database backups that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`created`)
     """
     __args__ = dict()
+    __args__['backups'] = backups
     __args__['databaseId'] = database_id
     __args__['databaseType'] = database_type
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -172,15 +174,16 @@
         id=__ret__.id,
         latest=__ret__.latest,
         order=__ret__.order,
         order_by=__ret__.order_by)
 
 
 @_utilities.lift_output_func(get_database_backups)
-def get_database_backups_output(database_id: Optional[pulumi.Input[int]] = None,
+def get_database_backups_output(backups: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseBackupsBackupArgs']]]]] = None,
+                                database_id: Optional[pulumi.Input[int]] = None,
                                 database_type: Optional[pulumi.Input[str]] = None,
                                 filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseBackupsFilterArgs']]]]] = None,
                                 latest: Optional[pulumi.Input[Optional[bool]]] = None,
                                 order: Optional[pulumi.Input[Optional[str]]] = None,
                                 order_by: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseBackupsResult]:
     """
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_engines.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_engines.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,27 +41,27 @@
         pulumi.set(__self__, "order", order)
         if order_by and not isinstance(order_by, str):
             raise TypeError("Expected argument 'order_by' to be a str")
         pulumi.set(__self__, "order_by", order_by)
 
     @property
     @pulumi.getter
-    def engines(self) -> Sequence['outputs.GetDatabaseEnginesEngineResult']:
+    def engines(self) -> Optional[Sequence['outputs.GetDatabaseEnginesEngineResult']]:
         return pulumi.get(self, "engines")
 
     @property
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.GetDatabaseEnginesFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The Managed Database engine ID in engine/version format.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def latest(self) -> Optional[bool]:
         return pulumi.get(self, "latest")
@@ -87,15 +87,16 @@
             filters=self.filters,
             id=self.id,
             latest=self.latest,
             order=self.order,
             order_by=self.order_by)
 
 
-def get_database_engines(filters: Optional[Sequence[pulumi.InputType['GetDatabaseEnginesFilterArgs']]] = None,
+def get_database_engines(engines: Optional[Sequence[pulumi.InputType['GetDatabaseEnginesEngineArgs']]] = None,
+                         filters: Optional[Sequence[pulumi.InputType['GetDatabaseEnginesFilterArgs']]] = None,
                          latest: Optional[bool] = None,
                          order: Optional[str] = None,
                          order_by: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseEnginesResult:
     """
     Provides information about Linode Managed Database engines that match a set of filters.
 
@@ -146,14 +147,15 @@
     :param bool latest: If true, only the latest engine version will be returned.
            
            * `filter` - (Optional) A set of filters used to select engines that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     __args__ = dict()
+    __args__['engines'] = engines
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseEngines:getDatabaseEngines', __args__, opts=opts, typ=GetDatabaseEnginesResult).value
 
@@ -163,15 +165,16 @@
         id=__ret__.id,
         latest=__ret__.latest,
         order=__ret__.order,
         order_by=__ret__.order_by)
 
 
 @_utilities.lift_output_func(get_database_engines)
-def get_database_engines_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseEnginesFilterArgs']]]]] = None,
+def get_database_engines_output(engines: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseEnginesEngineArgs']]]]] = None,
+                                filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseEnginesFilterArgs']]]]] = None,
                                 latest: Optional[pulumi.Input[Optional[bool]]] = None,
                                 order: Optional[pulumi.Input[Optional[str]]] = None,
                                 order_by: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseEnginesResult]:
     """
     Provides information about Linode Managed Database engines that match a set of filters.
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql_backups.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_mysql_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_postgresql.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_database_postgresql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_databases.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_databases.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,59 +19,51 @@
 ]
 
 @pulumi.output_type
 class GetDatabasesResult:
     """
     A collection of values returned by getDatabases.
     """
-    def __init__(__self__, databases=None, filters=None, id=None, latest=None, order=None, order_by=None):
+    def __init__(__self__, databases=None, filters=None, id=None, order=None, order_by=None):
         if databases and not isinstance(databases, list):
             raise TypeError("Expected argument 'databases' to be a list")
         pulumi.set(__self__, "databases", databases)
         if filters and not isinstance(filters, list):
             raise TypeError("Expected argument 'filters' to be a list")
         pulumi.set(__self__, "filters", filters)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if latest and not isinstance(latest, bool):
-            raise TypeError("Expected argument 'latest' to be a bool")
-        pulumi.set(__self__, "latest", latest)
         if order and not isinstance(order, str):
             raise TypeError("Expected argument 'order' to be a str")
         pulumi.set(__self__, "order", order)
         if order_by and not isinstance(order_by, str):
             raise TypeError("Expected argument 'order_by' to be a str")
         pulumi.set(__self__, "order_by", order_by)
 
     @property
     @pulumi.getter
-    def databases(self) -> Sequence['outputs.GetDatabasesDatabaseResult']:
+    def databases(self) -> Optional[Sequence['outputs.GetDatabasesDatabaseResult']]:
         return pulumi.get(self, "databases")
 
     @property
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.GetDatabasesFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The ID of the Managed Database.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def latest(self) -> Optional[bool]:
-        return pulumi.get(self, "latest")
-
-    @property
-    @pulumi.getter
     def order(self) -> Optional[str]:
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter(name="orderBy")
     def order_by(self) -> Optional[str]:
         return pulumi.get(self, "order_by")
@@ -82,21 +74,20 @@
     def __await__(self):
         if False:
             yield self
         return GetDatabasesResult(
             databases=self.databases,
             filters=self.filters,
             id=self.id,
-            latest=self.latest,
             order=self.order,
             order_by=self.order_by)
 
 
-def get_databases(filters: Optional[Sequence[pulumi.InputType['GetDatabasesFilterArgs']]] = None,
-                  latest: Optional[bool] = None,
+def get_databases(databases: Optional[Sequence[pulumi.InputType['GetDatabasesDatabaseArgs']]] = None,
+                  filters: Optional[Sequence[pulumi.InputType['GetDatabasesFilterArgs']]] = None,
                   order: Optional[str] = None,
                   order_by: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabasesResult:
     """
     Provides information about Linode Managed Databases that match a set of filters.
 
     ## Example Usage
@@ -121,40 +112,36 @@
         name="engine",
         values=["mysql"],
     )])
     pulumi.export("databaseIds", [__item.id for __item in mysql.databases])
     ```
 
 
-    :param bool latest: If true, only the latest create database will be returned.
-           
-           * `filter` - (Optional) A set of filters used to select databases that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     __args__ = dict()
+    __args__['databases'] = databases
     __args__['filters'] = filters
-    __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabases:getDatabases', __args__, opts=opts, typ=GetDatabasesResult).value
 
     return AwaitableGetDatabasesResult(
         databases=__ret__.databases,
         filters=__ret__.filters,
         id=__ret__.id,
-        latest=__ret__.latest,
         order=__ret__.order,
         order_by=__ret__.order_by)
 
 
 @_utilities.lift_output_func(get_databases)
-def get_databases_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabasesFilterArgs']]]]] = None,
-                         latest: Optional[pulumi.Input[Optional[bool]]] = None,
+def get_databases_output(databases: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabasesDatabaseArgs']]]]] = None,
+                         filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabasesFilterArgs']]]]] = None,
                          order: Optional[pulumi.Input[Optional[str]]] = None,
                          order_by: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabasesResult]:
     """
     Provides information about Linode Managed Databases that match a set of filters.
 
     ## Example Usage
@@ -179,14 +166,11 @@
         name="engine",
         values=["mysql"],
     )])
     pulumi.export("databaseIds", [__item.id for __item in mysql.databases])
     ```
 
 
-    :param bool latest: If true, only the latest create database will be returned.
-           
-           * `filter` - (Optional) A set of filters used to select databases that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_record.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_zonefile.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_domain_zonefile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_firewall.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_image.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_images.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,21 +48,21 @@
     def filters(self) -> Optional[Sequence['outputs.GetImagesFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The unique ID of this Image.  The ID of private images begin with `private/` followed by the numeric identifier of the private image, for example `private/12345`.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def images(self) -> Sequence['outputs.GetImagesImageResult']:
+    def images(self) -> Optional[Sequence['outputs.GetImagesImageResult']]:
         return pulumi.get(self, "images")
 
     @property
     @pulumi.getter
     def latest(self) -> Optional[bool]:
         return pulumi.get(self, "latest")
 
@@ -88,14 +88,15 @@
             images=self.images,
             latest=self.latest,
             order=self.order,
             order_by=self.order_by)
 
 
 def get_images(filters: Optional[Sequence[pulumi.InputType['GetImagesFilterArgs']]] = None,
+               images: Optional[Sequence[pulumi.InputType['GetImagesImageArgs']]] = None,
                latest: Optional[bool] = None,
                order: Optional[str] = None,
                order_by: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetImagesResult:
     """
     Provides information about Linode images that match a set of filters.
 
@@ -154,14 +155,15 @@
            
            * `filter` - (Optional) A set of filters used to select Linode images that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
+    __args__['images'] = images
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getImages:getImages', __args__, opts=opts, typ=GetImagesResult).value
 
     return AwaitableGetImagesResult(
@@ -171,14 +173,15 @@
         latest=__ret__.latest,
         order=__ret__.order,
         order_by=__ret__.order_by)
 
 
 @_utilities.lift_output_func(get_images)
 def get_images_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetImagesFilterArgs']]]]] = None,
+                      images: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetImagesImageArgs']]]]] = None,
                       latest: Optional[pulumi.Input[Optional[bool]]] = None,
                       order: Optional[pulumi.Input[Optional[str]]] = None,
                       order_by: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetImagesResult]:
     """
     Provides information about Linode images that match a set of filters.
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_backups.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_networking.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_networking.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_type.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_types.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instance_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def filters(self) -> Optional[Sequence['outputs.GetInstanceTypesFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The ID representing the Linode Type.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def order(self) -> Optional[str]:
         return pulumi.get(self, "order")
@@ -61,15 +61,15 @@
     @property
     @pulumi.getter(name="orderBy")
     def order_by(self) -> Optional[str]:
         return pulumi.get(self, "order_by")
 
     @property
     @pulumi.getter
-    def types(self) -> Sequence['outputs.GetInstanceTypesTypeResult']:
+    def types(self) -> Optional[Sequence['outputs.GetInstanceTypesTypeResult']]:
         return pulumi.get(self, "types")
 
 
 class AwaitableGetInstanceTypesResult(GetInstanceTypesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -81,14 +81,15 @@
             order_by=self.order_by,
             types=self.types)
 
 
 def get_instance_types(filters: Optional[Sequence[pulumi.InputType['GetInstanceTypesFilterArgs']]] = None,
                        order: Optional[str] = None,
                        order_by: Optional[str] = None,
+                       types: Optional[Sequence[pulumi.InputType['GetInstanceTypesTypeArgs']]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstanceTypesResult:
     """
     Provides information about Linode Instance types that match a set of filters.
 
     ## Example Usage
 
     Get information about all Linode Instance types with a certain number of VCPUs:
@@ -135,14 +136,15 @@
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
+    __args__['types'] = types
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceTypes:getInstanceTypes', __args__, opts=opts, typ=GetInstanceTypesResult).value
 
     return AwaitableGetInstanceTypesResult(
         filters=__ret__.filters,
         id=__ret__.id,
         order=__ret__.order,
@@ -150,14 +152,15 @@
         types=__ret__.types)
 
 
 @_utilities.lift_output_func(get_instance_types)
 def get_instance_types_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstanceTypesFilterArgs']]]]] = None,
                               order: Optional[pulumi.Input[Optional[str]]] = None,
                               order_by: Optional[pulumi.Input[Optional[str]]] = None,
+                              types: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstanceTypesTypeArgs']]]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceTypesResult]:
     """
     Provides information about Linode Instance types that match a set of filters.
 
     ## Example Usage
 
     Get information about all Linode Instance types with a certain number of VCPUs:
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instances.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ipv6_range.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_kernel.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_kernel.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_linode_object_storage_bucket.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_linode_object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_cluster.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_versions.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_lke_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_networking_ip.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_networking_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_config.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_node.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_object_storage_cluster.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_object_storage_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_profile.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_region.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_region.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
+from ._inputs import *
 
 __all__ = [
     'GetRegionResult',
     'AwaitableGetRegionResult',
     'get_region',
     'get_region_output',
 ]
@@ -69,15 +70,15 @@
         """
         Detailed location information for this Region, including city, state or region, and country.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
-    def resolvers(self) -> Sequence['outputs.GetRegionResolverResult']:
+    def resolvers(self) -> Optional[Sequence['outputs.GetRegionResolverResult']]:
         return pulumi.get(self, "resolvers")
 
     @property
     @pulumi.getter
     def status(self) -> str:
         """
         This region’s current operational status (ok or outage).
@@ -95,16 +96,16 @@
             country=self.country,
             id=self.id,
             label=self.label,
             resolvers=self.resolvers,
             status=self.status)
 
 
-def get_region(country: Optional[str] = None,
-               id: Optional[str] = None,
+def get_region(id: Optional[str] = None,
+               resolvers: Optional[Sequence[pulumi.InputType['GetRegionResolverArgs']]] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegionResult:
     """
     `get_region` provides details about a specific Linode region. See all regions [here](https://api.linode.com/v4/regions).
 
     ## Example Usage
 
     The following example shows how the resource might be used to obtain additional information about a Linode region.
@@ -113,35 +114,34 @@
     import pulumi
     import pulumi_linode as linode
 
     region = linode.get_region(id="us-east")
     ```
 
 
-    :param str country: The country the region resides in.
     :param str id: The code name of the region to select.
     """
     __args__ = dict()
-    __args__['country'] = country
     __args__['id'] = id
+    __args__['resolvers'] = resolvers
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getRegion:getRegion', __args__, opts=opts, typ=GetRegionResult).value
 
     return AwaitableGetRegionResult(
         capabilities=__ret__.capabilities,
         country=__ret__.country,
         id=__ret__.id,
         label=__ret__.label,
         resolvers=__ret__.resolvers,
         status=__ret__.status)
 
 
 @_utilities.lift_output_func(get_region)
-def get_region_output(country: Optional[pulumi.Input[Optional[str]]] = None,
-                      id: Optional[pulumi.Input[str]] = None,
+def get_region_output(id: Optional[pulumi.Input[str]] = None,
+                      resolvers: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetRegionResolverArgs']]]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionResult]:
     """
     `get_region` provides details about a specific Linode region. See all regions [here](https://api.linode.com/v4/regions).
 
     ## Example Usage
 
     The following example shows how the resource might be used to obtain additional information about a Linode region.
@@ -150,11 +150,10 @@
     import pulumi
     import pulumi_linode as linode
 
     region = linode.get_region(id="us-east")
     ```
 
 
-    :param str country: The country the region resides in.
     :param str id: The code name of the region to select.
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_regions.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ssh_key.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_script.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_scripts.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_stack_scripts.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def filters(self) -> Optional[Sequence['outputs.GetStackScriptsFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The unique ID of the StackScript.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def latest(self) -> Optional[bool]:
         return pulumi.get(self, "latest")
@@ -69,15 +69,15 @@
     @property
     @pulumi.getter(name="orderBy")
     def order_by(self) -> Optional[str]:
         return pulumi.get(self, "order_by")
 
     @property
     @pulumi.getter
-    def stackscripts(self) -> Sequence['outputs.GetStackScriptsStackscriptResult']:
+    def stackscripts(self) -> Optional[Sequence['outputs.GetStackScriptsStackscriptResult']]:
         return pulumi.get(self, "stackscripts")
 
 
 class AwaitableGetStackScriptsResult(GetStackScriptsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -91,14 +91,15 @@
             stackscripts=self.stackscripts)
 
 
 def get_stack_scripts(filters: Optional[Sequence[pulumi.InputType['GetStackScriptsFilterArgs']]] = None,
                       latest: Optional[bool] = None,
                       order: Optional[str] = None,
                       order_by: Optional[str] = None,
+                      stackscripts: Optional[Sequence[pulumi.InputType['GetStackScriptsStackscriptArgs']]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetStackScriptsResult:
     """
     Provides information about Linode StackScripts that match a set of filters.
 
     **NOTICE:** Due to the large number of public StackScripts, this data source may time out if `is_public` is not filtered on.
 
     ## Example Usage
@@ -149,14 +150,15 @@
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
+    __args__['stackscripts'] = stackscripts
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getStackScripts:getStackScripts', __args__, opts=opts, typ=GetStackScriptsResult).value
 
     return AwaitableGetStackScriptsResult(
         filters=__ret__.filters,
         id=__ret__.id,
         latest=__ret__.latest,
@@ -166,14 +168,15 @@
 
 
 @_utilities.lift_output_func(get_stack_scripts)
 def get_stack_scripts_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetStackScriptsFilterArgs']]]]] = None,
                              latest: Optional[pulumi.Input[Optional[bool]]] = None,
                              order: Optional[pulumi.Input[Optional[str]]] = None,
                              order_by: Optional[pulumi.Input[Optional[str]]] = None,
+                             stackscripts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetStackScriptsStackscriptArgs']]]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetStackScriptsResult]:
     """
     Provides information about Linode StackScripts that match a set of filters.
 
     **NOTICE:** Due to the large number of public StackScripts, this data source may time out if `is_public` is not filtered on.
 
     ## Example Usage
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_user.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 ]
 
 @pulumi.output_type
 class GetUserResult:
     """
     A collection of values returned by getUser.
     """
-    def __init__(__self__, domain_grants=None, email=None, firewall_grants=None, global_grants=None, id=None, image_grants=None, linode_grants=None, longview_grants=None, nodebalancer_grants=None, restricted=None, ssh_keys=None, stackscript_grants=None, username=None, volume_grants=None):
+    def __init__(__self__, database_grants=None, domain_grants=None, email=None, firewall_grants=None, global_grants=None, id=None, image_grants=None, linode_grants=None, longview_grants=None, nodebalancer_grants=None, restricted=None, ssh_keys=None, stackscript_grants=None, username=None, volume_grants=None):
+        if database_grants and not isinstance(database_grants, list):
+            raise TypeError("Expected argument 'database_grants' to be a list")
+        pulumi.set(__self__, "database_grants", database_grants)
         if domain_grants and not isinstance(domain_grants, list):
             raise TypeError("Expected argument 'domain_grants' to be a list")
         pulumi.set(__self__, "domain_grants", domain_grants)
         if email and not isinstance(email, str):
             raise TypeError("Expected argument 'email' to be a str")
         pulumi.set(__self__, "email", email)
         if firewall_grants and not isinstance(firewall_grants, list):
@@ -64,14 +67,22 @@
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
         if volume_grants and not isinstance(volume_grants, list):
             raise TypeError("Expected argument 'volume_grants' to be a list")
         pulumi.set(__self__, "volume_grants", volume_grants)
 
     @property
+    @pulumi.getter(name="databaseGrants")
+    def database_grants(self) -> Sequence['outputs.GetUserDatabaseGrantResult']:
+        """
+        The grants this User has pertaining to Databases on this Account.
+        """
+        return pulumi.get(self, "database_grants")
+
+    @property
     @pulumi.getter(name="domainGrants")
     def domain_grants(self) -> Sequence['outputs.GetUserDomainGrantResult']:
         """
         The grants this User has pertaining to Domains on this Account.
         """
         return pulumi.get(self, "domain_grants")
 
@@ -98,17 +109,14 @@
         The Account-level grants a User has.
         """
         return pulumi.get(self, "global_grants")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="imageGrants")
     def image_grants(self) -> Sequence['outputs.GetUserImageGrantResult']:
         """
         The grants this User has pertaining to Images on this Account.
@@ -179,14 +187,15 @@
 
 class AwaitableGetUserResult(GetUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetUserResult(
+            database_grants=self.database_grants,
             domain_grants=self.domain_grants,
             email=self.email,
             firewall_grants=self.firewall_grants,
             global_grants=self.global_grants,
             id=self.id,
             image_grants=self.image_grants,
             linode_grants=self.linode_grants,
@@ -195,63 +204,56 @@
             restricted=self.restricted,
             ssh_keys=self.ssh_keys,
             stackscript_grants=self.stackscript_grants,
             username=self.username,
             volume_grants=self.volume_grants)
 
 
-def get_user(domain_grants: Optional[Sequence[pulumi.InputType['GetUserDomainGrantArgs']]] = None,
+def get_user(database_grants: Optional[Sequence[pulumi.InputType['GetUserDatabaseGrantArgs']]] = None,
+             domain_grants: Optional[Sequence[pulumi.InputType['GetUserDomainGrantArgs']]] = None,
              firewall_grants: Optional[Sequence[pulumi.InputType['GetUserFirewallGrantArgs']]] = None,
              image_grants: Optional[Sequence[pulumi.InputType['GetUserImageGrantArgs']]] = None,
              linode_grants: Optional[Sequence[pulumi.InputType['GetUserLinodeGrantArgs']]] = None,
              longview_grants: Optional[Sequence[pulumi.InputType['GetUserLongviewGrantArgs']]] = None,
              nodebalancer_grants: Optional[Sequence[pulumi.InputType['GetUserNodebalancerGrantArgs']]] = None,
              stackscript_grants: Optional[Sequence[pulumi.InputType['GetUserStackscriptGrantArgs']]] = None,
              username: Optional[str] = None,
              volume_grants: Optional[Sequence[pulumi.InputType['GetUserVolumeGrantArgs']]] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Provides information about a Linode user
 
-    ## Example Usage
-
-    The following example shows how one might use this data source to access information about a Linode user.
-
-    ```python
-    import pulumi
-    import pulumi_linode as linode
-
-    foo = linode.get_user(username="foo")
-    ```
-
 
+    :param Sequence[pulumi.InputType['GetUserDatabaseGrantArgs']] database_grants: The grants this User has pertaining to Databases on this Account.
     :param Sequence[pulumi.InputType['GetUserDomainGrantArgs']] domain_grants: The grants this User has pertaining to Domains on this Account.
     :param Sequence[pulumi.InputType['GetUserFirewallGrantArgs']] firewall_grants: The grants this User has pertaining to Firewalls on this Account.
     :param Sequence[pulumi.InputType['GetUserImageGrantArgs']] image_grants: The grants this User has pertaining to Images on this Account.
     :param Sequence[pulumi.InputType['GetUserLinodeGrantArgs']] linode_grants: The grants this User has pertaining to Linodes on this Account.
     :param Sequence[pulumi.InputType['GetUserLongviewGrantArgs']] longview_grants: The grants this User has pertaining to Longview Clients on this Account.
     :param Sequence[pulumi.InputType['GetUserNodebalancerGrantArgs']] nodebalancer_grants: The grants this User has pertaining to NodeBalancers on this Account.
     :param Sequence[pulumi.InputType['GetUserStackscriptGrantArgs']] stackscript_grants: The grants this User has pertaining to StackScripts on this Account.
     :param str username: The unique username of this User.
     :param Sequence[pulumi.InputType['GetUserVolumeGrantArgs']] volume_grants: The grants this User has pertaining to Volumes on this Account.
     """
     __args__ = dict()
+    __args__['databaseGrants'] = database_grants
     __args__['domainGrants'] = domain_grants
     __args__['firewallGrants'] = firewall_grants
     __args__['imageGrants'] = image_grants
     __args__['linodeGrants'] = linode_grants
     __args__['longviewGrants'] = longview_grants
     __args__['nodebalancerGrants'] = nodebalancer_grants
     __args__['stackscriptGrants'] = stackscript_grants
     __args__['username'] = username
     __args__['volumeGrants'] = volume_grants
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
+        database_grants=__ret__.database_grants,
         domain_grants=__ret__.domain_grants,
         email=__ret__.email,
         firewall_grants=__ret__.firewall_grants,
         global_grants=__ret__.global_grants,
         id=__ret__.id,
         image_grants=__ret__.image_grants,
         linode_grants=__ret__.linode_grants,
@@ -261,39 +263,30 @@
         ssh_keys=__ret__.ssh_keys,
         stackscript_grants=__ret__.stackscript_grants,
         username=__ret__.username,
         volume_grants=__ret__.volume_grants)
 
 
 @_utilities.lift_output_func(get_user)
-def get_user_output(domain_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserDomainGrantArgs']]]]] = None,
+def get_user_output(database_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserDatabaseGrantArgs']]]]] = None,
+                    domain_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserDomainGrantArgs']]]]] = None,
                     firewall_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserFirewallGrantArgs']]]]] = None,
                     image_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserImageGrantArgs']]]]] = None,
                     linode_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserLinodeGrantArgs']]]]] = None,
                     longview_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserLongviewGrantArgs']]]]] = None,
                     nodebalancer_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserNodebalancerGrantArgs']]]]] = None,
                     stackscript_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserStackscriptGrantArgs']]]]] = None,
                     username: Optional[pulumi.Input[str]] = None,
                     volume_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserVolumeGrantArgs']]]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Provides information about a Linode user
 
-    ## Example Usage
-
-    The following example shows how one might use this data source to access information about a Linode user.
-
-    ```python
-    import pulumi
-    import pulumi_linode as linode
-
-    foo = linode.get_user(username="foo")
-    ```
-
 
+    :param Sequence[pulumi.InputType['GetUserDatabaseGrantArgs']] database_grants: The grants this User has pertaining to Databases on this Account.
     :param Sequence[pulumi.InputType['GetUserDomainGrantArgs']] domain_grants: The grants this User has pertaining to Domains on this Account.
     :param Sequence[pulumi.InputType['GetUserFirewallGrantArgs']] firewall_grants: The grants this User has pertaining to Firewalls on this Account.
     :param Sequence[pulumi.InputType['GetUserImageGrantArgs']] image_grants: The grants this User has pertaining to Images on this Account.
     :param Sequence[pulumi.InputType['GetUserLinodeGrantArgs']] linode_grants: The grants this User has pertaining to Linodes on this Account.
     :param Sequence[pulumi.InputType['GetUserLongviewGrantArgs']] longview_grants: The grants this User has pertaining to Longview Clients on this Account.
     :param Sequence[pulumi.InputType['GetUserNodebalancerGrantArgs']] nodebalancer_grants: The grants this User has pertaining to NodeBalancers on this Account.
     :param Sequence[pulumi.InputType['GetUserStackscriptGrantArgs']] stackscript_grants: The grants this User has pertaining to StackScripts on this Account.
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_vlans.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_vlans.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,32 +44,29 @@
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.GetVlansFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def order(self) -> Optional[str]:
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter(name="orderBy")
     def order_by(self) -> Optional[str]:
         return pulumi.get(self, "order_by")
 
     @property
     @pulumi.getter
-    def vlans(self) -> Sequence['outputs.GetVlansVlanResult']:
+    def vlans(self) -> Optional[Sequence['outputs.GetVlansVlanResult']]:
         return pulumi.get(self, "vlans")
 
 
 class AwaitableGetVlansResult(GetVlansResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -81,14 +78,15 @@
             order_by=self.order_by,
             vlans=self.vlans)
 
 
 def get_vlans(filters: Optional[Sequence[pulumi.InputType['GetVlansFilterArgs']]] = None,
               order: Optional[str] = None,
               order_by: Optional[str] = None,
+              vlans: Optional[Sequence[pulumi.InputType['GetVlansVlanArgs']]] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVlansResult:
     """
     Provides details about Linode VLANs.
 
     ## Example Usage
 
     ```python
@@ -121,14 +119,15 @@
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
+    __args__['vlans'] = vlans
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getVlans:getVlans', __args__, opts=opts, typ=GetVlansResult).value
 
     return AwaitableGetVlansResult(
         filters=__ret__.filters,
         id=__ret__.id,
         order=__ret__.order,
@@ -136,14 +135,15 @@
         vlans=__ret__.vlans)
 
 
 @_utilities.lift_output_func(get_vlans)
 def get_vlans_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetVlansFilterArgs']]]]] = None,
                      order: Optional[pulumi.Input[Optional[str]]] = None,
                      order_by: Optional[pulumi.Input[Optional[str]]] = None,
+                     vlans: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetVlansVlanArgs']]]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVlansResult]:
     """
     Provides details about Linode VLANs.
 
     ## Example Usage
 
     ```python
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_volume.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/image.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_disk.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/instance_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_ip.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/instance_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_shared_ips.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/instance_shared_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/ipv6_range.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/lke_cluster.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_config.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_node.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_bucket.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_key.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/object_storage_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_object.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/object_storage_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/outputs.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,16 @@
     'GetInstanceNetworkingIpv4ReservedResult',
     'GetInstanceNetworkingIpv4SharedResult',
     'GetInstanceNetworkingIpv6Result',
     'GetInstanceNetworkingIpv6GlobalResult',
     'GetInstanceNetworkingIpv6LinkLocalResult',
     'GetInstanceNetworkingIpv6SlaacResult',
     'GetInstanceTypeAddonsResult',
-    'GetInstanceTypeAddonsBackupsResult',
-    'GetInstanceTypeAddonsBackupsPriceResult',
+    'GetInstanceTypeAddonsBackupResult',
+    'GetInstanceTypeAddonsBackupPriceResult',
     'GetInstanceTypePriceResult',
     'GetInstanceTypesFilterResult',
     'GetInstanceTypesTypeResult',
     'GetInstanceTypesTypeAddonResult',
     'GetInstanceTypesTypeAddonBackupResult',
     'GetInstanceTypesTypeAddonBackupPriceResult',
     'GetInstanceTypesTypePriceResult',
@@ -128,14 +128,15 @@
     'GetRegionsFilterResult',
     'GetRegionsRegionResult',
     'GetRegionsRegionResolverResult',
     'GetStackScriptUserDefinedFieldResult',
     'GetStackScriptsFilterResult',
     'GetStackScriptsStackscriptResult',
     'GetStackScriptsStackscriptUserDefinedFieldResult',
+    'GetUserDatabaseGrantResult',
     'GetUserDomainGrantResult',
     'GetUserFirewallGrantResult',
     'GetUserGlobalGrantResult',
     'GetUserImageGrantResult',
     'GetUserLinodeGrantResult',
     'GetUserLongviewGrantResult',
     'GetUserNodebalancerGrantResult',
@@ -4985,37 +4986,37 @@
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class GetInstanceTypeAddonsResult(dict):
     def __init__(__self__, *,
-                 backups: 'outputs.GetInstanceTypeAddonsBackupsResult'):
+                 backups: Sequence['outputs.GetInstanceTypeAddonsBackupResult']):
         pulumi.set(__self__, "backups", backups)
 
     @property
     @pulumi.getter
-    def backups(self) -> 'outputs.GetInstanceTypeAddonsBackupsResult':
+    def backups(self) -> Sequence['outputs.GetInstanceTypeAddonsBackupResult']:
         return pulumi.get(self, "backups")
 
 
 @pulumi.output_type
-class GetInstanceTypeAddonsBackupsResult(dict):
+class GetInstanceTypeAddonsBackupResult(dict):
     def __init__(__self__, *,
-                 price: 'outputs.GetInstanceTypeAddonsBackupsPriceResult'):
-        pulumi.set(__self__, "price", price)
+                 prices: Sequence['outputs.GetInstanceTypeAddonsBackupPriceResult']):
+        pulumi.set(__self__, "prices", prices)
 
     @property
     @pulumi.getter
-    def price(self) -> 'outputs.GetInstanceTypeAddonsBackupsPriceResult':
-        return pulumi.get(self, "price")
+    def prices(self) -> Sequence['outputs.GetInstanceTypeAddonsBackupPriceResult']:
+        return pulumi.get(self, "prices")
 
 
 @pulumi.output_type
-class GetInstanceTypeAddonsBackupsPriceResult(dict):
+class GetInstanceTypeAddonsBackupPriceResult(dict):
     def __init__(__self__, *,
                  hourly: float,
                  monthly: float):
         pulumi.set(__self__, "hourly", hourly)
         pulumi.set(__self__, "monthly", monthly)
 
     @property
@@ -6868,30 +6869,30 @@
 @pulumi.output_type
 class GetStackScriptsStackscriptResult(dict):
     def __init__(__self__, *,
                  created: str,
                  deployments_active: int,
                  deployments_total: int,
                  description: str,
-                 id: int,
+                 id: str,
                  images: Sequence[str],
                  is_public: bool,
                  label: str,
                  rev_note: str,
                  script: str,
                  updated: str,
                  user_defined_fields: Sequence['outputs.GetStackScriptsStackscriptUserDefinedFieldResult'],
                  user_gravatar_id: str,
                  username: str):
         """
         :param str created: The date this StackScript was created.
         :param int deployments_active: Count of currently active, deployed Linodes created from this StackScript.
         :param int deployments_total: The total number of times this StackScript has been deployed.
         :param str description: A description for the StackScript.
-        :param int id: The unique ID of the StackScript.
+        :param str id: The unique ID of the StackScript.
         :param Sequence[str] images: An array of Image IDs representing the Images that this StackScript is compatible for deploying with.
         :param bool is_public: This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private.
         :param str label: A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
         :param str rev_note: This field allows you to add notes for the set of revisions made to this StackScript.
         :param str script: The script to execute when provisioning a new Linode with this StackScript.
         :param str updated: The date this StackScript was updated.
         :param Sequence['GetStackScriptsStackscriptUserDefinedFieldArgs'] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
@@ -6943,15 +6944,15 @@
         """
         A description for the StackScript.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def id(self) -> int:
+    def id(self) -> str:
         """
         The unique ID of the StackScript.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
@@ -7096,262 +7097,332 @@
         """
         A list of acceptable single values for the field.
         """
         return pulumi.get(self, "one_of")
 
 
 @pulumi.output_type
+class GetUserDatabaseGrantResult(dict):
+    def __init__(__self__, *,
+                 id: int,
+                 label: str,
+                 permissions: str):
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "permissions", permissions)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
+    def permissions(self) -> str:
+        return pulumi.get(self, "permissions")
+
+
+@pulumi.output_type
 class GetUserDomainGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserFirewallGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserGlobalGrantResult(dict):
     def __init__(__self__, *,
-                 account_access: Optional[str] = None,
-                 add_databases: Optional[bool] = None,
-                 add_domains: Optional[bool] = None,
-                 add_firewalls: Optional[bool] = None,
-                 add_images: Optional[bool] = None,
-                 add_linodes: Optional[bool] = None,
-                 add_longview: Optional[bool] = None,
-                 add_nodebalancers: Optional[bool] = None,
-                 add_stackscripts: Optional[bool] = None,
-                 add_volumes: Optional[bool] = None,
-                 cancel_account: Optional[bool] = None,
-                 longview_subscription: Optional[bool] = None):
-        if account_access is not None:
-            pulumi.set(__self__, "account_access", account_access)
-        if add_databases is not None:
-            pulumi.set(__self__, "add_databases", add_databases)
-        if add_domains is not None:
-            pulumi.set(__self__, "add_domains", add_domains)
-        if add_firewalls is not None:
-            pulumi.set(__self__, "add_firewalls", add_firewalls)
-        if add_images is not None:
-            pulumi.set(__self__, "add_images", add_images)
-        if add_linodes is not None:
-            pulumi.set(__self__, "add_linodes", add_linodes)
-        if add_longview is not None:
-            pulumi.set(__self__, "add_longview", add_longview)
-        if add_nodebalancers is not None:
-            pulumi.set(__self__, "add_nodebalancers", add_nodebalancers)
-        if add_stackscripts is not None:
-            pulumi.set(__self__, "add_stackscripts", add_stackscripts)
-        if add_volumes is not None:
-            pulumi.set(__self__, "add_volumes", add_volumes)
-        if cancel_account is not None:
-            pulumi.set(__self__, "cancel_account", cancel_account)
-        if longview_subscription is not None:
-            pulumi.set(__self__, "longview_subscription", longview_subscription)
+                 account_access: str,
+                 add_databases: bool,
+                 add_domains: bool,
+                 add_firewalls: bool,
+                 add_images: bool,
+                 add_linodes: bool,
+                 add_longview: bool,
+                 add_nodebalancers: bool,
+                 add_stackscripts: bool,
+                 add_volumes: bool,
+                 cancel_account: bool,
+                 longview_subscription: bool):
+        pulumi.set(__self__, "account_access", account_access)
+        pulumi.set(__self__, "add_databases", add_databases)
+        pulumi.set(__self__, "add_domains", add_domains)
+        pulumi.set(__self__, "add_firewalls", add_firewalls)
+        pulumi.set(__self__, "add_images", add_images)
+        pulumi.set(__self__, "add_linodes", add_linodes)
+        pulumi.set(__self__, "add_longview", add_longview)
+        pulumi.set(__self__, "add_nodebalancers", add_nodebalancers)
+        pulumi.set(__self__, "add_stackscripts", add_stackscripts)
+        pulumi.set(__self__, "add_volumes", add_volumes)
+        pulumi.set(__self__, "cancel_account", cancel_account)
+        pulumi.set(__self__, "longview_subscription", longview_subscription)
 
     @property
     @pulumi.getter(name="accountAccess")
-    def account_access(self) -> Optional[str]:
+    def account_access(self) -> str:
         return pulumi.get(self, "account_access")
 
     @property
     @pulumi.getter(name="addDatabases")
-    def add_databases(self) -> Optional[bool]:
+    def add_databases(self) -> bool:
         return pulumi.get(self, "add_databases")
 
     @property
     @pulumi.getter(name="addDomains")
-    def add_domains(self) -> Optional[bool]:
+    def add_domains(self) -> bool:
         return pulumi.get(self, "add_domains")
 
     @property
     @pulumi.getter(name="addFirewalls")
-    def add_firewalls(self) -> Optional[bool]:
+    def add_firewalls(self) -> bool:
         return pulumi.get(self, "add_firewalls")
 
     @property
     @pulumi.getter(name="addImages")
-    def add_images(self) -> Optional[bool]:
+    def add_images(self) -> bool:
         return pulumi.get(self, "add_images")
 
     @property
     @pulumi.getter(name="addLinodes")
-    def add_linodes(self) -> Optional[bool]:
+    def add_linodes(self) -> bool:
         return pulumi.get(self, "add_linodes")
 
     @property
     @pulumi.getter(name="addLongview")
-    def add_longview(self) -> Optional[bool]:
+    def add_longview(self) -> bool:
         return pulumi.get(self, "add_longview")
 
     @property
     @pulumi.getter(name="addNodebalancers")
-    def add_nodebalancers(self) -> Optional[bool]:
+    def add_nodebalancers(self) -> bool:
         return pulumi.get(self, "add_nodebalancers")
 
     @property
     @pulumi.getter(name="addStackscripts")
-    def add_stackscripts(self) -> Optional[bool]:
+    def add_stackscripts(self) -> bool:
         return pulumi.get(self, "add_stackscripts")
 
     @property
     @pulumi.getter(name="addVolumes")
-    def add_volumes(self) -> Optional[bool]:
+    def add_volumes(self) -> bool:
         return pulumi.get(self, "add_volumes")
 
     @property
     @pulumi.getter(name="cancelAccount")
-    def cancel_account(self) -> Optional[bool]:
+    def cancel_account(self) -> bool:
         return pulumi.get(self, "cancel_account")
 
     @property
     @pulumi.getter(name="longviewSubscription")
-    def longview_subscription(self) -> Optional[bool]:
+    def longview_subscription(self) -> bool:
         return pulumi.get(self, "longview_subscription")
 
 
 @pulumi.output_type
 class GetUserImageGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserLinodeGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserLongviewGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserNodebalancerGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserStackscriptGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetUserVolumeGrantResult(dict):
     def __init__(__self__, *,
                  id: int,
+                 label: str,
                  permissions: str):
         pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter
     def id(self) -> int:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
     def permissions(self) -> str:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
 class GetVlansFilterResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/provider.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/rdns.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/rdns.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/ssh_key.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/stack_script.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/token.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/user.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode/volume.py` & `pulumi_linode-4.4.0a1687557732/pulumi_linode/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/PKG-INFO` & `pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-linode
-Version: 4.3.0a1687424922
+Version: 4.4.0a1687557732
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/SOURCES.txt` & `pulumi_linode-4.4.0a1687557732/pulumi_linode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687424922/setup.py` & `pulumi_linode-4.4.0a1687557732/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.3.0a1687424922"
-PLUGIN_VERSION = "4.3.0-alpha.1687424922+8a494834"
+VERSION = "4.4.0a1687557732"
+PLUGIN_VERSION = "4.4.0-alpha.1687557732+e4f42e5d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'linode', PLUGIN_VERSION])
         except OSError as error:
```

