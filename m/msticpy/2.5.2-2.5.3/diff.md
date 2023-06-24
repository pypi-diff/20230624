# Comparing `tmp/msticpy-2.5.2.tar.gz` & `tmp/msticpy-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msticpy-2.5.2.tar", last modified: Tue Jun 13 23:56:50 2023, max compression
+gzip compressed data, was "msticpy-2.5.3.tar", last modified: Sat Jun 24 21:51:48 2023, max compression
```

## Comparing `msticpy-2.5.2.tar` & `msticpy-2.5.3.tar`

### file list

```diff
@@ -1,418 +1,418 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.220096 msticpy-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-13 23:56:38.000000 msticpy-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 23:56:38.000000 msticpy-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-06-13 23:56:38.000000 msticpy-2.5.2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-13 23:56:50.220096 msticpy-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-06-13 23:56:38.000000 msticpy-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.176097 msticpy-2.5.2/msticpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.176097 msticpy-2.5.2/msticpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.176097 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/anomalous.py
--rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/sessionize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.180097 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/cluster_auditd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/code_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/polling_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/analysis/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.180097 msticpy-2.5.2/msticpy/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/azure_auth_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/cloud_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/cred_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/keyring_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/keyvault_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/keyvault_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/msal_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/auth/secret_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.180097 msticpy-2.5.2/msticpy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/check_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/pkg_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/provider_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/proxy_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.184097 msticpy-2.5.2/msticpy/common/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/utility/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/utility/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/utility/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/utility/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/common/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.184097 msticpy-2.5.2/msticpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_azure_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_msticpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_other_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_simple_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_ti_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/ce_user_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/comp_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/compound_ctrls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/file_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/mp_config_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/mp_config_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/config/mp_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.188097 msticpy-2.5.2/msticpy/context/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.188097 msticpy-2.5.2/msticpy/context/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_dynamic_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_dynamic_summary_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_ti.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_watchlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/azure/sentinel_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/contextlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.188097 msticpy-2.5.2/msticpy/context/contextproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/contextproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/contextproviders/context_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/contextproviders/http_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/contextproviders/servicenow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/lookup_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/preprocess_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.192097 msticpy-2.5.2/msticpy/context/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/alienvault_otx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/azure_sent_byoti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/greynoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/ibm_xforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/intsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/kql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/mblookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/open_page_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/pulsedive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/result_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/riskiq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/ti_http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/tor_exit_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/tiproviders/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.192097 msticpy-2.5.2/msticpy/context/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/vtlookupv3/vtlookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/context/vtlookupv3/vtlookupv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.192097 msticpy-2.5.2/msticpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.192097 msticpy-2.5.2/msticpy/data/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/azure/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/azure_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.192097 msticpy-2.5.2/msticpy/data/core/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/data_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/param_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_provider_connections_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_provider_utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/core/query_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/data_obfus.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/data_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.196097 msticpy-2.5.2/msticpy/data/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/azure_kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23280 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/azure_monitor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/cybereason_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/driver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/elastic_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23295 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/kql_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/local_data_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/local_osquery_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/mdatp_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/mordor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/odata_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/resource_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/security_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/sentinel_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/splunk_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/drivers/sumologic_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.172097 msticpy-2.5.2/msticpy/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.196097 msticpy-2.5.2/msticpy/data/queries/cybereason/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/cybereason/cybereason_connections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/cybereason/cybereason_hosts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/cybereason/cybereason_processes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.196097 msticpy-2.5.2/msticpy/data/queries/localdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/localdata/local_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.196097 msticpy-2.5.2/msticpy/data/queries/m365d/
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29648 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/queries/mde/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/queries/msgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/msgraph/graph_alerts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/queries/mssentinel/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_net.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/queries/resourcegraph/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/queries/splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/splunk/splunk_alert_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/splunk/splunk_queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/queries/sumologic/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/queries/sumologic/sumologic_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/sql_to_kql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.200096 msticpy-2.5.2/msticpy/data/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/storage/azure_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.204096 msticpy-2.5.2/msticpy/data/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/uploaders/loganalytics_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/uploaders/splunk_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/data/uploaders/uploader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.204096 msticpy-2.5.2/msticpy/datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.208096 msticpy-2.5.2/msticpy/datamodel/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/azure_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/cloud_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/cloud_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/entity_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/entity_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/file_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/graph_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/host_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/iot_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/mail_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/malware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/network_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/registry_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/registry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/submission_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/threat_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/unknown_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/entities/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.208096 msticpy-2.5.2/msticpy/datamodel/soc/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/soc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/soc/incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/datamodel/soc/sentinel_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.208096 msticpy-2.5.2/msticpy/init/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/azure_ml_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/azure_synapse_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/mp_pandas_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/mp_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    31388 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/nbinit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/nbmagics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.208096 msticpy-2.5.2/msticpy/init/pivot_core/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_magic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_core/pivot_register_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.208096 msticpy-2.5.2/msticpy/init/pivot_init/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_init/pivot_data_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_init/pivot_ti_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/pivot_init/vt_pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/init/user_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/msticpyconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.212096 msticpy-2.5.2/msticpy/nbtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/entityschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/nbwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/security_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/security_alert_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/security_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/security_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbtools/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.212096 msticpy-2.5.2/msticpy/nbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/get_environment_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/get_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/lookback.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/option_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/query_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/select_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/select_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/nbwidgets/select_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.212096 msticpy-2.5.2/msticpy/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/resources/WinSecurityEvent.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/resources/cmd_line_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/resources/mp_pivot_reg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/resources/mpconfig_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/resources/obfuscation_cols.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.216096 msticpy-2.5.2/msticpy/sectools/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/proc_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/sectools_magics.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.216096 msticpy-2.5.2/msticpy/sectools/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/vtlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.216096 msticpy-2.5.2/msticpy/sectools/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/vtlookupv3/vtlookupv3.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/sectools/vtlookupv3/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.216096 msticpy-2.5.2/msticpy/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/transform/process_tree_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.220096 msticpy-2.5.2/msticpy/vis/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/code_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/data_viewer_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/entity_graph_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/figure_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/matrix_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/mordor_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/mp_pandas_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/network_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/query_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/timeline_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/timeline_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-13 23:56:38.000000 msticpy-2.5.2/msticpy/vis/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:56:50.176097 msticpy-2.5.2/msticpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-13 23:56:50.000000 msticpy-2.5.2/msticpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-13 23:56:50.000000 msticpy-2.5.2/msticpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:56:50.000000 msticpy-2.5.2/msticpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:56:49.000000 msticpy-2.5.2/msticpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-13 23:56:50.000000 msticpy-2.5.2/msticpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 23:56:50.000000 msticpy-2.5.2/msticpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 23:56:38.000000 msticpy-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-13 23:56:38.000000 msticpy-2.5.2/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 23:56:38.000000 msticpy-2.5.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-13 23:56:38.000000 msticpy-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-13 23:56:50.220096 msticpy-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-13 23:56:38.000000 msticpy-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.914789 msticpy-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-24 21:51:36.000000 msticpy-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-24 21:51:36.000000 msticpy-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-06-24 21:51:36.000000 msticpy-2.5.3/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-24 21:51:48.914789 msticpy-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-06-24 21:51:36.000000 msticpy-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.866788 msticpy-2.5.3/msticpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/anomalous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/sessionize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/cluster_auditd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/code_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/polling_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/azure_auth_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/cloud_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/cred_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/keyring_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/keyvault_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/keyvault_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/msal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/secret_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.874788 msticpy-2.5.3/msticpy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/pkg_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/provider_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/proxy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.874788 msticpy-2.5.3/msticpy/common/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.878788 msticpy-2.5.3/msticpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_azure_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_msticpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_other_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_simple_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_ti_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_user_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/comp_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/compound_ctrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/file_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/mp_config_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/mp_config_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/mp_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.878788 msticpy-2.5.3/msticpy/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.878788 msticpy-2.5.3/msticpy/context/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_ti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_watchlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.882789 msticpy-2.5.3/msticpy/context/contextproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/context_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/http_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/servicenow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/lookup_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/preprocess_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.882789 msticpy-2.5.3/msticpy/context/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/alienvault_otx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/azure_sent_byoti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/greynoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/ibm_xforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/intsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/kql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/mblookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/open_page_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/pulsedive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/result_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/riskiq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/ti_http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/tor_exit_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.882789 msticpy-2.5.3/msticpy/context/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookupv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.886788 msticpy-2.5.3/msticpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.886788 msticpy-2.5.3/msticpy/data/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.886788 msticpy-2.5.3/msticpy/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/data_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/param_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_provider_connections_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_provider_utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/data_obfus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/data_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/azure_kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/azure_monitor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/cybereason_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/driver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/elastic_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/kql_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/local_data_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/local_osquery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/mdatp_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/mordor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/odata_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/resource_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/security_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/sentinel_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/splunk_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/sumologic_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.862788 msticpy-2.5.3/msticpy/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/cybereason/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_connections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_hosts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_processes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/localdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/localdata/local_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/m365d/
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29648 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/mde/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/msgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/msgraph/graph_alerts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/mssentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_net.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/resourcegraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/splunk/splunk_alert_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/splunk/splunk_queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/sumologic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/sumologic/sumologic_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/sql_to_kql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/storage/azure_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/loganalytics_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/splunk_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/uploader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.898789 msticpy-2.5.3/msticpy/datamodel/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/azure_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/cloud_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/cloud_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/entity_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/entity_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/file_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/graph_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/host_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/mail_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/malware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/registry_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/registry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/submission_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/threat_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/unknown_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.898789 msticpy-2.5.3/msticpy/datamodel/soc/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/soc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/soc/incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/soc/sentinel_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.902789 msticpy-2.5.3/msticpy/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/azure_ml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/azure_synapse_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/mp_pandas_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/mp_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31388 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/nbinit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/nbmagics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.902789 msticpy-2.5.3/msticpy/init/pivot_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_magic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_register_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.902789 msticpy-2.5.3/msticpy/init/pivot_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/pivot_data_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/pivot_ti_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/vt_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/msticpyconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.906789 msticpy-2.5.3/msticpy/nbtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/entityschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/nbwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_alert_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.906789 msticpy-2.5.3/msticpy/nbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/get_environment_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/get_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/lookback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/option_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/query_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/select_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/select_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/select_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.906789 msticpy-2.5.3/msticpy/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/WinSecurityEvent.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/cmd_line_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/mp_pivot_reg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/mpconfig_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/obfuscation_cols.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/sectools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/sectools_magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/sectools/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/sectools/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtlookupv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/process_tree_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.914789 msticpy-2.5.3/msticpy/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/code_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/data_viewer_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/entity_graph_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/figure_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/matrix_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/mordor_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/mp_pandas_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/network_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/query_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.866788 msticpy-2.5.3/msticpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-24 21:51:36.000000 msticpy-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-24 21:51:36.000000 msticpy-2.5.3/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-24 21:51:36.000000 msticpy-2.5.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-24 21:51:36.000000 msticpy-2.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-24 21:51:48.914789 msticpy-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-24 21:51:36.000000 msticpy-2.5.3/setup.py
```

### Comparing `msticpy-2.5.2/LICENSE` & `msticpy-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/NOTICE.txt` & `msticpy-2.5.3/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/PKG-INFO` & `msticpy-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.5.2
+Version: 2.5.3
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
```

### Comparing `msticpy-2.5.2/README.md` & `msticpy-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/__init__.py` & `msticpy-2.5.3/msticpy/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/__init__.py` & `msticpy-2.5.3/msticpy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/anomalous.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/anomalous.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/model.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/model.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/sessionize.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/sessionize.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/cmds_only.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/data_structures.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/anomalous_sequence/utils/probabilities.py` & `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/probabilities.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/cluster_auditd.py` & `msticpy-2.5.3/msticpy/analysis/cluster_auditd.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/code_cleanup.py` & `msticpy-2.5.3/msticpy/analysis/code_cleanup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/eventcluster.py` & `msticpy-2.5.3/msticpy/analysis/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/observationlist.py` & `msticpy-2.5.3/msticpy/analysis/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/outliers.py` & `msticpy-2.5.3/msticpy/analysis/outliers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/polling_detection.py` & `msticpy-2.5.3/msticpy/analysis/polling_detection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/syslog_utils.py` & `msticpy-2.5.3/msticpy/analysis/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/analysis/timeseries.py` & `msticpy-2.5.3/msticpy/analysis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/__init__.py` & `msticpy-2.5.3/msticpy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/azure_auth.py` & `msticpy-2.5.3/msticpy/auth/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/azure_auth_core.py` & `msticpy-2.5.3/msticpy/auth/azure_auth_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/cloud_mappings.py` & `msticpy-2.5.3/msticpy/auth/cloud_mappings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/cred_wrapper.py` & `msticpy-2.5.3/msticpy/auth/cred_wrapper.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/keyring_client.py` & `msticpy-2.5.3/msticpy/auth/keyring_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/keyvault_client.py` & `msticpy-2.5.3/msticpy/auth/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/keyvault_settings.py` & `msticpy-2.5.3/msticpy/auth/keyvault_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/msal_auth.py` & `msticpy-2.5.3/msticpy/auth/msal_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/auth/secret_settings.py` & `msticpy-2.5.3/msticpy/auth/secret_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/__init__.py` & `msticpy-2.5.3/msticpy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/azure_auth.py` & `msticpy-2.5.3/msticpy/common/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/check_version.py` & `msticpy-2.5.3/msticpy/common/check_version.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/data_types.py` & `msticpy-2.5.3/msticpy/common/data_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/data_utils.py` & `msticpy-2.5.3/msticpy/common/data_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/exceptions.py` & `msticpy-2.5.3/msticpy/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/pkg_config.py` & `msticpy-2.5.3/msticpy/common/pkg_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/provider_settings.py` & `msticpy-2.5.3/msticpy/common/provider_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/proxy_settings.py` & `msticpy-2.5.3/msticpy/common/proxy_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/settings.py` & `msticpy-2.5.3/msticpy/common/settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/timespan.py` & `msticpy-2.5.3/msticpy/common/timespan.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/utility/__init__.py` & `msticpy-2.5.3/msticpy/common/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/utility/format.py` & `msticpy-2.5.3/msticpy/common/utility/format.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/utility/ipython.py` & `msticpy-2.5.3/msticpy/common/utility/ipython.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/utility/package.py` & `msticpy-2.5.3/msticpy/common/utility/package.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/utility/types.py` & `msticpy-2.5.3/msticpy/common/utility/types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/common/wsconfig.py` & `msticpy-2.5.3/msticpy/common/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/__init__.py` & `msticpy-2.5.3/msticpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_azure.py` & `msticpy-2.5.3/msticpy/config/ce_azure.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_azure_sentinel.py` & `msticpy-2.5.3/msticpy/config/ce_azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_common.py` & `msticpy-2.5.3/msticpy/config/ce_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_data_providers.py` & `msticpy-2.5.3/msticpy/config/ce_data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_keyvault.py` & `msticpy-2.5.3/msticpy/config/ce_keyvault.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_msticpy.py` & `msticpy-2.5.3/msticpy/config/ce_msticpy.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_other_providers.py` & `msticpy-2.5.3/msticpy/config/ce_other_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_provider_base.py` & `msticpy-2.5.3/msticpy/config/ce_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_simple_settings.py` & `msticpy-2.5.3/msticpy/config/ce_simple_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_ti_providers.py` & `msticpy-2.5.3/msticpy/config/ce_ti_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/ce_user_defaults.py` & `msticpy-2.5.3/msticpy/config/ce_user_defaults.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/comp_edit.py` & `msticpy-2.5.3/msticpy/config/comp_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/compound_ctrls.py` & `msticpy-2.5.3/msticpy/config/compound_ctrls.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/file_browser.py` & `msticpy-2.5.3/msticpy/config/file_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/mp_config_control.py` & `msticpy-2.5.3/msticpy/config/mp_config_control.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/mp_config_edit.py` & `msticpy-2.5.3/msticpy/config/mp_config_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/config/mp_config_file.py` & `msticpy-2.5.3/msticpy/config/mp_config_file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/__init__.py` & `msticpy-2.5.3/msticpy/context/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/azure_data.py` & `msticpy-2.5.3/msticpy/context/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_analytics.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_analytics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_bookmarks.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_bookmarks.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_core.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_dynamic_summary.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_dynamic_summary_types.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_incidents.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_incidents.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_search.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_search.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_ti.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_ti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_utils.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_watchlists.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_watchlists.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/azure/sentinel_workspaces.py` & `msticpy-2.5.3/msticpy/context/azure/sentinel_workspaces.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/contextlookup.py` & `msticpy-2.5.3/msticpy/context/contextlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/contextproviders/context_provider_base.py` & `msticpy-2.5.3/msticpy/context/contextproviders/context_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/contextproviders/http_context_provider.py` & `msticpy-2.5.3/msticpy/context/contextproviders/http_context_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/contextproviders/servicenow.py` & `msticpy-2.5.3/msticpy/context/contextproviders/servicenow.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/domain_utils.py` & `msticpy-2.5.3/msticpy/context/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/geoip.py` & `msticpy-2.5.3/msticpy/context/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/http_provider.py` & `msticpy-2.5.3/msticpy/context/http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/ip_utils.py` & `msticpy-2.5.3/msticpy/context/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/lookup.py` & `msticpy-2.5.3/msticpy/context/lookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/lookup_result.py` & `msticpy-2.5.3/msticpy/context/lookup_result.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/preprocess_observable.py` & `msticpy-2.5.3/msticpy/context/preprocess_observable.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/provider_base.py` & `msticpy-2.5.3/msticpy/context/provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tilookup.py` & `msticpy-2.5.3/msticpy/context/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/__init__.py` & `msticpy-2.5.3/msticpy/context/tiproviders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/alienvault_otx.py` & `msticpy-2.5.3/msticpy/context/tiproviders/alienvault_otx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/azure_sent_byoti.py` & `msticpy-2.5.3/msticpy/context/tiproviders/azure_sent_byoti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/greynoise.py` & `msticpy-2.5.3/msticpy/context/tiproviders/greynoise.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/ibm_xforce.py` & `msticpy-2.5.3/msticpy/context/tiproviders/ibm_xforce.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/intsights.py` & `msticpy-2.5.3/msticpy/context/tiproviders/intsights.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/kql_base.py` & `msticpy-2.5.3/msticpy/context/tiproviders/kql_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/mblookup.py` & `msticpy-2.5.3/msticpy/context/tiproviders/mblookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/open_page_rank.py` & `msticpy-2.5.3/msticpy/context/tiproviders/open_page_rank.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/pulsedive.py` & `msticpy-2.5.3/msticpy/context/tiproviders/pulsedive.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/result_severity.py` & `msticpy-2.5.3/msticpy/context/tiproviders/result_severity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/riskiq.py` & `msticpy-2.5.3/msticpy/context/tiproviders/riskiq.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/ti_http_provider.py` & `msticpy-2.5.3/msticpy/context/tiproviders/ti_http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/ti_provider_base.py` & `msticpy-2.5.3/msticpy/context/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/tor_exit_nodes.py` & `msticpy-2.5.3/msticpy/context/tiproviders/tor_exit_nodes.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/tiproviders/virustotal.py` & `msticpy-2.5.3/msticpy/context/tiproviders/virustotal.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/vtlookupv3/__init__.py` & `msticpy-2.5.3/msticpy/context/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/vtlookupv3/vtfile_behavior.py` & `msticpy-2.5.3/msticpy/context/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/vtlookupv3/vtlookup.py` & `msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/context/vtlookupv3/vtlookupv3.py` & `msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/__init__.py` & `msticpy-2.5.3/msticpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/azure/__init__.py` & `msticpy-2.5.3/msticpy/data/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/azure/azure_blob_storage.py` & `msticpy-2.5.3/msticpy/data/azure/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/azure/azure_data.py` & `msticpy-2.5.3/msticpy/data/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/azure_blob_storage.py` & `msticpy-2.5.3/msticpy/data/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/azure_data.py` & `msticpy-2.5.3/msticpy/data/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/azure_sentinel.py` & `msticpy-2.5.3/msticpy/data/azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/data_providers.py` & `msticpy-2.5.3/msticpy/data/core/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/data_query_reader.py` & `msticpy-2.5.3/msticpy/data/core/data_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/param_extractor.py` & `msticpy-2.5.3/msticpy/data/core/param_extractor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_container.py` & `msticpy-2.5.3/msticpy/data/core/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_defns.py` & `msticpy-2.5.3/msticpy/data/core/query_defns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_provider_connections_mixin.py` & `msticpy-2.5.3/msticpy/data/core/query_provider_connections_mixin.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_provider_utils_mixin.py` & `msticpy-2.5.3/msticpy/data/core/query_provider_utils_mixin.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_source.py` & `msticpy-2.5.3/msticpy/data/core/query_source.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_store.py` & `msticpy-2.5.3/msticpy/data/core/query_store.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/core/query_template.py` & `msticpy-2.5.3/msticpy/data/core/query_template.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/data_obfus.py` & `msticpy-2.5.3/msticpy/data/data_obfus.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/data_providers.py` & `msticpy-2.5.3/msticpy/data/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/__init__.py` & `msticpy-2.5.3/msticpy/data/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/azure_kusto_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/azure_kusto_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/azure_monitor_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/azure_monitor_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from datetime import datetime
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, cast
 
 import httpx
 import pandas as pd
 from azure.core.exceptions import HttpResponseError
 from azure.core.pipeline.policies import UserAgentPolicy
+from pkg_resources import parse_version
 
 from ..._version import VERSION
 from ...auth.azure_auth import AzureCloudConfig, az_connect
 from ...common.exceptions import (
     MsticpyDataQueryError,
     MsticpyKqlConnectionError,
     MsticpyMissingDependencyError,
@@ -37,20 +38,22 @@
 from ...common.utility import export, mp_ua_header
 from ...common.wsconfig import WorkspaceConfig
 from ..core.query_defns import DataEnvironment
 from .driver_base import DriverBase, DriverProps, QuerySource
 
 logger = logging.getLogger(__name__)
 
+# pylint: disable=ungrouped-imports
 try:
     from azure.monitor.query import (
         LogsQueryClient,
         LogsQueryPartialResult,
         LogsQueryResult,
     )
+    from azure.monitor.query import __version__ as az_monitor_version
 except ImportError as imp_err:
     raise MsticpyMissingDependencyError(
         "Cannot use this feature without Azure monitor client installed",
         title="Error importing azure.monitor.query",
         packages="azure-monitor-query",
     ) from imp_err
 
@@ -145,17 +148,21 @@
             connection_str,
             kwargs,
         )
 
     @property
     def url_endpoint(self) -> str:
         """Return the current URL endpoint for Azure Monitor."""
-        return _LOGANALYTICS_URL_BY_CLOUD.get(
+        base_url = _LOGANALYTICS_URL_BY_CLOUD.get(
             AzureCloudConfig().cloud, _LOGANALYTICS_URL_BY_CLOUD["global"]
         )
+        # post v1.1.0 of azure-monitor-query, the API version requires a 'v1' suffix
+        if parse_version(az_monitor_version) > parse_version("1.1.0"):
+            return f"{base_url}v1"
+        return base_url
 
     def connect(self, connection_str: Optional[str] = None, **kwargs):
         """
         Connect to data source.
 
         Parameters
         ----------
```

### Comparing `msticpy-2.5.2/msticpy/data/drivers/cybereason_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/cybereason_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/driver_base.py` & `msticpy-2.5.3/msticpy/data/drivers/driver_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/elastic_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/elastic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/kql_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/kql_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         debug : bool
             print out additional diagnostic information.
 
         """
         self._ip = get_ipython()
         self._debug = kwargs.get("debug", False)
         super().__init__(**kwargs)
-
+        self.workspace_id: Optional[str] = None
         self.set_driver_property(
             DriverProps.FORMATTERS,
             {"datetime": self._format_datetime, "list": self._format_list},
         )
         self._loaded = self._is_kqlmagic_loaded()
 
         os.environ["KQLMAGIC_LOAD_MODE"] = "silent"
@@ -433,14 +433,16 @@
         os.environ[_KQL_ENV_OPTS] = kql_config
 
     @staticmethod
     def _get_kql_current_connection():
         """Get the current connection Workspace ID from KQLMagic."""
         connections = kql_exec("--conn")
         current_connection = [conn for conn in connections if conn.startswith(" * ")]
+        if not current_connection:
+            return ""
         return current_connection[0].strip(" * ").split("@")[0]
 
     def _set_kql_cloud(self):
         """If cloud is set in Azure Settings override default."""
         # Check that there isn't a cloud setting in the KQLMAGIC env var
         kql_config = os.environ.get(_KQL_ENV_OPTS, "")
         if "cloud" in kql_config:
```

### Comparing `msticpy-2.5.2/msticpy/data/drivers/kusto_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/kusto_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/local_data_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/local_data_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/local_osquery_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/local_osquery_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/mdatp_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/mdatp_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/mordor_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/mordor_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/odata_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/odata_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/resource_graph_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/resource_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/security_graph_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/security_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/sentinel_query_reader.py` & `msticpy-2.5.3/msticpy/data/drivers/sentinel_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/splunk_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/splunk_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/drivers/sumologic_driver.py` & `msticpy-2.5.3/msticpy/data/drivers/sumologic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/cybereason/cybereason_connections.yaml` & `msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_connections.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/cybereason/cybereason_hosts.yaml` & `msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_hosts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/cybereason/cybereason_processes.yaml` & `msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_processes.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/localdata/local_data.yaml` & `msticpy-2.5.3/msticpy/data/queries/localdata/local_data.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml` & `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_file.yaml` & `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_file.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml` & `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_network.yaml` & `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_process.yaml` & `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/m365d/kql_mdatp_user.yaml` & `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_alerts.yaml` & `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_file.yaml` & `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_file.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_hunting.yaml` & `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_hunting.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_network.yaml` & `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_process.yaml` & `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mde/kql_mdatp_user.yaml` & `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/msgraph/graph_alerts.yaml` & `msticpy-2.5.3/msticpy/data/queries/msgraph/graph_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_alert.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_alert.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_azure.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azure.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_net.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_net.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_o365.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_o365.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml` & `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml` & `msticpy-2.5.3/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/resourcegraph/sentinel_resources.yaml` & `msticpy-2.5.3/msticpy/data/queries/resourcegraph/sentinel_resources.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/splunk/splunk_alert_queries.yaml` & `msticpy-2.5.3/msticpy/data/queries/splunk/splunk_alert_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/splunk/splunk_authentication_queries.yaml` & `msticpy-2.5.3/msticpy/data/queries/splunk/splunk_authentication_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/splunk/splunk_queries.yaml` & `msticpy-2.5.3/msticpy/data/queries/splunk/splunk_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/queries/sumologic/sumologic_queries.yaml` & `msticpy-2.5.3/msticpy/data/queries/sumologic/sumologic_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/query_container.py` & `msticpy-2.5.3/msticpy/data/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/query_defns.py` & `msticpy-2.5.3/msticpy/data/query_defns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/sql_to_kql.py` & `msticpy-2.5.3/msticpy/data/sql_to_kql.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/storage/azure_blob_storage.py` & `msticpy-2.5.3/msticpy/data/storage/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/uploaders/__init__.py` & `msticpy-2.5.3/msticpy/data/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/uploaders/loganalytics_uploader.py` & `msticpy-2.5.3/msticpy/data/uploaders/loganalytics_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/uploaders/splunk_uploader.py` & `msticpy-2.5.3/msticpy/data/uploaders/splunk_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/data/uploaders/uploader_base.py` & `msticpy-2.5.3/msticpy/data/uploaders/uploader_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/__init__.py` & `msticpy-2.5.3/msticpy/datamodel/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/account.py` & `msticpy-2.5.3/msticpy/datamodel/entities/account.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/alert.py` & `msticpy-2.5.3/msticpy/datamodel/entities/alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/azure_resource.py` & `msticpy-2.5.3/msticpy/datamodel/entities/azure_resource.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/cloud_application.py` & `msticpy-2.5.3/msticpy/datamodel/entities/cloud_application.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/cloud_logon_session.py` & `msticpy-2.5.3/msticpy/datamodel/entities/cloud_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/dns.py` & `msticpy-2.5.3/msticpy/datamodel/entities/dns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/entity.py` & `msticpy-2.5.3/msticpy/datamodel/entities/entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/entity_enums.py` & `msticpy-2.5.3/msticpy/datamodel/entities/entity_enums.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/entity_graph.py` & `msticpy-2.5.3/msticpy/datamodel/entities/entity_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/file.py` & `msticpy-2.5.3/msticpy/datamodel/entities/file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/file_hash.py` & `msticpy-2.5.3/msticpy/datamodel/entities/file_hash.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/geo_location.py` & `msticpy-2.5.3/msticpy/datamodel/entities/geo_location.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/graph_property.py` & `msticpy-2.5.3/msticpy/datamodel/entities/graph_property.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/host.py` & `msticpy-2.5.3/msticpy/datamodel/entities/host.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/host_logon_session.py` & `msticpy-2.5.3/msticpy/datamodel/entities/host_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/iot_device.py` & `msticpy-2.5.3/msticpy/datamodel/entities/iot_device.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/ip_address.py` & `msticpy-2.5.3/msticpy/datamodel/entities/ip_address.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/mail_cluster.py` & `msticpy-2.5.3/msticpy/datamodel/entities/mail_cluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/mail_message.py` & `msticpy-2.5.3/msticpy/datamodel/entities/mail_message.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/mailbox.py` & `msticpy-2.5.3/msticpy/datamodel/entities/mailbox.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/malware.py` & `msticpy-2.5.3/msticpy/datamodel/entities/malware.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/network_connection.py` & `msticpy-2.5.3/msticpy/datamodel/entities/network_connection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/process.py` & `msticpy-2.5.3/msticpy/datamodel/entities/process.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/registry_key.py` & `msticpy-2.5.3/msticpy/datamodel/entities/registry_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/registry_value.py` & `msticpy-2.5.3/msticpy/datamodel/entities/registry_value.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/security_group.py` & `msticpy-2.5.3/msticpy/datamodel/entities/security_group.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/submission_mail.py` & `msticpy-2.5.3/msticpy/datamodel/entities/submission_mail.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/threat_intelligence.py` & `msticpy-2.5.3/msticpy/datamodel/entities/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/unknown_entity.py` & `msticpy-2.5.3/msticpy/datamodel/entities/unknown_entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/entities/url.py` & `msticpy-2.5.3/msticpy/datamodel/entities/url.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/pivot.py` & `msticpy-2.5.3/msticpy/datamodel/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/soc/incident.py` & `msticpy-2.5.3/msticpy/datamodel/soc/incident.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/datamodel/soc/sentinel_alert.py` & `msticpy-2.5.3/msticpy/datamodel/soc/sentinel_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/__init__.py` & `msticpy-2.5.3/msticpy/init/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/azure_ml_tools.py` & `msticpy-2.5.3/msticpy/init/azure_ml_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/azure_synapse_tools.py` & `msticpy-2.5.3/msticpy/init/azure_synapse_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/logging.py` & `msticpy-2.5.3/msticpy/init/logging.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/mp_pandas_accessors.py` & `msticpy-2.5.3/msticpy/init/mp_pandas_accessors.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/mp_plugins.py` & `msticpy-2.5.3/msticpy/init/mp_plugins.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/nbinit.py` & `msticpy-2.5.3/msticpy/init/nbinit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/nbmagics.py` & `msticpy-2.5.3/msticpy/init/nbmagics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot.py` & `msticpy-2.5.3/msticpy/init/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_browser.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_container.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_magic_core.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_magic_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_pd_accessor.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_pipeline.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_pipeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_register.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_register.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_core/pivot_register_reader.py` & `msticpy-2.5.3/msticpy/init/pivot_core/pivot_register_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_init/pivot_data_queries.py` & `msticpy-2.5.3/msticpy/init/pivot_init/pivot_data_queries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_init/pivot_ti_provider.py` & `msticpy-2.5.3/msticpy/init/pivot_init/pivot_ti_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/pivot_init/vt_pivot.py` & `msticpy-2.5.3/msticpy/init/pivot_init/vt_pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/init/user_config.py` & `msticpy-2.5.3/msticpy/init/user_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/__init__.py` & `msticpy-2.5.3/msticpy/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/data_viewer.py` & `msticpy-2.5.3/msticpy/nbtools/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/entityschema.py` & `msticpy-2.5.3/msticpy/nbtools/entityschema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/foliummap.py` & `msticpy-2.5.3/msticpy/nbtools/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/morph_charts.py` & `msticpy-2.5.3/msticpy/nbtools/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/nbdisplay.py` & `msticpy-2.5.3/msticpy/nbtools/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/nbwidgets.py` & `msticpy-2.5.3/msticpy/nbtools/nbwidgets.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/observationlist.py` & `msticpy-2.5.3/msticpy/nbtools/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/process_tree.py` & `msticpy-2.5.3/msticpy/nbtools/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/security_alert.py` & `msticpy-2.5.3/msticpy/nbtools/security_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/security_alert_graph.py` & `msticpy-2.5.3/msticpy/nbtools/security_alert_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/security_base.py` & `msticpy-2.5.3/msticpy/nbtools/security_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/security_event.py` & `msticpy-2.5.3/msticpy/nbtools/security_event.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/ti_browser.py` & `msticpy-2.5.3/msticpy/nbtools/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/timeline.py` & `msticpy-2.5.3/msticpy/nbtools/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/timeline_duration.py` & `msticpy-2.5.3/msticpy/nbtools/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/timeline_pd_accessor.py` & `msticpy-2.5.3/msticpy/nbtools/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/timeseries.py` & `msticpy-2.5.3/msticpy/nbtools/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/utility.py` & `msticpy-2.5.3/msticpy/nbtools/utility.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbtools/wsconfig.py` & `msticpy-2.5.3/msticpy/nbtools/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/__init__.py` & `msticpy-2.5.3/msticpy/nbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/core.py` & `msticpy-2.5.3/msticpy/nbwidgets/core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/get_environment_key.py` & `msticpy-2.5.3/msticpy/nbwidgets/get_environment_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/get_text.py` & `msticpy-2.5.3/msticpy/nbwidgets/get_text.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/lookback.py` & `msticpy-2.5.3/msticpy/nbwidgets/lookback.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/option_buttons.py` & `msticpy-2.5.3/msticpy/nbwidgets/option_buttons.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/progress.py` & `msticpy-2.5.3/msticpy/nbwidgets/progress.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/query_time.py` & `msticpy-2.5.3/msticpy/nbwidgets/query_time.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/select_alert.py` & `msticpy-2.5.3/msticpy/nbwidgets/select_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/select_item.py` & `msticpy-2.5.3/msticpy/nbwidgets/select_item.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/nbwidgets/select_subset.py` & `msticpy-2.5.3/msticpy/nbwidgets/select_subset.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/resources/WinSecurityEvent.json` & `msticpy-2.5.3/msticpy/resources/WinSecurityEvent.json`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/resources/mp_pivot_reg.yaml` & `msticpy-2.5.3/msticpy/resources/mp_pivot_reg.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/resources/mpconfig_defaults.yaml` & `msticpy-2.5.3/msticpy/resources/mpconfig_defaults.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/resources/obfuscation_cols.yaml` & `msticpy-2.5.3/msticpy/resources/obfuscation_cols.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/__init__.py` & `msticpy-2.5.3/msticpy/sectools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/auditdextract.py` & `msticpy-2.5.3/msticpy/sectools/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/base64unpack.py` & `msticpy-2.5.3/msticpy/sectools/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/cmd_line.py` & `msticpy-2.5.3/msticpy/sectools/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/domain_utils.py` & `msticpy-2.5.3/msticpy/sectools/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/eventcluster.py` & `msticpy-2.5.3/msticpy/sectools/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/geoip.py` & `msticpy-2.5.3/msticpy/sectools/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/iocextract.py` & `msticpy-2.5.3/msticpy/sectools/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/ip_utils.py` & `msticpy-2.5.3/msticpy/sectools/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/proc_tree_build_mde.py` & `msticpy-2.5.3/msticpy/sectools/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/proc_tree_build_winlx.py` & `msticpy-2.5.3/msticpy/sectools/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/proc_tree_builder.py` & `msticpy-2.5.3/msticpy/sectools/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/proc_tree_schema.py` & `msticpy-2.5.3/msticpy/sectools/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/proc_tree_utils.py` & `msticpy-2.5.3/msticpy/sectools/proc_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/sectools_magics.py` & `msticpy-2.5.3/msticpy/sectools/sectools_magics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/syslog_utils.py` & `msticpy-2.5.3/msticpy/sectools/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/tilookup.py` & `msticpy-2.5.3/msticpy/sectools/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/tiproviders/ti_provider_base.py` & `msticpy-2.5.3/msticpy/sectools/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/vtlookup.py` & `msticpy-2.5.3/msticpy/sectools/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/vtlookupv3/__init__.py` & `msticpy-2.5.3/msticpy/sectools/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/vtlookupv3/vtfile_behavior.py` & `msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/vtlookupv3/vtlookupv3.py` & `msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/sectools/vtlookupv3/vtobject_browser.py` & `msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/auditdextract.py` & `msticpy-2.5.3/msticpy/transform/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/base64unpack.py` & `msticpy-2.5.3/msticpy/transform/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/cmd_line.py` & `msticpy-2.5.3/msticpy/transform/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/iocextract.py` & `msticpy-2.5.3/msticpy/transform/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/network.py` & `msticpy-2.5.3/msticpy/transform/network.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/proc_tree_build_mde.py` & `msticpy-2.5.3/msticpy/transform/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/proc_tree_build_winlx.py` & `msticpy-2.5.3/msticpy/transform/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/proc_tree_builder.py` & `msticpy-2.5.3/msticpy/transform/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/proc_tree_schema.py` & `msticpy-2.5.3/msticpy/transform/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/transform/process_tree_utils.py` & `msticpy-2.5.3/msticpy/transform/process_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/__init__.py` & `msticpy-2.5.3/msticpy/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/code_view.py` & `msticpy-2.5.3/msticpy/vis/code_view.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/data_viewer.py` & `msticpy-2.5.3/msticpy/vis/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/data_viewer_panel.py` & `msticpy-2.5.3/msticpy/vis/data_viewer_panel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/entity_graph_tools.py` & `msticpy-2.5.3/msticpy/vis/entity_graph_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/figure_dimension.py` & `msticpy-2.5.3/msticpy/vis/figure_dimension.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/foliummap.py` & `msticpy-2.5.3/msticpy/vis/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/matrix_plot.py` & `msticpy-2.5.3/msticpy/vis/matrix_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/mordor_browser.py` & `msticpy-2.5.3/msticpy/vis/mordor_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/morph_charts.py` & `msticpy-2.5.3/msticpy/vis/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/mp_pandas_plot.py` & `msticpy-2.5.3/msticpy/vis/mp_pandas_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/nbdisplay.py` & `msticpy-2.5.3/msticpy/vis/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/network_plot.py` & `msticpy-2.5.3/msticpy/vis/network_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/process_tree.py` & `msticpy-2.5.3/msticpy/vis/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/query_browser.py` & `msticpy-2.5.3/msticpy/vis/query_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/ti_browser.py` & `msticpy-2.5.3/msticpy/vis/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/timeline.py` & `msticpy-2.5.3/msticpy/vis/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/timeline_common.py` & `msticpy-2.5.3/msticpy/vis/timeline_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/timeline_duration.py` & `msticpy-2.5.3/msticpy/vis/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/timeline_pd_accessor.py` & `msticpy-2.5.3/msticpy/vis/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/timeline_values.py` & `msticpy-2.5.3/msticpy/vis/timeline_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/timeseries.py` & `msticpy-2.5.3/msticpy/vis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy/vis/vtobject_browser.py` & `msticpy-2.5.3/msticpy/vis/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy.egg-info/PKG-INFO` & `msticpy-2.5.3/msticpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.5.2
+Version: 2.5.3
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
```

### Comparing `msticpy-2.5.2/msticpy.egg-info/SOURCES.txt` & `msticpy-2.5.3/msticpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/msticpy.egg-info/requires.txt` & `msticpy-2.5.3/msticpy.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython<3.0.0,>=2.0.0
 folium>=0.9.0
 geoip2>=2.9.0
 httpx==0.24.0
 html5lib
-ipywidgets<8.0.0,>=7.4.2
+ipywidgets<9.0.0,>=7.4.2
 KqlmagicCustom[auth_code_clipboard,jupyter-basic]>=0.1.114.post22
 lxml>=4.6.5
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
```

### Comparing `msticpy-2.5.2/requirements-all.txt` & `msticpy-2.5.3/requirements-all.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
 httpx==0.24.0
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
-ipywidgets>=7.4.2, <8.0.0
+ipywidgets>=7.4.2, <9.0.0
 keyring>=13.2.1
 KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 lxml>=4.6.5
 matplotlib>=3.0.0
 mo-sql-parsing>=8, <9.0.0
 msal>=1.12.0
```

### Comparing `msticpy-2.5.2/requirements-dev.txt` & `msticpy-2.5.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/requirements.txt` & `msticpy-2.5.3/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
 httpx==0.24.0
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
-ipywidgets>=7.4.2, <8.0.0
+ipywidgets>=7.4.2, <9.0.0
 KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 lxml>=4.6.5
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
```

### Comparing `msticpy-2.5.2/setup.cfg` & `msticpy-2.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.2/setup.py` & `msticpy-2.5.3/setup.py`

 * *Files identical despite different names*

