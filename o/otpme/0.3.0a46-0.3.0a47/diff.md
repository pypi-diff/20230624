# Comparing `tmp/otpme-0.3.0a46.tar.gz` & `tmp/otpme-0.3.0a47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpme-0.3.0a46.tar", last modified: Sat Jun 24 05:09:50 2023, max compression
+gzip compressed data, was "otpme-0.3.0a47.tar", last modified: Sat Jun 24 20:18:32 2023, max compression
```

## Comparing `otpme-0.3.0a46.tar` & `otpme-0.3.0a47.tar`

### file list

```diff
@@ -1,508 +1,508 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/
--rw-r--r--   0 root         (0) root         (0)    35121 2023-06-24 05:09:50.000000 otpme-0.3.0a46/LICENSE
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-24 05:09:50.000000 otpme-0.3.0a46/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-24 05:09:50.962409 otpme-0.3.0a46/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3821 2023-06-24 05:09:50.000000 otpme-0.3.0a46/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.926408 otpme-0.3.0a46/bash_completion/
--rw-r--r--   0 root         (0) root         (0)     1937 2023-06-24 05:09:50.000000 otpme-0.3.0a46/bash_completion/otpme
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.926408 otpme-0.3.0a46/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.926408 otpme-0.3.0a46/deploy/dicts/
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/abbreviations-it.gz
--rw-r--r--   0 root         (0) root         (0)    18683 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/at-surnames.gz
--rw-r--r--   0 root         (0) root         (0)   197269 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/common-passwords.gz
--rwxr-xr-x   0 root         (0) root         (0)      532 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/convert_dict.sh
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-female.gz
--rw-r--r--   0 root         (0) root         (0)     3070 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-male.gz
--rw-r--r--   0 root         (0) root         (0)    11343 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    34845 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/de-top10000.gz
--rw-r--r--   0 root         (0) root         (0)    30600 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/en-top10000.gz
--rw-r--r--   0 root         (0) root         (0)   127983 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/english-guessing.gz
--rw-r--r--   0 root         (0) root         (0)  1041710 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/english.gz
--rw-r--r--   0 root         (0) root         (0)   547291 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/german-guessing.gz
--rw-r--r--   0 root         (0) root         (0)   544600 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/german.gz
--rw-r--r--   0 root         (0) root         (0)    13539 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/us-female.gz
--rw-r--r--   0 root         (0) root         (0)     4089 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/us-male.gz
--rw-r--r--   0 root         (0) root         (0)    35682 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/dicts/us-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    13208 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/otpme.conf.dist
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/pam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/pam/pam-python/
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/pam/pam-python/README
--rw-r--r--   0 root         (0) root         (0)     2436 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/pam/pam_otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/radius/
--rw-r--r--   0 root         (0) root         (0)    13085 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/radius/dictionary
--rw-r--r--   0 root         (0) root         (0)     3851 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/radius/dictionary.freeradius
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/schema/
--rw-r--r--   0 root         (0) root         (0)    21610 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/core.schema
--rw-r--r--   0 root         (0) root         (0)    73993 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/cosine.schema
--rw-r--r--   0 root         (0) root         (0)     6267 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/inetorgperson.schema
--rw-r--r--   0 root         (0) root         (0)     7632 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/schema/nis.schema
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/deploy/scripts/
--rw-r--r--   0 root         (0) root         (0)     8600 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/agent_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/auth_script.sh
--rw-r--r--   0 root         (0) root         (0)    21137 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/key_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/login_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 05:09:50.000000 otpme-0.3.0a46/deploy/scripts/push_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/otpme/
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11946 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/
--rw-r--r--   0 root         (0) root         (0)    12877 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/arp.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/auth_script.py
--rw-r--r--   0 root         (0) root         (0)    45358 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/backends/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/backends/file/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89733 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/file.py
--rw-r--r--   0 root         (0) root         (0)    13013 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/index.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/models.py
--rw-r--r--   0 root         (0) root         (0)    74192 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/backends/file/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.934408 otpme-0.3.0a46/otpme/lib/cache/
--rw-r--r--   0 root         (0) root         (0)    33856 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/dogpile.py
--rw-r--r--   0 root         (0) root         (0)    19991 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/funccache.py
--rw-r--r--   0 root         (0) root         (0)     3538 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/lru.py
--rw-r--r--   0 root         (0) root         (0)    13901 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/memcache.py
--rw-r--r--   0 root         (0) root         (0)     6500 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/memcached.py
--rw-r--r--   0 root         (0) root         (0)     7344 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/memcachedb.py
--rw-r--r--   0 root         (0) root         (0)    26853 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.938408 otpme-0.3.0a46/otpme/lib/classes/
--rw-r--r--   0 root         (0) root         (0)      917 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85744 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)    14874 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/agent_conn.py
--rw-r--r--   0 root         (0) root         (0)   127394 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/auth_handler.py
--rw-r--r--   0 root         (0) root         (0)    54320 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/ca.py
--rw-r--r--   0 root         (0) root         (0)    40376 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/client.py
--rw-r--r--   0 root         (0) root         (0)   210451 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/command_handler.py
--rw-r--r--   0 root         (0) root         (0)     8601 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/conn_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/classes/data_objects/
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/cert.py
--rw-r--r--   0 root         (0) root         (0)     6543 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/failed_pass.py
--rw-r--r--   0 root         (0) root         (0)     7679 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/last_assigned_id.py
--rw-r--r--   0 root         (0) root         (0)    10578 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/revoked_signature.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/rsa_key.py
--rw-r--r--   0 root         (0) root         (0)     7020 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/skip_sync.py
--rw-r--r--   0 root         (0) root         (0)     5762 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/token_counter.py
--rw-r--r--   0 root         (0) root         (0)     5646 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_hash.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_otp.py
--rw-r--r--   0 root         (0) root         (0)     5723 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_slp.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/data_objects/used_sotp.py
--rw-r--r--   0 root         (0) root         (0)    28183 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    38860 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/group.py
--rw-r--r--   0 root         (0) root         (0)    49804 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/host.py
--rw-r--r--   0 root         (0) root         (0)    11992 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/login_handler.py
--rw-r--r--   0 root         (0) root         (0)     5500 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/mgmt_client.py
--rw-r--r--   0 root         (0) root         (0)    33067 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/node.py
--rw-r--r--   0 root         (0) root         (0)    21597 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/object_config.py
--rw-r--r--   0 root         (0) root         (0)    76766 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/otpme_agent.py
--rw-r--r--   0 root         (0) root         (0)    49375 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/otpme_host.py
--rw-r--r--   0 root         (0) root         (0)   300315 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/otpme_object.py
--rw-r--r--   0 root         (0) root         (0)    22938 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/policy.py
--rw-r--r--   0 root         (0) root         (0)    63265 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/realm.py
--rw-r--r--   0 root         (0) root         (0)    61677 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/resolver.py
--rw-r--r--   0 root         (0) root         (0)    44644 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/role.py
--rw-r--r--   0 root         (0) root         (0)    33753 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/script.py
--rw-r--r--   0 root         (0) root         (0)    56576 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/session.py
--rw-r--r--   0 root         (0) root         (0)    31485 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/signing.py
--rw-r--r--   0 root         (0) root         (0)   104716 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/site.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/ssh_agent.py
--rw-r--r--   0 root         (0) root         (0)   132552 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/token.py
--rw-r--r--   0 root         (0) root         (0)    49045 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/unit.py
--rw-r--r--   0 root         (0) root         (0)   170349 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/classes/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/cli/
--rw-r--r--   0 root         (0) root         (0)    64756 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12995 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     7091 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/ca.py
--rw-r--r--   0 root         (0) root         (0)    13451 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/client.py
--rw-r--r--   0 root         (0) root         (0)     5615 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    13271 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/group.py
--rw-r--r--   0 root         (0) root         (0)    13349 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/host.py
--rw-r--r--   0 root         (0) root         (0)    11183 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/node.py
--rw-r--r--   0 root         (0) root         (0)     6137 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/policy.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/realm.py
--rw-r--r--   0 root         (0) root         (0)     6572 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/resolver.py
--rw-r--r--   0 root         (0) root         (0)    21218 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/role.py
--rw-r--r--   0 root         (0) root         (0)     7355 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/script.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/site.py
--rw-r--r--   0 root         (0) root         (0)    16298 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/token.py
--rw-r--r--   0 root         (0) root         (0)     5391 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/unit.py
--rw-r--r--   0 root         (0) root         (0)     7604 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/cli/user.py
--rw-r--r--   0 root         (0) root         (0)    24404 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/compgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/compression/
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3941 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/compression/base.py
--rw-r--r--   0 root         (0) root         (0)    11149 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/connections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/daemon/
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/authd.py
--rw-r--r--   0 root         (0) root         (0)    99221 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/clusterd.py
--rw-r--r--   0 root         (0) root         (0)    44813 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/controld.py
--rw-r--r--   0 root         (0) root         (0)    73948 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/hostd.py
--rw-r--r--   0 root         (0) root         (0)     3141 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/joind.py
--rw-r--r--   0 root         (0) root         (0)     6780 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/ldapd.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/mgmtd.py
--rw-r--r--   0 root         (0) root         (0)    15556 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/otpme_daemon.py
--rw-r--r--   0 root         (0) root         (0)    11048 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/scriptd.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/syncd.py
--rw-r--r--   0 root         (0) root         (0)     6888 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/daemon/unix_daemon.py
--rw-r--r--   0 root         (0) root         (0)    19072 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/debug.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/encoding/
--rw-r--r--   0 root         (0) root         (0)      496 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encoding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encoding/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/encryption/
--rw-r--r--   0 root         (0) root         (0)     4020 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3362 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/aes.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/aes_cfb.py
--rw-r--r--   0 root         (0) root         (0)     7967 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/argon2.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/asymmetric_key_handler.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/ec.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/fernet.py
--rw-r--r--   0 root         (0) root         (0)     3304 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/hkdf.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/pbkdf2.py
--rw-r--r--   0 root         (0) root         (0)     7891 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/encryption/rsa.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/extensions/
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.942408 otpme-0.3.0a46/otpme/lib/extensions/base/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11447 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/base/base.py
--rw-r--r--   0 root         (0) root         (0)    40105 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/ldif_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/extensions/posix/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/posix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15729 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/posix/posix.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/extensions/utils.py
--rw-r--r--   0 root         (0) root         (0)    36868 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/filetools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/freeradius/
--rw-r--r--   0 root         (0) root         (0)     9274 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18752 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/otpme.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/radiusd.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/freeradius/radiusd_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/gpg/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/gpg/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    28565 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/gpg/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/help/
--rwxr-xr-x   0 root         (0) root         (0)    26596 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22571 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     5552 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/agent.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/auth.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/ca.py
--rw-r--r--   0 root         (0) root         (0)    16524 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/controld.py
--rw-r--r--   0 root         (0) root         (0)    10976 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/dictionary.py
--rw-r--r--   0 root         (0) root         (0)      589 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/get_authorized_keys.py
--rw-r--r--   0 root         (0) root         (0)    19149 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/group.py
--rw-r--r--   0 root         (0) root         (0)    23587 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/host.py
--rw-r--r--   0 root         (0) root         (0)    21011 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/node.py
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/pinentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/help/policy/
--rw-r--r--   0 root         (0) root         (0)     8665 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3777 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/authonaction.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/autodisable.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultgroups.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultpolicies.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultroles.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/defaultunits.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/idrange.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/logintimes.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/objecttemplates.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/password.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/policy/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)    19622 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/realm.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.946409 otpme-0.3.0a46/otpme/lib/help/resolver/
--rw-r--r--   0 root         (0) root         (0)    11252 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4381 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/resolver/ldap.py
--rw-r--r--   0 root         (0) root         (0)    17945 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/role.py
--rw-r--r--   0 root         (0) root         (0)    14711 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/script.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/session.py
--rw-r--r--   0 root         (0) root         (0)    21392 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/help/token/
--rw-r--r--   0 root         (0) root         (0)    19325 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/fido2.py
--rw-r--r--   0 root         (0) root         (0)     6369 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/hotp.py
--rw-r--r--   0 root         (0) root         (0)     6406 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/motp.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/otp_push.py
--rw-r--r--   0 root         (0) root         (0)     5018 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/otpme.py
--rw-r--r--   0 root         (0) root         (0)     3947 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/password.py
--rw-r--r--   0 root         (0) root         (0)     7318 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/ssh.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/totp.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/yubikey_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/token/yubikey_hotp.py
--rw-r--r--   0 root         (0) root         (0)    23731 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/tool.py
--rw-r--r--   0 root         (0) root         (0)    14774 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/unit.py
--rw-r--r--   0 root         (0) root         (0)    28280 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/help/user.py
--rw-r--r--   0 root         (0) root         (0)    16367 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/host.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/humanize/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/humanize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/humanize/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/index/
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23971 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/mysql.py
--rw-r--r--   0 root         (0) root         (0)    24446 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/postgres.py
--rw-r--r--   0 root         (0) root         (0)     8403 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/index/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/job/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18955 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/job/callback.py
--rw-r--r--   0 root         (0) root         (0)    12568 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/job/otpme_job.py
--rw-r--r--   0 root         (0) root         (0)    36904 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/join.py
--rw-r--r--   0 root         (0) root         (0)     4924 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/json.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/ldap/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/client.py
--rw-r--r--   0 root         (0) root         (0)    11129 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/schema.py
--rw-r--r--   0 root         (0) root         (0)    49844 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ldap/server.py
--rw-r--r--   0 root         (0) root         (0)    18710 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/locking.py
--rw-r--r--   0 root         (0) root         (0)     9515 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/log.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/messages.py
--rw-r--r--   0 root         (0) root         (0)     6048 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/mschap.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/mschap_util.py
--rw-r--r--   0 root         (0) root         (0)    35675 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/multiprocessing.py
--rw-r--r--   0 root         (0) root         (0)    10033 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/net.py
--rw-r--r--   0 root         (0) root         (0)    25699 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/nsscache.py
--rw-r--r--   0 root         (0) root         (0)    63395 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/offline_token.py
--rw-r--r--   0 root         (0) root         (0)    24416 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/oid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/oath/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/oath/hotp.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/oath/totp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/otpme/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/otp/yubico/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/yubico/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otp/yubico/yubiotp.py
--rw-r--r--   0 root         (0) root         (0)    19754 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otpme_acl.py
--rw-r--r--   0 root         (0) root         (0)   112530 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otpme_config.py
--rw-r--r--   0 root         (0) root         (0)     3586 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/otpme_pass.py
--rw-r--r--   0 root         (0) root         (0)    70426 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pam.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pickle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/pinentry/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pinentry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27532 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pinentry/pinentry.py
--rwxr-xr-x   0 root         (0) root         (0)     7947 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pinentry/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/pki/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9864 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/cert.py
--rw-r--r--   0 root         (0) root         (0)    22943 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/utils.py
--rw-r--r--   0 root         (0) root         (0)    16957 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/pki/utils_openssl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/authonaction/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/authonaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32525 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/authonaction/authonaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/autodisable/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/autodisable/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17448 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/autodisable/autodisable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultgroups/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultgroups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17153 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultgroups/defaultgroups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/defaultpolicies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultroles/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultroles/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13849 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultroles/defaultroles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.950409 otpme-0.3.0a46/otpme/lib/policy/defaultunits/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultunits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15386 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/defaultunits/defaultunits.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/forcetoken/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/forcetoken/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13989 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/forcetoken/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/idrange/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/idrange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27087 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/idrange/idrange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/logintimes/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/logintimes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22816 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/logintimes/logintimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/objecttemplates/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/objecttemplates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14703 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/objecttemplates/objecttemplates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/password/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28730 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/policy/tokenacls/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/tokenacls/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24736 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/tokenacls/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     8921 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/preload.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/protocols/
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/protocols/client/
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/agent1.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/auth1.py
--rw-r--r--   0 root         (0) root         (0)    13302 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/get_class.py
--rw-r--r--   0 root         (0) root         (0)     4712 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/host1.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/join1.py
--rwxr-xr-x   0 root         (0) root         (0)    11372 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    66489 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/client/sync1.py
--rw-r--r--   0 root         (0) root         (0)   158940 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/otpme_client.py
--rw-r--r--   0 root         (0) root         (0)    77419 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/otpme_server.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/request.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/protocols/server/
--rw-r--r--   0 root         (0) root         (0)      894 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40286 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/agent1.py
--rw-r--r--   0 root         (0) root         (0)    13083 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/auth1.py
--rw-r--r--   0 root         (0) root         (0)    30300 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/get_class.py
--rw-r--r--   0 root         (0) root         (0)    25856 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/host1.py
--rw-r--r--   0 root         (0) root         (0)    50743 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/join1.py
--rw-r--r--   0 root         (0) root         (0)    55241 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    46007 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/server/sync1.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     6712 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/protocols/utils.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/push_script.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/register/
--rw-r--r--   0 root         (0) root         (0)     9783 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/register/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/resolver/
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/resolver/ldap/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35657 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/ldap/ldap.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/resolver/utils.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/script.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/sign_key_cache.py
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/slp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/smartcard/
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.954409 otpme-0.3.0a46/otpme/lib/smartcard/fido2/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10228 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/get_class.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12018 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/usb.py
--rw-r--r--   0 root         (0) root         (0)     8142 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey/yubikey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6431 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12022 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/socket/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13129 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/connect.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/handler.py
--rw-r--r--   0 root         (0) root         (0)    30823 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/listen.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/socket/send_recv1.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/sotp.py
--rwxr-xr-x   0 root         (0) root         (0)    37180 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/spsc.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/srp.py
--rw-r--r--   0 root         (0) root         (0)    23521 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/ssh.py
--rw-r--r--   0 root         (0) root         (0)    61848 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/stuff.py
--rw-r--r--   0 root         (0) root         (0)    12345 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/sync_cache.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/system_command.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/
--rw-r--r--   0 root         (0) root         (0)     1981 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/advanced.py
--rw-r--r--   0 root         (0) root         (0)     9859 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/caching_query.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/environment.py
--rw-r--r--   0 root         (0) root         (0)     1764 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/fixture_data.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/helloworld.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/local_session_caching.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/model.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/relationship_caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9083 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/caches.py
--rw-r--r--   0 root         (0) root         (0)    14341 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/files.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/config.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/error.py
--rw-r--r--   0 root         (0) root         (0)     7963 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/group.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/maps.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/passwd.py
--rw-r--r--   0 root         (0) root         (0)     2387 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/shadow.py
--rw-r--r--   0 root         (0) root         (0)     4140 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/nss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/files_updater.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/map_updater.py
--rw-r--r--   0 root         (0) root         (0)    10980 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/updater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4117 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/file_formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/_compat.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/token/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/token/fido2/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14964 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)     1123 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.958409 otpme-0.3.0a46/otpme/lib/token/hotp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39686 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/hotp/hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/link/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/link/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9709 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/link/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/motp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/motp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27734 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/motp/motp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/oath/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18882 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/oath/oath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/otp_push/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otp_push/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23418 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otp_push/otp_push.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/otpme/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24757 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/password/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26093 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/script_otp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_otp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9744 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_otp/script_otp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/script_static/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_static/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9744 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/script_static/script_static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/ssh/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39544 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/ssh/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/totp/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/totp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35811 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/totp/totp.py
--rw-r--r--   0 root         (0) root         (0)      547 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.962409 otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25150 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 05:09:50.930408 otpme-0.3.0a46/otpme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13294 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1081 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      949 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-24 05:09:50.000000 otpme-0.3.0a46/otpme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 05:09:50.962409 otpme-0.3.0a46/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-24 05:09:50.000000 otpme-0.3.0a46/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.593524 otpme-0.3.0a47/
+-rw-r--r--   0 root         (0) root         (0)    35121 2023-06-24 20:18:32.000000 otpme-0.3.0a47/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-24 20:18:32.000000 otpme-0.3.0a47/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-24 20:18:32.589524 otpme-0.3.0a47/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-06-24 20:18:32.000000 otpme-0.3.0a47/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.541523 otpme-0.3.0a47/bash_completion/
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-06-24 20:18:32.000000 otpme-0.3.0a47/bash_completion/otpme
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.541523 otpme-0.3.0a47/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.553523 otpme-0.3.0a47/deploy/dicts/
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/abbreviations-it.gz
+-rw-r--r--   0 root         (0) root         (0)    18683 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/at-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)   197269 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/common-passwords.gz
+-rwxr-xr-x   0 root         (0) root         (0)      532 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/convert_dict.sh
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/de-female.gz
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/de-male.gz
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/de-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    34845 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/de-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)    30600 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/en-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)   127983 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/english-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)  1041710 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/english.gz
+-rw-r--r--   0 root         (0) root         (0)   547291 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/german-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)   544600 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/german.gz
+-rw-r--r--   0 root         (0) root         (0)    13539 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/us-female.gz
+-rw-r--r--   0 root         (0) root         (0)     4089 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/us-male.gz
+-rw-r--r--   0 root         (0) root         (0)    35682 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/dicts/us-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    13208 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/otpme.conf.dist
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.553523 otpme-0.3.0a47/deploy/pam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.553523 otpme-0.3.0a47/deploy/pam/pam-python/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/pam/pam-python/README
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/pam/pam_otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.557523 otpme-0.3.0a47/deploy/radius/
+-rw-r--r--   0 root         (0) root         (0)    13085 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/radius/dictionary
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/radius/dictionary.freeradius
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.557523 otpme-0.3.0a47/deploy/schema/
+-rw-r--r--   0 root         (0) root         (0)    21610 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/schema/core.schema
+-rw-r--r--   0 root         (0) root         (0)    73993 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/schema/cosine.schema
+-rw-r--r--   0 root         (0) root         (0)     6267 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/schema/inetorgperson.schema
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/schema/nis.schema
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.557523 otpme-0.3.0a47/deploy/scripts/
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/scripts/agent_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/scripts/auth_script.sh
+-rw-r--r--   0 root         (0) root         (0)    21137 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/scripts/key_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/scripts/login_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-24 20:18:32.000000 otpme-0.3.0a47/deploy/scripts/push_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.557523 otpme-0.3.0a47/otpme/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    12009 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.561524 otpme-0.3.0a47/otpme/lib/
+-rw-r--r--   0 root         (0) root         (0)    10490 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/arp.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/auth_script.py
+-rw-r--r--   0 root         (0) root         (0)    45358 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.561524 otpme-0.3.0a47/otpme/lib/backends/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.565523 otpme-0.3.0a47/otpme/lib/backends/file/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backends/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89733 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backends/file/file.py
+-rw-r--r--   0 root         (0) root         (0)    13013 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backends/file/index.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backends/file/models.py
+-rw-r--r--   0 root         (0) root         (0)    74192 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/backends/file/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.565523 otpme-0.3.0a47/otpme/lib/cache/
+-rw-r--r--   0 root         (0) root         (0)    33796 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)    19991 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/funccache.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/lru.py
+-rw-r--r--   0 root         (0) root         (0)    13901 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/memcache.py
+-rw-r--r--   0 root         (0) root         (0)     6500 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/memcached.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/memcachedb.py
+-rw-r--r--   0 root         (0) root         (0)    26853 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.569524 otpme-0.3.0a47/otpme/lib/classes/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85744 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)    14874 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/agent_conn.py
+-rw-r--r--   0 root         (0) root         (0)   127394 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/auth_handler.py
+-rw-r--r--   0 root         (0) root         (0)    54320 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/ca.py
+-rw-r--r--   0 root         (0) root         (0)    40376 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/client.py
+-rw-r--r--   0 root         (0) root         (0)   211612 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/command_handler.py
+-rw-r--r--   0 root         (0) root         (0)     8601 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/conn_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.569524 otpme-0.3.0a47/otpme/lib/classes/data_objects/
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/cert.py
+-rw-r--r--   0 root         (0) root         (0)     6543 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/failed_pass.py
+-rw-r--r--   0 root         (0) root         (0)     7679 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/last_assigned_id.py
+-rw-r--r--   0 root         (0) root         (0)    10578 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/revoked_signature.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/rsa_key.py
+-rw-r--r--   0 root         (0) root         (0)     7020 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/skip_sync.py
+-rw-r--r--   0 root         (0) root         (0)     5762 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/token_counter.py
+-rw-r--r--   0 root         (0) root         (0)     5646 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/used_hash.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/used_otp.py
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/used_slp.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/data_objects/used_sotp.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    38860 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/group.py
+-rw-r--r--   0 root         (0) root         (0)    49804 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/host.py
+-rw-r--r--   0 root         (0) root         (0)    12327 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/login_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5500 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/mgmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    33067 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/node.py
+-rw-r--r--   0 root         (0) root         (0)    21597 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/object_config.py
+-rw-r--r--   0 root         (0) root         (0)    77074 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/otpme_agent.py
+-rw-r--r--   0 root         (0) root         (0)    49470 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/otpme_host.py
+-rw-r--r--   0 root         (0) root         (0)   305483 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/otpme_object.py
+-rw-r--r--   0 root         (0) root         (0)    22938 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/policy.py
+-rw-r--r--   0 root         (0) root         (0)    62179 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/realm.py
+-rw-r--r--   0 root         (0) root         (0)    61677 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    44644 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/role.py
+-rw-r--r--   0 root         (0) root         (0)    33753 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/script.py
+-rw-r--r--   0 root         (0) root         (0)    56576 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/session.py
+-rw-r--r--   0 root         (0) root         (0)    31485 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/signing.py
+-rw-r--r--   0 root         (0) root         (0)   106817 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/site.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/ssh_agent.py
+-rw-r--r--   0 root         (0) root         (0)   133048 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/token.py
+-rw-r--r--   0 root         (0) root         (0)    49045 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/unit.py
+-rw-r--r--   0 root         (0) root         (0)   171469 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/classes/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.569524 otpme-0.3.0a47/otpme/lib/cli/
+-rw-r--r--   0 root         (0) root         (0)    64711 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12995 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/ca.py
+-rw-r--r--   0 root         (0) root         (0)    13451 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/client.py
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    13271 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/group.py
+-rw-r--r--   0 root         (0) root         (0)    13349 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/host.py
+-rw-r--r--   0 root         (0) root         (0)    11183 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/node.py
+-rw-r--r--   0 root         (0) root         (0)     6137 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/realm.py
+-rw-r--r--   0 root         (0) root         (0)     6572 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    21218 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/role.py
+-rw-r--r--   0 root         (0) root         (0)     7355 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/script.py
+-rw-r--r--   0 root         (0) root         (0)     7496 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/site.py
+-rw-r--r--   0 root         (0) root         (0)    16298 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/token.py
+-rw-r--r--   0 root         (0) root         (0)     5391 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/unit.py
+-rw-r--r--   0 root         (0) root         (0)     7604 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/cli/user.py
+-rw-r--r--   0 root         (0) root         (0)    24404 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/compgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.569524 otpme-0.3.0a47/otpme/lib/compression/
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3941 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/compression/base.py
+-rw-r--r--   0 root         (0) root         (0)    14165 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/connections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.569524 otpme-0.3.0a47/otpme/lib/daemon/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/authd.py
+-rw-r--r--   0 root         (0) root         (0)    98772 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/clusterd.py
+-rw-r--r--   0 root         (0) root         (0)    44820 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/controld.py
+-rw-r--r--   0 root         (0) root         (0)    73948 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/hostd.py
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/joind.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/ldapd.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/mgmtd.py
+-rw-r--r--   0 root         (0) root         (0)    15556 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/otpme_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    11048 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/scriptd.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/syncd.py
+-rw-r--r--   0 root         (0) root         (0)     6888 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/daemon/unix_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/debug.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/encoding/
+-rw-r--r--   0 root         (0) root         (0)      496 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encoding/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/encryption/
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/aes.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/aes_cfb.py
+-rw-r--r--   0 root         (0) root         (0)     7967 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/argon2.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/asymmetric_key_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/ec.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/fernet.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/hkdf.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/pbkdf2.py
+-rw-r--r--   0 root         (0) root         (0)     7891 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/encryption/rsa.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/extensions/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/extensions/base/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11447 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/base/base.py
+-rw-r--r--   0 root         (0) root         (0)    40105 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/ldif_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/extensions/posix/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/posix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15729 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/posix/posix.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/extensions/utils.py
+-rw-r--r--   0 root         (0) root         (0)    36868 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/filetools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/freeradius/
+-rw-r--r--   0 root         (0) root         (0)     9274 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/freeradius/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18752 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/freeradius/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/freeradius/radiusd.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/freeradius/radiusd_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.573524 otpme-0.3.0a47/otpme/lib/gpg/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/gpg/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    28565 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/gpg/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/help/
+-rwxr-xr-x   0 root         (0) root         (0)    26596 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22571 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/agent.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/auth.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/ca.py
+-rw-r--r--   0 root         (0) root         (0)    16524 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/controld.py
+-rw-r--r--   0 root         (0) root         (0)    10976 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/get_authorized_keys.py
+-rw-r--r--   0 root         (0) root         (0)    19149 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/group.py
+-rw-r--r--   0 root         (0) root         (0)    23587 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/host.py
+-rw-r--r--   0 root         (0) root         (0)    21011 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/node.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/pinentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/help/policy/
+-rw-r--r--   0 root         (0) root         (0)     8665 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/authonaction.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/autodisable.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/defaultgroups.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/defaultpolicies.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/defaultroles.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/defaultunits.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/idrange.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/logintimes.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/objecttemplates.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/password.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/policy/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)    19639 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/realm.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/help/resolver/
+-rw-r--r--   0 root         (0) root         (0)    11252 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/resolver/ldap.py
+-rw-r--r--   0 root         (0) root         (0)    17945 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/role.py
+-rw-r--r--   0 root         (0) root         (0)    14711 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/script.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/session.py
+-rw-r--r--   0 root         (0) root         (0)    22094 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/help/token/
+-rw-r--r--   0 root         (0) root         (0)    19856 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/motp.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/otp_push.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/password.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/totp.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/yubikey_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/token/yubikey_hotp.py
+-rw-r--r--   0 root         (0) root         (0)    23893 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/tool.py
+-rw-r--r--   0 root         (0) root         (0)    14774 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/unit.py
+-rw-r--r--   0 root         (0) root         (0)    28809 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/help/user.py
+-rw-r--r--   0 root         (0) root         (0)    16367 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/host.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/humanize/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/humanize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/humanize/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/index/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23971 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/index/mysql.py
+-rw-r--r--   0 root         (0) root         (0)    24446 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/index/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     8403 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/index/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/job/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18955 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/job/callback.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/job/otpme_job.py
+-rw-r--r--   0 root         (0) root         (0)    37185 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/join.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/json.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/ldap/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/ldap/client.py
+-rw-r--r--   0 root         (0) root         (0)    11129 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/ldap/schema.py
+-rw-r--r--   0 root         (0) root         (0)    49844 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/ldap/server.py
+-rw-r--r--   0 root         (0) root         (0)    18710 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/locking.py
+-rw-r--r--   0 root         (0) root         (0)     9515 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/log.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     6048 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/mschap.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/mschap_util.py
+-rw-r--r--   0 root         (0) root         (0)    35675 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/multiprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    10317 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/net.py
+-rw-r--r--   0 root         (0) root         (0)    25699 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/nsscache.py
+-rw-r--r--   0 root         (0) root         (0)    63395 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/offline_token.py
+-rw-r--r--   0 root         (0) root         (0)    24416 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/oid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/otp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/otp/oath/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/oath/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/oath/totp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.577524 otpme-0.3.0a47/otpme/lib/otp/otpme/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/otp/yubico/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/yubico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otp/yubico/yubiotp.py
+-rw-r--r--   0 root         (0) root         (0)    19754 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otpme_acl.py
+-rw-r--r--   0 root         (0) root         (0)   112772 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otpme_config.py
+-rw-r--r--   0 root         (0) root         (0)     3586 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/otpme_pass.py
+-rw-r--r--   0 root         (0) root         (0)    70426 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pam.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pickle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/pinentry/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pinentry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27532 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pinentry/pinentry.py
+-rwxr-xr-x   0 root         (0) root         (0)     7947 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pinentry/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/pki/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pki/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9864 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pki/cert.py
+-rw-r--r--   0 root         (0) root         (0)    22943 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pki/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16957 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/pki/utils_openssl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/authonaction/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/authonaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32426 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/authonaction/authonaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/autodisable/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/autodisable/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/autodisable/autodisable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/defaultgroups/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultgroups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17153 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultgroups/defaultgroups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/defaultpolicies/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultpolicies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultpolicies/defaultpolicies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/defaultroles/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultroles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13849 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultroles/defaultroles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/defaultunits/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultunits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15386 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/defaultunits/defaultunits.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/forcetoken/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/forcetoken/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13989 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/forcetoken/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/idrange/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/idrange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27087 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/idrange/idrange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/logintimes/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/logintimes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22816 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/logintimes/logintimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/objecttemplates/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/objecttemplates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14703 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/objecttemplates/objecttemplates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/password/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28730 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/policy/tokenacls/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/tokenacls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24736 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/tokenacls/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8921 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/preload.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.581524 otpme-0.3.0a47/otpme/lib/protocols/
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/protocols/client/
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/agent1.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    13302 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/host1.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/join1.py
+-rwxr-xr-x   0 root         (0) root         (0)    11372 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    66489 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/client/sync1.py
+-rw-r--r--   0 root         (0) root         (0)   156851 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/otpme_client.py
+-rw-r--r--   0 root         (0) root         (0)    77890 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/otpme_server.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/request.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/protocols/server/
+-rw-r--r--   0 root         (0) root         (0)      894 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40286 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/agent1.py
+-rw-r--r--   0 root         (0) root         (0)    13168 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    30371 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/get_class.py
+-rw-r--r--   0 root         (0) root         (0)    26622 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/host1.py
+-rw-r--r--   0 root         (0) root         (0)    50910 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/join1.py
+-rw-r--r--   0 root         (0) root         (0)    55421 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    46111 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/server/sync1.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/protocols/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/push_script.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/register/
+-rw-r--r--   0 root         (0) root         (0)     9783 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/register/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/resolver/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/resolver/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/resolver/ldap/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/resolver/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35657 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/resolver/ldap/ldap.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/resolver/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/script.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/sign_key_cache.py
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/slp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/smartcard/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/smartcard/fido2/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10228 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/smartcard/yubikey/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12018 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey/usb.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey/yubikey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_gpg/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_gpg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12022 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hotp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/socket/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/socket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13129 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/socket/connect.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/socket/handler.py
+-rw-r--r--   0 root         (0) root         (0)    30823 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/socket/listen.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/socket/send_recv1.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/sotp.py
+-rwxr-xr-x   0 root         (0) root         (0)    37180 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/spsc.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/srp.py
+-rw-r--r--   0 root         (0) root         (0)    23521 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/ssh.py
+-rw-r--r--   0 root         (0) root         (0)    63039 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/stuff.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/sync_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/system_command.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.585524 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/advanced.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/caching_query.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/fixture_data.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/helloworld.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/local_session_caching.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/model.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/relationship_caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/caches/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/caches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9083 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/caches/caches.py
+-rw-r--r--   0 root         (0) root         (0)    14341 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/caches/files.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/config.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/error.py
+-rw-r--r--   0 root         (0) root         (0)     7963 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/group.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/maps.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/passwd.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/shadow.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/nss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/files_updater.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/map_updater.py
+-rw-r--r--   0 root         (0) root         (0)    10980 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/updater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4117 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/nss_cache/util/file_formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/third_party/oath_toolkit/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/oath_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/oath_toolkit/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/third_party/oath_toolkit/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/fido2/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/hotp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39786 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/hotp/hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/link/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/link/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9709 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/link/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/motp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/motp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27734 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/motp/motp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/oath/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18882 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/oath/oath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/otp_push/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/otp_push/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23418 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/otp_push/otp_push.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/otpme/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24757 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/password/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26093 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/script_otp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/script_otp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/script_otp/script_otp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/script_static/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/script_static/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/script_static/script_static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/ssh/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39544 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/ssh/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/totp/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/totp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35891 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/totp/totp.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.589524 otpme-0.3.0a47/otpme/lib/token/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25150 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 20:18:32.561524 otpme-0.3.0a47/otpme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      949 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-24 20:18:32.000000 otpme-0.3.0a47/otpme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 20:18:32.593524 otpme-0.3.0a47/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-06-24 20:18:32.000000 otpme-0.3.0a47/setup.py
```

### Comparing `otpme-0.3.0a46/LICENSE` & `otpme-0.3.0a47/LICENSE`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/MANIFEST.in` & `otpme-0.3.0a47/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/PKG-INFO` & `otpme-0.3.0a47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a46
+Version: 0.3.0a47
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a46/README` & `otpme-0.3.0a47/README`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/bash_completion/otpme` & `otpme-0.3.0a47/bash_completion/otpme`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/abbreviations-it.gz` & `otpme-0.3.0a47/deploy/dicts/abbreviations-it.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/at-surnames.gz` & `otpme-0.3.0a47/deploy/dicts/at-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/common-passwords.gz` & `otpme-0.3.0a47/deploy/dicts/common-passwords.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/convert_dict.sh` & `otpme-0.3.0a47/deploy/dicts/convert_dict.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/de-female.gz` & `otpme-0.3.0a47/deploy/dicts/de-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/de-male.gz` & `otpme-0.3.0a47/deploy/dicts/de-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/de-surnames.gz` & `otpme-0.3.0a47/deploy/dicts/de-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/de-top10000.gz` & `otpme-0.3.0a47/deploy/dicts/de-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/en-top10000.gz` & `otpme-0.3.0a47/deploy/dicts/en-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/english-guessing.gz` & `otpme-0.3.0a47/deploy/dicts/english-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/english.gz` & `otpme-0.3.0a47/deploy/dicts/english.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/german-guessing.gz` & `otpme-0.3.0a47/deploy/dicts/german-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/german.gz` & `otpme-0.3.0a47/deploy/dicts/german.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/us-female.gz` & `otpme-0.3.0a47/deploy/dicts/us-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/us-male.gz` & `otpme-0.3.0a47/deploy/dicts/us-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/dicts/us-surnames.gz` & `otpme-0.3.0a47/deploy/dicts/us-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/otpme.conf.dist` & `otpme-0.3.0a47/deploy/otpme.conf.dist`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/pam/pam_otpme.py` & `otpme-0.3.0a47/deploy/pam/pam_otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/radius/dictionary` & `otpme-0.3.0a47/deploy/radius/dictionary`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/radius/dictionary.freeradius` & `otpme-0.3.0a47/deploy/radius/dictionary.freeradius`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/schema/core.schema` & `otpme-0.3.0a47/deploy/schema/core.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/schema/cosine.schema` & `otpme-0.3.0a47/deploy/schema/cosine.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/schema/inetorgperson.schema` & `otpme-0.3.0a47/deploy/schema/inetorgperson.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/schema/nis.schema` & `otpme-0.3.0a47/deploy/schema/nis.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/scripts/agent_script.sh` & `otpme-0.3.0a47/deploy/scripts/agent_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/deploy/scripts/key_script.sh` & `otpme-0.3.0a47/deploy/scripts/key_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/__init__.py` & `otpme-0.3.0a47/otpme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __project_url__ = "http://www.otpme.org"
 __copyright__ = "Copyright 2014-2022 the2nd <the2nd@otpme.org>"
 __project_description__ = "OTPme: A flexible One-Time-Password system."
 __author__ = "the2nd"
 __email__ = "the2nd@otpme.org"
 __credits__ = []
 __license__ = "GPLv2"
-__version__ = "0.3.0a46"
+__version__ = "0.3.0a47"
 __status__ = "Development Status :: 3 - Alpha"
 # In future versions :D
 #__status__ = "Development Status :: 4 - Beta"
 #__status__ = "Development Status :: 5 - Production/Stable"
 __pkg_name__ = __project_name__
 __maintainer__ = __author__
 __author_email__  = __email__
```

### Comparing `otpme-0.3.0a46/otpme/command.py` & `otpme-0.3.0a47/otpme/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     if not no_debug:
         if config.print_timing_results:
             from otpme.lib import debug
             debug.print_timing_result(print_status=True)
 
     return exit_code
 
-
 # We need this to get gettext module working with e.g. umlauts.
 if sys.version[0] == '2':
     reload(sys)
     sys.setdefaultencoding('utf8')
     #print(sys.getdefaultencoding())
 
 # Workaround used for OTPme development.
@@ -114,31 +113,31 @@
             x = x.replace("\n", "")
             if x in sys.path:
                 continue
             sys.path.append(x)
     finally:
         fd.close()
 
+# Get tool name.
+tool_name = str(os.path.basename(sys.argv[0]))
+# Get command from system command (e.g. otpme-user -> user).
+command = "-".join(tool_name.split("-")[1:])
+
+from otpme.lib.otpme_config import OTPmeConfig
+config = OTPmeConfig(tool_name, auto_load=False)
+
 #import trace
 from otpme.lib.help import get_help
 from otpme.lib.help import command_map
 from otpme.lib.messages import message
 from otpme.lib.help import get_main_opts
 from otpme.lib.messages import error_message
-
-from otpme.lib.exceptions import *
-
-# Register help.
 from otpme.lib.help.register import register_help
-register_help()
 
-# Get tool name.
-tool_name = str(os.path.basename(sys.argv[0]))
-# Get command from system command (e.g. otpme-user -> user).
-command = "-".join(tool_name.split("-")[1:])
+from otpme.lib.exceptions import *
 
 # Check if user requested our version.
 if len(sys.argv) > 1 and sys.argv[1] == "--version":
     from otpme import __version__
     message(__version__)
     sys.exit(0)
 
@@ -152,14 +151,15 @@
 setproctitle.setproctitle(new_proctitle)
 
 #setproctitle.setproctitle(tool_name)
 sys.argv.pop(0)
 
 help_needed = False
 help_message = None
+register_help()
 
 # Set cli object type.
 subcommand = None
 object_type = "main"
 if "--type" in sys.argv:
     opt_pos = sys.argv.index("--type")
     type_pos = opt_pos + 1
@@ -168,14 +168,15 @@
         sys.argv.pop(opt_pos)
         sys.argv.pop(opt_pos)
     except IndexError:
         help_message = "Missing object type: --type"
         help_msg = get_help(command, error=help_message)
         error_message(help_msg)
         sys.exit(0)
+config.cli_object_type = object_type
 
 # Check if we have to print the help screen.
 try:
     get_main_opts(mod_name=object_type)
 except OTPmeException as e:
     help_needed = True
     help_message = str(e)
@@ -283,23 +284,22 @@
                     if isinstance(_nt_hash, bytes):
                         _nt_hash = _nt_hash.decode()
                     if _nt_hash == nt_hash:
                         message("Accept")
                         sys.exit(0)
 
 # Load OTPme config.
-from otpme.lib.otpme_config import OTPmeConfig
-config = OTPmeConfig(tool_name, quiet=True)
-config.cli_object_type = object_type
+config.load(quiet=True)
 # Print warning if API mode is requested and daemon is running.
 if config.use_api:
-    if os.path.exists(config.controld_pidfile):
-        error_message("Warning!!! API mode should be used with care while "
-        + "daemons are running. Your changes may be lost or result in "
-        + "malfunction!")
+    if not "--compgen" in sys.argv:
+        if os.path.exists(config.controld_pidfile):
+            error_message("Warning!!! API mode should be used with care while "
+            + "daemons are running. Your changes may be lost or result in "
+            + "malfunction!")
 
 # Check if all required modules are installed.
 config.check_modules()
 
 # Verify OTPme config.
 try:
     config.verify()
```

### Comparing `otpme-0.3.0a46/otpme/lib/arp.py` & `otpme-0.3.0a47/otpme/lib/arp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/auth_script.py` & `otpme-0.3.0a47/otpme/lib/auth_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/backend.py` & `otpme-0.3.0a47/otpme/lib/backend.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/backends/file/file.py` & `otpme-0.3.0a47/otpme/lib/backends/file/file.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/backends/file/index.py` & `otpme-0.3.0a47/otpme/lib/backends/file/index.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/backends/file/models.py` & `otpme-0.3.0a47/otpme/lib/backends/file/models.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/backends/file/transaction.py` & `otpme-0.3.0a47/otpme/lib/backends/file/transaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/__init__.py` & `otpme-0.3.0a47/otpme/lib/cache/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,15 @@
 PROCESS_CACHE = "instance"
 MULTIPROCESSING_CACHE = "multiprocessing"
 
 ACL_CACHE_LOCK_TYPE = "cache.acl"
 LIST_CACHE_LOCK_TYPE = "cache.list"
 PICKLE_CACHE_LOCK_TYPE = "cache.pickle"
 
-try:
-    default_callback = config.get_callback()
-except AttributeError:
-    default_callback = None
+default_callback = config.get_callback()
 
 REGISTER_BEFORE = []
 REGISTER_AFTER = []
 
 modules = [
         'otpme.lib.cache.redis',
         'otpme.lib.cache.dogpile',
```

### Comparing `otpme-0.3.0a46/otpme/lib/cache/dogpile.py` & `otpme-0.3.0a47/otpme/lib/cache/dogpile.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/funccache.py` & `otpme-0.3.0a47/otpme/lib/cache/funccache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/lru.py` & `otpme-0.3.0a47/otpme/lib/cache/lru.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/memcache.py` & `otpme-0.3.0a47/otpme/lib/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/memcached.py` & `otpme-0.3.0a47/otpme/lib/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/memcachedb.py` & `otpme-0.3.0a47/otpme/lib/cache/memcachedb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cache/redis.py` & `otpme-0.3.0a47/otpme/lib/cache/redis.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/__init__.py` & `otpme-0.3.0a47/otpme/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/accessgroup.py` & `otpme-0.3.0a47/otpme/lib/classes/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/agent_conn.py` & `otpme-0.3.0a47/otpme/lib/classes/agent_conn.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/auth_handler.py` & `otpme-0.3.0a47/otpme/lib/classes/auth_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/ca.py` & `otpme-0.3.0a47/otpme/lib/classes/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/client.py` & `otpme-0.3.0a47/otpme/lib/classes/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/command_handler.py` & `otpme-0.3.0a47/otpme/lib/classes/command_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -811,15 +811,15 @@
             if subcommand == "join":
                 return self.handle_join_command(object_identifier, command_args)
 
             if subcommand == "leave":
                 return self.handle_leave_command(object_identifier, command_args)
 
         if subcommand == "login":
-            return self.handle_login_command(command_line)
+            return self.handle_login_command(command, subcommand, command_line)
 
         if subcommand == "logout":
             return self.logout()
 
         if subcommand == "whoami":
             return self.whoami()
 
@@ -1226,24 +1226,49 @@
                         site_key_len=site_key_len,
                         no_daemon_start=no_daemon_start,
                         trust_site_cert=trust_site_cert,
                         fingerprint_digest=fingerprint_digest,
                         check_site_cert=site_cert_fingerprint)
         return result
 
-    def handle_login_command(self, command_line):
+    def handle_login_command(self, command, subcommand, command_line):
         """ Handle login command. """
         #register_module("otpme.lib.protocols.client.host1")
         #register_module("otpme.lib.protocols.client.agent1")
         try:
+            command_syntax = self.get_command_syntax(command, subcommand)
+        except:
+            return self.get_help(_("Unknown command: %s") % subcommand)
+
+        command_args = {}
+        try:
+            object_cmd, \
+            object_required, \
+            object_identifier, \
+            command_args = cli.get_opts(command_syntax=command_syntax,
+                                            command_line=command_line,
+                                            command_args=command_args)
+        except Exception as e:
+            if str(e) == "help":
+                return self.get_help()
+            elif str(e) != "":
+                return self.get_help(str(e))
+        try:
             username = command_line[0]
         except:
             username = None
+        try:
+            node = command_args['node']
+        except:
+            node = None
+
         result = self.login(username=username,
-                    password=self.user_password)
+                        password=self.user_password,
+                        node=node)
+
         return result
 
     def handle_leave_command(self, object_identifier, command_args):
         """ Handle leave command. """
         try:
             lotp = command_args['lotp']
         except:
@@ -3557,46 +3582,54 @@
                                         lotp=lotp)
         finally:
             if disabled_interactive_policies:
                 if "interactive" in config.ignore_policy_tags:
                     config.ignore_policy_tags.remove("interactive")
         return result
 
-    def login(self, username=None, password=None):
+    def login(self, username=None, password=None, node=None):
         """ Do realm login. """
         from otpme.lib.classes.login_handler import LoginHandler
         #init_otpme(use_backend=False)
         self.init(use_backend=False)
         try:
             stuff.start_otpme_agent(user=config.system_user(),
                                     wait_for_socket=False,
                                     quiet=False)
         except Exception as e:
             config.raise_exception()
             raise OTPmeException(_("Unable to start otpme-agent: %s") % e)
         login_handler = LoginHandler()
-        login_handler.login(username=username,
-                            password=password,
-                            interactive=True,
-                            use_dns=config.use_dns,
-                            #cache_login_tokens=True,
-                            start_otpme_agent=False,
-                            login_use_dns=config.login_use_dns,
-                            use_ssh_agent=config.use_ssh_agent,
-                            use_smartcard=config.use_smartcard)
+        try:
+            login_handler.login(username=username,
+                                password=password,
+                                node=node,
+                                interactive=True,
+                                use_dns=config.use_dns,
+                                #cache_login_tokens=True,
+                                start_otpme_agent=False,
+                                login_use_dns=config.login_use_dns,
+                                use_ssh_agent=config.use_ssh_agent,
+                                use_smartcard=config.use_smartcard)
+        except Exception as e:
+            raise OTPmeException(str(e))
         login_message = login_handler.login_reply['login_message']
         return login_message
 
     def logout(self):
         """ Do realm logout. """
         from otpme.lib.classes.login_handler import LoginHandler
         #init_otpme(use_backend=False)
         self.init(use_backend=False)
         login_handler = LoginHandler()
-        return login_handler.logout()
+        try:
+            result = login_handler.logout()
+        except Exception as e:
+            raise OTPmeException(str(e))
+        return result
 
     def whoami(self):
         """ Get login status. """
         from otpme.lib.classes.login_handler import LoginHandler
         #init_otpme(use_backend=False)
         self.init(use_backend=False)
         login_handler = LoginHandler()
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/conn_handler.py` & `otpme-0.3.0a47/otpme/lib/classes/conn_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/__init__.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/cert.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/failed_pass.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/failed_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/last_assigned_id.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/last_assigned_id.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/revoked_signature.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/revoked_signature.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/rsa_key.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/rsa_key.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/skip_sync.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/skip_sync.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/token_counter.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/token_counter.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_hash.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/used_hash.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_otp.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/used_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_slp.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/used_slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/data_objects/used_sotp.py` & `otpme-0.3.0a47/otpme/lib/classes/data_objects/used_sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/dictionary.py` & `otpme-0.3.0a47/otpme/lib/classes/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/group.py` & `otpme-0.3.0a47/otpme/lib/classes/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/host.py` & `otpme-0.3.0a47/otpme/lib/classes/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/login_handler.py` & `otpme-0.3.0a47/otpme/lib/classes/login_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         print(_("Loading module: %s" % __name__))
 except:
     pass
 
 from otpme.lib import net
 from otpme.lib import config
 from otpme.lib import connections
-from otpme.lib.protocols.otpme_client import OTPmeClient
 
 from otpme.lib.exceptions import *
 
 class LoginHandler(object):
     """ Class to login, logout and auth users. """
     def __init__(self):
         self.login_reply = {}
@@ -45,15 +44,15 @@
         login_interface="tty", use_smartcard=False, use_ssh_agent=False,
         password_method=None, ssh_agent_method=None, need_ssh_key_pass=False,
         change_user=False, endpoint=True, unlock=False, interactive=False,
         add_agent_session=None, add_login_session=True, check_login_status=True,
         cache_login_tokens=False, sync_token_data=False, auth_only=False,
         start_otpme_agent=True, jwt_auth=False, jwt_method=None, message_method=None,
         error_message_method=None, connect_timeout=3, timeout=10,
-        offline_key_derivation_func=None, offline_key_func_opts={},
+        node=None, offline_key_derivation_func=None, offline_key_func_opts={},
         check_offline_pass_strength=False, offline_iterations_by_score={},
         offline_session_key=None, login_session_id=None, add_agent_acl=False,
         cleanup_method=None, socket_uri=None, login_use_dns=False, use_dns=False):
         """ Send realm login request. """
         login = True
         exception = None
 
@@ -86,17 +85,21 @@
             # Try to get realm/site to connect to via DNS.
             x = net.get_otpme_site(domain)
             realm = x['realm']
             site = x['site']
             # Try to get daemon socket URI via DNS.
             socket_uri = net.get_daemon_uri("authd", domain)
 
+        if node:
+            port = config.default_ports['authd']
+            socket_uri = "tcp://%s:%s" % (node, port)
+
         # Try to get connection to authd.
         try:
-            auth_conn = OTPmeClient(daemon="authd",
+            auth_conn = connections.get(daemon="authd",
                                     timeout=timeout,
                                     connect_timeout=connect_timeout,
                                     use_dns=use_dns,
                                     use_agent=False,
                                     use_ssh_agent=use_ssh_agent,
                                     ssh_agent_method=ssh_agent_method,
                                     start_otpme_agent=start_otpme_agent,
@@ -124,14 +127,18 @@
                                     interactive=interactive, endpoint=endpoint,
                                     offline_key_derivation_func=offline_key_derivation_func,
                                     offline_key_func_opts=offline_key_func_opts,
                                     check_offline_pass_strength=check_offline_pass_strength,
                                     offline_iterations_by_score=offline_iterations_by_score,
                                     offline_session_key=offline_session_key,
                                     socket_uri=socket_uri, realm=realm, site=site)
+        except ConnectionError as e:
+            msg = "Login connection failed: %s" % e
+            self.logger.warning(msg)
+            raise
         except Exception as e:
             config.raise_exception()
             msg = (_("Unable to connect to auth daemon: %s") % e)
             raise OTPmeException(msg)
 
         # Send auth/login request.
         login_message = None
@@ -256,24 +263,26 @@
 
         if not verify_server_session:
             return agent_username
 
         # Try to get connection to mgmtd.
         mgmt_conn = None
         try:
-            mgmt_conn = OTPmeClient(daemon="mgmtd",
-                                    realm=login_realm,
-                                    site=login_site,
-                                    use_agent=True,
-                                    username=agent_username,
-                                    autoconnect=True)
+            mgmt_conn = connections.get(daemon="mgmtd",
+                                        realm=login_realm,
+                                        site=login_site,
+                                        use_agent=True,
+                                        auto_auth=False,
+                                        username=agent_username,
+                                        autoconnect=True)
         except AuthFailed as e:
             msg = (_("Authentication failed: %s") % e)
             status_message = (_("%s (online: %s)") % (agent_username, msg))
         except Exception as e:
+            print("KKKKKK", e)
             status_message = (_("%s (offline)") % agent_username)
 
         if mgmt_conn:
             command_args = {}
             try:
                 status, \
                 status_code, \
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/mgmt_client.py` & `otpme-0.3.0a47/otpme/lib/classes/mgmt_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/node.py` & `otpme-0.3.0a47/otpme/lib/classes/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/object_config.py` & `otpme-0.3.0a47/otpme/lib/classes/object_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/otpme_agent.py` & `otpme-0.3.0a47/otpme/lib/classes/otpme_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 from otpme.lib import stuff
 from otpme.lib import cache
 from otpme.lib import config
 from otpme.lib import locking
 from otpme.lib import filetools
 from otpme.lib import otpme_pass
 from otpme.lib import init_otpme
+from otpme.lib import connections
 from otpme.lib import multiprocessing
 #from otpme.lib.messages import error_message
 from otpme.lib.protocols import status_codes
 from otpme.lib.register import register_module
 from otpme.lib.socket.listen import ListenSocket
 from otpme.lib.offline_token import OfflineToken
 from otpme.lib.multiprocessing import start_thread
 from otpme.lib.daemon.unix_daemon import UnixDaemon
 from otpme.lib.multiprocessing import get_sync_manager
 from otpme.lib.classes.conn_handler import ConnHandler
 from otpme.lib.socket.handler import SocketProtoHandler
-from otpme.lib.protocols.otpme_client import OTPmeClient
 
 from otpme.lib.exceptions import *
 
 CONN_LOCK_TYPE = "agent.connection"
 
 multiprocessing.register()
 locking.register_lock_type(CONN_LOCK_TYPE, module=__file__)
@@ -304,15 +304,15 @@
                 pid_end_command = "pid_ended %s" % login_pid
                 comm_handler = self.comm_queue.get_handler("wait_for_pid")
                 comm_handler.send(recipient="main_process",
                                     command=pid_end_command,
                                     timeout=1)
                 comm_handler.close()
             if not login_pid in self.login_sessions:
-                msg = ("Stopped watching PID with no more login session: %s"
+                msg = ("Stopped watching PID with no more login sessions: %s"
                         % login_pid)
                 self.logger.debug(msg)
                 break
         try:
             self.watch_pids.remove(login_pid)
         except:
             pass
@@ -581,21 +581,21 @@
         last_reneg = session['last_reneg']
         reneg_age = time.time() - last_reneg
 
         # Try to update session.
         msg = ("Trying to renegotiate session for user: %s" % login_user)
         self.logger.debug(msg)
         try:
-            auth_conn = OTPmeClient(daemon="authd", realm=realm, site=site,
-                                    connect_timeout=self.connect_timeout,
-                                    timeout=config.reneg_timeout, endpoint=False,
-                                    use_agent=False, username=login_user,
-                                    autoconnect=True, auto_auth=False,
-                                    allow_untrusted=True, sync_token_data=False,
-                                    reneg=True, rsp=rsp)
+            auth_conn = connections.get(daemon="authd", realm=realm, site=site,
+                                        connect_timeout=self.connect_timeout,
+                                        timeout=config.reneg_timeout, endpoint=False,
+                                        use_agent=False, username=login_user,
+                                        autoconnect=True, auto_auth=False,
+                                        allow_untrusted=True, sync_token_data=False,
+                                        reneg=True, rsp=rsp)
         except Exception as e:
             msg = ("Error getting daemon connection for session renegotiation: "
                     "%s" % e)
             self.logger.warning(msg)
             update_message = msg
             try_update = False
 
@@ -732,31 +732,37 @@
 
         # FIXME: Should we walk through all sessions and check if ssh_agent_pid is used by other session and if not kill agent and remove session??!
 
         # Try to logout user.
         self.logger.info("Trying to logout user: %s" % login_user)
 
         # Get connection to authd and logout.
-        try:
-            auth_conn = OTPmeClient(daemon="authd",
-                                    username=login_user,
-                                    realm=realm,
-                                    site=site,
-                                    slp=slp,
-                                    login=False,
-                                    logout=True,
-                                    use_agent=False,
-                                    auto_auth=False,
-                                    autoconnect=True,
-                                    allow_untrusted=True,
-                                    connect_timeout=self.connect_timeout,
-                                    timeout=self.timeout, endpoint=False)
-        except Exception as e:
-            msg = (_("Error connecting to auth daemon to logout: %s") % e)
-            raise OTPmeException(msg)
+        while True:
+            try:
+                auth_conn = connections.get(daemon="authd",
+                                            username=login_user,
+                                            realm=realm,
+                                            site=site,
+                                            slp=slp,
+                                            login=False,
+                                            logout=True,
+                                            use_agent=False,
+                                            auto_auth=False,
+                                            autoconnect=True,
+                                            allow_untrusted=True,
+                                            connect_timeout=self.connect_timeout,
+                                            timeout=self.timeout, endpoint=False)
+            except ConnectionError:
+                time.sleep(0.01)
+                continue
+            except Exception as e:
+                msg = (_("Error connecting to auth daemon to logout: %s") % e)
+                raise OTPmeException(msg)
+            else:
+                break
 
         # Send logout command.
         try:
             logout_message = auth_conn.authenticate()
             if logout_message:
                 msg = ("User logged out successfully: %s/%s" % (realm, site))
                 self.logger.info(msg)
@@ -1100,21 +1106,21 @@
             except Exception as e:
                 msg = (_("Error reading session infos: %s") % e)
                 self.logger.critical(msg)
                 raise Exception(msg)
 
             # Connect to daemon.
             try:
-                daemon_conn = OTPmeClient(daemon=daemon, realm=realm, site=site,
-                                        connect_timeout=self.connect_timeout,
-                                        timeout=self.timeout, endpoint=False,
-                                        use_agent=False, username=login_user,
-                                        rsp=rsp, autoconnect=True,
-                                        auto_auth=True, allow_untrusted=True,
-                                        sync_token_data=False)
+                daemon_conn = connections.get(daemon=daemon, realm=realm, site=site,
+                                            connect_timeout=self.connect_timeout,
+                                            timeout=self.timeout, endpoint=False,
+                                            use_agent=False, username=login_user,
+                                            rsp=rsp, autoconnect=True,
+                                            auto_auth=True, allow_untrusted=True,
+                                            sync_token_data=False)
             except AuthFailed as e:
                 msg = (_("Authentication failed while connecting to daemon: "
                         "%s: %s") % (daemon, e))
                 self.logger.warning(msg)
                 raise AuthFailed(msg)
             except Exception as e:
                 msg = (_("Error getting daemon connection: %s") % e)
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/otpme_host.py` & `otpme-0.3.0a47/otpme/lib/classes/otpme_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -772,15 +772,17 @@
                 config.raise_exception()
                 msg = str(e)
                 return callback.error(msg)
 
         # Set new cert.
         self.cert = cert
 
-        return self._cache(callback=callback)
+        self._cache(callback=callback)
+
+        return key, cert
 
     def gen_jotp(self):
         """ Gen realm join/leave OTP. """
         if self.type == "host":
             jotp_len = config.host_jotp_len
         if self.type == "node":
             jotp_len = config.node_jotp_len
@@ -906,18 +908,19 @@
 
             # Set cert.
             self.cert = cert
 
         # Create new host cert if needed.
         if cert_req:
             try:
-                self.renew_cert(cert_req=cert_req,
-                                cert_valid=cert_valid,
-                                verify_acls=False,
-                                callback=callback)
+                host_key, \
+                host_cert = self.renew_cert(cert_req=cert_req,
+                                            cert_valid=cert_valid,
+                                            verify_acls=False,
+                                            callback=callback)
             except Exception as e:
                 config.raise_exception()
                 msg = str(e)
                 return callback.error(msg)
 
         self.join_date = time.time()
         self.join_node = config.uuid
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/otpme_object.py` & `otpme-0.3.0a47/otpme/lib/classes/otpme_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from otpme.lib import stuff
 from otpme.lib import cache
 from otpme.lib import config
 from otpme.lib import locking
 from otpme.lib import backend
 from otpme.lib import otpme_acl
 from otpme.lib import encryption
+from otpme.lib.humanize import units
 from otpme.lib import multiprocessing
 from otpme.lib.pki.cert import SSLCert
 from otpme.lib.cache import ldif_cache
 from otpme.lib.cache import config_cache
 from otpme.lib.locking import object_lock
 from otpme.lib.otpme_acl import check_acls
 from otpme.lib.encoding.base import encode
@@ -1586,14 +1587,18 @@
         self.secret_format_warning = None
         self.signable = False
         self.signatures = {}
         self.creator = None
         self.creator_cache = None
         self.template_object = template
 
+        self.auto_disable = ""
+        self.unused_disable = False
+        self.auto_disable_start_time = 0.0
+
         # Config params of this object.
         self._config = {}
 
         self._base_sync_fields = {
                     'host'  : {
                         'trusted'  : [
                             "UUID",
@@ -1637,14 +1642,17 @@
                             "INDEX_JOURNAL_ID",
                             "INDEX_JOURNAL_ARCHIVE",
                             "TEMPLATE_INDEX",
                             "LDIF",
                             "LDIF_ATTRIBUTES",
                             "EXTENSION_ATTRIBUTES",
                             "ENABLED",
+                            "UNUSED_DISABLE",
+                            "AUTO_DISABLE",
+                            "AUTO_DISABLE_START_TIME",
                             "POLICIES",
                             "POLICY_OPTIONS",
                             "CONFIG_PARAMS",
                             "CHECKSUM",
                             "SYNC_CHECKSUM",
                             "SALT",
                             "DESCRIPTION",
@@ -1882,27 +1890,49 @@
                 logger.debug(msg)
             except Exception as e:
                 config.raise_exception()
                 msg = ("Error running 'exists' policy hook: %s: %s"
                         % (self.oid, e))
                 logger.warning(msg, exc_info=True)
 
+        # Check for auto-disable of object.
+        self.check_auto_disable()
+
         return True
 
     @property
     def enabled(self):
         if self.template_object:
             return False
+        self.check_auto_disable()
         return self._enabled
 
     @enabled.setter
     def enabled(self, enabled):
         self._enabled = enabled
 
     @property
+    def auto_disable_time(self):
+        if not self.auto_disable:
+            return 0.0
+        if self.unused_disable:
+            check_time = self.get_last_used_time()
+        else:
+            check_time = self.auto_disable_start_time
+        try:
+            # Check if given date string is valid.
+            auto_disable_time = units.string2unixtime(self.auto_disable, check_time)
+        except Exception as e:
+            msg = "Invalid date string: %s" % e
+            raise OTPmeException(msg)
+        auto_disable_time = datetime.datetime.fromtimestamp(auto_disable_time)
+        auto_disable_time = auto_disable_time.strftime('%d.%m.%Y %H:%M:%S')
+        return auto_disable_time
+
+    @property
     def valid_config_params(self):
         """ Get valid config parameters. """
         # Realm does support all config parameters.
         valid_config_params = []
         for x in config.valid_config_params:
             object_types = config.valid_config_params[x]['object_types']
             if self.type not in object_types:
@@ -1997,14 +2027,32 @@
 
             'ENABLED'                   : {
                                             'var_name'      : '_enabled',
                                             'type'          : bool,
                                             'required'      : True,
                                         },
 
+            'UNUSED_DISABLE'            : {
+                                            'var_name'      : 'unused_disable',
+                                            'type'          : bool,
+                                            'required'      : False,
+                                        },
+
+            'AUTO_DISABLE'            : {
+                                            'var_name'      : 'auto_disable',
+                                            'type'          : str,
+                                            'required'      : False,
+                                        },
+
+            'AUTO_DISABLE_START_TIME'   : {
+                                            'var_name'      : 'auto_disable_start_time',
+                                            'type'          : float,
+                                            'required'      : False,
+                                        },
+
             'LDIF'                      : {
                                             'var_name'      : 'ldif',
                                             'type'          : dict,
                                             'required'      : False,
                                         },
 
             'LDIF_ATTRIBUTES'           : {
@@ -4424,15 +4472,15 @@
     @check_acls(acls=['enable:object'])
     @check_special_user()
     @object_lock()
     def enable(self, force=False, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Enable the object. """
         if not force:
-            if self.enabled:
+            if self._enabled:
                 object_type = "%s%s" % (self.type[0].upper(), self.type[1:])
                 msg = (_("%s already enabled.") % object_type)
                 return callback.error(msg)
             if self.confirmation_policy == "paranoid":
                 msg = (_("Enable %(object_type)s '%(object_name)s'?: ")
                         % { "object_type":self.type, "object_name":self.name})
                 answer = callback.ask(msg)
@@ -4449,18 +4497,24 @@
                                 _caller=_caller,
                                 force=force)
             except Exception as e:
                 msg = str(e)
                 self.logger.warning(msg)
                 return callback.error()
 
-        self.enabled = True
+        self._enabled = True
         # Update index.
         self.update_index('enabled', True)
 
+        if self.auto_disable:
+            self.auto_disable_start_time = time.time()
+            msg = ("Auto-disable active for this object: %s"
+                    % self.auto_disable_time)
+            callback.send(msg)
+
         return self._cache(callback=callback)
 
     @check_acls(acls=['disable:object'])
     @object_lock()
     def disable(self, force=False, run_policies=True,
         _caller="API", callback=default_callback, **kwargs):
         """ Disable the object. """
@@ -4474,15 +4528,15 @@
                     dst_token = config.auth_token.get_destination_token()
                     if dst_token and dst_token.uuid == self.uuid and not force:
                         return callback.error("Cannot disable token used at login.")
             if self.name == config.admin_user_name:
                 return callback.error("Cannot disable admin user.")
 
         if not force:
-            if not self.enabled:
+            if not self._enabled:
                 object_type = "%s%s" % (self.type[0].upper(), self.type[1:])
                 msg = (_("%(object_type)s '%(object_name)s' already disabled.")
                         % {"object_type":object_type, "object_name":self.name})
                 return callback.error(msg)
 
         base_access_groups = config.get_base_objects("accessgroup")
         if self.name in base_access_groups:
@@ -4504,17 +4558,18 @@
                                 callback=callback,
                                 _caller=_caller)
                 self.run_policies("disable",
                                 callback=callback,
                                 _caller=_caller)
             except Exception as e:
                 msg = str(e)
+                config.raise_exception()
                 return callback.error(msg)
 
-        self.enabled = False
+        self._enabled = False
         # Update index.
         self.update_index('enabled', False)
 
         return self._cache(callback=callback)
 
     @object_lock()
     def enable_acl_inheritance(self, force=False, run_policies=True,
@@ -5288,14 +5343,84 @@
                 # Remove object from list because this list may be passed via
                 # kwargs to different handle_acl() calls e.g. in
                 # inherit_default_acl().
                 _acl_objects.remove(o)
 
         return callback.ok()
 
+    def check_auto_disable(self, **kwargs):
+        """ Handle auto disable. """
+        if not self.auto_disable:
+            return
+        if self.auto_disable_start_time == 0:
+            return
+        if not self._enabled:
+            return
+        if self.unused_disable:
+            check_time = self.get_last_used_time()
+        else:
+            check_time = self.auto_disable_start_time
+        disable_time = units.string2unixtime(self.auto_disable, check_time)
+        now = time.time()
+        if now >= disable_time:
+            try:
+                self.disable(force=True,
+                            verify_acls=False,
+                            run_policies=False)
+                object_disabled = True
+                self._write()
+            except Exception as e:
+                exception = e
+                object_disabled = False
+                config.raise_exception()
+            if object_disabled:
+                msg = (_("%s auto-disabled: %s") % (self.type, self.name))
+                logger.warning(msg)
+            else:
+                msg = (_("Cannot auto-disable object: %s: %s")
+                        % (self.name, exception))
+                logger.critical(msg)
+                return False
+        return True
+
+    @check_acls(['edit:auto_disable'])
+    @object_lock()
+    @backend.transaction
+    def change_auto_disable(self, auto_disable, unused=False,
+        run_policies=True, callback=default_callback,
+        _caller="API", **kwargs):
+        """ Change auto disable value. """
+        if auto_disable != 0:
+            try:
+                # Check if given date string is valid.
+                units.string2unixtime(auto_disable, time.time())
+            except Exception as e:
+                msg = "Invalid date string: %s" % e
+                return callback.error(msg)
+
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_auto_disable",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception:
+                return callback.error()
+
+        if auto_disable == 0:
+            self.auto_disable = ""
+        else:
+            self.unused_disable = unused
+            self.auto_disable = auto_disable
+            self.auto_disable_start_time = time.time()
+
+        return self._cache(callback=callback)
+
     def check_secret_format(self, secret, callback=default_callback):
         """ Check if the given secret is in the correct format """
         # Make sure secret is string.
         if isinstance(secret, bytes):
             secret = secret.decode()
         # Set secret format check stuff.
         self.secret_format_regex = '^[0-9A-Za-z]{%s}$' % self.secret_len
@@ -7032,14 +7157,22 @@
         if self.verify_acl("view:status") \
         or self.verify_acl("enable:object") \
         or self.verify_acl("disable:object"):
             lines.append('ENABLED="%s"' % self.enabled)
         else:
             lines.append('ENABLED=""')
 
+        if self.verify_acl("view:auto_disable") \
+        or self.verify_acl("edit:auto_disable"):
+            lines.append('AUTO_DISABLE="%s"' % self.auto_disable_time)
+            lines.append('UNUSED_DISABLE="%s"' % self.unused_disable)
+        else:
+            lines.append('AUTO_DISABLE=""')
+            lines.append('UNUSED_DISABLE=""')
+
         if self.verify_acl("view:extension") \
         or self.verify_acl("add:extension") \
         or self.verify_acl("remove:extension"):
             lines.append('EXTENSIONS="%s"' % ",".join(self.extensions))
         else:
             lines.append('EXTENSIONS=""')
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/policy.py` & `otpme-0.3.0a47/otpme/lib/classes/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/realm.py` & `otpme-0.3.0a47/otpme/lib/classes/realm.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,51 +101,28 @@
                                             'site_key_len',
                                             'site_valid',
                                             'node_key_len',
                                             'node_valid',
                                             'no_dicts',
                                             'dictionaries',
                                             'id_ranges',
-                                            ],
-                    'job_type'          : 'process',
-                    },
-                'exists'    : {
-                    'method'            : 'init',
-                    'oargs'             : [
-                                            'ca_country',
-                                            'ca_state',
-                                            'ca_locality',
-                                            'ca_organization',
-                                            'ca_ou',
-                                            'ca_email',
-                                            'ca_key_len',
-                                            'ca_valid',
-                                            'site_key_len',
-                                            'site_valid',
-                                            'node_key_len',
-                                            'node_valid',
-                                            'no_dicts',
-                                            'dictionaries',
+                                            'site_address',
+                                            'site_fqdn',
                                             ],
                     'job_type'          : 'process',
                     },
                 },
             },
     'add'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
                     'method'            : 'add',
                     'args'              : ['realm_address'],
                     'job_type'          : 'process',
                     },
-                'exists'    : {
-                    'method'            : 'add',
-                    'args'              : ['realm_address'],
-                    'job_type'          : 'process',
-                    },
                 },
             },
     'show'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
                     'method'            : cli.show_getter("realm"),
                     'oargs'              : [
@@ -1142,18 +1119,19 @@
         # Set new ca_data.
         self.ca_data = ca_data
 
         return self._write(callback=callback)
 
     @object_lock()
     #@backend.transaction
-    def init(self, realm_master, master_address, ca_key_len=None, ca_valid=None,
-        ca_country=None, ca_state=None, ca_locality=None, ca_organization=None,
-        ca_ou=None, ca_email=None, site_key_len=None, site_valid=None,
-        node_key_len=None, id_ranges=None, no_dicts=False, dictionaries=[],
+    def init(self, realm_master, site_fqdn, site_address=None,
+        ca_key_len=None, ca_valid=None, ca_country=None, ca_state=None,
+        ca_locality=None, ca_organization=None, ca_ou=None, ca_email=None,
+        site_key_len=None, site_valid=None, node_key_len=None,
+        id_ranges=None, no_dicts=False, dictionaries=[],
         callback=default_callback, **kwargs):
         """ Init OTPme realm. """
         from otpme.lib.classes.site import Site
         if ca_valid is None:
             ca_valid = config.default_ca_validity
         if ca_key_len is None:
             ca_key_len = config.default_ca_key_len
@@ -1184,27 +1162,25 @@
                         % {"object_type":t , "realm_name":self.name})
                 return callback.error(msg)
 
         # Disable interactive policies (e.g. reauth).
         if not "interactive" in config.ignore_policy_tags:
             config.ignore_policy_tags.append("interactive")
 
-        # Check if we got a IP address or a FQDN. This check is done on the
-        # node and not on the client because the node needs to connect to the
-        # site.
-        is_ip = net.is_ip(master_address)
-        if is_ip:
-            site_address = master_address
-        else:
+        if not site_address:
             # Try to get site address from DNS.
-            site_address = net.get_ip(master_address)
+            result = net.query_dns(site_fqdn)
+            if len(result) > 1:
+                msg = "Found round-robin DNS. Please give floating IP."
+                return callback.error(msg)
+            site_address = result[0]
 
         # We always need a site address as floaging cluster IP.
         if not site_address:
-            msg = ("Unable to resolve: %s" % master_address)
+            msg = ("Unable to resolve: %s" % site_fqdn)
             raise OTPmeException(msg)
 
         if site_address != "127.0.0.1":
             # Make sure we got a valid site address.
             callback.send("Verifying floaging IP: %s" % site_address)
             try:
                 net.configure_floating_ip(site_address, gratuitous_arp=False)
@@ -1251,30 +1227,31 @@
         master_site = Site(name=realm_master, realm=config.realm)
 
         if master_site.exists():
             msg = ("Uuuhhh, our master site already exists.")
             return callback.error(msg)
 
         msg = (_("Adding site '%(realm_master)s' with address "
-                    "'%(master_address)s' as realm master.")
+                    "'%(site_address)s' as realm master.")
                     % {"realm_master":realm_master,
-                    "master_address":master_address})
+                    "site_address":site_address})
         callback.send(msg)
 
         # Get node address from the host we are running on.
         import socket
         node_name = socket.gethostname()
 
         # Set our host type to "node" on realm init to prevent any issues (e.g.
         # CHECKSUM calculation in backend)
         if not config.host_data['type']:
             config.host_data['type'] = 'node'
 
         # Add our first site without initializing CA.
-        add_status = master_site.add(site_address=master_address,
+        add_status = master_site.add(site_fqdn=site_fqdn,
+                                    site_address=site_address,
                                     node_name=node_name,
                                     no_ca=True,
                                     no_node=True,
                                     verify_acls=False,
                                     id_ranges=id_ranges,
                                     callback=callback,
                                     **kwargs)
@@ -1282,15 +1259,17 @@
             return callback.error("Error creating master site.")
 
         # Write objects.
         cache.flush()
 
         config.set_site(name=master_site.name,
                         uuid=master_site.uuid,
-                        address=master_site.address)
+                        address=master_site.address,
+                        auth_fqdn=site_fqdn,
+                        mgmt_fqdn=site_fqdn)
         # Make this site our master.
         self.master = master_site.uuid
 
         if not self._write(callback=callback):
             msg = ("Error writing realm config")
             return callback.error(msg)
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/resolver.py` & `otpme-0.3.0a47/otpme/lib/classes/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/role.py` & `otpme-0.3.0a47/otpme/lib/classes/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/script.py` & `otpme-0.3.0a47/otpme/lib/classes/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/session.py` & `otpme-0.3.0a47/otpme/lib/classes/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/signing.py` & `otpme-0.3.0a47/otpme/lib/classes/signing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/site.py` & `otpme-0.3.0a47/otpme/lib/classes/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 read_acls = []
 write_acls = []
 
 read_value_acls = {
                     "view"      : [
                                 "trust",
                                 "address",
+                                "auth_fqdn",
+                                "mgmt_fqdn",
                                 "auth",
                                 "sync",
                                 "ca",
                                 "cert",
                                 "cert_key",
                                 "admin_role",
                                 "user_role",
@@ -80,14 +82,16 @@
                                 ],
                     "disable"   : [
                                 "auth",
                                 "sync",
                                 ],
                     "edit"      : [
                                 "address",
+                                "auth_fqdn",
+                                "mgmt_fqdn",
                                 "radius_cert",
                                 "radius_key",
                                 ],
                     "renew"     : [
                                 "cert",
                                 ],
                     "revoke"    : [
@@ -139,15 +143,15 @@
 
 commands = {
     'add'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
                     'method'            : 'add',
                     'args'              : ['node_name', 'site_address'],
-                    'oargs'             : ['dictionaries', 'id_ranges'],
+                    'oargs'             : ['site_fqdn', 'dictionaries', 'id_ranges'],
                     'job_type'          : 'process',
                     },
                 'exists'    : {
                     'method'            : 'add',
                     'args'              : ['node_name', 'site_address'],
                     'oargs'             : [
                                             'ca_country',
@@ -368,14 +372,32 @@
                 'exists'    : {
                     'method'            : 'change_address',
                     'args'              : ['address'],
                     'job_type'          : 'process',
                     },
                 },
             },
+    'auth_fqdn'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_auth_fqdn',
+                    'args'              : ['fqdn'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'mgmt_fqdn'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_mgmt_fqdn',
+                    'args'              : ['fqdn'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
     'dump_cert'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_cert',
                     'job_type'          : 'process',
                     },
                 },
@@ -680,15 +702,16 @@
     """ Register config stuff. """
     config.register_config_var("default_site_validity", int, 5475)
     config.register_config_var("default_site_key_len", int, 2048)
 
 def register_hooks():
     config.register_auth_on_action_hook("site", "add_unit")
     config.register_auth_on_action_hook("site", "change_address")
-    config.register_auth_on_action_hook("site", "change_fqdn")
+    config.register_auth_on_action_hook("site", "change_auth_fqdn")
+    config.register_auth_on_action_hook("site", "change_mgmt_fqdn")
     config.register_auth_on_action_hook("site", "enable_auth")
     config.register_auth_on_action_hook("site", "disable_auth")
     config.register_auth_on_action_hook("site", "enable_sync")
     config.register_auth_on_action_hook("site", "disable_sync")
     config.register_auth_on_action_hook("site", "renew_cert")
     config.register_auth_on_action_hook("site", "add_trust")
     config.register_auth_on_action_hook("site", "del_trust")
@@ -764,15 +787,16 @@
                                     path=path,
                                     **kwargs)
         self.ca = None
         self.admin_role_uuid = None
         self.user_role_uuid = None
         self.trusted_sites = []
 
-        self.fqdn = None
+        self.auth_fqdn = None
+        self.mgmt_fqdn = None
         self.address = None
         self.auth_enabled = True
         self.sync_enabled = True
         self.admin_token_uuid = None
         self._base_policies_post_methods = {}
         self.handle_cert_loading = True
         self.handle_key_loading = True
@@ -885,16 +909,22 @@
 
             'ADDRESS'                   : {
                                             'var_name'  : 'address',
                                             'type'      : str,
                                             'required'  : False,
                                         },
 
-            'FQDN'                      : {
-                                            'var_name'  : 'fqdn',
+            'MGMT_FQDN'                      : {
+                                            'var_name'  : 'mgmt_fqdn',
+                                            'type'      : str,
+                                            'required'  : False,
+                                        },
+
+            'AUTH_FQDN'                      : {
+                                            'var_name'  : 'auth_fqdn',
                                             'type'      : str,
                                             'required'  : False,
                                         },
 
             'AUTH_ENABLED'              : {
                                             'var_name'  : 'auth_enabled',
                                             'type'      : bool,
@@ -1038,34 +1068,56 @@
                 return callback.error()
         # FIXME: Check if we got a valid address
         self.address = address
         # Update index.
         self.update_index("address", self.address)
         return self._write(callback=callback)
 
-    @check_acls(['edit:fqdn'])
+    @check_acls(['edit:auth_fqdn'])
     @object_lock()
     @backend.transaction
-    def change_fqdn(self, fqdn, run_policies=True,
+    def change_auth_fqdn(self, fqdn, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
-        """ Change site FQDN. """
+        """ Change site auth FQDN. """
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
-                self.run_policies("change_fqdn",
+                self.run_policies("change_auth_fqdn",
                                 callback=callback,
                                 _caller=_caller)
             except Exception as e:
                 return callback.error()
         # FIXME: Check if we got a valid FQDN.
-        self.fqdn = fqdn
+        self.auth_fqdn = fqdn
         # Update index.
-        self.update_index("fqdn", self.fqdn)
+        self.update_index("auth_fqdn", self.auth_fqdn)
+        return self._write(callback=callback)
+
+    @check_acls(['edit:mgmt_fqdn'])
+    @object_lock()
+    @backend.transaction
+    def change_mgmt_fqdn(self, fqdn, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change site mgmt FQDN. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_mgmt_fqdn",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        # FIXME: Check if we got a valid FQDN.
+        self.mgmt_fqdn = fqdn
+        # Update index.
+        self.update_index("mgmt_fqdn", self.mgmt_fqdn)
         return self._write(callback=callback)
 
     @check_acls(['edit:radius_cert'])
     @object_lock()
     @backend.transaction
     def change_radius_cert(self, radius_cert, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
@@ -1641,16 +1693,17 @@
         if not add_result:
             return add_result
 
         config.site_init = False
         config.transactions_enabled = True
 
         # Update index.
-        self.update_index("fqdn", self.fqdn)
         self.update_index("address", self.address)
+        self.update_index("auth_fqdn", self.auth_fqdn)
+        self.update_index("mgmt_fqdn", self.mgmt_fqdn)
         self.update_index("auth_enabled", self.auth_enabled)
         self.update_index("sync_enabled", self.sync_enabled)
         callback.send("Site added successful.")
         return self._write(callback=callback)
 
     def add_per_site_objects(self, callback=default_callback):
         """ Add per site objects. """
@@ -1712,15 +1765,15 @@
             try:
                 x_object.add(verify_acls=False, callback=callback)
             except Exception as e:
                 msg = (_("Problem adding user: %s") % e)
                 raise OTPmeException(msg)
 
     @object_lock()
-    def _add(self, site_address, node_name, no_ca=False, no_node=False,
+    def _add(self, site_address, node_name, site_fqdn=None, no_ca=False, no_node=False,
         ca_country=None, ca_state=None, ca_locality=None, ca_organization=None,
         ca_ou=None, ca_email=None, ca_key_len=None, ca_valid=None,
         site_key_len=None, site_valid=None, dictionaries=None, no_dicts=False,
         id_ranges=None, verbose_level=0, callback=default_callback, **kwargs):
         """ Add a site. """
         if site_key_len is None:
             site_key_len = config.default_site_key_len
@@ -1734,29 +1787,26 @@
         if dictionaries is None:
             dictionaries = config.get_base_objects("dictionary")
 
         # Disable interactive policies (e.g. reauth).
         if not "interactive" in config.ignore_policy_tags:
             config.ignore_policy_tags.append("interactive")
 
-        # Check if we got a IP address or a FQDN. This check is done on the
-        # node and not on the client because the node needs to connect to the
-        # site.
-        site_fqdn = None
-        is_ip = net.is_ip(site_address)
-        if not is_ip:
-            # If its not a IP it must be the FQDN.
-            site_fqdn = site_address
+        if not site_address:
             # Try to get site address from DNS.
-            site_address = net.get_ip(site_fqdn)
+            result = net.query_dns(site_fqdn)
+            if len(result) > 1:
+                msg = "Found round-robin DNS. Please give floating IP."
+                return callback.error(msg)
+            site_address = result[0]
 
-        # We always need a site address as floating cluster IP.
+        # We always need a site address as floaging cluster IP.
         if not site_address:
             msg = ("Unable to resolve: %s" % site_fqdn)
-            return callback.error(msg)
+            raise OTPmeException(msg)
 
         if not config.realm_init:
             result = backend.search(object_type="host",
                                     attribute="name",
                                     value=node_name,
                                     realm=self.realm,
                                     site=self.name)
@@ -1769,25 +1819,26 @@
                                     realm=self.realm,
                                     site=self.name)
             if result:
                 msg = (_("Node already exists: %s") % node_name)
                 return callback.error(msg)
 
         # Set site FQDN.
-        self.fqdn = site_fqdn
+        self.auth_fqdn = site_fqdn
+        self.mgmt_fqdn = site_fqdn
 
         # Set site address.
         self.address = site_address
 
-        # Write site onfig before adding base units and policies.
-        if not self._write(callback=callback):
-            return callback.error("Error writing site config.")
-
         # Set config site.
-        config.set_site(name=self.name, uuid=self.uuid, address=self.address)
+        config.set_site(name=self.name,
+                        uuid=self.uuid,
+                        address=self.address,
+                        auth_fqdn=self.auth_fqdn,
+                        mgmt_fqdn=self.mgmt_fqdn)
 
         # Add site object BEFORE creating base objects (e.g. site gets default
         # policies).
         OTPmeObject.add(self, enabled=False,
                         verbose_level=verbose_level,
                         callback=callback,
                         **kwargs)
@@ -2446,15 +2497,16 @@
         return self._write(callback=callback)
 
     # zzzzzzzzzzzzzzzzzzzzz
     # FIXME: make sure we remove all references before deleting a site
     @check_acls(['delete:object'])
     @object_lock()
     @backend.transaction
-    def delete(self, force=False, run_policies=True, verbose_level=0,
+    def delete(self, force=False, verify_acls=True,
+        run_policies=True, verbose_level=0,
         callback=default_callback, _caller="API", **kwargs):
         """ Delete site. """
         # We should never delete ourselves ;)
         if config.site == self.name:
             return callback.error("Cannot delete own site!")
 
         # Get parent object to check ACLs.
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/ssh_agent.py` & `otpme-0.3.0a47/otpme/lib/classes/ssh_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/token.py` & `otpme-0.3.0a47/otpme/lib/classes/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,19 +58,24 @@
                         "token_type",
                         "accessgroups",
                         "groups",
                         "roles",
                         "pin",
                         "pin_status",
                         "used_otp_salt",
+                        "auto_disable",
                         "auth_script",
                         ],
             }
 
-write_value_acls = {}
+write_value_acls = {
+                    "edit"  : [
+                                "auto_disable",
+                            ],
+                }
 
 default_acls = []
 
 recursive_default_acls = []
 
 commands = {
     'add'   : {
@@ -160,14 +165,23 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'disable',
                     'job_type'          : 'process',
                     },
                 },
             },
+    'auto_disable'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_auto_disable',
+                    'args'              : ['auto_disable'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
     'rename'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'rename',
                     'args'              : ['new_name'],
                     'job_type'          : 'process',
                     },
```

### Comparing `otpme-0.3.0a46/otpme/lib/classes/unit.py` & `otpme-0.3.0a47/otpme/lib/classes/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/classes/user.py` & `otpme-0.3.0a47/otpme/lib/classes/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                         ],
             "view"      : [
                         "token",
                         "group",
                         "public_key",
                         "failcount",
                         "session",
+                        "auto_disable",
                         ],
         }
 
 write_value_acls = {
                     "add"       : [
                                 "token",
                                 ],
@@ -104,14 +105,15 @@
                                 "private_key",
                                 "private_key_pass",
                                 "public_key",
                                 "key_script",
                                 "auth_script",
                                 "agent_script",
                                 "login_script",
+                                "auto_disable",
                                 ],
                     "enable"    : [
                                 "autosign",
                                 "auth_script",
                                 "login_script",
                                 "token"
                                 ],
@@ -218,14 +220,23 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'disable',
                     'job_type'          : 'process',
                     },
                 },
             },
+    'auto_disable'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_auto_disable',
+                    'args'              : ['auto_disable'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
     'rename'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'rename',
                     'args'              : ['new_name'],
                     'job_type'          : 'process',
                     },
@@ -4075,14 +4086,29 @@
         oid_string = "\tOID:\t\t\t%s\n" % self.oid.full_oid
         lines.append(oid_string)
         if not self.enabled:
             lines.append("\tstatus:\t\t\tDisabled\n")
         else:
             lines.append("\tstatus:\t\t\tActive\n")
 
+        if self.verify_acl("view:auto_disable") \
+        or self.verify_acl("edit:auto_disable"):
+            if self.auto_disable_time == 0:
+                auto_disable = "\tauto-disable:\t\tdisabled\n"
+            else:
+                auto_disable = "\tauto-disable:\t\t%s\n" % self.auto_disable_time
+            lines.append(auto_disable)
+            unused_disable = "\tunused-disable:\t\t%s\n" % self.unused_disable
+            lines.append(unused_disable)
+        else:
+            auto_disable = "\tauto-disable:\t\t\tPermission denied\n"
+            lines.append(auto_disable)
+            unused_disable = "\tunused-disable:\t\t\tPermission denied\n"
+            lines.append(unused_disable)
+
         lines.append("\trealm:\t\t\t%s\n" % self.realm)
         lines.append("\tsite:\t\t\t%s\n" % self.site)
         if self.unit:
             lines.append("\tunit:\t\t\t%s\n" % self.unit)
         else:
             lines.append("\tunit:\t\t\t\n")
```

### Comparing `otpme-0.3.0a46/otpme/lib/cli/__init__.py` & `otpme-0.3.0a47/otpme/lib/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 from otpme.lib import config
 #from otpme.lib.messages import message
 from otpme.lib.messages import error_message
 from otpme.lib.cache import object_list_cache
 
 from otpme.lib.exceptions import *
 
-try:
-    default_callback = config.get_callback()
-except:
-    default_callback = None
+default_callback = config.get_callback()
 
 object_register = {}
 
 REGISTER_BEFORE = []
 REGISTER_AFTER = []
 
 # Protocol modules to register.
```

### Comparing `otpme-0.3.0a46/otpme/lib/cli/accessgroup.py` & `otpme-0.3.0a47/otpme/lib/cli/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/ca.py` & `otpme-0.3.0a47/otpme/lib/cli/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/client.py` & `otpme-0.3.0a47/otpme/lib/cli/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/dictionary.py` & `otpme-0.3.0a47/otpme/lib/cli/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/group.py` & `otpme-0.3.0a47/otpme/lib/cli/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/host.py` & `otpme-0.3.0a47/otpme/lib/cli/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/node.py` & `otpme-0.3.0a47/otpme/lib/cli/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/policy.py` & `otpme-0.3.0a47/otpme/lib/cli/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/realm.py` & `otpme-0.3.0a47/otpme/lib/cli/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/resolver.py` & `otpme-0.3.0a47/otpme/lib/cli/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/role.py` & `otpme-0.3.0a47/otpme/lib/cli/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/script.py` & `otpme-0.3.0a47/otpme/lib/cli/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/site.py` & `otpme-0.3.0a47/otpme/lib/cli/site.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,28 @@
 table_headers = [
                 "site",
                 "status",
                 "auth",
                 "sync",
                 "trusts",
                 "address",
+                "auth_fqdn",
+                "mgmt_fqdn",
                 "policies",
                 "description",
                 ]
 
 REGISTER_BEFORE = []
 REGISTER_AFTER = ["otpme.lib.filetools"]
 
 def register():
     return_attributes = [
                         'name',
-                        'fqdn',
+                        'auth_fqdn',
+                        'mgmt_fqdn',
                         'address',
                         'enabled',
                         'description',
                         'trusted_site',
                         'auth_enabled',
                         'sync_enabled',
                         'acl_inheritance_enabled',
@@ -65,15 +68,22 @@
 def row_getter(realm, site, site_order, site_data, acls,
     output_fields=[], acl_checker=None, **kwargs):
     """ Build table rows for sites. """
     _result = []
     for site_uuid in site_order:
         row = []
         site_name = site_data[site_uuid]['name']
-        site_fqdn = site_data[site_uuid]['fqdn'][0]
+        try:
+            site_auth_fqdn = site_data[site_uuid]['auth_fqdn'][0]
+        except KeyError:
+            site_auth_fqdn = "Unknown"
+        try:
+            site_mgmt_fqdn = site_data[site_uuid]['mgmt_fqdn'][0]
+        except KeyError:
+            site_mgmt_fqdn = "Unknown"
         site_address = site_data[site_uuid]['address'][0]
         try:
             enabled = site_data[site_uuid]['enabled'][0]
         except:
             enabled = False
         try:
             trusted_sites = site_data[site_uuid]['trusted_site']
@@ -149,19 +159,29 @@
                     x_oid = backend.get_oid(x, instance=True)
                     _trusted_sites.append(x_oid.name)
             row.append(",".join(_trusted_sites))
         # Addresses.
         if "address" in output_fields:
             if check_acl("view:address") \
             or check_acl("edit:address"):
-                if site_fqdn:
-                    site_address = "%s (%s)" % (site_address, site_fqdn)
                 row.append(site_address)
             else:
                 row.append("-")
+        if "auth_fqdn" in output_fields:
+            if check_acl("view:auth_fqdn") \
+            or check_acl("edit:auth_fqdn"):
+                row.append(site_auth_fqdn)
+            else:
+                row.append("-")
+        if "mgmt_fqdn" in output_fields:
+            if check_acl("view:mgmt_fqdn") \
+            or check_acl("edit:mgmt_fqdn"):
+                row.append(site_mgmt_fqdn)
+            else:
+                row.append("-")
         # Policies.
         if "policies" in output_fields:
             if check_acl("view:policy") \
             or check_acl("add:policy") \
             or check_acl("remove:policy"):
                 policies_string = get_policies_string(object_type="site",
                                                     object_uuid=site_uuid)
```

### Comparing `otpme-0.3.0a46/otpme/lib/cli/token.py` & `otpme-0.3.0a47/otpme/lib/cli/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/unit.py` & `otpme-0.3.0a47/otpme/lib/cli/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/cli/user.py` & `otpme-0.3.0a47/otpme/lib/cli/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/compgen.py` & `otpme-0.3.0a47/otpme/lib/compgen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/compression/__init__.py` & `otpme-0.3.0a47/otpme/lib/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/compression/base.py` & `otpme-0.3.0a47/otpme/lib/compression/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/__init__.py` & `otpme-0.3.0a47/otpme/lib/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/authd.py` & `otpme-0.3.0a47/otpme/lib/daemon/authd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/clusterd.py` & `otpme-0.3.0a47/otpme/lib/daemon/clusterd.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,32 +90,34 @@
 
 def get_lock_event(timestamp):
     lock_event_name = "/%s" % timestamp
     lock_event = multiprocessing.Event(lock_event_name)
     return lock_event
 
 def check_cluster_status():
-    if not config.cluster_status:
-        msg = "Cluster not ready."
-        raise OTPmeException(msg)
     if config.master_failover:
         msg = "Ongoing master failover."
         raise OTPmeException(msg)
+    if not config.cluster_status:
+        msg = "Cluster not ready."
+        raise OTPmeException(msg)
 
 def cluster_nsscache_sync():
     if config.use_api:
         return
     if config.one_node_setup:
         return
     multiprocessing.nsscache_sync_queue.clear()
     sync_time = time.time()
     try:
         multiprocessing.nsscache_sync_queue[sync_time] = []
     except ValueError:
         pass
+    if not multiprocessing.cluster_event:
+        return
     multiprocessing.cluster_event.set()
 
 def cluster_radius_reload():
     if config.use_api:
         return
     try:
         freeradius_reload()
@@ -128,14 +130,16 @@
         return
     multiprocessing.radius_reload_queue.clear()
     reload_time = time.time() + 5
     try:
         multiprocessing.radius_reload_queue[reload_time] = []
     except ValueError:
         pass
+    if not multiprocessing.cluster_event:
+        return
     multiprocessing.cluster_event.set()
 
 def cluster_sync_object(object_uuid, object_id, action, object_config=None,
     new_object_id=None, last_modified=None, checksum=None, wait_for_write=True):
     if config.one_node_setup:
         return
     handle_events = True
@@ -1562,25 +1566,22 @@
                 continue
             try:
                 current_master_node = multiprocessing.master_node['master']
             except KeyError:
                 current_master_node = None
             if current_master_node == new_master_node:
                 time.sleep(quorum_check_interval)
-                #config.master_failover = False
-                #config.cluster_status = True
                 continue
 
             try:
                 self.switch_master_node(current_master_node, new_master_node)
             except Exception as e:
                 msg = "Failed to switch master node: %s" % e
                 self.logger.critical(msg)
             config.master_failover = False
-            #config.cluster_status = True
             time.sleep(quorum_check_interval)
 
     def handle_two_node_setup(self):
         # Two node setups require some special handling if second node is down.
         if not config.two_node_setup:
             return
         if len(multiprocessing.member_nodes) > 0:
@@ -1927,16 +1928,14 @@
         if self.online_nodes != sorted(multiprocessing.online_nodes.keys()):
             processed_journal_entries.clear()
             self.online_nodes = sorted(multiprocessing.online_nodes.keys())
         if len(node_checksums) > 102400:
             node_checksums = node_checksums[51200:]
         if len(processed_journal_entries) > 102400:
             processed_journal_entries = processed_journal_entries[51200:]
-        if not config.cluster_status:
-            return True
         uuids_to_process = []
         entries_to_process = []
         cluster_journal_dirs = self.get_cluster_journal()
         for journal_entry_dir in cluster_journal_dirs:
             if not config.cluster_status:
                 return True
             if self.node_conn is None:
@@ -1966,16 +1965,14 @@
                 if cluster_journal_entry.action != "delete":
                     uuids_to_process.append(cluster_journal_entry.object_uuid)
             except ObjectDeleted:
                 pass
 
         written_entries = []
         unsync_status_set = False
-        objects_sync_started = True
-        objects_sync_successful = False
         for entry_timestamp in entries_to_process:
             if not config.cluster_status:
                 return True
             self.handle_two_node_setup()
             cluster_journal_entry = ClusterJournalEntry(timestamp=entry_timestamp)
             try:
                 object_id = cluster_journal_entry.object_id
@@ -2019,16 +2016,14 @@
                         if self.check_member_nodes(cluster_journal_entry):
                             # Check if object was written to all online nodes.
                             self.check_online_nodes(cluster_journal_entry)
                         continue
 
                 # Mark node as out of sync (tree objects).
                 if object_id.object_type in config.tree_object_types:
-                    objects_sync_started = True
-                    objects_sync_successful = True
                     if not unsync_status_set:
                         unsync_status_set = True
                         self.unset_node_sync(node_name)
                 # Write object to peer.
                 if action == "write":
                     try:
                         last_used = backend.get_last_used(object_id.realm,
@@ -2053,15 +2048,14 @@
                     except Exception as e:
                         self.node_disconnect(node_name)
                         msg = ("Error sending object: %s: %s: %s"
                                 % (node_name, object_id, e))
                         self.logger.warning(msg)
                         return True
                     if write_status != "done":
-                        objects_sync_successful = False
                         continue
                     written_entries.append(object_uuid)
                     try:
                         uuids_to_process.remove(object_uuid)
                     except ValueError:
                         pass
                     msg = ("Written object to node: %s: %s (%s)"
@@ -2086,15 +2080,14 @@
                     except Exception as e:
                         self.node_disconnect(node_name)
                         msg = ("Failed to rename object: %s: %s: %s"
                                 % (node_name, object_id, e))
                         self.logger.warning(msg)
                         return True
                     if rename_status != "done":
-                        objects_sync_successful = False
                         continue
                     written_entries.append(object_uuid)
                     try:
                         uuids_to_process.remove(object_uuid)
                     except ValueError:
                         pass
                     msg = ("Renamed object on node: %s: %s: %s"
@@ -2115,15 +2108,14 @@
                         return True
                     except Exception as e:
                         self.node_disconnect(node_name)
                         msg = "Failed to delete object: %s: %s" % (object_id, e)
                         self.logger.warning(msg)
                         return True
                     if del_status != "done":
-                        objects_sync_successful = False
                         continue
                     msg = ("Deleted object on node: %s: %s"
                             % (node_name, object_id))
                     self.logger.debug(msg)
                     node_checksums.append(object_checksum)
                     cluster_journal_entry.add_node(node_name)
                     processed_journal_entries.append(cluster_journal_entry.timestamp)
@@ -2132,15 +2124,15 @@
                 if self.check_member_nodes(cluster_journal_entry):
                     # Check if object was written to all online nodes.
                     self.check_online_nodes(cluster_journal_entry)
             except ObjectDeleted:
                 pass
 
         if config.master_node:
-            if objects_sync_started and objects_sync_successful:
+            if not config.master_failover:
                 sync_time = time.time()
                 config.touch_node_sync_file(sync_time)
                 # Mark node as in sync (tree objects).
                 self.set_node_sync(node_name, sync_time-300)
 
         journal_entries = self.get_cluster_journal()
         if journal_entries:
```

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/controld.py` & `otpme-0.3.0a47/otpme/lib/daemon/controld.py`

 * *Files 0% similar despite different names*

```diff
@@ -791,15 +791,15 @@
                 self.comm_handler.send(sender, command="daemons_ready")
             elif command == "send_keepalive":
                 self.ensure_daemons()
             elif command == "configure_floating_ip":
                 try:
                     self.configure_floating_ip(config.site_address)
                 except Exception as e:
-                    msg = "Failed to configure floating IP."
+                    msg = "Failed to configure floating IP: %s" % e
                     self.logger.critical(msg)
                     config.raise_exception()
             elif command == "deconfigure_floating_ip":
                 self.deconfigure_floating_ip()
                 #self.need_restart = True
             elif command == "reload":
                 self._reload()
```

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/hostd.py` & `otpme-0.3.0a47/otpme/lib/daemon/hostd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/joind.py` & `otpme-0.3.0a47/otpme/lib/daemon/joind.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/ldapd.py` & `otpme-0.3.0a47/otpme/lib/daemon/ldapd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/mgmtd.py` & `otpme-0.3.0a47/otpme/lib/daemon/mgmtd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/otpme_daemon.py` & `otpme-0.3.0a47/otpme/lib/daemon/otpme_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/scriptd.py` & `otpme-0.3.0a47/otpme/lib/daemon/scriptd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/syncd.py` & `otpme-0.3.0a47/otpme/lib/daemon/syncd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/daemon/unix_daemon.py` & `otpme-0.3.0a47/otpme/lib/daemon/unix_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/debug.py` & `otpme-0.3.0a47/otpme/lib/debug.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/doc.py` & `otpme-0.3.0a47/otpme/lib/doc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encoding/base.py` & `otpme-0.3.0a47/otpme/lib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/__init__.py` & `otpme-0.3.0a47/otpme/lib/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/aes.py` & `otpme-0.3.0a47/otpme/lib/encryption/aes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/aes_cfb.py` & `otpme-0.3.0a47/otpme/lib/encryption/aes_cfb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/argon2.py` & `otpme-0.3.0a47/otpme/lib/encryption/argon2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/asymmetric_key_handler.py` & `otpme-0.3.0a47/otpme/lib/encryption/asymmetric_key_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/ec.py` & `otpme-0.3.0a47/otpme/lib/encryption/ec.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/fernet.py` & `otpme-0.3.0a47/otpme/lib/encryption/fernet.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/hkdf.py` & `otpme-0.3.0a47/otpme/lib/encryption/hkdf.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/pbkdf2.py` & `otpme-0.3.0a47/otpme/lib/encryption/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/encryption/rsa.py` & `otpme-0.3.0a47/otpme/lib/encryption/rsa.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/exceptions.py` & `otpme-0.3.0a47/otpme/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/extensions/base/base.py` & `otpme-0.3.0a47/otpme/lib/extensions/base/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/extensions/ldif_handler.py` & `otpme-0.3.0a47/otpme/lib/extensions/ldif_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/extensions/posix/posix.py` & `otpme-0.3.0a47/otpme/lib/extensions/posix/posix.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/extensions/utils.py` & `otpme-0.3.0a47/otpme/lib/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/filetools.py` & `otpme-0.3.0a47/otpme/lib/filetools.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/freeradius/__init__.py` & `otpme-0.3.0a47/otpme/lib/freeradius/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/freeradius/otpme.py` & `otpme-0.3.0a47/otpme/lib/freeradius/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/freeradius/radiusd.py` & `otpme-0.3.0a47/otpme/lib/freeradius/radiusd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/freeradius/radiusd_test.py` & `otpme-0.3.0a47/otpme/lib/freeradius/radiusd_test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/gpg/utils.py` & `otpme-0.3.0a47/otpme/lib/gpg/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/__init__.py` & `otpme-0.3.0a47/otpme/lib/help/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/accessgroup.py` & `otpme-0.3.0a47/otpme/lib/help/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/agent.py` & `otpme-0.3.0a47/otpme/lib/help/agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/auth.py` & `otpme-0.3.0a47/otpme/lib/help/auth.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/ca.py` & `otpme-0.3.0a47/otpme/lib/help/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/client.py` & `otpme-0.3.0a47/otpme/lib/help/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/cluster.py` & `otpme-0.3.0a47/otpme/lib/help/cluster.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/controld.py` & `otpme-0.3.0a47/otpme/lib/help/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/dictionary.py` & `otpme-0.3.0a47/otpme/lib/help/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/get_authorized_keys.py` & `otpme-0.3.0a47/otpme/lib/help/get_authorized_keys.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/group.py` & `otpme-0.3.0a47/otpme/lib/help/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/host.py` & `otpme-0.3.0a47/otpme/lib/help/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/node.py` & `otpme-0.3.0a47/otpme/lib/help/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/pinentry.py` & `otpme-0.3.0a47/otpme/lib/help/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/__init__.py` & `otpme-0.3.0a47/otpme/lib/help/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/authonaction.py` & `otpme-0.3.0a47/otpme/lib/help/policy/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/autodisable.py` & `otpme-0.3.0a47/otpme/lib/help/policy/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/defaultgroups.py` & `otpme-0.3.0a47/otpme/lib/help/policy/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/defaultpolicies.py` & `otpme-0.3.0a47/otpme/lib/help/policy/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/defaultroles.py` & `otpme-0.3.0a47/otpme/lib/help/policy/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/defaultunits.py` & `otpme-0.3.0a47/otpme/lib/help/policy/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/forcetoken.py` & `otpme-0.3.0a47/otpme/lib/help/policy/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/idrange.py` & `otpme-0.3.0a47/otpme/lib/help/policy/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/logintimes.py` & `otpme-0.3.0a47/otpme/lib/help/policy/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/objecttemplates.py` & `otpme-0.3.0a47/otpme/lib/help/policy/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/password.py` & `otpme-0.3.0a47/otpme/lib/help/policy/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/policy/tokenacls.py` & `otpme-0.3.0a47/otpme/lib/help/policy/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/realm.py` & `otpme-0.3.0a47/otpme/lib/help/realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 cmd_help = {
     '_need_command'             : True,
     '_include_global_opts'      : True,
     '_usage_help'               : "Usage: otpme-realm {command} [realm]",
 
     'init'      : {
-                    '_cmd_usage_help' : 'Usage: otpme-realm init {realm} {site} {address}',
-                    'cmd'   :   '--country :ca_country: --state :ca_state: --locality :ca_locality: --organization :ca_organization: --ou :ca_ou: --email :ca_email: --ca-valid :ca_valid: --ca-key-len :ca_key_len: --site-valid :site_valid: --site-key-len :site_key_len: --node-valid :node_valid: --node-key-len :node_key_len: --no-dicts :no_dicts=True: --dicts ::[dictionaries]:: --id-ranges ::id_ranges:: <|object|> <realm_master> <master_address>',
+                    '_cmd_usage_help' : 'Usage: otpme-realm init {realm} {site} {fqdn} [address]',
+                    'cmd'   :   '--country :ca_country: --state :ca_state: --locality :ca_locality: --organization :ca_organization: --ou :ca_ou: --email :ca_email: --ca-valid :ca_valid: --ca-key-len :ca_key_len: --site-valid :site_valid: --site-key-len :site_key_len: --node-valid :node_valid: --node-key-len :node_key_len: --no-dicts :no_dicts=True: --dicts ::[dictionaries]:: --id-ranges ::id_ranges:: <|object|> <realm_master> <site_fqdn> [site_address]',
                     '_help' :   {
                                     'cmd'                               : 'init realm',
                                     '--ca-valid'                        : 'CA certificates validity in days.',
                                     '--ca-key-len'                      : 'Key length for CA certificates in bits.',
                                     '--country'                         : 'Set CA certificate <country> field.',
                                     '--state'                           : 'Set CA certificate <state> field.',
                                     '--locality'                        : 'Set CA certificate <locality> field.',
```

### Comparing `otpme-0.3.0a46/otpme/lib/help/register.py` & `otpme-0.3.0a47/otpme/lib/help/register.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/resolver/__init__.py` & `otpme-0.3.0a47/otpme/lib/help/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/resolver/ldap.py` & `otpme-0.3.0a47/otpme/lib/help/resolver/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/role.py` & `otpme-0.3.0a47/otpme/lib/help/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/script.py` & `otpme-0.3.0a47/otpme/lib/help/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/session.py` & `otpme-0.3.0a47/otpme/lib/help/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/site.py` & `otpme-0.3.0a47/otpme/lib/help/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
                     'cmd'   :   '[|object|]',
                     '_help' :   {
                                     'cmd'                   : 'show sites config parameters',
                                 },
                 },
 
     'add'    : {
-                    '_cmd_usage_help' : 'Usage: otpme-site add {site} {node_name} {site_address}',
-                    'cmd'   :   '--country :ca_country: --state :ca_state: --locality :ca_locality: --organization :ca_organization: --ou :ca_ou: --email :ca_email: --ca-valid :ca_valid: --ca-key-len :ca_key_len: --site-valid :site_valid: --site-key-len :site_key_len: --node-valid :node_valid: --node-key-len :node_key_len: --no-dicts :no_dicts=True: --dicts :[dictionaries]: --id-ranges ::id_ranges:: <|object|> <node_name> <site_address>',
+                    '_cmd_usage_help' : 'Usage: otpme-site add {site} {node_name} {site_fqdn} [site_address]',
+                    'cmd'   :   '--country :ca_country: --state :ca_state: --locality :ca_locality: --organization :ca_organization: --ou :ca_ou: --email :ca_email: --ca-valid :ca_valid: --ca-key-len :ca_key_len: --site-valid :site_valid: --site-key-len :site_key_len: --node-valid :node_valid: --node-key-len :node_key_len: --no-dicts :no_dicts=True: --dicts :[dictionaries]: --id-ranges ::id_ranges:: <|object|> <node_name> <site_fqdn> [site_address]',
                     '_help' :   {
                                     'cmd'                               : 'Add new site.',
                                     '--ca-valid'                        : 'CA certificates validity in days.',
                                     '--ca-key-len'                      : 'Key length for CA certificates in bits.',
                                     '--country'                         : 'Set CA certificate <country> field.',
                                     '--state'                           : 'Set CA certificate <state> field.',
                                     '--locality'                        : 'Set CA certificate <locality> field.',
@@ -407,14 +407,30 @@
                     '_cmd_usage_help' : 'Usage: otpme-site address {site} [ip_address]',
                     'cmd'   :   '<|object|> [address]',
                     '_help' :   {
                                     'cmd'                   : 'change sites IP address',
                                 },
                 },
 
+    'auth_fqdn'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-site auth_fqdn {site} [fqdn]',
+                    'cmd'   :   '<|object|> [fqdn]',
+                    '_help' :   {
+                                    'cmd'                   : 'Change sites auth fqdn.',
+                                },
+                },
+
+    'mgmt_fqdn'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-site mgmt_fqdn {site} [fqdn]',
+                    'cmd'   :   '<|object|> [fqdn]',
+                    '_help' :   {
+                                    'cmd'                   : 'Change sites mgmt fqdn.',
+                                },
+                },
+
     'enable_auth'    : {
                     '_cmd_usage_help' : 'Usage: otpme-site enable_auth {site}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'enable authentication with site',
                                 },
                 },
```

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/__init__.py` & `otpme-0.3.0a47/otpme/lib/help/token/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,23 @@
                     '_cmd_usage_help' : 'Usage: otpme-token disable {token}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'disable token',
                                 },
                 },
 
+    'auto_disable'          : {
+                    '_cmd_usage_help' : 'Usage: otpme-token auto_disable {token} {time}',
+                    'cmd'   :   '<|object|> <auto_disable> -u :unused=True:',
+                    '_help' :   {
+                                    'cmd'                   : 'Change auto disable value (e.g "1d" or "09:53 13.06.2023").',
+                                    '-u'                    : 'Disable object if it was unused for the given time.',
+                                },
+                },
+
     'rename'    : {
                     '_cmd_usage_help' : 'Usage: otpme-token rename {token} {new_name}',
                     'cmd'   :   '<|object|> <new_name>',
                     '_help' :   {
                                     'cmd'                   : 'rename token',
                                 },
                 },
```

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/fido2.py` & `otpme-0.3.0a47/otpme/lib/help/token/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/hotp.py` & `otpme-0.3.0a47/otpme/lib/help/token/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/motp.py` & `otpme-0.3.0a47/otpme/lib/help/token/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/otp_push.py` & `otpme-0.3.0a47/otpme/lib/help/token/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/otpme.py` & `otpme-0.3.0a47/otpme/lib/help/token/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/password.py` & `otpme-0.3.0a47/otpme/lib/help/token/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/ssh.py` & `otpme-0.3.0a47/otpme/lib/help/token/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/totp.py` & `otpme-0.3.0a47/otpme/lib/help/token/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/yubikey_hmac.py` & `otpme-0.3.0a47/otpme/lib/help/token/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/token/yubikey_hotp.py` & `otpme-0.3.0a47/otpme/lib/help/token/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/tool.py` & `otpme-0.3.0a47/otpme/lib/help/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,17 +361,19 @@
                                     '--keep-cert'           : 'Do not revoke host certficiate when leaving.',
                                     '--keep-auth-key'       : 'Do not revoke host auth key when leaving.',
                                 },
                 },
 
 
     'login'    : {
-                    '_cmd_usage_help' : 'Usage: otpme-tool login [username]',
+                    '_cmd_usage_help' : 'Usage: otpme-tool login --node {node} [username]',
+                    'cmd'   :   '--node :node:',
                     '_help' :   {
                                     'cmd'                   : 'login to OTPme realm',
+                                    '--node <node>'         : 'Send login request to given node.',
                                 },
                 },
 
     'logout'    : {
                     '_cmd_usage_help' : 'Usage: otpme-tool logout',
                     '_help' :   {
                                     'cmd'                   : 'logout from OTPme realm',
```

### Comparing `otpme-0.3.0a46/otpme/lib/help/unit.py` & `otpme-0.3.0a47/otpme/lib/help/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/help/user.py` & `otpme-0.3.0a47/otpme/lib/help/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,23 @@
                     '_cmd_usage_help' : 'Usage: otpme-user disable {user}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'disable user',
                                 },
                 },
 
+    'auto_disable'          : {
+                    '_cmd_usage_help' : 'Usage: otpme-user auto_disable {user} {time}',
+                    'cmd'   :   '<|object|> <auto_disable> -u :unused=True:',
+                    '_help' :   {
+                                    'cmd'                   : 'Change auto disable value (e.g "1d" or "09:53 13.06.2023").',
+                                    '-u'                    : 'Disable object if it was unused for the given time.',
+                                },
+                },
+
     'rename'    : {
                     '_cmd_usage_help' : 'Usage: otpme-user rename {user} {new_name}',
                     'cmd'   :   '<|object|> <new_name>',
                     '_help' :   {
                                     'cmd'                   : 'rename user',
                                 },
                 },
```

### Comparing `otpme-0.3.0a46/otpme/lib/host.py` & `otpme-0.3.0a47/otpme/lib/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/index/mysql.py` & `otpme-0.3.0a47/otpme/lib/index/mysql.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/index/postgres.py` & `otpme-0.3.0a47/otpme/lib/index/postgres.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/index/sqlite3.py` & `otpme-0.3.0a47/otpme/lib/index/sqlite3.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/job/callback.py` & `otpme-0.3.0a47/otpme/lib/job/callback.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/job/otpme_job.py` & `otpme-0.3.0a47/otpme/lib/job/otpme_job.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/join.py` & `otpme-0.3.0a47/otpme/lib/join.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,16 +339,16 @@
         callback = JobCallback(api_mode=True)
         self._my_site.add_base_objects(callback=callback)
         self._my_site.add_base_groups(callback=callback)
         self._my_site.add_per_site_objects(callback=callback)
 
         # Finish node join and create node cert.
         self._my_host.join_realm(verify_acls=False,
-                            cert_req=host_cert_req,
-                            finish=True)
+                                cert_req=host_cert_req,
+                                finish=True)
 
         # Reload CA after node cert generation.
         self._my_site_ca = backend.get_object(object_type="ca", uuid=self._my_site.ca)
 
         logger.debug("Sending CRL to joind...")
         # Build command.
         #command_args = {}
@@ -375,14 +375,18 @@
                             command_args,
                             request,
                             **conn_kwargs)
         if not status:
             msg = (_("Sending CRL failed: %s") % join_reply)
             raise OTPmeException(msg)
 
+        # Make sure master node is ready.
+        config.touch_node_sync_file()
+
+        return self._my_host.cert
 
     def process_objects(self, join_reply):
         """ Add base objects etc.. """
         # Get base objects from reply.
         object_configs = join_reply['object_configs']
 
         add_list = {}
@@ -672,16 +676,17 @@
         try:
             host_key = config.host_data['key']
         except Exception as e:
             host_key = None
 
         host_cert_req = None
         # Generate new host cert CSR and key if needed.
-        if not host_cert or not host_key:
-            host_cert_req, host_key = self.gen_host_cert_req(key_len=host_key_len)
+        if not master_node_join:
+            if not host_cert or not host_key:
+                host_cert_req, host_key = self.gen_host_cert_req(key_len=host_key_len)
 
         # Generate host auth key.
         host_private_key = self._my_host.gen_auth_key()
 
         # Make sure changes get committed.
         self._my_host._cache()
         # Save changes. This must be done before sending final join request
@@ -697,20 +702,21 @@
                                     host_cert=host_cert,
                                     jotp=finish_jotp)
 
         # Get join message.
         join_message = join_reply['message']
 
         if master_node_join:
-            self.handle_master_node_stuff(join_reply,
-                                        site_ca_key,
-                                        host_cert_req,
-                                        password, jotp,
-                                        conn_kwargs)
-            host_cert = self._my_host.cert
+            node_cert_req, host_key = self.gen_host_cert_req(key_len=host_key_len)
+            host_cert = self.handle_master_node_stuff(join_reply,
+                                                        site_ca_key,
+                                                        node_cert_req,
+                                                        password, jotp,
+                                                        conn_kwargs)
+
         elif host_cert_req:
             host_cert = join_reply['host_cert']
             self._my_host.cert = host_cert
 
         self._my_host.enable(force=True,
                             verify_acls=False)
         self._my_host._write()
```

### Comparing `otpme-0.3.0a46/otpme/lib/json.py` & `otpme-0.3.0a47/otpme/lib/json.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/jwt.py` & `otpme-0.3.0a47/otpme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/ldap/client.py` & `otpme-0.3.0a47/otpme/lib/ldap/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/ldap/schema.py` & `otpme-0.3.0a47/otpme/lib/ldap/schema.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/ldap/server.py` & `otpme-0.3.0a47/otpme/lib/ldap/server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/locking.py` & `otpme-0.3.0a47/otpme/lib/locking.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/log.py` & `otpme-0.3.0a47/otpme/lib/log.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/messages.py` & `otpme-0.3.0a47/otpme/lib/messages.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/mschap.py` & `otpme-0.3.0a47/otpme/lib/mschap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/mschap_util.py` & `otpme-0.3.0a47/otpme/lib/mschap_util.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/multiprocessing.py` & `otpme-0.3.0a47/otpme/lib/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/net.py` & `otpme-0.3.0a47/otpme/lib/net.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,31 @@
     pass
 
 from otpme.lib import arp
 from otpme.lib import config
 
 from otpme.lib.exceptions import *
 
-logger = config.logger
-
-
 def is_ip(ip):
     """ Check if given IP is valid. """
     try:
         socket.inet_aton(ip)
         return True
     except:
         return False
 
 def get_ip(fqdn):
     """ Resolve given FQDN via gethostbyname(). """
-    logger.debug("Trying to resolve: %s" % fqdn)
+    config.logger.debug("Trying to resolve: %s" % fqdn)
     try:
         ip = socket.gethostbyname(fqdn)
     except:
-        logger.debug("Unable to resolve: %s")
+        config.logger.debug("Unable to resolve: %s")
         return False
-    logger.debug("Got IP from gethostbyname(): %s" % ip)
+    config.logger.debug("Got IP from gethostbyname(): %s" % ip)
     return ip
 
 def get_host_fqdn():
     """ Get host DNS FQDN. """
     # Try to get host FQDN.
     try:
         host_fqdn = socket.getfqdn()
@@ -82,25 +79,25 @@
                     'realm' : realm_record,
                     'site'  : site_record,
                 }
 
     result = {}
     for x in query_records:
         x_record = query_records[x]
-        logger.debug("Trying to resolve OTPme %s via DNS: %s (TXT)"
+        config.logger.debug("Trying to resolve OTPme %s via DNS: %s (TXT)"
                     % (x, x_record))
         try:
             answers = dns.resolver.query(x_record, 'TXT')
         except Exception as e:
             msg = ("Failed to query OTPme %s via DNS: %s" % (x, e))
             raise OTPmeException(msg)
         for a in answers:
             text = a.to_text().strip('"')
             result[x] = text
-            logger.debug("Got OTPme %s from DNS: %s" % (x, text))
+            config.logger.debug("Got OTPme %s from DNS: %s" % (x, text))
             break
         if not x in result:
             msg = ("Unable to get OTPme %s via DNS.")
             raise OTPmeException(msg)
     return result
 
 def get_daemon_uri(daemon, domain):
@@ -118,40 +115,47 @@
         srv_record = '_otpme-login._tcp.%s' % domain
     elif daemon == "joind":
         srv_record = '_otpme-join._tcp.%s' % domain
     else:
         msg = ("Unsupported daemon: %s" % daemon)
         raise OTPmeException(msg)
 
-    logger.debug("Trying to resolve %s socket URI via DNS: %s (SRV)"
+    config.logger.debug("Trying to resolve %s socket URI via DNS: %s (SRV)"
                 % (daemon, srv_record))
     try:
         answers = dns.resolver.query(srv_record, 'SRV')
     except Exception as e:
         msg = ("Failed to query OTPme %s attributes via DNS: %s"
                 % (daemon, e))
         raise OTPmeException(msg)
     for a in answers:
         text = a.to_text().strip('"')
         host = text.split()[-1].rstrip(".")
         port = text.split()[-2]
         socket_uri = "tcp://%s:%s" % (host, port)
-        logger.debug("Got %s socket URI from DNS: %s"
+        config.logger.debug("Got %s socket URI from DNS: %s"
                     % (daemon, socket_uri))
         return socket_uri
-    logger.debug("Unable to get %s address via SRV record, trying A "
+    config.logger.debug("Unable to get %s address via SRV record, trying A "
                 "record..." % daemon)
     try:
         socket.gethostbyname(domain)
         port = config.default_ports[daemon]
         socket_uri = "tcp://%s:%s" % (domain, port)
         return socket_uri
     except:
         return None
 
+def query_dns(name, record="A"):
+    result = dns.resolver.query(name, record)
+    addresses = []
+    for a in result:
+        addresses.append(a.to_text().strip('"'))
+    return addresses
+
 def get_interfaces():
     """ Get all interface configs. """
     interfaces = {}
     for interface in netifaces.interfaces():
         addresses = netifaces.ifaddresses(interface)
         if not 2 in addresses:
             continue
@@ -212,59 +216,59 @@
 
     if not phy_interface:
         msg = (_("No interface is configured for network of IP: %s")
                 % floating_ip)
         raise OTPmeException(msg)
 
     floating_interface = phy_interface
-    logger.debug("Found interface '%s' for network '%s/%s'"
+    config.logger.debug("Found interface '%s' for network '%s/%s'"
                 % (floating_interface, floating_ip_network, floating_ip_netmask))
 
     if ping:
-        logger.info("Pinging address '%s'" % floating_ip)
+        config.logger.info("Pinging address '%s'" % floating_ip)
         ping_command = "ping -w 1 -c 1 %s > /dev/null 2>&1" % floating_ip
         response = os.system(ping_command)
         if response == 0:
             msg = (_("Cannot add address '%s': already in use") % floating_ip)
             raise AddressAlreadyInUse(msg)
 
     msg = ("Adding address '%s/%s' to interface '%s'"
         % (floating_ip, floating_ip_netmask, floating_interface))
-    logger.info(msg)
+    config.logger.info(msg)
 
     ip_netmask = "%s/%s" % (floating_ip, floating_ip_netmask)
     ifup_command = [
                     "ip",
                     "addr",
                     "add",
                     "dev",
                     floating_interface,
                     ip_netmask,
                     ]
 
-    logger.debug("Running: %s" % " ".join(ifup_command))
+    config.logger.debug("Running: %s" % " ".join(ifup_command))
 
     pipe = Popen(ifup_command, stdout=PIPE, stderr=PIPE, shell=False)
     script_stdout, script_stderr = pipe.communicate()
     script_returncode = pipe.returncode
 
     if script_returncode != 0:
         msg = (_("Error adding address '%s/%s' to interface '%s': %s")
                 % (floating_ip, floating_ip_netmask,
                 floating_interface, script_stderr))
         raise OTPmeException(msg)
 
     if gratuitous_arp:
         msg = ("Sending gratuitous ARP for floating IP: %s (%s)"
                 % (floating_ip, floating_interface))
-        logger.debug(msg)
+        config.logger.debug(msg)
         # Send gratuitous ARP.
         arp.send_gratuitous_arp(floating_interface, floating_ip)
 
-    logger.debug("Floating IP address configured successful.")
+    config.logger.debug("Floating IP address configured successful.")
 
 def deconfigure_floating_ip(address):
     """ Deconfigure floating IP. """
     floating_interface = None
     floating_ip = address
     interfaces = get_interfaces()
 
@@ -275,32 +279,32 @@
             if ip == floating_ip:
                 floating_interface = iface
                 floating_ip_netmask = netmask
                 break
 
     if floating_interface:
         msg = ("Deconfiguring floating interface '%s'" % floating_interface)
-        logger.debug(msg)
+        config.logger.debug(msg)
 
         ip_netmask = "%s/%s" % (floating_ip, floating_ip_netmask)
         ifdown_command = [
                             "ip",
                             "addr",
                             "del",
                             "dev",
                             floating_interface,
                             ip_netmask,
                         ]
 
-        logger.debug("Running: %s" % " ".join(ifdown_command))
+        config.logger.debug("Running: %s" % " ".join(ifdown_command))
 
         pipe = Popen(ifdown_command, stdout=PIPE, stderr=PIPE, shell=False)
         script_stdout, script_stderr = pipe.communicate()
         script_returncode = pipe.returncode
 
         if script_returncode != 0:
             msg = (_("Error removing address '%s/%s' from interface '%s': %s")
                     % (floating_ip, floating_ip_netmask,
                     floating_interface, script_stderr))
             raise OTPmeException(msg)
 
-        logger.debug("Floating IP address deconfigured successful.")
+        config.logger.debug("Floating IP address deconfigured successful.")
```

### Comparing `otpme-0.3.0a46/otpme/lib/nsscache.py` & `otpme-0.3.0a47/otpme/lib/nsscache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/offline_token.py` & `otpme-0.3.0a47/otpme/lib/offline_token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/oid.py` & `otpme-0.3.0a47/otpme/lib/oid.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/otp/oath/hotp.py` & `otpme-0.3.0a47/otpme/lib/otp/oath/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/otp/oath/totp.py` & `otpme-0.3.0a47/otpme/lib/otp/oath/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/otp/otpme/otpme.py` & `otpme-0.3.0a47/otpme/lib/otp/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/otp/yubico/yubiotp.py` & `otpme-0.3.0a47/otpme/lib/otp/yubico/yubiotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/otpme_acl.py` & `otpme-0.3.0a47/otpme/lib/otpme_acl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/otpme_config.py` & `otpme-0.3.0a47/otpme/lib/otpme_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     os.environ['OTPME_DEBUG_NEED_DECORATOR'] = "False"
 if "OTPME_DEBUG_FILE_READ" not in os.environ:
     os.environ['OTPME_DEBUG_FILE_READ'] = "False"
 if "OTPME_DEBUG_FILE_WRITE" not in os.environ:
     os.environ['OTPME_DEBUG_FILE_WRITE'] = "False"
 
 if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
-    print(_("Loading module: %s") % __name__)
+    print("Loading module: %s" % __name__)
 
 import otpme
 from otpme.lib import re
 from otpme.lib import log
 from otpme.lib.messages import message
 from otpme.lib.encryption import get_module
 from otpme.lib.messages import error_message
 
 from otpme.lib.exceptions import *
 
 class OTPmeConfig(object):
     def __init__(self, tool_name="otpme", use_syslog=False,
-        use_systemd_log=False, quiet=False):
+        use_systemd_log=False, auto_load=True, quiet=False):
         # All registered methods.
         self.methods = []
         # All registered properties.
         self.properties = []
         # All registered extensions.
         self.extensions = []
         self.default_extensions = {}
@@ -134,15 +134,16 @@
         self.register_config_var("posix_msgsize_max", None, 8192)
         # Realm infos.
         self.register_config_var("realm", str, None)
         self.register_config_var("realm_uuid", str, None)
         # Site infos.
         self.register_config_var("site", str, None)
         self.register_config_var("site_uuid", str, None)
-        self.register_config_var("site_fqdn", str, None)
+        self.register_config_var("site_auth_fqdn", str, None)
+        self.register_config_var("site_mgmt_fqdn", str, None)
         self.register_config_var("site_address", str, None)
 
         # Users otpme config.
         self.register_config_var("user_config", dict, None)
         # Indicates config reload.
         self.register_config_var("config_reload", bool, None)
         self.register_config_var("user_config_reload", bool, None)
@@ -632,16 +633,20 @@
         self.register_config_var("pwgen_bin", str, "pwgen",
                             config_file_parameter="PWGEN")
         self.register_config_var("timezone", str, "Europe/Berlin",
                                 config_file_parameter="TIMEZONE")
         # Debug stuff.
         self.register_config_var("debug_test", bool, False)
 
+        # Set config to be imported via "from otpme.lib import config"
+        otpme.lib.config = self
+
         # Load config etc.
-        self.load(quiet=quiet)
+        if auto_load:
+            self.load(quiet=quiet)
 
     def __setattr__(self, name, value):
         """ Handle config variables and type checks. """
         if name == "methods":
             return object.__setattr__(self, name, value)
         if name == "properties":
             return object.__setattr__(self, name, value)
@@ -734,16 +739,14 @@
         self.load(quiet=quiet)
 
     def load(self, quiet=False):
         """ Load config. """
         from otpme.lib.register import register_module
         # Set own PID.
         self.my_pid = os.getpid()
-        # Set config to be imported via "from otpme.lib import config"
-        otpme.lib.config = self
 
         # Get command line options.
         if not self.config_reload:
             from otpme.lib.help import get_main_opts
             main_opts = get_main_opts()
             for var in main_opts:
                 self.command_line_opts.append(var)
@@ -2235,20 +2238,21 @@
         return main_config
 
     def set_realm(self, name, uuid):
         """ Set our realm. """
         self.realm = name
         self.realm_uuid = uuid
 
-    def set_site(self, name, uuid, address, fqdn=None):
+    def set_site(self, name, uuid, address, auth_fqdn=None, mgmt_fqdn=None):
         """ Set our site. """
         self.site = name
         self.site_uuid = uuid
-        self.site_fqdn = fqdn
         self.site_address = address
+        self.site_auth_fqdn = auth_fqdn
+        self.site_mgmt_fqdn = mgmt_fqdn
 
     def get_master_node(self):
         from otpme.lib import multiprocessing
         try:
             master_node = multiprocessing.get_dict(name="master_node")['master']
         except KeyError:
             master_node = None
@@ -2448,16 +2452,17 @@
         import json
         from otpme.lib import filetools
         realm_data = {
                     'realm'         : self.realm,
                     'realm_uuid'    : self.realm_uuid,
                     'site'          : self.site,
                     'site_uuid'     : self.site_uuid,
-                    'site_fqdn'     : self.site_fqdn,
                     'site_address'  : self.site_address,
+                    'site_auth_fqdn': self.site_auth_fqdn,
+                    'site_mgmt_fqdn': self.site_mgmt_fqdn,
                     }
         realm_data = json.dumps(realm_data, sort_keys=True, indent=4)
         try:
             filetools.create_file(path=self.realm_data_file_path,
                                 content=realm_data,
                                 user=self.user,
                                 group=self.group,
```

### Comparing `otpme-0.3.0a46/otpme/lib/otpme_pass.py` & `otpme-0.3.0a47/otpme/lib/otpme_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pam.py` & `otpme-0.3.0a47/otpme/lib/pam.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pickle.py` & `otpme-0.3.0a47/otpme/lib/pickle.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pinentry/pinentry.py` & `otpme-0.3.0a47/otpme/lib/pinentry/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pinentry/wrapper.py` & `otpme-0.3.0a47/otpme/lib/pinentry/wrapper.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pki/cert.py` & `otpme-0.3.0a47/otpme/lib/pki/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pki/utils.py` & `otpme-0.3.0a47/otpme/lib/pki/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/pki/utils_openssl.py` & `otpme-0.3.0a47/otpme/lib/pki/utils_openssl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/__init__.py` & `otpme-0.3.0a47/otpme/lib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/authonaction/authonaction.py` & `otpme-0.3.0a47/otpme/lib/policy/authonaction/authonaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,20 +444,17 @@
             raise self.policy_exception(msg)
 
         if not '_caller' in kwargs:
             msg = (_("AuthonactionPolicy needs <_caller>."))
             raise OTPmeException(msg)
 
         if callback.api_mode:
-            try:
+            if config.reauth_callback:
                 callback = config.reauth_callback
-            except:
-                msg = (_("Cannot reauth without <callback>."))
-                raise OTPmeException(msg)
-            logger.debug("Using callback from previous call to do reauth.")
+                logger.debug("Using callback from previous call to do reauth.")
 
         if callback.api_mode:
             msg = (_("Cannot reauth in API mode."))
             exception = OTPmeException(msg)
             callback.exception(exception)
 
         config.reauth_callback = callback
```

### Comparing `otpme-0.3.0a46/otpme/lib/policy/autodisable/autodisable.py` & `otpme-0.3.0a47/otpme/lib/policy/autodisable/autodisable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2014 the2nd <the2nd@otpme.org>
 # Distributed under the terms of the GNU General Public License v2
 import os
 import time
-import datetime
 
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
     pass
 
@@ -69,15 +68,15 @@
 
 recursive_default_acls = default_acls
 
 commands = {
     'auto_disable'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_auto_disable',
+                    'method'            : '_change_auto_disable',
                     'args'              : ['auto_disable'],
                     'oargs'             : ['unused'],
                     'job_type'          : 'process',
                     },
                 },
             },
     }
@@ -143,47 +142,47 @@
     """ Register policy type. """
     config.register_sub_object_type("policy", POLICY_TYPE)
 
 def register_policy_object():
     """ Registger policy type. """
     # Register base policy.
     call_methods = [
-                    ({'change_auto_disable': {'auto_disable': '+1h'}},),
+                    ({'_change_auto_disable': {'auto_disable': '+1h'}},),
                 ]
     config.register_base_object(object_type="policy",
                                 name="auto_disable_hour",
                                 stype=POLICY_TYPE,
                                 call_methods=call_methods)
     # Register base policy.
     call_methods = [
-                    ({'change_auto_disable': {'auto_disable': '+1D'}},),
+                    ({'_change_auto_disable': {'auto_disable': '+1D'}},),
                 ]
     config.register_base_object(object_type="policy",
                                 name="auto_disable_day",
                                 stype=POLICY_TYPE,
                                 call_methods=call_methods)
     # Register base policy.
     call_methods = [
-                    ({'change_auto_disable': {'auto_disable': '+1W'}},),
+                    ({'_change_auto_disable': {'auto_disable': '+1W'}},),
                 ]
     config.register_base_object(object_type="policy",
                                 name="auto_disable_week",
                                 stype=POLICY_TYPE,
                                 call_methods=call_methods)
     # Register base policy.
     call_methods = [
-                    ({'change_auto_disable': {'auto_disable': '+1M'}},),
+                    ({'_change_auto_disable': {'auto_disable': '+1M'}},),
                 ]
     config.register_base_object(object_type="policy",
                                 name="auto_disable_month",
                                 stype=POLICY_TYPE,
                                 call_methods=call_methods)
     # Register base policy.
     call_methods = [
-                    ({'change_auto_disable': {'auto_disable': '+1Y'}},),
+                    ({'_change_auto_disable': {'auto_disable': '+1Y'}},),
                 ]
     config.register_base_object(object_type="policy",
                                 name="auto_disable_year",
                                 stype=POLICY_TYPE,
                                 call_methods=call_methods)
 
 class AutodisablePolicy(Policy):
@@ -225,16 +224,16 @@
                             'realm',
                             'group',
                             'client',
                             'policy',
                             'accessgroup',
                             ]
 
-        self.auto_disable = "+1M"
-        self.unused_disable = False
+        self._auto_disable = "+1M"
+        self._unused_disable = False
 
         self._sub_sync_fields = {
                     'host'  : {
                         'trusted'  : [
                             "AUTO_DISABLE",
                             "UNUSED_DISABLE",
                             #"EXTENSIONS",
@@ -249,101 +248,51 @@
                         },
                     }
 
     def _get_object_config(self):
         """ Merge policy config with config from parent class. """
         policy_config = {
             'AUTO_DISABLE'              : {
-                                            'var_name'      : 'auto_disable',
+                                            'var_name'      : '_auto_disable',
                                             'type'          : str,
                                             'required'      : True,
                                         },
             'UNUSED_DISABLE'            : {
-                                            'var_name'      : 'unused_disable',
+                                            'var_name'      : '_unused_disable',
                                             'type'          : bool,
                                             'required'      : True,
                                         },
             }
 
         # Use parent class method to merge policy configs.
         return Policy._get_object_config(self, policy_config=policy_config)
 
     def set_variables(self):
         """ Set instance variables. """
         # Run parent class method that may override default values with those
         # read from config.
         Policy.set_variables(self)
 
-    def string2unixtime(self, date_string, start_time):
-        """ Get unix time from string. """
-        hour = None
-        minute = None
-        day = None
-        month = None
-        year = None
-        if date_string.startswith("+"):
-            x = date_string.replace("+", "")
-            seconds = units.time2int(x)
-            start_time = datetime.datetime.fromtimestamp(start_time)
-            disable_time = start_time + datetime.timedelta(seconds=seconds)
-        else:
-            for x in date_string.split():
-                if len(x.split("/")) == 3:
-                    month = int(x.split("/")[0])
-                    day = int(x.split("/")[1])
-                    year = int(x.split("/")[2])
-                elif len(x.split("-")) == 3:
-                    year = int(x.split("-")[0])
-                    month = int(x.split("-")[1])
-                    day = int(x.split("-")[2])
-                elif len(x.split(".")) == 3:
-                    day = int(x.split(".")[0])
-                    month = int(x.split(".")[1])
-                    year = int(x.split(".")[2])
-                elif len(x.split(":")) == 2:
-                    hour = int(x.split(":")[0])
-                    minute = int(x.split(":")[1])
-                else:
-                    msg = (_("Unknown date string: %s") % date_string)
-                    raise OTPmeException(msg)
-
-            if year is None:
-                raise OTPmeException("Missing 'year'")
-            if month is None:
-                raise OTPmeException("Missing 'month'")
-            if hour is None:
-                raise OTPmeException("Missing 'hour'")
-            if minute is None:
-                raise OTPmeException("Missing 'minute'")
-
-            if len(str(year)) < 4:
-                raise OTPmeException(_("Unknown year: %s") % year)
-
-            disable_time = datetime.datetime(year, month, day, hour, minute)
-
-        disable_time = float(disable_time.strftime("%s"))
-        return disable_time
-
     def activate(self):
         """ Activate policy by returning per object policy data """
         policy_data = {
                     'policy_add_time'   : time.time(),
                     }
         return policy_data
 
     def test(self, force=False, verbose_level=0,
         _caller="API", callback=default_callback):
         """ Test the policy. """
-        return callback.ok(self.auto_disable)
+        return callback.ok(self._auto_disable)
 
     def handle_hook(self, hook_object, hook_name, force=False,
         callback=default_callback, **kwargs):
         """ Handle policy hooks. """
         if hook_name == "exists":
-            return self.check_auto_disable(hook_object, **kwargs)
+            return self._check_auto_disable(hook_object, **kwargs)
         if hook_name != "enable":
             return callback.error(_("Unknown policy hook: %s") % hook_name,
                                     exception=self.policy_exception)
         if not hook_object.enabled and not force:
             msg = (_("%s disabled by policy.") % hook_object.type)
             return callback.error(message=msg,
                                 raise_exception=True,
@@ -357,23 +306,23 @@
             msg = (_("Unable to update object policy: %s") % e)
             logger.warning(msg)
             callback.send(msg)
         except Exception as e:
             msg = ("Error updating object policy: %s" % e)
             logger.warning(msg)
 
-    def check_auto_disable(self, hook_object, policy_add_time=None, **kwargs):
+    def _check_auto_disable(self, hook_object, policy_add_time=None, **kwargs):
         """ Handle auto disable. """
         if not policy_add_time:
             return True
-        if self.unused_disable:
+        if self._unused_disable:
             check_time = hook_object.get_last_used_time()
         else:
             check_time = policy_add_time
-        disable_time = self.string2unixtime(self.auto_disable, check_time)
+        disable_time = units.string2unixtime(self._auto_disable, check_time)
         now = time.time()
         if now >= disable_time:
             if hook_object.enabled:
                 try:
                     hook_object.disable(force=True, verify_acls=False)
                     object_disabled = True
                     hook_object._write()
@@ -390,21 +339,21 @@
                     logger.critical(msg)
                     return False
         return True
 
     @check_acls(['edit:auto_disable'])
     @object_lock()
     @backend.transaction
-    def change_auto_disable(self, auto_disable, unused=False,
+    def _change_auto_disable(self, auto_disable, unused=False,
         run_policies=True, callback=default_callback,
         _caller="API", **kwargs):
         """ Change auto disable value. """
         try:
             # Check if given date string is valid.
-            self.string2unixtime(auto_disable, time.time())
+            units.string2unixtime(auto_disable, time.time())
         except Exception as e:
             msg = "Invalid date string: %s" % e
             return callback.error(msg)
 
         if run_policies:
             try:
                 self.run_policies("modify",
@@ -412,16 +361,16 @@
                                 _caller=_caller)
                 self.run_policies("change_auto_disable",
                                 callback=callback,
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
-        self.auto_disable = auto_disable
-        self.unused_disable = unused
+        self._auto_disable = auto_disable
+        self._unused_disable = unused
         return self._cache(callback=callback)
 
     @object_lock()
     def _add(self, callback=default_callback, **kwargs):
         """ Add a policy """
         return callback.ok()
 
@@ -432,21 +381,21 @@
             return callback.error(msg, exception=PermissionDenied)
 
         lines = []
 
         auto_disable = ""
         if self.verify_acl("view:auto_disable") \
         or self.verify_acl("edit:auto_disable"):
-            auto_disable = self.auto_disable
+            auto_disable = self._auto_disable
         lines.append('AUTO_DISABLE="%s"' % auto_disable)
 
         unused_disable = ""
         if self.verify_acl("view:unused_disable") \
         or self.verify_acl("edit:unused_disable"):
-            unused_disable = self.unused_disable
+            unused_disable = self._unused_disable
         lines.append('UNUSED_DISABLE="%s"' % unused_disable)
 
         return Policy.show_config(self,
                                 config_lines=lines,
                                 callback=callback,
                                 **kwargs)
     def show(self, **kwargs):
```

### Comparing `otpme-0.3.0a46/otpme/lib/policy/defaultgroups/defaultgroups.py` & `otpme-0.3.0a47/otpme/lib/policy/defaultgroups/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/defaultpolicies/defaultpolicies.py` & `otpme-0.3.0a47/otpme/lib/policy/defaultpolicies/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/defaultroles/defaultroles.py` & `otpme-0.3.0a47/otpme/lib/policy/defaultroles/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/defaultunits/defaultunits.py` & `otpme-0.3.0a47/otpme/lib/policy/defaultunits/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/forcetoken/forcetoken.py` & `otpme-0.3.0a47/otpme/lib/policy/forcetoken/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/get_class.py` & `otpme-0.3.0a47/otpme/lib/policy/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/idrange/idrange.py` & `otpme-0.3.0a47/otpme/lib/policy/idrange/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/logintimes/logintimes.py` & `otpme-0.3.0a47/otpme/lib/policy/logintimes/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/objecttemplates/objecttemplates.py` & `otpme-0.3.0a47/otpme/lib/policy/objecttemplates/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/password/password.py` & `otpme-0.3.0a47/otpme/lib/policy/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/tokenacls/tokenacls.py` & `otpme-0.3.0a47/otpme/lib/policy/tokenacls/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/policy/utils.py` & `otpme-0.3.0a47/otpme/lib/policy/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/preload.py` & `otpme-0.3.0a47/otpme/lib/preload.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/progress.py` & `otpme-0.3.0a47/otpme/lib/progress.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/__init__.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/agent1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/auth1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/cluster1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/get_class.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/host1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/join1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/mgmt1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/client/sync1.py` & `otpme-0.3.0a47/otpme/lib/protocols/client/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/otpme_client.py` & `otpme-0.3.0a47/otpme/lib/protocols/otpme_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,18 +222,14 @@
                 msg = "auto_preauth=True conflicts with use_agent=True"
                 raise OTPmeException(msg)
         else:
             if do_preauth is None:
                 do_preauth = True
             self.proto_handler_args['do_preauth'] = do_preauth
 
-        ## Set default username if none was given.
-        #if not username:
-        #    username = config.login_user
-
         if not local_socket:
             # Set default realm and site if needed.
             if not realm:
                 realm = config.connect_realm
             if not site:
                 site = config.connect_site
 
@@ -338,61 +334,18 @@
                     pass
                 try:
                     ca_data = config.host_data['ca_data']
                 except:
                     if self.verify_server:
                         raise OTPmeException(_("Host CA data missing."))
 
-            # If we got no socket URI build it from parameters we got.
-            use_ssl = self.use_ssl
-            if not self.socket_uri:
-                if self.daemon == "hostd":
-                    use_ssl = False
-                    self.encrypt_session = False
-                    self.socket_uri = config.hostd_socket_path
-                elif self.use_agent:
-                    use_ssl = False
-                    self.encrypt_session = False
-                    try:
-                        otpme_agent_user = kwargs['otpme_agent_user']
-                    except:
-                        otpme_agent_user = None
-                    self.socket_uri = config.get_agent_socket(otpme_agent_user)
-                else:
-                    if realm and site:
-                        try:
-                            site_address = stuff.get_site_address(realm, site, fqdn=True)
-                        except ConnectionError as e:
-                            msg = "Unable to get site address: %s" % e
-                            raise ConnectionError(msg)
-                        if not site_address:
-                            try:
-                                site_address = stuff.get_site_address(realm, site, fqdn=False)
-                            except ConnectionError as e:
-                                msg = "Unable to get site address: %s" % e
-                                raise ConnectionError(msg)
-                    else:
-                        site_address = config.site_fqdn
-                        if not site_address:
-                            site_address = config.site_address
-                            if not config.site_address:
-                                raise OTPmeException(_("Unable to get site address."))
-                    if not self.daemon in config.default_ports:
-                        msg = (_("Unable to get daemon port: %s") % self.daemon)
-                        raise OTPmeException(msg)
-
-                    # Set daemon port.
-                    daemon_port = config.default_ports[self.daemon]
-                    # Set socket URI.
-                    self.socket_uri = "tcp://%s:%s" % (site_address, daemon_port)
-
             # Create connect socket.
             self.connection = ConnectSocket(socket_uri=self.socket_uri,
                                             socket_handler=SocketProtoHandler,
-                                            use_ssl=use_ssl,
+                                            use_ssl=self.use_ssl,
                                             cert=cert,
                                             key=key,
                                             ca_data=ca_data,
                                             verify_server=self.verify_server)
         # Handle autoconnect.
         if self.autoconnect:
             try:
@@ -862,14 +815,18 @@
             if self.encrypt_session:
                 encrypt_request = True
 
         # No need to encrypt in API mode.
         if config.use_api:
             encrypt_request = False
 
+        # Allow unencrypted ping command.
+        if command == "ping":
+            encrypt_request = False
+
         # Set encryption type and key used for en- and decryption.
         if self.session_key:
             enc_mod = self.session_enc_mod
             enc_key = self.session_key
 
         # Build proxy request when using otpme-agent.
         if use_agent:
@@ -2269,14 +2226,17 @@
         #self.logger.debug(msg)
         if status_code == status_codes.ERR:
             raise AuthFailed(response)
 
         if status_code == status_codes.HOST_DISABLED:
             raise HostDisabled(response)
 
+        if status_code == status_codes.CLUSTER_NOT_READY:
+            raise ConnectionError(response)
+
         if status_code != status_codes.OK:
             msg = (_("Got unknown preauth reply code: %s") % status_code)
             raise OTPmeException(msg)
 
         if not isinstance(response, dict):
             msg = (_("Got wrong preauth reply: %s") % response)
             raise OTPmeException(msg)
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/otpme_server.py` & `otpme-0.3.0a47/otpme/lib/protocols/otpme_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,19 @@
         except:
             self.verify_host = True
         try:
             self.require_master_node
         except:
             self.require_master_node = True
 
+        try:
+            self.require_cluster_status
+        except:
+            self.require_cluster_status = True
+
         # Client infos.
         self.client = client
         self.client_name = client
         # Get process infos from unix socket client.
         if self.client.startswith("socket://"):
             self.client_proc = re.sub('^socket://([^:]*):([^:]*):([^:]*):([^:]*)$', r'\1',
                                     self.client)
@@ -416,24 +421,31 @@
         """ Process command. """
         #if len(data) == 0:
         #    msg = ("Client '%s' closed connection." % self.client)
         #    self.logger.warning(msg)
         #    message = "Bye bye..."
         #    raise ClientQuit(message)
         if config.host_data['type'] == "node":
-            if self.require_master_node:
-                if not config.use_api:
+            if not config.use_api:
+                if self.require_master_node:
                     try:
                         current_master_node = multiprocessing.master_node['master']
                     except:
                         current_master_node = None
                     if current_master_node != config.host_data['name']:
                         status = False
-                        response = "Please connect to master node."
-                        return self.build_response(status, response, encrypt=False)
+                        message = "Please connect to master node."
+                        return self.build_response(status, message, encrypt=False)
+                if self.require_cluster_status:
+                    try:
+                        self.check_cluster_status()
+                    except Exception as e:
+                        message = str(e)
+                        status = status_codes.CLUSTER_NOT_READY
+                        return self.build_response(status, message, encrypt=False)
 
         # Remove newline and carriage return.
         request = data.replace('\n', '').replace('\r', '')
 
         enc_key = None
         enc_mod = None
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/request.py` & `otpme-0.3.0a47/otpme/lib/protocols/request.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/response.py` & `otpme-0.3.0a47/otpme/lib/protocols/response.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/__init__.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/agent1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/auth1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/auth1.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         # Authd does not require any authentication on client connect.
         self.require_auth = None
         self.require_preauth = True
         # Instructs parent class to require a client certificate.
         self.require_client_cert = True
         # Auth request are allowed to any node.
         self.require_master_node = False
+        # We need a clean cluster status.
+        self.require_cluster_status = True
         # Call parent class init.
         OTPmeServer1.__init__(self, **kwargs)
 
     def _pre_init(self, *args, **kwargs):
         """ Init protocol handler. """
         # Our PID.
         self.pid = os.getpid()
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/cluster1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/cluster1.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
         self.name = "clusterd"
         # The protocol we support.
         self.protocol = PROTOCOL_VERSION
         # Indicates parent class that we need no authentication.
         self.require_auth = "host"
         self.require_preauth = False
         self.require_client_cert = True
-        # Communication with hostd is only done via unix sockets.
         self.encrypt_session = True
         self.require_master_node = False
+        self.require_cluster_status = False
         # Call parent class init.
         OTPmeServer1.__init__(self, **kwargs)
 
     def _pre_init(self, *args, **kwargs):
         """ Init protocol handler. """
         # Our PID.
         self.pid = os.getpid()
@@ -225,16 +225,17 @@
             status = True
             message = "Node online."
             multiprocessing.online_nodes[self.peer.name] = True
 
         elif command == "set_node_sync":
             status = True
             message = "Node in sync."
-            sync_time = command_args['sync_time']
-            config.touch_node_sync_file(sync_time)
+            if not config.master_failover:
+                sync_time = command_args['sync_time']
+                config.touch_node_sync_file(sync_time)
 
         elif command == "unset_node_sync":
             status = True
             message = "Node NOT in sync."
             config.remove_node_sync_file()
 
         elif command == "get_node_vote":
@@ -559,14 +560,15 @@
                         message = "Cannot do master failover because of running jobs"
                         message = "%s\n%s" % (message, running_jobs)
 
         elif command == "set_master_failover":
             status = True
             message = "Master failover started successful."
             config.cluster_status = False
+            config.master_failover = True
 
         elif command == "get_master_failover_status":
             message = "Master failover status."
             status = config.master_failover
 
         elif command == "do_nsscache_sync":
             from otpme.lib.classes.command_handler import CommandHandler
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/get_class.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/host1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/host1.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self.require_preauth = False
         # FIXME: Currently hostd only uses unix sockets so there is no
         #        encryption involved.
         self.require_client_cert = False
         # Communication with hostd is only done via unix sockets.
         self.encrypt_session = False
         self.require_master_node = False
+        self.require_cluster_status = False
         # Call parent class init.
         OTPmeServer1.__init__(self, **kwargs)
 
     def _pre_init(self, *args, **kwargs):
         """ Init protocol handler. """
         # Our PID.
         self.pid = os.getpid()
@@ -133,18 +134,19 @@
         # all valid commands
         valid_commands = [
                             "get_realm",
                             "get_realm_uuid",
                             "get_site",
                             "get_site_uuid",
                             "get_site_address",
+                            "get_site_auth_fqdn",
+                            "get_site_mgmt_fqdn",
                             "get_realm_master_uuid",
                             "get_realm_master_name",
                             "get_realm_master_address",
-                            "get_site_fqdn",
                             "get_site_cert",
                             "get_site_trust_status",
                             "get_user_uuid",
                             "get_user_name",
                             "get_user_site",
                             "get_host_status",
                             "get_pass_strength",
@@ -239,39 +241,61 @@
             else:
                 site_address = config.site_address
 
             if status:
                 message = site_address
 
 
-        elif command == "get_site_fqdn":
+        elif command == "get_site_auth_fqdn":
             status = True
             try:
                 realm = command_args['realm']
             except:
                 realm = None
             try:
                 site = command_args['site']
             except:
                 site = None
 
             if realm and site:
                 try:
-                    site_address = stuff.get_site_address(realm,
-                                                        site,
-                                                        fqdn=True)
+                    auth_fqdn = stuff.get_site_fqdn(realm, site)
                 except Exception as e:
                     status = False
                     message = "Failed to get site address: %s" % e
             else:
-                site_address = config.site_address
+                auth_fqdn = config.site_auth_fqdn
 
             if status:
-                message = site_address
+                message = auth_fqdn
+
+        elif command == "get_site_mgmt_fqdn":
+            status = True
+            try:
+                realm = command_args['realm']
+            except:
+                realm = None
+            try:
+                site = command_args['site']
+            except:
+                site = None
+
+            if realm and site:
+                try:
+                    mgmt_fqdn = stuff.get_site_fqdn(realm,
+                                                    site,
+                                                    mgmt=True)
+                except Exception as e:
+                    status = False
+                    message = "Failed to get site address: %s" % e
+            else:
+                mgmt_fqdn = config.site_mgmt_fqdn
 
+            if status:
+                message = mgmt_fqdn
 
         elif command == "get_site_trust_status":
             status = True
             try:
                 realm_name = command_args['realm']
             except:
                 realm_name = None
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/join1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/join1.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
         self.request_site = None
         # Join requests require master node.
         self.require_master_node = True
         # JOTP/LOTP to use for decryption.
         self.session_otp = None
         # OTP type in use.
         self.session_otp_type = None
+        # Indicates master node join.
+        self.master_node_join = False
         # Join/Leave job uuid.
         self.job_uuid = None
         self.callback = None
         # Call parent class init.
         OTPmeServer1.__init__(self, **kwargs)
 
     def _pre_init(self, *args, **kwargs):
@@ -143,47 +145,47 @@
                 config.raise_exception()
                 return self.build_response(status, message)
 
         # Write changed objects.
         cache.flush()
 
         # For master node join requests we have to check some things.
-        master_node_join = False
-        if host.site_uuid != config.site_uuid:
-            master_node_join = True
-            s = backend.get_object(object_type="site", uuid=host.site_uuid)
-            if not s:
-                message = (_("Unknown site: %s") % host.site_uuid)
-                status = False
-                return self.build_response(status, message)
-
-            # The site must be disabled for master node join.
-            if s.enabled:
-                message = (_("Cannot do master node join for enabled site: %s")
-                            % s.name)
-                status = False
-                return self.build_response(status, message)
-
-            # Check if the joining host is a node.
-            if host.type != "node":
-                message = (_("Wrong host type: %s") % host.type)
-                status = False
-                return self.build_response(status, message)
-
-            all_nodes = backend.search(object_type="node",
-                                        attribute="uuid",
-                                        value="*",
-                                        realm=host.realm,
-                                        site=host.site,
-                                        return_type="name")
-            # Check if the joining node is the first node of this site.
-            if len(all_nodes) != 1:
-                message = (_("Node is not master node of site: %s") % s.name)
-                status = False
-                return self.build_response(status, message)
+        if host_type == "node":
+            if host.site_uuid != config.site_uuid:
+                s = backend.get_object(object_type="site", uuid=host.site_uuid)
+                if not s:
+                    message = (_("Unknown site: %s") % host.site_uuid)
+                    status = False
+                    return self.build_response(status, message)
+
+                # The site must be disabled for master node join.
+                if s.enabled:
+                    message = (_("Cannot do master node join for enabled site: %s")
+                                % s.name)
+                    status = False
+                    return self.build_response(status, message)
+
+                # Check if the joining host is a node.
+                if host.type != "node":
+                    message = (_("Wrong host type: %s") % host.type)
+                    status = False
+                    return self.build_response(status, message)
+
+                all_nodes = backend.search(object_type="node",
+                                            attribute="uuid",
+                                            value="*",
+                                            realm=host.realm,
+                                            site=host.site,
+                                            return_type="name")
+                # Check if the joining node is the first node of this site.
+                if len(all_nodes) != 1:
+                    message = (_("Node is not the first node of site: %s") % s.name)
+                    status = False
+                    return self.build_response(status, message)
+                self.master_node_join = True
 
         # Make host join the realm.
         try:
             host.join_realm(verify_acls=verify_acls,
                             callback=callback)
         except Exception as e:
             config.raise_exception()
@@ -376,16 +378,16 @@
             object_config = o.get_sync_config(peer=host)
             object_id = o.oid.full_oid
             sync_object_configs[object_id] = object_config
 
         # Build join reply.
         join_reply = {
                     'jotp'                  : host.jotp,
-                    'master_node_join'      : master_node_join,
                     'object_configs'        : sync_object_configs,
+                    'master_node_join'      : self.master_node_join,
                     'password_hash_salt'    : config.password_hash_salt,
                     }
 
         # Encode join reply.
         message = json.encode(join_reply)
         status = True
 
@@ -1140,15 +1142,15 @@
             multiprocessing.running_jobs.pop(self.job_uuid)
             return leave_result
 
         if command == "add_site_cert":
             status = False
             message = (_("Permission denied"))
             # If this is a master node join we may have to update site cert.
-            if host.type == "node" and host.site_uuid != config.site_uuid:
+            if self.master_node_join:
                 # Get hosts site.
                 site = backend.get_object(object_type="site",
                                         uuid=host.site_uuid)
                 # Try to get cert.
                 try:
                     cert = _request['cert']
                 except:
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/mgmt1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/mgmt1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1083,15 +1083,16 @@
                                 return self.build_response(status, message)
                             except OTPmeException as e:
                                 message = "Error: %s" % e
                                 status = False
                                 return self.build_response(status, message)
                         if result:
                             o = result[0]
-                            object_status = "exists"
+                            if o.exists(run_policies=True):
+                                object_status = "exists"
 
                         # If we found no object we have to check if this is a
                         # request to add a new object.
                         elif subcommand == "add" or subcommand == "init":
                             # Class getter for new object.
                             class_getter, \
                             getter_args = backend.get_class_getter(object_type)
@@ -1139,15 +1140,16 @@
                                                     attribute=attribute,
                                                     value=object_identifier,
                                                     return_type="instance",
                                                     site=search_site,
                                                     realm=search_realm)
                             if result:
                                 o = result[0]
-                                object_status = "exists"
+                                if o.exists(run_policies=True):
+                                    object_status = "exists"
                                 if not config.use_api:
                                     if o.type == "site":
                                         site_realm = backend.get_object(object_type="realm",
                                                                         uuid=o.realm_uuid)
                                         master_site = backend.get_object(object_type="site",
                                                                         uuid=site_realm.master)
                                         if not master_site:
@@ -1213,16 +1215,17 @@
                     return self.build_response(status, response)
             else:
                 if subcommand == "init":
                     if not config.use_api:
                         response = ("MGMT_UNKNOWN_COMMAND: %s %s"
                                     % (command, subcommand))
                     args = {
-                        'realm_master' : None,
-                        'master_address' : None,
+                        'realm_master'  : None,
+                        'site_address'  : None,
+                        'site_fqdn'     : None,
                     }
 
         # Get object sub type.
         try:
             sub_type_attribute = sub_types[object_type]
             sub_type = getattr(o, sub_type_attribute)
         except:
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/server/sync1.py` & `otpme-0.3.0a47/otpme/lib/protocols/server/sync1.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,16 @@
         # Indicates parent class that we need an authenticated host.
         self.require_auth = "host"
         self.require_preauth = True
         # Indicates parent class to require a client certificate.
         self.require_client_cert = True
         # Allow sync between nodes.
         self.require_master_node = False
+        # Sync must be possible while master node failover.
+        self.require_cluster_status = False
         # Call parent class init.
         OTPmeServer1.__init__(self, **kwargs)
 
     def _pre_init(self, *args, **kwargs):
         """ Init protocol handler. """
         # Our PID.
         self.pid = os.getpid()
```

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/status_codes.py` & `otpme-0.3.0a47/otpme/lib/protocols/status_codes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/protocols/utils.py` & `otpme-0.3.0a47/otpme/lib/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/push_script.py` & `otpme-0.3.0a47/otpme/lib/push_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/qrcode.py` & `otpme-0.3.0a47/otpme/lib/qrcode.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/re.py` & `otpme-0.3.0a47/otpme/lib/re.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/register/__init__.py` & `otpme-0.3.0a47/otpme/lib/register/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/resolver/__init__.py` & `otpme-0.3.0a47/otpme/lib/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/resolver/get_class.py` & `otpme-0.3.0a47/otpme/lib/resolver/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/resolver/ldap/ldap.py` & `otpme-0.3.0a47/otpme/lib/resolver/ldap/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/resolver/utils.py` & `otpme-0.3.0a47/otpme/lib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/script.py` & `otpme-0.3.0a47/otpme/lib/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/sign_key_cache.py` & `otpme-0.3.0a47/otpme/lib/sign_key_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/slp.py` & `otpme-0.3.0a47/otpme/lib/slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/__init__.py` & `otpme-0.3.0a47/otpme/lib/smartcard/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/fido2/fido2.py` & `otpme-0.3.0a47/otpme/lib/smartcard/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/get_class.py` & `otpme-0.3.0a47/otpme/lib/smartcard/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/utils.py` & `otpme-0.3.0a47/otpme/lib/smartcard/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/yubikey/deploy.py` & `otpme-0.3.0a47/otpme/lib/smartcard/yubikey/deploy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/yubikey/usb.py` & `otpme-0.3.0a47/otpme/lib/smartcard/yubikey/usb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/yubikey/yubikey.py` & `otpme-0.3.0a47/otpme/lib/smartcard/yubikey/yubikey.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py` & `otpme-0.3.0a47/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py` & `otpme-0.3.0a47/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/socket/connect.py` & `otpme-0.3.0a47/otpme/lib/socket/connect.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/socket/handler.py` & `otpme-0.3.0a47/otpme/lib/socket/handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/socket/listen.py` & `otpme-0.3.0a47/otpme/lib/socket/listen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/socket/send_recv1.py` & `otpme-0.3.0a47/otpme/lib/socket/send_recv1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/sotp.py` & `otpme-0.3.0a47/otpme/lib/sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/spsc.py` & `otpme-0.3.0a47/otpme/lib/spsc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/srp.py` & `otpme-0.3.0a47/otpme/lib/srp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/ssh.py` & `otpme-0.3.0a47/otpme/lib/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/stuff.py` & `otpme-0.3.0a47/otpme/lib/stuff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1619,41 +1619,75 @@
         status_code, \
         reply = hostd_conn.send(command, command_args)
         user_name = reply
         if not status:
             return None
     return user_name
 
-def get_site_address(realm, site, fqdn=False):
+def get_site_address(realm, site):
     """ Get site address/FQDN. """
     from otpme.lib import config
     from otpme.lib import backend
     from otpme.lib import connections
     if config.use_backend:
         _site = backend.get_object(object_type="site",
                                     name=site,
                                     realm=realm)
         if _site:
-            if fqdn:
-                site_address = _site.fqdn
+            site_address = _site.address
+        else:
+            msg = (_("Unknown site: %s") % site)
+            raise OTPmeException(msg)
+    else:
+        try:
+            hostd_conn = connections.get("hostd")
+        except Exception as e:
+            msg = (_("Error connecting to hostd: %s") % e)
+            raise OTPmeException(msg)
+        daemon_command = "get_site_address"
+        command_args = {
+                        'realm' : realm,
+                        'site'  : site,
+                    }
+        status, \
+        status_code, \
+        reply = hostd_conn.send(daemon_command, command_args)
+        if not status:
+            msg = (_("Error getting site address from hostd: %s") % reply)
+            raise ConnectionError(msg)
+        site_address = reply
+    return site_address
+
+def get_site_fqdn(realm, site, mgmt=False):
+    """ Get site address/FQDN. """
+    from otpme.lib import config
+    from otpme.lib import backend
+    from otpme.lib import connections
+    if config.use_backend:
+        _site = backend.get_object(object_type="site",
+                                    name=site,
+                                    realm=realm)
+        if _site:
+            if mgmt:
+                site_address = _site.mgmt_fqdn
             else:
-                site_address = _site.address
+                site_address = _site.auth_fqdn
         else:
             msg = (_("Unknown site: %s") % site)
             raise OTPmeException(msg)
     else:
         try:
             hostd_conn = connections.get("hostd")
         except Exception as e:
             msg = (_("Error connecting to hostd: %s") % e)
             raise OTPmeException(msg)
-        if fqdn:
-            daemon_command = "get_site_fqdn"
+        if mgmt:
+            daemon_command = "get_site_mgmt_fqdn"
         else:
-            daemon_command = "get_site_address"
+            daemon_command = "get_site_auth_fqdn"
         command_args = {
                         'realm' : realm,
                         'site'  : site,
                     }
         status, \
         status_code, \
         reply = hostd_conn.send(daemon_command, command_args)
```

### Comparing `otpme-0.3.0a46/otpme/lib/sync_cache.py` & `otpme-0.3.0a47/otpme/lib/sync_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/system_command.py` & `otpme-0.3.0a47/otpme/lib/system_command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/test.py` & `otpme-0.3.0a47/otpme/lib/test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/__init__.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/advanced.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/advanced.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/caching_query.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/caching_query.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/environment.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/environment.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/fixture_data.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/fixture_data.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/helloworld.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/helloworld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/local_session_caching.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/local_session_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/model.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/model.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/dogpile_caching/relationship_caching.py` & `otpme-0.3.0a47/otpme/lib/third_party/dogpile_caching/relationship_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/__init__.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/caches.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/caches/caches.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/caches/files.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/caches/files.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/config.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/error.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/error.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/lock.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/lock.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/group.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/maps.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/maps.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/passwd.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/passwd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/maps/shadow.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/maps/shadow.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/nss.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/nss.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/files_updater.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/files_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/map_updater.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/map_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/update/updater.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/update/updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/nss_cache/util/file_formats.py` & `otpme-0.3.0a47/otpme/lib/third_party/nss_cache/util/file_formats.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/_compat.py` & `otpme-0.3.0a47/otpme/lib/third_party/oath_toolkit/_compat.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/third_party/oath_toolkit/uri.py` & `otpme-0.3.0a47/otpme/lib/third_party/oath_toolkit/uri.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/__init__.py` & `otpme-0.3.0a47/otpme/lib/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/fido2/fido2.py` & `otpme-0.3.0a47/otpme/lib/token/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/get_class.py` & `otpme-0.3.0a47/otpme/lib/token/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/hotp/hotp.py` & `otpme-0.3.0a47/otpme/lib/token/hotp/hotp.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,18 @@
         if otp_includes_pin:
             if len(otp) < (int(self.pin_len) + int(self.otp_len)):
                 msg = ("Token PIN enabled but the given OTP is too "
                         "short to include a PIN!")
                 logger.debug(msg)
                 return None
             _otp = otp[self.pin_len:]
-            pin = int(otp[:self.pin_len])
+            try:
+                pin = int(otp[:self.pin_len])
+            except ValueError:
+                return None
         else:
             _otp = otp
 
         # If we got a secret this request is to verify the secret itself
         # (e.g. mode change)
         if not secret:
             # Get token secret.
@@ -737,17 +740,18 @@
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
         if pin is None:
             if self.mode == "mode2":
                 pin = callback.askpass("Please enter PIN: ")
-                pin = int(pin)
-                if pin is None:
-                    msg = "Cannot gen qrcode without PIN."
+                try:
+                    pin = int(pin)
+                except ValueError:
+                    msg = "Invalid PIN."
                     return callback.error(msg)
 
         # Get secret to gen QRCode.
         secret = self.get_secret(pin=pin)
 
         token_counter_start, token_counter_end = self.get_counter_range()
 
@@ -800,17 +804,18 @@
                                 _caller=_caller)
             except Exception:
                 return callback.error()
 
         pin = None
         if self.mode == "mode2":
             pin = callback.askpass("Please enter PIN: ")
-            pin = int(pin)
-            if pin is None:
-                msg = "Cannot resync without PIN."
+            try:
+                pin = int(pin)
+            except ValueError:
+                msg = "Invalid PIN."
                 return callback.error(msg)
 
         # Get token secret.
         token_secret = self.get_secret(pin=pin, callback=callback)
 
         # Get current token counter.
         current_counter = self.get_token_counter()
```

### Comparing `otpme-0.3.0a46/otpme/lib/token/link/link.py` & `otpme-0.3.0a47/otpme/lib/token/link/link.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/motp/motp.py` & `otpme-0.3.0a47/otpme/lib/token/motp/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/oath/oath.py` & `otpme-0.3.0a47/otpme/lib/token/oath/oath.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/otp_push/otp_push.py` & `otpme-0.3.0a47/otpme/lib/token/otp_push/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/otpme/otpme.py` & `otpme-0.3.0a47/otpme/lib/token/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/password/password.py` & `otpme-0.3.0a47/otpme/lib/token/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/script_otp/script_otp.py` & `otpme-0.3.0a47/otpme/lib/token/script_otp/script_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/script_static/script_static.py` & `otpme-0.3.0a47/otpme/lib/token/script_static/script_static.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/ssh/ssh.py` & `otpme-0.3.0a47/otpme/lib/token/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/totp/totp.py` & `otpme-0.3.0a47/otpme/lib/token/totp/totp.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,15 +639,18 @@
         # Get PIN from OTP if needed.
         if otp_includes_pin:
             if len(otp) < (int(self.pin_len) + int(self.otp_len)):
                 logger.debug("Token PIN enabled but the given OTP is too short "
                             "to include a PIN!")
                 return None
             _otp = otp[self.pin_len:]
-            pin = int(otp[:self.pin_len])
+            try:
+                pin = int(otp[:self.pin_len])
+            except ValueError:
+                return None
         else:
             _otp = otp
 
         # Calculate epoch time to verify OTP.
         epoch_time = time.time()
 
         # Calculate times for log entry.
```

### Comparing `otpme-0.3.0a46/otpme/lib/token/utils.py` & `otpme-0.3.0a47/otpme/lib/token/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme/lib/token/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a47/otpme/lib/token/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme.egg-info/PKG-INFO` & `otpme-0.3.0a47/otpme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a46
+Version: 0.3.0a47
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a46/otpme.egg-info/SOURCES.txt` & `otpme-0.3.0a47/otpme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme.egg-info/entry_points.txt` & `otpme-0.3.0a47/otpme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/otpme.egg-info/requires.txt` & `otpme-0.3.0a47/otpme.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a46/setup.py` & `otpme-0.3.0a47/setup.py`

 * *Files identical despite different names*

