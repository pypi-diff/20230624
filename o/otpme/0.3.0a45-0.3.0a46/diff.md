# Comparing `tmp/otpme-0.3.0a45.tar.gz` & `tmp/otpme-0.3.0a46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpme-0.3.0a45.tar", last modified: Fri Jun 23 07:04:10 2023, max compression
+gzip compressed data, was "otpme-0.3.0a46.tar", last modified: Sat Jun 24 05:09:50 2023, max compression
```

## Comparing `otpme-0.3.0a45.tar` & `otpme-0.3.0a46.tar`

### file list

```diff
@@ -1,502 +1,508 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/
--rw-r--r--   0 root         (0) root         (0)    35121 2023-05-28 06:20:09.000000 otpme-0.3.0a45/LICENSE
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-10 16:25:47.000000 otpme-0.3.0a45/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-23 07:04:10.077535 otpme-0.3.0a45/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3821 2023-05-28 06:20:09.000000 otpme-0.3.0a45/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.037535 otpme-0.3.0a45/bash_completion/
--rw-r--r--   0 root         (0) root         (0)     1937 2023-06-14 14:55:51.000000 otpme-0.3.0a45/bash_completion/otpme
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.037535 otpme-0.3.0a45/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/deploy/dicts/
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/abbreviations-it.gz
--rw-r--r--   0 root         (0) root         (0)    18683 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/at-surnames.gz
--rw-r--r--   0 root         (0) root         (0)   197269 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/common-passwords.gz
--rwxr-xr-x   0 root         (0) root         (0)      532 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/convert_dict.sh
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/de-female.gz
--rw-r--r--   0 root         (0) root         (0)     3070 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/de-male.gz
--rw-r--r--   0 root         (0) root         (0)    11343 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/de-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    34845 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/de-top10000.gz
--rw-r--r--   0 root         (0) root         (0)    30600 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/en-top10000.gz
--rw-r--r--   0 root         (0) root         (0)   127983 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/english-guessing.gz
--rw-r--r--   0 root         (0) root         (0)  1041710 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/english.gz
--rw-r--r--   0 root         (0) root         (0)   547291 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/german-guessing.gz
--rw-r--r--   0 root         (0) root         (0)   544600 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/german.gz
--rw-r--r--   0 root         (0) root         (0)    13539 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/us-female.gz
--rw-r--r--   0 root         (0) root         (0)     4089 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/us-male.gz
--rw-r--r--   0 root         (0) root         (0)    35682 2023-06-07 15:39:48.000000 otpme-0.3.0a45/deploy/dicts/us-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    13208 2023-06-23 06:36:14.000000 otpme-0.3.0a45/deploy/otpme.conf.dist
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/deploy/pam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/deploy/pam/pam-python/
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-10 16:25:47.000000 otpme-0.3.0a45/deploy/pam/pam-python/README
--rw-r--r--   0 root         (0) root         (0)     2436 2023-05-28 06:20:09.000000 otpme-0.3.0a45/deploy/pam/pam_otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/deploy/schema/
--rw-r--r--   0 root         (0) root         (0)    21610 2023-05-28 06:20:09.000000 otpme-0.3.0a45/deploy/schema/core.schema
--rw-r--r--   0 root         (0) root         (0)    73993 2023-05-28 06:20:09.000000 otpme-0.3.0a45/deploy/schema/cosine.schema
--rw-r--r--   0 root         (0) root         (0)     6267 2023-05-28 06:20:09.000000 otpme-0.3.0a45/deploy/schema/inetorgperson.schema
--rw-r--r--   0 root         (0) root         (0)     7632 2023-05-28 06:20:09.000000 otpme-0.3.0a45/deploy/schema/nis.schema
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/deploy/scripts/
--rw-r--r--   0 root         (0) root         (0)     8600 2023-06-21 09:07:52.000000 otpme-0.3.0a45/deploy/scripts/agent_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-21 09:07:52.000000 otpme-0.3.0a45/deploy/scripts/auth_script.sh
--rw-r--r--   0 root         (0) root         (0)    21137 2023-06-21 09:07:52.000000 otpme-0.3.0a45/deploy/scripts/key_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-21 09:07:52.000000 otpme-0.3.0a45/deploy/scripts/login_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-21 09:07:52.000000 otpme-0.3.0a45/deploy/scripts/push_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/otpme/
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-23 07:03:44.000000 otpme-0.3.0a45/otpme/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11946 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.045535 otpme-0.3.0a45/otpme/lib/
--rw-r--r--   0 root         (0) root         (0)    12877 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-05-28 07:43:31.000000 otpme-0.3.0a45/otpme/lib/arp.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/auth_script.py
--rw-r--r--   0 root         (0) root         (0)    45358 2023-06-17 12:43:00.000000 otpme-0.3.0a45/otpme/lib/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.045535 otpme-0.3.0a45/otpme/lib/backends/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.049535 otpme-0.3.0a45/otpme/lib/backends/file/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/backends/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89733 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/backends/file/file.py
--rw-r--r--   0 root         (0) root         (0)    13013 2023-06-15 11:38:21.000000 otpme-0.3.0a45/otpme/lib/backends/file/index.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/backends/file/models.py
--rw-r--r--   0 root         (0) root         (0)    74192 2023-06-07 16:05:20.000000 otpme-0.3.0a45/otpme/lib/backends/file/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.049535 otpme-0.3.0a45/otpme/lib/cache/
--rw-r--r--   0 root         (0) root         (0)    33856 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/cache/dogpile.py
--rw-r--r--   0 root         (0) root         (0)    19991 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/cache/funccache.py
--rw-r--r--   0 root         (0) root         (0)     3538 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/cache/lru.py
--rw-r--r--   0 root         (0) root         (0)    13901 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/cache/memcache.py
--rw-r--r--   0 root         (0) root         (0)     6500 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/cache/memcached.py
--rw-r--r--   0 root         (0) root         (0)     7344 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/cache/memcachedb.py
--rw-r--r--   0 root         (0) root         (0)    26853 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.053535 otpme-0.3.0a45/otpme/lib/classes/
--rw-r--r--   0 root         (0) root         (0)      917 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85744 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)    14874 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/agent_conn.py
--rw-r--r--   0 root         (0) root         (0)   127394 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/classes/auth_handler.py
--rw-r--r--   0 root         (0) root         (0)    54320 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/ca.py
--rw-r--r--   0 root         (0) root         (0)    40376 2023-06-21 16:57:55.000000 otpme-0.3.0a45/otpme/lib/classes/client.py
--rw-r--r--   0 root         (0) root         (0)   209927 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/classes/command_handler.py
--rw-r--r--   0 root         (0) root         (0)     8601 2023-06-18 08:42:43.000000 otpme-0.3.0a45/otpme/lib/classes/conn_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.053535 otpme-0.3.0a45/otpme/lib/classes/data_objects/
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/cert.py
--rw-r--r--   0 root         (0) root         (0)     6543 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/failed_pass.py
--rw-r--r--   0 root         (0) root         (0)     7679 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/last_assigned_id.py
--rw-r--r--   0 root         (0) root         (0)    10578 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/revoked_signature.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/rsa_key.py
--rw-r--r--   0 root         (0) root         (0)     7020 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/skip_sync.py
--rw-r--r--   0 root         (0) root         (0)     5762 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/token_counter.py
--rw-r--r--   0 root         (0) root         (0)     5646 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/used_hash.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/used_otp.py
--rw-r--r--   0 root         (0) root         (0)     5723 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/used_slp.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/data_objects/used_sotp.py
--rw-r--r--   0 root         (0) root         (0)    28183 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    38860 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/group.py
--rw-r--r--   0 root         (0) root         (0)    49804 2023-06-13 10:56:05.000000 otpme-0.3.0a45/otpme/lib/classes/host.py
--rw-r--r--   0 root         (0) root         (0)    11992 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/login_handler.py
--rw-r--r--   0 root         (0) root         (0)     5500 2023-06-14 12:42:13.000000 otpme-0.3.0a45/otpme/lib/classes/mgmt_client.py
--rw-r--r--   0 root         (0) root         (0)    33067 2023-06-13 10:57:04.000000 otpme-0.3.0a45/otpme/lib/classes/node.py
--rw-r--r--   0 root         (0) root         (0)    21597 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/classes/object_config.py
--rw-r--r--   0 root         (0) root         (0)    76766 2023-06-13 08:06:14.000000 otpme-0.3.0a45/otpme/lib/classes/otpme_agent.py
--rw-r--r--   0 root         (0) root         (0)    49375 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/otpme_host.py
--rw-r--r--   0 root         (0) root         (0)   300315 2023-06-22 09:44:36.000000 otpme-0.3.0a45/otpme/lib/classes/otpme_object.py
--rw-r--r--   0 root         (0) root         (0)    22938 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/policy.py
--rw-r--r--   0 root         (0) root         (0)    63265 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/realm.py
--rw-r--r--   0 root         (0) root         (0)    61677 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/resolver.py
--rw-r--r--   0 root         (0) root         (0)    44644 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/role.py
--rw-r--r--   0 root         (0) root         (0)    33753 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/script.py
--rw-r--r--   0 root         (0) root         (0)    56576 2023-06-16 07:04:42.000000 otpme-0.3.0a45/otpme/lib/classes/session.py
--rw-r--r--   0 root         (0) root         (0)    31485 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/signing.py
--rw-r--r--   0 root         (0) root         (0)   105067 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/site.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/classes/ssh_agent.py
--rw-r--r--   0 root         (0) root         (0)   132558 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/token.py
--rw-r--r--   0 root         (0) root         (0)    49045 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/classes/unit.py
--rw-r--r--   0 root         (0) root         (0)   170349 2023-06-22 09:44:36.000000 otpme-0.3.0a45/otpme/lib/classes/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.053535 otpme-0.3.0a45/otpme/lib/cli/
--rw-r--r--   0 root         (0) root         (0)    64756 2023-06-22 14:13:01.000000 otpme-0.3.0a45/otpme/lib/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12995 2023-06-13 14:13:02.000000 otpme-0.3.0a45/otpme/lib/cli/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     7091 2023-06-13 10:39:51.000000 otpme-0.3.0a45/otpme/lib/cli/ca.py
--rw-r--r--   0 root         (0) root         (0)    13451 2023-06-13 10:40:55.000000 otpme-0.3.0a45/otpme/lib/cli/client.py
--rw-r--r--   0 root         (0) root         (0)     5615 2023-06-13 10:42:30.000000 otpme-0.3.0a45/otpme/lib/cli/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    13271 2023-06-13 10:44:18.000000 otpme-0.3.0a45/otpme/lib/cli/group.py
--rw-r--r--   0 root         (0) root         (0)    13349 2023-06-13 10:44:40.000000 otpme-0.3.0a45/otpme/lib/cli/host.py
--rw-r--r--   0 root         (0) root         (0)    11183 2023-06-13 10:57:59.000000 otpme-0.3.0a45/otpme/lib/cli/node.py
--rw-r--r--   0 root         (0) root         (0)     6137 2023-06-13 12:23:35.000000 otpme-0.3.0a45/otpme/lib/cli/policy.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-06-13 12:25:33.000000 otpme-0.3.0a45/otpme/lib/cli/realm.py
--rw-r--r--   0 root         (0) root         (0)     6572 2023-06-13 12:39:16.000000 otpme-0.3.0a45/otpme/lib/cli/resolver.py
--rw-r--r--   0 root         (0) root         (0)    21218 2023-06-13 12:31:39.000000 otpme-0.3.0a45/otpme/lib/cli/role.py
--rw-r--r--   0 root         (0) root         (0)     7355 2023-06-13 12:32:22.000000 otpme-0.3.0a45/otpme/lib/cli/script.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-06-13 12:33:04.000000 otpme-0.3.0a45/otpme/lib/cli/site.py
--rw-r--r--   0 root         (0) root         (0)    16298 2023-06-13 12:40:35.000000 otpme-0.3.0a45/otpme/lib/cli/token.py
--rw-r--r--   0 root         (0) root         (0)     5391 2023-06-13 11:24:43.000000 otpme-0.3.0a45/otpme/lib/cli/unit.py
--rw-r--r--   0 root         (0) root         (0)     7604 2023-06-13 10:31:45.000000 otpme-0.3.0a45/otpme/lib/cli/user.py
--rw-r--r--   0 root         (0) root         (0)    24404 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/compgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.053535 otpme-0.3.0a45/otpme/lib/compression/
--rw-r--r--   0 root         (0) root         (0)      514 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3941 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/compression/base.py
--rw-r--r--   0 root         (0) root         (0)    11149 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/connections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/daemon/
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/authd.py
--rw-r--r--   0 root         (0) root         (0)    99221 2023-06-21 07:35:11.000000 otpme-0.3.0a45/otpme/lib/daemon/clusterd.py
--rw-r--r--   0 root         (0) root         (0)    44813 2023-06-16 12:22:59.000000 otpme-0.3.0a45/otpme/lib/daemon/controld.py
--rw-r--r--   0 root         (0) root         (0)    73948 2023-06-16 15:46:57.000000 otpme-0.3.0a45/otpme/lib/daemon/hostd.py
--rw-r--r--   0 root         (0) root         (0)     3141 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/joind.py
--rw-r--r--   0 root         (0) root         (0)     6780 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/ldapd.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/mgmtd.py
--rw-r--r--   0 root         (0) root         (0)    15556 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/daemon/otpme_daemon.py
--rw-r--r--   0 root         (0) root         (0)    11048 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/scriptd.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/daemon/syncd.py
--rw-r--r--   0 root         (0) root         (0)     6888 2023-06-16 07:04:42.000000 otpme-0.3.0a45/otpme/lib/daemon/unix_daemon.py
--rw-r--r--   0 root         (0) root         (0)    19072 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/debug.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/encoding/
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encoding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encoding/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/encryption/
--rw-r--r--   0 root         (0) root         (0)     4020 2023-06-13 15:59:53.000000 otpme-0.3.0a45/otpme/lib/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3362 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/aes.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/aes_cfb.py
--rw-r--r--   0 root         (0) root         (0)     7967 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/argon2.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/asymmetric_key_handler.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/ec.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/fernet.py
--rw-r--r--   0 root         (0) root         (0)     3304 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/hkdf.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/pbkdf2.py
--rw-r--r--   0 root         (0) root         (0)     7891 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/encryption/rsa.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-20 07:02:59.000000 otpme-0.3.0a45/otpme/lib/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/extensions/
--rw-r--r--   0 root         (0) root         (0)      396 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/extensions/base/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/extensions/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11447 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/extensions/base/base.py
--rw-r--r--   0 root         (0) root         (0)    40105 2023-06-22 09:44:36.000000 otpme-0.3.0a45/otpme/lib/extensions/ldif_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/extensions/posix/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/extensions/posix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15729 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/extensions/posix/posix.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/extensions/utils.py
--rw-r--r--   0 root         (0) root         (0)    36868 2023-06-19 07:37:16.000000 otpme-0.3.0a45/otpme/lib/filetools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/freeradius/
--rw-r--r--   0 root         (0) root         (0)     9274 2023-06-21 16:57:55.000000 otpme-0.3.0a45/otpme/lib/freeradius/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18752 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/freeradius/otpme.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/freeradius/radiusd.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/freeradius/radiusd_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.057535 otpme-0.3.0a45/otpme/lib/gpg/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/gpg/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    28565 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/gpg/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.061535 otpme-0.3.0a45/otpme/lib/help/
--rwxr-xr-x   0 root         (0) root         (0)    26596 2023-06-14 10:24:54.000000 otpme-0.3.0a45/otpme/lib/help/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22571 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/help/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     5552 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/agent.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-06-21 16:57:55.000000 otpme-0.3.0a45/otpme/lib/help/auth.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/ca.py
--rw-r--r--   0 root         (0) root         (0)    16524 2023-06-13 16:04:18.000000 otpme-0.3.0a45/otpme/lib/help/client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-16 07:04:42.000000 otpme-0.3.0a45/otpme/lib/help/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/controld.py
--rw-r--r--   0 root         (0) root         (0)    10976 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/dictionary.py
--rw-r--r--   0 root         (0) root         (0)      589 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/get_authorized_keys.py
--rw-r--r--   0 root         (0) root         (0)    19149 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/group.py
--rw-r--r--   0 root         (0) root         (0)    23587 2023-06-14 09:26:28.000000 otpme-0.3.0a45/otpme/lib/help/host.py
--rw-r--r--   0 root         (0) root         (0)    21011 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/help/node.py
--rw-r--r--   0 root         (0) root         (0)      544 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/pinentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.061535 otpme-0.3.0a45/otpme/lib/help/policy/
--rw-r--r--   0 root         (0) root         (0)     8665 2023-06-14 08:30:14.000000 otpme-0.3.0a45/otpme/lib/help/policy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3777 2023-06-14 08:27:26.000000 otpme-0.3.0a45/otpme/lib/help/policy/authonaction.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-06-14 08:27:32.000000 otpme-0.3.0a45/otpme/lib/help/policy/autodisable.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-14 08:27:36.000000 otpme-0.3.0a45/otpme/lib/help/policy/defaultgroups.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-14 08:27:38.000000 otpme-0.3.0a45/otpme/lib/help/policy/defaultpolicies.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-06-14 08:27:40.000000 otpme-0.3.0a45/otpme/lib/help/policy/defaultroles.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-06-14 08:27:42.000000 otpme-0.3.0a45/otpme/lib/help/policy/defaultunits.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-14 08:27:51.000000 otpme-0.3.0a45/otpme/lib/help/policy/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-14 08:27:53.000000 otpme-0.3.0a45/otpme/lib/help/policy/idrange.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-06-14 08:28:15.000000 otpme-0.3.0a45/otpme/lib/help/policy/logintimes.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-14 08:28:17.000000 otpme-0.3.0a45/otpme/lib/help/policy/objecttemplates.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-06-14 08:28:18.000000 otpme-0.3.0a45/otpme/lib/help/policy/password.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-06-14 08:28:20.000000 otpme-0.3.0a45/otpme/lib/help/policy/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)    19622 2023-06-10 16:25:47.000000 otpme-0.3.0a45/otpme/lib/help/realm.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.061535 otpme-0.3.0a45/otpme/lib/help/resolver/
--rw-r--r--   0 root         (0) root         (0)    11252 2023-06-14 08:30:52.000000 otpme-0.3.0a45/otpme/lib/help/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4381 2023-06-14 08:26:48.000000 otpme-0.3.0a45/otpme/lib/help/resolver/ldap.py
--rw-r--r--   0 root         (0) root         (0)    17945 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/role.py
--rw-r--r--   0 root         (0) root         (0)    14711 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/script.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/help/session.py
--rw-r--r--   0 root         (0) root         (0)    21392 2023-06-10 16:25:47.000000 otpme-0.3.0a45/otpme/lib/help/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.061535 otpme-0.3.0a45/otpme/lib/help/token/
--rw-r--r--   0 root         (0) root         (0)    19325 2023-06-11 17:59:47.000000 otpme-0.3.0a45/otpme/lib/help/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/fido2.py
--rw-r--r--   0 root         (0) root         (0)     6369 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/hotp.py
--rw-r--r--   0 root         (0) root         (0)     6406 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/motp.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/otp_push.py
--rw-r--r--   0 root         (0) root         (0)     5018 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/otpme.py
--rw-r--r--   0 root         (0) root         (0)     3947 2023-06-14 09:40:07.000000 otpme-0.3.0a45/otpme/lib/help/token/password.py
--rw-r--r--   0 root         (0) root         (0)     7318 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/ssh.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/totp.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-06-18 06:44:27.000000 otpme-0.3.0a45/otpme/lib/help/token/yubikey_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-11 17:59:47.000000 otpme-0.3.0a45/otpme/lib/help/token/yubikey_hotp.py
--rw-r--r--   0 root         (0) root         (0)    23731 2023-06-19 06:14:28.000000 otpme-0.3.0a45/otpme/lib/help/tool.py
--rw-r--r--   0 root         (0) root         (0)    14774 2023-06-10 16:25:47.000000 otpme-0.3.0a45/otpme/lib/help/unit.py
--rw-r--r--   0 root         (0) root         (0)    28280 2023-06-14 09:25:52.000000 otpme-0.3.0a45/otpme/lib/help/user.py
--rw-r--r--   0 root         (0) root         (0)    16367 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/host.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.061535 otpme-0.3.0a45/otpme/lib/humanize/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/humanize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/humanize/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.061535 otpme-0.3.0a45/otpme/lib/index/
--rw-r--r--   0 root         (0) root         (0)      449 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23971 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/index/mysql.py
--rw-r--r--   0 root         (0) root         (0)    24446 2023-06-21 09:11:38.000000 otpme-0.3.0a45/otpme/lib/index/postgres.py
--rw-r--r--   0 root         (0) root         (0)     8403 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/index/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/job/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18955 2023-06-22 09:44:36.000000 otpme-0.3.0a45/otpme/lib/job/callback.py
--rw-r--r--   0 root         (0) root         (0)    12568 2023-06-22 09:44:36.000000 otpme-0.3.0a45/otpme/lib/job/otpme_job.py
--rw-r--r--   0 root         (0) root         (0)    36904 2023-06-20 13:23:33.000000 otpme-0.3.0a45/otpme/lib/join.py
--rw-r--r--   0 root         (0) root         (0)     4924 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/json.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/ldap/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/ldap/client.py
--rw-r--r--   0 root         (0) root         (0)    11129 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/ldap/schema.py
--rw-r--r--   0 root         (0) root         (0)    49844 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/ldap/server.py
--rw-r--r--   0 root         (0) root         (0)    18710 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/locking.py
--rw-r--r--   0 root         (0) root         (0)     9515 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/log.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/messages.py
--rw-r--r--   0 root         (0) root         (0)     6048 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/mschap.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/mschap_util.py
--rw-r--r--   0 root         (0) root         (0)    35675 2023-06-20 11:37:02.000000 otpme-0.3.0a45/otpme/lib/multiprocessing.py
--rw-r--r--   0 root         (0) root         (0)    10033 2023-05-28 07:38:27.000000 otpme-0.3.0a45/otpme/lib/net.py
--rw-r--r--   0 root         (0) root         (0)    25699 2023-06-19 06:14:28.000000 otpme-0.3.0a45/otpme/lib/nsscache.py
--rw-r--r--   0 root         (0) root         (0)    63395 2023-06-19 06:14:28.000000 otpme-0.3.0a45/otpme/lib/offline_token.py
--rw-r--r--   0 root         (0) root         (0)    24416 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/oid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/otp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/otp/oath/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/oath/hotp.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/oath/totp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/otp/otpme/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/otp/yubico/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/yubico/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otp/yubico/yubiotp.py
--rw-r--r--   0 root         (0) root         (0)    19754 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otpme_acl.py
--rw-r--r--   0 root         (0) root         (0)   112530 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/otpme_config.py
--rw-r--r--   0 root         (0) root         (0)     3586 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/otpme_pass.py
--rw-r--r--   0 root         (0) root         (0)    70426 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pam.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pickle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/pinentry/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pinentry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27532 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pinentry/pinentry.py
--rwxr-xr-x   0 root         (0) root         (0)     7947 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pinentry/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/pki/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pki/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9864 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pki/cert.py
--rw-r--r--   0 root         (0) root         (0)    22943 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/pki/utils.py
--rw-r--r--   0 root         (0) root         (0)    16957 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/pki/utils_openssl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/authonaction/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/authonaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32525 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/authonaction/authonaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/autodisable/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/autodisable/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17448 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/autodisable/autodisable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/defaultgroups/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/defaultgroups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17153 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/defaultgroups/defaultgroups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/defaultpolicies/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/defaultpolicies/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/defaultpolicies/defaultpolicies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/defaultroles/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/policy/defaultroles/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13849 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/defaultroles/defaultroles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/defaultunits/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/policy/defaultunits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15386 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/defaultunits/defaultunits.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/forcetoken/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/forcetoken/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13989 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/forcetoken/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/idrange/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/idrange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27087 2023-06-22 09:44:36.000000 otpme-0.3.0a45/otpme/lib/policy/idrange/idrange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/logintimes/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/logintimes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22816 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/logintimes/logintimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/objecttemplates/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/objecttemplates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14703 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/objecttemplates/objecttemplates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.065535 otpme-0.3.0a45/otpme/lib/policy/password/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28730 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/policy/tokenacls/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/tokenacls/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24736 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/policy/tokenacls/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     8921 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/preload.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/protocols/
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/protocols/client/
--rw-r--r--   0 root         (0) root         (0)      722 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/client/agent1.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/client/auth1.py
--rw-r--r--   0 root         (0) root         (0)    13302 2023-06-18 16:35:06.000000 otpme-0.3.0a45/otpme/lib/protocols/client/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/client/get_class.py
--rw-r--r--   0 root         (0) root         (0)     4712 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/client/host1.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/client/join1.py
--rwxr-xr-x   0 root         (0) root         (0)    11372 2023-06-14 14:28:57.000000 otpme-0.3.0a45/otpme/lib/protocols/client/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    66489 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/protocols/client/sync1.py
--rw-r--r--   0 root         (0) root         (0)   158940 2023-06-19 14:51:10.000000 otpme-0.3.0a45/otpme/lib/protocols/otpme_client.py
--rw-r--r--   0 root         (0) root         (0)    77419 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/protocols/otpme_server.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/request.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/protocols/server/
--rw-r--r--   0 root         (0) root         (0)      894 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40286 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/server/agent1.py
--rw-r--r--   0 root         (0) root         (0)    13083 2023-06-23 06:36:14.000000 otpme-0.3.0a45/otpme/lib/protocols/server/auth1.py
--rw-r--r--   0 root         (0) root         (0)    30300 2023-06-20 13:06:45.000000 otpme-0.3.0a45/otpme/lib/protocols/server/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/protocols/server/get_class.py
--rw-r--r--   0 root         (0) root         (0)    25856 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/protocols/server/host1.py
--rw-r--r--   0 root         (0) root         (0)    50743 2023-06-19 07:44:27.000000 otpme-0.3.0a45/otpme/lib/protocols/server/join1.py
--rw-r--r--   0 root         (0) root         (0)    55241 2023-06-15 11:38:21.000000 otpme-0.3.0a45/otpme/lib/protocols/server/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    46007 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/protocols/server/sync1.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/protocols/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     6712 2023-06-07 15:39:48.000000 otpme-0.3.0a45/otpme/lib/protocols/utils.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/push_script.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/register/
--rw-r--r--   0 root         (0) root         (0)     9783 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/register/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/resolver/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/resolver/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/resolver/ldap/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/resolver/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35657 2023-06-19 13:21:58.000000 otpme-0.3.0a45/otpme/lib/resolver/ldap/ldap.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/resolver/utils.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/script.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/sign_key_cache.py
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/slp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/smartcard/
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/smartcard/fido2/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10228 2023-06-11 17:59:47.000000 otpme-0.3.0a45/otpme/lib/smartcard/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-06-11 17:59:47.000000 otpme-0.3.0a45/otpme/lib/smartcard/get_class.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/smartcard/yubikey/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12018 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey/usb.py
--rw-r--r--   0 root         (0) root         (0)     8142 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey/yubikey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_gpg/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_gpg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6431 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.069535 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12022 2023-06-11 17:59:47.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hotp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-11 17:59:47.000000 otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/socket/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/socket/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13129 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/socket/connect.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/socket/handler.py
--rw-r--r--   0 root         (0) root         (0)    30823 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/socket/listen.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/socket/send_recv1.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/sotp.py
--rwxr-xr-x   0 root         (0) root         (0)    37180 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/spsc.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/srp.py
--rw-r--r--   0 root         (0) root         (0)    23521 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/ssh.py
--rw-r--r--   0 root         (0) root         (0)    61848 2023-06-16 07:04:42.000000 otpme-0.3.0a45/otpme/lib/stuff.py
--rw-r--r--   0 root         (0) root         (0)    12345 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/sync_cache.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/system_command.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/
--rw-r--r--   0 root         (0) root         (0)     1981 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/advanced.py
--rw-r--r--   0 root         (0) root         (0)     9859 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/caching_query.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/environment.py
--rw-r--r--   0 root         (0) root         (0)     1764 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/fixture_data.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/helloworld.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/local_session_caching.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/model.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/relationship_caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/caches/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/caches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9083 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/caches/caches.py
--rw-r--r--   0 root         (0) root         (0)    14341 2023-06-04 07:15:00.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/caches/files.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/config.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/error.py
--rw-r--r--   0 root         (0) root         (0)     7963 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/group.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/maps.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/passwd.py
--rw-r--r--   0 root         (0) root         (0)     2387 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/shadow.py
--rw-r--r--   0 root         (0) root         (0)     4140 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/nss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/files_updater.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/map_updater.py
--rw-r--r--   0 root         (0) root         (0)    10980 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/updater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4117 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/nss_cache/util/file_formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/third_party/oath_toolkit/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/oath_toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/oath_toolkit/_compat.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/third_party/oath_toolkit/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/token/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/token/fido2/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14964 2023-06-13 12:38:43.000000 otpme-0.3.0a45/otpme/lib/token/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)     1123 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/token/hotp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55042 2023-06-18 16:35:06.000000 otpme-0.3.0a45/otpme/lib/token/hotp/hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.073535 otpme-0.3.0a45/otpme/lib/token/link/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/link/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9709 2023-06-13 12:38:47.000000 otpme-0.3.0a45/otpme/lib/token/link/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/motp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/motp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27734 2023-06-13 12:38:49.000000 otpme-0.3.0a45/otpme/lib/token/motp/motp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/otp_push/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/otp_push/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23418 2023-06-13 12:40:08.000000 otpme-0.3.0a45/otpme/lib/token/otp_push/otp_push.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/otpme/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24757 2023-06-13 12:38:50.000000 otpme-0.3.0a45/otpme/lib/token/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/password/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26093 2023-06-13 12:38:54.000000 otpme-0.3.0a45/otpme/lib/token/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/script_otp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/script_otp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9744 2023-06-13 12:44:34.000000 otpme-0.3.0a45/otpme/lib/token/script_otp/script_otp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/script_static/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/script_static/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9744 2023-06-13 12:44:34.000000 otpme-0.3.0a45/otpme/lib/token/script_static/script_static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/ssh/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39544 2023-06-13 12:38:59.000000 otpme-0.3.0a45/otpme/lib/token/ssh/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/totp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/totp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49493 2023-06-13 12:39:00.000000 otpme-0.3.0a45/otpme/lib/token/totp/totp.py
--rw-r--r--   0 root         (0) root         (0)      547 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.077535 otpme-0.3.0a45/otpme/lib/token/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-28 06:20:09.000000 otpme-0.3.0a45/otpme/lib/token/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25150 2023-06-13 12:39:02.000000 otpme-0.3.0a45/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:04:10.041535 otpme-0.3.0a45/otpme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13171 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1081 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      904 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 07:04:09.000000 otpme-0.3.0a45/otpme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:04:10.077535 otpme-0.3.0a45/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8488 2023-06-22 14:13:01.000000 otpme-0.3.0a45/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/
+-rw-r--r--   0 root         (0) root         (0)    35121 2023-06-24 05:09:50.000000 otpme-0.3.0a46/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-24 05:09:50.000000 otpme-0.3.0a46/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-24 05:09:50.962409 otpme-0.3.0a46/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-06-24 05:09:50.000000 otpme-0.3.0a46/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.926408 otpme-0.3.0a46/bash_completion/
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-06-24 05:09:50.000000 otpme-0.3.0a46/bash_completion/otpme
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.926408 otpme-0.3.0a46/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.926408 otpme-0.3.0a46/deploy/dicts/
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/abbreviations-it.gz
+-rw-r--r--   0 root         (0) root         (0)    18683 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/at-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)   197269 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/common-passwords.gz
+-rwxr-xr-x   0 root         (0) root         (0)      532 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/convert_dict.sh
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-female.gz
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-male.gz
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    34845 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)    30600 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/en-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)   127983 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/english-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)  1041710 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/english.gz
+-rw-r--r--   0 root         (0) root         (0)   547291 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/german-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)   544600 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/german.gz
+-rw-r--r--   0 root         (0) root         (0)    13539 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/us-female.gz
+-rw-r--r--   0 root         (0) root         (0)     4089 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/us-male.gz
+-rw-r--r--   0 root         (0) root         (0)    35682 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/us-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    13208 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/otpme.conf.dist
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/pam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/pam/pam-python/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/pam/pam-python/README
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/pam/pam_otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/radius/
+-rw-r--r--   0 root         (0) root         (0)    13085 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/radius/dictionary
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/radius/dictionary.freeradius
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/schema/
+-rw-r--r--   0 root         (0) root         (0)    21610 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/core.schema
+-rw-r--r--   0 root         (0) root         (0)    73993 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/cosine.schema
+-rw-r--r--   0 root         (0) root         (0)     6267 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/inetorgperson.schema
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/nis.schema
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/scripts/
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/agent_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/auth_script.sh
+-rw-r--r--   0 root         (0) root         (0)    21137 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/key_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/login_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/push_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/otpme/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11946 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/
+-rw-r--r--   0 root         (0) root         (0)    12877 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/arp.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/auth_script.py
+-rw-r--r--   0 root         (0) root         (0)    45358 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/backends/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/backends/file/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89733 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/file.py
+-rw-r--r--   0 root         (0) root         (0)    13013 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/index.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/models.py
+-rw-r--r--   0 root         (0) root         (0)    74192 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/cache/
+-rw-r--r--   0 root         (0) root         (0)    33856 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)    19991 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/funccache.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/lru.py
+-rw-r--r--   0 root         (0) root         (0)    13901 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/memcache.py
+-rw-r--r--   0 root         (0) root         (0)     6500 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/memcached.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/memcachedb.py
+-rw-r--r--   0 root         (0) root         (0)    26853 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.938408 otpme-0.3.0a46/otpme/lib/classes/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85744 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)    14874 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/agent_conn.py
+-rw-r--r--   0 root         (0) root         (0)   127394 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/auth_handler.py
+-rw-r--r--   0 root         (0) root         (0)    54320 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/ca.py
+-rw-r--r--   0 root         (0) root         (0)    40376 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/client.py
+-rw-r--r--   0 root         (0) root         (0)   210451 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/command_handler.py
+-rw-r--r--   0 root         (0) root         (0)     8601 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/conn_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/classes/data_objects/
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/cert.py
+-rw-r--r--   0 root         (0) root         (0)     6543 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/failed_pass.py
+-rw-r--r--   0 root         (0) root         (0)     7679 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/last_assigned_id.py
+-rw-r--r--   0 root         (0) root         (0)    10578 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/revoked_signature.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/rsa_key.py
+-rw-r--r--   0 root         (0) root         (0)     7020 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/skip_sync.py
+-rw-r--r--   0 root         (0) root         (0)     5762 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/token_counter.py
+-rw-r--r--   0 root         (0) root         (0)     5646 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_hash.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_otp.py
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_slp.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_sotp.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    38860 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/group.py
+-rw-r--r--   0 root         (0) root         (0)    49804 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/host.py
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/login_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5500 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/mgmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    33067 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/node.py
+-rw-r--r--   0 root         (0) root         (0)    21597 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/object_config.py
+-rw-r--r--   0 root         (0) root         (0)    76766 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/otpme_agent.py
+-rw-r--r--   0 root         (0) root         (0)    49375 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/otpme_host.py
+-rw-r--r--   0 root         (0) root         (0)   300315 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/otpme_object.py
+-rw-r--r--   0 root         (0) root         (0)    22938 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/policy.py
+-rw-r--r--   0 root         (0) root         (0)    63265 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/realm.py
+-rw-r--r--   0 root         (0) root         (0)    61677 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    44644 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/role.py
+-rw-r--r--   0 root         (0) root         (0)    33753 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/script.py
+-rw-r--r--   0 root         (0) root         (0)    56576 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/session.py
+-rw-r--r--   0 root         (0) root         (0)    31485 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/signing.py
+-rw-r--r--   0 root         (0) root         (0)   104716 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/site.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/ssh_agent.py
+-rw-r--r--   0 root         (0) root         (0)   132552 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/token.py
+-rw-r--r--   0 root         (0) root         (0)    49045 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/unit.py
+-rw-r--r--   0 root         (0) root         (0)   170349 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/cli/
+-rw-r--r--   0 root         (0) root         (0)    64756 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12995 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/ca.py
+-rw-r--r--   0 root         (0) root         (0)    13451 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/client.py
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    13271 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/group.py
+-rw-r--r--   0 root         (0) root         (0)    13349 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/host.py
+-rw-r--r--   0 root         (0) root         (0)    11183 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/node.py
+-rw-r--r--   0 root         (0) root         (0)     6137 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/realm.py
+-rw-r--r--   0 root         (0) root         (0)     6572 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    21218 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/role.py
+-rw-r--r--   0 root         (0) root         (0)     7355 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/script.py
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/site.py
+-rw-r--r--   0 root         (0) root         (0)    16298 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/token.py
+-rw-r--r--   0 root         (0) root         (0)     5391 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/unit.py
+-rw-r--r--   0 root         (0) root         (0)     7604 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/user.py
+-rw-r--r--   0 root         (0) root         (0)    24404 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/compgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/compression/
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3941 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/compression/base.py
+-rw-r--r--   0 root         (0) root         (0)    11149 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/connections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/daemon/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/authd.py
+-rw-r--r--   0 root         (0) root         (0)    99221 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/clusterd.py
+-rw-r--r--   0 root         (0) root         (0)    44813 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/controld.py
+-rw-r--r--   0 root         (0) root         (0)    73948 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/hostd.py
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/joind.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/ldapd.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/mgmtd.py
+-rw-r--r--   0 root         (0) root         (0)    15556 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/otpme_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    11048 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/scriptd.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/syncd.py
+-rw-r--r--   0 root         (0) root         (0)     6888 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/unix_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/debug.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/encoding/
+-rw-r--r--   0 root         (0) root         (0)      496 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encoding/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/encryption/
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/aes.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/aes_cfb.py
+-rw-r--r--   0 root         (0) root         (0)     7967 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/argon2.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/asymmetric_key_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/ec.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/fernet.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/hkdf.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/pbkdf2.py
+-rw-r--r--   0 root         (0) root         (0)     7891 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/rsa.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/extensions/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/extensions/base/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11447 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/base/base.py
+-rw-r--r--   0 root         (0) root         (0)    40105 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/ldif_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/extensions/posix/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/posix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15729 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/posix/posix.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/utils.py
+-rw-r--r--   0 root         (0) root         (0)    36868 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/filetools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/freeradius/
+-rw-r--r--   0 root         (0) root         (0)     9274 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18752 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/radiusd.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/radiusd_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/gpg/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/gpg/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    28565 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/gpg/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/help/
+-rwxr-xr-x   0 root         (0) root         (0)    26596 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22571 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/agent.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/auth.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/ca.py
+-rw-r--r--   0 root         (0) root         (0)    16524 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/controld.py
+-rw-r--r--   0 root         (0) root         (0)    10976 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/get_authorized_keys.py
+-rw-r--r--   0 root         (0) root         (0)    19149 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/group.py
+-rw-r--r--   0 root         (0) root         (0)    23587 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/host.py
+-rw-r--r--   0 root         (0) root         (0)    21011 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/node.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/pinentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/help/policy/
+-rw-r--r--   0 root         (0) root         (0)     8665 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/authonaction.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/autodisable.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultgroups.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultpolicies.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultroles.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultunits.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/idrange.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/logintimes.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/objecttemplates.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/password.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)    19622 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/realm.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/help/resolver/
+-rw-r--r--   0 root         (0) root         (0)    11252 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/resolver/ldap.py
+-rw-r--r--   0 root         (0) root         (0)    17945 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/role.py
+-rw-r--r--   0 root         (0) root         (0)    14711 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/script.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/session.py
+-rw-r--r--   0 root         (0) root         (0)    21392 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/help/token/
+-rw-r--r--   0 root         (0) root         (0)    19325 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/motp.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/otp_push.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/password.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/totp.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/yubikey_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/yubikey_hotp.py
+-rw-r--r--   0 root         (0) root         (0)    23731 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/tool.py
+-rw-r--r--   0 root         (0) root         (0)    14774 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/unit.py
+-rw-r--r--   0 root         (0) root         (0)    28280 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/user.py
+-rw-r--r--   0 root         (0) root         (0)    16367 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/host.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/humanize/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/humanize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/humanize/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/index/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23971 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/mysql.py
+-rw-r--r--   0 root         (0) root         (0)    24446 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     8403 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/job/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18955 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/job/callback.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/job/otpme_job.py
+-rw-r--r--   0 root         (0) root         (0)    36904 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/join.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/json.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/ldap/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/client.py
+-rw-r--r--   0 root         (0) root         (0)    11129 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/schema.py
+-rw-r--r--   0 root         (0) root         (0)    49844 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/server.py
+-rw-r--r--   0 root         (0) root         (0)    18710 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/locking.py
+-rw-r--r--   0 root         (0) root         (0)     9515 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/log.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     6048 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/mschap.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/mschap_util.py
+-rw-r--r--   0 root         (0) root         (0)    35675 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/multiprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    10033 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/net.py
+-rw-r--r--   0 root         (0) root         (0)    25699 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/nsscache.py
+-rw-r--r--   0 root         (0) root         (0)    63395 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/offline_token.py
+-rw-r--r--   0 root         (0) root         (0)    24416 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/oid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/oath/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/oath/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/oath/totp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/otpme/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/yubico/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/yubico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/yubico/yubiotp.py
+-rw-r--r--   0 root         (0) root         (0)    19754 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otpme_acl.py
+-rw-r--r--   0 root         (0) root         (0)   112530 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otpme_config.py
+-rw-r--r--   0 root         (0) root         (0)     3586 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otpme_pass.py
+-rw-r--r--   0 root         (0) root         (0)    70426 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pam.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pickle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/pinentry/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pinentry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27532 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pinentry/pinentry.py
+-rwxr-xr-x   0 root         (0) root         (0)     7947 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pinentry/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/pki/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9864 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/cert.py
+-rw-r--r--   0 root         (0) root         (0)    22943 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16957 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/utils_openssl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/authonaction/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/authonaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32525 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/authonaction/authonaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/autodisable/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/autodisable/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17448 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/autodisable/autodisable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultgroups/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultgroups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17153 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultgroups/defaultgroups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/defaultpolicies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultroles/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultroles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13849 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultroles/defaultroles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultunits/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultunits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15386 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultunits/defaultunits.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/forcetoken/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/forcetoken/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13989 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/forcetoken/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/idrange/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/idrange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27087 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/idrange/idrange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/logintimes/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/logintimes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22816 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/logintimes/logintimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/objecttemplates/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/objecttemplates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14703 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/objecttemplates/objecttemplates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/password/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28730 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/tokenacls/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/tokenacls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24736 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/tokenacls/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8921 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/preload.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/protocols/
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/protocols/client/
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/agent1.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    13302 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/host1.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/join1.py
+-rwxr-xr-x   0 root         (0) root         (0)    11372 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    66489 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/sync1.py
+-rw-r--r--   0 root         (0) root         (0)   158940 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/otpme_client.py
+-rw-r--r--   0 root         (0) root         (0)    77419 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/otpme_server.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/request.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/protocols/server/
+-rw-r--r--   0 root         (0) root         (0)      894 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40286 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/agent1.py
+-rw-r--r--   0 root         (0) root         (0)    13083 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    30300 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/get_class.py
+-rw-r--r--   0 root         (0) root         (0)    25856 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/host1.py
+-rw-r--r--   0 root         (0) root         (0)    50743 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/join1.py
+-rw-r--r--   0 root         (0) root         (0)    55241 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    46007 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/sync1.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/push_script.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/register/
+-rw-r--r--   0 root         (0) root         (0)     9783 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/register/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/resolver/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/resolver/ldap/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35657 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/ldap/ldap.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/script.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/sign_key_cache.py
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/slp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/smartcard/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/smartcard/fido2/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10228 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12018 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/usb.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/yubikey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12022 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/socket/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13129 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/connect.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/handler.py
+-rw-r--r--   0 root         (0) root         (0)    30823 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/listen.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/send_recv1.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/sotp.py
+-rwxr-xr-x   0 root         (0) root         (0)    37180 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/spsc.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/srp.py
+-rw-r--r--   0 root         (0) root         (0)    23521 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ssh.py
+-rw-r--r--   0 root         (0) root         (0)    61848 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/stuff.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/sync_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/system_command.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/advanced.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/caching_query.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/fixture_data.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/helloworld.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/local_session_caching.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/model.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/relationship_caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9083 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/caches.py
+-rw-r--r--   0 root         (0) root         (0)    14341 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/files.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/config.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/error.py
+-rw-r--r--   0 root         (0) root         (0)     7963 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/group.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/maps.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/passwd.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/shadow.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/nss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/files_updater.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/map_updater.py
+-rw-r--r--   0 root         (0) root         (0)    10980 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/updater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4117 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/file_formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/token/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/token/fido2/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/token/hotp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39686 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/hotp/hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/link/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/link/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9709 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/link/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/motp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/motp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27734 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/motp/motp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/oath/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18882 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/oath/oath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/otp_push/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otp_push/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23418 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otp_push/otp_push.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/otpme/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24757 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/password/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26093 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/script_otp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_otp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_otp/script_otp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/script_static/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_static/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_static/script_static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/ssh/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39544 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/ssh/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/totp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/totp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35811 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/totp/totp.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25150 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/otpme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      949 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 05:09:50.962409 otpme-0.3.0a46/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-06-24 05:09:50.000000 otpme-0.3.0a46/setup.py
```

### Comparing `otpme-0.3.0a45/LICENSE` & `otpme-0.3.0a46/LICENSE`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/MANIFEST.in` & `otpme-0.3.0a46/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/PKG-INFO` & `otpme-0.3.0a46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a45
+Version: 0.3.0a46
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a45/README` & `otpme-0.3.0a46/README`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/bash_completion/otpme` & `otpme-0.3.0a46/bash_completion/otpme`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/abbreviations-it.gz` & `otpme-0.3.0a46/deploy/dicts/abbreviations-it.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/at-surnames.gz` & `otpme-0.3.0a46/deploy/dicts/at-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/common-passwords.gz` & `otpme-0.3.0a46/deploy/dicts/common-passwords.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/convert_dict.sh` & `otpme-0.3.0a46/deploy/dicts/convert_dict.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/de-female.gz` & `otpme-0.3.0a46/deploy/dicts/de-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/de-male.gz` & `otpme-0.3.0a46/deploy/dicts/de-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/de-surnames.gz` & `otpme-0.3.0a46/deploy/dicts/de-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/de-top10000.gz` & `otpme-0.3.0a46/deploy/dicts/de-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/en-top10000.gz` & `otpme-0.3.0a46/deploy/dicts/en-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/english-guessing.gz` & `otpme-0.3.0a46/deploy/dicts/english-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/english.gz` & `otpme-0.3.0a46/deploy/dicts/english.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/german-guessing.gz` & `otpme-0.3.0a46/deploy/dicts/german-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/german.gz` & `otpme-0.3.0a46/deploy/dicts/german.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/us-female.gz` & `otpme-0.3.0a46/deploy/dicts/us-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/us-male.gz` & `otpme-0.3.0a46/deploy/dicts/us-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/dicts/us-surnames.gz` & `otpme-0.3.0a46/deploy/dicts/us-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/otpme.conf.dist` & `otpme-0.3.0a46/deploy/otpme.conf.dist`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/pam/pam_otpme.py` & `otpme-0.3.0a46/deploy/pam/pam_otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/schema/core.schema` & `otpme-0.3.0a46/deploy/schema/core.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/schema/cosine.schema` & `otpme-0.3.0a46/deploy/schema/cosine.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/schema/inetorgperson.schema` & `otpme-0.3.0a46/deploy/schema/inetorgperson.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/schema/nis.schema` & `otpme-0.3.0a46/deploy/schema/nis.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/scripts/agent_script.sh` & `otpme-0.3.0a46/deploy/scripts/agent_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/deploy/scripts/key_script.sh` & `otpme-0.3.0a46/deploy/scripts/key_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/__init__.py` & `otpme-0.3.0a46/otpme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __project_url__ = "http://www.otpme.org"
 __copyright__ = "Copyright 2014-2022 the2nd <the2nd@otpme.org>"
 __project_description__ = "OTPme: A flexible One-Time-Password system."
 __author__ = "the2nd"
 __email__ = "the2nd@otpme.org"
 __credits__ = []
 __license__ = "GPLv2"
-__version__ = "0.3.0a45"
+__version__ = "0.3.0a46"
 __status__ = "Development Status :: 3 - Alpha"
 # In future versions :D
 #__status__ = "Development Status :: 4 - Beta"
 #__status__ = "Development Status :: 5 - Production/Stable"
 __pkg_name__ = __project_name__
 __maintainer__ = __author__
 __author_email__  = __email__
```

### Comparing `otpme-0.3.0a45/otpme/command.py` & `otpme-0.3.0a46/otpme/command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/__init__.py` & `otpme-0.3.0a46/otpme/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/arp.py` & `otpme-0.3.0a46/otpme/lib/arp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/auth_script.py` & `otpme-0.3.0a46/otpme/lib/auth_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/backend.py` & `otpme-0.3.0a46/otpme/lib/backend.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/backends/file/file.py` & `otpme-0.3.0a46/otpme/lib/backends/file/file.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/backends/file/index.py` & `otpme-0.3.0a46/otpme/lib/backends/file/index.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/backends/file/models.py` & `otpme-0.3.0a46/otpme/lib/backends/file/models.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/backends/file/transaction.py` & `otpme-0.3.0a46/otpme/lib/backends/file/transaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/__init__.py` & `otpme-0.3.0a46/otpme/lib/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/dogpile.py` & `otpme-0.3.0a46/otpme/lib/cache/dogpile.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/funccache.py` & `otpme-0.3.0a46/otpme/lib/cache/funccache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/lru.py` & `otpme-0.3.0a46/otpme/lib/cache/lru.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/memcache.py` & `otpme-0.3.0a46/otpme/lib/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/memcached.py` & `otpme-0.3.0a46/otpme/lib/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/memcachedb.py` & `otpme-0.3.0a46/otpme/lib/cache/memcachedb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cache/redis.py` & `otpme-0.3.0a46/otpme/lib/cache/redis.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/__init__.py` & `otpme-0.3.0a46/otpme/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/accessgroup.py` & `otpme-0.3.0a46/otpme/lib/classes/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/agent_conn.py` & `otpme-0.3.0a46/otpme/lib/classes/agent_conn.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/auth_handler.py` & `otpme-0.3.0a46/otpme/lib/classes/auth_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/ca.py` & `otpme-0.3.0a46/otpme/lib/classes/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/client.py` & `otpme-0.3.0a46/otpme/lib/classes/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/command_handler.py` & `otpme-0.3.0a46/otpme/lib/classes/command_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1051,15 +1051,17 @@
             except Exception as e:
                 msg = "Failed to get hostd connection: %s" % e
                 self.logger.warning(msg)
                 return
             hostd_conn.send(command="reload_radius")
 
         elif command == "test":
-            import radius
+            import pyrad.packet
+            from pyrad.client import Client
+            from pyrad.dictionary import Dictionary
             from radius_eap_mschapv2 import RADIUS
             mschap = False
             if "--mschap" in command_line:
                 mschap = True
                 command_line.remove("--mschap")
             usage_help = "Usage: otpme-tool radius test [--mschap] <username> <password> <nas_id> <secret>"
             if "-h" in command_line:
@@ -1080,20 +1082,29 @@
                 msg = "Sending MSCHAP radius request."
                 print(msg)
                 r = RADIUS(radius_host, radius_secret, radius_nas_ip, radius_nas_id, eap=True)
                 status = r.is_credential_valid(username, password)
             else:
                 msg = "Sending radius request."
                 print(msg)
-                status = radius.authenticate(username=username,
-                                    password=password,
-                                    secret=radius_secret,
-                                    host=radius_host,
-                                    nas_id=radius_nas_id,
-                                    port=1812)
+                radius_dict = os.path.join(config.config_dir, "radius", "dictionary")
+                radius_secret = radius_secret.encode()
+                srv = Client(server=radius_host,
+                			secret=radius_secret,
+                            dict=Dictionary(radius_dict))
+                # Create request.
+                req = srv.CreateAuthPacket(code=pyrad.packet.AccessRequest,
+                						   User_Name=username,
+                						   NAS_Identifier=radius_nas_id)
+                req["User-Password"] = req.PwCrypt(password)
+                # Send request.
+                reply = srv.SendPacket(req)
+                status = False
+                if reply.code == pyrad.packet.AccessAccept:
+                	status = True
             if not status:
                 msg = "Radius request failed."
                 raise OTPmeException(msg)
             msg = "Radius request successful."
             print(msg)
         else:
             msg = "Unknown command: %s" % command
```

### Comparing `otpme-0.3.0a45/otpme/lib/classes/conn_handler.py` & `otpme-0.3.0a46/otpme/lib/classes/conn_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/__init__.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/cert.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/failed_pass.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/failed_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/last_assigned_id.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/last_assigned_id.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/revoked_signature.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/revoked_signature.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/rsa_key.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/rsa_key.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/skip_sync.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/skip_sync.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/token_counter.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/token_counter.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/used_hash.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_hash.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/used_otp.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/used_slp.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/data_objects/used_sotp.py` & `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/dictionary.py` & `otpme-0.3.0a46/otpme/lib/classes/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/group.py` & `otpme-0.3.0a46/otpme/lib/classes/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/host.py` & `otpme-0.3.0a46/otpme/lib/classes/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/login_handler.py` & `otpme-0.3.0a46/otpme/lib/classes/login_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/mgmt_client.py` & `otpme-0.3.0a46/otpme/lib/classes/mgmt_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/node.py` & `otpme-0.3.0a46/otpme/lib/classes/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/object_config.py` & `otpme-0.3.0a46/otpme/lib/classes/object_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/otpme_agent.py` & `otpme-0.3.0a46/otpme/lib/classes/otpme_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/otpme_host.py` & `otpme-0.3.0a46/otpme/lib/classes/otpme_host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/otpme_object.py` & `otpme-0.3.0a46/otpme/lib/classes/otpme_object.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/policy.py` & `otpme-0.3.0a46/otpme/lib/classes/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/realm.py` & `otpme-0.3.0a46/otpme/lib/classes/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/resolver.py` & `otpme-0.3.0a46/otpme/lib/classes/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/role.py` & `otpme-0.3.0a46/otpme/lib/classes/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/script.py` & `otpme-0.3.0a46/otpme/lib/classes/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/session.py` & `otpme-0.3.0a46/otpme/lib/classes/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/signing.py` & `otpme-0.3.0a46/otpme/lib/classes/signing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/site.py` & `otpme-0.3.0a46/otpme/lib/classes/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -2385,15 +2385,15 @@
         callback.send(msg)
         admin_user = User(name=config.admin_user_name,
                             realm=self.realm,
                             site=self.name)
         if not admin_user.exists():
             try:
                 admin_user.add(add_default_token=True,
-                                gen_qrcode=False,
+                                gen_qrcode=True,
                                 verify_acls=False,
                                 callback=callback)
             except Exception as e:
                 msg = (_("Problem adding admin user: %s") % e)
                 config.raise_exception()
                 return callback.error(msg)
 
@@ -2436,21 +2436,14 @@
         except:
             auth_on_action_policy = None
 
         if auth_on_action_policy:
             auth_on_action_policy.add_whitelist(token_path=admin_token.rel_path,
                                                 verify_acls=False)
 
-        # Check if we can provide a QR code for admin token deployment.
-        if hasattr(admin_token, "gen_qrcode"):
-            admin_token_qrcode = admin_token.gen_qrcode(verify_acls=False)
-            msg = ("You can use this QRCode to deploy the site admin token:")
-            callback.send(msg)
-            callback.send(admin_token_qrcode)
-
         # Write objects.
         cache.flush()
 
         return self._write(callback=callback)
 
     # zzzzzzzzzzzzzzzzzzzzz
     # FIXME: make sure we remove all references before deleting a site
```

### Comparing `otpme-0.3.0a45/otpme/lib/classes/ssh_agent.py` & `otpme-0.3.0a46/otpme/lib/classes/ssh_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/token.py` & `otpme-0.3.0a46/otpme/lib/classes/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,22 +825,21 @@
         self.need_password = False
         # False means token type does not have a password.
         self.password_hash = False
         self.password_hash_params = []
         self.nt_hash = None
         self.mschap_enabled = None
         self.valid_otp_formats = []
-        self.valid_modes = []
-        self.mode = None
         self.supported_hardware_tokens = []
         self.smartcard_id = None
         self.client_options = []
         self.used_otp_salt = None
         self.signatures = {}
         self.valid_token_options = []
+        self.supports_qrcode = False
 
         self.track_last_used = True
         self.acl_inheritance_enabled = True
 
         self.temp_password_expire = 0.0
         self._temp_password_hash = None
         self.temp_password_hash_params = []
@@ -1756,15 +1755,15 @@
         return highest_counter
 
     @check_acls(['view_all:pin'])
     def show_pin(self, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Show token PIN. """
         if not self.pin:
-            return callback.error("Token does not have a PIN")
+            return callback.error("No PIN saved for thist token.")
         if run_policies:
             try:
                 self.run_policies("show_pin",
                                 callback=callback,
                                 _caller=_caller)
             except Exception as e:
                 return callback.error()
@@ -1772,21 +1771,21 @@
 
     @check_acls(['enable:pin'])
     @object_lock()
     @backend.transaction
     def enable_pin(self, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Enable optional token PIN. """
-        if not self.pin:
-            return callback.error("Token does not have a PIN")
-
         # Check if PIN is already enabled.
         if self.pin_enabled:
             return callback.error("PIN is already enabled for this token.")
 
+        if not self.pin:
+            return callback.error("No PIN saved for thist token.")
+
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
                 self.run_policies("enable_pin",
                                 callback=callback,
@@ -1807,20 +1806,20 @@
 
     @check_acls(['disable:pin'])
     @object_lock()
     @backend.transaction
     def disable_pin(self, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Disable optional token PIN. """
-        if not self.pin:
-            return callback.error("Token does not have a PIN")
-
         if self.pin_mandatory:
             return callback.error("PIN is mandatory for this token.")
 
+        if not self.pin:
+            return callback.error("No PIN saved for thist token.")
+
         # Check if PIN is already disabled.
         if not self.pin_enabled:
             return callback.error("PIN is already disabled for this token.")
 
         if run_policies:
             try:
                 self.run_policies("modify",
```

### Comparing `otpme-0.3.0a45/otpme/lib/classes/unit.py` & `otpme-0.3.0a46/otpme/lib/classes/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/classes/user.py` & `otpme-0.3.0a46/otpme/lib/classes/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/__init__.py` & `otpme-0.3.0a46/otpme/lib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/accessgroup.py` & `otpme-0.3.0a46/otpme/lib/cli/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/ca.py` & `otpme-0.3.0a46/otpme/lib/cli/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/client.py` & `otpme-0.3.0a46/otpme/lib/cli/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/dictionary.py` & `otpme-0.3.0a46/otpme/lib/cli/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/group.py` & `otpme-0.3.0a46/otpme/lib/cli/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/host.py` & `otpme-0.3.0a46/otpme/lib/cli/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/node.py` & `otpme-0.3.0a46/otpme/lib/cli/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/policy.py` & `otpme-0.3.0a46/otpme/lib/cli/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/realm.py` & `otpme-0.3.0a46/otpme/lib/cli/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/resolver.py` & `otpme-0.3.0a46/otpme/lib/cli/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/role.py` & `otpme-0.3.0a46/otpme/lib/cli/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/script.py` & `otpme-0.3.0a46/otpme/lib/cli/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/site.py` & `otpme-0.3.0a46/otpme/lib/cli/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/token.py` & `otpme-0.3.0a46/otpme/lib/cli/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/unit.py` & `otpme-0.3.0a46/otpme/lib/cli/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/cli/user.py` & `otpme-0.3.0a46/otpme/lib/cli/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/compgen.py` & `otpme-0.3.0a46/otpme/lib/compgen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/compression/__init__.py` & `otpme-0.3.0a46/otpme/lib/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/compression/base.py` & `otpme-0.3.0a46/otpme/lib/compression/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/connections.py` & `otpme-0.3.0a46/otpme/lib/connections.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/__init__.py` & `otpme-0.3.0a46/otpme/lib/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/authd.py` & `otpme-0.3.0a46/otpme/lib/daemon/authd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/clusterd.py` & `otpme-0.3.0a46/otpme/lib/daemon/clusterd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/controld.py` & `otpme-0.3.0a46/otpme/lib/daemon/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/hostd.py` & `otpme-0.3.0a46/otpme/lib/daemon/hostd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/joind.py` & `otpme-0.3.0a46/otpme/lib/daemon/joind.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/ldapd.py` & `otpme-0.3.0a46/otpme/lib/daemon/ldapd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/mgmtd.py` & `otpme-0.3.0a46/otpme/lib/daemon/mgmtd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/otpme_daemon.py` & `otpme-0.3.0a46/otpme/lib/daemon/otpme_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/scriptd.py` & `otpme-0.3.0a46/otpme/lib/daemon/scriptd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/syncd.py` & `otpme-0.3.0a46/otpme/lib/daemon/syncd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/daemon/unix_daemon.py` & `otpme-0.3.0a46/otpme/lib/daemon/unix_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/debug.py` & `otpme-0.3.0a46/otpme/lib/debug.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/doc.py` & `otpme-0.3.0a46/otpme/lib/doc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encoding/base.py` & `otpme-0.3.0a46/otpme/lib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/__init__.py` & `otpme-0.3.0a46/otpme/lib/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/aes.py` & `otpme-0.3.0a46/otpme/lib/encryption/aes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/aes_cfb.py` & `otpme-0.3.0a46/otpme/lib/encryption/aes_cfb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/argon2.py` & `otpme-0.3.0a46/otpme/lib/encryption/argon2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/asymmetric_key_handler.py` & `otpme-0.3.0a46/otpme/lib/encryption/asymmetric_key_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/ec.py` & `otpme-0.3.0a46/otpme/lib/encryption/ec.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/fernet.py` & `otpme-0.3.0a46/otpme/lib/encryption/fernet.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/hkdf.py` & `otpme-0.3.0a46/otpme/lib/encryption/hkdf.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/pbkdf2.py` & `otpme-0.3.0a46/otpme/lib/encryption/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/encryption/rsa.py` & `otpme-0.3.0a46/otpme/lib/encryption/rsa.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/exceptions.py` & `otpme-0.3.0a46/otpme/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/extensions/base/base.py` & `otpme-0.3.0a46/otpme/lib/extensions/base/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/extensions/ldif_handler.py` & `otpme-0.3.0a46/otpme/lib/extensions/ldif_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/extensions/posix/posix.py` & `otpme-0.3.0a46/otpme/lib/extensions/posix/posix.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/extensions/utils.py` & `otpme-0.3.0a46/otpme/lib/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/filetools.py` & `otpme-0.3.0a46/otpme/lib/filetools.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/freeradius/__init__.py` & `otpme-0.3.0a46/otpme/lib/freeradius/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/freeradius/otpme.py` & `otpme-0.3.0a46/otpme/lib/freeradius/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/freeradius/radiusd.py` & `otpme-0.3.0a46/otpme/lib/freeradius/radiusd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/freeradius/radiusd_test.py` & `otpme-0.3.0a46/otpme/lib/freeradius/radiusd_test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/gpg/utils.py` & `otpme-0.3.0a46/otpme/lib/gpg/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/__init__.py` & `otpme-0.3.0a46/otpme/lib/help/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/accessgroup.py` & `otpme-0.3.0a46/otpme/lib/help/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/agent.py` & `otpme-0.3.0a46/otpme/lib/help/agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/auth.py` & `otpme-0.3.0a46/otpme/lib/help/auth.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/ca.py` & `otpme-0.3.0a46/otpme/lib/help/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/client.py` & `otpme-0.3.0a46/otpme/lib/help/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/cluster.py` & `otpme-0.3.0a46/otpme/lib/help/cluster.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/controld.py` & `otpme-0.3.0a46/otpme/lib/help/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/dictionary.py` & `otpme-0.3.0a46/otpme/lib/help/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/get_authorized_keys.py` & `otpme-0.3.0a46/otpme/lib/help/get_authorized_keys.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/group.py` & `otpme-0.3.0a46/otpme/lib/help/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/host.py` & `otpme-0.3.0a46/otpme/lib/help/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/node.py` & `otpme-0.3.0a46/otpme/lib/help/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/pinentry.py` & `otpme-0.3.0a46/otpme/lib/help/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/__init__.py` & `otpme-0.3.0a46/otpme/lib/help/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/authonaction.py` & `otpme-0.3.0a46/otpme/lib/help/policy/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/autodisable.py` & `otpme-0.3.0a46/otpme/lib/help/policy/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/defaultgroups.py` & `otpme-0.3.0a46/otpme/lib/help/policy/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/defaultpolicies.py` & `otpme-0.3.0a46/otpme/lib/help/policy/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/defaultroles.py` & `otpme-0.3.0a46/otpme/lib/help/policy/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/defaultunits.py` & `otpme-0.3.0a46/otpme/lib/help/policy/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/forcetoken.py` & `otpme-0.3.0a46/otpme/lib/help/policy/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/idrange.py` & `otpme-0.3.0a46/otpme/lib/help/policy/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/logintimes.py` & `otpme-0.3.0a46/otpme/lib/help/policy/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/objecttemplates.py` & `otpme-0.3.0a46/otpme/lib/help/policy/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/password.py` & `otpme-0.3.0a46/otpme/lib/help/policy/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/policy/tokenacls.py` & `otpme-0.3.0a46/otpme/lib/help/policy/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/realm.py` & `otpme-0.3.0a46/otpme/lib/help/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/register.py` & `otpme-0.3.0a46/otpme/lib/help/register.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/resolver/__init__.py` & `otpme-0.3.0a46/otpme/lib/help/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/resolver/ldap.py` & `otpme-0.3.0a46/otpme/lib/help/resolver/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/role.py` & `otpme-0.3.0a46/otpme/lib/help/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/script.py` & `otpme-0.3.0a46/otpme/lib/help/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/session.py` & `otpme-0.3.0a46/otpme/lib/help/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/site.py` & `otpme-0.3.0a46/otpme/lib/help/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/__init__.py` & `otpme-0.3.0a46/otpme/lib/help/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/fido2.py` & `otpme-0.3.0a46/otpme/lib/help/token/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/hotp.py` & `otpme-0.3.0a46/otpme/lib/help/token/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/motp.py` & `otpme-0.3.0a46/otpme/lib/help/token/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/otp_push.py` & `otpme-0.3.0a46/otpme/lib/help/token/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/otpme.py` & `otpme-0.3.0a46/otpme/lib/help/token/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/password.py` & `otpme-0.3.0a46/otpme/lib/help/token/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/ssh.py` & `otpme-0.3.0a46/otpme/lib/help/token/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/totp.py` & `otpme-0.3.0a46/otpme/lib/help/token/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/yubikey_hmac.py` & `otpme-0.3.0a46/otpme/lib/help/token/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/token/yubikey_hotp.py` & `otpme-0.3.0a46/otpme/lib/help/token/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/tool.py` & `otpme-0.3.0a46/otpme/lib/help/tool.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/unit.py` & `otpme-0.3.0a46/otpme/lib/help/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/help/user.py` & `otpme-0.3.0a46/otpme/lib/help/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/host.py` & `otpme-0.3.0a46/otpme/lib/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/humanize/units.py` & `otpme-0.3.0a46/otpme/lib/humanize/units.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/index/mysql.py` & `otpme-0.3.0a46/otpme/lib/index/mysql.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/index/postgres.py` & `otpme-0.3.0a46/otpme/lib/index/postgres.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/index/sqlite3.py` & `otpme-0.3.0a46/otpme/lib/index/sqlite3.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/job/callback.py` & `otpme-0.3.0a46/otpme/lib/job/callback.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/job/otpme_job.py` & `otpme-0.3.0a46/otpme/lib/job/otpme_job.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/join.py` & `otpme-0.3.0a46/otpme/lib/join.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/json.py` & `otpme-0.3.0a46/otpme/lib/json.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/jwt.py` & `otpme-0.3.0a46/otpme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/ldap/client.py` & `otpme-0.3.0a46/otpme/lib/ldap/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/ldap/schema.py` & `otpme-0.3.0a46/otpme/lib/ldap/schema.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/ldap/server.py` & `otpme-0.3.0a46/otpme/lib/ldap/server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/locking.py` & `otpme-0.3.0a46/otpme/lib/locking.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/log.py` & `otpme-0.3.0a46/otpme/lib/log.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/messages.py` & `otpme-0.3.0a46/otpme/lib/messages.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/mschap.py` & `otpme-0.3.0a46/otpme/lib/mschap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/mschap_util.py` & `otpme-0.3.0a46/otpme/lib/mschap_util.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/multiprocessing.py` & `otpme-0.3.0a46/otpme/lib/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/net.py` & `otpme-0.3.0a46/otpme/lib/net.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/nsscache.py` & `otpme-0.3.0a46/otpme/lib/nsscache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/offline_token.py` & `otpme-0.3.0a46/otpme/lib/offline_token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/oid.py` & `otpme-0.3.0a46/otpme/lib/oid.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otp/oath/hotp.py` & `otpme-0.3.0a46/otpme/lib/otp/oath/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otp/oath/totp.py` & `otpme-0.3.0a46/otpme/lib/otp/oath/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otp/otpme/otpme.py` & `otpme-0.3.0a46/otpme/lib/otp/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otp/yubico/yubiotp.py` & `otpme-0.3.0a46/otpme/lib/otp/yubico/yubiotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otpme_acl.py` & `otpme-0.3.0a46/otpme/lib/otpme_acl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otpme_config.py` & `otpme-0.3.0a46/otpme/lib/otpme_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/otpme_pass.py` & `otpme-0.3.0a46/otpme/lib/otpme_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pam.py` & `otpme-0.3.0a46/otpme/lib/pam.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pickle.py` & `otpme-0.3.0a46/otpme/lib/pickle.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pinentry/pinentry.py` & `otpme-0.3.0a46/otpme/lib/pinentry/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pinentry/wrapper.py` & `otpme-0.3.0a46/otpme/lib/pinentry/wrapper.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pki/cert.py` & `otpme-0.3.0a46/otpme/lib/pki/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pki/utils.py` & `otpme-0.3.0a46/otpme/lib/pki/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/pki/utils_openssl.py` & `otpme-0.3.0a46/otpme/lib/pki/utils_openssl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/__init__.py` & `otpme-0.3.0a46/otpme/lib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/authonaction/authonaction.py` & `otpme-0.3.0a46/otpme/lib/policy/authonaction/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/autodisable/autodisable.py` & `otpme-0.3.0a46/otpme/lib/policy/autodisable/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/defaultgroups/defaultgroups.py` & `otpme-0.3.0a46/otpme/lib/policy/defaultgroups/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/defaultpolicies/defaultpolicies.py` & `otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/defaultroles/defaultroles.py` & `otpme-0.3.0a46/otpme/lib/policy/defaultroles/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/defaultunits/defaultunits.py` & `otpme-0.3.0a46/otpme/lib/policy/defaultunits/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/forcetoken/forcetoken.py` & `otpme-0.3.0a46/otpme/lib/policy/forcetoken/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/get_class.py` & `otpme-0.3.0a46/otpme/lib/policy/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/idrange/idrange.py` & `otpme-0.3.0a46/otpme/lib/policy/idrange/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/logintimes/logintimes.py` & `otpme-0.3.0a46/otpme/lib/policy/logintimes/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/objecttemplates/objecttemplates.py` & `otpme-0.3.0a46/otpme/lib/policy/objecttemplates/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/password/password.py` & `otpme-0.3.0a46/otpme/lib/policy/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/tokenacls/tokenacls.py` & `otpme-0.3.0a46/otpme/lib/policy/tokenacls/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/policy/utils.py` & `otpme-0.3.0a46/otpme/lib/policy/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/preload.py` & `otpme-0.3.0a46/otpme/lib/preload.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/progress.py` & `otpme-0.3.0a46/otpme/lib/progress.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/__init__.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/agent1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/auth1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/cluster1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/get_class.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/host1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/join1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/mgmt1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/client/sync1.py` & `otpme-0.3.0a46/otpme/lib/protocols/client/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/otpme_client.py` & `otpme-0.3.0a46/otpme/lib/protocols/otpme_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/otpme_server.py` & `otpme-0.3.0a46/otpme/lib/protocols/otpme_server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/request.py` & `otpme-0.3.0a46/otpme/lib/protocols/request.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/response.py` & `otpme-0.3.0a46/otpme/lib/protocols/response.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/__init__.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/agent1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/auth1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/cluster1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/get_class.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/host1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/join1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/mgmt1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/server/sync1.py` & `otpme-0.3.0a46/otpme/lib/protocols/server/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/status_codes.py` & `otpme-0.3.0a46/otpme/lib/protocols/status_codes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/protocols/utils.py` & `otpme-0.3.0a46/otpme/lib/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/push_script.py` & `otpme-0.3.0a46/otpme/lib/push_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/qrcode.py` & `otpme-0.3.0a46/otpme/lib/qrcode.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/re.py` & `otpme-0.3.0a46/otpme/lib/re.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/register/__init__.py` & `otpme-0.3.0a46/otpme/lib/register/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/resolver/__init__.py` & `otpme-0.3.0a46/otpme/lib/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/resolver/get_class.py` & `otpme-0.3.0a46/otpme/lib/resolver/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/resolver/ldap/ldap.py` & `otpme-0.3.0a46/otpme/lib/resolver/ldap/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/resolver/utils.py` & `otpme-0.3.0a46/otpme/lib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/script.py` & `otpme-0.3.0a46/otpme/lib/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/sign_key_cache.py` & `otpme-0.3.0a46/otpme/lib/sign_key_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/slp.py` & `otpme-0.3.0a46/otpme/lib/slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/__init__.py` & `otpme-0.3.0a46/otpme/lib/smartcard/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/fido2/fido2.py` & `otpme-0.3.0a46/otpme/lib/smartcard/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/get_class.py` & `otpme-0.3.0a46/otpme/lib/smartcard/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/utils.py` & `otpme-0.3.0a46/otpme/lib/smartcard/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/yubikey/deploy.py` & `otpme-0.3.0a46/otpme/lib/smartcard/yubikey/deploy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/yubikey/usb.py` & `otpme-0.3.0a46/otpme/lib/smartcard/yubikey/usb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/yubikey/yubikey.py` & `otpme-0.3.0a46/otpme/lib/smartcard/yubikey/yubikey.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py` & `otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py` & `otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/socket/connect.py` & `otpme-0.3.0a46/otpme/lib/socket/connect.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/socket/handler.py` & `otpme-0.3.0a46/otpme/lib/socket/handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/socket/listen.py` & `otpme-0.3.0a46/otpme/lib/socket/listen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/socket/send_recv1.py` & `otpme-0.3.0a46/otpme/lib/socket/send_recv1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/sotp.py` & `otpme-0.3.0a46/otpme/lib/sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/spsc.py` & `otpme-0.3.0a46/otpme/lib/spsc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/srp.py` & `otpme-0.3.0a46/otpme/lib/srp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/ssh.py` & `otpme-0.3.0a46/otpme/lib/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/stuff.py` & `otpme-0.3.0a46/otpme/lib/stuff.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/sync_cache.py` & `otpme-0.3.0a46/otpme/lib/sync_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/system_command.py` & `otpme-0.3.0a46/otpme/lib/system_command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/test.py` & `otpme-0.3.0a46/otpme/lib/test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/__init__.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/advanced.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/advanced.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/caching_query.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/caching_query.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/environment.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/environment.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/fixture_data.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/fixture_data.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/helloworld.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/helloworld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/local_session_caching.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/local_session_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/model.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/model.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/dogpile_caching/relationship_caching.py` & `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/relationship_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/__init__.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/caches/caches.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/caches.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/caches/files.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/files.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/config.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/error.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/error.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/lock.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/lock.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/group.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/maps.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/maps.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/passwd.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/passwd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/maps/shadow.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/shadow.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/nss.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/nss.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/files_updater.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/files_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/map_updater.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/map_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/update/updater.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/nss_cache/util/file_formats.py` & `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/file_formats.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/oath_toolkit/_compat.py` & `otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/_compat.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/third_party/oath_toolkit/uri.py` & `otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/uri.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/__init__.py` & `otpme-0.3.0a46/otpme/lib/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/fido2/fido2.py` & `otpme-0.3.0a46/otpme/lib/token/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/get_class.py` & `otpme-0.3.0a46/otpme/lib/token/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/hotp/hotp.py` & `otpme-0.3.0a46/otpme/lib/token/ssh/ssh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2014 the2nd <the2nd@otpme.org>
 # Distributed under the terms of the GNU General Public License v2
 import os
-import time
-#from pyotp.hotp import HOTP
 
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
     pass
 
+from otpme.lib import ssh
 from otpme.lib import stuff
 from otpme.lib import config
-from otpme.lib import qrcode
 from otpme.lib import backend
 from otpme.lib import otpme_acl
-from otpme.lib.otp.oath import hotp
 from otpme.lib.classes.token import Token
 from otpme.lib.locking import object_lock
 from otpme.lib.otpme_acl import check_acls
 from otpme.lib.encoding.base import decode
-from otpme.lib.third_party.oath_toolkit import uri
+from otpme.lib.encryption.rsa import RSAKey
 from otpme.lib.protocols.utils import register_commands
-
 from otpme.lib.classes.token \
             import get_acls \
             as _get_acls
 from otpme.lib.classes.token \
             import get_value_acls \
             as _get_value_acls
 from otpme.lib.classes.token \
@@ -35,207 +31,206 @@
             as _get_default_acls
 from otpme.lib.classes.token \
             import get_recursive_default_acls \
             as _get_recursive_default_acls
 
 from otpme.lib.exceptions import *
 
-logger = config.logger
-
 default_callback = config.get_callback()
 
+logger = config.logger
+
 read_acls =  []
-write_acls =  [
-                "generate",
-                "resync",
-        ]
+write_acls =  []
 
 read_value_acls = {
                 "view"      : [
-                            "secret",
-                            "server_secret",
-                            "pin",
+                            "2ftoken",
+                            "2ftoken_status",
+                            "card_type",
+                            "key_type",
+                            "ssh_public_key",
+                            "ssh_private_key",
                             "auth_script",
-                            "otp_format",
-                            "counter_check_range",
-                            "mode",
-                            "counter_sync_time",
                             "offline_status",
                             "offline_expiry",
                             "offline_unused_expiry",
                             "session_keep",
+                            "signature",
                             ],
-        }
+                }
 
 write_value_acls = {
-                "generate"  : [
-                            "otp",
-                            "qrcode",
+                "add"       : [
+                            "signature",
+                            ],
+                "delete"    : [
+                            "signature",
+                            ],
+                "verify"    : [
+                            "signature",
                             ],
                 "edit"      : [
-                            "secret",
-                            "pin",
+                            "2ftoken",
+                            "card_type",
+                            "key_type",
+                            "password",
+                            "ssh_public_key",
+                            "ssh_private_key",
                             "auth_script",
-                            "otp_format",
-                            "counter_check_range",
-                            "mode",
                             "offline_expiry",
                             "offline_unused_expiry",
                             ],
                 "enable"    : [
-                            "pin",
+                            "2ftoken",
                             "auth_script",
                             "offline",
                             "session_keep",
                             ],
                 "disable"   : [
-                            "pin",
+                            "2ftoken",
                             "auth_script",
                             "offline",
                             "session_keep",
                             ],
-            }
+                }
 
 default_acls = []
 
 recursive_default_acls = []
 
 commands = {
-    'secret'   : {
+    'password'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_secret',
-                    'oargs'             : ['auto_secret', 'secret'],
+                    'method'            : 'change_key_password',
+                    'oargs'             : ['auto_password', 'password'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'pin'   : {
+    'ssh_public_key'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_pin',
-                    'oargs'             : ['auto_pin', 'pin'],
+                    'method'            : 'change_ssh_public_key',
+                    'oargs'             : ['ssh_public_key'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'enable_pin'   : {
-            'OTPme-mgmt-1.0'    : {
-                'exists'    : {
-                    'method'            : 'enable_pin',
-                    'job_type'          : 'process',
-                    },
-                },
-            },
-    'disable_pin'   : {
+    'test'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'disable_pin',
+                    'method'            : 'test',
+                    'oargs'             : ['password'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'show_secret'   : {
+    '2f_token'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'show_secret',
+                    'method'            : 'change_2f_token',
+                    'args'              : ['second_factor_token'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'show_pin'   : {
+    'enable_2f'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'show_pin',
+                    'method'            : 'enable_2f_token',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'gen'   : {
+    'disable_2f'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'gen_otp',
+                    'method'            : 'disable_2f_token',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'gen_mschap'   : {
+    'card_type'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'gen_mschap',
+                    'method'            : 'change_card_type',
+                    'args'              : ['card_type'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'gen_qrcode'   : {
+    'key_type'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'gen_qrcode',
-                    'oargs'             : ['qrcode_file'],
+                    'method'            : 'change_key_type',
+                    'args'              : ['key_type'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'resync'   : {
+    'sign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'resync',
-                    'oargs'             : ['otp'],
+                    'method'            : 'sign',
+                    'oargs'             : ['tags', 'stdin_pass'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'test'   : {
+    'resign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'test',
-                    'oargs'             : ['password'],
+                    'method'            : 'resign',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'otp_format'   : {
+    'add_sign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_otp_format',
-                    'args'              : ['otp_format'],
+                    'method'            : 'add_sign',
+                    'oargs'             : ['signature', 'tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'mode'   : {
+    'del_sign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_mode',
-                    'args'              : ['new_mode'],
+                    'method'            : 'del_sign',
+                    'oargs'             : ['username', 'tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'counter_check_range'   : {
+    'verify_sign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_counter_check_range',
-                    'oargs'             : ['counter_check_range'],
+                    'method'            : 'verify_sign',
+                    'oargs'             : ['username', 'user_uuid', 'tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'enable_mschap'   : {
+    'get_sign_data'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'enable_mschap',
+                    'method'            : 'get_sign_data',
+                    'oargs'             : ['tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'disable_mschap'   : {
+    'get_sign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'disable_mschap',
+                    'method'            : 'get_sign',
+                    'oargs'             : ['username', 'user_uuid', 'tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
     }
 
 def get_acls(split=False, **kwargs):
@@ -275,1117 +270,756 @@
 def get_recursive_default_acls():
     """ Get all supported object recursive default ACLs """
     token_recursive_default_acls = _get_recursive_default_acls()
     _acls = otpme_acl.merge_acls(recursive_default_acls,
                                 token_recursive_default_acls)
     return _acls
 
-# OATH OTP formats and the resulting OTP lens.
-OATH_OTP_FORMATS = {
-        'dec4'          : 4,
-        'dec6'          : 6,
-        'dec7'          : 7,
-        'dec8'          : 8,
-        'hex'           : 4,
-        'hex-notrunc'   : 4,
-        }
-
 REGISTER_BEFORE = []
 REGISTER_AFTER = []
 
 def register():
     """ Register object. """
-    register_hooks()
     register_token_type()
-    register_config_params()
     register_commands("token",
                     commands,
-                    sub_type="hotp",
+                    sub_type="ssh",
                     sub_type_attribute="token_type")
 
 def register_hooks():
     config.register_auth_on_action_hook("token", "resync")
-    config.register_auth_on_action_hook("token", "gen_mschap")
-    config.register_auth_on_action_hook("token", "gen_qrcode")
-    config.register_auth_on_action_hook("token", "change_mode")
-    config.register_auth_on_action_hook("token", "show_secret")
-    config.register_auth_on_action_hook("token", "change_counter_check_range")
+    config.register_auth_on_action_hook("token", "change_key_type")
+    config.register_auth_on_action_hook("token", "change_card_type")
+    config.register_auth_on_action_hook("token", "change_2f_token")
+    config.register_auth_on_action_hook("token", "enable_2f_token")
+    config.register_auth_on_action_hook("token", "disable_2f_token")
+    config.register_auth_on_action_hook("token", "add_sign")
+    config.register_auth_on_action_hook("token", "del_sign")
+    config.register_auth_on_action_hook("token", "change_ssh_public_key")
 
 def register_token_type():
     """ Register token type. """
-    config.register_sub_object_type("token", "hotp")
-
-def register_config_params():
-    """ Register config params. """
-    # Valid object types for our config parameters..
-    object_types = [
-                    'realm',
-                    'site',
-                    'unit',
-                    'user',
-                ]
-    # Default HOTP OTP format.
-    config.register_config_parameter(name="hotp_format",
-                                    ctype=str,
-                                    default_value="dec6",
-                                    valid_values=list(OATH_OTP_FORMATS),
-                                    object_types=object_types)
-    # Counter check range when doing HOTP auth.
-    config.register_config_parameter(name="hotp_check_range",
-                                    ctype=int,
-                                    default_value=32,
-                                    object_types=object_types)
-    # Counter check range when doing token resync.
-    config.register_config_parameter(name="hotp_resync_check_range",
-                                    ctype=int,
-                                    default_value=1024,
-                                    object_types=object_types)
-    # The HOTP default PIN length.
-    config.register_config_parameter(name="hotp_default_pin_len",
-                                    ctype=int,
-                                    default_value=4,
-                                    object_types=object_types)
-    # The HOTP secret length.
-    config.register_config_parameter(name="hotp_secret_len",
-                                    ctype=int,
-                                    default_value=40,
-                                    object_types=object_types)
+    config.register_sub_object_type("token", "ssh")
 
-class HotpToken(Token):
-    """ Class for OATH HOTP tokens. """
+class SshToken(Token):
+    """ Class for SSH tokens. """
     def __init__(self, object_id=None, user=None, name=None,
         realm=None, site=None, path=None, **kwargs):
+
         # Call parent class init.
-        super(HotpToken, self).__init__(object_id=object_id,
-                                        realm=realm,
-                                        site=site,
-                                        user=user,
-                                        name=name,
-                                        path=path,
-                                        **kwargs)
+        super(SshToken, self).__init__(object_id=object_id,
+                                            realm=realm,
+                                            site=site,
+                                            user=user,
+                                            name=name,
+                                            path=path,
+                                            **kwargs)
 
         self._acls = get_acls()
         self._value_acls = get_value_acls()
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
-
+        # Set token type.
+        self.token_type = "ssh"
+        # Set password type.
+        self.pass_type = "ssh_key"
+        # Set SSH key type.
+        self.key_type = "rsa"
+        self.valid_key_types = [ "rsa", "dsa" ]
         # Set default values.
-        self.token_type = "hotp"
-        self.pass_type = "otp"
-        self.otp_type = "counter"
-        self.otp_format = None
-
-        self.valid_otp_formats = OATH_OTP_FORMATS
-        self.pin = None
-        self.pin_len = None
-        self.pin_enabled = True
-        self.need_password = True
-        self.auth_script_enabled = False
+        self.ssh_public_key = None
+        self.ssh_private_key = None
+        # Will hold decrypted SSH private key.
+        self._ssh_private_key = None
+        # Challenge to verify in offline mode.
+        self.offline_challenge = ""
+        # FIXME: allow to modify this list!?
+        # Valid token options (e.g. command=/some/script/path)
+        self.valid_token_options = [
+                                'cert-authority',
+                                'command',
+                                'restrict',
+                                'environment',
+                                'from',
+                                'no-agent-forwarding',
+                                'no-port-forwarding',
+                                'no-pty',
+                                'no-user-rc',
+                                'no-X11-forwarding',
+                                'permitopen',
+                                'principals',
+                                'tunnel',
+                                ]
+        # Hardware card/token type.
+        self.card_type = None
         self.allow_offline = False
         self.offline_expiry = 0
         self.offline_unused_expiry = 0
         self.keep_session = False
-        self.valid_modes = [ 'mode1', 'mode2' ]
-        # Default token mode should be mode2 which is more secure for offline
-        # usage.
-        self.mode = "mode2"
-        self.pin_mandatory = True
-        # HOTP specific settings.
-        self.counter_check_range = None
-        self.counter_sync_time = 1.0
-        self.sync_offline_token_counter = True
-        self.server_secret = None
+        self.signable = True
+        self.signatures = {}
+        self.cross_site_links = True
+        self.need_password = True
         # Hardware tokens that we can handle (e.g. on otpme-token deploy).
-        self.supported_hardware_tokens = [ 'yubikey_hotp' ]
-        # This dict is filled with used OTP(s) and its counters and read by
-        # self.add_used_otp() to get the token counter that needs to be saved.
-        self.otp_cache = {}
-        # Token ACLs to add to new token via tokenacls policy.
-        self.token_acls = [
-                            'generate:otp',
-                            'generate:qrcode',
-                        ]
-        self.user_acls = []
-        self.creator_acls = []
+        self.supported_hardware_tokens = [ 'yubikey-gpg', 'openssh' ]
+
+        self._sub_sync_fields = {
+                    'host'  : {
+                        'trusted'  : [
+                            "SSH_PUBLIC_KEY",
+                            ]
+                        },
+
+                    'node'  : {
+                        'untrusted'  : [
+                            "SSH_PUBLIC_KEY",
+                            ]
+                        },
+                    }
 
     def _get_object_config(self):
         """ Merge token config with config from parent class. """
         token_config = {
-            'PIN'                       : {
-                                            'var_name'      : 'pin',
+            'SSH_PRIVATE_KEY'           : {
+                                            'var_name'      : 'ssh_private_key',
                                             'type'          : str,
                                             'required'      : False,
                                             'encryption'    : config.disk_encryption,
                                         },
 
-            'PIN_ENABLED'               : {
-                                            'var_name'      : 'pin_enabled',
-                                            'type'          : bool,
+            'SSH_PUBLIC_KEY'            : {
+                                            'var_name'      : 'ssh_public_key',
+                                            'type'          : str,
                                             'required'      : False,
+                                            'encoding'      : 'BASE64',
                                         },
 
-            'PIN_LEN'                   : {
-                                            'var_name'      : 'pin_len',
-                                            'type'          : int,
-                                            'required'      : False,
-                                        },
 
-            'SERVER_SECRET'             : {
-                                            'var_name'      : 'server_secret',
+            'OFFLINE_CHALLENGE'         : {
+                                            'var_name'      : 'offline_challenge',
                                             'type'          : str,
                                             'required'      : False,
                                             'encryption'    : config.disk_encryption,
                                         },
 
-
-            'OTP_FORMAT'                : {
-                                            'var_name'      : 'otp_format',
+            'KEY_TYPE'                  : {
+                                            'var_name'      : 'key_type',
                                             'type'          : str,
                                             'required'      : False,
                                         },
 
-            'COUNTER'                   : {
-                                            'var_name'      : 'get_token_counter',
-                                            'type'          : int,
+            'CARD_TYPE'                 : {
+                                            'var_name'      : 'card_type',
+                                            'type'          : str,
                                             'required'      : False,
                                         },
 
-            'COUNTER_SYNC_TIME'         : {
-                                            'var_name'      : 'counter_sync_time',
-                                            'type'          : float,
+            'SECOND_FACTOR_TOKEN'       : {
+                                            'var_name'      : 'second_factor_token',
+                                            'type'          : 'uuid',
                                             'required'      : False,
                                         },
 
-            'COUNTER_CHECK_RANGE'       : {
-                                            'var_name'      : 'counter_check_range',
-                                            'type'          : int,
+
+            'SECOND_FACTOR_TOKEN_ENABLED': {
+                                            'var_name'      : 'second_factor_token_enabled',
+                                            'type'          : bool,
                                             'required'      : False,
                                         },
+
+            'SIGNATURES'                : {
+                                            'var_name'  : 'signatures',
+                                            'type'      : dict,
+                                            'required'  : False,
+                                        },
             }
 
         # Use parent class method to merge token configs.
         return Token._get_object_config(self, token_config=token_config)
 
     def set_variables(self):
-        """ Set instance variables """
+        """ Set instance variables. """
         # Run parent class method that may override default values with those
         # read from config.
         Token.set_variables(self)
-        # In mode2 the PIN is mandatory.
-        if self.mode == "mode2":
-            self.pin_enabled = True
-            self.pin_mandatory = True
-        else:
-            self.pin_mandatory = False
-
-    @property
-    def otp_len(self):
-        """ Set OTP len depending on the configured OTP format. """
-        try:
-            otp_len = OATH_OTP_FORMATS[self.otp_format]
-        except:
-            otp_len = 6
-        return otp_len
-
-    @property
-    def secret_len(self):
-        """ Get token secret length. """
-        secret_len = self.get_config_parameter("hotp_secret_len")
-        return secret_len
-
-    def get_secret(self, pin=None, mode=None,
-        callback=default_callback,
-        _caller="API", ** kwargs):
-        """ Get token secret """
-        if not mode:
-            mode = self.mode
-        if mode == "mode1":
-            secret = str(self.secret)
-        else:
-            import hashlib
-            if not pin:
-                pin = self.pin
-            server_secret = self.server_secret
-            if isinstance(pin, str):
-                pin = pin.encode("utf-8")
-            if isinstance(server_secret, str):
-                server_secret = server_secret.encode("utf-8")
-            hash_string = b"%s%s" % (pin, server_secret)
-            sha512 = hashlib.sha512()
-            sha512.update(hash_string)
-            secret = sha512.hexdigest()
-            secret = secret[0:self.secret_len]
-        if _caller == "API":
-            return secret
-        return callback.ok(secret)
 
     def get_offline_config(self, second_factor_usage=False):
         """ Get offline config of token. (e.g. without PIN). """
-        # Make sure our object config is up-to-date.
-        self.update_object_config()
-        # Get a copy of our object config.
         offline_config = self.object_config.copy()
-        # In offline mode we never need the PIN.
-        offline_config['PIN'] = ''
+        need_encryption = False
+
+        #if self.private_key:
+        #    need_encryption = True
 
+        # FIXME: implement self.allow_offline_rsp!!!
         need_encryption = True
-        if self.mode == "mode1":
-            # In mode1 we do not need the server secret in offline config.
-            offline_config['SERVER_SECRET'] = ''
-            if not self.pin_enabled:
-                need_encryption = False
-
-        if self.mode == "mode2":
-            # In mode2 there should be no HOTP secret so make sure we empty it.
-            offline_config['SECRET'] = ''
-            # In mode2 the token config includes only the server secret which is
-            # used in conjunction with the PIN to generate the HOTP secret. In
-            # offline mode the token config will include neither, not the PIN
-            # and not the HOTP secret. Thus its relatively save to store it
-            # unencrypted. Using the PIN to encrypt the token secret (like its
-            # done in mode1) is much more susceptible to brute force attacks.
-            need_encryption = False
-
-        # FIXME: how to decided if encryption is needed in second factor usage??
-        # When used as second factor token (e.g. with ssh or password token) it
-        # is probably saver to encrypt our config. If the first factor token is
-        # a weak password this may not be true but we currently have not way to
-        # get this info at this stage.
-        if second_factor_usage:
-            need_encryption = True
-        else:
-            # Wnen not used as second factor token remove PIN len from config to
-            # make brute force attacks harder.
-            offline_config['PIN_LEN'] = ''
+        #if self.allow_offline_rsp:
+        #    need_encryption = True
 
         offline_config['NEED_OFFLINE_ENCRYPTION'] = need_encryption
-
         return offline_config
 
-    @check_acls(['edit:mode'])
+    def verify_acl(self, action):
+        """ Verify ACLs required to allow <action>. """
+        # Parent class cannot know the ACL to allow verification of signatures
+        # e.g. "view:script" for script objects and "view_public_key" for SSH
+        # tokens.
+        if action == "verify_signature":
+            if self._verify_acl("verify:signature") \
+            or self._verify_acl("view:signature") \
+            or self._verify_acl("view:ssh_public_key"):
+                return True
+
+        if action == "get_signatures":
+            if self._verify_acl("view:signature") \
+            or self.verify_acl("view:ssh_public_key"):
+                return True
+
+        # Finally try to verify ACL via parent class method.
+        if self._verify_acl(action):
+            return True
+
+        return  False
+
+    @check_acls(['view:ssh_public_key'])
+    def get_sign_data(self, callback=default_callback, **kwargs):
+        """ Return public key to be signed by parent class method. """
+        ssh_public_key = self.ssh_public_key
+        return callback.ok(ssh_public_key)
+
+    def get_card_types(self, _caller="API", callback=default_callback, **kwargs):
+        """ Get supported hardware card/token types. """
+        card_types = [ 'gpg' ]
+        if _caller == "CLIENT":
+            card_types = "\n".join(card_types)
+        return callback.ok(card_types)
+
+    @check_acls(['edit:card_type'])
     @object_lock()
     @backend.transaction
-    def change_mode(self, new_mode, run_policies=True,
+    def change_card_type(self, card_type=None, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Change token operation mode. """
-        # Make sure new mode is of type string.
-        new_mode = str(new_mode)
-
-        if not new_mode in self.valid_modes:
-            return callback.error(_("Unknown mode: %s") % new_mode)
-
-        if new_mode == self.mode:
-            return callback.error(_("Token already in mode: %s") % new_mode)
+        """ Get supported hardware card/token types. """
+        if card_type:
+            if not card_type in self.get_card_types():
+                msg = (_("Unsupported card type: %s") % card_type)
+                return callback.error(msg)
+            if card_type == self.card_type:
+                msg = (_("Card type already set to: %s") % card_type)
+                return callback.error(msg)
 
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
-                self.run_policies("change_mode",
+                self.run_policies("change_card_type",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        if new_mode == "mode1":
-            self.secret = self.get_secret()
-            self.pin_mandatory = False
-            return_message = (_("Token switched to mode1."))
-
-        if new_mode == "mode2":
-            # if we have a server secret we can try to switch back to mode2
-            # without re-deploying token.
-            if self.server_secret:
-                otp = None
-                if not otp:
-                    otp = callback.askpass("Please enter PIN+OTP: ")
-                    otp = str(otp)
-
-                if not otp:
-                    return callback.error("Unable to get PIN+OTP.")
-
-                # Make sure OTP is str().
-                otp = str(otp)
-
-                # Split OTP in PIN and OTP.
-                pin = otp[:self.pin_len]
-                otp = otp[self.pin_len:]
-
-                # Generate secret from server secret and PIN.
-                secret = self.get_secret(pin=pin,
-                                        mode="mode2",
-                                        callback=callback)
-                # Verify OTP.
-                if not self.verify_otp(otp=pin+otp, secret=secret, mode="mode2"):
-                    msg = "Wrong PIN or token out of sync."
-                    return callback.error(msg)
-
-                self.secret = None
-                return_message = (_("Token switched to mode2."))
-            else:
-                msg = (_("WARNING: Changing token mode to 'mode2' requires "
-                        "re-deployment of the token!"))
-                callback.send(msg)
-                if self.pin:
-                    pin_question = "New PIN (RETURN to keep current PIN): "
-                else:
-                    pin_question = "New PIN: "
-                while True:
-                    new_pin1 = str(callback.askpass(pin_question, null_ok=True))
-                    if new_pin1 == "":
-                        if self.pin:
-                            break
-                        else:
-                            continue
-                    if not self.check_pin(pin=new_pin1, callback=callback):
-                        continue
-                    new_pin2 = callback.askpass("Repeat PIN: ")
-                    if new_pin1 == new_pin2:
-                        self.pin = str(new_pin1)
-                        break
-                self.server_secret = stuff.gen_secret(self.secret_len)
-                token_secret = self.get_secret(pin=self.pin,
-                                                mode="mode2",
-                                                callback=callback)
-                return_message = (_("New token secret: %s") % token_secret)
-                msg = ("Please re-sync token after deploying secret to token!")
-                callback.send(msg)
-                self.pin_enabled = True
-                self.pin_mandatory = True
+        self.card_type = card_type
+        return self._cache(callback=callback)
 
-        # Set new mode.
-        self.mode = new_mode
+    @check_acls(['edit:key_type'])
+    @object_lock()
+    @backend.transaction
+    def change_key_type(self, key_type="rsa", run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Get supported hardware card/token types. """
+        if key_type != "":
+            if not key_type in self.valid_key_types:
+                msg = (_("Unsupported key type: %s") % key_type)
+                return callback.error(msg)
+            if key_type == self.key_type:
+                msg = (_("Key type already set to: %s") % key_type)
+                return callback.error(msg)
 
-        callback.send(return_message)
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_key_type",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception:
+                return callback.error()
 
+        self.key_type = key_type
         return self._cache(callback=callback)
 
-    def _enable_pin(self, pre=False, callback=default_callback, **kwargs):
-        """ Enable token PIN. """
-        return True
-
-    def _disable_pin(self, pre=False, callback=default_callback, **kwargs):
-        """ Disable token PIN. """
-        if not pre:
-            return True
-        if self.mode == "mode2":
-            if self.allow_offline:
-                msg = (_("WARNING: Offline usage is enabled for this token. "
-                        "Anybody who is able to access the offline token file "
-                        "is able to use it for login."))
-                callback.send(msg)
-        return True
-
-    def _change_secret(self, secret=None, pre=False,
-        force=False, callback=default_callback, **kwargs):
-        """ Handle stuff when changing token secret """
-        if self.mode == "mode2":
-            if pre:
-                msg = (_("WARNING: Changing the secret of a token in mode2 is "
-                    "not supported. The secret changes if you change the PIN."))
-                callback.send(msg)
+    @check_acls(['edit:ssh_public_key'])
+    @object_lock()
+    @backend.transaction
+    def change_ssh_public_key(self, ssh_public_key=None, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change token SSH public key. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_ssh_public_key",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception:
                 return callback.error()
-        else:
-            if pre and not force:
-                msg = (_("WARNING: Changing the secret requires a "
-                        "re-deployment of the token."))
-                callback.send(msg)
-                answer = callback.ask("Change token secret?: ")
-                if answer.lower() == "y":
-                    return callback.ok()
-                else:
-                    return callback.error()
-            msg = "Please re-sync token after changing the secret!"
-            callback.send(msg)
-            self.server_secret = None
-        return callback.ok()
-
-    def _change_pin(self, pin=None, pre=False,
-        force=False, callback=default_callback, **kwargs):
-        """ Handle stuff when changing token PIN """
-        if self.mode == "mode2":
-            if pre and not force:
-                msg = (_("WARNING: Changing the PIN of a token in mode2 "
-                        "requires a re-deployment of the token."))
-                callback.send(msg)
-                answer = callback.ask("Change token PIN?: ")
-                if answer.lower() == "y":
-                    return callback.ok()
-                else:
-                    return callback.error()
-            self.server_secret = stuff.gen_secret(self.secret_len)
-            token_secret = self.get_secret(pin=pin, callback=callback)
-            callback.send(_("New token secret: %s") % token_secret)
-            msg = "Please re-sync token after deploying secret to token!"
-            callback.send(msg)
 
-        elif self.server_secret:
-            if pre and not force:
-                msg = (_("WARNING: This token was previously used in mode2. "
-                        "Changing the PIN requires a re-deployment when "
-                        "changing back to mode2."))
-                callback.send(msg)
-                answer = callback.ask("Change token PIN?: ")
-                if answer.lower() == "y":
-                    return callback.ok()
-                else:
-                    return callback.error()
-            self.server_secret = None
-
-        # Update PIN length.
-        if not pre:
-            self.pin_len = len(pin)
-
-        return callback.ok()
-
-    def _enable_offline(self, pre=False, callback=default_callback, **kwargs):
-        """ Handle stuff when enabling offline mode. """
-        if pre:
-            if self.mode == "mode1":
-                msg = (_("WARNING: Anybody who gets access to the offline "
-                        "token file is able to use it for logins and can see "
-                        "your PIN in clear-text!!"))
-                callback.send(msg)
-                msg = (_("You should consider changing token mode to mode2!!"))
-                callback.send(msg)
-            else:
-                msg = (_("INFO: Offline OTP tokens are by design vulnerable "
-                        "for brute force attacks if an attacker is able to "
-                        "steal them (e.g. from a notebook)"))
-                callback.send(msg)
-        return True
-
-    def update_otp_cache(self, otp, counter):
-        """ Add OTP + counter to OTP cache. """
-        self.otp_cache[otp] = counter
-
-    def get_counter_range(self):
-        """ Get start/stop counter for this token. """
-        start = self.get_token_counter() + 1
-        end = start + self.counter_check_range
-        return start, end
+        # Check if we got SSH public key as argument.
+        if ssh_public_key == None:
+            ssh_public_key = callback.ask("Please enter/paste SSH public key: ")
+        if ssh_public_key:
+            self.ssh_public_key = ssh_public_key
+            self.offline_challenge = stuff.gen_md5(ssh_public_key)
+        else:
+            self.ssh_public_key = None
+            self.offline_challenge = None
+        return self._cache(callback=callback)
 
-    @check_acls(['generate:otp'])
-    def gen_otp(self, secret=None, otp_count=1, prefix_pin=False,
-        callback=default_callback, _caller="API", **kwargs):
-        """
-        Generate one or more OTPs for this token within the valid counter range.
-        """
-        if not secret:
-            if self.secret:
-                secret = self.secret
-            else:
-                secret = self.get_secret(pin=prefix_pin, callback=callback)
+    def get_private_key(self, password, instance=False):
+        """ Get decrytped private key. """
+        if not self.ssh_private_key:
+            raise Exception("No private key set.")
+        # Try to decrypt RSA key.
+        try:
+            key = RSAKey(key=self.ssh_private_key, password=password)
+        except Exception as e:
+            msg = (_("Error decrypting private key: %s") % e)
+            raise Exception(msg)
+        if instance:
+            return key
+        private_key = key.private_key_base64
+        return private_key
 
-        if not secret:
-            return callback.error("Unable to get token secret.")
+    def resync(self, callback=default_callback, **kwargs):
+        """ Wrapper method to call resync() of 2ftoken. """
+        try:
+            sftoken = self.get_sftoken()
+        except Exception as e:
+            msg = (_("Error loading second factor token: %s") % e)
+            return callback.error(msg)
+        return sftoken.resync(callback=callback, **kwargs)
 
-        from otpme.lib.otp.oath import hotp
-        token_counter_start, token_counter_end = self.get_counter_range()
-        if otp_count > 1:
-            otps = []
-            for i in range(0, otp_count):
-                token_counter = token_counter_start + i
-                otp = hotp.generate_hotp(token_counter, secret, self.otp_format)
-                if prefix_pin:
-                    otp = "%s%s" % (prefix_pin, otp)
-                self.update_otp_cache(otp, token_counter)
-                otps.append(otp)
-            if _caller == "CLIENT":
-                return callback.ok(otps)
-            return otps
-        token_counter = token_counter_start + 1
-        otp = hotp.generate_hotp(token_counter, secret, self.otp_format)
-        if prefix_pin:
-            otp = "%s%s" % (prefix_pin, otp)
-        self.update_otp_cache(otp, token_counter)
-        if _caller == "CLIENT":
-            return callback.ok(otp)
-        return [otp]
+    def gen_challenge(self, **kwargs):
+        """ Generate challenge to be sigend by users private SSH key. """
+        if not self.ssh_public_key:
+            raise Exception("No SSH public key set.")
+        if self.second_factor_token_enabled:
+            sftoken = self.get_sftoken()
+            otp_len = sftoken.otp_len
+            if sftoken.pin_enabled:
+                otp_len = otp_len + sftoken.pin_len
+            return ssh.gen_challenge(self.ssh_public_key, otp_len=otp_len)
+        else:
+            return ssh.gen_challenge(self.ssh_public_key, otp_len=0)
 
     def test(self, password=None, callback=default_callback, **kwargs):
-        """ Test if the given OTP can be verified by this token. """
+        """ Test if SSH authentication with this token can be verified. """
         ok_message = "Token verified successful."
         error_message = "Token verification failed."
-        if self.pin_enabled:
-            otp_prompt = "PIN+OTP: "
-        else:
-            otp_prompt = "OTP: "
-        if not password:
-            password = callback.askpass(otp_prompt)
-        if not password:
-            return callback.error("Unable to get password.")
-        status = self.verify_otp(otp=str(password), **kwargs)
+
+        try:
+            challenge = self.gen_challenge()
+        except Exception as e:
+            callback.error(_("Unable to generate challenge: %s") % e)
+
+        response = callback.sshauth(challenge=challenge)
+
+        otp = None
+        if self.second_factor_token_enabled:
+            pass_prompt = "OTP: "
+            if not otp:
+                otp = callback.askpass(pass_prompt)
+            if not otp:
+                return callback.error("Unable to get OTP.")
+
+        status = self.verify(challenge=challenge, response=response, otp=otp)
+
         if status:
             return callback.ok(ok_message)
-        return callback.error(error_message)
 
-    def verify(self, challenge=None, response=None, **kwargs):
-        """ Call default verify method. """
-        if challenge and response:
-            return self.verify_mschap_otp(challenge=challenge,
-                                            response=response,
-                                            **kwargs)
-        return self.verify_otp(**kwargs)
+        return callback.error(error_message)
 
-    def verify_otp(self, otp, secret=None, handle_used_otps=True,
-        mode=None, otp_includes_pin=True, verify_pin=True, sft=None,
-        recursive_use=False, session_uuid=None, **kwargs):
-        """ Verify OTP for this token. """
-        pin = None
-        # Make sure OTP is str().
-        otp = str(otp)
+    def verify(self, challenge=None, response=None,
+        otp=None, session_uuid=None, **kwargs):
+        """ Verify challenge/response. """
+        import time
+        if not self.ssh_public_key:
+            logger.warning("Token '%s' is missing SSH public key." % self.name)
+            return None
 
-        if handle_used_otps:
-            if self.is_used_otp(otp):
-                return False
+        if self.second_factor_token_enabled:
+            try:
+                sftoken = self.get_sftoken()
+            except Exception as e:
+                logger.critical("Error loading second factor token: %s" % e)
+                return None
 
-        # Mode indicates for which mode we have to verify the OTP (e.g. if
-        # the OTP includes the PIN)
-        if not mode:
-            mode = self.mode
-
-        # If PIN is disabled OTP does not include a PIN we could verify.
-        if mode == "mode1":
-            if not self.pin_enabled:
+            # Check if token PIN is mandatory. by default we dont want a user to
+            # type in the token PIN when used as second factor token.
+            if sftoken.pin_mandatory:
+                verify_pin = True
+                otp_includes_pin = True
+            else:
                 verify_pin = False
-                # We decide on token mode if OTP includes a PIN because we
-                # allow to "emulate" the given token mode (e.g. use in
-                # change_mode())
                 otp_includes_pin = False
 
-        # Get PIN from OTP if needed.
-        if otp_includes_pin:
-            if len(otp) < (int(self.pin_len) + int(self.otp_len)):
-                msg = ("Token PIN enabled but the given OTP is too "
-                            "short to include a PIN!")
-                logger.debug(msg)
+            cutoff_len = sftoken.otp_len
+            if otp_includes_pin:
+                cutoff_len += sftoken.pin_len
+
+            if len(otp) <= cutoff_len:
+                logger.debug("Second factor OTP token enabled but password is "
+                            "too short to include a OTP.")
                 return None
-            _otp = otp[self.pin_len:]
-            pin = otp[:self.pin_len]
+            password = otp[:-cutoff_len]
+            otp = otp[-cutoff_len:]
         else:
-            _otp = otp
+            password = otp
 
-        # If we got a secret this request is to verify the secret itself
-        # (e.g. mode change)
-        if not secret:
-            # Get token secret.
-            secret = self.get_secret(pin=pin)
-
-        # Get token counter check range.
-        token_counter_start, token_counter_end = self.get_counter_range()
-
-        # Tokens do not include a PIN in offline config we could verify here.
-        # The PIN is verified in different ways:
-        # - in mode1 by using it to en-/decrypt the token config.
-        # - in mode2 the token secret is derived from server_secret+PIN and
-        #   thus OTP verification fails with the wrong PIN.
-        # If not used as second factor token we also have no PIN length in
-        # our config to make brute force attacks harder and thus we have to
-        # try all possible PIN lengths. The increased load should not be
-        # noticeable and outweigh the added security.
-        if self.offline and self.pin_enabled:
-            verify_pin = False
-            if not sft and not recursive_use:
-                org_pin_len = self.pin_len
-                self.pin_len = 0
-                while True:
-                    if self.pin_len >= (len(otp) - self.otp_len):
-                        self.pin_len = org_pin_len
-                        return None
-                    self.pin_len += 1
-                    status = self.verify_otp(otp,
-                                            secret=secret,
-                                            handle_used_otps=handle_used_otps,
-                                            mode=mode,
-                                            otp_includes_pin=otp_includes_pin,
-                                            verify_pin=False,
-                                            sft=None,
-                                            recursive_use=True,
-                                            **kwargs)
-                    if status:
-                        self.pin_len = org_pin_len
-                        return status
-
-        # Log token counter range.
-        msg = ("Verifiying OTP within counter range: start='%s' end='%s'."
-                % (token_counter_start, token_counter_end))
-        logger.debug(msg)
-
-        # Verify OTP.
-        hotp_status, \
-        hotp_count = hotp.verify_hotp(counter_start=token_counter_start,
-                                    counter_end=token_counter_end,
-                                    secret=secret, otp=_otp,
-                                    format=self.otp_format)
-        if hotp_status:
-            self.update_otp_cache(otp, hotp_count)
-            if otp_includes_pin:
-                self.update_otp_cache(_otp, hotp_count)
-            # Make sure the OTP was not already used (counter must be higher
-            # than the one from the last used OTP).
-            if hotp_count > self.get_token_counter():
-                # Verify PIN.
-                if verify_pin:
-                    if pin != self.pin:
-                        logger.debug("Got wrong token PIN: %s" % self.rel_path)
-                        # FIXME: A wrong PIN is not definitively a failed
-                        #        login with this token because it may be
-                        #        used as a second factor token (e.g. a
-                        #        password token) where a static password
-                        #        is prefixed and the PIN verification is
-                        #        disabled. It would be nice to prevent
-                        #        brute forcing the PIN with a stolen OTP
-                        #        here but for this we need to change the
-                        #        concept of add_used_otp() here and in
-                        #        User().authenticate()
-                        return None
-
-                if handle_used_otps:
-                    # Only log message for the first OTP we add.
-                    self.add_used_otp(otp=otp,
-                                    session_uuid=session_uuid,
-                                    quiet=False)
-                    if otp_includes_pin:
-                        self.add_used_otp(otp=_otp, session_uuid=session_uuid)
-                return otp
-
-        # Default should be None (which means no valid OTP found but not
-        # definitively failed because we havent found an already used OTP)
-        return None
-
-        # This point should never be reached.
-        msg = (_("WARNING: You may have hit a BUG of Token().verify_otp()."))
-        raise Exception(msg)
-
-    def verify_static(self, **kwargs):
-        """ Verify given password against 'password' token. """
-        msg = (_("Verifying static passwords is not supported with token type: "
-                "'%s'.") % self.token_type)
-        raise OTPmeException(msg)
-
-    def verify_mschap_static(self, **kwargs):
-        """ Verify MSCHAP challenge/response against static passwords. """
-        msg = (_("Verifying an static MSCHAP request is not supported with "
-                "token type '%s'.") % self.token_type)
-        raise OTPmeException(msg)
-
-    def verify_mschap_otp(self, challenge, response,
-        session_uuid=None, handle_used_otps=True, **kwargs):
-        """ Verify MSCHAP challenge/response against OTPs """
-        from otpme.lib.otp.oath import hotp
-        from otpme.lib import mschap_util
+        # In offline mode the token config is encrypted via challenge/response
+        # procedure using the SSH private key. The offline challenge is the MD5
+        # sum of the SSH public key. If decryption was successful the token is
+        # verified successful. We do this to make offline logins faster because
+        # we need only one singing process via ssh-agent.
+        if self.offline and not password:
+            public_key_md5 = stuff.gen_md5(self.ssh_public_key)
+            if self.offline_challenge != public_key_md5:
+                logger.warning("Failed to verify offline challenge.")
+                return False
 
-        nt_key = None
-        otp = None
-        pin = None
-        _otp = None
+        elif password:
+            if not self.ssh_private_key:
+                logger.debug("Skipping token without SSH private key for "
+                            "password authentication: %s" % self.rel_path)
+                return None
+            # Try to decrypt private key.
+            try:
+                self._ssh_private_key = self.get_private_key(password=password)
+                # When authenticating with the private key encryption passphrase
+                # set our pass type to static.
+                self.pass_type = "static"
+            except:
+                # If we got the wrong password this is not a failure because
+                # it may match an other token. So we continue to next token.
+                return None
 
-        # Set PIN we need to prefix our OTPs with needed.
-        if self.pin_enabled:
-            pin = self.pin
-
-        # Get token secret.
-        secret = self.get_secret(pin=pin)
-
-        # Get token counter check range.
-        token_counter_start, token_counter_end = self.get_counter_range()
-
-        # Get list with valid OTPs of this token for the given counter range.
-        otps = self.gen_otp(otp_count=self.counter_check_range,
-                            prefix_pin=pin, verify_acls=False)
-
-        # Set default return values.
-        return_value = None, None, None
-        failed_return_value = False, None, None
-
-        msg = ("Verifiying OTP within counter range: start='%s' end='%s'."
-                % (token_counter_start, token_counter_end))
-        logger.debug(msg)
-
-        # Walk through all valid OTPs.
-        for _otp in otps:
-            # Get NT key from verify().
-            status, \
-            nt_key = mschap_util.verify(stuff.gen_nt_hash(_otp),
-                                        challenge, response)
-            if status:
-                if self.pin_enabled:
-                    otp = _otp[self.pin_len:]
-                    check_otp = otp
-                else:
-                    check_otp = _otp
-
-                # Verify OTP.
-                hotp_status, \
-                hotp_count = hotp.verify_hotp(counter_start=token_counter_start,
-                                            counter_end=token_counter_end,
-                                            secret=secret, otp=check_otp,
-                                            format=self.otp_format)
-
-                if hotp_status:
-                    # Make sure the OTP was not already used (counter must be higher
-                    # than the one from the last used OTP).
-                    if hotp_count > self.get_token_counter():
-                        if handle_used_otps:
-                            if self.is_used_otp(_otp):
-                                return failed_return_value
-                            # Add OTP to used OTPs.
-                            self.update_otp_cache(_otp, hotp_count)
-                            self.add_used_otp(otp=_otp,
-                                session_uuid=session_uuid)
-                            # Add OTP without PIN to used OTPs.
-                            if otp:
-                                self.update_otp_cache(otp, hotp_count)
-                                self.add_used_otp(otp=otp,
-                                                session_uuid=session_uuid,
-                                                quiet=False)
-                        return status, nt_key, _otp
-
-        # Default should be None (which means no valid OTP found but not
-        # definitively failed because we havent found an already used OTP)
-        return return_value
-
-        # This point should never be reached.
-        msg = ("WARNING: You may have hit a BUG of Token().verify_mschap_otp().")
-        raise Exception(msg)
+        elif challenge and response:
+            if not ssh.verify_sign(public_key=decode(self.ssh_public_key, "base64"),
+                                    data=decode(response, "base64"),
+                                    plaintext=challenge):
+                logger.warning("Verifying SSH response failed.")
+                return False
+
+            challenge_time = int(challenge.split(":")[0])
+            epoch_time = int(time.time())
+            challenge_age = epoch_time - challenge_time
+            if challenge_age > 15:
+                logger.warning("SSH challenge too old.")
+                return False
+        else:
+            return None
+
+        # If no second factor token is configured we are done.
+        if not self.second_factor_token_enabled:
+            return True
+
+        # Verify second factor token.
+        logger.debug("Verifying second factor token: %s" % sftoken.rel_path)
+        if sftoken.verify_otp(otp,
+                            session_uuid=session_uuid,
+                            otp_includes_pin=otp_includes_pin,
+                            verify_pin=verify_pin, sft=True):
+            return True
+        return False
 
-    @check_acls(['generate:otp'])
-    def gen_mschap(self, run_policies=True,
+    @check_acls(['edit:2ftoken'])
+    @object_lock()
+    @backend.transaction
+    def change_2f_token(self, second_factor_token, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Generate MSCHAP challenge response stuff for testing. """
+        """ Change token second factor token. """
+        if second_factor_token == "":
+            self.second_factor_token = second_factor_token
+
+        # Get user instance of token owner.
+        user = backend.get_object(object_type="user", uuid=self.owner_uuid)
+        # Get token instance of 2f_token by name.
+        token = user.token(second_factor_token)
+
+        if not token:
+            msg = (_("Token '%s' does not exist.") % second_factor_token)
+            return callback.error(msg)
+        if token.pass_type != "otp":
+            msg = (_("Token '%s' is not an OTP token.") % second_factor_token)
+            return callback.error(msg)
+
         if run_policies:
             try:
-                self.run_policies("gen_mschap",
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_ssh_public_key",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
-        pin = None
-        if self.mode == "mode1":
-            if self.pin_enabled:
-                pin = self.pin
-        if self.mode == "mode2":
-            pin = self.pin
-        otp = self.gen_otp(prefix_pin=pin, verify_acls=False)[0]
-        return Token._gen_mschap(self, password=otp, callback=callback)
 
-    @check_acls(['generate:qrcode'])
-    def gen_qrcode(self, qrcode_file=None, run_policies=True,
+        # Set 2f token.
+        self.second_factor_token = token.uuid
+        return self._cache(callback=callback)
+
+    @check_acls(['enable:2ftoken'])
+    @object_lock()
+    @backend.transaction
+    def enable_2f_token(self, force=False, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Generate QRCode for token deployment. """
+        """ Enable the second factor token. """
+        if self.second_factor_token_enabled:
+            return callback.error("Second factor token already enabled.")
+
+        if self.second_factor_token == "":
+            return callback.error("No second factor token configured.")
+
+        # Check if second factor token is available.
+        try:
+            self.get_sftoken(callback=callback)
+        except Exception as e:
+            msg = (_("Unable to enable second factor token: %s") % e)
+            return callback.error(msg)
+
         if run_policies:
             try:
-                self.run_policies("gen_qrcode",
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("enable_2f_token",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        # Get secret to gen QRCode.
-        secret = self.get_secret()
+        if not force:
+            if self.confirmation_policy == "paranoid":
+                answer = callback.ask("Enable second factor token?: ")
+                if answer.lower() != "y":
+                    return callback.abort()
 
-        token_counter_start, token_counter_end = self.get_counter_range()
-
-        # Gen OATH URI.
-        user_string = "%s@%s" % (self.rel_path, self.realm)
-        #oath_uri = HOTP(secret, "hex")
-        #oath_uri = oath_uri.provisioning_uri(name=user_string,
-        #                                    issuer_name=config.my_name,
-        #                                    initial_count=token_counter_start)
-        # Use oath-toolkit.
-        oath_uri = uri.generate(key_type=self.token_type,
-                                key=decode(secret, "hex"),
-                                user=user_string,
-                                issuer=config.my_name,
-                                counter=token_counter_start)
-        # Generate QRcode.
-        _qrcode = qrcode.gen_qrcode(oath_uri, "terminal")
-        # xxxxxxxxxxxxx
-        # FIXME: How to create png/svg image without writing to file?
-        return callback.ok(_qrcode)
+        self.second_factor_token_enabled = True
+        return self._cache(callback=callback)
 
-    @check_acls(['resync'])
+    @check_acls(['disable:2ftoken'])
     @object_lock()
     @backend.transaction
-    def resync(self, otp=None, run_policies=True,
+    def disable_2f_token(self, force=False, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Resync our counter state with token by given OTP. """
-        from otpme.lib.otp.oath import hotp
-        if not otp:
-            otp = callback.askpass("Please enter OTP: ")
-
-        if not otp:
-            return callback.error("Unable to get OTP.")
-
-        # Make sure OTP is str().
-        otp = str(otp)
-
-        if len(otp) < self.otp_len:
-            return callback.error("OTP too short.")
-        if len(otp) > self.otp_len:
-            return callback.error("OTP too long.")
+        """ Disable the second factor token. """
+        if not self.second_factor_token_enabled:
+            return callback.error("Second factor token already disabled.")
 
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
-                self.run_policies("resync",
+                self.run_policies("disable_2f_token",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        # Get token secret.
-        token_secret = self.get_secret(pin=self.pin, callback=callback)
+        if not force:
+            if self.confirmation_policy == "paranoid":
+                answer = callback.ask("Disable second factor token?: ")
+                if answer.lower() != "y":
+                    return callback.abort()
 
-        # Get current token counter.
-        current_counter = self.get_token_counter()
-
-        # Get resync check range.
-        resync_check_range = self.get_config_parameter("hotp_resync_check_range")
-
-        # We will check resync_check_range below and above the current counter.
-        token_counter_start = 0
-        if current_counter >= resync_check_range:
-            token_counter_start = current_counter - resync_check_range
-        token_counter_end = current_counter + resync_check_range
-
-        hotp_status, \
-        hotp_count = hotp.verify_hotp(counter_start=token_counter_start,
-                                        counter_end=token_counter_end,
-                                        secret=token_secret,
-                                        otp=otp,
-                                        format=self.otp_format)
-        if not hotp_status:
-            return callback.error("Unable to synchronize token.")
-
-        # Add OTP with counter to our cache.
-        self.update_otp_cache(otp, hotp_count)
-        # Set new sync timestamp.
-        self.counter_sync_time = time.time()
+        self.second_factor_token_enabled = False
+        return self._cache(callback=callback)
 
-        try:
-            self.add_used_otp(otp, resync=True)
-        except Exception as e:
-            msg = "Error adding OTP to list of used OTPs: %s" % e
-            return callback.error(msg)
+    @object_lock()
+    @backend.transaction
+    def deploy(self, public_key=None, private_key=None, password=None,
+        pass_hash_type="PBKDF2", _caller="API", verbose_level=0,
+        callback=default_callback):
+        """ Deploy SSH token. """
+        if not public_key and not private_key:
+            return callback.error("Need at least public or private key.")
+        if private_key:
+            if not password:
+                return callback.error("Need password to add private key.")
 
-        if self.allow_offline:
-            msg = (_("Offline usage enabled for token. You "
-                    "should re-login after token resync!"))
+            msg = (_("Setting SSH private key to token: %s") % self.rel_path)
             callback.send(msg)
 
-        msg = (_("Token synchronized successful. Current counter: %s")
-                % hotp_count)
-        callback.send(msg)
+            # Encrypt private key with password.
+            rsa_key = RSAKey(key=private_key)
+            self.ssh_private_key = rsa_key.encrypt_key(password=password,
+                                                    hash_type=pass_hash_type)
+            # Get public key from private key if not given.
+            if not public_key:
+                public_key = rsa_key.ssh_public_key.split(" ")[1]
+            # We cannot support cross site token links if the token includes
+            # a SSH private key.
+            self.cross_site_links = False
 
-        return self._cache(callback=callback)
-
-    def add_used_otp(self, otp, resync=False, session_uuid=None, quiet=True):
-        """ Add used OTP + counter for this user/token. """
-        try:
-            token_counter = self.otp_cache[otp]
-        except:
-            msg = ("WARNING: Unable to find counter for the given OTP.")
-            raise OTPmeException(msg)
-
-        # Add used token counter using parent class method.
-        Token._add_token_counter(self, token_counter=token_counter,
-                                session_uuid=session_uuid)
-
-        # Update counter in token config on resync.
-        if resync:
-            self.object_config['COUNTER'] = token_counter
-
-        # FIXME: how long to cache already used HOTPs?
-        expiry = time.time() + 86400
-
-        # In offline mode we do not add used OTPs to make brute force attacks
-        # harder (no OTP hash saved to disk)
-        if self.offline:
-            return True
+        msg = (_("Setting SSH public key to token: %s") % self.rel_path)
+        callback.send(msg)
 
-        # Add used OTP using parent class method
-        try:
-            Token._add_used_otp(self,
-                                otp=otp,
-                                expiry=expiry,
-                                session_uuid=session_uuid,
-                                sync_time=self.counter_sync_time,
-                                quiet=quiet)
-        except Exception as e:
-            msg = "Failed to add used OTP: %s" % e
-            raise OTPmeException(msg)
+        self.ssh_public_key = public_key
 
-    def _check_range_format(self, check_range, callback=default_callback):
-        """ Check if the given counter range is valid. """
-        if isinstance(check_range, int):
-            if check_range > 0:
-                return callback.ok()
-            msg = (_("Counter check range must be greater than 0."))
-            return callback.error(msg)
-        msg = "Counter check range must be an integer."
-        return callback.error(msg)
+        return self._cache(callback=callback)
 
-    @check_acls(['edit:counter_check_range'])
+    @check_acls(['edit:password'])
     @object_lock()
     @backend.transaction
-    def change_counter_check_range(self, run_policies=True,
-        counter_check_range=None, _caller="API",
-        callback=default_callback, **kwargs):
-        """ Change token counter check range. """
+    def change_key_password(self, force=False, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change private key encryption password. """
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
-                self.run_policies("change_counter_check_range",
+                self.run_policies("change_password",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        if counter_check_range == None:
-            while True:
-                answer = callback.ask("Counter check range: ")
-                try:
-                    counter_check_range = int(answer)
-                except:
-                    pass
-                check_status, \
-                check_message = self._check_range_format(counter_check_range)
-                if check_status:
-                    break
-                else:
-                    callback.send(check_message)
-        else:
-            check_status, \
-            check_message = self._check_range_format(counter_check_range)
-            if not check_status:
-                return callback.error(check_message)
-
-        self.counter_check_range = counter_check_range
+        is_admin = False
+        if config.auth_token:
+            is_admin = config.auth_token.is_admin()
+        elif config.use_api:
+            is_admin = True
 
-        return self._cache(callback=callback)
-
-    @object_lock()
-    def pre_deploy(self, _caller="API", verbose_level=0,
-        callback=default_callback, **kwargs):
-        reply = {
-                'secret_len'    : self.secret_len,
-                }
-        return callback.ok(reply)
+        current_pass = callback.askpass("Current password: ")
+        try:
+            private_key = self.get_private_key(password=current_pass,
+                                                    instance=True)
+        except:
+            return callback.error("Wrong password.")
 
-    @object_lock()
-    @backend.transaction
-    def deploy(self, server_secret, pin, _caller="API",
-        verbose_level=0, callback=default_callback):
-        """ Deploy HOTP token """
-        if not self.check_pin(pin=pin, callback=callback):
-            return callback.error("Failed to set token PIN.")
+        password_checked = False
+        while True:
+            new_password1 = callback.askpass("New password: ")
+            if not force or not is_admin:
+                if not self.check_password(new_password1,
+                                        callback=callback):
+                    return callback.error()
+                password_checked = True
 
-        msg = (_("Setting received server secret to token: %s") % self.rel_path)
-        callback.send(msg)
+            new_password2 = callback.askpass("Re-type password: ")
+            if new_password1 == new_password2:
+                password = new_password1
+                break
+            else:
+                return callback.error("Sorry, passwords do not match.")
 
-        self.server_secret = str(server_secret)
+        # Make sure password is a string.
+        password = str(password)
 
-        msg = (_("Setting received PIN to token: %s") % self.rel_path)
-        callback.send(msg)
+        if password == "":
+            return callback.error("Cannot set empty password.")
 
-        self.pin = str(pin)
-        self.secret = None
-        self.mode = "mode2"
-
-        if verbose_level > 0:
-            token_secret = self.get_secret()
-            msg = (_("Token secret: %s") % token_secret)
-            callback.send(msg)
+        if not force or not is_admin:
+            if not password_checked:
+                 if not self.check_password(password, callback=callback):
+                    return callback.error()
 
-        msg = ("You have to resync the token after re-deploying.")
-        callback.send(msg)
+        if not force or not is_admin:
+            if len(password) < self.password_min_len:
+                msg = (_("Password too short (%s).") % self.password_min_len)
+                return callback.error(msg)
+            if len(password) > self.password_max_len:
+                msg = (_("Password too long (%s).") % self.password_max_len)
+                return callback.error(msg)
+
+        # Encrypt private key with new password.
+        #rsa_key = RSAKey(key=private_key)
+        #self.ssh_private_key = rsa_key.encrypt_key(password=password)
+        self.ssh_private_key = private_key.encrypt_key(password=password)
 
         return self._cache(callback=callback)
 
     @object_lock()
     @backend.transaction
-    def _add(self, gen_qrcode=True, callback=default_callback, **kwargs):
+    def _add(self, public_key=None, callback=default_callback, **kwargs):
         """ Add a token. """
-        # Get default HOTP settings.
-        self.otp_format = self.get_config_parameter("hotp_format")
-        self.counter_check_range = self.get_config_parameter("hotp_check_range")
-        # Gen server secret.
-        self.server_secret = stuff.gen_secret(self.secret_len)
-        # Gen PIN.
-        default_pin_len = self.get_config_parameter("hotp_default_pin_len")
-        self.pin = stuff.gen_pin(default_pin_len)
-        self.pin_len = len(self.pin)
-        # Get token secret.
-        token_secret = self.get_secret(pin=self.pin, callback=callback)
-        # Generate salt for used OTP hashes.
-        self.used_otp_salt = stuff.gen_secret(32)
         return_message = None
-        if self.verify_acl("view:secret"):
-            if gen_qrcode:
-                term_qrcode = self.gen_qrcode(run_policies=False)
-                callback.send(term_qrcode)
-            return_message = "Token secret: %s" % token_secret
-        if self.verify_acl("view:pin"):
-            message = "Token PIN: %s" % self.pin
-            if return_message:
-                return_message = "%s\n%s" % (return_message, message)
-            else:
-                return_message = message
-        return callback.ok(return_message)
+        if public_key:
+            self.ssh_public_key = public_key
+        else:
+            return_message = (_("NOTE: You have to add an SSH public key to "
+                                "this token to make it usable."))
 
-    @check_acls(['view_all:secret'])
-    def show_secret(self, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Show object secret. """
-        if run_policies:
-            try:
-                self.run_policies("show_secret",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
+        sf_note = (_("NOTE: You may want to add a second factor token "
+                    "(e.g. OTP token) to improve security."))
 
-        token_secret = self.get_secret(callback=callback)
-        callback.send(token_secret)
-        return callback.ok()
+        if return_message:
+            return_message = "%s\n%s" % (return_message, sf_note)
+        else:
+            return_message = sf_note
+
+        return callback.ok(return_message)
 
     def show_config(self, callback=default_callback, **kwargs):
-        """ Show token info. """
+        """ Show token config. """
         if not self.verify_acl("view_public:object"):
             msg = ("Permission denied.")
             return callback.error(msg, exception=PermissionDenied)
+
+        second_factor_token_name = ""
+        if self.verify_acl("view:2ftoken"):
+            # Get 2f token instance.
+            if self.second_factor_token:
+                try:
+                    sftoken = self.get_sftoken()
+                    second_factor_token_name = sftoken.name
+                except Exception as e:
+                    callback.send(_("Error loading second factor token: %s")
+                                    % e)
         lines = []
 
-        counter_check_range = ""
-        if self.verify_acl("view:counter_check_range") \
-        or self.verify_acl("edit:counter_check_range"):
-            counter_check_range = str(self.counter_check_range)
-        lines.append('COUNTER_CHECK_RANGE="%s"' % counter_check_range)
-
-        counter_sync_time = ""
-        if self.verify_acl("view:counter_sync_time") \
-        or self.verify_acl("resync"):
-            counter_sync_time = str(self.counter_sync_time)
-        lines.append('COUNTER_SYNC_TIME="%s"' % counter_sync_time)
-
-        server_secret = ""
-        if self.verify_acl("view:server_secret"):
-            server_secret = str(self.server_secret)
-        lines.append('SERVER_SECRET="%s"' % server_secret)
+        if self.verify_acl("view:ssh_public_key"):
+            lines.append('SSH_PUBLIC_KEY="%s"' % self.ssh_public_key)
+        else:
+            lines.append('SSH_PUBLIC_KEY=""')
+
+        if self.verify_acl("view_all:ssh_private_key"):
+            lines.append('SSH_PRIVATE_KEY="%s"' % self.ssh_private_key)
+        else:
+            lines.append('SSH_PRIVATE_KEY=""')
+
+        if self.verify_acl("view:key_type"):
+            lines.append('KEY_TYPE="%s"' % self.key_type)
+        else:
+            lines.append('KEY_TYPE=""')
+
+        lines.append('SECOND_FACTOR_TOKEN="%s"' % second_factor_token_name)
+
+        if self.verify_acl("view:2ftoken_status"):
+            lines.append('SECOND_FACTOR_TOKEN_ENABLED="%s"'
+                        % self.second_factor_token_enabled)
+        else:
+            lines.append('SECOND_FACTOR_TOKEN_ENABLED=""')
+
+        if self.verify_acl("view:card_type"):
+            lines.append('CARD_TYPE="%s"' % self.card_type)
+        else:
+            lines.append('CARD_TYPE=""')
+
+        lines.append('OFFLINE_CHALLENGE="%s"' % self.offline_challenge)
 
         return Token.show_config(self,
                                 config_lines=lines,
                                 callback=callback,
                                 **kwargs)
+
     def show(self, **kwargs):
-        """ Show token details """
+        """ Show token details. """
         #if not self.verify_acl("view_public:object"):
         #    msg = ("Permission denied.")
         #    return callback.error(msg, exception=PermissionDenied)
         return self.show_config(**kwargs)
```

### Comparing `otpme-0.3.0a45/otpme/lib/token/link/link.py` & `otpme-0.3.0a46/otpme/lib/token/link/link.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/motp/motp.py` & `otpme-0.3.0a46/otpme/lib/token/motp/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/otp_push/otp_push.py` & `otpme-0.3.0a46/otpme/lib/token/otp_push/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/otpme/otpme.py` & `otpme-0.3.0a46/otpme/lib/token/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/password/password.py` & `otpme-0.3.0a46/otpme/lib/token/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/script_otp/script_otp.py` & `otpme-0.3.0a46/otpme/lib/token/script_otp/script_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/script_static/script_static.py` & `otpme-0.3.0a46/otpme/lib/token/script_static/script_static.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/ssh/ssh.py` & `otpme-0.3.0a46/otpme/lib/token/hotp/hotp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2014 the2nd <the2nd@otpme.org>
 # Distributed under the terms of the GNU General Public License v2
 import os
+import time
+#from pyotp.hotp import HOTP
 
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
     pass
 
-from otpme.lib import ssh
 from otpme.lib import stuff
 from otpme.lib import config
+from otpme.lib import qrcode
 from otpme.lib import backend
 from otpme.lib import otpme_acl
-from otpme.lib.classes.token import Token
+from otpme.lib.otp.oath import hotp
 from otpme.lib.locking import object_lock
 from otpme.lib.otpme_acl import check_acls
 from otpme.lib.encoding.base import decode
-from otpme.lib.encryption.rsa import RSAKey
+from otpme.lib.token.oath.oath import OathToken
+from otpme.lib.third_party.oath_toolkit import uri
+from otpme.lib.token.oath.oath import OATH_OTP_FORMATS
 from otpme.lib.protocols.utils import register_commands
+
 from otpme.lib.classes.token \
             import get_acls \
             as _get_acls
 from otpme.lib.classes.token \
             import get_value_acls \
             as _get_value_acls
 from otpme.lib.classes.token \
@@ -31,206 +36,207 @@
             as _get_default_acls
 from otpme.lib.classes.token \
             import get_recursive_default_acls \
             as _get_recursive_default_acls
 
 from otpme.lib.exceptions import *
 
-default_callback = config.get_callback()
-
 logger = config.logger
 
+default_callback = config.get_callback()
+
 read_acls =  []
-write_acls =  []
+write_acls =  [
+                "generate",
+                "resync",
+        ]
 
 read_value_acls = {
                 "view"      : [
-                            "2ftoken",
-                            "2ftoken_status",
-                            "card_type",
-                            "key_type",
-                            "ssh_public_key",
-                            "ssh_private_key",
+                            "secret",
+                            "server_secret",
+                            "pin",
                             "auth_script",
+                            "otp_format",
+                            "counter_check_range",
+                            "mode",
+                            "counter_sync_time",
                             "offline_status",
                             "offline_expiry",
                             "offline_unused_expiry",
                             "session_keep",
-                            "signature",
                             ],
-                }
+        }
 
 write_value_acls = {
-                "add"       : [
-                            "signature",
-                            ],
-                "delete"    : [
-                            "signature",
-                            ],
-                "verify"    : [
-                            "signature",
+                "generate"  : [
+                            "otp",
+                            "qrcode",
                             ],
                 "edit"      : [
-                            "2ftoken",
-                            "card_type",
-                            "key_type",
-                            "password",
-                            "ssh_public_key",
-                            "ssh_private_key",
+                            "secret",
+                            "pin",
                             "auth_script",
+                            "otp_format",
+                            "counter_check_range",
+                            "mode",
                             "offline_expiry",
                             "offline_unused_expiry",
                             ],
                 "enable"    : [
-                            "2ftoken",
+                            "pin",
                             "auth_script",
                             "offline",
                             "session_keep",
                             ],
                 "disable"   : [
-                            "2ftoken",
+                            "pin",
                             "auth_script",
                             "offline",
                             "session_keep",
                             ],
-                }
+            }
 
 default_acls = []
 
 recursive_default_acls = []
 
 commands = {
-    'password'   : {
+    'secret'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_key_password',
-                    'oargs'             : ['auto_password', 'password'],
+                    'method'            : 'change_secret',
+                    'oargs'             : ['auto_secret', 'secret'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'ssh_public_key'   : {
+    'pin'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_ssh_public_key',
-                    'oargs'             : ['ssh_public_key'],
+                    'method'            : 'change_pin',
+                    'oargs'             : ['auto_pin', 'pin'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'test'   : {
+    'enable_pin'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'test',
-                    'oargs'             : ['password'],
+                    'method'            : 'enable_pin',
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'disable_pin'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'disable_pin',
                     'job_type'          : 'process',
                     },
                 },
             },
-    '2f_token'   : {
+    'show_secret'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_2f_token',
-                    'args'              : ['second_factor_token'],
+                    'method'            : 'show_secret',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'enable_2f'   : {
+    'show_pin'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'enable_2f_token',
+                    'method'            : 'show_pin',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'disable_2f'   : {
+    'gen'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'disable_2f_token',
+                    'method'            : 'gen_otp',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'card_type'   : {
+    'gen_mschap'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_card_type',
-                    'args'              : ['card_type'],
+                    'method'            : 'gen_mschap',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'key_type'   : {
+    'gen_qrcode'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_key_type',
-                    'args'              : ['key_type'],
+                    'method'            : 'gen_qrcode',
+                    'oargs'             : ['qrcode_file'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'sign'   : {
+    'resync'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'sign',
-                    'oargs'             : ['tags', 'stdin_pass'],
+                    'method'            : 'resync',
+                    'oargs'             : ['otp'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'resign'   : {
+    'test'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'resign',
+                    'method'            : 'test',
+                    'oargs'             : ['password'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'add_sign'   : {
+    'otp_format'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_sign',
-                    'oargs'             : ['signature', 'tags'],
+                    'method'            : 'change_otp_format',
+                    'args'              : ['otp_format'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'del_sign'   : {
+    'mode'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'del_sign',
-                    'oargs'             : ['username', 'tags'],
+                    'method'            : 'change_mode',
+                    'args'              : ['new_mode'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'verify_sign'   : {
+    'counter_check_range'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'verify_sign',
-                    'oargs'             : ['username', 'user_uuid', 'tags'],
+                    'method'            : 'change_counter_check_range',
+                    'oargs'             : ['counter_check_range'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'get_sign_data'   : {
+    'enable_mschap'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'get_sign_data',
-                    'oargs'             : ['tags'],
+                    'method'            : 'enable_mschap',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'get_sign'   : {
+    'disable_mschap'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'get_sign',
-                    'oargs'             : ['username', 'user_uuid', 'tags'],
+                    'method'            : 'disable_mschap',
                     'job_type'          : 'process',
                     },
                 },
             },
     }
 
 def get_acls(split=False, **kwargs):
@@ -275,751 +281,731 @@
     return _acls
 
 REGISTER_BEFORE = []
 REGISTER_AFTER = []
 
 def register():
     """ Register object. """
+    register_hooks()
     register_token_type()
+    register_config_params()
     register_commands("token",
                     commands,
-                    sub_type="ssh",
+                    sub_type="hotp",
                     sub_type_attribute="token_type")
 
 def register_hooks():
     config.register_auth_on_action_hook("token", "resync")
-    config.register_auth_on_action_hook("token", "change_key_type")
-    config.register_auth_on_action_hook("token", "change_card_type")
-    config.register_auth_on_action_hook("token", "change_2f_token")
-    config.register_auth_on_action_hook("token", "enable_2f_token")
-    config.register_auth_on_action_hook("token", "disable_2f_token")
-    config.register_auth_on_action_hook("token", "add_sign")
-    config.register_auth_on_action_hook("token", "del_sign")
-    config.register_auth_on_action_hook("token", "change_ssh_public_key")
+    config.register_auth_on_action_hook("token", "gen_mschap")
+    config.register_auth_on_action_hook("token", "gen_qrcode")
+    config.register_auth_on_action_hook("token", "change_mode")
+    config.register_auth_on_action_hook("token", "show_secret")
+    config.register_auth_on_action_hook("token", "change_counter_check_range")
 
 def register_token_type():
     """ Register token type. """
-    config.register_sub_object_type("token", "ssh")
+    config.register_sub_object_type("token", "hotp")
 
-class SshToken(Token):
-    """ Class for SSH tokens. """
+def register_config_params():
+    """ Register config params. """
+    # Valid object types for our config parameters..
+    object_types = [
+                    'realm',
+                    'site',
+                    'unit',
+                    'user',
+                ]
+    # Default HOTP OTP format.
+    config.register_config_parameter(name="hotp_format",
+                                    ctype=str,
+                                    default_value="dec6",
+                                    valid_values=list(OATH_OTP_FORMATS),
+                                    object_types=object_types)
+    # Counter check range when doing HOTP auth.
+    config.register_config_parameter(name="hotp_check_range",
+                                    ctype=int,
+                                    default_value=32,
+                                    object_types=object_types)
+    # Counter check range when doing token resync.
+    config.register_config_parameter(name="hotp_resync_check_range",
+                                    ctype=int,
+                                    default_value=1024,
+                                    object_types=object_types)
+    # The HOTP default PIN length.
+    config.register_config_parameter(name="hotp_default_pin_len",
+                                    ctype=int,
+                                    default_value=4,
+                                    object_types=object_types)
+    # The HOTP secret length.
+    config.register_config_parameter(name="hotp_secret_len",
+                                    ctype=int,
+                                    default_value=40,
+                                    object_types=object_types)
+
+class HotpToken(OathToken):
+    """ Class for OATH HOTP tokens. """
     def __init__(self, object_id=None, user=None, name=None,
         realm=None, site=None, path=None, **kwargs):
-
         # Call parent class init.
-        super(SshToken, self).__init__(object_id=object_id,
-                                            realm=realm,
-                                            site=site,
-                                            user=user,
-                                            name=name,
-                                            path=path,
-                                            **kwargs)
+        super(HotpToken, self).__init__(object_id=object_id,
+                                        realm=realm,
+                                        site=site,
+                                        user=user,
+                                        name=name,
+                                        path=path,
+                                        **kwargs)
 
         self._acls = get_acls()
         self._value_acls = get_value_acls()
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
-        # Set token type.
-        self.token_type = "ssh"
-        # Set password type.
-        self.pass_type = "ssh_key"
-        # Set SSH key type.
-        self.key_type = "rsa"
-        self.valid_key_types = [ "rsa", "dsa" ]
+
         # Set default values.
-        self.ssh_public_key = None
-        self.ssh_private_key = None
-        # Will hold decrypted SSH private key.
-        self._ssh_private_key = None
-        # Challenge to verify in offline mode.
-        self.offline_challenge = ""
-        # FIXME: allow to modify this list!?
-        # Valid token options (e.g. command=/some/script/path)
-        self.valid_token_options = [
-                                'cert-authority',
-                                'command',
-                                'restrict',
-                                'environment',
-                                'from',
-                                'no-agent-forwarding',
-                                'no-port-forwarding',
-                                'no-pty',
-                                'no-user-rc',
-                                'no-X11-forwarding',
-                                'permitopen',
-                                'principals',
-                                'tunnel',
-                                ]
-        # Hardware card/token type.
-        self.card_type = None
+        self.token_type = "hotp"
+        self.pass_type = "otp"
+        self.otp_type = "counter"
+        self.otp_format = None
+
+        self.need_password = True
+        self.auth_script_enabled = False
         self.allow_offline = False
         self.offline_expiry = 0
         self.offline_unused_expiry = 0
         self.keep_session = False
-        self.signable = True
-        self.signatures = {}
-        self.cross_site_links = True
-        self.need_password = True
-        # Hardware tokens that we can handle (e.g. on otpme-token deploy).
-        self.supported_hardware_tokens = [ 'yubikey-gpg', 'openssh' ]
 
-        self._sub_sync_fields = {
-                    'host'  : {
-                        'trusted'  : [
-                            "SSH_PUBLIC_KEY",
-                            ]
-                        },
-
-                    'node'  : {
-                        'untrusted'  : [
-                            "SSH_PUBLIC_KEY",
-                            ]
-                        },
-                    }
+        # HOTP specific settings.
+        self.counter_check_range = None
+        self.counter_sync_time = 1.0
+        self.sync_offline_token_counter = True
+        # Hardware tokens that we can handle (e.g. on otpme-token deploy).
+        self.supported_hardware_tokens = [ 'yubikey_hotp' ]
+        # This dict is filled with used OTP(s) and its counters and read by
+        # self.add_used_otp() to get the token counter that needs to be saved.
+        self.otp_cache = {}
+        # Token ACLs to add to new token via tokenacls policy.
+        self.token_acls = [
+                            'generate:otp',
+                            'generate:qrcode',
+                        ]
+        self.user_acls = []
+        self.creator_acls = []
 
     def _get_object_config(self):
         """ Merge token config with config from parent class. """
         token_config = {
-            'SSH_PRIVATE_KEY'           : {
-                                            'var_name'      : 'ssh_private_key',
+            'PIN'                       : {
+                                            'var_name'      : 'pin',
                                             'type'          : str,
                                             'required'      : False,
                                             'encryption'    : config.disk_encryption,
                                         },
 
-            'SSH_PUBLIC_KEY'            : {
-                                            'var_name'      : 'ssh_public_key',
-                                            'type'          : str,
+            'PIN_ENABLED'               : {
+                                            'var_name'      : 'pin_enabled',
+                                            'type'          : bool,
                                             'required'      : False,
-                                            'encoding'      : 'BASE64',
                                         },
 
-
-            'OFFLINE_CHALLENGE'         : {
-                                            'var_name'      : 'offline_challenge',
-                                            'type'          : str,
+            'PIN_LEN'                   : {
+                                            'var_name'      : 'pin_len',
+                                            'type'          : int,
                                             'required'      : False,
-                                            'encryption'    : config.disk_encryption,
                                         },
 
-            'KEY_TYPE'                  : {
-                                            'var_name'      : 'key_type',
+            'SERVER_SECRET'             : {
+                                            'var_name'      : 'server_secret',
                                             'type'          : str,
                                             'required'      : False,
+                                            'encryption'    : config.disk_encryption,
                                         },
 
-            'CARD_TYPE'                 : {
-                                            'var_name'      : 'card_type',
+
+            'OTP_FORMAT'                : {
+                                            'var_name'      : 'otp_format',
                                             'type'          : str,
                                             'required'      : False,
                                         },
 
-            'SECOND_FACTOR_TOKEN'       : {
-                                            'var_name'      : 'second_factor_token',
-                                            'type'          : 'uuid',
+            'COUNTER'                   : {
+                                            'var_name'      : 'get_token_counter',
+                                            'type'          : int,
                                             'required'      : False,
                                         },
 
-
-            'SECOND_FACTOR_TOKEN_ENABLED': {
-                                            'var_name'      : 'second_factor_token_enabled',
-                                            'type'          : bool,
+            'COUNTER_SYNC_TIME'         : {
+                                            'var_name'      : 'counter_sync_time',
+                                            'type'          : float,
                                             'required'      : False,
                                         },
 
-            'SIGNATURES'                : {
-                                            'var_name'  : 'signatures',
-                                            'type'      : dict,
-                                            'required'  : False,
+            'COUNTER_CHECK_RANGE'       : {
+                                            'var_name'      : 'counter_check_range',
+                                            'type'          : int,
+                                            'required'      : False,
                                         },
             }
 
         # Use parent class method to merge token configs.
-        return Token._get_object_config(self, token_config=token_config)
+        return super(HotpToken, self)._get_object_config(token_config=token_config)
 
     def set_variables(self):
-        """ Set instance variables. """
+        """ Set instance variables """
         # Run parent class method that may override default values with those
         # read from config.
-        Token.set_variables(self)
+        super(HotpToken, self).set_variables()
+        # In mode2 the PIN is mandatory.
+        if self.mode == "mode2":
+            self.pin_enabled = True
+            self.pin_mandatory = True
+        else:
+            self.pin_mandatory = False
+
+    @property
+    def secret_len(self):
+        """ Get token secret length. """
+        secret_len = self.get_config_parameter("hotp_secret_len")
+        return secret_len
+
+    def update_otp_cache(self, otp, counter):
+        """ Add OTP + counter to OTP cache. """
+        self.otp_cache[otp] = counter
+
+    def get_counter_range(self):
+        """ Get start/stop counter for this token. """
+        start = self.get_token_counter() + 1
+        end = start + self.counter_check_range
+        return start, end
 
-    def get_offline_config(self, second_factor_usage=False):
-        """ Get offline config of token. (e.g. without PIN). """
-        offline_config = self.object_config.copy()
-        need_encryption = False
-
-        #if self.private_key:
-        #    need_encryption = True
-
-        # FIXME: implement self.allow_offline_rsp!!!
-        need_encryption = True
-        #if self.allow_offline_rsp:
-        #    need_encryption = True
-
-        offline_config['NEED_OFFLINE_ENCRYPTION'] = need_encryption
-        return offline_config
-
-    def verify_acl(self, action):
-        """ Verify ACLs required to allow <action>. """
-        # Parent class cannot know the ACL to allow verification of signatures
-        # e.g. "view:script" for script objects and "view_public_key" for SSH
-        # tokens.
-        if action == "verify_signature":
-            if self._verify_acl("verify:signature") \
-            or self._verify_acl("view:signature") \
-            or self._verify_acl("view:ssh_public_key"):
-                return True
-
-        if action == "get_signatures":
-            if self._verify_acl("view:signature") \
-            or self.verify_acl("view:ssh_public_key"):
-                return True
-
-        # Finally try to verify ACL via parent class method.
-        if self._verify_acl(action):
-            return True
+    @check_acls(['generate:otp'])
+    def gen_otp(self, secret=None, otp_count=1, prefix_pin=False,
+        callback=default_callback, _caller="API", **kwargs):
+        """
+        Generate one or more OTPs for this token within the valid counter range.
+        """
+        if not secret:
+            if self.mode == "mode1":
+                secret = self.get_secret(callback=callback)
+            if self.mode == "mode2":
+                if not prefix_pin:
+                    msg = "Cannot generate OTP in mode2."
+                    return callback.error(msg)
+                secret = self.get_secret(pin=prefix_pin, callback=callback)
+
+        if not secret:
+            return callback.error("Unable to get token secret.")
+
+        from otpme.lib.otp.oath import hotp
+        token_counter_start, token_counter_end = self.get_counter_range()
+        if otp_count > 1:
+            otps = []
+            for i in range(0, otp_count):
+                token_counter = token_counter_start + i
+                otp = hotp.generate_hotp(token_counter, secret, self.otp_format)
+                if prefix_pin:
+                    otp = "%s%s" % (prefix_pin, otp)
+                self.update_otp_cache(otp, token_counter)
+                otps.append(otp)
+            if _caller == "CLIENT":
+                return callback.ok(otps)
+            return otps
+        token_counter = token_counter_start + 1
+        otp = hotp.generate_hotp(token_counter, secret, self.otp_format)
+        if prefix_pin:
+            otp = "%s%s" % (prefix_pin, otp)
+        self.update_otp_cache(otp, token_counter)
+        if _caller == "CLIENT":
+            return callback.ok(otp)
+        return [otp]
 
-        return  False
+    def verify_otp(self, otp, secret=None, handle_used_otps=True,
+        mode=None, otp_includes_pin=True, verify_pin=True, sft=None,
+        recursive_use=False, session_uuid=None, **kwargs):
+        """ Verify OTP for this token. """
+        pin = None
+        # Make sure OTP is str().
+        otp = str(otp)
 
-    @check_acls(['view:ssh_public_key'])
-    def get_sign_data(self, callback=default_callback, **kwargs):
-        """ Return public key to be signed by parent class method. """
-        ssh_public_key = self.ssh_public_key
-        return callback.ok(ssh_public_key)
-
-    def get_card_types(self, _caller="API", callback=default_callback, **kwargs):
-        """ Get supported hardware card/token types. """
-        card_types = [ 'gpg' ]
-        if _caller == "CLIENT":
-            card_types = "\n".join(card_types)
-        return callback.ok(card_types)
+        if handle_used_otps:
+            if self.is_used_otp(otp):
+                return False
 
-    @check_acls(['edit:card_type'])
-    @object_lock()
-    @backend.transaction
-    def change_card_type(self, card_type=None, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Get supported hardware card/token types. """
-        if card_type:
-            if not card_type in self.get_card_types():
-                msg = (_("Unsupported card type: %s") % card_type)
-                return callback.error(msg)
-            if card_type == self.card_type:
-                msg = (_("Card type already set to: %s") % card_type)
-                return callback.error(msg)
+        # Mode indicates for which mode we have to verify the OTP (e.g. if
+        # the OTP includes the PIN)
+        if not mode:
+            mode = self.mode
+
+        # If PIN is disabled OTP does not include a PIN we could verify.
+        if mode == "mode1":
+            if not self.pin_enabled:
+                verify_pin = False
+                # We decide on token mode if OTP includes a PIN because we
+                # allow to "emulate" the given token mode (e.g. use in
+                # change_mode())
+                otp_includes_pin = False
+        # In mode2 no PIN verification can be done as the PIN is not
+        # saved on server side.
+        if mode == "mode2":
+            verify_pin = False
+
+        # Get PIN from OTP if needed.
+        if otp_includes_pin:
+            if len(otp) < (int(self.pin_len) + int(self.otp_len)):
+                msg = ("Token PIN enabled but the given OTP is too "
+                        "short to include a PIN!")
+                logger.debug(msg)
+                return None
+            _otp = otp[self.pin_len:]
+            pin = int(otp[:self.pin_len])
+        else:
+            _otp = otp
 
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("change_card_type",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
+        # If we got a secret this request is to verify the secret itself
+        # (e.g. mode change)
+        if not secret:
+            # Get token secret.
+            secret = self.get_secret(pin=pin)
+
+        # Get token counter check range.
+        token_counter_start, token_counter_end = self.get_counter_range()
+
+        # Tokens do not include a PIN in offline config we could verify here.
+        # The PIN is verified in different ways:
+        # - in mode1 by using it to en-/decrypt the token config.
+        # - in mode2 the token secret is derived from server_secret+PIN and
+        #   thus OTP verification fails with the wrong PIN.
+        # If not used as second factor token we also have no PIN length in
+        # our config to make brute force attacks harder and thus we have to
+        # try all possible PIN lengths. The increased load should not be
+        # noticeable and outweigh the added security.
+        if self.offline and self.pin_enabled:
+            verify_pin = False
+            if not sft and not recursive_use:
+                org_pin_len = self.pin_len
+                self.pin_len = 0
+                while True:
+                    if self.pin_len >= (len(otp) - self.otp_len):
+                        self.pin_len = org_pin_len
+                        return None
+                    self.pin_len += 1
+                    status = self.verify_otp(otp,
+                                            secret=secret,
+                                            handle_used_otps=handle_used_otps,
+                                            mode=mode,
+                                            otp_includes_pin=otp_includes_pin,
+                                            verify_pin=False,
+                                            sft=None,
+                                            recursive_use=True,
+                                            **kwargs)
+                    if status:
+                        self.pin_len = org_pin_len
+                        return status
+
+        # Log token counter range.
+        msg = ("Verifiying OTP within counter range: start='%s' end='%s'."
+                % (token_counter_start, token_counter_end))
+        logger.debug(msg)
+
+        # Verify OTP.
+        hotp_status, \
+        hotp_count = hotp.verify_hotp(counter_start=token_counter_start,
+                                    counter_end=token_counter_end,
+                                    secret=secret, otp=_otp,
+                                    format=self.otp_format)
+        if hotp_status:
+            self.update_otp_cache(otp, hotp_count)
+            if otp_includes_pin:
+                self.update_otp_cache(_otp, hotp_count)
+            # Make sure the OTP was not already used (counter must be higher
+            # than the one from the last used OTP).
+            if hotp_count > self.get_token_counter():
+                # Verify PIN.
+                if verify_pin:
+                    # FIXME: A wrong PIN is not definitively a failed login
+                    #        with this token because it may be used as a
+                    #        second factor token (e.g. a password token)
+                    #        where a static password is prefixed and the PIN
+                    #        verification is disabled. It would be nice to
+                    #        prevent brute forcing the PIN with a stolen OTP
+                    #        here but for this we need to change the concept
+                    #        of add_used_otp() here and in User().authenticate()
+                    if pin != self.pin:
+                        logger.debug("Got wrong token PIN: %s" % self.rel_path)
+                        return None
+
+                if handle_used_otps:
+                    # Only log message for the first OTP we add.
+                    self.add_used_otp(otp=otp,
+                                    session_uuid=session_uuid,
+                                    quiet=False)
+                    if otp_includes_pin:
+                        self.add_used_otp(otp=_otp, session_uuid=session_uuid)
+                return otp
+
+        # Default should be None (which means no valid OTP found but not
+        # definitively failed because we havent found an already used OTP)
+        return None
+
+        # This point should never be reached.
+        msg = (_("WARNING: You may have hit a BUG of Token().verify_otp()."))
+        raise Exception(msg)
+
+    def verify_mschap_otp(self, challenge, response,
+        session_uuid=None, handle_used_otps=True, **kwargs):
+        """ Verify MSCHAP challenge/response against OTPs """
+        from otpme.lib.otp.oath import hotp
+        from otpme.lib import mschap_util
 
-        self.card_type = card_type
-        return self._cache(callback=callback)
+        nt_key = None
+        otp = None
+        _otp = None
+        # Set default return values.
+        return_value = None, None, None
+        failed_return_value = False, None, None
+
+        # Cannot verify token in mode2.
+        if self.mode == "mode2":
+            return return_value
+
+        # Get token secret.
+        secret = self.get_secret()
+
+        # Get token counter check range.
+        token_counter_start, token_counter_end = self.get_counter_range()
+
+        # Get list with valid OTPs of this token for the given counter range.
+        otps = self.gen_otp(otp_count=self.counter_check_range,
+                            prefix_pin=self.pin, verify_acls=False)
+
+        msg = ("Verifiying OTP within counter range: start='%s' end='%s'."
+                % (token_counter_start, token_counter_end))
+        logger.debug(msg)
+
+        # Walk through all valid OTPs.
+        for _otp in otps:
+            # Get NT key from verify().
+            status, \
+            nt_key = mschap_util.verify(stuff.gen_nt_hash(_otp),
+                                        challenge, response)
+            if status:
+                if self.pin_enabled:
+                    otp = _otp[self.pin_len:]
+                    check_otp = otp
+                else:
+                    check_otp = _otp
+
+                # Verify OTP.
+                hotp_status, \
+                hotp_count = hotp.verify_hotp(counter_start=token_counter_start,
+                                            counter_end=token_counter_end,
+                                            secret=secret, otp=check_otp,
+                                            format=self.otp_format)
+
+                if hotp_status:
+                    # Make sure the OTP was not already used (counter must be higher
+                    # than the one from the last used OTP).
+                    if hotp_count > self.get_token_counter():
+                        if handle_used_otps:
+                            if self.is_used_otp(_otp):
+                                return failed_return_value
+                            # Add OTP to used OTPs.
+                            self.update_otp_cache(_otp, hotp_count)
+                            self.add_used_otp(otp=_otp,
+                                session_uuid=session_uuid)
+                            # Add OTP without PIN to used OTPs.
+                            if otp:
+                                self.update_otp_cache(otp, hotp_count)
+                                self.add_used_otp(otp=otp,
+                                                session_uuid=session_uuid,
+                                                quiet=False)
+                        return status, nt_key, _otp
+
+        # Default should be None (which means no valid OTP found but not
+        # definitively failed because we havent found an already used OTP)
+        return return_value
+
+        # This point should never be reached.
+        msg = ("WARNING: You may have hit a BUG of Token().verify_mschap_otp().")
+        raise Exception(msg)
 
-    @check_acls(['edit:key_type'])
-    @object_lock()
-    @backend.transaction
-    def change_key_type(self, key_type="rsa", run_policies=True,
+    @check_acls(['generate:qrcode'])
+    def gen_qrcode(self, pin=None, qrcode_file=None, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Get supported hardware card/token types. """
-        if key_type != "":
-            if not key_type in self.valid_key_types:
-                msg = (_("Unsupported key type: %s") % key_type)
-                return callback.error(msg)
-            if key_type == self.key_type:
-                msg = (_("Key type already set to: %s") % key_type)
-                return callback.error(msg)
-
+        """ Generate QRCode for token deployment. """
         if run_policies:
             try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("change_key_type",
+                self.run_policies("gen_qrcode",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        self.key_type = key_type
-        return self._cache(callback=callback)
+        if pin is None:
+            if self.mode == "mode2":
+                pin = callback.askpass("Please enter PIN: ")
+                pin = int(pin)
+                if pin is None:
+                    msg = "Cannot gen qrcode without PIN."
+                    return callback.error(msg)
+
+        # Get secret to gen QRCode.
+        secret = self.get_secret(pin=pin)
+
+        token_counter_start, token_counter_end = self.get_counter_range()
+
+        # Gen OATH URI.
+        user_string = "%s@%s" % (self.rel_path, self.realm)
+        #oath_uri = HOTP(secret, "hex")
+        #oath_uri = oath_uri.provisioning_uri(name=user_string,
+        #                                    issuer_name=config.my_name,
+        #                                    initial_count=token_counter_start)
+        # Use oath-toolkit.
+        oath_uri = uri.generate(key_type=self.token_type,
+                                key=decode(secret, "hex"),
+                                user=user_string,
+                                issuer=config.my_name,
+                                counter=token_counter_start)
+        # Generate QRcode.
+        _qrcode = qrcode.gen_qrcode(oath_uri, "terminal")
+        # xxxxxxxxxxxxx
+        # FIXME: How to create png/svg image without writing to file?
+        return callback.ok(_qrcode)
 
-    @check_acls(['edit:ssh_public_key'])
+    @check_acls(['resync'])
     @object_lock()
     @backend.transaction
-    def change_ssh_public_key(self, ssh_public_key=None, run_policies=True,
+    def resync(self, otp=None, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Change token SSH public key. """
+        """ Resync our counter state with token by given OTP. """
+        from otpme.lib.otp.oath import hotp
+        if not otp:
+            otp = callback.askpass("Please enter OTP: ")
+
+        if not otp:
+            return callback.error("Unable to get OTP.")
+
+        # Make sure OTP is str().
+        otp = str(otp)
+
+        if len(otp) < self.otp_len:
+            return callback.error("OTP too short.")
+        if len(otp) > self.otp_len:
+            return callback.error("OTP too long.")
+
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
-                self.run_policies("change_ssh_public_key",
+                self.run_policies("resync",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        # Check if we got SSH public key as argument.
-        if ssh_public_key == None:
-            ssh_public_key = callback.ask("Please enter/paste SSH public key: ")
-        if ssh_public_key:
-            self.ssh_public_key = ssh_public_key
-            self.offline_challenge = stuff.gen_md5(ssh_public_key)
-        else:
-            self.ssh_public_key = None
-            self.offline_challenge = None
-        return self._cache(callback=callback)
+        pin = None
+        if self.mode == "mode2":
+            pin = callback.askpass("Please enter PIN: ")
+            pin = int(pin)
+            if pin is None:
+                msg = "Cannot resync without PIN."
+                return callback.error(msg)
 
-    def get_private_key(self, password, instance=False):
-        """ Get decrytped private key. """
-        if not self.ssh_private_key:
-            raise Exception("No private key set.")
-        # Try to decrypt RSA key.
-        try:
-            key = RSAKey(key=self.ssh_private_key, password=password)
-        except Exception as e:
-            msg = (_("Error decrypting private key: %s") % e)
-            raise Exception(msg)
-        if instance:
-            return key
-        private_key = key.private_key_base64
-        return private_key
+        # Get token secret.
+        token_secret = self.get_secret(pin=pin, callback=callback)
 
-    def resync(self, callback=default_callback, **kwargs):
-        """ Wrapper method to call resync() of 2ftoken. """
-        try:
-            sftoken = self.get_sftoken()
-        except Exception as e:
-            msg = (_("Error loading second factor token: %s") % e)
-            return callback.error(msg)
-        return sftoken.resync(callback=callback, **kwargs)
+        # Get current token counter.
+        current_counter = self.get_token_counter()
 
-    def gen_challenge(self, **kwargs):
-        """ Generate challenge to be sigend by users private SSH key. """
-        if not self.ssh_public_key:
-            raise Exception("No SSH public key set.")
-        if self.second_factor_token_enabled:
-            sftoken = self.get_sftoken()
-            otp_len = sftoken.otp_len
-            if sftoken.pin_enabled:
-                otp_len = otp_len + sftoken.pin_len
-            return ssh.gen_challenge(self.ssh_public_key, otp_len=otp_len)
-        else:
-            return ssh.gen_challenge(self.ssh_public_key, otp_len=0)
+        # Get resync check range.
+        resync_check_range = self.get_config_parameter("hotp_resync_check_range")
 
-    def test(self, password=None, callback=default_callback, **kwargs):
-        """ Test if SSH authentication with this token can be verified. """
-        ok_message = "Token verified successful."
-        error_message = "Token verification failed."
+        # We will check resync_check_range below and above the current counter.
+        token_counter_start = 0
+        if current_counter >= resync_check_range:
+            token_counter_start = current_counter - resync_check_range
+        token_counter_end = current_counter + resync_check_range
+
+        hotp_status, \
+        hotp_count = hotp.verify_hotp(counter_start=token_counter_start,
+                                        counter_end=token_counter_end,
+                                        secret=token_secret,
+                                        otp=otp,
+                                        format=self.otp_format)
+        if not hotp_status:
+            return callback.error("Unable to synchronize token.")
+
+        # Add OTP with counter to our cache.
+        self.update_otp_cache(otp, hotp_count)
+        # Set new sync timestamp.
+        self.counter_sync_time = time.time()
 
         try:
-            challenge = self.gen_challenge()
+            self.add_used_otp(otp, resync=True)
         except Exception as e:
-            callback.error(_("Unable to generate challenge: %s") % e)
-
-        response = callback.sshauth(challenge=challenge)
-
-        otp = None
-        if self.second_factor_token_enabled:
-            pass_prompt = "OTP: "
-            if not otp:
-                otp = callback.askpass(pass_prompt)
-            if not otp:
-                return callback.error("Unable to get OTP.")
-
-        status = self.verify(challenge=challenge, response=response, otp=otp)
-
-        if status:
-            return callback.ok(ok_message)
-
-        return callback.error(error_message)
-
-    def verify(self, challenge=None, response=None,
-        otp=None, session_uuid=None, **kwargs):
-        """ Verify challenge/response. """
-        import time
-        if not self.ssh_public_key:
-            logger.warning("Token '%s' is missing SSH public key." % self.name)
-            return None
-
-        if self.second_factor_token_enabled:
-            try:
-                sftoken = self.get_sftoken()
-            except Exception as e:
-                logger.critical("Error loading second factor token: %s" % e)
-                return None
-
-            # Check if token PIN is mandatory. by default we dont want a user to
-            # type in the token PIN when used as second factor token.
-            if sftoken.pin_mandatory:
-                verify_pin = True
-                otp_includes_pin = True
-            else:
-                verify_pin = False
-                otp_includes_pin = False
-
-            cutoff_len = sftoken.otp_len
-            if otp_includes_pin:
-                cutoff_len += sftoken.pin_len
-
-            if len(otp) <= cutoff_len:
-                logger.debug("Second factor OTP token enabled but password is "
-                            "too short to include a OTP.")
-                return None
-            password = otp[:-cutoff_len]
-            otp = otp[-cutoff_len:]
-        else:
-            password = otp
+            msg = "Error adding OTP to list of used OTPs: %s" % e
+            return callback.error(msg)
 
-        # In offline mode the token config is encrypted via challenge/response
-        # procedure using the SSH private key. The offline challenge is the MD5
-        # sum of the SSH public key. If decryption was successful the token is
-        # verified successful. We do this to make offline logins faster because
-        # we need only one singing process via ssh-agent.
-        if self.offline and not password:
-            public_key_md5 = stuff.gen_md5(self.ssh_public_key)
-            if self.offline_challenge != public_key_md5:
-                logger.warning("Failed to verify offline challenge.")
-                return False
+        if self.allow_offline:
+            msg = (_("Offline usage enabled for token. You "
+                    "should re-login after token resync!"))
+            callback.send(msg)
 
-        elif password:
-            if not self.ssh_private_key:
-                logger.debug("Skipping token without SSH private key for "
-                            "password authentication: %s" % self.rel_path)
-                return None
-            # Try to decrypt private key.
-            try:
-                self._ssh_private_key = self.get_private_key(password=password)
-                # When authenticating with the private key encryption passphrase
-                # set our pass type to static.
-                self.pass_type = "static"
-            except:
-                # If we got the wrong password this is not a failure because
-                # it may match an other token. So we continue to next token.
-                return None
+        msg = (_("Token synchronized successful. Current counter: %s")
+                % hotp_count)
+        callback.send(msg)
 
-        elif challenge and response:
-            if not ssh.verify_sign(public_key=decode(self.ssh_public_key, "base64"),
-                                    data=decode(response, "base64"),
-                                    plaintext=challenge):
-                logger.warning("Verifying SSH response failed.")
-                return False
+        return self._cache(callback=callback)
 
-            challenge_time = int(challenge.split(":")[0])
-            epoch_time = int(time.time())
-            challenge_age = epoch_time - challenge_time
-            if challenge_age > 15:
-                logger.warning("SSH challenge too old.")
-                return False
-        else:
-            return None
+    def add_used_otp(self, otp, resync=False, session_uuid=None, quiet=True):
+        """ Add used OTP + counter for this user/token. """
+        try:
+            token_counter = self.otp_cache[otp]
+        except:
+            msg = ("WARNING: Unable to find counter for the given OTP.")
+            raise OTPmeException(msg)
 
-        # If no second factor token is configured we are done.
-        if not self.second_factor_token_enabled:
+        # Add used token counter using parent class method.
+        self._add_token_counter(token_counter=token_counter,
+                                session_uuid=session_uuid)
+
+        # Update counter in token config on resync.
+        if resync:
+            self.object_config['COUNTER'] = token_counter
+
+        # FIXME: how long to cache already used HOTPs?
+        expiry = time.time() + 86400
+
+        # In offline mode we do not add used OTPs to make brute force attacks
+        # harder (no OTP hash saved to disk)
+        if self.offline:
             return True
 
-        # Verify second factor token.
-        logger.debug("Verifying second factor token: %s" % sftoken.rel_path)
-        if sftoken.verify_otp(otp,
+        # Add used OTP using parent class method
+        try:
+            self._add_used_otp(otp=otp,
+                            expiry=expiry,
                             session_uuid=session_uuid,
-                            otp_includes_pin=otp_includes_pin,
-                            verify_pin=verify_pin, sft=True):
-            return True
-        return False
-
-    @check_acls(['edit:2ftoken'])
-    @object_lock()
-    @backend.transaction
-    def change_2f_token(self, second_factor_token, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Change token second factor token. """
-        if second_factor_token == "":
-            self.second_factor_token = second_factor_token
-
-        # Get user instance of token owner.
-        user = backend.get_object(object_type="user", uuid=self.owner_uuid)
-        # Get token instance of 2f_token by name.
-        token = user.token(second_factor_token)
+                            sync_time=self.counter_sync_time,
+                            quiet=quiet)
+        except Exception as e:
+            msg = "Failed to add used OTP: %s" % e
+            raise OTPmeException(msg)
 
-        if not token:
-            msg = (_("Token '%s' does not exist.") % second_factor_token)
-            return callback.error(msg)
-        if token.pass_type != "otp":
-            msg = (_("Token '%s' is not an OTP token.") % second_factor_token)
+    def _check_range_format(self, check_range, callback=default_callback):
+        """ Check if the given counter range is valid. """
+        if isinstance(check_range, int):
+            if check_range > 0:
+                return callback.ok()
+            msg = (_("Counter check range must be greater than 0."))
             return callback.error(msg)
+        msg = "Counter check range must be an integer."
+        return callback.error(msg)
 
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("change_ssh_public_key",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
-
-        # Set 2f token.
-        self.second_factor_token = token.uuid
-        return self._cache(callback=callback)
-
-    @check_acls(['enable:2ftoken'])
+    @check_acls(['edit:counter_check_range'])
     @object_lock()
     @backend.transaction
-    def enable_2f_token(self, force=False, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Enable the second factor token. """
-        if self.second_factor_token_enabled:
-            return callback.error("Second factor token already enabled.")
-
-        if self.second_factor_token == "":
-            return callback.error("No second factor token configured.")
-
-        # Check if second factor token is available.
-        try:
-            self.get_sftoken(callback=callback)
-        except Exception as e:
-            msg = (_("Unable to enable second factor token: %s") % e)
-            return callback.error(msg)
-
+    def change_counter_check_range(self, run_policies=True,
+        counter_check_range=None, _caller="API",
+        callback=default_callback, **kwargs):
+        """ Change token counter check range. """
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
-                self.run_policies("enable_2f_token",
+                self.run_policies("change_counter_check_range",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        if not force:
-            if self.confirmation_policy == "paranoid":
-                answer = callback.ask("Enable second factor token?: ")
-                if answer.lower() != "y":
-                    return callback.abort()
-
-        self.second_factor_token_enabled = True
-        return self._cache(callback=callback)
-
-    @check_acls(['disable:2ftoken'])
-    @object_lock()
-    @backend.transaction
-    def disable_2f_token(self, force=False, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Disable the second factor token. """
-        if not self.second_factor_token_enabled:
-            return callback.error("Second factor token already disabled.")
-
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("disable_2f_token",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
+        if counter_check_range == None:
+            while True:
+                answer = callback.ask("Counter check range: ")
+                try:
+                    counter_check_range = int(answer)
+                except:
+                    pass
+                check_status, \
+                check_message = self._check_range_format(counter_check_range)
+                if check_status:
+                    break
+                else:
+                    callback.send(check_message)
+        else:
+            check_status, \
+            check_message = self._check_range_format(counter_check_range)
+            if not check_status:
+                return callback.error(check_message)
 
-        if not force:
-            if self.confirmation_policy == "paranoid":
-                answer = callback.ask("Disable second factor token?: ")
-                if answer.lower() != "y":
-                    return callback.abort()
+        self.counter_check_range = counter_check_range
 
-        self.second_factor_token_enabled = False
         return self._cache(callback=callback)
 
     @object_lock()
     @backend.transaction
-    def deploy(self, public_key=None, private_key=None, password=None,
-        pass_hash_type="PBKDF2", _caller="API", verbose_level=0,
-        callback=default_callback):
-        """ Deploy SSH token. """
-        if not public_key and not private_key:
-            return callback.error("Need at least public or private key.")
-        if private_key:
-            if not password:
-                return callback.error("Need password to add private key.")
-
-            msg = (_("Setting SSH private key to token: %s") % self.rel_path)
-            callback.send(msg)
-
-            # Encrypt private key with password.
-            rsa_key = RSAKey(key=private_key)
-            self.ssh_private_key = rsa_key.encrypt_key(password=password,
-                                                    hash_type=pass_hash_type)
-            # Get public key from private key if not given.
-            if not public_key:
-                public_key = rsa_key.ssh_public_key.split(" ")[1]
-            # We cannot support cross site token links if the token includes
-            # a SSH private key.
-            self.cross_site_links = False
+    def deploy(self, server_secret, pin, _caller="API",
+        verbose_level=0, callback=default_callback):
+        """ Deploy HOTP token """
+        if not self.check_pin(pin=pin, callback=callback):
+            return callback.error("Invalid PIN.")
 
-        msg = (_("Setting SSH public key to token: %s") % self.rel_path)
+        msg = (_("Setting received server secret to token: %s") % self.rel_path)
         callback.send(msg)
 
-        self.ssh_public_key = public_key
-
-        return self._cache(callback=callback)
-
-    @check_acls(['edit:password'])
-    @object_lock()
-    @backend.transaction
-    def change_key_password(self, force=False, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Change private key encryption password. """
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("change_password",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
-
-        is_admin = False
-        if config.auth_token:
-            is_admin = config.auth_token.is_admin()
-        elif config.use_api:
-            is_admin = True
-
-        current_pass = callback.askpass("Current password: ")
-        try:
-            private_key = self.get_private_key(password=current_pass,
-                                                    instance=True)
-        except:
-            return callback.error("Wrong password.")
-
-        password_checked = False
-        while True:
-            new_password1 = callback.askpass("New password: ")
-            if not force or not is_admin:
-                if not self.check_password(new_password1,
-                                        callback=callback):
-                    return callback.error()
-                password_checked = True
-
-            new_password2 = callback.askpass("Re-type password: ")
-            if new_password1 == new_password2:
-                password = new_password1
-                break
-            else:
-                return callback.error("Sorry, passwords do not match.")
-
-        # Make sure password is a string.
-        password = str(password)
-
-        if password == "":
-            return callback.error("Cannot set empty password.")
-
-        if not force or not is_admin:
-            if not password_checked:
-                 if not self.check_password(password, callback=callback):
-                    return callback.error()
-
-        if not force or not is_admin:
-            if len(password) < self.password_min_len:
-                msg = (_("Password too short (%s).") % self.password_min_len)
-                return callback.error(msg)
-            if len(password) > self.password_max_len:
-                msg = (_("Password too long (%s).") % self.password_max_len)
-                return callback.error(msg)
+        self.mode = "mode2"
+        self.secret = None
+        self.server_secret = str(server_secret)
+
+        if verbose_level > 0:
+            token_secret = self.get_secret(pin=pin)
+            msg = (_("Token secret: %s") % token_secret)
+            callback.send(msg)
 
-        # Encrypt private key with new password.
-        #rsa_key = RSAKey(key=private_key)
-        #self.ssh_private_key = rsa_key.encrypt_key(password=password)
-        self.ssh_private_key = private_key.encrypt_key(password=password)
+        msg = ("You have to resync the token after re-deploying.")
+        callback.send(msg)
 
         return self._cache(callback=callback)
 
     @object_lock()
     @backend.transaction
-    def _add(self, public_key=None, callback=default_callback, **kwargs):
+    def _add(self, *args, **kwargs):
         """ Add a token. """
-        return_message = None
-        if public_key:
-            self.ssh_public_key = public_key
-        else:
-            return_message = (_("NOTE: You have to add an SSH public key to "
-                                "this token to make it usable."))
-
-        sf_note = (_("NOTE: You may want to add a second factor token "
-                    "(e.g. OTP token) to improve security."))
-
-        if return_message:
-            return_message = "%s\n%s" % (return_message, sf_note)
-        else:
-            return_message = sf_note
-
-        return callback.ok(return_message)
+        # Get default TOTP settings.
+        self.otp_format = self.get_config_parameter("hotp_format")
+        self.counter_check_range = self.get_config_parameter("hotp_check_range")
+        return super(HotpToken, self)._add(*args, **kwargs)
 
     def show_config(self, callback=default_callback, **kwargs):
-        """ Show token config. """
+        """ Show token info. """
         if not self.verify_acl("view_public:object"):
             msg = ("Permission denied.")
             return callback.error(msg, exception=PermissionDenied)
-
-        second_factor_token_name = ""
-        if self.verify_acl("view:2ftoken"):
-            # Get 2f token instance.
-            if self.second_factor_token:
-                try:
-                    sftoken = self.get_sftoken()
-                    second_factor_token_name = sftoken.name
-                except Exception as e:
-                    callback.send(_("Error loading second factor token: %s")
-                                    % e)
         lines = []
 
-        if self.verify_acl("view:ssh_public_key"):
-            lines.append('SSH_PUBLIC_KEY="%s"' % self.ssh_public_key)
-        else:
-            lines.append('SSH_PUBLIC_KEY=""')
-
-        if self.verify_acl("view_all:ssh_private_key"):
-            lines.append('SSH_PRIVATE_KEY="%s"' % self.ssh_private_key)
-        else:
-            lines.append('SSH_PRIVATE_KEY=""')
-
-        if self.verify_acl("view:key_type"):
-            lines.append('KEY_TYPE="%s"' % self.key_type)
-        else:
-            lines.append('KEY_TYPE=""')
-
-        lines.append('SECOND_FACTOR_TOKEN="%s"' % second_factor_token_name)
-
-        if self.verify_acl("view:2ftoken_status"):
-            lines.append('SECOND_FACTOR_TOKEN_ENABLED="%s"'
-                        % self.second_factor_token_enabled)
-        else:
-            lines.append('SECOND_FACTOR_TOKEN_ENABLED=""')
-
-        if self.verify_acl("view:card_type"):
-            lines.append('CARD_TYPE="%s"' % self.card_type)
-        else:
-            lines.append('CARD_TYPE=""')
-
-        lines.append('OFFLINE_CHALLENGE="%s"' % self.offline_challenge)
-
-        return Token.show_config(self,
-                                config_lines=lines,
-                                callback=callback,
-                                **kwargs)
+        counter_check_range = ""
+        if self.verify_acl("view:counter_check_range") \
+        or self.verify_acl("edit:counter_check_range"):
+            counter_check_range = str(self.counter_check_range)
+        lines.append('COUNTER_CHECK_RANGE="%s"' % counter_check_range)
+
+        counter_sync_time = ""
+        if self.verify_acl("view:counter_sync_time") \
+        or self.verify_acl("resync"):
+            counter_sync_time = str(self.counter_sync_time)
+        lines.append('COUNTER_SYNC_TIME="%s"' % counter_sync_time)
+
+        server_secret = ""
+        if self.verify_acl("view:server_secret"):
+            server_secret = str(self.server_secret)
+        lines.append('SERVER_SECRET="%s"' % server_secret)
+
+        return super(HotpToken, self).show_config(config_lines=lines,
+                                                callback=callback,
+                                                **kwargs)
 
     def show(self, **kwargs):
-        """ Show token details. """
+        """ Show token details """
         #if not self.verify_acl("view_public:object"):
         #    msg = ("Permission denied.")
         #    return callback.error(msg, exception=PermissionDenied)
         return self.show_config(**kwargs)
```

### Comparing `otpme-0.3.0a45/otpme/lib/token/totp/totp.py` & `otpme-0.3.0a46/otpme/lib/token/totp/totp.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 from otpme.lib import stuff
 from otpme.lib import config
 from otpme.lib import qrcode
 from otpme.lib import backend
 from otpme.lib import otpme_acl
 from otpme.lib.otp.oath import totp
-from otpme.lib.classes.token import Token
 from otpme.lib.locking import object_lock
 from otpme.lib.otpme_acl import check_acls
 from otpme.lib.encoding.base import decode
+from otpme.lib.token.oath.oath import OathToken
 from otpme.lib.third_party.oath_toolkit import uri
+from otpme.lib.token.oath.oath import OATH_OTP_FORMATS
 from otpme.lib.protocols.utils import register_commands
 
 from otpme.lib.classes.token \
             import get_acls \
             as _get_acls
 from otpme.lib.classes.token \
             import get_value_acls \
@@ -286,24 +287,14 @@
 def get_recursive_default_acls():
     """ Get all supported object recursive default ACLs """
     token_recursive_default_acls = _get_recursive_default_acls()
     _acls = otpme_acl.merge_acls(recursive_default_acls,
                                 token_recursive_default_acls)
     return _acls
 
-# OATH OTP formats and the resulting OTP lens.
-OATH_OTP_FORMATS = {
-        'dec4'          : 4,
-        'dec6'          : 6,
-        'dec7'          : 7,
-        'dec8'          : 8,
-        'hex'           : 4,
-        'hex-notrunc'   : 4,
-        }
-
 REGISTER_BEFORE = []
 REGISTER_AFTER = []
 
 def register():
     """ Register object. """
     register_hooks()
     register_token_type()
@@ -360,15 +351,15 @@
                                     object_types=object_types)
     # The TOTP secret length.
     config.register_config_parameter(name="totp_secret_len",
                                     ctype=int,
                                     default_value=40,
                                     object_types=object_types)
 
-class TotpToken(Token):
+class TotpToken(OathToken):
     """ Class for OATH TOTP tokens. """
     def __init__(self, object_id=None, user=None, name=None,
         realm=None, site=None, path=None, **kwargs):
         # Call parent class init.
         super(TotpToken, self).__init__(object_id=object_id,
                                             realm=realm,
                                             site=site,
@@ -382,35 +373,25 @@
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
         # Set default values.
         self.token_type = "totp"
         self.pass_type = "otp"
         self.otp_type = "time"
 
-        self.valid_otp_formats = OATH_OTP_FORMATS
         self.otp_format = None
-        self.pin = None
-        self.pin_len = None
-        self.pin_enabled = True
         self.need_password = True
         self.auth_script_enabled = False
         self.allow_offline = False
         self.offline_expiry = 0
         self.offline_unused_expiry = 0
         self.keep_session = False
-        self.valid_modes = [ 'mode1', 'mode2' ]
-        # Default token mode should be mode2 which is more secure for offline.
-        # usage.
-        self.mode = "mode2"
-        self.pin_mandatory = True
+
         # TOTP specific settings
-        # xxxxxxxxxxxxxxxx
         # FIXME: make this per token config setting!
         self.drift = 0
-        self.server_secret = None
         self.period = None
         self.forward_drift = None
         self.backward_drift = None
         # Token ACLs to add to new token via tokenacls policy.
         self.token_acls = [
                             'generate:otp',
                             'generate:qrcode',
@@ -469,228 +450,34 @@
                                             'var_name'      : 'backward_drift',
                                             'type'          : int,
                                             'required'      : False,
                                         },
             }
 
         # Use parent class method to merge token configs.
-        return Token._get_object_config(self, token_config=token_config)
+        return super(TotpToken, self)._get_object_config(token_config=token_config)
 
     def set_variables(self):
         """ Set instance variables """
         # Run parent class method that may override default values with those
         # read from config.
-        Token.set_variables(self)
+        super(TotpToken, self).set_variables()
         # In mode2 the PIN is mandatory.
         if self.mode == "mode2":
             self.pin_enabled = True
             self.pin_mandatory = True
         else:
             self.pin_mandatory = False
 
     @property
-    def otp_len(self):
-        """ Set OTP len depending on the configured OTP format. """
-        try:
-            otp_len = OATH_OTP_FORMATS[self.otp_format]
-        except:
-            otp_len = 6
-        return otp_len
-
-    @property
     def secret_len(self):
         """ Get token secret length. """
         secret_len = self.get_config_parameter("totp_secret_len")
         return secret_len
 
-    def get_secret(self, pin=None, mode=None,
-        callback=default_callback,
-        _caller="API", ** kwargs):
-        """ Get token secret """
-        if not mode:
-            mode = self.mode
-        if mode == "mode1":
-            secret = str(self.secret)
-        else:
-            import hashlib
-            if not pin:
-                pin = self.pin
-            server_secret = self.server_secret
-            if isinstance(pin, str):
-                pin = pin.encode("utf-8")
-            if isinstance(server_secret, str):
-                server_secret = server_secret.encode("utf-8")
-            hash_string = b"%s%s" % (pin, server_secret)
-            sha512 = hashlib.sha512()
-            sha512.update(hash_string)
-            secret = sha512.hexdigest()
-            secret = secret[0:self.secret_len]
-        if _caller == "API":
-            return secret
-        return callback.ok(secret)
-
-    def get_offline_config(self, second_factor_usage=False):
-        """ Get offline config of token. (e.g. without PIN) """
-        # Make sure our object config is up-to-date.
-        self.update_object_config()
-        # Get a copy of our object config.
-        offline_config = self.object_config.copy()
-        # In offline mode we never need the PIN.
-        offline_config['PIN'] = ''
-
-        need_encryption = True
-        if self.mode == "mode1":
-            # In mode1 we do not need the server secret in offline config.
-            offline_config['SERVER_SECRET'] = ''
-            if not self.pin_enabled:
-                need_encryption = False
-
-        if self.mode == "mode2":
-            # In mode2 there should be no TOTP secret so make sure we empty it.
-            offline_config['SECRET'] = ''
-            # In mode2 the token config includes only the server secret which is
-            # used in conjunction with the PIN to generate the TOTP secret. In
-            # offline mode the token config will include neither, not the PIN
-            # and not the TOTP secret. Thus its relatively save to store it
-            # unencrypted. Using the PIN to encrypt the token secret (like its
-            # done in mode1) is much more susceptible to brute force attacks.
-            need_encryption = False
-
-        # FIXME: how to decided if encryption is needed in second factor usage??
-        # When used as second factor token (e.g. with ssh or password token) it
-        # is probably saver to encrypt our config. if the first factor token is
-        # a weak password not true but we currently have not way the get this
-        # info at this stage.
-        if second_factor_usage:
-            need_encryption = True
-        else:
-            # Wnen not used as second factor token remove PIN len from config to
-            # make brute force attacks harder.
-            offline_config['PIN_LEN'] = ''
-
-        offline_config['NEED_OFFLINE_ENCRYPTION'] = need_encryption
-        return offline_config
-
-    @check_acls(['edit:mode'])
-    @object_lock()
-    @backend.transaction
-    def change_mode(self, new_mode, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Change token operation mode. """
-        # Make sure new mode is of type string.
-        new_mode = str(new_mode)
-
-        if not new_mode in self.valid_modes:
-            return callback.error(_("Unknown mode: %s") % new_mode)
-
-        if new_mode == self.mode:
-            return callback.error(_("Token already in mode: %s") % new_mode)
-
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("change_mode",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
-
-        if new_mode == "mode1":
-            self.secret = self.get_secret()
-            self.pin_mandatory = False
-            return_message = (_("Token switched to mode1."))
-
-        if new_mode == "mode2":
-            # If we have a server secret we can try to switch back to mode2
-            # without re-deploying token.
-            if self.server_secret:
-                otp = None
-                if not otp:
-                    otp = callback.askpass(_("Please enter PIN+OTP: "))
-                if not otp:
-                    return callback.error("Unable to get PIN+OTP.")
-
-                # Make sure OTP is str().
-                otp = str(otp)
-
-                # Split OTP in PIN and OTP.
-                pin = otp[:self.pin_len]
-                otp = otp[self.pin_len:]
-
-                # Generate secret from server secret and PIN.
-                secret = self.get_secret(pin=pin,
-                                        mode="mode2")
-                # Verify OTP.
-                if not self.verify_otp(otp=pin+otp, secret=secret, mode="mode2"):
-                    return callback.error("Wrong PIN or token out of sync.")
-
-                # Make sure OTP cannot be re-used.
-                try:
-                    self.add_used_otp(otp=pin+otp)
-                except Exception as e:
-                    msg = "Error adding OTP to list of used OTPs: %s" % e
-                    return callback.error(msg)
-
-                self.secret = None
-                return_message = (_("Token switched to mode2."))
-            else:
-                msg = (_("WARNING: Changing token mode to 'mode2' requires "
-                        "re-deployment of the token!"))
-                callback.send(msg)
-
-                if self.pin:
-                    pin_question = "New PIN (RETURN to keep current PIN): "
-                else:
-                    pin_question = "New PIN: "
-                while True:
-                    new_pin1 = str(callback.askpass(pin_question, null_ok=True))
-                    if new_pin1 == "":
-                        if self.pin:
-                            break
-                        else:
-                            continue
-                    if not self.check_pin(pin=new_pin1, callback=callback):
-                        continue
-                    new_pin2 = callback.askpass("Repeat PIN: ")
-                    if new_pin1 == new_pin2:
-                        self.pin = str(new_pin1)
-                        break
-                self.server_secret = stuff.gen_secret(self.secret_len)
-                token_secret = self.get_secret(pin=self.pin,
-                                                mode="mode2")
-                return_message = (_("New token secret: %s") % token_secret)
-                self.pin_enabled = True
-                self.pin_mandatory = True
-
-        # Set new mode.
-        self.mode = new_mode
-
-        callback.send(return_message)
-
-        return self._cache(callback=callback)
-
-    def _enable_pin(self, pre=False, callback=default_callback, **kwargs):
-        """ Enable token PIN """
-        return True
-
-    def _disable_pin(self, pre=False, callback=default_callback, **kwargs):
-        """ Disable token PIN """
-        if not pre:
-            return True
-
-        if self.mode == "mode2":
-            if self.allow_offline:
-                callback.send(_("WARNING: Offline usage is enabled for this "
-                                "token. Anybody who is able to access the "
-                                "offline token file is able to use it for "
-                                "login."))
-        return True
-
     @check_acls(['edit:period'])
     @object_lock()
     @backend.transaction
     def change_period(self, run_policies=True, period=None,
         _caller="API", callback=default_callback, **kwargs):
         """ Change token check period. """
         if run_policies:
@@ -773,94 +560,26 @@
                 except:
                     pass
 
         self.forward_drift = forward_drift
 
         return self._cache(callback=callback)
 
-    def _change_secret(self, secret=None, pre=False,
-        force=False, callback=default_callback, **kwargs):
-        """ Handle stuff when changing token secret """
-        if self.mode == "mode2":
-            if pre:
-                callback.send(_("WARNING: Changing the secret of a token in "
-                                "mode2 is not supported. The secret changes "
-                                "if you change the PIN."))
-                return False
-        else:
-            if pre and not force:
-                callback.send(_("WARNING: Changing the secret requires a "
-                                "re-deployment of the token."))
-                answer = callback.ask("Change token secret?: ")
-                if answer.lower() == "y":
-                    return True
-                else:
-                    return False
-            self.server_secret = None
-        return True
-
-    def _change_pin(self, pin=None, pre=False,
-        callback=default_callback, **kwargs):
-        """ Handle stuff when changing token PIN """
-        if self.mode == "mode2":
-            if pre:
-                callback.send(_("WARNING: Changing the PIN of a token in mode2 "
-                                "requires a re-deployment of the token."))
-                answer = callback.ask("Change token PIN?: ")
-                if answer.lower() == "y":
-                    return True
-                else:
-                    return False
-            self.server_secret = stuff.gen_secret(self.secret_len)
-            token_secret = self.get_secret(pin=pin)
-            callback.send(_("New token secret: %s") % token_secret)
-
-        elif self.server_secret:
-            if pre:
-                callback.send(_("WARNING: This token was previously used in "
-                                "mode2. Changing the PIN requires a "
-                                "re-deployment when changing back to mode2."))
-                answer = callback.ask("Change token PIN?: ")
-                if answer.lower() == "y":
-                    return True
-                else:
-                    return False
-            self.server_secret = None
-
-        # Update PIN length.
-        if not pre:
-            self.pin_len = len(pin)
-        return True
-
-    def _enable_offline(self, pre=False, callback=default_callback, **kwargs):
-        """ Handle stuff when enabling offline mode """
-        if pre:
-            if self.mode == "mode1":
-                msg = (_("WARNING: Anybody who gets access to the offline "
-                        "token file is able to use it for logins and can see "
-                        "your PIN in clear-text!!"))
-                callback.send(msg)
-                msg = (_("You should consider changing token mode to mode2!!"))
-                callback.send(msg)
-            else:
-                msg = (_("INFO: Offline OTP tokens are by design vulnerable "
-                        "for brute force attacks if an attacker is able to "
-                        "steal them (e.g. from a notebook)"))
-                callback.send(msg)
-        return True
-
     @check_acls(['generate:otp'])
     def gen_otp(self, otp_count=1, secret=None, prefix_pin=False,
         callback=default_callback, _caller="API", **kwargs):
         """ Generate one or more OTPs for this token. """
         if not secret:
-            if self.secret:
-                secret = self.secret
-            else:
-                secret = self.get_secret(pin=prefix_pin)
+            if self.mode == "mode1":
+                secret = self.get_secret(callback=callback)
+            if self.mode == "mode2":
+                if not prefix_pin:
+                    msg = "Cannot generate OTP in mode2."
+                    return callback.error(msg)
+                secret = self.get_secret(pin=prefix_pin, callback=callback)
 
         if not secret:
             callback.error("Unable to get token secret.")
 
         epoch_time = time.time()
         if otp_count > 1:
             otps = []
@@ -882,46 +601,14 @@
                                 format=self.otp_format)
         if prefix_pin:
             otp = "%s%s" % (prefix_pin, otp)
         if _caller == "CLIENT":
             return callback.ok(otp)
         return [otp]
 
-    def test(self, password=None, callback=default_callback, **kwargs):
-        """ Test if the given OTP can be verified by this token. """
-        ok_message = "Token verified successful."
-        error_message = "Token verification failed."
-
-        if self.pin_enabled:
-            otp_prompt = "PIN+OTP: "
-        else:
-            otp_prompt = "OTP: "
-
-        if not password:
-            password = callback.askpass(otp_prompt)
-
-        if not password:
-            return callback.error("Unable to get OTP.")
-
-        status = self.verify_otp(otp=str(password), **kwargs)
-
-        if status:
-            return callback.ok(ok_message)
-        else:
-            return callback.error(error_message)
-
-    def verify(self, challenge=None, response=None, **kwargs):
-        """ Call default verify method. """
-        if challenge and response:
-            return self.verify_mschap_otp(challenge=challenge,
-                                            response=response,
-                                            **kwargs)
-        else:
-            return self.verify_otp(**kwargs)
-
     def verify_otp(self, otp, secret=None, handle_used_otps=True,
         mode=None, otp_includes_pin=True, verify_pin=True, sft=None,
         recursive_use=False, session_uuid=None, **kwargs):
         """ Verify OTP for this token.  """
         # Make sure OTP is str().
         otp = str(otp)
 
@@ -940,23 +627,27 @@
         if mode == "mode1":
             if not self.pin_enabled:
                 verify_pin = False
                 # We decide on token mode if OTP includes a PIN because we
                 # allow to "emulate" the given token mode (e.g. use in
                 # change_mode())
                 otp_includes_pin = False
+        # In mode2 no PIN verification can be done as the PIN is not
+        # saved on server side.
+        if mode == "mode2":
+            verify_pin = False
 
         # Get PIN from OTP if needed.
         if otp_includes_pin:
             if len(otp) < (int(self.pin_len) + int(self.otp_len)):
                 logger.debug("Token PIN enabled but the given OTP is too short "
                             "to include a PIN!")
                 return None
             _otp = otp[self.pin_len:]
-            pin = otp[:self.pin_len]
+            pin = int(otp[:self.pin_len])
         else:
             _otp = otp
 
         # Calculate epoch time to verify OTP.
         epoch_time = time.time()
 
         # Calculate times for log entry.
@@ -1051,20 +742,19 @@
 
     def verify_mschap_otp(self, challenge, response,
         handle_used_otps=True, session_uuid=None, **kwargs):
         """ Verify MSCHAP challenge/response against OTPs. """
         from otpme.lib import mschap_util
         nt_key = None
         otp = None
-        pin = None
         _otp = None
 
-        # Set PIN we need to prefix our OTPs with needed.
-        if self.pin_enabled:
-            pin = self.pin
+        # Cannot verify token in mode2.
+        if self.mode == "mode2":
+            return return_value
 
         # Calculate epoch time to verify OTP.
         epoch_time = time.time()
 
         # Calculate times for log entry.
         otp_validity_range_start_timestamp = float(epoch_time - (self.period * self.backward_drift))
         otp_validity_range_start_timestamp = float(str(otp_validity_range_start_timestamp)[:-2])
@@ -1073,15 +763,15 @@
         otp_validity_start_time = str(datetime.fromtimestamp(otp_validity_range_start_timestamp))
         otp_validity_end_time = str(datetime.fromtimestamp(otp_validity_range_end_timestamp))
 
         # xxxxxxxxxxxxxxxxxxxxx
         # FIXME: we also need OTPs from self.backward_drift here!
         # Get list with valid OTPs of this token.
         otps = self.gen_otp(otp_count=self.forward_drift + 1,
-                            prefix_pin=pin,
+                            prefix_pin=self.pin,
                             verify_acls=False)
 
         # Set default return values.
         failed_return_value = False, False, False
         return_value = None, False, False
 
         logger.debug("Verifiying OTP within timerange: start='%s' end='%s'."
@@ -1107,50 +797,35 @@
         # definitively failed because we havent found an already used OTP)
         return return_value
 
         # This point should never be reached.
         msg = ("WARNING: You may have hit a BUG of Token().verify_mschap_otp().")
         raise Exception(msg)
 
-    @check_acls(['generate:otp'])
-    def gen_mschap(self, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Generate MSCHAP challenge response stuff for testing. """
-        if run_policies:
-            try:
-                self.run_policies("gen_mschap",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception:
-                return callback.error()
-
-        pin = None
-        if self.mode == "mode1":
-            if self.pin_enabled:
-                pin = self.pin
-        if self.mode == "mode2":
-            pin = self.pin
-        otp = self.gen_otp(prefix_pin=pin, verify_acls=False)[0]
-        return Token._gen_mschap(self, password=otp, callback=callback)
-
     @check_acls(['generate:qrcode'])
-    def gen_qrcode(self, qrcode_file=None, run_policies=True,
+    def gen_qrcode(self, pin=None, qrcode_file=None, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Generate QRCode to deploy token secret. """
         if run_policies:
             try:
                 self.run_policies("gen_qrcode",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        # FIXME: implement qrcode_file stuff
+        if pin is None:
+            if self.mode == "mode2":
+                pin = callback.askpass("Please enter PIN: ")
+                if pin is None:
+                    msg = "Cannot gen qrcode without PIN."
+                    return callback.error(msg)
+
         # Get secret to gen QRCode.
-        secret = self.get_secret()
+        secret = self.get_secret(pin=pin)
 
         # Gen OATH URI.
         user_string = "%s@%s" % (self.rel_path, self.realm)
         #oath_uri = TOTP(secret)
         #oath_uri = oath_uri.provisioning_uri(name=user_string,
         #                                    issuer_name=config.my_name)
         # Use oath-toolkit.
@@ -1166,58 +841,34 @@
         # xxxxxxxxxxxxx
         # FIXME: how to create png/svg image without writing to file?
         return callback.ok(_qrcode)
 
     def add_used_otp(self, otp, session_uuid=None, quiet=True):
         """ Add used OTP for this user/token. """
         # In offline mode we do not add used OTPs to make brute force attacks
-        # harder (no OTP hash saved to disk)
+        # harder (no OTP hash saved to disk).
         if self.offline:
             return True
         # Cache TOTPs twice the time they are valid.
         expiry = time.time() + (self.period * self.forward_drift * 2)
         # Add used OTP using parent class method.
-        return Token._add_used_otp(self, otp, expiry,
-                                session_uuid=session_uuid,
-                                quiet=quiet)
+        self._add_used_otp(otp, expiry,
+                        session_uuid=session_uuid,
+                        quiet=quiet)
 
     @object_lock()
     @backend.transaction
-    def _add(self, gen_qrcode=True, callback=default_callback, **kwargs):
+    def _add(self, *args, **kwargs):
         """ Add a token. """
         # Get default TOTP settings.
         self.otp_format = self.get_config_parameter("totp_format")
         self.period = self.get_config_parameter("totp_period")
         self.forward_drift = self.get_config_parameter("totp_forward_drift")
         self.backward_drift = self.get_config_parameter("totp_backward_drift")
-        # Gen server secret.
-        self.server_secret = stuff.gen_secret(self.secret_len)
-        # Gen PIN.
-        default_pin_len = self.get_config_parameter("totp_default_pin_len")
-        self.pin = stuff.gen_pin(default_pin_len)
-        self.pin_len = len(self.pin)
-        # Get token secret.
-        token_secret = self.get_secret(pin=self.pin)
-        # Generate salt for used OTP hashes.
-        self.used_otp_salt = stuff.gen_secret(32)
-
-        return_message = None
-        if self.verify_acl("view:secret"):
-            if gen_qrcode:
-                term_qrcode = self.gen_qrcode(run_policies=False)
-                callback.send(term_qrcode)
-            return_message = "Token secret: %s" % token_secret
-        if self.verify_acl("view:pin"):
-            message = "Token PIN: %s" % self.pin
-            if return_message:
-                return_message = "%s\n%s" % (return_message, message)
-            else:
-                return_message = message
-
-        return callback.ok(return_message)
+        return super(TotpToken, self)._add(*args, **kwargs)
 
     def show_config(self, callback=default_callback, **kwargs):
         """ Show token info. """
         if not self.verify_acl("view_public:object"):
             msg = ("Permission denied.")
             return callback.error(msg, exception=PermissionDenied)
         lines = []
@@ -1241,18 +892,17 @@
         lines.append('FORWARD_DRIFT="%s"' % forward_drift)
 
         server_secret = ""
         if self.verify_acl("view:server_secret"):
             server_secret = str(self.server_secret)
         lines.append('SERVER_SECRET="%s"' % server_secret)
 
-        return Token.show_config(self,
-                                config_lines=lines,
-                                callback=callback,
-                                **kwargs)
+        return super(TotpToken, self).show_config(config_lines=lines,
+                                                callback=callback,
+                                                **kwargs)
 
     def show(self, **kwargs):
         """ Show token details. """
         #if not self.verify_acl("view_public:object"):
         #    msg = ("Permission denied.")
         #    return callback.error(msg, exception=PermissionDenied)
         return self.show_config(**kwargs)
```

### Comparing `otpme-0.3.0a45/otpme/lib/token/utils.py` & `otpme-0.3.0a46/otpme/lib/token/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme/lib/token/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme.egg-info/PKG-INFO` & `otpme-0.3.0a46/otpme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a45
+Version: 0.3.0a46
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a45/otpme.egg-info/SOURCES.txt` & `otpme-0.3.0a46/otpme.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 deploy/dicts/german-guessing.gz
 deploy/dicts/german.gz
 deploy/dicts/us-female.gz
 deploy/dicts/us-male.gz
 deploy/dicts/us-surnames.gz
 deploy/pam/pam_otpme.py
 deploy/pam/pam-python/README
+deploy/radius/dictionary
+deploy/radius/dictionary.freeradius
 deploy/schema/core.schema
 deploy/schema/cosine.schema
 deploy/schema/inetorgperson.schema
 deploy/schema/nis.schema
 deploy/scripts/agent_script.sh
 deploy/scripts/auth_script.sh
 deploy/scripts/key_script.sh
@@ -391,14 +393,16 @@
 otpme/lib/token/fido2/fido2.py
 otpme/lib/token/hotp/__init__.py
 otpme/lib/token/hotp/hotp.py
 otpme/lib/token/link/__init__.py
 otpme/lib/token/link/link.py
 otpme/lib/token/motp/__init__.py
 otpme/lib/token/motp/motp.py
+otpme/lib/token/oath/__init__.py
+otpme/lib/token/oath/oath.py
 otpme/lib/token/otp_push/__init__.py
 otpme/lib/token/otp_push/otp_push.py
 otpme/lib/token/otpme/__init__.py
 otpme/lib/token/otpme/otpme.py
 otpme/lib/token/password/__init__.py
 otpme/lib/token/password/password.py
 otpme/lib/token/script_otp/__init__.py
```

### Comparing `otpme-0.3.0a45/otpme.egg-info/entry_points.txt` & `otpme-0.3.0a46/otpme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a45/otpme.egg-info/requires.txt` & `otpme-0.3.0a46/otpme.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -34,20 +34,22 @@
 psutil>=5.5.1
 psycopg2>=2.8.6
 pyOpenSSL>=0.15.1
 pycryptodome>=3.4.3
 pycryptodomex>=3.7.3
 pylibacl>=0.5.1
 pylibmc>=1.6.3
+pyrad>=2.4
 pyre2>=0.3.6
 pysodium>=0.7.10
 python-magic>=0.4.15
 python-yubico>=1.3.3
 pytz>=2019.3
 qrcode>=5.1
+radius-eap-mschapv2-client>=1.0.6
 redis>=3.3.11
 scapy>=2.4.4
 service_identity
 setproctitle>=1.1.10
 termcolor>=1.1.0
 tinydb>=4.5.2
 ujson>=5.7.0
```

### Comparing `otpme-0.3.0a45/setup.py` & `otpme-0.3.0a46/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,16 @@
                 #"pyoath-toolkit>=2.0.dev1",
                 "PyQRCode>=1.2.1",
                 "pyre2>=0.3.6",
                 #"re2>=0.2.22",
                 # Failes to install via pip.
                 #"systemd>=0.16.1",
                 "termcolor>=1.1.0",
-                #"radius-eap-mschapv2-client>=1.0.6",
+                "radius-eap-mschapv2-client>=1.0.6",
+                "pyrad>=2.4",
                 #"py-radius>=2.0.2.post1",
 
                 # apt-get install libffi-dev libssl-dev
 
                 # For use with U2F token (client site only).
                 #"hidapi>=0.7.99.post8",
                 #"python-u2flib-host>=3.0.0",
@@ -179,14 +180,17 @@
                 ),
                 ('/etc/otpme/dicts',
                     get_files("deploy/dicts/")
                 ),
                 ('/etc/otpme/scripts',
                     get_files("deploy/scripts/")
                 ),
+                ('/etc/otpme/radius',
+                    get_files("deploy/radius/")
+                ),
                 ('/etc/bash_completion.d/',
                     [
                         'bash_completion/otpme',
                     ]
                 ),
                 ('/etc/deploy/',
                     [
```

